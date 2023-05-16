# Comparing `tmp/py42-1.8.2.tar.gz` & `tmp/py42-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py42-1.8.2.tar", last modified: Thu Oct  1 16:39:59 2020, max compression
+gzip compressed data, was "dist/py42-1.9.0.tar", last modified: Fri Oct  2 15:13:29 2020, max compression
```

## Comparing `py42-1.8.2.tar` & `py42-1.9.0.tar`

### file list

```diff
@@ -1,93 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.677040 py42-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (116)    31925 2020-10-01 16:39:47.000000 py42-1.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-10-01 16:39:47.000000 py42-1.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)       74 2020-10-01 16:39:47.000000 py42-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8125 2020-10-01 16:39:59.677040 py42-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5703 2020-10-01 16:39:47.000000 py42-1.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      436 2020-10-01 16:39:59.677040 py42-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1859 2020-10-01 16:39:47.000000 py42-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.661040 py42-1.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.665040 py42-1.8.2/src/py42/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)      594 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/clients/
--rw-r--r--   0 runner    (1001) docker     (116)      155 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11185 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/_archive_access.py
--rw-r--r--   0 runner    (1001) docker     (116)     6196 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/alertrules.py
--rw-r--r--   0 runner    (1001) docker     (116)     2448 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/alerts.py
--rw-r--r--   0 runner    (1001) docker     (116)     9103 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/archive.py
--rw-r--r--   0 runner    (1001) docker     (116)      254 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/authority.py
--rw-r--r--   0 runner    (1001) docker     (116)     5126 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/detectionlists.py
--rw-r--r--   0 runner    (1001) docker     (116)    17182 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/clients/securitydata.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/constants/
--rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5850 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4167 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/response.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/sdk/
--rw-r--r--   0 runner    (1001) docker     (116)    10656 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/sdk/queries/
--rw-r--r--   0 runner    (1001) docker     (116)      754 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/sdk/queries/alerts/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2036 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/alerts/alert_query.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/sdk/queries/alerts/filters/
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/alerts/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5432 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/alerts/filters/alert_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.669040 py42-1.8.2/src/py42/sdk/queries/fileevents/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6510 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/file_event_query.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.673040 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/
--rw-r--r--   0 runner    (1001) docker     (116)      510 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      423 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/activity_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1823 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/cloud_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)      995 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/device_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/email_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3695 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/event_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     4721 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/exposure_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2243 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/file_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)      344 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/fileevents/filters/print_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)    20218 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/sdk/queries/query_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.673040 py42-1.8.2/src/py42/services/
--rw-r--r--   0 runner    (1001) docker     (116)      579 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1193 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/_auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     7871 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/_connection.py
--rw-r--r--   0 runner    (1001) docker     (116)      405 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/_keyvaluestore.py
--rw-r--r--   0 runner    (1001) docker     (116)      741 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/administration.py
--rw-r--r--   0 runner    (1001) docker     (116)     4748 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/alertrules.py
--rw-r--r--   0 runner    (1001) docker     (116)     4467 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/alerts.py
--rw-r--r--   0 runner    (1001) docker     (116)     4548 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.677040 py42-1.8.2/src/py42/services/detectionlists/
--rw-r--r--   0 runner    (1001) docker     (116)      502 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/detectionlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7792 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/detectionlists/departing_employee.py
--rw-r--r--   0 runner    (1001) docker     (116)     6650 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/detectionlists/high_risk_employee.py
--rw-r--r--   0 runner    (1001) docker     (116)     6630 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/detectionlists/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (116)    11222 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/devices.py
--rw-r--r--   0 runner    (1001) docker     (116)     1533 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/fileevent.py
--rw-r--r--   0 runner    (1001) docker     (116)    14330 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/legalhold.py
--rw-r--r--   0 runner    (1001) docker     (116)     7566 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/orgs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1054 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/preservationdata.py
--rw-r--r--   0 runner    (1001) docker     (116)     2174 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/savedsearch.py
--rw-r--r--   0 runner    (1001) docker     (116)      281 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/securitydata.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.677040 py42-1.8.2/src/py42/services/storage/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2092 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/storage/_auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     3297 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/storage/_service_factory.py
--rw-r--r--   0 runner    (1001) docker     (116)     4808 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/storage/archive.py
--rw-r--r--   0 runner    (1001) docker     (116)     1733 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/storage/preservationdata.py
--rw-r--r--   0 runner    (1001) docker     (116)     2554 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/storage/securitydata.py
--rw-r--r--   0 runner    (1001) docker     (116)    11866 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/users.py
--rw-r--r--   0 runner    (1001) docker     (116)      457 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/services/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.677040 py42-1.8.2/src/py42/settings/
--rw-r--r--   0 runner    (1001) docker     (116)      605 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      494 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/settings/debug.py
--rw-r--r--   0 runner    (1001) docker     (116)      584 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/usercontext.py
--rw-r--r--   0 runner    (1001) docker     (116)     2108 2020-10-01 16:39:47.000000 py42-1.8.2/src/py42/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-01 16:39:59.665040 py42-1.8.2/src/py42.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8125 2020-10-01 16:39:59.000000 py42-1.8.2/src/py42.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2603 2020-10-01 16:39:59.000000 py42-1.8.2/src/py42.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-01 16:39:59.000000 py42-1.8.2/src/py42.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-01 16:39:59.000000 py42-1.8.2/src/py42.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      100 2020-10-01 16:39:59.000000 py42-1.8.2/src/py42.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-10-01 16:39:59.000000 py42-1.8.2/src/py42.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      801 2020-10-01 16:39:47.000000 py42-1.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.483379 py42-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)    34223 2020-10-02 15:13:22.000000 py42-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-10-02 15:13:22.000000 py42-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (116)       74 2020-10-02 15:13:22.000000 py42-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8125 2020-10-02 15:13:29.483379 py42-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5703 2020-10-02 15:13:22.000000 py42-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      436 2020-10-02 15:13:29.483379 py42-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1859 2020-10-02 15:13:22.000000 py42-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.467379 py42-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.471379 py42-1.9.0/src/py42/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      739 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/clients/
+-rw-r--r--   0 runner    (1001) docker     (116)      224 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11185 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/_archive_access.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6196 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/alertrules.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3103 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9103 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/archive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4605 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/auditlogs.py
+-rw-r--r--   0 runner    (1001) docker     (116)      254 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/authority.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5130 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/detectionlists.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17318 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/securitydata.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/clients/settings/
+-rw-r--r--   0 runner    (1001) docker     (116)     5464 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1445 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/settings/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20263 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/settings/device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13790 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/clients/settings/org_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/constants/
+-rw-r--r--   0 runner    (1001) docker     (116)      311 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6458 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4167 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/response.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/sdk/
+-rw-r--r--   0 runner    (1001) docker     (116)    11735 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/sdk/queries/
+-rw-r--r--   0 runner    (1001) docker     (116)      883 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/sdk/queries/alerts/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2036 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/alerts/alert_query.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/sdk/queries/alerts/filters/
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/alerts/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5608 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/alerts/filters/alert_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.475379 py42-1.9.0/src/py42/sdk/queries/fileevents/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7317 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/file_event_query.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.479379 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/
+-rw-r--r--   0 runner    (1001) docker     (116)      510 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      423 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/activity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1827 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/cloud_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      995 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/device_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/email_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3750 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4737 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/exposure_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2247 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      344 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/fileevents/filters/print_filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19971 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/sdk/queries/query_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.479379 py42-1.9.0/src/py42/services/
+-rw-r--r--   0 runner    (1001) docker     (116)      601 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1396 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7871 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/_keyvaluestore.py
+-rw-r--r--   0 runner    (1001) docker     (116)      741 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/administration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4748 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/alertrules.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4151 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4548 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/archive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2665 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/auditlogs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.479379 py42-1.9.0/src/py42/services/detectionlists/
+-rw-r--r--   0 runner    (1001) docker     (116)      502 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/detectionlists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8188 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/detectionlists/departing_employee.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6654 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/detectionlists/high_risk_employee.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6630 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/detectionlists/user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12116 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/devices.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1533 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/fileevent.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14330 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/legalhold.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9782 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/orgs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1054 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/preservationdata.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/savedsearch.py
+-rw-r--r--   0 runner    (1001) docker     (116)      281 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/securitydata.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.479379 py42-1.9.0/src/py42/services/storage/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2092 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/storage/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3297 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/storage/_service_factory.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4808 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/storage/archive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1733 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/storage/preservationdata.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2441 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/storage/securitydata.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11866 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/users.py
+-rw-r--r--   0 runner    (1001) docker     (116)      457 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/services/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.483379 py42-1.9.0/src/py42/settings/
+-rw-r--r--   0 runner    (1001) docker     (116)      638 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      494 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/settings/debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)      584 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/usercontext.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3694 2020-10-02 15:13:22.000000 py42-1.9.0/src/py42/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-02 15:13:29.471379 py42-1.9.0/src/py42.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8125 2020-10-02 15:13:29.000000 py42-1.9.0/src/py42.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2830 2020-10-02 15:13:29.000000 py42-1.9.0/src/py42.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-02 15:13:29.000000 py42-1.9.0/src/py42.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-02 15:13:29.000000 py42-1.9.0/src/py42.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      100 2020-10-02 15:13:29.000000 py42-1.9.0/src/py42.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2020-10-02 15:13:29.000000 py42-1.9.0/src/py42.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      801 2020-10-02 15:13:22.000000 py42-1.9.0/tox.ini
```

### Comparing `py42-1.8.2/CHANGELOG.md` & `py42-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,65 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 The intended audience of this file is for py42 consumers -- as such, changes that don't affect
 how a consumer would use the library (e.g. adding unit tests, updating documentation, etc) are not captured here.
 
