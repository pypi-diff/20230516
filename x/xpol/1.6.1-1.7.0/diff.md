# Comparing `tmp/xpol-1.6.1.tar.gz` & `tmp/xpol-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xpol-1.6.1.tar", last modified: Tue Apr 19 11:33:46 2022, max compression
+gzip compressed data, was "xpol-1.7.0.tar", last modified: Tue May 16 12:43:24 2023, max compression
```

## Comparing `xpol-1.6.1.tar` & `xpol-1.7.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2022-04-19 11:33:46.000000 xpol-1.6.1/
-drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2022-04-19 11:33:46.000000 xpol-1.6.1/xpol.egg-info/
--rw-rw-r--   0 mtristra  (3192) planck     (236)      263 2022-04-19 11:33:43.000000 xpol-1.6.1/xpol.egg-info/SOURCES.txt
--rw-rw-r--   0 mtristra  (3192) planck     (236)       11 2022-04-19 11:33:43.000000 xpol-1.6.1/xpol.egg-info/top_level.txt
--rw-rw-r--   0 mtristra  (3192) planck     (236)        1 2022-04-19 11:33:43.000000 xpol-1.6.1/xpol.egg-info/dependency_links.txt
--rw-rw-r--   0 mtristra  (3192) planck     (236)     3531 2022-04-19 11:33:43.000000 xpol-1.6.1/xpol.egg-info/PKG-INFO
--rw-rw-r--   0 mtristra  (3192) planck     (236)       22 2022-04-19 11:33:43.000000 xpol-1.6.1/xpol.egg-info/requires.txt
--rw-rw-r--   0 mtristra  (3192) planck     (236)     2532 2022-04-19 10:50:45.000000 xpol-1.6.1/README.rst
-drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2022-04-19 11:33:46.000000 xpol-1.6.1/xpol/
--rw-rw-r--   0 mtristra  (3192) planck     (236)    29966 2022-04-19 11:13:04.000000 xpol-1.6.1/xpol/xpol.py
--rw-rw-r--   0 mtristra  (3192) planck     (236)    27511 2021-01-14 09:14:31.000000 xpol-1.6.1/xpol/xpol_sym.py
--rw-rw-r--   0 mtristra  (3192) planck     (236)       20 2020-12-01 08:21:32.000000 xpol-1.6.1/xpol/__init__.py
-drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2022-04-19 11:33:46.000000 xpol-1.6.1/src/
--rw-rw-r--   0 mtristra  (3192) planck     (236)    15156 2020-12-01 14:53:59.000000 xpol-1.6.1/src/xpol.h
--rw-rw-r--   0 mtristra  (3192) planck     (236)     4946 2022-04-19 11:13:28.000000 xpol-1.6.1/src/xpol.f90
--rw-rw-r--   0 mtristra  (3192) planck     (236)    13508 2020-12-01 14:53:59.000000 xpol-1.6.1/src/wig3j.f
--rw-rw-r--   0 mtristra  (3192) planck     (236)     6847 2020-12-01 14:53:59.000000 xpol-1.6.1/src/xpol_fits_param.h
--rw-rw-r--   0 mtristra  (3192) planck     (236)       38 2022-04-19 11:33:46.000000 xpol-1.6.1/setup.cfg
--rw-rw-r--   0 mtristra  (3192) planck     (236)     3531 2022-04-19 11:33:46.000000 xpol-1.6.1/PKG-INFO
--rw-rw-r--   0 mtristra  (3192) planck     (236)     1602 2022-04-19 11:32:09.000000 xpol-1.6.1/setup.py
+drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2023-05-16 12:43:24.780503 xpol-1.7.0/
+-rw-rw-r--   0 mtristra  (3192) planck     (236)     3535 2023-05-16 12:43:24.778648 xpol-1.7.0/PKG-INFO
+-rw-rw-r--   0 mtristra  (3192) planck     (236)     2532 2023-03-28 09:48:04.000000 xpol-1.7.0/README.rst
+-rw-rw-r--   0 mtristra  (3192) planck     (236)       38 2023-05-16 12:43:24.781911 xpol-1.7.0/setup.cfg
+-rw-rw-r--   0 mtristra  (3192) planck     (236)     1606 2023-05-16 12:41:19.000000 xpol-1.7.0/setup.py
+drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2023-05-16 12:43:24.712524 xpol-1.7.0/src/
+-rw-rw-r--   0 mtristra  (3192) planck     (236)    13508 2023-03-27 16:14:50.000000 xpol-1.7.0/src/wig3j.f
+-rw-rw-r--   0 mtristra  (3192) planck     (236)     4899 2023-05-16 12:32:16.000000 xpol-1.7.0/src/xpol.f90
+-rw-rw-r--   0 mtristra  (3192) planck     (236)    15156 2023-03-27 16:14:50.000000 xpol-1.7.0/src/xpol.h
+-rw-rw-r--   0 mtristra  (3192) planck     (236)     6847 2023-03-27 16:14:50.000000 xpol-1.7.0/src/xpol_fits_param.h
+drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2023-05-16 12:43:24.745089 xpol-1.7.0/xpol/
+-rw-rw-r--   0 mtristra  (3192) planck     (236)       20 2023-03-27 16:14:50.000000 xpol-1.7.0/xpol/__init__.py
+-rw-rw-r--   0 mtristra  (3192) planck     (236)    35032 2023-05-16 12:34:29.000000 xpol-1.7.0/xpol/xpol.py
+drwxrwsr-x   0 mtristra  (3192) planck     (236)        0 2023-05-16 12:43:24.770722 xpol-1.7.0/xpol.egg-info/
+-rw-rw-r--   0 mtristra  (3192) planck     (236)     3535 2023-05-16 12:43:24.000000 xpol-1.7.0/xpol.egg-info/PKG-INFO
+-rw-rw-r--   0 mtristra  (3192) planck     (236)      246 2023-05-16 12:43:24.000000 xpol-1.7.0/xpol.egg-info/SOURCES.txt
+-rw-rw-r--   0 mtristra  (3192) planck     (236)        1 2023-05-16 12:43:24.000000 xpol-1.7.0/xpol.egg-info/dependency_links.txt
+-rw-rw-r--   0 mtristra  (3192) planck     (236)       22 2023-05-16 12:43:24.000000 xpol-1.7.0/xpol.egg-info/requires.txt
+-rw-rw-r--   0 mtristra  (3192) planck     (236)       11 2023-05-16 12:43:24.000000 xpol-1.7.0/xpol.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xpol-1.6.1/xpol.egg-info/PKG-INFO` & `xpol-1.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.0
 Name: xpol
