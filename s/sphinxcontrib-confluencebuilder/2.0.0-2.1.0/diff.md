# Comparing `tmp/sphinxcontrib-confluencebuilder-2.0.0.tar.gz` & `tmp/sphinxcontrib_confluencebuilder-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-confluencebuilder-2.0.0.tar", last modified: Mon Jan  2 23:49:53 2023, max compression
+gzip compressed data, was "sphinxcontrib_confluencebuilder-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-confluencebuilder-2.0.0.tar` & `sphinxcontrib_confluencebuilder-2.1.0.tar`

### file list

```diff
@@ -1,258 +1,146 @@
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.346266 sphinxcontrib-confluencebuilder-2.0.0/
--rw-rw-rw-   0        0        0     1303 2023-01-02 23:38:07.000000 sphinxcontrib-confluencebuilder-2.0.0/AUTHORS
--rw-rw-rw-   0        0        0     3159 2023-01-02 23:38:07.000000 sphinxcontrib-confluencebuilder-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      145 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5783 2023-01-02 23:49:53.346266 sphinxcontrib-confluencebuilder-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4264 2023-01-02 06:38:55.000000 sphinxcontrib-confluencebuilder-2.0.0/README.rst
--rw-rw-rw-   0        0        0     1664 2023-01-02 06:38:55.000000 sphinxcontrib-confluencebuilder-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1250 2023-01-02 23:49:53.352266 sphinxcontrib-confluencebuilder-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      249 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.115266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.181266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/
--rw-rw-rw-   0        0        0    17028 2023-01-02 23:48:24.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/__init__.py
--rw-rw-rw-   0        0        0     3678 2022-07-23 17:34:21.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/__main__.py
--rw-rw-rw-   0        0        0    14636 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/assets.py
--rw-rw-rw-   0        0        0    46516 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/builder.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.185267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/
--rw-rw-rw-   0        0        0       25 2021-11-14 01:09:10.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/__init__.py
--rw-rw-rw-   0        0        0     2481 2022-07-23 17:34:21.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/build.py
--rw-rw-rw-   0        0        0    11587 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/report.py
--rw-rw-rw-   0        0        0     6891 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/wipe.py
--rw-rw-rw-   0        0        0     3163 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/compat.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.192267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/
--rw-rw-rw-   0        0        0     2775 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/__init__.py
--rw-rw-rw-   0        0        0    27150 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/checks.py
--rw-rw-rw-   0        0        0     3802 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/defaults.py
--rw-rw-rw-   0        0        0     1474 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/env.py
--rw-rw-rw-   0        0        0     3574 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/manager.py
--rw-rw-rw-   0        0        0     3358 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/notifications.py
--rw-rw-rw-   0        0        0    17747 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/validation.py
--rw-rw-rw-   0        0        0     9784 2023-01-02 05:52:38.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/directives.py
--rw-rw-rw-   0        0        0     9752 2022-05-29 19:12:07.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/exceptions.py
--rw-rw-rw-   0        0        0     3105 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/intersphinx.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.195267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/
--rw-rw-rw-   0        0        0      475 2022-05-29 19:12:07.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.117266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ar/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.197266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0      590 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1387 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.117266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bg/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.199266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/
--rw-rw-rw-   0        0        0      533 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1330 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.118266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bn/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.201266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/
--rw-rw-rw-   0        0        0      458 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1284 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.118266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ca/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.203267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0        0        0      500 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1297 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.119266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cs/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.205268 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0      526 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1323 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.119266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cy/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.207266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/
--rw-rw-rw-   0        0        0      579 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1376 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.120266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/da/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.209265 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/
--rw-rw-rw-   0        0        0      499 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1296 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.122267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/de/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.212267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      503 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1300 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.123265 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/el/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.214267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/
--rw-rw-rw-   0        0        0      518 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1315 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.124266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eo/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.216267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/
--rw-rw-rw-   0        0        0      460 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1300 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.124266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/es/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.218266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0      458 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1287 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.125265 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/et/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.221266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/
--rw-rw-rw-   0        0        0      505 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1302 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.125265 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eu/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.223267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/
--rw-rw-rw-   0        0        0      500 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1297 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.126266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fi/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.225269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      505 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1302 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.127272 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.227266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      503 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1300 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.127272 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/he/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.229267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/
--rw-rw-rw-   0        0        0      507 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1333 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.128269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hi/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.231267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      535 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1332 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.128269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hr/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.233266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      573 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1370 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.129268 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hu/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.235271 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0      510 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1307 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.130266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/id/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.238268 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/
--rw-rw-rw-   0        0        0      497 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1294 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.130266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/it/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.240269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0      458 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1284 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.131266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ja/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.242267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0      499 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1296 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.131266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ko/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.244267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0        0        0      492 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1289 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.132266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lt/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.246267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/
--rw-rw-rw-   0        0        0      609 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1406 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.133267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lv/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.248267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0        0        0      535 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1332 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.133267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/mk/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.250267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/
--rw-rw-rw-   0        0        0      535 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1332 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.134267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nb/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.252270 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/
--rw-rw-rw-   0        0        0      509 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1306 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.134267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ne/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.254267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/
--rw-rw-rw-   0        0        0      551 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1351 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.135269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nl/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.257268 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0      498 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1295 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.135269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pl/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.259267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0      648 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1445 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.136265 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pt_BR/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.262267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0        0        0      513 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1313 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.137267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ro/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.264268 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/
--rw-rw-rw-   0        0        0      546 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1343 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.137267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ru/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.266267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0      623 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1449 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.138266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/si/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.268267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/
--rw-rw-rw-   0        0        0      458 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1287 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.138266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sk/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.270269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/
--rw-rw-rw-   0        0        0      527 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1324 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.139267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sl/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.272267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0        0        0      512 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1338 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-rw-rw-   0        0        0      821 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.139267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sq/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.274266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/
--rw-rw-rw-   0        0        0      511 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1308 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.140267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sr_CS/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.276266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/
--rw-rw-rw-   0        0        0      540 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1369 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.141266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sv/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.278267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0        0        0      502 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1302 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.141266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ta/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.280269 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/
--rw-rw-rw-   0        0        0      546 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1343 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.142266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/te/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.282266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/
--rw-rw-rw-   0        0        0      538 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1335 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.142266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/tr/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.285270 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      505 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1302 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.143266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/uk/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.288266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/
--rw-rw-rw-   0        0        0      689 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1486 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.144266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/vi/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.290271 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      496 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1293 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.144266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/zh_TW/
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.292268 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-rw-rw-   0        0        0     1304 2023-01-02 19:45:34.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-rw-rw-   0        0        0     4587 2022-07-23 17:34:21.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/logger.py
--rw-rw-rw-   0        0        0     5334 2023-01-02 05:52:38.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/nodes.py
--rw-rw-rw-   0        0        0    41254 2023-01-02 23:23:55.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/publisher.py
--rw-rw-rw-   0        0        0      478 2022-05-29 19:12:07.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/reportbuilder.py
--rw-rw-rw-   0        0        0    14809 2023-01-02 23:24:00.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/rest.py
--rw-rw-rw-   0        0        0     5649 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/roles.py
--rw-rw-rw-   0        0        0    11912 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/singlebuilder.py
--rw-rw-rw-   0        0        0     9528 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/state.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.295266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/std/
--rw-rw-rw-   0        0        0       25 2021-05-30 13:45:40.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/std/__init__.py
--rw-rw-rw-   0        0        0    11140 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/std/confluence.py
--rw-rw-rw-   0        0        0      367 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/std/sphinx.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.299266 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/
--rw-rw-rw-   0        0        0     2096 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/index.py
--rw-rw-rw-   0        0        0     1232 2022-07-23 17:34:21.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/search.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.306267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/
--rw-rw-rw-   0        0        0       25 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
--rw-rw-rw-   0        0        0     1825 2022-05-29 19:12:07.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
--rw-rw-rw-   0        0        0     1663 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
--rw-rw-rw-   0        0        0     2225 2022-09-03 17:36:26.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
--rw-rw-rw-   0        0        0     2352 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
--rw-rw-rw-   0        0        0      770 2022-05-29 19:12:07.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/search.html
--rw-rw-rw-   0        0        0   127051 2023-01-02 23:38:01.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/translator.py
--rw-rw-rw-   0        0        0     7619 2022-07-26 01:08:52.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/svg.py
--rw-rw-rw-   0        0        0    17778 2022-11-27 20:04:11.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/translator.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.313267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/
--rw-rw-rw-   0        0        0    12143 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/__init__.py
--rw-rw-rw-   0        0        0     1953 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
--rw-rw-rw-   0        0        0     1786 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
--rw-rw-rw-   0        0        0     2582 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
--rw-rw-rw-   0        0        0     1604 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
--rw-rw-rw-   0        0        0     4306 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
--rw-rw-rw-   0        0        0     2568 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
--rw-rw-rw-   0        0        0    11331 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/util.py
--rw-rw-rw-   0        0        0      707 2023-01-02 01:52:19.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/writer.py
-drwxrwxrwx   0        0        0        0 2023-01-02 23:49:53.345267 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/
--rw-rw-rw-   0        0        0     5783 2023-01-02 23:49:52.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11147 2023-01-02 23:49:53.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-02 23:49:52.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-01-02 23:49:52.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-01-02 23:49:52.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-02 23:49:52.000000 sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib_confluencebuilder.egg-info/top_level.txt
+-rw-r--r--   0        0        0     4076 2023-05-16 00:58:11.667937 sphinxcontrib_confluencebuilder-2.1.0/README.rst
+-rw-r--r--   0        0        0     1774 2023-05-07 18:59:45.812201 sphinxcontrib_confluencebuilder-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    18061 2023-05-16 01:13:54.764696 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__init__.py
+-rw-r--r--   0        0        0     3630 2023-04-07 19:29:44.220864 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__main__.py
+-rw-r--r--   0        0        0    14586 2023-04-15 14:46:27.000054 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/assets.py
+-rw-r--r--   0        0        0    48600 2023-05-13 15:11:25.713682 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/builder.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.404126 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/build.py
+-rw-r--r--   0        0        0    11521 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/report.py
+-rw-r--r--   0        0        0     6780 2023-04-08 16:47:36.734308 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/wipe.py
+-rw-r--r--   0        0        0     3476 2023-04-07 19:29:44.224766 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/compat.py
+-rw-r--r--   0        0        0     2929 2023-04-08 16:47:36.735307 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/__init__.py
+-rw-r--r--   0        0        0    28152 2023-04-17 01:06:14.719799 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/checks.py
+-rw-r--r--   0        0        0     4150 2023-04-16 01:30:57.889226 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/defaults.py
+-rw-r--r--   0        0        0     1431 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/env.py
+-rw-r--r--   0        0        0     3529 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/manager.py
+-rw-r--r--   0        0        0     3402 2023-04-08 16:47:36.736308 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/notifications.py
+-rw-r--r--   0        0        0    17687 2023-04-07 19:29:44.229651 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/validation.py
+-rw-r--r--   0        0        0    11596 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/directives.py
+-rw-r--r--   0        0        0     9196 2023-04-07 19:29:44.230626 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/exceptions.py
+-rw-r--r--   0        0        0     3057 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/intersphinx.py
+-rw-r--r--   0        0        0      432 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/__init__.py
+-rw-r--r--   0        0        0      590 2023-01-05 22:53:18.094822 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1387 2023-05-16 00:43:39.061378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      533 2023-01-05 22:53:18.096782 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1330 2023-05-16 00:43:39.062380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.098731 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.063378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2023-01-05 22:53:18.099707 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      526 2023-01-05 22:53:18.100682 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1323 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      579 2023-01-05 22:53:18.101658 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1376 2023-05-16 00:43:39.065377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2023-01-05 22:53:18.103611 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.066377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2023-01-05 22:53:18.104592 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      518 2023-01-05 22:53:18.106543 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1315 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      460 2023-01-05 22:53:18.108080 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.109032 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.110006 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2023-01-05 22:53:18.111962 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.113918 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.070376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2023-01-05 22:53:18.114891 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      507 2023-01-05 22:53:18.116843 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1333 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.117819 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      573 2023-01-05 22:53:18.118796 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1370 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      510 2023-01-05 22:53:18.120751 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1307 2023-05-16 00:43:39.073376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      497 2023-01-05 22:53:18.122701 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1294 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.124656 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2023-01-05 22:53:18.125629 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      492 2023-01-05 22:53:18.127584 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1289 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      609 2023-01-05 22:53:18.128562 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1406 2023-05-16 00:43:39.076379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.130512 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.077376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.133442 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.080380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      509 2023-01-05 22:53:18.135398 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1306 2023-05-16 00:43:39.081380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      551 2023-01-05 22:53:18.137353 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1351 2023-05-16 00:43:39.082381 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      498 2023-01-05 22:53:18.139304 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1295 2023-05-16 00:43:39.083377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      648 2023-01-05 22:53:18.141258 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1445 2023-05-16 00:43:39.084381 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      513 2023-01-05 22:53:18.143207 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1313 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2023-01-05 22:53:18.144187 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      623 2023-01-05 22:53:18.146138 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1449 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.148092 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      527 2023-01-05 22:53:18.150044 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1324 2023-05-16 00:43:39.087380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      512 2023-01-05 22:53:18.151996 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1338 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      821 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
+-rw-r--r--   0        0        0      511 2023-01-05 22:53:18.153947 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1308 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      540 2023-01-05 22:53:18.155966 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1369 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      502 2023-01-05 22:53:18.158443 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.090376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2023-01-05 22:53:18.160396 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      538 2023-01-05 22:53:18.162349 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1335 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.164303 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      689 2023-01-05 22:53:18.165278 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1486 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      496 2023-01-05 22:53:18.167232 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1293 2023-05-16 00:43:39.093380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      504 2023-01-05 22:48:19.243628 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1304 2023-05-16 00:43:53.313328 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0     4581 2023-04-07 19:29:44.232579 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/logger.py
+-rw-r--r--   0        0        0     6304 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/nodes.py
+-rw-r--r--   0        0        0    49499 2023-05-14 05:04:32.872359 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/publisher.py
+-rw-r--r--   0        0        0      430 2023-04-07 19:29:44.234534 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/reportbuilder.py
+-rw-r--r--   0        0        0    14702 2023-04-07 19:29:44.235511 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/rest.py
+-rw-r--r--   0        0        0     7784 2023-05-13 21:00:30.924232 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/roles.py
+-rw-r--r--   0        0        0    11845 2023-04-07 19:29:44.236486 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/singlebuilder.py
+-rw-r--r--   0        0        0     9455 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/state.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.418126 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/__init__.py
+-rw-r--r--   0        0        0    12663 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/confluence.py
+-rw-r--r--   0        0        0      319 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/sphinx.py
+-rw-r--r--   0        0        0     2038 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/__init__.py
+-rw-r--r--   0        0        0     4747 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/index.py
+-rw-r--r--   0        0        0     1189 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/search.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.420125 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-07 19:29:44.240391 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
+-rw-r--r--   0        0        0     1634 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
+-rw-r--r--   0        0        0     2201 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
+-rw-r--r--   0        0        0     2323 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
+-rw-r--r--   0        0        0      758 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/search.html
+-rw-r--r--   0        0        0   136506 2023-05-14 03:33:11.714778 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/translator.py
+-rw-r--r--   0        0        0     7571 2023-04-08 04:21:05.378651 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/svg.py
+-rw-r--r--   0        0        0    17887 2023-04-22 17:53:45.115343 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/translator.py
+-rw-r--r--   0        0        0    12095 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/__init__.py
+-rw-r--r--   0        0        0     1910 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
+-rw-r--r--   0        0        0     1743 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
+-rw-r--r--   0        0        0     2534 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
+-rw-r--r--   0        0        0     1556 2023-04-07 19:29:44.248204 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
+-rw-r--r--   0        0        0     4240 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
+-rw-r--r--   0        0        0     2520 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
+-rw-r--r--   0        0        0    11692 2023-05-14 03:23:15.068220 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/util.py
+-rw-r--r--   0        0        0      659 2023-04-07 19:29:44.250159 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/writer.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.1.0/PKG-INFO
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/PKG-INFO` & `sphinxcontrib_confluencebuilder-2.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,174 +1,165 @@
-Metadata-Version: 2.1
-Name: sphinxcontrib-confluencebuilder
-Version: 2.0.0
-Summary: Sphinx extension to build Atlassian Confluence Storage Markup
-Author-email: Anthony Shaw <anthonyshaw@apache.org>
-Maintainer-email: James Knight <james.d.knight@live.com>
-License: BSD-2-Clause
-Project-URL: Documentation, https://sphinxcontrib-confluencebuilder.readthedocs.io
-Project-URL: Download, https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder
-Project-URL: Source, https://github.com/sphinx-contrib/confluencebuilder
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Sphinx
-Classifier: Framework :: Sphinx :: Extension
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Documentation
-Classifier: Topic :: Documentation :: Sphinx
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS
-
-.. -*- restructuredtext -*-
-
-=======================================
-Atlassian Confluence Builder for Sphinx
-=======================================
-
-.. image:: https://img.shields.io/pypi/v/sphinxcontrib-confluencebuilder.svg
-   :target: https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder
-   :alt: pip Version
-
-.. image:: https://github.com/sphinx-contrib/confluencebuilder/actions/workflows/build.yml/badge.svg
-    :target: https://github.com/sphinx-contrib/confluencebuilder/actions/workflows/build.yml
-    :alt: Build Status
-
-.. image:: https://readthedocs.org/projects/sphinxcontrib-confluencebuilder/badge/?version=latest
-   :target: https://sphinxcontrib-confluencebuilder.readthedocs.io/
-   :alt: Documentation Status
-
-.. image:: https://img.shields.io/pypi/dm/sphinxcontrib-confluencebuilder.svg
-   :target: https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder/
-   :alt: PyPI download month
-
-Sphinx_ extension to build Confluence® compatible markup format files and
-optionally publish them to a Confluence instance.
-
-Requirements
-============
-
-Active release (v1.9) requirements:
-
-* Confluence_ Cloud or Data Center / Server 7.8+
-* Python_ 2.7 or 3.7+
-* Requests_ 2.14.0+
-* Sphinx_ 1.8 or 4.1+
-
-Next release requirements:
-
-* Confluence_ Cloud or Data Center / Server 7.11+
-* Python_ 3.7+
-* Requests_ 2.14.0+
-* Sphinx_ 5.0+
-
-Installing
-==========
-
-The recommended method to installing this extension is using pip_:
-
-.. code-block:: shell
-
-   pip install sphinxcontrib-confluencebuilder
-    (or)
-   python -m pip install sphinxcontrib-confluencebuilder
-
-For a more in-depth installation information, see also:
-
- | Atlassian Confluence Builder for Sphinx - Installation
- | https://sphinxcontrib-confluencebuilder.readthedocs.io/install
-
-Usage
-=====
-
-- Register the extension ``sphinxcontrib.confluencebuilder`` in the project's
-  configuration script (``conf.py``):
-
-.. code-block:: python
-
-   extensions = [
-       'sphinxcontrib.confluencebuilder',
-   ]
-
-- Run sphinx-build with the builder ``confluence``:
-
-.. code-block:: shell
-
-   sphinx-build -b confluence . _build/confluence -E -a
-    (or)
-   python -m sphinx -b confluence . _build/confluence -E -a
-
-For more information on the usage of this extension, see also:
-
- | Atlassian Confluence Builder for Sphinx - Tutorial
- | https://sphinxcontrib-confluencebuilder.readthedocs.io/tutorial
-
-Configuration
-=============
-
-The following is an example of a simple configuration for Confluence generation
-and publishing:
-
-.. code-block:: python
-
-   extensions = [
-       'sphinxcontrib.confluencebuilder',
-   ]
-   confluence_publish = True
-   confluence_space_name = 'TEST'
-   confluence_parent_page = 'Documentation'
-   confluence_server_url = 'https://intranet-wiki.example.com/'
-   confluence_ask_user = True
-   confluence_ask_password = True
-
-For a complete list of configuration options, see also:
-
- | Atlassian Confluence Builder for Sphinx - Configuration
- | https://sphinxcontrib-confluencebuilder.readthedocs.io/configuration
-
-Features
-========
-
-For a complete list of supported markup, extensions, etc.; see:
-
- | Atlassian Confluence Builder for Sphinx - Features
- | https://sphinxcontrib-confluencebuilder.readthedocs.io/features
-
-For a complete list of directives supported by this extension, see:
-
- | Atlassian Confluence Builder for Sphinx - Directives
- | https://sphinxcontrib-confluencebuilder.readthedocs.io/directives
-
-Demonstration
-=============
-
-A demonstration of this extension can be seen by inspecting the published
-validation/testing documents found here:
-
- | Atlassian Confluence Builder for Sphinx - Online Demo on Confluence Cloud
- | https://sphinxcontrib-confluencebuilder.atlassian.net/
-
-----
-
-| Atlassian Confluence Builder for Sphinx project is unaffiliated with
-  Atlassian.
-| Atlassian is a registered trademark of Atlassian Pty Ltd.
-| Confluence is a registered trademark of Atlassian Pty Ltd.
-
-.. _Confluence: https://www.atlassian.com/software/confluence
-.. _Python: https://www.python.org/
-.. _Requests: https://pypi.python.org/pypi/requests
-.. _Sphinx: https://www.sphinx-doc.org/
-.. _pip: https://pip.pypa.io/
+Metadata-Version: 2.1
+Name: sphinxcontrib-confluencebuilder
+Version: 2.1.0
+Summary: Sphinx extension to build Atlassian Confluence Storage Markup
+Author-email: Anthony Shaw <anthonyshaw@apache.org>
+Maintainer-email: James Knight <james.d.knight@live.com>
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Sphinx
+Classifier: Framework :: Sphinx :: Extension
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Utilities
+Requires-Dist: requests>=2.14.0
+Requires-Dist: sphinx>=5.0
+Project-URL: Documentation, https://sphinxcontrib-confluencebuilder.readthedocs.io
+Project-URL: Download, https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder
+Project-URL: Source, https://github.com/sphinx-contrib/confluencebuilder
+
+.. -*- restructuredtext -*-
+
+=======================================
+Atlassian Confluence Builder for Sphinx
+=======================================
+
+.. image:: https://img.shields.io/pypi/v/sphinxcontrib-confluencebuilder.svg
+   :target: https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder
+   :alt: pip Version
+
+.. image:: https://github.com/sphinx-contrib/confluencebuilder/actions/workflows/build.yml/badge.svg
+    :target: https://github.com/sphinx-contrib/confluencebuilder/actions/workflows/build.yml
+    :alt: Build Status
+
+.. image:: https://readthedocs.org/projects/sphinxcontrib-confluencebuilder/badge/?version=latest
+   :target: https://sphinxcontrib-confluencebuilder.readthedocs.io/
+   :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/dm/sphinxcontrib-confluencebuilder.svg
+   :target: https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder/
+   :alt: PyPI download month
+
+Sphinx_ extension to build Confluence® compatible markup format files and
+optionally publish them to a Confluence instance.
+
+Requirements
+============
+
+* Confluence_ Cloud or Data Center / Server 7.13+
+* Python_ 3.7+
+* Requests_ 2.14.0+
+* Sphinx_ 5.3+
+
+Installing
+==========
+
+The recommended method to installing this extension is using pip_:
+
+.. code-block:: shell
+
+   pip install sphinxcontrib-confluencebuilder
+    (or)
+   python -m pip install sphinxcontrib-confluencebuilder
+
+For a more in-depth installation information, see also:
+
+ | Atlassian Confluence Builder for Sphinx - Installation
+ | https://sphinxcontrib-confluencebuilder.readthedocs.io/install
+
+Usage
+=====
+
+- Register the extension ``sphinxcontrib.confluencebuilder`` in the project's
+  configuration script (``conf.py``):
+
+.. code-block:: python
+
+   extensions = [
+       'sphinxcontrib.confluencebuilder',
+   ]
+
+- Run sphinx-build with the builder ``confluence``:
+
+.. code-block:: shell
+
+   sphinx-build -b confluence . _build/confluence -E -a
+    (or)
+   python -m sphinx -b confluence . _build/confluence -E -a
+
+For more information on the usage of this extension, see also:
+
+ | Atlassian Confluence Builder for Sphinx - Tutorial
+ | https://sphinxcontrib-confluencebuilder.readthedocs.io/tutorial
+
+Configuration
+=============
+
+The following is an example of a simple configuration for Confluence generation
+and publishing:
+
+.. code-block:: python
+
+   extensions = [
+       'sphinxcontrib.confluencebuilder',
+   ]
+   confluence_publish = True
+   confluence_space_name = 'TEST'
+   confluence_parent_page = 'Documentation'
+   confluence_server_url = 'https://intranet-wiki.example.com/'
+   confluence_ask_user = True
+   confluence_ask_password = True
+
+For a complete list of configuration options, see also:
+
+ | Atlassian Confluence Builder for Sphinx - Configuration
+ | https://sphinxcontrib-confluencebuilder.readthedocs.io/configuration
+
+Features
+========
+
+For a complete list of supported markup, extensions, etc.; see:
+
+ | Atlassian Confluence Builder for Sphinx - Features
+ | https://sphinxcontrib-confluencebuilder.readthedocs.io/features
+
+For a complete list of directives supported by this extension, see:
+
+ | Atlassian Confluence Builder for Sphinx - Directives
+ | https://sphinxcontrib-confluencebuilder.readthedocs.io/directives
+
+Demonstration
+=============
+
+A demonstration of this extension can be seen by inspecting the published
+validation/testing documents found here:
+
+ | Atlassian Confluence Builder for Sphinx - Online Demo on Confluence Cloud
+ | https://sphinxcontrib-confluencebuilder.atlassian.net/
+
+----
+
+| Atlassian Confluence Builder for Sphinx project is unaffiliated with
+  Atlassian.
+| Atlassian is a registered trademark of Atlassian Pty Ltd.
+| Confluence is a registered trademark of Atlassian Pty Ltd.
+
+.. _Confluence: https://www.atlassian.com/software/confluence
+.. _Python: https://www.python.org/
+.. _Requests: https://pypi.python.org/pypi/requests
+.. _Sphinx: https://www.sphinx-doc.org/
+.. _pip: https://pip.pypa.io/
+
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/README.rst` & `sphinxcontrib_confluencebuilder-2.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,27 +22,18 @@
 
 Sphinx_ extension to build Confluence® compatible markup format files and
 optionally publish them to a Confluence instance.
 
 Requirements
 ============
 
-Active release (v1.9) requirements:
-
-* Confluence_ Cloud or Data Center / Server 7.8+
-* Python_ 2.7 or 3.7+
-* Requests_ 2.14.0+
-* Sphinx_ 1.8 or 4.1+
-
-Next release requirements:
-
-* Confluence_ Cloud or Data Center / Server 7.11+
+* Confluence_ Cloud or Data Center / Server 7.13+
 * Python_ 3.7+
 * Requests_ 2.14.0+
-* Sphinx_ 5.0+
+* Sphinx_ 5.3+
 
 Installing
 ==========
 
 The recommended method to installing this extension is using pip_:
 
 .. code-block:: shell
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/pyproject.toml` & `sphinxcontrib_confluencebuilder-2.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    'setuptools',
+    'flit_core>=3.7',
 ]
-build-backend = 'setuptools.build_meta'
+build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'sphinxcontrib-confluencebuilder'
 description = 'Sphinx extension to build Atlassian Confluence Storage Markup'
 authors = [
     {name = 'Anthony Shaw', email = 'anthonyshaw@apache.org'},
 ]
@@ -33,19 +33,25 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Documentation',
     'Topic :: Documentation :: Sphinx',
     'Topic :: Utilities',
 ]
+dependencies = [
+    'requests>=2.14.0',
+    'sphinx>=5.0',
+]
 dynamic = [
-    'entry-points',
     'version',
 ]
 
 [project.urls]
 Documentation = 'https://sphinxcontrib-confluencebuilder.readthedocs.io'
 Download = 'https://pypi.python.org/pypi/sphinxcontrib-confluencebuilder'
 Source = 'https://github.com/sphinx-contrib/confluencebuilder'
 
 [project.scripts]
 sphinx-build-confluence = 'sphinxcontrib.confluencebuilder.__main__:main'
+
+[tool.flit.module]
+name = 'sphinxcontrib.confluencebuilder'
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/setup.cfg` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,81 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2073 7068 696e 7863 6f6e 7472 6962   = sphinxcontrib
-00000020: 2d63 6f6e 666c 7565 6e63 6562 7569 6c64  -confluencebuild
-00000030: 6572 0d0a 7665 7273 696f 6e20 3d20 6174  er..version = at
-00000040: 7472 3a20 7370 6869 6e78 636f 6e74 7269  tr: sphinxcontri
-00000050: 622e 636f 6e66 6c75 656e 6365 6275 696c  b.confluencebuil
-00000060: 6465 722e 5f5f 7665 7273 696f 6e5f 5f0d  der.__version__.
-00000070: 0a0d 0a5b 7364 6973 745d 0d0a 6f77 6e65  ...[sdist]..owne
-00000080: 7220 3d20 726f 6f74 0d0a 6772 6f75 7020  r = root..group 
-00000090: 3d20 726f 6f74 0d0a 0d0a 5b6f 7074 696f  = root....[optio
-000000a0: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-000000b0: 6669 6e64 5f6e 616d 6573 7061 6365 3a0d  find_namespace:.
-000000c0: 0a74 6573 745f 7375 6974 6520 3d20 7465  .test_suite = te
-000000d0: 7374 730d 0a69 6e73 7461 6c6c 5f72 6571  sts..install_req
-000000e0: 7569 7265 7320 3d20 0d0a 0972 6571 7565  uires = ...reque
-000000f0: 7374 733e 3d32 2e31 342e 300d 0a09 7370  sts>=2.14.0...sp
-00000100: 6869 6e78 3e3d 342e 330d 0a0d 0a5b 6f70  hinx>=4.3....[op
-00000110: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-00000120: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-00000130: 6970 7473 203d 200d 0a09 7370 6869 6e78  ipts = ...sphinx
-00000140: 2d62 7569 6c64 2d63 6f6e 666c 7565 6e63  -build-confluenc
-00000150: 6520 3d20 7370 6869 6e78 636f 6e74 7269  e = sphinxcontri
-00000160: 622e 636f 6e66 6c75 656e 6365 6275 696c  b.confluencebuil
-00000170: 6465 722e 5f5f 6d61 696e 5f5f 3a6d 6169  der.__main__:mai
-00000180: 6e0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  n....[options.pa
-00000190: 636b 6167 6573 2e66 696e 645d 0d0a 696e  ckages.find]..in
-000001a0: 636c 7564 6520 3d20 7370 6869 6e78 636f  clude = sphinxco
-000001b0: 6e74 7269 622a 0d0a 0d0a 5b63 6f6d 7069  ntrib*....[compi
-000001c0: 6c65 5f63 6174 616c 6f67 5d0d 0a64 6f6d  le_catalog]..dom
-000001d0: 6169 6e20 3d20 7370 6869 6e78 636f 6e74  ain = sphinxcont
-000001e0: 7269 622e 636f 6e66 6c75 656e 6365 6275  rib.confluencebu
-000001f0: 696c 6465 720d 0a64 6972 6563 746f 7279  ilder..directory
-00000200: 203d 2073 7068 696e 7863 6f6e 7472 6962   = sphinxcontrib
-00000210: 2f63 6f6e 666c 7565 6e63 6562 7569 6c64  /confluencebuild
-00000220: 6572 2f6c 6f63 616c 652f 0d0a 0d0a 5b65  er/locale/....[e
-00000230: 7874 7261 6374 5f6d 6573 7361 6765 735d  xtract_messages]
-00000240: 0d0a 6b65 7977 6f72 6473 203d 204c 2043  ..keywords = L C
-00000250: 0d0a 6d61 7070 696e 675f 6669 6c65 203d  ..mapping_file =
-00000260: 2062 6162 656c 2e63 6667 0d0a 6e6f 5f64   babel.cfg..no_d
-00000270: 6566 6175 6c74 5f6b 6579 776f 7264 7320  efault_keywords 
-00000280: 3d20 5472 7565 0d0a 6f6d 6974 5f68 6561  = True..omit_hea
-00000290: 6465 7220 3d20 5472 7565 0d0a 6f75 7470  der = True..outp
-000002a0: 7574 5f66 696c 6520 3d20 7370 6869 6e78  ut_file = sphinx
-000002b0: 636f 6e74 7269 622f 636f 6e66 6c75 656e  contrib/confluen
-000002c0: 6365 6275 696c 6465 722f 6c6f 6361 6c65  cebuilder/locale
-000002d0: 2f73 7068 696e 7863 6f6e 7472 6962 2e63  /sphinxcontrib.c
-000002e0: 6f6e 666c 7565 6e63 6562 7569 6c64 6572  onfluencebuilder
-000002f0: 2e70 6f74 0d0a 0d0a 5b69 6e69 745f 6361  .pot....[init_ca
-00000300: 7461 6c6f 675d 0d0a 646f 6d61 696e 203d  talog]..domain =
-00000310: 2073 7068 696e 7863 6f6e 7472 6962 2e63   sphinxcontrib.c
-00000320: 6f6e 666c 7565 6e63 6562 7569 6c64 6572  onfluencebuilder
-00000330: 0d0a 696e 7075 745f 6669 6c65 203d 2073  ..input_file = s
-00000340: 7068 696e 7863 6f6e 7472 6962 2f63 6f6e  phinxcontrib/con
-00000350: 666c 7565 6e63 6562 7569 6c64 6572 2f6c  fluencebuilder/l
-00000360: 6f63 616c 652f 7370 6869 6e78 636f 6e74  ocale/sphinxcont
-00000370: 7269 622e 636f 6e66 6c75 656e 6365 6275  rib.confluencebu
-00000380: 696c 6465 722e 706f 740d 0a6f 6d69 745f  ilder.pot..omit_
-00000390: 6865 6164 6572 203d 2054 7275 650d 0a6f  header = True..o
-000003a0: 7574 7075 745f 6469 7220 3d20 7370 6869  utput_dir = sphi
-000003b0: 6e78 636f 6e74 7269 622f 636f 6e66 6c75  nxcontrib/conflu
-000003c0: 656e 6365 6275 696c 6465 722f 6c6f 6361  encebuilder/loca
-000003d0: 6c65 2f0d 0a0d 0a5b 7570 6461 7465 5f63  le/....[update_c
-000003e0: 6174 616c 6f67 5d0d 0a64 6f6d 6169 6e20  atalog]..domain 
-000003f0: 3d20 7370 6869 6e78 636f 6e74 7269 622e  = sphinxcontrib.
-00000400: 636f 6e66 6c75 656e 6365 6275 696c 6465  confluencebuilde
-00000410: 720d 0a69 6e70 7574 5f66 696c 6520 3d20  r..input_file = 
-00000420: 7370 6869 6e78 636f 6e74 7269 622f 636f  sphinxcontrib/co
-00000430: 6e66 6c75 656e 6365 6275 696c 6465 722f  nfluencebuilder/
-00000440: 6c6f 6361 6c65 2f73 7068 696e 7863 6f6e  locale/sphinxcon
-00000450: 7472 6962 2e63 6f6e 666c 7565 6e63 6562  trib.confluenceb
-00000460: 7569 6c64 6572 2e70 6f74 0d0a 6f6d 6974  uilder.pot..omit
-00000470: 5f68 6561 6465 7220 3d20 5472 7565 0d0a  _header = True..
-00000480: 6f75 7470 7574 5f64 6972 203d 2073 7068  output_dir = sph
-00000490: 696e 7863 6f6e 7472 6962 2f63 6f6e 666c  inxcontrib/confl
-000004a0: 7565 6e63 6562 7569 6c64 6572 2f6c 6f63  uencebuilder/loc
-000004b0: 616c 652f 0d0a 0d0a 5b65 6767 5f69 6e66  ale/....[egg_inf
-000004c0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000004d0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004e0: 0d0a                                     ..
+00000000: 6d73 6769 6420 2222 0d0a 6d73 6773 7472  msgid ""..msgstr
+00000010: 2022 220d 0a22 506c 7572 616c 2d46 6f72   "".."Plural-For
+00000020: 6d73 3a20 6e70 6c75 7261 6c73 3d31 3b20  ms: nplurals=1; 
+00000030: 706c 7572 616c 3d30 3b5c 6e22 0d0a 2258  plural=0;\n".."X
+00000040: 2d43 726f 7764 696e 2d50 726f 6a65 6374  -Crowdin-Project
+00000050: 3a20 7370 6869 6e78 636f 6e74 7269 622d  : sphinxcontrib-
+00000060: 636f 6e66 6c75 656e 6365 6275 696c 6465  confluencebuilde
+00000070: 725c 6e22 0d0a 2258 2d43 726f 7764 696e  r\n".."X-Crowdin
+00000080: 2d50 726f 6a65 6374 2d49 443a 2035 3538  -Project-ID: 558
+00000090: 3638 355c 6e22 0d0a 2258 2d43 726f 7764  685\n".."X-Crowd
+000000a0: 696e 2d4c 616e 6775 6167 653a 206a 615c  in-Language: ja\
+000000b0: 6e22 0d0a 2258 2d43 726f 7764 696e 2d46  n".."X-Crowdin-F
+000000c0: 696c 653a 2073 7068 696e 7863 6f6e 7472  ile: sphinxcontr
+000000d0: 6962 2e63 6f6e 666c 7565 6e63 6562 7569  ib.confluencebui
+000000e0: 6c64 6572 2e70 6f74 5c6e 220d 0a22 582d  lder.pot\n".."X-
+000000f0: 4372 6f77 6469 6e2d 4669 6c65 2d49 443a  Crowdin-File-ID:
+00000100: 2033 5c6e 220d 0a22 5072 6f6a 6563 742d   3\n".."Project-
+00000110: 4964 2d56 6572 7369 6f6e 3a20 7370 6869  Id-Version: sphi
+00000120: 6e78 636f 6e74 7269 622d 636f 6e66 6c75  nxcontrib-conflu
+00000130: 656e 6365 6275 696c 6465 725c 6e22 0d0a  encebuilder\n"..
+00000140: 2243 6f6e 7465 6e74 2d54 7970 653a 2074  "Content-Type: t
+00000150: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
+00000160: 6574 3d55 5446 2d38 5c6e 220d 0a22 4c61  et=UTF-8\n".."La
+00000170: 6e67 7561 6765 2d54 6561 6d3a 204a 6170  nguage-Team: Jap
+00000180: 616e 6573 655c 6e22 0d0a 224c 616e 6775  anese\n".."Langu
+00000190: 6167 653a 206a 615f 4a50 5c6e 220d 0a22  age: ja_JP\n".."
+000001a0: 504f 2d52 6576 6973 696f 6e2d 4461 7465  PO-Revision-Date
+000001b0: 3a20 3230 3233 2d30 312d 3032 2031 383a  : 2023-01-02 18:
+000001c0: 3536 5c6e 220d 0a0d 0a23 3a20 7370 6869  56\n"....#: sphi
+000001d0: 6e78 636f 6e74 7269 622f 636f 6e66 6c75  nxcontrib/conflu
+000001e0: 656e 6365 6275 696c 6465 722f 7369 6e67  encebuilder/sing
+000001f0: 6c65 6275 696c 6465 722e 7079 3a38 310d  lebuilder.py:81.
+00000200: 0a6d 7367 6964 2022 6173 7365 6d62 6c69  .msgid "assembli
+00000210: 6e67 2073 696e 676c 6520 636f 6e66 6c75  ng single conflu
+00000220: 656e 6365 2064 6f63 756d 656e 7422 0d0a  ence document"..
+00000230: 6d73 6773 7472 2022 220d 0a0d 0a23 3a20  msgstr ""....#: 
+00000240: 7370 6869 6e78 636f 6e74 7269 622f 636f  sphinxcontrib/co
+00000250: 6e66 6c75 656e 6365 6275 696c 6465 722f  nfluencebuilder/
+00000260: 7369 6e67 6c65 6275 696c 6465 722e 7079  singlebuilder.py
+00000270: 3a31 3130 0d0a 6d73 6769 6420 2277 7269  :110..msgid "wri
+00000280: 7469 6e67 2073 696e 676c 6520 636f 6e66  ting single conf
+00000290: 6c75 656e 6365 2064 6f63 756d 656e 7422  luence document"
+000002a0: 0d0a 6d73 6773 7472 2022 220d 0a0d 0a23  ..msgstr ""....#
+000002b0: 3a20 7370 6869 6e78 636f 6e74 7269 622f  : sphinxcontrib/
+000002c0: 636f 6e66 6c75 656e 6365 6275 696c 6465  confluencebuilde
+000002d0: 722f 7374 6f72 6167 652f 7465 6d70 6c61  r/storage/templa
+000002e0: 7465 732f 646f 6d61 696e 696e 6465 782e  tes/domainindex.
+000002f0: 6874 6d6c 3a31 310d 0a23 3a20 7370 6869  html:11..#: sphi
+00000300: 6e78 636f 6e74 7269 622f 636f 6e66 6c75  nxcontrib/conflu
+00000310: 656e 6365 6275 696c 6465 722f 7374 6f72  encebuilder/stor
+00000320: 6167 652f 7465 6d70 6c61 7465 732f 646f  age/templates/do
+00000330: 6d61 696e 696e 6465 785f 7632 2e68 746d  mainindex_v2.htm
+00000340: 6c3a 3131 0d0a 233a 2073 7068 696e 7863  l:11..#: sphinxc
+00000350: 6f6e 7472 6962 2f63 6f6e 666c 7565 6e63  ontrib/confluenc
+00000360: 6562 7569 6c64 6572 2f73 746f 7261 6765  ebuilder/storage
+00000370: 2f74 656d 706c 6174 6573 2f67 656e 696e  /templates/genin
+00000380: 6465 782e 6874 6d6c 3a33 370d 0a23 3a20  dex.html:37..#: 
+00000390: 7370 6869 6e78 636f 6e74 7269 622f 636f  sphinxcontrib/co
+000003a0: 6e66 6c75 656e 6365 6275 696c 6465 722f  nfluencebuilder/
+000003b0: 7374 6f72 6167 652f 7465 6d70 6c61 7465  storage/template
+000003c0: 732f 6765 6e69 6e64 6578 5f76 322e 6874  s/genindex_v2.ht
+000003d0: 6d6c 3a33 370d 0a23 3a20 7370 6869 6e78  ml:37..#: sphinx
+000003e0: 636f 6e74 7269 622f 636f 6e66 6c75 656e  contrib/confluen
+000003f0: 6365 6275 696c 6465 722f 7374 6f72 6167  cebuilder/storag
+00000400: 652f 7465 6d70 6c61 7465 732f 7365 6172  e/templates/sear
+00000410: 6368 2e68 746d 6c3a 3130 0d0a 233a 2073  ch.html:10..#: s
+00000420: 7068 696e 7863 6f6e 7472 6962 2f63 6f6e  phinxcontrib/con
+00000430: 666c 7565 6e63 6562 7569 6c64 6572 2f73  fluencebuilder/s
+00000440: 746f 7261 6765 2f74 7261 6e73 6c61 746f  torage/translato
+00000450: 722e 7079 3a32 3239 390d 0a6d 7367 6964  r.py:2299..msgid
+00000460: 2022 5468 6973 2070 6167 6520 6861 7320   "This page has 
+00000470: 6265 656e 2061 7574 6f6d 6174 6963 616c  been automatical
+00000480: 6c79 2067 656e 6572 6174 6564 2e22 0d0a  ly generated."..
+00000490: 6d73 6773 7472 2022 220d 0a0d 0a23 3a20  msgstr ""....#: 
+000004a0: 7370 6869 6e78 636f 6e74 7269 622f 636f  sphinxcontrib/co
+000004b0: 6e66 6c75 656e 6365 6275 696c 6465 722f  nfluencebuilder/
+000004c0: 7374 6f72 6167 652f 7472 616e 736c 6174  storage/translat
+000004d0: 6f72 2e70 793a 3233 3233 0d0a 6d73 6769  or.py:2323..msgi
+000004e0: 6420 2245 6469 7420 536f 7572 6365 220d  d "Edit Source".
+000004f0: 0a6d 7367 7374 7220 22e3 82bd e383 bce3  .msgstr ".......
+00000500: 82b9 e382 92e7 b7a8 e99b 8622 0d0a 0d0a  ..........."....
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from os import path
 from sphinx.util import docutils
 from sphinxcontrib.confluencebuilder.builder import ConfluenceBuilder
 from sphinxcontrib.confluencebuilder.config import handle_config_inited
 from sphinxcontrib.confluencebuilder.config.manager import ConfigManager
+from sphinxcontrib.confluencebuilder.directives import ConfluenceDocDirective
 from sphinxcontrib.confluencebuilder.directives import ConfluenceExcerptDirective
 from sphinxcontrib.confluencebuilder.directives import ConfluenceExcerptIncludeDirective
 from sphinxcontrib.confluencebuilder.directives import ConfluenceExpandDirective
 from sphinxcontrib.confluencebuilder.directives import ConfluenceLatexDirective
+from sphinxcontrib.confluencebuilder.directives import ConfluenceLinkDirective
 from sphinxcontrib.confluencebuilder.directives import ConfluenceMetadataDirective
 from sphinxcontrib.confluencebuilder.directives import ConfluenceNewline
 from sphinxcontrib.confluencebuilder.directives import ConfluenceToc
 from sphinxcontrib.confluencebuilder.directives import JiraDirective
 from sphinxcontrib.confluencebuilder.directives import JiraIssueDirective
 from sphinxcontrib.confluencebuilder.locale import MESSAGE_CATALOG_NAME
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger
 from sphinxcontrib.confluencebuilder.nodes import confluence_metadata
 from sphinxcontrib.confluencebuilder.nodes import jira
 from sphinxcontrib.confluencebuilder.nodes import jira_issue
 from sphinxcontrib.confluencebuilder.reportbuilder import ConfluenceReportBuilder
+from sphinxcontrib.confluencebuilder.roles import ConfluenceDocRole
 from sphinxcontrib.confluencebuilder.roles import ConfluenceEmoticonRole
 from sphinxcontrib.confluencebuilder.roles import ConfluenceLatexRole
+from sphinxcontrib.confluencebuilder.roles import ConfluenceLinkRole
 from sphinxcontrib.confluencebuilder.roles import ConfluenceMentionRole
 from sphinxcontrib.confluencebuilder.roles import ConfluenceStatusRole
+from sphinxcontrib.confluencebuilder.roles import ConfluenceStrikeRole
 from sphinxcontrib.confluencebuilder.roles import JiraRole
 from sphinxcontrib.confluencebuilder.singlebuilder import SingleConfluenceBuilder
 
 # load autosummary extension if available to add additional nodes
 try:
     from sphinx.ext import autosummary
 except ImportError:
@@ -39,15 +41,15 @@
 
 # load imgmath extension if available to handle math configuration options
 try:
     from sphinx.ext import imgmath
 except ImportError:
     imgmath = None
 
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 
 
 def setup(app):
     ConfluenceLogger.initialize()
     cm = app.config_manager_ = ConfigManager(app)
 
     app.require_sphinx('1.8')
@@ -117,28 +119,34 @@
     cm.add_conf_bool('confluence_ask_user')
     # Enablement of archiving legacy child pages.
     cm.add_conf_bool('confluence_cleanup_archive')
     # Enablement of cleaning legacy child pages from a root page.
     cm.add_conf_bool('confluence_cleanup_from_root')
     # Enablement of purging legacy child pages.
     cm.add_conf_bool('confluence_cleanup_purge')
+    # The mode to search for legacy child pages.
+    cm.add_conf('confluence_cleanup_search_mode')
     # Explicitly prevent auto-generation of titles for titleless documents.
     cm.add_conf_bool('confluence_disable_autogen_title')
     # Explicitly prevent page notifications on update.
     cm.add_conf_bool('confluence_disable_notifications')
     # Define a series of labels to apply to all published pages.
     cm.add_conf('confluence_global_labels')
     # Enablement of configuring root as space's homepage.
     cm.add_conf_bool('confluence_root_homepage')
     # Parent page's name or identifier to publish documents under.
     cm.add_conf('confluence_parent_page')
     # Perform a dry run of publishing to inspect what publishing will do.
     cm.add_conf_bool('confluence_publish_dryrun')
     # Publish only new content (no page updates, etc.).
     cm.add_conf_bool('confluence_publish_onlynew')
+    # Publish orphan pages to Confluence.
+    cm.add_conf_bool('confluence_publish_orphan')
+    # Container page to publish orphan pages under.
+    cm.add_conf_int('confluence_publish_orphan_container')
     # Postfix to apply to title of published pages.
     cm.add_conf('confluence_publish_postfix', 'env')
     # Prefix to apply to published pages.
     cm.add_conf('confluence_publish_prefix', 'env')
     # Root page's identifier to publish documents into.
     cm.add_conf_int('confluence_publish_root')
     # docname-2-title dictionary for title overrides.
@@ -177,14 +185,16 @@
     cm.add_conf('confluence_publish_allowlist')
     # Enable debugging for publish requests.
     cm.add_conf_bool('confluence_publish_debug')
     # Duration (in seconds) to delay each API request.
     cm.add_conf('confluence_publish_delay')
     # Subset of documents which are denied to be published.
     cm.add_conf('confluence_publish_denylist')
+    # Whether to check for changes on remote before publishing.
+    cm.add_conf_bool('confluence_publish_force')
     # Disable adding `rest/api` to REST requests.
     cm.add_conf_bool('confluence_publish_disable_api_prefix')
     # Header(s) to use for Confluence REST interaction.
     cm.add_conf('confluence_publish_headers')
     # Whether to publish a generated intersphinx database to the root document
     cm.add_conf_bool('confluence_publish_intersphinx')
     # Manipulate a requests instance.
@@ -215,16 +225,14 @@
     cm.add_conf('confluence_mentions', 'env')
     # Inject navigational hints into the documentation.
     cm.add_conf('confluence_navdocs_transform')
     # Remove a detected title from generated documents.
     cm.add_conf_bool('confluence_remove_title', 'env')
 
     # (configuration - undocumented)
-    # Enablement for aggressive descendents search (for cleanup).
-    cm.add_conf_bool('confluence_adv_aggressive_search')
     # Enablement for bulk archiving of packages (for premium environments).
     cm.add_conf_bool('confluence_adv_bulk_archiving')
     # Flag to permit the use of embedded certificates from requests.
     cm.add_conf_bool('confluence_adv_embedded_certs')
     # List of node types to ignore if no translator support exists.
     cm.add_conf('confluence_adv_ignore_nodes')
     # Unknown node handler dictionary for advanced integrations.
@@ -237,14 +245,16 @@
     cm.add_conf('confluence_adv_restricted', 'env')
     # Enablement of tracing processed data.
     cm.add_conf_bool('confluence_adv_trace_data')
     # Do not cap sections to a maximum of six (6) levels.
     cm.add_conf_bool('confluence_adv_writer_no_section_cap', 'env')
 
     # (configuration - deprecated)
+    # replaced by confluence_cleanup_search_mode
+    cm.add_conf_bool('confluence_adv_aggressive_search')
     # replaced by confluence_root_homepage
     cm.add_conf('confluence_master_homepage')
     # replaced by confluence_publish_allowlist
     cm.add_conf('confluence_publish_subset')
     # replaced by confluence_purge_from_root
     cm.add_conf_bool('confluence_purge_from_master')
     # replaced by confluence_cleanup_from_root
@@ -287,30 +297,35 @@
         app.add_node(confluence_metadata)
     if not docutils.is_node_registered(jira):
         app.add_node(jira)
     if not docutils.is_node_registered(jira_issue):
         app.add_node(jira_issue)
 
     # register directives
+    app.add_directive('confluence_doc', ConfluenceDocDirective)
     app.add_directive('confluence_excerpt', ConfluenceExcerptDirective)
     app.add_directive('confluence_excerpt_include',
         ConfluenceExcerptIncludeDirective)
     app.add_directive('confluence_expand', ConfluenceExpandDirective)
     app.add_directive('confluence_latex', ConfluenceLatexDirective)
+    app.add_directive('confluence_link', ConfluenceLinkDirective)
     app.add_directive('confluence_metadata', ConfluenceMetadataDirective)
     app.add_directive('confluence_newline', ConfluenceNewline)
     app.add_directive('confluence_toc', ConfluenceToc)
     app.add_directive('jira', JiraDirective)
     app.add_directive('jira_issue', JiraIssueDirective)
 
     # register roles
+    app.add_role('confluence_doc', ConfluenceDocRole)
     app.add_role('confluence_emoticon', ConfluenceEmoticonRole)
     app.add_role('confluence_latex', ConfluenceLatexRole)
+    app.add_role('confluence_link', ConfluenceLinkRole)
     app.add_role('confluence_mention', ConfluenceMentionRole)
     app.add_role('confluence_status', ConfluenceStatusRole)
+    app.add_role('confluence_strike', ConfluenceStrikeRole)
     app.add_role('jira', JiraRole)
 
     # inject compatible autosummary nodes if the extension is available/loaded
     if autosummary:
         for ext in app.extensions.values():
             if ext.name == 'sphinx.ext.autosummary':
                 app.registry.add_translation_handlers(
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/__main__.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinx.util.console import color_terminal
 from sphinx.util.console import nocolor  # pylint: disable=no-name-in-module
 from sphinxcontrib.confluencebuilder import __version__ as version
 from sphinxcontrib.confluencebuilder.cmd.build import build_main
 from sphinxcontrib.confluencebuilder.cmd.report import report_main
 from sphinxcontrib.confluencebuilder.cmd.wipe import wipe_main
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/assets.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2018-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from sphinx import addnodes
 from sphinx.util.osutil import canon_path
 from sphinx.util.images import guess_mimetype
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
@@ -83,25 +80,25 @@
             docname: the document's name to attach to
 
         Returns:
             the key, document name and path
         """
         logger.verbose('adding manual attachment: %s' % path)
         abspath = find_env_abspath(self.env, self.outdir, path)
-        return self._handle_entry(abspath, docname, True)
+        return self._handle_entry(abspath, docname, standalone=True)
 
     def build(self):
         """
         build a list of all assets tracked by the manager
 
         Returns a list of tuples for all asset entries tracked by this manager.
         A tuple entry will contain the following:
 
          - The key (or name) of the asset.
-         - The absolulte path of the asset on the system.
+         - The absolute path of the asset on the system.
          - The content-type value of the asset.
          - The hash value of the asset.
          - The name of the document this asset should be published to.
 
         Returns:
             the list of assets
         """
@@ -294,15 +291,15 @@
                 for rep in INVALID_CHARS:
                     key = key.replace(rep, '_')
 
                 filename, file_ext = os.path.splitext(key)
                 idx = 1
                 while key in self.keys:
                     idx += 1
-                    key = '{}_{}{}'.format(filename, idx, file_ext)
+                    key = f'{filename}_{idx}{file_ext}'
                 self.keys.add(key)
 
                 asset = ConfluenceAsset(key, path, type_, hash_)
                 self.assets.append(asset)
                 self.path2asset[path] = asset
                 if not hash_exists:
                     self.hash2asset[hash_] = asset
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/builder.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:copyright: Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
+# Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
 
 from collections import defaultdict
 from docutils import nodes
 from docutils.io import StringOutput
 from os import path
 from sphinx import addnodes
 from sphinx import version_info as sphinx_version_info
 from sphinx.builders import Builder
 from sphinx.locale import _ as SL
-from sphinx.util import status_iterator
 from sphinx.util.osutil import ensuredir
 from sphinxcontrib.confluencebuilder.assets import ConfluenceAssetManager
 from sphinxcontrib.confluencebuilder.assets import ConfluenceSupportedImages
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
+from sphinxcontrib.confluencebuilder.compat import status_iterator
 from sphinxcontrib.confluencebuilder.config import process_ask_configs
 from sphinxcontrib.confluencebuilder.config.checks import validate_configuration
 from sphinxcontrib.confluencebuilder.config.defaults import apply_defaults
 from sphinxcontrib.confluencebuilder.config.env import apply_env_overrides
 from sphinxcontrib.confluencebuilder.intersphinx import build_intersphinx
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger
 from sphinxcontrib.confluencebuilder.nodes import confluence_footer
@@ -37,47 +34,49 @@
 from sphinxcontrib.confluencebuilder.storage.translator import ConfluenceStorageFormatTranslator
 from sphinxcontrib.confluencebuilder.transmute import doctree_transmute
 from sphinxcontrib.confluencebuilder.util import ConfluenceUtil
 from sphinxcontrib.confluencebuilder.util import extract_strings_from_file
 from sphinxcontrib.confluencebuilder.util import first
 from sphinxcontrib.confluencebuilder.util import handle_cli_file_subset
 from sphinxcontrib.confluencebuilder.writer import ConfluenceWriter
-import io
 import os
+import tempfile
 
 
 class ConfluenceBuilder(Builder):
     allow_parallel = True
     default_translator_class = ConfluenceStorageFormatTranslator
     name = 'confluence'
     format = 'confluence_storage'
     supported_image_types = ConfluenceSupportedImages()
+    supported_linkcode = True
     supported_remote_images = True
 
     def __init__(self, app, env=None):
         # As of Sphinx v5.1.0, builders will accept an `env` option to
         # configure against an environment (over later having an environment
         # assigned.
         if sphinx_version_info >= (5, 1):
             # pylint: disable=too-many-function-args
-            super(ConfluenceBuilder, self).__init__(app, env)
+            super().__init__(app, env)
             # pylint: enable=too-many-function-args
         else:
-            super(ConfluenceBuilder, self).__init__(app)
+            super().__init__(app)  # pylint: disable=E1120
 
         self.cache_doctrees = {}
         self.cloud = False
         self.domain_indices = {}
         self.file_suffix = '.conf'
         self.info = ConfluenceLogger.info
         self.link_suffix = None
         self.metadata = defaultdict(dict)
         self.nav_next = {}
         self.nav_prev = {}
         self.omitted_docnames = []
+        self.orphan_docnames = []
         self.publish_allowlist = None
         self.publish_denylist = None
         self.publish_docnames = []
         self.publisher = ConfluencePublisher()
         self.root_doc_page_id = None
         self.secnumbers = {}
         self.state = ConfluenceState
@@ -114,14 +113,26 @@
                 self.supported_image_types.register(type_)
 
         if 'graphviz_output_format' in self.config:
             self.graphviz_output_format = self.config['graphviz_output_format']
         else:
             self.graphviz_output_format = 'png'
 
+        # For users building with Windows and using `dvisvgm` from MiKTeX, the
+        # process may fail when dealing with temporary file locations that do
+        # not share a common partition as the output directory.
+        #
+        #  ERROR: Windows API error 87: The parameter is incorrect.
+        #
+        # The imgmath extension allows a builder to override where temporary
+        # files are build -- use this to hint to using a temporary directory
+        # on the same partition the output directory to help prevent issues.
+        self._imgmath_tempdir = tempfile.mkdtemp(
+            prefix='.imgmath-', dir=self.outdir)
+
         if self.config.confluence_publish:
             process_ask_configs(self.config)
 
         old_url = self.config.confluence_server_url
         new_url = ConfluenceUtil.normalize_base_url(old_url)
         if old_url != new_url:
             self.warn('normalizing confluence url from '
@@ -237,15 +248,15 @@
         # generate domain index information
         self.domain_indices = {}
         indices_config = self.config.confluence_domain_indices
         if indices_config and self.name != 'singleconfluence':
             for domain_name in sorted(self.env.domains):
                 domain = self.env.domains[domain_name]
                 for indexcls in domain.indices:
-                    indexname = '%s-%s' % (domain.name, indexcls.name)
+                    indexname = f'{domain.name}-{indexcls.name}'
 
                     if isinstance(indices_config, list):
                         if indexname not in indices_config:
                             continue
 
                     content, _ = indexcls(domain).generate()
                     if content:
@@ -255,22 +266,33 @@
         #
         # We'll temporarily override the environment's 'get_doctree' method to
         # allow this extension to manipulate the doctree for a document inside
         # the pre-writing stage to also take effect in the writing stage.
         self._original_get_doctree = self.env.get_doctree
         self.env.get_doctree = self._get_doctree
 
+        # TMPFIX: as of Sphinx v6.1.x, doctrees can be cached when first
+        # written, which can prevent manipulating them between the doctree
+        # (pickle) write state and re-reading them later (specifically, this
+        # extension's means of manipulation) -- for now, if we detect the
+        # environment is performing any doctree caching, clear the entire
+        # cache
+        if getattr(self.env, '_write_doc_doctree_cache', None):
+            self.env._write_doc_doctree_cache = {}
+
         # process the document structure of the root document, populating a
         # publish order to ensure parent pages are created first (when using
         # hierarchy mode)
         self.process_tree_structure(
             ordered_docnames, self.config.root_doc, traversed)
 
         # add orphans (if any) to the publish list
-        ordered_docnames.extend(x for x in docnames if x not in traversed)
+        if self.config.confluence_publish_orphan:
+            self.orphan_docnames = [x for x in docnames if x not in traversed]
+            ordered_docnames.extend(self.orphan_docnames)
 
         for docname in ordered_docnames:
             doctree = self.env.get_doctree(docname)
 
             # acquire title from override (if any), or parse first title entity
             if (self.config.confluence_title_overrides and
                     docname in self.config.confluence_title_overrides):
@@ -451,33 +473,41 @@
         destination = StringOutput(encoding='utf-8')
 
         self.writer.write(doctree, destination)
         outfilename = path.join(self.outdir, self.file_transform(docname))
         if self.writer.output is not None:
             ensuredir(path.dirname(outfilename))
             try:
-                with io.open(outfilename, 'w', encoding='utf-8') as file:
+                with open(outfilename, 'w', encoding='utf-8') as file:
                     if self.writer.output:
                         file.write(self.writer.output)
             except (IOError, OSError) as err:
-                self.warn('error writing file %s: %s' % (outfilename, err))
+                self.warn(f'error writing file {outfilename}: {err}')
 
     def publish_doc(self, docname, output):
         conf = self.config
         title = self.state.title(docname)
         is_root_doc = self.config.root_doc == docname
 
         parent_id = None
         if self.config.root_doc and self.config.confluence_page_hierarchy:
             if self.config.root_doc != docname:
                 parent = self.state.parent_docname(docname)
                 parent_id = self.state.upload_id(parent)
         if not parent_id:
             parent_id = self.parent_id
 
+            # if a custom orphan root has been configured and this is an orphan
+            # page, override the parent to publish under; either the provided
+            # orphan root ID or no parent (zero value)
+            orphan_root_id = conf.confluence_publish_orphan_container
+            if orphan_root_id is not None:
+                if docname in self.orphan_docnames:
+                    parent_id = orphan_root_id
+
         data = {
             'content': output,
             'labels': [],
         }
 
         if self.config.confluence_global_labels:
             data['labels'].extend(self.config.confluence_global_labels)
@@ -514,18 +544,23 @@
 
             # if no base identifier and dry running, ignore legacy page
             # searching as there is no initial root document to reference
             # against
             if (conf.confluence_cleanup_from_root and
                     conf.confluence_publish_dryrun and not baseid):
                 self.legacy_pages = []
-            elif self.config.confluence_adv_aggressive_search is True:
-                self.legacy_pages = self.publisher.get_descendants_compat(baseid)
             else:
-                self.legacy_pages = self.publisher.get_descendants(baseid)
+                self.legacy_pages = self.publisher.get_descendants(
+                    baseid, conf.confluence_cleanup_search_mode)
+
+            # remove any configured orphan root id from a cleanup check
+            orphan_root_id = str(conf.confluence_publish_orphan_container)
+            if conf.confluence_publish_orphan and orphan_root_id:
+                if orphan_root_id in self.legacy_pages:
+                    self.legacy_pages.remove(orphan_root_id)
 
             # only populate a list of possible legacy assets when a user is
             # configured to check or push assets to the target space
             asset_override = conf.confluence_asset_override
             if asset_override is None or asset_override:
                 for legacy_page in self.legacy_pages:
                     attachments = self.publisher.get_attachments(legacy_page)
@@ -658,15 +693,15 @@
 
             if not self._verbose:
                 self.info(' done')
 
         # build domain indexes
         if self.domain_indices:
             for indexname, indexdata in self.domain_indices.items():
-                self.info('generating index ({})...'.format(indexname),
+                self.info(f'generating index ({indexname})...',
                     nonl=(not self._verbose))
 
                 self._generate_special_document(indexname,
                     generate_storage_format_domainindex)
 
                 if not self._verbose:
                     self.info(' done')
@@ -693,20 +728,20 @@
                     verbosity=self._verbose):
                 if self._check_publish_skip(docname):
                     self.verbose(docname + ' skipped due to configuration')
                     continue
                 docfile = path.join(self.outdir, self.file_transform(docname))
 
                 try:
-                    with io.open(docfile, 'r', encoding='utf-8') as file:
+                    with open(docfile, 'r', encoding='utf-8') as file:
                         output = file.read()
                         self.publish_doc(docname, output)
 
                 except (IOError, OSError) as err:
-                    self.warn('error reading file %s: %s' % (docfile, err))
+                    self.warn(f'error reading file {docfile}: {err}')
 
             self.info('building intersphinx... ', nonl=(not self._verbose))
             build_intersphinx(self)
             self.info('done')
 
             if self.config.confluence_publish_intersphinx:
                 inv = path.join(self.outdir, 'objects.inv')
@@ -729,15 +764,15 @@
                     continue
 
                 try:
                     with open(absfile, 'rb') as file:
                         output = file.read()
                         self.publish_asset(key, docname, output, type_, hash_)
                 except (IOError, OSError) as err:
-                    self.warn('error reading asset %s: %s' % (key, err))
+                    self.warn(f'error reading asset {key}: {err}')
 
             self.publish_cleanup()
             self.publish_finalize()
 
     def cleanup(self):
         if self.publish:
             self.publisher.disconnect()
@@ -824,18 +859,18 @@
             self._cached_header_data = ''
             header_template_data = ''
 
             if self.config.confluence_header_file is not None:
                 fname = path.join(self.env.srcdir,
                     self.config.confluence_header_file)
                 try:
-                    with io.open(fname, encoding='utf-8') as file:
+                    with open(fname, encoding='utf-8') as file:
                         header_template_data = file.read() + '\n'
                 except (IOError, OSError) as err:
-                    self.warn('error reading file {}: {}'.format(fname, err))
+                    self.warn(f'error reading file {fname}: {err}')
 
                 # if no data is supplied, the file is plain text
                 if self.config.confluence_header_data is None:
                     self._cached_header_data = header_template_data
                 else:
                     self._cached_header_data = self.templates.render_string(
                         header_template_data,
@@ -846,31 +881,31 @@
             self._cached_footer_data = ''
             footer_template_data = ''
 
             if self.config.confluence_footer_file is not None:
                 fname = path.join(self.env.srcdir,
                     self.config.confluence_footer_file)
                 try:
-                    with io.open(fname, encoding='utf-8') as file:
+                    with open(fname, encoding='utf-8') as file:
                         footer_template_data = file.read() + '\n'
                 except (IOError, OSError) as err:
-                    self.warn('error reading file {}: {}'.format(fname, err))
+                    self.warn(f'error reading file {fname}: {err}')
 
                 # if no data is supplied, the file is plain text
                 if self.config.confluence_footer_data is None:
                     self._cached_footer_data = footer_template_data
                 else:
                     self._cached_header_data = self.templates.render_string(
                         footer_template_data,
                         self.config.confluence_footer_data)
 
         # generate/replace the document in the output directory
         fname = path.join(self.outdir, docname + self.file_suffix)
         try:
-            with io.open(fname, 'w', encoding='utf-8') as f:
+            with open(fname, 'w', encoding='utf-8') as f:
                 f.write(self._cached_header_data)
                 generator(self, docname, f)
                 f.write(self._cached_footer_data)
         except (IOError, OSError) as err:
             self.warn('error writing file %s: %s', docname, err)
 
     def _get_doctree(self, docname):
@@ -924,24 +959,27 @@
                 url_base = '{protocol}://{host}/{owner}/{repo}/'
 
                 source_type = sourcelink.get('type')
                 if source_type == 'bitbucket':
                     default_host = 'bitbucket.org'
                     default_view = 'view'
                     url = 'src/{version}/{container}{page}{suffix}?mode={view}'
+                elif source_type == 'codeberg':
+                    default_host = 'codeberg.org'
+                    url = 'src/{version}/{container}{page}{suffix}'
                 elif source_type == 'github':
                     default_host = 'github.com'
                     url = '{view}/{version}/{container}{page}{suffix}'
                 elif source_type == 'gitlab':
                     default_host = 'gitlab.com'
                     url = '{view}/{version}/{container}{page}{suffix}'
                 else:
                     # unsupported source type should not pass here after this
                     # extension's configuration check
-                    assert False
+                    raise AssertionError('unsupported source type')
 
                 sourcelink['url'] = url_base + url
 
             sourcelink.setdefault('container', '')
             sourcelink.setdefault('protocol', 'https')
             sourcelink.setdefault('host', default_host)
             sourcelink.setdefault('view', default_view)
@@ -1045,18 +1083,18 @@
                         if secnumber:
                             target = ('.'.join(map(str, secnumber)) +
                                 self.secnumber_suffix + target)
 
                     section_id = doc_used_names.get(target, 0)
                     doc_used_names[target] = section_id + 1
                     if section_id > 0:
-                        target = '{}.{}'.format(target, section_id)
+                        target = f'{target}.{section_id}'
 
                     for id_ in section_node['ids']:
-                        id_ = '{}#{}'.format(docname, id_)
+                        id_ = f'{docname}#{id_}'
                         self.state.register_target(id_, target)
 
     def _top_ref_check(self, node):
         """
         report if the provided node is consider a #top reference
 
         Allows an implementer extending this call to provide a hint if the
@@ -1081,15 +1119,15 @@
         doctitle = None
         title_element = self._find_title_element(doctree)
         if title_element:
             doctitle = title_element.astext()
 
         if not doctitle:
             if not self.config.confluence_disable_autogen_title:
-                doctitle = "autogen-{}".format(docname)
+                doctitle = f'autogen-{docname}'
                 if self.publish:
                     self.warn('document will be published using an '
                         'generated title value: {}'.format(docname))
             elif self.publish:
                 self.warn('document will not be published since it '
                     'has no title: {}'.format(docname))
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/build.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
+from contextlib import suppress
 from sphinx.application import Sphinx
 from sphinx.util.docutils import docutils_namespace
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 import os
 import sys
 
 #: default builder to invoke when one is not specified
@@ -50,18 +48,16 @@
     else:
         output_dir = os.path.join(work_dir, '_build', 'confluence')
     doctrees_dir = os.path.join(output_dir, '.doctrees')
     builder = args.action if args.action else DEFAULT_BUILDER
 
     verbosity = 0
     if args.verbose:
-        try:
+        with suppress(ValueError):
             verbosity = int(args.verbose)
-        except ValueError:
-            pass
 
     # run sphinx engine
     with docutils_namespace():
         app = Sphinx(
             work_dir,               # document sources
             work_dir,               # directory with configuration
             output_dir,             # output for generated documents
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/report.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from collections import OrderedDict
 from docutils import __version__ as docutils_version
 from requests import __version__ as requests_version
 from sphinx import __version__ as sphinx_version
 from sphinx.application import Sphinx
 from sphinx.util.docutils import docutils_namespace
@@ -186,15 +183,15 @@
                     for o in root.findall('version'):
                         info += '   version: ' + o.text + '\n'
                     for o in root.findall('buildNumber'):
                         info += '     build: ' + o.text + '\n'
                 else:
                     logger.error('bad response from server ({})'.format(
                         rsp.status_code))
-                    info += '   fetched: error ({})\n'.format(rsp.status_code)
+                    info += f'   fetched: error ({rsp.status_code})\n'
                     rv = 1
             except Exception:
                 sys.stdout.flush()
                 logger.error(traceback.format_exc())
                 info += 'failure to determine confluence data\n'
                 rv = 1
 
@@ -278,15 +275,15 @@
     print(' requests:', single_line_version(requests_version))
     print('  builder:', single_line_version(scb_version))
 
     print('')
     print('(configuration)')
     if config:
         for k, v in OrderedDict(sorted(config.items())).items():
-            print('{}: {}'.format(k, v))
+            print(f'{k}: {v}')
     else:
         print('~default configuration~')
 
     if configuration_load_issue:
         print('')
         print('(error loading configuration)')
         print(configuration_load_issue)
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/cmd/wipe.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/wipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinx.application import Sphinx
 from sphinx.locale import __
 from sphinx.util.docutils import docutils_namespace
 from sphinxcontrib.confluencebuilder.config import process_ask_configs
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.publisher import ConfluencePublisher
@@ -71,15 +68,14 @@
                     work_dir,            # directory with configuration
                     tmp_dir,             # output for built documents
                     tmp_dir,             # output for doctree files
                     'confluence',        # builder to execute
                     status=sys.stdout,   # sphinx status output
                     warning=sys.stderr)  # sphinx warning output
 
-                aggressive_search = app.config.confluence_adv_aggressive_search
                 dryrun = app.config.confluence_publish_dryrun
                 server_url = app.config.confluence_server_url
                 space_key = app.config.confluence_space_key
                 parent_ref = app.config.confluence_parent_page
 
                 # initialize the publisher (if permitted)
                 if app.config.confluence_publish:
@@ -127,18 +123,17 @@
     # user has confirmed; start an attempt to wipe
     publisher.connect()
 
     base_page_id = None
     if args.parent:
         base_page_id = publisher.get_base_page_id()
 
-    if aggressive_search:
-        legacy_pages = publisher.get_descendants_compat(base_page_id)
-    else:
-        legacy_pages = publisher.get_descendants(base_page_id)
+    # find all legacy pages; always search aggressive to prevent any Confluence
+    # caching issues/delays
+    legacy_pages = publisher.get_descendants(base_page_id, 'search-aggressive')
 
     print('         URL:', server_url)
     print('       Space:', space_key)
     if base_page_id:
         logger.note('       Pages: Child pages of ' + parent_ref)
     else:
         logger.note('       Pages: All Pages')
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/compat.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/compat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:copyright: Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
+# Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
 
 from docutils import __version_info__ as docutils_version_info
 from docutils import nodes
 from sphinx import addnodes
 from sphinx import version_info as sphinx_version_info
 from sphinx.locale import __
 from sphinx.util.nodes import inline_all_toctrees as sphinx_inline_all_toctrees
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from typing import cast
 
+# pylint: disable=no-name-in-module
+if sphinx_version_info >= (6, 1):
+    from sphinx.util.display import status_iterator  # noqa: F401
+    from sphinx.util.display import progress_message  # noqa: F401
+else:
+    from sphinx.util import status_iterator  # noqa: F401
+    from sphinx.util import progress_message  # noqa: F401
+# pylint: enable=no-name-in-module
+
 
 # use docutil's findall call over traverse (obsolete)
 def docutils_findall(doctree, *args, **kwargs):
     if docutils_version_info >= (0, 18, 1):
         return doctree.findall(*args, **kwargs)
     else:
         return doctree.traverse(*args, **kwargs)
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder import util
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceConfigurationError
 import sys
 
 
 def handle_config_inited(app, config):
@@ -28,14 +25,18 @@
     # copy over deprecated configuration names to new names (if any)
     legacy('confluence_publish_allowlist', 'confluence_publish_subset')
     legacy('confluence_cleanup_from_root', 'confluence_purge_from_master')
     legacy('confluence_cleanup_from_root', 'confluence_purge_from_root')
     legacy('confluence_root_homepage', 'confluence_master_homepage')
     legacy('confluence_space_key', 'confluence_space_name')
 
+    if getattr(config, 'confluence_adv_aggressive_search') is True:
+        if getattr(config, 'confluence_cleanup_search_mode') is None:
+            config['confluence_cleanup_search_mode'] = 'search-aggressive'
+
 
 def process_ask_configs(config):
     """
     process any ask-based configurations for a user
 
     A series of asking configurations can be set in a configuration, such as
     asking for a password on a command line. This call will help process through
@@ -49,17 +50,17 @@
     if config.confluence_ask_user:
         print('(request to accept username from interactive session)')
         print(' Instance: ' + config.confluence_server_url)
 
         default_user = config.confluence_server_user
         u_str = ''
         if default_user:
-            u_str = ' [{}]'.format(default_user)
+            u_str = f' [{default_user}]'
 
-        target_user = input(' User{}: '.format(u_str)) or default_user
+        target_user = input(f' User{u_str}: ') or default_user
         if not target_user:
             raise ConfluenceConfigurationError('no user provided')
 
         config.confluence_server_user = target_user
 
     if config.confluence_ask_password:
         print('(request to accept password from interactive session)')
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/checks.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.config.notifications import deprecated
 from sphinxcontrib.confluencebuilder.config.notifications import warnings
 from sphinxcontrib.confluencebuilder.config.validation import ConfigurationValidation
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceConfigurationError
 from sphinxcontrib.confluencebuilder.std.confluence import EDITORS
 from sphinxcontrib.confluencebuilder.util import handle_cli_file_subset
@@ -132,14 +129,33 @@
 
     # confluence_cleanup_purge
     validator.conf('confluence_cleanup_purge') \
              .bool()
 
     # ##################################################################
 
+    # confluence_cleanup_search_mode
+    try:
+        validator.conf('confluence_cleanup_search_mode').matching(
+            'direct',
+            'direct-aggressive',
+            'search',
+            'search-aggressive',
+        )
+    except ConfluenceConfigurationError as e:
+        raise ConfluenceConfigurationError('''\
+{msg}
+
+The option 'confluence_cleanup_search_mode' has been provided to override the
+default search method for page descendants. Accepted values include 'direct',
+'search' and '<mode>-aggressive'.
+'''.format(msg=e))
+
+    # ##################################################################
+
     if config.confluence_client_cert is not None:
         client_cert = config.confluence_client_cert
         if isinstance(client_cert, tuple):
             cert_files = client_cert
         else:
             cert_files = (client_cert, None)
 
@@ -528,14 +544,26 @@
 
     # confluence_publish_onlynew
     validator.conf('confluence_publish_onlynew') \
              .bool()
 
     # ##################################################################
 
+    # confluence_publish_orphan
+    validator.conf('confluence_publish_orphan') \
+             .bool()
+
+    # ##################################################################
+
+    # confluence_publish_orphan_container
+    validator.conf('confluence_publish_orphan_container') \
+             .int_()
+
+    # ##################################################################
+
     # confluence_publish_postfix
     validator.conf('confluence_publish_postfix') \
              .string()
 
     # ##################################################################
 
     # confluence_publish_prefix
@@ -619,14 +647,15 @@
 
     if config.confluence_sourcelink:
         sourcelink = config.confluence_sourcelink
 
         # check if a supported template type is provided
         supported_types = [
             'bitbucket',
+            'codeberg',
             'github',
             'gitlab',
         ]
         if 'type' in sourcelink:
             if sourcelink['type'] not in supported_types:
                 raise ConfluenceConfigurationError('''\
 unsupported type provided in confluence_sourcelink
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/defaults.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.util import str2bool
 
 
 # configures the default editor to publication
 #
 # The following configures the default editor to use for publication. The
@@ -39,14 +36,20 @@
 
     if conf.confluence_adv_ignore_nodes is None:
         conf.confluence_adv_ignore_nodes = []
 
     if conf.confluence_adv_restricted is None:
         conf.confluence_adv_restricted = []
 
+    if conf.confluence_cleanup_search_mode is None:
+        # the default is `search`, since on Confluence Server/DC; the `direct`
+        # mode may always fail since Confluence may not completely implement
+        # the API capability
+        conf.confluence_cleanup_search_mode = 'search'
+
     if conf.confluence_client_cert is not None:
         if not isinstance(conf.confluence_client_cert, tuple):
             conf.confluence_client_cert = (conf.confluence_client_cert, None)
 
     if conf.confluence_editor is None:
         conf.confluence_editor = DEFAULT_EDITOR
 
@@ -69,14 +72,17 @@
 
     if conf.confluence_page_hierarchy is None:
         conf.confluence_page_hierarchy = True
 
     if conf.confluence_publish_intersphinx is None:
         conf.confluence_publish_intersphinx = True
 
+    if conf.confluence_publish_orphan is None:
+        conf.confluence_publish_orphan = True
+
     if conf.confluence_remove_title is None:
         conf.confluence_remove_title = True
 
     if conf.confluence_secnumber_suffix is None:
         conf.confluence_secnumber_suffix = '. '
 
     if conf.confluence_sourcelink is None:
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/env.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.util import str2bool
 import os
 
 
 def apply_env_overrides(builder):
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/manager.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
-
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 class ConfigManager:
     def __init__(self, app):
         """
         configuration manager
 
         The goal of a configuration manager is to track Confluence-specific
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/notifications.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/notifications.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.std.confluence import EDITORS
 import mimetypes
 
 # dictionary of deprecated configuration entries and associated message
 DEPRECATED_CONFIGS = {
+    'confluence_adv_aggressive_search':
+        'use "confluence_cleanup_search_mode" instead',
     'confluence_adv_trace_data':
         'to be removed in a future version',
     'confluence_adv_writer_no_section_cap':
         'to be removed in a future version',
     'confluence_master_homepage':
         'use "confluence_root_homepage" instead',
     'confluence_max_doc_depth':
@@ -44,15 +43,15 @@
     """
 
     config = validator.config
 
     # inform users of a deprecated configuration being used
     for key, msg in DEPRECATED_CONFIGS.items():
         if config[key] is not None:
-            logger.warn('%s deprecated; %s' % (key, msg))
+            logger.warn(f'{key} deprecated; {msg}')
 
 
 def warnings(validator):
     """
     inform users of any warnings related to a configuration state
 
     This call will check if the provided configuration has any configurations
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/config/validation.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceConfigurationError
 from sphinxcontrib.confluencebuilder.util import extract_strings_from_file
 from sphinxcontrib.confluencebuilder.util import str2bool
 import os
 
 
@@ -162,15 +159,15 @@
 
             for docname in value:
                 if not any(
                         os.path.isfile(
                             os.path.join(self.env.srcdir, docname + suffix))
                         for suffix in self.config.source_suffix):
                     raise ConfluenceConfigurationError(
-                        '%s is missing document %s' % (self.key, docname))
+                        f'{self.key} is missing document {docname}')
 
         return self
 
     def docnames_from_file(self):
         """
         checks if a configuration is a collection of valid docnames from a file
 
@@ -197,15 +194,15 @@
             docnames = extract_strings_from_file(value)
             for docname in docnames:
                 if not any(
                         os.path.isfile(
                             os.path.join(self.env.srcdir, docname + suffix))
                         for suffix in self.config.source_suffix):
                     raise ConfluenceConfigurationError(
-                        '%s is missing document %s' % (self.key, docname))
+                        f'{self.key} is missing document {docname}')
 
         return self
 
     def file(self):
         """
         checks if a configuration is a valid file
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/directives.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/directives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils.parsers.rst import Directive
 from docutils.parsers.rst import directives
+from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
+from sphinxcontrib.confluencebuilder.nodes import confluence_doc_card
 from sphinxcontrib.confluencebuilder.nodes import confluence_expand
 from sphinxcontrib.confluencebuilder.nodes import confluence_excerpt
 from sphinxcontrib.confluencebuilder.nodes import confluence_excerpt_include
 from sphinxcontrib.confluencebuilder.nodes import confluence_latex_block
+from sphinxcontrib.confluencebuilder.nodes import confluence_link_card
 from sphinxcontrib.confluencebuilder.nodes import confluence_metadata
 from sphinxcontrib.confluencebuilder.nodes import confluence_newline
 from sphinxcontrib.confluencebuilder.nodes import confluence_toc
 from sphinxcontrib.confluencebuilder.nodes import jira
 from sphinxcontrib.confluencebuilder.nodes import jira_issue
 from uuid import UUID
 
@@ -38,14 +38,68 @@
                 label = label.strip()
                 if label:
                     data.append(label)
 
     return data
 
 
+class ConfluenceCardDirective(Directive):
+    has_content = False
+    option_spec = {
+        'card': lambda x: directives.choice(x, ('block', 'embed')),
+        'layout': lambda x: directives.choice(x, ('align-start', 'align-end',
+            'center', 'wrap-left', 'wrap-right')),
+        'width': directives.positive_int,
+    }
+    required_arguments = 1
+    final_argument_whitespace = True
+
+    def run(self):
+        node = self._build_card_node()
+        node.params['href'] = self.arguments[0]
+        warnings = []
+
+        card = self.options.get('card', None)
+        layout = self.options.get('layout', None)
+        width = self.options.get('width', None)
+
+        if card:
+            node.params['data-card-appearance'] = card
+
+        if layout and card == 'embed':
+            node.params['data-layout'] = layout
+        elif layout:
+            warnings.append('layout only allowed for embedded card')
+
+        if width and card == 'embed':
+            node.params['data-width'] = width
+        elif width:
+            warnings.append('width only allowed for embedded card')
+
+        for warning in warnings:
+            reporter = self.state.document.reporter
+            source, lineno = reporter.get_source_and_line(self.lineno)
+            logger.warn('%s:%s: %s', source, lineno, warning)
+
+        return [node]
+
+    def _build_card_node(self):
+        raise NotImplementedError()
+
+
+class ConfluenceDocDirective(ConfluenceCardDirective):
+    def _build_card_node(self):
+        return confluence_doc_card()
+
+
+class ConfluenceLinkDirective(ConfluenceCardDirective):
+    def _build_card_node(self):
+        return confluence_link_card()
+
+
 class ConfluenceExcerptDirective(Directive):
     has_content = True
     option_spec = {
         'atlassian-macro-output-type':
             lambda x: directives.choice(x, ('block', 'inline')),
         'hidden': lambda x: directives.choice(x, ('true', 'false')),
         'name': directives.unchanged,
@@ -127,15 +181,14 @@
 
 
 class ConfluenceMetadataDirective(Directive):
     has_content = False
     option_spec = {
         'labels': string_list,
     }
-    final_argument_whitespace = True
 
     def run(self):
         node = confluence_metadata()
 
         for k, v in self.options.items():
             node.params[kebab_case_to_camel_case(k)] = v
 
@@ -162,15 +215,14 @@
         'min-level': directives.positive_int,
         'outline': lambda x: directives.choice(x, ('true', 'false')),
         'printable': lambda x: directives.choice(x, ('true', 'false')),
         'separator': directives.unchanged,
         'style': directives.unchanged,
         'type': lambda x: directives.choice(x, ('flat', 'list')),
     }
-    final_argument_whitespace = True
 
     def run(self):
         node = confluence_toc()
 
         for k, v in self.options.items():
             node.params[kebab_case_to_camel_case(k)] = v
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/exceptions.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinx.errors import ConfigError
 from sphinx.errors import SphinxError
 
 
 class ConfluenceError(SphinxError):
     category = 'sphinxcontrib.confluencebuilder error'
 
 
 class ConfluenceAuthenticationFailedUrlError(ConfluenceError):
     def __init__(self):
-        super(ConfluenceAuthenticationFailedUrlError, self).__init__('''
+        super().__init__('''
 ---
 Unable to authenticate with Confluence
 
 Unable to authenticate with the Confluence instance. Ensure the
 configured username and password are correct. If credentials appear to
 be correct, the user may need to be unlocked be re-logging in with above
 browser or asking an administrator of the Confluence instance for help.
 ---
 ''')
 
 
 class ConfluenceBadApiError(ConfluenceError):
     def __init__(self, code, details):
-        super(ConfluenceBadApiError, self).__init__('''
+        super().__init__('''
 ---
 Unsupported Confluence API call
 
 An unsupported Confluence API call has been made. See the following
 details for more information:
 
 {details}
@@ -42,15 +39,15 @@
 
 
 class ConfluenceBadSpaceError(ConfluenceError):
     def __init__(self, space_key, uname, pw_set, token_set, extras):
         uname_value = uname if uname else '(empty)'
         pw_value = '<set>' if pw_set else '(empty)'
         token_value = '<set>' if token_set else '(empty)'
-        super(ConfluenceBadSpaceError, self).__init__('''
+        super().__init__('''
 ---
 Invalid Confluence URL detected
 
 The configured Confluence space key does not appear to be valid:
 
     Space key: {space_key}
      Username: {uname}
@@ -65,15 +62,15 @@
 ---
 '''.format(space_key=space_key, uname=uname_value, pw=pw_value,
         token=token_value, details=extras))
 
 
 class ConfluenceBadServerUrlError(ConfluenceError):
     def __init__(self, server_url, ex):
-        super(ConfluenceBadServerUrlError, self).__init__('''
+        super().__init__('''
 ---
 Invalid Confluence URL detected
 
 An issue has been detected when trying to communicate with the
 configured Confluence instance. Ensure the instance is running and
 inspect that the configured Confluence URL is valid:
 
@@ -82,15 +79,15 @@
 (details: {details})
 ---
 '''.format(url=server_url, details=ex))
 
 
 class ConfluenceCertificateError(ConfluenceError):
     def __init__(self, ex):
-        super(ConfluenceCertificateError, self).__init__('''
+        super().__init__('''
 ---
 SSL certificate issue
 
 An SSL issue has been detected when trying to load the configured
 certificates.
 
 (details: {details})
@@ -100,15 +97,15 @@
 
 class ConfluenceConfigurationError(ConfluenceError, ConfigError):
     pass
 
 
 class ConfluenceMissingPageIdError(ConfluenceError):
     def __init__(self, space_key, page_id):
-        super(ConfluenceMissingPageIdError, self).__init__('''
+        super().__init__('''
 ---
 Unable to find a requested page
 
 A request to publish to a specific Confluence page identifier has failed
 as the identifier could not be found.
 
       Space: {space_key}
@@ -116,28 +113,28 @@
 
 ---
 '''.format(space_key=space_key, page_id=page_id))
 
 
 class ConfluencePermissionError(ConfluenceError):
     def __init__(self, details):
-        super(ConfluencePermissionError, self).__init__('''
+        super().__init__('''
 ---
 Permission denied on Confluence ({desc})
 
 The configured user does not have permission to perform an action on the
 Confluence instance. If the user should have access and this request is
 using a personal access token, ensure the token is not expired/revoked.
 ---
 '''.format(desc=details))
 
 
 class ConfluenceProxyPermissionError(ConfluenceError):
     def __init__(self):
-        super(ConfluenceProxyPermissionError, self).__init__('''
+        super().__init__('''
 ---
 Unable to authenticate with the proxy server
 
 The proxy server being used is reporting that authentication is
 required. Verify that the credentials used for the system's proxy
 configuration are correct (this is unrelated to the configured
 Confluence username/password configurations).
@@ -147,15 +144,15 @@
 
 class ConfluencePublishCheckError(ConfluenceError):
     pass
 
 
 class ConfluencePublishAncestorError(ConfluencePublishCheckError):
     def __init__(self, page_name):
-        super(ConfluencePublishAncestorError, self).__init__('''
+        super().__init__('''
 ---
 Ancestor publish check failed for: {name}
 
 A request has been made to publish a page as a nested child of itself.
 This is most likely a result of an existing documentation set on a
 Confluence instance where a publish attempt is trying to push new pages
 into a parent page which has an ancestor with a matching name:
@@ -176,15 +173,15 @@
 please inform the maintainers of this extension.
 ---
 '''.format(name=page_name))
 
 
 class ConfluencePublishSelfAncestorError(ConfluencePublishCheckError):
     def __init__(self, page_name):
-        super(ConfluencePublishSelfAncestorError, self).__init__('''
+        super().__init__('''
 ---
 Ancestor (self) publish check failed for: {name}
 
 A request has been made to publish a page as a child of itself. This is
 most likely due to a configuration of `confluence_parent_page` with the
 same value of the title page for the documentation's `root_doc`. If this
 is the case and the configuration uses `confluence_page_hierarchy`,
@@ -197,43 +194,43 @@
 please inform the maintainers of this extension.
 ---
 '''.format(name=page_name))
 
 
 class ConfluenceRateLimited(ConfluenceError):
     def __init__(self):
-        super(ConfluenceRateLimited, self).__init__('''
+        super().__init__('''
 ---
 Request has been rate limited
 
 The configured Confluence instance is reporting that too many requests
 are being made and has instructed to client to limit the amount of
 requests to make at this time.
 ---
 ''')
 
 
 class ConfluenceSeraphAuthenticationFailedUrlError(ConfluenceError):
     def __init__(self):
-        super(ConfluenceSeraphAuthenticationFailedUrlError, self).__init__('''
+        super().__init__('''
 ---
 Unable to authenticate with the Confluence instance (Seraph)
 
 While this could be the configured username or password being incorrect,
 this plugin as detected that the Atlassian Seraph instance has logged
 this user out. This may be a result of a Confluence instance-related
 issue. If this persisted, try contacting an administrator of the
 Confluence instance for help.
 ---
 ''')
 
 
 class ConfluenceSslError(ConfluenceError):
     def __init__(self, server_url, ex):
-        super(ConfluenceSslError, self).__init__('''
+        super().__init__('''
 ---
 SSL connection issue has been detected
 
 An SSL issue has been detected when trying to communicate with the
 configured Confluence instance. Ensure the instance is running and
 inspect that the configured Confluence URL is valid:
 
@@ -248,15 +245,15 @@
 (details: {details})
 ---
 '''.format(url=server_url, details=ex))
 
 
 class ConfluenceTimeoutError(ConfluenceError):
     def __init__(self, server_url):
-        super(ConfluenceTimeoutError, self).__init__('''
+        super().__init__('''
 ---
 Connection has timed out
 
 A request to communicate with the configured Confluence instance has
 timed out. Ensure the instance is running and inspect that the
 configured Confluence URL is valid:
 
@@ -264,15 +261,15 @@
 
 ---
 '''.format(url=server_url))
 
 
 class ConfluenceUnreconciledPageError(ConfluenceError):
     def __init__(self, page_name, page_id, url, ex):
-        super(ConfluenceUnreconciledPageError, self).__init__('''
+        super().__init__('''
 ---
 Unable to update unreconciled page: {name} (id: {id})
 
 Unable to update the target page due to the Confluence instance
 reporting an unreconciled page. This is either due to a conflict with
 another instance updating the page, Confluence having trouble updating a
 large page request or possibly an old Confluence version
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/intersphinx.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/intersphinx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:copyright: Copyright 2007-2020 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
+# Copyright 2007-2020 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
 
 from os import path
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 import re
 import requests
 import zlib
 
@@ -35,43 +32,43 @@
     else:
         pages_part = 'pages/viewpage.action?pageId={}'
 
     with open(path.join(builder.outdir, INVENTORY_FILENAME), 'wb') as f:
         # header
         f.write((
             '# Sphinx inventory version 2\n'
-            '# Project: %s\n'
-            '# Version: %s\n'
-            '# The remainder of this file is compressed using zlib.\n' % (
+            '# Project: {}\n'
+            '# Version: {}\n'
+            '# The remainder of this file is compressed using zlib.\n'.format(
                 escape(builder.env.config.project),
                 escape(builder.env.config.version))).encode())
 
         # contents
         compressor = zlib.compressobj(9)
 
         for domainname, domain in sorted(builder.env.domains.items()):
             for name, dispname, typ, docname, raw_anchor, prio in sorted(
                     domain.get_objects()):
 
                 page_id = builder.state.upload_id(docname)
                 if not page_id:
                     continue
 
-                target_name = '{}#{}'.format(docname, raw_anchor)
+                target_name = f'{docname}#{raw_anchor}'
                 target = builder.state.target(target_name)
 
                 if raw_anchor and target:
                     title = builder.state.title(docname)
                     anchor = 'id-' + title + '-' + target
                     anchor = anchor.replace(' ', '')
 
                     # confluence will convert quotes to right-quotes for
                     # anchor values; replace and encode the anchor value
                     anchor = anchor.replace('"', '”')
-                    anchor = anchor.replace("'", '’')
+                    anchor = anchor.replace("'", '’')  # noqa: RUF001
                     anchor = requests.utils.quote(anchor.encode('utf-8'))
                 else:
                     anchor = ''
 
                 uri = pages_part.format(page_id)
                 if anchor:
                     uri += '#' + anchor
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Crowdin-Project: sphinxcontrib-confluencebuilder\n"
 "X-Crowdin-Project-ID: 558685\n"
-"X-Crowdin-Language: ja\n"
+"X-Crowdin-Language: sr-CS\n"
 "X-Crowdin-File: sphinxcontrib.confluencebuilder.pot\n"
 "X-Crowdin-File-ID: 3\n"
 "Project-Id-Version: sphinxcontrib-confluencebuilder\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language-Team: Japanese\n"
-"Language: ja_JP\n"
+"Language-Team: Serbian (Latin)\n"
+"Language: sr_CS\n"
 "PO-Revision-Date: 2023-01-02 18:56\n"
 
 #: sphinxcontrib/confluencebuilder/singlebuilder.py:81
 msgid "assembling single confluence document"
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/singlebuilder.py:110
@@ -27,9 +27,9 @@
 #: sphinxcontrib/confluencebuilder/storage/templates/search.html:10
 #: sphinxcontrib/confluencebuilder/storage/translator.py:2299
 msgid "This page has been automatically generated."
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/storage/translator.py:2323
 msgid "Edit Source"
-msgstr "ソースを編集"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Crowdin-Project: sphinxcontrib-confluencebuilder\n"
 "X-Crowdin-Project-ID: 558685\n"
-"X-Crowdin-Language: sr-CS\n"
+"X-Crowdin-Language: sv-SE\n"
 "X-Crowdin-File: sphinxcontrib.confluencebuilder.pot\n"
 "X-Crowdin-File-ID: 3\n"
 "Project-Id-Version: sphinxcontrib-confluencebuilder\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language-Team: Serbian (Latin)\n"
-"Language: sr_CS\n"
+"Language-Team: Swedish\n"
+"Language: sv_SE\n"
 "PO-Revision-Date: 2023-01-02 18:56\n"
 
 #: sphinxcontrib/confluencebuilder/singlebuilder.py:81
 msgid "assembling single confluence document"
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/singlebuilder.py:110
@@ -27,9 +27,9 @@
 #: sphinxcontrib/confluencebuilder/storage/templates/search.html:10
 #: sphinxcontrib/confluencebuilder/storage/translator.py:2299
 msgid "This page has been automatically generated."
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/storage/translator.py:2323
 msgid "Edit Source"
-msgstr ""
+msgstr "Redigera källa"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 msgid ""
 msgstr ""
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "X-Crowdin-Project: sphinxcontrib-confluencebuilder\n"
 "X-Crowdin-Project-ID: 558685\n"
-"X-Crowdin-Language: sv-SE\n"
+"X-Crowdin-Language: zh-TW\n"
 "X-Crowdin-File: sphinxcontrib.confluencebuilder.pot\n"
 "X-Crowdin-File-ID: 3\n"
 "Project-Id-Version: sphinxcontrib-confluencebuilder\n"
 "Content-Type: text/plain; charset=UTF-8\n"
-"Language-Team: Swedish\n"
-"Language: sv_SE\n"
+"Language-Team: Chinese Traditional\n"
+"Language: zh_TW\n"
 "PO-Revision-Date: 2023-01-02 18:56\n"
 
 #: sphinxcontrib/confluencebuilder/singlebuilder.py:81
 msgid "assembling single confluence document"
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/singlebuilder.py:110
@@ -27,9 +27,9 @@
 #: sphinxcontrib/confluencebuilder/storage/templates/search.html:10
 #: sphinxcontrib/confluencebuilder/storage/translator.py:2299
 msgid "This page has been automatically generated."
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/storage/translator.py:2323
 msgid "Edit Source"
-msgstr "Redigera källa"
+msgstr "編輯來源"
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/logger.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from collections import deque
+from contextlib import suppress
 from sphinx.util import logging
 from sphinx.util.console import bold  # pylint: disable=no-name-in-module
-import io
 import sys
 
 
 class ConfluenceLogger:
     """
     confluence logger class
 
@@ -40,18 +37,18 @@
         if preload:
             class MockSphinx:
                 def __init__(self):
                     self.messagelog = deque(maxlen=10)
                     self.verbosity = 0
                     self.warningiserror = False
                     self._warncount = 0
-            try:
+
+            # fail silently if mocked application is missing something
+            with suppress(Exception):
                 logging.setup(MockSphinx(), sys.stdout, sys.stderr)
-            except Exception:
-                pass  # fail silently if mocked application is missing something
 
     @staticmethod
     def error(msg, *args, **kwargs):
         """
         log an error message
 
         Log a message at the error level. `msg` is a format string with the
@@ -104,25 +101,26 @@
         log a warning message
 
         Log a message at the warning level. `msg` is a format string with the
         arguments provided by `args`. See also:
          https://docs.python.org/3/library/logging.html#logging.Logger.warning
         """
         if ConfluenceLogger.logger:
+            kwargs['type'] = 'confluence'
             ConfluenceLogger.logger.warning(msg, *args, **kwargs)
 
     @staticmethod
     def trace(container, data):
         """
         trace data for a given container name
 
         Traces data with a given container name by dumping the contents directly
         to a log file `trace.log`. The log file, if exists, will be appended.
         This is solely for manually debugging unexpected scenarios.
         """
         try:
-            with io.open('trace.log', 'a', encoding='utf-8') as file:
-                file.write(u'[%s]\n' % container)
+            with open('trace.log', 'a', encoding='utf-8') as file:
+                file.write('[%s]\n' % container)
                 file.write(data)
-                file.write(u'\n')
+                file.write('\n')
         except (IOError, OSError) as err:
             ConfluenceLogger.warn('unable to trace: %s' % err)
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/nodes.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2019-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 
 
 class ConfluenceParams(nodes.Element):
     """
     confluence parameter-holding node
@@ -24,14 +21,32 @@
         params: the tracked confluence parameters
     """
     def __init__(self, rawsource='', *children, **attributes):
         nodes.Element.__init__(self, rawsource, *children, **attributes)
         self.params = self.attributes.setdefault('confluence-params', {})
 
 
+class confluence_doc_card(nodes.Structural, ConfluenceParams):
+    """
+    confluence document card node
+
+    A Confluence builder defined document card node, used to help add
+    Confluence document-CARD for a block section.
+    """
+
+
+class confluence_doc_card_inline(nodes.Inline, ConfluenceParams):
+    """
+    confluence document card inline node
+
+    A Confluence builder defined document card inline node, used to help add
+    Confluence document-CARD for an inlined section of a paragraph.
+    """
+
+
 class confluence_emoticon_inline(nodes.Inline, nodes.TextElement):
     """
     confluence emoticon inline node
 
     A Confluence builder defined emoticon inline node, used to help manage
     emoticon content designed for an inlined section of a paragraph.
     """
@@ -117,14 +132,32 @@
     confluence latex inline node
 
     A Confluence builder defined LaTeX inline node, used to help manage LaTeX
     content designed for an inlined section of a paragraph.
     """
 
 
+class confluence_link_card(nodes.Structural, ConfluenceParams):
+    """
+    confluence link card node
+
+    A Confluence builder defined link card node, used to help add
+    Confluence link-CARD for a block section.
+    """
+
+
+class confluence_link_card_inline(nodes.Inline, ConfluenceParams):
+    """
+    confluence card inline node
+
+    A Confluence builder defined inline card node, used to help add
+    Confluence link-CARD for an inlined section of a paragraph.
+    """
+
+
 class confluence_mention_inline(nodes.Inline, nodes.TextElement):
     """
     confluence mention inline node
 
     A Confluence builder defined mention inline node, used to help add
     Confluence @mentions for an inlined section of a paragraph.
     """
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/publisher.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/publisher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
+"""
 See also:
     Confluence Cloud REST API Reference
     https://docs.atlassian.com/confluence/REST/latest/
 """
 
 from sphinx.util.logging import skip_warningiserror
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadApiError
@@ -16,19 +15,24 @@
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceMissingPageIdError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePermissionError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePublishAncestorError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePublishSelfAncestorError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceUnreconciledPageError
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.rest import Rest
+from sphinxcontrib.confluencebuilder.util import ConfluenceUtil
 import json
 import logging
 import time
 
 
+# key used for managing this extension's properties on a Confluence instance
+PROP_KEY = 'sphinx'
+
+
 class ConfluencePublisher:
     def __init__(self):
         self.cloud = None
         self.editor = None
         self.space_display_name = None
         self.space_type = None
         self._ancestors_cache = set()
@@ -63,15 +67,15 @@
     def connect(self):
         self.rest_client = Rest(self.config)
         server_url = self.config.confluence_server_url
 
         try:
             rsp = self.rest_client.get('space', {
                 'spaceKey': self.space_key,
-                'limit': 1
+                'limit': 1,
             })
         except ConfluenceBadApiError as e:
             raise ConfluenceBadServerUrlError(server_url, e)
 
         # if no size entry is provided, this a non-Confluence API server
         if 'size' not in rsp:
             raise ConfluenceBadServerUrlError(server_url,
@@ -170,15 +174,15 @@
 
             # wait for the archiving of the page to complete
             MAX_WAIT_FOR_PAGE_ARCHIVE = 4  # ~2 seconds
             attempt = 1
             while attempt <= MAX_WAIT_FOR_PAGE_ARCHIVE:
                 time.sleep(0.5)
 
-                rsp = self.rest_client.get('longtask/{}'.format(longtask_id))
+                rsp = self.rest_client.get(f'longtask/{longtask_id}')
                 if rsp['finished']:
                     break
 
                 attempt += 1
                 if attempt > MAX_WAIT_FOR_PAGE_ARCHIVE:
                     raise ConfluenceBadApiError(
                         -1, 'timeout waiting for archive completion')
@@ -255,15 +259,15 @@
 
             return base_page_id
 
         rsp = self.rest_client.get('content', {
             'type': 'page',
             'spaceKey': self.space_key,
             'title': self.parent_ref,
-            'status': 'current'
+            'status': 'current',
         })
         if rsp['size'] == 0:
             raise ConfluenceConfigurationError(
                 '''Configured parent page name does not exist.''')
         page = rsp['results'][0]
         if self.parent_id and page['id'] != str(self.parent_id):
             raise ConfluenceConfigurationError("""Configured parent """
@@ -273,58 +277,115 @@
 
         if not base_page_id and self.parent_id:
             raise ConfluenceConfigurationError("""Unable to find the """
                 """parent page matching the ID or name provided.""")
 
         return base_page_id
 
-    def get_descendants(self, page_id):
+    def get_descendants(self, page_id, mode):
         """
         generate a list of descendants
 
         Queries the configured Confluence instance for a set of descendants for
         the provided `page_id` or (if set to `None`) the configured space.
 
+        There are a series of modes supported by this call:
+
+        - `direct`
+            Descendants will be queried for by asking Confluence the list of
+            descendants by looking at the content data cached for the specified
+            page/space. In theory, this should be the proper/fastest call to
+            use. However, it has been observed in some scenarios that not all
+            descendants will be listed (depending on the version of Confluence,
+            possible caching, etc.).
+
+        - `search`
+            Descendants will be queried for by asking Confluence the list of
+            descendants by performing a CQL search for descendants of a
+            specified page/space. This method of searching for descendants is
+            available since it appeared to provide more consistent results in
+            earlier versions of Confluence. However, this method (in the
+            same manner for `direct`), may be missing some descendants
+            (depending on the version of Confluence, possible caching, etc.).
+
+        - `<mode>-aggressive`
+            Descendants will be queried in the same manner as the specied mode
+            type, with the addition that for each page found, an additional
+            fetching will be performed to check for descendants for a found
+            descendant. Querying stops when all descendants have been fetched
+            on. This method of searching provides the most consistent results in
+            populating known descendants. However, this call significantly
+            increases the amount of API calls performed.
+
         Args:
             page_id: the ancestor to search on (if not `None`)
+            mode: the mode to search for descendants
 
         Returns:
             the descendants
         """
+
+        if 'aggressive' in mode:
+            descendants = self._get_descendants_aggressive(page_id, mode)
+        else:
+            descendants = self._get_descendants(page_id, mode)
+
+        return descendants
+
+    def _get_descendants(self, page_id, mode):
+        """
+        generate a list of descendants
+
+        Queries the configured Confluence instance for a set of descendants for
+        the provided `page_id` or (if set to `None`) the configured space.
+
+        Args:
+            page_id: the ancestor to search on (if not `None`)
+            mode: the mode to search for descendants
+
+        Returns:
+            the descendants
+        """
+
+        api_endpoint = 'content/search'
         descendants = set()
+        search_fields = {}
 
         if page_id:
-            search_fields = {'cql': 'ancestor=' + str(page_id)}
+            if 'direct' in mode:
+                api_endpoint = f'content/{page_id}/descendant/page'
+            else:
+                search_fields['cql'] = f'ancestor={page_id}'
         else:
-            search_fields = {'cql': 'space="' + self.space_key +
-                '" and type=page'}
+            # always use search if no page id was provided (e.g. a space search)
+            search_fields['cql'] = f'space="{self.space_key}" and type=page'
 
         # Configure a larger limit value than the default (no provided
         # limit defaults to 25). This should reduce the number of queries
         # needed to fetch a complete descendants set (for larger sets).
         search_fields['limit'] = 1000
 
-        rsp = self.rest_client.get('content/search', search_fields)
+        rsp = self.rest_client.get(api_endpoint, search_fields)
         idx = 0
         while rsp['size'] > 0:
             for result in rsp['results']:
                 descendants.add(result['id'])
                 self._name_cache[result['id']] = result['title']
 
             if rsp['size'] != rsp['limit']:
                 break
 
             idx += int(rsp['limit'])
             sub_search_fields = dict(search_fields)
             sub_search_fields['start'] = idx
-            rsp = self.rest_client.get('content/search', sub_search_fields)
+            rsp = self.rest_client.get(api_endpoint, sub_search_fields)
 
         return descendants
 
-    def get_descendants_compat(self, page_id):
+    def _get_descendants_aggressive(self, page_id, mode):
         """
         generate a list of descendants (aggressive)
 
         Queries the configured Confluence instance for a set of descendants for
         the provided `page_id` or (if set to `None`) the configured space. This
         request is a more aggressive search for descendants when compared to
         `getDescendants`. Each page found will be again searched on for
@@ -332,22 +393,23 @@
         does not provide a complete set of descendants (this has been observed
         on some instances of Confluence server; speculated to be possible
         cache corruption). This search can be extremely slow for large document
         sets.
 
         Args:
             page_id: the ancestor to search on (if not `None`)
+            mode: the mode to search for descendants
 
         Returns:
             the descendants
         """
         visited_pages = set()
 
         def find_legacy_pages(page_id, pages):
-            descendants = self.get_descendants(page_id)
+            descendants = self._get_descendants(page_id, mode)
             for descendant in descendants:
                 if descendant not in pages:
                     pages.add(descendant)
                     find_legacy_pages(descendant, pages)
 
         find_legacy_pages(page_id, visited_pages)
         return visited_pages
@@ -367,15 +429,15 @@
 
         Returns:
             the attachment id and attachment object
         """
         attachment = None
         attachment_id = None
 
-        url = 'content/{}/child/attachment'.format(page_id)
+        url = f'content/{page_id}/child/attachment'
         rsp = self.rest_client.get(url, {
             'filename': name,
         })
 
         if rsp['size'] != 0:
             attachment = rsp['results'][0]
             attachment_id = attachment['id']
@@ -394,15 +456,15 @@
             page_id: the page identifier
 
         Returns:
             dictionary of attachment identifiers to their respective names
         """
         attachment_info = {}
 
-        url = 'content/{}/child/attachment'.format(page_id)
+        url = f'content/{page_id}/child/attachment'
         search_fields = {}
 
         # Configure a larger limit value than the default (no provided
         # limit defaults to 25). This should reduce the number of queries
         # needed to fetch a complete attachment set (for larger sets).
         search_fields['limit'] = 1000
 
@@ -471,15 +533,15 @@
             page_id: the page identifier
             expand (optional): data to expand on
 
         Returns:
             the page id and page object
         """
 
-        page = self.rest_client.get('content/{}'.format(page_id), {
+        page = self.rest_client.get(f'content/{page_id}', {
             'status': 'current',
             'expand': expand,
         })
 
         if page:
             assert int(page_id) == int(page['id'])
             self._name_cache[page_id] = page['title']
@@ -526,14 +588,44 @@
             idx += int(rsp['limit'])
             sub_search_fields = dict(search_fields)
             sub_search_fields['start'] = idx
             rsp = self.rest_client.get('content/search', sub_search_fields)
 
         return page_id, page
 
+    def get_page_properties(self, page_id, expand='version'):
+        """
+        get properties from the provided page id
+
+        Performs an API call to acquire known properties about a specific page.
+        This call can returns the page properties dictionary if found;
+        otherwise ``None`` will be returned.
+
+        Args:
+            page_id: the page identifier
+            expand (optional): data to expand on
+
+        Returns:
+            the properties
+        """
+
+        props = None
+
+        try:
+            property_path = f'content/{page_id}/property/{PROP_KEY}'
+            props = self.rest_client.get(property_path, {
+                'status': 'current',
+                'expand': expand,
+            })
+        except ConfluenceBadApiError as ex:
+            if ex.status_code != 404:
+                raise
+
+        return props
+
     def store_attachment(self, page_id, name, data, mimetype, hash_, force=False):
         """
         request to store an attachment on a provided page
 
         Makes a request to a Confluence instance to either publish a new
         attachment or update an existing attachment. If the attachment's hash
         matches the tracked hash (via the comment field) of an existing
@@ -586,32 +678,74 @@
             self._onlynew('skipping existing attachment', attachment['id'])
             return attachment['id']
 
         # publish attachment
         try:
             # split hash comment into chunks to minimize rendering issues with a
             # single one-world-long-hash value
-            hash_ = '{}:{}'.format(HASH_KEY, hash_)
+            hash_ = f'{HASH_KEY}:{hash_}'
             chunked_hash = '\n'.join(
                 [hash_[i:i + 16] for i in range(0, len(hash_), 16)])
 
             data = {
                 'comment': chunked_hash,
                 'file': (name, data, mimetype),
             }
 
             if not self.notify:
                 # using str over bool to support requests pre-v2.19.0
                 data['minorEdit'] = 'true'
 
             if not attachment:
-                url = 'content/{}/child/attachment'.format(page_id)
-                rsp = self.rest_client.post(url, None, files=data)
-                uploaded_attachment_id = rsp['results'][0]['id']
-            else:
+                url = f'content/{page_id}/child/attachment'
+
+                try:
+                    rsp = self.rest_client.post(url, None, files=data)
+                    uploaded_attachment_id = rsp['results'][0]['id']
+                except ConfluenceBadApiError as ex:
+                    # file type restricted? generate a warning
+                    #
+                    # Be a bit flexible in the situation where a specific
+                    # file type is restricted. Instead of hard failing, only
+                    # generate a warning that an attachment could not be added.
+                    # This has been observed for environments using Akeles
+                    # Consulting's "Attachment Checker for Confluence".
+                    if 'file type is not allowed' in str(ex):
+                        fail_msg = f'unable to upload attachment "{name}" '
+                        fail_msg += f'(page: "{self._name_cache[page_id]}"); '
+                        fail_msg += 'this Confluence instance restricts this '
+                        fail_msg += f'file extension ({mimetype})'
+                        logger.warn(fail_msg)
+                        return None
+
+                    if ex.status_code != 503:
+                        raise
+
+                    # retry 503-failed new attachment uploads
+                    #
+                    # It has been observed on Confluence Cloud that in some
+                    # cases when a user publishes a new attachment to a page
+                    # (and maybe specifically attached to a newly created page),
+                    # Confluence may report a 503 error. The behaviour is odd
+                    # since Confluence does partially process the new
+                    # attachment (a viewable entry on the page's list of
+                    # attachments), but the data for the attachment entry is
+                    # corrupted. And in a next publish attempt, since the
+                    # comment hash is unchanged, this extension will not
+                    # attempt to re-upload. To help prevent this case, if a 503
+                    # error state is detected, check to see if the attachment
+                    # entry was created with corrupted data (i.e. can we query
+                    # for an existing attachment). If we find it, re-attempt
+                    # to publish the attachment.
+                    with skip_warningiserror():
+                        logger.warn('attachment failure (503); retrying...')
+                    time.sleep(0.5)
+                    _, attachment = self.get_attachment(page_id, name)
+
+            if attachment:
                 url = 'content/{}/child/attachment/{}/data'.format(
                     page_id, attachment['id'])
                 rsp = self.rest_client.post(url, None, files=data)
                 uploaded_attachment_id = rsp['id']
 
             if not self.watch:
                 self.rest_client.delete('user/watch/content',
@@ -679,14 +813,33 @@
                 self.remove_page(page['id'])
                 page = None
 
         if self.onlynew and page:
             self._onlynew('skipping existing page', page['id'])
             return page['id']
 
+        # fetch known properties (associated with this extension) from the page
+        if page:
+            props = self.get_page_properties(page['id'])
+        else:
+            props = None
+
+        # calculate the hash for a page; we will first use this to check if
+        # there is a update to apply, and if we do need to update, we will
+        # add this value into the page's properties
+        new_page_hash = ConfluenceUtil.hash(data['content'])
+
+        # if we are not force uploading, check if the new page hash matches
+        # the remote hash; if so, do not publish
+        if props and not self.config.confluence_publish_force:
+            remote_hash = props.get('value', {}).get('hash')
+            if new_page_hash == remote_hash:
+                logger.verbose('no changes in page: {}'.format(page_name))
+                return page['id']
+
         try:
             # new page
             if not page:
                 new_page = self._build_page(page_name, data)
                 self._populate_labels(new_page, data['labels'])
 
                 if parent_id:
@@ -708,15 +861,15 @@
 
                     uploaded_page_id = rsp['id']
 
                     # if we have labels and this is a non-cloud instance,
                     # initial labels need to be applied in their own request
                     labels = new_page['metadata']['labels']
                     if not self.cloud and labels:
-                        url = 'content/{}/label'.format(uploaded_page_id)
+                        url = f'content/{uploaded_page_id}/label'
                         self.rest_client.post(url, labels)
 
                 except ConfluenceBadApiError as ex:
                     # Check if Confluence reports that the new page request
                     # fails, indicating it already exists. This is usually
                     # (outside of possible permission use cases) that the page
                     # name's casing does not match. In this case, attempt to
@@ -737,14 +890,28 @@
                         return page['id']
 
             # update existing page
             if page:
                 self._update_page(page, page_name, data, parent_id=parent_id)
                 uploaded_page_id = page['id']
 
+            if not props:
+                props = {
+                    'value': {},
+                    'version': {
+                        'number': 1,
+                    },
+                }
+            else:
+                last_props_version = int(props['version']['number'])
+                props['version']['number'] = last_props_version + 1
+
+            props['value']['hash'] = new_page_hash
+            self.store_page_properties(uploaded_page_id, props)
+
         except ConfluencePermissionError:
             raise ConfluencePermissionError(
                 """Publish user does not have permission to add page """
                 """content to the configured space."""
             )
 
         if not self.watch:
@@ -800,14 +967,29 @@
             )
 
         if not self.watch:
             self.rest_client.delete('user/watch/content', page_id)
 
         return page_id
 
+    def store_page_properties(self, page_id, data):
+        """
+        request to store properties on a page to a confluence instance
+
+        Performs a request which will attempt to store properties on a
+        provided page.
+
+        Args:
+            page_id: the id of the page to update
+            data: the properties data to apply
+        """
+
+        property_path = f'{page_id}/property/{PROP_KEY}'
+        self.rest_client.put('content', property_path, data)
+
     def remove_attachment(self, id_):
         """
         request to remove an attachment
 
         Makes a request to a Confluence instance to remove an existing
         attachment.
 
@@ -920,22 +1102,26 @@
         page = {
             'type': 'page',
             'title': page_name,
             'body': {
                 'storage': {
                     'representation': 'storage',
                     'value': data['content'],
-                }
+                },
             },
             'metadata': {
                 'properties': {},
             },
             'space': {
                 'key': self.space_key,
             },
+            'version': {
+                'number': 1,
+                'message': self.config.confluence_version_comment,
+            },
         }
 
         if self.editor:
             page['metadata']['properties'] = {
                 'editor': {
                     'value': self.editor,
                 },
@@ -969,18 +1155,15 @@
             data: the new page data to apply
             parent_id (optional): the id of the ancestor to use
         """
         last_version = int(page['version']['number'])
 
         update_page = self._build_page(page_name, data)
         update_page['id'] = page['id']
-        update_page['version'] = {
-            'number': last_version + 1,
-            'message': self.config.confluence_version_comment,
-        }
+        update_page['version']['number'] = last_version + 1
 
         labels = list(data['labels'])
         if self.append_labels:
             labels.extend([lbl.get('name')
                 for lbl in page.get('metadata', {}).get(
                     'labels', {}).get('results', {})
             ])
@@ -995,14 +1178,19 @@
                 raise ConfluencePublishAncestorError(page_name)
 
             update_page['ancestors'] = [{'id': parent_id}]
 
             if page['id'] == parent_id:
                 raise ConfluencePublishSelfAncestorError(page_name)
 
+        # zero-id parent ~ a hint to remove the ancestor
+        # (looks like setting a value of "1" is a way to "clear" the option)
+        elif parent_id is not None:
+            update_page['ancestors'] = [{'id': '1'}]
+
         page_id_explicit = page['id'] + '?status=current'
         try:
             self.rest_client.put('content', page_id_explicit, update_page)
         except ConfluenceBadApiError as ex:
 
             # Handle select API failures by waiting a moment and retrying the
             # content request. If it happens again, the put request will fail as
@@ -1056,15 +1244,15 @@
             misc (optional): additional information to append
         """
         s = '[dryrun] '
         s += msg
         if id_ and id_ in self._name_cache:
             s += ' ' + self._name_cache[id_]
         if id_:
-            s += ' ({})'.format(id_)
+            s += f' ({id_})'
         if misc:
             s += ' ' + misc
         logger.info(s + min(80, 80 - len(s)) * ' ')  # 80c-min clearing
 
     def _onlynew(self, msg, id_=None):
         """
         log an only-new mode message
@@ -1078,15 +1266,15 @@
             id_ (optional): identifier (name mapping) associated with the message
         """
         s = '[only-new] '
         s += msg
         if id_ and id_ in self._name_cache:
             s += ' ' + self._name_cache[id_]
         if id_:
-            s += ' ({})'.format(id_)
+            s += f' ({id_})'
         logger.info(s + min(80, 80 - len(s)) * ' ')  # 80c-min clearing
 
     def _populate_labels(self, page, labels):
         """
         populate a page with label metadata information
 
         Accepts a page definition (new or existing page) and populates the
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/rest.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from functools import wraps
 from email.utils import mktime_tz
 from email.utils import parsedate_tz
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceAuthenticationFailedUrlError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadApiError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadServerUrlError
@@ -37,15 +34,15 @@
 # delayed
 RATE_LIMITED_MAX_RETRY_DURATION = 30
 
 
 class SslAdapter(HTTPAdapter):
     def __init__(self, config, *args, **kwargs):
         self._config = config
-        super(SslAdapter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def init_poolmanager(self, *args, **kwargs):
         context = ssl.create_default_context()
 
         # if a custom certificate is provided, load it into this session's
         # SSL context
         if self._config.confluence_client_cert:
@@ -59,18 +56,18 @@
         else:
             context.load_default_certs()
 
         if self._config.confluence_disable_ssl_validation:
             context.check_hostname = False
 
         kwargs['ssl_context'] = context
-        return super(SslAdapter, self).init_poolmanager(*args, **kwargs)
+        return super().init_poolmanager(*args, **kwargs)
 
     def cert_verify(self, conn, url, verify, *args, **kwargs):
-        super(SslAdapter, self).cert_verify(conn, url, verify, *args, **kwargs)
+        super().cert_verify(conn, url, verify, *args, **kwargs)
 
         # prevent requests from injected an embedded certificates to instead
         # rely on the default certificate stores loaded by the context
         if verify is True and not self._config.confluence_adv_embedded_certs:
             conn.ca_certs = None
 
 
@@ -158,15 +155,15 @@
             except requests.exceptions.ConnectionError as ex:
                 raise ConfluenceBadServerUrlError(self.url, ex)
 
         return _wrapper
     return _decorator
 
 
-class Rest(object):
+class Rest:
     CONFLUENCE_DEFAULT_ENCODING = 'utf-8'
 
     def __init__(self, config):
         self.bind_path = API_REST_BIND_PATH
         self.config = config
         self.last_retry = 1
         self.next_delay = None
@@ -217,15 +214,15 @@
         session.mount('https://', adapter)
 
         if config.confluence_server_auth:
             session.auth = config.confluence_server_auth
         elif config.confluence_server_user:
             passwd = config.confluence_server_pass
             if passwd is None:
-                passwd = ''
+                passwd = ''  # noqa: S105
             session.auth = (config.confluence_server_user, passwd)
 
         if config.confluence_server_cookies:
             session.cookies.update(config.confluence_server_cookies)
 
         # provides users a direct hook into manipulating a built requests
         # session, to allow full control over requests capabilities which may
@@ -325,20 +322,20 @@
             raise ConfluenceBadApiError(rsp.status_code, errdata)
 
     def close(self):
         self.session.close()
 
     def _format_error(self, rsp, key):
         err = ""
-        err += "REQ: {0}\n".format(rsp.request.method)
+        err += f"REQ: {rsp.request.method}\n"
         err += "RSP: " + str(rsp.status_code) + "\n"
         err += "URL: " + self.url + self.bind_path + "\n"
         err += "API: " + key + "\n"
         try:
-            err += 'DATA: {}'.format(json.dumps(rsp.json(), indent=2))
+            err += f'DATA: {json.dumps(rsp.json(), indent=2)}'
         except:  # noqa: E722
             err += 'DATA: <not-or-invalid-json>'
         return err
 
     def _handle_common_request(self, rsp):
 
         # if confluence or a proxy reports a retry-after delay (to pace us),
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/roles.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/roles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
+"""
 See also docutils roles:
 
     https://docutils.sourceforge.io/docs/howto/rst-roles.html#define-the-role-function
 """
 
+from docutils import nodes
+from sphinxcontrib.confluencebuilder.nodes import confluence_doc_card_inline
 from sphinxcontrib.confluencebuilder.nodes import confluence_emoticon_inline
 from sphinxcontrib.confluencebuilder.nodes import confluence_latex_inline
+from sphinxcontrib.confluencebuilder.nodes import confluence_link_card_inline
 from sphinxcontrib.confluencebuilder.nodes import confluence_mention_inline
 from sphinxcontrib.confluencebuilder.nodes import confluence_status_inline
 from sphinxcontrib.confluencebuilder.nodes import jira_issue
+from sphinx.roles import XRefRole
+
+
+ConfluenceDocRole = XRefRole(nodeclass=confluence_doc_card_inline,
+    innernodeclass=nodes.inline, warn_dangling=True)
 
 
 def ConfluenceEmoticonRole(name, rawtext, text, lineno, inliner, options=None, content=None):
     """
     a confluence emoticon role
 
     Defines an inline Confluence emoticon role where users can inject inlined
@@ -61,14 +68,40 @@
     """
 
     node = confluence_latex_inline(rawsource=text, text=text)
 
     return [node], []
 
 
+def ConfluenceLinkRole(name, rawtext, text, lineno, inliner, options=None, content=None):
+    """
+    a confluence link role
+
+    Defines an inline Confluence link role where users can inject inlined
+    card link (v2 editor) for a target link.
+
+    Args:
+        name: local name of the interpreted text role
+        rawtext: the entire interpreted text construct
+        text: the interpreted text content
+        lineno: the line number where the interpreted text beings
+        inliner: inliner object that called the role function
+        options: dictionary of directive options for customization
+        content: list of strings, the directive content for customization
+
+    Returns:
+        returns a tuple include a list of nodes and a list of system messages
+    """
+
+    node = confluence_link_card_inline(rawsource=text, text=text)
+    node.params['href'] = text
+
+    return [node], []
+
+
 def ConfluenceMentionRole(name, rawtext, text, lineno, inliner, options=None, content=None):
     """
     a confluence mention role
 
     Defines an inline Confluence mention role where users can inject inlined
     @mentions.
 
@@ -134,14 +167,39 @@
     node.params['title'] = text
     if outlined:
         node.params['subtle'] = 'true'
 
     return [node], []
 
 
+def ConfluenceStrikeRole(name, rawtext, text, lineno, inliner, options=None, content=None):
+    """
+    a confluence strike role
+
+    Defines an inline Confluence strike role where users can inject inlined
+    node to styled with a strikethrough.
+
+    Args:
+        name: local name of the interpreted text role
+        rawtext: the entire interpreted text construct
+        text: the interpreted text content
+        lineno: the line number where the interpreted text beings
+        inliner: inliner object that called the role function
+        options: dictionary of directive options for customization
+        content: list of strings, the directive content for customization
+
+    Returns:
+        returns a tuple include a list of nodes and a list of system messages
+    """
+
+    node = nodes.inline(rawsource=text, text=text, classes=['strike'])
+
+    return [node], []
+
+
 def JiraRole(name, rawtext, text, lineno, inliner, options=None, content=None):
     """
     a jira role
 
     Defines an inline Jira role where users can inject a Jira issue macro inside
     a block of text.
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/singlebuilder.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/singlebuilder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2020-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:copyright: Copyright 2007-2019 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
+# Copyright 2007-2019 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
 
 from docutils import nodes
-from sphinx.util import progress_message
 from sphinx.util.console import darkgreen  # pylint: disable=no-name-in-module
 from sphinxcontrib.confluencebuilder.builder import ConfluenceBuilder
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.compat import inline_all_toctrees
+from sphinxcontrib.confluencebuilder.compat import progress_message
 from sphinxcontrib.confluencebuilder.locale import C
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 
 
 class SingleConfluenceBuilder(ConfluenceBuilder):
     name = 'singleconfluence'
 
@@ -32,25 +29,25 @@
         return tree
 
     def assemble_toc_secnumbers(self):
         new_secnumbers = {}
 
         for docname, secnums in self.env.toc_secnumbers.items():
             for id_, secnum in secnums.items():
-                alias = '{}/{}'.format(docname, id_)
+                alias = f'{docname}/{id_}'
                 new_secnumbers[alias] = secnum
 
         return {self.config.root_doc: new_secnumbers}
 
     def assemble_toc_fignumbers(self):
         new_fignumbers = {}
 
         for docname, fignumlist in self.env.toc_fignumbers.items():
             for figtype, fignums in fignumlist.items():
-                alias = '{}/{}'.format(docname, figtype)
+                alias = f'{docname}/{figtype}'
                 new_fignumbers.setdefault(alias, {})
 
                 for id_, fignum in fignums.items():
                     new_fignumbers[alias][id_] = fignum
 
         return {self.config.root_doc: new_fignumbers}
 
@@ -214,28 +211,28 @@
                 section_node = node.parent
                 if 'ids' in section_node:
                     title_name = ''.join(node.astext().split())
 
                     for id_ in section_node['ids']:
                         target = title_name
 
-                        anchorname = '%s/#%s' % (docname, id_)
+                        anchorname = f'{docname}/#{id_}'
                         if anchorname not in secnumbers:
                             anchorname = '%s/' % id_
 
                         if self.add_secnumbers:
                             secnumber = secnumbers.get(anchorname)
                             if secnumber:
                                 target = ('.'.join(map(str, secnumber)) +
                                     self.secnumber_suffix + target)
 
                         section_id = doc_used_names.get(target, 0)
                         doc_used_names[target] = section_id + 1
                         if section_id > 0:
-                            target = '{}.{}'.format(target, section_id)
+                            target = f'{target}.{section_id}'
 
                         self.state.register_target(anchorname, target)
 
                         # register a "document target" if the document's base
                         # identifier is set to a value which does not match the
                         # document's docname
                         #
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/state.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 import hashlib
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceConfigurationError
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.std.confluence import CONFLUENCE_MAX_TITLE_LEN
 
 
@@ -37,16 +34,15 @@
         document and track publish upload identifiers (see `registerUploadId`),
         the publish operation can help ensure pages are structured in a
         hierarchical fashion (see also `parentDocname`).
 
         [1]: http://www.sphinx-doc.org/en/stable/markup/toctree.html#directive-toctree
         """
         ConfluenceState.doc2parentDoc[docname] = parent_docname
-        logger.verbose(
-            'setting parent of %s to: %s' % (docname, parent_docname))
+        logger.verbose(f'setting parent of {docname} to: {parent_docname}')
 
     @staticmethod
     def register_target(refid, target):
         """
         register a reference to a specific (anchor) target
 
         When interpreting a reference in reStructuredText, the reference could
@@ -54,15 +50,15 @@
         in another document. In Confluence, the target name is typically
         dependent on the document's title name (auto-generated targets provided
         by Confluence; ex. title#header). This register method allows a builder
         to track the target value to use for a provided reference (so that a
         writer can properly prepare a link; see also `target`).
         """
         ConfluenceState.refid2target[refid] = target
-        logger.verbose('mapping %s to target: %s' % (refid, target))
+        logger.verbose(f'mapping {refid} to target: {target}')
 
     @staticmethod
     def register_title(docname, title, config):
         """
         register the title for the provided document name
 
         In Confluence, a page is identified by the name/title of a page (at
@@ -82,15 +78,15 @@
 
         if config and (not config.confluence_ignore_titlefix_on_index or
                 docname != config.root_doc):
             prefix = config.confluence_publish_prefix
 
             postfix = ConfluenceState._format_postfix(
                 postfix=config.confluence_publish_postfix, docname=docname,
-                config=config
+                config=config,
             )
 
         if prefix:
             title = prefix + title
 
         if postfix:
             base_tail += postfix
@@ -109,24 +105,24 @@
         offset = 2
         while title.lower() in ConfluenceState.title2doc:
             if offset == 2:
                 logger.warn('title conflict detected with '
                     "'{}' and '{}'".format(
                         ConfluenceState.title2doc[title.lower()], docname))
 
-            tail = ' ({}){}'.format(offset, base_tail)
+            tail = f' ({offset}){base_tail}'
             if len(base_title) + len(tail) > try_max:
                 base_title = base_title[0:(try_max - len(tail))]
 
             title = base_title + tail
             offset += 1
 
         ConfluenceState.doc2title[docname] = title
         ConfluenceState.title2doc[title.lower()] = docname
-        logger.verbose('mapping %s to title: %s' % (docname, title))
+        logger.verbose(f'mapping {docname} to title: {title}')
         return title
 
     @staticmethod
     def register_toctree_depth(docname, depth):
         """
         register the toctree-depth for the provided document name
 
@@ -134,15 +130,15 @@
         option [1]. This method provides the ability to track the depth of a
         document before toctree resolution removes any hints at the maximum
         depth desired.
 
         [1]: http://www.sphinx-doc.org/en/stable/markup/toctree.html#id3
         """
         ConfluenceState.doc2ttd[docname] = depth
-        logger.verbose('track %s toc-depth: %s' % (docname, depth))
+        logger.verbose(f'track {docname} toc-depth: {depth}')
 
     @staticmethod
     def register_upload_id(docname, id_):
         """
         register a page (upload) identifier for a docname
 
         When a publisher creates/updates a page on a Confluence instance, the
@@ -151,15 +147,16 @@
         registration method. This method is primarily used to help track/order
         published documents into a hierarchical fashion (see
         `registerParentDocname`). It is important to note that the order of
         published documents will determine if a page's upload identifier is
         tracked in this state (see also `uploadId`).
         """
         ConfluenceState.doc2uploadId[docname] = id_
-        logger.verbose("tracking docname %s's upload id: %s" % (docname, id_))
+        logger.verbose(
+            f"tracking docname {docname}'s upload id: {id_}")
 
     @staticmethod
     def reset():
         """
         reset all state information
 
         Provides the ability for uses of a Confluence state singleton to reset
@@ -240,8 +237,8 @@
         Create a unique(ish) hash for the given source file to avoid collisions
         when pushing pages to confluence.
         """
         prehash = docname
         prehash += str(config.project)
         prehash += str(config.confluence_parent_page)
         prehash += str(config.confluence_publish_root)
-        return hashlib.sha1(prehash.encode()).hexdigest()
+        return hashlib.sha1(prehash.encode()).hexdigest()  # noqa: S324
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/std/confluence.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/confluence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2017-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.std.sphinx import DEFAULT_HIGHLIGHT_STYLE
 import os
 
 # confluence trailing bind path for rest api
 API_REST_BIND_PATH = 'rest/api'
 
@@ -390,14 +387,66 @@
     # To follow Sphinx's method of highlighting, use Confluence's 'python'
     # highlight type as the target language for the default type.
     #
     # [1]: http://www.sphinx-doc.org/en/stable/config.html#confval-highlight_language
     DEFAULT_HIGHLIGHT_STYLE: 'python'
 }
 
+# sphinx literal to confluence language map (fallbacks)
+#
+# Provides an extended map to help provide fallback language types where an
+# "unsupported code language" warning is still desired but an alternative
+# language type is better than a default/"plain" language type. For example,
+# Confluence does not support interactive Python code blocks. A warning should
+# be generated to inform users that their documentation cannot render them
+# (specifically, the interactive part); however, it will be still nice to
+# render the content as Python code instead of plain text.
+LITERAL2LANG_FBMAP_COMMON = {
+    # C-like languages
+    'arduino': 'cpp',
+    'charmci': 'cpp',
+    'clay': 'cpp',
+    'cu': 'cpp',
+    'cuda': 'cpp',
+    'ec': 'cpp',
+    'mq4': 'cpp',
+    'mq5': 'cpp',
+    'mql': 'cpp',
+    'mql4': 'cpp',
+    'mql5': 'cpp',
+    'nesc': 'cpp',
+    'omg-idl': 'cpp',
+    'pike': 'cpp',
+    'swig': 'cpp',
+    'vala': 'cpp',
+    'vapi': 'cpp',
+}
+
+LITERAL2LANG_FBMAP_V1 = {
+    **LITERAL2LANG_FBMAP_COMMON,
+    # Interactive Python
+    'ipython': 'python',
+    'ipython2': 'python',
+    'ipython3': 'python',
+    # JSON (if JSON is not explicitly supported, Python style slightly works)
+    'json': 'python',
+    'json-object': 'python',
+}
+
+LITERAL2LANG_FBMAP_V2 = {
+    **LITERAL2LANG_FBMAP_COMMON,
+    # Interactive Python
+    'ipython': 'py',
+    'ipython2': 'py',
+    'ipython3': 'py',
+    # JSON (if JSON is not explicitly supported, Python style slightly works)
+    'json': 'py',
+    'json-object': 'py',
+}
+
 # fallback highlight language
 #
 # When provided a language type that is not supported by Confluence is detected on
 # a code block, this fallback style will be applied instead.
 FALLBACK_HIGHLIGHT_STYLE = 'none'
 
 # no-check value to inject into a X-Atlassian-Token header
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.state import ConfluenceState
 
 
 def encode_storage_format(data):
     """
     encodes text to be inserted directly into a storage format area
@@ -54,15 +51,15 @@
     Returns:
         the encoded text
     """
 
     anchor_value = None
     if '#' in refuri:
         anchor = refuri.split('#')[1]
-        target_name = '{}#{}'.format(docname, anchor)
+        target_name = f'{docname}#{anchor}'
 
         # check if this target is reachable without an anchor; if so, use
         # the identifier value instead
         target = ConfluenceState.target(target_name)
         if target:
             anchor_value = target
         else:
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/index.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinx.environment.adapters.indexentries import IndexEntries
 from sphinxcontrib.confluencebuilder.locale import L as sccb_translation
 from sphinxcontrib.confluencebuilder.state import ConfluenceState
 from sphinxcontrib.confluencebuilder.storage import intern_uri_anchor_value
 import os
 import pkgutil
@@ -31,20 +28,20 @@
     if not content:
         return
 
     # pre-process link entries to use final document titles/anchor values
     for key, entries in content:
         for (i, entry) in enumerate(entries):
             if isinstance(entry, list):
-                refuri = '{}#{}'.format(entry[2], entry[3])
+                refuri = f'{entry[2]}#{entry[3]}'
                 doctitle, anchor_value = process_doclink(builder.config, refuri)
                 entry[2] = doctitle
                 entry[3] = anchor_value
             else:
-                refuri = '{}#{}'.format(entry.docname, entry.anchor)
+                refuri = f'{entry.docname}#{entry.anchor}'
                 doctitle, anchor_value = process_doclink(builder.config, refuri)
                 entries[i] = entries[i]._replace(
                     docname=doctitle, anchor=anchor_value)
 
     # fetch raw template data
     if builder.config.confluence_editor:
         domainindex_fname = 'domainindex_v2.html'
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/search.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.locale import L as sccb_translation
 import os
 import pkgutil
 
 
 def generate_storage_format_search(builder, docname, f):
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {#
-Template for a storage-format domainindex document.
+SPDX-License-Identifier: BSD-2-Clause
+Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
+Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
-:copyright: Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:copyright: Copyright 2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+Template for a storage-format domainindex document.
 #}
 
 {%- if pagegen_notice -%}
     <div style="color: #707070; font-size: 12px;">
         {{ L('This page has been automatically generated.') }}
     </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{# Template for a storage-format domainindex document. :copyright: Copyright
-2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS) :copyright: Copyright
-2021 Sphinx Confluence Builder Contributors (AUTHORS) :license: BSD-2-Clause
-(LICENSE) #} {%- if pagegen_notice -%}
+{# SPDX-License-Identifier: BSD-2-Clause Copyright 2007-2021 by the Sphinx team
+(sphinx-doc/sphinx#AUTHORS) Copyright Sphinx Confluence Builder Contributors
+(AUTHORS) Template for a storage-format domainindex document. #} {%- if
+pagegen_notice -%}
 {{ L('This page has been automatically generated.') }}
 ===============================================================================
 {%- else -%}
 ===============================================================================
 {%- endif %}
 {% for (key, _) in index -%}  {{ key|upper }}  {% if not loop.last %}| {% endif
 %} {%- endfor %}
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {#
-Template for a storage-format domainindex document.
+SPDX-License-Identifier: BSD-2-Clause
+Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
+Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
-:copyright: Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+Template for a storage-format domainindex document.
 #}
 
 {%- if pagegen_notice -%}
     <div style="color: #707070; font-size: 12px;">
         {{ L('This page has been automatically generated.') }}
     </div>
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {#
-Template for a storage-format genindex document.
+SPDX-License-Identifier: BSD-2-Clause
+Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
+Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
-:copyright: Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:copyright: Copyright 2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+Template for a storage-format genindex document.
 #}
 
 {% macro indexentry(name, links) %}
     {%- if links -%}
         {%- set ismain = links[0][0] -%}
         {%- set docname, anchor = links[0][1] -%}
         {%- if ismain %}<strong>{% endif -%}
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {#
-Template for a storage-format genindex document.
+SPDX-License-Identifier: BSD-2-Clause
+Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
+Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
-:copyright: Copyright 2007-2021 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+Template for a storage-format genindex document.
 #}
 
 {% macro indexentry(name, links) %}
     {%- if links -%}
         {%- set ismain = links[0][0] -%}
         {%- set docname, anchor = links[0][1] -%}
         {%- if ismain %}<strong>{% endif -%}
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/templates/search.html` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/search.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {#
-Template for a storage-format search document.
+SPDX-License-Identifier: BSD-2-Clause
+Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
-:copyright: Copyright 2021 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
+Template for a storage-format search document.
 #}
 
 {%- if pagegen_notice -%}
     <div style="color: #707070; font-size: 12px;">
         {{ L('This page has been automatically generated.') }}
     </div>
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/storage/translator.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:copyright: Copyright 2018-2020 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
+# Copyright 2018-2020 by the Sphinx team (sphinx-doc/sphinx#AUTHORS)
 
+from contextlib import suppress
 from docutils import nodes
 from os import path
 from sphinx import addnodes
 from sphinx.locale import _ as SL
 from sphinx.locale import admonitionlabels
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceError
 from sphinxcontrib.confluencebuilder.locale import L
 from sphinxcontrib.confluencebuilder.std.confluence import FALLBACK_HIGHLIGHT_STYLE
 from sphinxcontrib.confluencebuilder.std.confluence import FCMMO
 from sphinxcontrib.confluencebuilder.std.confluence import INDENT
+from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_FBMAP_V1
+from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_FBMAP_V2
 from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_MAP_V1
 from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_MAP_V2
 from sphinxcontrib.confluencebuilder.std.sphinx import DEFAULT_HIGHLIGHT_STYLE
 from sphinxcontrib.confluencebuilder.storage import encode_storage_format
 from sphinxcontrib.confluencebuilder.storage import intern_uri_anchor_value
 from sphinxcontrib.confluencebuilder.translator import ConfluenceBaseTranslator
 from sphinxcontrib.confluencebuilder.util import convert_length
@@ -76,15 +76,15 @@
         if node.get('secnumber'):
             return node['secnumber']
 
         if isinstance(node.parent, nodes.section):
             if self.builder.name == 'singleconfluence':
                 docname = self._docnames[-1]
                 raw_anchor = node.parent['ids'][0]
-                anchorname = '%s/#%s' % (docname, node.parent['ids'][0])
+                anchorname = '{}/#{}'.format(docname, node.parent['ids'][0])
                 if anchorname not in self.builder.secnumbers:
                     anchorname = '%s/' % raw_anchor
             else:
                 anchorname = '#' + node.parent['ids'][0]
                 if anchorname not in self.builder.secnumbers:
                     anchorname = ''
 
@@ -113,15 +113,15 @@
             return ''
 
         figtype = self.builder.env.domains['std'].get_enumerable_node_type(node)
         if not figtype:
             return ''
 
         if self.builder.name == 'singleconfluence':
-            key = '%s/%s' % (self._docnames[-1], figtype)
+            key = f'{self._docnames[-1]}/{figtype}'
         else:
             key = figtype
 
         figid = first(node['ids'])
         if figid in self.builder.fignumbers.get(key, {}):
             prefix = self.numfig_format.get(figtype)
             if prefix:
@@ -154,18 +154,42 @@
             doc_target = self.state.target(doc_anchorname)
             if not doc_target:
                 doc_id = node['docname']
                 self.body.append(self._start_ac_macro(node, 'anchor'))
                 self.body.append(self._build_ac_param(node, '', doc_id))
                 self.body.append(self._end_ac_macro(node, suffix=''))
 
+    def pre_body_data(self):
+        data = ''
+
+        # Confluence's v1 editor ignores a full-width page style on
+        # publication (most likely since the concept of page width was
+        # developed for v2 and newer). To emulate a non-full-width state with
+        # a v1 editor, apply a layout around the page contents.
+        if not self.v2 and self.builder.config.confluence_full_width is False:
+            data += '<ac:layout>'
+            data += '<ac:layout-section ac:type="fixed-width">'
+            data += '<ac:layout-cell>'
+
+        return data
+
+    def post_body_data(self):
+        data = ''
+
+        if not self.v2 and self.builder.config.confluence_full_width is False:
+            data += '</ac:layout-cell>'
+            data += '</ac:layout-section>'
+            data += '</ac:layout>'
+
+        return data
+
     def visit_title(self, node):
         if isinstance(node.parent, (nodes.section, nodes.topic)):
             self.body.append(
-                self._start_tag(node, 'h{}'.format(self._title_level)))
+                self._start_tag(node, f'h{self._title_level}'))
 
             # generate anchors inside headers for v2, to avoid extra
             # spacing from an anchor macro
             if self.v2:
                 # hinted to build an anchor for a target
                 anchor = node.parent.get('section-embedded-anchor', None)
                 if anchor:
@@ -183,31 +207,39 @@
             self.add_fignumber(node.parent)
             self.context.append(self._end_tag(node))
 
             # if title points to a section and does not already contain a
             # reference, create a link to it
             if 'refid' in node and not node.next_node(nodes.reference):
                 anchor_value = ''.join(node['refid'].split())
-                self.body.append(self._start_ac_link(node, anchor_value))
-                self.context.append(self._end_ac_link(node))
-                self.body.append(self._start_ac_link_body(node))
-                self.context.append(self._end_ac_link_body(node))
+
+                if self.v2:
+                    attribs = {
+                        'href': f'#{anchor_value}',
+                    }
+
+                    self.body.append(self._start_tag(node, 'a', **attribs))
+                    self.context.append(self._end_tag(node, suffix=''))
+                else:
+                    self.body.append(self._start_ac_link(node, anchor_value))
+                    self.body.append(self._start_ac_link_body(node))
+                    self.context.append(self._end_ac_link_body(node) +
+                        self._end_ac_link(node))
         elif (isinstance(node.parent, addnodes.compact_paragraph) and
                 node.parent.get('toctree')):
             self.visit_caption(node)
         else:
             # Only render section/topic titles in headers. For all other nodes,
             # they must explicitly manage their own title entries.
             raise nodes.SkipNode
 
     def depart_title(self, node):
         if isinstance(node.parent, (nodes.section, nodes.topic)):
             if 'refid' in node and not node.next_node(nodes.reference):
-                self.body.append(self.context.pop())  # ac_link_body
-                self.body.append(self.context.pop())  # end_ac_link
+                self.body.append(self.context.pop())  # link
 
             self.body.append(self.context.pop())  # h<x>
         elif (isinstance(node.parent, addnodes.compact_paragraph) and
                 node.parent.get('toctree')):
             self.depart_caption(node)
 
     def visit_paragraph(self, node):
@@ -220,17 +252,17 @@
         if self.v2 and self._indent_level > 0:
             style += 'margin-left: {}px;'.format(INDENT * self._indent_level)
 
         # MyST-Parser will inject text-align hints in the node's classes
         # attribute; if set, attempt to apply the style
         if isinstance(node.parent, nodes.entry):
             for class_ in node.parent.get('classes', []):
-                if 'text-center' == class_:
+                if class_ == 'text-center':
                     style += 'text-align: center;'
-                elif 'text-right' == class_:
+                elif class_ == 'text-right':
                     style += 'text-align: right;'
                 # (legacy)
                 elif class_.startswith('text-align:'):
                     style += self.encode(class_)
                     break
 
         if style:
@@ -306,15 +338,15 @@
                 child.__confluence_list_item_margin = True
 
         # If this list is nested inside a complex list, ensure this list starts
         # off with a margin (to offset it's position inside the complex list).
         if isinstance(node.parent, nodes.list_item):
             try:
                 if node.parent.__confluence_list_item_margin:
-                    attribs['style'] = 'margin-top: {}px;'.format(FCMMO)
+                    attribs['style'] = f'margin-top: {FCMMO}px;'
             except AttributeError:
                 pass
 
     def visit_bullet_list(self, node):
         # [sphinx-gallery] if a list item is build with sphinx-gallery providing
         # a `horizontal` class type, the extension produces html output in an
         # hlist fashion; replicate this here
@@ -381,15 +413,15 @@
             self.visit_hlistcol(node)
             return
 
         # apply margin offset if flagged (see _apply_leading_list_item_offets)
         attribs = {}
         try:
             if node.__confluence_list_item_margin:
-                attribs['style'] = 'margin-top: {}px;'.format(FCMMO)
+                attribs['style'] = f'margin-top: {FCMMO}px;'
         except AttributeError:
             pass
 
         self.body.append(self._start_tag(node, 'li', suffix=self.nl, **attribs))
         self.context.append(self._end_tag(node))
 
     def depart_list_item(self, node):
@@ -661,14 +693,15 @@
     # -------------------------------
     # body elements -- literal blocks
     # -------------------------------
 
     def visit_literal_block(self, node):
         lang = None
         lang_map = LITERAL2LANG_MAP_V2 if self.v2 else LITERAL2LANG_MAP_V1
+        fb_map = LITERAL2LANG_FBMAP_V2 if self.v2 else LITERAL2LANG_FBMAP_V1
 
         # non-raw literal
         if node.rawsource != node.astext():
             # include marked with a literal flag; ignore parsed literals for
             # v2 editor since they are no longer supported
             if 'source' in node or self.v2:
                 lang = 'none'
@@ -683,23 +716,29 @@
                 self.context.append(self._end_tag(node))
                 self.body.append(self._start_tag(node, 'code'))
                 self.context.append(self._end_tag(node))
                 return
 
         if not lang:
             lang = node.get('language', self._highlight).lower()
+
+        translated_lang = None
         if self.builder.lang_transform:
-            lang = self.builder.lang_transform(lang)
-        elif lang in lang_map.keys():
+            translated_lang = self.builder.lang_transform(lang)
+
+        if translated_lang:
+            lang = translated_lang
+        elif lang in lang_map:
             lang = lang_map[lang]
         else:
             if lang not in self._tracked_unknown_code_lang:
-                self.warn('unsupported code language for confluence: ' + lang)
+                self.warn('unsupported code language for confluence: ' + lang,
+                    subtype='unsupported_code_lang')
                 self._tracked_unknown_code_lang.append(lang)
-            lang = lang_map[FALLBACK_HIGHLIGHT_STYLE]
+            lang = fb_map.get(lang, FALLBACK_HIGHLIGHT_STYLE)
 
         data = self.nl.join(node.astext().splitlines())
 
         title = node.get('scb-caption', None)
         if title:
             title = self.encode(title)
 
@@ -708,18 +747,16 @@
         elif data.count('\n') >= self._linenothreshold:
             num = 'true'
         else:
             num = 'false'
 
         firstline = None
         if num == 'true':
-            try:
+            with suppress(KeyError):
                 firstline = node.attributes['highlight_args']['linenostart']
-            except KeyError:
-                pass
 
         self.body.append(self._start_ac_macro(node, 'code'))
         self.body.append(self._build_ac_param(node, 'language', lang))
         self.body.append(self._build_ac_param(node, 'linenumbers', num))
 
         if firstline is not None and firstline > 1:
             self.body.append(
@@ -788,15 +825,15 @@
             self._indent_level += 1
         else:
             style = ''
 
             # Confluence's WYSIWYG, when indenting paragraphs, will produce
             # paragraphs will margin values offset by 30 pixels units. The same
             # indentation is applied here via a style value.
-            style += 'margin-left: {}px;'.format(INDENT)
+            style += f'margin-left: {INDENT}px;'
 
             # Confluence's provided styles remove first-child elements leading
             # margins. This causes some unexpected styling issues when various
             # indentation patterns are applied (between div elements and
             # multiple paragraphs). To overcome this, the indent container being
             # added will be given a top-padding-offset matching Confluence's
             # common non-first-child element top-margins (i.e. 10 pixels).
@@ -825,15 +862,15 @@
             firstchild_margin = True
 
             next_child = first(findall(node, include_self=False))
             if isinstance(next_child, nodes.block_quote):
                 firstchild_margin = False
 
             if firstchild_margin:
-                style += 'padding-top: {}px;'.format(FCMMO)
+                style += f'padding-top: {FCMMO}px;'
 
             self.body.append(self._start_tag(node, 'div', suffix=self.nl,
                 **{'style': style}))
             self.context.append(self._end_tag(node))
 
     def depart_block_quote(self, node):
         if first(findall(node, nodes.attribution)) or not self.v2:
@@ -976,17 +1013,18 @@
             self.body.append(self._end_tag(node))
 
         table_classes = node.get('classes', [])
         attribs = {}
 
         # [sphinxcontrib-needs]
         # force needs tables to a maximum width
+        # (do not for v2 editor, as it will already use the page's width)
         needs_styles = ['need', 'NEEDS_TABLE', 'NEEDS_DATATABLES']
         node.__needs_table = any(ns in table_classes for ns in needs_styles)
-        if node.__needs_table:
+        if node.__needs_table and not self.v2:
             attribs['style'] = 'width: 100%;'
 
         self.body.append(self._start_tag(
             node, 'table', suffix=self.nl, **attribs))
         self.context.append(self._end_tag(node))
 
         # track the thead context
@@ -997,14 +1035,22 @@
         # proper type. A context list is needed to support nested tables.
         self._thead_context.append(False)
 
     def depart_table(self, node):
         self.body.append(self.context.pop())  # table
         self._thead_context.pop()
 
+        # [sphinxcontrib-needs]
+        # inject a newline on v1 editor for needs tables, to help space out
+        # different requirements; note v2 editor tables already force some
+        # level of spacing
+        if node.__needs_table and not self.v2:
+            self.body.append(self._start_tag(
+                node, 'br', suffix=self.nl, empty=True))
+
     def visit_tgroup(self, node):
         node.stubs = []
 
         apply_colwidths = False
         table_classes = node.parent.get('classes', [])
 
         # if column widths are explicitly given, apply specific column widths
@@ -1019,16 +1065,26 @@
         if apply_colwidths:
             has_colspec = False
             for colspec in findall(node, nodes.colspec):
                 if not has_colspec:
                     self.body.append(self._start_tag(node, 'colgroup'))
                     has_colspec = True
 
-                self.body.append(self._start_tag(node, 'col', empty=True,
-                    **{'style': 'width: {}%'.format(colspec['colwidth'])}))
+                # apply a width percentage based on the configured colwidth
+                # value; however, if this is a v2 editor and it is detected
+                # that the configured width is set to 100%, do not apply any
+                # styling, v2 tables are already 100% by default, and
+                # configuring it explicitly may break the editor's page
+                # width configuration
+                attribs = {}
+                if colspec['colwidth'] != 100 or not self.v2:
+                    attribs['style'] = 'width: {}%'.format(colspec['colwidth'])
+
+                self.body.append(self._start_tag(
+                    node, 'col', empty=True, **attribs))
 
             if has_colspec:
                 self.body.append(self._end_tag(node))
 
     def depart_tgroup(self, node):
         pass
 
@@ -1081,19 +1137,36 @@
         if table.__needs_table:
             if 'head' in row.get('classes', []):
                 target_tag = 'th'
             if 'head_center' in node.get('classes', []):
                 attribs['style'] = 'text-align: center;'
             if 'head_right' in node.get('classes', []):
                 attribs['style'] = 'text-align: right;'
+            if 'footer_right' in node.get('classes', []):
+                attribs['style'] = 'text-align: right;'
 
         self.body.append(self._start_tag(node, target_tag, **attribs))
         self.context.append(self._end_tag(node))
 
+        # [sphinxcontrib-needs]
+        # for meta-like fields, attempt to make the font smaller
+        node.__needs_table_extra = False
+        entry_classes = node.get('classes', [])
+        sup_styles = ['meta', 'head_right', 'head_left',
+                      'footer_left', 'footer_right']
+        if table.__needs_table:
+            if any(ns in entry_classes for ns in sup_styles):
+                self.body.append(self._start_tag(node, 'sup'))
+                self.context.append(self._end_tag(node, suffix=''))
+                node.__needs_table_extra = True
+
     def depart_entry(self, node):
+        if node.__needs_table_extra:
+            self.body.append(self.context.pop())  # sup
+
         self.body.append(self.context.pop())  # td/th
 
     def visit_tabular_col_spec(self, node):
         raise nodes.SkipNode
 
     def visit_colspec(self, node):
         self.colspecs.append(node)
@@ -1140,36 +1213,39 @@
 
         attribs = {}
         attribs['href'] = uri
 
         next_child = first(findall(node, include_self=False))
         if isinstance(next_child, nodes.inline):
             if 'viewcode-link' in next_child.get('classes', []):
-                self.body.append(self._start_tag(node, 'div',
-                    **{'style': 'float: right'}))
-                self._reference_context.append(self._end_tag(node))
+                if self.v2:
+                    self.body.append(' ')
+                else:
+                    self.body.append(self._start_tag(node, 'div',
+                        **{'style': 'float: right'}))
+                    self._reference_context.append(self._end_tag(node))
 
         if 'reftitle' in node:
             title = node['reftitle']
             title = self.encode(title)
             attribs['title'] = title
 
         self.body.append(self._start_tag(node, 'a', **attribs))
         self._reference_context.append(self._end_tag(node, suffix=''))
 
     def _visit_reference_intern_id(self, node):
         raw_anchor = ''.join(node['refid'].split())
 
         if self.builder.name == 'singleconfluence':
             docname = self._docnames[-1]
-            anchorname = '%s/#%s' % (docname, raw_anchor)
+            anchorname = f'{docname}/#{raw_anchor}'
             if anchorname not in self.builder.secnumbers:
                 anchorname = '%s/' % raw_anchor
         else:
-            anchorname = '{}#{}'.format(self.docname, raw_anchor)
+            anchorname = f'{self.docname}#{raw_anchor}'
 
         # check if this target is reachable without an anchor; if so, use the
         # identifier value instead
         target = self.state.target(anchorname)
         if target:
             anchor_value = target
             anchor_value = self.encode(anchor_value)
@@ -1186,23 +1262,31 @@
                 self.body.append(self._end_ac_macro(node, suffix=''))
 
         if is_citation:
             self.body.append(self._start_tag(node, 'sup'))
             self._reference_context.append(self._end_tag(node, suffix=''))
 
         if anchor_value:
-            # build link to internal anchor (on the same page)
-            #  Note: plain-text-link body cannot have inline markup; content
-            #        will be added into body already and skip-children should be
-            #        invoked for this use case.
-            self.body.append(self._start_ac_link(node, anchor_value))
-            self._reference_context.append(self._end_ac_link(node))
+            if self.v2:
+                attribs = {
+                    'href': f'#{anchor_value}',
+                }
 
-            self.body.append(self._start_ac_link_body(node))
-            self._reference_context.append(self._end_ac_link_body(node))
+                self.body.append(self._start_tag(node, 'a', **attribs))
+                self._reference_context.append(self._end_tag(node, suffix=''))
+            else:
+                # build link to internal anchor (on the same page)
+                #  Note: plain-text-link body cannot have inline markup; content
+                #        will be added into body already and skip-children
+                #        should be invoked for this use case.
+                self.body.append(self._start_ac_link(node, anchor_value))
+                self._reference_context.append(self._end_ac_link(node))
+
+                self.body.append(self._start_ac_link_body(node))
+                self._reference_context.append(self._end_ac_link_body(node))
 
     def _visit_reference_intern_uri(self, node):
         docname = posixpath.normpath(
             self.docparent + path.splitext(node['refuri'].split('#')[0])[0])
         doctitle = self.state.title(docname)
         if not doctitle:
             self.warn('unable to build link to document due to '
@@ -1300,15 +1384,15 @@
                     include_self=False, descend=False, siblings=True))
                 if isinstance(next_sibling, nodes.section):
                     next_sibling['section-embedded-anchor'] = anchor
                     raise nodes.SkipNode
 
             # only build an anchor if required (e.g. is a reference label
             # already provided by a build section element)
-            target_name = '{}#{}'.format(self.docname, anchor)
+            target_name = f'{self.docname}#{anchor}'
             target = self.state.target(target_name)
             if not target:
                 self.body.append(self._start_ac_macro(node, 'anchor'))
                 self.body.append(self._build_ac_param(node, '', anchor))
                 self.body.append(self._end_ac_macro(node, suffix=''))
         elif 'ids' in node and 'refuri' not in node:
             for id_ in node['ids']:
@@ -1374,24 +1458,42 @@
                 self.body.append(self._start_tag(node, 'div'))
             self.body.append(self._start_tag(node, 'em'))
             self.body.append('(')
 
             for idx, backref in enumerate(node['backrefs']):
                 if idx != 0:
                     self.body.append(', ')
-                self.body.append(self._start_ac_link(node, backref))
-                self.body.append(
-                    self._start_ac_plain_text_link_body_macro(node))
-                self.body.append(self._escape_cdata(str(idx + 1)))
-                self.body.append(self._end_ac_plain_text_link_body_macro(node))
-                self.body.append(self._end_ac_link(node))
+
+                if self.v2:
+                    attribs = {
+                        'href': f'#{backref}',
+                    }
+
+                    self.body.append(self._start_tag(node, 'a', **attribs))
+                    self.body.append(self._escape_cdata(str(idx + 1)))
+                    self.body.append(self._end_tag(node, suffix=''))
+                else:
+                    self.body.append(self._start_ac_link(node, backref))
+                    self.body.append(
+                        self._start_ac_plain_text_link_body_macro(node))
+                    self.body.append(self._escape_cdata(str(idx + 1)))
+                    self.body.append(self._end_ac_plain_text_link_body_macro(node))
+                    self.body.append(self._end_ac_link(node))
             self.body.append(')')
             self.body.append(self._end_tag(node, suffix=''))  # em
             if not self.v2:
                 self.body.append(self._end_tag(node))  # div
+        elif self.v2:
+            attribs = {
+                'href': '#' + node['backrefs'][0],
+            }
+
+            self.body.append(self._start_tag(node, 'a', **attribs))
+            self.body.append(self._escape_cdata(label_text))
+            self.body.append(self._end_tag(node, suffix=''))
         else:
             self.body.append(self._start_ac_link(node, node['backrefs'][0]))
             self.body.append(self._start_ac_plain_text_link_body_macro(node))
             self.body.append(self._escape_cdata(label_text))
             self.body.append(self._end_ac_plain_text_link_body_macro(node))
             self.body.append(self._end_ac_link(node))
 
@@ -1417,30 +1519,39 @@
                     node, 'hr', suffix=self.nl, empty=True))
             else:
                 self.body.append(self.context.pop())  # tbody
                 self.body.append(self.context.pop())  # table
             self._building_footnotes = False
 
     def visit_footnote_reference(self, node):
-        text = "[{}]".format(node.astext())
+        text = f"[{node.astext()}]"
 
         # build an anchor for back reference
         self.body.append(self._start_ac_macro(node, 'anchor'))
         self.body.append(self._build_ac_param(node, '', node['ids'][0]))
         self.body.append(self._end_ac_macro(node, suffix=''))
 
         # link to anchor
         target_anchor = ''.join(node['refid'].split())
 
         self.body.append(self._start_tag(node, 'sup'))
-        self.body.append(self._start_ac_link(node, target_anchor))
-        self.body.append(self._start_ac_plain_text_link_body_macro(node))
-        self.body.append(self._escape_cdata(text))
-        self.body.append(self._end_ac_plain_text_link_body_macro(node))
-        self.body.append(self._end_ac_link(node))
+        if self.v2:
+            attribs = {
+                'href': f'#{target_anchor}',
+            }
+
+            self.body.append(self._start_tag(node, 'a', **attribs))
+            self.body.append(self._escape_cdata(text))
+            self.body.append(self._end_tag(node, suffix=''))
+        else:
+            self.body.append(self._start_ac_link(node, target_anchor))
+            self.body.append(self._start_ac_plain_text_link_body_macro(node))
+            self.body.append(self._escape_cdata(text))
+            self.body.append(self._end_ac_plain_text_link_body_macro(node))
+            self.body.append(self._end_ac_link(node))
         self.body.append(self._end_tag(node, suffix=''))  # sup
         raise nodes.SkipNode
 
     def visit_label(self, node):
         # Label entries are skipped as their context has been already processed
         # from within footnote/citation processing (see visit_footnote).
         raise nodes.SkipNode
@@ -1496,14 +1607,23 @@
             has_added = True
         elif classes in [['accelerator']]:
             self.body.append(self._start_tag(node, 'u'))
             has_added = True
         elif classes in [['strike']]:
             self.body.append(self._start_tag(node, 's'))
             has_added = True
+        # [sphinxcontrib-needs]
+        # ignore collapse buttons, since they will not work in Confluence
+        elif 'needs_collapse' in classes:
+            raise nodes.SkipNode
+        # [sphinxcontrib-needs]
+        # strong text any title content
+        elif 'needs_title' in classes:
+            self.body.append(self._start_tag(node, 'strong'))
+            has_added = True
         elif isinstance(node.parent, addnodes.desc_parameter):
             # check if an identifier in signature
             if classes in [['n']]:
                 self.body.append(self._start_tag(node, 'em'))
                 has_added = True
 
         if has_added:
@@ -1591,28 +1711,28 @@
             self.context.append(self._end_tag(node))
 
         node.math_number = None
         if node.get('from_math') and node.get('number'):
             if self.builder.config.math_numfig and self.builder.config.numfig:
                 figtype = 'displaymath'
                 if self.builder.name == 'singleconfluence':
-                    key = '%s/%s' % (self._docnames[-1], figtype)
+                    key = f'{self._docnames[-1]}/{figtype}'
                 else:
                     key = figtype
 
                 id_ = node['ids'][0]
                 number = self.builder.fignumbers.get(key, {}).get(id_, ())
                 node.math_number = '.'.join(map(str, number))
             else:
                 node.math_number = node['number']
 
         if not self.v2 and node.math_number:
             self.body.append(self._start_tag(node, 'div',
                 **{'style': 'float: right'}))
-            self.body.append('({})'.format(node.math_number))
+            self.body.append(f'({node.math_number})')
             self.body.append(self._end_tag(node))
 
         attribs = {}
 
         alignment = self._fetch_alignment(node)
         if alignment:
             attribs['ac:align'] = alignment
@@ -1627,20 +1747,20 @@
         # if this in an internal (attached image) and a percentage is applied,
         # these length cannot be applied to the ac:width/height fields or a
         # macro render error can occur; instead, wrap the image around
         if opts['key'] and (hu == '%' or wu == '%'):
             style = 'display: inline-block;'
 
             if hu == '%':
-                style += 'height: {}%;'.format(height)
+                style += f'height: {height}%;'
                 height = None
                 hu = None
 
             if wu == '%':
-                style += 'width: {}%;'.format(width)
+                style += f'width: {width}%;'
                 width = None
                 wu = None
 
             self.body.append(self._start_tag(node, 'div', **{'style': style}))
             self.context.append(self._end_tag(node))
             node.__confluence_wrapped_img = True
 
@@ -1718,26 +1838,26 @@
 
         if self.v2 and node.math_number:
             self.body.append(self.context.pop())  # layout-cell
             self.body.append(self._start_tag(node, 'ac:layout-cell'))
 
             self.body.append(self._start_tag(node, 'p',
                 **{'style': 'text-align: right'}))
-            self.body.append('({})'.format(node.math_number))
+            self.body.append(f'({node.math_number})')
             self.body.append(self._end_tag(node))
 
             self.body.append(self._end_tag(node))  # layout-cell
             self.body.append(self.context.pop())  # ac:layout-section
             self.body.append(self.context.pop())  # ac:layout
 
     def visit_legend(self, node):
         attribs = {}
         alignment = self._fetch_alignment(node)
         if alignment and alignment != 'left':
-            attribs['style'] = 'text-align: {};'.format(alignment)
+            attribs['style'] = f'text-align: {alignment};'
 
         self.body.append(self._start_tag(node, 'div', **attribs))
         self.context.append(self._end_tag(node))
 
     def depart_legend(self, node):
         self.body.append(self.context.pop())  # div
 
@@ -1843,15 +1963,15 @@
             self.context.append(self._end_tag(node))
             self.body.append(self._start_tag(node, 'tr', suffix=self.nl))
             self.context.append(self._end_tag(node))
 
     def depart_hlist(self, node):
         if self.v2:
             # add empty sections to complete the three column requirement
-            for x in range(self._hlist_columns_left % 3):
+            for _ in range(self._hlist_columns_left % 3):
                 self.body.append(self._start_tag(node, 'ac:layout-cell'))
                 self.body.append(self._end_tag(node))
 
             self.body.append(self.context.pop())  # ac:layout-section
             self.body.append(self.context.pop())  # ac:layout
         else:
             self.body.append(self.context.pop())  # tr
@@ -1916,15 +2036,15 @@
 
         self.body.append(self._start_tag(node, 'pre'))
 
         for production in node:
             if production['tokenname']:
                 formatted_token = production['tokenname'].ljust(max_len)
                 formatted_token = self.encode(formatted_token)
-                self.body.append('{} ::='.format(formatted_token))
+                self.body.append(f'{formatted_token} ::=')
                 lastname = production['tokenname']
             else:
                 self.body.append('{}    '.format(' ' * len(lastname)))
             text = production.astext()
             text = self.encode(text)
             self.body.append(text + self.nl)
 
@@ -2283,20 +2403,20 @@
         if self.v2:
             assert not self._v2_marginals_partial
             self.body.append(self._start_tag(node, 'ac:layout-cell'))
 
             # v2: does not support font-size assignment; use sup tag
             # to make small
             self.body.append(self._start_tag(node, 'span', **{
-                'style': 'color: #707070;'
+                'style': 'color: #707070;',
             }))
             self.body.append(self._start_tag(node, 'sup'))
         else:
             self.body.append(self._start_tag(node, 'div', **{
-                'style': 'color: #707070; font-size: 12px;'
+                'style': 'color: #707070; font-size: 12px;',
             }))
 
         self.body.append(self.encode(
             L('This page has been automatically generated.')))
 
         if self.v2:
             self.body.append(self._end_tag(node, suffix=''))  # sup
@@ -2363,14 +2483,111 @@
 
             # flag that if any navnodes are created, additional
             # spacing is needed
             self._needs_navnode_spacing = True
 
         raise nodes.SkipNode
 
+    # ------------------------------------------
+    # confluence-builder -- enhancements -- card
+    # ------------------------------------------
+
+    def visit_confluence_doc_card(self, node):
+        # v1 editor does not support cards; contain in a panel to emulate a
+        # block feel
+        if not self.v2:
+            self.body.append(self._start_ac_macro(node, 'panel'))
+            self.body.append(self._start_ac_rich_text_body_macro(node))
+
+        docname = posixpath.normpath(self.docparent +
+            path.splitext(node.params['href'].split('#')[0])[0])
+        doctitle = self.state.title(docname)
+        if doctitle:
+            attribs = {}
+
+            if 'data-card-appearance' in node.params:
+                attribs['ac:card-appearance'] = \
+                    node.params['data-card-appearance']
+
+            if 'data-layout' in node.params:
+                attribs['ac:layout'] = node.params['data-layout']
+
+            if 'data-width' in node.params:
+                attribs['ac:width'] = node.params['data-width']
+
+            doctitle = self.encode(doctitle)
+            self.body.append(self._start_tag(node, 'ac:link', **attribs))
+            self.body.append(self._start_tag(node, 'ri:page',
+                suffix=self.nl, empty=True, **{'ri:content-title': doctitle}))
+            self.body.append(self._end_tag(node, suffix=''))
+        else:
+            self.warn('unable to build link to document card due to '
+                'missing title (in {}): {}'.format(self.docname, docname))
+            self.body.append(node.astext())
+
+        if not self.v2:
+            self.body.append(self._end_ac_rich_text_body_macro(node))
+            self.body.append(self._end_ac_macro(node))  # panel
+
+        raise nodes.SkipNode
+
+    def visit_confluence_doc_card_inline(self, node):
+        docname = posixpath.normpath(self.docparent +
+            path.splitext(node['reftarget'].split('#')[0])[0])
+        doctitle = self.state.title(docname)
+        if doctitle:
+            doctitle = self.encode(doctitle)
+            self.body.append(self._start_ac_link(node, appearance='inline'))
+            self.body.append(self._start_tag(node, 'ri:page',
+                suffix=self.nl, empty=True, **{'ri:content-title': doctitle}))
+            self.body.append(self._start_ac_link_body(node))
+            self.body.append(node.astext())
+            self.body.append(self._end_ac_link_body(node))
+            self.body.append(self._end_ac_link(node))
+        else:
+            self.warn('unable to build link to document card due to '
+                'missing title (in {}): {}'.format(self.docname, docname))
+            self.body.append(node.astext())
+
+        raise nodes.SkipNode
+
+    def visit_confluence_link_card(self, node):
+        options = dict(node.params)
+        url = self.encode(options.pop('href'))
+        options['href'] = url
+
+        # v1 editor does not support cards; contain in a panel to emulate a
+        # block feel
+        if not self.v2:
+            self.body.append(self._start_ac_macro(node, 'panel'))
+            self.body.append(self._start_ac_rich_text_body_macro(node))
+
+        self.body.append(self._start_tag(node, 'a', **options))
+        self.body.append(url)
+        self.body.append(self._end_tag(node, suffix=''))
+
+        if not self.v2:
+            self.body.append(self._end_ac_rich_text_body_macro(node))
+            self.body.append(self._end_ac_macro(node))  # panel
+
+        raise nodes.SkipNode
+
+    def visit_confluence_link_card_inline(self, node):
+        # raw href | give it an inline card appearance
+        attribs = {
+            'data-card-appearance': 'inline',
+            'href': self.encode(node.params['href']),
+        }
+
+        self.body.append(self._start_tag(node, 'a', **attribs))
+        self.body.append(attribs['href'])
+        self.body.append(self._end_tag(node, suffix=''))
+
+        raise nodes.SkipNode
+
     # ----------------------------------------------
     # confluence-builder -- enhancements -- emoticon
     # ----------------------------------------------
 
     def visit_confluence_emoticon_inline(self, node):
         self.body.append(self._start_tag(node, 'ac:emoticon', empty=True,
             **{'ac:name': self.encode(node.rawsource)}))
@@ -2385,27 +2602,27 @@
         latex_content = node.rawsource
 
         # if this block is numbered, attempt to align in on the following macro
         if node.get('from_math') and node.get('number'):
             if self.builder.config.math_numfig and self.builder.config.numfig:
                 figtype = 'displaymath'
                 if self.builder.name == 'singleconfluence':
-                    key = '%s/%s' % (self._docnames[-1], figtype)
+                    key = f'{self._docnames[-1]}/{figtype}'
                 else:
                     key = figtype
 
                 id_ = node['ids'][0]
                 number = self.builder.fignumbers.get(key, {}).get(id_, ())
                 number = '.'.join(map(str, number))
             else:
                 number = node['number']
 
             self.body.append(self._start_tag(node, 'div',
                 **{'style': 'float: right'}))
-            self.body.append('({})'.format(number))
+            self.body.append(f'({number})')
             self.body.append(self._end_tag(node))
 
         self.body.append(self._start_ac_macro(node, macro))
         if param is not None:
             latex_content = self.encode(latex_content)
             self.body.append(self._build_ac_param(node, param, latex_content))
         else:
@@ -2606,15 +2823,15 @@
             width = convert_length(width, wu)
             if width is None:
                 self.warn('unsupported unit type for confluence: ' + wu)
 
         attribs = {}
         alignment = self._fetch_alignment(node)
         if alignment and alignment != 'left':
-            attribs['style'] = 'text-align: {};'.format(alignment)
+            attribs['style'] = f'text-align: {alignment};'
 
         ri_url = self._start_tag(
             node, 'ri:url', empty=True, **{'ri:value': self.encode(uri)})
 
         self.body.append(self._start_tag(node, 'div', **attribs))
         self.body.append(self._start_ac_macro(node, 'widget'))
         self.body.append(self._build_ac_param(node, 'url', ri_url))
@@ -2656,16 +2873,22 @@
         self.body.append(self._start_tag(node, 'acronym'))
         self.context.append(self._end_tag(node, suffix=''))
 
     def depart_acronym(self, node):
         self.body.append(self.context.pop())  # acronym
 
     def visit_container(self, node):
-        self.body.append(self._start_tag(node, 'div'))
-        self.context.append(self._end_tag(node))
+        if 'collapse' in node.get('classes', []):
+            self.body.append(self._start_ac_macro(node, 'expand'))
+            self.body.append(self._start_ac_rich_text_body_macro(node))
+            self.context.append(self._end_ac_rich_text_body_macro(node) +
+                self._end_ac_macro(node))
+        else:
+            self.body.append(self._start_tag(node, 'div'))
+            self.context.append(self._end_tag(node))
 
     def depart_container(self, node):
         self.body.append(self.context.pop())  # div
 
     def depart_line(self, node):
         next_sibling = first(findall(node,
             include_self=False, descend=False, siblings=True))
@@ -2681,15 +2904,15 @@
         else:
             tag = 'div'
 
             # if this line-block is not the first element in the parent and the
             # parent is not a line-block, add some separation from a previous
             # sibling element
             if node.parent[0] != node and not isinstance(node.parent, nodes.line_block):
-                style += 'padding-top: {}px;'.format(FCMMO)
+                style += f'padding-top: {FCMMO}px;'
 
         # indent this line-block if its not the first element in the parent
         # (excluding titles for a new section), or if the parent is
         # also a line-block
         if (node.parent[0] != node and
                 not isinstance(node.parent[0], nodes.title)) or \
                 isinstance(node.parent, nodes.line_block):
@@ -2697,15 +2920,15 @@
             indent = INDENT
 
             # if v2, apply additional indentation (if needed)
             # (see "visit_paragraph")
             if self.v2:
                 indent = INDENT * (self._indent_level + 1)
 
-            style += 'margin-left: {}px;'.format(indent)
+            style += f'margin-left: {indent}px;'
         elif self.v2:
             # (see "visit_paragraph")
             style += 'margin-left: {}px;'.format(INDENT * self._indent_level)
 
         if style:
             attribs['style'] = style
 
@@ -2764,15 +2987,15 @@
         data = [tag]
 
         attribs = {}
         for key, value in kwargs.items():
             attribs[key.lower()] = value
 
         for key, value in sorted(attribs.items()):
-            data.append('{}="{}"'.format(key, value))
+            data.append(f'{key}="{value}"')
 
         if suffix is None:
             suffix = ''
 
         suffix = '>' + suffix
         if empty:
             suffix = ' /' + suffix
@@ -2804,15 +3027,15 @@
             tag = node.__confluence_tag.pop()
         except IndexError:
             raise ConfluenceError('end tag invoke without matching start tag')
 
         if suffix is None:
             suffix = self.nl
 
-        return '</{}>{}'.format(tag, suffix)
+        return f'</{tag}>{suffix}'
 
     def _build_ac_param(self, node, name, value):
         """
         generates a confluence parameter element
 
         A helper used to return content to be appended to a document which
         builds a complete storage format parameter element. The 'ac:parameter'
@@ -2859,33 +3082,36 @@
             node: the node processing the image
 
         Returns:
             the content
         """
         return self._end_tag(node, suffix='')
 
-    def _start_ac_link(self, node, anchor=None):
+    def _start_ac_link(self, node, anchor=None, appearance=None):
         """
         generates a confluence link start tag
 
         A helper used to return content to be appended to a document which
         initializes the start of a storage format link element of a specific
         `type`. The 'ac:link' element will be initialized. This method may use
         provided `node` to tweak the final content.
 
         Args:
             node: the node processing the link
             anchor (optional): the anchor value to use (defaults to None)
+            appearance (optional): card appearance to use (defaults to None)
 
         Returns:
             the content
         """
         attribs = {}
         if anchor:
             attribs['ac:anchor'] = anchor
+        if appearance:
+            attribs['ac:card-appearance'] = appearance
         return self._start_tag(node, 'ac:link', suffix=self.nl, **attribs)
 
     def _end_ac_link(self, node):
         """
         generates confluence link end tag content for a node
 
         A helper used to return content to be appended to a document which
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/svg.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from hashlib import sha256
 from sphinx.util.images import guess_mimetype
 from sphinx.util.osutil import ensuredir
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.util import convert_length
 from sphinxcontrib.confluencebuilder.util import extract_length
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/translator.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from docutils.nodes import NodeVisitor as BaseTranslator
 from os import path
 from sphinx.util.images import get_image_size
 from sphinx.util.images import guess_mimetype
 from sphinx.util.osutil import SEP
@@ -14,15 +11,14 @@
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger
 from sphinxcontrib.confluencebuilder.std.sphinx import DEFAULT_ALIGNMENT
 from sphinxcontrib.confluencebuilder.std.sphinx import DEFAULT_HIGHLIGHT_STYLE
 from sphinxcontrib.confluencebuilder.svg import confluence_supported_svg
 from sphinxcontrib.confluencebuilder.util import convert_length
 from sphinxcontrib.confluencebuilder.util import extract_length
 from sphinxcontrib.confluencebuilder.util import remove_nonspace_control_chars
-import io
 import sys
 
 
 class ConfluenceBaseTranslator(BaseTranslator):
     _tracked_deprecated_raw_type = False
 
     """
@@ -91,65 +87,73 @@
 
         # prepend header (if any)
         if self.builder.config.confluence_header_file is not None:
             header_template_data = ''
             header_file = path.join(self.builder.env.srcdir,
                 self.builder.config.confluence_header_file)
             try:
-                with io.open(header_file, encoding='utf-8') as file:
+                with open(header_file, encoding='utf-8') as file:
                     header_template_data = file.read()
             except (IOError, OSError) as err:
-                self.warn('error reading file {}: {}'.format(header_file, err))
+                self.warn(f'error reading file {header_file}: {err}')
 
             # if no data is supplied, the file is plain text
             if self.builder.config.confluence_header_data is None:
                 header = header_template_data
             else:
                 header = self.builder.templates.render_string(
                     header_template_data,
                     self.builder.config.confluence_header_data)
 
             self.body_final += header + self.nl
 
+        self.body_final += self.pre_body_data()
         self.body_final += ''.join(self.body)
+        self.body_final += self.post_body_data()
 
         # append footer (if any)
         if self.builder.config.confluence_footer_file is not None:
             footer_template_data = ''
             footer_file = path.join(self.builder.env.srcdir,
                 self.builder.config.confluence_footer_file)
             try:
-                with io.open(footer_file, encoding='utf-8') as file:
+                with open(footer_file, encoding='utf-8') as file:
                     footer_template_data = file.read()
             except (IOError, OSError) as err:
-                self.warn('error reading file {}: {}'.format(footer_file, err))
+                self.warn(f'error reading file {footer_file}: {err}')
 
             # if no data is supplied, the file is plain text
             if self.builder.config.confluence_footer_data is None:
                 footer = footer_template_data
             else:
                 footer = self.builder.templates.render_string(
                     footer_template_data,
                     self.builder.config.confluence_footer_data)
 
             self.body_final += footer + self.nl
 
+    def pre_body_data(self):
+        return ''
+
+    def post_body_data(self):
+        return ''
+
     def visit_Text(self, node):
         text = node.astext()
         if not self._literal:
             text = text.replace(self.nl, ' ')
         text = self.encode(text)
         self.body.append(text)
         raise nodes.SkipNode
 
     def unknown_visit(self, node):
         node_name = node.__class__.__name__
         ignore_nodes = self.builder.config.confluence_adv_ignore_nodes
         if node_name in ignore_nodes:
-            self.verbose('ignore node {} (conf)'.format(node_name))
+            self.verbose(f'ignore node {node_name} (conf)')
             raise nodes.SkipNode
 
         # allow users to override unknown nodes
         #
         # A node handler allows an advanced user to provide implementation to
         # process a node not supported by this extension. This is to assist in
         # providing a quick alternative to supporting another third party
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from os import path
 from sphinx.util.math import wrap_displaymath
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger
 from sphinxcontrib.confluencebuilder.nodes import confluence_latex_block
@@ -288,15 +285,15 @@
                 continue
 
             new_node = nodes.image(candidates={'?'}, uri=out_filename)
             if 'align' in node:
                 new_node['align'] = node['align']
             node.replace_self(new_node)
         except GraphvizError as exc:
-            ConfluenceLogger.warn('dot code {}: {}'.format(dotcode, exc))
+            ConfluenceLogger.warn(f'dot code {dotcode}: {exc}')
             node.parent.remove(node)
 
 
 def replace_math_blocks(builder, doctree):
     """
     replace math blocks with images
 
@@ -318,15 +315,15 @@
     # convert math blocks into Confluence LaTeX blocks
     for node in itertools.chain(findall(doctree, nodes.math),
             findall(doctree, nodes.math_block)):
         if not isinstance(node, nodes.math):
             if node['nowrap']:
                 latex = node.astext()
             else:
-                latex = wrap_displaymath(node.astext(), None, False)
+                latex = wrap_displaymath(node.astext(), None, numbering=False)
             new_node_type = confluence_latex_block
         else:
             latex = '$' + node.astext() + '$'
             new_node_type = confluence_latex_inline
 
         new_node = new_node_type(latex, latex, **node.attributes)
         new_node['from_math'] = True
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 
 # ##############################################################################
 # disable import/except warnings for third-party modules
 # pylint: disable=E
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 import itertools
 
 # ##############################################################################
 # disable import/except warnings for third-party modules
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger
 
 # ##############################################################################
 # disable import/except warnings for third-party modules
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 
 # ##############################################################################
 # disable import/except warnings for third-party modules
 # pylint: disable=E
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from os import path
 from sphinx import addnodes
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.nodes import confluence_expand
 from sphinxcontrib.confluencebuilder.util import first
@@ -94,17 +91,17 @@
             node = first(itertools.chain(
                 findall(doctree, sphinx_toolbox_IssueNode),
                 findall(doctree, sphinx_toolbox_IssueNodeWithName)))
             if not node:
                 break
 
             if isinstance(node, sphinx_toolbox_IssueNodeWithName):
-                title = '{}#{}'.format(node.repo_name, node.issue_number)
+                title = f'{node.repo_name}#{node.issue_number}'
             else:
-                title = '#{}'.format(node.issue_number)
+                title = f'#{node.issue_number}'
 
             new_node = nodes.reference(title, title, refuri=node.issue_url)
             node.replace_self(new_node)
 
     if sphinx_toolbox_github_repos_and_users:
         for node in findall(doctree, sphinx_toolbox_GitHubObjectLinkNode):
             new_node = nodes.reference(node.name, node.name, refuri=node.url)
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2021-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import nodes
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger
 
 # ##############################################################################
 # disable import/except warnings for third-party modules
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/util.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2018-2023 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from contextlib import contextmanager
 from sphinxcontrib.confluencebuilder.std.confluence import API_REST_BIND_PATH
 from sphinxcontrib.confluencebuilder.std.confluence import FONT_SIZE
 from sphinxcontrib.confluencebuilder.std.confluence import FONT_X_HEIGHT
 from hashlib import sha256
 import getpass
@@ -22,14 +19,30 @@
     """
     confluence utility helper class
 
     This class is used to hold a series of utility methods.
     """
 
     @staticmethod
+    def hash(data):
+        """
+        generate a hash of the provided string
+
+        Calculate a hash for a string. When publishing Confluence pages, hashes
+        can be used to check if pages needs to be uploaded again.
+
+        Args:
+            data: the raw string
+
+        Returns:
+            the hash
+        """
+        return sha256(data.encode()).hexdigest()
+
+    @staticmethod
     def hash_asset(asset):
         """
         generate a hash of the provided asset
 
         Calculate a hash for an asset file (e.g. an image file). When publishing
         assets as attachments for a Confluence page, hashes can be used to check
         if an attachment needs to be uploaded again.
```

### Comparing `sphinxcontrib-confluencebuilder-2.0.0/sphinxcontrib/confluencebuilder/writer.py` & `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/writer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# -*- coding: utf-8 -*-
-"""
-:copyright: Copyright 2016-2022 Sphinx Confluence Builder Contributors (AUTHORS)
-:license: BSD-2-Clause (LICENSE)
-"""
+# SPDX-License-Identifier: BSD-2-Clause
+# Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from docutils import writers
 
 
 class ConfluenceWriter(writers.Writer):
     supported = ('text',)
     settings_spec = ('No options here.', '', ())
```

