# Comparing `tmp/housekeeper-4.3.0.tar.gz` & `tmp/housekeeper-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/housekeeper-4.3.0.tar", last modified: Thu May 11 10:16:42 2023, max compression
+gzip compressed data, was "dist/housekeeper-4.4.0.tar", last modified: Tue May 16 11:18:43 2023, max compression
```

## Comparing `housekeeper-4.3.0.tar` & `housekeeper-4.4.0.tar`

### file list

```diff
@@ -1,105 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-11 10:16:30.000000 housekeeper-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-11 10:16:30.000000 housekeeper-4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-11 10:16:42.000000 housekeeper-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-11 10:16:30.000000 housekeeper-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/handlers/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-11 10:16:30.000000 housekeeper-4.3.0/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-11 10:16:42.000000 housekeeper-4.3.0/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 10:16:41.000000 housekeeper-4.3.0/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 10:16:30.000000 housekeeper-4.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 10:16:30.000000 housekeeper-4.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 10:16:42.000000 housekeeper-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-11 10:16:30.000000 housekeeper-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/fixtures/sequencing_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/sequencing_files/lane1.spring
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/sequencing_files/lane2.spring
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_file_join_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/filters/test_version_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:16:42.000000 housekeeper-4.3.0/tests/store/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/handlers/test_createhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/handlers/test_readhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/store/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-11 10:16:30.000000 housekeeper-4.3.0/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-16 11:18:33.000000 housekeeper-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-16 11:18:33.000000 housekeeper-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-16 11:18:43.000000 housekeeper-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-16 11:18:33.000000 housekeeper-4.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/handlers/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-16 11:18:33.000000 housekeeper-4.4.0/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 11:18:43.000000 housekeeper-4.4.0/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 11:18:33.000000 housekeeper-4.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 11:18:33.000000 housekeeper-4.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 11:18:43.000000 housekeeper-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-16 11:18:33.000000 housekeeper-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/fixtures/sequencing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/sequencing_files/lane1.spring
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/sequencing_files/lane2.spring
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_archive_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/filters/test_version_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:18:43.000000 housekeeper-4.4.0/tests/store/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/handlers/test_createhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/handlers/test_readhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/handlers/test_updatehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/store/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-16 11:18:33.000000 housekeeper-4.4.0/tests/test_include.py
```

### Comparing `housekeeper-4.3.0/LICENSE` & `housekeeper-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/PKG-INFO` & `housekeeper-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.3.0
+Version: 4.4.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.3.0/README.md` & `housekeeper-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/add.py` & `housekeeper-4.4.0/housekeeper/cli/add.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/core.py` & `housekeeper-4.4.0/housekeeper/cli/core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/delete.py` & `housekeeper-4.4.0/housekeeper/cli/delete.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/get.py` & `housekeeper-4.4.0/housekeeper/cli/get.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/include.py` & `housekeeper-4.4.0/housekeeper/cli/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/init.py` & `housekeeper-4.4.0/housekeeper/cli/init.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/cli/tables.py` & `housekeeper-4.4.0/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/date.py` & `housekeeper-4.4.0/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/files.py` & `housekeeper-4.4.0/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/include.py` & `housekeeper-4.4.0/housekeeper/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/api/core.py` & `housekeeper-4.4.0/housekeeper/store/api/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 import logging
 from pathlib import Path
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker, scoped_session
 
+from housekeeper.store.api.handlers.update import UpdateHandler
 from housekeeper.store.models import Model
 from housekeeper.store.api.handlers.create import CreateHandler
 from housekeeper.store.api.handlers.read import ReadHandler
 
 LOG = logging.getLogger(__name__)
 
 
-class CoreHandler(ReadHandler, CreateHandler):
+class CoreHandler(CreateHandler, ReadHandler, UpdateHandler):
     """Aggregating class for the store api handlers"""
 
     def __init__(self, session):
         ReadHandler(session=session)
         CreateHandler(session=session)
