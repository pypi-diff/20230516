# Comparing `tmp/ms2ml-0.0.7.tar.gz` & `tmp/ms2ml-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2ml-0.0.7.tar", max compression
+gzip compressed data, was "ms2ml-0.0.8.tar", max compression
```

## Comparing `ms2ml-0.0.7.tar` & `ms2ml-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2022-10-18 09:04:38.334050 ms2ml-0.0.7/LICENSE
--rw-r--r--   0        0        0      437 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/__init__.py
--rw-r--r--   0        0        0     2269 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/annotation_classes.py
--rw-r--r--   0        0        0     5969 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/config.py
--rw-r--r--   0        0        0      758 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/constants.py
--rw-r--r--   0        0        0      226 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/__init__.py
--rw-r--r--   0        0        0      453 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/adapters/__init__.py
--rw-r--r--   0        0        0     3002 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/adapters/base.py
--rw-r--r--   0        0        0     2427 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/adapters/msp.py
--rw-r--r--   0        0        0     5248 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/adapters/mzml.py
--rw-r--r--   0        0        0     5411 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/adapters/pin.py
--rw-r--r--   0        0        0     1710 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/adapters/spectronaut.py
--rw-r--r--   0        0        0        0 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/parsing/__init__.py
--rw-r--r--   0        0        0      861 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/parsing/base.py
--rw-r--r--   0        0        0     4909 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/parsing/bibliospec.py
--rw-r--r--   0        0        0     5924 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/parsing/msp.py
--rw-r--r--   0        0        0     5517 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/parsing/pin.py
--rw-r--r--   0        0        0     1084 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/parsing/spectronaut.py
--rw-r--r--   0        0        0    12022 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/data/utils.py
--rw-r--r--   0        0        0     4594 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/landmarks.py
--rw-r--r--   0        0        0     1412 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/metrics/base.py
--rw-r--r--   0        0        0    19187 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/peptide.py
--rw-r--r--   0        0        0     1210 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/proforma_utils.py
--rw-r--r--   0        0        0    20508 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/spectrum.py
--rw-r--r--   0        0        0       61 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/types.py
--rw-r--r--   0        0        0     9329 2022-10-18 09:04:38.334050 ms2ml-0.0.7/ms2ml/utils.py
--rw-r--r--   0        0        0     2595 2022-10-18 09:04:38.334050 ms2ml-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 ms2ml-0.0.7/setup.py
--rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 ms2ml-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-20 07:29:23.368790 ms2ml-0.0.8/LICENSE
+-rw-r--r--   0        0        0      437 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/__init__.py
+-rw-r--r--   0        0        0     2269 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/annotation_classes.py
+-rw-r--r--   0        0        0     5969 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/config.py
+-rw-r--r--   0        0        0      758 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/constants.py
+-rw-r--r--   0        0        0      226 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/__init__.py
+-rw-r--r--   0        0        0      453 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/adapters/__init__.py
+-rw-r--r--   0        0        0     3002 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/adapters/base.py
+-rw-r--r--   0        0        0     2427 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/adapters/msp.py
+-rw-r--r--   0        0        0     5335 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/adapters/mzml.py
+-rw-r--r--   0        0        0     5411 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/adapters/pin.py
+-rw-r--r--   0        0        0     1710 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/adapters/spectronaut.py
+-rw-r--r--   0        0        0        0 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/parsing/__init__.py
+-rw-r--r--   0        0        0      861 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/parsing/base.py
+-rw-r--r--   0        0        0     4909 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/parsing/bibliospec.py
+-rw-r--r--   0        0        0     5924 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/parsing/msp.py
+-rw-r--r--   0        0        0     5517 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/parsing/pin.py
+-rw-r--r--   0        0        0     1084 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/parsing/spectronaut.py
+-rw-r--r--   0        0        0    12022 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/data/utils.py
+-rw-r--r--   0        0        0     4594 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/landmarks.py
+-rw-r--r--   0        0        0     1412 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/metrics/base.py
+-rw-r--r--   0        0        0    19187 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/peptide.py
+-rw-r--r--   0        0        0     1210 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/proforma_utils.py
+-rw-r--r--   0        0        0    20676 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/spectrum.py
+-rw-r--r--   0        0        0       61 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/types.py
+-rw-r--r--   0        0        0     9329 2022-10-20 07:29:23.372789 ms2ml-0.0.8/ms2ml/utils.py
+-rw-r--r--   0        0        0     2595 2022-10-20 07:29:23.372789 ms2ml-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 ms2ml-0.0.8/setup.py
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 ms2ml-0.0.8/PKG-INFO
```

### Comparing `ms2ml-0.0.7/LICENSE` & `ms2ml-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/annotation_classes.py` & `ms2ml-0.0.8/ms2ml/annotation_classes.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/config.py` & `ms2ml-0.0.8/ms2ml/config.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/constants.py` & `ms2ml-0.0.8/ms2ml/constants.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/adapters/base.py` & `ms2ml-0.0.8/ms2ml/data/adapters/base.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/adapters/msp.py` & `ms2ml-0.0.8/ms2ml/data/adapters/msp.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/adapters/mzml.py` & `ms2ml-0.0.8/ms2ml/data/adapters/mzml.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,33 +37,34 @@
             out_hook=out_hook,
             in_hook=in_hook,
             collate_fn=collate_fn,
         )
         self.file = str(file)
         self.config = config
         self.out_hook = out_hook
