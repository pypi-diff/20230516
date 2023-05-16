# Comparing `tmp/rddensity-2.2.0.tar.gz` & `tmp/rddensity-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rddensity-2.2.0.tar", last modified: Wed May 25 17:47:15 2022, max compression
+gzip compressed data, was "rddensity-2.4.0.tar", last modified: Tue Jan 24 17:27:25 2023, max compression
```

## Comparing `rddensity-2.2.0.tar` & `rddensity-2.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-25 17:47:15.411818 rddensity-2.2.0/
--rw-r--r--   0 rajitachandak   (501) staff       (20)     1083 2022-05-25 17:47:15.411879 rddensity-2.2.0/PKG-INFO
--rw-r--r--   0 rajitachandak   (501) staff       (20)      575 2022-05-25 17:46:52.000000 rddensity-2.2.0/README.md
--rw-r--r--   0 rajitachandak   (501) staff       (20)      104 2022-05-25 17:46:52.000000 rddensity-2.2.0/pyproject.toml
--rw-r--r--   0 rajitachandak   (501) staff       (20)      725 2022-05-25 17:47:15.412155 rddensity-2.2.0/setup.cfg
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-25 17:47:15.410133 rddensity-2.2.0/src/
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-25 17:47:15.411091 rddensity-2.2.0/src/rddensity/
--rw-r--r--   0 rajitachandak   (501) staff       (20)      111 2022-05-25 17:46:52.000000 rddensity-2.2.0/src/rddensity/__init__.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    15242 2022-05-25 17:46:52.000000 rddensity-2.2.0/src/rddensity/funs.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    15291 2022-05-25 17:46:52.000000 rddensity-2.2.0/src/rddensity/rdbwdensity.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    27761 2022-05-25 17:46:52.000000 rddensity-2.2.0/src/rddensity/rddensity.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    11944 2022-05-25 17:46:52.000000 rddensity-2.2.0/src/rddensity/rdplotdensity.py
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-25 17:47:15.411716 rddensity-2.2.0/src/rddensity.egg-info/
--rw-r--r--   0 rajitachandak   (501) staff       (20)     1083 2022-05-25 17:47:15.000000 rddensity-2.2.0/src/rddensity.egg-info/PKG-INFO
--rw-r--r--   0 rajitachandak   (501) staff       (20)      353 2022-05-25 17:47:15.000000 rddensity-2.2.0/src/rddensity.egg-info/SOURCES.txt
--rw-r--r--   0 rajitachandak   (501) staff       (20)        1 2022-05-25 17:47:15.000000 rddensity-2.2.0/src/rddensity.egg-info/dependency_links.txt
--rw-r--r--   0 rajitachandak   (501) staff       (20)       44 2022-05-25 17:47:15.000000 rddensity-2.2.0/src/rddensity.egg-info/requires.txt
--rw-r--r--   0 rajitachandak   (501) staff       (20)       10 2022-05-25 17:47:15.000000 rddensity-2.2.0/src/rddensity.egg-info/top_level.txt
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-24 17:27:25.261452 rddensity-2.4.0/
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     3660 2023-01-24 17:27:25.261531 rddensity-2.4.0/PKG-INFO
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     3152 2023-01-24 16:50:18.000000 rddensity-2.4.0/README.md
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      104 2022-12-31 06:54:46.000000 rddensity-2.4.0/pyproject.toml
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      725 2023-01-24 17:27:25.261835 rddensity-2.4.0/setup.cfg
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-24 17:27:25.258038 rddensity-2.4.0/src/
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-24 17:27:25.260428 rddensity-2.4.0/src/rddensity/
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      111 2022-12-31 06:54:46.000000 rddensity-2.4.0/src/rddensity/__init__.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    15242 2022-12-31 06:54:46.000000 rddensity-2.4.0/src/rddensity/funs.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    15291 2022-12-31 06:54:46.000000 rddensity-2.4.0/src/rddensity/rdbwdensity.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    28351 2023-01-24 17:23:20.000000 rddensity-2.4.0/src/rddensity/rddensity.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    11944 2022-12-31 06:54:46.000000 rddensity-2.4.0/src/rddensity/rdplotdensity.py
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-24 17:27:25.261321 rddensity-2.4.0/src/rddensity.egg-info/
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     3660 2023-01-24 17:27:25.000000 rddensity-2.4.0/src/rddensity.egg-info/PKG-INFO
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      353 2023-01-24 17:27:25.000000 rddensity-2.4.0/src/rddensity.egg-info/SOURCES.txt
+-rw-r--r--   0 rajitachandak   (501) staff       (20)        1 2023-01-24 17:27:25.000000 rddensity-2.4.0/src/rddensity.egg-info/dependency_links.txt
+-rw-r--r--   0 rajitachandak   (501) staff       (20)       44 2023-01-24 17:27:25.000000 rddensity-2.4.0/src/rddensity.egg-info/requires.txt
+-rw-r--r--   0 rajitachandak   (501) staff       (20)       10 2023-01-24 17:27:25.000000 rddensity-2.4.0/src/rddensity.egg-info/top_level.txt
```

### Comparing `rddensity-2.2.0/setup.cfg` & `rddensity-2.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rddensity
-version = 2.2.0
+version = 2.4.0
 author = Rajita Chandak
 author_email = rchandak@princeton.edu
 description = Mainpulation testing based on Density Discontinuity
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rdpackages/rddensity
 project_urls =
