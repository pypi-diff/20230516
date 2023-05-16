# Comparing `tmp/tap-impact-1.0.2.tar.gz` & `tmp/tap-impact-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-impact-1.0.2.tar", last modified: Fri May 12 05:12:23 2023, max compression
+gzip compressed data, was "tap-impact-2.0.0.tar", last modified: Tue May 16 10:31:57 2023, max compression
```

## Comparing `tap-impact-1.0.2.tar` & `tap-impact-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 05:12:23.000000 tap-impact-1.0.2/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3454 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/transform.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6545 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1042 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/api_submissions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7122 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/tracking_value_requests.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/exception_lists.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/unique_urls.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4363 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/company_information.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      502 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/exception_list_items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      652 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/phone_numbers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3305 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/media_partners.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      870 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/media_partner_groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/notes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1976 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/contacts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1877 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/action_updates.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9160 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/conversion_paths.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5146 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/promo_codes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2119 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/invoices.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2511 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/clicks.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      365 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/reports.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4879 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/catalog_items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2745 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/actions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4332 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/deals.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5323 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/ftp_file_submissions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2214 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/action_inquiries.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6842 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/report_metadata.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schemas/catalogs.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8588 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1341 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1327 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19020 2023-05-12 05:00:43.000000 tap-impact-1.0.2/tap_impact/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2023-05-11 12:09:24.000000 tap-impact-1.0.2/tap_impact/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-05-11 12:09:24.000000 tap-impact-1.0.2/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1358 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-12 05:12:23.000000 tap-impact-1.0.2/tap_impact.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-12 05:12:23.000000 tap-impact-1.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-12 05:12:23.000000 tap-impact-1.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      828 2023-05-12 05:00:43.000000 tap-impact-1.0.2/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-05-11 12:09:24.000000 tap-impact-1.0.2/LICENSE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:31:57.274167 tap-impact-2.0.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-05-16 10:29:39.000000 tap-impact-2.0.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-05-16 10:29:39.000000 tap-impact-2.0.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      274 2023-05-16 10:31:57.274167 tap-impact-2.0.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19252 2023-05-16 10:29:39.000000 tap-impact-2.0.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 10:31:57.274167 tap-impact-2.0.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      828 2023-05-16 10:29:39.000000 tap-impact-2.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:31:57.270167 tap-impact-2.0.0/tap_impact/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1327 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6545 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1341 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:31:57.274167 tap-impact-2.0.0/tap_impact/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2214 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/action_inquiries.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1876 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/action_updates.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2745 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/actions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6842 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1042 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/api_submissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5323 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4879 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/catalog_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/catalogs.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2511 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/clicks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4363 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/company_information.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1976 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/contacts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9160 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/conversion_paths.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4332 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/deals.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      502 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/exception_list_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/exception_lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/ftp_file_submissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2119 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/invoices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      870 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/media_partner_groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3305 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/media_partners.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/notes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      652 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/phone_numbers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5146 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/promo_codes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/report_metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      365 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/reports.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7122 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/tracking_value_requests.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/schemas/unique_urls.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8588 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19020 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3454 2023-05-16 10:29:39.000000 tap-impact-2.0.0/tap_impact/transform.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 10:31:57.270167 tap-impact-2.0.0/tap_impact.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      274 2023-05-16 10:31:57.000000 tap-impact-2.0.0/tap_impact.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-05-16 10:31:57.000000 tap-impact-2.0.0/tap_impact.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 10:31:57.000000 tap-impact-2.0.0/tap_impact.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-05-16 10:31:57.000000 tap-impact-2.0.0/tap_impact.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-16 10:31:57.000000 tap-impact-2.0.0/tap_impact.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-16 10:31:57.000000 tap-impact-2.0.0/tap_impact.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-impact-1.0.2/tap_impact/transform.py` & `tap-impact-2.0.0/tap_impact/transform.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/client.py` & `tap-impact-2.0.0/tap_impact/client.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/api_submissions.json` & `tap-impact-2.0.0/tap_impact/schemas/api_submissions.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/tracking_value_requests.json` & `tap-impact-2.0.0/tap_impact/schemas/tracking_value_requests.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/exception_lists.json` & `tap-impact-2.0.0/tap_impact/schemas/exception_lists.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/unique_urls.json` & `tap-impact-2.0.0/tap_impact/schemas/unique_urls.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/company_information.json` & `tap-impact-2.0.0/tap_impact/schemas/company_information.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/phone_numbers.json` & `tap-impact-2.0.0/tap_impact/schemas/phone_numbers.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/media_partners.json` & `tap-impact-2.0.0/tap_impact/schemas/media_partners.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/media_partner_groups.json` & `tap-impact-2.0.0/tap_impact/schemas/media_partner_groups.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/notes.json` & `tap-impact-2.0.0/tap_impact/schemas/notes.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/contacts.json` & `tap-impact-2.0.0/tap_impact/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/action_updates.json` & `tap-impact-2.0.0/tap_impact/schemas/action_updates.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989711934156379%*

 * *Differences: {"'properties'": "{'customer_id': {'type': {insert: [(1, 'string')], delete: [1]}}}"}*

```diff
@@ -62,15 +62,15 @@
                 "null",
                 "string"
             ]
         },
         "customer_id": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "customer_status": {
             "type": [
                 "null",
                 "string"
             ]
```

### Comparing `tap-impact-1.0.2/tap_impact/schemas/conversion_paths.json` & `tap-impact-2.0.0/tap_impact/schemas/conversion_paths.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/promo_codes.json` & `tap-impact-2.0.0/tap_impact/schemas/promo_codes.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/invoices.json` & `tap-impact-2.0.0/tap_impact/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/clicks.json` & `tap-impact-2.0.0/tap_impact/schemas/clicks.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/catalog_items.json` & `tap-impact-2.0.0/tap_impact/schemas/catalog_items.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/actions.json` & `tap-impact-2.0.0/tap_impact/schemas/actions.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/deals.json` & `tap-impact-2.0.0/tap_impact/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/campaigns.json` & `tap-impact-2.0.0/tap_impact/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/ftp_file_submissions.json` & `tap-impact-2.0.0/tap_impact/schemas/ftp_file_submissions.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/action_inquiries.json` & `tap-impact-2.0.0/tap_impact/schemas/action_inquiries.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/ads.json` & `tap-impact-2.0.0/tap_impact/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/report_metadata.json` & `tap-impact-2.0.0/tap_impact/schemas/report_metadata.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schemas/catalogs.json` & `tap-impact-2.0.0/tap_impact/schemas/catalogs.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/streams.py` & `tap-impact-2.0.0/tap_impact/streams.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/schema.py` & `tap-impact-2.0.0/tap_impact/schema.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/__init__.py` & `tap-impact-2.0.0/tap_impact/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/sync.py` & `tap-impact-2.0.0/tap_impact/sync.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact/discover.py` & `tap-impact-2.0.0/tap_impact/discover.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.2/tap_impact.egg-info/SOURCES.txt` & `tap-impact-2.0.0/tap_impact.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+README.md
 setup.py
 tap_impact/__init__.py
 tap_impact/client.py
 tap_impact/discover.py
 tap_impact/schema.py
 tap_impact/streams.py
 tap_impact/sync.py
```

### Comparing `tap-impact-1.0.2/setup.py` & `tap-impact-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-impact',
-      version='1.0.2',
+      version='2.0.0',
       description='Singer.io tap for extracting data from the Impact Advertiser, Partner, Agency APIs',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_impact'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-impact-1.0.2/LICENSE` & `tap-impact-2.0.0/LICENSE`

 * *Files identical despite different names*

