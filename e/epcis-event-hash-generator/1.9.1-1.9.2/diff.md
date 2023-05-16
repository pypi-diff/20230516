# Comparing `tmp/epcis-event-hash-generator-1.9.1.tar.gz` & `tmp/epcis-event-hash-generator-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epcis-event-hash-generator-1.9.1.tar", last modified: Tue May 16 19:54:28 2023, max compression
+gzip compressed data, was "epcis-event-hash-generator-1.9.2.tar", last modified: Tue May 16 20:05:36 2023, max compression
```

## Comparing `epcis-event-hash-generator-1.9.1.tar` & `epcis-event-hash-generator-1.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 19:54:28.245029 epcis-event-hash-generator-1.9.1/
--rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1065 2020-01-15 09:04:43.000000 epcis-event-hash-generator-1.9.1/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    21377 2023-05-16 19:54:28.245029 epcis-event-hash-generator-1.9.1/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    20622 2023-04-06 11:40:50.000000 epcis-event-hash-generator-1.9.1/README.md
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 19:54:28.241029 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4932 2023-05-16 14:42:03.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/__init__.py
--rwxrwxr-x   0 sebastian  (1000) sebastian  (1000)     5086 2022-04-12 14:10:06.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/__main__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      140 2021-03-25 18:01:10.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/context.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    26376 2023-04-06 11:40:50.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/dl_normaliser.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2168 2021-03-08 11:41:20.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/events_from_file_reader.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2056 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/file_document_loader.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11624 2023-03-28 09:17:42.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/hash_generator.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8200 2023-03-28 09:17:42.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/json_to_py.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3774 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/json_xml_model_mismatch_correction.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5923 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/xml_to_py.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 19:54:28.241029 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    21377 2023-05-16 19:54:28.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      950 2023-05-16 19:54:28.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-05-16 19:54:28.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       67 2023-05-16 19:54:28.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-05-16 19:54:28.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       27 2023-05-16 19:54:28.000000 epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/top_level.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-05-16 19:54:28.245029 epcis-event-hash-generator-1.9.1/setup.cfg
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1254 2023-05-16 19:54:14.000000 epcis-event-hash-generator-1.9.1/setup.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 19:54:28.245029 epcis-event-hash-generator-1.9.1/tests/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2367 2023-03-28 09:17:42.000000 epcis-event-hash-generator-1.9.1/tests/test_all_values_present.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1339 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.1/tests/test_bare_string_normalisation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1051 2021-03-08 11:41:20.000000 epcis-event-hash-generator-1.9.1/tests/test_explicit_hash_values.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1508 2021-03-08 11:41:20.000000 epcis-event-hash-generator-1.9.1/tests/test_required_properties.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3383 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.1/tests/test_xml_to_py.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 20:05:36.694286 epcis-event-hash-generator-1.9.2/
+-rw-r--r--   0 sebastian  (1000) sebastian  (1000)     1065 2020-01-15 09:04:43.000000 epcis-event-hash-generator-1.9.2/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    21377 2023-05-16 20:05:36.694286 epcis-event-hash-generator-1.9.2/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    20622 2023-04-06 11:40:50.000000 epcis-event-hash-generator-1.9.2/README.md
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 20:05:36.690286 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4932 2023-05-16 14:42:03.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/__init__.py
+-rwxrwxr-x   0 sebastian  (1000) sebastian  (1000)     5086 2022-04-12 14:10:06.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/__main__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      140 2021-03-25 18:01:10.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/context.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    26376 2023-04-06 11:40:50.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/dl_normaliser.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2168 2021-03-08 11:41:20.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/events_from_file_reader.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2070 2023-05-16 19:59:24.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/file_document_loader.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11624 2023-03-28 09:17:42.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/hash_generator.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8200 2023-03-28 09:17:42.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/json_to_py.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3774 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/json_xml_model_mismatch_correction.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5923 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/xml_to_py.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 20:05:36.690286 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    21377 2023-05-16 20:05:36.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      950 2023-05-16 20:05:36.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-05-16 20:05:36.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       67 2023-05-16 20:05:36.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-05-16 20:05:36.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       27 2023-05-16 20:05:36.000000 epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/top_level.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-05-16 20:05:36.694286 epcis-event-hash-generator-1.9.2/setup.cfg
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1254 2023-05-16 20:05:23.000000 epcis-event-hash-generator-1.9.2/setup.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-05-16 20:05:36.694286 epcis-event-hash-generator-1.9.2/tests/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     2367 2023-03-28 09:17:42.000000 epcis-event-hash-generator-1.9.2/tests/test_all_values_present.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1339 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.2/tests/test_bare_string_normalisation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1051 2021-03-08 11:41:20.000000 epcis-event-hash-generator-1.9.2/tests/test_explicit_hash_values.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1508 2021-03-08 11:41:20.000000 epcis-event-hash-generator-1.9.2/tests/test_required_properties.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3383 2023-02-10 10:37:47.000000 epcis-event-hash-generator-1.9.2/tests/test_xml_to_py.py
```

### Comparing `epcis-event-hash-generator-1.9.1/LICENSE` & `epcis-event-hash-generator-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/PKG-INFO` & `epcis-event-hash-generator-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epcis-event-hash-generator
-Version: 1.9.1
+Version: 1.9.2
 Summary: Exemplary implementation of the EPCIS event hash generator algorithm described in the README
 Home-page: https://github.com/RalphTro/epcis-event-hash-generator
 Author: Package author: Sebastian Schmittner
     Code authors: https://github.com/RalphTro/epcis-event-hash-generator/graphs/contributors
 Author-email: sebastian.schmittner@eecc.de
 License: MIT
 Keywords: epcis GS1 hashing traceability
