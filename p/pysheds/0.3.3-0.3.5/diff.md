# Comparing `tmp/pysheds-0.3.3.tar.gz` & `tmp/pysheds-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysheds-0.3.3.tar", last modified: Sun Feb 27 08:36:03 2022, max compression
+gzip compressed data, was "pysheds-0.3.5.tar", last modified: Tue May 16 20:26:09 2023, max compression
```

## Comparing `pysheds-0.3.3.tar` & `pysheds-0.3.5.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 08:36:03.802626 pysheds-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-02-27 08:35:52.000000 pysheds-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-02-27 08:35:52.000000 pysheds-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-27 08:36:03.802626 pysheds-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16865 2022-02-27 08:35:52.000000 pysheds-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 08:36:03.802626 pysheds-0.3.3/pysheds/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    71744 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/_sgrid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5453 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/_sview.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    12888 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/io.py
--rw-r--r--   0 runner    (1001) docker     (121)   169170 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/pgrid.py
--rw-r--r--   0 runner    (1001) docker     (121)    14886 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/pview.py
--rw-r--r--   0 runner    (1001) docker     (121)    24804 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/rfsm.py
--rw-r--r--   0 runner    (1001) docker     (121)   115470 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/sgrid.py
--rw-r--r--   0 runner    (1001) docker     (121)    39294 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/sview.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-02-27 08:35:52.000000 pysheds-0.3.3/pysheds/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-27 08:36:03.802626 pysheds-0.3.3/pysheds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-27 08:36:03.000000 pysheds-0.3.3/pysheds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-02-27 08:36:03.000000 pysheds-0.3.3/pysheds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-27 08:36:03.000000 pysheds-0.3.3/pysheds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-02-27 08:36:03.000000 pysheds-0.3.3/pysheds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-27 08:36:03.000000 pysheds-0.3.3/pysheds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-27 08:36:03.802626 pysheds-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-02-27 08:35:52.000000 pysheds-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-16 20:25:58.000000 pysheds-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 20:25:58.000000 pysheds-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 20:26:09.151716 pysheds-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-05-16 20:25:58.000000 pysheds-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/pysheds/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71744 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/_sgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/_sview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169233 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/pgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/pview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24804 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/rfsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115201 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/sgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/sview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 20:25:58.000000 pysheds-0.3.5/pysheds/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/pysheds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 20:26:09.000000 pysheds-0.3.5/pysheds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:26:09.151716 pysheds-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 20:25:58.000000 pysheds-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:26:09.151716 pysheds-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-05-16 20:25:58.000000 pysheds-0.3.5/tests/test_grid.py
```

### Comparing `pysheds-0.3.3/LICENSE` & `pysheds-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.3/README.md` & `pysheds-0.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pysheds [![Build Status](https://travis-ci.org/mdbartos/pysheds.svg?branch=master)](https://travis-ci.org/mdbartos/pysheds) [![Coverage Status](https://coveralls.io/repos/github/mdbartos/pysheds/badge.svg?branch=master&service=github)](https://coveralls.io/github/mdbartos/pysheds?branch=master) [![Python Versions](https://img.shields.io/badge/python-3.6%7C3.7%7C3.8%7C3.9-blue.svg)](https://www.python.org/downloads/)
+# pysheds [![Build Status](https://github.com/mdbartos/pysheds/actions/workflows/python-package.yml/badge.svg)](https://github.com/mdbartos/pysheds/actions) [![Coverage Status](https://coveralls.io/repos/github/mdbartos/pysheds/badge.svg?branch=master&service=github)](https://coveralls.io/github/mdbartos/pysheds?branch=master) [![Python Versions](https://img.shields.io/badge/python-3.7%7C3.8%7C3.9%7C3.10%7C3.11-blue.svg)](https://www.python.org/downloads/)
 🌎 Simple and fast watershed delineation in python.
 
 ## Documentation
 
 Read the docs [here 📖](https://mdbartos.github.io/pysheds).
 
 ## Media
```

### Comparing `pysheds-0.3.3/pysheds/_sgrid.py` & `pysheds-0.3.5/pysheds/_sgrid.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.3/pysheds/_sview.py` & `pysheds-0.3.5/pysheds/_sview.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.3/pysheds/io.py` & `pysheds-0.3.5/pysheds/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import ast
 import warnings
 import numpy as np
 import pyproj
 import rasterio
-import rasterio.features
 from affine import Affine
-from distutils.version import LooseVersion
 from pysheds.sview import Raster, ViewFinder, View
+from rasterio.features import geometry_mask
 
-_OLD_PYPROJ = LooseVersion(pyproj.__version__) < LooseVersion('2.2')
-_pyproj_crs = lambda Proj: Proj.crs if not _OLD_PYPROJ else Proj
-_pyproj_crs_is_geographic = 'is_latlong' if _OLD_PYPROJ else 'is_geographic'
-_pyproj_init = '+init=epsg:4326' if _OLD_PYPROJ else 'epsg:4326'
+from . import projection
 
-def read_ascii(data, skiprows=6, mask=None, crs=pyproj.Proj(_pyproj_init),
+def read_ascii(data, skiprows=6, mask=None, crs=projection.init(),
                xll='lower', yll='lower', metadata={}, **kwargs):
     """
     Reads data from an ascii file and returns a Raster.
 
     Parameters
     ----------
     data : str
@@ -93,46 +89,42 @@
     Returns
     -------
     out : Raster
           Raster object containing loaded data.
     """
     mask = None
     with rasterio.open(data, **kwargs) as f:
-        crs = pyproj.Proj(f.crs, preserve_units=True)
+        crs = projection.to_proj(f.crs)
         if window is None:
             shape = f.shape
             if len(f.indexes) > 1:
                 data = np.ma.filled(f.read(band))
             else:
                 data = np.ma.filled(f.read())
             affine = f.transform
             data = data.reshape(shape)
         else:
             if window_crs is not None:
                 if window_crs.srs != crs.srs:
                     xmin, ymin, xmax, ymax = window
-                    if _OLD_PYPROJ:
-                        extent = pyproj.transform(window_crs, crs, (xmin, xmax),
-                                                (ymin, ymax))
-                    else:
-                        extent = pyproj.transform(window_crs, crs, (xmin, xmax),
-                                                    (ymin, ymax), errcheck=True,
-                                                    always_xy=True)
+                    extent = projection.transform(window_crs, crs, (xmin, xmax),
+                                                (ymin, ymax), errcheck=True,
+                                                always_xy=True)
                     window = (extent[0][0], extent[1][0], extent[0][1], extent[1][1])
             # If window crs not specified, assume it is in raster crs
             ix_window = f.window(*window)
             if len(f.indexes) > 1:
                 data = np.ma.filled(f.read(band, window=ix_window))
             else:
                 data = np.ma.filled(f.read(window=ix_window))
             affine = f.window_transform(ix_window)
             data = np.squeeze(data)
             shape = data.shape
         if mask_geometry:
-            mask = rasterio.features.geometry_mask(mask_geometry, shape, affine, invert=True)
+            mask = geometry_mask(mask_geometry, shape, affine, invert=True)
             # No mask was applied if all False, out of bounds
             if not mask.any():
                 # Return mask to all True and deliver warning
                 warnings.warn('`mask_geometry` does not fall within the bounds of the raster.')
                 mask = ~mask
         # If no `nodata` value specified, read intended nodata value from file
         if nodata is None:
@@ -267,14 +259,15 @@
             Coordinate reference system (overrides target_view.crs)
     mask : np.ndarray or Raster
             Boolean array to mask output (overrides target_view.mask)
     nodata : int or float
                 Value indicating no data in output Raster (overrides target_view.nodata)
     dtype : numpy datatype
             Desired datatype of the output array.
+    kwargs : Keyword arguments passed to rasterio.open together with the profile, eg. compress='lzw'
     """
     if target_view is None:
         target_view = data.viewfinder
     data = View.view(data, target_view, interpolation=interpolation,
                      apply_input_mask=apply_input_mask,
                      apply_output_mask=apply_output_mask,
                      inherit_nodata=inherit_nodata, affine=affine, shape=shape,
@@ -295,10 +288,11 @@
         'transform' : data.affine,
         'dtype' : data.dtype.name,
         'nodata' : data.nodata,
         'height' : height,
         'width' : width
     }
     profile.update(profile_updates)
+    profile.update(kwargs)
     with rasterio.open(file_name, 'w', **profile) as dst:
         dst.write(np.asarray(data), 1)
```

### Comparing `pysheds-0.3.3/pysheds/pgrid.py` & `pysheds-0.3.5/pysheds/pgrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import sys
 import ast
-import copy
 import warnings
 import pyproj
 import numpy as np
 import pandas as pd
 import geojson
 from affine import Affine
 from distutils.version import LooseVersion
 try:
     import scipy.sparse
     import scipy.spatial
     from scipy.sparse import csgraph
     import scipy.interpolate
     _HAS_SCIPY = True
-except:
+except (ModuleNotFoundError, ImportError):
     _HAS_SCIPY = False
 try:
     import skimage.measure
     import skimage.transform
     import skimage.morphology
     _HAS_SKIMAGE = True
-except:
+except ModuleNotFoundError:
     _HAS_SKIMAGE = False
 try:
     import rasterio
     import rasterio.features
     _HAS_RASTERIO = True
-except:
+except ModuleNotFoundError:
     _HAS_RASTERIO = False
 
 _OLD_PYPROJ = LooseVersion(pyproj.__version__) < LooseVersion('2.2')
 _pyproj_crs = lambda Proj: Proj.crs if not _OLD_PYPROJ else Proj
 _pyproj_crs_is_geographic = 'is_latlong' if _OLD_PYPROJ else 'is_geographic'
 _pyproj_init = '+init=epsg:4326' if _OLD_PYPROJ else 'epsg:4326'
```

### Comparing `pysheds-0.3.3/pysheds/pview.py` & `pysheds-0.3.5/pysheds/pview.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.3/pysheds/rfsm.py` & `pysheds-0.3.5/pysheds/rfsm.py`

 * *Files identical despite different names*

### Comparing `pysheds-0.3.3/pysheds/sgrid.py` & `pysheds-0.3.5/pysheds/sgrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 import sys
 import ast
 import copy
-import pyproj
+# import pyproj
 import numpy as np
 import pandas as pd
 import geojson
 from affine import Affine
-from distutils.version import LooseVersion
 try:
     import skimage.measure
     import skimage.morphology
     _HAS_SKIMAGE = True
-except:
+except ModuleNotFoundError:
     _HAS_SKIMAGE = False
 try:
     import rasterio
     import rasterio.features
     _HAS_RASTERIO = True
-except:
+except ModuleNotFoundError:
     _HAS_RASTERIO = False
 
-_OLD_PYPROJ = LooseVersion(pyproj.__version__) < LooseVersion('2.2')
-_pyproj_crs = lambda Proj: Proj.crs if not _OLD_PYPROJ else Proj
-_pyproj_crs_is_geographic = 'is_latlong' if _OLD_PYPROJ else 'is_geographic'
-_pyproj_init = '+init=epsg:4326' if _OLD_PYPROJ else 'epsg:4326'
-
 # Import input/output functions
 import pysheds.io
 
 # Import viewing functions
 from pysheds.sview import Raster, MultiRaster
 from pysheds.sview import View, ViewFinder
 
 # Import numba functions
 import pysheds._sgrid as _self
+from . import projection
 
 class sGrid():
     """
     Container class for holding, aligning, and manipulating gridded data.
 
     Attributes
     ==========
@@ -129,15 +124,15 @@
 
     @property
     def defaults(self):
         props = {
             'affine' : Affine(1.,0.,0.,0.,1.,0.),
             'shape' : (1,1),
             'nodata' : 0,
-            'crs' : pyproj.Proj(_pyproj_init),
+            'crs' : projection.init(),
         }
         return props
 
     @property
     def affine(self):
         return self.viewfinder.affine
 
@@ -188,15 +183,15 @@
     @property
     def extent(self):
         bbox = self.bbox
         extent = (self.bbox[0], self.bbox[2], self.bbox[1], self.bbox[3])
         return extent
 
     def read_ascii(self, data, skiprows=6, mask=None,
-                   crs=pyproj.Proj(_pyproj_init), xll='lower', yll='lower',
+                   crs=projection.init(), xll='lower', yll='lower',
                    metadata={}, **kwargs):
         """
         Reads data from an ascii file and returns a Raster.
 
         Parameters
         ----------
         data : str
```

### Comparing `pysheds-0.3.3/pysheds/sview.py` & `pysheds-0.3.5/pysheds/sview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import copy
 import numpy as np
-import pyproj
+from . import projection
 from affine import Affine
 from distutils.version import LooseVersion
 try:
     import scipy.spatial
     _HAS_SCIPY = True
-except:
+except ModuleNotFoundError:
     _HAS_SCIPY = False
 
 import pysheds._sview as _self
 
-_OLD_PYPROJ = LooseVersion(pyproj.__version__) < LooseVersion('2.2')
-_pyproj_init = '+init=epsg:4326' if _OLD_PYPROJ else 'epsg:4326'
 
 class Raster(np.ndarray):
     """
     Array-like data structure with a coordinate reference system. A Raster is instantiated
     from an array-like object and a ViewFinder. Optional metadata may also be provided
     as a keyword argument.
 
@@ -230,15 +228,15 @@
         top = np.column_stack([X[0, :], Y[0, :]])
         bottom = np.column_stack([X[-1, :], Y[-1, :]])
         left = np.column_stack([X[:, 0], Y[:, 0]])
         right = np.column_stack([X[:, -1], Y[:, -1]])
         boundary = np.vstack([top, bottom, left, right])
         xi, yi = boundary[:,0], boundary[:,1]
         xb, yb = View.affine_transform(self.affine, xi, yi)
-        xb_p, yb_p = pyproj.transform(old_crs, new_crs, xb, yb,
+        xb_p, yb_p = projection.transform(old_crs, new_crs, xb, yb,
                                       errcheck=True, always_xy=True)
         x0_p = xb_p.min() if (dx > 0) else xb_p.max()
         y0_p = yb_p.min() if (dy > 0) else yb_p.max()
         xn_p = xb_p.max() if (dx > 0) else xb_p.min()
         yn_p = yb_p.max() if (dy > 0) else yb_p.min()
         a = (xn_p - x0_p) / n
         e = (yn_p - y0_p) / m
@@ -327,15 +325,15 @@
            top-left corners of the leftmost and upper edges of the dataset, respectively).
     properties : A dict containing the names and values of the essential properties
                  that define the coordinate reference system, including `affine`,
                  `shape`, `mask`, `crs`, and `nodata`.
     dy_dx : Tuple describing the cell size in the y and x directions.
     """
     def __init__(self, affine=Affine(1., 0., 0., 0., 1., 0.), shape=(1,1),
-                 nodata=0, mask=None, crs=pyproj.Proj(_pyproj_init)):
+                 nodata=0, mask=None, crs=projection.init()):
         self.affine = affine
         self.crs = crs
         self.nodata = nodata
         if mask is None:
             self.mask = np.ones(shape, dtype=np.bool8)
         else:
             self.mask = mask
@@ -407,19 +405,15 @@
 
     @property
     def crs(self):
         return self._crs
 
     @crs.setter
     def crs(self, new_crs):
-        try:
-            assert (isinstance(new_crs, pyproj.Proj))
-        except:
-            raise TypeError('`crs` must be a `pyproj.Proj` object.')
-        self._crs = new_crs
+        self._crs = projection.to_proj(new_crs)
 
     @property
     def size(self):
         return np.prod(self.shape)
 
     @property
     def bbox(self):
@@ -788,24 +782,23 @@
         if return_dist:
             return tree_xy[ix], dist
         else:
             return tree_xy[ix]
 
     @classmethod
     def trim_zeros(cls, data, pad=(0,0,0,0)):
-        """
-        Clip a Raster to the smallest area that contains all non-null data.
+        """Clip a Raster to the smallest area that contains all non-null data.
 
         Parameters
         ----------
         data : Raster
-               A Raster dataset.
+            A Raster dataset.
         pad : tuple of int (length 4)
-              Apply padding to edges of new view (left, bottom, right, top). A pad of
-              (1,1,1,1), for instance, will add a one-cell rim around the new view.
+            Apply padding to edges of new view (left, bottom, right, top).
+            A pad of (1,1,1,1), for instance, will add a one-cell rim around the new view.
 
         Returns
         -------
         out : Raster
               A Raster dataset clipped to the bounding box of its non-null values.
         """
         try:
@@ -822,27 +815,25 @@
             mask = (~np.isnan(data))
         else:
             mask = (data != data.nodata)
         return cls.clip_to_mask(data, mask=mask, pad=pad)
 
     @classmethod
     def clip_to_mask(cls, data, mask=None, pad=(0,0,0,0)):
-        """
-        Clip a Raster to the smallest area that contains all nonzero entries for a
-        given boolean mask.
+        """Clip a Raster to the smallest area that contains all nonzero entries for a given boolean mask.
 
         Parameters
         ----------
         data : Raster
-               A Raster dataset.
+            A Raster dataset.
         mask : Raster
-               A Raster dataset representing a boolean mask. Defaults to data.mask.
+            A Raster dataset representing a boolean mask. Defaults to data.mask.
         pad : tuple of int (length 4)
-              Apply padding to edges of new view (left, bottom, right, top). A pad of
-              (1,1,1,1), for instance, will add a one-cell rim around the new view.
+            Apply padding to edges of new view (left, bottom, right, top).
+            A pad of (1,1,1,1), for instance, will add a one-cell rim around the new view.
 
         Returns
         -------
         out : Raster
               A Raster dataset clipped to the bounding box of the non-null entries
               in the given mask.
         """
@@ -964,15 +955,15 @@
         else:
             raise ValueError('Interpolation method must be one of: `nearest`, `linear`')
         return view
 
     @classmethod
     def _view_different_crs(cls, view, data, data_view, target_view, interpolation='nearest'):
         y, x = target_view.coords.T
-        xt, yt = pyproj.transform(target_view.crs, data_view.crs, x=x, y=y,
+        xt, yt = projection.transform(target_view.crs, data_view.crs, x=x, y=y,
                                   errcheck=True, always_xy=True)
         inv_affine = ~data_view.affine
         x_ix, y_ix = cls.affine_transform(inv_affine, xt, yt)
         nodata = target_view.nodata
         if interpolation == 'nearest':
             view = _self._view_fill_by_entries_nearest_numba(data, view, y_ix, x_ix, nodata)
         elif interpolation == 'linear':
```

