# Comparing `tmp/naclib-1.0.0.tar.gz` & `tmp/naclib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naclib-1.0.0.tar", last modified: Fri Jul 22 14:52:14 2022, max compression
+gzip compressed data, was "naclib-1.0.1.tar", last modified: Tue Jul 26 13:51:36 2022, max compression
```

## Comparing `naclib-1.0.0.tar` & `naclib-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2022-07-22 14:52:14.625043 naclib-1.0.0/
--rw-rw-rw-   0        0        0     1229 2022-07-22 14:52:14.625043 naclib-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-22 14:52:14.625043 naclib-1.0.0/naclib/
--rw-rw-rw-   0        0        0        0 2021-01-12 12:56:50.952485 naclib-1.0.0/naclib/__init__.py
--rw-rw-rw-   0        0        0    19319 2022-07-22 14:33:15.251017 naclib-1.0.0/naclib/stpol.py
--rw-rw-rw-   0        0        0     3135 2022-04-19 17:18:19.168563 naclib-1.0.0/naclib/util.py
--rw-rw-rw-   0        0        0       63 2021-10-06 13:53:55.809142 naclib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1604 2022-07-22 14:51:54.693588 naclib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-26 13:51:36.016629 naclib-1.0.1/
+-rw-rw-rw-   0        0        0     1183 2022-07-26 13:51:36.016629 naclib-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-07-26 13:51:36.015607 naclib-1.0.1/naclib/
+-rw-rw-rw-   0        0        0        0 2022-07-26 11:23:34.612408 naclib-1.0.1/naclib/__init__.py
+-rw-rw-rw-   0        0        0    19344 2022-07-26 12:01:16.415656 naclib-1.0.1/naclib/stpol.py
+-rw-rw-rw-   0        0        0     3135 2022-07-26 11:23:34.612408 naclib-1.0.1/naclib/util.py
+-rw-rw-rw-   0        0        0       63 2022-07-26 11:23:34.612408 naclib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1558 2022-07-26 11:25:00.880747 naclib-1.0.1/setup.py
```

### Comparing `naclib-1.0.0/PKG-INFO` & `naclib-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: naclib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Non-Affine Corrections on microscopy images using S/T Polynomial Decomposition
-Home-page: https://gitlab.tudelft.nl/nynke-dekker-lab/public/naclib
+Home-page: https://github.com/edovanveen/naclib
 Author: Edo van Veen & Kaley McCluskey
-Author-email: e.n.w.vanveen@tudelft.nl
+Author-email: edovanveen@gmail.nl
 License: MIT
-Download-URL: https://gitlab.tudelft.nl/nynke-dekker-lab/public/naclib/-/raw/master/dist/naclib-1.0.0.tar.gz
+Download-URL: https://github.com/edovanveen/naclib/blob/master/dist/naclib-1.0.1.tar.gz
 Description: NAClib is a python library for applying a global alignment method for single-molecule fluorescence microscopy, using S/T Polynomial Decomposition (STPD). STPD employs linear combinations of Zernike polynomial gradients to decompose the distortion between two images, correcting both affine and higher-order components of the distortion in a single step, while requiring only minimal reference data.
 Keywords: colocalization,microscopy,distortion correction,STPD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `naclib-1.0.0/naclib/stpol.py` & `naclib-1.0.1/naclib/stpol.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 # Calculate derivatives from https://doi.org/10.1364/OE.26.018878
 # Use equations 44-51
 # Convert U to Z with equations 6-7
 # Checked results with https://doi.org/10.1364/OE.15.018014
 def get_Z_derivatives(j_max):
-    """Calculate Zernike polynomial derivatives."""
+    """Calculate Zernike polynomial derivatives, from https://doi.org/10.1364/OE.26.018878 eqs 44-51."""
     z = get_Rzern(j_max)
 
     dU_dx = dict()  # Key is (n, m) pair, value is dU_j/dx in terms of U coefficients starting at j=0
     dU_dy = dict()  # Key is (n, m) pair, value is dU_j/dy in terms of U coefficients starting at j=0
     Nj = np.zeros(j_max + 1)
     Nj[1] = Nnmu(*z.noll2nm(k=1))
     Nj[2] = Nnmu(*z.noll2nm(k=2))
@@ -205,26 +205,26 @@
 
     return Sx, Sy, Tx, Ty
 
 
 # Class that ties it all together.
 class STPolynomials:
     """ST-polynomials class for calculating the ST-polynomial decomposition coefficients of a distortion map,
-    and for calculating a correction field from decomposition coefficents."""
+    and for calculating a correction field from decomposition coefficents.
 
-    def __init__(self, j_max_S, j_max_T):
-        """Initialize.
+    Parameters
+    ----------
+    j_max_S : int
+        Maximum term for S-polynomials.
+    j_max_T : int
+        Maximum term for T-polynomials.
+    """
 
-        Parameters
-        ----------
-        j_max_S : int
-            Maximum term for S-polynomials.
-        j_max_T : int
-            Maximum term for T-polynomials.
-        """
+    def __init__(self, j_max_S, j_max_T):
+        """Initialize."""
 
         self.j_max_S = j_max_S
         self.j_max_T = j_max_T
         self.j_max_ST = max(j_max_S, j_max_T)
         self.cart = get_Rzern(self.j_max_ST)
         self.j_max = self.cart.nk
         self.Sx = dict()  # Key is j, value is Sj_x in terms of Z coefficients starting at j=1.
```

### Comparing `naclib-1.0.0/naclib/util.py` & `naclib-1.0.1/naclib/util.py`

 * *Files identical despite different names*

### Comparing `naclib-1.0.0/setup.py` & `naclib-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from distutils.core import setup
 
 setup(
     name='naclib',
     packages=['naclib'],
-    version='1.0.0',
+    version='1.0.1',
     license='MIT',
     description='Non-Affine Corrections on microscopy images using S/T Polynomial Decomposition',
     long_description='NAClib is a python library for applying a global alignment method ' + \
                      'for single-molecule fluorescence microscopy, using S/T Polynomial ' + \
                      'Decomposition (STPD). STPD employs linear combinations of Zernike ' + \
                      'polynomial gradients to decompose the distortion between two images, ' + \
                      'correcting both affine and higher-order components of the distortion ' + \
                      'in a single step, while requiring only minimal reference data.',
     author='Edo van Veen & Kaley McCluskey',
-    author_email='e.n.w.vanveen@tudelft.nl',
-    url='https://gitlab.tudelft.nl/nynke-dekker-lab/public/naclib',
-    download_url='https://gitlab.tudelft.nl/nynke-dekker-lab/public/naclib/-/raw/master/dist/naclib-1.0.0.tar.gz',
+    author_email='edovanveen@gmail.nl',
+    url='https://github.com/edovanveen/naclib',
+    download_url='https://github.com/edovanveen/naclib/blob/master/dist/naclib-1.0.1.tar.gz',
     keywords=['colocalization', 'microscopy', 'distortion correction', 'STPD'],
     install_requires=[
         'scipy',
         'numpy',
         'zernike',
         'h5py'
     ],
```

