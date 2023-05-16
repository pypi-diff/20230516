# Comparing `tmp/ezbeq-1.0.0b7.tar.gz` & `tmp/ezbeq-1.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezbeq-1.0.0b7.tar", last modified: Tue May 16 19:23:32 2023, max compression
+gzip compressed data, was "ezbeq-1.0.0b8.tar", last modified: Tue May 16 19:40:54 2023, max compression
```

## Comparing `ezbeq-1.0.0b7.tar` & `ezbeq-1.0.0b8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.476365 ezbeq-1.0.0b7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 19:23:32.472365 ezbeq-1.0.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.464365 ezbeq-1.0.0b7/ezbeq/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.468365 ezbeq-1.0.0b7/ezbeq/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/audiotypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/apis/years.py
--rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/htp1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/iir.py
--rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/jriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    41683 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/minidsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/ezbeq/qsys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.472365 ezbeq-1.0.0b7/ezbeq/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.472365 ezbeq-1.0.0b7/ezbeq/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   860016 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/index-4ab4fdce.js
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/index-fce6f16f.css
--rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 19:22:38.000000 ezbeq-1.0.0b7/ezbeq/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-16 19:22:37.000000 ezbeq-1.0.0b7/ezbeq/ui/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.464365 ezbeq-1.0.0b7/ezbeq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 19:23:32.000000 ezbeq-1.0.0b7/ezbeq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:23:32.476365 ezbeq-1.0.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:23:32.472365 ezbeq-1.0.0b7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-05-16 19:20:54.000000 ezbeq-1.0.0b7/tests/test_minidsp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.965958 ezbeq-1.0.0b8/ezbeq/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 19:40:13.000000 ezbeq-1.0.0b8/ezbeq/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.969958 ezbeq-1.0.0b8/ezbeq/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/audiotypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/apis/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/htp1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/iir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/jriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41683 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/minidsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/ezbeq/qsys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.969958 ezbeq-1.0.0b8/ezbeq/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/ezbeq/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   860016 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/index-4ab4fdce.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/index-fce6f16f.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-16 19:40:12.000000 ezbeq-1.0.0b8/ezbeq/ui/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.969958 ezbeq-1.0.0b8/ezbeq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 19:40:54.000000 ezbeq-1.0.0b8/ezbeq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:40:54.973958 ezbeq-1.0.0b8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    96452 2023-05-16 19:38:54.000000 ezbeq-1.0.0b8/tests/test_minidsp_api.py
```

### Comparing `ezbeq-1.0.0b7/LICENSE` & `ezbeq-1.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/PKG-INFO` & `ezbeq-1.0.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b7/README.md` & `ezbeq-1.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/audiotypes.py` & `ezbeq-1.0.0b8/ezbeq/apis/audiotypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/catalogue.py` & `ezbeq-1.0.0b8/ezbeq/apis/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/contenttypes.py` & `ezbeq-1.0.0b8/ezbeq/apis/contenttypes.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/devices.py` & `ezbeq-1.0.0b8/ezbeq/apis/devices.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/languages.py` & `ezbeq-1.0.0b8/ezbeq/apis/languages.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/meta.py` & `ezbeq-1.0.0b8/ezbeq/apis/meta.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/search.py` & `ezbeq-1.0.0b8/ezbeq/apis/search.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/ws.py` & `ezbeq-1.0.0b8/ezbeq/apis/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     def onOpen(self):
         logger.info("WebSocket connection open")
         self.factory.register(self)
 
     def onClose(self, was_clean, code, reason):
         logger.info(f"WebSocket connection closed: clean? {was_clean}, code: {code}, reason: {reason}")
+        self.factory.unregister_for_levels(self)
 
     def onMessage(self, payload, is_binary):
         try:
             s = payload.decode('utf-8')
             logger.info(f"Received {s}")
             if s.startswith(SUBSCRIBE_LEVELS_CMD):
                 self.factory.register_for_levels(s[len(SUBSCRIBE_LEVELS_CMD) + 1:], self)