```

### Comparing `rddensity-2.2.0/src/rddensity/funs.py` & `rddensity-2.4.0/src/rddensity/funs.py`

 * *Files identical despite different names*

### Comparing `rddensity-2.2.0/src/rddensity/rdbwdensity.py` & `rddensity-2.4.0/src/rddensity/rdbwdensity.py`

 * *Files identical despite different names*

### Comparing `rddensity-2.2.0/src/rddensity/rddensity.py` & `rddensity-2.4.0/src/rddensity/rddensity.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,31 +51,31 @@
     regularize: Boolean, Default *True*.
         Specifies whether to conduct local sample size checking. When True, the bandwidth is chosen such that the local region includes at least *nLocalMin* observations and at least *nUniqueMin* unique observations.
     nLocalMin: Nonnegative integer
         Specifies the minimum number of observations in each local neighbourhood. This option will be ignored if set to *0* or if *regularize=False*. Default is *20+p+1*.
     nUniqueMin: Nonnegative integer
         Specifies the minimum number of unqieu observations in each local neighbourhood. This option will be ignored if set to *0* or if *regularize=False*. Default is *20+p+1*.
     bino: Boolean (Default True).
-        Specifies whether to conduct binomial tests. By default the initial (smallest) window contains 20 observations, and its length is also used as the increment for subsequent windows.
+        Specifies whether to conduct binomial tests. By default the initial (smallest) window contains at least 20 observations on each side, and its length is also used as the increment for subsequent windows.
     binoW: Numeric.
         Specifies the half length(s) of the initial window. If two values are provided, they will be used for the data below and above the cutoff separately.
     binoN: Nonnegative integer.
-        Specifies the number of observations (closest to the cutoff) used for the binomial test. This is ignored if *binoW* is provided.
+        Specifies the minimum number of observations on each side of the cutoff used for the binomial test. This is ignored if *binoW* is provided.
     binoWStep: Numeric.
         Specifies the increment in half lengths.
     binoNStep: Nonnegative integer.
-        Specifies the increment in sample size. This is ignored if *binoWStep* is provided.
+        Specifies the minimum increment in sample size (on each side of the cutoff). This is ignored if *binoWStep* is provided.
     binoNW: Nonnegative integer.
         Specifies the total number of windows. Default is *10*.
     binoP: Numeric.
         Specifies the null hypothesis of the binomial test. Default is *0.5*.
 
     Returns
     -------
-    hat: 
+    hat:
         left/right: density estimate to the left/right of the cutoff. diff: difference in estimated densities on the two sides of the cutoff.
     sd_asy:
         left/right: standard error for the estimated density to the left/right of the cutoff, diff: standard error for difference in estimated densities on the two sides of the cutoff. (based on asymptotic method)
     sd_jk:
         left/right: standard error for the estimated density to the left/right of the cutoff, diff: standard error for difference in estimated densities on the two sides of the cutoff. (based on jackknife method)
     test:
         t_asy/t_jk: t statistic for the density discontinuity test. p_asy/p_jk: p-value for the density discontinuity test.