-Version: 1.6.1
+Version: 1.7.0
 Summary: XPOL cross power-spectrum estimator
 Home-page: UNKNOWN
 Author: Matthieu Tristram
-Author-email: tristram@lal.in2p3.fr
+Author-email: matthieu.tristram@cnrs.fr
 License: UNKNOWN
 Description: ====
         Xpol
         ====
         
         A code to compute angular power spectra based on cross-correlation between maps and covariance matrices.
         
@@ -20,15 +20,15 @@
         Install Python
         ==============
         
         The easiest way to install ``Xpol`` is via ``pip``
         
         .. code:: shell
         
-         pip install pspy [--user]
+         pip install xpol [--user]
         
         
         If you plan to develop the code, it is better to clone the repository
         
         .. code:: shell
         
          git clone https://gitlab.in2p3.fr/tristram/Xpol.git /where/to/clone
```

### Comparing `xpol-1.6.1/README.rst` & `xpol-1.7.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Install Python
 ==============
 
 The easiest way to install ``Xpol`` is via ``pip``
 
 .. code:: shell
 
- pip install pspy [--user]
+ pip install xpol [--user]
 
 
 If you plan to develop the code, it is better to clone the repository
 
 .. code:: shell
 
  git clone https://gitlab.in2p3.fr/tristram/Xpol.git /where/to/clone
```

### Comparing `xpol-1.6.1/xpol/xpol.py` & `xpol-1.7.0/xpol/xpol.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from __future__ import division
 
 import healpy as hp
 import numpy as np
 import _flib as flib
 import os
 from astropy.io import fits
+import logging
 
-__all__ = ['Xpol','Xcov','Bins','fsky','Xpol_Wrapper','apodization','sample_variance','listcross']
+__all__ = ['Xpol','Xcov','Bins','fsky','Xpol_Wrapper','apodization','sample_variance','listcross','fit_dipole']
 
+log = logging.getLogger("healpy")
 
 
 def fsky(mask):
     """
     Return sky fraction as fsky = <m^2>**2 / <m^4> 
     """
     return np.mean(mask**2)**2/np.mean(mask**4)
 
 def apodization( mask, deg, threshold=1e-5, method="Gaussian"):
+    log.setLevel(logging.INFO)
+    
     if method == "Gaussian":
-        smask = hp.smoothing( mask, fwhm=np.deg2rad(deg), verbose=False)
+        smask = hp.smoothing( mask, fwhm=np.deg2rad(deg))
         smask[smask < (0. + threshold)] = 0.+ threshold
         smask[smask > (1. - threshold)] = 1.- threshold
     else:
         print( "Method allowed: Gaussian")
         return
     return smask
 
@@ -37,29 +41,52 @@
 
     Optional:
         fsky: sky fraction (default=1)
 
     Output:
         array of cosmic variance
     """
-    cosmic = np.sqrt( 2./(2*l+1))/fsky * cl
-    cosmic[3] = np.sqrt( 1./(2*l+1)*(cl[0]*cl[1]+cl[3]*cl[3]))/fsky
+    acl = np.asarray( cl)
+    cosmic = 2./(2*l+1)/fsky * acl*acl
+    cosmic[3] = (acl[0]*acl[1]+acl[3]*acl[3])/(2*l+1)/fsky
     if len(cl) > 4:
-        cosmic[4] = np.sqrt( 1./(2*l+1)*(cl[0]*cl[2]+cl[4]*cl[4]))/fsky
+        cosmic[4] = (acl[0]*acl[2]+acl[4]*acl[4])/(2*l+1)/fsky
     if len(cl) > 5:
-        cosmic[5] = np.sqrt( 1./(2*l+1)*(cl[1]*cl[2]+cl[5]*cl[5]))/fsky
+        cosmic[5] = (acl[1]*acl[2]+acl[5]*acl[5])/(2*l+1)/fsky
 
     return cosmic
 
-def listcross( nmap, auto=False):
+def get_variance( clAB, clBA, clAA, clBB, fsky=1.):
+    """
+    Compute cross-spectra variance for a given sky fraction
+
+    Inputs:
+        clAB, clBA, clAA, clBB: arrays of power spectra (can be any length but order should be TT,EE,BB,TE,TB,EB)
+
+    Optional:
+        fsky: sky fraction (default=1)
+
+    Output:
+        array of cross-spectra variance
+    """
+    ntag,nell = np.shape(clAB)
+    ell = np.arange( nell)
+    var = abs(clAA*clBB + clAB*clBA) / (2*ell+1) / fsky
+    var[3] = abs(clAA[0]*clBB[1] + clAB[3]*clBA[3]) / (2*ell+1) / fsky  #TE
+    var[4] = abs(clAA[0]*clBB[2] + clAB[4]*clBA[4]) / (2*ell+1) / fsky  #TB
+    var[5] = abs(clAA[1]*clBB[2] + clAB[5]*clBA[5]) / (2*ell+1) / fsky  #EB
+
+    return var
+
+def listcross( listmap, auto=False):
     import itertools
     if auto:
-        return list(itertools.combinations_with_replacement(np.arange(nmap),2))
+        return list(itertools.combinations_with_replacement(listmap,2))
     else:
-        return list(itertools.combinations(np.arange(nmap),2))
+        return list(itertools.combinations(listmap,2))
 
 
 class Bins(object):
     """
         lmins : list of integers
             Lower bound of the bins
         lmaxs : list of integers
