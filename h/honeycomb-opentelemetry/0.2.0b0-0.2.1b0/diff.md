# Comparing `tmp/honeycomb_opentelemetry-0.2.0b0.tar.gz` & `tmp/honeycomb_opentelemetry-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeycomb_opentelemetry-0.2.0b0.tar", max compression
+gzip compressed data, was "honeycomb_opentelemetry-0.2.1b0.tar", max compression
```

## Comparing `honeycomb_opentelemetry-0.2.0b0.tar` & `honeycomb_opentelemetry-0.2.1b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-12 10:22:34.666372 honeycomb_opentelemetry-0.2.0b0/LICENSE
--rw-r--r--   0        0        0     1612 2023-04-12 10:22:34.666372 honeycomb_opentelemetry-0.2.0b0/README.md
--rw-r--r--   0        0        0      836 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1416 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/baggage.py
--rw-r--r--   0        0        0     2665 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/distro.py
--rw-r--r--   0        0        0     3161 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/local_exporter.py
--rw-r--r--   0        0        0     1664 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/metrics.py
--rw-r--r--   0        0        0    15162 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/options.py
--rw-r--r--   0        0        0      842 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/resource.py
--rw-r--r--   0        0        0     3127 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/sampler.py
--rw-r--r--   0        0        0     2223 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/trace.py
--rw-r--r--   0        0        0      101 2023-04-12 10:22:34.670372 honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/version.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/LICENSE
+-rw-r--r--   0        0        0     1612 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/README.md
+-rw-r--r--   0        0        0      836 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1416 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     2750 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/distro.py
+-rw-r--r--   0        0        0     3161 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/local_exporter.py
+-rw-r--r--   0        0        0     1664 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    15162 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/options.py
+-rw-r--r--   0        0        0      842 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3266 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     2223 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/trace.py
+-rw-r--r--   0        0        0      101 2023-05-16 14:27:01.915888 honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/version.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.2.1b0/PKG-INFO
```

### Comparing `honeycomb_opentelemetry-0.2.0b0/LICENSE` & `honeycomb_opentelemetry-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/README.md` & `honeycomb_opentelemetry-0.2.1b0/README.md`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/pyproject.toml` & `honeycomb_opentelemetry-0.2.1b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "honeycomb-opentelemetry"
-version = "0.2.0b0"
+version = "0.2.1b0"
 description = "Honeycomb OpenTelemetry Distro for Python"
 authors = ["Honeycomb <support@honeycomb.io>"]
 readme = "README.md"
 packages = [{include = "honeycomb", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
```

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/baggage.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/distro.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/distro.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,41 @@
             debug=True,
             apikey=os.getenv("HONEYCOMB_API_KEY"),
             service_name="otel-python-example"
         )
     )
 """
 from logging import getLogger
+from typing import Optional
 from opentelemetry.instrumentation.distro import BaseDistro
 from opentelemetry.metrics import set_meter_provider
 from opentelemetry.trace import set_tracer_provider
 from honeycomb.opentelemetry.metrics import create_meter_provider
 from honeycomb.opentelemetry.options import HoneycombOptions
 from honeycomb.opentelemetry.resource import create_resource
 from honeycomb.opentelemetry.trace import create_tracer_provider
 
 _logger = getLogger(__name__)
 
 
 def configure_opentelemetry(
-    options: HoneycombOptions = HoneycombOptions(),
+    options: Optional[HoneycombOptions] = None,
 ):
     """
     Configures the OpenTelemetry SDK to send telemetry to Honeycomb.
 
     Args:
         options (HoneycombOptions, optional): the HoneycombOptions used to
         configure the the SDK. These options can be set either as parameters
         to this function or through environment variables
 
         Note: API key is a required option.
     """
+    if options is None:
+        options = HoneycombOptions()
     _logger.info("🐝 Configuring OpenTelemetry using Honeycomb distro 🐝")
     _logger.debug(vars(options))
     resource = create_resource(options)
     set_tracer_provider(
         create_tracer_provider(options, resource)
     )
     if options.metrics_dataset:
```

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/local_exporter.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/local_exporter.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/metrics.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/options.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/options.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/resource.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/sampler.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/sampler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from logging import getLogger
+from typing import Optional
 
 from opentelemetry.sdk.trace.sampling import (
     ALWAYS_OFF,
     ALWAYS_ON,
     TraceIdRatioBased,
     Sampler,
     SamplingResult
 )
 
 from opentelemetry.trace import Link, SpanKind
 from opentelemetry.trace.span import TraceState
 from opentelemetry.util.types import Attributes
 from opentelemetry.context import Context
 
-from honeycomb.opentelemetry.options import HoneycombOptions
+from honeycomb.opentelemetry.options import (
+    DEFAULT_SAMPLE_RATE,
+    HoneycombOptions
+)
 
 _logger = getLogger(__name__)
 
 
 def configure_sampler(
-    options: HoneycombOptions = HoneycombOptions(),
+    options: Optional[HoneycombOptions] = None,
 ):
     """Configures and returns an OpenTelemetry Sampler that is
     configured based on the sample_rate determined in HoneycombOptions.
     The configuration initializes a DeterministicSampler with
     an inner sampler of either AlwaysOn (1), AlwaysOff (0),
     or a TraceIdRatio as 1/N.
 
@@ -33,14 +37,17 @@
     Args:
         options (HoneycombOptions): the HoneycombOptions containing
         sample_rate used to configure the deterministic sampler.
 
     Returns:
         DeterministicSampler: the configured Sampler based on sample_rate
     """
+    if options is None:
+        return DeterministicSampler(DEFAULT_SAMPLE_RATE)
+
     return DeterministicSampler(options.sample_rate)
 
 
 class DeterministicSampler(Sampler):
     """Implementation of :class:`Sampler` that uses an inner sampler
     of either AlwaysOn (1), AlwaysOff (0), or a TraceIdRatio as 1/N
     to determine a SamplingResult and SamplingDecision for a given span
```

### Comparing `honeycomb_opentelemetry-0.2.0b0/src/honeycomb/opentelemetry/trace.py` & `honeycomb_opentelemetry-0.2.1b0/src/honeycomb/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.2.0b0/PKG-INFO` & `honeycomb_opentelemetry-0.2.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeycomb-opentelemetry
-Version: 0.2.0b0
+Version: 0.2.1b0
 Summary: Honeycomb OpenTelemetry Distro for Python
 Author: Honeycomb
 Author-email: support@honeycomb.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