@@ -285,36 +285,36 @@
         elif binoP[0] < 0 or binoP[0] > 1:
             raise Exception("Option binoP incorrectly specified.")
 
         #binoW and binoN check
         if binoW is None:
             if binoN is None:
                 binoN = 20
-                binomTempLW[0] = XSort[XSort.columns[0]][min(binoN, n)-1]
-                binomTempRW[0] = XSort[XSort.columns[0]][min(binoN, n)-1]
+                binomTempLW[0] = max(XL[XL.columns[0]][min(binoN, nl)-1], XR[XR.columns[0]][min(binoN, nr)-1])
+                binomTempRW[0] = max(XL[XL.columns[0]][min(binoN, nl)-1], XR[XR.columns[0]][min(binoN, nr)-1])
             elif len(binoN) == 1:
                 if binoN <= 0 :
                     raise Exception("Option binoN incorrectly specified.")
                 binoN = math.ceil(binoN)
                 binomTempLW[0] = XSort[XSort.columns[0]][min(binoN, n)-1]
                 binomTempRW[0] = XSort[XSort.columns[0]][min(binoN, n)-1]
             else:
                 raise Exception("Option binoN incorrectly specified.")
         elif len(binoW) == 1:
             if binoW <= 0:
                 raise Exception("Option binoW incorrectly specified.")
             binomTempLW[0] = binoW
             binomTempRW[0] = binoW
-            binoN = sum(XL <= binomTemp[0]) + sum(XR <= binomTempRW[0])
+            binoN = min(sum(XL <= binomTempLW[0]), sum(XR <= binomTempRW[0]))
         elif len(binoW) == 2:
             if min(binoW) <= 0:
                 raise Exception("Option binoW incorrectly specified.")
             binomTempLW[0] = binoW[0]
             binomTempRW[0] = binoW[1]
-            binoN = sum(XL <= binomTemp[0]) + sum(XR <= binomTempRW[0])
+            binoN = min(sum(XL <= binomTempLW[0]), sum(XR <= binomTempRW[0]))
         else:
             raise Exception("Option binoW incorrectly specified.")
 
 
         #binoWStep check
         if binoNW >1 :
             if binoWStep is None:
@@ -334,17 +334,19 @@
                         else:
                             binomTempRW[1:(binoNW)] = binomTempRW[0] + np.array(range(1, binoNW))*binomTempRW[0]
 
                 elif len(binoNStep) == 1:
                     if binoNStep[0] <= 0:
                         raise Exception("Option binoNStep incorrectly specified.")
                     binoNStep = math.ceil(binoNStep)
-                    for jj in range(binoNW):
-                        binomTempLW[jj] = XSort[XSort.columns[0]][min(binoN + jj*binoNStep, n)]
-                        binomTempRW[jj] = XSort[XSort.columns[0]][min(binoN + jj*binoNStep, n)]
+                    for jj in range(1, binoNW):
+                        binomTempLW[jj] = binomTempLW[jj-1] + max(XL[XL.columns[0]][min(sum(XL<=binomTempLW[jj-1]) + binoNStep, nl)-1] - binomTempLW[jj-1],
+                                                                  XR[XR.columns[0]][min(sum(XL<=binomTempRW[jj-1]) + binoNStep, nr)-1] - binomTempRW[jj-1])
+                        binomTempRW[jj] = binomTempRW[jj-1] + max(XL[XL.columns[0]][min(sum(XL<=binomTempLW[jj-1]) + binoNStep, nl)-1] - binomTempLW[jj-1],
+                                                                  XR[XR.columns[0]][min(sum(XL<=binomTempRW[jj-1]) + binoNStep, nr)-1] - binomTempRW[jj-1])
                 else:
                     raise Exception("Option binoNStep incorrectly specified.")
             elif len(binoWStep) == 1:
                 if binWStep[0] <= 0:
                     raise Exception("Option binoWStep incorrectly specified.")
                 binomTempLW[1:(binoNW-1)] = binomTempLW[0] + np.array(range(binoNW))*binoWStep
                 binomTempRW[1:(binoNW-1)] = binomTempRW[0] + np.array(range(binoNW))*binoWStep
```

### Comparing `rddensity-2.2.0/src/rddensity/rdplotdensity.py` & `rddensity-2.4.0/src/rddensity/rdplotdensity.py`

 * *Files identical despite different names*