+## 1.9.0 - 2020-10-02
+
+### Changed
+
+- The following methods now support string timestamp formats (`yyyy-MM-dd HH:MM:SS`) as well as a `datetime` instance:
+    - `sdk.auditlogs.get_page()`, arguments `begin_time` and `end_time`.
+    - `sdk.auditlogs.get_all()`, arguments `begin_time` and `end_time`.
+    - `sdk.securitydata.get_all_plan_security_events()`, arguments `min_timestamp` and `max_timestamp`.
+    - `sdk.securitydata.get_all_user_security_events()`, arguments `min_timestamp` and `max_timestamp`.
+
+- The `departure_date` parameter for methods:
+    - `sdk.detectionlists.departing_employee.add()`
+    - `sdk.detectionlists.departing_employee.update_departure_date()`
+    now support a `datetime` instance.
+
+- The following methods on timestamp-based query filters (e.g. `EventTimestamp`, `DateObserved`) now support string timestamp format (`yyyy-MM-dd HH:MM:SS`) as well as a `datetime` instance:
+    - `on_or_before()`
+    - `or_or_after()`
+    - `in_range()`
+
+### Removed
+
+- Removed faulty `within_the_last()` method from `sdk.queries.alerts.filters.alert_filter.DateObserved`.
+
+### Added
+
+- Added additional user-adjustable setting for security events page size:
+    - `py42.settings.security_events_per_page`
+
+- Page page_number and page_size parameters for saved search queries:
+    - `py42.securitydata.savedsearches.get_query()`
+    - `py42.securitydata.savedsearches.execute()`
+
+- `sdk.alerts.update_state()` method to update state.
+
+- Support for two-factor authentication in `sdk.from_local_account()`
+
+- `OrgSettings` and `DeviceSettings` classes to help with Org and Device setting management.
+    - `sdk.orgs.get_settings(org_id)` now returns an instance of `OrgSettings` which can be used to view
+        existing Org settings and modify them by passing the updated `OrgSettings` object to `sdk.orgs.update_settings()`
+    - `sdk.devices.get_settings(org_id)` now returns an instance of `DeviceSettings` which can be used to view
+        existing Device settings and modify them by passing the updated `DeviceSettings` object to `sdk.devices.update_settings()`
+
+- `sdk.auditlogs` method:
+    - `sdk.auditlogs.get_page()`
+    - `sdk.auditlogs.get_all()`
+
+### Changed
+
+- `py42.sdk.queries.query_filter.filter_attributes` renamed to `py42.util.get_attribute_keys_from_class`
+
 ## 1.8.2 - 2020-09-30
 
 ### Fixed
 
 - Corrected an issue that caused `sdk.detectionlists.departing_employee.get_all()`
   and `sdk.detectionslists.high_risk_employee.get_all()` to only return the first page (first 100) records. This same issue also caused other `get_all_X()` methods to only return the first page if the requested `page_size` was less than `settings.items_per_page`.
```

### Comparing `py42-1.8.2/LICENSE.md` & `py42-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/PKG-INFO` & `py42-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py42
-Version: 1.8.2
+Version: 1.9.0
 Summary: The Official Code42 Python API Client
 Home-page: https://github.com/code42/py42
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/code42/py42/issues
 Project-URL: Documentation, https://py42docs.code42.com/
 Project-URL: Source Code, https://github.com/code42/py42
 Description:
```

### Comparing `py42-1.8.2/README.md` & `py42-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/setup.py` & `py42-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/clients/_archive_access.py` & `py42-1.9.0/src/py42/clients/_archive_access.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/clients/alertrules.py` & `py42-1.9.0/src/py42/clients/alertrules.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/clients/alerts.py` & `py42-1.9.0/src/py42/clients/alerts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from py42.sdk.queries.alerts.filters import AlertState
+
+
 class AlertsClient(object):
     def __init__(self, alert_service, alert_rules_client):
         self._alert_service = alert_service
         self._alert_rules_client = alert_rules_client
 
     @property
     def rules(self):
