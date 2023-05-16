# Comparing `tmp/pure_ocean_breeze-3.9.4.tar.gz` & `tmp/pure_ocean_breeze-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.4.tar", last modified: Tue May  9 07:52:53 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.5.tar", last modified: Tue May 16 13:39:02 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.4.tar` & `pure_ocean_breeze-3.9.5.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31550 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   239812 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.180527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.184527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:52:53.176527 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 07:52:53.000000 pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 07:52:53.188527 pure_ocean_breeze-3.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-09 07:52:41.000000 pure_ocean_breeze-3.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.100108 pure_ocean_breeze-3.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49390 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   240111 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.092108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.096108 pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:39:02.088107 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 13:39:02.000000 pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:39:02.100108 pure_ocean_breeze-3.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-16 13:38:50.000000 pure_ocean_breeze-3.9.5/setup.py
```

### Comparing `pure_ocean_breeze-3.9.4/LICENSE` & `pure_ocean_breeze-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/PKG-INFO` & `pure_ocean_breeze-3.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.4
+Version: 3.9.5
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.4/README.md` & `pure_ocean_breeze-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-05-09 15:28:47"
-__version__ = "3.9.4"
+__updated__ = "2023-05-13 09:20:38"
+__version__ = "3.9.5"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-__updated__ = "2023-03-22 20:22:04"
+__updated__ = "2023-05-16 11:40:07"
 
 import pandas as pd
 import pymysql
 from sqlalchemy import create_engine
 from sqlalchemy import FLOAT, INT, VARCHAR, BIGINT
 from loguru import logger
 import datetime
 import psycopg2 as pg
 import numpy as np
 import requests
 import os
 from typing import Union, Dict, List
 from psycopg2.extensions import register_adapter, AsIs
-from tenacity import retry, stop_after_attempt
+from tenacity import retry, stop_after_attempt, wait_fixed
 import questdb.ingress as qdbing
 from pure_ocean_breeze.state.states import STATES
 from pure_ocean_breeze.state.homeplace import HomePlace
 
 
 class MetaSQLDriver(object):
     """所有sql类数据库通用的一些功能"""
@@ -594,14 +594,15 @@
         -------
         pd.DataFrame
             读取的结果
         """
         a = pd.read_sql(sql_order, con=self.engine)
         return a
 
+    @retry(stop=stop_after_attempt(10), wait=wait_fixed(3))
     def get_data(
         self, sql_order: str, only_array: bool = 0
     ) -> Union[pd.DataFrame, np.ndarray]:
         """以sql命令的方式，从数据库中读取数据
 
         Parameters
         ----------
@@ -819,14 +820,15 @@
 
     def __addapt_numpy_float64(self, numpy_float64):
         return AsIs(numpy_float64)
 
     def __addapt_numpy_int64(self, numpy_int64):
         return AsIs(numpy_int64)
 
+    @retry(stop=stop_after_attempt(10), wait=wait_fixed(3))
     def write_via_df(
         self,
         df: pd.DataFrame,
         table_name: str,
         symbols: Union[str, bool, List[int], List[str]] = None,
         tuple_col: Union[str, List[str]] = None,
     ) -> None:
@@ -853,14 +855,15 @@
         if symbols is not None:
             with qdbing.Sender(self.host, 9009) as sender:
                 sender.dataframe(df, table_name=table_name, symbols=symbols)
         else:
             with qdbing.Sender(self.host, 9009) as sender:
                 sender.dataframe(df, table_name=table_name)
 
