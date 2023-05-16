# Comparing `tmp/logging_opentelemetry_format-0.0.1.tar.gz` & `tmp/logging_opentelemetry_format-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_opentelemetry_format-0.0.1.tar", last modified: Thu Dec  1 06:16:59 2022, max compression
+gzip compressed data, was "dist/logging_opentelemetry_format-0.0.2.tar", last modified: Tue May 16 08:46:05 2023, max compression
```

## Comparing `logging_opentelemetry_format-0.0.1.tar` & `logging_opentelemetry_format-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 06:16:59.672472 logging_opentelemetry_format-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2022-12-01 06:16:59.672472 logging_opentelemetry_format-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 06:16:59.668472 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 06:16:59.672472 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2022-12-01 06:16:59.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-01 06:16:59.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 06:16:59.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-01 06:16:59.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-01 06:16:59.000000 logging_opentelemetry_format-0.0.1/logging_opentelemetry_format.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-01 06:16:59.672472 logging_opentelemetry_format-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 06:16:59.672472 logging_opentelemetry_format-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2022-12-01 06:16:50.000000 logging_opentelemetry_format-0.0.1/tests/test_logging.py
+drwxr-xr-x   0 hiteshjha   (503) staff       (20)        0 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/
+-rw-r--r--   0 hiteshjha   (503) staff       (20)     2787 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/PKG-INFO
+drwxr-xr-x   0 hiteshjha   (503) staff       (20)        0 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format/
+-rw-r--r--   0 hiteshjha   (503) staff       (20)        0 2022-11-29 05:04:49.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format/__init__.py
+-rw-r--r--   0 hiteshjha   (503) staff       (20)     5884 2023-05-04 11:34:44.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format/utils.py
+drwxr-xr-x   0 hiteshjha   (503) staff       (20)        0 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/tests/
+-rw-r--r--   0 hiteshjha   (503) staff       (20)      966 2022-11-29 05:59:23.000000 logging_opentelemetry_format-0.0.2/tests/conftest.py
+-rw-r--r--   0 hiteshjha   (503) staff       (20)     1909 2023-05-16 08:29:01.000000 logging_opentelemetry_format-0.0.2/tests/test_logging.py
+-rw-r--r--   0 hiteshjha   (503) staff       (20)        0 2022-11-29 05:16:08.000000 logging_opentelemetry_format-0.0.2/tests/__init__.py
+-rw-r--r--   0 hiteshjha   (503) staff       (20)     2023 2022-12-01 05:49:19.000000 logging_opentelemetry_format-0.0.2/README.md
+drwxr-xr-x   0 hiteshjha   (503) staff       (20)        0 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format.egg-info/
+-rw-r--r--   0 hiteshjha   (503) staff       (20)     2787 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format.egg-info/PKG-INFO
+-rw-r--r--   0 hiteshjha   (503) staff       (20)      424 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format.egg-info/SOURCES.txt
+-rw-r--r--   0 hiteshjha   (503) staff       (20)       58 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format.egg-info/requires.txt
+-rw-r--r--   0 hiteshjha   (503) staff       (20)       35 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format.egg-info/top_level.txt
+-rw-r--r--   0 hiteshjha   (503) staff       (20)        1 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/logging_opentelemetry_format.egg-info/dependency_links.txt
+-rw-r--r--   0 hiteshjha   (503) staff       (20)      941 2023-05-05 08:11:56.000000 logging_opentelemetry_format-0.0.2/setup.py
+-rw-r--r--   0 hiteshjha   (503) staff       (20)      290 2023-05-16 08:46:05.000000 logging_opentelemetry_format-0.0.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `logging_opentelemetry_format-0.0.1/PKG-INFO` & `logging_opentelemetry_format-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: logging_opentelemetry_format
-Version: 0.0.1
-Summary: opentelemetry formatter for python logging module.
-Home-page: https://github.com/jha-hitesh/logging-opentelemetry-format
-Author: hitesh jha
-Author-email: hitesh4official@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # logging-opentelemetry-format
 
 a simple logging formatter which can be used to format logs to opentelemetry specification coming out from a system.
 it also provides some additional size control over log body and log attributes
 
 
 #### Installation
@@ -44,8 +31,8 @@
 - run the image `docker-compose up`
 - go to the container `docker exec -it loggingoplttester sh`
 - to run tests  `pytest tests/` to run the actual tests.
 
 
 #### License
 
-- this project is licensed under [MIT License](LICENSE)
+- this project is licensed under [MIT License](LICENSE)
```