@@ -45,20 +48,35 @@
         Args:
             alert_ids (iter[str]): The identification numbers for the alerts to resolve.
             reason (str, optional): The reason the alerts are now resolved. Defaults to None.
 
         Returns:
             :class:`py42.response.Py42Response`
         """
-        return self._alert_service.resolve(alert_ids, reason=reason)
+        return self._alert_service.update_state(
+            AlertState.DISMISSED, alert_ids, note=reason
+        )
 
     def reopen(self, alert_ids, reason=None):
         """Reopens the resolved alerts with the given IDs.
 
         Args:
             alert_ids (iter[str]): The identification numbers for the alerts to reopen.
             reason (str, optional): The reason the alerts are reopened. Defaults to None.
 
         Returns:
             :class:`py42.response.Py42Response`
         """
-        return self._alert_service.reopen(alert_ids, reason=reason)
+        return self._alert_service.update_state(AlertState.OPEN, alert_ids, note=reason)
+
+    def update_state(self, status, alert_ids, note=None):
+        """Update status for given alert IDs.
+
+        Args:
+            status (str): Status to set from OPEN, RESOLVED, PENDING, IN_PROGRESS
+            alert_ids (iter[str]): The identification numbers for the alerts to reopen.
+            note (str, optional): User note regarding the status. Defaults to None.
+
+        Returns:
+            :class:`py42.response.Py42Response`
+        """
+        return self._alert_service.update_state(status, alert_ids, note=note)
```

### Comparing `py42-1.8.2/src/py42/clients/archive.py` & `py42-1.9.0/src/py42/clients/archive.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/clients/detectionlists.py` & `py42-1.9.0/src/py42/clients/detectionlists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from py42.sdk.queries.query_filter import filter_attributes
+from py42.util import get_attribute_keys_from_class
 
 
 class RiskTags(object):
     """The available RiskTags for :meth:`~py42.clients.detectionlists.DetectionListsClient.add_user_risk_tags()`
     and :meth:`~py42.clients.detectionlists.DetectionListsClient.remove_user_risk_tags()`"""
 
     FLIGHT_RISK = u"FLIGHT_RISK"
@@ -11,15 +11,15 @@
     PERFORMANCE_CONCERNS = u"PERFORMANCE_CONCERNS"
     SUSPICIOUS_SYSTEM_ACTIVITY = u"SUSPICIOUS_SYSTEM_ACTIVITY"
     POOR_SECURITY_PRACTICES = u"POOR_SECURITY_PRACTICES"
     CONTRACT_EMPLOYEE = u"CONTRACT_EMPLOYEE"
 
     @staticmethod
     def choices():
-        return filter_attributes(RiskTags)
+        return get_attribute_keys_from_class(RiskTags)
 
 
 class DetectionListsClient(object):
     def __init__(
         self,
         user_profile_service,
         departing_employee_service,
```

### Comparing `py42-1.8.2/src/py42/clients/securitydata.py` & `py42-1.9.0/src/py42/clients/securitydata.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,18 +98,18 @@
                         - ``RESTORE_FILE``
                         - ``FILE_OPENED``
                         - ``RULE_MATCH``
                         - ``DEVICE_SCAN_RESULT``
                         - ``PERSONAL_CLOUD_SCAN_RESULT``
 
                     Defaults to None.
-            min_timestamp (float, optional): A POSIX timestamp representing the beginning of the
-                date range of events to get. Defaults to None.
-            max_timestamp (float, optional): A POSIX timestamp representing the end of the date
-                range of events to get. Defaults to None.
+            min_timestamp (int or float or str or datetime, optional): Timestamp in milliseconds or
+                str format "yyyy-MM-DD HH:MM:SS" or a datetime instance. Defaults to None.
+            max_timestamp (int or float or str or datetime, optional): Timestamp in milliseconds or
+                str format "yyyy-MM-DD HH:MM:SS" or a datetime instance. Defaults to None.
 
         Returns:
             generator: An object that iterates over :class:`py42.response.Py42Response` objects
             that each contain a page of events.
         """
         return self._get_security_detection_events(
             plan_storage_info,
@@ -148,18 +148,18 @@
                         - ``RESTORE_FILE``
                         - ``FILE_OPENED``
                         - ``RULE_MATCH``
                         - ``DEVICE_SCAN_RESULT``
                         - ``PERSONAL_CLOUD_SCAN_RESULT``
 
                     Defaults to None.
-            min_timestamp (float, optional): A POSIX timestamp representing the beginning of the
-                date range of events to get. Defaults to None.
-            max_timestamp (float, optional): A POSIX timestamp representing the end of the date
-                range of events to get. Defaults to None.
+            min_timestamp (int or float or str or datetime, optional): Timestamp in milliseconds or
+                str format "yyyy-MM-DD HH:MM:SS" or a datetime instance. Defaults to None.
+            max_timestamp (int or float or str or datetime, optional): Timestamp in milliseconds or
+                str format "yyyy-MM-DD HH:MM:SS" or a datetime instance. Defaults to None.
 
         Returns:
             generator: An object that iterates over :class:`py42.response.Py42Response` objects
             that each contain a page of events.
         """
         security_plan_storage_infos = self.get_security_plan_storage_info_list(user_uid)
         return self._get_security_detection_events(
```

### Comparing `py42-1.8.2/src/py42/exceptions.py` & `py42-1.9.0/src/py42/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,21 +136,35 @@
         msg = u"Only alert rules with a source of 'Alerting' can be targeted by this command. "
         msg += u"Rule {0} has a source of '{1}'."
         super(Py42InvalidRuleOperationError, self).__init__(
             exception, msg.format(rule_id, source)
         )
 
 
+class Py42MFARequiredError(Py42UnauthorizedError):
+    """An exception raised when a request requires multi-factor authentication"""
+
+    def __init__(self, exception, message=None):
+        message = message or u"User requires multi-factor authentication."
+        super(Py42MFARequiredError, self).__init__(exception, message)
+
+
 def raise_py42_error(raised_error):
     """Raises the appropriate :class:`py42.exceptions.Py42HttpError` based on the given
     HTTPError's response status code.
     """
     if raised_error.response.status_code == 400:
         raise Py42BadRequestError(raised_error)
     elif raised_error.response.status_code == 401:
+        if raised_error.response.text:
+            if (
+                "TOTP_AUTH_CONFIGURATION_REQUIRED_FOR_USER"
+                or "TIME_BASED_ONE_TIME_PASSWORD_REQUIRED" in raised_error.response.text
+            ):
+                raise Py42MFARequiredError(raised_error)
         raise Py42UnauthorizedError(raised_error)
     elif raised_error.response.status_code == 403:
         raise Py42ForbiddenError(raised_error)
     elif raised_error.response.status_code == 404:
         raise Py42NotFoundError(raised_error)
     elif 500 <= raised_error.response.status_code < 600:
         raise Py42InternalServerError(raised_error)
```

### Comparing `py42-1.8.2/src/py42/response.py` & `py42-1.9.0/src/py42/response.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/sdk/__init__.py` & `py42-1.9.0/src/py42/sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from requests.auth import HTTPBasicAuth
 
 from py42.clients import Clients
 from py42.clients._archive_access import ArchiveAccessorManager
 from py42.clients.alertrules import AlertRulesClient
 from py42.clients.alerts import AlertsClient
 from py42.clients.archive import ArchiveClient
+from py42.clients.auditlogs import AuditLogsClient
 from py42.clients.authority import AuthorityClient
 from py42.clients.detectionlists import DetectionListsClient
 from py42.clients.securitydata import SecurityDataClient
 from py42.services import Services
 from py42.services._auth import V3Auth
 from py42.services._connection import Connection
-from py42.services._keyvaluestore import KeyValueStoreClient
+from py42.services._keyvaluestore import KeyValueStoreService
 from py42.services.administration import AdministrationService
 from py42.services.alertrules import AlertRulesService
 from py42.services.alerts import AlertService
 from py42.services.archive import ArchiveService
+from py42.services.auditlogs import AuditLogsService
 from py42.services.detectionlists.departing_employee import DepartingEmployeeService
 from py42.services.detectionlists.high_risk_employee import HighRiskEmployeeService
 from py42.services.detectionlists.user_profile import DetectionListUserService
 from py42.services.devices import DeviceService
 from py42.services.fileevent import FileEventService
 from py42.services.legalhold import LegalHoldService
 from py42.services.orgs import OrgService
@@ -28,63 +30,66 @@
 from py42.services.securitydata import SecurityDataService
 from py42.services.storage._service_factory import ConnectionManager
 from py42.services.storage._service_factory import StorageServiceFactory
 from py42.services.users import UserService
 from py42.usercontext import UserContext
 
 
-def from_local_account(host_address, username, password):
+def from_local_account(host_address, username, password, totp=None):
     """Creates a :class:`~py42.sdk.SDKClient` object for accessing the Code42 REST APIs using the
     supplied credentials. Currently, only accounts created within the Code42 console or using the
     APIs (including py42) are supported. Username/passwords that are based on Active Directory,
     Okta, or other Identity providers cannot be used with this method.
 
     Args:
         host_address (str): The domain name of the Code42 instance being authenticated to, e.g.
             console.us.code42.com
         username (str): The username of the authenticating account.
         password (str): The password of the authenticating account.
+        totp (callable or str, optional): The time-based one-time password of the authenticating account. Include only
+            if the account uses Code42's two-factor authentication. Defaults to None.
 
     Returns:
         :class:`py42.sdk.SDKClient`
     """
-    client = SDKClient.from_local_account(host_address, username, password)
+    client = SDKClient.from_local_account(host_address, username, password, totp)
 
     # test credentials
     client.users.get_current()
     return client
 
 
 class SDKClient(object):
     def __init__(self, main_connection, auth):
         services, user_ctx = _init_services(main_connection, auth)
         self._clients = _init_clients(services, main_connection)
         self._user_ctx = user_ctx
 
     @classmethod
-    def from_local_account(cls, host_address, username, password):
+    def from_local_account(cls, host_address, username, password, totp=None):
         """Creates a :class:`~py42.sdk.SDKClient` object for accessing the Code42 REST APIs using
         the supplied credentials. Currently, only accounts created within the Code42 console or
         using the APIs (including py42) are supported. Username/passwords that are based on Active
         Directory, Okta, or other Identity providers cannot be used with this method.
 
         Args:
             host_address (str): The domain name of the Code42 instance being authenticated to, e.g.
                 console.us.code42.com
             username (str): The username of the authenticating account.
             password (str): The password of the authenticating account.
-
+            totp (callable or str, optional): The time-based one-time password of the authenticating account. Include only
+                if the account uses Code42's two-factor authentication. Defaults to None.
         Returns:
             :class:`py42.sdk.SDKClient`
         """
         basic_auth = None
         if username and password:
             basic_auth = HTTPBasicAuth(username, password)
         auth_connection = Connection.from_host_address(host_address, auth=basic_auth)
-        v3_auth = V3Auth(auth_connection)
+        v3_auth = V3Auth(auth_connection, totp)
         main_connection = Connection.from_host_address(host_address, auth=v3_auth)
 
         return cls(main_connection, v3_auth)
 
     @property
     def serveradmin(self):
         """A collection of methods for getting server information for on-premise environments
@@ -182,25 +187,35 @@
         """A collection of methods related to retrieving and updating alerts rules.
 
         Returns:
             :class:`py42.services.alertrules.AlertRulesClient`
         """
         return self._clients.alerts
 
+    @property
+    def auditlogs(self):
+        """A collections of methods for retrieving audit logs.
+
+        Returns:
+            :class:`py42.services.auditlogs.AuditLogsService`
+        """
+        return self._clients.auditlogs
+
 
 def _init_services(main_connection, main_auth):
     alert_rules_key = u"FedObserver-API_URL"
     alerts_key = u"AlertService-API_URL"
     file_events_key = u"FORENSIC_SEARCH-API_URL"
     preservation_data_key = u"PRESERVATION-DATA-SERVICE_API-URL"
     employee_case_mgmt_key = u"employeecasemanagement-API_URL"
     kv_prefix = u"simple-key-value-store"
+    audit_logs_key = u"AUDIT-LOG_API-URL"
 
     kv_connection = Connection.from_microservice_prefix(main_connection, kv_prefix)
-    kv_service = KeyValueStoreClient(kv_connection)
+    kv_service = KeyValueStoreService(kv_connection)
 
     alert_rules_conn = Connection.from_microservice_key(
         kv_service, alert_rules_key, auth=main_auth
     )
     alerts_conn = Connection.from_microservice_key(
         kv_service, alerts_key, auth=main_auth
     )
@@ -209,15 +224,17 @@
     )
     pds_conn = Connection.from_microservice_key(
         kv_service, preservation_data_key, auth=main_auth
     )
     ecm_conn = Connection.from_microservice_key(
         kv_service, employee_case_mgmt_key, auth=main_auth
     )
