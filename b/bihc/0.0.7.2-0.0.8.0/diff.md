# Comparing `tmp/bihc-0.0.7.2.tar.gz` & `tmp/bihc-0.0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bihc-0.0.7.2.tar", last modified: Thu May  4 18:03:51 2023, max compression
+gzip compressed data, was "bihc-0.0.8.0.tar", last modified: Tue May 16 17:05:03 2023, max compression
```

## Comparing `bihc-0.0.7.2.tar` & `bihc-0.0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.873334 bihc-0.0.7.2/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-05-04 17:43:24.000000 bihc-0.0.7.2/LICENSE
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-05-04 17:43:24.000000 bihc-0.0.7.2/MANIFEST.in
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-04 18:03:51.873334 bihc-0.0.7.2/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-05-04 17:43:24.000000 bihc-0.0.7.2/README.md
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.512548 bihc-0.0.7.2/bihc/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/__init__.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27058 2023-05-04 18:03:15.000000 bihc-0.0.7.2/bihc/beam.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6251 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/impedance.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/plot.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 17:43:24.000000 bihc-0.0.7.2/bihc/power.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.732705 bihc-0.0.7.2/bihc.egg-info/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-04 18:03:51.000000 bihc-0.0.7.2/bihc.egg-info/SOURCES.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/dependency_links.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/requires.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-04 18:03:50.000000 bihc-0.0.7.2/bihc.egg-info/top_level.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-05-04 17:43:25.000000 bihc-0.0.7.2/pyproject.toml
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-04 18:03:51.873334 bihc-0.0.7.2/setup.cfg
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-04 18:03:28.000000 bihc-0.0.7.2/setup.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-04 18:03:51.826455 bihc-0.0.7.2/tests/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 17:43:26.000000 bihc-0.0.7.2/tests/test_analyticBunchShapes.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 17:43:26.000000 bihc-0.0.7.2/tests/test_numericBunchShapes.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.948450 bihc-0.0.8.0/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-05-04 17:43:24.000000 bihc-0.0.8.0/LICENSE
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-05-04 17:43:24.000000 bihc-0.0.8.0/MANIFEST.in
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-16 17:05:03.941222 bihc-0.0.8.0/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-05-04 17:43:24.000000 bihc-0.0.8.0/README.md
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.496882 bihc-0.0.8.0/bihc/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 17:43:24.000000 bihc-0.0.8.0/bihc/__init__.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27391 2023-05-16 11:07:39.000000 bihc-0.0.8.0/bihc/beam.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6330 2023-05-16 13:35:53.000000 bihc-0.0.8.0/bihc/impedance.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 17:43:24.000000 bihc-0.0.8.0/bihc/plot.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 17:43:24.000000 bihc-0.0.8.0/bihc/power.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.753240 bihc-0.0.8.0/bihc.egg-info/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/PKG-INFO
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/requires.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/top_level.txt
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-05-04 17:43:25.000000 bihc-0.0.8.0/pyproject.toml
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-16 17:05:03.950495 bihc-0.0.8.0/setup.cfg
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-16 17:02:58.000000 bihc-0.0.8.0/setup.py
+drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.865760 bihc-0.0.8.0/tests/
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 17:43:26.000000 bihc-0.0.8.0/tests/test_analyticBunchShapes.py
+-rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 17:43:26.000000 bihc-0.0.8.0/tests/test_numericBunchShapes.py
```

### Comparing `bihc-0.0.7.2/LICENSE` & `bihc-0.0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.2/PKG-INFO` & `bihc-0.0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.7.2
+Version: 0.0.8.0
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.7.2/README.md` & `bihc-0.0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.2/bihc/beam.py` & `bihc-0.0.8.0/bihc/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,26 @@
             return self._spectrum
         
     #@spectrum.setter
     def setSpectrum(self, newSpectrum): 
         self._spectrum = newSpectrum
         self._isSpectrumReady = True
         #raise Exception("Spectrum can not be assigned")
-                       
+                     
+    def setBunches(self, newLongitudinalProfile, interp=True):
+        [t,s] = newlongitudinalProfile
+    
+        if interp:
+            [to,so] = self.longitudinalProfile
+            s = np.interp(to, t, s)
+            t = to
+
+        self.profile_1_bunch = [t[0:self.ppbk], s[0:self.ppbk]]
+        self.longitudinalProfile = [t,s]
+
     def _setBunches(self):
         '''_setBunches method
 
         Computes the longitudinal profile of the bunches 
         with the shape specified in the class instance
 
          'GAUSSIAN', 'BINOMIAL' , 'COS2' or 'q-GAUSSIAN'
```

### Comparing `bihc-0.0.7.2/bihc/impedance.py` & `bihc-0.0.8.0/bihc/impedance.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,19 @@
         
         if unit == 'GHz':
             self.f= data[:,0]*1e9
         elif unit == 'MHz':
             self.f= data[:,0]*1e6
   
         self.Zr = data[:,1]
-        self.Zi = data[:,2]
+        try:
+            self.Zi = data[:,2]
+        except:
+            self.Zi = np.zeros_like(self.Zr)
+
         self.Z = self.Zr+1j*self.Zi
 
         return [self.f, self.Z]
     
     def getImpedanceFromPandas(self, path, unit='GHz'):
         import pandas as pd
```

### Comparing `bihc-0.0.7.2/bihc/plot.py` & `bihc-0.0.8.0/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.2/bihc/power.py` & `bihc-0.0.8.0/bihc/power.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.2/bihc.egg-info/PKG-INFO` & `bihc-0.0.8.0/bihc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.7.2
+Version: 0.0.8.0
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.7.2/setup.py` & `bihc-0.0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.7.2",
+    version="0.0.8.0",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.7.2/tests/test_analyticBunchShapes.py` & `bihc-0.0.8.0/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.7.2/tests/test_numericBunchShapes.py` & `bihc-0.0.8.0/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

