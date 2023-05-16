# Comparing `tmp/baseflow-0.0.7.tar.gz` & `tmp/baseflow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseflow-0.0.7.tar", last modified: Mon May 15 18:13:35 2023, max compression
+gzip compressed data, was "baseflow-0.0.8.tar", last modified: Tue May 16 20:46:19 2023, max compression
```

## Comparing `baseflow-0.0.7.tar` & `baseflow-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.818788 baseflow-0.0.7/
--rw-rw-rw-   0        0        0     2696 2023-05-15 18:13:35.817788 baseflow-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1964 2023-04-25 17:32:50.000000 baseflow-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.801788 baseflow-0.0.7/baseflow/
--rw-rw-rw-   0        0        0      243 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/__init__.py
--rw-rw-rw-   0        0        0     3424 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/comparision.py
--rw-rw-rw-   0        0        0   644797 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/example.csv
-drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.816788 baseflow-0.0.7/baseflow/methods/
--rw-rw-rw-   0        0        0      661 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Boughton.py
--rw-rw-rw-   0        0        0      587 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/CM.py
--rw-rw-rw-   0        0        0      606 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Chapman.py
--rw-rw-rw-   0        0        0      609 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/EWMA.py
--rw-rw-rw-   0        0        0      685 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Eckhardt.py
--rw-rw-rw-   0        0        0      644 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Fixed.py
--rw-rw-rw-   0        0        0      659 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Furey.py
--rw-rw-rw-   0        0        0      914 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/LH.py
--rw-rw-rw-   0        0        0     1534 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Local.py
--rw-rw-rw-   0        0        0      781 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Slide.py
--rw-rw-rw-   0        0        0     1510 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/UKIH.py
--rw-rw-rw-   0        0        0      783 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/Willems.py
--rw-rw-rw-   0        0        0      446 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/methods/__init__.py
--rw-rw-rw-   0        0        0     2766 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/param_estimate.py
--rw-rw-rw-   0        0        0     2393 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/separation.py
--rw-rw-rw-   0        0        0     3729 2023-04-25 17:32:50.000000 baseflow-0.0.7/baseflow/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 18:13:35.805787 baseflow-0.0.7/baseflow.egg-info/
--rw-rw-rw-   0        0        0     2696 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 18:13:35.000000 baseflow-0.0.7/baseflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 18:13:35.818788 baseflow-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3863 2023-05-15 18:11:53.000000 baseflow-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:46:19.419759 baseflow-0.0.8/
+-rw-rw-rw-   0        0        0     2696 2023-05-16 20:46:19.418757 baseflow-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1964 2023-04-25 17:32:50.000000 baseflow-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 20:46:19.398200 baseflow-0.0.8/baseflow/
+-rw-rw-rw-   0        0        0      216 2023-05-16 19:43:54.000000 baseflow-0.0.8/baseflow/__init__.py
+-rw-rw-rw-   0        0        0     3424 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/comparision.py
+-rw-rw-rw-   0        0        0   644797 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/example.csv
+drwxrwxrwx   0        0        0        0 2023-05-16 20:46:19.417757 baseflow-0.0.8/baseflow/methods/
+-rw-rw-rw-   0        0        0      661 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Boughton.py
+-rw-rw-rw-   0        0        0      587 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/CM.py
+-rw-rw-rw-   0        0        0      606 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Chapman.py
+-rw-rw-rw-   0        0        0      609 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/EWMA.py
+-rw-rw-rw-   0        0        0      685 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Eckhardt.py
+-rw-rw-rw-   0        0        0      644 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Fixed.py
+-rw-rw-rw-   0        0        0      659 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Furey.py
+-rw-rw-rw-   0        0        0      914 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/LH.py
+-rw-rw-rw-   0        0        0     1625 2023-05-16 14:23:19.000000 baseflow-0.0.8/baseflow/methods/Local.py
+-rw-rw-rw-   0        0        0      781 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Slide.py
+-rw-rw-rw-   0        0        0     1601 2023-05-16 14:23:21.000000 baseflow-0.0.8/baseflow/methods/UKIH.py
+-rw-rw-rw-   0        0        0      783 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/Willems.py
+-rw-rw-rw-   0        0        0      446 2023-04-25 17:32:50.000000 baseflow-0.0.8/baseflow/methods/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-16 20:40:17.000000 baseflow-0.0.8/baseflow/param_estimate.py
+-rw-rw-rw-   0        0        0     3759 2023-05-16 19:44:18.000000 baseflow-0.0.8/baseflow/separation.py
+-rw-rw-rw-   0        0        0    69206 2023-05-16 07:53:09.000000 baseflow-0.0.8/baseflow/thawed.npz
+-rw-rw-rw-   0        0        0     3305 2023-05-16 20:10:34.000000 baseflow-0.0.8/baseflow/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:46:19.403201 baseflow-0.0.8/baseflow.egg-info/
+-rw-rw-rw-   0        0        0     2696 2023-05-16 20:46:19.000000 baseflow-0.0.8/baseflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-05-16 20:46:19.000000 baseflow-0.0.8/baseflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 20:46:19.000000 baseflow-0.0.8/baseflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-16 20:46:19.000000 baseflow-0.0.8/baseflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 20:46:19.000000 baseflow-0.0.8/baseflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 20:46:19.419759 baseflow-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3884 2023-05-16 19:48:44.000000 baseflow-0.0.8/setup.py
```

### Comparing `baseflow-0.0.7/PKG-INFO` & `baseflow-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseflow
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package for baseflow separation
 Home-page: https://github.com/xiejx5/baseflow
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `baseflow-0.0.7/README.md` & `baseflow-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/comparision.py` & `baseflow-0.0.8/baseflow/comparision.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/example.csv` & `baseflow-0.0.8/baseflow/example.csv`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/Boughton.py` & `baseflow-0.0.8/baseflow/methods/Boughton.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/CM.py` & `baseflow-0.0.8/baseflow/methods/CM.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/Chapman.py` & `baseflow-0.0.8/baseflow/methods/Chapman.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/EWMA.py` & `baseflow-0.0.8/baseflow/methods/EWMA.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/Eckhardt.py` & `baseflow-0.0.8/baseflow/methods/Eckhardt.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/Fixed.py` & `baseflow-0.0.8/baseflow/methods/Fixed.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/Furey.py` & `baseflow-0.0.8/baseflow/methods/Furey.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/LH.py` & `baseflow-0.0.8/baseflow/methods/LH.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/Local.py` & `baseflow-0.0.8/baseflow/methods/Local.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     """Local minimum graphical method from HYSEP program (Sloto & Crouse, 1996)
 
     Args:
         Q (np.array): streamflow
         area (float): basin area in km^2
     """
     idx_turn = Local_turn(Q, hysep_interval(area))