@@ -144,18 +171,18 @@
     """
     (Cross-) power spectra estimation using the Xpol method.
     Hinshaw et al. 2003, Tristram et al. 2005.
 
     Example
     -------
     import xpol
-    bins = xpol.Bins( lmins, lmaxs)
-    xp = xpol.Xpol(mask, bins)
-    biased, unbiased = xp.get_spectra(map)
-    biased, unbiased = xp.get_spectra(map1, map2)
+    binning = xpol.Bins( lmins, lmaxs)
+    xp = xpol.Xpol(mask, bins=binning)
+    pcl,cl = xp.get_spectra( dT, Dl=True)
+    pcl12,cl12 = xp.get_spectra( dT1, dT2, Dl=True)
 
     """
     def __init__(self, mask, mask2=None, bins=None, polar=True, verbose=False, wlmax=None, Dl=False):
         """
 
         Inputs
         ------
@@ -175,37 +202,42 @@
             bins = Bins.fromdeltal(2,3*self.nside-1,1)
         self.lmin = int(bins.lmin)
         self.lmax = int(bins.lmax)
         self.verbose = verbose
         self.polar = polar
         if self.lmax > 3*self.nside-1:
             raise ValueError('Input lmax is too high for resolution.')
+
+        if verbose:
+            log.setLevel(logging.DEBUG)
+        else:
+            log.setLevel(logging.INFO)
         
-        if self.verbose: print( "Compute bin operators")
+        if self.verbose: print( "\tCompute bin operators")
         self._p, self._q = bins._bin_operators(Dl=Dl)
         self.lbin = bins.lbin
         self.bin_spectra = bins.bin_spectra
         
         #compute cross-spectrum of weight mask
-        if self.verbose: print( "alm2map mask")
+        if self.verbose: print( "\talm2map mask")
         if wlmax is None:
-            wlmax = self.lmax
+            wlmax = self.lmax ###3*self.nside-1
         if mask2 is None:
             wl = hp.anafast(mask,lmax=wlmax)
             self.mask = self.mask2 = mask
         else:
             wl = hp.anafast(mask,map2=mask2,lmax=wlmax)
             self.mask  = mask
-            self.mask2 = mask2        
+            self.mask2 = mask2
         
         #compute coupling kernels for covariance
-        if self.verbose: print( "Compute coupling kernels Mll")
+        if self.verbose: print( "\tCompute coupling kernels Mll")
         mll_binned = self._get_Mbb( wl)
-
-        if self.verbose: print( "Inverse Mll")
+        
+        if self.verbose: print( "\tInverse Mll")
         self.mll_binned_inv = self._inv_mll(mll_binned)
 
     def get_spectra(self, m1, m2=None, bell=None, bell1=None, bell2=None, pixwin=True, Dl=False, remove_dipole=True, iter=3):
         """
         Return biased and Xpol-debiased estimations of the power spectra of
         a Healpix map or of the cross-power spectra if *map2* is provided.
         
