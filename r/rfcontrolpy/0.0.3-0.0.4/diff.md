# Comparing `tmp/rfcontrolpy-0.0.3.tar.gz` & `tmp/rfcontrolpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcontrolpy-0.0.3.tar", last modified: Fri May 12 14:57:19 2023, max compression
+gzip compressed data, was "rfcontrolpy-0.0.4.tar", last modified: Mon May 15 22:20:57 2023, max compression
```

## Comparing `rfcontrolpy-0.0.3.tar` & `rfcontrolpy-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.435018 rfcontrolpy-0.0.3/rfcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/rfcontrol/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/_skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/generic2.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/pir3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch25.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/switch8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/weather19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/protocols/weather7.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/rfcontrol/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 14:57:19.000000 rfcontrolpy-0.0.3/rfcontrolpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:57:19.439018 rfcontrolpy-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    97702 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 14:57:05.000000 rfcontrolpy-0.0.3/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.043381 rfcontrolpy-0.0.4/rfcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/rfcontrol/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/_skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/generic2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/pir3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/switch8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/weather19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/protocols/weather7.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/rfcontrol/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 22:20:57.000000 rfcontrolpy-0.0.4/rfcontrolpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:20:57.047381 rfcontrolpy-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    97702 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 22:20:43.000000 rfcontrolpy-0.0.4/tests/test_helpers.py
```

### Comparing `rfcontrolpy-0.0.3/LICENSE` & `rfcontrolpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/PKG-INFO` & `rfcontrolpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcontrolpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library.
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/rfcontrolpy
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/rfcontrolpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `rfcontrolpy-0.0.3/README.md` & `rfcontrolpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/pyproject.toml` & `rfcontrolpy-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rfcontrolpy"
-version = "0.0.3"
+version = "0.0.4"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `rfcontrolpy-0.0.3/rfcontrol/controller.py` & `rfcontrolpy-0.0.4/rfcontrol/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 def prepare_compressed_pulses(input: str):
     """ """
     # Input is something like:
     # 268 2632 1282 10168 0 0 0 0 010002000202000002000200020200020002...
     # The first 8 numbers are the pulse length and the last string is the pulse sequence
     parts = input.split(" ")
-    pulse_lengths = [int(i) for i in parts[0:7]]
+    pulse_lengths = [int(i) for i in parts[0:8]]
     pulse_sequence = parts[8]
 
     # Now lets filter out 0 pulses
     pulse_lengths = list(filter(lambda pulse_length: pulse_length > 0, pulse_lengths))
 
     # Next sort the pulses from short to long and update indices in pulses.
     return sort_compressed_pulses(pulse_lengths, pulse_sequence)
```

### Comparing `rfcontrolpy-0.0.3/rfcontrol/helpers.py` & `rfcontrolpy-0.0.4/rfcontrol/helpers.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/__init__.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/_skeleton.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/_skeleton.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer1.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer1.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/dimmer2.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/dimmer2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/generic.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/generic.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/generic2.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/generic2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/pir3.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/pir3.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch1.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch1.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch10.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch10.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch11.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch11.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch2.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch2.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch25.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch25.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch3.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch3.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch4.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch4.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch5.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch5.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch6.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch6.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch7.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch7.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/switch8.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/switch8.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/weather19.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/weather19.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrol/protocols/weather7.py` & `rfcontrolpy-0.0.4/rfcontrol/protocols/weather7.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/rfcontrolpy.egg-info/PKG-INFO` & `rfcontrolpy-0.0.4/rfcontrolpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcontrolpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library with protocol support for different 433MHz switches and weather stations for the RFControl Arduino library.
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/rfcontrolpy
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/rfcontrolpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `rfcontrolpy-0.0.3/rfcontrolpy.egg-info/SOURCES.txt` & `rfcontrolpy-0.0.4/rfcontrolpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/tests/test_controller.py` & `rfcontrolpy-0.0.4/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `rfcontrolpy-0.0.3/tests/test_helpers.py` & `rfcontrolpy-0.0.4/tests/test_helpers.py`

 * *Files identical despite different names*