-
+    audit_logs_conn = Connection.from_microservice_key(
+        kv_service, audit_logs_key, auth=main_auth
+    )
     user_svc = UserService(main_connection)
     administration_svc = AdministrationService(main_connection)
     file_event_svc = FileEventService(file_events_conn)
     user_ctx = UserContext(administration_svc)
     user_profile_svc = DetectionListUserService(ecm_conn, user_ctx, user_svc)
 
     services = Services(
@@ -234,14 +251,15 @@
         savedsearch=SavedSearchService(file_events_conn, file_event_svc),
         preservationdata=PreservationDataService(pds_conn),
         departingemployee=DepartingEmployeeService(
             ecm_conn, user_ctx, user_profile_svc
         ),
         highriskemployee=HighRiskEmployeeService(ecm_conn, user_ctx, user_profile_svc),
         userprofile=user_profile_svc,
+        auditlogs=AuditLogsService(audit_logs_conn),
     )
 
     return services, user_ctx
 
 
 def _init_clients(services, connection):
     authority = AuthorityClient(
@@ -269,15 +287,17 @@
         storage_service_factory,
     )
     alerts = AlertsClient(services.alerts, alertrules)
     archive_accessor_mgr = ArchiveAccessorManager(
         services.archive, storage_service_factory
     )
     archive = ArchiveClient(archive_accessor_mgr, services.archive)
+    auditlogs = AuditLogsClient(services.auditlogs)
     clients = Clients(
         authority=authority,
         detectionlists=detectionlists,
         alerts=alerts,
         securitydata=securitydata,
         archive=archive,
+        auditlogs=auditlogs,
     )
     return clients
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/__init__.py` & `py42-1.9.0/src/py42/sdk/queries/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from py42 import settings
 from py42.sdk.queries.query_filter import FilterGroup
 
 
 class BaseQuery(object):
     def __init__(self, *args, **kwargs):
         self._filter_group_list = list(args)
         self._group_clause = kwargs.get(u"group_clause", u"AND")
-        self.page_size = 10000
+        self.page_number = kwargs.get(u"page_number") or 1
+        self.page_size = kwargs.get(u"page_size") or settings.security_events_per_page
         self.sort_direction = u"asc"
 
         # Override
-        self.page_number = None
         self.sort_key = None
 
     @classmethod
-    def from_dict(cls, _dict, group_clause=u"AND"):
+    def from_dict(cls, _dict, group_clause=u"AND", **kwargs):
         filter_groups = [FilterGroup.from_dict(item) for item in _dict[u"groups"]]
-        return cls(*filter_groups, group_clause=group_clause)
+        return cls(*filter_groups, group_clause=group_clause, **kwargs)
 
     @classmethod
     def any(cls, *args):
         return cls(*args, group_clause=u"OR")
 
     @classmethod
     def all(cls, *args):
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/alerts/alert_query.py` & `py42-1.9.0/src/py42/sdk/queries/alerts/alert_query.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/sdk/queries/alerts/filters/alert_filter.py` & `py42-1.9.0/src/py42/sdk/queries/alerts/filters/alert_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from py42.sdk.queries.query_filter import create_filter_group
 from py42.sdk.queries.query_filter import create_query_filter
-from py42.sdk.queries.query_filter import filter_attributes
 from py42.sdk.queries.query_filter import QueryFilterStringField
 from py42.sdk.queries.query_filter import QueryFilterTimestampField
+from py42.util import get_attribute_keys_from_class
 
 
 def create_contains_filter_group(term, value):
     """Creates a :class:`~py42.sdk.queries.query_filter.FilterGroup` for filtering results
     where the value with key ``term`` contains the given value. Useful for creating ``CONTAINS``
     filters that are not yet supported in py42 or programmatically crafting filter groups.
 
@@ -112,15 +112,15 @@
 
     ALERTING = u"Alerting"
     DEPARTING_EMPLOYEE = u"Departing Employee"
     HIGH_RISK_EMPLOYEE = u"High Risk Employee"
 
     @staticmethod
     def choices():
-        return filter_attributes(RuleSource)
+        return get_attribute_keys_from_class(RuleSource)
 
 
 class RuleType(QueryFilterStringField):
     """Class that filters alerts based on rule type.
 
     Available options are:
         - :attr:`RuleType.ENDPOINT_EXFILTRATION`
@@ -132,15 +132,15 @@
 
     ENDPOINT_EXFILTRATION = u"FedEndpointExfiltration"
     CLOUD_SHARE_PERMISSIONS = u"FedCloudSharePermissions"
     FILE_TYPE_MISMATCH = u"FedFileTypeMismatch"
 
     @staticmethod
     def choices():
-        return filter_attributes(RuleType)
+        return get_attribute_keys_from_class(RuleType)
 
 
 class Description(AlertQueryFilterStringField):
     """Class that filters alerts based on rule description text."""
 
     _term = u"description"
 
@@ -158,26 +158,30 @@
 
     HIGH = u"HIGH"
     MEDIUM = u"MEDIUM"
     LOW = u"LOW"
 
     @staticmethod
     def choices():
-        return filter_attributes(Severity)
+        return get_attribute_keys_from_class(Severity)
 
 
 class AlertState(QueryFilterStringField):
     """Class that filters alerts based on alert state.
 
     Available options are:
         - :attr:`AlertState.OPEN`
         - :attr:`AlertState.DISMISSED`
+        - :attr:`AlertState.PENDING`
+        - :attr:`AlertState.IN_PROGRESS`
     """
 
     _term = u"state"
 
     OPEN = u"OPEN"
     DISMISSED = u"RESOLVED"
+    PENDING = u"PENDING"
+    IN_PROGRESS = u"IN_PROGRESS"
 
     @staticmethod
     def choices():
-        return filter_attributes(AlertState)
+        return get_attribute_keys_from_class(AlertState)
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/file_event_query.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/file_event_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from py42._compat import str
 from py42.sdk.queries import BaseQuery
 from py42.sdk.queries.query_filter import create_filter_group
 from py42.sdk.queries.query_filter import create_query_filter
+from py42.sdk.queries.query_filter import create_within_the_last_filter_group
 from py42.sdk.queries.query_filter import QueryFilterStringField
+from py42.sdk.queries.query_filter import QueryFilterTimestampField
 
 
 class FileEventQuery(BaseQuery):
     """Helper class for building Code42 Forensic Search queries.
 
     A FileEventQuery instance's ``all()`` and ``any()`` take one or more
     :class:`~py42.sdk.queries.query_filter.FilterGroup` objects to construct a query that
@@ -23,15 +25,14 @@
         query = FileEventQuery.all(email_filter, exposure_filter)
 
     """
 
     def __init__(self, *args, **kwargs):
         super(FileEventQuery, self).__init__(*args, **kwargs)
         self.sort_key = u"eventId"