```

### Comparing `epcis-event-hash-generator-1.9.1/README.md` & `epcis-event-hash-generator-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/__init__.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/__main__.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/__main__.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/dl_normaliser.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/dl_normaliser.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/events_from_file_reader.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/events_from_file_reader.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/file_document_loader.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/file_document_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
     :return: the RemoteDocument loader function.
     """
     from pyld import jsonld
 
     context_file_hashes = {
         "https://gs1.github.io/EPCIS/epcis-context.jsonld":
-        "14b10c9d3e92d35f577bfc610fe5ec15aa2941124987919389d7cd9998516861",
+        "14b10c9d3e92d35f577bfc610fe5ec15aa2941124987919389d7cd9998516861.jsonld",
         "https://ref.gs1.org/standards/epcis/2.0.0/epcis-context.jsonld":
-        "e532647e8eb371379b8b0e8602d8981c8566bc60f7351f22c76a5bc865962008"
+        "e532647e8eb371379b8b0e8602d8981c8566bc60f7351f22c76a5bc865962008.jsonld"
     }
 
     def loader(url, options={}):
         """
         Retrieves JSON-LD for the given name (URL).
 
         :return: the RemoteDocument.
```

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/hash_generator.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/hash_generator.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/json_to_py.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/json_to_py.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/json_xml_model_mismatch_correction.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/json_xml_model_mismatch_correction.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator/xml_to_py.py` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator/xml_to_py.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/PKG-INFO` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epcis-event-hash-generator
-Version: 1.9.1
+Version: 1.9.2
 Summary: Exemplary implementation of the EPCIS event hash generator algorithm described in the README
 Home-page: https://github.com/RalphTro/epcis-event-hash-generator
 Author: Package author: Sebastian Schmittner
     Code authors: https://github.com/RalphTro/epcis-event-hash-generator/graphs/contributors
 Author-email: sebastian.schmittner@eecc.de
 License: MIT
 Keywords: epcis GS1 hashing traceability
```

### Comparing `epcis-event-hash-generator-1.9.1/epcis_event_hash_generator.egg-info/SOURCES.txt` & `epcis-event-hash-generator-1.9.2/epcis_event_hash_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/setup.py` & `epcis-event-hash-generator-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="epcis-event-hash-generator",
     keywords="epcis GS1 hashing traceability",
-    version="1.9.1",
+    version="1.9.2",
     author="""Package author: Sebastian Schmittner
     Code authors: https://github.com/RalphTro/epcis-event-hash-generator/graphs/contributors""",
     author_email="sebastian.schmittner@eecc.de",
     license="MIT",
     description="Exemplary implementation of the EPCIS event hash generator algorithm described in the README",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `epcis-event-hash-generator-1.9.1/tests/test_all_values_present.py` & `epcis-event-hash-generator-1.9.2/tests/test_all_values_present.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/tests/test_bare_string_normalisation.py` & `epcis-event-hash-generator-1.9.2/tests/test_bare_string_normalisation.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/tests/test_explicit_hash_values.py` & `epcis-event-hash-generator-1.9.2/tests/test_explicit_hash_values.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/tests/test_required_properties.py` & `epcis-event-hash-generator-1.9.2/tests/test_required_properties.py`

 * *Files identical despite different names*

### Comparing `epcis-event-hash-generator-1.9.1/tests/test_xml_to_py.py` & `epcis-event-hash-generator-1.9.2/tests/test_xml_to_py.py`

 * *Files identical despite different names*