@@ -89,14 +90,22 @@
                     else:
                         logger.info(f"Client {client.peer} subscribed to levels for {device}")
                         v.append(client)
             self.__levels_provider[device]()
         else:
             logger.warning(f"Unknown device {device} requested by {client.peer}")
 
+    def unregister_for_levels(self, client: WsProtocol):
+        for k, v in self.__levels_client.items():
+            try:
+                v.remove(client)
+                logger.info(f"Client {client.peer} unsubscribed from levels for {k}")
+            except ValueError:
+                pass
+
     def unregister(self, client: WsProtocol):
         if client in self.__clients:
             logger.info(f"Unregistering client {client.peer}")
             self.__clients.remove(client)
         else:
             found = False
             for device, clients in self.__levels_client.items():
```

### Comparing `ezbeq-1.0.0b7/ezbeq/apis/years.py` & `ezbeq-1.0.0b8/ezbeq/apis/years.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/catalogue.py` & `ezbeq-1.0.0b8/ezbeq/catalogue.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/config.py` & `ezbeq-1.0.0b8/ezbeq/config.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/device.py` & `ezbeq-1.0.0b8/ezbeq/device.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/htp1.py` & `ezbeq-1.0.0b8/ezbeq/htp1.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/iir.py` & `ezbeq-1.0.0b8/ezbeq/iir.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/jriver.py` & `ezbeq-1.0.0b8/ezbeq/jriver.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/main.py` & `ezbeq-1.0.0b8/ezbeq/main.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/minidsp.py` & `ezbeq-1.0.0b8/ezbeq/minidsp.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/qsys.py` & `ezbeq-1.0.0b8/ezbeq/qsys.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/android-chrome-192x192.png` & `ezbeq-1.0.0b8/ezbeq/ui/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/android-chrome-512x512.png` & `ezbeq-1.0.0b8/ezbeq/ui/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/apple-touch-icon.png` & `ezbeq-1.0.0b8/ezbeq/ui/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/index-4ab4fdce.js` & `ezbeq-1.0.0b8/ezbeq/ui/assets/index-4ab4fdce.js`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/index-fce6f16f.css` & `ezbeq-1.0.0b8/ezbeq/ui/assets/index-fce6f16f.css`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-all-400-normal-e41533d5.woff`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-400-normal-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-cyrillic-ext-400-normal-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-greek-400-normal-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-400-normal-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-latin-ext-400-normal-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2` & `ezbeq-1.0.0b8/ezbeq/ui/assets/roboto-vietnamese-400-normal-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/favicon-16x16.png` & `ezbeq-1.0.0b8/ezbeq/ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/favicon-32x32.png` & `ezbeq-1.0.0b8/ezbeq/ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/favicon.ico` & `ezbeq-1.0.0b8/ezbeq/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/index.html` & `ezbeq-1.0.0b8/ezbeq/ui/index.html`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/mstile-150x150.png` & `ezbeq-1.0.0b8/ezbeq/ui/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq/ui/safari-pinned-tab.svg` & `ezbeq-1.0.0b8/ezbeq/ui/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq.egg-info/PKG-INFO` & `ezbeq-1.0.0b8/ezbeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezbeq
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: A small webapp which can send beqcatalogue filters to a DSP device
 Home-page: http://github.com/3ll3d00d/ezbeq
 Author: Matt Khan
 Author-email: mattkhan+ezbeq@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ezbeq-1.0.0b7/ezbeq.egg-info/SOURCES.txt` & `ezbeq-1.0.0b8/ezbeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/ezbeq.egg-info/requires.txt` & `ezbeq-1.0.0b8/ezbeq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/setup.py` & `ezbeq-1.0.0b8/setup.py`

 * *Files identical despite different names*

### Comparing `ezbeq-1.0.0b7/tests/test_minidsp_api.py` & `ezbeq-1.0.0b8/tests/test_minidsp_api.py`

 * *Files identical despite different names*