@@ -232,84 +264,90 @@
             The anafast's pseudo (cross-) power spectra for TT,EE,BB,TE,TB,EB,ET,BT,BE.
             The corresponding l values are given by `np.arange(lmax + 1)`.
 
         unbiased : float array of shape (9, nbins)
             The Xpol's (cross-) power spectra for TT,EE,BB,TE,TB,EB,ET,BT,BE.
             The corresponding l values are given by `xpol.lbin`.
         """
-
+        cross = m2 is not None
+        npix = hp.nside2npix(self.nside)
+        
         #Map1
         if self.verbose:
-            if m2 is None:
-                print( "Compute alms")
+            if cross:
+                print( "\tCompute alms map1")
             else:
-                print( "Compute alms map1")
+                print( "\tCompute alms")
         map1 = np.array(m1)
         if map1.shape[-1] == 3:
             map1 = map1.T
-        
+        map1 = map1.reshape(-1,npix)
         self._removeUndef(map1)
         if remove_dipole: self._remove_dipole( map1[0], self.mask, bad=0.)
         alms1 = hp.map2alm(map1*self.mask, pol=self.polar, lmax=self.lmax, iter=iter)
         del(map1)
         
         #Map2
-        if m2 is None:
-            alms2 = alms1
-        else:
-            if self.verbose: print( "Compute alms map2")
+        if cross:
+            if self.verbose: print( "\tCompute alms map2")
             map2 = np.array(m2)
             if map2.shape[-1] == 3:
                 map2 = map2.T
+            map2 = map2.reshape(-1,npix)
             self._removeUndef(map2)
             if remove_dipole: self._remove_dipole( map2[0], self.mask2, bad=0.)
             alms2 = hp.map2alm( map2*self.mask2, pol=self.polar, lmax=self.lmax, iter=iter)
             del(map2)
-        
+        else:
+            alms2 = alms1
+
         #alm2cl
-        if self.verbose: print( "Alms 2 cl")
+        if self.verbose: print( "\tAlms 2 cl")
         biased = hp.alm2cl( alms1, alms2, lmax=self.lmax) #healpy order (TT,EE,BB,TE,EB,TB)
         if self.polar:
             biased = biased[[0,1,2,3,5,4]] #swith TB and EB
-            biased21 = hp.alm2cl( alms2, alms1, lmax=self.lmax)
-            biased21 = biased21[[0,1,2,3,5,4]] #swith TB and EB
-            biased = np.array( np.concatenate( (biased, biased21[[3,4,5]]))) #concatenate with alms2xalms1
+            if cross:
+                biased21 = hp.alm2cl( alms2, alms1, lmax=self.lmax)
+                biased21 = biased21[[0,1,2,3,5,4]] #swith TB and EB
+                biased = np.array( np.concatenate( (biased, biased21[[3,4,5]]))) #concatenate with alms2xalms1
         del( alms1)
         del( alms2)
         
         #beam function
-        if self.verbose: print( "Correct beams")
+        if self.verbose: print( "\tCorrect beams")
         if bell is not None:
             bl = bell[:self.lmax+1]**2
         else:
             bl = np.ones(self.lmax+1)
         if bell1 is not None:
             if bell2 is None:
                 bell2 = bell1
             bl *= bell1[:self.lmax+1]*bell2[:self.lmax+1]
         if pixwin:
             bl *= hp.pixwin(self.nside)[:self.lmax+1]**2
         
         #bin spectra
-        if self.verbose: print( "Bin spectrum")
+        if self.verbose: print( "\tBin spectrum")
         binned = self.bin_spectra(biased,Dl=Dl)
         
         #debias
-        if self.verbose: print( "Debias spectra")
+        if self.verbose: print( "\tDebias spectra")
         unbiased = self._debias_spectra( binned)
         unbiased /= self.bin_spectra(bl,Dl=False)
         
         return biased, unbiased
 
     def _debias_spectra(self, binned):
+        cross = len(binned) == 9
+        
         if self.polar:
             TT_TT, EE_EE, EE_BB, TE_TE = self.mll_binned_inv
         else:
             TT_TT = self.mll_binned_inv
-
+        
         n = len(TT_TT)
         if self.polar is False:
             TT = np.dot( TT_TT, binned)
             return np.asarray(TT)
         
         out = np.zeros( (2*n,2*n) )
         out[0*n:1*n, 0*n:1*n] = EE_EE
@@ -319,58 +357,61 @@
         vec = np.dot( out, binned[1:3].ravel())
         
         TT = np.dot( TT_TT, binned[0])
         EE = vec[0:n]
         BB = vec[n:]
         TE = np.dot( TE_TE, binned[3])
         TB = np.dot( TE_TE, binned[4])
-        ET = np.dot( TE_TE, binned[6])
-        BT = np.dot( TE_TE, binned[7])
+        if cross:
+            ET = np.dot( TE_TE, binned[6])
+            BT = np.dot( TE_TE, binned[7])
+        
+        if cross:
+            out[0*n:1*n, 0*n:1*n] = EE_EE
+            out[1*n:2*n, 1*n:2*n] = EE_EE
+            out[0*n:1*n, 1*n:2*n] = -EE_BB
+            out[1*n:2*n, 0*n:1*n] = -EE_BB
+            vec = np.dot( out, binned[[5,8]].ravel())
+            EB = vec[0:n]
+            BE = vec[n:]
+        else:
+            EB = np.dot( EE_EE, binned[5])
 
-        out[0*n:1*n, 0*n:1*n] = EE_EE
-        out[1*n:2*n, 1*n:2*n] = EE_EE
-        out[0*n:1*n, 1*n:2*n] = -EE_BB
-        out[1*n:2*n, 0*n:1*n] = -EE_BB
-        vec = np.dot( out, binned[[5,8]].ravel())
-        EB = vec[0:n]
-        BE = vec[n:]
-        
-        return np.asarray( [TT,EE,BB,TE,TB,EB,ET,BT,BE])
+        if cross:
+            spec = [TT,EE,BB,TE,TB,EB,ET,BT,BE]
+        else:
+            spec = [TT,EE,BB,TE,TB,EB]
+
+        return spec
 
     def _replaceUndefWith0(self,mymap):
         badpix = np.isclose( mymap,hp.UNSEEN)
         mymap[badpix] = 0.
-#        for i in range(len(mymap)):
-#            if np.isclose( mymap[i],hp.UNSEEN):
-#                mymap[i] = 0.
 
     def _removeUndef(self,mymap):
-        if self.polar:
-            for m in mymap:
-                self._replaceUndefWith0( m)
-        else:
-            self._replaceUndefWith0( mymap)
+        for m in mymap:
+            self._replaceUndefWith0( m)
 
     def _remove_dipole(self, m, mask, bad=hp.UNSEEN):
         npix = m.size
         nside = hp.npix2nside(npix)
         bunchsize = npix // 24 if nside > 128 else npix
 
-        #fit dipole with mask
-        mono, dipole = hp.fit_dipole(m*mask, bad=0.)
+        #fit dipole where mask != 0
+        mono, dipole = hp.fit_dipole(m*(mask>0), bad=0.)
 
         #remove dipole
         for ibunch in range(npix // bunchsize):
             ipix = np.arange(ibunch * bunchsize, (ibunch + 1) * bunchsize)
             ipix = ipix[(m.flat[ipix] != bad) & (np.isfinite(m.flat[ipix]))]
             x, y, z = hp.pix2vec(nside, ipix)
+            m.flat[ipix] -= mono
             m.flat[ipix] -= dipole[0] * x
             m.flat[ipix] -= dipole[1] * y
             m.flat[ipix] -= dipole[2] * z
-            m.flat[ipix] -= mono
 
     def _inv_mll(self, mll_binned):
         if self.polar:
             TT_TT, EE_EE, EE_BB, TE_TE = mll_binned
         else:
             TT_TT = mll_binned
 
@@ -431,48 +472,82 @@
 
 class Xcov(Xpol):
     """
     (Cross-) power spectra covariance matrix estimation.
     Tristram et al. 2005, MNRAS 358, 3
     Couchot et al. 2017, A&A 602, A41
 
+    Compute cross-spectra covariance block for <AB,CD>
+
     Example
     -------
     import xpol
-    bins = xpol.Bins( lmins, lmaxs)
-    xp = xpol.Xpol(mask, bins)
-    biased, unbiased = xp.get_spectra(map)
-    biased, unbiased = xp.get_spectra(map1, map2)
-
+    binning = xpol.Bins( lmins, lmaxs)
+    xp = xpol.Xcov(maskA, , maskB, bins=binning)
+    clcov = xc.get_clcov_blocks( clAC, clBD, clAD, clBC)
+    
     """
-    def __init__(self, mask, mask2=None, bins=None, polar=True, verbose=False):
+    def __init__(self, maskA, maskB=None, maskC=None, maskD=None, bins=None, polar=True, verbose=False, wlmax=None):
         """
         Inputs
         ------
-            mask: array, weighting mask to apply on data
-
+            maskA: array, weighting mask to apply on mapA
+        
         Options
         -------
+            maskB: array, weighting mask to apply on mapB
+            maskC: array, weighting mask to apply on mapC
+            maskD: array, weighting mask to apply on mapD
             bins: Class Bins, binning scheme
