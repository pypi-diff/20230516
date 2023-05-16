# Comparing `tmp/sfft-1.3.4.tar.gz` & `tmp/sfft-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfft-1.3.4.tar", last modified: Thu Sep 29 11:06:40 2022, max compression
+gzip compressed data, was "sfft-1.4.0.tar", last modified: Tue May 16 11:59:07 2023, max compression
```

## Comparing `sfft-1.3.4.tar` & `sfft-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.108515 sfft-1.3.4/
--rw-r--r--   0 thomas     (501) staff       (20)    20576 2022-09-29 11:06:40.107938 sfft-1.3.4/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)    18306 2022-09-28 20:01:24.000000 sfft-1.3.4/README.rst
--rw-r--r--   0 thomas     (501) staff       (20)       38 2022-09-29 11:06:40.108611 sfft-1.3.4/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)     1523 2022-09-28 20:01:24.000000 sfft-1.3.4/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.094613 sfft-1.3.4/sfft/
--rw-r--r--   0 thomas     (501) staff       (20)     7616 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/AutoCrowdedPrep.py
--rw-r--r--   0 thomas     (501) staff       (20)    22790 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/AutoSparsePrep.py
--rw-r--r--   0 thomas     (501) staff       (20)    10285 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/CustomizedPacket.py
--rw-r--r--   0 thomas     (501) staff       (20)    17366 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/EasyCrowdedPacket.py
--rw-r--r--   0 thomas     (501) staff       (20)    31984 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/EasySparsePacket.py
--rw-r--r--   0 thomas     (501) staff       (20)    31664 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/MultiEasyCrowdedPacket.py
--rw-r--r--   0 thomas     (501) staff       (20)    49927 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/MultiEasySparsePacket.py
--rw-r--r--   0 thomas     (501) staff       (20)      938 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.096538 sfft-1.3.4/sfft/sfftcore/
--rw-r--r--   0 thomas     (501) staff       (20)    96304 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/sfftcore/SFFTConfigure.py
--rw-r--r--   0 thomas     (501) staff       (20)    69206 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/sfftcore/SFFTSubtract.py
--rw-r--r--   0 thomas     (501) staff       (20)      197 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/sfftcore/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.104872 sfft-1.3.4/sfft/utils/
--rw-r--r--   0 thomas     (501) staff       (20)     5842 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/CombineHeader.py
--rw-r--r--   0 thomas     (501) staff       (20)     1762 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/ConvKernelConvertion.py
--rw-r--r--   0 thomas     (501) staff       (20)     4513 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/DeCorrelationCalculator.py
--rw-r--r--   0 thomas     (501) staff       (20)     5416 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/HoughDetection.py
--rw-r--r--   0 thomas     (501) staff       (20)    12154 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/HoughMorphClassifier.py
--rw-r--r--   0 thomas     (501) staff       (20)     2675 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/NeighboringPixelCovariance.py
--rw-r--r--   0 thomas     (501) staff       (20)     5018 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/SExSkySubtract.py
--rw-r--r--   0 thomas     (501) staff       (20)     5193 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/SFFTSolutionReader.py
--rw-r--r--   0 thomas     (501) staff       (20)    16888 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/SkyLevelEstimator.py
--rw-r--r--   0 thomas     (501) staff       (20)     8076 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/StampGenerator.py
--rw-r--r--   0 thomas     (501) staff       (20)     4150 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/SymmetricMatch.py
--rw-r--r--   0 thomas     (501) staff       (20)     3018 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/WeightedQuantile.py
--rw-r--r--   0 thomas     (501) staff       (20)      924 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.105907 sfft-1.3.4/sfft/utils/meta/
--rw-r--r--   0 thomas     (501) staff       (20)     4117 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/meta/FileLockKit.py
--rw-r--r--   0 thomas     (501) staff       (20)     1814 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/meta/MultiProc.py
--rw-r--r--   0 thomas     (501) staff       (20)     1921 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/meta/TimeoutKit.py
--rw-r--r--   0 thomas     (501) staff       (20)      171 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/meta/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.107450 sfft-1.3.4/sfft/utils/pyAstroMatic/
--rw-r--r--   0 thomas     (501) staff       (20)     2506 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/pyAstroMatic/AMConfigMaker.py
--rw-r--r--   0 thomas     (501) staff       (20)    49931 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/pyAstroMatic/PYSEx.py
--rw-r--r--   0 thomas     (501) staff       (20)     9468 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/pyAstroMatic/PYSWarp.py
--rw-r--r--   0 thomas     (501) staff       (20)      352 2022-09-28 20:01:24.000000 sfft-1.3.4/sfft/utils/pyAstroMatic/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2022-09-29 11:06:40.095695 sfft-1.3.4/sfft.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)    20576 2022-09-29 11:06:39.000000 sfft-1.3.4/sfft.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     1121 2022-09-29 11:06:39.000000 sfft-1.3.4/sfft.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2022-09-29 11:06:39.000000 sfft-1.3.4/sfft.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)      123 2022-09-29 11:06:39.000000 sfft-1.3.4/sfft.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        5 2022-09-29 11:06:39.000000 sfft-1.3.4/sfft.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.298135 sfft-1.4.0/
+-rw-rw-r--   0 thomas     (501) staff       (20)     1071 2023-05-16 11:52:46.000000 sfft-1.4.0/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)    19849 2023-05-16 11:59:07.297973 sfft-1.4.0/PKG-INFO
+-rw-rw-r--   0 thomas     (501) staff       (20)    19191 2023-05-16 11:52:46.000000 sfft-1.4.0/README.rst
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2023-05-16 11:59:07.298181 sfft-1.4.0/setup.cfg
+-rw-rw-r--   0 thomas     (501) staff       (20)     1532 2023-05-16 11:52:46.000000 sfft-1.4.0/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.293896 sfft-1.4.0/sfft/
+-rw-rw-r--   0 thomas     (501) staff       (20)     8022 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/AutoCrowdedPrep.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    24269 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/AutoSparsePrep.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    10967 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/CustomizedPacket.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    23156 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/EasyCrowdedPacket.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    37963 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/EasySparsePacket.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    44104 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/MultiEasyCrowdedPacket.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    62965 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/MultiEasySparsePacket.py
+-rw-rw-r--   0 thomas     (501) staff       (20)      938 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.295046 sfft-1.4.0/sfft/sfftcore/
+-rw-rw-r--   0 thomas     (501) staff       (20)    60906 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/sfftcore/SFFTConfigure.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    43853 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/sfftcore/SFFTSubtract.py
+-rw-rw-r--   0 thomas     (501) staff       (20)      177 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/sfftcore/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.296939 sfft-1.4.0/sfft/utils/
+-rw-rw-r--   0 thomas     (501) staff       (20)     1748 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/CombineHeader.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     1762 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/ConvKernelConvertion.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     5123 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/DeCorrelationCalculator.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    11117 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/HoughDetection.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    14478 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/HoughMorphClassifier.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     2681 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/NeighboringPixelCovariance.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     4862 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/ReadWCS.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     5445 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/SExSkySubtract.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     7992 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/SFFTSolutionReader.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    16888 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/SkyLevelEstimator.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    10072 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/StampGenerator.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     4150 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/SymmetricMatch.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     3018 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/WeightedQuantile.py
+-rw-rw-r--   0 thomas     (501) staff       (20)      979 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.297301 sfft-1.4.0/sfft/utils/meta/
+-rw-rw-r--   0 thomas     (501) staff       (20)     1847 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/meta/MultiProc.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     1921 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/meta/TimeoutKit.py
+-rw-rw-r--   0 thomas     (501) staff       (20)      137 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/meta/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.297799 sfft-1.4.0/sfft/utils/pyAstroMatic/
+-rw-rw-r--   0 thomas     (501) staff       (20)     2097 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/pyAstroMatic/AMConfigMaker.py
+-rw-rw-r--   0 thomas     (501) staff       (20)    51660 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/pyAstroMatic/PYSEx.py
+-rw-rw-r--   0 thomas     (501) staff       (20)     9670 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/pyAstroMatic/PYSWarp.py
+-rw-rw-r--   0 thomas     (501) staff       (20)      352 2023-05-16 11:52:46.000000 sfft-1.4.0/sfft/utils/pyAstroMatic/__init__.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 11:59:07.294600 sfft-1.4.0/sfft.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)    19849 2023-05-16 11:59:07.000000 sfft-1.4.0/sfft.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     1120 2023-05-16 11:59:07.000000 sfft-1.4.0/sfft.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-16 11:59:07.000000 sfft-1.4.0/sfft.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)      132 2023-05-16 11:59:07.000000 sfft-1.4.0/sfft.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        5 2023-05-16 11:59:07.000000 sfft-1.4.0/sfft.egg-info/top_level.txt
```

### Comparing `sfft-1.3.4/PKG-INFO` & `sfft-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,219 +1,232 @@
 Metadata-Version: 2.1
 Name: sfft
-Version: 1.3.4
+Version: 1.4.0
 Summary: Image Subtraction in Fourier Space
-Home-page: UNKNOWN
+Download-URL: https://github.com/thomasvrussell/sfft
 Author: Lei Hu
 Author-email: hulei@pmo.ac.cn
 Maintainer: Lei Hu
 Maintainer-email: hulei@pmo.ac.cn
 License: MIT Licence
-Download-URL: https://github.com/thomasvrussell/sfft
-Description: ..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_logo_gwbkg.png
-        
-        Package Description
-        -------------------
-        
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6576426.svg
-           :target: https://doi.org/10.5281/zenodo.6576426
-        .. image:: https://img.shields.io/pypi/v/sfft.svg
-            :target: https://pypi.python.org/pypi/sfft
-            :alt: Latest Version
-        .. image:: https://static.pepy.tech/personalized-badge/sfft?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads
-         :target: https://pepy.tech/project/sfft
-        .. image:: https://static.pepy.tech/personalized-badge/sfft?period=month&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads/month
-            :target: https://pepy.tech/project/sfft
-        .. image:: https://img.shields.io/badge/python-3.7-green.svg
-            :target: https://www.python.org/downloads/release/python-370/
-        .. image:: https://img.shields.io/badge/License-MIT-blue.svg
-            :target: https://opensource.org/licenses/MIT
-        |
-        Saccadic Fast Fourier Transform (SFFT) is an algorithm for image subtraction in Fourier space. SFFT brings about a remarkable improvement of computational performance of around an order of magnitude compared to other published image subtraction codes. 
-        
-        ..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_subtract_speed.png
-        
-        To get a clear picture of our method, we summarize a variety of features from different perspectives for SFFT and other existing image subtraction methods.
-        
-        ..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_features.png
-        
-        Installation
-        -----------
-        One can install the latest stable version of sfft from pip (recommended): ::
-            
-            pip install sfft
-        
-        Or alternatively, install any desired version of sfft from Github `<https://github.com/thomasvrussell/sfft>`_: ::
-        
-            python setup.py install
-        
-        sfft has the following three backends to perform the image subtraction.
-        
-        .. [#] **NumPy backend** : sfft will totally run on the CPU devices. NO GPU devices and CUDA dependencies are required for this backend.
-        .. [#] **PyCUDA backend** : The core functions of sfft are written in `PyCUDA <https://github.com/inducer/pycuda>`_ and `Scikit-Cuda <https://github.com/lebedov/scikit-cuda>`_. Users need to install PyCUDA and Scikit-Cuda according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
-        .. [#] **CuPy backend** : The core functions of sfft are written in `CuPy <https://github.com/cupy/cupy>`_. Users need to install CuPy according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
-        
-        - CUDA 11: E.g, you may enable the CuPy backend for CUDA 11.5 via: ::
-        
-            pip install cupy-cuda115  # CuPy backend
-        
-        - CUDA 10: E.g, you may enable the GPU backends (i.e., PyCUDA backend and CuPy backend) for CUDA 10.1 via: ::
-        
-            pip install pycuda==2020.1 scikit-cuda==0.5.3  # PyCUDA backend
-            pip install cupy-cuda101                       # CuPy backend
-                           
-        **Additional Remarks**: CuPy backend is faster than PyCUDA backend, while it consumes more GPU memory. Generally, I strongly recommend users to adopt CuPy backend as long as it does not incur GPU out-of-memory issue. Note that PyCUDA backend is still not compatiable with CUDA 11.
-        
-        Dependencies
-        -----------
-        
-        You need further to install additional astronomical software for sfft.
-        
-        - `SExtractor <https://github.com/astromatic/sextractor>`_: SExtractor is required for sfft preprocessing, as it enables sfft to determine a proper pixel mask over the input image-pair before the image subtraction (this is critical for a more reasonable parameter-solving). Note that we have wrapped SExtractor into a Python module ``sfft.utils.pyAstroMatic.PYSEx`` so that one can trigger SExtractor within Python (please type help(``sfft.utils.pyAstroMatic.PYSEx``) to find its usage). As an AstrOmatic software, you can install SExtractor following `<https://www.astromatic.net/software/sextractor/>`_, or alternatively, install via conda: ::
-        
-            conda install -c conda-forge astromatic-source-extractor
-        
-        - `SWarp <https://github.com/astromatic/swarp>`_ (optional): This is not required for sfft subtraction itself. However, it is normally necessary to align the input image-pair before image subtraction. We have additionally wrapped SWarp into a Python module ``sfft.utils.pyAstroMatic.PYSWarp`` so that you can align images in a more Pythonic way (please type help(``sfft.utils.pyAstroMatic.PYSWarp``) to find its usage). As an AstrOmatic software, you can install SWarp following `<https://www.astromatic.net/software/swarp/>`_, or alternatively, install via conda: ::
-        
-            conda install -c conda-forge astromatic-swarp
-        
-        Quick start guide
-        -----------
-        We have prepared several examples in the test directory so that you can familar with the usage of the main functions in our software:
-        
-        .. [*] **sfft subtraction for crowded field** : The example in subdirectory named subtract_test_crowded_flavor. We use crowded-flavor-sfft (module ``sfft.EasyCrowdedPacket``) to perform image subtraction for ZTF M31 observations. More detailed explanations of this module, see help(``sfft.EasyCrowdedPacket``).
-        
-        .. [*] **sfft subtraction for sparse field** : The example in subdirectory named subtract_test_sparse_flavor. We use sparse-flavor-sfft (module ``sfft.EasySparsePacket``) to perform image subtraction for CTIO-4m DECam observations. More detailed explanations of this module, see help(``sfft.EasySparsePacket``).
-        
-        - **IMPORTANT NOTICE: the input images of sparse-flavor-sfft should be SKY-SUBTRACTED!** One can make use of SExtractor to subtract the sky background, which has been also wrapped in this package, please use the module ``sfft.utils.SExSkySubtract`` and type help(``sfft.utils.SExSkySubtract``) to find its usage. There is an additional example in subtract_test_sparse_flavor (see directory prepare_data_example), that shows how to prepare the input image pair for sparse-flavor-sfft by ``sfft.utils.SExSkySubtract`` for sky subtraction and ``sfft.utils.pyAstroMatic.PYSWarp`` for image alignment, respecitvely.
-        
-        - Our software provides two flavors for image subtraction, crowded-flavor-sfft and sparse-flavor-sfft, to accommodate the situations for the crowded and sparse fields, respectively. The two flavors actually follow the same routine for image subtraction and differ only in ways of masking the data. 
-        
-        - Proper image-masking is required in the current version of SFFT to identify the pixels that are not correctly modeled by SFFT (hereafter, distraction pixels), e.g., saturated sources, casual cosmic rays and moving objects, bad CCD pixels, optical ghosts, and even the variable objects and transients themselves. The pre-subtraction processing for image-masking is referred to as **preprocessing** in sfft.
-        
-        - Our software provides a generic and robust function to perform **preprocessing** of the data, which has been extensively tested with data from various transient surveys. When you run crowded-flavor-sfft and sparse-flavor-sfft, sfft actually performs the generic **preprocessing** for image-masking and do the sfft subtraction subsequently. 
-        
-        - More specificially, the built-in preprocessing in sfft consists of two steps: [1] identify the distraction pixels in the input image-pair [2] create the masked version of the input image-pair via replacing the identified distraction pixels by proper flux values. In sparse-flavor-sfft, we designed a source-selection based on SExtractor catalogs and identify the unselected regions as distraction pixels. Given that the input images are required to be sky-subtracted in sparse-flavor-sfft, we simply replace the distraction pixels by zeros; In crowded-flavor-sfft, we only identify the pixels contaminated by saturated sources as distraction pixels using SExtractor, and then replace the distraction pixels by local background flux. 
-        
-        Customized usage
-        -----------
-        
-        The built-in **preprocessing** in sfft (based on SExtractor) is only designed to provide a safe and generic approach which can adapt to diverse imaging data. In contrast to the high speed of the image subtraction, the computing performance of the built-in **preprocessing** is much less remarkable (says, 10 times more computing time). Given a particular time-domain program, we do believe there is plenty of room for further optimization of the computing expense on the **preprocessing**. The two suggestions below might be helpful for users who would like to incorporate sfft in their pipeline efficiently:
-        
-        - For sparse-flavor-sfft, the built-in **preprocessing** performs a source-selection based on SExtractor catalogs and then create the masked images for subsequent subtraction. To optimize the overall computing expense of the pipeline, one can make use of the SExtractor products already generated in the preceding modules (e.g., astrometric calibration) for the source-selection (which is much faster than SExtractor) of sfft. It will avoid repeated SExtractor photometry and reduce computing time significantly.
-        
-        - For crowded-flavor-sfft, the built-in **preprocessing** only mask the saturation-contaminated pixels using SExtractor. When data quality masks for the observed imaging data are available in a survey program, one can instead identify the invalid pixels using the data quality masks and mask them by local background. Hence, the built-in **preprocessing** can be totally skipped.
-        
-        Besides, we encourage users to design dedicated image-masking strategies for their survey programs to unleash the great power of sfft subtraction!
-        
-        Our software provides a customized module which allows users to feed their own image-masking results, i.e., the module only perform the sfft subtraction. In this test, you would see the lightning fast speed of sfft subtraction on GPU devices!
-        
-        .. [*] **customized sfft subtraction** : The example in subdirectory named subtract_test_customized. The test data is the same as those for crowded-flavor-sfft (ZTF-M31 observations), however, the built-in automatic image-masking has been skipped by using given customized masked images as inputs. Such *pure* version of sfft is conducted by the module ``sfft.CustomizedPacket``. More detailed explanations of the module: help(``sfft.CustomizedPacket``).
-        
-        **Additional Remarks**: If you are using GPU backends and you have a queue of observations to be processed, the first time in the loop of sfft subtraction can be very slow, and runtime is going to be stable after the first time. This might be due to some unknown initialization process in GPU devices. You can find in above test that the GPU warming-up is quite slow. Fortunately, this problem can be esaily solved by running a trivial subtraction (e.g., on empty images) in advance and making the pipe waiting for the subsequent observations (see above test).
-        
-        Parallel Computing
-        -----------
-        
-        We have also developed modules to optimize the overall computing performance of sparse-flavor-sfft and crowded-flavor-sfft for the cases when you need to deal with multiple tasks simultaneously.
-        
-        - In a particular time-domain survey, one may need to process a large set of image-pairs simultaneously. Assume that you have Nt tasks which should be processed by a computing platform with Nc CPU threads and Ng GPU devices. Generally, Nt >> Ng and Nc >> Ng. 
-        
-            E.g., Nt = 61 (A DECam exposure with CCDs), Nc = 40 (A CPU with 40 threads), and Ng = 1 (A Tesla A100 available).
-        
-        - Note that we generally need to avoid multiple tasks using one GPU at the same time (GPU out-of-memory issue). That is to say, we CANNOT simply trigger a set of sfft functions (e.g., ``sfft.EasySparsePacket``) to process a large set of image-pairs simultaneously.
-        
-        - Since version 1.1, sfft has allowed for multiple tasks without conflicting GPU usage, by using the modules ``sfft.MultiEasySparsePacket`` for sparse-flavor-sfft and ``sfft.MultiEasyCrowdedPacket`` for crowded-flavor-sfft, respectively. Please see the directory test/subtract_test_multiprocessing to find the examples. Note that ONLY the CuPy backend is supported in multiprocessing mode.
-        
-        Remarks on the direction of image subtraction
-        -----------
-        
-        There is a universal argument named -ForceConv to control the direction of image subtraction, which works on all image subtraction modules in sfft.
-        
-        - 'AUTO' means sfft will determine the direction of image subtraction automatically according to the estimated FWHM of reference image and science image. The image which has smaller FWHM will be convolved in the image subtraction to avoid deconvolution. After comparing the FWHM, 'AUTO' becomes 'REF' or 'SCI' (see below). One can get to know which image is eventually convolved in image subtraction from the primary header of the difference image (see the keyword 'CONVD'). This mode does not supported in the Customized module ``sfft.CustomizedPacket``.
-        
-        - 'REF' means sfft will convolve the reference image and DIFF = SCI - Convolved_REF. As a result, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the science image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the science image: using the same psf model / aperture and magnitude zeropoint.
-        
-        - 'SCI' means sfft will convolve the reference image and DIFF = Convolved_SCI - REF. Consequently, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the reference image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the reference image: using the same psf model / aperture and magnitude zeropoint (but of course, not including the observation date!).
-        
-        Note that a transient on science image is always a positive signal on difference image whatever -ForceConv is.
-        
-        Additional Function
-        -----------
-        
-        We also present a decorrelation module to whiten the background noise of the difference image.
-        
-        .. [*] **difference noise decorrelation** : The example in subdirectory named difference_noise_decorrelation. We use noise-decorrelation toolkit (module ``sfft.utils.DeCorrelationCalculator``) to whiten the background noise on difference image. In this test, the difference image is generated from image subtraction (by sfft) between a coadded reference image and a coadded science image, each stacked from 5 DECam individual observations with PSF homogenization (by sfft). The toolkit can be also applied to whiten a coadded image as long as convolution is involved in the stacking process.
-        
-        
-        Comments on Backward Compatiablity
-        -----------
-        
-        We have tried our best to ensure the backward compatiablity, however, the rule was sometimes overrided in the development of sfft, e.g., some arguments might be deprecated in higher version of sfft. Users might get errors when they use old scripts but update sfft to a higher version. To solve the problem, I have been maintaining the test scripts on Github to make sure they can always work for the lastest version of sfft. You can also find the change log of arguments in the test scripts. 
-        
-        What's new
-        -----------
-        
-        - The preprocessing in sparse-flavor-sfft is refined using an additional rejection of mild varaibles since version 1.3.0. [Lei, Aug 19, 2022]
-        
-        - The sfft is now optimized for multiple tasks since version 1.1.0. [Lei, May 24, 2022]
-        
-        - A few argument-names have been changed since version 1.1.0, please see the test scripts. [Lei, May 24, 2022]
-        
-        - Locking file is removed since version 1.1.0, as I found it unreliable in our tests, i.e., -GLockFile is removed. [Lei, May 24, 2022]
-        
-        - The trial subtraction for refinement is removed since version 1.1.0. However, I add a post-subtraction check to search anomalies on the difference image using the same logic. One can feed the coordinates of the anomalies to sfft again as Prior-Banned sources to refine the subtraction (see -XY_PriorBan in ``sfft.MultiEasySparsePacket``). [Lei, May 24, 2022]
-        
-        Todo list
-        -----------
-        
-        - Incorporate the separate functions (in the folder beta4spline) for spline form sfft into the unified sfft functions. Note that only Numpy backend is currently available and the spline form is very memory-consuming. [Lei, July 6, 2022]
-        
-        - Write a detailed documentation for sfft! [Lei, May 24, 2022]
-        
-        - We notice that SExtractor may have been called to perform astrometric calibration before image subtraction. It is definitely not wise to run SExtractor again in sfft, I need to develop a module which allows users to feed SExtractor products as inputs of sfft, which will significantly reduce the preprocessing time in sfft. [Lei, May 24, 2022]
-        
-        - The multiprocessing mode is expected to accomondate multiple GPU devices, however, the function has not tested on such a multi-GPUs platform. [Lei, May 24, 2022]
-        
-        - Add a function for optimizing sfft on a given computing platform with multiple CPU threading and one/multiple GPU card(s). This would be very useful to reduce the overall time cost when users have a large set of image-pairs to be processed simultaneously (e.g., serve for DECam, each exposure produces 61 CCD images). [Lei, May 20, 2022] **[ALREADY DONE]**
-        
-        Common issues
-        -----------
-        
-        - If your Python environment already has some version of llvmlite (a package required by NumPy backend) before installing sfft. The setup.py in sfft cannot properly update llvmlite to the desired version, then you may get errors related to Numba or llvmlite. If so, please manually install llvmlite by: ::
-        
-            pip install llvmlite==0.36.0 --ignore-installed
-        
-        Development
-        -----------
-        The latest source code can be obtained from
-        `<https://github.com/thomasvrussell/sfft>`_.
-        
-        When submitting bug reports or questions via the `issue tracker 
-        <https://github.com/thomasvrussell/sfft/issues>`_, please include the following 
-        information:
-        
-        - OS platform.
-        - Python version.
-        - CUDA, PyCUDA and CuPy version.
-        - Version of sfft.
-        
-        Citing
-        ------
-        
-        *Image Subtraction in Fourier Space. Hu, L., Wang, L., Chen, X., & Yang, J. 2022, The Astrophysical Journal, 936, 157*
-        
-        Arxiv link: `<https://arxiv.org/abs/2109.09334>`_.
-        
-        ApJ Publication link: `<https://doi.org/10.3847/1538-4357/ac7394>`_.
-        
-        Related DOI: 10.3847/1538-4357/ac7394
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_logo_gwbkg.png
+
+Package Description
+-------------------
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6576426.svg
+   :target: https://doi.org/10.5281/zenodo.6576426
+.. image:: https://img.shields.io/pypi/v/sfft.svg
+    :target: https://pypi.python.org/pypi/sfft
+    :alt: Latest Version
+.. image:: https://static.pepy.tech/personalized-badge/sfft?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads
+ :target: https://pepy.tech/project/sfft
+.. image:: https://static.pepy.tech/personalized-badge/sfft?period=month&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads/month
+    :target: https://pepy.tech/project/sfft
+.. image:: https://img.shields.io/badge/python-3.7-green.svg
+    :target: https://www.python.org/downloads/release/python-370/
+.. image:: https://img.shields.io/badge/License-MIT-blue.svg
+    :target: https://opensource.org/licenses/MIT
+|
+Saccadic Fast Fourier Transform (SFFT) is an algorithm for image subtraction in Fourier space. SFFT brings about a remarkable improvement of computational performance of around an order of magnitude compared to other published image subtraction codes. 
+
+..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_subtract_speed.png
+
+To get a clear picture of our method, we summarize a variety of features from different perspectives for SFFT and other existing image subtraction methods.
+
+..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_features.png
+
+Installation
+-----------
+One can install the latest stable version of sfft from pip (recommended): ::
+    
+    pip install sfft
+
+Or alternatively, install any desired version of sfft from Github `<https://github.com/thomasvrussell/sfft>`_: ::
+
+    python setup.py install
+
+sfft now has the following two backends to perform the image subtraction.
+
+.. [#] **CuPy backend** : The core functions of sfft are written in `CuPy <https://github.com/cupy/cupy>`_. Users need to install CuPy according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
+.. [#] **NumPy backend** : sfft will totally run on the CPU devices. NO GPU devices and CUDA dependencies are required for this backend.
+
+- CUDA 12: E.g, you may enable the CuPy backend for CUDA 12.0 via: ::
+
+    pip install cupy-cuda12x
+
+- CUDA 11: E.g, you may enable the CuPy backend for CUDA 11.5 via: ::
+
+    pip install cupy-cuda115
+
+- CUDA 10: E.g, you may enable the CuPy backend for CUDA 10.1 via: ::
+
+    pip install cupy-cuda101
+
+**Additional Remarks**: There was a PyCUDA backend in sfft but now deprecated since v1.4.0. For sfft < v1.4.0, PyCUDA backend was preserved as it consumes less GPU memory. However, the CuPy backend is now better implemented for GPU memory allocation, making the PyCUDA backend no longer useful.
+
+Dependencies
+-----------
+
+You need further to install additional astronomical software for sfft.
+
+- `SExtractor <https://github.com/astromatic/sextractor>`_: SExtractor is required for sfft preprocessing, as it enables sfft to determine a proper pixel mask over the input image-pair before the image subtraction (this is critical for a more reasonable parameter-solving). Note that we have wrapped SExtractor into a Python module ``sfft.utils.pyAstroMatic.PYSEx`` so that one can trigger SExtractor within Python (please type help(``sfft.utils.pyAstroMatic.PYSEx``) to find its usage). As an AstrOmatic software, you can install SExtractor following `<https://www.astromatic.net/software/sextractor/>`_, or alternatively, install via conda: ::
+
+    conda install -c conda-forge astromatic-source-extractor
+
+- `SWarp <https://github.com/astromatic/swarp>`_ (optional): This is not required for sfft subtraction itself. However, it is normally necessary to align the input image-pair before image subtraction. We have additionally wrapped SWarp into a Python module ``sfft.utils.pyAstroMatic.PYSWarp`` so that you can align images in a more Pythonic way (please type help(``sfft.utils.pyAstroMatic.PYSWarp``) to find its usage). As an AstrOmatic software, you can install SWarp following `<https://www.astromatic.net/software/swarp/>`_, or alternatively, install via conda: ::
+
+    conda install -c conda-forge astromatic-swarp
+
+Quick start guide
+-----------
+We have prepared several examples in the test directory so that you can familar with the usage of the main functions in our software:
+
+.. [*] **sfft subtraction for crowded field** : The example in subdirectory named subtract_test_crowded_flavor. We use crowded-flavor-sfft (module ``sfft.EasyCrowdedPacket``) to perform image subtraction for ZTF M31 observations. More detailed explanations of this module, see help(``sfft.EasyCrowdedPacket``).
+
+.. [*] **sfft subtraction for sparse field** : The example in subdirectory named subtract_test_sparse_flavor. We use sparse-flavor-sfft (module ``sfft.EasySparsePacket``) to perform image subtraction for CTIO-4m DECam observations. More detailed explanations of this module, see help(``sfft.EasySparsePacket``).
+
+- **IMPORTANT NOTICE: the input images of sparse-flavor-sfft should be SKY-SUBTRACTED!** One can make use of SExtractor to subtract the sky background, which has been also wrapped in this package, please use the module ``sfft.utils.SExSkySubtract`` and type help(``sfft.utils.SExSkySubtract``) to find its usage. There is an additional example in subtract_test_sparse_flavor (see directory prepare_data_example), that shows how to prepare the input image pair for sparse-flavor-sfft by ``sfft.utils.SExSkySubtract`` for sky subtraction and ``sfft.utils.pyAstroMatic.PYSWarp`` for image alignment, respecitvely.
+
+- Our software provides two flavors for image subtraction, crowded-flavor-sfft and sparse-flavor-sfft, to accommodate the situations for the crowded and sparse fields, respectively. The two flavors actually follow the same routine for image subtraction and differ only in ways of masking the data. 
+
+- Proper image-masking is required in the current version of SFFT to identify the pixels that are not correctly modeled by SFFT (hereafter, distraction pixels), e.g., saturated sources, casual cosmic rays and moving objects, bad CCD pixels, optical ghosts, and even the variable objects and transients themselves. The pre-subtraction processing for image-masking is referred to as **preprocessing** in sfft.
+
+- Our software provides a generic and robust function to perform **preprocessing** of the data, which has been extensively tested with data from various transient surveys. When you run crowded-flavor-sfft and sparse-flavor-sfft, sfft actually performs the generic **preprocessing** for image-masking and do the sfft subtraction subsequently. 
+
+- More specificially, the built-in preprocessing in sfft consists of two steps: [1] identify the distraction pixels in the input image-pair [2] create the masked version of the input image-pair via replacing the identified distraction pixels by proper flux values. In sparse-flavor-sfft, we designed a source-selection based on SExtractor catalogs and identify the unselected regions as distraction pixels. Given that the input images are required to be sky-subtracted in sparse-flavor-sfft, we simply replace the distraction pixels by zeros; In crowded-flavor-sfft, we only identify the pixels contaminated by saturated sources as distraction pixels using SExtractor, and then replace the distraction pixels by local background flux. 
+
+Customized usage
+-----------
+
+The built-in **preprocessing** in sfft (based on SExtractor) is only designed to provide a safe and generic approach which can adapt to diverse imaging data. In contrast to the high speed of the image subtraction, the computing performance of the built-in **preprocessing** is much less remarkable (says, 10 times more computing time). Given a particular time-domain program, we do believe there is plenty of room for further optimization of the computing expense on the **preprocessing**. The two suggestions below might be helpful for users who would like to incorporate sfft in their pipeline efficiently:
+
+- For sparse-flavor-sfft, the built-in **preprocessing** performs a source-selection based on SExtractor catalogs and then create the masked images for subsequent subtraction. To optimize the overall computing expense of the pipeline, one can make use of the SExtractor products already generated in the preceding modules (e.g., astrometric calibration) for the source-selection (which is much faster than SExtractor) of sfft. It will avoid repeated SExtractor photometry and reduce computing time significantly.
+
+- For crowded-flavor-sfft, the built-in **preprocessing** only mask the saturation-contaminated pixels using SExtractor. When data quality masks for the observed imaging data are available in a survey program, one can instead identify the invalid pixels using the data quality masks and mask them by local background. Hence, the built-in **preprocessing** can be totally skipped.
+
+Besides, we encourage users to design dedicated image-masking strategies for their survey programs to unleash the great power of sfft subtraction!
+
+Our software provides a customized module which allows users to feed their own image-masking results, i.e., the module only perform the sfft subtraction. In this test, you would see the lightning fast speed of sfft subtraction on GPU devices!
+
+.. [*] **customized sfft subtraction** : The example in subdirectory named subtract_test_customized. The test data is the same as those for crowded-flavor-sfft (ZTF-M31 observations), however, the built-in automatic image-masking has been skipped by using given customized masked images as inputs. Such *pure* version of sfft is conducted by the module ``sfft.CustomizedPacket``. More detailed explanations of the module: help(``sfft.CustomizedPacket``).
+
+**Additional Remarks**: If you are using GPU backends and you have a queue of observations to be processed, the first time in the loop of sfft subtraction can be very slow, and runtime is going to be stable after the first time. This might be due to some unknown initialization process in GPU devices. You can find in above test that the GPU warming-up is quite slow. Fortunately, this problem can be esaily solved by running a trivial subtraction (e.g., on empty images) in advance and making the pipe waiting for the subsequent observations (see above test).
+
+Parallel Computing
+-----------
+
+We have also developed modules to optimize the overall computing performance of sparse-flavor-sfft and crowded-flavor-sfft for the cases when you need to deal with multiple tasks simultaneously.
+
+- In a particular time-domain survey, one may need to process a large set of image-pairs simultaneously. Assume that you have Nt tasks which should be processed by a computing platform with Nc CPU threads and Ng GPU devices. Generally, Nt >> Ng and Nc >> Ng. 
+
+    E.g., Nt = 61 (A DECam exposure with CCDs), Nc = 40 (A CPU with 40 threads), and Ng = 1 (A Tesla A100 available).
+
+- Note that we generally need to avoid multiple tasks using one GPU at the same time (GPU out-of-memory issue). That is to say, we CANNOT simply trigger a set of sfft functions (e.g., ``sfft.EasySparsePacket``) to process a large set of image-pairs simultaneously.
+
+- Since version 1.1, sfft has allowed for multiple tasks without conflicting GPU usage, by using the modules ``sfft.MultiEasySparsePacket`` for sparse-flavor-sfft and ``sfft.MultiEasyCrowdedPacket`` for crowded-flavor-sfft, respectively. Please see the directory test/subtract_test_multiprocessing to find the examples. Note that ONLY the CuPy backend is supported in multiprocessing mode.
+
+Remarks on the direction of image subtraction
+-----------
+
+There is a universal argument named -ForceConv to control the direction of image subtraction, which works on all image subtraction modules in sfft.
+
+- 'AUTO' means sfft will determine the direction of image subtraction automatically according to the estimated FWHM of reference image and science image. The image which has smaller FWHM will be convolved in the image subtraction to avoid deconvolution. After comparing the FWHM, 'AUTO' becomes 'REF' or 'SCI' (see below). One can get to know which image is eventually convolved in image subtraction from the primary header of the difference image (see the keyword 'CONVD'). This mode does not supported in the Customized module ``sfft.CustomizedPacket``.
+
+- 'REF' means sfft will convolve the reference image and DIFF = SCI - Convolved_REF. As a result, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the science image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the science image: using the same psf model / aperture and magnitude zeropoint.
+
+- 'SCI' means sfft will convolve the reference image and DIFF = Convolved_SCI - REF. Consequently, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the reference image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the reference image: using the same psf model / aperture and magnitude zeropoint (but of course, not including the observation date!).
+
+Note that a transient on science image is always a positive signal on difference image whatever -ForceConv is.
+
+Additional Function
+-----------
+
+We also present a decorrelation module to whiten the background noise of the difference image.
+
+.. [*] **difference noise decorrelation** : The example in subdirectory named difference_noise_decorrelation. We use noise-decorrelation toolkit (module ``sfft.utils.DeCorrelationCalculator``) to whiten the background noise on difference image. In this test, the difference image is generated from image subtraction (by sfft) between a coadded reference image and a coadded science image, each stacked from 5 DECam individual observations with PSF homogenization (by sfft). The toolkit can be also applied to whiten a coadded image as long as convolution is involved in the stacking process.
+
+
+Comments on Backward Compatiablity
+-----------
+
+We have tried our best to ensure the backward compatiablity, however, the rule was sometimes overrided in the development of sfft, e.g., some arguments might be deprecated in higher version of sfft. Users might get errors when they use old scripts but update sfft to a higher version. To solve the problem, I have been maintaining the test scripts on Github to make sure they can always work for the lastest version of sfft. You can also find the change log of arguments in the test scripts. 
+
+What's new
+-----------
+
+- A warning for users: As scikit-image has changed something in its function of hough detection since version 0.19.0, I recently found that the source selection in sfft will be affected by this upgrade. I have not checked the new function yet, for the time being I would recommend users to install a scikit-image >= 0.16.2 but <= 0.18.3. Possibly I may add a constrain on scikit-image version in sfft 1.3.5. [Lei, Nov 9, 2022]
+
+- A warning message about the usage of ``sfft.MultiEasySparsePacket`` and ``sfft.MultiEasyCrowdedPacket`` is added in the related test scripts. [Lei, Oct 25, 2022]
+
+- The preprocessing in sparse-flavor-sfft is refined using an additional rejection of mild varaibles since version 1.3.0. [Lei, Aug 19, 2022]
+
+- The sfft is now optimized for multiple tasks since version 1.1.0. [Lei, May 24, 2022]
+
+- A few argument-names have been changed since version 1.1.0, please see the test scripts. [Lei, May 24, 2022]
+
+- Locking file is removed since version 1.1.0, as I found it unreliable in our tests, i.e., -GLockFile is removed. [Lei, May 24, 2022]
+
+- The trial subtraction for refinement is removed since version 1.1.0. However, I add a post-subtraction check to search anomalies on the difference image using the same logic. One can feed the coordinates of the anomalies to sfft again as Prior-Banned sources to refine the subtraction (see -XY_PriorBan in ``sfft.MultiEasySparsePacket``). [Lei, May 24, 2022]
+
+Todo list
+-----------
+
+- The total GPU memory usage is only optimized for KerPolyOrder = 2 & BGPolyOrder = 2, I will extend the optimization to other cases ASAP! In fact, I believe there is ample space for reducing the total GPU usage and I will explore it. [Lei, Nov 11, 2022] **[ALREADY DONE]**
+
+- I will allows users to disable the hough detection for preprocessing when there are too few sources in the field in the next version sfft v1.3.5. [Lei, Nov 11, 2022]
+
+- Add a verbose argument for sfft so that users can get more clean printed messages. [Lei, Nov 9, 2022] **[ALREADY DONE]**
+
+- Test if we can use sep to replace SExtractor in preprocessing to make sfft more Pythonic. [Lei, Nov 9, 2022] 
+
+- Incorporate the separate functions (in the folder beta4spline) for spline form sfft into the unified sfft functions. Note that only Numpy backend is currently available and the spline form is very memory-consuming. [Lei, July 6, 2022]
+
+- Write a detailed documentation for sfft! [Lei, May 24, 2022]
+
+- We notice that SExtractor may have been called to perform astrometric calibration before image subtraction. It is definitely not wise to run SExtractor again in sfft, I need to develop a module which allows users to feed SExtractor products as inputs of sfft, which will significantly reduce the preprocessing time in sfft. [Lei, May 24, 2022]
+
+- The multiprocessing mode is expected to accomondate multiple GPU devices, however, the function has not tested on such a multi-GPUs platform. [Lei, May 24, 2022] **[ALREADY DONE]**
+
+- Add a function for optimizing sfft on a given computing platform with multiple CPU threading and one/multiple GPU card(s). This would be very useful to reduce the overall time cost when users have a large set of image-pairs to be processed simultaneously (e.g., serve for DECam, each exposure produces 61 CCD images). [Lei, May 20, 2022] **[ALREADY DONE]**
+
+Common issues
+-----------
+
+- If your Python environment already has some version of llvmlite (a package required by NumPy backend) before installing sfft. The setup.py in sfft cannot properly update llvmlite to the desired version, then you may get errors related to Numba or llvmlite. If so, please manually install llvmlite by: ::
+
+    pip install llvmlite==0.36.0 --ignore-installed
+
+Development
+-----------
+The latest source code can be obtained from
+`<https://github.com/thomasvrussell/sfft>`_.
+
+When submitting bug reports or questions via the `issue tracker 
+<https://github.com/thomasvrussell/sfft/issues>`_, please include the following 
+information:
+
+- OS platform.
+- Python version.
+- CUDA and CuPy (or PyCUDA) version.
+- Version of sfft.
+
+Citing
+------
+
+*Image Subtraction in Fourier Space. Hu, L., Wang, L., Chen, X., & Yang, J. 2022, The Astrophysical Journal, 936, 157*
+
+Arxiv link: `<https://arxiv.org/abs/2109.09334>`_.
+
+ApJ Publication link: `<https://doi.org/10.3847/1538-4357/ac7394>`_.
+
+Related DOI: 10.3847/1538-4357/ac7394
```

### Comparing `sfft-1.3.4/README.rst` & `sfft-1.4.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,30 +31,32 @@
     
     pip install sfft
 
 Or alternatively, install any desired version of sfft from Github `<https://github.com/thomasvrussell/sfft>`_: ::
 
     python setup.py install
 
-sfft has the following three backends to perform the image subtraction.
+sfft now has the following two backends to perform the image subtraction.
 
-.. [#] **NumPy backend** : sfft will totally run on the CPU devices. NO GPU devices and CUDA dependencies are required for this backend.
-.. [#] **PyCUDA backend** : The core functions of sfft are written in `PyCUDA <https://github.com/inducer/pycuda>`_ and `Scikit-Cuda <https://github.com/lebedov/scikit-cuda>`_. Users need to install PyCUDA and Scikit-Cuda according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
 .. [#] **CuPy backend** : The core functions of sfft are written in `CuPy <https://github.com/cupy/cupy>`_. Users need to install CuPy according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
+.. [#] **NumPy backend** : sfft will totally run on the CPU devices. NO GPU devices and CUDA dependencies are required for this backend.
+
+- CUDA 12: E.g, you may enable the CuPy backend for CUDA 12.0 via: ::
+
+    pip install cupy-cuda12x
 
 - CUDA 11: E.g, you may enable the CuPy backend for CUDA 11.5 via: ::
 
-    pip install cupy-cuda115  # CuPy backend
+    pip install cupy-cuda115
+
+- CUDA 10: E.g, you may enable the CuPy backend for CUDA 10.1 via: ::
 
-- CUDA 10: E.g, you may enable the GPU backends (i.e., PyCUDA backend and CuPy backend) for CUDA 10.1 via: ::
+    pip install cupy-cuda101
 
-    pip install pycuda==2020.1 scikit-cuda==0.5.3  # PyCUDA backend
-    pip install cupy-cuda101                       # CuPy backend
-                   
-**Additional Remarks**: CuPy backend is faster than PyCUDA backend, while it consumes more GPU memory. Generally, I strongly recommend users to adopt CuPy backend as long as it does not incur GPU out-of-memory issue. Note that PyCUDA backend is still not compatiable with CUDA 11.
+**Additional Remarks**: There was a PyCUDA backend in sfft but now deprecated since v1.4.0. For sfft < v1.4.0, PyCUDA backend was preserved as it consumes less GPU memory. However, the CuPy backend is now better implemented for GPU memory allocation, making the PyCUDA backend no longer useful.
 
 Dependencies
 -----------
 
 You need further to install additional astronomical software for sfft.
 
 - `SExtractor <https://github.com/astromatic/sextractor>`_: SExtractor is required for sfft preprocessing, as it enables sfft to determine a proper pixel mask over the input image-pair before the image subtraction (this is critical for a more reasonable parameter-solving). Note that we have wrapped SExtractor into a Python module ``sfft.utils.pyAstroMatic.PYSEx`` so that one can trigger SExtractor within Python (please type help(``sfft.utils.pyAstroMatic.PYSEx``) to find its usage). As an AstrOmatic software, you can install SExtractor following `<https://www.astromatic.net/software/sextractor/>`_, or alternatively, install via conda: ::
@@ -138,34 +140,46 @@
 -----------
 
 We have tried our best to ensure the backward compatiablity, however, the rule was sometimes overrided in the development of sfft, e.g., some arguments might be deprecated in higher version of sfft. Users might get errors when they use old scripts but update sfft to a higher version. To solve the problem, I have been maintaining the test scripts on Github to make sure they can always work for the lastest version of sfft. You can also find the change log of arguments in the test scripts. 
 
 What's new
 -----------
 
+- A warning for users: As scikit-image has changed something in its function of hough detection since version 0.19.0, I recently found that the source selection in sfft will be affected by this upgrade. I have not checked the new function yet, for the time being I would recommend users to install a scikit-image >= 0.16.2 but <= 0.18.3. Possibly I may add a constrain on scikit-image version in sfft 1.3.5. [Lei, Nov 9, 2022]
+
+- A warning message about the usage of ``sfft.MultiEasySparsePacket`` and ``sfft.MultiEasyCrowdedPacket`` is added in the related test scripts. [Lei, Oct 25, 2022]
+
 - The preprocessing in sparse-flavor-sfft is refined using an additional rejection of mild varaibles since version 1.3.0. [Lei, Aug 19, 2022]
 
 - The sfft is now optimized for multiple tasks since version 1.1.0. [Lei, May 24, 2022]
 
 - A few argument-names have been changed since version 1.1.0, please see the test scripts. [Lei, May 24, 2022]
 
 - Locking file is removed since version 1.1.0, as I found it unreliable in our tests, i.e., -GLockFile is removed. [Lei, May 24, 2022]
 
 - The trial subtraction for refinement is removed since version 1.1.0. However, I add a post-subtraction check to search anomalies on the difference image using the same logic. One can feed the coordinates of the anomalies to sfft again as Prior-Banned sources to refine the subtraction (see -XY_PriorBan in ``sfft.MultiEasySparsePacket``). [Lei, May 24, 2022]
 
 Todo list
 -----------
 
+- The total GPU memory usage is only optimized for KerPolyOrder = 2 & BGPolyOrder = 2, I will extend the optimization to other cases ASAP! In fact, I believe there is ample space for reducing the total GPU usage and I will explore it. [Lei, Nov 11, 2022] **[ALREADY DONE]**
+
+- I will allows users to disable the hough detection for preprocessing when there are too few sources in the field in the next version sfft v1.3.5. [Lei, Nov 11, 2022]
+
+- Add a verbose argument for sfft so that users can get more clean printed messages. [Lei, Nov 9, 2022] **[ALREADY DONE]**
+
+- Test if we can use sep to replace SExtractor in preprocessing to make sfft more Pythonic. [Lei, Nov 9, 2022] 
+
 - Incorporate the separate functions (in the folder beta4spline) for spline form sfft into the unified sfft functions. Note that only Numpy backend is currently available and the spline form is very memory-consuming. [Lei, July 6, 2022]
 
 - Write a detailed documentation for sfft! [Lei, May 24, 2022]
 
 - We notice that SExtractor may have been called to perform astrometric calibration before image subtraction. It is definitely not wise to run SExtractor again in sfft, I need to develop a module which allows users to feed SExtractor products as inputs of sfft, which will significantly reduce the preprocessing time in sfft. [Lei, May 24, 2022]
 
-- The multiprocessing mode is expected to accomondate multiple GPU devices, however, the function has not tested on such a multi-GPUs platform. [Lei, May 24, 2022]
+- The multiprocessing mode is expected to accomondate multiple GPU devices, however, the function has not tested on such a multi-GPUs platform. [Lei, May 24, 2022] **[ALREADY DONE]**
 
 - Add a function for optimizing sfft on a given computing platform with multiple CPU threading and one/multiple GPU card(s). This would be very useful to reduce the overall time cost when users have a large set of image-pairs to be processed simultaneously (e.g., serve for DECam, each exposure produces 61 CCD images). [Lei, May 20, 2022] **[ALREADY DONE]**
 
 Common issues
 -----------
 
 - If your Python environment already has some version of llvmlite (a package required by NumPy backend) before installing sfft. The setup.py in sfft cannot properly update llvmlite to the desired version, then you may get errors related to Numba or llvmlite. If so, please manually install llvmlite by: ::
@@ -179,15 +193,15 @@
 
 When submitting bug reports or questions via the `issue tracker 
 <https://github.com/thomasvrussell/sfft/issues>`_, please include the following 
 information:
 
 - OS platform.
 - Python version.
-- CUDA, PyCUDA and CuPy version.
+- CUDA and CuPy (or PyCUDA) version.
 - Version of sfft.
 
 Citing
 ------
 
 *Image Subtraction in Fourier Space. Hu, L., Wang, L., Chen, X., & Yang, J. 2022, The Astrophysical Journal, 936, 157*
```

### Comparing `sfft-1.3.4/setup.py` & `sfft-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 AUTHOR = "Lei Hu"
 AUTHOR_EMAIL = "hulei@pmo.ac.cn"
 MAINTAINER = "Lei Hu"
 MAINTAINER_EMAIL = "hulei@pmo.ac.cn"
 DOWNLOAD_URL = 'https://github.com/thomasvrussell/sfft'
 
 LICENSE = 'MIT Licence'
-VERSION = '1.3.4'
+VERSION = '1.4.0'
 
 install_reqs = ['scipy>=1.5.2',
                 'astropy>=3.2.3',
-                'scikit-image>=0.16.2',
+                'scikit-image>=0.16.2,<=0.18.3',
                 'fastremap>=1.7.0',
                 'sep>=1.0.3',
                 'numba==0.53.1',
                 'llvmlite==0.36.0',
                 'pyfftw==0.12.0']
 
 setup(name = NAME,
```

### Comparing `sfft-1.3.4/sfft/AutoCrowdedPrep.py` & `sfft-1.4.0/sfft/AutoCrowdedPrep.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import sep
 import fastremap
 import numpy as np
 from astropy.io import fits
 import scipy.ndimage as ndimage
 from sfft.utils.pyAstroMatic.PYSEx import PY_SEx
 from sfft.utils.WeightedQuantile import TopFlatten_Weighted_Quantile
-# version: Aug 17, 2022
+# version: Feb 4, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class Auto_CrowdedPrep:
     def __init__(self, FITS_REF, FITS_SCI, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', BACK_TYPE='AUTO', BACK_VALUE=0.0, \
-        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=5.0, DETECT_MINAREA=5, DETECT_MAXAREA=0, \
-        DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=None, BoundarySIZE=0.0):
+        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=5.0, ANALYSIS_THRESH=5.0, DETECT_MINAREA=5, DETECT_MAXAREA=0, \
+        DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=None, BoundarySIZE=0.0, VERBOSE_LEVEL=2):
 
         self.FITS_REF = FITS_REF
         self.FITS_SCI = FITS_SCI
 
         self.GAIN_KEY = GAIN_KEY
         self.SATUR_KEY = SATUR_KEY
 
         self.BACK_TYPE = BACK_TYPE
         self.BACK_VALUE = BACK_VALUE
         self.BACK_SIZE = BACK_SIZE
         self.BACK_FILTERSIZE = BACK_FILTERSIZE
 
         self.DETECT_THRESH = DETECT_THRESH
+        self.ANALYSIS_THRESH = ANALYSIS_THRESH
         self.DETECT_MINAREA = DETECT_MINAREA
         self.DETECT_MAXAREA = DETECT_MAXAREA
         self.DEBLEND_MINCONT = DEBLEND_MINCONT
         self.BACKPHOTO_TYPE = BACKPHOTO_TYPE
 
         self.ONLY_FLAGS = ONLY_FLAGS
         self.BoundarySIZE = BoundarySIZE
+        self.VERBOSE_LEVEL = VERBOSE_LEVEL
     
     def AutoMask(self, BACK_SIZE_SUPER=128, StarExt_iter=2, PriorBanMask=None):
 
         # * Generate Super-Background for REF & SCI
         PixA_REF = fits.getdata(self.FITS_REF, ext=0).T
         PixA_SCI = fits.getdata(self.FITS_SCI, ext=0).T
 
@@ -53,21 +55,23 @@
         PixA_SBG_REF = sep.Background(PixA_REF, bw=BACK_SIZE_SUPER, bh=BACK_SIZE_SUPER, fw=3, fh=3).back()        
         PixA_SBG_SCI = sep.Background(PixA_SCI, bw=BACK_SIZE_SUPER, bh=BACK_SIZE_SUPER, fw=3, fh=3).back()
 
         # * Generate Saturation-Mask for REF & SCI
         def GenSatMask(FITS_obj):
 
             # ** trigger a very-cold SExtractor
-            PL = ['X_IMAGE', 'Y_IMAGE', 'FLUX_AUTO', 'FLUXERR_AUTO', 'FLUX_MAX', 'FWHM_IMAGE']
-            PYSEX_OP = PY_SEx.PS(FITS_obj=FITS_obj, PL=PL, GAIN_KEY=self.GAIN_KEY, SATUR_KEY=self.SATUR_KEY, \
-                BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, BACK_SIZE=self.BACK_SIZE, \
-                BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, DETECT_MINAREA=self.DETECT_MINAREA, \
-                DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, \
-                CHECKIMAGE_TYPE='SEGMENTATION', AddRD=False, ONLY_FLAGS=self.ONLY_FLAGS, \
-                XBoundary=self.BoundarySIZE, YBoundary=self.BoundarySIZE, MDIR=None)
+            SExParam = ['X_IMAGE', 'Y_IMAGE', 'FLUX_AUTO', 'FLUXERR_AUTO', 'FLUX_MAX', 'FWHM_IMAGE']
+            PYSEX_OP = PY_SEx.PS(FITS_obj=FITS_obj, SExParam=SExParam, GAIN_KEY=self.GAIN_KEY, \
+                SATUR_KEY=self.SATUR_KEY, BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, \
+                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, \
+                ANALYSIS_THRESH=self.ANALYSIS_THRESH, DETECT_MINAREA=self.DETECT_MINAREA, \
+                DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, \
+                BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, CHECKIMAGE_TYPE='SEGMENTATION', AddRD=False, \
+                ONLY_FLAGS=self.ONLY_FLAGS, XBoundary=self.BoundarySIZE, YBoundary=self.BoundarySIZE, \
+                MDIR=None, VERBOSE_LEVEL=self.VERBOSE_LEVEL)
             AstSEx, PixA_SEG = PYSEX_OP[0], PYSEX_OP[1][0].astype(int)
             
             # *** Note on the crude estimate of FWHM ***
             # our strategy is to calculate a median FWHM_IMAGE weighted by the source flux, meanwhile, 
             # we modulate the weights by applying a penalty on the sources with large FWHM_IMAGE.
 
             NTE_4FWHM = 30  # NUM_TOP_END for FWHM, default value used herein.
@@ -101,44 +105,48 @@
             NUM_SAT = len(AstSEx_SAT)
             SatPROP = np.sum(SatMask) / (SatMask.shape[0] * SatMask.shape[1])
             return SATLEVEL, FWHM, SatMask, NUM_SAT, SatPROP
 
         SATLEVEL_REF, FWHM_REF, SatMask_REF, NUM_SAT_REF, SatPROP_REF = GenSatMask(self.FITS_REF)
         SATLEVEL_SCI, FWHM_SCI, SatMask_SCI, NUM_SAT_SCI, SatPROP_SCI = GenSatMask(self.FITS_SCI)
 
-        _message = 'Estimated [FWHM_REF = %.3f pix] & [FWHM_SCI = %.3f pix]!' %(FWHM_REF, FWHM_SCI)
-        print('\nMeLOn CheckPoint: %s' %_message)
-
-        _message = 'The SATURATED Regions --- Number (Pixel Proportion) '
-        _message += '[REF = %d (%s)] & ' %(NUM_SAT_REF, '{:.2%}'.format(SatPROP_REF))
-        _message += '[SCI = %d (%s)]!' %(NUM_SAT_SCI, '{:.2%}'.format(SatPROP_SCI))
-        print('\nMeLOn CheckPoint: %s' %_message)
+        if self.VERBOSE_LEVEL in [1, 2]:
+            _message = 'Estimated [FWHM_REF = %.3f pix] & [FWHM_SCI = %.3f pix]!' %(FWHM_REF, FWHM_SCI)
+            print('\nMeLOn CheckPoint: %s' %_message)
+
+        if self.VERBOSE_LEVEL in [2]:
+            _message = 'The SATURATED Regions --- Number (Pixel Proportion) '
+            _message += '[REF = %d (%s)] & ' %(NUM_SAT_REF, '{:.2%}'.format(SatPROP_REF))
+            _message += '[SCI = %d (%s)]!' %(NUM_SAT_SCI, '{:.2%}'.format(SatPROP_SCI))
+            print('\nMeLOn CheckPoint: %s' %_message)
         
         # * Define ProhibitedZone
         NaNmask_U = None
         if PriorBanMask is None:
             ProZone = np.logical_or(SatMask_REF, SatMask_SCI)
         else: ProZone = np.logical_or.reduce((PriorBanMask, SatMask_REF, SatMask_SCI))
         
         NaNmask_REF = np.isnan(PixA_REF)
         NaNmask_SCI = np.isnan(PixA_SCI)
         if NaNmask_REF.any() or NaNmask_SCI.any():
             NaNmask_U = np.logical_or(NaNmask_REF, NaNmask_SCI)
             ProZone[NaNmask_U] = True
 
         # * Make ActiveMask > PixA_mREF & PixA_mSCI
-        ActiveMask = ~ProZone
         PixA_mREF = PixA_REF.copy()
         PixA_mSCI = PixA_SCI.copy()
-        PixA_mREF[ProZone] = PixA_SBG_REF[ProZone]      # NOTE REF is not sky-subtracted yet
-        PixA_mSCI[ProZone] = PixA_SBG_SCI[ProZone]      # NOTE SCI is not sky-subtracted yet
-
+        
         # NOTE: The preparation can guarantee that mREF & mSCI are NaN-Free !
-        ActivePROP = np.sum(ActiveMask) / (ActiveMask.shape[0] * ActiveMask.shape[1])
-        print('\nMeLOn CheckPoint: Active-Mask Pixel Proportion [%s]' %('{:.2%}'.format(ActivePROP)))
+        PixA_mREF[ProZone] = PixA_SBG_REF[ProZone]      # NOTE REF is not sky-subtracted
+        PixA_mSCI[ProZone] = PixA_SBG_SCI[ProZone]      # NOTE SCI is not sky-subtracted
+
+        ActiveMask = ~ProZone
+        if self.VERBOSE_LEVEL in [1, 2]:
+            ActivePROP = np.sum(ActiveMask) / (ActiveMask.shape[0] * ActiveMask.shape[1])
+            print('\nMeLOn CheckPoint: Active-Mask Pixel Proportion [%s]' %('{:.2%}'.format(ActivePROP)))
 
         # * Create sfft-prep master dictionary
         SFFTPrepDict = {}
         SFFTPrepDict['PixA_REF'] = PixA_REF
         SFFTPrepDict['PixA_SCI'] = PixA_SCI
         SFFTPrepDict['Union-NaN-Mask'] = NaNmask_U
```

### Comparing `sfft-1.3.4/sfft/AutoSparsePrep.py` & `sfft-1.4.0/sfft/AutoSparsePrep.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 from astropy.io import fits
 import scipy.ndimage as ndimage
 from astropy.table import Column, hstack
 from sfft.utils.pyAstroMatic.PYSEx import PY_SEx
 from sfft.utils.SymmetricMatch import Symmetric_Match
 from sfft.utils.HoughMorphClassifier import Hough_MorphClassifier
 from sfft.utils.WeightedQuantile import TopFlatten_Weighted_Quantile
-# version: Sep 18, 2022
+# version: Feb 10, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class Auto_SparsePrep:
-    def __init__(self, FITS_REF, FITS_SCI, GAIN_KEY='GAIN', SATUR_KEY='ESATUR', \
-        BACK_TYPE='MANUAL', BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, \
-        DETECT_THRESH=2.0, DETECT_MINAREA=5, DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, \
-        BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=[0], BoundarySIZE=30):
+    def __init__(self, FITS_REF, FITS_SCI, GAIN_KEY='GAIN', SATUR_KEY='ESATUR', BACK_TYPE='MANUAL', \
+        BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=2.0, ANALYSIS_THRESH=2.0, DETECT_MINAREA=5, \
+        DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=[0], BoundarySIZE=30, VERBOSE_LEVEL=2):
 
         self.FITS_REF = FITS_REF
         self.FITS_SCI = FITS_SCI
 
         self.GAIN_KEY = GAIN_KEY
         self.SATUR_KEY = SATUR_KEY
 
         self.BACK_TYPE = BACK_TYPE
         self.BACK_VALUE = BACK_VALUE
         self.BACK_SIZE = BACK_SIZE
         self.BACK_FILTERSIZE = BACK_FILTERSIZE
 
         self.DETECT_THRESH = DETECT_THRESH
+        self.ANALYSIS_THRESH = ANALYSIS_THRESH
         self.DETECT_MINAREA = DETECT_MINAREA
         self.DETECT_MAXAREA = DETECT_MAXAREA
         self.DEBLEND_MINCONT = DEBLEND_MINCONT
         self.BACKPHOTO_TYPE = BACKPHOTO_TYPE
 
         self.ONLY_FLAGS = ONLY_FLAGS
         self.BoundarySIZE = BoundarySIZE
+        self.VERBOSE_LEVEL = VERBOSE_LEVEL
 
     def run_image_mask(self, AstSEx_SS, PixA_SEGr, PixA_SEGs, StarExt_iter, XY_PriorBan):
         
         PixA_REF = fits.getdata(self.FITS_REF, ext=0).T
         if np.issubdtype(PixA_REF.dtype, np.integer):
             PixA_REF = PixA_REF.astype(np.float64)
         
@@ -96,32 +97,35 @@
             #    NOTE: Unlike Prior-Selection, the Prior-Ban coordinates do not have to be accurate.
             #    WARNING NOTE: AstSEx_SS will be updated in this step!
 
             SEGL_PB = np.unique([SFFTLmap[int(_x - 0.5), int(_y - 0.5)] for _x, _y in XY_PriorBan])
             SEGL_PB = SEGL_PB[SEGL_PB > 0] 
             PBMASK_SS = np.in1d(SEGL_SS, SEGL_PB)
             AstSEx_SS.add_column(Column(PBMASK_SS, name='MASK_PriorBan'))
-            _message = 'Find / Given [%d / %d] Prior-Banned ' %(np.sum(PBMASK_SS), XY_PriorBan.shape[0])
-            _message += 'in current [%d] SubSources!' %(len(AstSEx_SS))
-            print('MeLOn CheckPoint: %s' %_message)
-
+            
+            if self.VERBOSE_LEVEL in [1, 2]:
+                _message = 'Find / Given [%d / %d] Prior-Banned ' %(np.sum(PBMASK_SS), XY_PriorBan.shape[0])
+                _message += 'in current [%d] SubSources!' %(len(AstSEx_SS))
+                print('MeLOn CheckPoint: %s' %_message)
+            
             # ** Update Label Map (SFFTLmap) by inactivating the Prior-Banned SubSources
             _mappings = {label: -64 for label in SEGL_SS[PBMASK_SS]}
             fastremap.remap(SFFTLmap, _mappings, preserve_missing_labels=True, in_place=True)
         else:
-            _message = 'Find / Given [0 / 0] Prior-Banned '
-            _message += 'in current [%d] SubSources!' %(len(AstSEx_SS))
-            print('MeLOn CheckPoint: %s' %_message)
-        
+            if self.VERBOSE_LEVEL in [1, 2]:
+                print('MeLOn CheckPoint: SKIP, NO Prior-Banned Coordinates Given!')
+
         # * Create ActiveMask
         #   NOTE: The preparation can guarantee that mREF & mSCI are NaN-Free !
         ActiveMask = SFFTLmap > 0
-        ActivePROP = np.sum(ActiveMask) / (ActiveMask.shape[0] * ActiveMask.shape[1])
-        print('MeLOn CheckPoint: Active-Mask (Non-Prior-Banned SubSources) Pixel Proportion [%s]' \
-               %('{:.2%}'.format(ActivePROP)))
+        
+        if self.VERBOSE_LEVEL in [1, 2]:
+            ActivePROP = np.sum(ActiveMask) / (ActiveMask.shape[0] * ActiveMask.shape[1])
+            print('MeLOn CheckPoint: Active-Mask (Non-Prior-Banned SubSources) Pixel Proportion [%s]' \
+                   %('{:.2%}'.format(ActivePROP)))
 
         # * Produce masked images PixA_mREF & PixA_mSCI
         PixA_mREF = PixA_REF.copy()
         PixA_mSCI = PixA_SCI.copy()
         PixA_mREF[~ActiveMask] = 0.0      # NOTE REF has been sky-subtracted
         PixA_mSCI[~ActiveMask] = 0.0      # NOTE SCI has been sky-subtracted
 
@@ -140,50 +144,64 @@
         SFFTPrepDict['SFFT-LabelMap'] = SFFTLmap
         SFFTPrepDict['Active-Mask'] = ActiveMask
         SFFTPrepDict['PixA_mREF'] = PixA_mREF
         SFFTPrepDict['PixA_mSCI'] = PixA_mSCI
 
         return SFFTPrepDict
 
-    def HoughAutoMask(self, Hough_FRLowerLimit=0.1, Hough_peak_clip=0.7, BeltHW=0.2, PS_ELLIPThresh=0.3, \
+    def HoughAutoMask(self, Hough_MINFR=0.1, Hough_PeakClip=0.7, BeltHW=0.2, PointSource_MINELLIP=0.3, \
         MatchTol=None, MatchTolFactor=3.0, COARSE_VAR_REJECTION=True, CVREJ_MAGD_THRESH=0.12, \
-        ELABO_VAR_REJECTION=False, EVREJ_RATIO_THREH=5.0, EVREJ_SAFE_MAGDEV=0.04, StarExt_iter=4, XY_PriorBan=None):
+        ELABO_VAR_REJECTION=False, EVREJ_RATIO_THREH=5.0, EVREJ_SAFE_MAGDEV=0.04, \
+        StarExt_iter=4, XY_PriorBan=None):
+
         # - Hough Transform is used to determine subtraction-sources
+        # TODO: change parameter names
+        # TODO: add a robust clipping on SNR & FR, use the DECam examples to determine ...
+        # TODO: allows PointSource_ELLIP_Thresh being None?
 
         # * Use Hough-MorphClassifer to identify GoodSources in REF & SCI
         def main_hough(FITS_obj):
             # NOTE: SEGMENTATION map is sensitive to DETECT_THRESH
             Hmc = Hough_MorphClassifier.MakeCatalog(FITS_obj=FITS_obj, GAIN_KEY=self.GAIN_KEY, \
-                SATUR_KEY=self.SATUR_KEY, BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, BACK_SIZE=self.BACK_SIZE, \
-                BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, DETECT_MINAREA=self.DETECT_MINAREA, \
-                DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, \
+                SATUR_KEY=self.SATUR_KEY, BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, \
+                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, \
+                DETECT_THRESH=self.DETECT_THRESH, ANALYSIS_THRESH=self.ANALYSIS_THRESH, \
+                DETECT_MINAREA=self.DETECT_MINAREA, DETECT_MAXAREA=self.DETECT_MAXAREA, \
+                DEBLEND_MINCONT=self.DEBLEND_MINCONT, BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, \
                 CHECKIMAGE_TYPE='SEGMENTATION', AddRD=False, ONLY_FLAGS=self.ONLY_FLAGS, \
-                BoundarySIZE=self.BoundarySIZE, AddSNR=False)
+                BoundarySIZE=self.BoundarySIZE, AddSNR=False, VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+            PixA_SEG = Hmc[1][0].astype(int)
 
-            Hc = Hough_MorphClassifier.Classifier(AstSEx=Hmc[0], Hough_FRLowerLimit=Hough_FRLowerLimit, \
-                Hough_peak_clip=Hough_peak_clip, BeltHW=BeltHW, PS_ELLIPThresh=PS_ELLIPThresh)    
-            AstSEx_GS, FHWM, PixA_SEG = Hmc[0][Hc[2]], Hc[0], Hmc[1][0].astype(int)
+            Hc = Hough_MorphClassifier.Classifier(AstSEx=Hmc[0], Hough_MINFR=Hough_MINFR, \
+                Hough_PeakClip=Hough_PeakClip, BeltHW=BeltHW, PointSource_MINELLIP=PointSource_MINELLIP, \
+                VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+            FHWM = Hc[5]
+            AstSEx_GS = Hmc[0][Hc[3]]
             return AstSEx_GS, FHWM, PixA_SEG
         
         AstSEx_GSr, FWHM_REF, PixA_SEGr = main_hough(self.FITS_REF)
         AstSEx_GSs, FWHM_SCI, PixA_SEGs = main_hough(self.FITS_SCI)
-        _message = 'Estimated [FWHM_REF = %.3f pix] & [FWHM_SCI = %.3f pix]!' %(FWHM_REF, FWHM_SCI)
-        print('\nMeLOn CheckPoint: %s' %_message)
+
+        if self.VERBOSE_LEVEL in [1, 2]:
+            _message = 'Estimated [FWHM_REF = %.3f pix] & [FWHM_SCI = %.3f pix]!' %(FWHM_REF, FWHM_SCI)
+            print('\nMeLOn CheckPoint: %s' %_message)
 
         # * Determine Matched-GoodSources (abbr. MGS)
         XY_GSr = np.array([AstSEx_GSr['X_IMAGE'], AstSEx_GSr['Y_IMAGE']]).T
         XY_GSs = np.array([AstSEx_GSs['X_IMAGE'], AstSEx_GSs['Y_IMAGE']]).T
         
         UMatchTol = MatchTol
         if MatchTol is None:
             # - Given precise WCS, one can use a high MatchTolFactor ~ 3.0
             # - For very sparse fields where WCS is inaccurate, one can loosen MatchTolFactor to ~ 1.0
             # - WARNING NOTE: it can go wrong when the estimated FWHM is highly inaccurate.
             UMatchTol = np.sqrt((FWHM_REF / MatchTolFactor)**2 + (FWHM_SCI / MatchTolFactor)**2)
-        print('MeLOn CheckPoint: Tolerance [%.3f pix] For Source Cross-Match!' %UMatchTol)
+
+        if self.VERBOSE_LEVEL in [2]:
+            print('MeLOn CheckPoint: Tolerance [%.3f pix] For Source Cross-Match!' %UMatchTol)
 
         Symm = Symmetric_Match.SM(XY_A=XY_GSr, XY_B=XY_GSs, tol=UMatchTol, return_distance=False)
         AstSEx_MGSr = AstSEx_GSr[Symm[:, 0]]
         AstSEx_MGSs = AstSEx_GSs[Symm[:, 1]]
         NUM_MGS = Symm.shape[0]
 
         # * Determine Magnitude Offset from MGS
@@ -194,44 +212,52 @@
 
         MAGD_MGS = MAG_MGSs - MAG_MGSr
         MAG_OFFSET0 = np.median(MAGD_MGS)
 
         NTE_4MO = 30  # NUM_TOP_END for MAG_OFFSET, default value used herein.
         MAG_OFFSETr = TopFlatten_Weighted_Quantile.TFWQ(values=MAGD_MGS, weights=FLUX_MGSr, \
             quantiles=[0.5], NUM_TOP_END=NTE_4MO)[0]
+        
         MAG_OFFSETs = TopFlatten_Weighted_Quantile.TFWQ(values=MAGD_MGS, weights=FLUX_MGSs, \
             quantiles=[0.5], NUM_TOP_END=NTE_4MO)[0]
         MAG_OFFSET = (MAG_OFFSETr + MAG_OFFSETs)/2.0
         
         if np.abs(MAG_OFFSET - MAG_OFFSET0) > 0.05:
-            _warn_message = 'Magnitude Offset Estimate --- WEIGHTED-MEDIAN IS HIGHLY DEVIATED FROM MEDIAN '
-            _warn_message += '[median: %.3f mag] >>> [weighted-median: %.3f mag]!' %(MAG_OFFSET0, MAG_OFFSET)
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
-        else:
+            if self.VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'Magnitude Offset Estimate --- WEIGHTED-MEDIAN IS HIGHLY DEVIATED FROM MEDIAN '
+                _warn_message += '[median: %.3f mag] >>> [weighted-median: %.3f mag]!' %(MAG_OFFSET0, MAG_OFFSET)
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+        
+        if self.VERBOSE_LEVEL in [2]:
             _message = 'Magnitude Offset Estimate --- '
             _message += '[median: %.3f mag] >>> [weighted-median: %.3f mag]!' %(MAG_OFFSET0, MAG_OFFSET)
             print('\nMeLOn CheckPoint: %s' %_message)
 
         # * Apply a coarse variable rejection (abbr. CVREJ)
         if COARSE_VAR_REJECTION:
             CVREJ_MASK = np.abs(MAGD_MGS - MAG_OFFSET) > CVREJ_MAGD_THRESH
             AstSEx_iSSr = AstSEx_MGSr[~CVREJ_MASK]
             AstSEx_iSSs = AstSEx_MGSs[~CVREJ_MASK]
-            _message = 'Coarse Variable Rejection [magnitude deviation > %.3f mag] ' %CVREJ_MAGD_THRESH
-            _message += 'on Matched-GoodSources [%d / %d]!' %(np.sum(CVREJ_MASK), NUM_MGS)
-            print('\nMeLOn CheckPoint: %s' %_message)
+            
+            if self.VERBOSE_LEVEL in [1, 2]:
+                _message = 'Coarse Variable Rejection [magnitude deviation > %.3f mag] ' %CVREJ_MAGD_THRESH
+                _message += 'on Matched-GoodSources [%d / %d]!' %(np.sum(CVREJ_MASK), NUM_MGS)
+                print('\nMeLOn CheckPoint: %s' %_message)
         else:
             AstSEx_iSSr = AstSEx_MGSr
             AstSEx_iSSs = AstSEx_MGSs
-            print('\nMeLOn CheckPoint: SKIP Coarse Variable Rejection!')
+
+            if self.VERBOSE_LEVEL in [1, 2]:
+                print('\nMeLOn CheckPoint: SKIP Coarse Variable Rejection!')
 
         # * Apply a more elaborate variable rejection (abbr. EVREJ)
         if ELABO_VAR_REJECTION:
-            warnings.warn('\nMeLOn WARNING: Elaborate Variable Rejection requires CORRECT GAIN in FITS HEADER!')
-            # TODO: Incorporate weight-maps of the input image pair for more accurate SExtractor FLUXERR.
+
+            if self.VERBOSE_LEVEL in [2]:
+                warnings.warn('\nMeLOn WARNING: Elaborate Variable Rejection requires CORRECT GAIN in FITS HEADER!')
 
             """
             # Remarks on the Elaborate Variable Rejection
             # [1] The coarse variable rejection by CVREJ_MAGD_THRESH can only exclude the most drastic variable sources.
             #     As a result, the possible missing varaibles, especially at the bright end, can strongly affect the subtraction. 
             #
             # [2] Elaborate Variable Rejection (EVREJ) is designed to further identify variables by taking their 
@@ -277,91 +303,107 @@
             _SAFEMASK = np.abs(MAGD_iSS - MAG_OFFSET) <= EVREJ_SAFE_MAGDEV
             
             EVREJ_MASK = np.logical_and(_OUTMASK, ~_SAFEMASK)
             AstSEx_SSr = AstSEx_iSSr[~EVREJ_MASK]
             AstSEx_SSs = AstSEx_iSSs[~EVREJ_MASK]
 
             EVREJ_PERC = np.sum(EVREJ_MASK) / NUM_MGS
-            _message = 'Elaborate Variable Rejection [flux deviation > %.2f sigma] & ' %EVREJ_RATIO_THREH
-            _message += '[magnitude deviation > %.3f mag] ' %EVREJ_SAFE_MAGDEV
-            _message += 'on Matched-GoodSources [%d / %d] ' %(np.sum(EVREJ_MASK), NUM_MGS)
-            _message += 'or [%s]!' %('{:.2%}'.format(EVREJ_PERC))
-            print('\nMeLOn CheckPoint: %s' %_message)
+
+            if self.VERBOSE_LEVEL in [1, 2]:
+                _message = 'Elaborate Variable Rejection [flux deviation > %.2f sigma] & ' %EVREJ_RATIO_THREH
+                _message += '[magnitude deviation > %.3f mag] ' %EVREJ_SAFE_MAGDEV
+                _message += 'on Matched-GoodSources [%d / %d] ' %(np.sum(EVREJ_MASK), NUM_MGS)
+                _message += 'or [%s]!' %('{:.2%}'.format(EVREJ_PERC))
+                print('\nMeLOn CheckPoint: %s' %_message)
 
             if EVREJ_PERC > 0.1:
-                _warn_message = '[%s] Matched-GoodSources ARE REJECTED BY EVREJ!' %('{:.2%}'.format(EVREJ_PERC))
-                warnings.warn('\nMeLOn IMPORTANT WARNING: %s' %_warn_message)
+                if self.VERBOSE_LEVEL in [0, 1, 2]:
+                    _warn_message = '[%s] Matched-GoodSources ARE REJECTED BY EVREJ!' %('{:.2%}'.format(EVREJ_PERC))
+                    warnings.warn('\nMeLOn IMPORTANT WARNING: %s' %_warn_message)
         else:
             AstSEx_SSr = AstSEx_iSSr
             AstSEx_SSs = AstSEx_iSSs
-            print('\nMeLOn CheckPoint: SKIP Elaborate Variable Rejection!')
+            
+            if self.VERBOSE_LEVEL in [1, 2]:
+                print('\nMeLOn CheckPoint: SKIP Elaborate Variable Rejection!')
 
         # * Combine catalogs for survived MGS (i.e., SubSources)
         for coln in AstSEx_SSr.colnames:
             AstSEx_SSr[coln].name = coln + '_REF'
             AstSEx_SSs[coln].name = coln + '_SCI'
         AstSEx_SS = hstack([AstSEx_SSr, AstSEx_SSs])
         
         # create unified segmentation label
         AstSEx_SS.add_column(Column(1+np.arange(len(AstSEx_SS)), name='SEGLABEL'), index=0)
-        print('\nMeLOn CheckPoint: SubSources out of Matched-GoodSources [%d / %d]!' %(len(AstSEx_SS), NUM_MGS))
+        if self.VERBOSE_LEVEL in [1, 2]:
+            print('\nMeLOn CheckPoint: SubSources out of Matched-GoodSources [%d / %d]!' %(len(AstSEx_SS), NUM_MGS))
         
         # * Run Image Masking (P.S. some SubSources might be marked as invalid by the Prior-Ban list)
         SFFTPrepDict = self.run_image_mask(AstSEx_SS=AstSEx_SS, PixA_SEGr=PixA_SEGr, \
             PixA_SEGs=PixA_SEGs, StarExt_iter=StarExt_iter, XY_PriorBan=XY_PriorBan)
         
         # * Append Additional information
         SFFTPrepDict['MAG_OFFSET'] = MAG_OFFSET
         SFFTPrepDict['FWHM_REF'] = FWHM_REF
         SFFTPrepDict['FWHM_SCI'] = FWHM_SCI
 
         return SFFTPrepDict
 
-    def SemiAutoMask(self, XY_PriorSelect=None, MatchTol=None, MatchTolFactor=3.0, StarExt_iter=4, XY_PriorBan=None):
+    def SemiAutoMask(self, XY_PriorSelect=None, MatchTol=None, MatchTolFactor=3.0, \
+        StarExt_iter=4, XY_PriorBan=None):
         # - We directly use given Prior-Selection to determine subtraction-sources
 
         def func4phot(FITS_obj):
             # run SExtractor photometry
-            PL = ['X_IMAGE', 'Y_IMAGE', 'FLUX_AUTO', 'FLUXERR_AUTO', 'MAG_AUTO', 'MAGERR_AUTO', \
-                  'FLAGS', 'FLUX_RADIUS', 'FWHM_IMAGE', 'A_IMAGE', 'B_IMAGE']
-            PYSEX_OP = PY_SEx.PS(FITS_obj=FITS_obj, PL=PL, GAIN_KEY=self.GAIN_KEY, SATUR_KEY=self.SATUR_KEY, \
-                BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, BACK_SIZE=self.BACK_SIZE, \
-                BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, DETECT_MINAREA=self.DETECT_MINAREA, \
-                DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, \
-                CHECKIMAGE_TYPE='SEGMENTATION', AddRD=False, ONLY_FLAGS=self.ONLY_FLAGS, \
-                XBoundary=self.BoundarySIZE, YBoundary=self.BoundarySIZE, MDIR=None)
+            SExParam = ['X_IMAGE', 'Y_IMAGE', 'FLUX_AUTO', 'FLUXERR_AUTO', 'MAG_AUTO', \
+                        'MAGERR_AUTO', 'FLAGS', 'FLUX_RADIUS', 'FWHM_IMAGE', 'A_IMAGE', 'B_IMAGE']
+            
+            PYSEX_OP = PY_SEx.PS(FITS_obj=FITS_obj, SExParam=SExParam, GAIN_KEY=self.GAIN_KEY, \
+                SATUR_KEY=self.SATUR_KEY, BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, \
+                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, \
+                ANALYSIS_THRESH=self.ANALYSIS_THRESH, DETECT_MINAREA=self.DETECT_MINAREA, \
+                DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, \
+                BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, CHECKIMAGE_TYPE='SEGMENTATION', AddRD=False, \
+                ONLY_FLAGS=self.ONLY_FLAGS, XBoundary=self.BoundarySIZE, YBoundary=self.BoundarySIZE, \
+                MDIR=None, VERBOSE_LEVEL=self.VERBOSE_LEVEL)
             AstSEx, PixA_SEG = PYSEX_OP[0], PYSEX_OP[1][0].astype(int)
             
             # *** Note on the crude estimate of FWHM ***
             # our strategy is to calculate a median FWHM_IMAGE weighted by the source flux, meanwhile, 
             # we modulate the weights by applying a penalty on the sources with large FWHM_IMAGE.
 
             NTE_4FWHM = 30  # NUM_TOP_END for FWHM, default value used herein.
             _values, _weights = np.array(AstSEx['FWHM_IMAGE']), np.array(AstSEx['FLUX_AUTO'])
-            _weights /= np.clip(_values, a_min=1.0, a_max=None)**2  
+            _weights /= np.clip(_values, a_min=1.0, a_max=None)**2
+
             FWHM = TopFlatten_Weighted_Quantile.TFWQ(values=_values, weights=_weights, \
                 quantiles=[0.5], NUM_TOP_END=NTE_4FWHM)[0]
             return AstSEx, FWHM, PixA_SEG
         
         AstSExr, FWHM_REF, PixA_SEGr = func4phot(self.FITS_REF)
         AstSExs, FWHM_SCI, PixA_SEGs = func4phot(self.FITS_SCI)
-        _message = 'Estimated [FWHM_REF = %.3f pix] & [FWHM_SCI = %.3f pix]!' %(FWHM_REF, FWHM_SCI)
-        print('\nMeLOn CheckPoint: %s' %_message)
+        
+        if self.VERBOSE_LEVEL in [1, 2]:
+            _message = 'Estimated [FWHM_REF = %.3f pix] & [FWHM_SCI = %.3f pix]!' %(FWHM_REF, FWHM_SCI)
+            print('\nMeLOn CheckPoint: %s' %_message)
 
         # * Cross Match REF & SCI catalogs
         XYr = np.array([AstSExr['X_IMAGE'], AstSExr['Y_IMAGE']]).T
         XYs = np.array([AstSExs['X_IMAGE'], AstSExs['Y_IMAGE']]).T
 
         UMatchTol = MatchTol
         if MatchTol is None:
             # - Given precise WCS, one can use a high MatchTolFactor ~ 3.0
             # - For very sparse fields where WCS is inaccurate, one can loosen MatchTolFactor to ~ 1.0
             # - WARNING NOTE: it can go wrong when the estimated FWHM is highly inaccurate.
             UMatchTol = np.sqrt((FWHM_REF / MatchTolFactor)**2 + (FWHM_SCI / MatchTolFactor)**2)
-        print('MeLOn CheckPoint: Tolerance [%.3f pix] For Source Cross-Match!' %UMatchTol)
+        
+        if self.VERBOSE_LEVEL in [2]:
+            print('MeLOn CheckPoint: Tolerance [%.3f pix] For Source Cross-Match!' %UMatchTol)
+
         _Symm = Symmetric_Match.SM(XY_A=XYr, XY_B=XYs, tol=UMatchTol, return_distance=False)
         AstSEx_Mr = AstSExr[_Symm[:, 0]]
         AstSEx_Ms = AstSExs[_Symm[:, 1]]
 
         # * Determine Magnitude Offset from Matched Sources
         MAG_Mr = np.array(AstSEx_Mr['MAG_AUTO'])
         MAG_Ms = np.array(AstSEx_Ms['MAG_AUTO'])
@@ -370,23 +412,26 @@
 
         MAGD_M = MAG_Ms - MAG_Mr
         MAG_OFFSET0 = np.median(MAGD_M)
 
         NTE_4MO = 30  # NUM_TOP_END for MAG_OFFSET, default value used herein.
         MAG_OFFSETr = TopFlatten_Weighted_Quantile.TFWQ(values=MAGD_M, weights=FLUX_Mr, \
             quantiles=[0.5], NUM_TOP_END=NTE_4MO)[0]
+        
         MAG_OFFSETs = TopFlatten_Weighted_Quantile.TFWQ(values=MAGD_M, weights=FLUX_Ms, \
             quantiles=[0.5], NUM_TOP_END=NTE_4MO)[0]
         MAG_OFFSET = (MAG_OFFSETr + MAG_OFFSETs)/2.0
-
+        
         if np.abs(MAG_OFFSET - MAG_OFFSET0) > 0.05:
-            _warn_message = 'Magnitude Offset Estimate --- HIGHLY DEVIATED FROM DIRECT MEDIAN '
-            _warn_message += '[%.3f mag -> %.3f mag]!' %(MAG_OFFSET0, MAG_OFFSET)
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
-        else:
+            if self.VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'Magnitude Offset Estimate --- HIGHLY DEVIATED FROM DIRECT MEDIAN '
+                _warn_message += '[%.3f mag -> %.3f mag]!' %(MAG_OFFSET0, MAG_OFFSET)
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+
+        if self.VERBOSE_LEVEL in [2]:
             _message = 'Magnitude Offset Estimate --- '
             _message += '[%.3f mag -> %.3f mag]!' %(MAG_OFFSET0, MAG_OFFSET)
             print('\nMeLOn CheckPoint: %s' %_message)
         
         # * Combine catalogs
         for coln in AstSEx_Mr.colnames:
             AstSEx_Mr[coln].name = coln + '_REF'
@@ -405,16 +450,18 @@
         XY_iSS = np.array([AstSEx_iSS['X_IMAGE_REF_SCI_MEAN'], AstSEx_iSS['Y_IMAGE_REF_SCI_MEAN']]).T
         _Symm = Symmetric_Match.SM(XY_A=XY_PriorSelect, XY_B=XY_iSS, tol=UMatchTol, return_distance=False)
         AstSEx_SS = AstSEx_iSS[_Symm[:, 1]]
         
         # record matching and create unified segmentation label
         AstSEx_SS.add_column(Column(_Symm[:, 0], name='INDEX_PRIOR_SELECTION'), index=0)
         AstSEx_SS.add_column(Column(1+np.arange(len(AstSEx_SS)), name='SEGLABEL'), index=0)
-        print('MeLOn CheckPoint: Find / Given [%d / %d] Prior-Selected in [%d] Matched-Sources!' \
-               %(len(AstSEx_SS), XY_PriorSelect.shape[0], len(AstSEx_iSS)))
+
+        if self.VERBOSE_LEVEL in [1, 2]:
+            print('MeLOn CheckPoint: Find / Given [%d / %d] Prior-Selected in [%d] Matched-Sources!' \
+                   %(len(AstSEx_SS), XY_PriorSelect.shape[0], len(AstSEx_iSS)))
         
         # * Run Image Masking (P.S. some SubSources might be marked as invalid by the Prior-Ban list)
         SFFTPrepDict = self.run_image_mask(AstSEx_SS=AstSEx_SS, PixA_SEGr=PixA_SEGr, \
             PixA_SEGs=PixA_SEGs, StarExt_iter=StarExt_iter, XY_PriorBan=XY_PriorBan)
         
         SFFTPrepDict['MAG_OFFSET'] = MAG_OFFSET
         SFFTPrepDict['FWHM_REF'] = FWHM_REF
```

### Comparing `sfft-1.3.4/sfft/CustomizedPacket.py` & `sfft-1.4.0/sfft/CustomizedPacket.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import time
+import cupy as cp
 import numpy as np
 import os.path as pa
 from astropy.io import fits
+from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+# version: Feb 25, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.1"
+__version__ = "v1.4"
 
 class Customized_Packet:
     @staticmethod
     def CP(FITS_REF, FITS_SCI, FITS_mREF, FITS_mSCI, ForceConv, GKerHW, \
         FITS_DIFF=None, FITS_Solution=None, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, \
-        BACKEND_4SUBTRACT='Cupy', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
+        BACKEND_4SUBTRACT='Cupy', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
         
         """
         * Parameters for Customized SFFT
-        # @ Customized: Skip built-in preprocessing (automatic image-masking) 
-        #               by a given customized masked image-pair.
+        # @ Customized: Skip built-in preprocessing (automatic image-masking) by a customized masked image-pair.
         #
         # ----------------------------- Computing Enviornment --------------------------------- #
 
-        -BACKEND_4SUBTRACT ['Cupy']         # can be 'Pycuda', 'Cupy' and 'Numpy'. 
-                                            # Pycuda backend and Cupy backend require GPU device(s), 
-                                            # while 'Numpy' is a pure CPU-based backend for sfft subtraction.
-                                            # Cupy backend is even faster than Pycuda, however, it consume more GPU memory.
-                                            # NOTE: Cupy backend can support CUDA 11*, while Pycuda does not (issues from Scikit-Cuda).
+        -BACKEND_4SUBTRACT ['Cupy']         # 'Cupy' or 'Numpy'.
+                                            # Cupy backend require GPU(s) that is capable of performing double-precision calculations,
+                                            # while Numpy backend is a pure CPU-based backend for sfft subtraction.
+                                            # NOTE: 'Pycuda' backend is no longer supported since sfft v1.4.0.
 
         -CUDA_DEVICE_4SUBTRACT ['0']        # it specifies certain GPU device (index) to conduct the subtraction task.
                                             # the GPU devices are usually numbered 0 to N-1 (you may use command nvidia-smi to check).
                                             # this argument becomes trivial for Numpy backend.
 
         -NUM_CPU_THREADS_4SUBTRACT [8]      # it specifies the number of CPU threads used for sfft subtraction in Numpy backend.
                                             # SFFT in Numpy backend has been implemented with pyFFTW and numba, 
@@ -62,14 +64,19 @@
         -FITS_mSCI []                       # File path of input masked science image (NaN-free).
 
         -FITS_DIFF [None]                   # File path of output difference image.
 
         -FITS_Solution [None]               # File path of the solution of the linear system.
                                             # it is an array of (..., a_ijab, ... b_pq, ...).
 
+        # ----------------------------- Miscellaneous --------------------------------- #
+        
+        -VERBOSE_LEVEL [2]                  # The level of verbosity, can be [0, 1, 2]
+                                            # 0/1/2: QUIET/NORMAL/FULL mode
+
         # Important Notice:
         #
         # a): if reference is convolved in SFFT (-ForceConv='REF'), then DIFF = SCI - Convolved_REF.
         #     [the difference image is expected to have PSF & flux zero-point consistent with science image]
         #
         # b): if science is convolved in SFFT (-ForceConv='SCI'), then DIFF = Convolved_SCI - REF
         #     [the difference image is expected to have PSF & flux zero-point consistent with reference image]
@@ -110,27 +117,34 @@
         assert np.sum(np.isnan(PixA_mREF)) == 0
         assert np.sum(np.isnan(PixA_mSCI)) == 0
         
         assert ForceConv in ['REF', 'SCI']
         ConvdSide = ForceConv
         KerHW = GKerHW
 
+        # * Choose GPU device for Cupy backend
+        if BACKEND_4SUBTRACT == 'Cupy':
+            device = cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT))
+            device.use()
+
         # * Compile Functions in SFFT Subtraction
-        from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER Function Compilations of SFFT-SUBTRACTION!')
 
         Tcomp_start = time.time()
         SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], KerHW=KerHW, \
             KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-            BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, \
-            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
-        print('\nMeLOn Report: Compiling Functions in SFFT Subtraction Takes [%.3f s]' %(time.time() - Tcomp_start))
+            BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, \
+            VERBOSE_LEVEL=VERBOSE_LEVEL)
 
-        # * Perform SFFT Subtraction
-        from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'Function Compilations of SFFT-SUBTRACTION TAKES [%.3f s]' %(time.time() - Tcomp_start)
+            print('\nMeLOn Report: %s' %_message)
 
+        # * Perform SFFT Subtraction
         if ConvdSide == 'REF':
             PixA_mI, PixA_mJ = PixA_mREF, PixA_mSCI
             if NaNmask_U is not None:
                 PixA_I, PixA_J = PixA_REF.copy(), PixA_SCI.copy()
                 PixA_I[NaNmask_U] = PixA_mI[NaNmask_U]
                 PixA_J[NaNmask_U] = PixA_mJ[NaNmask_U]
             else: PixA_I, PixA_J = PixA_REF, PixA_SCI
@@ -139,20 +153,26 @@
             PixA_mI, PixA_mJ = PixA_mSCI, PixA_mREF
             if NaNmask_U is not None:
                 PixA_I, PixA_J = PixA_SCI.copy(), PixA_REF.copy()
                 PixA_I[NaNmask_U] = PixA_mI[NaNmask_U]
                 PixA_J[NaNmask_U] = PixA_mJ[NaNmask_U]
             else: PixA_I, PixA_J = PixA_SCI, PixA_REF
         
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER SFFT-SUBTRACTION!')
+
         Tsub_start = time.time()
         _tmp = GeneralSFFTSubtract.GSS(PixA_I=PixA_I, PixA_J=PixA_J, PixA_mI=PixA_mI, PixA_mJ=PixA_mJ, \
             SFFTConfig=SFFTConfig, ContamMask_I=None, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-            CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
+            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)
+
         Solution, PixA_DIFF = _tmp[:2]
-        print('\nMeLOn Report: SFFT Subtraction Takes [%.3f s]' %(time.time() - Tsub_start))
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'SFFT-SUBTRACTION TAKES [%.3f s]' %(time.time() - Tsub_start)
+            print('\nMeLOn Report: %s' %_message)
         
         # * Modifications on the difference image
         #   a) when REF is convolved, DIFF = SCI - Conv(REF)
         #      PSF(DIFF) is coincident with PSF(SCI), transients on SCI are positive signal in DIFF.
         #   b) when SCI is convolved, DIFF = Conv(SCI) - REF
         #      PSF(DIFF) is coincident with PSF(REF), transients on SCI are still positive signal in DIFF.
 
@@ -169,15 +189,15 @@
             _hdl[0].data[:, :] = PixA_DIFF.T
             _hdl[0].header['NAME_REF'] = (pa.basename(FITS_REF), 'MeLOn: SFFT')
             _hdl[0].header['NAME_SCI'] = (pa.basename(FITS_SCI), 'MeLOn: SFFT')
             _hdl[0].header['KERORDER'] = (KerPolyOrder, 'MeLOn: SFFT')
             _hdl[0].header['BGORDER'] = (BGPolyOrder, 'MeLOn: SFFT')
             _hdl[0].header['CPHOTR'] = (str(ConstPhotRatio), 'MeLOn: SFFT')
             _hdl[0].header['KERHW'] = (KerHW, 'MeLOn: SFFT')
-            _hdl[0].header['CONVD'] = (ConvdSide  , 'MeLOn: SFFT')
+            _hdl[0].header['CONVD'] = (ConvdSide, 'MeLOn: SFFT')
             _hdl.writeto(FITS_DIFF, overwrite=True)
             _hdl.close()
         
         # * Save solution array
         if FITS_Solution is not None:
             phdu = fits.PrimaryHDU()
             phdu.header['N0'] = (SFFTConfig[0]['N0'], 'MeLOn: SFFT')
```

### Comparing `sfft-1.3.4/sfft/EasyCrowdedPacket.py` & `sfft-1.4.0/sfft/EasyCrowdedPacket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import time
+import cupy as cp
 import numpy as np
 import os.path as pa
 from astropy.io import fits
 from sfft.AutoCrowdedPrep import Auto_CrowdedPrep
-# version: Sep 16, 2022
+from sfft.utils.SFFTSolutionReader import Realize_FluxScaling
+from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+# version: Feb 25, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.2"
+__version__ = "v1.4"
 
 class Easy_CrowdedPacket:
     @staticmethod
-    def ECP(FITS_REF, FITS_SCI, FITS_DIFF=None, FITS_Solution=None, ForceConv='AUTO', \
-        GKerHW=None, KerHWRatio=2.0, KerHWLimit=(2, 20), KerPolyOrder=2, BGPolyOrder=2, \
-        ConstPhotRatio=True, MaskSatContam=False, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', \
-        BACK_TYPE='AUTO', BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=5.0, \
+    def ECP(FITS_REF, FITS_SCI, FITS_DIFF=None, FITS_Solution=None, ForceConv='AUTO', GKerHW=None, \
+        KerHWRatio=2.0, KerHWLimit=(2, 20), KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, \
+        MaskSatContam=False, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', BACK_TYPE='AUTO', \
+        BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=5.0, ANALYSIS_THRESH=5.0, \
         DETECT_MINAREA=5, DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', \
         ONLY_FLAGS=None, BoundarySIZE=0.0, BACK_SIZE_SUPER=128, StarExt_iter=2, PriorBanMask=None, \
-        BACKEND_4SUBTRACT='Cupy', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
-
+        BACKEND_4SUBTRACT='Cupy', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
+        
         """
         # NOTE: This function is to Perform Crowded-Flavor SFFT for single task:
-        #       Pycuda & Cupy backend: do preprocessing on one CPU thread, and do subtraction on one GPU device.
-        #       Numpy backend: do preprocessing on one CPU thread, and do subtraction with pyFFTW and Numba 
+        #       Cupy backend: do preprocessing on one CPU thread, and perform subtraction on one GPU device.
+        #       Numpy backend: do preprocessing on one CPU thread, and perform subtraction with pyFFTW and Numba 
         #                      using multiple threads (-NUM_CPU_THREADS_4SUBTRACT).
         
         * Parameters for Crowded-Flavor SFFT [single task]
         
         # ----------------------------- Computing Enviornment --------------------------------- #
 
-        -BACKEND_4SUBTRACT ['Cupy']         # can be 'Pycuda', 'Cupy' and 'Numpy'. 
-                                            # Pycuda backend and Cupy backend require GPU device(s), 
-                                            # while 'Numpy' is a pure CPU-based backend for sfft subtraction.
-                                            # Cupy backend is even faster than Pycuda, however, it consume more GPU memory.
-                                            # NOTE: Cupy backend can support CUDA 11*, while Pycuda does not (issues from Scikit-Cuda).
+        -BACKEND_4SUBTRACT ['Cupy']         # 'Cupy' or 'Numpy'. 
+                                            # Cupy backend require GPU(s) that is capable of performing double-precision calculations,
+                                            # while Numpy backend is a pure CPU-based backend for sfft subtraction.
+                                            # NOTE: 'Pycuda' backend is no longer supported since sfft v1.4.0.
 
         -CUDA_DEVICE_4SUBTRACT ['0']        # it specifies certain GPU device (index) to conduct the subtraction task.
                                             # the GPU devices are usually numbered 0 to N-1 (you may use command nvidia-smi to check).
                                             # this argument becomes trivial for Numpy backend.
 
         -NUM_CPU_THREADS_4SUBTRACT [8]      # it specifies the number of CPU threads used for sfft subtraction in Numpy backend.
                                             # SFFT in Numpy backend has been implemented with pyFFTW and numba, 
@@ -65,14 +68,17 @@
 
         -DETECT_THRESH [5.0]                # SExtractor Parameter DETECT_THRESH
                                             # NOTE: One may notice that the default DETECT_THRESH in SExtractor is 1.5.
                                             #       Using a 'very cold' detection threshold here is to speed up SExtractor.
                                             #       Although DETECT_THRESH = 5.0 means we will miss the faint-end sources with 
                                             #       SNR < 20 (approximately), the cost is generally acceptable for saturation mask.
 
+        -ANALYSIS_THRESH [5.0]              # SExtractor Parameter ANALYSIS_THRESH
+                                            # NOTE: By default, let -ANALYSIS_THRESH = -DETECT_THRESH
+
         -DETECT_MINAREA [5]                 # SExtractor Parameter DETECT_MINAREA
         
         -DETECT_MAXAREA [0]                 # SExtractor Parameter DETECT_MAXAREA
 
         -DEBLEND_MINCONT [0.005]            # SExtractor Parameter DEBLEND_MINCONT (typically, 0.001 - 0.005)
 
         -BACKPHOTO_TYPE ['LOCAL']           # SExtractor Parameter BACKPHOTO_TYPE
@@ -140,36 +146,47 @@
 
         -FITS_SCI []                        # File path of input science image.
 
         -FITS_DIFF [None]                   # File path of output difference image.
 
         -FITS_Solution [None]               # File path of the solution of the linear system. 
                                             # it is an array of (..., a_ijab, ... b_pq, ...).
+        
+        # ----------------------------- Miscellaneous --------------------------------- #
+        
+        -VERBOSE_LEVEL [2]                  # The level of verbosity, can be [0, 1, 2]
+                                            # 0/1/2: QUIET/NORMAL/FULL mode
 
         # Important Notice:
         #
         # a): if reference is convolved in SFFT, then DIFF = SCI - Convolved_REF.
         #     [difference image is expected to have PSF & flux zero-point consistent with science image]
         #     e.g., -ForceConv='REF' or -ForceConv='AUTO' when reference has better seeing.
         #
         # b): if science is convolved in SFFT, then DIFF = Convolved_SCI - REF
         #     [difference image is expected to have PSF & flux zero-point consistent with reference image]
         #     e.g., -ForceConv='SCI' or -ForceConv='AUTO' when science has better seeing.
         #
-        # Remarks: this convention is to guarantee that transients emerge on science image always 
-        #          show a positive signal on difference images.
+        # Remarks: this convention is to guarantee that a transient emerge on science image 
+        #          always shows itself as a positive signal on the difference images.
 
         """
 
         # * Perform Auto Crowded-Prep [Mask Saturation]
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER Crowded-Flavor Auto Preprocessing!')
+
         _ACP = Auto_CrowdedPrep(FITS_REF=FITS_REF, FITS_SCI=FITS_SCI, GAIN_KEY=GAIN_KEY, SATUR_KEY=SATUR_KEY, \
             BACK_TYPE=BACK_TYPE, BACK_VALUE=BACK_VALUE, BACK_SIZE=BACK_SIZE, BACK_FILTERSIZE=BACK_FILTERSIZE, \
-            DETECT_THRESH=DETECT_THRESH, DETECT_MINAREA=DETECT_MINAREA, DETECT_MAXAREA=DETECT_MAXAREA, \
-            DEBLEND_MINCONT=DEBLEND_MINCONT, BACKPHOTO_TYPE=BACKPHOTO_TYPE, ONLY_FLAGS=ONLY_FLAGS, BoundarySIZE=BoundarySIZE)
-        SFFTPrepDict = _ACP.AutoMask(BACK_SIZE_SUPER=BACK_SIZE_SUPER, StarExt_iter=StarExt_iter, PriorBanMask=PriorBanMask)
+            DETECT_THRESH=DETECT_THRESH, ANALYSIS_THRESH=ANALYSIS_THRESH, DETECT_MINAREA=DETECT_MINAREA, \
+            DETECT_MAXAREA=DETECT_MAXAREA, DEBLEND_MINCONT=DEBLEND_MINCONT, BACKPHOTO_TYPE=BACKPHOTO_TYPE, \
+            ONLY_FLAGS=ONLY_FLAGS, BoundarySIZE=BoundarySIZE, VERBOSE_LEVEL=VERBOSE_LEVEL)
+
+        SFFTPrepDict = _ACP.AutoMask(BACK_SIZE_SUPER=BACK_SIZE_SUPER, \
+            StarExt_iter=StarExt_iter, PriorBanMask=PriorBanMask)
 
         # * Determine ConvdSide & KerHW
         FWHM_REF = SFFTPrepDict['FWHM_REF']
         FWHM_SCI = SFFTPrepDict['FWHM_SCI']
 
         assert ForceConv in ['AUTO', 'REF', 'SCI']
         if ForceConv == 'AUTO':
@@ -178,30 +195,37 @@
         else: ConvdSide = ForceConv
 
         if GKerHW is None:
             FWHM_La = np.max([FWHM_REF, FWHM_SCI])
             KerHW = int(np.clip(KerHWRatio * FWHM_La, KerHWLimit[0], KerHWLimit[1]))
         else: KerHW = GKerHW
 
-        # * Compile Functions in SFFT Subtraction
-        from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+        # * Choose GPU device for Cupy backend
+        if BACKEND_4SUBTRACT == 'Cupy':
+            device = cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT))
+            device.use()
 
+        # * Compile Functions in SFFT Subtraction
         PixA_REF = SFFTPrepDict['PixA_REF']
         PixA_SCI = SFFTPrepDict['PixA_SCI']
         
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER Function Compilations of SFFT-SUBTRACTION!')
+
         Tcomp_start = time.time()
         SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], KerHW=KerHW, \
             KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-            BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, \
-            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
-        print('\nMeLOn Report: Compiling Functions in SFFT Subtraction Takes [%.3f s]' %(time.time() - Tcomp_start))
+            BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, \
+            VERBOSE_LEVEL=VERBOSE_LEVEL)
 
-        # * Perform SFFT Subtraction
-        from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'Function Compilations of SFFT-SUBTRACTION TAKES [%.3f s]' %(time.time() - Tcomp_start)
+            print('\nMeLOn Report: %s' %_message)
 
+        # * Perform SFFT Subtraction
         SatMask_REF = SFFTPrepDict['REF-SAT-Mask']
         SatMask_SCI = SFFTPrepDict['SCI-SAT-Mask']
         NaNmask_U = SFFTPrepDict['Union-NaN-Mask']
         PixA_mREF = SFFTPrepDict['PixA_mREF']
         PixA_mSCI = SFFTPrepDict['PixA_mSCI']
 
         if ConvdSide == 'REF':
@@ -224,66 +248,151 @@
                 PixA_J[NaNmask_U] = PixA_mJ[NaNmask_U]
             else: PixA_I, PixA_J = PixA_SCI, PixA_REF
             if MaskSatContam: 
                 ContamMask_I = SatMask_SCI
                 ContamMask_J = SatMask_REF
             else: ContamMask_I = None
         
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER SFFT-SUBTRACTION!')
+
         Tsub_start = time.time()
         _tmp = GeneralSFFTSubtract.GSS(PixA_I=PixA_I, PixA_J=PixA_J, PixA_mI=PixA_mI, PixA_mJ=PixA_mJ, \
             SFFTConfig=SFFTConfig, ContamMask_I=ContamMask_I, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-            CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
+            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)
+
         Solution, PixA_DIFF, ContamMask_CI = _tmp
-        if MaskSatContam:
-            ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
-        print('\nMeLOn Report: SFFT Subtraction Takes [%.3f s]' %(time.time() - Tsub_start))
-        
-        # * Modifications on the difference image
-        #   a) when REF is convolved, DIFF = SCI - Conv(REF)
-        #      PSF(DIFF) is coincident with PSF(SCI), transients on SCI are positive signal in DIFF.
-        #   b) when SCI is convolved, DIFF = Conv(SCI) - REF
-        #      PSF(DIFF) is coincident with PSF(REF), transients on SCI are still positive signal in DIFF.
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'SFFT-SUBTRACTION TAKES [%.3f s]' %(time.time() - Tsub_start)
+            print('\nMeLOn Report: %s' %_message)
+        
+        # ** adjust the sign of difference image 
+        #    NOTE: Our convention is to make the transients on SCI always show themselves as positive signal on DIFF
+        #    (a) when REF is convolved, DIFF = SCI - Conv(REF)
+        #    (b) when SCI is convolved, DIFF = Conv(SCI) - REF
 
-        if NaNmask_U is not None:
-            # ** Mask Union-NaN region
-            PixA_DIFF[NaNmask_U] = np.nan
-        if MaskSatContam:
-            # ** Mask Saturate-Contaminate region 
-            PixA_DIFF[ContamMask_DIFF] = np.nan
-        if ConvdSide == 'SCI': 
-            # ** Flip difference when science is convolved
+        if ConvdSide == 'SCI':
             PixA_DIFF = -PixA_DIFF
+
+        if VERBOSE_LEVEL in [1, 2]:
+            if ConvdSide == 'REF':
+                _message = 'Reference Image is Convolved in SFFT-SUBTRACTION [DIFF = SCI - Conv(REF)]!'
+                print('MeLOn CheckPoint: %s' %_message)
+
+            if ConvdSide == 'SCI':
+                _message = 'Science Image is Convolved in SFFT-SUBTRACTION [DIFF = Conv(SCI) - REF]!'
+                print('MeLOn CheckPoint: %s' %_message)
+
+        # ** estimate the flux scaling through the convolution of image subtraction
+        #    NOTE: if photometric ratio is not constant (ConstPhotRatio=False), we measure of a grid
+        #          of coordinates to estimate the flux scaling and its fluctuation (polynomial form).
+        #    NOTE: here we set the tile-size of the grid about 64 x 64 pix, but meanwhile, 
+        #          we also require the tiles should no less than 6 along each axis.
+
+        N0, N1 = SFFTConfig[0]['N0'], SFFTConfig[0]['N1']
+        L0, L1 = SFFTConfig[0]['L0'], SFFTConfig[0]['L1']
+        DK, Fpq = SFFTConfig[0]['DK'], SFFTConfig[0]['Fpq']
+
+        if ConstPhotRatio:
+            SFFT_FSCAL_NSAMP = 1
+            XY_q = np.array([[N0/2.0, N1/2.0]]) + 0.5
+            RFS = Realize_FluxScaling(XY_q=XY_q)
+            SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+            SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = SFFT_FSCAL_q[0], 0.0
+        
+        if not ConstPhotRatio:
+            TILESIZE_X, TILESIZE_Y = 64, 64    # FIXME emperical/arbitrary values
+            NTILE_X = np.max([round(N0/TILESIZE_X), 6])
+            NTILE_Y = np.max([round(N1/TILESIZE_Y), 6])
+            GX = np.linspace(0.5, N0+0.5, NTILE_X+1)
+            GY = np.linspace(0.5, N1+0.5, NTILE_Y+1)
+            YY, XX = np.meshgrid(GY, GX)
+            XY_q = np.array([XX.flatten(), YY.flatten()]).T
+            SFFT_FSCAL_NSAMP = XY_q.shape[0]
+            
+            RFS = Realize_FluxScaling(XY_q=XY_q)
+            SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+            SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = np.mean(SFFT_FSCAL_q), np.std(SFFT_FSCAL_q)
+        
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'The Flux Scaling through the Convolution of SFFT-SUBTRACTION '
+            _message += '[%.6f +/- %.6f] from [%d] positions!\n' %(SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG, SFFT_FSCAL_NSAMP)
+            print('MeLOn CheckPoint: %s' %_message)
         
+        # ** final tweaks on the difference image
+        if NaNmask_U is not None:
+            PixA_DIFF[NaNmask_U] = np.nan   # Mask Union-NaN regions
+        
+        if MaskSatContam:
+            ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
+            PixA_DIFF[ContamMask_DIFF] = np.nan   # Mask Saturation-Contaminated regions
+
         # * Save difference image
         if FITS_DIFF is not None:
+
+            """
+            # Remarks on header of difference image
+            # [1] In general, the FITS header of difference image would mostly be inherited from science image.
+            #
+            # [2] when science image is convolved, we turn to set GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN (unit: e-/ADU)
+            #     so that one can correctly convert ADU to e- for a transient appears on science image.
+            #     WARNING: for a transient appears on reference image, GAIN_DIFF = GAIN_SCI is correct.
+            #              we should keep in mind that GAIN_DIFF is not an absolute instrumental value.
+            #     WARNING: one can only estimate the Poission noise from the science transient via GIAN_DIFF.
+            #              the Poission noise from the background source (host galaxy) can enhance the 
+            #              background noise at the position of the transient. photometry softwares which 
+            #              only take background noise and transient Possion noise into account would tend 
+            #              to overestimate the SNR of the transient.
+            # 
+            # [3] when science image is convolved, we turn to set SATURA_DIFF = SATURA_SCI * SFFT_FSCAL_MEAN         
+            #     WARNING: it is still not a good idea to use SATURA_DIFF to identify the SATURATION regions
+            #              on difference image. more appropriate way is masking the saturation contaminated 
+            #              regions on difference image (MaskSatContam=True), or alternatively, leave them  
+            #              alone and using AI stamp classifier to reject saturation-related bogus.
+            #
+            """
+
             _hdl = fits.open(FITS_SCI)
             _hdl[0].data[:, :] = PixA_DIFF.T
+
             _hdl[0].header['NAME_REF'] = (pa.basename(FITS_REF), 'MeLOn: SFFT')
             _hdl[0].header['NAME_SCI'] = (pa.basename(FITS_SCI), 'MeLOn: SFFT')
             _hdl[0].header['FWHM_REF'] = (FWHM_REF, 'MeLOn: SFFT')
             _hdl[0].header['FWHM_SCI'] = (FWHM_SCI, 'MeLOn: SFFT')
             _hdl[0].header['KERORDER'] = (KerPolyOrder, 'MeLOn: SFFT')
             _hdl[0].header['BGORDER'] = (BGPolyOrder, 'MeLOn: SFFT')
             _hdl[0].header['CPHOTR'] = (str(ConstPhotRatio), 'MeLOn: SFFT')
             _hdl[0].header['KERHW'] = (KerHW, 'MeLOn: SFFT')
-            _hdl[0].header['CONVD'] = (ConvdSide  , 'MeLOn: SFFT')
+            _hdl[0].header['CONVD'] = (ConvdSide, 'MeLOn: SFFT')
+
+            if ConvdSide == 'SCI':
+                GAIN_SCI = _hdl[0].header[GAIN_KEY]
+                SATUR_SCI = _hdl[0].header[SATUR_KEY]
+                GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN
+                SATUR_DIFF = SATUR_SCI * SFFT_FSCAL_MEAN
+
+                _hdl[0].header[GAIN_KEY] = (GAIN_DIFF, 'MeLOn: SFFT')
+                _hdl[0].header[SATUR_KEY] = (SATUR_DIFF, 'MeLOn: SFFT')
+
             _hdl.writeto(FITS_DIFF, overwrite=True)
             _hdl.close()
         
         # * Save solution array
         if FITS_Solution is not None:
             phdu = fits.PrimaryHDU()
+            phdu.header['N0'] = (SFFTConfig[0]['N0'], 'MeLOn: SFFT')
+            phdu.header['N1'] = (SFFTConfig[0]['N1'], 'MeLOn: SFFT')
             phdu.header['DK'] = (SFFTConfig[0]['DK'], 'MeLOn: SFFT')
             phdu.header['DB'] = (SFFTConfig[0]['DB'], 'MeLOn: SFFT')
             phdu.header['L0'] = (SFFTConfig[0]['L0'], 'MeLOn: SFFT')
             phdu.header['L1'] = (SFFTConfig[0]['L1'], 'MeLOn: SFFT')
             
             phdu.header['FIJ'] = (SFFTConfig[0]['Fij'], 'MeLOn: SFFT')
             phdu.header['FAB'] = (SFFTConfig[0]['Fab'], 'MeLOn: SFFT')
             phdu.header['FPQ'] = (SFFTConfig[0]['Fpq'], 'MeLOn: SFFT')
             phdu.header['FIJAB'] = (SFFTConfig[0]['Fijab'], 'MeLOn: SFFT')
 
             PixA_Solution = Solution.reshape((-1, 1))
             phdu.data = PixA_Solution.T
             fits.HDUList([phdu]).writeto(FITS_Solution, overwrite=True)
-        
-        return SFFTPrepDict, Solution, PixA_DIFF
+
+        return PixA_DIFF, SFFTPrepDict, Solution, SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG
```

### Comparing `sfft-1.3.4/sfft/EasySparsePacket.py` & `sfft-1.4.0/sfft/EasySparsePacket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 import time
 import warnings
+import cupy as cp
 import numpy as np
 import os.path as pa
 from astropy.io import fits
 import scipy.ndimage as ndimage
 from astropy.table import Column
 from sfft.AutoSparsePrep import Auto_SparsePrep
-# version: Aug 31, 2022
+from sfft.utils.SFFTSolutionReader import Realize_FluxScaling
+from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+# version: Mar 18, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class Easy_SparsePacket:
     @staticmethod
     def ESP(FITS_REF, FITS_SCI, FITS_DIFF=None, FITS_Solution=None, ForceConv='AUTO', GKerHW=None, \
         KerHWRatio=2.0, KerHWLimit=(2, 20), KerPolyOrder=2, BGPolyOrder=0, ConstPhotRatio=True, \
         MaskSatContam=False, GAIN_KEY='GAIN', SATUR_KEY='ESATUR', BACK_TYPE='MANUAL', BACK_VALUE=0.0, \
-        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=2.0, DETECT_MINAREA=5, DETECT_MAXAREA=0, \
-        DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=[0], BoundarySIZE=30, \
-        XY_PriorSelect=None, Hough_FRLowerLimit=0.1, Hough_peak_clip=0.7, BeltHW=0.2, PS_ELLIPThresh=0.3, \
+        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=2.0, ANALYSIS_THRESH=2.0, DETECT_MINAREA=5, \
+        DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=[0], BoundarySIZE=30, \
+        XY_PriorSelect=None, Hough_MINFR=0.1, Hough_PeakClip=0.7, BeltHW=0.2, PointSource_MINELLIP=0.3, \
         MatchTol=None, MatchTolFactor=3.0, COARSE_VAR_REJECTION=True, CVREJ_MAGD_THRESH=0.12, \
         ELABO_VAR_REJECTION=True, EVREJ_RATIO_THREH=5.0, EVREJ_SAFE_MAGDEV=0.04, StarExt_iter=4, \
         XY_PriorBan=None, PostAnomalyCheck=False, PAC_RATIO_THRESH=5.0, BACKEND_4SUBTRACT='Cupy', \
-        CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
+        CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
         
         """
         # NOTE: This function is to Perform Sparse-Flavor SFFT for a single task:
-        #       Pycuda & Cupy backend: do preprocessing on one CPU thread, and do subtraction on one GPU device.
-        #       Numpy backend: do preprocessing on one CPU thread, and do subtraction with pyFFTW and Numba 
+        #       Cupy backend: do preprocessing on one CPU thread, and perform subtraction on one GPU device.
+        #       Numpy backend: do preprocessing on one CPU thread, and perform subtraction with pyFFTW and Numba 
         #                      using multiple threads (-NUM_CPU_THREADS_4SUBTRACT).
 
         * Parameters for Sparse-Flavor SFFT [single task]
 
         # ----------------------------- Computing Enviornment --------------------------------- #
 
-        -BACKEND_4SUBTRACT ['Cupy']     # can be 'Pycuda', 'Cupy' and 'Numpy'. 
-                                        # Pycuda backend and Cupy backend require GPU device(s), 
-                                        # while 'Numpy' is a pure CPU-based backend for sfft subtraction.
-                                        # Cupy backend is even faster than Pycuda, however, it consume more GPU memory.
-                                        # NOTE: Cupy backend can support CUDA 11*, while Pycuda does not (issues from Scikit-Cuda).
-
+        -BACKEND_4SUBTRACT ['Cupy']     # 'Cupy' or 'Numpy'. 
+                                        # Cupy backend require GPU(s) that is capable of performing double-precision calculations,
+                                        # while Numpy backend is a pure CPU-based backend for sfft subtraction.
+                                        # NOTE: 'Pycuda' backend is no longer supported since sfft v1.4.0.
+        
         -CUDA_DEVICE_4SUBTRACT ['0']    # it specifies certain GPU device (index) to conduct the subtraction task.
                                         # the GPU devices are usually numbered 0 to N-1 (you may use command nvidia-smi to check).
                                         # this argument becomes trivial for Numpy backend.
 
         -NUM_CPU_THREADS_4SUBTRACT [8]  # it specifies the number of CPU threads used for sfft subtraction in Numpy backend.
                                         # SFFT in Numpy backend has been implemented with pyFFTW and numba, 
                                         # that allow for parallel computing on CPUs. Of course, the Numpy 
@@ -79,14 +82,17 @@
 
         -DETECT_THRESH [2.0]           # SExtractor Parameter DETECT_THRESH
                                        # NOTE: One may notice that the default DETECT_THRESH in SExtractor is 1.5,
                                        #       Using a 'cold' detection threshold here is to speed up SExtractor.
                                        #       Although DETECT_THRESH = 2.0 means we will miss the faint-end sources with 
                                        #       SNR < 9 (approximately), the cost is generally acceptable for source selection.
 
+        -ANALYSIS_THRESH [2.0]         # SExtractor Parameter ANALYSIS_THRESH
+                                       # NOTE: By default, let -ANALYSIS_THRESH = -DETECT_THRESH
+
         -DETECT_MINAREA [5]            # SExtractor Parameter DETECT_MINAREA
         
         -DETECT_MAXAREA [0]            # SExtractor Parameter DETECT_MAXAREA
 
         -DEBLEND_MINCONT [0.005]       # SExtractor Parameter DEBLEND_MINCONT (typically, 0.001 - 0.005)
 
         -BACKPHOTO_TYPE ['LOCAL']      # SExtractor Parameter BACKPHOTO_TYPE
@@ -98,36 +104,42 @@
                                        # 2: the object has been deblended
                                        # 4: at least one object pixel is saturated
 
         -BoundarySIZE [30]             # Restrict SExtractor Output Photometry Catalog by Dropping Sources at Boundary 
                                        # NOTE: This would help to avoid selecting sources too close to image boundary. 
 
         # > Configurations for Source-Selction
+        #
+        # Remarks on two modes 
+        #   [HOUGH-AUTO] MODE: Source-Selection based on SExtractor & Hough Transformation, following Hu, et al. (2022).
+        #   [SEMI-AUTO] MODE:  Source-Selection directly make use of a prior-selected source list.
+        #
 
         -XY_PriorSelect [None]         # a Numpy array of pixels coordinates, with shape (N, 2) (e.g., [[x0, y0], [x1, y1], ...])
                                        # this allows sfft to us a prior source selection to solve the subtraction.
                                        # NOTE: ONLY WORKS FOR Auto-Sparse-Prep [SEMI-AUTO] MODE
 
-        -Hough_FRLowerLimit [0.1]      # The lower bound of FLUX_RATIO for line feature detection using Hough transformation.
+        -Hough_MINFR [0.1]             # The lower bound of FLUX_RATIO for line feature detection using Hough transformation.
                                        # Setting a proper lower bound can avoid to detect some line features by chance,
                                        # which are not contributed from point sources but resides in the small-FLUX_RATIO region.
-                                       # NOTE: Recommended values of Hough_FRLowerLimit: 0.1 ~ 1.0
+                                       # NOTE: Recommended values of Hough_MINFR: 0.1 ~ 1.0
                                        # NOTE: ONLY WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE
 
-        -Hough_peak_clip [0.7]         # It determines the lower bound of the sensitivity of the line feature detection.
+        -Hough_PeakClip [0.7]          # It determines the lower bound of the sensitivity of the line feature detection.
                                        # NOTE: When the point-source-belt is not very pronounced (e.g., in galaxy dominated fields),
                                        #       one may consider to reduce the parameter from default 0.7 to, says, ~ 0.4.
                                        # NOTE: ONLY WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE
     
         -BeltHW [0.2]                  # The half-width of point-source-belt detected by Hough Transformation.
                                        # Remarks: if you want to tune this parameter, it is helpful to draw 
                                        #          a figure of MAG_AUTO against FLUX_RADIUS.
                                        # NOTE: IT WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE :::: determine point-source-belt
 
-        -PS_ELLIPThresh [0.3]          # An additiona Restriction on ELLIPTICITY (ELLIPTICITY < PS_ELLIPThresh) for point sources.
+        -PointSource_MINELLIP [0.3]    # An additiona Restriction on ELLIPTICITY (ELLIPTICITY < PointSource_MINELLIP) 
+                                       # for point sources.
                                        # NOTE: IT WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE :::: determine point-sources
 
         -MatchTol [None]               # Given separation tolerance (pix) for source matching 
                                        # NOTE: IT WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE :::: Cross-Match between REF & SCI
                                        # NOTE: IT WORKS FOR Auto-Sparse-Prep [SEMI-AUTO] MODE :::: Cross-Match between REF & SCI AND
                                        #       Cross-Match between the prior selection and mean image coordinates of matched REF-SCI sources.
 
@@ -241,48 +253,59 @@
         -FITS_SCI []                # File path of input science image
 
         -FITS_DIFF [None]           # File path of output difference image
 
         -FITS_Solution [None]       # File path of the solution of the linear system 
                                     # it is an array of (..., a_ijab, ... b_pq, ...)
 
+        # ----------------------------- Miscellaneous --------------------------------- #
+        
+        -VERBOSE_LEVEL [2]          # The level of verbosity, can be [0, 1, 2]
+                                    # 0/1/2: QUIET/NORMAL/FULL mode
+
         # Important Notice:
         #
         # a): if reference is convolved in SFFT, then DIFF = SCI - Convolved_REF.
         #     [difference image is expected to have PSF & flux zero-point consistent with science image]
         #     e.g., -ForceConv='REF' or -ForceConv='AUTO' when reference has better seeing.
         #
         # b): if science is convolved in SFFT, then DIFF = Convolved_SCI - REF
         #     [difference image is expected to have PSF & flux zero-point consistent with reference image]
         #     e.g., -ForceConv='SCI' or -ForceConv='AUTO' when science has better seeing.
         #
-        # Remarks: this convention is to guarantee that transients emerge on science image always 
-        #          show a positive signal on difference images.
+        # Remarks: this convention is to guarantee that a transient emerge on science image 
+        #          always shows itself as a positive signal on the difference images.
 
         """
         
         # * Perform Auto Sparse-Prep
-        warnings.warn('\nMeLOn WARNING: Input images for sparse-flavor sfft should be SKY-SUBTRACTED !!!')
+        if VERBOSE_LEVEL in [2]:
+            warnings.warn('\nMeLOn REMINDER: Input images for sparse-flavor sfft should be SKY-SUBTRACTED!')
+        
         _ASP = Auto_SparsePrep(FITS_REF=FITS_REF, FITS_SCI=FITS_SCI, GAIN_KEY=GAIN_KEY, SATUR_KEY=SATUR_KEY, \
             BACK_TYPE=BACK_TYPE, BACK_VALUE=BACK_VALUE, BACK_SIZE=BACK_SIZE, BACK_FILTERSIZE=BACK_FILTERSIZE, \
-            DETECT_THRESH=DETECT_THRESH, DETECT_MINAREA=DETECT_MINAREA, DETECT_MAXAREA=DETECT_MAXAREA, \
-            DEBLEND_MINCONT=DEBLEND_MINCONT, BACKPHOTO_TYPE=BACKPHOTO_TYPE, \
-            ONLY_FLAGS=ONLY_FLAGS, BoundarySIZE=BoundarySIZE)
+            DETECT_THRESH=DETECT_THRESH, ANALYSIS_THRESH=ANALYSIS_THRESH, DETECT_MINAREA=DETECT_MINAREA, \
+            DETECT_MAXAREA=DETECT_MAXAREA, DEBLEND_MINCONT=DEBLEND_MINCONT, BACKPHOTO_TYPE=BACKPHOTO_TYPE, \
+            ONLY_FLAGS=ONLY_FLAGS, BoundarySIZE=BoundarySIZE, VERBOSE_LEVEL=VERBOSE_LEVEL)
 
         if XY_PriorSelect is None:
             IMAGE_MASK_METHOD = 'HOUGH-AUTO'
-            print('MeLOn CheckPoint: TRIGGER Auto-Sparse-Prep [%s] MODE!' %IMAGE_MASK_METHOD)
-            SFFTPrepDict = _ASP.HoughAutoMask(Hough_FRLowerLimit=Hough_FRLowerLimit, Hough_peak_clip=Hough_peak_clip, \
-                BeltHW=BeltHW, PS_ELLIPThresh=PS_ELLIPThresh, MatchTol=MatchTol, MatchTolFactor=MatchTolFactor, \
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                print('MeLOn CheckPoint: TRIGGER Sparse-Flavor Auto Preprocessing [%s] MODE!' %IMAGE_MASK_METHOD)
+
+            SFFTPrepDict = _ASP.HoughAutoMask(Hough_MINFR=Hough_MINFR, Hough_PeakClip=Hough_PeakClip, \
+                BeltHW=BeltHW, PointSource_MINELLIP=PointSource_MINELLIP, MatchTol=MatchTol, MatchTolFactor=MatchTolFactor, \
                 COARSE_VAR_REJECTION=COARSE_VAR_REJECTION, CVREJ_MAGD_THRESH=CVREJ_MAGD_THRESH, \
                 ELABO_VAR_REJECTION=ELABO_VAR_REJECTION, EVREJ_RATIO_THREH=EVREJ_RATIO_THREH, \
                 EVREJ_SAFE_MAGDEV=EVREJ_SAFE_MAGDEV, StarExt_iter=StarExt_iter, XY_PriorBan=XY_PriorBan)
         else:
             IMAGE_MASK_METHOD = 'SEMI-AUTO'
-            print('MeLOn CheckPoint: TRIGGER Auto-Sparse-Prep [%s] MODE!' %IMAGE_MASK_METHOD)
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                print('MeLOn CheckPoint: TRIGGER Sparse-Flavor Auto Preprocessing [%s] MODE!' %IMAGE_MASK_METHOD)
+            
             SFFTPrepDict = _ASP.SemiAutoMask(XY_PriorSelect=XY_PriorSelect, MatchTol=MatchTol, \
                 MatchTolFactor=MatchTolFactor, StarExt_iter=StarExt_iter, XY_PriorBan=XY_PriorBan)
 
         # * Determine ConvdSide & KerHW
         FWHM_REF = SFFTPrepDict['FWHM_REF']
         FWHM_SCI = SFFTPrepDict['FWHM_SCI']
 
@@ -293,30 +316,38 @@
         else: ConvdSide = ForceConv
 
         if GKerHW is None:
             FWHM_La = np.max([FWHM_REF, FWHM_SCI])
             KerHW = int(np.clip(KerHWRatio * FWHM_La, KerHWLimit[0], KerHWLimit[1]))
         else: KerHW = GKerHW
 
+        # * Choose GPU device for Cupy backend
+        if BACKEND_4SUBTRACT == 'Cupy':
+            device = cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT))
+            device.use()
+        
         # * Compile Functions in SFFT Subtraction
-        from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
-
         PixA_REF = SFFTPrepDict['PixA_REF']
         PixA_SCI = SFFTPrepDict['PixA_SCI']
 
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER Function Compilations of SFFT-SUBTRACTION!')
+
         Tcomp_start = time.time()
         SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], KerHW=KerHW, \
             KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-            BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, \
-            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
-        print('\nMeLOn Report: Compiling Functions in SFFT Subtraction Takes [%.3f s]' %(time.time() - Tcomp_start))
-       
+            BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, \
+            VERBOSE_LEVEL=VERBOSE_LEVEL)
+        
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'Function Compilations of SFFT-SUBTRACTION '
+            _message += 'TAKES [%.3f s]!' %(time.time() - Tcomp_start)
+            print('\nMeLOn Report: %s' %_message)
+        
         # * Perform SFFT Subtraction
-        from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
-
         SatMask_REF = SFFTPrepDict['REF-SAT-Mask']
         SatMask_SCI = SFFTPrepDict['SCI-SAT-Mask']
         NaNmask_U = SFFTPrepDict['Union-NaN-Mask']
         PixA_mREF = SFFTPrepDict['PixA_mREF']
         PixA_mSCI = SFFTPrepDict['PixA_mSCI']
 
         if ConvdSide == 'REF':
@@ -339,78 +370,137 @@
                 PixA_J[NaNmask_U] = PixA_mJ[NaNmask_U]
             else: PixA_I, PixA_J = PixA_SCI, PixA_REF
             if MaskSatContam: 
                 ContamMask_I = SatMask_SCI
                 ContamMask_J = SatMask_REF
             else: ContamMask_I = None
 
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            print('MeLOn CheckPoint: TRIGGER SFFT-SUBTRACTION!')
+
         Tsub_start = time.time()
         _tmp = GeneralSFFTSubtract.GSS(PixA_I=PixA_I, PixA_J=PixA_J, PixA_mI=PixA_mI, PixA_mJ=PixA_mJ, \
             SFFTConfig=SFFTConfig, ContamMask_I=ContamMask_I, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-            CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
+            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)
+        
         Solution, PixA_DIFF, ContamMask_CI = _tmp
-        if MaskSatContam:
-            ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
-        print('\nMeLOn Report: SFFT Subtraction Takes [%.3f s]' %(time.time() - Tsub_start))
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'SFFT-SUBTRACTION TAKES [%.3f s]!' %(time.time() - Tsub_start)
+            print('\nMeLOn Report: %s' %_message)
+        
+        # ** adjust the sign of difference image 
+        #    NOTE: Our convention is to make the transients on SCI always show themselves as positive signal on DIFF
+        #    (a) when REF is convolved, DIFF = SCI - Conv(REF)
+        #    (b) when SCI is convolved, DIFF = Conv(SCI) - REF
 
+        if ConvdSide == 'SCI':
+            PixA_DIFF = -PixA_DIFF
+
+        if VERBOSE_LEVEL in [1, 2]:
+            if ConvdSide == 'REF':
+                _message = 'Reference Image is Convolved in SFFT-SUBTRACTION [DIFF = SCI - Conv(REF)]!'
+                print('MeLOn CheckPoint: %s' %_message)
+
+            if ConvdSide == 'SCI':
+                _message = 'Science Image is Convolved in SFFT-SUBTRACTION [DIFF = Conv(SCI) - REF]!'
+                print('MeLOn CheckPoint: %s' %_message)
+
+        # ** estimate the flux scaling through the convolution of image subtraction
+        #    NOTE: if photometric ratio is not constant (ConstPhotRatio=False), we measure of a grid
+        #          of coordinates to estimate the flux scaling and its fluctuation (polynomial form).
+        #    NOTE: here we set the tile-size of the grid about 64 x 64 pix, but meanwhile, 
+        #          we also require the tiles should no less than 6 along each axis.
+
+        N0, N1 = SFFTConfig[0]['N0'], SFFTConfig[0]['N1']
+        L0, L1 = SFFTConfig[0]['L0'], SFFTConfig[0]['L1']
+        DK, Fpq = SFFTConfig[0]['DK'], SFFTConfig[0]['Fpq']
+
+        if ConstPhotRatio:
+            SFFT_FSCAL_NSAMP = 1
+            XY_q = np.array([[N0/2.0, N1/2.0]]) + 0.5
+            RFS = Realize_FluxScaling(XY_q=XY_q)
+            SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+            SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = SFFT_FSCAL_q[0], 0.0
+        
+        if not ConstPhotRatio:
+            TILESIZE_X, TILESIZE_Y = 64, 64    # FIXME emperical/arbitrary values
+            NTILE_X = np.max([round(N0/TILESIZE_X), 6])
+            NTILE_Y = np.max([round(N1/TILESIZE_Y), 6])
+            GX = np.linspace(0.5, N0+0.5, NTILE_X+1)
+            GY = np.linspace(0.5, N1+0.5, NTILE_Y+1)
+            YY, XX = np.meshgrid(GY, GX)
+            XY_q = np.array([XX.flatten(), YY.flatten()]).T
+            SFFT_FSCAL_NSAMP = XY_q.shape[0]
+            
+            RFS = Realize_FluxScaling(XY_q=XY_q)
+            SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+            SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = np.mean(SFFT_FSCAL_q), np.std(SFFT_FSCAL_q)
+
+        PHOT_FSCAL = 10**(SFFTPrepDict['MAG_OFFSET']/-2.5)  # FLUX_SCI/FLUX_REF
+        if ConvdSide == 'SCI': PHOT_FSCAL = 1.0/PHOT_FSCAL
+
+        if VERBOSE_LEVEL in [1, 2]:
+            _message = 'The Flux Scaling through the Convolution of SFFT-SUBTRACTION '
+            _message += '[%.6f +/- %.6f] from [%d] positions!\n' %(SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG, SFFT_FSCAL_NSAMP)
+            _message += 'P.S. The approximated Flux Scaling from Photometry [%.6f].' %PHOT_FSCAL
+            print('MeLOn CheckPoint: %s' %_message)
+        
+        # ** run post anomaly check (PAC)
         if PostAnomalyCheck:
-            warnings.warn('\nMeLOn WARNING: Post-Anomaly Check requires CORRECT GAIN in FITS HEADER!')
-            # TODO: Incorporate weight-maps of the input image pair for more accurate SExtractor FLUXERR.
 
             """
             # Remarks on the Post Anomaly Check (PAC)
-            # [1] Recall that Elaborate Variable Rejection (EVREJ) also use SExtractor photometric errors to identify variables.
-            #     I would say, PAC should be more accurate than EVREJ.
+            # [1] One may notice that Elaborate Variable Rejection (EVREJ) also use SExtractor 
+            #     photometric errors to identify variables. However, PAC should be more accurate than EVREJ.
             #     NOTE: Bright transients (compared with its host) can be also identified by PAC.
             #
             # [2] distribution mean: image subtraction is expected to have better accuracy on the determination 
             #     of the photometric scaling, compared with the constant MAG_OFFSET in EVREJ. As a result,
             #     the flux change counted on the difference image is likely more 'real' than that in EVREJ.
             #
-            # [3] distribution variance: i) inaccurate SExtractor FLUXERR especially at the bright end
-            #     and ii) the error of MAG_OFFSET affect one FLUXERR scaling.
-            #     NOTE: The imperfections on distribution variance are just same as EVREJ.
-            #     NOTE: Using SFFT kernel sum would be better than MAG_OFFSET for scaling FLUXERR. 
-            #           For simplicity, howerver, we use MAG_OFFSET (with error << 5%) which is good enough here.
+            # [3] distribution variance: SExtractor FLUXERR_AUTO can be inaccurate, and the convolution effect
+            #     on the photometric errors has been simplified as multiplying an average flux scaling on an image.
             #
             """
 
+            if VERBOSE_LEVEL in [2]:
+                warnings.warn('\nMeLOn REMINDER: Post-Anomaly Check requires CORRECT GAIN in FITS HEADER!')
+
             AstSEx_SS = SFFTPrepDict['SExCatalog-SubSource']
             SFFTLmap = SFFTPrepDict['SFFT-LabelMap']
             
             # ** Only consider the Non-Prior-Banned SubSources
             if 'MASK_PriorBan' in AstSEx_SS.colnames:
                 nPBMASK_SS = ~np.array(AstSEx_SS['MASK_PriorBan'])
                 AstSEx_vSS = AstSEx_SS[nPBMASK_SS]
             else: AstSEx_vSS = AstSEx_SS
             
             # ** Estimate expected variance of Non-Prior-Banned SubSources on the difference
-            MAG_OFFSET = SFFTPrepDict['MAG_OFFSET']
-            FLUX_SCAL = 10**(MAG_OFFSET/-2.5)  # FLUX_SCI/FLUX_REF
-
             FLUXERR_vSSr = np.array(AstSEx_vSS['FLUXERR_AUTO_REF'])
             FLUXERR_vSSs = np.array(AstSEx_vSS['FLUXERR_AUTO_SCI'])
 
             if ConvdSide == 'REF':
-                sFLUXERR_vSSr = FLUXERR_vSSr * FLUX_SCAL
+                sFLUXERR_vSSr = FLUXERR_vSSr * SFFT_FSCAL_MEAN
                 ExpDVAR_vSS = sFLUXERR_vSSr**2 + FLUXERR_vSSs**2
+
             if ConvdSide == 'SCI':
-                sFLUXERR_vSSs = FLUXERR_vSSs / FLUX_SCAL
+                sFLUXERR_vSSs = FLUXERR_vSSs * SFFT_FSCAL_MEAN
                 ExpDVAR_vSS = FLUXERR_vSSr**2 + sFLUXERR_vSSs**2
 
             # ** Measure the ratios of Non-Prior-Banned SubSources on the difference for PAC
             SEGL_vSS = np.array(AstSEx_vSS['SEGLABEL']).astype(int)
             DFSUM_vSS = ndimage.labeled_comprehension(PixA_DIFF, SFFTLmap, SEGL_vSS, np.sum, float, 0.0)
             RATIO_vSS = DFSUM_vSS / np.clip(np.sqrt(ExpDVAR_vSS), a_min=1e-8, a_max=None)
             PAMASK_vSS = np.abs(RATIO_vSS) > PAC_RATIO_THRESH
 
-            _message = 'FIND [%d] PostAnomaly SubSources [> %.2f sigma] ' %(np.sum(PAMASK_vSS), PAC_RATIO_THRESH)
-            _message += 'out of [%d] Non-Prior-Banned SubSources!\n' %(len(AstSEx_vSS))
-            _message += 'P.S. there are [%d] Prior-Banned SubSources!' %(len(AstSEx_SS) - len(AstSEx_vSS))
-            print('\nMeLOn CheckPoint: %s' %_message)
+            if VERBOSE_LEVEL in [1, 2]:
+                _message = 'Identified [%d] PostAnomaly SubSources [> %.2f sigma] ' %(np.sum(PAMASK_vSS), PAC_RATIO_THRESH)
+                _message += 'out of [%d] Non-Prior-Banned SubSources!\n' %(len(AstSEx_vSS))
+                _message += 'P.S. there are [%d] Prior-Banned SubSources!' %(len(AstSEx_SS) - len(AstSEx_vSS))
+                print('\nMeLOn CheckPoint: %s' %_message)
             
             # ** Record the results (decorate AstSEx_SS in SFFTPrepDict)
             if 'MASK_PriorBan' in AstSEx_SS.colnames:
                 ExpDVAR_SS = np.nan * np.ones(len(AstSEx_SS))       # NOTE Prior-Ban is trivial NaN
                 DFSUM_SS = np.nan * np.ones(len(AstSEx_SS))         # NOTE Prior-Ban is trivial NaN
                 RATIO_SS = np.nan * np.ones(len(AstSEx_SS))         # NOTE Prior-Ban is trivial NaN
                 PAMASK_SS = np.zeros(len(AstSEx_SS)).astype(bool)   # NOTE Prior-Ban is trivial False
@@ -425,44 +515,70 @@
                 RATIO_SS = RATIO_vSS
                 PAMASK_SS = PAMASK_vSS
 
             AstSEx_SS.add_column(Column(ExpDVAR_SS, name='ExpDVAR_PostAnomaly'))
             AstSEx_SS.add_column(Column(DFSUM_SS, name='DFSUM_PostAnomaly'))
             AstSEx_SS.add_column(Column(RATIO_SS, name='RATIO_PostAnomaly'))
             AstSEx_SS.add_column(Column(PAMASK_SS, name='MASK_PostAnomaly'))
-
-        # * Modifications on the difference image
-        #   a) when REF is convolved, DIFF = SCI - Conv(REF)
-        #      PSF_DIFF is coincident with SCI, transients on SCI are positive signal in DIFF.
-        #   b) when SCI is convolved, DIFF = Conv(SCI) - REF
-        #      PSF_DIFF is coincident with REF, transients on SCI are still positive signal in DIFF.
-
+        
+        # ** final tweaks on the difference image
         if NaNmask_U is not None:
-            # ** Mask Union-NaN region
-            PixA_DIFF[NaNmask_U] = np.nan
+            PixA_DIFF[NaNmask_U] = np.nan   # Mask Union-NaN regions
+        
         if MaskSatContam:
-            # ** Mask Saturate-Contaminate region 
-            PixA_DIFF[ContamMask_DIFF] = np.nan
-        if ConvdSide == 'SCI': 
-            # ** Flip difference when science is convolved
-            PixA_DIFF = -PixA_DIFF
-
+            ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
+            PixA_DIFF[ContamMask_DIFF] = np.nan   # Mask Saturation-Contaminated regions
+        
         # * Save difference image
         if FITS_DIFF is not None:
+
+            """
+            # Remarks on header of difference image
+            # [1] In general, the FITS header of difference image would mostly be inherited from science image.
+            #
+            # [2] when science image is convolved, we turn to set GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN (unit: e-/ADU)
+            #     so that one can correctly convert ADU to e- for a transient appears on science image.
+            #     WARNING: for a transient appears on reference image, GAIN_DIFF = GAIN_SCI is correct.
+            #              we should keep in mind that GAIN_DIFF is not an absolute instrumental value.
+            #     WARNING: one can only estimate the Poission noise from the science transient via GIAN_DIFF.
+            #              the Poission noise from the background source (host galaxy) can enhance the 
+            #              background noise at the position of the transient. photometry softwares which 
+            #              only take background noise and transient Possion noise into account would tend 
+            #              to overestimate the SNR of the transient.
+            # 
+            # [3] when science image is convolved, we turn to set SATURA_DIFF = SATURA_SCI * SFFT_FSCAL_MEAN         
+            #     WARNING: it is still not a good idea to use SATURA_DIFF to identify the SATURATION regions
+            #              on difference image. more appropriate way is masking the saturation contaminated 
+            #              regions on difference image (MaskSatContam=True), or alternatively, leave them  
+            #              alone and using AI stamp classifier to reject saturation-related bogus.
+            #
+            """
+
             _hdl = fits.open(FITS_SCI)
             _hdl[0].data[:, :] = PixA_DIFF.T
+
             _hdl[0].header['NAME_REF'] = (pa.basename(FITS_REF), 'MeLOn: SFFT')
             _hdl[0].header['NAME_SCI'] = (pa.basename(FITS_SCI), 'MeLOn: SFFT')
             _hdl[0].header['FWHM_REF'] = (FWHM_REF, 'MeLOn: SFFT')
             _hdl[0].header['FWHM_SCI'] = (FWHM_SCI, 'MeLOn: SFFT')
             _hdl[0].header['KERORDER'] = (KerPolyOrder, 'MeLOn: SFFT')
             _hdl[0].header['BGORDER'] = (BGPolyOrder, 'MeLOn: SFFT')
             _hdl[0].header['CPHOTR'] = (str(ConstPhotRatio), 'MeLOn: SFFT')
             _hdl[0].header['KERHW'] = (KerHW, 'MeLOn: SFFT')
             _hdl[0].header['CONVD'] = (ConvdSide, 'MeLOn: SFFT')
+
+            if ConvdSide == 'SCI':
+                GAIN_SCI = _hdl[0].header[GAIN_KEY]
+                SATUR_SCI = _hdl[0].header[SATUR_KEY]
+                GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN
+                SATUR_DIFF = SATUR_SCI * SFFT_FSCAL_MEAN
+
+                _hdl[0].header[GAIN_KEY] = (GAIN_DIFF, 'MeLOn: SFFT')
+                _hdl[0].header[SATUR_KEY] = (SATUR_DIFF, 'MeLOn: SFFT')
+
             _hdl.writeto(FITS_DIFF, overwrite=True)
             _hdl.close()
         
         # * Save solution array
         if FITS_Solution is not None:
             phdu = fits.PrimaryHDU()
             phdu.header['N0'] = (SFFTConfig[0]['N0'], 'MeLOn: SFFT')
@@ -477,8 +593,8 @@
             phdu.header['FPQ'] = (SFFTConfig[0]['Fpq'], 'MeLOn: SFFT')
             phdu.header['FIJAB'] = (SFFTConfig[0]['Fijab'], 'MeLOn: SFFT')
 
             PixA_Solution = Solution.reshape((-1, 1))
             phdu.data = PixA_Solution.T
             fits.HDUList([phdu]).writeto(FITS_Solution, overwrite=True)
 
-        return SFFTPrepDict, Solution, PixA_DIFF
+        return PixA_DIFF, SFFTPrepDict, Solution, SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG
```

### Comparing `sfft-1.3.4/sfft/MultiEasyCrowdedPacket.py` & `sfft-1.4.0/sfft/MultiEasyCrowdedPacket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+import sys
 import time
 import math
 import warnings
 import threading
+import cupy as cp
 import numpy as np
 import os.path as pa
 from astropy.io import fits
 from sfft.AutoCrowdedPrep import Auto_CrowdedPrep
 from sfft.utils.meta.TimeoutKit import TimeoutAfter
-# version: Sep 16, 2022
+from sfft.utils.SFFTSolutionReader import Realize_FluxScaling
+from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+# version: Feb 24, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class MultiEasy_CrowdedPacket:
     def __init__(self, FITS_REF_Queue, FITS_SCI_Queue, FITS_DIFF_Queue=[], FITS_Solution_Queue=[], \
-        ForceConv_Queue=[], GKerHW_Queue=[], KerHWRatio=2.0, KerHWLimit=(2, 20), KerPolyOrder=2, BGPolyOrder=2, \
-        ConstPhotRatio=True, MaskSatContam=False, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', \
-        BACK_TYPE='AUTO', BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=5.0, \
-        DETECT_MINAREA=5, DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', \
-        ONLY_FLAGS=None, BoundarySIZE=0.0, BACK_SIZE_SUPER=128, StarExt_iter=2, PriorBanMask_Queue=[]):
+        ForceConv_Queue=[], GKerHW_Queue=[], KerHWRatio=2.0, KerHWLimit=(2, 20), KerPolyOrder=2, \
+        BGPolyOrder=2, ConstPhotRatio=True, MaskSatContam=False, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', \
+        BACK_TYPE='AUTO', BACK_VALUE='0.0', BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=5.0, \
+        ANALYSIS_THRESH=5.0, DETECT_MINAREA=5, DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', \
+        ONLY_FLAGS=None, BoundarySIZE=0.0, BACK_SIZE_SUPER=128, StarExt_iter=2, PriorBanMask_Queue=[], \
+        CLEAN_GPU_MEMORY=False, VERBOSE_LEVEL=2):
 
         """
-        # NOTE: This function is to Perform Crowded-Flavor SFFT for multiple tasks:
-        #       @ it makes sense when users have multiple CPU threads and GPU(s) available.
-        #       @ WARNING: the module currently only support Cupy backend!
+        # NOTE: This function is to perform Crowded-Flavor SFFT for multiple tasks:
+        #       @ this module (only support Cupy backend) would help making the 
+        #         best use of the available CPU and GPU resources.
 
-        * Parameters for Sparse-Flavor SFFT [multiple tasks]
+        * Parameters for Crowded-Flavor SFFT [multiple tasks]
         
         # ----------------------------- Computing Enviornment [Cupy backend ONLY] --------------------------------- #
 
         -NUM_THREADS_4PREPROC [8]           # the number of Python threads for preprocessing.
                                             # WARNING: Empirically, the current code is only optimized for 
                                             #          NUM_TASK / NUM_THREADS_4PREPROC in [1.0 - 4.0].
                                             #          The computing effeciency goes down sharply as the ratio increases.
@@ -37,15 +43,16 @@
 
         -NUM_THREADS_4SUBTRACT [1]          # the number of Python threads for sfft subtraction.
                                             # says, if you have four GPU cards, then set it to 4.
                                             # NOTE: please do not confused the Python threads 
                                             #       with the CUDA threads (block, threads ...).
 
         -CUDA_DEVICES_4SUBTRACT [['0']]     # it specifies certain GPU devices (indices) to conduct the subtractions.
-                                            # the GPU devices are usually numbered 0 to N-1 (you may use command nvidia-smi to check).
+                                            # the GPU devices are usually numbered 0 to N-1. 
+                                            # (you may use command nvidia-smi to check for Nvidia GPU devices).
 
         -TIMEOUT_4PREPROC_EACHTASK [300]    # timeout of each task during preprocessing.
                                             
         -TIMEOUT_4SUBTRACT_EACHTASK [300]   # timeout of each task during sfft subtraction.
 
         # ----------------------------- Preprocessing with Saturation Rejection for Image-Masking --------------------------------- #
 
@@ -57,25 +64,28 @@
         -SATUR_KEY ['SATURATE']             # SExtractor Parameter SATUR_KEY
                                             # i.e., keyword of effective saturation in FITS header (of reference & science)
                                             # Remarks: note that Crowded-Flavor SFFT does not require sky-subtracted images as inputs,
                                             #          so the default keyword is the common name for saturation level.
         
         -BACK_TYPE ['AUTO']                 # SExtractor Parameter BACK_TYPE = [AUTO or MANUAL].
          
-        -BACK_VALUE [0.0]                   # SExtractor Parameter BACK_VALUE (only work for BACK_TYPE='MANUAL')
+        -BACK_VALUE [0]                     # SExtractor Parameter BACK_VALUE (only work for BACK_TYPE='MANUAL')
 
         -BACK_SIZE [64]                     # SExtractor Parameter BACK_SIZE
 
         -BACK_FILTERSIZE [3]                # SExtractor Parameter BACK_FILTERSIZE
 
         -DETECT_THRESH [5.0]                # SExtractor Parameter DETECT_THRESH
                                             # NOTE: One may notice that the default DETECT_THRESH in SExtractor is 1.5.
                                             #       Using a 'very cold' detection threshold here is to speed up SExtractor.
-                                            #       Although DETECT_THRESH = 5.0 means we will miss the faint-end sources with 
-                                            #       SNR < 20 (approximately), the cost is generally acceptable for saturation mask.
+                                            #       Although DETECT_THRESH = 5.0 means we will miss the faint-end sources with SNR < 20 
+                                            #       (approximately), the cost is generally acceptable for saturation mask.
+
+        -ANALYSIS_THRESH [5.0]              # SExtractor Parameter ANALYSIS_THRESH
+                                            # NOTE: By default, let -ANALYSIS_THRESH = -DETECT_THRESH
 
         -DETECT_MINAREA [5]                 # SExtractor Parameter DETECT_MINAREA
         
         -DETECT_MAXAREA [0]                 # SExtractor Parameter DETECT_MAXAREA
 
         -DEBLEND_MINCONT [0.005]            # SExtractor Parameter DEBLEND_MINCONT (typically, 0.001 - 0.005)
 
@@ -140,26 +150,33 @@
                                             #   by a polynomial with degree -KerPolyOrder.
 
         -MaskSatContam [False]              # Mask saturation-contaminated regions on difference image ? can be True or False
                                             # NOTE the pixels enclosed in the regions are replaced by NaN.
 
         # ----------------------------- Input & Output --------------------------------- #
 
-        -FITS_REF_Queue []                 # A queue of -FITS_REF in sfft.Easy_CrowdedPacket.
-                                           # File path of input reference image.
+        -FITS_REF_Queue []                  # A queue of -FITS_REF in sfft.Easy_CrowdedPacket.
+                                            # File path of input reference image.
+
+        -FITS_SCI_Queue []                  # A queue of -FITS_SCI in sfft.Easy_CrowdedPacket.
+                                            # File path of input science image.
 
-        -FITS_SCI_Queue []                 # A queue of -FITS_SCI in sfft.Easy_CrowdedPacket.
-                                           # File path of input science image.
+        -FITS_DIFF_Queue [None]             # A queue of -FITS_DIFF in sfft.Easy_CrowdedPacket.
+                                            # File path of output difference image.
 
-        -FITS_DIFF_Queue [None]            # A queue of -FITS_DIFF in sfft.Easy_CrowdedPacket.
-                                           # File path of output difference image.
+        -FITS_Solution_Queue [None]         # A queue of -FITS_Solution in sfft.Easy_CrowdedPacket.
+                                            # File path of the solution of the linear system.
+                                            # it is an array of (..., a_ijab, ... b_pq, ...).
+
+        # ----------------------------- Miscellaneous --------------------------------- #
+        
+        -CLEAN_GPU_MEMORY [False]           # Clean GPU memory or not after all subtractions done in a GPU device.
 
-        -FITS_Solution_Queue [None]        # A queue of -FITS_Solution in sfft.Easy_CrowdedPacket.
-                                           # File path of the solution of the linear system.
-                                           # it is an array of (..., a_ijab, ... b_pq, ...).
+        -VERBOSE_LEVEL [2]                  # The level of verbosity, can be [0, 1, 2]
+                                            # 0/1/2: QUIET/NORMAL/FULL mode
 
         # Important Notice:
         #
         # a): if reference is convolved in SFFT, then DIFF = SCI - Convolved_REF.
         #     [difference image is expected to have PSF & flux zero-point consistent with science image]
         #     e.g., -ForceConv='REF' or -ForceConv='AUTO' when reference has better seeing.
         #
@@ -170,14 +187,15 @@
         # Remarks: this convention is to guarantee that transients emerge on science image always 
         #          show a positive signal on difference images.
 
         """
 
         self.FITS_REF_Queue = FITS_REF_Queue
         self.FITS_SCI_Queue = FITS_SCI_Queue
+        self.NUM_TASK = len(FITS_SCI_Queue)
 
         self.KerHWRatio = KerHWRatio
         self.KerHWLimit = KerHWLimit
         self.KerPolyOrder = KerPolyOrder
         self.BGPolyOrder = BGPolyOrder
         self.ConstPhotRatio = ConstPhotRatio
         self.MaskSatContam = MaskSatContam
@@ -186,174 +204,223 @@
         self.SATUR_KEY = SATUR_KEY
         self.BACK_TYPE = BACK_TYPE
         self.BACK_VALUE = BACK_VALUE
         self.BACK_SIZE = BACK_SIZE
         self.BACK_FILTERSIZE = BACK_FILTERSIZE
         
         self.DETECT_THRESH = DETECT_THRESH
+        self.ANALYSIS_THRESH = ANALYSIS_THRESH
         self.DETECT_MINAREA = DETECT_MINAREA
         self.DETECT_MAXAREA = DETECT_MAXAREA
         self.DEBLEND_MINCONT = DEBLEND_MINCONT
         self.BACKPHOTO_TYPE = BACKPHOTO_TYPE
         self.ONLY_FLAGS = ONLY_FLAGS
         self.BoundarySIZE = BoundarySIZE
         
         self.BACK_SIZE_SUPER = BACK_SIZE_SUPER
         self.StarExt_iter = StarExt_iter
-        self.NUM_TASK = len(FITS_SCI_Queue)
+        
+        self.CLEAN_GPU_MEMORY = CLEAN_GPU_MEMORY
+        self.VERBOSE_LEVEL = VERBOSE_LEVEL
 
         if FITS_DIFF_Queue == []:
-            _warn_message = 'Argument FITS_DIFF_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument FITS_DIFF_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.FITS_DIFF_Queue = [None] * self.NUM_TASK
         else: self.FITS_DIFF_Queue = FITS_DIFF_Queue
         
         if FITS_Solution_Queue == []:
-            _warn_message = 'Argument FITS_Solution_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument FITS_Solution_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.FITS_Solution_Queue = [None] * self.NUM_TASK
         else: self.FITS_Solution_Queue = FITS_Solution_Queue
         
         if ForceConv_Queue == []:
-            _warn_message = 'Argument ForceConv_Queue is EMPTY then Use default [...AUTO...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'Argument ForceConv_Queue is EMPTY then Use default [...AUTO...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.ForceConv_Queue = ['AUTO'] * self.NUM_TASK
         else: self.ForceConv_Queue = ForceConv_Queue
 
         if GKerHW_Queue == []:
-            _warn_message = 'Argument GKerHW_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument GKerHW_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.GKerHW_Queue = [None] * self.NUM_TASK
         else: self.GKerHW_Queue = GKerHW_Queue
 
         if PriorBanMask_Queue == []:
-            _warn_message = 'Argument PriorBanMask_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument PriorBanMask_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.PriorBanMask_Queue = [None] * self.NUM_TASK
         else: self.PriorBanMask_Queue = PriorBanMask_Queue
-    
+
     def MESP_Cupy(self, NUM_THREADS_4PREPROC=8, NUM_THREADS_4SUBTRACT=1, CUDA_DEVICES_4SUBTRACT=['0'], \
         TIMEOUT_4PREPROC_EACHTASK=300, TIMEOUT_4SUBTRACT_EACHTASK=300):
 
         # * define task-oriented dictionaries of status-bar and products
         #   status 0: Initial State
         #   status 1: Preprocessing SUCCESS || status -1: Preprocessing FAIL
         #   status 2: Subtraction SUCCESS || status -2: Subtraction FAIL
         #   status 32: Preprocessing is IN-PROGRESS ...
         #   status 64: Subtraction is IN-PROGRESS ...
         #   NOTE: Subtraction would not be triggered when Preprocessing fails
         
         _RATIO = self.NUM_TASK / NUM_THREADS_4PREPROC
         if _RATIO > 4.0:
-            _warn_message = 'THIS FUNCTION IS NOT OPTIMIZED FOR RATIO OF '
-            _warn_message += 'NUM_TASK / NUM_THREADS_4PREPROC BEING TO HIGH [%.1f > 4.0]!' %_RATIO
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'THIS FUNCTION IS NOT OPTIMIZED FOR RATIO OF '
+                _warn_message += 'NUM_TASK / NUM_THREADS_4PREPROC BEING TO HIGH [%.1f > 4.0]!' %_RATIO
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
 
         BACKEND_4SUBTRACT = 'Cupy'
         taskidx_lst = np.arange(self.NUM_TASK)
         assert NUM_THREADS_4SUBTRACT == len(CUDA_DEVICES_4SUBTRACT)
         
-        DICT_STATUS_BAR = {'task-[%d]' %taskidx: 0 for taskidx in taskidx_lst}
-        DICT_PRODUCTS = {'task-[%d]' %taskidx: {} for taskidx in taskidx_lst}
+        DICT_STATUS_BAR = {'TASK-[%d]' %taskidx: 0 for taskidx in taskidx_lst}
+        DICT_PRODUCTS = {'TASK-[%d]' %taskidx: {} for taskidx in taskidx_lst}
         lock = threading.RLock()
 
         # * define the function for preprocessing (see sfft.EasyCrowdedPacket)
         def FUNC_4PREPROC(INDEX_THREAD_4PREPROC):
 
             THREAD_ALIVE_4PREPROC = True
             while THREAD_ALIVE_4PREPROC:
                 with lock:
-                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['task-[%d]' %taskidx] for taskidx in taskidx_lst])
+                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['TASK-[%d]' %taskidx] for taskidx in taskidx_lst])
                     OPEN_MASK_4PREPROC = STATUS_SNAPSHOT == 0
                     if np.sum(OPEN_MASK_4PREPROC) > 0:
                         taskidx_acquired = taskidx_lst[OPEN_MASK_4PREPROC][0]
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = 32
-                        _message = 'Preprocessing thread-[%d] ACQUIRED task-[%d]!' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
-                        print('\nMeLOn CheckPoint: %s' %_message)
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = 32
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4PREPROC-[%d] ACQUIRED TASK-[%d] ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                            _message += '(Crowded-Flavor Auto Preprocessing)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
                     else: 
                         THREAD_ALIVE_4PREPROC = False
                         taskidx_acquired = None
-                        _message = 'TERMINATE Preprocessing thread-[%d] AS NO TASK WILL BE ALLOCATED!' %INDEX_THREAD_4PREPROC
-                        print('\nMeLOn CheckPoint: %s' %_message)
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4PREPROC-[%d] TERMINATED ' %INDEX_THREAD_4PREPROC
+                            _message += 'SINCE NO MORE TASK WILL BE ALLOCATED '
+                            _message += '(Crowded-Flavor Auto Preprocessing)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
 
                 if taskidx_acquired is not None:
                     FITS_REF = self.FITS_REF_Queue[taskidx_acquired]
                     FITS_SCI = self.FITS_SCI_Queue[taskidx_acquired]
                     PriorBanMask = self.PriorBanMask_Queue[taskidx_acquired]
+
                     try:
                         with TimeoutAfter(timeout=TIMEOUT_4PREPROC_EACHTASK, exception=TimeoutError):
+                            
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                                _message += 'TRIGGER Crowded-Flavor Auto Preprocessing!'
+                                print('MeLOn CheckPoint: %s' %_message)
+
+                            # ** perform Auto-Crowded-Prep
                             _ACP = Auto_CrowdedPrep(FITS_REF=FITS_REF, FITS_SCI=FITS_SCI, GAIN_KEY=self.GAIN_KEY, \
                                 SATUR_KEY=self.SATUR_KEY, BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, \
-                                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, \
-                                DETECT_MINAREA=self.DETECT_MINAREA, DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, \
-                                BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, ONLY_FLAGS=self.ONLY_FLAGS, BoundarySIZE=self.BoundarySIZE)
-                            SFFTPrepDict = _ACP.AutoMask(BACK_SIZE_SUPER=self.BACK_SIZE_SUPER, StarExt_iter=self.StarExt_iter, \
-                                PriorBanMask=PriorBanMask)
+                                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, \
+                                DETECT_THRESH=self.DETECT_THRESH, ANALYSIS_THRESH=self.ANALYSIS_THRESH, \
+                                DETECT_MINAREA=self.DETECT_MINAREA, DETECT_MAXAREA=self.DETECT_MAXAREA, \
+                                DEBLEND_MINCONT=self.DEBLEND_MINCONT, BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, \
+                                ONLY_FLAGS=self.ONLY_FLAGS, BoundarySIZE=self.BoundarySIZE, VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+                            
+                            SFFTPrepDict = _ACP.AutoMask(BACK_SIZE_SUPER=self.BACK_SIZE_SUPER, \
+                                StarExt_iter=self.StarExt_iter, PriorBanMask=PriorBanMask)
                         
                         NEW_STATUS = 1
-                        _message = 'Successful Preprocessing for task-[%d] ' %taskidx_acquired
-                        _message += 'in Preprocessing thread-[%d]!' %INDEX_THREAD_4PREPROC
-                        print('\nMeLOn CheckPoint: %s' %_message)
-                    except:
+                        if self.VERBOSE_LEVEL in [1, 2]:
+                            _message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                            _message += 'SUCCESSFUL Crowded-Flavor Auto Preprocessing!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
+
+                    except Exception as e:
                         NEW_STATUS = -1
-                        _error_message = 'UnSuccessful Preprocessing for task-[%d] ' %taskidx_acquired
-                        _error_message += 'in Preprocessing thread-[%d]!' %INDEX_THREAD_4PREPROC
-                        print('\nMeLOn ERROR: %s' %_error_message)
                         SFFTPrepDict = None
+                        if self.VERBOSE_LEVEL in [0, 1, 2]:
+                            print(e, file=sys.stderr)
+                            _error_message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                            _error_message += 'FAILED Crowded-Flavor Auto Preprocessing!'
+                            print('\nMeLOn ERROR: %s' %_error_message)
                     
                     with lock:
                         # NOTE: IN FACT, THERE IS NO RISK HERE EVEN WITHOUT LOCK.
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = NEW_STATUS
-                        DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['SFFTPrepDict'] = SFFTPrepDict
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = NEW_STATUS
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFTPrepDict'] = SFFTPrepDict
 
             return None
         
         # * define the function for sfft subtraction (see sfft.EasyCrowdedPacket)
         def FUNC_4SUBTRCT(INDEX_THREAD_4SUBTRACT):
             
             CUDA_DEVICE_4SUBTRACT = CUDA_DEVICES_4SUBTRACT[INDEX_THREAD_4SUBTRACT]
+            device = cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT))
+            device.use()
+
             THREAD_ALIVE_4SUBTRCT = True
+            GPU_MEMORY_CLEANED = True
+
             while THREAD_ALIVE_4SUBTRCT:
                 SHORT_PAUSE = False
+
                 with lock:
-                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['task-[%d]' %taskidx] for taskidx in taskidx_lst])
+                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['TASK-[%d]' %taskidx] for taskidx in taskidx_lst])
                     OPEN_MASK_4SUBTRACT = STATUS_SNAPSHOT == 1
                     WAIT_MASK_4SUBTRACT = np.in1d(STATUS_SNAPSHOT, [0, 32])
+
                     if np.sum(OPEN_MASK_4SUBTRACT) > 0:
                         taskidx_acquired = taskidx_lst[OPEN_MASK_4SUBTRACT][0]
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = 64
-                        _message = 'Subtraction thread-[%d] ACQUIRED task-[%d]!' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
-                        print('\nMeLOn CheckPoint: %s' %_message)
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = 64
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] ACQUIRED TASK-[%d] ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _message += '(SFFT-SUBTRACTION)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
+
                     elif np.sum(WAIT_MASK_4SUBTRACT) > 0:
                         SHORT_PAUSE = True
                         taskidx_acquired = None
+
                     else:
                         THREAD_ALIVE_4SUBTRCT = False
                         taskidx_acquired = None
-                        _message = 'TERMINATE Subtraction thread-[%d] AS NO TASK WILL BE ALLOCATED!' %INDEX_THREAD_4SUBTRACT
-                        print('\nMeLOn CheckPoint: %s' %_message)
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] TERMINATED ' %INDEX_THREAD_4SUBTRACT
+                            _message += 'SINCE NO MORE TASK WILL BE ALLOCATED '
+                            _message += '(SFFT-SUBTRACTION)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
 
                 if SHORT_PAUSE:
                     # run a short sleep, otherwise this thread may always hold the lock by the while loop
                     time.sleep(0.01)
                 
                 if taskidx_acquired is not None:
+
                     FITS_REF = self.FITS_REF_Queue[taskidx_acquired]
                     FITS_SCI = self.FITS_SCI_Queue[taskidx_acquired]
                     FITS_DIFF = self.FITS_DIFF_Queue[taskidx_acquired]
                     FITS_Solution = self.FITS_Solution_Queue[taskidx_acquired]
                     ForceConv = self.ForceConv_Queue[taskidx_acquired]
                     GKerHW = self.GKerHW_Queue[taskidx_acquired]
 
                     with lock:
                         # NOTE: IN FACT, THERE IS NO RISK HERE EVEN WITHOUT LOCK.
-                        SFFTPrepDict = DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['SFFTPrepDict']
+                        SFFTPrepDict = DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFTPrepDict']
 
                     try:
                         with TimeoutAfter(timeout=TIMEOUT_4SUBTRACT_EACHTASK, exception=TimeoutError):
+
                             # * Determine ConvdSide & KerHW
                             FWHM_REF = SFFTPrepDict['FWHM_REF']
                             FWHM_SCI = SFFTPrepDict['FWHM_SCI']
 
                             assert ForceConv in ['AUTO', 'REF', 'SCI']
                             if ForceConv == 'AUTO':
                                 if FWHM_SCI >= FWHM_REF: ConvdSide = 'REF'
@@ -363,28 +430,36 @@
                             if GKerHW is None:
                                 FWHM_La = np.max([FWHM_REF, FWHM_SCI])
                                 KerHW = int(np.clip(self.KerHWRatio * FWHM_La, \
                                                     self.KerHWLimit[0], self.KerHWLimit[1]))
                             else: KerHW = GKerHW
 
                             # * Compile Functions in SFFT Subtraction
-                            from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
-
                             PixA_REF = SFFTPrepDict['PixA_REF']
                             PixA_SCI = SFFTPrepDict['PixA_SCI']
                             
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'TRIGGER Function Compilations of SFFT-SUBTRACTION'
+                                print('MeLOn CheckPoint: %s' %_message)
+                            
                             Tcomp_start = time.time()
-                            SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], KerHW=KerHW, \
-                                KerPolyOrder=self.KerPolyOrder, BGPolyOrder=self.BGPolyOrder, ConstPhotRatio=self.ConstPhotRatio, \
-                                BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
-                            print('\nMeLOn Report: Compiling Functions in SFFT Subtraction Takes [%.3f s]' %(time.time() - Tcomp_start))
+                            GPU_MEMORY_CLEANED = False
+                            SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], \
+                                KerHW=KerHW, KerPolyOrder=self.KerPolyOrder, BGPolyOrder=self.BGPolyOrder, \
+                                ConstPhotRatio=self.ConstPhotRatio, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
+                                VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'Function Compilations of SFFT-SUBTRACTION '
+                                _message += 'TAKES [%.3f s]!' %(time.time() - Tcomp_start)
+                                print('\nMeLOn Report: %s' %_message)
 
                             # * Perform SFFT Subtraction
-                            from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
-
                             SatMask_REF = SFFTPrepDict['REF-SAT-Mask']
                             SatMask_SCI = SFFTPrepDict['SCI-SAT-Mask']
                             NaNmask_U = SFFTPrepDict['Union-NaN-Mask']
                             PixA_mREF = SFFTPrepDict['PixA_mREF']
                             PixA_mSCI = SFFTPrepDict['PixA_mSCI']
 
                             if ConvdSide == 'REF':
@@ -407,52 +482,142 @@
                                     PixA_J[NaNmask_U] = PixA_mJ[NaNmask_U]
                                 else: PixA_I, PixA_J = PixA_SCI, PixA_REF
                                 if self.MaskSatContam: 
                                     ContamMask_I = SatMask_SCI
                                     ContamMask_J = SatMask_REF
                                 else: ContamMask_I = None
                             
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'TRIGGER Function Executions of SFFT-SUBTRACTION!'
+                                print('MeLOn CheckPoint: %s' %_message)
+                            
                             Tsub_start = time.time()
                             _tmp = GeneralSFFTSubtract.GSS(PixA_I=PixA_I, PixA_J=PixA_J, PixA_mI=PixA_mI, PixA_mJ=PixA_mJ, \
                                 SFFTConfig=SFFTConfig, ContamMask_I=ContamMask_I, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-                                CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
+                                VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+
                             Solution, PixA_DIFF, ContamMask_CI = _tmp
-                            if self.MaskSatContam:
-                                ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
-                            print('\nMeLOn Report: SFFT Subtraction Takes [%.3f s]' %(time.time() - Tsub_start))
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'Function Executions of SFFT-SUBTRACTION'
+                                _message += 'TAKES [%.3f s]!' %(time.time() - Tsub_start)
+                                print('\nMeLOn Report: %s' %_message)
+
+                            # ** adjust the sign of difference image 
+                            #    NOTE: Our convention is to make the transients on SCI always show themselves as positive signal on DIFF
+                            #    (a) when REF is convolved, DIFF = SCI - Conv(REF)
+                            #    (b) when SCI is convolved, DIFF = Conv(SCI) - REF
+
+                            if ConvdSide == 'SCI':
+                                PixA_DIFF = -PixA_DIFF
+
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                if ConvdSide == 'REF':
+                                    _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                    _message += 'Reference Image is Convolved in SFFT-SUBTRACTION [DIFF = SCI - Conv(REF)]!'
+                                    print('MeLOn CheckPoint: %s' %_message)
+
+                                if ConvdSide == 'SCI':
+                                    _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                    _message += 'Science Image is Convolved in SFFT-SUBTRACTION [DIFF = Conv(SCI) - REF]!'
+                                    print('MeLOn CheckPoint: %s' %_message)
+
+                            # ** estimate the flux scaling through the convolution of image subtraction
+                            #    NOTE: if photometric ratio is not constant (ConstPhotRatio=False), we measure of a grid
+                            #          of coordinates to estimate the flux scaling and its fluctuation (polynomial form).
+                            #    NOTE: here we set the tile-size of the grid about 64 x 64 pix, but meanwhile, 
+                            #          we also require the tiles should no less than 6 along each axis.
+
+                            N0, N1 = SFFTConfig[0]['N0'], SFFTConfig[0]['N1']
+                            L0, L1 = SFFTConfig[0]['L0'], SFFTConfig[0]['L1']
+                            DK, Fpq = SFFTConfig[0]['DK'], SFFTConfig[0]['Fpq']
+
+                            if self.ConstPhotRatio:
+                                SFFT_FSCAL_NSAMP = 1
+                                XY_q = np.array([[N0/2.0, N1/2.0]]) + 0.5
+                                RFS = Realize_FluxScaling(XY_q=XY_q)
+                                SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+                                SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = SFFT_FSCAL_q[0], 0.0
                             
-                            # * Modifications on the difference image
-                            #   a) when REF is convolved, DIFF = SCI - Conv(REF)
-                            #      PSF(DIFF) is coincident with PSF(SCI), transients on SCI are positive signal in DIFF.
-                            #   b) when SCI is convolved, DIFF = Conv(SCI) - REF
-                            #      PSF(DIFF) is coincident with PSF(REF), transients on SCI are still positive signal in DIFF.
+                            if not self.ConstPhotRatio:
+                                TILESIZE_X, TILESIZE_Y = 64, 64    # FIXME emperical/arbitrary values
+                                NTILE_X = np.max([round(N0/TILESIZE_X), 6])
+                                NTILE_Y = np.max([round(N1/TILESIZE_Y), 6])
+                                GX = np.linspace(0.5, N0+0.5, NTILE_X+1)
+                                GY = np.linspace(0.5, N1+0.5, NTILE_Y+1)
+                                YY, XX = np.meshgrid(GY, GX)
+                                XY_q = np.array([XX.flatten(), YY.flatten()]).T
+                                SFFT_FSCAL_NSAMP = XY_q.shape[0]
+                                
+                                RFS = Realize_FluxScaling(XY_q=XY_q)
+                                SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+                                SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = np.mean(SFFT_FSCAL_q), np.std(SFFT_FSCAL_q)
+
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'The Flux Scaling through the Convolution of SFFT-SUBTRACTION '
+                                _message += '[%.6f +/- %.6f] from [%d] positions!\n' %(SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG, SFFT_FSCAL_NSAMP)
+                                print('MeLOn CheckPoint: %s' %_message)
 
+                            # ** final tweaks on the difference image
                             if NaNmask_U is not None:
-                                # ** Mask Union-NaN region
-                                PixA_DIFF[NaNmask_U] = np.nan
+                                PixA_DIFF[NaNmask_U] = np.nan   # Mask Union-NaN regions
+                            
                             if self.MaskSatContam:
-                                # ** Mask Saturate-Contaminate region 
-                                PixA_DIFF[ContamMask_DIFF] = np.nan
-                            if ConvdSide == 'SCI': 
-                                # ** Flip difference when science is convolved
-                                PixA_DIFF = -PixA_DIFF
+                                ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
+                                PixA_DIFF[ContamMask_DIFF] = np.nan   # Mask Saturation-Contaminated regions
                             
                             # * Save difference image
                             if FITS_DIFF is not None:
+
+                                """
+                                # Remarks on header of difference image
+                                # [1] In general, the FITS header of difference image would mostly be inherited from science image.
+                                #
+                                # [2] when science image is convolved, we turn to set GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN (unit: e-/ADU)
+                                #     so that one can correctly convert ADU to e- for a transient appears on science image.
+                                #     WARNING: for a transient appears on reference image, GAIN_DIFF = GAIN_SCI is correct.
+                                #              we should keep in mind that GAIN_DIFF is not an absolute instrumental value.
+                                #     WARNING: one can only estimate the Poission noise from the science transient via GIAN_DIFF.
+                                #              the Poission noise from the background source (host galaxy) can enhance the 
+                                #              background noise at the position of the transient. photometry softwares which 
+                                #              only take background noise and transient Possion noise into account would tend 
+                                #              to overestimate the SNR of the transient.
+                                # 
+                                # [3] when science image is convolved, we turn to set SATURA_DIFF = SATURA_SCI * SFFT_FSCAL_MEAN         
+                                #     WARNING: it is still not a good idea to use SATURA_DIFF to identify the SATURATION regions
+                                #              on difference image. more appropriate way is masking the saturation contaminated 
+                                #              regions on difference image (MaskSatContam=True), or alternatively, leave them  
+                                #              alone and using AI stamp classifier to reject saturation-related bogus.
+                                #
+                                """
+
                                 _hdl = fits.open(FITS_SCI)
                                 _hdl[0].data[:, :] = PixA_DIFF.T
+
                                 _hdl[0].header['NAME_REF'] = (pa.basename(FITS_REF), 'MeLOn: SFFT')
                                 _hdl[0].header['NAME_SCI'] = (pa.basename(FITS_SCI), 'MeLOn: SFFT')
                                 _hdl[0].header['FWHM_REF'] = (FWHM_REF, 'MeLOn: SFFT')
                                 _hdl[0].header['FWHM_SCI'] = (FWHM_SCI, 'MeLOn: SFFT')
                                 _hdl[0].header['KERORDER'] = (self.KerPolyOrder, 'MeLOn: SFFT')
                                 _hdl[0].header['BGORDER'] = (self.BGPolyOrder, 'MeLOn: SFFT')
                                 _hdl[0].header['CPHOTR'] = (str(self.ConstPhotRatio), 'MeLOn: SFFT')
                                 _hdl[0].header['KERHW'] = (KerHW, 'MeLOn: SFFT')
                                 _hdl[0].header['CONVD'] = (ConvdSide, 'MeLOn: SFFT')
+
+                                if ConvdSide == 'SCI':
+                                    GAIN_SCI = _hdl[0].header[self.GAIN_KEY]
+                                    SATUR_SCI = _hdl[0].header[self.SATUR_KEY]
+                                    GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN
+                                    SATUR_DIFF = SATUR_SCI * SFFT_FSCAL_MEAN
+
+                                    _hdl[0].header[self.GAIN_KEY] = (GAIN_DIFF, 'MeLOn: SFFT')
+                                    _hdl[0].header[self.SATUR_KEY] = (SATUR_DIFF, 'MeLOn: SFFT')
+
                                 _hdl.writeto(FITS_DIFF, overwrite=True)
                                 _hdl.close()
                             
                             # * Save solution array
                             if FITS_Solution is not None:
                                 phdu = fits.PrimaryHDU()
                                 phdu.header['N0'] = (SFFTConfig[0]['N0'], 'MeLOn: SFFT')
@@ -468,38 +633,67 @@
                                 phdu.header['FIJAB'] = (SFFTConfig[0]['Fijab'], 'MeLOn: SFFT')
 
                                 PixA_Solution = Solution.reshape((-1, 1))
                                 phdu.data = PixA_Solution.T
                                 fits.HDUList([phdu]).writeto(FITS_Solution, overwrite=True)
 
                         NEW_STATUS = 2
-                        _message = 'Successful Subtraction for task-[%d] ' %taskidx_acquired
-                        _message += 'in Subtraction thread-[%d]!' %INDEX_THREAD_4SUBTRACT
-                        print('\nMeLOn CheckPoint: %s' %_message)
-
-                    except:
-                        # ** free GPU memory when the subtraction fails
-                        import cupy as cp
-                        with cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT)):
-                            mempool = cp.get_default_memory_pool()
-                            pinned_mempool = cp.get_default_pinned_memory_pool()
-                            mempool.free_all_blocks()
-                            pinned_mempool.free_all_blocks()
+                        if self.VERBOSE_LEVEL in [1, 2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _message += 'SUCCESSFUL SFFT-SUBTRACTION!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
+                    
+                    except Exception as e:
+                        PixA_DIFF, Solution = None, None
+                        SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = np.nan, np.nan
+
+                        # ** clean GPU memory when the subtraction fails
+                        mempool = cp.get_default_memory_pool()
+                        pinned_mempool = cp.get_default_pinned_memory_pool()
+                        mempool.free_all_blocks()
+                        pinned_mempool.free_all_blocks()
+                        
+                        GPU_MEMORY_CLEANED = True
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _message += 'CLEAN GPU-[%s] MEMORY!' %CUDA_DEVICE_4SUBTRACT
+                            print('\nMeLOn CheckPoint: %s' %_message)
 
                         NEW_STATUS = -2
-                        _error_message = 'UnSuccessful Subtraction for task-[%d] ' %taskidx_acquired
-                        _error_message += 'in Subtraction thread-[%d]!' %INDEX_THREAD_4SUBTRACT
-                        print('\nMeLOn ERROR: %s' %_error_message)
                         Solution = None
                         PixA_DIFF = None
+                        if self.VERBOSE_LEVEL in [0, 1, 2]:
+                            print(e, file=sys.stderr)
+                            _error_message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _error_message += 'FAILED SFFT-SUBTRACTION!'
+                            print('\nMeLOn ERROR: %s' %_error_message)
 
                     with lock:
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = NEW_STATUS
-                        DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['Solution'] = Solution
-                        DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['PixA_DIFF'] = PixA_DIFF
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = NEW_STATUS
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['PixA_DIFF'] = PixA_DIFF
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['Solution'] = Solution
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFT_FSCAL_MEAN'] = SFFT_FSCAL_MEAN
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFT_FSCAL_SIG'] = SFFT_FSCAL_SIG
+
+            if self.CLEAN_GPU_MEMORY:
+                if not GPU_MEMORY_CLEANED:
+                    mempool = cp.get_default_memory_pool()
+                    pinned_mempool = cp.get_default_pinned_memory_pool()
+                    mempool.free_all_blocks()
+                    pinned_mempool.free_all_blocks()
+                    
+                    if self.VERBOSE_LEVEL in [1, 2]:
+                        _message = 'THREAD-4SUBTRACT-[%d]: ' %INDEX_THREAD_4SUBTRACT
+                        _message += 'FINAL CLEAN GPU-[%s] MEMORY ' %CUDA_DEVICE_4SUBTRACT
+                        print('\nMeLOn CheckPoint: %s' %_message)
+                else:
+                    if self.VERBOSE_LEVEL in [1, 2]:
+                        _message = 'THREAD-4SUBTRACT-[%d]: ' %INDEX_THREAD_4SUBTRACT
+                        _message += 'SKIP FINAL CLEAN, SINCE GPU-[%s] MEMORY ALREADY CLEANED' %CUDA_DEVICE_4SUBTRACT
+                        print('\nMeLOn CheckPoint: %s' %_message)
 
             return None
 
         # * trigger the threads for the preprocessing and subtraction
         MyThreadQueue = []
         for INDEX_THREAD_4PREPROC in range(NUM_THREADS_4PREPROC):
             MyThread = threading.Thread(target=FUNC_4PREPROC, args=(INDEX_THREAD_4PREPROC,))
@@ -510,8 +704,13 @@
             MyThread = threading.Thread(target=FUNC_4SUBTRCT, args=(INDEX_THREAD_4SUBTRACT,))
             MyThreadQueue.append(MyThread)
             MyThread.start()
   
         for MyThread in MyThreadQueue:
             MyThread.join()
         
+        # * show a summary
+        if self.VERBOSE_LEVEL in [0, 1, 2]:
+            NUM_SUCCESS = np.sum(np.array([DICT_STATUS_BAR[task] for task in DICT_STATUS_BAR]) == 2)
+            print('\nMeLOn CheckPoint: SFFT PROCESSED TASKS SUCCESSFULLY [%d / %d]!' %(NUM_SUCCESS, self.NUM_TASK))
+        
         return DICT_STATUS_BAR, DICT_PRODUCTS
```

### Comparing `sfft-1.3.4/sfft/MultiEasySparsePacket.py` & `sfft-1.4.0/sfft/MultiEasySparsePacket.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+import sys
 import time
-import math
 import warnings
 import threading
+import cupy as cp
 import numpy as np
 import os.path as pa
 from astropy.io import fits
 import scipy.ndimage as ndimage
 from astropy.table import Column
 from sfft.AutoSparsePrep import Auto_SparsePrep
 from sfft.utils.meta.TimeoutKit import TimeoutAfter
-# version: Sep 16, 2022
+from sfft.utils.SFFTSolutionReader import Realize_FluxScaling
+from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+# version: Mar 18, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class MultiEasy_SparsePacket:
     def __init__(self, FITS_REF_Queue, FITS_SCI_Queue, FITS_DIFF_Queue=[], FITS_Solution_Queue=[], \
         ForceConv_Queue=[], GKerHW_Queue=[], KerHWRatio=2.0, KerHWLimit=(2, 20), KerPolyOrder=2, BGPolyOrder=0, \
         ConstPhotRatio=True, MaskSatContam=False, GAIN_KEY='GAIN', SATUR_KEY='ESATUR', BACK_TYPE='MANUAL', \
-        BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=2.0, DETECT_MINAREA=5, \
+        BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=2.0, ANALYSIS_THRESH=2.0, DETECT_MINAREA=5, \
         DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', ONLY_FLAGS=[0], BoundarySIZE=30, \
-        XY_PriorSelect_Queue=[], Hough_FRLowerLimit=0.1, Hough_peak_clip=0.7, BeltHW=0.2, PS_ELLIPThresh=0.3, \
+        XY_PriorSelect_Queue=[], Hough_MINFR=0.1, Hough_PeakClip=0.7, BeltHW=0.2, PointSource_MINELLIP=0.3, \
         MatchTol=None, MatchTolFactor=3.0, COARSE_VAR_REJECTION=True, CVREJ_MAGD_THRESH=0.12, \
         ELABO_VAR_REJECTION=True, EVREJ_RATIO_THREH=5.0, EVREJ_SAFE_MAGDEV=0.04, StarExt_iter=4, \
-        XY_PriorBan_Queue=[], PostAnomalyCheck=False, PAC_RATIO_THRESH=5.0):
+        XY_PriorBan_Queue=[], PostAnomalyCheck=False, PAC_RATIO_THRESH=5.0, CLEAN_GPU_MEMORY=False, VERBOSE_LEVEL=2):
 
         """
-        # NOTE: This function is to Perform Sparse-Flavor SFFT for multiple tasks:
-        #       @ it makes sense when users have multiple CPU threads and GPU(s) available.
-        #       @ WARNING: the module currently only support Cupy backend!
+        # NOTE: This function is to perform Sparse-Flavor SFFT for multiple tasks:
+        #       @ this module (only support Cupy backend) would help making the 
+        #         best use of the available CPU and GPU resources.
 
         * Parameters for Sparse-Flavor SFFT [multiple tasks]
 
         # ----------------------------- Computing Enviornment [Cupy backend ONLY] --------------------------------- #
 
         -NUM_THREADS_4PREPROC [8]           # the number of Python threads for preprocessing.
                                             # WARNING: Empirically, the current code is only optimized for 
@@ -42,15 +46,16 @@
 
         -NUM_THREADS_4SUBTRACT [1]          # the number of Python threads for sfft subtraction.
                                             # says, if you have four GPU cards, then set it to 4.
                                             # NOTE: please do not confused the Python threads 
                                             #       with the CUDA threads (block, threads ...).
 
         -CUDA_DEVICES_4SUBTRACT [['0']]     # it specifies certain GPU devices (indices) to conduct the subtractions.
-                                            # the GPU devices are usually numbered 0 to N-1 (you may use command nvidia-smi to check).
+                                            # the GPU devices are usually numbered 0 to N-1.
+                                            # (you may use command nvidia-smi to check for Nvidia GPU devices).
 
         -TIMEOUT_4PREPROC_EACHTASK [300]    # timeout of each task during preprocessing.
                                             
         -TIMEOUT_4SUBTRACT_EACHTASK [300]   # timeout of each task during sfft subtraction.
 
         # ----------------------------- Preprocessing with Source Selection for Image-Masking --------------------------------- #
 
@@ -82,14 +87,17 @@
 
         -DETECT_THRESH [2.0]                # SExtractor Parameter DETECT_THRESH
                                             # NOTE: One may notice that the default DETECT_THRESH in SExtractor is 1.5,
                                             #       Using a 'cold' detection threshold here is to speed up SExtractor.
                                             #       Although DETECT_THRESH = 2.0 means we will miss the faint-end sources with 
                                             #       SNR < 9 (approximately), the cost is generally acceptable for source selection.
 
+        -ANALYSIS_THRESH [2.0]              # SExtractor Parameter ANALYSIS_THRESH
+                                            # NOTE: By default, let -ANALYSIS_THRESH = -DETECT_THRESH
+
         -DETECT_MINAREA [5]                 # SExtractor Parameter DETECT_MINAREA
         
         -DETECT_MAXAREA [0]                 # SExtractor Parameter DETECT_MAXAREA
 
         -DEBLEND_MINCONT [0.005]            # SExtractor Parameter DEBLEND_MINCONT (typically, 0.001 - 0.005)
 
         -BACKPHOTO_TYPE ['LOCAL']           # SExtractor Parameter BACKPHOTO_TYPE
@@ -109,31 +117,31 @@
         -XY_PriorSelect_Queue [[]]      # A queue of -XY_PriorSelect in sfft.Easy_SparsePacket.
                                         # Recall -XY_PriorSelect: 
                                         # a Numpy array of pixels coordinates, 
                                         # with shape (N, 2) (e.g., [[x0, y0], [x1, y1], ...]).
                                         # this allows sfft to us a prior source selection to solve the subtraction.
                                         # NOTE: ONLY WORKS FOR Auto-Sparse-Prep [SEMI-AUTO] MODE
 
-        -Hough_FRLowerLimit [0.1]       # The lower bound of FLUX_RATIO for line feature detection using Hough transformation.
+        -Hough_MINFR [0.1]              # The lower bound of FLUX_RATIO for line feature detection using Hough transformation.
                                         # Setting a proper lower bound can avoid to detect some line features by chance,
                                         # which are not contributed from point sources but resides in the small-FLUX_RATIO region.
-                                        # NOTE: Recommended values of Hough_FRLowerLimit: 0.1 ~ 1.0
+                                        # NOTE: Recommended values of Hough_MINFR: 0.1 ~ 1.0
                                         # NOTE: ONLY WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE
 
-        -Hough_peak_clip [0.7]          # It determines the lower bound of the sensitivity of the line feature detection.
+        -Hough_PeakClip [0.7]           # It determines the lower bound of the sensitivity of the line feature detection.
                                         # NOTE: When the point-source-belt is not very pronounced (e.g., in galaxy dominated fields),
                                         #       one may consider to reduce the parameter from default 0.7 to, says, ~ 0.4.
                                         # NOTE: ONLY WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE
 
         -BeltHW [0.2]                   # The half-width of point-source-belt detected by Hough Transformation.
                                         # Remarks: if you want to tune this parameter, it is helpful to draw 
                                         #          a figure of MAG_AUTO against FLUX_RADIUS.
                                         # NOTE: IT WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE :::: determine point-source-belt
 
-        -PS_ELLIPThresh [0.3]           # An additiona Restriction on ELLIPTICITY (ELLIPTICITY < PS_ELLIPThresh) for point sources.
+        -PointSource_MINELLIP [0.3]     # An additiona Restriction on ELLIPTICITY (ELLIPTICITY < PointSource_MINELLIP) for point sources.
                                         # NOTE: IT WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE :::: determine point-sources
                                     
         -MatchTol [None]                # Given separation tolerance (pix) for source matching 
                                         # NOTE: IT WORKS FOR Auto-Sparse-Prep [HOUGH-AUTO] MODE :::: Cross-Match between REF & SCI
                                         # NOTE: IT WORKS FOR Auto-Sparse-Prep [SEMI-AUTO] MODE :::: Cross-Match between REF & SCI AND
                                         #       Cross-Match between the prior selection and mean image coordinates of matched REF-SCI sources.
 
@@ -255,15 +263,22 @@
                                             # Recall -FITS_SCI: File path of input science image.
 
         -FITS_DIFF_Queue [[]]               # A queue of -FITS_DIFF in sfft.Easy_SparsePacket.
                                             # Recall -FITS_DIFF:File path of output difference image.
 
         -FITS_Solution_Queue [[]]           # A queue of -FITS_Solution in sfft.Easy_SparsePacket.
                                             # Recall -FITS_Solution: File path of the solution of the linear system. 
-                                            #   it is an array of (..., a_ijab, ... b_pq, ...).
+                                            # it is an array of (..., a_ijab, ... b_pq, ...).
+
+        # ----------------------------- Miscellaneous --------------------------------- #
+        
+        -CLEAN_GPU_MEMORY [False]           # Clean GPU memory or not after all subtractions done in a GPU device.
+
+        -VERBOSE_LEVEL [2]                  # The level of verbosity, can be [0, 1, 2]
+                                            # 0/1/2: QUIET/NORMAL/FULL mode
 
         # Important Notice:
         #
         # a): if reference is convolved in SFFT, then DIFF = SCI - Convolved_REF.
         #     [difference image is expected to have PSF & flux zero-point consistent with science image]
         #     e.g., -ForceConv='REF' or -ForceConv='AUTO' when reference has better seeing.
         #
@@ -271,15 +286,15 @@
         #     [difference image is expected to have PSF & flux zero-point consistent with reference image]
         #     e.g., -ForceConv='SCI' or -ForceConv='AUTO' when science has better seeing.
         #
         # Remarks: this convention is to guarantee that transients emerge on science image always 
         #          show a positive signal on difference images.
 
         """
-
+        
         self.FITS_REF_Queue = FITS_REF_Queue
         self.FITS_SCI_Queue = FITS_SCI_Queue
         self.NUM_TASK = len(FITS_SCI_Queue)
 
         self.KerHWRatio = KerHWRatio
         self.KerHWLimit = KerHWLimit
         self.KerPolyOrder = KerPolyOrder
@@ -291,213 +306,270 @@
         self.SATUR_KEY = SATUR_KEY
         self.BACK_TYPE = BACK_TYPE
         self.BACK_VALUE = BACK_VALUE
         self.BACK_SIZE = BACK_SIZE
         self.BACK_FILTERSIZE = BACK_FILTERSIZE
         
         self.DETECT_THRESH = DETECT_THRESH
+        self.ANALYSIS_THRESH = ANALYSIS_THRESH
         self.DETECT_MINAREA = DETECT_MINAREA
         self.DETECT_MAXAREA = DETECT_MAXAREA
         self.DEBLEND_MINCONT = DEBLEND_MINCONT
         self.BACKPHOTO_TYPE = BACKPHOTO_TYPE
         self.ONLY_FLAGS = ONLY_FLAGS
         self.BoundarySIZE = BoundarySIZE
 
-        self.Hough_FRLowerLimit = Hough_FRLowerLimit
-        self.Hough_peak_clip = Hough_peak_clip
+        self.Hough_MINFR = Hough_MINFR
+        self.Hough_PeakClip = Hough_PeakClip
         self.BeltHW = BeltHW
-        self.PS_ELLIPThresh = PS_ELLIPThresh
+        self.PointSource_MINELLIP = PointSource_MINELLIP
 
         self.MatchTol = MatchTol
         self.MatchTolFactor = MatchTolFactor
 
         self.COARSE_VAR_REJECTION = COARSE_VAR_REJECTION
         self.CVREJ_MAGD_THRESH = CVREJ_MAGD_THRESH
         self.ELABO_VAR_REJECTION = ELABO_VAR_REJECTION
         self.EVREJ_RATIO_THREH = EVREJ_RATIO_THREH
         self.EVREJ_SAFE_MAGDEV = EVREJ_SAFE_MAGDEV
         
         self.StarExt_iter = StarExt_iter
 
         self.PostAnomalyCheck = PostAnomalyCheck
         self.PAC_RATIO_THRESH = PAC_RATIO_THRESH
-        
+
+        self.CLEAN_GPU_MEMORY = CLEAN_GPU_MEMORY
+        self.VERBOSE_LEVEL = VERBOSE_LEVEL
+
         if FITS_DIFF_Queue == []:
-            _warn_message = 'Argument FITS_DIFF_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument FITS_DIFF_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.FITS_DIFF_Queue = [None] * self.NUM_TASK
         else: self.FITS_DIFF_Queue = FITS_DIFF_Queue
         
         if FITS_Solution_Queue == []:
-            _warn_message = 'Argument FITS_Solution_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument FITS_Solution_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.FITS_Solution_Queue = [None] * self.NUM_TASK
         else: self.FITS_Solution_Queue = FITS_Solution_Queue
         
         if ForceConv_Queue == []:
-            _warn_message = 'Argument ForceConv_Queue is EMPTY then Use default [...AUTO...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'Argument ForceConv_Queue is EMPTY then Use default [...AUTO...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.ForceConv_Queue = ['AUTO'] * self.NUM_TASK
         else: self.ForceConv_Queue = ForceConv_Queue
 
         if GKerHW_Queue == []:
-            _warn_message = 'Argument GKerHW_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument GKerHW_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.GKerHW_Queue = [None] * self.NUM_TASK
         else: self.GKerHW_Queue = GKerHW_Queue
 
         if XY_PriorSelect_Queue == []:
-            _warn_message = 'Argument XY_PriorSelect_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument XY_PriorSelect_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.XY_PriorSelect_Queue = [None] * self.NUM_TASK
         else: self.XY_PriorSelect_Queue = XY_PriorSelect_Queue
 
         if XY_PriorBan_Queue == []:
-            _warn_message = 'Argument XY_PriorBan_Queue is EMPTY then Use default [...None...] instead!'
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [2]:
+                _warn_message = 'Argument XY_PriorBan_Queue is EMPTY then Use default [...None...] instead!'
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
             self.XY_PriorBan_Queue = [None] * self.NUM_TASK
         else: self.XY_PriorBan_Queue = XY_PriorBan_Queue
 
+        if self.PostAnomalyCheck:
+            if self.VERBOSE_LEVEL in [2]:    
+                warnings.warn('\nMeLOn REMINDER: Post-Anomaly Check requires correct GAIN values!')
+
+        if self.VERBOSE_LEVEL in [2]:
+            warnings.warn('\nMeLOn REMINDER: Input images for sparse-flavor sfft should be SKY-SUBTRACTED!')
+
     def MESP_Cupy(self, NUM_THREADS_4PREPROC=8, NUM_THREADS_4SUBTRACT=1, CUDA_DEVICES_4SUBTRACT=['0'], \
         TIMEOUT_4PREPROC_EACHTASK=300, TIMEOUT_4SUBTRACT_EACHTASK=300):
 
         # * define task-oriented dictionaries of status-bar and products
         #   status 0: Initial State
         #   status 1: Preprocessing SUCCESS || status -1: Preprocessing FAIL
         #   status 2: Subtraction SUCCESS || status -2: Subtraction FAIL
         #   status 32: Preprocessing is IN-PROGRESS ...
         #   status 64: Subtraction is IN-PROGRESS ...
         #   NOTE: Subtraction would not be triggered when Preprocessing fails
     
         _RATIO = self.NUM_TASK / NUM_THREADS_4PREPROC
         if _RATIO > 4.0:
-            _warn_message = 'THIS FUNCTION IS NOT OPTIMIZED FOR RATIO OF '
-            _warn_message += 'NUM_TASK / NUM_THREADS_4PREPROC BEING TO HIGH [%.1f > 4.0]!' %_RATIO
-            warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
+            if self.VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'THIS FUNCTION IS NOT OPTIMIZED FOR RATIO OF '
+                _warn_message += 'NUM_TASK / NUM_THREADS_4PREPROC BEING TO HIGH [%.1f > 4.0]!' %_RATIO
+                warnings.warn('\nMeLOn WARNING: %s' %_warn_message)
 
         BACKEND_4SUBTRACT = 'Cupy'
         taskidx_lst = np.arange(self.NUM_TASK)
         assert NUM_THREADS_4SUBTRACT == len(CUDA_DEVICES_4SUBTRACT)
 
-        DICT_STATUS_BAR = {'task-[%d]' %taskidx: 0 for taskidx in taskidx_lst}
-        DICT_PRODUCTS = {'task-[%d]' %taskidx: {} for taskidx in taskidx_lst}
+        DICT_STATUS_BAR = {'TASK-[%d]' %taskidx: 0 for taskidx in taskidx_lst}
+        DICT_PRODUCTS = {'TASK-[%d]' %taskidx: {} for taskidx in taskidx_lst}
         lock = threading.RLock()
 
         # * define the function for preprocessing (see sfft.EasySparsePacket)
         def FUNC_4PREPROC(INDEX_THREAD_4PREPROC):
             
             THREAD_ALIVE_4PREPROC = True
             while THREAD_ALIVE_4PREPROC:
                 with lock:
-                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['task-[%d]' %taskidx] for taskidx in taskidx_lst])
+                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['TASK-[%d]' %taskidx] for taskidx in taskidx_lst])
                     OPEN_MASK_4PREPROC = STATUS_SNAPSHOT == 0
                     if np.sum(OPEN_MASK_4PREPROC) > 0:
                         taskidx_acquired = taskidx_lst[OPEN_MASK_4PREPROC][0]
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = 32
-                        _message = 'Preprocessing thread-[%d] ACQUIRED task-[%d]!' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
-                        print('\nMeLOn CheckPoint: %s' %_message)
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = 32
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4PREPROC-[%d] ACQUIRED TASK-[%d] ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                            _message += '(Sparse-Flavor Auto Preprocessing)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
                     else: 
                         THREAD_ALIVE_4PREPROC = False
                         taskidx_acquired = None
-                        _message = 'TERMINATE Preprocessing thread-[%d] AS NO TASK WILL BE ALLOCATED!' %INDEX_THREAD_4PREPROC
-                        print('\nMeLOn CheckPoint: %s' %_message)
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4PREPROC-[%d] TERMINATED ' %INDEX_THREAD_4PREPROC
+                            _message += 'SINCE NO MORE TASK WILL BE ALLOCATED '
+                            _message += '(Sparse-Flavor Auto Preprocessing)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
 
                 if taskidx_acquired is not None:
                     FITS_REF = self.FITS_REF_Queue[taskidx_acquired]
                     FITS_SCI = self.FITS_SCI_Queue[taskidx_acquired]
                     XY_PriorBan = self.XY_PriorBan_Queue[taskidx_acquired]
                     XY_PriorSelect = self.XY_PriorSelect_Queue[taskidx_acquired]
 
                     try:
                         with TimeoutAfter(timeout=TIMEOUT_4PREPROC_EACHTASK, exception=TimeoutError):
-                            warnings.warn('\nMeLOn WARNING: Input images for sparse-flavor sfft should be SKY-SUBTRACTED !!!')
 
-                            # ** perform auto sparse-prep
+                            # ** perform Auto-Sparse-Prep
                             _ASP = Auto_SparsePrep(FITS_REF=FITS_REF, FITS_SCI=FITS_SCI, GAIN_KEY=self.GAIN_KEY, \
                                 SATUR_KEY=self.SATUR_KEY, BACK_TYPE=self.BACK_TYPE, BACK_VALUE=self.BACK_VALUE, \
-                                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, DETECT_THRESH=self.DETECT_THRESH, \
-                                DETECT_MINAREA=self.DETECT_MINAREA, DETECT_MAXAREA=self.DETECT_MAXAREA, DEBLEND_MINCONT=self.DEBLEND_MINCONT, \
-                                BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, ONLY_FLAGS=self.ONLY_FLAGS, BoundarySIZE=self.BoundarySIZE)
+                                BACK_SIZE=self.BACK_SIZE, BACK_FILTERSIZE=self.BACK_FILTERSIZE, \
+                                DETECT_THRESH=self.DETECT_THRESH, ANALYSIS_THRESH=self.ANALYSIS_THRESH, \
+                                DETECT_MINAREA=self.DETECT_MINAREA, DETECT_MAXAREA=self.DETECT_MAXAREA, \
+                                DEBLEND_MINCONT=self.DEBLEND_MINCONT, BACKPHOTO_TYPE=self.BACKPHOTO_TYPE, \
+                                ONLY_FLAGS=self.ONLY_FLAGS, BoundarySIZE=self.BoundarySIZE, \
+                                VERBOSE_LEVEL=self.VERBOSE_LEVEL)
 
                             if XY_PriorSelect is None:
                                 IMAGE_MASK_METHOD = 'HOUGH-AUTO'
-                                print('MeLOn CheckPoint: TRIGGER Auto-Sparse-Prep [%s] MODE for task-[%d]!' %(IMAGE_MASK_METHOD, taskidx_acquired))
-                                SFFTPrepDict = _ASP.HoughAutoMask(Hough_FRLowerLimit=self.Hough_FRLowerLimit, \
-                                    Hough_peak_clip=self.Hough_peak_clip, BeltHW=self.BeltHW, PS_ELLIPThresh=self.PS_ELLIPThresh, \
-                                    MatchTol=self.MatchTol, MatchTolFactor=self.MatchTolFactor, ELABO_VAR_REJECTION=self.ELABO_VAR_REJECTION, \
+                                if self.VERBOSE_LEVEL in [1, 2]:
+                                    _message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                                    _message += 'TRIGGER Sparse-Flavor Auto Preprocessing [%s] MODE!' %IMAGE_MASK_METHOD
+                                    print('MeLOn CheckPoint: %s' %_message)
+                                
+                                SFFTPrepDict = _ASP.HoughAutoMask(Hough_MINFR=self.Hough_MINFR, \
+                                    Hough_PeakClip=self.Hough_PeakClip, BeltHW=self.BeltHW, \
+                                    PointSource_MINELLIP=self.PointSource_MINELLIP, MatchTol=self.MatchTol, \
+                                    MatchTolFactor=self.MatchTolFactor, ELABO_VAR_REJECTION=self.ELABO_VAR_REJECTION, \
                                     EVREJ_RATIO_THREH=self.EVREJ_RATIO_THREH, EVREJ_SAFE_MAGDEV=self.EVREJ_SAFE_MAGDEV, \
                                     StarExt_iter=self.StarExt_iter, XY_PriorBan=XY_PriorBan)
-                            
-                            if XY_PriorSelect is not None:
+                            else:
                                 IMAGE_MASK_METHOD = 'SEMI-AUTO'
-                                print('MeLOn CheckPoint: TRIGGER Auto-Sparse-Prep [%s] MODE for task-[%d]!' %(IMAGE_MASK_METHOD, taskidx_acquired))
+                                if self.VERBOSE_LEVEL in [1, 2]:
+                                    _message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                                    _message += 'TRIGGER Sparse-Flavor Auto Preprocessing [%s] MODE!' %IMAGE_MASK_METHOD
+                                    print('MeLOn CheckPoint: %s' %_message)
+
                                 SFFTPrepDict = _ASP.SemiAutoMask(XY_PriorSelect=XY_PriorSelect, MatchTol=self.MatchTol, \
                                     MatchTolFactor=self.MatchTolFactor, StarExt_iter=self.StarExt_iter)
 
                         NEW_STATUS = 1
-                        _message = 'Successful Preprocessing for task-[%d] ' %taskidx_acquired
-                        _message += 'in Preprocessing thread-[%d]!' %INDEX_THREAD_4PREPROC
-                        print('\nMeLOn CheckPoint: %s' %_message)
-                    except:
+                        if self.VERBOSE_LEVEL in [1, 2]:
+                            _message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                            _message += 'SUCCESSFUL Sparse-Flavor Auto Preprocessing!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
+
+                    except Exception as e:
                         NEW_STATUS = -1
-                        _error_message = 'UnSuccessful Preprocessing for task-[%d] ' %taskidx_acquired
-                        _error_message += 'in Preprocessing thread-[%d]!' %INDEX_THREAD_4PREPROC
-                        print('\nMeLOn ERROR: %s' %_error_message)
                         SFFTPrepDict = None
-            
+                        if self.VERBOSE_LEVEL in [0, 1, 2]:
+                            print(e, file=sys.stderr)
+                            _error_message = 'THREAD-4PREPROC-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4PREPROC, taskidx_acquired)
+                            _error_message += 'FAILED Sparse-Flavor Auto Preprocessing!'
+                            print('\nMeLOn ERROR: %s' %_error_message)
+
                     with lock:
                         # NOTE: IN FACT, THERE IS NO RISK HERE EVEN WITHOUT LOCK.
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = NEW_STATUS
-                        DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['SFFTPrepDict'] = SFFTPrepDict
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = NEW_STATUS
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFTPrepDict'] = SFFTPrepDict
 
             return None
 
         # * define the function for sfft subtraction (see sfft.EasySparsePacket)
         def FUNC_4SUBTRCT(INDEX_THREAD_4SUBTRACT):
             
             CUDA_DEVICE_4SUBTRACT = CUDA_DEVICES_4SUBTRACT[INDEX_THREAD_4SUBTRACT]
+            device = cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT))
+            device.use()
+
             THREAD_ALIVE_4SUBTRCT = True
+            GPU_MEMORY_CLEANED = True
+
             while THREAD_ALIVE_4SUBTRCT:
                 SHORT_PAUSE = False
+
                 with lock:
-                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['task-[%d]' %taskidx] for taskidx in taskidx_lst])
+                    STATUS_SNAPSHOT = np.array([DICT_STATUS_BAR['TASK-[%d]' %taskidx] for taskidx in taskidx_lst])
                     OPEN_MASK_4SUBTRACT = STATUS_SNAPSHOT == 1
                     WAIT_MASK_4SUBTRACT = np.in1d(STATUS_SNAPSHOT, [0, 32])
+
                     if np.sum(OPEN_MASK_4SUBTRACT) > 0:
                         taskidx_acquired = taskidx_lst[OPEN_MASK_4SUBTRACT][0]
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = 64
-                        _message = 'Subtraction thread-[%d] ACQUIRED task-[%d]!' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
-                        print('\nMeLOn CheckPoint: %s' %_message)
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = 64
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] ACQUIRED TASK-[%d] ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _message += '(SFFT-SUBTRACTION)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
+
                     elif np.sum(WAIT_MASK_4SUBTRACT) > 0:
                         SHORT_PAUSE = True
                         taskidx_acquired = None
+
                     else:
                         THREAD_ALIVE_4SUBTRCT = False
                         taskidx_acquired = None
-                        _message = 'TERMINATE Subtraction thread-[%d] AS NO TASK WILL BE ALLOCATED!' %INDEX_THREAD_4SUBTRACT
-                        print('\nMeLOn CheckPoint: %s' %_message)
+
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] TERMINATED ' %INDEX_THREAD_4SUBTRACT
+                            _message += 'SINCE NO MORE TASK WILL BE ALLOCATED '
+                            _message += '(SFFT-SUBTRACTION)!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
 
                 if SHORT_PAUSE:
                     # run a short sleep, otherwise this thread may always hold the lock by the while loop
                     time.sleep(0.01)
                 
                 if taskidx_acquired is not None:
+
                     FITS_REF = self.FITS_REF_Queue[taskidx_acquired]
                     FITS_SCI = self.FITS_SCI_Queue[taskidx_acquired]
                     FITS_DIFF = self.FITS_DIFF_Queue[taskidx_acquired]
                     FITS_Solution = self.FITS_Solution_Queue[taskidx_acquired]
                     ForceConv = self.ForceConv_Queue[taskidx_acquired]
                     GKerHW = self.GKerHW_Queue[taskidx_acquired]
 
                     with lock:
                         # NOTE: IN FACT, THERE IS NO RISK HERE EVEN WITHOUT LOCK.
-                        SFFTPrepDict = DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['SFFTPrepDict']
+                        SFFTPrepDict = DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFTPrepDict']
                     
                     try:
                         with TimeoutAfter(timeout=TIMEOUT_4SUBTRACT_EACHTASK, exception=TimeoutError):                    
+                            
                             # * Determine ConvdSide & KerHW
                             FWHM_REF = SFFTPrepDict['FWHM_REF']
                             FWHM_SCI = SFFTPrepDict['FWHM_SCI']
 
                             assert ForceConv in ['AUTO', 'REF', 'SCI']
                             if ForceConv == 'AUTO':
                                 if FWHM_SCI >= FWHM_REF: ConvdSide = 'REF'
@@ -507,27 +579,39 @@
                             if GKerHW is None:
                                 FWHM_La = np.max([FWHM_REF, FWHM_SCI])
                                 KerHW = int(np.clip(self.KerHWRatio * FWHM_La, \
                                                     self.KerHWLimit[0], self.KerHWLimit[1]))
                             else: KerHW = GKerHW
                             
                             # * Compile Functions in SFFT Subtraction
-                            from sfft.sfftcore.SFFTConfigure import SingleSFFTConfigure
+                            
 
                             PixA_REF = SFFTPrepDict['PixA_REF']
                             PixA_SCI = SFFTPrepDict['PixA_SCI']
+                            
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'TRIGGER Function Compilations of SFFT-SUBTRACTION'
+                                print('MeLOn CheckPoint: %s' %_message)
 
                             Tcomp_start = time.time()
-                            SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], KerHW=KerHW, \
-                                KerPolyOrder=self.KerPolyOrder, BGPolyOrder=self.BGPolyOrder, ConstPhotRatio=self.ConstPhotRatio, \
-                                BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
-                            print('\nMeLOn Report: Compiling Functions in SFFT Subtraction Takes [%.3f s]' %(time.time() - Tcomp_start))
+                            GPU_MEMORY_CLEANED = False
+                            SFFTConfig = SingleSFFTConfigure.SSC(NX=PixA_REF.shape[0], NY=PixA_REF.shape[1], \
+                                KerHW=KerHW, KerPolyOrder=self.KerPolyOrder, BGPolyOrder=self.BGPolyOrder, \
+                                ConstPhotRatio=self.ConstPhotRatio, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
+                                VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'Function Compilations of SFFT-SUBTRACTION '
+                                _message += 'TAKES [%.3f s]!' %(time.time() - Tcomp_start)
+                                print('\nMeLOn Report: %s' %_message)
 
                             # * Perform SFFT Subtraction
-                            from sfft.sfftcore.SFFTSubtract import GeneralSFFTSubtract
+                            
 
                             SatMask_REF = SFFTPrepDict['REF-SAT-Mask']
                             SatMask_SCI = SFFTPrepDict['SCI-SAT-Mask']
                             NaNmask_U = SFFTPrepDict['Union-NaN-Mask']
                             PixA_mREF = SFFTPrepDict['PixA_mREF']
                             PixA_mSCI = SFFTPrepDict['PixA_mSCI']
 
@@ -551,78 +635,145 @@
                                     PixA_J[NaNmask_U] = PixA_mJ[NaNmask_U]
                                 else: PixA_I, PixA_J = PixA_SCI, PixA_REF
                                 if self.MaskSatContam: 
                                     ContamMask_I = SatMask_SCI
                                     ContamMask_J = SatMask_REF
                                 else: ContamMask_I = None
 
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'TRIGGER Function Executions of SFFT-SUBTRACTION!'
+                                print('MeLOn CheckPoint: %s' %_message)
+
                             Tsub_start = time.time()
                             _tmp = GeneralSFFTSubtract.GSS(PixA_I=PixA_I, PixA_J=PixA_J, PixA_mI=PixA_mI, PixA_mJ=PixA_mJ, \
                                 SFFTConfig=SFFTConfig, ContamMask_I=ContamMask_I, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-                                CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
+                                VERBOSE_LEVEL=self.VERBOSE_LEVEL)
+                            
                             Solution, PixA_DIFF, ContamMask_CI = _tmp
-                            if self.MaskSatContam:
-                                ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
-                            print('\nMeLOn Report: SFFT Subtraction Takes [%.3f s]' %(time.time() - Tsub_start))
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'Function Executions of SFFT-SUBTRACTION'
+                                _message += 'TAKES [%.3f s]!' %(time.time() - Tsub_start)
+                                print('\nMeLOn Report: %s' %_message)
+
+                            # ** adjust the sign of difference image 
+                            #    NOTE: Our convention is to make the transients on SCI always show themselves as positive signal on DIFF
+                            #    (a) when REF is convolved, DIFF = SCI - Conv(REF)
+                            #    (b) when SCI is convolved, DIFF = Conv(SCI) - REF
 
+                            if ConvdSide == 'SCI':
+                                PixA_DIFF = -PixA_DIFF
+
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                if ConvdSide == 'REF':
+                                    _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                    _message += 'Reference Image is Convolved in SFFT-SUBTRACTION [DIFF = SCI - Conv(REF)]!'
+                                    print('MeLOn CheckPoint: %s' %_message)
+
+                                if ConvdSide == 'SCI':
+                                    _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                    _message += 'Science Image is Convolved in SFFT-SUBTRACTION [DIFF = Conv(SCI) - REF]!'
+                                    print('MeLOn CheckPoint: %s' %_message)
+
+                            # ** estimate the flux scaling through the convolution of image subtraction
+                            #    NOTE: if photometric ratio is not constant (ConstPhotRatio=False), we measure of a grid
+                            #          of coordinates to estimate the flux scaling and its fluctuation (polynomial form).
+                            #    NOTE: here we set the tile-size of the grid about 64 x 64 pix, but meanwhile, 
+                            #          we also require the tiles should no less than 6 along each axis.
+
+                            N0, N1 = SFFTConfig[0]['N0'], SFFTConfig[0]['N1']
+                            L0, L1 = SFFTConfig[0]['L0'], SFFTConfig[0]['L1']
+                            DK, Fpq = SFFTConfig[0]['DK'], SFFTConfig[0]['Fpq']
+
+                            if self.ConstPhotRatio:
+                                SFFT_FSCAL_NSAMP = 1
+                                XY_q = np.array([[N0/2.0, N1/2.0]]) + 0.5
+                                RFS = Realize_FluxScaling(XY_q=XY_q)
+                                SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+                                SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = SFFT_FSCAL_q[0], 0.0
+                            
+                            if not self.ConstPhotRatio:
+                                TILESIZE_X, TILESIZE_Y = 64, 64    # FIXME emperical/arbitrary values
+                                NTILE_X = np.max([round(N0/TILESIZE_X), 6])
+                                NTILE_Y = np.max([round(N1/TILESIZE_Y), 6])
+                                GX = np.linspace(0.5, N0+0.5, NTILE_X+1)
+                                GY = np.linspace(0.5, N1+0.5, NTILE_Y+1)
+                                YY, XX = np.meshgrid(GY, GX)
+                                XY_q = np.array([XX.flatten(), YY.flatten()]).T
+                                SFFT_FSCAL_NSAMP = XY_q.shape[0]
+                                
+                                RFS = Realize_FluxScaling(XY_q=XY_q)
+                                SFFT_FSCAL_q = RFS.FromArray(Solution=Solution, N0=N0, N1=N1, L0=L0, L1=L1, DK=DK, Fpq=Fpq)
+                                SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = np.mean(SFFT_FSCAL_q), np.std(SFFT_FSCAL_q)
+
+                            PHOT_FSCAL = 10**(SFFTPrepDict['MAG_OFFSET']/-2.5)  # FLUX_SCI/FLUX_REF
+                            if ConvdSide == 'SCI': PHOT_FSCAL = 1.0/PHOT_FSCAL
+
+                            if self.VERBOSE_LEVEL in [1, 2]:
+                                _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                _message += 'The Flux Scaling through the Convolution of SFFT-SUBTRACTION '
+                                _message += '[%.6f +/- %.6f] from [%d] positions!\n' %(SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG, SFFT_FSCAL_NSAMP)
+                                _message += 'P.S. The approximated Flux Scaling from Photometry [%.6f].' %PHOT_FSCAL
+                                print('MeLOn CheckPoint: %s' %_message)
+                            
+                            # ** run post anomaly check (PAC)
                             if self.PostAnomalyCheck:
-                                warnings.warn('\nMeLOn WARNING: Post-Anomaly Check requires correct GAIN values!')
-                                # TODO: Incorporate weight-maps of the input image pair for more accurate FLUXERR.
 
                                 """
                                 # Remarks on the Post Anomaly Check (PAC)
-                                # [1] Recall that Elaborate Variable Rejection (EVREJ) also use SExtractor photometric errors to identify variables.
-                                #     I would say, PAC should be more accurate than EVREJ.
+                                # [1] One may notice that Elaborate Variable Rejection (EVREJ) also use SExtractor 
+                                #     photometric errors to identify variables. However, PAC should be more accurate than EVREJ.
                                 #     NOTE: Bright transients (compared with its host) can be also identified by PAC.
                                 #
                                 # [2] distribution mean: image subtraction is expected to have better accuracy on the determination 
                                 #     of the photometric scaling, compared with the constant MAG_OFFSET in EVREJ. As a result,
                                 #     the flux change counted on the difference image is likely more 'real' than that in EVREJ.
                                 #
-                                # [3] distribution variance: i) inaccurate SExtractor FLUXERR especially at the bright end
-                                #     and ii) the error of MAG_OFFSET affect one FLUXERR scaling.
-                                #     NOTE: The imperfections on distribution variance are just same as EVREJ.
-                                #     NOTE: Using SFFT kernel sum would be better than MAG_OFFSET for scaling FLUXERR. 
-                                #           For simplicity, howerver, we use MAG_OFFSET (with error << 5%) which is good enough here.
+                                # [3] distribution variance: SExtractor FLUXERR_AUTO can be inaccurate, and the convolution effect
+                                #     on the photometric errors has been simplified as multiplying an average flux scaling on an image.
                                 #
                                 """
-                                
+
+                                if self.VERBOSE_LEVEL in [2]:
+                                    warnings.warn('\nMeLOn REMINDER: Post-Anomaly Check requires CORRECT GAIN in FITS HEADER!')
+
                                 AstSEx_SS = SFFTPrepDict['SExCatalog-SubSource']
                                 SFFTLmap = SFFTPrepDict['SFFT-LabelMap']
                                 
                                 # ** Only consider the Non-Prior-Banned SubSources
                                 if 'MASK_PriorBan' in AstSEx_SS.colnames:
                                     nPBMASK_SS = ~np.array(AstSEx_SS['MASK_PriorBan'])
                                     AstSEx_vSS = AstSEx_SS[nPBMASK_SS]
                                 else: AstSEx_vSS = AstSEx_SS
                                 
                                 # ** Estimate expected variance of Non-Prior-Banned SubSources on the difference
-                                MAG_OFFSET = SFFTPrepDict['MAG_OFFSET']
-                                FLUX_SCAL = 10**(MAG_OFFSET/-2.5)  # FLUX_SCI/FLUX_REF
-
                                 FLUXERR_vSSr = np.array(AstSEx_vSS['FLUXERR_AUTO_REF'])
                                 FLUXERR_vSSs = np.array(AstSEx_vSS['FLUXERR_AUTO_SCI'])
 
                                 if ConvdSide == 'REF':
-                                    sFLUXERR_vSSr = FLUXERR_vSSr * FLUX_SCAL
+                                    sFLUXERR_vSSr = FLUXERR_vSSr * SFFT_FSCAL_MEAN
                                     ExpDVAR_vSS = sFLUXERR_vSSr**2 + FLUXERR_vSSs**2
+
                                 if ConvdSide == 'SCI':
-                                    sFLUXERR_vSSs = FLUXERR_vSSs / FLUX_SCAL
+                                    sFLUXERR_vSSs = FLUXERR_vSSs * SFFT_FSCAL_MEAN
                                     ExpDVAR_vSS = FLUXERR_vSSr**2 + sFLUXERR_vSSs**2
 
                                 # ** Measure the ratios of Non-Prior-Banned SubSources on the difference for PAC
                                 SEGL_vSS = np.array(AstSEx_vSS['SEGLABEL']).astype(int)
                                 DFSUM_vSS = ndimage.labeled_comprehension(PixA_DIFF, SFFTLmap, SEGL_vSS, np.sum, float, 0.0)
                                 RATIO_vSS = DFSUM_vSS / np.clip(np.sqrt(ExpDVAR_vSS), a_min=1e-8, a_max=None)
                                 PAMASK_vSS = np.abs(RATIO_vSS) > self.PAC_RATIO_THRESH
 
-                                _message = 'FIND [%d] PostAnomaly SubSources [> %.2f sigma] ' %(np.sum(PAMASK_vSS), self.PAC_RATIO_THRESH)
-                                _message += 'out of [%d] Non-Prior-Banned SubSources!\n' %(len(AstSEx_vSS))
-                                _message += 'P.S. there are [%d] Prior-Banned SubSources!' %(len(AstSEx_SS) - len(AstSEx_vSS))
-                                print('\nMeLOn CheckPoint: %s' %_message)
+                                if self.VERBOSE_LEVEL in [1, 2]:
+                                    _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                                    _message += 'Identified [%d] PostAnomaly SubSources [> %.2f sigma] ' %(np.sum(PAMASK_vSS), self.PAC_RATIO_THRESH)
+                                    _message += 'out of [%d] Non-Prior-Banned SubSources!\n' %(len(AstSEx_vSS))
+                                    _message += 'P.S. there are [%d] Prior-Banned SubSources!' %(len(AstSEx_SS) - len(AstSEx_vSS))
+                                    print('\nMeLOn CheckPoint: %s' %_message)
                                 
                                 # ** Record the results (decorate AstSEx_SS in SFFTPrepDict)
                                 if 'MASK_PriorBan' in AstSEx_SS.colnames:
                                     ExpDVAR_SS = np.nan * np.ones(len(AstSEx_SS))       # NOTE Prior-Ban is trivial NaN
                                     DFSUM_SS = np.nan * np.ones(len(AstSEx_SS))         # NOTE Prior-Ban is trivial NaN
                                     RATIO_SS = np.nan * np.ones(len(AstSEx_SS))         # NOTE Prior-Ban is trivial NaN
                                     PAMASK_SS = np.zeros(len(AstSEx_SS)).astype(bool)   # NOTE Prior-Ban is trivial False
@@ -637,44 +788,70 @@
                                     RATIO_SS = RATIO_vSS
                                     PAMASK_SS = PAMASK_vSS
 
                                 AstSEx_SS.add_column(Column(ExpDVAR_SS, name='ExpDVAR_PostAnomaly'))
                                 AstSEx_SS.add_column(Column(DFSUM_SS, name='DFSUM_PostAnomaly'))
                                 AstSEx_SS.add_column(Column(RATIO_SS, name='RATIO_PostAnomaly'))
                                 AstSEx_SS.add_column(Column(PAMASK_SS, name='MASK_PostAnomaly'))
-
-                            # * Modifications on the difference image
-                            #   a) when REF is convolved, DIFF = SCI - Conv(REF)
-                            #      PSF_DIFF is coincident with SCI, transients on SCI are positive signal in DIFF.
-                            #   b) when SCI is convolved, DIFF = Conv(SCI) - REF
-                            #      PSF_DIFF is coincident with REF, transients on SCI are still positive signal in DIFF.
-
+                            
+                            # ** final tweaks on the difference image
                             if NaNmask_U is not None:
-                                # ** Mask Union-NaN region
-                                PixA_DIFF[NaNmask_U] = np.nan
+                                PixA_DIFF[NaNmask_U] = np.nan   # Mask Union-NaN regions
+                            
                             if self.MaskSatContam:
-                                # ** Mask Saturate-Contaminate region 
-                                PixA_DIFF[ContamMask_DIFF] = np.nan
-                            if ConvdSide == 'SCI': 
-                                # ** Flip difference when science is convolved
-                                PixA_DIFF = -PixA_DIFF
+                                ContamMask_DIFF = np.logical_or(ContamMask_CI, ContamMask_J)
+                                PixA_DIFF[ContamMask_DIFF] = np.nan   # Mask Saturation-Contaminated regions
                             
                             # * Save difference image
                             if FITS_DIFF is not None:
+
+                                """
+                                # Remarks on header of difference image
+                                # [1] In general, the FITS header of difference image would mostly be inherited from science image.
+                                #
+                                # [2] when science image is convolved, we turn to set GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN (unit: e-/ADU)
+                                #     so that one can correctly convert ADU to e- for a transient appears on science image.
+                                #     WARNING: for a transient appears on reference image, GAIN_DIFF = GAIN_SCI is correct.
+                                #              we should keep in mind that GAIN_DIFF is not an absolute instrumental value.
+                                #     WARNING: one can only estimate the Poission noise from the science transient via GIAN_DIFF.
+                                #              the Poission noise from the background source (host galaxy) can enhance the 
+                                #              background noise at the position of the transient. photometry softwares which 
+                                #              only take background noise and transient Possion noise into account would tend 
+                                #              to overestimate the SNR of the transient.
+                                # 
+                                # [3] when science image is convolved, we turn to set SATURA_DIFF = SATURA_SCI * SFFT_FSCAL_MEAN         
+                                #     WARNING: it is still not a good idea to use SATURA_DIFF to identify the SATURATION regions
+                                #              on difference image. more appropriate way is masking the saturation contaminated 
+                                #              regions on difference image (MaskSatContam=True), or alternatively, leave them  
+                                #              alone and using AI stamp classifier to reject saturation-related bogus.
+                                #
+                                """
+
                                 _hdl = fits.open(FITS_SCI)
                                 _hdl[0].data[:, :] = PixA_DIFF.T
+
                                 _hdl[0].header['NAME_REF'] = (pa.basename(FITS_REF), 'MeLOn: SFFT')
                                 _hdl[0].header['NAME_SCI'] = (pa.basename(FITS_SCI), 'MeLOn: SFFT')
                                 _hdl[0].header['FWHM_REF'] = (FWHM_REF, 'MeLOn: SFFT')
                                 _hdl[0].header['FWHM_SCI'] = (FWHM_SCI, 'MeLOn: SFFT')
                                 _hdl[0].header['KERORDER'] = (self.KerPolyOrder, 'MeLOn: SFFT')
                                 _hdl[0].header['BGORDER'] = (self.BGPolyOrder, 'MeLOn: SFFT')
                                 _hdl[0].header['CPHOTR'] = (str(self.ConstPhotRatio), 'MeLOn: SFFT')
                                 _hdl[0].header['KERHW'] = (KerHW, 'MeLOn: SFFT')
                                 _hdl[0].header['CONVD'] = (ConvdSide, 'MeLOn: SFFT')
+
+                                if ConvdSide == 'SCI':
+                                    GAIN_SCI = _hdl[0].header[self.GAIN_KEY]
+                                    SATUR_SCI = _hdl[0].header[self.SATUR_KEY]
+                                    GAIN_DIFF = GAIN_SCI / SFFT_FSCAL_MEAN
+                                    SATUR_DIFF = SATUR_SCI * SFFT_FSCAL_MEAN
+
+                                    _hdl[0].header[self.GAIN_KEY] = (GAIN_DIFF, 'MeLOn: SFFT')
+                                    _hdl[0].header[self.SATUR_KEY] = (SATUR_DIFF, 'MeLOn: SFFT')
+
                                 _hdl.writeto(FITS_DIFF, overwrite=True)
                                 _hdl.close()
                             
                             # * Save solution array
                             if FITS_Solution is not None:
                                 phdu = fits.PrimaryHDU()
                                 phdu.header['N0'] = (SFFTConfig[0]['N0'], 'MeLOn: SFFT')
@@ -688,40 +865,68 @@
                                 phdu.header['FAB'] = (SFFTConfig[0]['Fab'], 'MeLOn: SFFT')
                                 phdu.header['FPQ'] = (SFFTConfig[0]['Fpq'], 'MeLOn: SFFT')
                                 phdu.header['FIJAB'] = (SFFTConfig[0]['Fijab'], 'MeLOn: SFFT')
 
                                 PixA_Solution = Solution.reshape((-1, 1))
                                 phdu.data = PixA_Solution.T
                                 fits.HDUList([phdu]).writeto(FITS_Solution, overwrite=True)
-
+                        
                         NEW_STATUS = 2
-                        _message = 'Successful Subtraction for task-[%d] ' %taskidx_acquired
-                        _message += 'in Subtraction thread-[%d]!' %INDEX_THREAD_4SUBTRACT
-                        print('\nMeLOn CheckPoint: %s' %_message)
-
-                    except:
-                        # ** free GPU memory when the subtraction fails
-                        import cupy as cp
+                        if self.VERBOSE_LEVEL in [1, 2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _message += 'SUCCESSFUL SFFT-SUBTRACTION!'
+                            print('\nMeLOn CheckPoint: %s' %_message)
+                    
+                    except Exception as e:
+                        PixA_DIFF, Solution = None, None
+                        SFFT_FSCAL_MEAN, SFFT_FSCAL_SIG = np.nan, np.nan
+                        
+                        # ** clean GPU memory when the subtraction fails
                         with cp.cuda.Device(int(CUDA_DEVICE_4SUBTRACT)):
                             mempool = cp.get_default_memory_pool()
                             pinned_mempool = cp.get_default_pinned_memory_pool()
                             mempool.free_all_blocks()
                             pinned_mempool.free_all_blocks()
-
+                            
+                        GPU_MEMORY_CLEANED = True
+                        if self.VERBOSE_LEVEL in [2]:
+                            _message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _message += 'CLEAN GPU-[%s] MEMORY!' %CUDA_DEVICE_4SUBTRACT
+                            print('\nMeLOn CheckPoint: %s' %_message)
+                        
                         NEW_STATUS = -2
-                        _error_message = 'UnSuccessful Subtraction for task-[%d] ' %taskidx_acquired
-                        _error_message += 'in Subtraction thread-[%d]!' %INDEX_THREAD_4SUBTRACT
-                        print('\nMeLOn ERROR: %s' %_error_message)
-                        Solution = None
-                        PixA_DIFF = None
-
+                        if self.VERBOSE_LEVEL in [0, 1, 2]:
+                            print(e, file=sys.stderr)
+                            _error_message = 'THREAD-4SUBTRACT-[%d] & TASK-[%d]: ' %(INDEX_THREAD_4SUBTRACT, taskidx_acquired)
+                            _error_message += 'FAILED SFFT-SUBTRACTION!'
+                            print('\nMeLOn ERROR: %s' %_error_message)
+                    
                     with lock:
-                        DICT_STATUS_BAR['task-[%d]' %taskidx_acquired] = NEW_STATUS
-                        DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['Solution'] = Solution
-                        DICT_PRODUCTS['task-[%d]' %taskidx_acquired]['PixA_DIFF'] = PixA_DIFF
+                        DICT_STATUS_BAR['TASK-[%d]' %taskidx_acquired] = NEW_STATUS
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['PixA_DIFF'] = PixA_DIFF
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['Solution'] = Solution
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFT_FSCAL_MEAN'] = SFFT_FSCAL_MEAN
+                        DICT_PRODUCTS['TASK-[%d]' %taskidx_acquired]['SFFT_FSCAL_SIG'] = SFFT_FSCAL_SIG
+                    
+            if self.CLEAN_GPU_MEMORY:
+                if not GPU_MEMORY_CLEANED:
+                    mempool = cp.get_default_memory_pool()
+                    pinned_mempool = cp.get_default_pinned_memory_pool()
+                    mempool.free_all_blocks()
+                    pinned_mempool.free_all_blocks()
+                    
+                    if self.VERBOSE_LEVEL in [1, 2]:
+                        _message = 'THREAD-4SUBTRACT-[%d]: ' %INDEX_THREAD_4SUBTRACT
+                        _message += 'FINAL CLEAN GPU-[%s] MEMORY ' %CUDA_DEVICE_4SUBTRACT
+                        print('\nMeLOn CheckPoint: %s' %_message)
+                else:
+                    if self.VERBOSE_LEVEL in [1, 2]:
+                        _message = 'THREAD-4SUBTRACT-[%d]: ' %INDEX_THREAD_4SUBTRACT
+                        _message += 'SKIP FINAL CLEAN, SINCE GPU-[%s] MEMORY ALREADY CLEANED' %CUDA_DEVICE_4SUBTRACT
+                        print('\nMeLOn CheckPoint: %s' %_message)
 
             return None
         
         # * trigger the threads for the preprocessing and subtraction
         MyThreadQueue = []
         for INDEX_THREAD_4PREPROC in range(NUM_THREADS_4PREPROC):
             MyThread = threading.Thread(target=FUNC_4PREPROC, args=(INDEX_THREAD_4PREPROC,))
@@ -732,8 +937,13 @@
             MyThread = threading.Thread(target=FUNC_4SUBTRCT, args=(INDEX_THREAD_4SUBTRACT,))
             MyThreadQueue.append(MyThread)
             MyThread.start()
   
         for MyThread in MyThreadQueue:
             MyThread.join()
         
+        # * show a summary
+        if self.VERBOSE_LEVEL in [0, 1, 2]:
+            NUM_SUCCESS = np.sum(np.array([DICT_STATUS_BAR[task] for task in DICT_STATUS_BAR]) == 2)
+            print('\nMeLOn CheckPoint: SFFT PROCESSED [%d / %d] TASKS SUCCESSFULLY!' %(NUM_SUCCESS, self.NUM_TASK))
+
         return DICT_STATUS_BAR, DICT_PRODUCTS
```

### Comparing `sfft-1.3.4/sfft/__init__.py` & `sfft-1.4.0/sfft/__init__.py`

 * *Files identical despite different names*

### Comparing `sfft-1.3.4/sfft/sfftcore/SFFTConfigure.py` & `sfft-1.4.0/sfft/sfftcore/SFFTConfigure.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,850 +1,39 @@
-import os
-import sys
 import numpy as np
+# version: Feb 5, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.1"
+__version__ = "v1.4"
 
-class SingleSFFTConfigure_Pycuda:
-    @staticmethod
-    def SSCP(NX, NY, KerHW, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, CUDA_DEVICE_4SUBTRACT='0'):
-
-        import pycuda.autoinit
-        from pycuda.compiler import SourceModule
-        os.environ["CUDA_DEVICE"] = CUDA_DEVICE_4SUBTRACT
-
-        N0, N1 = int(NX), int(NY)
-        w0, w1 = int(KerHW), int(KerHW)
-        DK, DB = int(KerPolyOrder), int(BGPolyOrder)
-        MaxThreadPerB = 8     # FIXME USER-DEFINED
-        SFFTParam_dict = {}
-        SFFTModule_dict = {}
-        
-        if DK not in [0, 1, 2, 3]:
-            # NOTE DK = 0 means a spatial invariant matching-kernel.
-            sys.exit('MeLOn ERROR: Input KerPolyOrder should be 0 / 1 / 2 / 3 !')
-        if DB not in [0, 1, 2, 3]:
-            # NOTE DB = 0 means a flat differential-background, however, we cannot kill the sky term in our script.
-            sys.exit('MeLOn ERROR: Input BGPolyOrder should be 0 / 1 / 2 / 3 !')
-        if (N0 < MaxThreadPerB) or (N1 < MaxThreadPerB):
-            sys.exit('MeLOn ERROR: Input Image has dramatically small size !')
-
-        print('\n  --//--//--//--//-- TRIGGER SFFT COMPILATION --//--//--//--//-- ')
-        print('\n  ---//--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---//--- ' %(DK, DB, w0))
-
-        # * Make a dictionary for SFFT parameters
-        L0 = 2*w0+1                       # matching-kernel XSize
-        L1 = 2*w1+1                       # matching-kernel YSize
-        Fab = L0 * L1                     # dof for index 𝛼𝛽
-        Fij = int((DK+1)*(DK+2)/2)        # dof for matching-kernel polynomial index ij 
-        Fpq = int((DB+1)*(DB+2)/2)        # dof for differential-background polynomial index pq 
-        SCALE = np.float64(1/(N0*N1))     # Scale of Image-Size
-        SCALE_L = np.float64(1/SCALE)     # Reciprocal Scale of Image Size
-
-        NEQ = Fij*Fab+Fpq                         # Linear-System side-length
-        Fijab = Fij * Fab                         # Linear-System Major side-length
-        NEQ_FSfree = NEQ - (Fij - 1)              # Forbidden-Stripes-Free Linear-System side-length
-
-        FOMG, FGAM, FTHE = Fij**2, Fij*Fpq, Fij   # OMG / GAM / THE has shape (dof, N0, N1)
-        FPSI, FPHI, FDEL = Fpq*Fij, Fpq**2, Fpq   # PSI / PHI / DEL has shape (dof, N0, N1)
-
-        SFFTParam_dict['N0'] = N0
-        SFFTParam_dict['N1'] = N1
-        SFFTParam_dict['w0'] = w0
-        SFFTParam_dict['w1'] = w1
-        SFFTParam_dict['DK'] = DK
-        SFFTParam_dict['DB'] = DB
-        SFFTParam_dict['ConstPhotRatio'] = ConstPhotRatio
-        SFFTParam_dict['MaxThreadPerB'] = MaxThreadPerB
-
-        SFFTParam_dict['L0'] = L0
-        SFFTParam_dict['L1'] = L1
-        SFFTParam_dict['Fab'] = Fab
-        SFFTParam_dict['Fij'] = Fij
-        SFFTParam_dict['Fpq'] = Fpq
-        SFFTParam_dict['SCALE'] = SCALE
-        SFFTParam_dict['SCALE_L'] = SCALE_L
-        SFFTParam_dict['NEQ'] = NEQ
-        SFFTParam_dict['Fijab'] = Fijab
-        SFFTParam_dict['NEQ_FSfree'] = NEQ_FSfree
-
-        SFFTParam_dict['FOMG'] = FOMG
-        SFFTParam_dict['FGAM'] = FGAM
-        SFFTParam_dict['FTHE'] = FTHE
-        SFFTParam_dict['FPSI'] = FPSI
-        SFFTParam_dict['FPHI'] = FPHI
-        SFFTParam_dict['FDEL'] = FDEL
-
-        # * Load SFFT CUDA modules
-        #   NOTE: Generally, a kernel function is defined without knowledge about Grid-Block-Thread Management.
-        #         However, we need to know the size of threads per block if SharedMemory is called.
-
-        # ************************************ SpatialCoor.cu ************************************ #
-
-        # ** produce spatial coordinate X/Y/oX/oY-map
-        _refdict = {'N0': N0, 'N1': N1}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(int PixA_X_GPU[%(N0)s][%(N1)s], int PixA_Y_GPU[%(N0)s][%(N1)s], 
-            double PixA_CX_GPU[%(N0)s][%(N1)s], double PixA_CY_GPU[%(N0)s][%(N1)s])
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            
-            if (ROW < N0 && COL < N1) {
-                double cx = (ROW + 1.0) / N0;  
-                double cy = (COL + 1.0) / N1;
-                PixA_X_GPU[ROW][COL] = ROW;
-                PixA_Y_GPU[ROW][COL] = COL;
-                PixA_CX_GPU[ROW][COL] = cx;
-                PixA_CY_GPU[ROW][COL] = cy;
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['SpatialCoor'] = _module
-
-        # ************************************ SpatialPoly.cu ************************************ #
-
-        # ** produce Tij, Iij, Tpq
-        _refdict = {'N0': N0, 'N1': N1, 'Fij': Fij, 'Fpq': Fpq}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(int REF_ij_GPU[%(Fij)s][2], int REF_pq_GPU[%(Fpq)s][2],
-            double PixA_CX_GPU[%(N0)s][%(N1)s], double PixA_CY_GPU[%(N0)s][%(N1)s], double PixA_I_GPU[%(N0)s][%(N1)s], 
-            double SPixA_Tij_GPU[%(Fij)s][%(N0)s][%(N1)s], double SPixA_Iij_GPU[%(Fij)s][%(N0)s][%(N1)s], 
-            double SPixA_Tpq_GPU[%(Fpq)s][%(N0)s][%(N1)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-        
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fij = %(Fij)s;
-            int Fpq = %(Fpq)s;
-            
-            if (ROW < N0 && COL < N1) {
-                for(int ij = 0; ij < Fij; ++ij) {
-                    int i = REF_ij_GPU[ij][0];
-                    int j = REF_ij_GPU[ij][1];
-                    double poly_kterm = pow(PixA_CX_GPU[ROW][COL], i) * pow(PixA_CY_GPU[ROW][COL], j);
-                    SPixA_Tij_GPU[ij][ROW][COL] = poly_kterm;
-                    SPixA_Iij_GPU[ij][ROW][COL] = PixA_I_GPU[ROW][COL] * poly_kterm;
-                }
-                    
-                for(int pq = 0; pq < Fpq; ++pq) {
-                    int p = REF_pq_GPU[pq][0];
-                    int q = REF_pq_GPU[pq][1];
-                    double poly_bterm = pow(PixA_CX_GPU[ROW][COL], p) * pow(PixA_CY_GPU[ROW][COL], q);
-                    SPixA_Tpq_GPU[pq][ROW][COL] = poly_bterm;
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['SpatialPoly'] = _module
-
-        # ************************************ HadProd_OMG.cu & FillLS_OMG.cu ************************************ #
-
-        # ** Hadamard Product [𝛀]
-        _refdict = {'N0': N0, 'N1': N1, 'Fij': Fij, 'FOMG': FOMG, 'ThreadPerB': MaxThreadPerB}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(int SREF_iji0j0_GPU[%(FOMG)s][2],
-            cuDoubleComplex SPixA_FIij_GPU[%(Fij)s][%(N0)s][%(N1)s],
-            cuDoubleComplex SPixA_CFIij_GPU[%(Fij)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex HpOMG_GPU[%(FOMG)s][%(N0)s][%(N1)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fij = %(Fij)s;
-            int FOMG = %(FOMG)s;
-
-            __shared__ cuDoubleComplex ShSPixA_FIij_GPU[%(Fij)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int ij = 0; ij < Fij; ++ij){
-                    ShSPixA_FIij_GPU[ij][threadIdx.x][threadIdx.y] = SPixA_FIij_GPU[ij][ROW][COL];
-                }
-            }
-
-            __shared__ cuDoubleComplex ShSPixA_CFIij_GPU[%(Fij)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int ij = 0; ij < Fij; ++ij){
-                    ShSPixA_CFIij_GPU[ij][threadIdx.x][threadIdx.y] = SPixA_CFIij_GPU[ij][ROW][COL];
-                }
-            }
-            __syncthreads();
-
-            if (ROW < N0 && COL < N1) {
-                for(int i8j8ij = 0; i8j8ij < FOMG; ++i8j8ij){
-                    
-                    int i8j8 = SREF_iji0j0_GPU[i8j8ij][0];
-                    int ij = SREF_iji0j0_GPU[i8j8ij][1];
-
-                    HpOMG_GPU[i8j8ij][ROW][COL] = cuCmul(ShSPixA_FIij_GPU[i8j8][threadIdx.x][threadIdx.y], 
-                        ShSPixA_CFIij_GPU[ij][threadIdx.x][threadIdx.y]);
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['HadProd_OMG'] = _module
-
-        # ** Fill Linear-System [𝛀]
-        _refdict = {'N0': N0, 'N1': N1, 'Fijab': Fijab, 'Fab': Fab, 'Fij': Fij, 'NEQ': NEQ, 'FOMG': FOMG}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(int SREF_ijab_GPU[%(Fijab)s][2], int REF_ab_GPU[%(Fab)s][2], 
-            double PreOMG_GPU[%(FOMG)s][%(N0)s][%(N1)s], double LHMAT_GPU[%(NEQ)s][%(NEQ)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fij = %(Fij)s;
-            int Fijab = %(Fijab)s;
-            
-            if (ROW < Fijab && COL < Fijab) {
-                
-                // INDEX Analysis
-                int i8j8 = SREF_ijab_GPU[ROW][0];
-                int a8b8 = SREF_ijab_GPU[ROW][1];
-                int ij = SREF_ijab_GPU[COL][0];
-                int ab = SREF_ijab_GPU[COL][1];
-
-                int a8 = REF_ab_GPU[a8b8][0];
-                int b8 = REF_ab_GPU[a8b8][1];
-                int a = REF_ab_GPU[ab][0];
-                int b = REF_ab_GPU[ab][1];
-                int idx = i8j8 * Fij + ij;
-
-                // Define Mod_N0(rho), Mod_N1(eps)
-                float tmp = 0.0;
-                tmp = fmod(float(a8), float(N0));
-                if (tmp < 0.0) {tmp += float(N0);}
-                int MODa8 = tmp;
-
-                tmp = fmod(float(b8), float(N1));
-                if (tmp < 0.0) {tmp += float(N1);}
-                int MODb8 = tmp;
-
-                tmp = fmod(float(-a), float(N0));
-                if (tmp < 0.0) {tmp += float(N0);}
-                int MOD_a = tmp;
-
-                tmp = fmod(float(-b), float(N1));
-                if (tmp < 0.0) {tmp += float(N1);}
-                int MOD_b = tmp;
-
-                tmp = fmod(float(a8-a), float(N0));
-                if (tmp < 0.0) {tmp += float(N0);}
-                int MODa8_a = tmp;
-
-                tmp = fmod(float(b8-b), float(N1));
-                if (tmp < 0.0) {tmp += float(N1);}
-                int MODb8_b = tmp;
-
-                // Fill Linear System [A-component]
-                if ((a8 != 0 || b8 != 0) && (a != 0 || b != 0)) {
-                    LHMAT_GPU[ROW][COL] = - PreOMG_GPU[idx][MODa8][MODb8]
-                                          - PreOMG_GPU[idx][MOD_a][MOD_b] 
-                                          + PreOMG_GPU[idx][MODa8_a][MODb8_b] 
-                                          + PreOMG_GPU[idx][0][0];
-                }
-
-                if ((a8 == 0 && b8 == 0) && (a != 0 || b != 0)) {
-                    LHMAT_GPU[ROW][COL] = PreOMG_GPU[idx][MOD_a][MOD_b] - PreOMG_GPU[idx][0][0];
-                }
-
-                if ((a8 != 0 || b8 != 0) && (a == 0 && b == 0)) {
-                    LHMAT_GPU[ROW][COL] = PreOMG_GPU[idx][MODa8][MODb8] - PreOMG_GPU[idx][0][0];
-                }
-
-                if ((a8 == 0 && b8 == 0) && (a == 0 && b == 0)) {
-                    LHMAT_GPU[ROW][COL] = PreOMG_GPU[idx][0][0];
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['FillLS_OMG'] = _module
-
-        # ************************************ HadProd_GAM.cu & FillLS_GAM.cu ************************************ #
-
-        # ** Hadamard Product [𝜦]
-        _refdict = {'N0': N0, 'N1': N1, 'Fij': Fij, 'Fpq': Fpq, 'FGAM': FGAM, 'ThreadPerB': MaxThreadPerB}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(int SREF_ijpq_GPU[%(FGAM)s][2], 
-            cuDoubleComplex SPixA_FIij_GPU[%(Fij)s][%(N0)s][%(N1)s],
-            cuDoubleComplex SPixA_CFTpq_GPU[%(Fpq)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex HpGAM_GPU[%(FGAM)s][%(N0)s][%(N1)s])
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fij = %(Fij)s;
-            int Fpq = %(Fpq)s;
-            int FGAM = %(FGAM)s;
-            
-            __shared__ cuDoubleComplex ShSPixA_FIij_GPU[%(Fij)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int ij = 0; ij < Fij; ++ij){
-                    ShSPixA_FIij_GPU[ij][threadIdx.x][threadIdx.y] = SPixA_FIij_GPU[ij][ROW][COL];
-                }
-            }
-
-            __shared__ cuDoubleComplex ShSPixA_CFTpq_GPU[%(Fpq)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int pq = 0; pq < Fpq; ++pq){
-                    ShSPixA_CFTpq_GPU[pq][threadIdx.x][threadIdx.y] = SPixA_CFTpq_GPU[pq][ROW][COL];
-                }
-            }
-            __syncthreads();
-            
-            if (ROW < N0 && COL < N1) {        
-                for(int i8j8pq = 0; i8j8pq < FGAM; ++i8j8pq){
-
-                    int i8j8 = SREF_ijpq_GPU[i8j8pq][0];
-                    int pq = SREF_ijpq_GPU[i8j8pq][1];
-
-                    HpGAM_GPU[i8j8pq][ROW][COL] = cuCmul(ShSPixA_FIij_GPU[i8j8][threadIdx.x][threadIdx.y], 
-                        ShSPixA_CFTpq_GPU[pq][threadIdx.x][threadIdx.y]);
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['HadProd_GAM'] = _module
-
-        # ** Fill Linear-System [𝜦]
-        _refdict = {'N0': N0, 'N1': N1, 'NEQ': NEQ, 'Fab': Fab, 'Fpq': Fpq, 'Fijab': Fijab, 'FGAM': FGAM}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(int SREF_ijab_GPU[%(Fijab)s][2], int REF_ab_GPU[%(Fab)s][2], 
-            double PreGAM_GPU[%(FGAM)s][%(N0)s][%(N1)s], double LHMAT_GPU[%(NEQ)s][%(NEQ)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fpq = %(Fpq)s;
-            int Fijab = %(Fijab)s;
-            
-            if (ROW < Fijab && COL < Fpq) {
-                
-                // INDEX Analysis
-                int i8j8 = SREF_ijab_GPU[ROW][0];
-                int a8b8 = SREF_ijab_GPU[ROW][1];
-                int pq = COL;
-
-                int a8 = REF_ab_GPU[a8b8][0];
-                int b8 = REF_ab_GPU[a8b8][1];
-                int idx = i8j8 * Fpq + pq;
-                int cCOL = Fijab + COL;              // add offset
-
-                // Define Mod_N0(rho), Mod_N1(eps)
-                float tmp = 0.0;
-                tmp = fmod(float(a8), float(N0));
-                if (tmp < 0.0) {tmp += float(N0);}
-                int MODa8 = tmp;
-
-                tmp = fmod(float(b8), float(N1));
-                if (tmp < 0.0) {tmp += float(N1);}
-                int MODb8 = tmp;
-
-                // Fill Linear System [B-component]
-                if (a8 != 0 || b8 != 0) {
-                    LHMAT_GPU[ROW][cCOL] = PreGAM_GPU[idx][MODa8][MODb8] - PreGAM_GPU[idx][0][0];
-                }
-
-                if (a8 == 0 && b8 == 0) {
-                    LHMAT_GPU[ROW][cCOL] = PreGAM_GPU[idx][0][0];
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['FillLS_GAM'] = _module
-
-        # ************************************ HadProd_PSI.cu & FillLS_PSI.cu ************************************ #
-
-        # ** Hadamard Product [𝜳]
-        _refdict = {'N0': N0, 'N1': N1, 'Fij': Fij, 'Fpq': Fpq, 'FPSI': FPSI, 'ThreadPerB': MaxThreadPerB}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(int SREF_pqij_GPU[%(FPSI)s][2],
-            cuDoubleComplex SPixA_CFIij_GPU[%(Fij)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex SPixA_FTpq_GPU[%(Fpq)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex HpPSI_GPU[%(FPSI)s][%(N0)s][%(N1)s]) 
-        {    
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fpq = %(Fpq)s;
-            int Fij = %(Fij)s;
-            int FPSI = %(FPSI)s;
-            
-            __shared__ cuDoubleComplex ShSPixA_FTpq_GPU[%(Fpq)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int pq = 0; pq < Fpq; ++pq){
-                    ShSPixA_FTpq_GPU[pq][threadIdx.x][threadIdx.y] = SPixA_FTpq_GPU[pq][ROW][COL];
-                }
-            }
-
-            __shared__ cuDoubleComplex ShSPixA_CFIij_GPU[%(Fij)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int ij = 0; ij < Fij; ++ij){
-                    ShSPixA_CFIij_GPU[ij][threadIdx.x][threadIdx.y] = SPixA_CFIij_GPU[ij][ROW][COL];
-                }
-            }
-            __syncthreads();
-
-            if (ROW < N0 && COL < N1) {
-                for(int p8q8ij = 0; p8q8ij < FPSI; ++p8q8ij){
-                    
-                    int p8q8 = SREF_pqij_GPU[p8q8ij][0];
-                    int ij = SREF_pqij_GPU[p8q8ij][1];
-
-                    HpPSI_GPU[p8q8ij][ROW][COL] = cuCmul(ShSPixA_FTpq_GPU[p8q8][threadIdx.x][threadIdx.y], 
-                        ShSPixA_CFIij_GPU[ij][threadIdx.x][threadIdx.y]);
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['HadProd_PSI'] = _module
-
-        # ** Fill Linear-System [𝜳]
-        _refdict = {'N0': N0, 'N1': N1, 'NEQ': NEQ, 'Fab': Fab, 'Fij': Fij, 'Fpq': Fpq, 'Fijab': Fijab, 'FPSI': FPSI}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(int SREF_ijab_GPU[%(Fijab)s][2], int REF_ab_GPU[%(Fab)s][2], 
-            double PrePSI_GPU[%(FPSI)s][%(N0)s][%(N1)s], double LHMAT_GPU[%(NEQ)s][%(NEQ)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fij = %(Fij)s;
-            int Fpq = %(Fpq)s;
-            int Fijab = %(Fijab)s;
-
-            if (ROW < Fpq && COL < Fijab) {
-
-                // INDEX Analysis
-                int cROW = Fijab + ROW;              // add offset
-                int p8q8 = ROW;
-                int ij = SREF_ijab_GPU[COL][0];
-                int ab = SREF_ijab_GPU[COL][1];
-                int a = REF_ab_GPU[ab][0];
-                int b = REF_ab_GPU[ab][1];
-                int idx = p8q8 * Fij + ij;
-
-                // Define Mod_N0(rho), Mod_N1(eps)
-                float tmp = 0.0;
-                tmp = fmod(float(-a), float(N0));
-                if (tmp < 0.0) {tmp += float(N0);}
-                int MOD_a = tmp;
-
-                tmp = fmod(float(-b), float(N1));
-                if (tmp < 0.0) {tmp += float(N1);}
-                int MOD_b = tmp;
-                
-                // Fill Linear System [B#-component]
-                if (a != 0 || b != 0) {
-                    LHMAT_GPU[cROW][COL] = PrePSI_GPU[idx][MOD_a][MOD_b] - PrePSI_GPU[idx][0][0];
-                }
-
-                if (a == 0 && b == 0) {
-                    LHMAT_GPU[cROW][COL] = PrePSI_GPU[idx][0][0];
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['FillLS_PSI'] = _module
-
-        # ************************************ HadProd_PHI.cu & FillLS_PHI.cu ************************************ #
-
-        # ** Hadamard Product [𝚽]
-        _refdict = {'N0': N0, 'N1': N1, 'Fpq': Fpq, 'FPHI': FPHI, 'ThreadPerB': MaxThreadPerB}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(int SREF_pqp0q0_GPU[%(FPHI)s][2], 
-            cuDoubleComplex SPixA_FTpq_GPU[%(Fpq)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex SPixA_CFTpq_GPU[%(Fpq)s][%(N0)s][%(N1)s],  
-            cuDoubleComplex HpPHI_GPU[%(FPHI)s][%(N0)s][%(N1)s]) 
-        {    
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fpq = %(Fpq)s;
-            int FPHI = %(FPHI)s;
-
-            __shared__ cuDoubleComplex ShSPixA_FTpq_GPU[%(Fpq)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int pq = 0; pq < Fpq; ++pq){
-                    ShSPixA_FTpq_GPU[pq][threadIdx.x][threadIdx.y] = SPixA_FTpq_GPU[pq][ROW][COL];
-                }
-            }
-
-            __shared__ cuDoubleComplex ShSPixA_CFTpq_GPU[%(Fpq)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int pq = 0; pq < Fpq; ++pq){
-                    ShSPixA_CFTpq_GPU[pq][threadIdx.x][threadIdx.y] = SPixA_CFTpq_GPU[pq][ROW][COL];
-                }
-            }
-            __syncthreads();
-            
-            if (ROW < N0 && COL < N1) {
-                for(int p8q8pq = 0; p8q8pq < FPHI; ++p8q8pq){
-                    
-                    int p8q8 = SREF_pqp0q0_GPU[p8q8pq][0];
-                    int pq = SREF_pqp0q0_GPU[p8q8pq][1];
-
-                    HpPHI_GPU[p8q8pq][ROW][COL] = cuCmul(ShSPixA_FTpq_GPU[p8q8][threadIdx.x][threadIdx.y], 
-                        ShSPixA_CFTpq_GPU[pq][threadIdx.x][threadIdx.y]);
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['HadProd_PHI'] = _module
-
-        # ** Fill Linear-System [𝚽]
-        _refdict = {'N0': N0, 'N1': N1, 'NEQ': NEQ, 'Fpq': Fpq, 'Fijab': Fijab, 'FPHI': FPHI}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(double PrePHI_GPU[%(FPHI)s][%(N0)s][%(N1)s], 
-            double LHMAT_GPU[%(NEQ)s][%(NEQ)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int Fpq = %(Fpq)s;
-            int Fijab = %(Fijab)s;
-
-            if (ROW < Fpq && COL < Fpq) {
-                
-                // INDEX Analysis
-                int cROW = Fijab + ROW;              // add offset
-                int cCOL = Fijab + COL;              // add offset
-                
-                int p8q8 = ROW;
-                int pq = COL;
-                int idx = p8q8 * Fpq + pq;
-
-                // Fill Linear System [C-component]
-                LHMAT_GPU[cROW][cCOL] = PrePHI_GPU[idx][0][0];
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['FillLS_PHI'] = _module
-
-        # ************************************ HadProd_THE.cu & FillLS_THE.cu ************************************ #
-
-        # ** Hadamard Product [𝚯]
-        _refdict = {'N0': N0, 'N1': N1, 'Fij': Fij, 'FTHE': FTHE}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(cuDoubleComplex SPixA_FIij_GPU[%(Fij)s][%(N0)s][%(N1)s],
-            cuDoubleComplex PixA_CFJ_GPU[%(N0)s][%(N1)s], cuDoubleComplex HpTHE_GPU[%(FTHE)s][%(N0)s][%(N1)s])
-        {    
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int FTHE = %(FTHE)s;
-
-            if (ROW < N0 && COL < N1) {
-                for(int i8j8 = 0; i8j8 < FTHE; ++i8j8){
-                    HpTHE_GPU[i8j8][ROW][COL] = cuCmul(PixA_CFJ_GPU[ROW][COL], SPixA_FIij_GPU[i8j8][ROW][COL]);
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['HadProd_THE'] = _module
-
-        # ** Fill Linear-System [𝚯]
-        _refdict = {'N0': N0, 'N1': N1, 'NEQ': NEQ, 'Fijab': Fijab, 'Fab': Fab, 'FTHE': FTHE}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(int SREF_ijab_GPU[%(Fijab)s][2], int REF_ab_GPU[%(Fab)s][2], 
-            double PreTHE_GPU[%(FTHE)s][%(N0)s][%(N1)s], double RHb_GPU[%(NEQ)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int Fijab = %(Fijab)s;
-
-            if (ROW < Fijab && COL == 0) {
-
-                // INDEX Analysis
-                int i8j8 = SREF_ijab_GPU[ROW][0];
-                int a8b8 = SREF_ijab_GPU[ROW][1];
-                int a8 = REF_ab_GPU[a8b8][0];
-                int b8 = REF_ab_GPU[a8b8][1];
-                int idx = i8j8;
-
-                // Define Mod_N0(rho), Mod_N1(eps)
-                float tmp = 0.0;
-                tmp = fmod(float(a8), float(N0));
-                if (tmp < 0.0) {tmp += float(N0);}
-                int MODa8 = tmp;
-
-                tmp = fmod(float(b8), float(N1));
-                if (tmp < 0.0) {tmp += float(N1);}
-                int MODb8 = tmp;
-                
-                // Fill Linear System [D-component]
-                if (a8 != 0 || b8 != 0) {
-                    RHb_GPU[ROW] = PreTHE_GPU[idx][MODa8][MODb8] - PreTHE_GPU[idx][0][0];
-                }
-
-                if (a8 == 0 && b8 == 0) {
-                    RHb_GPU[ROW] = PreTHE_GPU[idx][0][0];
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['FillLS_THE'] = _module
-
-        # ************************************ HadProd_DEL.cu & FillLS_DEL.cu ************************************ #
-
-        # ** Hadamard Product [𝚫]
-        _refdict = {'N0': N0, 'N1': N1, 'Fpq': Fpq, 'FDEL': FDEL}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(cuDoubleComplex SPixA_FTpq_GPU[%(Fpq)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex PixA_CFJ_GPU[%(N0)s][%(N1)s], cuDoubleComplex HpDEL_GPU[%(FDEL)s][%(N0)s][%(N1)s])
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int FDEL = %(FDEL)s;
-
-            if (ROW < N0 && COL < N1) {
-                for(int p8q8 = 0; p8q8 < FDEL; ++p8q8){
-                    HpDEL_GPU[p8q8][ROW][COL] = 
-                        cuCmul(PixA_CFJ_GPU[ROW][COL], SPixA_FTpq_GPU[p8q8][ROW][COL]);
-                }
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['HadProd_DEL'] = _module
-
-        # ** Fill Linear-System [𝚫]
-        _refdict = {'N0': N0, 'N1': N1, 'NEQ': NEQ, 'Fpq': Fpq, 'Fijab': Fijab, 'FDEL': FDEL}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(double PreDEL_GPU[%(FDEL)s][%(N0)s][%(N1)s], 
-            double RHb_GPU[%(NEQ)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int Fpq = %(Fpq)s;
-            int Fijab = %(Fijab)s;
-
-            if (ROW < Fpq && COL == 0) {
-                // INDEX Analysis
-                int cROW = Fijab + ROW;              // add offset
-                int idx = ROW;                       // i.e. p8q8
-
-                // Fill Linear System [E-component]
-                RHb_GPU[cROW] = PreDEL_GPU[idx][0][0];
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['FillLS_DEL'] = _module
-
-        # ************************************ Remove_LSFStripes.cu ************************************ #
-
-        # ** Remove Forbidden Stripes in Linear-System
-        _refdict = {'NEQ': NEQ, 'NEQ_FSfree': NEQ_FSfree}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(double LHMAT_GPU[%(NEQ)s][%(NEQ)s], int IDX_nFS_GPU[%(NEQ_FSfree)s], 
-            double LHMAT_FSfree_GPU[%(NEQ_FSfree)s][%(NEQ_FSfree)s]) 
-        {
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            int NEQ_FSfree = %(NEQ_FSfree)s;
-
-            if (ROW < NEQ_FSfree && COL < NEQ_FSfree) {
-                int ROW_nFS = IDX_nFS_GPU[ROW];
-                int COL_nFS = IDX_nFS_GPU[COL];
-                LHMAT_FSfree_GPU[ROW][COL] = LHMAT_GPU[ROW_nFS][COL_nFS];
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['Remove_LSFStripes'] = _module
-
-        # ************************************ Extend_Solution.cu ************************************ #
-
-        # ** Extend Solution from Forbidden-Stripes-Free Linear-System
-        _refdict = {'NEQ_FSfree': NEQ_FSfree, 'NEQ': NEQ}
-        _funcstr = r"""
-        extern "C" __global__ void kmain(double Solution_FSfree_GPU[%(NEQ_FSfree)s], 
-            int IDX_nFS_GPU[%(NEQ_FSfree)s], double Solution_GPU[%(NEQ)s]) 
-        {    
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int NEQ_FSfree = %(NEQ_FSfree)s;
-            
-            if (ROW < NEQ_FSfree) {
-                int ROW_nFS = IDX_nFS_GPU[ROW];
-                Solution_GPU[ROW_nFS] = Solution_FSfree_GPU[ROW];
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['Extend_Solution'] = _module
-
-        # ************************************ Construct_FDIFF.cu ************************************ #
-
-        # ** Construct DIFF Image in Fourier Space 
-        _refdict = {'N0': N0, 'N1': N1, 'L0': L0, 'L1': L1, 'w0': w0, 'w1': w1, \
-                        'Fijab': Fijab, 'Fab': Fab, 'Fij': Fij, 'Fpq': Fpq, \
-                        'SCALE': SCALE, 'ThreadPerB': MaxThreadPerB}
-        _funcstr = r"""
-        #include "cuComplex.h"
-        extern "C" __global__ void kmain(int SREF_ijab_GPU[%(Fijab)s][2], int REF_ab_GPU[%(Fab)s][2],  
-            cuDoubleComplex a_ijab_GPU[%(Fijab)s], cuDoubleComplex SPixA_FIij_GPU[%(Fij)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex Kab_Wla_GPU[%(L0)s][%(N0)s][%(N1)s], cuDoubleComplex Kab_Wmb_GPU[%(L1)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex b_pq_GPU[%(Fpq)s], cuDoubleComplex SPixA_FTpq_GPU[%(Fpq)s][%(N0)s][%(N1)s], 
-            cuDoubleComplex PixA_FJ_GPU[%(N0)s][%(N1)s], cuDoubleComplex PixA_FDIFF_GPU[%(N0)s][%(N1)s])
-        {       
-            int ROW = blockIdx.x*blockDim.x+threadIdx.x;
-            int COL = blockIdx.y*blockDim.y+threadIdx.y;
-            
-            int N0 = %(N0)s;
-            int N1 = %(N1)s;
-            int w0 = %(w0)s;
-            int w1 = %(w1)s;
-            int Fij = %(Fij)s;
-            int Fab = %(Fab)s;
-            int Fpq = %(Fpq)s;
-
-            double One_re = 1.0;
-            double Zero_re = 0.0;
-            double Zero_im = 0.0;
-            double SCALE_re = %(SCALE)s;
-            cuDoubleComplex ZERO = make_cuDoubleComplex(Zero_re, Zero_im);
-            cuDoubleComplex ONE = make_cuDoubleComplex(One_re, Zero_im);
-            cuDoubleComplex SCA = make_cuDoubleComplex(SCALE_re, Zero_im);
-            cuDoubleComplex PVAL = ZERO;
-            cuDoubleComplex PVAL_FKab = ZERO;
-
-            __shared__ cuDoubleComplex ShSPixA_FIij_GPU[%(Fij)s][%(ThreadPerB)s][%(ThreadPerB)s];
-            if (ROW < N0 && COL < N1) {
-                for(int ij = 0; ij < Fij; ++ij){
-                    ShSPixA_FIij_GPU[ij][threadIdx.x][threadIdx.y] = SPixA_FIij_GPU[ij][ROW][COL];
-                }
-            }
-            __syncthreads();
-
-            if (ROW < N0 && COL < N1) {
-
-                PVAL = ZERO;
-                PVAL_FKab = ZERO;
-                for(int ab = 0; ab < Fab; ++ab){
-                    int a = REF_ab_GPU[ab][0];
-                    int b = REF_ab_GPU[ab][1];
-                    
-                    if (a == 0 && b == 0) {
-                        PVAL_FKab = SCA;
-                    }
-                    
-                    if (a != 0 || b != 0) {
-                        PVAL_FKab = cuCmul(SCA, cuCsub(cuCmul(Kab_Wla_GPU[w0 + a][ROW][COL], Kab_Wmb_GPU[w1 + b][ROW][COL]), ONE));
-                    }
-
-                    for(int ij = 0; ij < Fij; ++ij){
-                        int ijab = ij * Fab + ab;
-                        PVAL = cuCadd(PVAL, cuCmul(cuCmul(a_ijab_GPU[ijab], ShSPixA_FIij_GPU[ij][threadIdx.x][threadIdx.y]), PVAL_FKab));
-                    }
-                }
-
-                for(int pq = 0; pq < Fpq; ++pq){
-                    PVAL = cuCadd(PVAL, cuCmul(b_pq_GPU[pq], SPixA_FTpq_GPU[pq][ROW][COL]));
-                }
-                
-                PixA_FDIFF_GPU[ROW][COL] = cuCsub(PixA_FJ_GPU[ROW][COL], PVAL);
-            }
-        }
-        """
-        _code = _funcstr % _refdict
-        _module = SourceModule(source=_code, nvcc='nvcc')
-        SFFTModule_dict['Construct_FDIFF'] = _module
-        
-        SFFTConfig = (SFFTParam_dict, SFFTModule_dict)
-        print('\n  --//--//--//--//-- EXIT SFFT COMPILATION --//--//--//--//-- ')
-
-        return SFFTConfig
-    
 class SingleSFFTConfigure_Cupy:
     @staticmethod
-    def SSCC(NX, NY, KerHW, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, CUDA_DEVICE_4SUBTRACT='0'):
+    def SSCC(NX, NY, KerHW, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, VERBOSE_LEVEL=2):
         
         import cupy as cp
-        os.environ["CUDA_DEVICE"] = CUDA_DEVICE_4SUBTRACT
-
         N0, N1 = int(NX), int(NY)
         w0, w1 = int(KerHW), int(KerHW)
         DK, DB = int(KerPolyOrder), int(BGPolyOrder)
-        MaxThreadPerB = 8     # FIXME USER-DEFINED
+        MaxThreadPerB = 8     # FIXME emperical value
         SFFTParam_dict = {}
         SFFTModule_dict = {}
         
         if DK not in [0, 1, 2, 3]:
             # NOTE DK = 0 means a spatial invariant matching-kernel.
-            sys.exit('MeLOn ERROR: Input KerPolyOrder should be 0 / 1 / 2 / 3 !')
+            raise Exception('MeLOn ERROR: Input KerPolyOrder should be 0/1/2/3!')
+
         if DB not in [0, 1, 2, 3]:
             # NOTE DB = 0 means a flat differential-background, however, we cannot kill the sky term in our script.
-            sys.exit('MeLOn ERROR: Input BGPolyOrder should be 0 / 1 / 2 / 3 !')
+            raise Exception('MeLOn ERROR: Input BGPolyOrder should be 0/1/2/3!')
+        
         if (N0 < MaxThreadPerB) or (N1 < MaxThreadPerB):
-            sys.exit('MeLOn ERROR: Input Image has dramatically small size !')
+            raise Exception('MeLOn ERROR: Input Image has dramatically small size!')
 
-        print('\n  --//--//--//--//-- TRIGGER SFFT COMPILATION --//--//--//--//-- ')
-        print('\n  ---//--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---//--- ' %(DK, DB, w0))
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --//--//--//--//-- TRIGGER SFFT COMPILATION --//--//--//--//-- ')
+            print('\n ---//--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---//--- ' %(DK, DB, w0))
 
         # * Make a dictionary for SFFT parameters
         L0 = 2*w0+1                       # matching-kernel XSize
         L1 = 2*w1+1                       # matching-kernel YSize
         Fab = L0 * L1                     # dof for index 𝛼𝛽
         Fij = int((DK+1)*(DK+2)/2)        # dof for matching-kernel polynomial index ij 
         Fpq = int((DB+1)*(DB+2)/2)        # dof for differential-background polynomial index pq 
@@ -883,15 +72,15 @@
         SFFTParam_dict['FTHE'] = FTHE
         SFFTParam_dict['FPSI'] = FPSI
         SFFTParam_dict['FPHI'] = FPHI
         SFFTParam_dict['FDEL'] = FDEL
 
         # * Load SFFT CUDA modules
         #   NOTE: Generally, a kernel function is defined without knowledge about Grid-Block-Thread Management.
-        #               However, we need to know the size of threads per block if SharedMemory is called.
+        #         However, we need to know the size of threads per block if SharedMemory is called.
 
         # ************************************ SpatialCoor.cu ************************************ #
 
         # ** produce spatial coordinate X/Y/oX/oY-map
         _refdict = {'N0': N0, 'N1': N1}
         _funcstr = r"""
         extern "C" __global__ void kmain(int PixA_X_GPU[%(N0)s][%(N1)s], int PixA_Y_GPU[%(N0)s][%(N1)s], 
@@ -915,36 +104,34 @@
         """
         _code = _funcstr % _refdict
         _module = cp.RawModule(code=_code, backend=u'nvcc', translate_cucomplex=False)
         SFFTModule_dict['SpatialCoor'] = _module
 
         # ************************************ SpatialPoly.cu ************************************ #
 
-        # ** produce Tij, Iij, Tpq
+        # ** produce Iij, Tpq
         _refdict = {'N0': N0, 'N1': N1, 'Fij': Fij, 'Fpq': Fpq}
         _funcstr = r"""
         extern "C" __global__ void kmain(int REF_ij_GPU[%(Fij)s][2], int REF_pq_GPU[%(Fpq)s][2],
             double PixA_CX_GPU[%(N0)s][%(N1)s], double PixA_CY_GPU[%(N0)s][%(N1)s], double PixA_I_GPU[%(N0)s][%(N1)s], 
-            double SPixA_Tij_GPU[%(Fij)s][%(N0)s][%(N1)s], double SPixA_Iij_GPU[%(Fij)s][%(N0)s][%(N1)s], 
-            double SPixA_Tpq_GPU[%(Fpq)s][%(N0)s][%(N1)s]) 
+            double SPixA_Iij_GPU[%(Fij)s][%(N0)s][%(N1)s], double SPixA_Tpq_GPU[%(Fpq)s][%(N0)s][%(N1)s]) 
         {
             int ROW = blockIdx.x*blockDim.x+threadIdx.x;
             int COL = blockIdx.y*blockDim.y+threadIdx.y;
         
             int N0 = %(N0)s;
             int N1 = %(N1)s;
             int Fij = %(Fij)s;
             int Fpq = %(Fpq)s;
             
             if (ROW < N0 && COL < N1) {
                 for(int ij = 0; ij < Fij; ++ij) {
                     int i = REF_ij_GPU[ij][0];
                     int j = REF_ij_GPU[ij][1];
                     double poly_kterm = pow(PixA_CX_GPU[ROW][COL], i) * pow(PixA_CY_GPU[ROW][COL], j);
-                    SPixA_Tij_GPU[ij][ROW][COL] = poly_kterm;
                     SPixA_Iij_GPU[ij][ROW][COL] = PixA_I_GPU[ROW][COL] * poly_kterm;
                 }
                     
                 for(int pq = 0; pq < Fpq; ++pq) {
                     int p = REF_pq_GPU[pq][0];
                     int q = REF_pq_GPU[pq][1];
                     double poly_bterm = pow(PixA_CX_GPU[ROW][COL], p) * pow(PixA_CY_GPU[ROW][COL], q);
@@ -1618,43 +805,43 @@
         }
         """
         _code = _funcstr % _refdict
         _module = cp.RawModule(code=_code, backend=u'nvcc', translate_cucomplex=True)
         SFFTModule_dict['Construct_FDIFF'] = _module
         
         SFFTConfig = (SFFTParam_dict, SFFTModule_dict)
-        print('\n  --//--//--//--//-- EXIT SFFT COMPILATION --//--//--//--//-- ')
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --//--//--//--//-- EXIT SFFT COMPILATION --//--//--//--//-- ')
 
         return SFFTConfig
 
 class SingleSFFTConfigure_Numpy:
     @staticmethod
-    def SSCN(NX, NY, KerHW, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, NUM_CPU_THREADS_4SUBTRACT=8):
+    def SSCN(NX, NY, KerHW, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
 
         import numba as nb
         nb.set_num_threads = NUM_CPU_THREADS_4SUBTRACT
 
         N0, N1 = int(NX), int(NY)
         w0, w1 = int(KerHW), int(KerHW)
         DK, DB = int(KerPolyOrder), int(BGPolyOrder)
-        MaxThreadPerB = 8     # FIXME USER-DEFINED
         SFFTParam_dict = {}
         SFFTModule_dict = {}
         
         if DK not in [0, 1, 2, 3]:
             # NOTE DK = 0 means a spatial invariant matching-kernel.
-            sys.exit('MeLOn ERROR: Input KerPolyOrder should be 0 / 1 / 2 / 3 !')
+            raise Exception('MeLOn ERROR: Input KerPolyOrder should be 0/1/2/3!')
+        
         if DB not in [0, 1, 2, 3]:
             # NOTE DB = 0 means a flat differential-background, however, we cannot kill the sky term in our script.
-            sys.exit('MeLOn ERROR: Input BGPolyOrder should be 0 / 1 / 2 / 3 !')
-        if (N0 < MaxThreadPerB) or (N1 < MaxThreadPerB):
-            sys.exit('MeLOn ERROR: Input Image has dramatically small size !')
+            raise Exception('MeLOn ERROR: Input BGPolyOrder should be 0/1/2/3!')
 
-        print('\n  --//--//--//--//-- TRIGGER SFFT COMPILATION --//--//--//--//-- ')
-        print('\n  ---//--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---//--- ' %(DK, DB, w0))
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --//--//--//--//-- TRIGGER SFFT COMPILATION --//--//--//--//-- ')
+            print('\n ---//--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---//--- ' %(DK, DB, w0))
 
         # * Make a dictionary for SFFT parameters
         L0 = 2*w0+1                       # matching-kernel XSize
         L1 = 2*w1+1                       # matching-kernel YSize
         Fab = L0 * L1                     # dof for index 𝛼𝛽
         Fij = int((DK+1)*(DK+2)/2)        # dof for matching-kernel polynomial index ij 
         Fpq = int((DB+1)*(DB+2)/2)        # dof for differential-background polynomial index pq 
@@ -1671,15 +858,14 @@
         SFFTParam_dict['N0'] = N0
         SFFTParam_dict['N1'] = N1
         SFFTParam_dict['w0'] = w0
         SFFTParam_dict['w1'] = w1
         SFFTParam_dict['DK'] = DK
         SFFTParam_dict['DB'] = DB
         SFFTParam_dict['ConstPhotRatio'] = ConstPhotRatio
-        SFFTParam_dict['MaxThreadPerB'] = MaxThreadPerB
 
         SFFTParam_dict['L0'] = L0
         SFFTParam_dict['L1'] = L1
         SFFTParam_dict['Fab'] = Fab
         SFFTParam_dict['Fij'] = Fij
         SFFTParam_dict['Fpq'] = Fpq
         SFFTParam_dict['SCALE'] = SCALE
@@ -1716,43 +902,40 @@
                     PixA_CY[ROW, COL] = (float(COL) + 1.0) / N1   # NOTE UPDATE
 
             return PixA_X, PixA_Y, PixA_CX, PixA_CY
 
         SFFTModule_dict['SpatialCoor'] = SpatialCoor
         # ************************************ SpatialPoly.py ************************************ #
 
-        # ** produce Tij, Iij, Tpq
-        _strdec = 'Tuple((f8[:,:,:], f8[:,:,:], f8[:,:,:]))' + \
-            '(i4[:,:], i4[:,:], f8[:,:], f8[:,:], f8[:,:], f8[:,:,:], f8[:,:,:], f8[:,:,:])'
+        # ** produce Iij, Tpq
+        _strdec = 'Tuple((f8[:,:,:], f8[:,:,:]))' + '(i4[:,:], i4[:,:], f8[:,:], f8[:,:], f8[:,:], f8[:,:,:], f8[:,:,:])'
         @nb.njit(_strdec, parallel=True)
-        def SpatialPoly(REF_ij, REF_pq, PixA_CX, PixA_CY, PixA_I, SPixA_Tij, SPixA_Iij, SPixA_Tpq):
+        def SpatialPoly(REF_ij, REF_pq, PixA_CX, PixA_CY, PixA_I, SPixA_Iij, SPixA_Tpq):
             
             #assert REF_ij.dtype == np.int32 and REF_ij.shape == (Fij, 2)
             #assert REF_pq.dtype == np.int32 and REF_pq.shape == (Fpq, 2)
             
             #assert PixA_CX.dtype == np.float64 and PixA_CX.shape == (N0, N1)
             #assert PixA_CY.dtype == np.float64 and PixA_CY.shape == (N0, N1)
             #assert PixA_I.dtype == np.float64 and PixA_I.shape == (N0, N1)
             
-            #assert SPixA_Tij.dtype == np.float64 and SPixA_Tij.shape == (Fij, N0, N1)
             #assert SPixA_Iij.dtype == np.float64 and SPixA_Iij.shape == (Fij, N0, N1)
             #assert SPixA_Tpq.dtype == np.float64 and SPixA_Tpq.shape == (Fpq, N0, N1)
 
             for ij in nb.prange(Fij):
                 i, j = REF_ij[ij]
                 PixA_kpoly = np.power(PixA_CX, i) * np.power(PixA_CY, j)
-                SPixA_Tij[ij, :, :] = PixA_kpoly   # NOTE UPDATE
                 SPixA_Iij[ij, :, :] = PixA_I * PixA_kpoly   # NOTE UPDATE
             
             for pq in nb.prange(Fpq):
                 p, q = REF_pq[pq]
                 PixA_bpoly = np.power(PixA_CX, p) * np.power(PixA_CY, q)
                 SPixA_Tpq[pq, :, :] = PixA_bpoly   # NOTE UPDATE
             
-            return SPixA_Tij, SPixA_Iij, SPixA_Tpq
+            return SPixA_Iij, SPixA_Tpq
 
         SFFTModule_dict['SpatialPoly'] = SpatialPoly
         # ************************************ HadProd_OMG.py & FillLS_OMG.py ************************************ #
 
         # ** Hadamard Product [𝛀]
         _strdec = 'c16[:,:,:](i4[:,:], c16[:,:,:], c16[:,:,:], c16[:,:,:])'
         @nb.njit(_strdec, parallel=True)
@@ -2173,60 +1356,40 @@
                     PixA_FDIFF[ROW, COL] = PixA_FJ[ROW, COL] - PVAL
             
             return PixA_FDIFF
 
         SFFTModule_dict['Construct_FDIFF'] = Construct_FDIFF
 
         SFFTConfig = (SFFTParam_dict, SFFTModule_dict)
-        print('\n  --//--//--//--//-- EXIT SFFT COMPILATION --//--//--//--//-- ')
+        if VERBOSE_LEVEL in [1, 2]: 
+            print('\n --//--//--//--//-- EXIT SFFT COMPILATION --//--//--//--//-- ')
 
         return SFFTConfig
 
 class SingleSFFTConfigure:
     @staticmethod
     def SSC(NX, NY, KerHW, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, \
-        BACKEND_4SUBTRACT='Pycuda', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
+        BACKEND_4SUBTRACT='Cupy', NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
 
         """
         # Arguments:
         # a) NX, NY: Image Size (pixels) along X / Y axis.
         # b) KerHW: Kernel half width for compilation.
         # c) KerPolyOrder: The order of Polynomial Variation for PSF-Matching Kernel.
         # d) BGPolyOrder: The order of Polynomial Variation for Differential Background.
-        # e) ConstPhotRatio: Use a constant photometric ratio in image subtraction ?
-        # f) BACKEND_4SUBTRACT: Which backend would you like to perform SFFT subtraction on ?
-        # g) CUDA_DEVICE_4SUBTRACT (BACKEND_4SUBTRACT = Pycuda / Cupy): Which GPU device would you want to perform SFFT subtraction on ?
-        # h) NUM_CPU_THREADS_4SUBTRACT (BACKEND_4SUBTRACT = Numpy): How many CPU threads would you want to perform SFFT subtraction on ?
-        
+        # e) ConstPhotRatio: Use a constant photometric ratio in image subtraction?
+        # f) BACKEND_4SUBTRACT : Which backend would you like to perform SFFT subtraction on? (Cupy/Numpy)
+        # h) NUM_CPU_THREADS_4SUBTRACT: How many CPU threads would you want to perform SFFT subtraction on? (Numpy)
+        #
         """
-
-        if BACKEND_4SUBTRACT == 'Pycuda':
-            SFFTConfig = SingleSFFTConfigure_Pycuda.SSCP(NX=NX, NY=NY, KerHW=KerHW, \
-                KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-                CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
         
         if BACKEND_4SUBTRACT == 'Cupy':
             SFFTConfig = SingleSFFTConfigure_Cupy.SSCC(NX=NX, NY=NY, KerHW=KerHW, \
                 KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-                CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
+                VERBOSE_LEVEL=VERBOSE_LEVEL)
         
         if BACKEND_4SUBTRACT == 'Numpy':
             SFFTConfig = SingleSFFTConfigure_Numpy.SSCN(NX=NX, NY=NY, KerHW=KerHW, \
                 KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-                NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
+                NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)
         
         return SFFTConfig
-
-class BatchSFFTConfigure:
-    @staticmethod
-    def BSCP(NX, NY, KerHW_CLst, KerPolyOrder=2, BGPolyOrder=2, ConstPhotRatio=True, \
-        BACKEND_4SUBTRACT='Pycuda', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
-    
-        SFFTConfig_Dict = {}
-        for KerHW in KerHW_CLst:            
-            SFFTConfig = SingleSFFTConfigure.SSC(NX=NX, NY=NY, KerHW=KerHW, \
-                KerPolyOrder=KerPolyOrder, BGPolyOrder=BGPolyOrder, ConstPhotRatio=ConstPhotRatio, \
-                BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, \
-                NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
-            SFFTConfig_Dict[KerHW] = SFFTConfig
-
-        return SFFTConfig_Dict
```

### Comparing `sfft-1.3.4/sfft/sfftcore/SFFTSubtract.py` & `sfft-1.4.0/sfft/sfftcore/SFFTSubtract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,561 +1,46 @@
-import os
-import sys
 import time
 import numpy as np
+# version: Feb 25, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.1"
-
-class ElementalSFFTSubtract_Pycuda:
-    @staticmethod
-    def ESSP(PixA_I, PixA_J, SFFTConfig, SFFTSolution=None, Subtract=False, CUDA_DEVICE_4SUBTRACT='0'):
-
-        import warnings
-        import pycuda.autoinit
-        from pycuda.cumath import exp
-        import pycuda.gpuarray as gpuarray
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            import skcuda.fft as cu_fft
-            import skcuda.linalg as sklinalg
-            import skcuda.cusolver as sksolver
-        os.environ["CUDA_DEVICE"] = CUDA_DEVICE_4SUBTRACT
-
-        def LSSolver(LHMAT_GPU, RHb_GPU):
-
-            H, W = LHMAT_GPU.shape
-            A_GPU = LHMAT_GPU.T.copy().astype(np.float64)
-            b_GPU = RHb_GPU.copy().astype(np.float64)
-
-            handle = sksolver.cusolverDnCreate()
-            Lwork = sksolver.cusolverDnDgetrf_bufferSize(handle, H, W, A_GPU.gpudata, H)
-            workspace_gpu = gpuarray.zeros(Lwork, dtype=np.float64)
-
-            devipiv_GPU = gpuarray.zeros(min(A_GPU.shape), dtype=np.int64)
-            devinfo_GPU = gpuarray.zeros(1, dtype=np.int64)
-
-            # * LU decomposition 
-            sksolver.cusolverDnDgetrf(handle=handle, m=H, n=W, \
-                a=A_GPU.gpudata, lda=H, workspace=workspace_gpu.gpudata, \
-                devIpiv=devipiv_GPU.gpudata, devInfo=devinfo_GPU.gpudata)
-
-            # * cusolver-based (~200 times faster than np.linalg.solve)
-            sksolver.cusolverDnDgetrs(handle=handle, trans="n", n=H, nrhs=1, a=A_GPU.gpudata, lda=H, \
-                devIpiv=devipiv_GPU.gpudata, B=b_GPU.gpudata, ldb=H, devInfo=devinfo_GPU.gpudata)
-            sksolver.cusolverDnDestroy(handle)
-            Solution_GPU = b_GPU
-
-            return Solution_GPU
-
-        ta = time.time()
-        # * Read SFFT parameters
-        print('\n  --||--||--||--||-- TRIGGER SFFT SUBTRACTION --||--||--||--||-- ')
-        print('\n  ---||--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---||--- '\
-            %(SFFTConfig[0]['DK'], SFFTConfig[0]['DB'], SFFTConfig[0]['w0']))
-
-        SFFTParam_dict, SFFTModule_dict = SFFTConfig
-        N0, N1 = SFFTParam_dict['N0'], SFFTParam_dict['N1']
-        w0, w1 = SFFTParam_dict['w0'], SFFTParam_dict['w1']
-        DK, DB = SFFTParam_dict['DK'], SFFTParam_dict['DB']
-
-        if PixA_I.shape != (N0, N1) or PixA_J.shape != (N0, N1):
-            sys.exit('MeLOn ERROR: Inconsistent Shape of Input Images I & J, required [%d, %d] !' %(N0, N1))
-
-        ConstPhotRatio = SFFTParam_dict['ConstPhotRatio']
-        MaxThreadPerB = SFFTParam_dict['MaxThreadPerB']
-        
-        L0, L1 = SFFTParam_dict['L0'], SFFTParam_dict['L1']
-        Fab, Fij, Fpq = SFFTParam_dict['Fab'], SFFTParam_dict['Fij'], SFFTParam_dict['Fpq']
-        SCALE, SCALE_L = SFFTParam_dict['SCALE'], SFFTParam_dict['SCALE_L']
-
-        NEQ, Fijab = SFFTParam_dict['NEQ'], SFFTParam_dict['Fijab']
-        NEQ_FSfree = SFFTParam_dict['NEQ_FSfree']
-
-        FOMG, FGAM = SFFTParam_dict['FOMG'], SFFTParam_dict['FGAM']
-        FTHE, FPSI = SFFTParam_dict['FTHE'], SFFTParam_dict['FPSI']
-        FPHI, FDEL = SFFTParam_dict['FPHI'], SFFTParam_dict['FDEL']
-        
-        # * Grid-Block-Thread Managaement [Pixel-Level]
-        GPUManage = lambda NT: ((NT-1)//MaxThreadPerB + 1, min(NT, MaxThreadPerB))
-        BpG_PIX0, TpB_PIX0 = GPUManage(N0)
-        BpG_PIX1, TpB_PIX1 = GPUManage(N1)
-        BpG_PIX, TpB_PIX = (BpG_PIX0, BpG_PIX1), (TpB_PIX0, TpB_PIX1, 1)
-
-        # * Define First-order MultiIndex Reference
-        REF_pq = np.array([(p, q) for p in range(DB+1) for q in range(DB+1-p)]).astype(np.int32)
-        REF_ij = np.array([(i, j) for i in range(DK+1) for j in range(DK+1-i)]).astype(np.int32)
-        REF_ab = np.array([(a_pos-w0, b_pos-w1) for a_pos in range(L0) for b_pos in range(L1)]).astype(np.int32)
-        REF_pq_GPU = gpuarray.to_gpu(REF_pq)
-        REF_ij_GPU = gpuarray.to_gpu(REF_ij)
-        REF_ab_GPU = gpuarray.to_gpu(REF_ab)
-
-        # * Define Second-order MultiIndex Reference
-        SREF_iji0j0 = np.array([(ij, i0j0) for ij in range(Fij) for i0j0 in range(Fij)]).astype(np.int32)
-        SREF_pqp0q0 = np.array([(pq, p0q0) for pq in range(Fpq) for p0q0 in range(Fpq)]).astype(np.int32)
-        SREF_ijpq = np.array([(ij, pq) for ij in range(Fij) for pq in range(Fpq)]).astype(np.int32)
-        SREF_pqij = np.array([(pq, ij) for pq in range(Fpq) for ij in range(Fij)]).astype(np.int32)
-        SREF_ijab = np.array([(ij, ab) for ij in range(Fij) for ab in range(Fab)]).astype(np.int32)
-
-        SREF_iji0j0_GPU = gpuarray.to_gpu(SREF_iji0j0)
-        SREF_pqp0q0_GPU = gpuarray.to_gpu(SREF_pqp0q0)
-        SREF_ijpq_GPU = gpuarray.to_gpu(SREF_ijpq)
-        SREF_pqij_GPU = gpuarray.to_gpu(SREF_pqij)
-        SREF_ijab_GPU = gpuarray.to_gpu(SREF_ijab)
-
-        # * Define the Forbidden ij-ab Rule
-        ij00 = np.arange(w0 * L1 + w1, Fijab, Fab).astype(np.int32)
-        if ConstPhotRatio:
-            FBijab = ij00[1:]
-            MASK_nFS = np.ones(NEQ).astype(bool)
-            MASK_nFS[FBijab] = False            
-            IDX_nFS = np.where(MASK_nFS)[0].astype(np.int32)
-            IDX_nFS_GPU = gpuarray.to_gpu(IDX_nFS)
-            NEQ_FSfree = len(IDX_nFS)
-
-        t0 = time.time()
-        # * Read input images as C-order arrays
-        if not PixA_I.flags['C_CONTIGUOUS']:
-            PixA_I = np.ascontiguousarray(PixA_I, np.float64)
-            PixA_I_GPU = gpuarray.to_gpu(PixA_I)
-        else: PixA_I_GPU = gpuarray.to_gpu(PixA_I.astype(np.float64))
-        
-        if not PixA_J.flags['C_CONTIGUOUS']:
-            PixA_J = np.ascontiguousarray(PixA_J, np.float64)
-            PixA_J_GPU = gpuarray.to_gpu(PixA_J)
-        else: PixA_J_GPU = gpuarray.to_gpu(PixA_J.astype(np.float64))
-        dt0 = time.time() - t0
-
-        # * Symbol Convention NOTE
-        #    X (x) / Y (y) ----- pixel row / column index
-        #    CX (cx) / CY (cy) ----- ScaledFortranCoor of pixel (x, y) center   
-        #    e.g. pixel (x, y) = (3, 5) corresponds (cx, cy) = (4.0/N0, 6.0/N1)
-        #    NOTE cx / cy is literally \mathtt{x} / \mathtt{y} in sfft paper.
-        #    NOTE Without special definition, MeLOn convention refers to X (x) / Y (y) as FortranCoor.
-
-        # * Get Spatial Coordinates
-        t1 = time.time()
-        PixA_X_GPU = gpuarray.zeros((N0, N1), dtype=np.int32)      # row index, [0, N0)
-        PixA_Y_GPU = gpuarray.zeros((N0, N1), dtype=np.int32)      # column index, [0, N1)
-        PixA_CX_GPU = gpuarray.zeros((N0, N1), dtype=np.float64)   # coordinate.x
-        PixA_CY_GPU = gpuarray.zeros((N0, N1), dtype=np.float64)   # coordinate.y 
-
-        _module = SFFTModule_dict['SpatialCoor']
-        _func = _module.get_function('kmain')
-        _func(PixA_X_GPU, PixA_Y_GPU, PixA_CX_GPU, PixA_CY_GPU, block=TpB_PIX, grid=BpG_PIX)
-
-        # * Spatial Polynomial terms Tij, Iij, Tpq
-        SPixA_Tij_GPU = gpuarray.zeros((Fij, N0, N1), dtype=np.float64)
-        SPixA_Iij_GPU = gpuarray.zeros((Fij, N0, N1), dtype=np.float64)
-        SPixA_Tpq_GPU = gpuarray.zeros((Fpq, N0, N1), dtype=np.float64)
-
-        _module = SFFTModule_dict['SpatialPoly']
-        _func = _module.get_function('kmain')
-        _func(REF_ij_GPU, REF_pq_GPU, PixA_CX_GPU, PixA_CY_GPU, PixA_I_GPU, \
-            SPixA_Tij_GPU, SPixA_Iij_GPU, SPixA_Tpq_GPU, block=TpB_PIX, grid=BpG_PIX)
-        PixA_I_GPU.gpudata.free()
-        dt1 = time.time() - t1
-
-        t2 = time.time()
-        # * Empirical Trick on FFT-Plan
-        EmpFFTPlan = False
-        plan_once = cu_fft.Plan((N0, N1), np.complex128, np.complex128)
-        if DK == 2 and DB == 2:
-            EmpFFTPlan = True
-            plan_12 = cu_fft.Plan((N0, N1), np.complex128, np.complex128, 12)
-
-        # * Make DFT of J, Iij, Tpq and their conjugates
-        if EmpFFTPlan:
-            PixA_FJ_GPU = PixA_J_GPU.astype(np.complex128)
-            cu_fft.fft(PixA_FJ_GPU, PixA_FJ_GPU, plan_once, scale=True)
-
-            _SPixA_FFT_GPU = gpuarray.empty((12, N0, N1), dtype=np.complex128)
-            _SPixA_FFT_GPU[:6, :] = SPixA_Iij_GPU.astype(np.complex128)
-            _SPixA_FFT_GPU[6:, :] = SPixA_Tpq_GPU.astype(np.complex128)
-
-            cu_fft.fft(_SPixA_FFT_GPU, _SPixA_FFT_GPU, plan_12, scale=True)
-            SPixA_FIij_GPU = _SPixA_FFT_GPU[:6, :]
-            SPixA_FTpq_GPU = _SPixA_FFT_GPU[6:, :]
-            
-        if not EmpFFTPlan:
-            Batchsize = 1 + Fij + Fpq
-            _SPixA_FFT_GPU = gpuarray.empty((Batchsize, N0, N1), dtype=np.complex128)
-            _SPixA_FFT_GPU[0, :, :] = PixA_J_GPU.astype(np.complex128)
-            _SPixA_FFT_GPU[1: Fij+1, :, :] = SPixA_Iij_GPU.astype(np.complex128)
-            _SPixA_FFT_GPU[Fij+1:, :, :] = SPixA_Tpq_GPU.astype(np.complex128)
-
-            plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, Batchsize)
-            cu_fft.fft(_SPixA_FFT_GPU, _SPixA_FFT_GPU, plan, scale=True)
-            PixA_FJ_GPU = _SPixA_FFT_GPU[0, :, :]
-            SPixA_FIij_GPU = _SPixA_FFT_GPU[1: Fij+1, :, :]
-            SPixA_FTpq_GPU = _SPixA_FFT_GPU[Fij+1:, :, :]
-
-        SPixA_Iij_GPU.gpudata.free()
-        SPixA_Tpq_GPU.gpudata.free()
-
-        PixA_CFJ_GPU = sklinalg.conj(PixA_FJ_GPU)
-        SPixA_CFIij_GPU = sklinalg.conj(SPixA_FIij_GPU)
-        SPixA_CFTpq_GPU = sklinalg.conj(SPixA_FTpq_GPU)
-        dt2 = time.time() - t2
-        dta = time.time() - ta
-
-        print('\nMeLOn CheckPoint: Priminary Time     [%.4fs]' %dta)
-        print('/////   a   ///// Read Input Images  (%.4fs)' %dt0)
-        print('/////   b   ///// Spatial Polynomial (%.4fs)' %dt1)
-        print('/////   c   ///// DFT-%d             (%.4fs)' %(1 + Fij + Fpq, dt2))
-
-        # * Consider The Major Sources of the Linear System 
-        #     𝛀_i8j8ij     &    𝜦_i8j8pq    ||     𝚯_i8j8
-        #     𝜳_p8q8ij     &    𝚽_p8q8pq    ||     𝚫_p8q8   
-        #
-        # * Remarks
-        #    a. They have consistent form: Greek(rho, eps) = PreGreek(Mod_N0(rho), Mod_N1(eps))
-        #    b. PreGreek = s * Re[DFT(HpGreek)], where HpGreek = GLH * GRH and s is some real-scale.
-        #    c. Considering the subscripted variables, HpGreek / PreGreek is Complex / Real 3D with shape (F_Greek, N0, N1).
-        
-        if SFFTSolution is not None:
-            Solution = SFFTSolution 
-            Solution_GPU = gpuarray.to_gpu(Solution.astype(np.float64))
-            a_ijab_GPU = Solution_GPU[: Fijab]
-            b_pq_GPU = Solution_GPU[Fijab: ]
-
-        if SFFTSolution is None:
-            tb = time.time()
-            # * Grid-Block-Thread Managaement [for Greek]
-            BpG_OMG0, TpB_OMG0 = GPUManage(Fijab)
-            BpG_OMG1, TpB_OMG1 = GPUManage(Fijab)
-            BpG_OMG, TpB_OMG = (BpG_OMG0, BpG_OMG1), (TpB_OMG0, TpB_OMG1, 1)
-
-            BpG_GAM0, TpB_GAM0 = GPUManage(Fijab)
-            BpG_GAM1, TpB_GAM1 = GPUManage(Fpq)
-            BpG_GAM, TpB_GAM = (BpG_GAM0, BpG_GAM1), (TpB_GAM0, TpB_GAM1, 1)
-
-            BpG_THE0, TpB_THE0 = GPUManage(Fijab)
-            BpG_THE, TpB_THE = (BpG_THE0, 1), (TpB_THE0, 1, 1)
-
-            BpG_PSI0, TpB_PSI0 = GPUManage(Fpq)
-            BpG_PSI1, TpB_PSI1 = GPUManage(Fijab)
-            BpG_PSI, TpB_PSI = (BpG_PSI0, BpG_PSI1), (TpB_PSI0, TpB_PSI1, 1)
-
-            BpG_PHI0, TpB_PHI0 = GPUManage(Fpq)
-            BpG_PHI1, TpB_PHI1 = GPUManage(Fpq)
-            BpG_PHI, TpB_PHI = (BpG_PHI0, BpG_PHI1), (TpB_PHI0, TpB_PHI1, 1)
-
-            BpG_DEL0, TpB_DEL0 = GPUManage(Fpq)
-            BpG_DEL, TpB_DEL = (BpG_DEL0, 1), (TpB_DEL0, 1, 1)
-
-            LHMAT_GPU = gpuarray.empty((NEQ, NEQ), dtype=np.float64)
-            RHb_GPU = gpuarray.empty(NEQ, dtype=np.float64)
-            t3 = time.time()
-
-            # * -- -- -- -- -- -- -- -- Establish Linear System through 𝛀  -- -- -- -- -- -- -- -- *
-
-            # a. Hadamard Product for 𝛀 [HpOMG]
-            _module = SFFTModule_dict['HadProd_OMG']
-            _func = _module.get_function('kmain')
-            HpOMG_GPU = gpuarray.empty((FOMG, N0, N1), dtype=np.complex128)
-            _func(SREF_iji0j0_GPU, SPixA_FIij_GPU, SPixA_CFIij_GPU, HpOMG_GPU, \
-                block=TpB_PIX, grid=BpG_PIX)
-
-            # b. PreOMG = SCALE * Re[DFT(HpOMG)]
-            if EmpFFTPlan:
-                cu_fft.fft(HpOMG_GPU[:12], HpOMG_GPU[:12], plan_12, scale=True)
-                cu_fft.fft(HpOMG_GPU[12: 24], HpOMG_GPU[12: 24], plan_12, scale=True)
-                cu_fft.fft(HpOMG_GPU[24: 36], HpOMG_GPU[24: 36], plan_12, scale=True)
-
-            if not EmpFFTPlan:
-                plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, FOMG)
-                cu_fft.fft(HpOMG_GPU, HpOMG_GPU, plan, scale=True)
-
-            HpOMG_GPU = HpOMG_GPU.real 
-            HpOMG_GPU *= SCALE 
-            PreOMG_GPU = HpOMG_GPU
-
-            # c. Fill Linear System with PreOMG
-            _module = SFFTModule_dict['FillLS_OMG']
-            _func = _module.get_function('kmain')
-            _func(SREF_ijab_GPU, REF_ab_GPU, PreOMG_GPU, LHMAT_GPU, \
-                block=TpB_OMG, grid=BpG_OMG)
-
-            PreOMG_GPU.gpudata.free()
-            dt3 = time.time() - t3
-
-            t4 = time.time()
-            # * -- -- -- -- -- -- -- -- Establish Linear System through 𝜦  -- -- -- -- -- -- -- -- *
-
-            # a. Hadamard Product for 𝜦 [HpGAM]
-            _module = SFFTModule_dict['HadProd_GAM']
-            _func = _module.get_function('kmain')
-            HpGAM_GPU = gpuarray.empty((FGAM, N0, N1), dtype=np.complex128)
-            _func(SREF_ijpq_GPU, SPixA_FIij_GPU, SPixA_CFTpq_GPU, HpGAM_GPU, \
-                block=TpB_PIX, grid=BpG_PIX)
-
-            # b. PreGAM = 1 * Re[DFT(HpGAM)]
-            if EmpFFTPlan:
-                cu_fft.fft(HpGAM_GPU[:12], HpGAM_GPU[:12], plan_12, scale=True)
-                cu_fft.fft(HpGAM_GPU[12: 24], HpGAM_GPU[12: 24], plan_12, scale=True)
-                cu_fft.fft(HpGAM_GPU[24: 36], HpGAM_GPU[24: 36], plan_12, scale=True)
-
-            if not EmpFFTPlan:
-                plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, FGAM)
-                cu_fft.fft(HpGAM_GPU, HpGAM_GPU, plan, scale=True)
-
-            HpGAM_GPU = HpGAM_GPU.real 
-            PreGAM_GPU = HpGAM_GPU
-
-            # c. Fill Linear System with PreGAM
-            _module = SFFTModule_dict['FillLS_GAM']
-            _func = _module.get_function('kmain')
-            _func(SREF_ijab_GPU, REF_ab_GPU, PreGAM_GPU, LHMAT_GPU, \
-                block=TpB_GAM, grid=BpG_GAM)
-
-            PreGAM_GPU.gpudata.free()
-            dt4 = time.time() - t4
-
-            t5 = time.time()
-            # * -- -- -- -- -- -- -- -- Establish Linear System through 𝜳  -- -- -- -- -- -- -- -- *
-            
-            # a. Hadamard Product for 𝜳  [HpPSI]
-            _module = SFFTModule_dict['HadProd_PSI']
-            _func = _module.get_function('kmain')
-            HpPSI_GPU = gpuarray.empty((FPSI, N0, N1), dtype=np.complex128)
-            _func(SREF_pqij_GPU, SPixA_CFIij_GPU, SPixA_FTpq_GPU, HpPSI_GPU, \
-                block=TpB_PIX, grid=BpG_PIX)
-
-            # b. PrePSI = 1 * Re[DFT(HpPSI)]
-            if EmpFFTPlan:
-                cu_fft.fft(HpPSI_GPU[:12], HpPSI_GPU[:12], plan_12, scale=True)
-                cu_fft.fft(HpPSI_GPU[12: 24], HpPSI_GPU[12: 24], plan_12, scale=True)
-                cu_fft.fft(HpPSI_GPU[24: 36], HpPSI_GPU[24: 36], plan_12, scale=True)
-
-            if not EmpFFTPlan:
-                plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, FPSI)
-                cu_fft.fft(HpPSI_GPU, HpPSI_GPU, plan, scale=True)
-
-            HpPSI_GPU = HpPSI_GPU.real
-            PrePSI_GPU = HpPSI_GPU
-
-            # c. Fill Linear System with PrePSI
-            _module = SFFTModule_dict['FillLS_PSI']
-            _func = _module.get_function('kmain')
-            _func(SREF_ijab_GPU, REF_ab_GPU, PrePSI_GPU, LHMAT_GPU, \
-                block=TpB_PSI, grid=BpG_PSI)
-
-            PrePSI_GPU.gpudata.free()
-            dt5 = time.time() - t5
-
-            t6 = time.time()
-            # * -- -- -- -- -- -- -- -- Establish Linear System through 𝚽  -- -- -- -- -- -- -- -- *
-            
-            
-            # a. Hadamard Product for 𝚽  [HpPHI]
-            _module = SFFTModule_dict['HadProd_PHI']
-            _func = _module.get_function('kmain')
-            HpPHI_GPU = gpuarray.empty((FPHI, N0, N1), dtype=np.complex128)
-            _func(SREF_pqp0q0_GPU, SPixA_FTpq_GPU, SPixA_CFTpq_GPU, HpPHI_GPU, \
-                block=TpB_PIX, grid=BpG_PIX)
-
-            # b. PrePHI = SCALE_L * Re[DFT(HpPHI)]
-            if EmpFFTPlan:
-                cu_fft.fft(HpPHI_GPU[:12], HpPHI_GPU[:12], plan_12, scale=True)
-                cu_fft.fft(HpPHI_GPU[12: 24], HpPHI_GPU[12: 24], plan_12, scale=True)
-                cu_fft.fft(HpPHI_GPU[24: 36], HpPHI_GPU[24: 36], plan_12, scale=True)
-
-            if not EmpFFTPlan:
-                plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, FPHI)
-                cu_fft.fft(HpPHI_GPU, HpPHI_GPU, plan, scale=True)
-
-            HpPHI_GPU = HpPHI_GPU.real
-            HpPHI_GPU *= SCALE_L
-            PrePHI_GPU = HpPHI_GPU
-
-            # c. Fill Linear System with PrePHI
-            _module = SFFTModule_dict['FillLS_PHI']
-            _func = _module.get_function('kmain')
-            _func(PrePHI_GPU, LHMAT_GPU, block=TpB_PHI, grid=BpG_PHI)
-
-            PrePHI_GPU.gpudata.free()
-            dt6 = time.time() - t6
-
-            t7 = time.time()
-            # * -- -- -- -- -- -- -- -- Establish Linear System through 𝚯 & 𝚫  -- -- -- -- -- -- -- -- *
-
-            # a1. Hadamard Product for 𝚯  [HpTHE]
-            _module = SFFTModule_dict['HadProd_THE']
-            _func = _module.get_function('kmain')
-            HpTHE_GPU = gpuarray.empty((FTHE, N0, N1), dtype=np.complex128)
-            _func(SPixA_FIij_GPU, PixA_CFJ_GPU, HpTHE_GPU, block=TpB_PIX, grid=BpG_PIX)
-
-            # a2. Hadamard Product for 𝚫  [HpDEL]
-            _module = SFFTModule_dict['HadProd_DEL']
-            _func = _module.get_function('kmain')
-            HpDEL_GPU = gpuarray.empty((FDEL, N0, N1), dtype=np.complex128)
-            _func(SPixA_FTpq_GPU, PixA_CFJ_GPU, HpDEL_GPU, block=TpB_PIX, grid=BpG_PIX)
-
-            # b1. PreTHE = 1 * Re[DFT(HpTHE)]
-            # b2. PreDEL = SCALE_L * Re[DFT(HpDEL)]
-            if EmpFFTPlan:
-                SPixA_FFT_GPU = gpuarray.empty((12, N0, N1), dtype=np.complex128)
-                SPixA_FFT_GPU[:6, :] = HpTHE_GPU
-                SPixA_FFT_GPU[6:, :] = HpDEL_GPU
-                HpTHE_GPU.gpudata.free()
-                HpDEL_GPU.gpudata.free()
-                
-                cu_fft.fft(SPixA_FFT_GPU, SPixA_FFT_GPU, plan_12, scale=True)
-                HpTHE_GPU = SPixA_FFT_GPU[:6, :]
-                HpDEL_GPU = SPixA_FFT_GPU[6:, :]
-
-            if not EmpFFTPlan:
-                plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, FTHE)
-                cu_fft.fft(HpTHE_GPU, HpTHE_GPU, plan, scale=True)
-
-                plan = cu_fft.Plan((N0, N1), np.complex128, np.complex128, FDEL)
-                cu_fft.fft(HpDEL_GPU, HpDEL_GPU, plan, scale=True)
-            
-            HpTHE_GPU = HpTHE_GPU.real
-            PreTHE_GPU = HpTHE_GPU
-
-            HpDEL_GPU = HpDEL_GPU.real
-            HpDEL_GPU *= SCALE_L
-            PreDEL_GPU = HpDEL_GPU
-
-            # c1. Fill Linear System with PreTHE
-            _module = SFFTModule_dict['FillLS_THE']
-            _func = _module.get_function('kmain')
-            _func(SREF_ijab_GPU, REF_ab_GPU, PreTHE_GPU, RHb_GPU, \
-                block=TpB_THE, grid=BpG_THE)
-            PreTHE_GPU.gpudata.free()
-
-            # c2. Fill Linear System with PreDEL
-            _module = SFFTModule_dict['FillLS_DEL']
-            _func = _module.get_function('kmain')
-            _func(PreDEL_GPU, RHb_GPU, block=TpB_DEL, grid=BpG_DEL)
-            
-            PreDEL_GPU.gpudata.free()
-            dt7 = time.time() - t7
-
-            # * -- -- -- -- -- -- -- -- Remove Forbidden Stripes  -- -- -- -- -- -- -- -- *
-            if not ConstPhotRatio: pass
-            if ConstPhotRatio:
-                RHb_FSfree_GPU = gpuarray.take(RHb_GPU, IDX_nFS_GPU)
-                _module = SFFTModule_dict['Remove_LSFStripes']
-                _func = _module.get_function('kmain')
-                BpG_FSfree_PA, TpB_FSfree_PA = GPUManage(NEQ_FSfree)     # Per Axis
-                BpG_FSfree, TpB_FSfree = (BpG_FSfree_PA, BpG_FSfree_PA), (TpB_FSfree_PA, TpB_FSfree_PA, 1)
-                LHMAT_FSfree_GPU = gpuarray.empty((NEQ_FSfree, NEQ_FSfree), dtype=np.float64)
-                _func(LHMAT_GPU, IDX_nFS_GPU, LHMAT_FSfree_GPU, block=TpB_FSfree, grid=BpG_FSfree)
-
-            t8 = time.time()
-            # * -- -- -- -- -- -- -- -- Solve Linear System  -- -- -- -- -- -- -- -- *
-            if not ConstPhotRatio: 
-                Solution_GPU = LSSolver(LHMAT_GPU=LHMAT_GPU, RHb_GPU=RHb_GPU)
-
-            if ConstPhotRatio:
-                # Extend the solution to be consistent form
-                Solution_FSfree_GPU = LSSolver(LHMAT_GPU=LHMAT_FSfree_GPU, RHb_GPU=RHb_FSfree_GPU)
-                _module = SFFTModule_dict['Extend_Solution']
-                _func = _module.get_function('kmain')
-                BpG_ES, TpB_ES = (BpG_FSfree_PA, 1), (TpB_FSfree_PA, 1, 1)
-                Solution_GPU = gpuarray.zeros(NEQ, dtype=np.float64)
-                _func(Solution_FSfree_GPU, IDX_nFS_GPU, Solution_GPU, block=TpB_ES, grid=BpG_ES)
-            
-            a_ijab_GPU = Solution_GPU[: Fijab]
-            b_pq_GPU = Solution_GPU[Fijab: ]
-            Solution = Solution_GPU.get()
-            dt8 = time.time() - t8
-            dtb = time.time() - tb
-
-            print('\nMeLOn CheckPoint: Establish & Solve Linear System     [%.4fs]' %dtb)
-            print('/////   d   ///// Establish OMG                       (%.4fs)' %dt3)
-            print('/////   e   ///// Establish GAM                       (%.4fs)' %dt4)
-            print('/////   f   ///// Establish PSI                       (%.4fs)' %dt5)
-            print('/////   g   ///// Establish PHI                       (%.4fs)' %dt6)
-            print('/////   h   ///// Establish THE & DEL                 (%.4fs)' %dt7)
-            print('/////   i   ///// Solve                               (%.4fs)' %dt8)
-
-        # * Perform Subtraction 
-        PixA_DIFF = None
-        if Subtract:
-            tc = time.time()
-            t9 = time.time()
-            # Calculate Kab components
-            Wl_GPU = exp((-2j*np.pi/N0) * PixA_X_GPU.astype(np.float64))    # row index l, [0, N0)
-            Wm_GPU = exp((-2j*np.pi/N1) * PixA_Y_GPU.astype(np.float64))    # column index m, [0, N1)
-            Kab_Wla_GPU = gpuarray.empty((L0, N0, N1), dtype=np.complex128)
-            Kab_Wmb_GPU = gpuarray.empty((L1, N0, N1), dtype=np.complex128)
-
-            if w0 == w1:
-                wx = w0   # a little bit faster
-                for aob in range(-wx, wx+1):
-                    Kab_Wla_GPU[aob + wx] = Wl_GPU ** aob    # offset 
-                    Kab_Wmb_GPU[aob + wx] = Wm_GPU ** aob    # offset 
-            else:
-                for a in range(-w0, w0+1): 
-                    Kab_Wla_GPU[a + w0] = Wl_GPU ** a      # offset 
-                for b in range(-w1, w1+1): 
-                    Kab_Wmb_GPU[b + w1] = Wm_GPU ** b      # offset 
-            dt9 = time.time() - t9
-
-            t10 = time.time()
-            # Construct Difference in Fourier Space
-            _module = SFFTModule_dict['Construct_FDIFF']
-            _func = _module.get_function('kmain')     
-            PixA_FDIFF_GPU = gpuarray.empty((N0, N1), dtype=np.complex128)
-            _func(SREF_ijab_GPU, REF_ab_GPU, a_ijab_GPU.astype(np.complex128), \
-                SPixA_FIij_GPU, Kab_Wla_GPU, Kab_Wmb_GPU, b_pq_GPU.astype(np.complex128), \
-                SPixA_FTpq_GPU, PixA_FJ_GPU, PixA_FDIFF_GPU, block=TpB_PIX, grid=BpG_PIX)
-            
-            # Get Difference & Reconstructed Images
-            PixA_DIFF_GPU = gpuarray.empty_like(PixA_FDIFF_GPU)
-            cu_fft.ifft(PixA_FDIFF_GPU, PixA_DIFF_GPU, plan_once, scale=False)
-            PixA_DIFF_GPU = PixA_DIFF_GPU.real
-            PixA_DIFF = PixA_DIFF_GPU.get()
-            dt10 = time.time() - t10
-            dtc = time.time() - tc
-
-            print('\nMeLOn CheckPoint: Perform Subtraction     [%.4fs]' %dtc)
-            print('/////   j   ///// Calculate Kab           (%.4fs)' %dt9)
-            print('/////   k   ///// Construct DIFF        (%.4fs)' %dt10)
-        
-        print('\n  --||--||--||--||-- EXIT SFFT SUBTRACTION --||--||--||--||-- ')
-
-        return Solution, PixA_DIFF
+__version__ = "v1.4"
 
 class ElementalSFFTSubtract_Cupy:
     @staticmethod
-    def ESSC(PixA_I, PixA_J, SFFTConfig, SFFTSolution=None, Subtract=False, CUDA_DEVICE_4SUBTRACT='0'):
-
+    def ESSC(PixA_I, PixA_J, SFFTConfig, SFFTSolution=None, Subtract=False, VERBOSE_LEVEL=2):
+        
         import cupy as cp
         import cupyx.scipy.linalg as cpx_linalg
-        os.environ["CUDA_DEVICE"] = CUDA_DEVICE_4SUBTRACT
 
         def LSSolver(LHMAT_GPU, RHb_GPU):
             """
-            # deprecated cupy version (moderately slow)
+            # NOTE: cupy/numpy (moderately/extremely) slow version has been DEPRECATED!
             Solution_GPU = cp.linalg.solve(LHMAT_GPU, RHb_GPU)
-            # deprecated numpy version (very slow)
             Solution_GPU = cp.array(np.linalg.solve(cp.asnumpy(LHMAT_GPU), cp.asnumpy(RHb_GPU)), dtype=np.float64)
             """
             lu_piv_GPU = cpx_linalg.lu_factor(LHMAT_GPU, overwrite_a=False, check_finite=True)
             Solution_GPU = cpx_linalg.lu_solve(lu_piv_GPU, RHb_GPU)
             return Solution_GPU
-
+        
         ta = time.time()
         # * Read SFFT parameters
-        print('\n  --||--||--||--||-- TRIGGER SFFT SUBTRACTION --||--||--||--||-- ')
-        print('\n  ---||--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---||--- '\
-            %(SFFTConfig[0]['DK'], SFFTConfig[0]['DB'], SFFTConfig[0]['w0']))
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --||--||--||--||-- TRIGGER SFFT SUBTRACTION --||--||--||--||-- ')
+            print('\n ---||--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---||--- '\
+                   %(SFFTConfig[0]['DK'], SFFTConfig[0]['DB'], SFFTConfig[0]['w0']))
 
         SFFTParam_dict, SFFTModule_dict = SFFTConfig
         N0, N1 = SFFTParam_dict['N0'], SFFTParam_dict['N1']
         w0, w1 = SFFTParam_dict['w0'], SFFTParam_dict['w1']
         DK, DB = SFFTParam_dict['DK'], SFFTParam_dict['DB']
 
         if PixA_I.shape != (N0, N1) or PixA_J.shape != (N0, N1):
-            sys.exit('MeLOn ERROR: Inconsistent Shape of Input Images I & J, required [%d, %d] !' %(N0, N1))
+            _error_message = 'INCONSISTENT shape of input images I & J, [%d, %d] required!' %(N0, N1)
+            raise Exception('MeLOn ERROR: %s' %_error_message)
 
         ConstPhotRatio = SFFTParam_dict['ConstPhotRatio']
         MaxThreadPerB = SFFTParam_dict['MaxThreadPerB']
         
         L0, L1 = SFFTParam_dict['L0'], SFFTParam_dict['L1']
         Fab, Fij, Fpq = SFFTParam_dict['Fab'], SFFTParam_dict['Fij'], SFFTParam_dict['Fpq']
         SCALE, SCALE_L = SFFTParam_dict['SCALE'], SFFTParam_dict['SCALE_L']
@@ -631,76 +116,70 @@
         PixA_CX_GPU = cp.zeros((N0, N1), dtype=np.float64)   # coordinate.x
         PixA_CY_GPU = cp.zeros((N0, N1), dtype=np.float64)   # coordinate.y 
 
         _module = SFFTModule_dict['SpatialCoor']
         _func = _module.get_function('kmain')
         _func(args=(PixA_X_GPU, PixA_Y_GPU, PixA_CX_GPU, PixA_CY_GPU), block=TpB_PIX, grid=BpG_PIX)
 
-        # * Spatial Polynomial terms Tij, Iij, Tpq
-        SPixA_Tij_GPU = cp.zeros((Fij, N0, N1), dtype=np.float64)
+        # * Spatial Polynomial terms Iij, Tpq
         SPixA_Iij_GPU = cp.zeros((Fij, N0, N1), dtype=np.float64)
         SPixA_Tpq_GPU = cp.zeros((Fpq, N0, N1), dtype=np.float64)
 
         _module = SFFTModule_dict['SpatialPoly']
         _func = _module.get_function('kmain')
         _func(args=(REF_ij_GPU, REF_pq_GPU, PixA_CX_GPU, PixA_CY_GPU, PixA_I_GPU, \
-            SPixA_Tij_GPU, SPixA_Iij_GPU, SPixA_Tpq_GPU), block=TpB_PIX, grid=BpG_PIX)
+            SPixA_Iij_GPU, SPixA_Tpq_GPU), block=TpB_PIX, grid=BpG_PIX)
         
         del PixA_I_GPU
         dt1 = time.time() - t1
 
         t2 = time.time()
-        # * Empirical Trick on FFT-Plan
-        EmpFFTPlan = False
-        if DK == 2 and DB == 2:
-            EmpFFTPlan = True
 
         """
-        # may be alternative to perform FFT
+        # alternative way to perform FFT
         import cupyx as cpx
         plan = cpx.scipy.fftpack.get_fft_plan(x)
         y = cpx.scipy.fftpack.fftn(x, plan=plan)
-
+        
         """
 
         # * Make DFT of J, Iij, Tpq and their conjugates
-        if EmpFFTPlan:
-            PixA_FJ_GPU = SCALE * cp.fft.fft2(PixA_J_GPU)
-            _SPixA_FFT_GPU = cp.empty((12, N0, N1), dtype=np.complex128)
-            _SPixA_FFT_GPU[:6, :] = SPixA_Iij_GPU.astype(np.complex128)
-            _SPixA_FFT_GPU[6:, :] = SPixA_Tpq_GPU.astype(np.complex128)  
-            _SPixA_FFT_GPU = SCALE * cp.fft.fft2(_SPixA_FFT_GPU)
-            SPixA_FIij_GPU = _SPixA_FFT_GPU[:6, :]
-            SPixA_FTpq_GPU = _SPixA_FFT_GPU[6:, :]
-
-        if not EmpFFTPlan:
-            Batchsize = 1 + Fij + Fpq
-            _SPixA_FFT_GPU = cp.empty((Batchsize, N0, N1), dtype=np.complex128)
-            _SPixA_FFT_GPU[0, :, :] = PixA_J_GPU.astype(np.complex128)
-            _SPixA_FFT_GPU[1: Fij+1, :, :] = SPixA_Iij_GPU.astype(np.complex128)
-            _SPixA_FFT_GPU[Fij+1:, :, :] = SPixA_Tpq_GPU.astype(np.complex128)
-            
-            _SPixA_FFT_GPU = SCALE * cp.fft.fft2(_SPixA_FFT_GPU)
-            PixA_FJ_GPU = _SPixA_FFT_GPU[0, :, :]
-            SPixA_FIij_GPU = _SPixA_FFT_GPU[1: Fij+1, :, :]
-            SPixA_FTpq_GPU = _SPixA_FFT_GPU[Fij+1:, :, :]
+        PixA_FJ_GPU = cp.empty((N0, N1), dtype=np.complex128)
+        PixA_FJ_GPU[:, :] = PixA_J_GPU.astype(np.complex128)
+        PixA_FJ_GPU[:, :] = cp.fft.fft2(PixA_FJ_GPU)
+        PixA_FJ_GPU[:, :] *= SCALE
+
+        SPixA_FIij_GPU = cp.empty((Fij, N0, N1), dtype=np.complex128)
+        SPixA_FIij_GPU[:, :, :] = SPixA_Iij_GPU.astype(np.complex128)
+        for k in range(Fij): 
+            SPixA_FIij_GPU[k: k+1] = cp.fft.fft2(SPixA_FIij_GPU[k: k+1])
+        SPixA_FIij_GPU[:, :] *= SCALE
+
+        SPixA_FTpq_GPU = cp.empty((Fpq, N0, N1), dtype=np.complex128)
+        SPixA_FTpq_GPU[:, :, :] = SPixA_Tpq_GPU.astype(np.complex128)
+        for k in range(Fpq): 
+            SPixA_FTpq_GPU[k: k+1] = cp.fft.fft2(SPixA_FTpq_GPU[k: k+1])
+        SPixA_FTpq_GPU[:, :] *= SCALE
 
         del SPixA_Iij_GPU
         del SPixA_Tpq_GPU
 
         PixA_CFJ_GPU = cp.conj(PixA_FJ_GPU)
         SPixA_CFIij_GPU = cp.conj(SPixA_FIij_GPU)
         SPixA_CFTpq_GPU = cp.conj(SPixA_FTpq_GPU)
         dt2 = time.time() - t2
         dta = time.time() - ta
 
-        print('\nMeLOn CheckPoint: Priminary Time     [%.4fs]' %dta)
-        print('/////   a   ///// Read Input Images  (%.4fs)' %dt0)
-        print('/////   b   ///// Spatial Polynomial (%.4fs)' %dt1)
-        print('/////   c   ///// DFT-%d             (%.4fs)' %(1 + Fij + Fpq, dt2))
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\nMeLOn CheckPoint: SFFT-SUBTRACTION Preliminary Steps takes [%.4fs]' %dta)
+
+        if VERBOSE_LEVEL in [2]:
+            print('/////   a   ///// Read Input Images  (%.4fs)' %dt0)
+            print('/////   b   ///// Spatial Polynomial (%.4fs)' %dt1)
+            print('/////   c   ///// DFT-%d             (%.4fs)' %(1 + Fij + Fpq, dt2))
 
         # * Consider The Major Sources of the Linear System 
         #     𝛀_i8j8ij     &    𝜦_i8j8pq    ||     𝚯_i8j8
         #     𝜳_p8q8ij     &    𝚽_p8q8pq    ||     𝚫_p8q8   
         #
         # * Remarks
         #    a. They have consistent form: Greek(rho, eps) = PreGreek(Mod_N0(rho), Mod_N1(eps))
@@ -748,23 +227,21 @@
             _module = SFFTModule_dict['HadProd_OMG']
             _func = _module.get_function('kmain')
             HpOMG_GPU = cp.empty((FOMG, N0, N1), dtype=np.complex128)
             _func(args=(SREF_iji0j0_GPU, SPixA_FIij_GPU, SPixA_CFIij_GPU, HpOMG_GPU), \
                 block=TpB_PIX, grid=BpG_PIX)
 
             # b. PreOMG = SCALE * Re[DFT(HpOMG)]
-            if EmpFFTPlan:
-                HpOMG_GPU[:12] = SCALE * cp.fft.fft2(HpOMG_GPU[:12])
-                HpOMG_GPU[12: 24] = SCALE * cp.fft.fft2(HpOMG_GPU[12: 24])
-                HpOMG_GPU[24: 36] = SCALE * cp.fft.fft2(HpOMG_GPU[24: 36])
-
-            if not EmpFFTPlan:
-                HpOMG_GPU = SCALE * cp.fft.fft2(HpOMG_GPU)
-
-            PreOMG_GPU = cp.array(SCALE * HpOMG_GPU.real, dtype=np.float64)
+            for k in range(FOMG):
+                HpOMG_GPU[k: k+1] = cp.fft.fft2(HpOMG_GPU[k: k+1])
+            HpOMG_GPU *= SCALE
+
+            PreOMG_GPU = cp.empty((FOMG, N0, N1), dtype=np.float64)
+            PreOMG_GPU[:, :, :] = HpOMG_GPU.real
+            PreOMG_GPU[:, :, :] *= SCALE
             del HpOMG_GPU
 
             # c. Fill Linear System with PreOMG
             _module = SFFTModule_dict['FillLS_OMG']
             _func = _module.get_function('kmain')
             _func(args=(SREF_ijab_GPU, REF_ab_GPU, PreOMG_GPU, LHMAT_GPU), \
                 block=TpB_OMG, grid=BpG_OMG)
@@ -779,23 +256,20 @@
             _module = SFFTModule_dict['HadProd_GAM']
             _func = _module.get_function('kmain')
             HpGAM_GPU = cp.empty((FGAM, N0, N1), dtype=np.complex128)
             _func(args=(SREF_ijpq_GPU, SPixA_FIij_GPU, SPixA_CFTpq_GPU, HpGAM_GPU), \
                 block=TpB_PIX, grid=BpG_PIX)
 
             # b. PreGAM = 1 * Re[DFT(HpGAM)]
-            if EmpFFTPlan:
-                HpGAM_GPU[:12] = SCALE * cp.fft.fft2(HpGAM_GPU[:12])
-                HpGAM_GPU[12: 24] = SCALE * cp.fft.fft2(HpGAM_GPU[12: 24])
-                HpGAM_GPU[24: 36] = SCALE * cp.fft.fft2(HpGAM_GPU[24: 36])
+            for k in range(FGAM):
+                HpGAM_GPU[k: k+1] = cp.fft.fft2(HpGAM_GPU[k: k+1])
+            HpGAM_GPU *= SCALE
 
-            if not EmpFFTPlan:
-                HpGAM_GPU = SCALE * cp.fft.fft2(HpGAM_GPU)
-            
-            PreGAM_GPU = cp.array(HpGAM_GPU.real, dtype=np.float64)
+            PreGAM_GPU = cp.empty((FGAM, N0, N1), dtype=np.float64)
+            PreGAM_GPU[:, :, :] = HpGAM_GPU.real
             del HpGAM_GPU
 
             # c. Fill Linear System with PreGAM
             _module = SFFTModule_dict['FillLS_GAM']
             _func = _module.get_function('kmain')
             _func(args=(SREF_ijab_GPU, REF_ab_GPU, PreGAM_GPU, LHMAT_GPU), \
                 block=TpB_GAM, grid=BpG_GAM)
@@ -810,23 +284,20 @@
             _module = SFFTModule_dict['HadProd_PSI']
             _func = _module.get_function('kmain')
             HpPSI_GPU = cp.empty((FPSI, N0, N1), dtype=np.complex128)
             _func(args=(SREF_pqij_GPU, SPixA_CFIij_GPU, SPixA_FTpq_GPU, HpPSI_GPU), \
                 block=TpB_PIX, grid=BpG_PIX)
 
             # b. PrePSI = 1 * Re[DFT(HpPSI)]
-            if EmpFFTPlan:
-                HpPSI_GPU[:12] = SCALE * cp.fft.fft2(HpPSI_GPU[:12])
-                HpPSI_GPU[12: 24] = SCALE * cp.fft.fft2(HpPSI_GPU[12: 24])
-                HpPSI_GPU[24: 36] = SCALE * cp.fft.fft2(HpPSI_GPU[24: 36])
+            for k in range(FPSI):
+                HpPSI_GPU[k: k+1] = cp.fft.fft2(HpPSI_GPU[k: k+1])
+            HpPSI_GPU *= SCALE
 
-            if not EmpFFTPlan:
-                HpPSI_GPU = SCALE * cp.fft.fft2(HpPSI_GPU)
-
-            PrePSI_GPU = cp.array(HpPSI_GPU.real, dtype=np.float64)
+            PrePSI_GPU = cp.empty((FPSI, N0, N1), dtype=np.float64)
+            PrePSI_GPU[:, :, :] = HpPSI_GPU.real
             del HpPSI_GPU
 
             # c. Fill Linear System with PrePSI
             _module = SFFTModule_dict['FillLS_PSI']
             _func = _module.get_function('kmain')
             _func(args=(SREF_ijab_GPU, REF_ab_GPU, PrePSI_GPU, LHMAT_GPU), \
                 block=TpB_PSI, grid=BpG_PSI)
@@ -841,23 +312,21 @@
             _module = SFFTModule_dict['HadProd_PHI']
             _func = _module.get_function('kmain')
             HpPHI_GPU = cp.empty((FPHI, N0, N1), dtype=np.complex128)
             _func(args=(SREF_pqp0q0_GPU, SPixA_FTpq_GPU, SPixA_CFTpq_GPU, HpPHI_GPU), \
                 block=TpB_PIX, grid=BpG_PIX)
 
             # b. PrePHI = SCALE_L * Re[DFT(HpPHI)]
-            if EmpFFTPlan:
-                HpPHI_GPU[:12] = SCALE * cp.fft.fft2(HpPHI_GPU[:12])
-                HpPHI_GPU[12: 24] = SCALE * cp.fft.fft2(HpPHI_GPU[12: 24])
-                HpPHI_GPU[24: 36] = SCALE * cp.fft.fft2(HpPHI_GPU[24: 36])
-
-            if not EmpFFTPlan:
-                HpPHI_GPU = SCALE * cp.fft.fft2(HpPHI_GPU)
-
-            PrePHI_GPU = cp.array(SCALE_L * HpPHI_GPU.real, dtype=np.float64)
+            for k in range(FPHI):
+                HpPHI_GPU[k: k+1] = cp.fft.fft2(HpPHI_GPU[k: k+1])
+            HpPHI_GPU *= SCALE
+
+            PrePHI_GPU = cp.empty((FPHI, N0, N1), dtype=np.float64)
+            PrePHI_GPU[:, :, :] = HpPHI_GPU.real
+            PrePHI_GPU[:, :, :] *= SCALE_L
             del HpPHI_GPU
 
             # c. Fill Linear System with PrePHI
             _module = SFFTModule_dict['FillLS_PHI']
             _func = _module.get_function('kmain')
             _func(args=(PrePHI_GPU, LHMAT_GPU), block=TpB_PHI, grid=BpG_PHI)
 
@@ -877,33 +346,31 @@
             _module = SFFTModule_dict['HadProd_DEL']
             _func = _module.get_function('kmain')
             HpDEL_GPU = cp.empty((FDEL, N0, N1), dtype=np.complex128)
             _func(args=(SPixA_FTpq_GPU, PixA_CFJ_GPU, HpDEL_GPU), block=TpB_PIX, grid=BpG_PIX)
 
             # b1. PreTHE = 1 * Re[DFT(HpTHE)]
             # b2. PreDEL = SCALE_L * Re[DFT(HpDEL)]
-            if EmpFFTPlan:
-                _SPixA_FFT_GPU = cp.empty((12, N0, N1), dtype=np.complex128)
-                _SPixA_FFT_GPU[:6, :] = HpTHE_GPU
-                _SPixA_FFT_GPU[6:, :] = HpDEL_GPU
-                del HpTHE_GPU
-                del HpDEL_GPU                
-                _SPixA_FFT_GPU = SCALE * cp.fft.fft2(_SPixA_FFT_GPU)
-                HpTHE_GPU = _SPixA_FFT_GPU[:6, :]
-                HpDEL_GPU = _SPixA_FFT_GPU[6:, :]
-
-            if not EmpFFTPlan:
-                HpTHE_GPU = SCALE * cp.fft.fft2(HpTHE_GPU)
-                HpDEL_GPU = SCALE * cp.fft.fft2(HpDEL_GPU)
+            for k in range(FTHE):
+                HpTHE_GPU[k: k+1] = cp.fft.fft2(HpTHE_GPU[k: k+1])
+            HpTHE_GPU[:, :, :] *= SCALE
+            
+            for k in range(FDEL):
+                HpDEL_GPU[k: k+1] = cp.fft.fft2(HpDEL_GPU[k: k+1])
+            HpDEL_GPU[:, :, :] *= SCALE
 
-            PreTHE_GPU = cp.array(HpTHE_GPU.real, dtype=np.float64)
-            PreDEL_GPU = cp.array(SCALE_L * HpDEL_GPU.real, dtype=np.float64)
+            PreTHE_GPU = cp.empty((FTHE, N0, N1), dtype=np.float64)
+            PreTHE_GPU[:, :, :] = HpTHE_GPU.real
             del HpTHE_GPU
+            
+            PreDEL_GPU = cp.empty((FDEL, N0, N1), dtype=np.float64)
+            PreDEL_GPU[:, :, :] = HpDEL_GPU.real
+            PreDEL_GPU[:, :, :] *= SCALE_L
             del HpDEL_GPU
-
+            
             # c1. Fill Linear System with PreTHE
             _module = SFFTModule_dict['FillLS_THE']
             _func = _module.get_function('kmain')
             _func(args=(SREF_ijab_GPU, REF_ab_GPU, PreTHE_GPU, RHb_GPU), \
                 block=TpB_THE, grid=BpG_THE)
             del PreTHE_GPU
 
@@ -942,21 +409,24 @@
             
             a_ijab_GPU = Solution_GPU[: Fijab]
             b_pq_GPU = Solution_GPU[Fijab: ]
             Solution = cp.asnumpy(Solution_GPU)
             dt8 = time.time() - t8
             dtb = time.time() - tb
 
-            print('\nMeLOn CheckPoint: Establish & Solve Linear System     [%.4fs]' %dtb)
-            print('/////   d   ///// Establish OMG                       (%.4fs)' %dt3)
-            print('/////   e   ///// Establish GAM                       (%.4fs)' %dt4)
-            print('/////   f   ///// Establish PSI                       (%.4fs)' %dt5)
-            print('/////   g   ///// Establish PHI                       (%.4fs)' %dt6)
-            print('/////   h   ///// Establish THE & DEL                 (%.4fs)' %dt7)
-            print('/////   i   ///// Solve                               (%.4fs)' %dt8)
+            if VERBOSE_LEVEL in [1, 2]:
+                print('\nMeLOn CheckPoint: SFFT-SUBTRACTION Establish & Solve Linear System takes [%.4fs]' %dtb)
+
+            if VERBOSE_LEVEL in [2]:
+                print('/////   d   ///// Establish OMG                       (%.4fs)' %dt3)
+                print('/////   e   ///// Establish GAM                       (%.4fs)' %dt4)
+                print('/////   f   ///// Establish PSI                       (%.4fs)' %dt5)
+                print('/////   g   ///// Establish PHI                       (%.4fs)' %dt6)
+                print('/////   h   ///// Establish THE & DEL                 (%.4fs)' %dt7)
+                print('/////   i   ///// Solve Linear System                 (%.4fs)' %dt8)
 
         # * Perform Subtraction 
         PixA_DIFF = None
         if Subtract:
             tc = time.time()
             t9 = time.time()
             # Calculate Kab components
@@ -988,47 +458,51 @@
             
             # Get Difference & Reconstructed Images
             PixA_DIFF_GPU = SCALE_L * cp.fft.ifft2(PixA_FDIFF_GPU)
             PixA_DIFF = cp.asnumpy(PixA_DIFF_GPU.real)
             dt10 = time.time() - t10
             dtc = time.time() - tc
 
-            print('\nMeLOn CheckPoint: Perform Subtraction     [%.4fs]' %dtc)
-            print('/////   j   ///// Calculate Kab           (%.4fs)' %dt9)
-            print('/////   k   ///// Construct DIFF        (%.4fs)' %dt10)
+            if VERBOSE_LEVEL in [1, 2]:
+                print('\nMeLOn CheckPoint: SFFT-SUBTRACTION Perform Subtraction takes [%.4fs]' %dtc)
+            
+            if VERBOSE_LEVEL in [2]:
+                print('/////   j   ///// Calculate Kab         (%.4fs)' %dt9)
+                print('/////   k   ///// Construct DIFF        (%.4fs)' %dt10)
         
-        print('\n  --||--||--||--||-- EXIT SFFT SUBTRACTION --||--||--||--||-- ')
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --||--||--||--||-- EXIT SFFT SUBTRACTION --||--||--||--||-- ')
 
-        return Solution, PixA_DIFF    
+        return Solution, PixA_DIFF
 
 class ElementalSFFTSubtract_Numpy:
     @staticmethod
-    def ESSN(PixA_I, PixA_J, SFFTConfig, SFFTSolution=None, Subtract=False, NUM_CPU_THREADS_4SUBTRACT=8):
+    def ESSN(PixA_I, PixA_J, SFFTConfig, SFFTSolution=None, Subtract=False, NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
 
         import pyfftw
         pyfftw.config.NUM_THREADS = NUM_CPU_THREADS_4SUBTRACT
         pyfftw.interfaces.cache.enable()
         
         ta = time.time()
         # * Read SFFT parameters
-        print('\n  --||--||--||--||-- TRIGGER SFFT SUBTRACTION --||--||--||--||-- ')
-        print('\n  ---||--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---||--- '\
-            %(SFFTConfig[0]['DK'], SFFTConfig[0]['DB'], SFFTConfig[0]['w0']))
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --||--||--||--||-- TRIGGER SFFT SUBTRACTION --||--||--||--||-- ')
+            print('\n ---||--- KerPolyOrder %d | BGPolyOrder %d | KerHW [%d] ---||--- '\
+                   %(SFFTConfig[0]['DK'], SFFTConfig[0]['DB'], SFFTConfig[0]['w0']))
 
         SFFTParam_dict, SFFTModule_dict = SFFTConfig
         N0, N1 = SFFTParam_dict['N0'], SFFTParam_dict['N1']
         w0, w1 = SFFTParam_dict['w0'], SFFTParam_dict['w1']
         DK, DB = SFFTParam_dict['DK'], SFFTParam_dict['DB']
 
         if PixA_I.shape != (N0, N1) or PixA_J.shape != (N0, N1):
-            sys.exit('MeLOn ERROR: Inconsistent Shape of Input Images I & J, required [%d, %d] !' %(N0, N1))
+            _error_message = 'INCONSISTENT shape of input images I & J, [%d, %d] required!' %(N0, N1)
+            raise Exception('MeLOn ERROR: %s' %_error_message)
 
         ConstPhotRatio = SFFTParam_dict['ConstPhotRatio']
-        MaxThreadPerB = SFFTParam_dict['MaxThreadPerB']
-
         L0, L1 = SFFTParam_dict['L0'], SFFTParam_dict['L1']
         Fab, Fij, Fpq = SFFTParam_dict['Fab'], SFFTParam_dict['Fij'], SFFTParam_dict['Fpq']
         SCALE, SCALE_L = SFFTParam_dict['SCALE'], SFFTParam_dict['SCALE_L']
 
         NEQ, Fijab = SFFTParam_dict['NEQ'], SFFTParam_dict['Fijab']
         NEQ_FSfree = SFFTParam_dict['NEQ_FSfree']
 
@@ -1081,22 +555,21 @@
         PixA_Y = np.zeros((N0, N1), dtype=np.int32)      # column index, [0, N1)
         PixA_CX = np.zeros((N0, N1), dtype=np.float64)   # coordinate.x
         PixA_CY = np.zeros((N0, N1), dtype=np.float64)   # coordinate.y 
 
         _func = SFFTModule_dict['SpatialCoor']
         _func(PixA_X=PixA_X, PixA_Y=PixA_Y, PixA_CX=PixA_CX, PixA_CY=PixA_CY)
 
-        # * Spatial Polynomial terms Tij, Iij, Tpq
-        SPixA_Tij = np.zeros((Fij, N0, N1), dtype=np.float64)
+        # * Spatial Polynomial terms Iij, Tpq
         SPixA_Iij = np.zeros((Fij, N0, N1), dtype=np.float64)
         SPixA_Tpq = np.zeros((Fpq, N0, N1), dtype=np.float64)
 
         _func = SFFTModule_dict['SpatialPoly']
-        _func(REF_ij=REF_ij, REF_pq=REF_pq, PixA_CX=PixA_CX, PixA_CY=PixA_CY, PixA_I=PixA_I, \
-            SPixA_Tij=SPixA_Tij, SPixA_Iij=SPixA_Iij, SPixA_Tpq=SPixA_Tpq)
+        _func(REF_ij=REF_ij, REF_pq=REF_pq, PixA_CX=PixA_CX, PixA_CY=PixA_CY, \
+            PixA_I=PixA_I, SPixA_Iij=SPixA_Iij, SPixA_Tpq=SPixA_Tpq)
         dt1 = time.time() - t1
 
         t2 = time.time()
         Batchsize = 1 + Fij + Fpq
         _SPixA_FFT = np.empty((Batchsize, N0, N1), dtype=np.complex128)
         _SPixA_FFT[0, :, :] = PixA_J.astype(np.complex128)
         _SPixA_FFT[1: Fij+1, :, :] = SPixA_Iij.astype(np.complex128)
@@ -1111,18 +584,21 @@
 
         PixA_CFJ = np.conj(PixA_FJ)
         SPixA_CFIij = np.conj(SPixA_FIij)
         SPixA_CFTpq = np.conj(SPixA_FTpq)
         dt2 = time.time() - t2
         dta = time.time() - ta
 
-        print('\nMeLOn CheckPoint: Priminary Time     [%.4fs]' %dta)
-        print('/////   a   ///// Read Input Images  (%.4fs)' %dt0)
-        print('/////   b   ///// Spatial Polynomial (%.4fs)' %dt1)
-        print('/////   c   ///// DFT-%d             (%.4fs)' %(1 + Fij + Fpq, dt2))
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\nMeLOn CheckPoint: SFFT-SUBTRACTION Preliminary Steps takes [%.4fs]' %dta)
+
+        if VERBOSE_LEVEL in [2]:
+            print('/////   a   ///// Read Input Images  (%.4fs)' %dt0)
+            print('/////   b   ///// Spatial Polynomial (%.4fs)' %dt1)
+            print('/////   c   ///// DFT-%d             (%.4fs)' %(1 + Fij + Fpq, dt2))
 
         # * Consider The Major Sources of the Linear System 
         #     𝛀_i8j8ij     &    𝜦_i8j8pq    ||     𝚯_i8j8
         #     𝜳_p8q8ij     &    𝚽_p8q8pq    ||     𝚫_p8q8   
         #
         # * Remarks
         #    a. They have consistent form: Greek(rho, eps) = PreGreek(Mod_N0(rho), Mod_N1(eps))
@@ -1277,21 +753,24 @@
 
             a_ijab = Solution[: Fijab]
             b_pq = Solution[Fijab: ]
 
             dt8 = time.time() - t8
             dtb = time.time() - tb
 
-            print('\nMeLOn CheckPoint: Establish & Solve Linear System     [%.4fs]' %dtb)
-            print('/////   d   ///// Establish OMG                       (%.4fs)' %dt3)
-            print('/////   e   ///// Establish GAM                       (%.4fs)' %dt4)
-            print('/////   f   ///// Establish PSI                       (%.4fs)' %dt5)
-            print('/////   g   ///// Establish PHI                       (%.4fs)' %dt6)
-            print('/////   h   ///// Establish THE & DEL                 (%.4fs)' %dt7)
-            print('/////   i   ///// Solve                               (%.4fs)' %dt8)
+            if VERBOSE_LEVEL in [1, 2]:
+                print('\nMeLOn CheckPoint: SFFT-SUBTRACTION Establish & Solve Linear System takes [%.4fs]' %dtb)
+
+            if VERBOSE_LEVEL in [2]:
+                print('/////   d   ///// Establish OMG                       (%.4fs)' %dt3)
+                print('/////   e   ///// Establish GAM                       (%.4fs)' %dt4)
+                print('/////   f   ///// Establish PSI                       (%.4fs)' %dt5)
+                print('/////   g   ///// Establish PHI                       (%.4fs)' %dt6)
+                print('/////   h   ///// Establish THE & DEL                 (%.4fs)' %dt7)
+                print('/////   i   ///// Solve Linear System                 (%.4fs)' %dt8)
         
         # * Perform Subtraction
         PixA_DIFF = None
         if Subtract:
 
             tc = time.time()
             t9 = time.time()
@@ -1325,120 +804,122 @@
             PixA_DIFF = np.empty_like(PixA_FDIFF)
             PixA_DIFF[:, :] = SCALE_L * pyfftw.interfaces.numpy_fft.ifft2(PixA_FDIFF)
             
             PixA_DIFF = PixA_DIFF.real
             dt10 = time.time() - t10
             dtc = time.time() - tc
 
-            print('\nMeLOn CheckPoint: Perform Subtraction     [%.4fs]' %dtc)
-            print('/////   j   ///// Calculate Kab           (%.4fs)' %dt9)
-            print('/////   k   ///// Construct DIFF        (%.4fs)' %dt10)
+            if VERBOSE_LEVEL in [1, 2]:
+                print('\nMeLOn CheckPoint: SFFT-SUBTRACTION Perform Subtraction takes [%.4fs]' %dtc)
+            
+            if VERBOSE_LEVEL in [2]:
+                print('/////   j   ///// Calculate Kab         (%.4fs)' %dt9)
+                print('/////   k   ///// Construct DIFF        (%.4fs)' %dt10)
         
-        print('\n  --||--||--||--||-- EXIT SFFT SUBTRACTION --||--||--||--||-- ')
+        if VERBOSE_LEVEL in [1, 2]:
+            print('\n --||--||--||--||-- EXIT SFFT SUBTRACTION --||--||--||--||-- ')
 
         return Solution, PixA_DIFF
 
 class ElementalSFFTSubtract:
     @staticmethod
     def ESS(PixA_I, PixA_J, SFFTConfig, SFFTSolution=None, Subtract=False, \
-        BACKEND_4SUBTRACT='Pycuda', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
+        BACKEND_4SUBTRACT='Cupy', NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
 
-        if BACKEND_4SUBTRACT == 'Pycuda':
-            Solution, PixA_DIFF = ElementalSFFTSubtract_Pycuda.ESSP(PixA_I=PixA_I, PixA_J=PixA_J, SFFTConfig=SFFTConfig, \
-                SFFTSolution=SFFTSolution, Subtract=Subtract, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
-        
         if BACKEND_4SUBTRACT == 'Cupy':
-            Solution, PixA_DIFF = ElementalSFFTSubtract_Cupy.ESSC(PixA_I=PixA_I, PixA_J=PixA_J, SFFTConfig=SFFTConfig, \
-                SFFTSolution=SFFTSolution, Subtract=Subtract, CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT)
+            Solution, PixA_DIFF = ElementalSFFTSubtract_Cupy.ESSC(PixA_I=PixA_I, PixA_J=PixA_J, \
+                SFFTConfig=SFFTConfig, SFFTSolution=SFFTSolution, Subtract=Subtract, VERBOSE_LEVEL=VERBOSE_LEVEL)
 
         if BACKEND_4SUBTRACT == 'Numpy':
-            Solution, PixA_DIFF = ElementalSFFTSubtract_Numpy.ESSN(PixA_I=PixA_I, PixA_J=PixA_J, SFFTConfig=SFFTConfig, \
-                SFFTSolution=SFFTSolution, Subtract=Subtract, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)
+            Solution, PixA_DIFF = ElementalSFFTSubtract_Numpy.ESSN(PixA_I=PixA_I, PixA_J=PixA_J, \
+                SFFTConfig=SFFTConfig, SFFTSolution=SFFTSolution, Subtract=Subtract, \
+                NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)
         
         return Solution, PixA_DIFF
 
 class GeneralSFFTSubtract:
     @staticmethod
     def GSS(PixA_I, PixA_J, PixA_mI, PixA_mJ, SFFTConfig, ContamMask_I=None, \
-        BACKEND_4SUBTRACT='Pycuda', CUDA_DEVICE_4SUBTRACT='0', NUM_CPU_THREADS_4SUBTRACT=8):
+        BACKEND_4SUBTRACT='Cupy', NUM_CPU_THREADS_4SUBTRACT=8, VERBOSE_LEVEL=2):
 
         """
+        # Perform image subtraction on I & J with SFFT parameters solved from mI & mJ.
+        #
         # Arguments:
         # a) PixA_I: Image I that will be convolved [NaN-Free]
         # b) PixA_J: Image J that won't be convolved [NaN-Free]
         # c) PixA_mI: Masked version of Image I. 'same' means it is identical with I [NaN-Free]
         # d) PixA_mJ: Masked version of Image J. 'same' means it is identical with J [NaN-Free]
         # e) SFFTConfig: Configuration of SFFT
         # f) ContamMask_I: Contaminate-Region in Image I (e.g., Saturation and Bad pixels).
-        #               We will calculate the propagated Contaminate-Region on convolved I.
+        #                  We will calculate the propagated Contaminate-Region on convolved I.
         # 
-        # g) BACKEND_4SUBTRACT: Which backend would you like to perform SFFT subtraction on ?
-        # h) CUDA_DEVICE_4SUBTRACT (BACKEND_4SUBTRACT = Pycuda / Cupy): Which GPU device would you want to perform SFFT subtraction on ?
-        # i) NUM_CPU_THREADS_4SUBTRACT (BACKEND_4SUBTRACT = Numpy): How many CPU threads would you want to perform SFFT subtraction on ?
-        #
-        # NOTE: The SFFT parameter-solving is performed between mI & mJ, 
-        #       then we apply the solution to input Images I & J.
+        # g) BACKEND_4SUBTRACT: Which backend would you like to perform SFFT subtraction on? (Cupy/Numpy)
+        # i) NUM_CPU_THREADS_4SUBTRACT: How many CPU threads would you want to perform SFFT subtraction on? (Numpy)
         #
         """
         
-        print(r"""
+        SFFT_BANNER = r"""
                                 __    __    __    __
                                /  \  /  \  /  \  /  \
                               /    \/    \/    \/    \
             █████████████████/  /██/  /██/  /██/  /█████████████████████████
                             /  / \   / \   / \   / \  \____
                            /  /   \_/   \_/   \_/   \    o \__,
                           / _/                       \_____/  `
                           |/
-
+        
                       █████████  ███████████ ███████████ ███████████        
                      ███░░░░░███░░███░░░░░░█░░███░░░░░░█░█░░░███░░░█            
                     ░███    ░░░  ░███   █ ░  ░███   █ ░ ░   ░███  ░ 
                     ░░█████████  ░███████    ░███████       ░███    
                      ░░░░░░░░███ ░███░░░█    ░███░░░█       ░███    
                      ███    ░███ ░███  ░     ░███  ░        ░███    
                     ░░█████████  █████       █████          █████   
                      ░░░░░░░░░  ░░░░░       ░░░░░          ░░░░░         
-
+        
                     Saccadic Fast Fourier Transform (SFFT) algorithm
                     sfft (v1.*) supported by @LeiHu
-
+        
                     GitHub: https://github.com/thomasvrussell/sfft
                     Related Paper: https://arxiv.org/abs/2109.09334
                     
             ████████████████████████████████████████████████████████████████
             
-            """)
+            """
+        
+        if VERBOSE_LEVEL in [2]:
+            print(SFFT_BANNER)
         
-        # * Size-Check Processes
-        tmplst = [PixA_I.shape, PixA_J.shape]
-        tmplst += [PixA_mI.shape, PixA_mI.shape]
+        # * Size-Check
+        tmplst = [PixA_I.shape, PixA_J.shape, PixA_mI.shape, PixA_mI.shape]
         if len(set(tmplst)) > 1:
-            sys.exit('MeLOn ERROR: Input images should have same size !')
-
+            raise Exception('MeLOn ERROR: Input images should have same size!')
+        
         # * Subtraction Solution derived from input masked image-pair
         Solution = ElementalSFFTSubtract.ESS(PixA_I=PixA_mI, PixA_J=PixA_mJ, \
             SFFTConfig=SFFTConfig, SFFTSolution=None, Subtract=False, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-            CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)[0]
+            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)[0]
         
         # * Subtraction of the input image-pair (use above solution)
         PixA_DIFF = ElementalSFFTSubtract.ESS(PixA_I=PixA_I, PixA_J=PixA_J, \
             SFFTConfig=SFFTConfig, SFFTSolution=Solution, Subtract=True, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-            CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)[1]
-
+            NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)[1]
+        
         # * Identify propagated contamination region through convolving I
         ContamMask_CI = None
         if ContamMask_I is not None:
             tSolution = Solution.copy()
             DB = SFFTConfig[0]['DB']
             Fpq = int((DB+1)*(DB+2)/2)
             tSolution[-Fpq:] = 0.0
+
             _tmpI = ContamMask_I.astype(np.float64)
             _tmpJ = np.zeros(PixA_J.shape).astype(np.float64)
-
-            # NOTE Convolved_I is inverse DIFF
             _tmpD = ElementalSFFTSubtract.ESS(PixA_I=_tmpI, PixA_J=_tmpJ, \
                 SFFTConfig=SFFTConfig, SFFTSolution=tSolution, Subtract=True, BACKEND_4SUBTRACT=BACKEND_4SUBTRACT, \
-                CUDA_DEVICE_4SUBTRACT=CUDA_DEVICE_4SUBTRACT, NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT)[1]
-            ContamMask_CI = _tmpD < -0.001     # FIXME Customizable
+                NUM_CPU_THREADS_4SUBTRACT=NUM_CPU_THREADS_4SUBTRACT, VERBOSE_LEVEL=VERBOSE_LEVEL)[1]
+            
+            FTHRESH = -0.001  # Emperical
+            ContamMask_CI = _tmpD < FTHRESH
         
         return Solution, PixA_DIFF, ContamMask_CI
```

### Comparing `sfft-1.3.4/sfft/utils/CombineHeader.py` & `sfft-1.4.0/sfft/utils/ReadWCS.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,76 @@
-from astropy.wcs import WCS
+import warnings
+from astropy.wcs import WCS, FITSFixedWarning
+# version: Mar 17, 2023
 
-class Combine_Header:
+__author__ = "Lei Hu <hulei@pmo.ac.cn>"
+__version__ = "v1.4"
+
+class Read_WCS:
     @staticmethod
-    def CH(hdr_base, hdr_wcs):
+    def RW(hdr, VERBOSE_LEVEL=2):
 
         """
-        # Remarks on the wcs convention discrepancy between FITS header and Astropy
+        # Remarks on the WCS in FITS header and astropy.WCS
         # Case A:
-        #    FITS HEADER: 
+        #    FITS header: 
         #        CTYPE1 = 'RA---TAN'   CTYPE2 = 'DEC--TAN'
         #        CD1_1 = ...           CD1_2 = ...
         #        CD2_1 = ...           CD2_2 = ... 
         #        NOTE: NO DISTORTION TERMS!
         #    
-        #    Astropy:        
+        #    astropy.WCS:        
         #        # print(WCS(phr).to_header())
         #        CTYPE1 = 'RA---TAN'   CTYPE2 = 'DEC--TAN'
         #        PC1_1 = ...           PC1_2 = ...
         #        PC2_1 = ...           PC2_2 = ... 
         #        NOTE: if CD1_2 = CD2_1 = 0.0, then PC1_2 and PC2_1 will be absent.
-        
-        # Case B:
-        #    FITS HEADER: 
+        #
+        # Case B (Distorted tangential with the TPV FITS convention, added officially to the FITS registry in Aug. 2012):
+        #    FITS header: 
         #        CTYPE1 = 'RA---TPV'   CTYPE2 = 'DEC--TPV'
         #        CD1_1 = ...           CD1_2 = ...
         #        CD2_1 = ...           CD2_2 = ... 
         #        PV1_0 = ...           PV1_1 = ...
         #        ...
         #    
-        #    Astropy:        
+        #    astropy.WCS:        
         #        # print(WCS(phr).to_header())
         #        CTYPE1 = 'RA---TPV'   CTYPE2 = 'DEC--TPV'
         #        PC1_1 = ...           PC1_2 = ...
         #        PC2_1 = ...           PC2_2 = ... 
         #        PV1_0 = ...           PV1_1 = ...
         #        ...
         #        NOTE: if CD1_2 = CD2_1 = 0.0, then PC1_2 and PC2_1 will be absent.
         #
-        # Case B': a possible common situation that causes Astropy.WCS incompatibility.
-        #    FITS HEADER:
+        # Case B' (Distorted tangential with Greisen & Calabretta's 2000 draft, obsoleted):
+        #    FITS header:
         #        CTYPE1 = 'RA---TAN'   CTYPE2 = 'DEC--TAN'
         #        CD1_1 = ...           CD1_2 = ...
         #        CD2_1 = ...           CD2_2 = ... 
         #        PV1_0 = ...           PV1_1 = ...
         #        ...
-        #     
-        #    NOTE: One need to correct as follows to avoid the error
-        #          phr['CTYPE1'] = 'RA---TPV'
-        #          phr['CTYPE1'] = 'DEC--TPV'
-        #          w = WCS(phr)
-        #
-        #    Astropy:        
+        #    
+        #    WARNING: To avoid Astropy.WCS incompatibility, one should make corrections 
+        #        as follows before reading by Astropy.WCS
+        #        phr['CTYPE1'] = 'RA---TPV'
+        #        phr['CTYPE1'] = 'DEC--TPV'
+        #        w = WCS(phr)
+        #      
+        #    astropy.WCS:        
         #        # print(w.to_header())
         #        CTYPE1 = 'RA---TPV'   CTYPE2 = 'DEC--TPV'
         #        PC1_1 = ...           PC1_2 = ...
         #        PC2_1 = ...           PC2_2 = ... 
         #        PV1_0 = ...           PV1_1 = ...
         #        ...
         #        NOTE: if CD1_2 = CD2_1 = 0.0, then PC1_2 and PC2_1 will be absent.
-        
+        #
         # Case C:
-        #    FITS HEADER: 
+        #    FITS header: 
         #        CTYPE1 = 'RA---TAN-SIP'   CTYPE2 = 'DEC--TAN-SIP'
         #        CD1_1 = ...           CD1_2 = ...
         #        CD2_1 = ...           CD2_2 = ... 
         #        A_ORDER = 2           
         #        A_0_0 = ...           A_0_1 = ...
         #        ...
         #        B_ORDER = 2           
@@ -73,15 +79,15 @@
         #        AP_ORDER = 2           
         #        AP_0_0 = ...          AP_0_1 = ...
         #        ...
         #        BP_ORDER = 2           
         #        BP_0_0 = ...          BP_0_1 = ...
         #        ...
         #    
-        #    Astropy:        
+        #    astropy.WCS:        
         #        # print(WCS(phr).to_header(relax=True))
         #        CTYPE1 = 'RA---TAN-SIP'   CTYPE2 = 'DEC--TAN-SIP'
         #        PC1_1 = ...           PC1_2 = ...
         #        PC2_1 = ...           PC2_2 = ... 
         #        A_ORDER = 2           
         #        A_0_0 = ...           A_0_1 = ...
         #        ...
@@ -91,59 +97,25 @@
         #        AP_ORDER = 2           
         #        AP_0_0 = ...          AP_0_1 = ...
         #        ...
         #        BP_ORDER = 2           
         #        BP_0_0 = ...          BP_0_1 = ...
         #        ...
         #        NOTE: if CD1_2 = CD2_1 = 0.0, then PC1_2 and PC2_1 will be absent.
-        #        NOTE: here remember use relax=True!
-        
-        # NOTE: You may also use PC1_1 in FITS HEADER instead of CD1_1 in above cases.
-        #       It is readable, however, we do not recommend this.
+        #
+        # P.S. One may use PC1_1 to replace CD1_1 in FITS header for above cases, not recommended though.
+        #
         """
 
-        def read_wcs(hdr):
+        with warnings.catch_warnings():
+            if VERBOSE_LEVEL in [0, 1]: behavior = 'ignore'
+            if VERBOSE_LEVEL in [2]: behavior = 'default'
+            warnings.filterwarnings(behavior, category=FITSFixedWarning)
+
             if hdr['CTYPE1'] == 'RA---TAN' and 'PV1_0' in hdr:
                 _hdr = hdr.copy()
                 _hdr['CTYPE1'] = 'RA---TPV'
                 _hdr['CTYPE2'] = 'DEC--TPV'
-                w = WCS(_hdr)
-            else: w = WCS(hdr)
-            return w
-
-        # ** Remove wcs entries in hdr_base
-        hdr_b = hdr_base.copy()
-        delkeys = list(read_wcs(hdr_b).to_header(relax=True).keys())
-        if 'CD1_1' in hdr_base: 
-            delkeys += ['CD1_1', 'CD1_2', 'CD2_1', 'CD2_2']
-        if 'MJD-OBS' in delkeys:
-            delkeys.remove('MJD-OBS')
-        if 'DATE-OBS' in delkeys:
-            delkeys.remove('DATE-OBS')
-        for key in delkeys:
-            if key in hdr_b:
-                del hdr_b[key]
-        
-        # ** Extract wcs entries in hdr_wcs
-        hdr_w = hdr_wcs.copy()
-        wcshdr = read_wcs(hdr_w).to_header(relax=True)
-        if 'PC1_2' not in wcshdr: wcshdr['PC1_2'] = 0.0
-        if 'PC2_1' not in wcshdr: wcshdr['PC2_1'] = 0.0
-        if 'MJD-OBS' in wcshdr: del wcshdr['MJD-OBS']
-        if 'DATE-OBS' in wcshdr: del wcshdr['DATE-OBS']
-
-        # ** Combine 
-        hdr_op = hdr_b.copy()
-        hdr_op.update(wcshdr)
-
-        # ** Post corrections
-        if hdr_wcs['CTYPE1'] == 'RA---TAN' and 'PV1_0' in hdr_wcs:
-            hdr_op['CTYPE1'] = 'RA---TAN'
-            hdr_op['CTYPE2'] = 'DEC--TAN'
-
-        if 'CD1_1' in hdr_wcs and 'PC1_1' in hdr_op:
-            hdr_op.rename_keyword('PC1_1', 'CD1_1')
-            hdr_op.rename_keyword('PC1_2', 'CD1_2')
-            hdr_op.rename_keyword('PC2_1', 'CD2_1')
-            hdr_op.rename_keyword('PC2_2', 'CD2_2')
+            else: _hdr = hdr
+            w = WCS(_hdr)
         
-        return hdr_op
+        return w
```

### Comparing `sfft-1.3.4/sfft/utils/ConvKernelConvertion.py` & `sfft-1.4.0/sfft/utils/ConvKernelConvertion.py`

 * *Files identical despite different names*

### Comparing `sfft-1.3.4/sfft/utils/HoughMorphClassifier.py` & `sfft-1.4.0/sfft/utils/HoughMorphClassifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,198 +1,253 @@
+import skimage
 import warnings
 import numpy as np
+from pkg_resources import parse_version
 from sfft.utils.pyAstroMatic.PYSEx import PY_SEx
 from sfft.utils.HoughDetection import Hough_Detection
 from sfft.utils.WeightedQuantile import TopFlatten_Weighted_Quantile
-# version: Sep 16, 2022
+
+# version: Feb 10, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class Hough_MorphClassifier:
     
-    """
-    # @ Point-Source Extractor
-    #   A) A PSFEx suggested Morphological Classifier, based on a 2D distribution diagram
-    #      FLUX_RADIUS [X-axis] - MAG_AUTO [Y-axis], A universal but naive approach.
-    #      We first draw all isolated sources on the plane, and the typical distribution will form a 'Y' shape.
-    #      A nearly vertical branch, A nearly horizontal branch and their cross with a tail at faint side.
-    #
-    #      Here I give rough conclusions with comments, note I have compared with Legacy Survety Tractor Catalog.
-    #      a. The point sources would be distributed around the nearly vertical stright line. {vertical branch}
-    #         NOTE At the faint end, point sources no longer cling to the line, being diffuse in the cross and tail.
-    #      b. Close to the bright end of the stright-line are saturated or slight-nonlinear sources, with a deviated direction.
-    #      c. The right side of the line are typically extended structure, mainly including various galaxies. {horizontal branch}
-    #         NOTE At the faint end, likewise, extended sources also exist, being diffuse in the cross and tail.
-    #      d. Scattering points are located at very left side of the line, they are generally hotpix, cosmic-ray or 
-    #         some small-scale artifacts. Keep in mind, they are typically outlier-like and away from the cross and tail.
-    #
-    #      METHOD: For simplicity, we only crudely divide the diagram into 3 regions, w.r.t. the vetical line.
-    #              they are, Radius-Mid (FR-M), Radius-Large (FR-L) and Radius-Small (FR-S).
-    #
-    #   B) 3 hierarchic groups                
-    #      > Good Sources:
-    #        + NOT in FR-S region (union of FR-M & FR-L)
-    #          NOTE Good Sources is consist of the vertical & horizontal branches with their cross (not the tail), 
-    #               which is roughly equivalent to the set of REAL Point-Sources & Extended Sources 
-    #               with rejection the samples in the tail (at faint & small-radius end).
-    #          NOTE Good Sources are commonly used as FITTING Candidates in Image Subtraction.
-    #               It is acceptable to lose the samples in the tail.
-    #         
-    #        >> {subgroup} Point Sources:
-    #               + Restricted into FR-M Region   |||   Should be located around the Hough-Line
-    #               + Basically Circular-Shape      |||   PSFEx-ELLIPTICITY = (A-B) / (A+B) < PS_ELLIPThresh
-    #                 NOTE At cross region, this identification criteria mis-include some extended source
-    #                      On the flip side, some REAL PointSource samples are missing in the tail.
-    #                 NOTE Point Sources are usually employed as FWHM Estimator.
-    #                 NOTE We may lossen PS_ELLIPThresh if psf itself is significantly asymmetric (e.g. tracking problem).
-    #
-    #                 WARNING: At the faint end, this subgroup would be contaminated by round extended sources 
-    #                          (meet PS_ELLIPThresh) which also lie in the cross region. Especially when the field 
-    #                          is galaxy-dominated, the contamination can be considerable. In light of the fact that 
-    #                          cross region is located at the faint end in the belt, we calculate the median FWHM 
-    #                          weighted by source flux, to suppress the over-estimate trend driven by the extended sources.
-    #
-    #   C) Additional WARNINGS
-    #      a. This extracor is ONLY designed for sparse field (isolated sources dominated cases).
-    #         We usually only take these isloated & non-saturated sources (FLAGS=0) into account in this function.
-    #         Sometimes, we may loosen the constrain on FLAGS to be [0,2].
-    #
-    #      b. We employ Hough Transformation to detect the Stright-Line feature in the image, 
-    #         naturally sampled from the raw scatter diagram. But note such diagram makes sense 
-    #         only if we could detect enough sources (typically > 200) in the given image.
-    #         NOTE Reversed axes employed --- MAG_AUTO [X-axis] - FLUX_RADIUS [Y-axis].
-    #
-    """
-
-    def MakeCatalog(FITS_obj, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', \
-        BACK_TYPE='AUTO', BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, \
-        DETECT_THRESH=1.5, DETECT_MINAREA=5, DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, \
-        BACKPHOTO_TYPE='LOCAL', CHECKIMAGE_TYPE='NONE', AddRD=False, ONLY_FLAGS=[0], \
-        BoundarySIZE=30, AddSNR=True):
-
-        # * Trigger SExtractor
-        #   NOTE: it is a compromise to adopt XY rather than XYWIN for both point and extended sources.
-        #   NOTE: only takes Isolated & Non-Saturated sources (FLAGS = 0) into account.
-        #   FIXME: one may need to tune DETECT_THRESH & DETECT_MINAREA for specific program.
-
-        PL = ['X_IMAGE', 'Y_IMAGE', 'FLUX_AUTO', 'FLUXERR_AUTO', 'MAG_AUTO', 'MAGERR_AUTO', \
-              'FLAGS', 'FLUX_RADIUS', 'FWHM_IMAGE', 'A_IMAGE', 'B_IMAGE']
-        if AddSNR: PL.append('SNR_WIN')
+    def __init__(self):
+        
+        """
+        # MeLOn Notes
+        # @ Point-Source Extractor
+        #   A) A PSFEx suggested Morphological Classifier, based on a 2D distribution diagram
+        #      FLUX_RADIUS [X-axis] - MAG_AUTO [Y-axis], A universal but naive approach.
+        #      We first draw all isolated sources on the plane, and the typical distribution will form a 'Y' shape.
+        #      A nearly vertical branch, A nearly horizontal branch and their cross with a tail at faint side.
+        #
+        #      Here I give rough conclusions with comments, note I have compared with Legacy Survety Tractor Catalog.
+        #      a. The point sources would be distributed around the nearly vertical stright line. {vertical branch}
+        #         NOTE At the faint end, point sources no longer cling to the line, being diffuse in the cross and tail.
+        #      b. Close to the bright end of the stright-line are saturated or slight-nonlinear sources, with a deviated direction.
+        #      c. The right side of the line are typically extended structure, mainly including various galaxies. {horizontal branch}
+        #         NOTE At the faint end, likewise, extended sources also exist, being diffuse in the cross and tail.
+        #      d. Scattering points are located at very left side of the line, they are generally hotpix, cosmic-ray or 
+        #         some small-scale artifacts. Keep in mind, they are typically outlier-like and away from the cross and tail.
+        #
+        #      METHOD: For simplicity, we only crudely divide the diagram into 3 regions, w.r.t. the vertical line.
+        #              they are, Radius-Mid (FR-M), Radius-Large (FR-L) and Radius-Small (FR-S).
+        #
+        #   B) 3 hierarchic groups                
+        #      > "Good" Sources:
+        #        + NOT in FR-S region (union of FR-M & FR-L)
+        #          NOTE Good Sources is consist of the vertical & horizontal branches with their cross (not the tail), 
+        #               which is roughly equivalent to the set of REAL Point-Sources & Extended Sources 
+        #               with rejection the samples in the tail (at faint & small-radius end).
+        #          NOTE Good Sources are commonly used as FITTING Candidates in Image Subtraction.
+        #               It is acceptable to lose the samples in the tail.
+        #         
+        #        >> {subgroup} "Point-like" Sources:
+        #               + Restricted into FR-M Region   |||   Should be located around the Hough-Line
+        #               + Basically Circular-Shape      |||   PSFEx-ELLIPTICITY = (A-B) / (A+B) < PointSource_MINELLIP
+        #
+        #                 NOTE At cross region, this identification criteria mis-include some extended source
+        #                      On the flip side, some REAL PointSource samples are missing in the tail.
+        #                 NOTE Point Sources are usually employed as FWHM Estimator.
+        #                 NOTE We may lossen PointSource_MINELLIP if psf itself is significantly asymmetric (e.g. tracking problem).
+        #
+        #                 WARNING: At the faint end, this subgroup would be contaminated by round extended sources 
+        #                          (meet PointSource_MINELLIP) which also lie in the cross region. Especially when the field 
+        #                          is galaxy-dominated, the contamination can be considerable. In light of the fact that 
+        #                          cross region is located at the faint end in the belt, we calculate the median FWHM 
+        #                          weighted by source flux, to suppress the over-estimate trend driven by the extended sources.
+        #
+        #   C) Additional WARNINGS
+        #      a. This extracor is ONLY designed for sparse field (isolated sources dominated cases).
+        #         We generally only take these isloated & non-saturated sources (FLAGS = 0) into account.
+        #         But one may also loosen the constrain on FLAGS to be [0,2].
+        #
+        #      b. We employ Hough Transform to detect the Stright-Line feature in the image, 
+        #         naturally sampled from the raw scatter diagram. But note such diagram makes sense 
+        #         only if we could detect enough sources (typically > 200) in the given image.
+        #         NOTE Reversed axes employed --- MAG_AUTO [X-axis] - FLUX_RADIUS [Y-axis].
+        #
+        """
+
+        pass
+
+    def MakeCatalog(FITS_obj, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', BACK_TYPE='AUTO', BACK_VALUE=0.0, \
+        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=1.5, ANALYSIS_THRESH=1.5, DETECT_MINAREA=5, \
+        DETECT_MAXAREA=0, DEBLEND_MINCONT=0.005, BACKPHOTO_TYPE='LOCAL', CHECKIMAGE_TYPE='NONE', \
+        AddRD=False, ONLY_FLAGS=[0], BoundarySIZE=30, AddSNR=True, VERBOSE_LEVEL=2):
+
+        """
+        # * Remarks on the SExtractor Catalog for Hough Transform
+        #   [1] Although XYWIN can be more accurate than XY for point sources, here 
+        #       we adopt XY rather than XYWIN for both point and extended sources as a trade-off.
+        #   [2] by default, it only takes isolated & non-saturated sources (FLAGS = 0) into account.
+        #   [3] one may need to tune DETECT_THRESH & DETECT_MINAREA for a specific program.
+        #
+        """
 
-        PYSEX_OP = PY_SEx.PS(FITS_obj=FITS_obj, PL=PL, GAIN_KEY=GAIN_KEY, SATUR_KEY=SATUR_KEY, \
+        SExParam = ['X_IMAGE', 'Y_IMAGE', 'FLUX_AUTO', 'FLUXERR_AUTO', 'MAG_AUTO', 'MAGERR_AUTO', \
+                     'FLAGS', 'FLUX_RADIUS', 'FWHM_IMAGE', 'A_IMAGE', 'B_IMAGE']
+        
+        if AddSNR: SExParam.append('SNR_WIN')
+        PYSEX_OP = PY_SEx.PS(FITS_obj=FITS_obj, SExParam=SExParam, GAIN_KEY=GAIN_KEY, SATUR_KEY=SATUR_KEY, \
             BACK_TYPE=BACK_TYPE, BACK_VALUE=BACK_VALUE, BACK_SIZE=BACK_SIZE, BACK_FILTERSIZE=BACK_FILTERSIZE, \
-            DETECT_THRESH=DETECT_THRESH, DETECT_MINAREA=DETECT_MINAREA, DETECT_MAXAREA=DETECT_MAXAREA, \
-            DEBLEND_MINCONT=DEBLEND_MINCONT, BACKPHOTO_TYPE=BACKPHOTO_TYPE, CHECKIMAGE_TYPE=CHECKIMAGE_TYPE, \
-            AddRD=AddRD, ONLY_FLAGS=ONLY_FLAGS, XBoundary=BoundarySIZE, YBoundary=BoundarySIZE, MDIR=None)
+            DETECT_THRESH=DETECT_THRESH, ANALYSIS_THRESH=ANALYSIS_THRESH, DETECT_MINAREA=DETECT_MINAREA, \
+            DETECT_MAXAREA=DETECT_MAXAREA, DEBLEND_MINCONT=DEBLEND_MINCONT, BACKPHOTO_TYPE=BACKPHOTO_TYPE, \
+            CHECKIMAGE_TYPE=CHECKIMAGE_TYPE, AddRD=AddRD, ONLY_FLAGS=ONLY_FLAGS, XBoundary=BoundarySIZE, \
+            YBoundary=BoundarySIZE, MDIR=None, VERBOSE_LEVEL=VERBOSE_LEVEL)
         
         return PYSEX_OP
     
-    def Classifier(AstSEx, Hough_FRLowerLimit=0.1, Hough_peak_clip=0.7, BeltHW=0.2, PS_ELLIPThresh=0.3):
+    def Classifier(AstSEx, Hough_MINFR=0.1, Hough_MAXFR=10.0, Hough_PeakClip=0.7, \
+        BeltHW=0.2, PointSource_MINELLIP=0.3, VERBOSE_LEVEL=2):
+
+        """
+        # * calssifier based on hough detection  
+        #   We use hough transform to detect the point source belt from the scatter points 
+        #   (X: MAG_AUTO, Y: FLUX_RADIUS). The belt is a nearly horizontal straight line.
+        #
+        #   NOTE: the point source belt has a typical theta of 1.5d +/- 1.0d. on this occasion, 
+        #         we should stick with the classic implementation of hough transform in 
+        #         scikit-image [0.16.1 to 0.18.3], where the measurement bias on rho
+        #         is closer to zero than the new implementation!
+        #
+        #   NOTE: in general, the point source belt is the strongest line feature. 
+        #         by default, -Hough_PeakClip=0.7 is proper in most cases.
+        #         however, for galaxy dominated fields (e.g., JWST imagines of galaxy cluster),
+        #         the point-source-belt can be not very pronounced, and one may should reduce 
+        #         the parameter from default 0.7 to, says, ~ 0.4.
+        #
+        #   Remarks on the Mask
+        #   It can be essential to apply restrictions on FLUX_RADIUS (R) for the scatter points used in hough transform. 
+        #   (1) Exclude the sources with unusally large R (e.g., R > 20.0) can speed up the calculations.
+        #       One can control the upper limit of R using parameter -Hough_MAXFR
+        #
+        #   (2) The sources with very small R (e.g., R < 0.5) may become districtions for hough detection.
+        #       They are not point sources, likely hot pixels or cosmic rays, sometimes,
+        #       wrong line features will be detected by chance without proper rejections.
+        #
+        #       NOTE: One can control the lower limit of R via parameter -Hough_MINFR,
+        #             the recommended values of Hough_MINFR range from 0.1 to 1.0. One should choose 
+        #             a proper value according to the instrument configuration and typical seeing conditions.
+        #
+        """
+
+        skimage_version = parse_version(skimage.__version__)
+        assert parse_version('0.16.1') <= skimage_version <= parse_version('0.18.3')
         
         A_IMAGE = np.array(AstSEx['A_IMAGE'])
         B_IMAGE = np.array(AstSEx['B_IMAGE'])
         MA_FR = np.array([AstSEx['MAG_AUTO'], AstSEx['FLUX_RADIUS']]).T
+        
         ELLIP = (A_IMAGE - B_IMAGE) / (A_IMAGE + B_IMAGE)
-        MASK_ELLIP = ELLIP < PS_ELLIPThresh
+        if PointSource_MINELLIP is not None:
+            MASK_ELLIP = ELLIP < PointSource_MINELLIP
+        else: MASK_ELLIP = np.ones(len(ELLIP)).astype(bool)
 
-        # * Trigger Hough Dectection 
-        #    Use Hough-Transformation detect the Point-Source-Line from the scatter points in 
-        #    diagram X [MAG_AUTO] - Y [FLUX_RADIUS], which is a nearly-horizon stright line.
-        
-        # ** Remarks on the Mask for Hough Transformation
-        #    It is s useful to make restriction on FLUX_RADIUS (R) of the scatter points for hough detection.
-        #    I. Exclude the sources with unusally large R > 20.0 can speed up the process.
-        #    II. The sources with small R (typically ~ 0.5) are likely hot pixels or cosmic rays.
-        #        The parameter Hough_FRLowerLimit is the lower bound of FLUX_RATIO for Hough transformation.
-        #        Setting a proper lower bound can avoid to detect some line features by chance,
-        #        which are not contributed from point sources but resides in the small-FLUX_RATIO region.
-        #        NOTE: One need to choose a proper Hough_FRLowerLimit according to the fact if the image is 
-        #              under/well/over-sampling (depending on the instrumental configuration and typical seeing conditions)
-        #              recommended values of Hough_FRLowerLimit range from 0.1 to 1.0.
-        #        NOTE: When the point-source-belt is not very pronounced (e.g., in galaxy dominated fields),
-        #              one may consider to reduce the parameter from default 0.7 to, says, ~ 0.4.
-        
         MA, FR = MA_FR[:, 0], MA_FR[:, 1]
         MA_MID = np.nanmedian(MA)
-        Hmask = np.logical_and.reduce((FR > Hough_FRLowerLimit, FR < 10.0, \
-            MA > MA_MID-7.0, MA < MA_MID+7.0))
         
-        Hough_grid_pixsize, Hough_count_thresh = 0.05, 1   # Emperical
-        HDOP = Hough_Detection.HD(XY_obj=MA_FR, Hmask=Hmask, grid_pixsize=Hough_grid_pixsize, \
-            count_thresh=Hough_count_thresh, peak_clip=Hough_peak_clip)
-        ThetaPeaks, RhoPeaks, ScaLineDIST = HDOP[2:]
-        
-        Belt_theta_thresh = 0.2   # Emperical
-        Avmask = np.abs(ThetaPeaks) < Belt_theta_thresh
-        AvIDX = np.where(Avmask)[0]
-
-        if len(AvIDX) == 0: 
-            Horindex = None
-            warnings.warn('MeLOn WARNING: [NO] nearly-horizon peak as Point-Source-Belt!')
-        if len(AvIDX) == 1:
-            Horindex = AvIDX[0]
-            print('MeLOn CheckPoint: [UNIQUE] nearly-horizon peak as Point-Source-Belt!')
-        if len(AvIDX) > 1:
-            Horindex = np.min(AvIDX)
-            warnings.warn('MeLOn WARNING: [MULTIPLE] nearly-horizon peaks, use the [STRONGEST] as Point-Source-Belt!')
-        
-        if Horindex is not None:
-            HorThetaPeak = ThetaPeaks[Horindex]
-            HorRhoPeak = RhoPeaks[Horindex]
-            HorScaLineDIST = ScaLineDIST[:, Horindex]
-
-            _message = 'The Point-Source-Belt detected by Hough Transform '
-            _message += 'is characterized by [%.6f, %.6f]!' %(HorThetaPeak, HorRhoPeak)
-            print('MeLOn CheckPoint: %s' %_message)
+        magnitude_main_range = (-7.0, 7.0)   # emperical
+        Hmask = np.logical_and.reduce((FR > Hough_MINFR, FR < Hough_MAXFR, \
+            MA > MA_MID + magnitude_main_range[0], MA < MA_MID + magnitude_main_range[1]))
+
+        grid_pixsize, count_thresh = 0.05, 1   # emperical
+        _res = Hough_Detection.HD(XY_obj=MA_FR, Hmask=Hmask, grid_pixsize=grid_pixsize, \
+            count_thresh=count_thresh, peak_clip=Hough_PeakClip)
+        ThetaPeaks, RhoPeaks, ScaLineDIST = _res[2:]
+
+        BeltTheta_thresh = 0.2   # emperical
+        NHOR_INDEX = np.where(np.abs(ThetaPeaks) < BeltTheta_thresh)[0]
+        
+        if len(NHOR_INDEX) == 0: 
+            bingo_index = None
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = '[NO] near-horizon peak as Point-Source-Belt!'
+                warnings.warn('MeLOn WARNING: %s' %_warn_message)
+
+        elif len(NHOR_INDEX) == 1:
+            bingo_index = NHOR_INDEX[0]
+            if VERBOSE_LEVEL in [1, 2]:
+                _message = '[UNIQUE] near-horizon peak as Point-Source-Belt!'
+                print('MeLOn CheckPoint: %s' %_message)
+        
+        else:
+            bingo_index = np.min(NHOR_INDEX)
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = '[MULTIPLE] near-horizon peaks, of which [strongest] as Point-Source-Belt!'
+                warnings.warn('MeLOn WARNING: %s' %_warn_message)
+        
+        if bingo_index is not None:
+            # * use hough detection method
+            BeltTheta = ThetaPeaks[bingo_index]
+            BeltRho = RhoPeaks[bingo_index]
+            MASK_FRM = ScaLineDIST[:, bingo_index] < BeltHW
+
+            if VERBOSE_LEVEL in [2]:
+                _message = 'The Point-Source-Belt detected by Hough Transform '
+                _message += 'is characterized by [%f, %f]!' %(BeltTheta, BeltRho)
+                print('MeLOn CheckPoint: %s' %_message)
 
             # *** Note on the FRL region *** 
-            # (1) HorThetaPeak is around 0, then cos(HorThetaPeak) around 1 thus >> 0.
-            # (2) FRL region (above the line) is x_above * sin(HorThetaPeak) + y_above * cos(HorRhoPeak) > rho.
-
-            MASK_FRM = HorScaLineDIST < BeltHW
-            MASK_FRL = MA_FR[:, 0] * np.sin(HorThetaPeak) + MA_FR[:, 1] * np.cos(HorThetaPeak) > HorRhoPeak
-            MASK_FRL = np.logical_and(MASK_FRL, ~MASK_FRM)
+            # geometrically, we know the scatter points above the near-horizon straight line have
+            # x*sin(theta) + y*cos(theta) > rho, where theta is BeltTheta and rho is BeltRho
+            
+            MASK_FRL = MA_FR[:, 0]*np.sin(BeltTheta) + MA_FR[:, 1]*np.cos(BeltTheta) > BeltRho
+            MASK_FRL = np.logical_and(MASK_FRL, ~MASK_FRM)  # exlcude the points in the FR-M region.
 
         else:
-            warnings.warn('MeLOn WARNING: [STANDBY] approach is active to determine the FRM regions!')
-
-            # *** Note on the belt determination when Hough transform fails *** 
-            # (1) It is quite tricky to find a generic way to determine the point source belt when Hough transform fails.
-            #     Typically, the bright sources with moderate Flux Radius are likely point sources.
-            # (2) Our strategy is to calculate a median Flux Radius weighted by the source flux, meanwhile,
-            #     we modulate the weights by applying a penalty on the sources with large Flux Radius.
+            # * use standby method
+            BeltTheta, BeltRho = np.nan, np.nan
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = '[STANDBY] method to determine FR-S/M/L regions!'
+                warnings.warn('MeLOn WARNING: %s' %_warn_message)
+
+            # *** Note on the standby belt determination *** 
+            # it is quite tricky to find a generic way to determine the point source belt when 
+            # hough detection does not work. we noticed that the bright sources with moderate 
+            # Flux Radius are more likely point sources. a standby strategy is to calculate 
+            # a median Flux Radius weighted by the source flux, and meanwhile, we modulate 
+            # the weights by applying a penalty on the sources with large Flux Radius.
 
             NTE_4FRM = 30  # NUM_TOP_END for FRM, default value used herein.
             _values, _weights = MA_FR[:, 1], np.array(AstSEx['FLUX_AUTO'])
             _weights /= np.clip(_values, a_min=0.5, a_max=None)**2  
-            FRM = TopFlatten_Weighted_Quantile.TFWQ(values=_values, weights=_weights, \
-                quantiles=[0.5], NUM_TOP_END=NTE_4FRM)[0]
             
-            MASK_FRM = np.abs(MA_FR[:, 1]  - FRM) < BeltHW
-            MASK_FRL = MA_FR[:, 1]  - FRM > BeltHW
-        
+            FR_MID = TopFlatten_Weighted_Quantile.TFWQ(values=_values, \
+                weights=_weights, quantiles=[0.5], NUM_TOP_END=NTE_4FRM)[0]
+            
+            MASK_FRM = np.abs(MA_FR[:, 1]  - FR_MID) < BeltHW
+            MASK_FRL = MA_FR[:, 1]  - FR_MID > BeltHW
+
         MASK_FRS = ~np.logical_or(MASK_FRM, MASK_FRL)
         LABEL_FR = np.array(['FR-S'] * len(AstSEx))
         LABEL_FR[MASK_FRM] = 'FR-M'
         LABEL_FR[MASK_FRL] = 'FR-L'
 
-        _message = 'Label Counts [FR-S (%s) / FR-M (%s) / FR-L (%s)]!' \
-            %(np.sum(MASK_FRS), np.sum(MASK_FRM), np.sum(MASK_FRL))
-        print('MeLOn CheckPoint: HoughMorphClassifier --- %s' %_message)
+        if VERBOSE_LEVEL in [2]:
+            _message = 'HoughMorphClassifier FR-S/M/L counts are '
+            _message += '[%d / %d / %d]' %(np.sum(MASK_FRS), np.sum(MASK_FRM), np.sum(MASK_FRL))
+            print('MeLOn CheckPoint: %s' %_message)
 
-        # * Produce the 3 hierarchic groups
-        # ** Good Sources
+        # * determine Good Sources
         MASK_GS = ~MASK_FRS
 
-        # *** Point Sources 
+        # * determine Point Sources
         MASK_PS = np.logical_and(MASK_FRM, MASK_ELLIP)
-        print('MeLOn CheckPoint: [%d] Good-Sources on the Image!' %np.sum(MASK_GS))
-        print('MeLOn CheckPoint: [%d] Point-Sources on the Image!' %np.sum(MASK_PS))
-        
+        if VERBOSE_LEVEL in [1, 2]:
+            print('MeLOn CheckPoint: [%d] Good-Sources on the Image!' %np.sum(MASK_GS))
+            print('MeLOn CheckPoint: [%d] Point-Sources on the Image!' %np.sum(MASK_PS))
+
+        # * estimate FWHM
         NTE_4FWHM = 30  # NUM_TOP_END for FWHM, default value used herein.
         _values, _weights = np.array(AstSEx[MASK_PS]['FWHM_IMAGE']), np.array(AstSEx[MASK_PS]['FLUX_AUTO'])
-        FWHM = round(TopFlatten_Weighted_Quantile.TFWQ(values=_values, weights=_weights, \
-            quantiles=[0.5], NUM_TOP_END=NTE_4FWHM)[0], 6)
-        print('MeLOn CheckPoint: Estimated [FWHM = %.3f pix] From Point-Sources' %FWHM)
+        FWHM = TopFlatten_Weighted_Quantile.TFWQ(values=_values, weights=_weights, \
+            quantiles=[0.5], NUM_TOP_END=NTE_4FWHM)[0]
+        
+        FWHM = round(FWHM, 6)
+        if VERBOSE_LEVEL in [1, 2]:
+            print('MeLOn CheckPoint: Estimated [FWHM = %.3f pix] from Point-Sources' %FWHM)
 
-        return FWHM, LABEL_FR, MASK_GS, MASK_PS
+        return BeltTheta, BeltRho, LABEL_FR, MASK_GS, MASK_PS, FWHM
```

### Comparing `sfft-1.3.4/sfft/utils/NeighboringPixelCovariance.py` & `sfft-1.4.0/sfft/utils/NeighboringPixelCovariance.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 import numpy as np
+# version: Feb 5, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.0"
-
-# MeLOn Notes
-# @ Calculate Covariance of Neighboring Pixels
-# Consider 2 random variables
-# a: pixel value at coordinate (r, c)
-# b: pixel value at coordinate (r+1, c+1)
-# For given astronomical image, it is possible to do sampling from the joint probability distribution of a & b.
-# Each sample is a pair of pixels cross through the image, note we should pick such pairs on background 
-# if we only concern the Covariance of neighboring background pixels.
-# * One of the most efficient ways to get massive samples is rolling the image.
-#    Samples of (a, b): {image.flatten(), np.roll(image, 1, 1).flatten()}
-#    NOTE we denote a as (0, 0) and b (1, 1), here we concerns 25 random variables {(0, 0), (1, 0), (-1, 0) ...}
-#    NOTE image has physical boundary thus some samples above should be rejected.
-#               For a random variable denoted as (p, q)
-#               tmp = np.roll(image, p, q)
-#               tmp[:p, :] (p > 0) & tmp[p:, :] (p < 0)  are invalid 
-#               tmp[:, :q] (q > 0) & tmp[:, q:] (q < 0)  are invalid
+__version__ = "v1.4"
 
 class NeighboringPixel_Covariance:
     @staticmethod
     def NPC(PixA_obj):
-
+        
+        """
+        # MeLOn Notes
+        # @ Convariance Calculator of Neighboring Pixels
+        # (I) Consider two random vairbales: a is the pixel value at coordinate (r, c) and 
+        #     b is the pixel value at coordinate (r+1, c+1). 
+        #
+        # (II) For a given astronomical image, exhuasting all possible r, c would produce a large 
+        #      set of pairs (a, b), as sampled from the joint probability distribution of a & b.
+        #      NOTE: In general, we concern the background covariance so only background pixels used.
+        #       
+        # (III) Rolling the image can easily produce the large sample set.
+        #       Samples of (a, b): {image.flatten(), np.roll(image, 1, 1).flatten()}
+        #       NOTE: we can replace (+1, +1) with other neighboring position (p, q) 
+        #             here we concern 25 relative positions {(0, 0), (+1, 0), (-1, 0) ...}
+        #       NOTE: please reject the rolling samples out of image boundary.
+        #             tmp = np.roll(image, p, q)
+        #             tmp[:p, :] (p > 0) & tmp[p:, :] (p < 0)  are invalid 
+        #             tmp[:, :q] (q > 0) & tmp[:, q:] (q < 0)  are invalid
+        #
+        """
+        
         RVs = ([0, 0], \
-                    [1, 0], [-1, 0], [0, 1], [0, -1], \
-                    [1, 1], [1, -1], [-1, 1], [-1, -1], \
-                    [2, 0], [-2, 0], [0, 2], [0, -2], \
-                    [3, 0], [-3, 0], [0, 3], [0, -3], \
-                    [4, 0], [-4, 0], [0, 4], [0, -4], \
-                    [5, 0], [-5, 0], [0, 5], [0, -5])
+               [1, 0], [-1, 0], [0, 1], [0, -1], \
+               [1, 1], [1, -1], [-1, 1], [-1, -1], \
+               [2, 0], [-2, 0], [0, 2], [0, -2], \
+               [3, 0], [-3, 0], [0, 3], [0, -3], \
+               [4, 0], [-4, 0], [0, 4], [0, -4], \
+               [5, 0], [-5, 0], [0, 5], [0, -5])
 
         im = PixA_obj / PixA_obj.std()
         shiftedim_lst, rejmask_lst = [], []
         for rv in RVs:
             p, q = rv
             shiftedim = np.roll(np.roll(im, p, axis=0), q, axis=1)
             rejmask = np.zeros(im.shape).astype(bool)
@@ -42,18 +47,16 @@
             if p < 0: rejmask[p:, :] = True
             if q > 0: rejmask[:, :q] = True
             if q < 0: rejmask[:, q:] = True
             shiftedim_lst.append(shiftedim)
             rejmask_lst.append(rejmask)
         
         RMask = np.logical_or.reduce(tuple(rejmask_lst))
-        SampleSet = np.array([shiftedim[~RMask].flatten() for shiftedim in shiftedim_lst])  # Shape (Ndim, Nsamp)
-        #print('MeLOn CheckPoint: SampleSet has shape (Ndim, Nsamp) = (%d, %d)' \
-        #    %(SampleSet.shape[0], SampleSet.shape[1]))
+        SampleSet = np.array([shiftedim[~RMask].flatten() for shiftedim in shiftedim_lst])  # (Ndim, Nsamp)
+        CovMatrix = np.cov(SampleSet, bias=True)
 
-        CovMatrix = np.cov(SampleSet, bias=True)   #TODO: Why do we use bias ?
         tmp_ = CovMatrix.copy()
         np.fill_diagonal(tmp_, np.NaN)
         tmp_ = np.abs(tmp_)
         CovLevel = (np.nansum(tmp_) / np.sum(np.diag(CovMatrix)))
+        
         return CovMatrix, CovLevel
-
```

### Comparing `sfft-1.3.4/sfft/utils/SExSkySubtract.py` & `sfft-1.4.0/sfft/utils/SExSkySubtract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import sep
+import warnings
 import numpy as np
 from astropy.io import fits
 from scipy.stats import iqr
 from sfft.utils.pyAstroMatic.PYSEx import PY_SEx
-# version: Sep 28, 2022
+# version: Feb 4, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class SEx_SkySubtract:
     @staticmethod
     def SSS(FITS_obj, FITS_skysub=None, FITS_sky=None, FITS_skyrms=None, SATUR_KEY='SATURATE', ESATUR_KEY='ESATUR', \
-        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=1.5, DETECT_MINAREA=5, DETECT_MAXAREA=0):
+        BACK_SIZE=64, BACK_FILTERSIZE=3, DETECT_THRESH=1.5, DETECT_MINAREA=5, DETECT_MAXAREA=0, VERBOSE_LEVEL=2):
 
         """
         # Inputs & Outputs:
 
         -FITS_obj []                    # FITS file path of the input image 
  
         -FITS_skysub [None]             # FITS file path of the output sky-subtracted image
@@ -25,66 +26,73 @@
         -FITS_skyrms [None]             # FITS file path of the output sky RMS image
 
         -ESATUR_KEY ['ESATUR']          # Keyword for the effective saturation level of sky-subtracted image
                                         # P.S. the value will be saved in the primary header of -FITS_skysub
 
         # Configurations for SExtractor:
         
-        -SATUR_KEY ['SATURATE']        # SExtractor Parameter SATUR_KEY
-                                       # i.e., keyword of the saturation level in the input image header
+        -SATUR_KEY ['SATURATE']         # SExtractor Parameter SATUR_KEY
+                                        # i.e., keyword of the saturation level in the input image header
 
-        -BACK_SIZE [64]                # SExtractor Parameter BACK_SIZE
+        -BACK_SIZE [64]                 # SExtractor Parameter BACK_SIZE
 
-        -BACK_FILTERSIZE [3]           # SExtractor Parameter BACK_FILTERSIZE
+        -BACK_FILTERSIZE [3]            # SExtractor Parameter BACK_FILTERSIZE
 
-        -DETECT_THRESH [1.5]           # SExtractor Parameter DETECT_THRESH
+        -DETECT_THRESH [1.5]            # SExtractor Parameter DETECT_THRESH
 
-        -DETECT_MINAREA [5]            # SExtractor Parameter DETECT_MINAREA
+        -DETECT_MINAREA [5]             # SExtractor Parameter DETECT_MINAREA
         
-        -DETECT_MAXAREA [0]            # SExtractor Parameter DETECT_MAXAREA
+        -DETECT_MAXAREA [0]             # SExtractor Parameter DETECT_MAXAREA
+
+        # Miscellaneous
+        
+        -VERBOSE_LEVEL [2]              # The level of verbosity, can be [0, 1, 2]
+                                        # 0/1/2: QUIET/NORMAL/FULL mode
 
         # Returns:
 
-            SKYDIP                     # The flux peak of the sky image (outliers rejected)
+            SKYDIP                      # The flux peak of the sky image (outliers rejected)
 
-            SKYPEAK                    # The flux dip of the sky image (outliers rejected)
+            SKYPEAK                     # The flux dip of the sky image (outliers rejected)
             
-            PixA_skysub                # Pixel Array of the sky-subtracted image 
+            PixA_skysub                 # Pixel Array of the sky-subtracted image 
             
-            PixA_sky                   # Pixel Array of the sky image 
+            PixA_sky                    # Pixel Array of the sky image 
             
-            PixA_skyrms                # Pixel Array of the sky RMS image 
+            PixA_skyrms                 # Pixel Array of the sky RMS image 
 
         """
 
         # * Generate SExtractor OBJECT-MASK
-        #   NOTE: GAIN, DEBLEND_MINCONT, BACKPHOTO_TYPE do not matter in the determination of detection mask.
-        DETECT_MASK = PY_SEx.PS(FITS_obj=FITS_obj, PL=['X_IMAGE', 'Y_IMAGE'], GAIN_KEY='GAIN', SATUR_KEY=SATUR_KEY, \
-            BACK_TYPE='AUTO', BACK_SIZE=BACK_SIZE, BACK_FILTERSIZE=BACK_FILTERSIZE, DETECT_THRESH=DETECT_THRESH, \
-            DETECT_MINAREA=DETECT_MINAREA, DETECT_MAXAREA=DETECT_MAXAREA, DEBLEND_MINCONT=0.005, \
-            BACKPHOTO_TYPE='GLOBAL', CHECKIMAGE_TYPE='OBJECTS')[1][0].astype(bool)
-
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            # NOTE: GAIN, SATURATE, ANALYSIS_THRESH, DEBLEND_MINCONT, BACKPHOTO_TYPE do not affect the detection mask.
+            DETECT_MASK = PY_SEx.PS(FITS_obj=FITS_obj, SExParam=['X_IMAGE', 'Y_IMAGE'], GAIN_KEY='PHGAIN', SATUR_KEY=SATUR_KEY, \
+                BACK_TYPE='AUTO', BACK_SIZE=BACK_SIZE, BACK_FILTERSIZE=BACK_FILTERSIZE, DETECT_THRESH=DETECT_THRESH, \
+                ANALYSIS_THRESH=1.5, DETECT_MINAREA=DETECT_MINAREA, DETECT_MAXAREA=DETECT_MAXAREA, DEBLEND_MINCONT=0.005, \
+                BACKPHOTO_TYPE='GLOBAL', CHECKIMAGE_TYPE='OBJECTS', MDIR=None, VERBOSE_LEVEL=VERBOSE_LEVEL)[1][0].astype(bool)
+        
         # * Extract SExtractor SKY-MAP from the Unmasked Image
         PixA_obj = fits.getdata(FITS_obj, ext=0).T
         _PixA = PixA_obj.astype(np.float64, copy=True)    # default copy=True, just to emphasize
         _PixA[DETECT_MASK] = np.nan
         if not _PixA.flags['C_CONTIGUOUS']: _PixA = np.ascontiguousarray(_PixA)
 
         # NOTE: here we use faster sep package instead of SExtractor.
         sepbkg = sep.Background(_PixA, bw=BACK_SIZE, bh=BACK_SIZE, fw=BACK_FILTERSIZE, fh=BACK_FILTERSIZE)
         PixA_sky, PixA_skyrms = sepbkg.back(), sepbkg.rms()
         PixA_skysub = PixA_obj - PixA_sky
 
         # * Make simple statistics for the SKY-MAP
         Q1 = np.percentile(PixA_sky, 25)
-        Q3 = np.percentile(PixA_sky, 55)
+        Q3 = np.percentile(PixA_sky, 75)
         IQR = iqr(PixA_sky)
         SKYDIP = Q1 - 1.5*IQR    # outlier rejected dip
         SKYPEAK = Q3 + 1.5*IQR   # outlier rejected peak
-
+        
         if FITS_skysub is not None:
             with fits.open(FITS_obj) as hdl:
                 hdl[0].header['SKYDIP'] = (SKYDIP, 'MeLOn: IQR-MINIMUM of SEx-SKY-MAP')
                 hdl[0].header['SKYPEAK'] = (SKYPEAK, 'MeLOn: IQR-MAXIMUM of SEx-SKY-MAP')
                 ESATUR = float(hdl[0].header[SATUR_KEY]) - SKYPEAK    # use a conservative value
                 hdl[0].header[ESATUR_KEY] = (ESATUR, 'MeLOn: Effective SATURATE after SEx-SKY-SUB')
                 hdl[0].data[:, :] = PixA_skysub.T
```

### Comparing `sfft-1.3.4/sfft/utils/SkyLevelEstimator.py` & `sfft-1.4.0/sfft/utils/SkyLevelEstimator.py`

 * *Files identical despite different names*

### Comparing `sfft-1.3.4/sfft/utils/StampGenerator.py` & `sfft-1.4.0/sfft/utils/StampGenerator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+import sys
 import numpy as np
 import os.path as pa
 from astropy.io import fits
-from astropy.wcs import WCS
-from tempfile import mkdtemp
 from astropy.nddata.utils import Cutout2D
-# version: Sep 18, 2022
+from sfft.utils.ReadWCS import Read_WCS
+# version: Feb 6, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class Stamp_Generator:
     @staticmethod
-    def SG(FITS_obj=None, StampImgSize=None, Coordinates=None, \
-        CoorType='Image', AutoFill='NaN', MDIR=None):
+    def SG(FITS_obj=None, EXTINDEX=0, EXTNAME=None, COORD=None, COORD_TYPE='IMAGE', \
+        STAMP_IMGSIZE=None, FILL_VALUE=np.nan, FITS_StpLst=None, VERBOSE_LEVEL=2):
 
         """
         # MeLOn Notes
-        # @Stamp Generator
-        # * Remarks on the 2 basic Coordinate System
+        # @ Stamp Generator
+        # * Remarks on the 2 basic coordinate systems
         #   A. Fortran & FITS ( ds9 & SEx & WCS ) version
         #      @ Matrix Index start from 1. Thus the first pixel of a matrix is < r_F, c_F > = < 1, 1 >
         #      @ [Basic Consistence Rule in Fortran]
         #        Corresponding xy-Coordinate System: Pixel < r_F, c_F > has Center with xy-coordinate ( x_F, y_F ) = ( r_F, c_F )
         #        NOTE the origin point this system is located at the center point of the pixel < r_F, c_F > = < 0, 0 >, 
         #             which is not physical existed.
         #      @ [Basic inclusion Rule in Fortran]
@@ -34,20 +34,19 @@
         #        Corresponding xy-Coordinate System: Pixel < r_C, c_C > has Center with xy-coordinate ( x_C, y_C ) = ( r_C, c_C )
         #        NOTE the origin point this system is located at the center point of the pixel < r_C, c_C > = < 0, 0 >, 
         #             which is just the first pixel.
         #      @ [Basic inclusion Rule in C]
         #        Given Coordinate is enclosed in which pixel ?
         #        Hold Pixel < r_C, c_C > = < int(x_C + 0.5), int(y_C + 0.5) >
         #        (Hold Pixel has solid boundary at bottom and left side, and dashed boundary at upper and right side.)
-        #     
-        # NOTE < r_F, c_F > = < r_C + 1, c_C + 1 >
-        # NOTE < x_F, y_F > = < x_C + 1, y_C + 1 >
+        #   
+        #   P.S. < r_F, c_F > = < r_C + 1, c_C + 1 > and < x_F, y_F > = < x_C + 1, y_C + 1 >
         #
-        # * Our Convention
-        #   We generally use C Matrix Index System with Fortran Coordinate System !
+        # * Our MeLOn Convention
+        #   In our context, we always use C Matrix Index System with Fortran Coordinate System!
         #   henceforth, Let r, c means r_C, c_C and x, y indicate x_F, y_F.
         #
         #   @ [Basic Consistence Rule in Our Convention]
         #     Pixel < r, c > has Center with xy-coordinate (x, y) = (r + 1.0, c + 1.0)      
         #   @ [Basic Inclusion Rule in Our Convention]
         #     Hold Pixel < r, c > = < int(x - 0.5), int(y - 0.5) >
         #   @ Image Center has xy-coordinate (x, y) = (NX/2 + 0.5, NY/2 + 0.5)
@@ -55,97 +54,140 @@
         #     Without boundary: 0 <= r, c < NX, NY
         #                       0.5 <= x, y < NX + 0.5, NY + 0.5 
         #     With boundary: NBX, NBY <= r, c < NX - NBX, NY - NBY  
         #                    NBX + 0.5, NBY + 0.5 <= x, y < NX - NBX + 0.5, NY - NBY + 0.5
         #
         # * The convertion function in Astropy
         #   Both w.all_pix2world and w.all_world2pix has an argument called origin 
-        #   origin = 1, Fortran xy-coordinate   |   This is what we generally use !
+        #   origin = 1, Fortran xy-coordinate   |   This is what we always use!
         #   origin = 0, C xy-coordinate
         #
         # * Stamp-Procedure for digital image
         #   Given (x, y) ----- Enclosed in Pixel < r, c > = < ⌊x - 0.5⌋,  ⌊y - 0.5⌋ >
         #   Stamp(PixA, x, y, P, Q) = PixA[r - ⌊P/2⌋: r + ⌈P/2⌉, c - ⌊Q/2⌋: c + ⌈Q/2⌉]
         #
         # * Equivalent Stamp-Procedure for given row & column range
         #   Given RowRange = (r0, r1) and ColRange = (c0, c1)
-        #   Let  P = r1 - r0 and Q = c1 - c0, then 
+        #   Let P = r1 - r0 and Q = c1 - c0, then 
         #   PixA[r0: r1, c0: c1] = Stamp(PixA, x, y, P, Q) 
         #   where x = r0 + ⌊P/2⌋ + 1.0 and y = c0 + ⌊Q/2⌋ + 1.0
         #
         # * Might be right, but haven't been Checked yet.
         #   PixA[E: -E, F: -F] = Stamp(PixA, U/2, V/2, U-2*E, V-2*F), where U, V = PixA.shape
         #   Stamp(PixA, x, y, P, Q)[E: -E, F: -F] = Stamp(PixA, x, y, P-E, Q-F)
         #
         # * Additional Remarks 
         #   a. Only Support Single-Extension FITS file currently.
         #   b. The Boundary Pixels could be filled with np.nan | median vaule | given value 
-        #   c. Here we just care the essential cases with CoorType='Image' since other 'World' cases could be transformed.
-        #   d. Cutout2D size parameter has the form of (ny, nx), However the required stamp with StampImgSize has a form of (NSX, NSY)
-        #      We require the input of Cutout2D should only be < r, c >, even this function actually support float values as input.
+        #   c. Here we just care the essential cases with COORD_TYPE='IMAGE' since other 'WORLD' cases could be transformed.
+        #   d. Cutout2D size parameter has the form of (ny, nx), however, the required stamp with STAMP_IMGSIZE 
+        #      has a form of (NSX, NSY). We require the input of Cutout2D should only be < r, c >, even this 
+        #      function actually also support float values as inputs.
         #   e. We should note NAXIS in the header would be automatic updated to adjust the image size.
         #   f. For general purpose, We do use the astropy generated wcs for the stamps.
         #      Alternatively, a more naive method is employed with correction of CRPIX1 & CRPIX2
         #      which is reasonable at least for TPV and SIP transformation, where the equations 
         #      are only dependent on the relative pixel coordinate, that it, the pixel-vector.   
         #      Ref https://fits.gsfc.nasa.gov/registry/tpvwcs/tpv.html  
         #      Ref https://fits.gsfc.nasa.gov/registry/sip/SIP_distortion_v1_0.pdf
-
+        #
         """
 
-        NSX, NSY = StampImgSize
-        NCoors = Coordinates.shape[0]
-        hdl = fits.open(FITS_obj)
-        hdr = hdl[0].header
-        data = hdl[0].data
-
-        # * Covert Coordinates to Image-Type 
-        positions = (Coordinates - 0.5).astype(int)
-        if CoorType == 'World':
-            w_obj = WCS(hdr, hdl)
-            positions = (w_obj.all_world2pix(Coordinates, 1) - 0.5).astype(int)
-        hdl.close()
-
-        # * Determin the auto fill value for boundary case
-        fill_value = AutoFill
-        if AutoFill == 'MEDIAN':
-            fill_value = np.nanmedian(data)
-        if AutoFill == 'NaN':
-            fill_value = -65536    # FIXME In most cases, It works
+        NSX, NSY = STAMP_IMGSIZE
+        assert len(COORD.shape) == 2 and COORD.shape[1] == 2
+        NPOS = COORD.shape[0]
+        
+        if EXTNAME is not None:
+            hdr_obj = fits.getheader(FITS_obj, extname=EXTNAME)
+            data_obj = fits.getdata(FITS_obj, extname=EXTNAME)
+        else: 
+            hdr_obj = fits.getheader(FITS_obj, ext=EXTINDEX)
+            data_obj = fits.getdata(FITS_obj, ext=EXTINDEX)
+        dtype_obj = data_obj.dtype
+        
+        # * read positions
+        if np.issubdtype(COORD.dtype, np.floating):
+            UCOORD = COORD
+        elif np.issubdtype(COORD.dtype, np.integer):
+            UCOORD = COORD.astype(float)
+            if VERBOSE_LEVEL in [2]:
+                _warn_message = 'COORD has integer data type, covert to float automatically!'
+                print('MeLOn WARNING: %s' %_warn_message)
+        else: 
+            _error_message = 'WRONG data type for COORD!'
+            sys.exit('MeLOn ERROR: %s' %_error_message)
+        
+        assert COORD_TYPE in ['IMAGE', 'WORLD']
+        if COORD_TYPE == 'IMAGE':
+            positions = (UCOORD - 0.5).astype(int)
+        if COORD_TYPE == 'WORLD':
+            w_obj = Read_WCS.RW(hdr_obj, VERBOSE_LEVEL=VERBOSE_LEVEL)
+            positions = (w_obj.all_world2pix(UCOORD, 1) - 0.5).astype(int)
+
+        # * read fill_value, as same type with data
+        if type(FILL_VALUE) == float:
+            fv = FILL_VALUE
+            if np.issubdtype(dtype_obj, np.integer):
+                fv = np.array([fv], dtype=dtype_obj)[0]
+                if VERBOSE_LEVEL in [1, 2]:
+                    _warn_message = 'float FILL_VALUE is coverted to integer automatically!'
+                    print('MeLOn WARNING: %s' %_warn_message)
+        
+        elif type(FILL_VALUE) == int:
+            fv = FILL_VALUE
+            if np.issubdtype(dtype_obj, np.floating):
+                fv = np.array([fv], dtype=dtype_obj)[0]
+                if VERBOSE_LEVEL in [2]:
+                    _warn_message = 'integer FILL_VALUE is coverted to float automatically!'
+                    print('MeLOn WARNING: %s' %_warn_message)
         
-        # * Make stamps with function Cutout2D
-        #   FIXME collection of stamp arrays can be memory-consuming 
+        elif FILL_VALUE in ['MEDIAN', 'MEAN']:
+            if FILL_VALUE == 'MEDIAN': fv = np.nanmedian(data_obj)
+            if FILL_VALUE == 'MEAN': fv = np.nanmean(data_obj)
+
+            if np.issubdtype(dtype_obj, np.integer) and type(fv) == float:
+                fv = np.array([fv], dtype=dtype_obj)[0]
+                if VERBOSE_LEVEL in [1, 2]:
+                    _warn_message = 'float FILL_VALUE is coverted to integer automatically!'
+                    print('MeLOn WARNING: %s' %_warn_message)
+            
+            if np.issubdtype(dtype_obj, np.floating) and type(fv) == int:
+                fv = np.array([fv], dtype=dtype_obj)[0]
+                if VERBOSE_LEVEL in [2]:
+                    _warn_message = 'integer FILL_VALUE is coverted to float automatically!'
+                    print('MeLOn WARNING: %s' %_warn_message)
+
+        else:
+            _error_message = 'FILL_VALUE is not recognized!'
+            sys.exit('MeLOn ERROR: %s' %_error_message)
+        
+        # * create stamps with astropy function Cutout2D
         PixA_StpLst = []
-        Rsize = (NSY, NSX)
-        for i in range(NCoors):
-            try: PixA_Stp = Cutout2D(data, positions[i], Rsize, mode='partial', fill_value=fill_value).data.T.astype(float)
-            except: PixA_Stp = fill_value * np.ones((StampImgSize[0], StampImgSize[1])).astype(float)
-            if AutoFill == 'NaN': PixA_Stp[PixA_Stp == -65536] = np.nan
+        for i in range(NPOS):
+            try:
+                PixA_Stp = Cutout2D(data_obj, position=positions[i], size=(NSY, NSX), \
+                    mode='partial', fill_value=fv).data.T
+            except: PixA_Stp = fv * np.array(np.ones(STAMP_IMGSIZE), dtype=dtype_obj)
             PixA_StpLst.append(PixA_Stp)
-        
-        # * Make header for the stamps with modification of CRPIX1 CRPIX2 offset then save them
-        #    NOTE I have checked the correctness of this operation.
-        FITS_StpLst = []
-        if MDIR is not None:
+
+        # * save stamps to FITS files with WCS updated
+        if FITS_StpLst is not None:
+            hdr_StpLst = [] 
             FNAME = pa.basename(FITS_obj)
-            TDIR = mkdtemp(suffix=None, prefix='SG_', dir=MDIR)
-            hdr_StpLst = []
-            for i in range(NCoors):
-                hdr_Stp = hdr.copy()
-                row_stpcent, col_stpcent = positions[i]
-                row_stpo, col_stpo = row_stpcent - int(NSX/2), col_stpcent - int(NSY/2)
-                try: 
-                    hdr_Stp['CRPIX1'] = float(hdr_Stp['CRPIX1']) - row_stpo
-                    hdr_Stp['CRPIX2'] = float(hdr_Stp['CRPIX2']) - col_stpo
+            for i in range(NPOS):
+                hdr_Stp = hdr_obj.copy()
+                row_StpCent, col_StpCent = positions[i]
+                row_StpO, col_StpO = row_StpCent - int(NSX/2), col_StpCent - int(NSY/2)
+                try:
+                    hdr_Stp['CRPIX1'] = float(hdr_Stp['CRPIX1']) - row_StpO
+                    hdr_Stp['CRPIX2'] = float(hdr_Stp['CRPIX2']) - col_StpO
                 except: pass
-                hdr_Stp['COMMENT'] = 'Make Stamp from %s ' %FNAME + \
-                                     'with row_stpcent %d col_stpcent %d ' %(row_stpcent, col_stpcent) + \
-                                     'with stamp image size %d %d' %(NSX, NSY)
+                hdr_Stp['COMMENT'] = 'Stamp created from %s ' %FNAME + \
+                    'centred at row-colum [%d, %d] ' %(row_StpCent, col_StpCent) + \
+                    'with stamp image size (%d %d)' %(NSX, NSY)
                 hdr_StpLst.append(hdr_Stp)
             
-            for i in range(NCoors):
+            for i in range(NPOS):
                 PixA_Stp, hdr_Stp = PixA_StpLst[i], hdr_StpLst[i]
-                FITS_Stp = pa.join(TDIR, '%s.Stp%d.fits' %(FNAME[:-5], i))
-                fits.HDUList([fits.PrimaryHDU(PixA_Stp.T, header=hdr_Stp)]). writeto(FITS_Stp, overwrite=True)
-                FITS_StpLst.append(FITS_Stp)
-        
-        return PixA_StpLst, FITS_StpLst
+                fits.HDUList([fits.PrimaryHDU(PixA_Stp.T, header=hdr_Stp)]).writeto(FITS_StpLst[i], overwrite=True)
+
+        return PixA_StpLst
```

### Comparing `sfft-1.3.4/sfft/utils/SymmetricMatch.py` & `sfft-1.4.0/sfft/utils/SymmetricMatch.py`

 * *Files identical despite different names*

### Comparing `sfft-1.3.4/sfft/utils/WeightedQuantile.py` & `sfft-1.4.0/sfft/utils/WeightedQuantile.py`

 * *Files identical despite different names*

### Comparing `sfft-1.3.4/sfft/utils/__init__.py` & `sfft-1.4.0/sfft/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 Remarks on Internal Packages Imports:
     from sfft.utils.HoughDetection import Hough_Detection
     from sfft.utils.WeightedQuantile import TopFlatten_Weighted_Quantile
     from sfft.utils.pyAstroMatic.PYSEx import PY_SEx
 
 """
 
+from .ReadWCS import Read_WCS
 from .CombineHeader import Combine_Header
 from .SymmetricMatch import Symmetric_Match
 from .StampGenerator import Stamp_Generator
 from .SExSkySubtract import SEx_SkySubtract
 from .HoughDetection import Hough_Detection
 from .SkyLevelEstimator import SkyLevel_Estimator
 from .HoughMorphClassifier import Hough_MorphClassifier
 from .ConvKernelConvertion import ConvKernel_Convertion
 from .DeCorrelationCalculator import DeCorrelation_Calculator
 from .NeighboringPixelCovariance import NeighboringPixel_Covariance
 from .WeightedQuantile import Weighted_Quantile, TopFlatten_Weighted_Quantile
-from .SFFTSolutionReader import ReadSFFTSolution, SVKDict_ST2SFFT, SVKDict_SFFT2ST, RealizeSFFTSolution
+from .SFFTSolutionReader import Read_SFFTSolution, SVKDict_ST2SFFT, SVKDict_SFFT2ST, Realize_MatchingKernel, Realize_FluxScaling
```

### Comparing `sfft-1.3.4/sfft/utils/meta/MultiProc.py` & `sfft-1.4.0/sfft/utils/meta/MultiProc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 import threading
 import multiprocessing
+# version: Feb 6, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.0"
+__version__ = "v1.4"
 
 class Multi_Proc:
     @staticmethod
     def MP(taskid_lst=None, func=None, nproc=8, mode='mp'):
         
         if mode == 'mp':
             # Ref: https://gist.github.com/tappoz/cb88f7a9d9ba27cfee1e2f03537fac16
@@ -20,15 +21,15 @@
             
             out_q = multiprocessing.Queue()
             chunksize = int(math.ceil(len(taskid_lst) / float(nproc)))
             
             procs = []
             for i in range(nproc):
                 p = multiprocessing.Process(target=worker, \
-                    args=(taskid_lst[chunksize*i: chunksize*(i+1)], out_q))
+                    args=(taskid_lst[chunksize * i:chunksize * (i + 1)], out_q)) 
                 procs.append(p)
                 p.start()
 
             resultdict = {}
             for i in range(nproc):
                 resultdict.update(out_q.get())
 
@@ -42,17 +43,16 @@
             def trigger(klst):
                 for k in klst: func(k)
                 return None
 
             myThread_Queue = []
             chunksize = int(math.ceil(len(taskid_lst) / float(nproc)))
             for i in range(nproc):
-                taskid_asslst = taskid_lst[chunksize*i: chunksize*(i+1)]
+                taskid_asslst = taskid_lst[chunksize * i:chunksize * (i + 1)]
                 myThread = threading.Thread(target=trigger, args=(taskid_asslst,))
                 myThread_Queue.append(myThread)
                 myThread.start()
             
             for t in myThread_Queue:
                 t.join()
             
             return None
-
```

### Comparing `sfft-1.3.4/sfft/utils/meta/TimeoutKit.py` & `sfft-1.4.0/sfft/utils/meta/TimeoutKit.py`

 * *Files identical despite different names*

### Comparing `sfft-1.3.4/sfft/utils/pyAstroMatic/PYSEx.py` & `sfft-1.4.0/sfft/utils/pyAstroMatic/PYSEx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 import re
 import os
-import sys
 import warnings
 import subprocess
 import numpy as np
 import os.path as pa
 from astropy.io import fits
-from astropy.wcs import WCS
 from tempfile import mkdtemp
 from astropy.table import Table, Column
+from sfft.utils.ReadWCS import Read_WCS
 from sfft.utils.StampGenerator import Stamp_Generator
-from sfft.utils.SymmetricMatch import Symmetric_Match, Sky_Symmetric_Match
 from sfft.utils.pyAstroMatic.AMConfigMaker import AMConfig_Maker
-# version: Sep 28, 2022
+from sfft.utils.SymmetricMatch import Symmetric_Match, Sky_Symmetric_Match
+# version: Mar 12, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class PY_SEx:
     @staticmethod
-    def PS(FITS_obj, PSF_obj=None, FITS_ref=None, PL=None, CATALOG_TYPE='FITS_LDAC', \
+    def PS(FITS_obj, PSF_obj=None, FITS_ref=None, SExParam=None, CATALOG_TYPE='FITS_LDAC', \
         GAIN_KEY='GAIN', SATUR_KEY='SATURATE', PIXEL_SCALE=1.0, SEEING_FWHM=1.2, BACK_TYPE='AUTO', \
-        BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, USE_FILT=True, DETECT_THRESH=1.5, \
+        BACK_VALUE=0.0, BACK_SIZE=64, BACK_FILTERSIZE=3, USE_FILT=True, DETECT_THRESH=1.5, ANALYSIS_THRESH=1.5, \
         DETECT_MINAREA=5, DETECT_MAXAREA=0, DEBLEND_NTHRESH=32, DEBLEND_MINCONT=0.005, CLEAN='Y', \
         BACKPHOTO_TYPE='LOCAL', PHOT_APERTURES=5.0, NegativeCorr=True, CHECKIMAGE_TYPE='NONE', \
-        VIGNET=None, StampImgSize=None, AddRD=False, ONLY_FLAGS=None, XBoundary=0.0, YBoundary=0.0, \
+        VIGNET=None, STAMP_IMGSIZE=None, AddRD=False, ONLY_FLAGS=None, XBoundary=0.0, YBoundary=0.0, \
         Coor4Match='XY_', XY_Quest=None, Match_xytol=2.0, RD_Quest=None, Match_rdtol=1.0, \
-        Preserve_NoMatch=False, MDIR=None, verbose='QUIET'):
+        Preserve_NoMatch=False, MDIR=None, VERBOSE_TYPE='QUIET', VERBOSE_LEVEL=2):
 
         """
         # Inputs & Outputs:
 
         -FITS_obj []                    # FITS file path of the input image for photometry
  
         -PSF_obj [None]                 # PSFEx .psf file path for PSF photometry
 
         -FITS_ref [None]                # FITS file path of the input image for detection 
                                         # (a) -FITS_ref = None means single image mode:  
                                         #     SEx detection & SEx photometry on same image -FITS_obj.
                                         # (b) -FITS_ref != None mean dual image mode:
                                         #     SEx detection on -FITS_ref & SEx photometry on -FITS_obj
 
-        -PL [None]                      # Parameter List (Python list here) of SExtractor output catalog
+        -SExParam [None]               # Parameter List (Python list here) of SExtractor output catalog
                                         # one can use command line 'sex -dp' to find all available parameters
 
         # Configurations for SExtractor:
 
         -CATALOG_TYPE ['FITS_LDAC']     # SExtractor Parameter CATALOG_TYPE
                                         # NONE,ASCII,ASCII_HEAD, ASCII_SKYCAT,
                                         # ASCII_VOTABLE, FITS_1.0 or FITS_LDAC
@@ -72,14 +71,18 @@
         -BACK_SIZE [64]                 # SExtractor Parameter BACK_SIZE
 
         -BACK_FILTERSIZE [3]            # SExtractor Parameter BACK_FILTERSIZE
 
         -DETECT_THRESH [1.5]            # SExtractor Parameter DETECT_THRESH
                                         # <sigmas> or <threshold>,<ZP> in mag.arcsec-2
 
+        -ANALYSIS_THRESH [1.5]          # SExtractor Parameter ANALYSIS_THRESH
+                                        # <sigmas> or <threshold>,<ZP> in mag.arcsec-2
+                                        # Threshold at which CLASS STAR and FWHM_ operate.
+
         -DETECT_MINAREA [5]             # SExtractor Parameter DETECT_MINAREA
                                         # min. # of pixels above threshold
         
         -DETECT_MAXAREA [0]             # SExtractor Parameter DETECT_MAXAREA
                                         # max. # of pixels above threshold (0=unlimited)
 
         -DEBLEND_MINCONT [0.005]        # SExtractor Parameter DEBLEND_MINCONT (typically, 0.001 - 0.005)
@@ -96,30 +99,30 @@
                                         # MAG_APER aperture diameter(s) in pixels
                                         # P.S. Here it can be a Python list of apertures
 
         -CHECKIMAGE_TYPE ['NONE']       # SExtractor Parameter CHECKIMAGE_TYPE
                                         # can be NONE, BACKGROUND, BACKGROUND_RMS, MINIBACKGROUND, MINIBACK_RMS, 
                                         # -BACKGROUND, FILTERED, OBJECTS, -OBJECTS, SEGMENTATION, or APERTURES
 
-        -verbose ['QUIET']              # SExtractor Parameter VERBOSE_TYPE
+        -VERBOSE_TYPE ['QUIET']         # SExtractor Parameter VERBOSE_TYPE
                                         # can be QUIET, NORMAL or FULL
 
         # Other parameters
 
         -NegativeCorr [True]            # In SExtractor, MAG_* = 99. and MAGERR_* = 99. for FLUX_* < 0.0 
                                         # If -NegativeCorr = True, PYSEx will correct MAG_* and MAGERR_* 
                                         # to be a valid values using abs(FLUX_*) and FLUXERR_*.
 
         -VIGNET [None]                  # VIGNET for generating PSFEx input catalog
                                         # e.g., set -VIGNET = (51, 51), PYSEx will add 'VIGNET(51, 51)' into 
                                         #       the SExtractor output parameter list.
 
-        -StampImgSize [None]            # PYSEx allows for making a stamp for each detected source on -FITS_obj,
+        -STAMP_IMGSIZE [None]            # PYSEx allows for making a stamp for each detected source on -FITS_obj,
                                         # the stamps will be saved in a new column named 'Stamp' in the output catalog.
-                                        # -StampImgSize is the stamp size, e.g., -StampImgSize = (31, 31)
+                                        # -STAMP_IMGSIZE is the stamp size, e.g., -STAMP_IMGSIZE = (31, 31)
 
         -AddRD [False]                  # Add columns for Ra. and Decl. in the output catalog?
                                         # P.S. The columns are X_WORLD, Y_WORLD or XWIN_WORLD, YWIN_WORLD.
                                         #      Although SExtractor itself can generate these columns, here we use 
                                         #      astropy.wcs to convert image coordinates to world coordinates instead.
                                         #      (Because I feel like that astropy has better WCS compatibility than SExtractor)
 
@@ -156,147 +159,163 @@
         -RD_Quest [None]                # The world coordinates you would like to cross match with SExtractor photometry catalog.
                                         # P.S. it is a Python array with shape (2, NUM_SOURCE), a collection of (ra, dec)
 
         -Match_rdtol [1.0]              # The cross match tolerance (arcsec)
 
         -Preserve_NoMatch [False]       # Preserve the detected sources in SExtractor photometry catalog without cross match counterpart
 
-        -MDIR [None]                    # Directory for output files
+        -MDIR [None]                    # Parent Directory for output files
+                                        # PYSEx will generate a child directory with a random name under the paraent directory 
+                                        # all output files are stored in the child directory
+
+        -VERBOSE_LEVEL [2]              # The level of verbosity, can be [0, 1, 2]
+                                        # 0/1/2: QUIET/NORMAL/FULL mode
+                                        # NOTE: it only controls the verbosity out of SExtractor.
         
         # Returns:
 
             AstSEx                      # astropy Table of SExtractor photometry catalog
 
             PixA_SExCheckLst            # List of Pixel arrays for SExtractor check images
                                         # P.S. PixA = fits.getdata(FITS, ext=0).T
             
             FITS_SExCat                 # File path of SExtractor photometry catalog
                                         # P.S. only for -MDIR is not None
 
             FITS_SExCheckLst            # List of file path of SExtractor check images
                                         # P.S. only for -MDIR is not None
 
-        
+
         # ---------------- MORE DESCRIPTION ON HOW SEXTRACTOR WORK ---------------- 
         #
         # * SExtractor Inputs
         #    ** Array-Inputs:
         #       SEx works on one image for signal detection and another image for photometry 
-        #       @Individual Mode (Common): Image4detect and Image4phot are the same image (-FITS_obj).
-        #       @Dual Mode: Image4detect (-FITS_ref) and Image4phot (-FITS_obj) are different images .
+        #       @ Individual Mode (Common): Image4detect and Image4phot are the same image (-FITS_obj).
+        #       @ Dual Mode: Image4detect (-FITS_ref) and Image4phot (-FITS_obj) are different images .
         #    ** PSF-Input:
         #       SEx can accept given PSF model for PSF-Photometry (-PSF_obj).
         #    ** Parameter-Inputs: 
         #       a. Basic keywords in FITS header of Image4detect:
         #          (-GAIN_KEY, -SATUR_KEY).
         #       b. How to generate Global Background Map:
         #          (-BACK_TYPE, -BACK_VALUE, -BACK_SIZE, -BACK_FILTERSIZE).
         #       c. Give the criteria for SExtractor Source Detection
         #          (-DETECT_THRESH, -DETECT_MINAREA, -DETECT_MAXAREA, -DEBLEND_NTHRESH, -DEBLEND_MINCONT, -CLEAN).
         #       d. Which photometry method(s) used by SExtractor: 
-        #          (parameters in -PL, e.g., FLUX_AUTO, FLUX_APER, FLUX_PSF).
+        #          (parameters in -SExParam, e.g., FLUX_AUTO, FLUX_APER, FLUX_PSF).
         #       e. Specify output Check-Images: 
         #          (-CHECKIMAGE_TYPE).
         #       f. Specify output columns in output SExtractor photometry table: 
-        #          (-PL).
+        #          (-SExParam).
         #
-        #    TODO: Incorporate the Weight-Map Image as Input of PYSEx
-        #          SExtractor allows users to feed a weight-map image. It is very useful for mosaic image, which has
-        #          vairable effective GAIN and background noise level across the field due to different Num_Exposure.
-        #          A weight-map image would help SExtractor to calculate errors, such as, FLUXERR and MAGERR, more accurately. 
-        #          For current version, I would recommend users to set an average effective GAIN for mosaic image, 
-        #          and keep in mind it may cause inaccurate error estimation (to some extent) in SExtractor.
+        #    Remarks on Weight-Map:
+        #       SExtractor allows users to feed a weight-map image. It is very useful for mosaic image, which has
+        #       vairable effective GAIN and background noise level across the field due to different Num_Exposure.
+        #       Weight-map would help SExtractor to calculate errors, such as, FLUXERR and MAGERR, more accurately.
+        #
+        #       WARNING: For current version, PYSEx does not include this feature, and I would recommend users  
+        #                to set an average effective GAIN for mosaic image, and keep in mind it may, to some extent, 
+        #                cause inaccurate error estimations.
         #
         # * SExtractor Workflow (Background)
         #    ** Extract Global_Background_Map (GBMap) and its RMS (GBRMap) from Image4detect & Image4phot
         #       Control Parameters: BACK_TYPE, BACK_VALUE, BACK_SIZE and BACK_FILTERSIZE.
         #       @ Produce GBMap 
         #         a. Manual-FLAT (e.g. BACK_TYPE='MANUAL', BACK_VALUE=100.0)
         #            SEx directly define GBMap as a FLAT image with given constant BACK_VALUE.
         #         b. Auto (e.g. BACK_TYPE='AUTO', BACK_SIZE=64, BACK_FILTERSIZE=3)
         #            SEx defines a mesh of a grid that covers the whole frame by [BACK_SIZE].
         #            i. Convergence-based sigma-clipping method on the flux histogram of each tile.
-        #               More specificly, the flux histogram is clipped iteratively until convergence at +/- 3sigma around its median.
+        #               More specificly, the flux histogram is clipped iteratively until convergence 
+        #               at +/- 3sigma around its median.
         #            ii. SEx compute local background estimator from the clipped histogram of each tile.
         #                If sigma is changed by less than 20% during clipping process (the tile is not crowded), 
         #                use the mean of the clipped histogram as estimator
         #                otherwise (the tile is crowded), mode = 2.5*median - 1.5*mean is employed instead.
         #            iii. Once the estimate grid is calculated, a median filter [BACK_FILTERSIZE] can be applied 
         #                 to suppress possible local overestimations.
-        #            iv. The resulting background map is them simply a bicubic-spline interpolation between the meshes of the grid.
+        #            iv. The resulting background map is them simply a bicubic-spline interpolation 
+        #                between the meshes of the grid.
         #
         #        @ Generate GBRMap
-        #            only Auto (e.g, BACK_SIZE=64, BACK_FILTERSIZE=3)
-        #            SEx produces the noise map by the same approach of Auto style of GBMap, where the only difference is that
-        #            SEx is [probably] use standard deviation as estimator of the clipped flux historgram, other than mean or mode.
+        #          only Auto (e.g, BACK_SIZE=64, BACK_FILTERSIZE=3)
+        #          SEx produces the noise map by the same approach of Auto style of GBMap, where the only 
+        #          difference is that SEx is [probably] use standard deviation as estimator of the 
+        #          clipped flux historgram, other than mean or mode.
         #        
         #        NOTE Abbr. GBMap / GBRMap from Image4detect: GBMap_4d / GBRMap_4d
         #             Abbr. GBMap / GBRMap from Image4phot: GBMap_4p / GBRMap_4p
+        #
         #        NOTE WARNING: Dual Mode have to use consistent control parameters for Image4detect & Image4phot, 
         #                      as it is not allowed to set some secondary configuration in SEx software framework, 
         #                      despite that it  is not necessarily reasonable in some cases.
         #
         # * SExtractor Workflow (Detection)
         #    ** a. SEx-Detect on Image4detect: SkySubtraction & Filtering & Thresholding & Deblending & AreaConstrain & Clean
         #          @ SkySubtraction & Filtering Process (e.g. FILTER='Y', FILTER_NAME='default.conv')
-        #              SEx Remove GBMap_4d from Image4detect and then perform a convolution to maximizes detectability. 
-        #              NOTE The power-spectrum of the noise and that of the superimposed signal can be signiﬁcantly different.
-        #              NOTE Although Filtering is a beneﬁt for detection, it distorts proﬁles and correlates the noise.
-        #              NOTE Filtering is applied 'on the ﬂy' to the image, and directly affects only the following 
-        #                   Thresholding process and Isophotal parameters.
+        #            SEx Remove GBMap_4d from Image4detect and then perform a convolution to maximizes detectability. 
+        #            NOTE The power-spectrum of the noise and that of the superimposed signal can be significantly different.
+        #            NOTE Although Filtering is a benefit for detection, it distorts profiles and correlates the noise.
+        #            NOTE Filtering is applied 'on the fly' to the image, and directly affects only the following 
+        #                 Thresholding process and Isophotal parameters.
         #
         #          @ Thresholding Process (e.g. DETECT_THRESH=1.5, THRESH_TYPE='RELATIVE')
-        #              SEx highlights the pixels in Filtered_Image with Threshold_Map = DETECT_THRESH * GBRMap_4d
-        #              We would be bettter to imagine SEx actually make a hovering mask.
+        #            SEx highlights the pixels in Filtered_Image with Threshold_Map = DETECT_THRESH * GBRMap_4d
+        #            We would be bettter to imagine SEx actually make a hovering mask.
         #
         #          @ Deblending Process (e.g. DEBLEND_MINCONT=0.005, DEBLEND_NTHRESH=32)
-        #              SEx triggers a deblending process to dentify signal islands from the hovering mask [probably] on Filtered_Image,
-        #              which converts the hovering mask to be a hovering label map.
+        #            SEx triggers a deblending process to dentify signal islands from the hovering 
+        #            mask [probably] on Filtered_Image,
+        #            which converts the hovering mask to be a hovering label map.
         #
         #          @ Put AreaConstrain (e.g. DETECT_MINAREA=5, DETECT_MAXAREA=0)
-        #              MinMax AreaContrain is applied and then iolated cases then lose their hovering labels. 
+        #            MinMax AreaContrain is applied and then iolated cases then lose their hovering labels. 
         #
         #          @ Clean Process (e.g. CLEAN='YES')
-        #              SEx will clean the list of objects of artifacts caused by bright objects.
-        #              As a correction process, all cleaned objects are subsequently removed from the hovering label map.
-        #              NOTE Now the hovering label map is the SEGMENTATION check image. One may refer to such label island as ISOIsland
-        #              NOTE These labels are consistent with the indices in the ouput photometry table.
-        #              NOTE SEx will report something like this: Objects: detected 514 / sextracted 397 
-        #                   SET CLEAN='N', you could find detected == sextracted.
+        #            SEx will clean the list of objects of artifacts caused by bright objects.
+        #            As a correction process, all cleaned objects are subsequently removed from the hovering label map.
+        #            NOTE Now the hovering label map is the SEGMENTATION check image. 
+        #                 One may refer to such label island as ISOIsland
+        #            NOTE These labels are consistent with the indices in the ouput photometry table.
+        #            NOTE SEx will report something like this: Objects: detected 514 / sextracted 397 
+        #                 SET CLEAN='N', you could find detected == sextracted.
         #
         #    ** b. Generate Positional & BasicShape Paramters from isophotal profile
         #          NOTE In this section 'pixel flux' means values of Filtered_Image.
-        #          i. XMIN, XMAX, YMIN, YMAX deﬁne a rectangle which encloses the ISOIsland.
+        #          i. XMIN, XMAX, YMIN, YMAX define a rectangle which encloses the ISOIsland.
         #          ii. Barycenter X_IMAGE, Y_IMAGE is the first order moments of the profile, where the pixel flux of
         #              ISOIsand is the corresponding weight for cacluatuing Barycenter.
         #          iii. Centered second-order moments X2_IMAGE, Y2_IMAGE, XY2_IMAGE are convenient for
-        #               measuring the spatial spread of a source proﬁle. likewise, pixel fluxs of ISOIsand are weights.
+        #               measuring the spatial spread of a source profile. likewise, pixel fluxs of ISOIsand are weights.
         #               (if a parameter can be fully expressed by them, we will use $ to indicate).
         #          iv. Describe ISOIsand as an elliptical shape, centred at Barycenter.
         #               $A_IMAGE, $B_IMAGE are ellipse semi-major and semi-minor axis lengths, respectively.
         #               The ellipse is uniquely determined by $CXX_IMAGE, $CYY_IMAGE, $CXY_IMAGE with KRON_RADIUS, 
         #               where KRON_RADIUS is independently calculated in a routine inspired by Kron's 'first moment' algorithm.
         #               NOTE By-products: $ELONGATION = A / B and $ELLIPTICITY = 1 - B / A
         #
         #    ** c. Generate Positional & BasicShape Paramters from Window
         #          NOTE In this section 'pixel flux' [likely] means values of Image4phot !
-        #          NOTE It is designed for Refinement, NOT for Photometry, thereby all of these parameters are irrelevant to Photometry !
+        #          NOTE It is designed for Refinement, NOT for Photometry, thereby these parameters are irrelevant to Photometry!
+        #
         #          METHOD: The computations involved are roughly the same except that the domain is a circular Gaussian window,
         #                  (I don't know what is the window radius) as opposed to the object's isophotal footprint (ISOIsland).
+        #
         #          MOTIVATION: Parameters measured within an object's isophotal limit are sensitive to two main factors: 
         #                      + Changes in the detection threshold, which create a variable bias 
         #                      + Irregularities in the object's isophotal boundaries, which act as 
         #                        additional 'noise' in the measurements.
         #
         #          @Positional: This is an iterative process. The computation starts by initializing 
         #                       the windowed centroid coordinates to the Barycenter.
         #                       The process will adjust window and finally its centroid converges 
         #                       at some point: XWIN_IMAGE, YWIN_IMAGE.
         #                       (If the process is failed then XWIN_IMAGE, YWIN_IMAGE = X_IMAGE, Y_IMAGE)
-        #                       It has been veriﬁed that for isolated, Gaussian-like PSFs, its accuracy is close to 
+        #                       It has been verified that for isolated, Gaussian-like PSFs, its accuracy is close to 
         #                       the theoretical limit set by image noise. 
         #                       NOTE: We preferably use it for point sources, like in transient detection. 
         #                             However it may not optimal for extended sources like glaxies.
         #                       NOTE: X_IMAGE & Y_IMAGE seems to be a good compromise choice.
         #
         #          @BasicShape: Windowed second-order moments are computed once the centering process has converged.
         #                       X2WIN_IMAGE, Y2WIN_IMAGE, XY2WIN_IMAGE
@@ -309,34 +328,34 @@
         #
         #    ** d. Generate Positional Paramters from PSF Fitting
         #          NOTE In this section 'pixel flux' is [possibly] means values of skysubtracted-Image4detect !
         #          METHOD: XPSF_IMAGE and YPSF_IMAGE are fitted from given PSF model.
         #
         # * SExtractor Workflow (Photometry)
         #    ** Count Flux with various photometry methods
-        #          NOTE This process always works on Image4phot.
-        #          @ISO: SEx simply count flux according to the hovering label map (ISOIsland).
-        #          @APER: SEx count flux on a Circular Aperture with given PHOT_APERTURES (centred at Barycenter X_IMAGE, Y_IMAGE).
-        #          @AUTO: SEx count flux on a Elliptic Aperture, which is determined by the hovering isophotal ellipse 
-        #                 (centred at Barycenter X_IMAGE, Y_IMAGE). The leaked light fraction is typically less than 10%.
-        #          @PSF: SEx count flux according to the PSF fitting results (centred at XPSF_IMAGE and YPSF_IMAGE).
-        #                This is optimal for pointsource but fairly wrong for extended objects.
+        #       NOTE This process always works on Image4phot.
+        #       @ISO: SEx simply count flux according to the hovering label map (ISOIsland).
+        #       @APER: SEx count flux on a Circular Aperture with given PHOT_APERTURES (centred at Barycenter X_IMAGE, Y_IMAGE).
+        #       @AUTO: SEx count flux on a Elliptic Aperture, which is determined by the hovering isophotal ellipse 
+        #              (centred at Barycenter X_IMAGE, Y_IMAGE). The leaked light fraction is typically less than 10%.
+        #       @PSF: SEx count flux according to the PSF fitting results (centred at XPSF_IMAGE and YPSF_IMAGE).
+        #             This is optimal for pointsource but fairly wrong for extended objects.
         #
         #    ** Peel background contribution from Counted Flux
-        #          @BACKPHOTO_TYPE='LOCAL': background will take a rectangular annulus into account, 
-        #                                   which has a donnut shape around the object, measured on Image4phot.
-        #          @BACKPHOTO_TYPE='GLOBAL': background will directly use GBMap_4p,
-        #                                    which can be Manual-Flat or Auto.
+        #       @BACKPHOTO_TYPE='LOCAL': background will take a rectangular annulus into account, 
+        #                                which has a donnut shape around the object, measured on Image4phot.
+        #       @BACKPHOTO_TYPE='GLOBAL': background will directly use GBMap_4p,
+        #                                 which can be Manual-Flat or Auto.
         #
         #    ** Noise Estimation
-        #          METHOD: SEx estimate the photometric noise contributed from photon possion distribution and sky background.
-        #                  that is, FLUXERR^2 = FLUX / GAIN + Area * skysig^2
-        #          NOTE: Area means the pixel area of flux-count domain for various photometry methods.
-        #          NOTE: skysig^2 is [probably] the sum of GBRMap_4p within the flux-count domain.
-        #          NOTE: Bright Sources are Photon Noise Dominated cases, while Faint Sources are Sky Noise Dominated cases.
+        #       METHOD: SEx estimate the photometric noise contributed from photon possion distribution and sky background.
+        #               that is, FLUXERR^2 = FLUX / GAIN + Area * skysig^2
+        #       NOTE: Area means the pixel area of flux-count domain for various photometry methods.
+        #       NOTE: skysig^2 is [probably] the sum of GBRMap_4p within the flux-count domain.
+        #       NOTE: Bright Sources are Photon Noise Dominated cases, while Faint Sources are Sky Noise Dominated cases.
         #
         # * SExtractor Workflow (Check-Image)
         #    @BACKGROUND : GBMap_4p
         #    @BACKGROUND_RMS : GBRMap_4d
         #    @-BACKGROUND : Image4phot - GBMap_4p
         #    @FILTERED: Filtered_Image 
         #    @SEGMENTATION: ISOIsland Label Map
@@ -424,87 +443,101 @@
         #     some constant leaked light when we measure on SCI. Equivalently, DMAG = MAG_APER_SCI - MAG_APER_REF 
         #     deviate zero-baseline, and it becomes increasingly serious (towards to the faint end).
         #
         #     ------------------------------------ 
         #     We guess the problem is caused by the fact: the background value calculated from the annulus 
         #     around target might be a biased (over/under-) estimation. One observation supports our argument: 
         #     the flux bias is much more evident when we increase the aperture size.
-        #     NOTE:  As we have found the flux bias is basically a constant, we can do relative-calibration by calculate the compensation 
-        #            offset FLUX_APER_REF - FLUX_APER_SCI for a collection of sationary stars. It is 'relative' since we have just assumed 
-        #            background estimation of REF is correct, which is proper if we are going to derive the variability (light curve).
+        #     NOTE: As we have found the flux bias is basically a constant, we can do relative-calibration by 
+        #           calculating the compensation offset FLUX_APER_REF - FLUX_APER_SCI for a collection of sationary stars. 
+        #           It is 'relative' since we have just assumed background estimation of REF is correct, 
+        #           which is proper if we are going to derive the variability (light curve).
         #
-        #   @ In which cases, Re-Run SExtractor can get the same coordinate list ?
+        #   @ In which cases, Re-Run SExtractor can get the same coordinate list?
         #     a. Same configurations but only change photometric method, e.g. from AUTO to APER 
         #     b. Same configurations but from Single-Image Mode to Dual-Image Mode
-        #     NOTE: FLAGS is correlated to object image, if we add constraint FLAG=0 then we fail to get the same coordinate list.
+        #     NOTE: FLAGS is correlated to object image, if we add constraint FLAG=0
+        #           then we fail to get the same coordinate list.
         #
         """
 
         # * sex or sextractor?
         for cmd in ['sex', 'sextractor']:
             try:
                 p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
                 del p
                 break
             except OSError:
                 continue
         else:
-            raise FileNotFoundError('Source Extractor command not found.')
+            raise FileNotFoundError('Source Extractor command NOT FOUND!')
         SEx_KEY = cmd
         del cmd
 
         # * Make Directory as workplace
+        objname = pa.basename(FITS_obj)
         TDIR = mkdtemp(suffix=None, prefix='PYSEx_', dir=MDIR)
-        print('\nMeLOn: Run Python Version of SExtractor on FITS file: %s' %FITS_obj)
+        if VERBOSE_LEVEL in [0, 1, 2]:
+            _message = 'Run Python Wrapper of SExtractor!'
+            print('\nMeLOn CheckPoint [%s]: %s' %(objname, _message))
 
         # * Keyword Configurations 
         phr_obj = fits.getheader(FITS_obj, ext=0)       
         if GAIN_KEY in phr_obj:
             GAIN = phr_obj[GAIN_KEY]
-            print('MeLOn CheckPoint: SEx use GAIN=%s [READ from FITS header %s]' %(GAIN, GAIN_KEY))
+            if VERBOSE_LEVEL in [1, 2]:
+                _message = 'SExtractor uses GAIN = [%s] from keyword [%s]!' %(GAIN, GAIN_KEY)
+                print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
         else: 
-            GAIN = 0.0
-            warnings.warn('MeLOn WARNING: SEx use GAIN=%s [SExtractor default value]' %GAIN)
+            GAIN = 0.0  # infinite GAIN, Poission noise ignored
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'SExtractor has to use default GAIN = 0!'
+                warnings.warn('MeLOn WARNING [%s]: %s' %(objname, _warn_message))
         
         if SATUR_KEY in phr_obj:
             SATURATION = phr_obj[SATUR_KEY]
-            print('MeLOn CheckPoint: SEx use SATURATION=%s [READ from FITS header %s]' %(SATURATION, SATUR_KEY))
+            if VERBOSE_LEVEL in [1, 2]:
+                _message = 'SExtractor uses SATURATION = [%s] from keyword [%s]!' %(SATURATION, SATUR_KEY)
+                print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
         else: 
             SATURATION = 50000.0
-            warnings.warn('MeLOn WARNING: SEx use SATURATION=%s [SExtractor default value]' %SATURATION)
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'SExtractor has to use default SATURATION = 50000.0!'
+                warnings.warn('MeLOn WARNING [%s]: %s' %(objname, _warn_message))
         
         """
-        # some additional remarks
+        # A few additional remarks
         # [1] MAGERR/FLUXERR/SNR are very sensitive to GAIN value.
         # [2] PIXEL_SCALE (unit: arcsec) only works for surface brightness parameters, 
         #     FWHM (FWHM_WORLD) and star/galaxy separation. PIXEL_SCALE=0 uses FITS WCS info.
         # [3] SEEING_FWHM (unit: arcsec) is only for star/galaxy separation.
         #     VIP: You'd better to give a good estimate if star/galaxy separation is needed.
         # [4] A common criteria for isolated point sources:
         #     CLASS_STAR (output parameter) > 0.95 & FLAG = 0
         #
         """
 
         # * Main Configurations
         ConfigDict = {}
         ConfigDict['CATALOG_TYPE'] = CATALOG_TYPE
-        ConfigDict['VERBOSE_TYPE'] = '%s' %verbose
+        ConfigDict['VERBOSE_TYPE'] = '%s' %VERBOSE_TYPE
 
         ConfigDict['GAIN_KEY'] = '%s' %GAIN_KEY
         ConfigDict['SATUR_KEY'] = '%s' %SATUR_KEY
         ConfigDict['MAG_ZEROPOINT'] = '0.0'        
         ConfigDict['PIXEL_SCALE'] = '%s' %PIXEL_SCALE
         ConfigDict['SEEING_FWHM'] = '%s' %SEEING_FWHM
         
         ConfigDict['BACK_TYPE'] = '%s' %BACK_TYPE
         ConfigDict['BACK_VALUE'] = '%s' %BACK_VALUE
         ConfigDict['BACK_SIZE'] = '%s' %BACK_SIZE
         ConfigDict['BACK_FILTERSIZE'] = '%s' %BACK_FILTERSIZE
 
         ConfigDict['DETECT_THRESH'] = '%s' %DETECT_THRESH
+        ConfigDict['ANALYSIS_THRESH'] = '%s' %ANALYSIS_THRESH
         ConfigDict['DETECT_MINAREA'] = '%s' %DETECT_MINAREA
         ConfigDict['DETECT_MAXAREA'] = '%s' %DETECT_MAXAREA
         ConfigDict['DEBLEND_NTHRESH'] = '%s' %DEBLEND_NTHRESH
         ConfigDict['DEBLEND_MINCONT'] = '%s' %DEBLEND_MINCONT
         ConfigDict['CLEAN'] = '%s' %CLEAN
         
         ConfigDict['CHECKIMAGE_TYPE'] = '%s' %CHECKIMAGE_TYPE
@@ -524,15 +557,15 @@
             conv_text += "1 2 1"
             conv_path = ''.join([TDIR, "/PYSEx.conv"])
             _cfile = open(conv_path, 'w')
             _cfile.write(conv_text)
             _cfile.close()
         
         USE_NNW = False
-        if 'CLASS_STAR' in PL: 
+        if 'CLASS_STAR' in SExParam: 
             USE_NNW = True
         
         if USE_NNW:
             # see https://github.com/astromatic/sextractor/blob/master/config/default.nnw
             nnw_text = r"""
             NNW
             # Neural Network Weights for the SExtractor star/galaxy classifier (V1.3)
@@ -567,24 +600,24 @@
             nnw_text = '\n'.join([line[nintent: ] for line in re.split('\n', nnw_text)[1:]])
             nnw_path = ''.join([TDIR, "/PYSEx.nnw"])
             _cfile = open(nnw_path, 'w')
             _cfile.write(nnw_text)
             _cfile.close()
 
         # create configuration file .param
-        Param_lst = PL.copy()
-        if PL is None: Param_lst = []
-        if 'X_IMAGE' not in Param_lst: 
-            Param_lst.append('X_IMAGE')
-        if 'Y_IMAGE' not in Param_lst: 
-            Param_lst.append('Y_IMAGE')
+        USExParam = SExParam.copy()
+        if SExParam is None: USExParam = []
+        if 'X_IMAGE' not in USExParam: 
+            USExParam.append('X_IMAGE')
+        if 'Y_IMAGE' not in USExParam: 
+            USExParam.append('Y_IMAGE')
 
         Param_path = ''.join([TDIR, "/PYSEx.param"])
-        if VIGNET is not None: Param_lst += ['VIGNET(%d, %d)' %(VIGNET[0], VIGNET[1])]
-        Param_text = '\n'.join(Param_lst)
+        if VIGNET is not None: USExParam += ['VIGNET(%d, %d)' %(VIGNET[0], VIGNET[1])]
+        Param_text = '\n'.join(USExParam)
         pfile = open(Param_path, 'w')
         pfile.write(Param_text)
         pfile.close()
 
         # create configuration file .sex
         if not USE_FILT: ConfigDict['FILTER'] = 'N'
         if USE_FILT: ConfigDict['FILTER_NAME'] = "%s" %conv_path
@@ -592,37 +625,40 @@
         ConfigDict['PARAMETERS_NAME'] = "%s" %Param_path
 
         FNAME = pa.basename(FITS_obj)
         FITS_SExCat = ''.join([TDIR, '/%s_PYSEx_CAT.fits' %FNAME[:-5]])
         _cklst = re.split(',', CHECKIMAGE_TYPE)
         FITS_SExCheckLst = [''.join([TDIR, '/%s_PYSEx_CHECK_%s.fits' %(FNAME[:-5], ck)]) for ck in _cklst]
 
-        sexconfig_path = AMConfig_Maker.AMCM(MDIR=TDIR, AstroMatic_KEY=SEx_KEY, \
+        sex_config_path = AMConfig_Maker.AMCM(MDIR=TDIR, AstroMatic_KEY=SEx_KEY, \
             ConfigDict=ConfigDict, tag='PYSEx')
             
         # * Trigger SExtractor
         if FITS_ref is None:
-            os.system("cd %s && %s %s -c %s -CATALOG_NAME %s -CHECKIMAGE_NAME %s"\
-                %(pa.dirname(FITS_obj), SEx_KEY, FNAME, sexconfig_path, FITS_SExCat, ','.join(FITS_SExCheckLst)))
+            os.system("cd %s && %s %s -c %s -CATALOG_NAME %s -CHECKIMAGE_NAME %s" \
+                %(pa.dirname(FITS_obj), SEx_KEY, FNAME, sex_config_path, \
+                  FITS_SExCat, ','.join(FITS_SExCheckLst)))
         
         if FITS_ref is not None:
             # WARNING: more risky to fail due to the too long string.
-            os.system("%s %s,%s -c %s -CATALOG_NAME %s -CHECKIMAGE_NAME %s"\
-                %(SEx_KEY, FITS_ref, FITS_obj, sexconfig_path, FITS_SExCat, ','.join(FITS_SExCheckLst)))    
+            os.system("%s %s,%s -c %s -CATALOG_NAME %s -CHECKIMAGE_NAME %s" \
+                %(SEx_KEY, FITS_ref, FITS_obj, sex_config_path, \
+                  FITS_SExCat, ','.join(FITS_SExCheckLst)))    
         
         """
-        # deprecated as it requires WCSTools, and seems not very useful
+        # Deprecated as it requires WCSTools, and seems not very useful
         def record(FITS):
             os.system('sethead %s SOURCE=%s' %(FITS, FITS_obj))
             os.system('sethead %s RSOURCE=%s' %(FITS, FITS_ref))
             for key in ConfigDict:
                 value = ConfigDict[key]
                 pack = ' : '.join(['Sex Parameters', key, value])
                 os.system('sethead %s HISTORY="%s"' %(FITS, pack))
             return None
+        
         """
 
         if CATALOG_TYPE == 'FITS_LDAC': tbhdu = 2
         if CATALOG_TYPE == 'FITS_1.0': tbhdu = 1
         if pa.exists(FITS_SExCat):
             #if MDIR is not None: record(FITS_SExCat)
             AstSEx = Table.read(FITS_SExCat, hdu=tbhdu)
@@ -638,43 +674,46 @@
             PixA_SExCheckLst.append(PixA_SExCheck)
         FITS_SExCheckLst = FtmpLst
 
         # * Optional functions
         if AstSEx is not None:
             Modify_AstSEx = False
 
-            print('MeLOn CheckPoint: SExtractor finds [%d] sources | [%s]!' \
-                   %(len(AstSEx), pa.basename(FITS_obj)))
+            if VERBOSE_LEVEL in [1, 2]:
+                _message = 'SExtractor found [%d] sources!'  %(len(AstSEx))
+                print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
 
             # ** a. CORRECT the SExtractor bug on MAG & MAGERR due to negative flux count.
-            #       For such cases, corresponding MAG & MAGERR will turn to be a trivial 99
-            #       PYSEx will re-calculate them from FLUX & FLUXERR 
-            #       if MAG & MAGERR in PL and NegativeCorr=True.
-                        
-            MAG_TYPES = [p for p in Param_lst if p[:4] == 'MAG_']
+            #       For such cases, corresponding MAG & MAGERR will turn to be a trivial 99.
+            #       PYSEx will re-calculate them from FLUX & FLUXERR if MAG & MAGERR in PL and NegativeCorr=True.
+
+            MAG_TYPES = [p for p in USExParam if p[:4] == 'MAG_']
             if len(MAG_TYPES) > 0:
                 if NegativeCorr:
                     MAGERR_TYPES = ['MAGERR_' + MAGT[4:] for MAGT in MAG_TYPES]
                     FLUX_TYPES = ['FLUX_' + MAGT[4:] for MAGT in MAG_TYPES]
                     FLUXERR_TYPES = ['FLUXERR_' + MAGT[4:] for MAGT in MAG_TYPES]
                     
                     for i in range(len(MAG_TYPES)):
-                        pcomplete = (MAGERR_TYPES[i] in Param_lst) & \
-                                    (FLUX_TYPES[i] in Param_lst) & \
-                                    (FLUXERR_TYPES[i] in Param_lst)
+
+                        pcomplete = (MAGERR_TYPES[i] in USExParam) & \
+                                    (FLUX_TYPES[i] in USExParam) & \
+                                    (FLUXERR_TYPES[i] in USExParam)
                         
                         if not pcomplete:
-                            sys.exit('MeLOn ERROR: NEGATIVE FLUX Correction requires ' + \
-                                     'complete FLUX FLUXERR MAG MAGERR columns')
+                            _error_message = 'Please use complete FLUX FLUXERR MAG MAGERR ' 
+                            _error_message += 'in SExParam for Negative Flux Correction!'
+                            raise Exception('MeLOn ERROR [%s]: %s' %(objname, _error_message))
 
                         FLUX = np.array(AstSEx[FLUX_TYPES[i]])
                         FLUXERR = np.array(AstSEx[FLUXERR_TYPES[i]])
                         Mask_NC = FLUX < 0.0
                         MAG_NC = -2.5*np.log10(np.abs(FLUX[Mask_NC]))
                         MAGERR_NC = 1.0857 * np.abs(FLUXERR[Mask_NC] / FLUX[Mask_NC])
+                        
                         AstSEx[MAG_TYPES[i]][Mask_NC] = MAG_NC
                         AstSEx[MAGERR_TYPES[i]][Mask_NC] = MAGERR_NC
                     Modify_AstSEx = True
 
             # ** b. ADD-COLUMN SEGLABEL if SEGMENTATION requested.
             #       If some lines are discarded later, corresponding 
             #       SEGLABEL will be lost in the output table.
@@ -685,82 +724,75 @@
                 Modify_AstSEx = True
 
             # ** c. ADD-COLUMN of Sky-Coordinates by Astropy
             #       (X_IMAGE, Y_IMAGE) to (X_WORLD, Y_WORLD)
             #       (XWIN_IMAGE, YWIN_IMAGE) to (XWIN_WORLD, YWIN_WORLD)
 
             if AddRD:
-                def read_wcs(FITS_obj):
-                    phr = fits.getheader(FITS_obj, ext=0)
-                    if phr['CTYPE1'] == 'RA---TAN' and 'PV1_0' in phr:
-                        _hdr = phr.copy()
-                        _hdr['CTYPE1'] = 'RA---TPV'
-                        _hdr['CTYPE2'] = 'DEC--TPV'
-                        w = WCS(_hdr)
-                    else: w = WCS(phr)
-                    return w
-                
-                w_obj = read_wcs(FITS_obj)
+                w_obj = Read_WCS.RW(phr_obj, VERBOSE_LEVEL=VERBOSE_LEVEL)
                 _XY = np.array([AstSEx['X_IMAGE'], AstSEx['Y_IMAGE']]).T
                 _RD = w_obj.all_pix2world(_XY, 1)
                 AstSEx.add_column(Column(_RD[:, 0], name='X_WORLD'))          
                 AstSEx.add_column(Column(_RD[:, 1], name='Y_WORLD'))
 
-                if 'XWIN_IMAGE' in Param_lst:
-                    if 'YWIN_IMAGE' in Param_lst:
+                if 'XWIN_IMAGE' in USExParam:
+                    if 'YWIN_IMAGE' in USExParam:
                         _XY = np.array([AstSEx['XWIN_IMAGE'], AstSEx['YWIN_IMAGE']]).T
                         _RD = w_obj.all_pix2world(_XY, 1)
                         AstSEx.add_column(Column(_RD[:, 0], name='XWIN_WORLD'))          
                         AstSEx.add_column(Column(_RD[:, 1], name='YWIN_WORLD'))
                 Modify_AstSEx = True
             
             # ** d. Restriction on FLAGS
             if ONLY_FLAGS is not None:
-                if 'FLAGS' not in PL:
-                    sys.exit('MeLOn ERROR: Restriction of FLAGS required column FLAGS!')
+                if 'FLAGS' not in SExParam:
+                    _error_message = 'FLAGS is required in SExParam to apply restriction on FLAGS!'
+                    raise Exception('MeLOn ERROR [%s]: %s' %(objname, _error_message))
                 else:
                     _OLEN = len(AstSEx)
                     AstSEx = AstSEx[np.in1d(AstSEx['FLAGS'], ONLY_FLAGS)]    
                     Modify_AstSEx = True
 
-                    print('MeLOn CheckPoint: PYSEx excludes [%d / %d] sources by FLAGS restriction | [%s]!' \
-                           %(_OLEN - len(AstSEx), _OLEN, pa.basename(FITS_obj)))
+                    if VERBOSE_LEVEL in [2]:
+                        _message = 'PYSEx excludes [%d / %d] sources by FLAGS restriction!' %(_OLEN - len(AstSEx), _OLEN)
+                        print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
             
             # ** e. Remove Boundary Sources
             if XBoundary != 0.0 or XBoundary != 0.0:
                 NX, NY = int(phr_obj['NAXIS1']), int(phr_obj['NAXIS2'])
                 _XY = np.array([AstSEx['X_IMAGE'], AstSEx['Y_IMAGE']]).T
+
                 InnerMask = np.logical_and.reduce((_XY[:, 0] > XBoundary + 0.5, \
                                                    _XY[:, 0] < NX - XBoundary + 0.5, \
                                                    _XY[:, 1] > YBoundary + 0.5, \
                                                    _XY[:, 1] < NY - YBoundary + 0.5))
+                
                 _OLEN = len(AstSEx)
                 AstSEx = AstSEx[InnerMask]
                 Modify_AstSEx = True
 
-                print('MeLOn CheckPoint: PYSEx excludes [%d / %d] sources close to boundary | [%s]!' \
-                   %(_OLEN - len(AstSEx), _OLEN, pa.basename(FITS_obj)))
-            
+                if VERBOSE_LEVEL in [2]:
+                    _message = 'PYSEx excludes [%d / %d] sources by boundary rejection!' %(_OLEN - len(AstSEx), _OLEN)
+                    print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
+
             # ** f. Only preserve the sources matched to the quest coordinates
             if Coor4Match == 'XY_':
                 Xcoln_4Match, Ycoln_4Match = 'X_IMAGE', 'Y_IMAGE'
                 RAcoln_4Match, DECcoln_4Match = 'X_WORLD', 'Y_WORLD'
 
             if Coor4Match == 'XYWIN_':
-                assert 'XWIN_IMAGE' in Param_lst
-                assert 'YWIN_IMAGE' in Param_lst
+                assert 'XWIN_IMAGE' in USExParam
+                assert 'YWIN_IMAGE' in USExParam
                 Xcoln_4Match, Ycoln_4Match = 'XWIN_IMAGE', 'YWIN_IMAGE'
                 RAcoln_4Match, DECcoln_4Match = 'XWIN_WORLD', 'YWIN_WORLD'
 
-            if XY_Quest is not None:
-                if RD_Quest is not None:
-                    sys.exit('MeLOn ERROR: Please feed only one type XY_Quest / RD_Quest!')
-            if RD_Quest is not None:
-                if not AddRD:
-                    sys.exit('MeLOn ERROR: RD_Quest requires AddRD!')
+            assert XY_Quest is None or RD_Quest is None
+            if RD_Quest is not None and not AddRD:
+                _error_message = 'AddRD is required in SExParam when RD_Quest is given!'
+                raise Exception('MeLOn ERROR [%s]: %s' %(objname, _error_message))
 
             Symm = None
             if XY_Quest is not None:
                 _XY = np.array([AstSEx[Xcoln_4Match], AstSEx[Ycoln_4Match]]).T
                 Symm = Symmetric_Match.SM(XY_A=XY_Quest, XY_B=_XY, tol=Match_xytol, return_distance=False)
             if RD_Quest is not None:
                 _RD = np.array([AstSEx[RAcoln_4Match], AstSEx[DECcoln_4Match]]).T
@@ -781,41 +813,43 @@
                     AstSEx = AstSEx[Symm[:, 1]]
                     
                     QuestMATCH = np.ones(len(AstSEx)).astype(bool)
                     AstSEx.add_column(Column(QuestMATCH, name='QuestMATCH'))
                     
                     QuestINDEX = Symm[:, 0]
                     AstSEx.add_column(Column(QuestINDEX, name='QuestINDEX'))
-
-                    print('MeLOn CheckPoint: PYSEx excludes [%d / %d] sources by symmetric matching | [%s]!' \
-                           %(_OLEN - len(AstSEx), _OLEN, pa.basename(FITS_obj)))
-
-            print('MeLOn CheckPoint: PYSEx output catalog contains [%d] sources | [%s]!' \
-                   %(len(AstSEx), pa.basename(FITS_obj)))
+                    
+                    if VERBOSE_LEVEL in [2]:
+                        _message = 'PYSEx excludes [%d / %d] sources by symmetric matching!' %(_OLEN - len(AstSEx), _OLEN)
+                        print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
+
+            if VERBOSE_LEVEL in [1, 2]:
+                _message = 'PYSEx output catalog contains [%d] sources!' %(len(AstSEx))
+                print('MeLOn CheckPoint [%s]: %s' %(objname, _message))
 
             # ** g. ADD-COLUMN Stamp
-            if StampImgSize is not None:
+            if STAMP_IMGSIZE is not None:
                 _XY = np.array([AstSEx['X_IMAGE'], AstSEx['Y_IMAGE']]).T
-                PixA_StpLst = Stamp_Generator.SG(FITS_obj=FITS_obj, StampImgSize=StampImgSize, \
-                    Coordinates=_XY, CoorType='Image', AutoFill='NaN', MDIR=None)[0]
+                PixA_StpLst = Stamp_Generator.SG(FITS_obj=FITS_obj, EXTINDEX=0, \
+                    COORD=_XY, COORD_TYPE='IMAGE', STAMP_IMGSIZE=STAMP_IMGSIZE, \
+                    FILL_VALUE=np.nan, FITS_StpLst=None, VERBOSE_LEVEL=VERBOSE_LEVEL)
                 AstSEx.add_column(Column(PixA_StpLst, name='Stamp'))
                 Modify_AstSEx = True
             
             # ** UPDATE the file FITS_SExCat
             if MDIR is not None and Modify_AstSEx:
+                tFITS_SExCat = ''.join([TDIR, '/TMPCAT_%s' %FNAME])
+                AstSEx.write(tFITS_SExCat, overwrite=True)
+
                 hdl = fits.open(FITS_SExCat)
-                FITS_tmp = ''.join([TDIR, '/TMP_SEX_%s' %FNAME])
-                AstSEx.write(FITS_tmp, overwrite=True)
-                hdl_tmp = fits.open(FITS_tmp)
-                if tbhdu == 2: 
-                    fits.HDUList([hdl[0], hdl[1], hdl_tmp[1]]).writeto(FITS_SExCat, overwrite=True)
-                if tbhdu == 1: 
-                    fits.HDUList([hdl[0], hdl_tmp[1]]).writeto(FITS_SExCat, overwrite=True)
+                thdl = fits.open(tFITS_SExCat)
+                if tbhdu == 2: fits.HDUList([hdl[0], hdl[1], thdl[1]]).writeto(FITS_SExCat, overwrite=True)
+                if tbhdu == 1: fits.HDUList([hdl[0], thdl[1]]).writeto(FITS_SExCat, overwrite=True)
                 hdl.close()
-                hdl_tmp.close()
-                os.system('rm %s' %FITS_tmp)
+                thdl.close()
+                os.system('rm %s' %tFITS_SExCat)
 
         # ** REMOVE temporary directory
         if MDIR is None: 
             os.system('rm -rf %s' %TDIR)
 
         return AstSEx, PixA_SExCheckLst, FITS_SExCat, FITS_SExCheckLst
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sfft-1.3.4/sfft/utils/pyAstroMatic/PYSWarp.py` & `sfft-1.4.0/sfft/utils/pyAstroMatic/PYSWarp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,191 +1,193 @@
 import os
-import sys
 import warnings
 import os.path as pa
 from astropy.io import fits
-from astropy.wcs import WCS
 from tempfile import mkdtemp
+from sfft.utils.ReadWCS import Read_WCS
 from sfft.utils.CombineHeader import Combine_Header
 from sfft.utils.pyAstroMatic.AMConfigMaker import AMConfig_Maker
-# version: Sep 27, 2022
+# version: Apr 7, 2023
 
 __author__ = "Lei Hu <hulei@pmo.ac.cn>"
-__version__ = "v1.3"
+__version__ = "v1.4"
 
 class PY_SWarp:
     @staticmethod
-    def PS(FITS_obj, FITS_ref, FITS_resamp=None, FITS_resamp_weight=None, \
-        GAIN_KEY='GAIN', SATUR_KEY='SATURATE', OVERSAMPLING=1, RESAMPLING_TYPE='LANCZOS3', \
-        SUBTRACT_BACK='N', FILL_VALUE=None, WEIGHT_SUFFIX='.weight.fits', WRITE_XML='N', VERBOSE_TYPE='NORMAL'):
-
+    def PS(FITS_obj, FITS_ref, FITS_resamp=None, GAIN_KEY='GAIN', SATUR_KEY='SATURATE', \
+        OVERSAMPLING=1, RESAMPLING_TYPE='LANCZOS3', SUBTRACT_BACK='N', FILL_VALUE=None, \
+        VERBOSE_TYPE='NORMAL', VERBOSE_LEVEL=2):
+        
         """
         # Inputs & Outputs:
 
         -FITS_obj []                        # FITS file path of the input image to be resampled
 
         -FITS_ref []                        # FITS file path of the input image as resampling reference
 
         -FITS_resamp [None]                 # FITS file path of the output image of resampled -FITS_obj
 
-        -FITS_resamp_weight [None]          # FITS file path of the output weight image for resampled -FITS_obj
-
         # SWarp parameters:
 
         -GAIN_KEY ['GAIN']                  # SWarp Parameter GAIN_KEYWORD
                                             # i.e., keyword of GAIN in FITS image header
 
         -SATUR_KEY ['SATURATE']             # SWarp Parameter SATLEV_KEYWORD
                                             # i.e., keyword of the saturation level in the FITS image header
 
         -OVERSAMPLING [1]                   # SWarp Parameter OVERSAMPLING
                                             # Oversampling in each dimension
                                             # (0 = automatic)
                                             # P.S. Here I changed the default value from 0 to 1
+                                            # NOTE: large OVERSAMPLING may cause higher pixel correlation
 
         -RESAMPLING_TYPE ['LANCZOS3']       # SWarp Parameter RESAMPLING_TYPE
                                             # NEAREST,BILINEAR,LANCZOS2,LANCZOS3
                                             # LANCZOS4 (1 per axis) or FLAGS
+                                            # NOTE: LANCZOS4 is relatively time-consuming
 
         -SUBTRACT_BACK ['N']                # SWarp Parameter SUBTRACT_BACK 
                                             # Subtraction sky background (Y/N)? (all or for each image)
                                             # P.S. Here I changed the default value from 'Y' to 'N'
-
-        -WEIGHT_SUFFIX ['.weight.fits']     # SWarp Parameter WEIGHT_SUFFIX
-                                            # Suffix to use for weight-maps
-                                            # Weightmap filename if suffix not used (all or for each weight-map)
-
-        -WRITE_XML ['N']                    # SWarp Parameter WRITE_XML
-                                            # Write XML file (Y/N)?
-                                            # P.S. Here I changed the default value from 'Y' to 'N'
                                        
         -VERBOSE_TYPE ['NORMAL']            # SWarp Parameter VERBOSE_TYPE
                                             # QUIET,LOG,NORMAL, or FULL
 
+        -VERBOSE_LEVEL [2]                  # The level of verbosity, can be [0, 1, 2]
+                                            # 0/1/2: QUIET/NORMAL/FULL mode
+                                            # NOTE: it only controls the verbosity out of SWarp.
+
         # Other parameters:
 
         -FILL_VALUE [None]                  # How to fill the invalid (boundary) pixels in -FITS_resamp and -FITS_resamp_weight
                                             # e.g., -FILL_VALUE = 0.0, -FILL_VALUE = np.nan
 
         # Returns:
 
             PixA_resamp                     # Pixel array of the resampled image
                                             # P.S. PixA_resamp = fits.getdata(FITS_resamp, ext=0).T
             
-            PixA_resamp_weight              # Pixel array of the weight image for resampled image
-                                            # P.S. PixA_resamp_weight = fits.getdata(FITS_resamp_weight, ext=0).T
-            
-            MISSING_MASK                    # Pixel array of the invalid pixels
-                                            # P.S. -FILL_VALUE will fill the pixels where MISSING_MASK is True  
+            MissingMask                    # Pixel array of the invalid pixels
+                                            # P.S. -FILL_VALUE will fill the pixels where MissingMask is True
         
-        # ---------------- MORE REMARKS ON PYSWarp ----------------  
+        # * Remarks on PYSWarp
+        #   [1] SWarp itself can perform resampling and subsequent image combination.
+        #       However, the current python wrapper PYSWarp only performs image resampling.
+        #     
+        #   [2] In SWarp, one need provide a target WCS-frame stored in fname.head, with name coincident with FITS_resamp.
+        #       If no target WCS-frame is available, the output image will have a canonical N-E orientation.
+        #       However, the current python wrapper PYSWarp must read a target WCS-frame from a given FITS_ref.
         #
-        #  a) PYSWarp Purpose
-        #     1. The current python version only implement Resampling of single SEF-FITS image.
-        #     2. Note SWarp can also do the simple combination procedure after Resampling.
+        #   [3] SWarp allows users to feed a corresponding weight map as input.
+        #       However, the current python wrapper PYSWarp does not support this feature.
         #
-        #  b) SWarp destination-frame
-        #     @ Default-NE Mode
-        #       The output WCS-frame simply use canonical N-E orientation, i.e., NE-WCS-Frame. 
-        #       NOTE this mode is not supported in our function.
-        #     @ Given-REF Mode
-        #       The output WCS-frame (including image size) is determined by the given FITS_ref, 
-        #       we ganna to prepare a .head file, coincident name with FITS_resamp, to store REF-WCS-Frame.
-        # 
-        #  c) SWarp resulting header 
-        #     a. SWarp will automatically calculate Maximum equivalent Gain (to GAIN) & Exposure (to EXPTIME)
-        #        with additional Saturation (SATURATE) value, into resulting product's header. 
-        #        However, they are trivial for our non-combination purpose.
-        #     b. In our function, the resulting product's header is constructed by removing 
-        #        wcs keywords in FITS_obj and adding those in FITS_ref. In additional, 
-        #        we will record the SWarp parameters used in the function.
-        #     c. SWarp will automatically record the processing time in resulting header.
-        #
-        #  d) Tips on resampling method -RESAMPLING_TYPE
-        #     NOTE: LANCZOS4 is relatively time-consuming
-        #     NOTE: large OVERSAMPLING may cause higher pixel correlation
+        #   [4] SWarp will automatically calculate the following keywords and set them into the output image.
+        #       > EXPTIME: sum of exposure times in the part of coadd with the most overlaps.
+        #       > GAIN: effective gain with flux and weighting applied.
+        #         Note that any change in pixel scale only redistribute the flux with total flux conservative,
+        #         therefore, the image resampling does not alter the GAIN value.
+        #       > SATURATE: Minimum of all input saturation levels with flux scaling applied.
+        #         Note that a change in pixel scale can alter the saturation level.
+        #       > MJD-OBS: MJD of earliest start of exposures 
+        #       
+        #       For PYSWarp which only performs image resampling:
+        #       > We can safely preserve EXPTIME, GAIN, MJD-OBS, and use SWarp output SATURATE value.
+        #       > The resulting header of the PYSWarp output is constructed by combining
+        #         FITS_obj header with WCS keywords removed & FITS_ref header only with WCS keywords
+        #         In additional, we will update SATURATE value as described above, and 
+        #         record the SWarp parameters used in the function.
         #
         """
 
-        # * Check Process for FITS_obj header
-        phr_obj = fits.getheader(FITS_obj, ext=0)        
+        # * check FITS_obj header
+        objname = pa.basename(FITS_obj)
+        phr_obj = fits.getheader(FITS_obj, ext=0)
         assert GAIN_KEY in phr_obj and SATUR_KEY in phr_obj
-        if 'EXPTIME' not in phr_obj:
-            warnings.warn('MeLOn WARNING: SWarp does not find EXPTIME in header at [%s]' %(pa.basename(FITS_obj)))
-        if 'MJD-OBS' not in phr_obj:
-            warnings.warn('MeLOn WARNING: SWarp does not find MJD-OBS in header at [%s]' %(pa.basename(FITS_obj)))
 
-        # * Make Directory as workplace of PYSwarp operation
+        # a mild warning
+        if VERBOSE_LEVEL in [1, 2]:
+            if 'EXPTIME' not in phr_obj:
+                _warn_message = 'SWarp cannot find keyword EXPTIME in FITS header of [%s]!' %objname
+                warnings.warn('MeLOn WARNING: %s' %_warn_message)
+        
+        # a mild warning
+        if VERBOSE_LEVEL in [1, 2]:
+            if 'MJD-OBS' not in phr_obj:
+                _warn_message = 'SWarp cannot find keyword MJD-OBS in FITS header of [%s]!' %objname
+                warnings.warn('MeLOn WARNING: %s' %_warn_message)
+
+        # * make directory as a workplace
         TDIR = mkdtemp(suffix=None, prefix='PYSWarp_', dir=None)
 
-        # * Make Swarp configuration file in TDIR.
+        # * create SWarp configuration file in TDIR
         ConfigDict = {}
         ConfigDict['GAIN_KEYWORD'] = '%s' %GAIN_KEY
         ConfigDict['SATLEV_KEYWORD'] = '%s' %SATUR_KEY
 
         ConfigDict['OVERSAMPLING'] = '%d' %OVERSAMPLING
         ConfigDict['RESAMPLING_TYPE'] = '%s' %RESAMPLING_TYPE
         ConfigDict['SUBTRACT_BACK'] = '%s' %SUBTRACT_BACK
-        ConfigDict['COMBINE_TYPE'] = 'MEDIAN'  # trivial here
 
-        ConfigDict['WEIGHT_SUFFIX'] = '%s' %WEIGHT_SUFFIX
-        ConfigDict['WRITE_XML'] = '%s' %WRITE_XML
+        ConfigDict['COMBINE'] = 'Y'  # trivial here
+        ConfigDict['COMBINE_TYPE'] = 'MEDIAN'  # trivial here
+        
+        ConfigDict['WEIGHT_SUFFIX'] = '.weight.fits'  # trivial here
+        ConfigDict['WRITE_XML'] = 'N'
         ConfigDict['VERBOSE_TYPE'] = '%s' %VERBOSE_TYPE
         
-        swarpconfig_path = AMConfig_Maker.AMCM(MDIR=TDIR, \
+        swarp_config_path = AMConfig_Maker.AMCM(MDIR=TDIR, \
             AstroMatic_KEY='swarp', ConfigDict=ConfigDict, tag='PYSWarp')
 
-        # * Make temporary FITS_resamp & FIT_resamp_weight in TDIR
+        # * make temporary FITS_resamp & FIT_resamp_weight in TDIR
         tFITS_resamp = TDIR + '/%s.tmp_resamp.fits' %pa.basename(FITS_obj)[:-5]
         tFITS_resamp_weight = TDIR + '/%s.tmp_resamp_weight.fits' %pa.basename(FITS_obj)[:-5]
 
-        # * Build .head file from FITS_ref
+        # * build .head file from FITS_ref
         phr_ref = fits.getheader(FITS_ref, ext=0)
-        w_ref = WCS(phr_ref)            
+        w_ref = Read_WCS.RW(phr_ref, VERBOSE_LEVEL=VERBOSE_LEVEL)
         _headfile = tFITS_resamp[:-5] + '.head'
         wcshdr_ref = w_ref.to_header(relax=True)   # SIP distorsion requires relax=True
 
         wcshdr_ref['BITPIX'] = phr_ref['BITPIX']
-        wcshdr_ref['NAXIS'] = phr_ref['NAXIS']            
+        wcshdr_ref['NAXIS'] = phr_ref['NAXIS']
         wcshdr_ref['NAXIS1'] = phr_ref['NAXIS1']
         wcshdr_ref['NAXIS2'] = phr_ref['NAXIS2']
         wcshdr_ref.tofile(_headfile)
 
-        # * Trigger SWarp 
+        # * trigger SWarp 
         os.system('cd %s && swarp %s -IMAGEOUT_NAME %s -WEIGHTOUT_NAME %s -c %s' \
-            %(TDIR, FITS_obj, tFITS_resamp, tFITS_resamp_weight, swarpconfig_path))
-
-        # * Make a combined header for resulting products
-        hdr_base = fits.getheader(FITS_obj, ext=0)
-        hdr_wcs = fits.getheader(FITS_ref, ext=0)
-        hdr_op = Combine_Header.CH(hdr_base=hdr_base, hdr_wcs=hdr_wcs)
+            %(TDIR, FITS_obj, tFITS_resamp, tFITS_resamp_weight, swarp_config_path))
+        
+        # * make a combined header for output FITS
+        hdr_op = Combine_Header.CH(hdr_base=phr_obj, hdr_wcs=phr_ref, VERBOSE_LEVEL=VERBOSE_LEVEL)
+        
+        # * update header by the SWarp generated saturation level
+        NEW_SATUR = fits.getheader(tFITS_resamp, ext=0)['SATURATE']
+        hdr_op[SATUR_KEY] = (NEW_SATUR, 'MeLOn: PYSWarp')
 
+        # * add history
         hdr_op['SWARP_O'] = (pa.basename(FITS_obj), 'MeLOn: PYSWarp')
         hdr_op['SWARP_R'] = (pa.basename(FITS_ref), 'MeLOn: PYSWarp')
-
         for key in ConfigDict:
             value = ConfigDict[key]
-            pack = ' : '.join(['SWarp Parameters', key, value])
+            pack = ' : '.join(['SWarp Parameter', key, value])
             hdr_op.add_history(pack)
 
-        # * Fill the missing data in resampled image [SWarp default 0]
-        PixA_resamp, PixA_resamp_weight = None, None
-        MISSING_MASK = None
+        # * fill the missing data in resampled image [SWarp default 0]
+        PixA_resamp, MissingMask = None, None
         try: 
             PixA_resamp = fits.getdata(tFITS_resamp, ext=0).T
             PixA_resamp_weight = fits.getdata(tFITS_resamp_weight, ext=0).T
-            MISSING_MASK = PixA_resamp_weight == 0
-
+            MissingMask = PixA_resamp_weight == 0
             if FILL_VALUE is not None:
-                PixA_resamp[MISSING_MASK] = FILL_VALUE
+                PixA_resamp[MissingMask] = FILL_VALUE
             if FITS_resamp is not None:
                 hdl_op = fits.HDUList(fits.PrimaryHDU(PixA_resamp.T, header=hdr_op))
                 hdl_op.writeto(FITS_resamp, overwrite=True)
-            if FITS_resamp_weight is not None:
-                hdl_op = fits.HDUList(fits.PrimaryHDU(PixA_resamp_weight.T, header=hdr_op))
-                hdl_op.writeto(FITS_resamp_weight, overwrite=True)
+        except:
+            if VERBOSE_LEVEL in [0, 1, 2]:
+                _warn_message = 'SWarp FAILED on [%s]!' %objname
+                warnings.warn('MeLOn WARNING: %s' %_warn_message)
         
-        except: 
-            warnings.warn('MeLOn WARNING: SWarp FAILS at [%s]' %(pa.basename(FITS_obj)))
         os.system('rm -rf %s'%TDIR)
 
-        return PixA_resamp, PixA_resamp_weight, MISSING_MASK
+        return PixA_resamp, MissingMask
```

### Comparing `sfft-1.3.4/sfft.egg-info/PKG-INFO` & `sfft-1.4.0/sfft.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,219 +1,232 @@
 Metadata-Version: 2.1
 Name: sfft
-Version: 1.3.4
+Version: 1.4.0
 Summary: Image Subtraction in Fourier Space
-Home-page: UNKNOWN
+Download-URL: https://github.com/thomasvrussell/sfft
 Author: Lei Hu
 Author-email: hulei@pmo.ac.cn
 Maintainer: Lei Hu
 Maintainer-email: hulei@pmo.ac.cn
 License: MIT Licence
-Download-URL: https://github.com/thomasvrussell/sfft
-Description: ..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_logo_gwbkg.png
-        
-        Package Description
-        -------------------
-        
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6576426.svg
-           :target: https://doi.org/10.5281/zenodo.6576426
-        .. image:: https://img.shields.io/pypi/v/sfft.svg
-            :target: https://pypi.python.org/pypi/sfft
-            :alt: Latest Version
-        .. image:: https://static.pepy.tech/personalized-badge/sfft?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads
-         :target: https://pepy.tech/project/sfft
-        .. image:: https://static.pepy.tech/personalized-badge/sfft?period=month&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads/month
-            :target: https://pepy.tech/project/sfft
-        .. image:: https://img.shields.io/badge/python-3.7-green.svg
-            :target: https://www.python.org/downloads/release/python-370/
-        .. image:: https://img.shields.io/badge/License-MIT-blue.svg
-            :target: https://opensource.org/licenses/MIT
-        |
-        Saccadic Fast Fourier Transform (SFFT) is an algorithm for image subtraction in Fourier space. SFFT brings about a remarkable improvement of computational performance of around an order of magnitude compared to other published image subtraction codes. 
-        
-        ..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_subtract_speed.png
-        
-        To get a clear picture of our method, we summarize a variety of features from different perspectives for SFFT and other existing image subtraction methods.
-        
-        ..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_features.png
-        
-        Installation
-        -----------
-        One can install the latest stable version of sfft from pip (recommended): ::
-            
-            pip install sfft
-        
-        Or alternatively, install any desired version of sfft from Github `<https://github.com/thomasvrussell/sfft>`_: ::
-        
-            python setup.py install
-        
-        sfft has the following three backends to perform the image subtraction.
-        
-        .. [#] **NumPy backend** : sfft will totally run on the CPU devices. NO GPU devices and CUDA dependencies are required for this backend.
-        .. [#] **PyCUDA backend** : The core functions of sfft are written in `PyCUDA <https://github.com/inducer/pycuda>`_ and `Scikit-Cuda <https://github.com/lebedov/scikit-cuda>`_. Users need to install PyCUDA and Scikit-Cuda according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
-        .. [#] **CuPy backend** : The core functions of sfft are written in `CuPy <https://github.com/cupy/cupy>`_. Users need to install CuPy according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
-        
-        - CUDA 11: E.g, you may enable the CuPy backend for CUDA 11.5 via: ::
-        
-            pip install cupy-cuda115  # CuPy backend
-        
-        - CUDA 10: E.g, you may enable the GPU backends (i.e., PyCUDA backend and CuPy backend) for CUDA 10.1 via: ::
-        
-            pip install pycuda==2020.1 scikit-cuda==0.5.3  # PyCUDA backend
-            pip install cupy-cuda101                       # CuPy backend
-                           
-        **Additional Remarks**: CuPy backend is faster than PyCUDA backend, while it consumes more GPU memory. Generally, I strongly recommend users to adopt CuPy backend as long as it does not incur GPU out-of-memory issue. Note that PyCUDA backend is still not compatiable with CUDA 11.
-        
-        Dependencies
-        -----------
-        
-        You need further to install additional astronomical software for sfft.
-        
-        - `SExtractor <https://github.com/astromatic/sextractor>`_: SExtractor is required for sfft preprocessing, as it enables sfft to determine a proper pixel mask over the input image-pair before the image subtraction (this is critical for a more reasonable parameter-solving). Note that we have wrapped SExtractor into a Python module ``sfft.utils.pyAstroMatic.PYSEx`` so that one can trigger SExtractor within Python (please type help(``sfft.utils.pyAstroMatic.PYSEx``) to find its usage). As an AstrOmatic software, you can install SExtractor following `<https://www.astromatic.net/software/sextractor/>`_, or alternatively, install via conda: ::
-        
-            conda install -c conda-forge astromatic-source-extractor
-        
-        - `SWarp <https://github.com/astromatic/swarp>`_ (optional): This is not required for sfft subtraction itself. However, it is normally necessary to align the input image-pair before image subtraction. We have additionally wrapped SWarp into a Python module ``sfft.utils.pyAstroMatic.PYSWarp`` so that you can align images in a more Pythonic way (please type help(``sfft.utils.pyAstroMatic.PYSWarp``) to find its usage). As an AstrOmatic software, you can install SWarp following `<https://www.astromatic.net/software/swarp/>`_, or alternatively, install via conda: ::
-        
-            conda install -c conda-forge astromatic-swarp
-        
-        Quick start guide
-        -----------
-        We have prepared several examples in the test directory so that you can familar with the usage of the main functions in our software:
-        
-        .. [*] **sfft subtraction for crowded field** : The example in subdirectory named subtract_test_crowded_flavor. We use crowded-flavor-sfft (module ``sfft.EasyCrowdedPacket``) to perform image subtraction for ZTF M31 observations. More detailed explanations of this module, see help(``sfft.EasyCrowdedPacket``).
-        
-        .. [*] **sfft subtraction for sparse field** : The example in subdirectory named subtract_test_sparse_flavor. We use sparse-flavor-sfft (module ``sfft.EasySparsePacket``) to perform image subtraction for CTIO-4m DECam observations. More detailed explanations of this module, see help(``sfft.EasySparsePacket``).
-        
-        - **IMPORTANT NOTICE: the input images of sparse-flavor-sfft should be SKY-SUBTRACTED!** One can make use of SExtractor to subtract the sky background, which has been also wrapped in this package, please use the module ``sfft.utils.SExSkySubtract`` and type help(``sfft.utils.SExSkySubtract``) to find its usage. There is an additional example in subtract_test_sparse_flavor (see directory prepare_data_example), that shows how to prepare the input image pair for sparse-flavor-sfft by ``sfft.utils.SExSkySubtract`` for sky subtraction and ``sfft.utils.pyAstroMatic.PYSWarp`` for image alignment, respecitvely.
-        
-        - Our software provides two flavors for image subtraction, crowded-flavor-sfft and sparse-flavor-sfft, to accommodate the situations for the crowded and sparse fields, respectively. The two flavors actually follow the same routine for image subtraction and differ only in ways of masking the data. 
-        
-        - Proper image-masking is required in the current version of SFFT to identify the pixels that are not correctly modeled by SFFT (hereafter, distraction pixels), e.g., saturated sources, casual cosmic rays and moving objects, bad CCD pixels, optical ghosts, and even the variable objects and transients themselves. The pre-subtraction processing for image-masking is referred to as **preprocessing** in sfft.
-        
-        - Our software provides a generic and robust function to perform **preprocessing** of the data, which has been extensively tested with data from various transient surveys. When you run crowded-flavor-sfft and sparse-flavor-sfft, sfft actually performs the generic **preprocessing** for image-masking and do the sfft subtraction subsequently. 
-        
-        - More specificially, the built-in preprocessing in sfft consists of two steps: [1] identify the distraction pixels in the input image-pair [2] create the masked version of the input image-pair via replacing the identified distraction pixels by proper flux values. In sparse-flavor-sfft, we designed a source-selection based on SExtractor catalogs and identify the unselected regions as distraction pixels. Given that the input images are required to be sky-subtracted in sparse-flavor-sfft, we simply replace the distraction pixels by zeros; In crowded-flavor-sfft, we only identify the pixels contaminated by saturated sources as distraction pixels using SExtractor, and then replace the distraction pixels by local background flux. 
-        
-        Customized usage
-        -----------
-        
-        The built-in **preprocessing** in sfft (based on SExtractor) is only designed to provide a safe and generic approach which can adapt to diverse imaging data. In contrast to the high speed of the image subtraction, the computing performance of the built-in **preprocessing** is much less remarkable (says, 10 times more computing time). Given a particular time-domain program, we do believe there is plenty of room for further optimization of the computing expense on the **preprocessing**. The two suggestions below might be helpful for users who would like to incorporate sfft in their pipeline efficiently:
-        
-        - For sparse-flavor-sfft, the built-in **preprocessing** performs a source-selection based on SExtractor catalogs and then create the masked images for subsequent subtraction. To optimize the overall computing expense of the pipeline, one can make use of the SExtractor products already generated in the preceding modules (e.g., astrometric calibration) for the source-selection (which is much faster than SExtractor) of sfft. It will avoid repeated SExtractor photometry and reduce computing time significantly.
-        
-        - For crowded-flavor-sfft, the built-in **preprocessing** only mask the saturation-contaminated pixels using SExtractor. When data quality masks for the observed imaging data are available in a survey program, one can instead identify the invalid pixels using the data quality masks and mask them by local background. Hence, the built-in **preprocessing** can be totally skipped.
-        
-        Besides, we encourage users to design dedicated image-masking strategies for their survey programs to unleash the great power of sfft subtraction!
-        
-        Our software provides a customized module which allows users to feed their own image-masking results, i.e., the module only perform the sfft subtraction. In this test, you would see the lightning fast speed of sfft subtraction on GPU devices!
-        
-        .. [*] **customized sfft subtraction** : The example in subdirectory named subtract_test_customized. The test data is the same as those for crowded-flavor-sfft (ZTF-M31 observations), however, the built-in automatic image-masking has been skipped by using given customized masked images as inputs. Such *pure* version of sfft is conducted by the module ``sfft.CustomizedPacket``. More detailed explanations of the module: help(``sfft.CustomizedPacket``).
-        
-        **Additional Remarks**: If you are using GPU backends and you have a queue of observations to be processed, the first time in the loop of sfft subtraction can be very slow, and runtime is going to be stable after the first time. This might be due to some unknown initialization process in GPU devices. You can find in above test that the GPU warming-up is quite slow. Fortunately, this problem can be esaily solved by running a trivial subtraction (e.g., on empty images) in advance and making the pipe waiting for the subsequent observations (see above test).
-        
-        Parallel Computing
-        -----------
-        
-        We have also developed modules to optimize the overall computing performance of sparse-flavor-sfft and crowded-flavor-sfft for the cases when you need to deal with multiple tasks simultaneously.
-        
-        - In a particular time-domain survey, one may need to process a large set of image-pairs simultaneously. Assume that you have Nt tasks which should be processed by a computing platform with Nc CPU threads and Ng GPU devices. Generally, Nt >> Ng and Nc >> Ng. 
-        
-            E.g., Nt = 61 (A DECam exposure with CCDs), Nc = 40 (A CPU with 40 threads), and Ng = 1 (A Tesla A100 available).
-        
-        - Note that we generally need to avoid multiple tasks using one GPU at the same time (GPU out-of-memory issue). That is to say, we CANNOT simply trigger a set of sfft functions (e.g., ``sfft.EasySparsePacket``) to process a large set of image-pairs simultaneously.
-        
-        - Since version 1.1, sfft has allowed for multiple tasks without conflicting GPU usage, by using the modules ``sfft.MultiEasySparsePacket`` for sparse-flavor-sfft and ``sfft.MultiEasyCrowdedPacket`` for crowded-flavor-sfft, respectively. Please see the directory test/subtract_test_multiprocessing to find the examples. Note that ONLY the CuPy backend is supported in multiprocessing mode.
-        
-        Remarks on the direction of image subtraction
-        -----------
-        
-        There is a universal argument named -ForceConv to control the direction of image subtraction, which works on all image subtraction modules in sfft.
-        
-        - 'AUTO' means sfft will determine the direction of image subtraction automatically according to the estimated FWHM of reference image and science image. The image which has smaller FWHM will be convolved in the image subtraction to avoid deconvolution. After comparing the FWHM, 'AUTO' becomes 'REF' or 'SCI' (see below). One can get to know which image is eventually convolved in image subtraction from the primary header of the difference image (see the keyword 'CONVD'). This mode does not supported in the Customized module ``sfft.CustomizedPacket``.
-        
-        - 'REF' means sfft will convolve the reference image and DIFF = SCI - Convolved_REF. As a result, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the science image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the science image: using the same psf model / aperture and magnitude zeropoint.
-        
-        - 'SCI' means sfft will convolve the reference image and DIFF = Convolved_SCI - REF. Consequently, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the reference image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the reference image: using the same psf model / aperture and magnitude zeropoint (but of course, not including the observation date!).
-        
-        Note that a transient on science image is always a positive signal on difference image whatever -ForceConv is.
-        
-        Additional Function
-        -----------
-        
-        We also present a decorrelation module to whiten the background noise of the difference image.
-        
-        .. [*] **difference noise decorrelation** : The example in subdirectory named difference_noise_decorrelation. We use noise-decorrelation toolkit (module ``sfft.utils.DeCorrelationCalculator``) to whiten the background noise on difference image. In this test, the difference image is generated from image subtraction (by sfft) between a coadded reference image and a coadded science image, each stacked from 5 DECam individual observations with PSF homogenization (by sfft). The toolkit can be also applied to whiten a coadded image as long as convolution is involved in the stacking process.
-        
-        
-        Comments on Backward Compatiablity
-        -----------
-        
-        We have tried our best to ensure the backward compatiablity, however, the rule was sometimes overrided in the development of sfft, e.g., some arguments might be deprecated in higher version of sfft. Users might get errors when they use old scripts but update sfft to a higher version. To solve the problem, I have been maintaining the test scripts on Github to make sure they can always work for the lastest version of sfft. You can also find the change log of arguments in the test scripts. 
-        
-        What's new
-        -----------
-        
-        - The preprocessing in sparse-flavor-sfft is refined using an additional rejection of mild varaibles since version 1.3.0. [Lei, Aug 19, 2022]
-        
-        - The sfft is now optimized for multiple tasks since version 1.1.0. [Lei, May 24, 2022]
-        
-        - A few argument-names have been changed since version 1.1.0, please see the test scripts. [Lei, May 24, 2022]
-        
-        - Locking file is removed since version 1.1.0, as I found it unreliable in our tests, i.e., -GLockFile is removed. [Lei, May 24, 2022]
-        
-        - The trial subtraction for refinement is removed since version 1.1.0. However, I add a post-subtraction check to search anomalies on the difference image using the same logic. One can feed the coordinates of the anomalies to sfft again as Prior-Banned sources to refine the subtraction (see -XY_PriorBan in ``sfft.MultiEasySparsePacket``). [Lei, May 24, 2022]
-        
-        Todo list
-        -----------
-        
-        - Incorporate the separate functions (in the folder beta4spline) for spline form sfft into the unified sfft functions. Note that only Numpy backend is currently available and the spline form is very memory-consuming. [Lei, July 6, 2022]
-        
-        - Write a detailed documentation for sfft! [Lei, May 24, 2022]
-        
-        - We notice that SExtractor may have been called to perform astrometric calibration before image subtraction. It is definitely not wise to run SExtractor again in sfft, I need to develop a module which allows users to feed SExtractor products as inputs of sfft, which will significantly reduce the preprocessing time in sfft. [Lei, May 24, 2022]
-        
-        - The multiprocessing mode is expected to accomondate multiple GPU devices, however, the function has not tested on such a multi-GPUs platform. [Lei, May 24, 2022]
-        
-        - Add a function for optimizing sfft on a given computing platform with multiple CPU threading and one/multiple GPU card(s). This would be very useful to reduce the overall time cost when users have a large set of image-pairs to be processed simultaneously (e.g., serve for DECam, each exposure produces 61 CCD images). [Lei, May 20, 2022] **[ALREADY DONE]**
-        
-        Common issues
-        -----------
-        
-        - If your Python environment already has some version of llvmlite (a package required by NumPy backend) before installing sfft. The setup.py in sfft cannot properly update llvmlite to the desired version, then you may get errors related to Numba or llvmlite. If so, please manually install llvmlite by: ::
-        
-            pip install llvmlite==0.36.0 --ignore-installed
-        
-        Development
-        -----------
-        The latest source code can be obtained from
-        `<https://github.com/thomasvrussell/sfft>`_.
-        
-        When submitting bug reports or questions via the `issue tracker 
-        <https://github.com/thomasvrussell/sfft/issues>`_, please include the following 
-        information:
-        
-        - OS platform.
-        - Python version.
-        - CUDA, PyCUDA and CuPy version.
-        - Version of sfft.
-        
-        Citing
-        ------
-        
-        *Image Subtraction in Fourier Space. Hu, L., Wang, L., Chen, X., & Yang, J. 2022, The Astrophysical Journal, 936, 157*
-        
-        Arxiv link: `<https://arxiv.org/abs/2109.09334>`_.
-        
-        ApJ Publication link: `<https://doi.org/10.3847/1538-4357/ac7394>`_.
-        
-        Related DOI: 10.3847/1538-4357/ac7394
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_logo_gwbkg.png
+
+Package Description
+-------------------
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.6576426.svg
+   :target: https://doi.org/10.5281/zenodo.6576426
+.. image:: https://img.shields.io/pypi/v/sfft.svg
+    :target: https://pypi.python.org/pypi/sfft
+    :alt: Latest Version
+.. image:: https://static.pepy.tech/personalized-badge/sfft?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads
+ :target: https://pepy.tech/project/sfft
+.. image:: https://static.pepy.tech/personalized-badge/sfft?period=month&units=international_system&left_color=grey&right_color=yellow&left_text=Downloads/month
+    :target: https://pepy.tech/project/sfft
+.. image:: https://img.shields.io/badge/python-3.7-green.svg
+    :target: https://www.python.org/downloads/release/python-370/
+.. image:: https://img.shields.io/badge/License-MIT-blue.svg
+    :target: https://opensource.org/licenses/MIT
+|
+Saccadic Fast Fourier Transform (SFFT) is an algorithm for image subtraction in Fourier space. SFFT brings about a remarkable improvement of computational performance of around an order of magnitude compared to other published image subtraction codes. 
+
+..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_subtract_speed.png
+
+To get a clear picture of our method, we summarize a variety of features from different perspectives for SFFT and other existing image subtraction methods.
+
+..  image:: https://github.com/thomasvrussell/sfft/blob/master/docs/sfft_features.png
+
+Installation
+-----------
+One can install the latest stable version of sfft from pip (recommended): ::
+    
+    pip install sfft
+
+Or alternatively, install any desired version of sfft from Github `<https://github.com/thomasvrussell/sfft>`_: ::
+
+    python setup.py install
+
+sfft now has the following two backends to perform the image subtraction.
+
+.. [#] **CuPy backend** : The core functions of sfft are written in `CuPy <https://github.com/cupy/cupy>`_. Users need to install CuPy according to their CUDA version to enable this backend. Note this backend require GPU device(s) with double-precision support.
+.. [#] **NumPy backend** : sfft will totally run on the CPU devices. NO GPU devices and CUDA dependencies are required for this backend.
+
+- CUDA 12: E.g, you may enable the CuPy backend for CUDA 12.0 via: ::
+
+    pip install cupy-cuda12x
+
+- CUDA 11: E.g, you may enable the CuPy backend for CUDA 11.5 via: ::
+
+    pip install cupy-cuda115
+
+- CUDA 10: E.g, you may enable the CuPy backend for CUDA 10.1 via: ::
+
+    pip install cupy-cuda101
+
+**Additional Remarks**: There was a PyCUDA backend in sfft but now deprecated since v1.4.0. For sfft < v1.4.0, PyCUDA backend was preserved as it consumes less GPU memory. However, the CuPy backend is now better implemented for GPU memory allocation, making the PyCUDA backend no longer useful.
+
+Dependencies
+-----------
+
+You need further to install additional astronomical software for sfft.
+
+- `SExtractor <https://github.com/astromatic/sextractor>`_: SExtractor is required for sfft preprocessing, as it enables sfft to determine a proper pixel mask over the input image-pair before the image subtraction (this is critical for a more reasonable parameter-solving). Note that we have wrapped SExtractor into a Python module ``sfft.utils.pyAstroMatic.PYSEx`` so that one can trigger SExtractor within Python (please type help(``sfft.utils.pyAstroMatic.PYSEx``) to find its usage). As an AstrOmatic software, you can install SExtractor following `<https://www.astromatic.net/software/sextractor/>`_, or alternatively, install via conda: ::
+
+    conda install -c conda-forge astromatic-source-extractor
+
+- `SWarp <https://github.com/astromatic/swarp>`_ (optional): This is not required for sfft subtraction itself. However, it is normally necessary to align the input image-pair before image subtraction. We have additionally wrapped SWarp into a Python module ``sfft.utils.pyAstroMatic.PYSWarp`` so that you can align images in a more Pythonic way (please type help(``sfft.utils.pyAstroMatic.PYSWarp``) to find its usage). As an AstrOmatic software, you can install SWarp following `<https://www.astromatic.net/software/swarp/>`_, or alternatively, install via conda: ::
+
+    conda install -c conda-forge astromatic-swarp
+
+Quick start guide
+-----------
+We have prepared several examples in the test directory so that you can familar with the usage of the main functions in our software:
+
+.. [*] **sfft subtraction for crowded field** : The example in subdirectory named subtract_test_crowded_flavor. We use crowded-flavor-sfft (module ``sfft.EasyCrowdedPacket``) to perform image subtraction for ZTF M31 observations. More detailed explanations of this module, see help(``sfft.EasyCrowdedPacket``).
+
+.. [*] **sfft subtraction for sparse field** : The example in subdirectory named subtract_test_sparse_flavor. We use sparse-flavor-sfft (module ``sfft.EasySparsePacket``) to perform image subtraction for CTIO-4m DECam observations. More detailed explanations of this module, see help(``sfft.EasySparsePacket``).
+
+- **IMPORTANT NOTICE: the input images of sparse-flavor-sfft should be SKY-SUBTRACTED!** One can make use of SExtractor to subtract the sky background, which has been also wrapped in this package, please use the module ``sfft.utils.SExSkySubtract`` and type help(``sfft.utils.SExSkySubtract``) to find its usage. There is an additional example in subtract_test_sparse_flavor (see directory prepare_data_example), that shows how to prepare the input image pair for sparse-flavor-sfft by ``sfft.utils.SExSkySubtract`` for sky subtraction and ``sfft.utils.pyAstroMatic.PYSWarp`` for image alignment, respecitvely.
+
+- Our software provides two flavors for image subtraction, crowded-flavor-sfft and sparse-flavor-sfft, to accommodate the situations for the crowded and sparse fields, respectively. The two flavors actually follow the same routine for image subtraction and differ only in ways of masking the data. 
+
+- Proper image-masking is required in the current version of SFFT to identify the pixels that are not correctly modeled by SFFT (hereafter, distraction pixels), e.g., saturated sources, casual cosmic rays and moving objects, bad CCD pixels, optical ghosts, and even the variable objects and transients themselves. The pre-subtraction processing for image-masking is referred to as **preprocessing** in sfft.
+
+- Our software provides a generic and robust function to perform **preprocessing** of the data, which has been extensively tested with data from various transient surveys. When you run crowded-flavor-sfft and sparse-flavor-sfft, sfft actually performs the generic **preprocessing** for image-masking and do the sfft subtraction subsequently. 
+
+- More specificially, the built-in preprocessing in sfft consists of two steps: [1] identify the distraction pixels in the input image-pair [2] create the masked version of the input image-pair via replacing the identified distraction pixels by proper flux values. In sparse-flavor-sfft, we designed a source-selection based on SExtractor catalogs and identify the unselected regions as distraction pixels. Given that the input images are required to be sky-subtracted in sparse-flavor-sfft, we simply replace the distraction pixels by zeros; In crowded-flavor-sfft, we only identify the pixels contaminated by saturated sources as distraction pixels using SExtractor, and then replace the distraction pixels by local background flux. 
+
+Customized usage
+-----------
+
+The built-in **preprocessing** in sfft (based on SExtractor) is only designed to provide a safe and generic approach which can adapt to diverse imaging data. In contrast to the high speed of the image subtraction, the computing performance of the built-in **preprocessing** is much less remarkable (says, 10 times more computing time). Given a particular time-domain program, we do believe there is plenty of room for further optimization of the computing expense on the **preprocessing**. The two suggestions below might be helpful for users who would like to incorporate sfft in their pipeline efficiently:
+
+- For sparse-flavor-sfft, the built-in **preprocessing** performs a source-selection based on SExtractor catalogs and then create the masked images for subsequent subtraction. To optimize the overall computing expense of the pipeline, one can make use of the SExtractor products already generated in the preceding modules (e.g., astrometric calibration) for the source-selection (which is much faster than SExtractor) of sfft. It will avoid repeated SExtractor photometry and reduce computing time significantly.
+
+- For crowded-flavor-sfft, the built-in **preprocessing** only mask the saturation-contaminated pixels using SExtractor. When data quality masks for the observed imaging data are available in a survey program, one can instead identify the invalid pixels using the data quality masks and mask them by local background. Hence, the built-in **preprocessing** can be totally skipped.
+
+Besides, we encourage users to design dedicated image-masking strategies for their survey programs to unleash the great power of sfft subtraction!
+
+Our software provides a customized module which allows users to feed their own image-masking results, i.e., the module only perform the sfft subtraction. In this test, you would see the lightning fast speed of sfft subtraction on GPU devices!
+
+.. [*] **customized sfft subtraction** : The example in subdirectory named subtract_test_customized. The test data is the same as those for crowded-flavor-sfft (ZTF-M31 observations), however, the built-in automatic image-masking has been skipped by using given customized masked images as inputs. Such *pure* version of sfft is conducted by the module ``sfft.CustomizedPacket``. More detailed explanations of the module: help(``sfft.CustomizedPacket``).
+
+**Additional Remarks**: If you are using GPU backends and you have a queue of observations to be processed, the first time in the loop of sfft subtraction can be very slow, and runtime is going to be stable after the first time. This might be due to some unknown initialization process in GPU devices. You can find in above test that the GPU warming-up is quite slow. Fortunately, this problem can be esaily solved by running a trivial subtraction (e.g., on empty images) in advance and making the pipe waiting for the subsequent observations (see above test).
+
+Parallel Computing
+-----------
+
+We have also developed modules to optimize the overall computing performance of sparse-flavor-sfft and crowded-flavor-sfft for the cases when you need to deal with multiple tasks simultaneously.
+
+- In a particular time-domain survey, one may need to process a large set of image-pairs simultaneously. Assume that you have Nt tasks which should be processed by a computing platform with Nc CPU threads and Ng GPU devices. Generally, Nt >> Ng and Nc >> Ng. 
+
+    E.g., Nt = 61 (A DECam exposure with CCDs), Nc = 40 (A CPU with 40 threads), and Ng = 1 (A Tesla A100 available).
+
+- Note that we generally need to avoid multiple tasks using one GPU at the same time (GPU out-of-memory issue). That is to say, we CANNOT simply trigger a set of sfft functions (e.g., ``sfft.EasySparsePacket``) to process a large set of image-pairs simultaneously.
+
+- Since version 1.1, sfft has allowed for multiple tasks without conflicting GPU usage, by using the modules ``sfft.MultiEasySparsePacket`` for sparse-flavor-sfft and ``sfft.MultiEasyCrowdedPacket`` for crowded-flavor-sfft, respectively. Please see the directory test/subtract_test_multiprocessing to find the examples. Note that ONLY the CuPy backend is supported in multiprocessing mode.
+
+Remarks on the direction of image subtraction
+-----------
+
+There is a universal argument named -ForceConv to control the direction of image subtraction, which works on all image subtraction modules in sfft.
+
+- 'AUTO' means sfft will determine the direction of image subtraction automatically according to the estimated FWHM of reference image and science image. The image which has smaller FWHM will be convolved in the image subtraction to avoid deconvolution. After comparing the FWHM, 'AUTO' becomes 'REF' or 'SCI' (see below). One can get to know which image is eventually convolved in image subtraction from the primary header of the difference image (see the keyword 'CONVD'). This mode does not supported in the Customized module ``sfft.CustomizedPacket``.
+
+- 'REF' means sfft will convolve the reference image and DIFF = SCI - Convolved_REF. As a result, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the science image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the science image: using the same psf model / aperture and magnitude zeropoint.
+
+- 'SCI' means sfft will convolve the reference image and DIFF = Convolved_SCI - REF. Consequently, the psf and flux zero-point of difference image is consistent with the unconvolved image, i.e., the reference image. One can perform PSF / Aperture photometry on the transients on difference image as if it is an object living in the reference image: using the same psf model / aperture and magnitude zeropoint (but of course, not including the observation date!).
+
+Note that a transient on science image is always a positive signal on difference image whatever -ForceConv is.
+
+Additional Function
+-----------
+
+We also present a decorrelation module to whiten the background noise of the difference image.
+
+.. [*] **difference noise decorrelation** : The example in subdirectory named difference_noise_decorrelation. We use noise-decorrelation toolkit (module ``sfft.utils.DeCorrelationCalculator``) to whiten the background noise on difference image. In this test, the difference image is generated from image subtraction (by sfft) between a coadded reference image and a coadded science image, each stacked from 5 DECam individual observations with PSF homogenization (by sfft). The toolkit can be also applied to whiten a coadded image as long as convolution is involved in the stacking process.
+
+
+Comments on Backward Compatiablity
+-----------
+
+We have tried our best to ensure the backward compatiablity, however, the rule was sometimes overrided in the development of sfft, e.g., some arguments might be deprecated in higher version of sfft. Users might get errors when they use old scripts but update sfft to a higher version. To solve the problem, I have been maintaining the test scripts on Github to make sure they can always work for the lastest version of sfft. You can also find the change log of arguments in the test scripts. 
+
+What's new
+-----------
+
+- A warning for users: As scikit-image has changed something in its function of hough detection since version 0.19.0, I recently found that the source selection in sfft will be affected by this upgrade. I have not checked the new function yet, for the time being I would recommend users to install a scikit-image >= 0.16.2 but <= 0.18.3. Possibly I may add a constrain on scikit-image version in sfft 1.3.5. [Lei, Nov 9, 2022]
+
+- A warning message about the usage of ``sfft.MultiEasySparsePacket`` and ``sfft.MultiEasyCrowdedPacket`` is added in the related test scripts. [Lei, Oct 25, 2022]
+
+- The preprocessing in sparse-flavor-sfft is refined using an additional rejection of mild varaibles since version 1.3.0. [Lei, Aug 19, 2022]
+
+- The sfft is now optimized for multiple tasks since version 1.1.0. [Lei, May 24, 2022]
+
+- A few argument-names have been changed since version 1.1.0, please see the test scripts. [Lei, May 24, 2022]
+
+- Locking file is removed since version 1.1.0, as I found it unreliable in our tests, i.e., -GLockFile is removed. [Lei, May 24, 2022]
+
+- The trial subtraction for refinement is removed since version 1.1.0. However, I add a post-subtraction check to search anomalies on the difference image using the same logic. One can feed the coordinates of the anomalies to sfft again as Prior-Banned sources to refine the subtraction (see -XY_PriorBan in ``sfft.MultiEasySparsePacket``). [Lei, May 24, 2022]
+
+Todo list
+-----------
+
+- The total GPU memory usage is only optimized for KerPolyOrder = 2 & BGPolyOrder = 2, I will extend the optimization to other cases ASAP! In fact, I believe there is ample space for reducing the total GPU usage and I will explore it. [Lei, Nov 11, 2022] **[ALREADY DONE]**
+
+- I will allows users to disable the hough detection for preprocessing when there are too few sources in the field in the next version sfft v1.3.5. [Lei, Nov 11, 2022]
+
+- Add a verbose argument for sfft so that users can get more clean printed messages. [Lei, Nov 9, 2022] **[ALREADY DONE]**
+
+- Test if we can use sep to replace SExtractor in preprocessing to make sfft more Pythonic. [Lei, Nov 9, 2022] 
+
+- Incorporate the separate functions (in the folder beta4spline) for spline form sfft into the unified sfft functions. Note that only Numpy backend is currently available and the spline form is very memory-consuming. [Lei, July 6, 2022]
+
+- Write a detailed documentation for sfft! [Lei, May 24, 2022]
+
+- We notice that SExtractor may have been called to perform astrometric calibration before image subtraction. It is definitely not wise to run SExtractor again in sfft, I need to develop a module which allows users to feed SExtractor products as inputs of sfft, which will significantly reduce the preprocessing time in sfft. [Lei, May 24, 2022]
+
+- The multiprocessing mode is expected to accomondate multiple GPU devices, however, the function has not tested on such a multi-GPUs platform. [Lei, May 24, 2022] **[ALREADY DONE]**
+
+- Add a function for optimizing sfft on a given computing platform with multiple CPU threading and one/multiple GPU card(s). This would be very useful to reduce the overall time cost when users have a large set of image-pairs to be processed simultaneously (e.g., serve for DECam, each exposure produces 61 CCD images). [Lei, May 20, 2022] **[ALREADY DONE]**
+
+Common issues
+-----------
+
+- If your Python environment already has some version of llvmlite (a package required by NumPy backend) before installing sfft. The setup.py in sfft cannot properly update llvmlite to the desired version, then you may get errors related to Numba or llvmlite. If so, please manually install llvmlite by: ::
+
+    pip install llvmlite==0.36.0 --ignore-installed
+
+Development
+-----------
+The latest source code can be obtained from
+`<https://github.com/thomasvrussell/sfft>`_.
+
+When submitting bug reports or questions via the `issue tracker 
+<https://github.com/thomasvrussell/sfft/issues>`_, please include the following 
+information:
+
+- OS platform.
+- Python version.
+- CUDA and CuPy (or PyCUDA) version.
+- Version of sfft.
+
+Citing
+------
+
+*Image Subtraction in Fourier Space. Hu, L., Wang, L., Chen, X., & Yang, J. 2022, The Astrophysical Journal, 936, 157*
+
+Arxiv link: `<https://arxiv.org/abs/2109.09334>`_.
+
+ApJ Publication link: `<https://doi.org/10.3847/1538-4357/ac7394>`_.
+
+Related DOI: 10.3847/1538-4357/ac7394
```

### Comparing `sfft-1.3.4/sfft.egg-info/SOURCES.txt` & `sfft-1.4.0/sfft.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.py
 sfft/AutoCrowdedPrep.py
 sfft/AutoSparsePrep.py
 sfft/CustomizedPacket.py
 sfft/EasyCrowdedPacket.py
 sfft/EasySparsePacket.py
@@ -18,22 +19,22 @@
 sfft/sfftcore/__init__.py
 sfft/utils/CombineHeader.py
 sfft/utils/ConvKernelConvertion.py
 sfft/utils/DeCorrelationCalculator.py
 sfft/utils/HoughDetection.py
 sfft/utils/HoughMorphClassifier.py
 sfft/utils/NeighboringPixelCovariance.py
+sfft/utils/ReadWCS.py
 sfft/utils/SExSkySubtract.py
 sfft/utils/SFFTSolutionReader.py
 sfft/utils/SkyLevelEstimator.py
 sfft/utils/StampGenerator.py
 sfft/utils/SymmetricMatch.py
 sfft/utils/WeightedQuantile.py
 sfft/utils/__init__.py
-sfft/utils/meta/FileLockKit.py
 sfft/utils/meta/MultiProc.py
 sfft/utils/meta/TimeoutKit.py
 sfft/utils/meta/__init__.py
 sfft/utils/pyAstroMatic/AMConfigMaker.py
 sfft/utils/pyAstroMatic/PYSEx.py
 sfft/utils/pyAstroMatic/PYSWarp.py
 sfft/utils/pyAstroMatic/__init__.py
```