+        UpdateHandler(session=session)
 
 
 class Store(CoreHandler):
 
     """
     Handles interactions with the database in the context when a temporary
     database connection is needed, e.g. a command line interface.
```

### Comparing `housekeeper-4.3.0/housekeeper/store/api/handlers/base.py` & `housekeeper-4.4.0/housekeeper/store/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/api/handlers/create.py` & `housekeeper-4.4.0/housekeeper/store/api/handlers/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,38 +53,32 @@
 
         version_obj.bundle = bundle_obj
         return bundle_obj, version_obj
 
     def _add_files_to_version(self, files: List[dict], version_obj: Version) -> None:
         """Create file objects and the tags and add them to a version object"""
 
-        tag_names = set(
-            tag_name for file_data in files for tag_name in file_data["tags"]
-        )
+        tag_names = set(tag_name for file_data in files for tag_name in file_data["tags"])
         tag_map = self._build_tags(tag_names)
 
         for file_data in files:
             # This if can be removed after decoupling
             if isinstance(file_data["path"], str):
                 paths = [file_data["path"]]
             else:
                 paths = file_data["path"]
             for path in paths:
                 LOG.debug("adding file: %s", path)
                 if not Path(path).exists():
                     raise FileNotFoundError(path)
                 tags = [tag_map[tag_name] for tag_name in file_data["tags"]]
-                new_file = self.new_file(
-                    path, to_archive=file_data["archive"], tags=tags
-                )
+                new_file = self.new_file(path, to_archive=file_data["archive"], tags=tags)
                 version_obj.files.append(new_file)
 
-    def new_version(
-        self, created_at: dt.datetime, expires_at: dt.datetime = None
-    ) -> Version:
+    def new_version(self, created_at: dt.datetime, expires_at: dt.datetime = None) -> Version:
         """Create a new bundle version."""
         LOG.info("Created new version")
         new_version = self.Version(created_at=created_at, expires_at=expires_at)
         return new_version
 
     def add_version(
         self,
@@ -157,8 +151,7 @@
         """Create a new tag object based on the information given."""
         new_tag = self.Tag(name=name, category=category)
         return new_tag
 
     def create_archive(self, file_id: int, archiving_task_id: int) -> Archive:
         """Creates an archive object to the given file, with the given archive task id."""
         return Archive(file_id=file_id, archiving_task_id=archiving_task_id)
-
```

### Comparing `housekeeper-4.3.0/housekeeper/store/api/handlers/read.py` & `housekeeper-4.4.0/housekeeper/store/api/handlers/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
 This module handles finding things in the store/database
 """
 import datetime as dt
 import logging
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Set
 from sqlalchemy.orm import Query, Session
 
 from housekeeper.store.filters.bundle_filters import BundleFilters, apply_bundle_filter
-from housekeeper.store.filters.file_filters import FileFilter, apply_file_filter
 from housekeeper.store.filters.file_filters import (
     FileFilter,
     apply_file_filter,
 )
 from housekeeper.store.filters.version_bundle_filters import (
     VersionBundleFilters,
     apply_version_bundle_filter,
 )
 from housekeeper.store.filters.version_filters import (
     VersionFilter,
     apply_version_filter,
 )
-from housekeeper.store.models import Bundle, File, Tag, Version
+from housekeeper.store.models import Bundle, File, Tag, Version, Archive
 from housekeeper.store.filters.tag_filters import TagFilter, apply_tag_filter
 
-from .base import BaseHandler
-
+from housekeeper.store.api.handlers.base import BaseHandler
+from housekeeper.store.filters.archive_filters import (
+    apply_archive_filter,
+    ArchiveFilter,
+)
 
 LOG = logging.getLogger(__name__)
 
 
 class ReadHandler(BaseHandler):
     """Handler for searching the database"""
 
@@ -208,7 +210,29 @@
             filter_functions=[
                 FileFilter.FILTER_FILES_BY_TAGS,
                 FileFilter.FILTER_FILES_BY_IS_ARCHIVED,
             ],
             is_archived=False,
             tag_names=tags,
         ).all()