-            mask2: array, weighting mask to apply on the second map (for cross-correlation)
-            polar: boolean, polarisation computation
-            verbose: boolean
-
+            polar: boolean, polarisation computation [default=True]
+            verbose: boolean [default=False]
+        
         """
-        Xpol.__init__( self, mask, mask2=mask2, bins=bins, polar=polar, verbose=verbose)
+
+        if verbose:
+            log.setLevel(logging.DEBUG)
+        else:
+            log.setLevel(logging.INFO)
+
+        #compute Mll mixing kernels
+        if verbose: print( "Compute kernel AB")
+        Xpol.__init__( self, maskA, mask2=maskB, bins=bins, polar=polar, verbose=False, Dl=False)
+        self.invmll_AB = np.copy(self.mll_binned_inv)
+        if maskC is None:
+            self.invmll_CD = self.invmll_AB
+        else:
+            if verbose: print( "Compute kernel CD")
+            Xpol.__init__( self, maskC, mask2=maskD, bins=bins, polar=polar, verbose=False, Dl=False)
+            self.invmll_CD = np.copy(self.mll_binned_inv)
         
         self.dl = bins.dl
-
+        
         #compute coupling kernels for covariance
-        wlmax = 3*self.nside-1
-        if mask2 is None:
-            wl = hp.anafast(mask**2,lmax=wlmax)
-        else:
-            wl = hp.anafast(mask**2,map2=mask2**2,lmax=wlmax)
-        self.TT_TT, self.EE_EE, self.EE_BB, self.TE_TE = self._get_Mbb( wl)
+        if wlmax is None:
+            wlmax = bins.lmax
+
+        #only one mask
+        if maskB is None:
+            if self.verbose: print( "\tCompute covariance kernels ")
+            wl = hp.anafast(maskA*maskA,lmax=wlmax)
+            self.mll_ACBD = self.mll_ADBC = self._get_Mbb( wl)
+            return
+
+        #same masks fro cross-spectra for A=C and B=D
+        if maskC is None:
+            maskC = maskA
+            maskD = maskB
+        if maskD is None: maskD = maskC 
+        
+        if verbose: print( "\tCompute covariance kernel AC-BD")
+        wl = hp.anafast(maskA*maskC,map2=maskB*maskD,lmax=wlmax)
+        self.mll_ACBD = self._get_Mbb( wl)
+        if verbose: print( "\tCompute covariance kernel AD-BC")
+        wl = hp.anafast(maskA*maskD,map2=maskB*maskC,lmax=wlmax)
+        self.mll_ADBC = self._get_Mbb( wl)
 
 
     def _smooth_cl( self, cl, lcut=0, nsm=2):
         import scipy.ndimage as nd
 
         if nsm == 0:
             return(cl)
@@ -488,139 +563,167 @@
         scl[lcut:] = data[shift:]
         
         return scl
 
     def _get_pcl_cov(self, clAC, clBD, clAD, clBC):
         """
         Compute covariance matrix for pseudo-spectra <AB,CD>
-        tags=[TT,EE,BB,TE,ET]
         
         inputs:
             cl: 2d array (ntag,nbin)
+                [TT,EE,BB,TE,TB,EB,ET,BT,BE]
 
         output:
             out: 2d array (5*nbin,5*nbin)
