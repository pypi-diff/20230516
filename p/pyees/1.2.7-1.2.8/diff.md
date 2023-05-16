# Comparing `tmp/pyees-1.2.7.tar.gz` & `tmp/pyees-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.7.tar", last modified: Fri May 12 12:43:11 2023, max compression
+gzip compressed data, was "pyees-1.2.8.tar", last modified: Tue May 16 05:20:22 2023, max compression
```

## Comparing `pyees-1.2.7.tar` & `pyees-1.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:43:11.526607 pyees-1.2.7/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-05-12 12:43:11.542232 pyees-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 12:43:11.211525 pyees-1.2.7/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.2.7/pyees/__init__.py
--rw-rw-rw-   0        0        0    12829 2023-05-11 09:38:32.000000 pyees-1.2.7/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.7/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.7/pyees/prop.py
--rw-rw-rw-   0        0        0    17718 2023-05-12 12:35:32.000000 pyees-1.2.7/pyees/sheet.py
--rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.7/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.7/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.7/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.7/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.2.7/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15668 2023-05-12 12:42:26.000000 pyees-1.2.7/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.7/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.2.7/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81858 2023-05-12 06:34:53.000000 pyees-1.2.7/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.7/pyees/unit.py
--rw-rw-rw-   0        0        0    35130 2023-05-11 11:54:28.000000 pyees-1.2.7/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:43:11.463334 pyees-1.2.7/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-05-12 12:43:09.000000 pyees-1.2.7/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-12 12:43:09.000000 pyees-1.2.7/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:43:09.000000 pyees-1.2.7/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-12 12:43:09.000000 pyees-1.2.7/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 12:43:09.000000 pyees-1.2.7/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-12 12:43:11.589108 pyees-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-05-12 12:43:04.000000 pyees-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:20:22.614370 pyees-1.2.8/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-05-16 05:20:22.620355 pyees-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 05:20:22.458248 pyees-1.2.8/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.2.8/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12841 2023-05-16 05:19:59.000000 pyees-1.2.8/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.8/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.8/pyees/prop.py
+-rw-rw-rw-   0        0        0    17718 2023-05-12 12:35:32.000000 pyees-1.2.8/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.8/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.8/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.8/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.8/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.2.8/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15668 2023-05-12 12:42:26.000000 pyees-1.2.8/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.8/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.2.8/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81858 2023-05-12 06:34:53.000000 pyees-1.2.8/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.8/pyees/unit.py
+-rw-rw-rw-   0        0        0    35130 2023-05-16 05:20:22.473746 pyees-1.2.8/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:20:22.598413 pyees-1.2.8/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 05:20:22.607388 pyees-1.2.8/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-16 05:20:22.643293 pyees-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-05-16 05:20:04.000000 pyees-1.2.8/setup.py
```

### Comparing `pyees-1.2.7/LICENSE.txt` & `pyees-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/PKG-INFO` & `pyees-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.7
+Version: 1.2.8
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.7/README.md` & `pyees-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/fit.py` & `pyees-1.2.8/pyees/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         # scatter
         if showUncert:
             ax.errorbar(self.xVal, self.yVal, xerr=self.xUncert, yerr=self.yUncert, linestyle='', label=label, **kwargs)
         else:
             ax.scatter(self.xVal, self.yVal, label=label, **kwargs)
 
-    def plotNormalizedResiduals(self, ax, label = True, **kwargs):
+    def scatterNormalizedResiduals(self, ax, label = True, **kwargs):
         
         # parse label
         if isinstance(label, str):
             label = label
         elif label == True:
             label = 'Normalized residuals'
         elif label == False:
@@ -119,31 +119,31 @@
         else:
             raise ValueError('The label has to be a string, a bool or None')
         
         np.seterr('ignore')
         scale = variable(np.array([1 / ((elemX**2 + elemY**2)**(1/2)) for elemX, elemY in zip(self._sx, self._sy)]))
         normRes = scale * self._residuals
         np.seterr('warn')
-        ax.plot(self.xVal, normRes.value, label=label, **kwargs)
+        ax.scatter(self.xVal, normRes.value, label=label, **kwargs)
 
-    def plotResiduals(self, ax, label = True, **kwargs):
+    def scatterResiduals(self, ax, label = True, **kwargs):
         
         # parse label
         if isinstance(label, str):
             label = label
         elif label == True:
             label = 'Normalized residuals'
         elif label == False:
             label = None
         elif label is None:
             label = None
         else:
             raise ValueError('The label has to be a string, a bool or None')
         
-        ax.plot(self.xVal, self._residuals.value, label=label, **kwargs)
+        ax.scatter(self.xVal, self._residuals.value, label=label, **kwargs)
 
     def plotData(self, ax, label=True, **kwargs):
 
         # parse label
         if isinstance(label, str):
             label = label
         elif label == True:
```

### Comparing `pyees-1.2.7/pyees/profilePyees.py` & `pyees-1.2.8/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/prop.py` & `pyees-1.2.8/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/sheet.py` & `pyees-1.2.8/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/solve.py` & `pyees-1.2.8/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/stackOverflowODR.py` & `pyees-1.2.8/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testFit.py` & `pyees-1.2.8/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testProp.py` & `pyees-1.2.8/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testPyees.py` & `pyees-1.2.8/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testSheet.py` & `pyees-1.2.8/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testSolve.py` & `pyees-1.2.8/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testUnit.py` & `pyees-1.2.8/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/testVariable.py` & `pyees-1.2.8/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/unit.py` & `pyees-1.2.8/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees/variable.py` & `pyees-1.2.8/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.7/pyees.egg-info/PKG-INFO` & `pyees-1.2.8/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.7
+Version: 1.2.8
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.7/setup.py` & `pyees-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.7',
+    version='1.2.8',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