+    @retry(stop=stop_after_attempt(10), wait=wait_fixed(3))
     def get_data_with_tuple(
         self,
         sql_order: str,
         tuple_col: Union[str, List[str]] = "fac",
         without_timestamp: bool = 1,
     ) -> pd.DataFrame:
         """从questdb数据库中，读取那些值中带有元组或列表的表格
```

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/data/write_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-03-26 22:29:53"
+__updated__ = "2023-05-16 11:40:12"
 
 import time
 
 try:
     import rqdatac
 
     rqdatac.init()
@@ -384,15 +384,15 @@
         "lows_unadj",
         "closes_unadj",
         "sharenums",
         "total_sharenums",
         "ages",
         "sts",
         "states",
-        "volumes",
+        "amounts",
         "pb",
         "pe",
         "vwaps",
         "adjfactors",
         "stop_ups",
         "stop_downs",
     ]
@@ -708,30 +708,34 @@
         "booktoprice",
         "leverage",
         "liquidity",
         "nonlinearsize",
     ]
     ds = {k: [] for k in style_names}
     if len(tradedates) >= 1:
-        codes=[convert_code(i)[0] for i in list(read_daily(open=1).columns)]
-        style = rqdatac.get_factor_exposure(order_book_ids=codes,start_date=pd.Timestamp(last_date)+pd.Timedelta(days=1), end_date=now).reset_index()
+        codes = [convert_code(i)[0] for i in list(read_daily(open=1).columns)]
+        style = rqdatac.get_factor_exposure(
+            order_book_ids=codes,
+            start_date=pd.Timestamp(last_date) + pd.Timedelta(days=1),
+            end_date=now,
+        ).reset_index()
         style = style.rename(
             columns={
                 "earnings_yield": "earningsyield",
                 "tradedate": "date",
                 "ticker": "code",
                 "residual_volatility": "residualvolatility",
                 "book_to_price": "booktoprice",
                 "non_linear_size": "nonlinearsize",
-                'order_book_id':'code'
+                "order_book_id": "code",
             }
         )
-        style=style[style_names+['date','code']]
+        style = style[style_names + ["date", "code"]]
         style.date = pd.to_datetime(style.date)
-        style.code = style.code.apply(lambda x:convert_code(x)[0])
+        style.code = style.code.apply(lambda x: convert_code(x)[0])
         for s in style_names:
             ds[s].append(style.pivot(columns="code", index="date", values=s))
         for k, v in ds.items():
             old = pd.read_parquet(homeplace.barra_data_file + k + ".parquet")
             new = pd.concat(v)
             new = pd.concat([old, new])
             new.to_parquet(homeplace.barra_data_file + k + ".parquet")
```

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/labor/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-05-09 15:46:45"
+__updated__ = "2023-05-16 11:40:18"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -3765,15 +3765,15 @@
             [self.factors] + list(self.barras.values()), axis=1
         ).dropna()
 
     # DONE: 修改风格因子展示顺序至报告的顺序
     def get_corr(self):
         """计算每一期的相关系数，再求平均值"""
         self.corr_by_step = self.corr_pri.groupby(["date"]).apply(
-            lambda x: x.corr().head(1)
+            lambda x: x.rank().corr().head(1)
         )
         self.__corr = self.corr_by_step.mean()
         self.__corr = self.__corr.rename(index=self.rename_dict)
         self.__corr = self.__corr.to_frame("相关系数").T
 
         self.__corr = self.__corr[self.sort_names]
         self.__corr = self.__corr.T
@@ -4118,49 +4118,52 @@
         if history_file is not None:
             if os.path.exists(homeplace.update_data_file + history_file):
                 old = pd.read_parquet(homeplace.update_data_file + history_file)
                 old_date = old.index.max()
                 if old_date == self.fac.date.max():
                     logger.info(f"本地文件已经是最新的了，无需计算")
                 else:
-                    new_date = self.find_begin(self.tradedays, old_date, self.backsee)
-                    fac = self.fac[self.fac.date > new_date]
-                    iter_item = [i for i in iter_item if i > new_date]
-                    if whole_cross:
-                        for end_date in tqdm.auto.tqdm(iter_item):
-                            start_date = self.find_begin(
-                                self.tradedays, end_date, self.backsee
+                    try:
+                        new_date = self.find_begin(self.tradedays, old_date, self.backsee)
+                        fac = self.fac[self.fac.date > new_date]
+                        iter_item = [i for i in iter_item if i > new_date]
+                        if whole_cross:
+                            for end_date in tqdm.auto.tqdm(iter_item):
+                                start_date = self.find_begin(
+                                    self.tradedays, end_date, self.backsee
+                                )
+                                df = fac[(fac.date >= start_date) & (fac.date <= end_date)]
+                                df = func(df)
+                                df = df.to_frame().T
+                                df.index = [end_date]
+                                res.append(df)
+                            fac = pd.concat(res).resample("M").last()
+                            self.fac = pd.concat([old, fac])
+                        else:
+                            tqdm.auto.tqdm.pandas(
+                                desc="when the dawn comes, tonight will be a memory too."
                             )
-                            df = fac[(fac.date >= start_date) & (fac.date <= end_date)]
-                            df = func(df)
-                            df = df.to_frame().T
-                            df.index = [end_date]
-                            res.append(df)
-                        fac = pd.concat(res).resample("M").last()
-                        self.fac = pd.concat([old, fac])
-                    else:
-                        tqdm.auto.tqdm.pandas(
-                            desc="when the dawn comes, tonight will be a memory too."
-                        )
-                        fac = fac.groupby(["code"]).progress_apply(
-                            lambda x: self.make_monthly_factors_single_code(
-                                x, func, daily=daily
+                            fac = fac.groupby(["code"]).progress_apply(
+                                lambda x: self.make_monthly_factors_single_code(
+                                    x, func, daily=daily
+                                )
                             )
-                        )
-                        fac = (
-                            fac.reset_index(level=1, drop=True)
-                            .reset_index()
-                            .set_index(["date", "code"])
-                            .unstack()
-                        )
-                        fac.columns = [i[1] for i in list(fac.columns)]
-                        fac = fac.resample("M").last()
-                        self.fac = pd.concat([old, fac])
-                    self.fac.to_parquet(homeplace.update_data_file + history_file)
-                    logger.success(f"本地文件已经更新完成")
+                            fac = (
+                                fac.reset_index(level=1, drop=True)
+                                .reset_index()
+                                .set_index(["date", "code"])
+                                .unstack()
+                            )
+                            fac.columns = [i[1] for i in list(fac.columns)]
+                            fac = fac.resample("M").last()
+                            self.fac = pd.concat([old, fac])
+                        self.fac.to_parquet(homeplace.update_data_file + history_file)
+                        logger.success(f"本地文件已经更新完成")
+                    except Exception:
+                        logger.info(f"本地文件已经是最新的了，无需计算")
             else:
                 logger.info("第一次计算，请耐心等待……")
                 if whole_cross:
                     for end_date in tqdm.auto.tqdm(iter_item):
                         start_date = self.find_begin(
                             self.tradedays, end_date, self.backsee
                         )
```

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/homeplace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 初始化时保存的路径
 """
 
-__updated__ = "2022-11-14 11:38:53"
+__updated__ = "2023-05-11 22:01:50"
 
 import os
 import pickle
 
 
 class HomePlace(object):
     """
```

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.4
+Version: 3.9.5
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.4/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.5/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.4/setup.py` & `pure_ocean_breeze-3.9.5/setup.py`

 * *Files identical despite different names*

