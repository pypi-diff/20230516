# Comparing `tmp/aiontutil-0.0.5.tar.gz` & `tmp/aiontutil-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiontutil-0.0.5.tar", max compression
+gzip compressed data, was "aiontutil-0.0.6.tar", max compression
```

## Comparing `aiontutil-0.0.5.tar` & `aiontutil-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.5/README.md
--rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.5/aiontutil/__init__.py
--rw-r--r--   0        0        0     4708 2023-05-11 08:20:57.105808 aiontutil-0.0.5/aiontutil/signal.py
--rw-r--r--   0        0        0      355 2023-05-11 08:22:45.517195 aiontutil-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 aiontutil-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.6/aiontutil/__init__.py
+-rw-r--r--   0        0        0     5234 2023-05-16 02:19:08.832054 aiontutil-0.0.6/aiontutil/signal.py
+-rw-r--r--   0        0        0      355 2023-05-16 02:21:52.085449 aiontutil-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 aiontutil-0.0.6/PKG-INFO
```

### Comparing `aiontutil-0.0.5/aiontutil/signal.py` & `aiontutil-0.0.6/aiontutil/signal.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,37 +82,55 @@
     "rms": get_rms,
     "skew": stats.skew,
     "std": np.std,
     "zcr": get_zcr,
 }
 
 
-def get_feature(x: np.ndarray, name=None, keepdims=False):
+def get_feature(x: np.ndarray, names=None) -> pd.DataFrame:
     """
     Examples
     --------
     >>> n_samples = 4
     >>> n_size = 1024
     >>> x = np.random.randn(n_samples, n_size)
-    >>> entropy = get_feature(x, name='entropy')
+    >>> feats = get_feature(x)
+    >>> isinstance(feats, pd.DataFrame)
+    True
+    >>> feats = get_feature(x, names="entropy")
+    >>> feats.shape
+    (4, 1)
+    >>> feats = get_feature(x, names=["entropy", "kurtosis"])
+    >>> feats.shape
+    (4, 2)
     """
     x = x.copy()
     if np.ndim(x) == 1:
         x = x[np.newaxis, ...]
 
-    if name is None:
-        name = "mean"
+    if names is None:
+        names = list_all_feature_names()
 
-    func = name_dict.get(name)
-    if not func:
+    if not isinstance(names, list):
+        names = [names]
+
+    if not set(names).issubset(names):
         raise TypeError("Unsupported provided name.")
-    out = func(x, axis=1)
-    if keepdims:
-        out = out[..., np.newaxis]
-    return out
+
+    feats = []
+    for name in names:
+        func = name_dict[name]
+        _x = abs(x.copy()) if name == "entropy" else x.copy()
+        partial_feats = func(_x, axis=1)
+        feats.append(partial_feats)
+
+    feats = np.array(feats).T.reshape(x.shape[0], len(names))
+    feats = pd.DataFrame(feats, columns=names)
+
+    return feats
 
 
 def get_spectral_feature(
     x: np.ndarray,
     fs: int,
     freq_intervals: list,
     names=None,
@@ -166,17 +184,17 @@
     for name in names:
         feats_given_name = []
         for interval in freq_intervals:
             start = interval[0]
             end = interval[-1]
             cond = np.where((start < freq) & (freq < end))[0]
 
-            partial_feats = get_feature(x=amps[..., cond], name=name)
-            feats_given_name.append(partial_feats)
+            partial_feats = get_feature(x=amps[..., cond], names=name)
+            feats_given_name.append(partial_feats.values.ravel())
         feats_given_name = np.array(feats_given_name).T
         feats.append(feats_given_name)
     feats = np.concatenate(feats, axis=1)
 
     columns = [f"{n}_{seg[0]}_{seg[1]}" for n in names for seg in freq_intervals]
-    feats = pd.DataFrame(np.array(feats), columns=columns)
+    feats = pd.DataFrame(feats, columns=columns)
     assert feats.shape == (x.shape[0], len(columns))
     return feats
```

### Comparing `aiontutil-0.0.5/PKG-INFO` & `aiontutil-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiontutil
-Version: 0.0.5
+Version: 0.0.6
 Summary: aiont utility package
 Author: jlan
 Author-email: jlan@aiont.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