+
+    def get_ongoing_archiving_tasks(self) -> Set[int]:
+        """Returns all archiving tasks in the archive table, for entries where the archiving
+        field is empty."""
+        return {
+            archive.archiving_task_id
+            for archive in apply_archive_filter(
+                archives=self._get_query(table=Archive),
+                filter_functions=[ArchiveFilter.FILTER_ARCHIVING_ONGOING],
+            ).all()
+        }
+
+    def get_ongoing_retrieval_tasks(self) -> Set[int]:
+        """Returns all retrieval tasks in the archive table, for entries where the retrieved_at
+        field is empty."""
+        return {
+            archive.retrieval_task_id
+            for archive in apply_archive_filter(
+                archives=self._get_query(table=Archive),
+                filter_functions=[ArchiveFilter.FILTER_RETRIEVAL_ONGOING],
+            ).all()
+        }
```

### Comparing `housekeeper-4.3.0/housekeeper/store/api/schema.py` & `housekeeper-4.4.0/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.4.0/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/filters/file_filters.py` & `housekeeper-4.4.0/housekeeper/store/filters/file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/filters/tag_filters.py` & `housekeeper-4.4.0/housekeeper/store/filters/tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.4.0/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/filters/version_filters.py` & `housekeeper-4.4.0/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper/store/models.py` & `housekeeper-4.4.0/housekeeper/store/models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/housekeeper.egg-info/PKG-INFO` & `housekeeper-4.4.0/housekeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.3.0
+Version: 4.4.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.3.0/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.4.0/housekeeper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 housekeeper/store/api/__init__.py
 housekeeper/store/api/core.py
 housekeeper/store/api/schema.py
 housekeeper/store/api/handlers/__init__.py
 housekeeper/store/api/handlers/base.py
 housekeeper/store/api/handlers/create.py
 housekeeper/store/api/handlers/read.py
+housekeeper/store/api/handlers/update.py
 housekeeper/store/filters/__init__.py
+housekeeper/store/filters/archive_filters.py
 housekeeper/store/filters/bundle_filters.py
 housekeeper/store/filters/file_filters.py
 housekeeper/store/filters/tag_filters.py
 housekeeper/store/filters/version_bundle_filters.py
 housekeeper/store/filters/version_filters.py
 tests/__init__.py
 tests/conftest.py
@@ -70,15 +72,16 @@
 tests/fixtures/vcfs/example.2.vcf
 tests/fixtures/vcfs/example.vcf
 tests/fixtures/vcfs/family.2.vcf
 tests/fixtures/vcfs/family.3.vcf
 tests/fixtures/vcfs/family.vcf
 tests/store/conftest.py
 tests/store/test_models.py
+tests/store/filters/test_archive_filters.py
 tests/store/filters/test_bundle_filters.py
 tests/store/filters/test_file_filters.py
-tests/store/filters/test_file_join_filters.py
 tests/store/filters/test_tag_filters.py
 tests/store/filters/test_version_bundle_filters.py
 tests/store/filters/test_version_filters.py
 tests/store/handlers/test_createhandler.py
-tests/store/handlers/test_readhandler.py
+tests/store/handlers/test_readhandler.py
+tests/store/handlers/test_updatehandler.py
```

### Comparing `housekeeper-4.3.0/setup.py` & `housekeeper-4.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.3.0",
+    version="4.4.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.3.0/tests/cli/add/conftest.py` & `housekeeper-4.4.0/tests/cli/add/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.4.0/tests/cli/add/test_cli_add_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.4.0/tests/cli/add/test_cli_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.4.0/tests/cli/add/test_cli_add_tags.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.4.0/tests/cli/add/test_cli_add_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/conftest.py` & `housekeeper-4.4.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.4.0/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/get/test_get_bundle.py` & `housekeeper-4.4.0/tests/cli/get/test_get_bundle.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/get/test_get_files.py` & `housekeeper-4.4.0/tests/cli/get/test_get_files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/get/test_get_tag.py` & `housekeeper-4.4.0/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/get/test_get_version.py` & `housekeeper-4.4.0/tests/cli/get/test_get_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/test_cli_core.py` & `housekeeper-4.4.0/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/cli/test_cli_include.py` & `housekeeper-4.4.0/tests/cli/test_cli_include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/conftest.py` & `housekeeper-4.4.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
 
 @pytest.fixture(scope="function", name="archiving_task_id")
 def fixture_archiving_task_id() -> int:
     """Return an id of an archiving task."""
     return 1234
 
+
 @pytest.fixture(scope="function", name="retrieval_task_id")
 def fixture_retrieval_task_id() -> int:
     """Return an id of a retrieval task."""
     return 4321
 
 
 @pytest.fixture(scope="function", name="case_id")
@@ -106,26 +107,22 @@
 @pytest.fixture(scope="function", name="sample2_data")
 def fixture_sample2_data(sample_tag_names: List[str], second_sample_vcf: Path) -> dict:
     """Return file and tags for sample."""
     return {"tags": sample_tag_names, "file": second_sample_vcf}
 
 
 @pytest.fixture(scope="function", name="spring_file_1_with_tags")
