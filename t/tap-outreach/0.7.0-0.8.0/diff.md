# Comparing `tmp/tap-outreach-0.7.0.tar.gz` & `tmp/tap-outreach-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-outreach-0.7.0.tar", last modified: Mon Jun 28 15:22:50 2021, max compression
+gzip compressed data, was "tap-outreach-0.8.0.tar", last modified: Tue May 16 11:42:33 2023, max compression
```

## Comparing `tap-outreach-0.7.0.tar` & `tap-outreach-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-28 15:22:50.143973 tap-outreach-0.7.0/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    34523 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/LICENSE
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       51 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/MANIFEST.in
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      291 2021-06-28 15:22:50.143973 tap-outreach-0.7.0/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5753 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/README.md
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2021-06-28 15:22:50.143973 tap-outreach-0.7.0/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      679 2021-06-28 15:21:12.000000 tap-outreach-0.7.0/setup.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-28 15:22:50.107973 tap-outreach-0.7.0/tap_outreach/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1185 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4236 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/client.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1931 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/discover.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-28 15:22:50.139973 tap-outreach-0.7.0/tap_outreach/schemas/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4935 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/accounts.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      685 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/call_dispositions.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      604 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/call_purposes.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2596 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/calls.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      787 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/content_categories.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      306 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/duties.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1367 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/tap_outreach/schemas/events.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4628 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/mailboxes.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4357 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/mailings.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10000 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/opportunities.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      525 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/personas.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    13097 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/prospects.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2693 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/tap_outreach/schemas/sequence_states.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2489 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/tap_outreach/schemas/sequence_steps.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2014 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/tap_outreach/schemas/sequence_templates.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4642 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/tap_outreach/schemas/sequences.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      767 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/stages.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2715 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/tasks.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      519 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/teams.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5560 2021-04-13 23:23:26.000000 tap-outreach-0.7.0/tap_outreach/schemas/users.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10595 2021-06-28 14:11:06.000000 tap-outreach-0.7.0/tap_outreach/sync.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-28 15:22:50.115973 tap-outreach-0.7.0/tap_outreach.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      291 2021-06-28 15:22:50.000000 tap-outreach-0.7.0/tap_outreach.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1087 2021-06-28 15:22:50.000000 tap-outreach-0.7.0/tap_outreach.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-06-28 15:22:50.000000 tap-outreach-0.7.0/tap_outreach.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       76 2021-06-28 15:22:50.000000 tap-outreach-0.7.0/tap_outreach.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       53 2021-06-28 15:22:50.000000 tap-outreach-0.7.0/tap_outreach.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       13 2021-06-28 15:22:50.000000 tap-outreach-0.7.0/tap_outreach.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 11:42:33.599176 tap-outreach-0.8.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      246 2023-05-16 11:42:33.599176 tap-outreach-0.8.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5779 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 11:42:33.599176 tap-outreach-0.8.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      679 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 11:42:33.595176 tap-outreach-0.8.0/tap_outreach/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4236 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1931 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 11:42:33.599176 tap-outreach-0.8.0/tap_outreach/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4935 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/accounts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      685 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/call_dispositions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      604 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/call_purposes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/calls.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      787 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/content_categories.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      306 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/duties.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1367 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4628 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/mailboxes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4357 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/mailings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10000 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/opportunities.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      525 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/personas.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13097 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/prospects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2693 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/sequence_states.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2489 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/sequence_steps.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2014 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/sequence_templates.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4642 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/sequences.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      767 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/stages.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2715 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/tasks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      519 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/teams.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5560 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/schemas/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10742 2023-05-16 11:40:57.000000 tap-outreach-0.8.0/tap_outreach/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 11:42:33.595176 tap-outreach-0.8.0/tap_outreach.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      246 2023-05-16 11:42:33.000000 tap-outreach-0.8.0/tap_outreach.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1087 2023-05-16 11:42:33.000000 tap-outreach-0.8.0/tap_outreach.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 11:42:33.000000 tap-outreach-0.8.0/tap_outreach.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-05-16 11:42:33.000000 tap-outreach-0.8.0/tap_outreach.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-05-16 11:42:33.000000 tap-outreach-0.8.0/tap_outreach.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-05-16 11:42:33.000000 tap-outreach-0.8.0/tap_outreach.egg-info/top_level.txt
```

### Comparing `tap-outreach-0.7.0/LICENSE` & `tap-outreach-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/README.md` & `tap-outreach-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tap-outreach
 
 This is a [Singer](https://singer.io) tap that produces JSON-formatted data
 following the [Singer
-spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md).
+spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md#singer-specification).
 
 This tap:
 
 - Pulls raw data from Outreach API
 - Outputs the schema for each resource
 - Incrementally pulls data based on the input state
```

### Comparing `tap-outreach-0.7.0/setup.py` & `tap-outreach-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-outreach',
-      version='0.7.0',
+      version='0.8.0',
       description='Singer.io tap for extracting data from the Outreach.io API',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_outreach'],
       install_requires=[
           'backoff==1.8.0',
```

### Comparing `tap-outreach-0.7.0/tap_outreach/__init__.py` & `tap-outreach-0.8.0/tap_outreach/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/client.py` & `tap-outreach-0.8.0/tap_outreach/client.py`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/discover.py` & `tap-outreach-0.8.0/tap_outreach/discover.py`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/accounts.json` & `tap-outreach-0.8.0/tap_outreach/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/call_dispositions.json` & `tap-outreach-0.8.0/tap_outreach/schemas/call_dispositions.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/call_purposes.json` & `tap-outreach-0.8.0/tap_outreach/schemas/call_purposes.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/calls.json` & `tap-outreach-0.8.0/tap_outreach/schemas/calls.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/content_categories.json` & `tap-outreach-0.8.0/tap_outreach/schemas/content_categories.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/events.json` & `tap-outreach-0.8.0/tap_outreach/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/mailboxes.json` & `tap-outreach-0.8.0/tap_outreach/schemas/mailboxes.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/mailings.json` & `tap-outreach-0.8.0/tap_outreach/schemas/mailings.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/opportunities.json` & `tap-outreach-0.8.0/tap_outreach/schemas/opportunities.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/personas.json` & `tap-outreach-0.8.0/tap_outreach/schemas/personas.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/prospects.json` & `tap-outreach-0.8.0/tap_outreach/schemas/prospects.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/sequence_states.json` & `tap-outreach-0.8.0/tap_outreach/schemas/sequence_states.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/sequence_steps.json` & `tap-outreach-0.8.0/tap_outreach/schemas/sequence_steps.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/sequence_templates.json` & `tap-outreach-0.8.0/tap_outreach/schemas/sequence_templates.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/sequences.json` & `tap-outreach-0.8.0/tap_outreach/schemas/sequences.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/stages.json` & `tap-outreach-0.8.0/tap_outreach/schemas/stages.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/tasks.json` & `tap-outreach-0.8.0/tap_outreach/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/teams.json` & `tap-outreach-0.8.0/tap_outreach/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/schemas/users.json` & `tap-outreach-0.8.0/tap_outreach/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap-outreach-0.7.0/tap_outreach/sync.py` & `tap-outreach-0.8.0/tap_outreach/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,17 +223,18 @@
 
                     if 'data' in value and fk_field_name in fks:
                         data_value = value['data']
                         if data_value is not None and 'id' not in data_value:
                             raise Exception(
                                 'null or `id` field expected for `data` relationship')
 
-                        if fk_field_name in record_flat:
-                            raise Exception(
-                                '`{}` exists as both an attribute and generated relationship name'.format(fk_field_name))
+                        # potential fix for the issue - https://github.com/singer-io/tap-outreach/issues/20
+                        if stream.tap_stream_id != "prospects":
+                            if fk_field_name in record_flat:
+                                raise Exception('`{}` exists as both an attribute and generated relationship name'.format(fk_field_name))
 
                         if data_value == None:
                             record_flat[fk_field_name] = None
                         else:
                             record_flat[fk_field_name] = data_value['id']
 
             if filter_field in record_flat and record_flat[filter_field] > max_modified:
```

### Comparing `tap-outreach-0.7.0/tap_outreach.egg-info/SOURCES.txt` & `tap-outreach-0.8.0/tap_outreach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