-        self.page_number = 1
 
     def __str__(self):
         groups_string = u",".join(
             str(group_item) for group_item in self._filter_group_list
         )
         json = u'{{"groupClause":"{0}", "groups":[{1}], "pgNum":{2}, "pgSize":{3}, "srtDir":"{4}", "srtKey":"{5}"}}'.format(
             self._group_clause,
@@ -173,7 +174,24 @@
             value (str or int or float): The value used to filter file events.
 
         Returns:
             :class:`~py42.sdk.queries.query_filter.FilterGroup`
         """
         value = int(value)
         return create_less_than_filter_group(cls._term, value)
+
+
+class FileEventFilterTimestampField(QueryFilterTimestampField):
+    @classmethod
+    def within_the_last(cls, value):
+        """Returns a :class:`~py42.sdk.queries.query_filter.FilterGroup` that is useful
+        for finding results where the key ``self._term`` is a timestamp-related term,
+        such as ``EventTimestamp._term``, and ``value`` is one of it's accepted values,
+        such as one of the values in ``EventTimestamp.choices()``.
+
+        Args:
+            value (str): The value used to filter file events.
+
+        Returns:
+            :class:`~py42.sdk.queries.query_filter.FilterGroup`
+        """
+        return create_within_the_last_filter_group(cls._term, value)
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/filters/cloud_filter.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/filters/cloud_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from py42.sdk.queries.fileevents.file_event_query import FileEventFilterStringField
-from py42.sdk.queries.query_filter import filter_attributes
 from py42.sdk.queries.query_filter import QueryFilterBooleanField
+from py42.util import get_attribute_keys_from_class
 
 
 class Actor(FileEventFilterStringField):
     """Class that filters events by the cloud service username of the event originator
     (applies to cloud data source events only).
     """
 
@@ -49,8 +49,8 @@
 
     SHARED_VIA_LINK = u"SharedViaLink"
     IS_PUBLIC = u"IsPublic"
     OUTSIDE_TRUSTED_DOMAIN = u"OutsideTrustedDomains"
 
     @staticmethod
     def choices():
-        return filter_attributes(SharingTypeAdded)
+        return get_attribute_keys_from_class(SharingTypeAdded)
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/filters/device_filter.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/filters/device_filter.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/filters/email_filter.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/filters/email_filter.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/filters/event_filter.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/filters/event_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from py42.sdk.queries.fileevents.file_event_query import FileEventFilterStringField
-from py42.sdk.queries.query_filter import filter_attributes
+from py42.sdk.queries.fileevents.file_event_query import FileEventFilterTimestampField
 from py42.sdk.queries.query_filter import QueryFilterBooleanField
-from py42.sdk.queries.query_filter import QueryFilterTimestampField
+from py42.util import get_attribute_keys_from_class
 
 
-class EventTimestamp(QueryFilterTimestampField):
+class EventTimestamp(FileEventFilterTimestampField):
     """Class that filters events based on the timestamp of the event that occurred.
 
     Available event timestamp constants are provided as class attributes, These
     constants should be used only with class method `within_the_last`:
 
         - :attr:`EventTimestamp.FIFTEEN_MINUTES`
         - :attr:`EventTimestamp.ONE_HOUR`
@@ -34,15 +34,15 @@
     THREE_DAYS = u"P3D"
     SEVEN_DAYS = u"P7D"
     FOURTEEN_DAYS = u"P14D"
     THIRTY_DAYS = u"P30D"
 
     @staticmethod
     def choices():
-        return filter_attributes(EventTimestamp)
+        return get_attribute_keys_from_class(EventTimestamp)
 
 
 class EventType(FileEventFilterStringField):
     """Class that filters file events based on event type.
 
     Available event types are provided as class attributes:
 
@@ -66,18 +66,18 @@
     DELETED = u"DELETED"
     READ_BY_APP = u"READ_BY_APP"
     EMAILED = u"EMAILED"
     PRINTED = u"PRINTED"
 
     @staticmethod
     def choices():
-        return filter_attributes(EventType)
+        return get_attribute_keys_from_class(EventType)
 
 
-class InsertionTimestamp(QueryFilterTimestampField):
+class InsertionTimestamp(FileEventFilterTimestampField):
     """Class that filters events based on the timestamp of when the event was actually added to the
     event store (which can be after the event occurred on the device itself).
 
     `value` must be a POSIX timestamp. (see the :ref:`Dates <anchor_dates>` section of the Basics
     user guide for details on timestamp arguments in py42)
     """
 
@@ -108,15 +108,15 @@
     ONE_DRIVE = u"OneDrive"
     BOX = u"Box"
     GMAIL = u"Gmail"
     OFFICE_365 = u"Office365"
 
     @staticmethod
     def choices():
-        return filter_attributes(Source)
+        return get_attribute_keys_from_class(Source)
 
 
 class MimeTypeMismatch(QueryFilterBooleanField):
     """Class that filters events by whether or not a file's mime type matches its extension type."""
 
     _term = u"mimeTypeMismatch"
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/filters/exposure_filter.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/filters/exposure_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from py42.sdk.queries.fileevents.file_event_query import FileEventFilterStringField
-from py42.sdk.queries.query_filter import filter_attributes
+from py42.util import get_attribute_keys_from_class
 
 
 class ExposureType(FileEventFilterStringField):
     """Class that filters events based on exposure type.
 
     Available options are provided as class attributes:
         - :attr:`ExposureType.SHARED_VIA_LINK`
@@ -22,15 +22,15 @@
     CLOUD_STORAGE = u"CloudStorage"
     REMOVABLE_MEDIA = u"RemovableMedia"
     IS_PUBLIC = u"IsPublic"
     OUTSIDE_TRUSTED_DOMAINS = u"OutsideTrustedDomains"
 
     @staticmethod
     def choices():
-        return filter_attributes(ExposureType)
+        return get_attribute_keys_from_class(ExposureType)
 
 
 class ProcessName(FileEventFilterStringField):
     """Class that filters events based on the process name involved in the exposure (applies to
     ``read by browser or other app`` events only).
     """
 
@@ -117,15 +117,15 @@
     GOOGLE_DRIVE = u"GoogleDrive"
     GOOGLE_BACKUP_AND_SYNC = u"GoogleBackupAndSync"
     DROPBOX = u"Dropbox"
     ONEDRIVE = u"OneDrive"
 
     @staticmethod
     def choices():
-        return filter_attributes(SyncDestination)
+        return get_attribute_keys_from_class(SyncDestination)
 
 
 class TabURL(FileEventFilterStringField):
     """Class that filters events based on the URL of the active browser tab at the time the file
     contents were read by the browser (applies to ``read by browser or other app`` events only).
     """
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/fileevents/filters/file_filter.py` & `py42-1.9.0/src/py42/sdk/queries/fileevents/filters/file_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from py42.sdk.queries.fileevents.file_event_query import FileEventFilterComparableField
 from py42.sdk.queries.fileevents.file_event_query import FileEventFilterStringField
-from py42.sdk.queries.query_filter import filter_attributes
+from py42.util import get_attribute_keys_from_class
 
 
 class FileCategory(FileEventFilterStringField):
     """Class that filters events by category of the file observed.
 
     Available file categories are provided as class attributes:
         - :attr:`FileCategory.AUDIO`
@@ -35,15 +35,15 @@
     SPREADSHEET = u"SPREADSHEET"
     VIDEO = u"VIDEO"
     VIRTUAL_DISK_IMAGE = u"VIRTUAL_DISK_IMAGE"
     ZIP = u"ARCHIVE"
 
     @staticmethod
     def choices():
-        return filter_attributes(FileCategory)
+        return get_attribute_keys_from_class(FileCategory)
 
 
 class FileName(FileEventFilterStringField):
     """Class that filters events by the name of the file observed."""
 
     _term = u"fileName"
```

### Comparing `py42-1.8.2/src/py42/sdk/queries/query_filter.py` & `py42-1.9.0/src/py42/sdk/queries/query_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections import OrderedDict
 from datetime import datetime
 
 from py42._compat import str
 from py42._compat import string_type
+from py42.util import convert_datetime_to_epoch
 from py42.util import convert_datetime_to_timestamp_str
-from py42.util import convert_timestamp_to_str
+from py42.util import DATE_STR_FORMAT
+from py42.util import parse_timestamp_to_milliseconds_precision
 
 
 def create_query_filter(term, operator, value=None):
     """Creates a :class:`~py42.sdk.queries.query_filter.QueryFilter` object. Useful for
     programmatically crafting query filters, such as filters not yet defined in py42.
 
     Args:
@@ -181,23 +183,14 @@
     Returns:
         :class:`~py42.sdk.queries.query_filter.FilterGroup`
     """
     filter_list = [create_query_filter(term, u"WITHIN_THE_LAST", value)]
     return create_filter_group(filter_list, u"AND")
 
 
-def filter_attributes(cls):
-
-    return [
-        cls().__getattribute__(attr)
-        for attr in dir(cls)
-        if not callable(cls().__getattribute__(attr)) and not attr.startswith(u"_")
-    ]
-
-
 class QueryFilterStringField(object):
     """Helper class for creating filters where the search value is a string."""
 
     _term = u"override_string_field_name"
 
     @classmethod
     def eq(cls, value):
@@ -263,95 +256,85 @@
     @classmethod
     def on_or_after(cls, value):
         """Returns a :class:`~py42.sdk.queries.query_filter.FilterGroup` that is useful
         for finding results where the value with key ``self._term` is on or after the
         provided ``value``.
 
         Args:
-            value (str or int): The value used to filter results.
+            value (str or int or float or datetime): The value used to filter results.
 
         Returns:
             :class:`~py42.sdk.queries.query_filter.FilterGroup`
         """
-        formatted_timestamp = convert_timestamp_to_str(value)
+        formatted_timestamp = parse_timestamp_to_milliseconds_precision(value)
         return create_on_or_after_filter_group(cls._term, formatted_timestamp)
 
     @classmethod
     def on_or_before(cls, value):
         """Returns a :class:`~py42.sdk.queries.query_filter.FilterGroup` that is useful
         for finding results where the value with key ``self._term`` is on or before the
         provided ``value``.
 
         Args:
-            value (str or int): The value used to filter results.
+            value (str or int or float or datetime): The value used to filter results.
 
         Returns:
             :class:`~py42.sdk.queries.query_filter.FilterGroup`
         """
-        formatted_timestamp = convert_timestamp_to_str(value)
+        formatted_timestamp = parse_timestamp_to_milliseconds_precision(value)
         return create_on_or_before_filter_group(cls._term, formatted_timestamp)
 
     @classmethod
     def in_range(cls, start_value, end_value):
         """Returns a :class:`~py42.sdk.queries.query_filter.FilterGroup` that is useful
         for finding results where the value with key ``self._term`` is in range between
         the provided ``start_value`` and ``end_value``.
 
         Args:
-            start_value (str or int): The start value used to filter results.
-            end_value (str or int): The end value used to filter results.
+            start_value (str or int or float or datetime): The start value used to filter results.
+            end_value (str or int or float or datetime): The end value used to filter results.
 
         Returns:
             :class:`~py42.sdk.queries.query_filter.FilterGroup`
         """
-        formatted_start_time = convert_timestamp_to_str(start_value)
-        formatted_end_time = convert_timestamp_to_str(end_value)
+        formatted_start_time = parse_timestamp_to_milliseconds_precision(start_value)
+        formatted_end_time = parse_timestamp_to_milliseconds_precision(end_value)
         return create_in_range_filter_group(
             cls._term, formatted_start_time, formatted_end_time
         )
 
     @classmethod
     def on_same_day(cls, value):
         """Returns a :class:`~py42.sdk.queries.query_filter.FilterGroup` that is useful
         for finding results where the value with key ``self._term`` is within the same
         calendar day as the provided ``value``.
 
         Args:
-            value (str or int): The value used to filter results.
+            value (str or int or float or datetime): The value used to filter results.
 
         Returns:
             :class:`~py42.sdk.queries.query_filter.FilterGroup`
         """
+        if isinstance(value, str):
+            value = convert_datetime_to_epoch(datetime.strptime(value, DATE_STR_FORMAT))
+        elif isinstance(value, datetime):
+            value = convert_datetime_to_epoch(value)
         date_from_value = datetime.utcfromtimestamp(value)
         start_time = datetime(
             date_from_value.year, date_from_value.month, date_from_value.day, 0, 0, 0
         )
         end_time = datetime(
             date_from_value.year, date_from_value.month, date_from_value.day, 23, 59, 59
         )
         formatted_start_time = convert_datetime_to_timestamp_str(start_time)
         formatted_end_time = convert_datetime_to_timestamp_str(end_time)
         return create_in_range_filter_group(
             cls._term, formatted_start_time, formatted_end_time
         )
 
-    @classmethod
-    def within_the_last(cls, value):
-        """Returns a :class:`~py42.sdk.queries.query_filter.FilterGroup` that is useful
-        for finding results where the key ``self._term`` is an ``EventTimestamp._term``
-        and the value is one of the ``EventTimestamp`` attributes as ``value``.
-
-        Args:
-            value (str): `EventTimestamp` attribute.
-
-        Returns:
-            :class:`~py42.sdk.queries.query_filter.FilterGroup`
-        """
-        return create_within_the_last_filter_group(cls._term, value)
-
 
 class QueryFilterBooleanField(object):
     """Helper class for creating filters where the search value is a boolean."""
 
     _term = u"override_boolean_field_name"
 
     @classmethod
```

### Comparing `py42-1.8.2/src/py42/services/__init__.py` & `py42-1.9.0/src/py42/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,9 +23,10 @@
         u"alerts",
         u"fileevents",
         u"savedsearch",
         u"preservationdata",
         u"departingemployee",
         u"highriskemployee",
         u"userprofile",
+        u"auditlogs",
     ],
 )