+    if idx_turn.shape[0] < 3:
+        raise IndexError('Less than 3 turning points found')
     b = linear_interpolation(Q, idx_turn, return_exceed=return_exceed)
     b[:idx_turn[0]] = b_LH[:idx_turn[0]]
     b[idx_turn[-1] + 1:] = b_LH[idx_turn[-1] + 1:]
     return b
 
 
 def hysep_interval(area):
```

### Comparing `baseflow-0.0.7/baseflow/methods/Slide.py` & `baseflow-0.0.8/baseflow/methods/Slide.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/methods/UKIH.py` & `baseflow-0.0.8/baseflow/methods/UKIH.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
         Q (np.array): streamflow
     """
     N = 5
     block_end = Q.shape[0] // N * N
     idx_min = np.argmin(Q[:block_end].reshape(-1, N), axis=1)
     idx_min = idx_min + np.arange(0, block_end, N)
     idx_turn = UKIH_turn(Q, idx_min)
+    if idx_turn.shape[0] < 3:
+        raise IndexError('Less than 3 turning points found')
     b = linear_interpolation(Q, idx_turn, return_exceed=return_exceed)
     b[:idx_turn[0]] = b_LH[:idx_turn[0]]
     b[idx_turn[-1] + 1:] = b_LH[idx_turn[-1] + 1:]
     return b
 
 
 @njit
```

### Comparing `baseflow-0.0.7/baseflow/methods/Willems.py` & `baseflow-0.0.8/baseflow/methods/Willems.py`

 * *Files identical despite different names*

### Comparing `baseflow-0.0.7/baseflow/param_estimate.py` & `baseflow-0.0.8/baseflow/param_estimate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from numba import njit, prange
-from baseflow.utils import NSE, moving_average, multi_arange
+from baseflow.utils import moving_average, multi_arange
 
 
 def recession_coefficient(Q, strict):
     cQ, dQ = Q[1:-1], (Q[2:] - Q[:-2]) / 2
     cQ, dQ = cQ[strict[1:-1]], dQ[strict[1:-1]]
 
     idx = np.argsort(-dQ / cQ)[np.floor(dQ.shape[0] * 0.05).astype(int)]
@@ -15,24 +15,35 @@
 def param_calibrate(param_range, method, Q, b_LH, a):
     idx_rec = recession_period(Q)
     idx_oth = np.full(Q.shape[0], True)
     idx_oth[idx_rec] = False
     return param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth)
 
 
-@njit
+@njit(parallel=True)
 def param_calibrate_jit(param_range, method, Q, b_LH, a, idx_rec, idx_oth):
     logQ = np.log1p(Q)
     loss = np.zeros(param_range.shape)
     for i in prange(param_range.shape[0]):
         p = param_range[i]
         b_exceed = method(Q, b_LH, a, p, return_exceed=True)
         f_exd, logb = b_exceed[-1] / Q.shape[0], np.log1p(b_exceed[:-1])
-        NSE_rec = NSE(logQ[idx_rec], logb[idx_rec])
-        NSE_oth = NSE(logQ[idx_oth], logb[idx_oth])
+
+        # NSE for recession part
+        Q_obs, Q_sim = logQ[idx_rec], logb[idx_rec]
+        SS_res = np.sum(np.square(Q_obs - Q_sim))
+        SS_tot = np.sum(np.square(Q_obs - np.mean(Q_obs)))
+        NSE_rec = (1 - SS_res / (SS_tot + 1e-10)) - 1e-10
+
+        # NSE for other part
+        Q_obs, Q_sim = logQ[idx_oth], logb[idx_oth]
+        SS_res = np.sum(np.square(Q_obs - Q_sim))
+        SS_tot = np.sum(np.square(Q_obs - np.mean(Q_obs)))
+        NSE_oth = (1 - SS_res / (SS_tot + 1e-10)) - 1e-10
+
         loss[i] = 1 - (1 - (1 - NSE_rec) / (1 - NSE_oth)) * (1 - f_exd)
     return param_range[np.argmin(loss)]
 
 
 def recession_period(Q):
     idx_dec = np.zeros(Q.shape[0] - 1, dtype=np.int64)
     Q_ave = moving_average(Q, 3)
```

### Comparing `baseflow-0.0.7/baseflow/utils.py` & `baseflow-0.0.8/baseflow/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 from numba import njit
+from pathlib import Path
 
 
 def load_streamflow(path):
     """load streamflow into memory
 
     Args:
-        path (str|DataFrame): path of streamflow csv file, or pandas DataFrame
+        path (str|Path|DataFrame): path of streamflow csv file, or pandas DataFrame
 
     Returns:
         tuple: (date of np.datetime64, streamflow of float)
     """
-    if isinstance(path, str):
+    if isinstance(path, (str, Path)):
         date, Q = np.loadtxt(path, delimiter=',', skiprows=1, unpack=True,
                              dtype=[('date', 'datetime64[D]'), ('Q', float)],
                              converters={0: np.datetime64}, encoding='utf8')
         year = date.astype('datetime64[Y]').astype(int) + int(str(np.datetime64(0, 'Y')))
         month = date.astype('datetime64[M]').astype(int) % 12 + 1
         day = (date - date.astype('datetime64[M]')).astype(int) + 1
         date = np.rec.fromarrays([year, month, day], dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
@@ -28,29 +29,20 @@
         date = np.rec.fromarrays([path.index.year, path.index.month, path.index.day],
                                  dtype=[('Y', 'i4'), ('M', 'i4'), ('D', 'i4')])
         Q = path.values.astype(float)
     return clean_streamflow(date, Q)
 
 
 def clean_streamflow(date, Q):
-    Q = np.abs(Q)
+    has_value = np.isfinite(Q)
+    date, Q = date[has_value], np.abs(Q[has_value])
     year = date['Y']
-    year_unique = np.unique(year)
-    year_delete = clean_streamflow_jit(year, year_unique, Q)
-    idx_delete = np.isin(year, year_delete) | np.isnan(Q)
-    return Q[~idx_delete], date[~idx_delete]
-
-
-@njit
-def clean_streamflow_jit(year, year_unique, Q):
-    year_delete = []
-    for y in year_unique:
-        if (Q[year == y] >= 0).sum() < 120:
-            year_delete.append(y)
-    return year_delete
+    year_unique, counts = np.unique(year, return_counts=True)
+    keep = np.isin(year, year_unique[counts >= 120])
+    return Q[keep], date[keep]
 
 
 def exist_ice(date, ice_period):
     if (date is None) or (ice_period is None):
         return None
 
     if isinstance(ice_period, np.ndarray):
@@ -70,44 +62,32 @@
 
 def moving_average(x, w):
     res = np.convolve(x, np.ones(w)) / w
     return res[w - 1:-w + 1]
 
 
 @njit
-def multi_arange_steps(starts, stops, steps):
-    pos = 0
-    cnt = np.sum((stops - starts + steps - np.sign(steps)) // steps, dtype=np.int64)
-    res = np.zeros((cnt,), dtype=np.int64)
-    for i in range(starts.size):
-        v, stop, step = starts[i], stops[i], steps[i]
-        if step > 0:
-            while v < stop:
-                res[pos] = v
-                pos += 1
-                v += step
-        elif step < 0:
-            while v > stop:
-                res[pos] = v
-                pos += 1
-                v += step
-    assert pos == cnt
-    return res
-
-
-@njit
 def multi_arange(starts, stops):
     pos = 0
     cnt = np.sum(stops - starts, dtype=np.int64)
     res = np.zeros((cnt,), dtype=np.int64)
     for i in range(starts.size):
         num = stops[i] - starts[i]
         res[pos:pos + num] = np.arange(starts[i], stops[i])
         pos += num
     return res
 
 
-@njit
-def NSE(Q_obs, Q_sim):
-    SS_res = np.sum(np.square(Q_obs - Q_sim))
-    SS_tot = np.sum(np.square(Q_obs - np.mean(Q_obs)))
-    return (1 - SS_res / (SS_tot + 1e-10)) - 1e-10
+def geo2imagexy(x, y):
+    a = np.array([[0.5, 0.0], [0.0, -0.5]])
+    b = np.array([x - -180, y - 90])
+    col, row = np.linalg.solve(a, b) - 0.5
+    return np.round(col).astype(int), np.round(row).astype(int)
+
+
+def format_method(method):
+    if method == 'all':
+        method = ['UKIH', 'Local', 'Fixed', 'Slide', 'LH', 'Chapman',
+                  'CM', 'Boughton', 'Furey', 'Eckhardt', 'EWMA', 'Willems']
+    elif isinstance(method, str):
+        method = [method]
+    return method
```

### Comparing `baseflow-0.0.7/baseflow.egg-info/PKG-INFO` & `baseflow-0.0.8/baseflow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseflow
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package for baseflow separation
 Home-page: https://github.com/xiejx5/baseflow
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `baseflow-0.0.7/baseflow.egg-info/SOURCES.txt` & `baseflow-0.0.8/baseflow.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 baseflow/__init__.py
 baseflow/comparision.py
 baseflow/example.csv
 baseflow/param_estimate.py
 baseflow/separation.py
+baseflow/thawed.npz
 baseflow/utils.py
 baseflow.egg-info/PKG-INFO
 baseflow.egg-info/SOURCES.txt
 baseflow.egg-info/dependency_links.txt
 baseflow.egg-info/requires.txt
 baseflow.egg-info/top_level.txt
 baseflow/methods/Boughton.py
```

### Comparing `baseflow-0.0.7/setup.py` & `baseflow-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # Package meta-data.
 NAME = 'baseflow'
 DESCRIPTION = 'A python package for baseflow separation'
 URL = 'https://github.com/xiejx5/baseflow'
 EMAIL = 'xiejx5@gmail.com'
 AUTHOR = 'Cody James'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'numpy', 'numba',
+    'numpy', 'numba', 'tqdm', 'pandas'
 ]
 
 # What packages are optional?
 EXTRAS = {
-    'fancy feature': ['pandas', 'matplotlib', 'scipy'],
+    'fancy feature': ['matplotlib', 'scipy'],
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
@@ -102,15 +102,15 @@
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(
         exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={"baseflow": ["example.csv"]},
+    package_data={"baseflow": ["example.csv", "thawed.npz"]},
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['baseflow'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