-def fixture_spring_file_1_with_tags(
-    sample_id: str, spring_tag: str, spring_file_1: Path
-) -> dict:
+def fixture_spring_file_1_with_tags(sample_id: str, spring_tag: str, spring_file_1: Path) -> dict:
     """Return spring file and tags for a sample."""
     return {"tags": [sample_id, spring_tag], "file": spring_file_1}
 
 
 @pytest.fixture(scope="function", name="spring_file_2_with_tags")
-def fixture_spring_file_2_with_tags(
-    sample_id: str, spring_tag: str, spring_file_2: Path
-) -> dict:
-    """Return a second spring file and tags for a sample."""
+def fixture_spring_file_2_with_tags(sample_id: str, spring_tag: str, spring_file_2: Path) -> dict:
+    """Return a second SPRING file and tags for a sample."""
     return {"tags": [sample_id, spring_tag], "file": spring_file_2}
 
 
 @pytest.fixture(scope="function", name="family_data")
 def fixture_family_data(family_tag_names: List[str], family_vcf: Path) -> dict:
     """Return file and tags for sample."""
     return {"tags": family_tag_names, "file": family_vcf}
@@ -190,26 +187,22 @@
         case_id=sample_id,
         files=[spring_file_1_with_tags, spring_file_2_with_tags],
         created_at=timestamp,
     )
 
 
 @pytest.fixture(scope="function", name="empty_version_data")
-def fixture_empty_version_data(
-    later_timestamp: datetime.datetime, case_id: str
-) -> dict:
+def fixture_empty_version_data(later_timestamp: datetime.datetime, case_id: str) -> dict:
     """Return a dummy bundle."""
     data = {"bundle_name": case_id, "created_at": later_timestamp, "files": []}
     return data
 
 
 @pytest.fixture(scope="function", name="version_data")