```

### Comparing `py42-1.8.2/src/py42/services/_auth.py` & `py42-1.9.0/src/py42/services/_auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,16 +25,19 @@
         return self._credentials
 
     def _get_credentials(self):
         raise NotImplementedError()
 
 
 class V3Auth(C42RenewableAuth):
-    def __init__(self, auth_connection):
+    def __init__(self, auth_connection, totp=None):
         super(V3Auth, self).__init__()
         self._auth_connection = auth_connection
+        self._totp = totp if callable(totp) else lambda: totp
 
     def _get_credentials(self):
         uri = u"/c42api/v3/auth/jwt"
         params = {u"useBody": True}
-        response = self._auth_connection.get(uri, params=params)
+        currentToken = self._totp()
+        headers = {"totp-auth": str(currentToken)} if currentToken else None
+        response = self._auth_connection.get(uri, params=params, headers=headers)
         return u"v3_user_token {}".format(response["v3_user_token"])
```

### Comparing `py42-1.8.2/src/py42/services/_connection.py` & `py42-1.9.0/src/py42/services/_connection.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/administration.py` & `py42-1.9.0/src/py42/services/administration.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/alertrules.py` & `py42-1.9.0/src/py42/services/alertrules.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/alerts.py` & `py42-1.9.0/src/py42/services/alerts.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,29 +27,26 @@
             alert_ids = [alert_ids]
         tenant_id = self._user_context.get_current_tenant_id()
         uri = self._uri_prefix.format(u"query-details")
         data = {u"tenantId": tenant_id, u"alertIds": alert_ids}
         results = self._connection.post(uri, json=data)
         return _convert_observation_json_strings_to_objects(results)
 
-    def resolve(self, alert_ids, reason=None):
+    def update_state(self, state, alert_ids, note=""):
         if not isinstance(alert_ids, (list, tuple)):
             alert_ids = [alert_ids]
+        note = note or ""
         tenant_id = self._user_context.get_current_tenant_id()
-        reason = reason or u""
-        uri = self._uri_prefix.format(u"resolve-alert")
-        data = {u"tenantId": tenant_id, u"alertIds": alert_ids, u"reason": reason}
-        return self._connection.post(uri, json=data)
-
-    def reopen(self, alert_ids, reason=None):
-        if not isinstance(alert_ids, (list, tuple)):
-            alert_ids = [alert_ids]
-        tenant_id = self._user_context.get_current_tenant_id()
-        uri = self._uri_prefix.format(u"reopen-alert")
-        data = {u"tenantId": tenant_id, u"alertIds": alert_ids, u"reason": reason}
+        uri = self._uri_prefix.format(u"update-state")
+        data = {
+            u"tenantId": tenant_id,
+            u"alertIds": alert_ids,
+            u"note": note,
+            u"state": state,
+        }
         return self._connection.post(uri, json=data)
 
     def _add_tenant_id_if_missing(self, query):
         query_dict = json.loads(str(query))
         tenant_id = query_dict.get(u"tenantId", None)
         if tenant_id is None:
             query_dict[u"tenantId"] = self._user_context.get_current_tenant_id()
```

### Comparing `py42-1.8.2/src/py42/services/archive.py` & `py42-1.9.0/src/py42/services/archive.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/detectionlists/departing_employee.py` & `py42-1.9.0/src/py42/services/detectionlists/departing_employee.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+from datetime import datetime
+
 from py42.exceptions import Py42BadRequestError
