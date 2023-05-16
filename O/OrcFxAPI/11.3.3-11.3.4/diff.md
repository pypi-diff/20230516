# Comparing `tmp/OrcFxAPI-11.3.3-py2.py3-none-any.whl.zip` & `tmp/OrcFxAPI-11.3.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 49911 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   317645 b- defN 23-Jan-18 17:15 OrcFxAPI.py
--rw-rw-rw-  2.0 fat     2027 b- defN 22-Nov-15 15:46 OrcFxAPIConfig.py
--rw-rw-rw-  2.0 fat     1137 b- defN 23-Feb-16 09:44 OrcFxAPI-11.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Feb-16 09:44 OrcFxAPI-11.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-Feb-16 09:44 OrcFxAPI-11.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      451 b- defN 23-Feb-16 09:44 OrcFxAPI-11.3.3.dist-info/RECORD
-6 files, 321394 bytes uncompressed, 49105 bytes compressed:  84.7%
+Zip file size: 49998 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat   318644 b- defN 23-Mar-29 15:40 OrcFxAPI.py
+-rw-rw-rw-  2.0 fat     2027 b- defN 22-Nov-08 15:58 OrcFxAPIConfig.py
+-rw-rw-rw-  2.0 fat     1137 b- defN 23-May-16 13:24 OrcFxAPI-11.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-16 13:24 OrcFxAPI-11.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 23-May-16 13:24 OrcFxAPI-11.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      451 b- defN 23-May-16 13:24 OrcFxAPI-11.3.4.dist-info/RECORD
+6 files, 322393 bytes uncompressed, 49192 bytes compressed:  84.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: OrcFxAPI.py
 Comment: 
 
 Filename: OrcFxAPIConfig.py
 Comment: 
 
-Filename: OrcFxAPI-11.3.3.dist-info/METADATA
+Filename: OrcFxAPI-11.3.4.dist-info/METADATA
 Comment: 
 
-Filename: OrcFxAPI-11.3.3.dist-info/WHEEL
+Filename: OrcFxAPI-11.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: OrcFxAPI-11.3.3.dist-info/top_level.txt
+Filename: OrcFxAPI-11.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: OrcFxAPI-11.3.3.dist-info/RECORD
+Filename: OrcFxAPI-11.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## OrcFxAPI.py

```diff
@@ -3482,14 +3482,25 @@
     ctypes.POINTER(ObjectExtra),
     ctypes.POINTER(Period),
     ctypes.c_int,
     ctypes.POINTER(RangeGraphCurveNames),
     ctypes.POINTER(ctypes.c_int),
 )
 
+_GetRangeGraphCurveNamesCollated = _bindToOrcFxAPI(
+    "C_GetRangeGraphCurveNamesCollatedW",
+    None,
+    Handle,
+    Handle,
+    ctypes.POINTER(ObjectExtra),
+    ctypes.c_int,
+    ctypes.POINTER(RangeGraphCurveNames),
+    ctypes.POINTER(ctypes.c_int),
+)
+
 _GetRangeGraphNumOfPoints = _bindToOrcFxAPI(
     "C_GetRangeGraphNumOfPoints",
     ctypes.c_int,
     Handle,
     ctypes.c_int,
     ctypes.POINTER(ctypes.c_int),
 )
@@ -3509,14 +3520,24 @@
     Handle,
     ctypes.POINTER(Period),
     ctypes.POINTER(ArclengthRange),
     ctypes.c_int,
     ctypes.POINTER(ctypes.c_int),
 )
 
+_GetRangeGraphNumOfPointsCollated = _bindToOrcFxAPI(
+    "C_GetRangeGraphNumOfPointsCollated",
+    ctypes.c_int,
+    Handle,
+    Handle,
+    ctypes.POINTER(ArclengthRange),
+    ctypes.c_int,
+    ctypes.POINTER(ctypes.c_int),
+)
+
 _GetRecommendedTimeSteps = _bindToOrcFxAPI(
     "C_GetRecommendedTimeSteps",
     None,
     Handle,
     ctypes.POINTER(TimeSteps),
     ctypes.POINTER(ctypes.c_int),
 )
@@ -8958,19 +8979,27 @@
             else:
                 return None
 
         status = ctypes.c_int()
         varID = obj.varID(varName)
         curveNames = RangeGraphCurveNames()
         defaultPeriod = HelperMethods.PreparePeriod(self.modelHandle, None)
-        _GetRangeGraphCurveNames(obj.handle, objectExtra, defaultPeriod, varID, curveNames, status)
-        _CheckStatus(status)
-        pointCount = HelperMethods.RangeGraphPointCount(
-            obj.handle, obj.type, varID, arclengthRange, defaultPeriod
-        )
+        if ImportedFunctionAvailable(_GetRangeGraphCurveNamesCollated):
+            _GetRangeGraphCurveNamesCollated(self.handle, obj.handle, objectExtra, varID, curveNames, status)
+            _CheckStatus(status)
+        else:
+            _GetRangeGraphCurveNames(obj.handle, objectExtra, defaultPeriod, varID, curveNames, status)
+            _CheckStatus(status)
+        if ImportedFunctionAvailable(_GetRangeGraphNumOfPointsCollated):
+            pointCount = _GetRangeGraphNumOfPointsCollated(self.handle, obj.handle, arclengthRange, varID, status)
+            _CheckStatus(status)
+        else:
+            pointCount = HelperMethods.RangeGraphPointCount(
+                obj.handle, obj.type, varID, arclengthRange, defaultPeriod
+            )
         x = _allocateArray(pointCount)
         min = allocIfCurveAvailable("Min", pointCount)
         max = allocIfCurveAvailable("Max", pointCount)
         mean = allocIfCurveAvailable("Mean", pointCount)
         stddev = allocIfCurveAvailable("StdDev", pointCount)
         upper = allocIfCurveAvailable("Upper", pointCount)
         lower = allocIfCurveAvailable("Lower", pointCount)
```

## Comparing `OrcFxAPI-11.3.3.dist-info/METADATA` & `OrcFxAPI-11.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OrcFxAPI
-Version: 11.3.3
+Version: 11.3.4
 Summary: Python interface to the OrcaFlex API
 Home-page: https://www.orcina.com/
 Author: Orcina
 Author-email: orcina@orcina.com
 License: Commercial
 Platform: Windows
 Requires-Python: >=3.6
```