+                 [TT,EE,BB,TE,ET]
         """
         n = len(self.lbin)
-        out = np.zeros((5*n, 5*n))
+        ndim = 5*n if self.polar else n
+        out = np.zeros((ndim, ndim))
         nu_l = (2.*self.lbin+1.) * self.dl
-
+        
         #symmetrization
-        tags = dict( zip( ["TT","EE","BB","TE","ET"], [0,1,2,3,4]))
+        tags = dict( zip( ["TT","EE","BB","TE","ET"], [0,1,2,3,6]))
         symcl = lambda cl,t: np.add.outer(cl[tags[t]],cl[tags[t]])/2.
-        
-        #TT_TT
-        out[0*n:1*n, 0*n:1*n] = symcl(clAC,"TT")*symcl(clBD,"TT")*self.TT_TT/nu_l + \
-                                symcl(clAD,"TT")*symcl(clBC,"TT")*self.TT_TT/nu_l
 
+        if self.polar:
+            s00_ACBD, sPP_ACBD, sMM_ACBD, s0P_ACBD = self.mll_ACBD
+            s00_ADBC, sPP_ADBC, sMM_ADBC, s0P_ADBC = self.mll_ADBC
+        else:
+            s00_ACBD = self.mll_ACBD
+            s00_ADBC = self.mll_ADBC
+
+        #TT_TT
+        out[0*n:1*n, 0*n:1*n] = symcl(clAC,"TT")*symcl(clBD,"TT")*s00_ACBD/nu_l + \
+                                symcl(clAD,"TT")*symcl(clBC,"TT")*s00_ADBC/nu_l
+        
+        if self.polar is False:
+            return out
+        
         #TT_EE
-        out[0*n:1*n, 1*n:2*n] = symcl(clAC,"TE")*symcl(clBD,"TE")*self.TT_TT/nu_l + \
-                                symcl(clAD,"TE")*symcl(clBC,"TE")*self.TT_TT/nu_l
+        out[0*n:1*n, 1*n:2*n] = symcl(clAC,"TE")*symcl(clBD,"TE")*s00_ACBD/nu_l + \
+                                symcl(clAD,"TE")*symcl(clBC,"TE")*s00_ADBC/nu_l
 
         #TT_BB
         out[0*n:1*n, 2*n:3*n] = 0.
 
         #TT_TE
-        out[0*n:1*n, 3*n:4*n]= symcl(clAC,"TT")*symcl(clBD,"TE")*self.TT_TT/nu_l + \
-                               symcl(clAD,"TE")*symcl(clBC,"TT")*self.TT_TT/nu_l
+        out[0*n:1*n, 3*n:4*n] = symcl(clAC,"TT")*symcl(clBD,"TE")*s00_ACBD/nu_l + \
+                                symcl(clAD,"TE")*symcl(clBC,"TT")*s00_ADBC/nu_l
 
         #TT_ET
-        out[0*n:1*n, 4*n:5*n] = symcl(clAC,"TE")*symcl(clBD,"TT")*self.TT_TT/nu_l + \
-                                symcl(clAD,"TT")*symcl(clBC,"TE")*self.TT_TT/nu_l
+        out[0*n:1*n, 4*n:5*n] = symcl(clAC,"TE")*symcl(clBD,"TT")*s00_ACBD/nu_l + \
+                                symcl(clAD,"TT")*symcl(clBC,"TE")*s00_ADBC/nu_l
 
         #EE_TT
-        out[1*n:2*n, 0*n:1*n] = symcl(clAC,"ET")*symcl(clBD,"ET")*self.TT_TT/nu_l + \
-                                symcl(clAD,"ET")*symcl(clBC,"ET")*self.TT_TT/nu_l
+        out[1*n:2*n, 0*n:1*n] = symcl(clAC,"ET")*symcl(clBD,"ET")*s00_ACBD/nu_l + \
+                                symcl(clAD,"ET")*symcl(clBC,"ET")*s00_ADBC/nu_l
 
         #EE_EE
-        out[1*n:2*n, 1*n:2*n] = symcl(clAC,"EE")*symcl(clBD,"EE")*self.EE_EE/nu_l + \
-                                symcl(clAD,"EE")*symcl(clBC,"EE")*self.EE_EE/nu_l
+        out[1*n:2*n, 1*n:2*n] = symcl(clAC,"EE")*symcl(clBD,"EE")*sPP_ACBD/nu_l + \
+                                symcl(clAD,"EE")*symcl(clBC,"EE")*sPP_ADBC/nu_l
 
         #EE_BB
         out[1*n:2*n, 2*n:3*n] = ( symcl(clAC,"EE")*symcl(clBD,"EE") + \
                                   symcl(clAC,"EE")*symcl(clBD,"BB") + \
                                   symcl(clAC,"BB")*symcl(clBD,"EE") + \
-                                  symcl(clAC,"BB")*symcl(clBD,"BB") )*self.EE_BB/nu_l + \
+                                  symcl(clAC,"BB")*symcl(clBD,"BB") )*sMM_ACBD/nu_l + \
                                 ( symcl(clAD,"EE")*symcl(clBC,"EE") + \
                                   symcl(clAD,"EE")*symcl(clBC,"BB") + \
                                   symcl(clAD,"BB")*symcl(clBC,"EE") + \
-                                  symcl(clAD,"BB")*symcl(clBC,"BB") )*self.EE_BB/nu_l
+                                  symcl(clAD,"BB")*symcl(clBC,"BB") )*sMM_ADBC/nu_l
 
         #EE_TE
-        out[1*n:2*n, 3*n:4*n] = symcl(clAC,"ET")*symcl(clBD,"EE")*self.TE_TE/nu_l + \
-                                symcl(clAD,"EE")*symcl(clBC,"ET")*self.TE_TE/nu_l
+        out[1*n:2*n, 3*n:4*n] = symcl(clAC,"ET")*symcl(clBD,"EE")*s0P_ACBD/nu_l + \
+                                symcl(clAD,"EE")*symcl(clBC,"ET")*s0P_ACBD/nu_l
 
         #EE_ET
-        out[1*n:2*n, 4*n:5*n] = symcl(clAC,"EE")*symcl(clBD,"ET")*self.TE_TE/nu_l + \
-                                symcl(clAD,"ET")*symcl(clBC,"EE")*self.TE_TE/nu_l
+        out[1*n:2*n, 4*n:5*n] = symcl(clAC,"EE")*symcl(clBD,"ET")*s0P_ACBD/nu_l + \
+                                symcl(clAD,"ET")*symcl(clBC,"EE")*s0P_ACBD/nu_l
         
         #BB_TT
         out[2*n:3*n, 0*n:1*n] = 0.
 
         #BB_EE
         out[2*n:3*n, 1*n:2*n] = ( symcl(clAC,"BB")*symcl(clBD,"BB") + \
                                   symcl(clAC,"BB")*symcl(clBD,"EE") + \
                                   symcl(clAC,"EE")*symcl(clBD,"BB") + \
-                                  symcl(clAC,"EE")*symcl(clBD,"EE") )*self.EE_BB/nu_l + \
+                                  symcl(clAC,"EE")*symcl(clBD,"EE") )*sMM_ACBD/nu_l + \
                                 ( symcl(clAD,"BB")*symcl(clBC,"BB") + \
                                   symcl(clAD,"BB")*symcl(clBC,"EE") + \
                                   symcl(clAD,"EE")*symcl(clBC,"BB") + \
-                                  symcl(clAD,"EE")*symcl(clBC,"EE") )*self.EE_BB/nu_l
+                                  symcl(clAD,"EE")*symcl(clBC,"EE") )*sMM_ADBC/nu_l
 
         #BB_BB
-        out[2*n:3*n, 2*n:3*n] = symcl(clAC,"BB")*symcl(clBD,"BB")*self.EE_EE/nu_l + \
-                                symcl(clAD,"BB")*symcl(clBC,"BB")*self.EE_EE/nu_l
+        out[2*n:3*n, 2*n:3*n] = symcl(clAC,"BB")*symcl(clBD,"BB")*sPP_ACBD/nu_l + \
+                                symcl(clAD,"BB")*symcl(clBC,"BB")*sPP_ADBC/nu_l
 
         #BB_TE
         out[2*n:3*n, 3*n:4*n] = 0.
 
         #BB_ET
         out[2*n:3*n, 4*n:5*n] = 0.
 
         #TE_TT
-        out[3*n:4*n, 0*n:1*n] = symcl(clAC,"TT")*symcl(clBD,"ET")*self.TT_TT/nu_l + \
-                                symcl(clAD,"TT")*symcl(clBC,"ET")*self.TT_TT/nu_l
+        out[3*n:4*n, 0*n:1*n] = symcl(clAC,"TT")*symcl(clBD,"ET")*s00_ACBD/nu_l + \
+                                symcl(clAD,"TT")*symcl(clBC,"ET")*s00_ADBC/nu_l
 
         #TE_EE
-        out[3*n:4*n, 1*n:2*n] = symcl(clAC,"TE")*symcl(clBD,"EE")*self.TE_TE/nu_l + \
-                                symcl(clAD,"TE")*symcl(clBC,"EE")*self.TE_TE/nu_l
+        out[3*n:4*n, 1*n:2*n] = symcl(clAC,"TE")*symcl(clBD,"EE")*s0P_ACBD/nu_l + \
+                                symcl(clAD,"TE")*symcl(clBC,"EE")*s0P_ADBC/nu_l
 
         #TE_BB
         out[3*n:4*n, 2*n:3*n] = 0.
 
         #TE_TE
-        out[3*n:4*n, 3*n:4*n] = symcl(clAC,"TT")*symcl(clBD,"EE")*self.TE_TE/nu_l + \
-                                symcl(clAD,"TE")*symcl(clBC,"ET")*self.TT_TT/nu_l
+        out[3*n:4*n, 3*n:4*n] = symcl(clAC,"TT")*symcl(clBD,"EE")*s0P_ACBD/nu_l + \
+                                symcl(clAD,"TE")*symcl(clBC,"ET")*s00_ADBC/nu_l
 
         #TE_ET
-        out[3*n:4*n, 4*n:5*n] = symcl(clAC,"TE")*symcl(clBD,"ET")*self.TT_TT/nu_l + \
-                                symcl(clAD,"TT")*symcl(clBC,"EE")*self.TE_TE/nu_l
+        out[3*n:4*n, 4*n:5*n] = symcl(clAC,"TE")*symcl(clBD,"ET")*s00_ACBD/nu_l + \
+                                symcl(clAD,"TT")*symcl(clBC,"EE")*s0P_ADBC/nu_l
 
         #ET_TT
-        out[4*n:5*n, 0*n:1*n] = symcl(clAC,"ET")*symcl(clBD,"TT")*self.TT_TT/nu_l + \
-                                symcl(clAD,"ET")*symcl(clBC,"TT")*self.TT_TT/nu_l
+        out[4*n:5*n, 0*n:1*n] = symcl(clAC,"ET")*symcl(clBD,"TT")*s00_ACBD/nu_l + \
+                                symcl(clAD,"ET")*symcl(clBC,"TT")*s00_ADBC/nu_l
 
         #ET_EE
-        out[4*n:5*n, 1*n:2*n] = symcl(clAC,"EE")*symcl(clBD,"TE")*self.TE_TE/nu_l + \
-                                symcl(clAD,"EE")*symcl(clBC,"TE")*self.TE_TE/nu_l
+        out[4*n:5*n, 1*n:2*n] = symcl(clAC,"EE")*symcl(clBD,"TE")*s0P_ACBD/nu_l + \
+                                symcl(clAD,"EE")*symcl(clBC,"TE")*s0P_ADBC/nu_l
 
         #ET_BB
         out[4*n:5*n, 2*n:3*n] = 0.
 
         #ET_TE
-        out[4*n:5*n, 3*n:4*n] = symcl(clAC,"ET")*symcl(clBD,"TE")*self.TT_TT/nu_l + \
-                                symcl(clAD,"EE")*symcl(clBC,"TT")*self.TE_TE/nu_l
+        out[4*n:5*n, 3*n:4*n] = symcl(clAC,"ET")*symcl(clBD,"TE")*s00_ACBD/nu_l + \
+                                symcl(clAD,"EE")*symcl(clBC,"TT")*s0P_ADBC/nu_l
 
         #ET_ET
-        out[4*n:5*n, 4*n:5*n] = symcl(clAC,"EE")*symcl(clBD,"TT")*self.TE_TE/nu_l + \
-                                symcl(clAD,"ET")*symcl(clBC,"TE")*self.TT_TT/nu_l
+        out[4*n:5*n, 4*n:5*n] = symcl(clAC,"EE")*symcl(clBD,"TT")*s0P_ACBD/nu_l + \
+                                symcl(clAD,"ET")*symcl(clBC,"TE")*s00_ADBC/nu_l
         
         return out
 
+    def _block_to_mll( self, mll_blocks):
+        if self.polar is False: return mll_blocks
+
+        TT_TT, EE_EE, EE_BB, TE_TE = mll_blocks
+        
+        n = len(self.lbin)
+        mll = np.zeros((5*n, 5*n))
+        mll[0*n:1*n, 0*n:1*n] = TT_TT
+        mll[1*n:2*n, 1*n:2*n] = EE_EE
+        mll[2*n:3*n, 2*n:3*n] = EE_EE
+        mll[1*n:2*n, 2*n:3*n] = EE_BB
+        mll[2*n:3*n, 1*n:2*n] = EE_BB
+        mll[3*n:4*n, 3*n:4*n] = TE_TE
+        mll[4*n:5*n, 4*n:5*n] = TE_TE
 
+        return mll
+    
     def get_clcov_blocks(self, clAC, clBD, clAD, clBC, nsm=2):
         """
         Compute analytical covariance matrix for cross spectra: <AB,CD>
         tags=[TT,EE,BB,TE,ET]
         
         inputs:
             cl: 2d array (ntag,nbin)