-from py42.sdk.queries.query_filter import filter_attributes
 from py42.services import BaseService
 from py42.services.detectionlists import _DetectionListFilters
 from py42.services.detectionlists import _PAGE_SIZE
 from py42.services.detectionlists import handle_user_already_added_error
 from py42.services.util import get_all_pages
+from py42.util import get_attribute_keys_from_class
+
+_DATE_FORMAT = "%Y-%m-%d"
 
 
 class DepartingEmployeeFilters(_DetectionListFilters):
     """Constants available for filtering Departing Employee search results."""
 
     LEAVING_TODAY = u"LEAVING_TODAY"
 
     @staticmethod
     def choices():
-        return filter_attributes(DepartingEmployeeFilters)
+        return get_attribute_keys_from_class(DepartingEmployeeFilters)
 
 
 class DepartingEmployeeService(BaseService):
     """A service for interacting with Code42 Departing Employee APIs."""
 
     _uri_prefix = u"/svc/api/v2/departingemployee/{0}"
 
@@ -36,19 +40,22 @@
 
         Raises a :class:`Py42BadRequestError` when a user already exists in the Departing Employee \
             detection list.
 
         Args:
             user_id (str or int): The Code42 userUid of the user you want to add to the departing \
                 employees list.
-            departure_date (str, optional): Date in yyyy-MM-dd format. Date is treated as UTC. Defaults to None.
+            departure_date (str or datetime, optional): Date in yyyy-MM-dd format or instance of datetime.
+                Date is treated as UTC. Defaults to None.
 
         Returns:
             :class:`py42.response.Py42Response`
         """
+        if isinstance(departure_date, datetime):
+            departure_date = departure_date.strftime(_DATE_FORMAT)
         if self._user_profile_service.create_if_not_exists(user_id):
             tenant_id = self._user_context.get_current_tenant_id()
             data = {
                 u"tenantId": tenant_id,
                 u"userId": user_id,
                 u"departureDate": departure_date,
             }
@@ -177,22 +184,24 @@
 
     def update_departure_date(self, user_id, departure_date):
         """Add or modify details of an existing Departing Employee case.
         `REST Documentation <https://ecm-east.us.code42.com/svc/swagger/index.html?urls.primaryName=v2#/>`__
 
         Args:
             user_id (str): The Code42 userUid of the user.
-            departure_date (date): Date in yyyy-MM-dd format. Date is treated as UTC.
+            departure_date (str or datetime): Date in yyyy-MM-dd format or instance of datetime.
+                Date is treated as UTC.
 
         Returns:
             :class:`py42.sdk.response.Py42Response`
         """
 
         tenant_id = self._user_context.get_current_tenant_id()
-
+        if isinstance(departure_date, datetime):
+            departure_date = departure_date.strftime(_DATE_FORMAT)
         uri = self._uri_prefix.format(u"update")
         data = {
             u"tenantId": tenant_id,
             u"userId": user_id,
             u"departureDate": departure_date,
         }
         return self._connection.post(uri, json=data)
```

### Comparing `py42-1.8.2/src/py42/services/detectionlists/high_risk_employee.py` & `py42-1.9.0/src/py42/services/detectionlists/high_risk_employee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from py42.exceptions import Py42BadRequestError
-from py42.sdk.queries.query_filter import filter_attributes
 from py42.services import BaseService
 from py42.services.detectionlists import _DetectionListFilters
 from py42.services.detectionlists import _PAGE_SIZE
 from py42.services.detectionlists import handle_user_already_added_error
 from py42.services.util import get_all_pages
+from py42.util import get_attribute_keys_from_class
 
 
 class HighRiskEmployeeFilters(_DetectionListFilters):
     """Constants available for filtering High Risk Employee search results."""
 
     @staticmethod
     def choices():
-        return filter_attributes(HighRiskEmployeeFilters)
+        return get_attribute_keys_from_class(HighRiskEmployeeFilters)
 
 
 class HighRiskEmployeeService(BaseService):
     """A service for interacting with High Risk Employee APIs."""
 
     _api_version = u"v2"
     _uri_prefix = u"/svc/api/{}".format(_api_version)
```

### Comparing `py42-1.8.2/src/py42/services/detectionlists/user_profile.py` & `py42-1.9.0/src/py42/services/detectionlists/user_profile.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/devices.py` & `py42-1.9.0/src/py42/services/devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,20 @@
+from collections import namedtuple
+from time import time
+
 from py42 import settings
+from py42._compat import str
+from py42.clients.settings.device_settings import DeviceSettings
 from py42.services import BaseService
 from py42.services.util import get_all_pages
 
+DeviceSettingsResponse = namedtuple(
+    "DeviceSettingsResponse", ["error", "settings_response", "device_settings_response"]
+)
+
 
 class DeviceService(BaseService):
     """A class to interact with Code42 device/computer APIs."""
 
     def get_page(
         self,
         page_num,
@@ -218,29 +227,14 @@
 
         Returns:
             :class:`py42.response.Py42Response`
         """
         uri = u"/api/ComputerDeauthorization/{}".format(device_id)
         return self._connection.put(uri)
 
-    def get_settings(self, guid, keys=None):
-        """Gets settings of the device.
-        `REST Documentation <https://console.us.code42.com/apidocviewer/#DeviceSetting>`__
-
-        Args:
-            guid (str): The globally unique identifier of the device.
-            keys (str, optional): A comma separated list of device keys. Defaults to None.
-
-        Returns:
-            :class:`py42.response.Py42Response`: A response containing settings information.
-        """
-        uri = u"/api/v4/device-setting/view"
-        params = {u"guid": guid, u"keys": keys}
-        return self._connection.get(uri, params=params)
-
     def get_agent_state(self, guid, property_name):
         """Gets the agent state of the device.
             `REST Documentation <https://console.us.code42.com/swagger/index.html?urls.primaryName=v14#/agent-state/AgentState_ViewByDeviceGuid>`__
 
             Args:
                 guid (str): The globally unique identifier of the device.
                 property_name (str): The name of the property to retrieve (e.g. `fullDiskAccess`).
@@ -259,7 +253,35 @@
             Args:
                 guid (str): The globally unique identifier of the device.
 
             Returns:
                 :class:`py42.response.Py42Response`: A response containing settings information.
             """
         return self.get_agent_state(guid, u"fullDiskAccess")
+
+    def get_settings(self, guid):
+        """Gets setting data for a device and returns a `DeviceSettings` object for the target device.
+
+        Args:
+            guid (int,str): The globally unique identifier of the device.
+
+        Returns:
+            :class:`py42.clients.settings.device_settings.DeviceSettings`: A class to help manage device settings.
+        """
+        settings = self.get_by_guid(guid, incSettings=True)
+        return DeviceSettings(settings.data)
+
+    def update_settings(self, device_settings):
+        """Updates a device's settings based on changes to the passed in `DeviceSettings` instance.
+
+        Args:
+            device_settings (`DeviceSettings`): An instance of `DeviceSettings` with desired modifications to settings.
+
+        Returns:
+            :class:`py42.response.Py42Response`: A response containing the result of the setting change.
+        """
+        device_settings = dict(device_settings)
+        device_id = device_settings[u"computerId"]
+        uri = u"/api/Computer/{}".format(device_id)
+        new_config_date_ms = str(int(time() * 1000))
+        device_settings[u"settings"][u"configDateMs"] = new_config_date_ms
+        return self._connection.put(uri, json=device_settings)
```

### Comparing `py42-1.8.2/src/py42/services/fileevent.py` & `py42-1.9.0/src/py42/services/fileevent.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/legalhold.py` & `py42-1.9.0/src/py42/services/legalhold.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/orgs.py` & `py42-1.9.0/src/py42/services/orgs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+from collections import namedtuple
+
 from py42 import settings
+from py42.clients.settings.org_settings import OrgSettings
+from py42.exceptions import Py42Error
 from py42.services import BaseService
 from py42.services.util import get_all_pages
 
+OrgSettingsResponse = namedtuple(
+    u"OrgSettingsResponse", [u"error", u"org_response", u"org_settings_response"]
+)
+
 
 class OrgService(BaseService):
     """A service for interacting with Code42 organization APIs.
 
     Use the OrgService to create and retrieve organizations. You can also use it to block and
     deactivate organizations.
     """