+        self.reader = read_mzml(self.file)
 
-        with read_mzml(self.file) as reader:
-            # controllerType=0 controllerNumber=1 scan=2634
-            self._index_example = next(reader)["id"]
-            if "scan" in self._index_example:
-                template = re.sub(r"(?<=scan\=)\d+", "{}", self._index_example)
-                self._index_template = template
-
-            reader.reset()
-
-            reader.iterfind('referenceableParamGroup[@id="CommonInstrumentParams"]')
-            instrument_data = aux.cvquery(next(reader))
-            self.instrument = list(instrument_data.values())[0]
+        # controllerType=0 controllerNumber=1 scan=2634
+        self._index_example = next(self.reader)["id"]
+        if "scan" in self._index_example:
+            template = re.sub(r"(?<=scan\=)\d+", "{}", self._index_example)
+            self._index_template = template
+
+        self.reader.reset()
+
+        self.reader.iterfind('referenceableParamGroup[@id="CommonInstrumentParams"]')
+        instrument_data: dict
+        instrument_data = aux.cvquery(next(self.reader))  # type: ignore[operator]
+        self.instrument = list(instrument_data.values())[0]
 
     def parse(self):
-        with read_mzml(self.file) as reader:
-            for spec in reader:
-                spec["instrument"] = self.instrument
-                yield self._process_elem(spec)
+        self.reader.reset()
+        for spec in self.reader:
+            spec["instrument"] = self.instrument
+            yield self._process_elem(spec)
 
     def _to_elem(self, spec_dict):
         if "centroid spectrum" not in spec_dict:
             raise NotImplementedError(
                 "Only centroid spectra are supported at the moment."
             )
 
@@ -91,14 +92,18 @@
             }
             spec_dict.update(precursor_extras)
 
         elif "MS1 spectrum" in spec_dict:
             precursor_mz = None
             precursor_charge = None
 
+        else:
+            msg = f"Only MS1 and MSn spectra supported. got: {spec_dict}"
+            raise NotImplementedError(msg)
+
         rt = min([x["scan start time"] for x in spec_dict["scanList"]["scan"]])
         rt = RetentionTime(rt=float(rt), units=rt.unit_info, run=self.file)
 
         mz = spec_dict.pop("m/z array")
         intensity = spec_dict.pop("intensity array")
         ms_level = spec_dict.pop("ms level")
         instrument = spec_dict.pop("instrument")
@@ -121,28 +126,29 @@
 
         return spec_out
 
     def __repr__(self):
         return f"MS2ML MZML Adapter for {self.file}"
 
     def __getitem__(self, idx):
-        with read_mzml(self.file) as reader:
-            spec = None
-            if hasattr(self, "_index_template"):
-                try:
-                    spec = reader[self._index_template.format(idx)]
-                except TypeError:
-                    pass
-
-            if spec is None:
-                try:
-                    spec = reader[idx]
-                except TypeError:
-                    _ = "TypeError: 'NoneType' object is not subscriptable"
-                    err = f"Unable to find index {idx} in {self.file},"
-                    err += f" an example index is '{self._index_example}'"
-                    err = IndexError(err)
-                    raise err
+        reader = self.reader
+
+        spec = None
+        if hasattr(self, "_index_template"):
+            try:
+                spec = reader[self._index_template.format(idx)]
+            except TypeError:
+                pass
+
+        if spec is None:
+            try:
+                spec = reader[idx]
+            except TypeError:
+                _ = "TypeError: 'NoneType' object is not subscriptable"
+                err = f"Unable to find index {idx} in {self.file},"
+                err += f" an example index is '{self._index_example}'"
+                err = IndexError(err)
+                raise err
 