@@ -630,27 +733,19 @@
         """
 
         #use smooth data as signal model for covariance
         sclAC = self._smooth_cl( clAC, nsm=nsm)
         sclBD = self._smooth_cl( clBD, nsm=nsm)
         sclAD = self._smooth_cl( clAD, nsm=nsm)
         sclBC = self._smooth_cl( clBC, nsm=nsm)
-
-        n = len(self.lbin)
-        TT_TT, EE_EE, EE_BB, TE_TE = self.mll_binned_inv
-        invmll = np.zeros((5*n, 5*n))
-        invmll[  0:  n,   0:  n] = TT_TT
-        invmll[  n:2*n,   n:2*n] = EE_EE
-        invmll[2*n:3*n, 2*n:3*n] = EE_EE
-        invmll[  n:2*n, 2*n:3*n] = EE_BB
-        invmll[2*n:3*n,   n:2*n] = EE_BB
-        invmll[3*n:4*n, 3*n:4*n] = TE_TE
-        invmll[4*n:5*n, 4*n:5*n] = TE_TE
         
-        block =  invmll @ self._get_pcl_cov(sclAC, sclBD, sclAD, sclBC) @ invmll.T
+        invmllAB = self._block_to_mll( self.invmll_AB)
+        invmllCD = self._block_to_mll( self.invmll_CD)
+        block = invmllAB @ self._get_pcl_cov(sclAC, sclBD, sclAD, sclBC) @ invmllCD.T
+        
         return block
 
 
 
 class Xpol_Wrapper(object):
     """
     (Cross-) power spectra estimation using the Xpol method.
@@ -842,7 +937,64 @@
         self._clean( "cross_%d_0_0.fits" % self._runnb)
         self._clean( "cross_%d_0_1.fits" % self._runnb)
         self._clean( "cross_%d_1_0.fits" % self._runnb)
         self._clean( "cross_%d_1_1.fits" % self._runnb)
 
         return pcl, cl, err
 