### Comparing `logging_opentelemetry_format-0.0.1/logging_opentelemetry_format/utils.py` & `logging_opentelemetry_format-0.0.2/logging_opentelemetry_format/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Formatters."""
 import datetime
 import json
 import logging
+import os
+import socket
 
 from opentelemetry.sdk._logs import _RESERVED_ATTRS
 from opentelemetry.sdk._logs.severity import std_to_otlp
+from opentelemetry.sdk.environment_variables import (
+    OTEL_SERVICE_NAME,
+)
+from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace import (
     format_span_id,
     format_trace_id,
     get_current_span
 )
 import pkg_resources
 import ujson
@@ -16,17 +22,19 @@
 logger = logging.getLogger(__name__)
 
 
 class OpentelemetryLogFormatter(logging.Formatter):
     """OpentelemetryLogFormatter."""
 
     DEFAULT_RESOURCE = {
-        "telemetry.sdk.language": "python",
-        "telemetry.sdk.name": "opentelemetry",
-        "telemetry.sdk.version": pkg_resources.get_distribution(
+        ResourceAttributes.SERVICE_NAME: os.environ.get(OTEL_SERVICE_NAME, "unknown_service"),
+        ResourceAttributes.SERVICE_INSTANCE_ID: socket.gethostname(),
+        ResourceAttributes.TELEMETRY_SDK_LANGUAGE: "python",
+        ResourceAttributes.TELEMETRY_SDK_NAME: "opentelemetry",
+        ResourceAttributes.TELEMETRY_SDK_VERSION: pkg_resources.get_distribution(
             "opentelemetry-sdk"
         ).version,
     }
 
     MISSING_BODY_MESSAGE = "MissingLogBody"
 
     BODY_TOO_LARGE_ATTRIBUTE_NAME = "_body_too_large"
@@ -35,19 +43,16 @@
     META_ATTRIBUTE_NAME = "_meta"
     META_TOO_LARGE_ATTRIBUTE_NAME = "_meta_too_large"
     META_CHAR_LENGTH_ATTRIBUTE_NAME = "_meta_original_length"
 
     def __init__(self, **kwargs):
         """Init."""
         super().__init__()
-        self.resource_attributes = kwargs.get("resource_attributes") or {}
-        if not self.resource_attributes.get("service.name"):
-            raise Exception("service.name is mandatory in resource_attributes")
-        self.resource_attributes.update(self.DEFAULT_RESOURCE)
-        self.use_traces = kwargs.get("use_traces")
+        self.resource_attributes = {**self.DEFAULT_RESOURCE, **(kwargs.get("resource_attributes") or {})}
+        self.use_traces = kwargs.get("use_traces", True)
         self.json_indent = kwargs.get("json_indent", 0)
         self.meta_character_limit = kwargs.get("meta_character_limit", 1000)
         self.body_character_limit = kwargs.get("body_character_limit", 500)
 
         self.restrict_attributes_to = {
             self.BODY_TOO_LARGE_ATTRIBUTE_NAME, self.BODY_CHAR_LENGTH_ATTRIBUTE_NAME,
             self.META_TOO_LARGE_ATTRIBUTE_NAME, self.META_CHAR_LENGTH_ATTRIBUTE_NAME
```

### Comparing `logging_opentelemetry_format-0.0.1/setup.py` & `logging_opentelemetry_format-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="logging_opentelemetry_format",
-    version="0.0.1",
+    version="0.0.2",
     author="hitesh jha",
     author_email="hitesh4official@gmail.com",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jha-hitesh/logging-opentelemetry-format",
     packages=find_packages(
```

### Comparing `logging_opentelemetry_format-0.0.1/tests/conftest.py` & `logging_opentelemetry_format-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logging_opentelemetry_format-0.0.1/tests/test_logging.py` & `logging_opentelemetry_format-0.0.2/tests/test_logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,25 +36,19 @@
             "()": ListHandler,
             "formatter": "opentelemetry_formatter"
         }
     },
     "formatters": {
         "opentelemetry_formatter": {
             "()": OpentelemetryLogFormatter,
-            "use_traces": True,
             "restrict_attributes_to": [
                 "key1", "key2", "key3"
             ],
-            "discard_attributes_from": _RESERVED_ATTRS,
             "meta_character_limit": 100,
-            "body_character_limit": 10,
-            "resource_attributes": {
-                "service.name": "app-main-server",
-                "service.instance.id": socket.gethostname()
-            }
+            "body_character_limit": 10
         }
     },
     "loggers": {
         "": {
             "level": "DEBUG",
             "handlers": ["list"],
             "propagate": True
```