-def fixture_version_data(
-    empty_version_data: dict, family2_data: dict, sample2_data: dict
-) -> dict:
+def fixture_version_data(empty_version_data: dict, family2_data: dict, sample2_data: dict) -> dict:
     """Return a dummy bundle."""
     data = copy.deepcopy(empty_version_data)
     data["files"] = [
         {
             "path": str(sample2_data["file"]),
             "archive": False,
             "tags": sample2_data["tags"],
@@ -317,14 +310,15 @@
 
 
 @pytest.fixture(scope="function", name="version_obj")
 def fixture_version_obj(bundle_data: dict, store: Store) -> Version:
     """Return a version object."""
     return store.add_bundle(bundle_data)[1]
 
+
 @pytest.fixture(scope="function", name="archive")
 def fixture_archive(populated_store: Store) -> Archive:
     """Return an archive object."""
     return populated_store._get_query(table=Archive).first()
 
 
 # dir fixtures
@@ -397,24 +391,27 @@
 
 
 @pytest.fixture(scope="function", name="spring_file_2")
 def fixture_spring_file_2(sequencing_files_dir: Path) -> Path:
     """Return the path to a SPRING file."""
     return Path(sequencing_files_dir, "lane2.spring")
 
+
 @pytest.fixture(scope="function", name="archived_file")
 def fixture_archived_file(spring_file_1: Path) -> Path:
     """Return the path to an archived file."""
     return spring_file_1
 
+
 @pytest.fixture(scope="function", name="non_archived_file")
 def fixture_non_archived_file(spring_file_2: Path) -> Path:
     """Return the path to a non-archived file."""
     return spring_file_2
 
+
 @pytest.fixture(scope="function", name="spring_file_2")
 def fixture_spring_file_2(sequencing_files_dir: Path) -> Path:
     """Return the path to a SPRING file."""
     return Path(sequencing_files_dir, "lane2.spring")
 
 
 @pytest.fixture(scope="function", name="family_vcf")
```

### Comparing `housekeeper-4.3.0/tests/helper_functions.py` & `housekeeper-4.4.0/tests/helper_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,26 +39,25 @@
     def add_bundle(store: Store, bundle: dict) -> None:
         """Add and commit bundle to housekeeper store"""
         bundle_obj, _ = store.add_bundle(bundle)
         store.session.add(bundle_obj)
         store.session.commit()
 
     @staticmethod
-    def add_archive(store: Store, file_id: int, archiving_task_id:int=1234) -> None:
+    def add_archive(store: Store, file_id: int, archiving_task_id: int = 1234) -> Archive:
         """Adds an archive object to the database."""
         new_archive: Archive = store.create_archive(
             file_id=file_id, archiving_task_id=archiving_task_id
         )
         store.session.add(new_archive)
         store.session.commit()
+        return new_archive
 
     @staticmethod
-    def create_bundle_data(
-        case_id: str, files: List[dict], created_at: dt.datetime = None
-    ) -> dict:
+    def create_bundle_data(case_id: str, files: List[dict], created_at: dt.datetime = None) -> dict:
         """
         Create a new bundle_data dictionary with the given parameters.
 
         :param case_id: The name of the bundle.
         :param files: A list of dictionaries representing file data.
         :param created_at: The timestamp when the bundle was created (optional).
         :return: A dictionary representing the bundle data.
```

### Comparing `housekeeper-4.3.0/tests/store/conftest.py` & `housekeeper-4.4.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/store/filters/test_bundle_filters.py` & `housekeeper-4.4.0/tests/store/filters/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/store/filters/test_file_join_filters.py` & `housekeeper-4.4.0/tests/store/filters/test_file_filters.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,93 @@
 from typing import List
 
+import pytest
 from sqlalchemy.orm import Query
 
-from housekeeper.store.api.core import Store
+from housekeeper.store import Store
+from housekeeper.store.models import File
 from housekeeper.store.filters.file_filters import (
+    filter_files_by_id,
+    filter_files_by_path,
     filter_files_by_tags,
     filter_files_by_is_archived,
 )
-from housekeeper.store.models import File
+
+
+def test_filter_files_by_id_returns_query(populated_store: Store):
+    """Test that filter_files_by_id returns a Query object."""
+
+    # GIVEN a store with a file
+    file: File = populated_store._get_query(table=File).first()
+    assert file
+
+    # WHEN retrieving the file by id
+    file_query: Query = filter_files_by_id(
+        files=populated_store._get_query(table=File), file_id=file.id
+    )
+
+    # THEN a query should be returned
+    assert isinstance(file_query, Query)
+
+
+def test_filter_files_by_id_returns_the_correct_file(populated_store: Store):
+    """Test filtering files by id returns the correct file."""
+
+    # GIVEN a store with a file
+    file: File = populated_store._get_query(table=File).first()
+    assert file
+
+    # WHEN retrieving the file by id
+    file_query: Query = filter_files_by_id(
+        files=populated_store._get_query(table=File),
+        file_id=file.id,
+    )
+
+    # THEN a file should be returned
+    filtered_file: File = file_query.first()
+    assert isinstance(filtered_file, File)
+
+    # THEN the id should match
+    assert filtered_file.id == file.id
+
+
+def test_filter_files_by_path_returns_the_correct_file(populated_store: Store):
+    """ "Test filtering files by path returns the correct file."""
+    # GIVEN a store with some files
+    files = populated_store._get_query(table=File)
+
+    file: File = files.first()
+    assert file
+
+    # WHEN retrieving the file by path
+    file_query: Query = filter_files_by_path(
+        files=files,
+        file_path=file.path,
+    )
+
+    # THEN a file should be returned
+    filtered_file: File = file_query.first()
+    assert isinstance(filtered_file, File)
+
+    # THEN the path should match
+    assert filtered_file.path == file.path
+
+
+@pytest.mark.parametrize("file_id", [-1, None, "non-existent"])
+def test_filter_files_by_id_returns_none_for_invalid_id(populated_store: Store, file_id):
+    """Test that filter_files_by_id returns None for invalid file ids."""
+
+    # WHEN retrieving the file by an invalid id
+    file_query: Query = filter_files_by_id(
+        files=populated_store._get_query(table=File), file_id=file_id
+    )
+
+    # THEN no file should be returned
+    filtered_file: File = file_query.first()
+    assert filtered_file is None
 
 
 def test_filter_files_by_tags_returns_correct_files(populated_store: Store):
     """Test filtering files by tags."""
 
     # GIVEN a store with files
     file: File = populated_store._get_query(table=File).first()
@@ -33,32 +109,32 @@
 def test_filter_files_by_tags_returns_empty_list_when_no_files_match_tags(
     populated_store: Store,
 ):
     """Test filtering files by tags when no files match the given tags."""
 
     # GIVEN a store with files
     # GIVEN a tag that does not exist in any files in the store
-    tag_name = "nonexistent_tag"
+    tag_name = "non_existent_tag"
 
-    # WHEN filtering files by the nonexistent tag
+    # WHEN filtering files by the non_existent tag
     filtered_files_query = filter_files_by_tags(
         files=populated_store._get_join_file_tag_query(),
         tag_names=[tag_name],
     )
 
     # THEN the filtered files list should be empty
     assert len(filtered_files_query.all()) == 0
 
 
 def test_filter_files_by_archive_true(populated_store: Store):
     """Tests the filtering for archived files."""
 
     # GIVEN as store with files
 
-    # WHEN filtering on archived files
+    # WHEN filtering by archived files
     archived_files_query: Query = filter_files_by_is_archived(
         files=populated_store._get_join_file_tags_archive_query(),
         is_archived=True,
     )
 
     # THEN all files returned should have an archive object linked to it
     for file in archived_files_query:
@@ -67,15 +143,15 @@
 
 def test_filter_files_by_archive_false(populated_store: Store):
     """Tests the filtering for non-archived files."""
 
     # GIVEN as store with files
 
     # WHEN filtering on non-archived files
-    archived_files_query: Query = filter_files_by_is_archived(
+    non_archived_files_query: Query = filter_files_by_is_archived(
         files=populated_store._get_join_file_tags_archive_query(),
         is_archived=False,
     )
 
     # THEN none of the files returned should have an archive object linked to it
-    for file in archived_files_query:
+    for file in non_archived_files_query:
         assert file.archive is None
```

### Comparing `housekeeper-4.3.0/tests/store/filters/test_tag_filters.py` & `housekeeper-4.4.0/tests/store/filters/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/store/filters/test_version_bundle_filters.py` & `housekeeper-4.4.0/tests/store/filters/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/store/filters/test_version_filters.py` & `housekeeper-4.4.0/tests/store/filters/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/store/handlers/test_createhandler.py` & `housekeeper-4.4.0/tests/store/handlers/test_createhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,50 +130,45 @@
     # THEN there should be two more files
     assert store._get_query(table=File).count() == starting_file_count + 2
 
 
 def test_add_archive(archiving_task_id: int, populated_store: Store, spring_file_2: Path):
     """Test that adding an archive works as expected."""
     # GIVEN a file that is not archived
-    non_archived_file: File = populated_store.get_files(
-        file_path=spring_file_2.as_posix()
-    ).first()
+    non_archived_file: File = populated_store.get_files(file_path=spring_file_2.as_posix()).first()
     # WHEN adding an archive
     new_archive: Archive = populated_store.create_archive(
         file_id=non_archived_file.id, archiving_task_id=archiving_task_id
     )
     populated_store.session.add(new_archive)
     populated_store.session.commit()
     # THEN an archive should be created
     assert isinstance(new_archive, Archive)
     # THEN the archive should be reachable via the file
     assert non_archived_file.archive == new_archive
 
 
-def test_add_archive_to_archived_file(archiving_task_id: int, populated_store: Store,
-                                      spring_file_1: Path):
+def test_add_archive_to_archived_file(
+    archiving_task_id: int, populated_store: Store, spring_file_1: Path
+):
     """Test that adding an archive to an already archived file raises an error."""
     # GIVEN a file that is archived
-    non_archived_file: File = populated_store.get_files(
-        file_path=spring_file_1.as_posix()
-    ).first()
+    non_archived_file: File = populated_store.get_files(file_path=spring_file_1.as_posix()).first()
     # WHEN adding an archive
     new_archive: Archive = populated_store.create_archive(
         file_id=non_archived_file.id, archiving_task_id=archiving_task_id
     )
     populated_store.session.add(new_archive)
 
     # THEN an SQLAlchemy error should be thrown
     with pytest.raises(IntegrityError):
         populated_store.session.commit()
 
 
-def test_add_file(
-    populated_store: Store, second_family_vcf: Path, family_tag_names: List[str]
-):
+def test_add_file(populated_store: Store, second_family_vcf: Path, family_tag_names: List[str]):
     """Test to create a file with the add file method."""
     # GIVEN the path and the tags for a file
 
     # GIVEN a store populated with a bundle
     bundle: Bundle = populated_store.bundles().first()
     assert isinstance(bundle, Bundle)
```

### Comparing `housekeeper-4.3.0/tests/store/test_models.py` & `housekeeper-4.4.0/tests/store/test_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/test_date.py` & `housekeeper-4.4.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.3.0/tests/test_include.py` & `housekeeper-4.4.0/tests/test_include.py`

 * *Files identical despite different names*