+
+
+def fit_dipole(m, mask=None, bad=hp.UNSEEN):
+    """Fit a dipole and a monopole to the map, excluding bad pixels.
+
+    Parameters
+    ----------
+    m : float, array-like
+      the map to which a dipole is fitted and subtracted, accepts masked maps
+    m : float, array-like
+      the mask with weight to be applied
+    bad : float
+      bad values of pixel, default to :const:`UNSEEN`.
+
+    Returns
+    -------
+    res : tuple of length 2
+      the monopole value in res[0] and the dipole vector (as array) in res[1]
+    """
+    m = np.asarray(m)
+    npix = m.size
+    nside = hp.npix2nside(npix)
+    bunchsize = npix // 24 if nside > 128 else npix
+
+    if mask is None:
+        mask = np.ones( npix)        
+        
+    aa = np.zeros((4, 4), dtype=np.float64)
+    v = np.zeros(4, dtype=np.float64)
+    for ibunch in range(npix // bunchsize):
+        ipix = np.arange(ibunch * bunchsize, (ibunch + 1) * bunchsize)
+        ipix = ipix[(m.flat[ipix] != bad) & (np.isfinite(m.flat[ipix]))]
+        x, y, z = hp.pix2vec(nside, ipix)
+        aa[0, 0] += np.sum(mask[ipix])
+        aa[1, 0] += np.sum(x*mask[ipix])
+        aa[2, 0] += np.sum(y*mask[ipix])
+        aa[3, 0] += np.sum(z*mask[ipix])
+        aa[1, 1] += np.sum(mask.flat[ipix] * x * x)
+        aa[2, 1] += np.sum(mask.flat[ipix] * x * y)
+        aa[3, 1] += np.sum(mask.flat[ipix] * x * z)
+        aa[2, 2] += np.sum(mask.flat[ipix] * y * y)
+        aa[3, 2] += np.sum(mask.flat[ipix] * y * z)
+        aa[3, 3] += np.sum(mask.flat[ipix] * z * z)
+        v[0] += np.sum(mask.flat[ipix]*m.flat[ipix])
+        v[1] += np.sum(mask.flat[ipix]*m.flat[ipix] * x)
+        v[2] += np.sum(mask.flat[ipix]*m.flat[ipix] * y)
+        v[3] += np.sum(mask.flat[ipix]*m.flat[ipix] * z)
+    aa[0, 1] = aa[1, 0]
+    aa[0, 2] = aa[2, 0]
+    aa[0, 3] = aa[3, 0]
+    aa[1, 2] = aa[2, 1]
+    aa[1, 3] = aa[3, 1]
+    aa[2, 3] = aa[3, 2]
+    res = np.dot(np.linalg.inv(aa), v)
+    mono = res[0]
+    dipole = res[1:4]
+    return mono, dipole
```

### Comparing `xpol-1.6.1/src/xpol.h` & `xpol-1.7.0/src/xpol.h`

 * *Files identical despite different names*

### Comparing `xpol-1.6.1/src/xpol.f90` & `xpol-1.7.0/src/xpol.f90`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     integer, intent(out) :: ier
 
     real(real64), parameter  :: one_fourpi = 1.d0 / (atan(1.d0) * 16.d0)
     real(real64), dimension(2*lmax+1)  :: wigner0, wigner2
     real(real64), dimension(0:nwell-1) :: well_TT, well_TP, well_PP, thewell,  &
                                           ell
     real(real64) :: rl1, rl2, rl1min, rl1max, wig00, wig02, wig22, coef,       &
-                    sum_TT, sum_TE, sum_EE_EE, sum_EE_BB, sum_EB
+                    sum_TT, sum_TE, sum_EE_EE, sum_EE_BB
     integer  :: l, l1, l2, l1min, l1max, ndim, ier_, iwig
     logical  :: mask
 
     ell = [(l, l=0, nwell-1)]
     thewell = well * (2 * ell + 1)
     well_TT = thewell
     well_TP = thewell
@@ -132,15 +132,14 @@
           wig22 = wigner2(iwig) * wigner2(iwig)
           sum_TT = sum_TT + well_TT(l) * wig00
           if (mask) sum_TE = sum_TE + well_TP(l) * wig02
           if (mask) sum_EE_EE = sum_EE_EE + well_PP(l) * wig22
           if (.not. mask) sum_EE_BB = sum_EE_BB + well_PP(l) * wig22
           mask = .not. mask
         end do
-        sum_EB = sum_EE_EE + sum_EE_BB
 
         coef = (2 * l2 + 1) * one_fourpi
         mll_TT_TT(l1, l2) = coef * sum_TT
         mll_EE_EE(l1, l2) = coef * sum_EE_EE
         mll_EE_BB(l1, l2) = coef * sum_EE_BB
         mll_TE_TE(l1, l2) = coef * sum_TE
```

### Comparing `xpol-1.6.1/src/wig3j.f` & `xpol-1.7.0/src/wig3j.f`

 * *Files identical despite different names*

### Comparing `xpol-1.6.1/src/xpol_fits_param.h` & `xpol-1.7.0/src/xpol_fits_param.h`

 * *Files identical despite different names*

### Comparing `xpol-1.6.1/PKG-INFO` & `xpol-1.7.0/xpol.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.0
 Name: xpol
-Version: 1.6.1
+Version: 1.7.0
 Summary: XPOL cross power-spectrum estimator
 Home-page: UNKNOWN
 Author: Matthieu Tristram
-Author-email: tristram@lal.in2p3.fr
+Author-email: matthieu.tristram@cnrs.fr
 License: UNKNOWN
 Description: ====
         Xpol
         ====
         
         A code to compute angular power spectra based on cross-correlation between maps and covariance matrices.
         
@@ -20,15 +20,15 @@
         Install Python
         ==============
         
         The easiest way to install ``Xpol`` is via ``pip``
         
         .. code:: shell
         
-         pip install pspy [--user]
+         pip install xpol [--user]
         
         
         If you plan to develop the code, it is better to clone the repository
         
         .. code:: shell
         
          git clone https://gitlab.in2p3.fr/tristram/Xpol.git /where/to/clone
```

### Comparing `xpol-1.6.1/setup.py` & `xpol-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 lib = Extension('_flib',
                 sources=['src/xpol.f90'],
                 include_dirs=['.', get_include()],
                 libraries=['gomp',('fmod', {'sources': ['src/wig3j.f']})],
                 **compile_opts)
 
 setup(name=name,
-      version="1.6.1",
+      version="1.7.0",
       description='XPOL cross power-spectrum estimator',
       long_description=long_description,
       url='',
       author='Matthieu Tristram',
-      author_email='tristram@lal.in2p3.fr',
+      author_email='matthieu.tristram@cnrs.fr',
       install_requires=["astropy","healpy>=0.6.1"],
       packages=['xpol'],
       ext_modules=[lib]
 )
```