@@ -181,7 +189,58 @@
             Args:
                 org_id (str): The org's identifier.
 
             Returns:
                 :class:`py42.response.Py42Response`: A response containing settings information.
             """
         return self.get_agent_state(org_id, u"fullDiskAccess")
+
+    def get_settings(self, org_id):
+        """Gets setting data for an org and returns an `OrgSettingsManager` for the target org.
+
+        Args:
+            org_id (int,str): The identifier of the org.
+
+        Returns:
+            :class:`py42.clients._settings_managers.OrgSettings`: A class to help manage org settings.
+                """
+        org_settings = self.get_by_id(
+            org_id, incSettings=True, incDeviceDefaults=True, incInheritedOrgInfo=True
+        )
+        uri = u"/api/OrgSetting/{}".format(org_id)
+        t_settings = self._connection.get(uri)
+        return OrgSettings(org_settings.data, t_settings.data)
+
+    def update_settings(self, org_settings):
+        """Updates an org's settings based on changes to the passed in `OrgSettings` instance.
+
+        Args:
+            org_settings (`OrgSettings`): An `OrgSettings` instance with desired modifications to settings.
+
+        Returns:
+            :class:`py42.services.orgs.OrgSettings`: A namedtuple containing the result of the setting change api calls.
+        """
+        org_id = org_settings.org_id
+        error = False
+        org_settings_response = org_response = None
+
+        if org_settings.packets:
+            uri = u"/api/OrgSetting/{}".format(org_id)
+            payload = {"packets": org_settings.packets}
+            try:
+                org_settings_response = self._connection.put(uri, json=payload)
+            except Py42Error as ex:
+                error = True
+                org_settings_response = ex
+
+        if org_settings.changes:
+            uri = "/api/Org/{}".format(org_id)
+            try:
+                org_response = self._connection.put(uri, json=org_settings.data)
+            except Py42Error as ex:
+                error = True
+                org_response = ex
+        return OrgSettingsResponse(
+            error=error,
+            org_response=org_response,
+            org_settings_response=org_settings_response,
+        )
```

### Comparing `py42-1.8.2/src/py42/services/preservationdata.py` & `py42-1.9.0/src/py42/services/preservationdata.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/savedsearch.py` & `py42-1.9.0/src/py42/services/savedsearch.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,32 +28,36 @@
             search_id (str): Unique search Id of the saved search.
         Returns:
             :class:`py42.response.Py42Response`
         """
         uri = u"{}/{}".format(self._resource, search_id)
         return self._connection.get(uri)
 
-    def get_query(self, search_id):
+    def get_query(self, search_id, page_number=None, page_size=None):
         """Get the saved search in form of a query(`py42.sdk.queries.fileevents.file_event_query`).
 
         Args:
             search_id (str): Unique search Id of the saved search.
+            page_number (int, optional): The consecutive group of results of size page_size in the result set to return. Defaults to None.
+            page_size (int, optional): The maximum number of results to be returned. Defaults to None.
         Returns:
             :class:`py42.sdk.queries.fileevents.file_event_query.FileEventQuery`
         """
         response = self.get_by_id(search_id)
         search = response[u"searches"][0]
-        return FileEventQuery.from_dict(search)
+        return FileEventQuery.from_dict(
+            search, page_number=page_number, page_size=page_size,
+        )
 
-    def execute(self, search_id, pg_num=1, pg_size=10000):
+    def execute(self, search_id, page_number=None, page_size=None):
         """
         Execute a saved search for given search Id and return its results.
 
         Args:
             search_id (str): Unique search Id of the saved search.
-            pg_num (int, optional): The consecutive group of results of size pg_size in the result set to return. Defaults to 1.
-            pg_size (int, optional): The maximum number of results to be returned. Defaults to 10,000.
+            page_number (int, optional): The consecutive group of results of size page_size in the result set to return. Defaults to None.
+            page_size (int, optional): The maximum number of results to be returned. Defaults to None.
         Returns:
             :class:`py42.response.Py42Response`
         """
-        query = self.get_query(search_id)
+        query = self.get_query(search_id, page_number=page_number, page_size=page_size)
         return self._file_event_client.search(query)
```

### Comparing `py42-1.8.2/src/py42/services/storage/_auth.py` & `py42-1.9.0/src/py42/services/storage/_auth.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/storage/_service_factory.py` & `py42-1.9.0/src/py42/services/storage/_service_factory.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/storage/archive.py` & `py42-1.9.0/src/py42/services/storage/archive.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/storage/preservationdata.py` & `py42-1.9.0/src/py42/services/storage/preservationdata.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/services/storage/securitydata.py` & `py42-1.9.0/src/py42/services/storage/securitydata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from datetime import datetime
-
 from py42.services import BaseService
+from py42.util import parse_timestamp_to_microseconds_precision
 
 
 class StorageSecurityDataService(BaseService):
     def _get_security_detection_events(
         self,
         user_uid=None,
         plan_uid=None,
@@ -16,24 +15,19 @@
         summarize=None,
     ):
         uri = u"/api/SecurityDetectionEvent"
 
         min_time_str = None
         max_time_str = None
 
-        def get_time_str_from_timestamp(timestamp):
-            return datetime.utcfromtimestamp(timestamp).strftime(
-                u"%Y-%m-%dT%H:%M:%S.%fZ"
-            )
-
         if min_timestamp:
-            min_time_str = get_time_str_from_timestamp(min_timestamp)
+            min_time_str = parse_timestamp_to_microseconds_precision(min_timestamp)
 
         if max_timestamp:
-            max_time_str = get_time_str_from_timestamp(max_timestamp)
+            max_time_str = parse_timestamp_to_microseconds_precision(max_timestamp)
 
         params = {
             u"userUid": user_uid,
             u"planUid": plan_uid,
             u"cursor": cursor,
             u"incFiles": include_files,
             u"eventType": event_types,
```

### Comparing `py42-1.8.2/src/py42/services/users.py` & `py42-1.9.0/src/py42/services/users.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42/settings/__init__.py` & `py42-1.9.0/src/py42/settings/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 proxies = None
 
 # Controls whether we verify the server's certificate.
 # True, False, or a path to a CA bundle to use.
 verify_ssl_certs = True
 
 items_per_page = 500
+security_events_per_page = 10000
 
 _custom_user_suffix = u""
 _python_version = u"{}.{}.{}".format(
     sys.version_info[0], sys.version_info[1], sys.version_info[2]
 )
```

### Comparing `py42-1.8.2/src/py42/usercontext.py` & `py42-1.9.0/src/py42/usercontext.py`

 * *Files identical despite different names*

### Comparing `py42-1.8.2/src/py42.egg-info/PKG-INFO` & `py42-1.9.0/src/py42.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py42
-Version: 1.8.2
+Version: 1.9.0
 Summary: The Official Code42 Python API Client
 Home-page: https://github.com/code42/py42
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/code42/py42/issues
 Project-URL: Documentation, https://py42docs.code42.com/
 Project-URL: Source Code, https://github.com/code42/py42
 Description:
```

### Comparing `py42-1.8.2/src/py42.egg-info/SOURCES.txt` & `py42-1.9.0/src/py42.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 src/py42.egg-info/requires.txt
 src/py42.egg-info/top_level.txt
 src/py42/clients/__init__.py
 src/py42/clients/_archive_access.py
 src/py42/clients/alertrules.py
 src/py42/clients/alerts.py
 src/py42/clients/archive.py
+src/py42/clients/auditlogs.py
 src/py42/clients/authority.py
 src/py42/clients/detectionlists.py
 src/py42/clients/securitydata.py
+src/py42/clients/settings/__init__.py
+src/py42/clients/settings/_converters.py
+src/py42/clients/settings/device_settings.py
+src/py42/clients/settings/org_settings.py
 src/py42/constants/__init__.py
 src/py42/sdk/__init__.py
 src/py42/sdk/queries/__init__.py
 src/py42/sdk/queries/query_filter.py
 src/py42/sdk/queries/alerts/__init__.py
 src/py42/sdk/queries/alerts/alert_query.py
 src/py42/sdk/queries/alerts/filters/__init__.py
@@ -49,14 +54,15 @@
 src/py42/services/_auth.py
 src/py42/services/_connection.py
 src/py42/services/_keyvaluestore.py
 src/py42/services/administration.py
 src/py42/services/alertrules.py
 src/py42/services/alerts.py
 src/py42/services/archive.py
+src/py42/services/auditlogs.py
 src/py42/services/devices.py
 src/py42/services/fileevent.py
 src/py42/services/legalhold.py
 src/py42/services/orgs.py
 src/py42/services/preservationdata.py
 src/py42/services/savedsearch.py
 src/py42/services/securitydata.py
```

### Comparing `py42-1.8.2/tox.ini` & `py42-1.9.0/tox.ini`

 * *Files identical despite different names*