-        spec["instrument"] = self.instrument
+        spec["instrument"] = self.instrument  # type: ignore
         out = self._process_elem(spec)
         return out
```

### Comparing `ms2ml-0.0.7/ms2ml/data/adapters/pin.py` & `ms2ml-0.0.8/ms2ml/data/adapters/pin.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/adapters/spectronaut.py` & `ms2ml-0.0.8/ms2ml/data/adapters/spectronaut.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/parsing/base.py` & `ms2ml-0.0.8/ms2ml/data/parsing/base.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/parsing/bibliospec.py` & `ms2ml-0.0.8/ms2ml/data/parsing/bibliospec.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/parsing/msp.py` & `ms2ml-0.0.8/ms2ml/data/parsing/msp.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/parsing/pin.py` & `ms2ml-0.0.8/ms2ml/data/parsing/pin.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/parsing/spectronaut.py` & `ms2ml-0.0.8/ms2ml/data/parsing/spectronaut.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/data/utils.py` & `ms2ml-0.0.8/ms2ml/data/utils.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/landmarks.py` & `ms2ml-0.0.8/ms2ml/landmarks.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/metrics/base.py` & `ms2ml-0.0.8/ms2ml/metrics/base.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/peptide.py` & `ms2ml-0.0.8/ms2ml/peptide.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/proforma_utils.py` & `ms2ml-0.0.8/ms2ml/proforma_utils.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/ms2ml/spectrum.py` & `ms2ml-0.0.8/ms2ml/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         >>> spectrum
         Spectrum(mz=array([1000., 1500., 2000.]), ...)
     """
 
     mz: np.ndarray
     intensity: np.ndarray
     ms_level: int
-    precursor_mz: float
+    precursor_mz: float | None
     precursor_charge: int | None = None
     instrument: str | None = None
     analyzer: str | None = None
     extras: dict | None = None
     retention_time: RetentionTime | float | None = None
     config: Config | None = field(repr=False, default=None)
 
@@ -57,14 +57,18 @@
 
         if self.config is None:
             self.config = get_default_config()
 
         if self.retention_time is None:
             self.retention_time = RetentionTime(rt=np.nan, units="minutes")
 
+    def _reset_cache(self):
+        """Resets the cached properties."""
+        delattr(self, "_tic")
+
     def filter_mz_range(self, min_mz, max_mz) -> Spectrum:
         """Filters the spectrum to a given m/z range.
 
         Note:
             This is an in-place operation.
 
         Returns:
@@ -305,14 +309,15 @@
             AnnotatedPeptideSpectrum(mz=array([  50. ... precursor_isotope=0)
         """
         if isinstance(peptide, str):
             peptide = Peptide.from_sequence(peptide, config=self.config)
 
         spec_dict = dataclasses.asdict(self)
         spec_dict["config"] = self.config
+        spec_dict["retention_time"] = self.retention_time
         spec = AnnotatedPeptideSpectrum(precursor_peptide=peptide, **spec_dict)
         return spec
 
 
 def _bin_spectrum(
     mz: np.ndarray,
     weights: np.ndarray,
```

### Comparing `ms2ml-0.0.7/ms2ml/utils.py` & `ms2ml-0.0.8/ms2ml/utils.py`

 * *Files identical despite different names*

### Comparing `ms2ml-0.0.7/pyproject.toml` & `ms2ml-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms2ml"
-version = "0.0.7"
+version = "0.0.8"
 description = "Provides an intermediate layer between mass spec data and ML applications, such as encoding."
 authors = ["J. Sebastian Paez <jspaezp@users.noreply.github.com>"]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pyteomics = "^4.5.5"
```

### Comparing `ms2ml-0.0.7/setup.py` & `ms2ml-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 extras_require = \
 {':python_version > "3.8" and python_version < "3.11"': ['psims>=1.2.0,<2.0.0'],
  ':python_version >= "3.8" and python_version < "3.11"': ['pandas-stubs>=1.4.4.220919,<2.0.0.0'],
  ':python_version >= "3.8" and python_version < "3.9"': ['importlib-metadata>=5.0.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'ms2ml',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Provides an intermediate layer between mass spec data and ML applications, such as encoding.',
     'long_description': 'None',
     'author': 'J. Sebastian Paez',
     'author_email': 'jspaezp@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ms2ml-0.0.7/PKG-INFO` & `ms2ml-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2ml
-Version: 0.0.7
+Version: 0.0.8
 Summary: Provides an intermediate layer between mass spec data and ML applications, such as encoding.
 License: Apache 2.0
 Author: J. Sebastian Paez
 Author-email: jspaezp@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

