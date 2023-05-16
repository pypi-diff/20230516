# Comparing `tmp/structuretoolkit-0.0.2.tar.gz` & `tmp/structuretoolkit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structuretoolkit-0.0.2.tar", last modified: Fri May  5 17:20:04 2023, max compression
+gzip compressed data, was "structuretoolkit-0.0.3.tar", last modified: Tue May 16 18:33:28 2023, max compression
```

## Comparing `structuretoolkit-0.0.2.tar` & `structuretoolkit-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 17:20:04.970569 structuretoolkit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.970569 structuretoolkit-0.0.2/structuretoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 17:20:04.970569 structuretoolkit-0.0.2/structuretoolkit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/structuretoolkit/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    47426 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/strain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/analyse/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/structuretoolkit/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/build/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30831 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/structuretoolkit/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.962569 structuretoolkit-0.0.2/structuretoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 17:20:04.000000 structuretoolkit-0.0.2/structuretoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:04.966569 structuretoolkit-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_high_index_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18819 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-05 17:20:01.000000 structuretoolkit-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-16 18:33:28.000000 structuretoolkit-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/structuretoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/structuretoolkit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.598732 structuretoolkit-0.0.3/structuretoolkit/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47432 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24392 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/analyse/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/structuretoolkit/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/build/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/build/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/build/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/build/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/structuretoolkit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/common/pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/common/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30843 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/structuretoolkit/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.598732 structuretoolkit-0.0.3/structuretoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-16 18:33:28.000000 structuretoolkit-0.0.3/structuretoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-16 18:33:28.000000 structuretoolkit-0.0.3/structuretoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:33:28.000000 structuretoolkit-0.0.3/structuretoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 18:33:28.000000 structuretoolkit-0.0.3/structuretoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 18:33:28.000000 structuretoolkit-0.0.3/structuretoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:33:28.602732 structuretoolkit-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_high_index_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_strain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-16 18:33:25.000000 structuretoolkit-0.0.3/versioneer.py
```

### Comparing `structuretoolkit-0.0.2/LICENSE` & `structuretoolkit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.2/PKG-INFO` & `structuretoolkit-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,10 +12,18 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: grainboundary
+Provides-Extra: pyscal
+Provides-Extra: nglview
+Provides-Extra: plotly
+Provides-Extra: clusters
+Provides-Extra: symmetry
+Provides-Extra: surface
+Provides-Extra: phonopy
 License-File: LICENSE
 
 http://pyiron.org
```

### Comparing `structuretoolkit-0.0.2/setup.py` & `structuretoolkit-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,19 +26,24 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
-        'aimsgb>=0.1.1',
         'ase>=3.22.1',
-        'matplotlib>=3.7.0',
-        'numpy>=1.24.2',
-        'phonopy>=2.17.1',
-        'pymatgen>=2022.11.7',
-        'scipy>=1.10.0',
-        'scikit-learn>=1.2.1',
-        'spglib>=2.0.2',
+        'matplotlib>=3.7.0',  # ase already requires matplotlib
+        'numpy>=1.24.2',  # ase already requires numpy
+        'scipy>=1.10.0',  # ase already requires scipy
     ],
+    extras_require={
+        "grainboundary": ['aimsgb>=0.1.1', 'pymatgen>=2022.11.7'],
+        "pyscal": ['pyscal2>=2.10.20'],
+        "nglview": ['nglview>=3.0.4'],
+        "plotly": ['plotly>=5.14.1'],
+        "clusters": ['scikit-learn>=1.2.1'],
+        "symmetry": ['spglib>=2.0.2'],
+        "surface": ['spglib>=2.0.2', 'pymatgen>=2022.11.7'],
+        "phonopy": ['phonopy>=2.17.1', 'spglib>=2.0.2'],
+    },
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/distance.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/distance.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/neighbors.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/neighbors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from sklearn.cluster import AgglomerativeClustering
 from scipy.sparse import coo_matrix
 from scipy.special import gamma
 from scipy.spatial.transform import Rotation
 from scipy.special import sph_harm
 from scipy.spatial import cKDTree
 import warnings
 import itertools
-from structuretoolkit.helper import get_extended_positions, get_average_of_unique_labels
+from structuretoolkit.common.helper import (
+    get_extended_positions,
+    get_average_of_unique_labels,
+)
 
 __author__ = "Joerg Neugebauer, Sam Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -47,15 +49,15 @@
     get_neighborhood.
 
     """
 
     def __init__(self, ref_structure):
         """
         Args:
-            ref_structure (pyiron_atomistics.atomistics.structure.atoms.Atoms): Reference
+            ref_structure (ase.atoms.Atoms): Reference
                 structure.
         """
         self._distances = None
         self._vectors = None
         self._indices = None
         self._mode = {"filled": True, "ragged": False, "flattened": False}
         self._extended_positions = None
@@ -395,15 +397,15 @@
             position: Position in a box whose neighborhood information is analysed
             num_neighbors (int): Number of nearest neighbors
             cutoff_radius (float): Upper bound of the distance to which the search is to be done
             width_buffer (float): Width of the layer to be added to account for pbc.
 
         Returns:
 
-            pyiron.atomistics.structure.atoms.Tree: Neighbors instances with the neighbor indices,
+            structuretoolkit.analyse.neighbors.Tree: Neighbors instances with the neighbor indices,
                 distances and vectors
 
         """
         new_neigh = self.copy()
         return new_neigh._get_neighborhood(
             positions=positions,
             num_neighbors=num_neighbors,
@@ -795,16 +797,16 @@
             chemical_pair (list): pair of chemical symbols (e.g. ['Fe', 'Ni'])
 
         Returns:
             list of sparse matrices for different shells
 
 
         Example:
-            from pyiron_atomistics import Project
-            structure = Project('.').create_structure('Fe', 'bcc', 2.83).repeat(2)
+            from ase.build import bulk
+            structure = bulk('Fe', 'bcc', 2.83).repeat(2)
             J = -0.1 # Ising parameter
             magmoms = 2*np.random.random((len(structure)), 3)-1 # Random magnetic moments between -1 and 1
             neigh = structure.get_neighbors(num_neighbors=8) # Iron first shell
             shell_matrices = neigh.get_shell_matrix()
             print('Energy =', 0.5*J*magmoms.dot(shell_matrices[0].dot(matmoms)))
         """
 
@@ -879,15 +881,15 @@
         return indices[np.arange(len(dist)), np.argmin(dist, axis=-1)]
 
     def cluster_by_vecs(
         self,
         distance_threshold=None,
         n_clusters=None,
         linkage="complete",
-        affinity="euclidean",
+        metric="euclidean",
     ):
         """
         Method to group vectors which have similar values. This method should be used as a part of
         neigh.get_global_shells(cluster_by_vecs=True) or neigh.get_local_shells(cluster_by_vecs=True).
         However, in order to specify certain arguments (such as n_jobs or max_iter), it might help to
         have run this function before calling parent functions, as the data obtained with this function
         will be stored in the variable `_cluster_vecs`
@@ -896,41 +898,43 @@
             distance_threshold (float/None): The linkage distance threshold above which, clusters
                 will not be merged. (cf. sklearn.cluster.AgglomerativeClustering)
             n_clusters (int/None): The number of clusters to find.
                 (cf. sklearn.cluster.AgglomerativeClustering)
             linkage (str): Which linkage criterion to use. The linkage criterion determines which
                 distance to use between sets of observation. The algorithm will merge the pairs of
                 cluster that minimize this criterion. (cf. sklearn.cluster.AgglomerativeClustering)
-            affinity (str/callable): Metric used to compute the linkage. Can be `euclidean`, `l1`,
+            metric (str/callable): Metric used to compute the linkage. Can be `euclidean`, `l1`,
                 `l2`, `manhattan`, `cosine`, or `precomputed`. If linkage is `ward`, only
                 `euclidean` is accepted.
 
         """
+        from sklearn.cluster import AgglomerativeClustering
+
         if distance_threshold is None and n_clusters is None:
             distance_threshold = np.min(self.filled.distances)
         dr = self.flattened.vecs
         self._cluster_vecs = AgglomerativeClustering(
             distance_threshold=distance_threshold,
             n_clusters=n_clusters,
             linkage=linkage,
-            affinity=affinity,
+            metric=metric,
         ).fit(dr)
         self._cluster_vecs.cluster_centers_ = get_average_of_unique_labels(
             self._cluster_vecs.labels_, dr
         )
         new_labels = -np.ones_like(self.filled.indices).astype(int)
         new_labels[self.filled.distances < np.inf] = self._cluster_vecs.labels_
         self._cluster_vecs.labels_ = new_labels
 
     def cluster_by_distances(
         self,
         distance_threshold=None,
         n_clusters=None,
         linkage="complete",
-        affinity="euclidean",
+        metric="euclidean",
         use_vecs=False,
     ):
         """
         Method to group vectors which have similar lengths. This method should be used as a part of
         neigh.get_global_shells(cluster_by_vecs=True) or
         neigh.get_local_shells(cluster_by_distances=True).  However, in order to specify certain
         arguments (such as n_jobs or max_iter), it might help to have run this function before
@@ -941,21 +945,23 @@
             distance_threshold (float/None): The linkage distance threshold above which, clusters
                 will not be merged. (cf. sklearn.cluster.AgglomerativeClustering)
             n_clusters (int/None): The number of clusters to find.
                 (cf. sklearn.cluster.AgglomerativeClustering)
             linkage (str): Which linkage criterion to use. The linkage criterion determines which
                 distance to use between sets of observation. The algorithm will merge the pairs of
                 cluster that minimize this criterion. (cf. sklearn.cluster.AgglomerativeClustering)
-            affinity (str/callable): Metric used to compute the linkage. Can be `euclidean`, `l1`,
+            metric (str/callable): Metric used to compute the linkage. Can be `euclidean`, `l1`,
                 `l2`, `manhattan`, `cosine`, or `precomputed`. If linkage is `ward`, only
                 `euclidean` is accepted.
             use_vecs (bool): Whether to form clusters for vecs beforehand. If true, the distances
                 obtained from the clustered vectors is used for the distance clustering. Otherwise
                 neigh.distances is used.
         """
+        from sklearn.cluster import AgglomerativeClustering
+
         if distance_threshold is None:
             distance_threshold = 0.1 * np.min(self.flattened.distances)
         dr = self.flattened.distances
         if use_vecs:
             if self._cluster_vecs is None:
                 self.cluster_by_vecs()
             labels_to_consider = self._cluster_vecs.labels_[
@@ -966,15 +972,15 @@
                 axis=-1,
                 ord=self.norm_order,
             )
         self._cluster_dist = AgglomerativeClustering(
             distance_threshold=distance_threshold,
             n_clusters=n_clusters,
             linkage=linkage,
-            affinity=affinity,
+            metric=metric,
         ).fit(dr.reshape(-1, 1))
         self._cluster_dist.cluster_centers_ = get_average_of_unique_labels(
             self._cluster_dist.labels_, dr
         )
         new_labels = -np.ones_like(self.filled.indices).astype(int)
         new_labels[self.filled.distances < np.inf] = self._cluster_dist.labels_
         self._cluster_dist.labels_ = new_labels
@@ -1122,15 +1128,15 @@
         norm_order (int): Norm to use for the neighborhood search and shell recognition. The
             definition follows the conventional Lp norm (cf.
             https://en.wikipedia.org/wiki/Lp_space). This is an feature and for anything
             other than norm_order=2, there is no guarantee that this works flawlessly.
 
     Returns:
 
-        pyiron.atomistics.structure.atoms.Neighbors: Neighbors instances with the neighbor
+        structuretoolkit.analyse.neighbors.Neighbors: Neighbors instances with the neighbor
             indices, distances and vectors
 
     """
     neigh = _get_neighbors(
         structure=structure,
         num_neighbors=num_neighbors,
         tolerance=tolerance,
@@ -1214,15 +1220,15 @@
         norm_order (int): Norm to use for the neighborhood search and shell recognition. The
             definition follows the conventional Lp norm (cf.
             https://en.wikipedia.org/wiki/Lp_space). This is an feature and for anything
             other than norm_order=2, there is no guarantee that this works flawlessly.
 
     Returns:
 
-        pyiron.atomistics.structure.atoms.Tree: Neighbors instances with the neighbor
+        structuretoolkit.analyse.neighbors.Tree: Neighbors instances with the neighbor
             indices, distances and vectors
 
     """
 
     neigh = _get_neighbors(
         structure=structure,
         num_neighbors=num_neighbors,
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/phonopy.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/phonopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from phonopy.structure.atoms import PhonopyAtoms
-import spglib as spg
 
 __author__ = "Osamu Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Osamu Waseda"
 __email__ = "waseda@mpie.de"
 __status__ = "development"
 __date__ = "Sep 1, 2018"
 
 
-def analyse_phonopy_equivalent_atoms(structure, symprec=1e-5, angle_tolerance=-1.0):
+def get_equivalent_atoms(structure, symprec=1e-5, angle_tolerance=-1.0):
     """
     Args: (read phonopy.structure.spglib for more details)
         symprec:
             float: Symmetry search tolerance in the unit of length.
         angle_tolerance:
             float: Symmetry search tolerance in the unit of angle deg.
                 If the value is negative, an internally optimized routine
                 is used to judge symmetry.
 
     """
+    import spglib as spg
+    from phonopy.structure.atoms import PhonopyAtoms
+
     positions = structure.get_scaled_positions()
     cell = structure.cell
     types = structure.get_chemical_symbols()
     types = list(types)
     natom = len(types)
     positions = np.reshape(np.array(positions), (natom, 3))
     cell = np.reshape(np.array(cell), (3, 3))
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/pyscal.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/pyscal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from ase.atoms import Atoms
-import pyscal.core as pc
-from sklearn import cluster
+from structuretoolkit.common.pyscal import ase_to_pyscal
 
 __author__ = "Sarath Menon, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sarath Menon"
 __email__ = "sarath.menon@rub.de"
 __status__ = "development"
 __date__ = "Nov 6, 2019"
 
 
-def get_steinhardt_parameter_structure(
+def get_steinhardt_parameters(
     structure,
     neighbor_method="cutoff",
     cutoff=0,
     n_clusters=2,
     q=None,
     averaged=False,
 ):
@@ -39,48 +38,52 @@
             uses (4, 6).)
         averaged (bool) : If True, calculates the averaged versions of the parameter. (Default is False.)
 
     Returns:
         numpy.ndarray: (number of q's, number of atoms) shaped array of q parameters
         numpy.ndarray: If `clustering=True`, an additional per-atom array of cluster ids is also returned
     """
-    sys = pyiron_to_pyscal_system(structure)
+    sys = ase_to_pyscal(structure)
     q = (4, 6) if q is None else q
 
     sys.find_neighbors(method=neighbor_method, cutoff=cutoff)
 
     sys.calculate_q(q, averaged=averaged)
 
     sysq = np.array(sys.get_qvals(q, averaged=averaged))
 
     if n_clusters is not None:
+        from sklearn import cluster
+
         cl = cluster.KMeans(n_clusters=n_clusters)
 
         ind = cl.fit(list(zip(*sysq))).labels_
         return sysq, ind
     else:
         return sysq
 
 
-def analyse_centro_symmetry(structure, num_neighbors=12):
+def get_centro_symmetry_descriptors(structure, num_neighbors=12):
     """
     Analyse centrosymmetry parameter
 
     Args:
         structure: Atoms object
         num_neighbors (int) : number of neighbors
 
     Returns:
         csm (list) : list of centrosymmetry parameter
     """
-    sys = pyiron_to_pyscal_system(structure)
+    sys = ase_to_pyscal(structure)
     return np.array(sys.calculate_centrosymmetry(nmax=num_neighbors))
 
 
-def analyse_diamond_structure(structure, mode="total", ovito_compatibility=False):
+def get_diamond_structure_descriptors(
+    structure, mode="total", ovito_compatibility=False
+):
     """
     Analyse diamond structure
 
     Args:
         structure: Atoms object
         mode ("total"/"numeric"/"str"): Controls the style and level
         of detail of the output.
@@ -89,15 +92,15 @@
                 1 fcc, 2 hcp, 3 bcc and 4 icosa
             - str : return a per atom string of sructures
         ovito_compatibility(bool): use ovito compatiblity mode
 
     Returns:
         (depends on `mode`)
     """
-    sys = pyiron_to_pyscal_system(structure)
+    sys = ase_to_pyscal(structure)
     diamond_dict = sys.identify_diamond()
 
     ovito_identifiers = [
         "Cubic diamond",
         "Cubic diamond (1st neighbor)",
         "Cubic diamond (2nd neighbor)",
         "Hexagonal diamond",
@@ -174,32 +177,32 @@
             )
     else:
         raise ValueError(
             "Only total, str and numeric mode is imported for analyse_diamond_structure()"
         )
 
 
-def analyse_cna_adaptive(structure, mode="total", ovito_compatibility=False):
+def get_adaptive_cna_descriptors(structure, mode="total", ovito_compatibility=False):
     """
     Use common neighbor analysis
 
     Args:
-        structure (pyiron_atomistics.structure.atoms.Atoms): The structure to analyze.
+        structure (ase.atoms.Atoms): The structure to analyze.
         mode ("total"/"numeric"/"str"): Controls the style and level
             of detail of the output.
             - total : return number of atoms belonging to each structure
             - numeric : return a per atom list of numbers- 0 for unknown,
                 1 fcc, 2 hcp, 3 bcc and 4 icosa
             - str : return a per atom string of sructures
         ovito_compatibility(bool): use ovito compatiblity mode
 
     Returns:
         (depends on `mode`)
     """
-    sys = pyiron_to_pyscal_system(structure)
+    sys = ase_to_pyscal(structure)
     if mode not in ["total", "numeric", "str"]:
         raise ValueError("Unsupported mode")
 
     pyscal_parameter = ["others", "fcc", "hcp", "bcc", "ico"]
     ovito_parameter = [
         "CommonNeighborAnalysis.counts.OTHER",
         "CommonNeighborAnalysis.counts.FCC",
@@ -229,47 +232,28 @@
                 return np.array([dd[int(x)] for x in cnalist])
         else:
             raise ValueError(
                 "Only total, str and numeric mode is imported for analyse_cna_adaptive()"
             )
 
 
-def analyse_voronoi_volume(structure):
+def get_voronoi_volumes(structure):
     """
     Calculate the Voronoi volume of atoms
 
     Args:
-        structure : (pyiron_atomistics.structure.atoms.Atoms): The structure to analyze.
+        structure : (ase.atoms.Atoms): The structure to analyze.
     """
-    sys = pyiron_to_pyscal_system(structure)
+    sys = ase_to_pyscal(structure)
     sys.find_neighbors(method="voronoi")
     structure = sys.atoms
     return np.array([atom.volume for atom in structure])
 
 
-def pyiron_to_pyscal_system(structure):
-    """
-    Converts atoms to ase atoms and than to a pyscal system.
-    Also adds the pyscal publication.
-
-    Args:
-        structure (pyiron atoms): Structure to convert.
-
-    Returns:
-        Pyscal system: See the pyscal documentation.
-    """
-    sys = pc.System()
-    sys.read_inputfile(
-        structure,
-        format="ase",
-    )
-    return sys
-
-
-def analyse_find_solids(
+def find_solids(
     structure,
     neighbor_method="cutoff",
     cutoff=0,
     bonds=0.5,
     threshold=0.5,
     avgthreshold=0.6,
     cluster=False,
@@ -292,15 +276,15 @@
         right (bool, optional): See pyscal documentation. Defaults to True.
         return_sys (bool, optional): Whether to return number of solid atoms or pyscal system. Defaults to False.
 
     Returns:
         int: number of solids,
         pyscal system: pyscal system when return_sys=True
     """
-    sys = pyiron_to_pyscal_system(structure)
+    sys = ase_to_pyscal(structure)
     sys.find_neighbors(method=neighbor_method, cutoff=cutoff)
     sys.find_solids(
         bonds=bonds,
         threshold=threshold,
         avgthreshold=avgthreshold,
         q=q,
         cutoff=cutoff,
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/spatial.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/spatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
-from sklearn.cluster import AgglomerativeClustering, DBSCAN
 from scipy.sparse import coo_matrix
 from scipy.spatial import Voronoi, Delaunay
 from scipy.spatial import ConvexHull
-from structuretoolkit.helper import (
+from structuretoolkit.common.helper import (
     get_extended_positions,
     get_wrapped_coordinates,
     get_vertical_length,
     get_average_of_unique_labels,
 )
 from structuretoolkit.analyse.neighbors import get_neighborhood
 
@@ -181,15 +180,15 @@
 
     @property
     def neigh(self):
         """
         Neighborhood information of each interstitial candidate and their surrounding atoms. E.g.
         `class.neigh.distances[0][0]` gives the distance from the first interstitial candidate to
         its nearest neighboring atoms. The functionalities of `neigh` follow those of
-        `pyiron_atomistics.structure.atoms.neighbors`.
+        `structuretoolkit.analyse.neighbors`.
         """
         if self._neigh is None:
             self._neigh = get_neighborhood(
                 structure=self.structure,
                 positions=self.positions,
                 num_neighbors=self.num_neighbors,
             )
@@ -257,14 +256,16 @@
 
     def _kick_out_points(self, variance_buffer=0.01):
         variance = self.get_variances()
         min_var = variance.min()
         self.positions = self.positions[variance < min_var + variance_buffer]
 
     def _cluster_points(self, eps=0.1):
+        from sklearn.cluster import DBSCAN
+
         if eps == 0:
             return
         extended_positions, indices = get_extended_positions(
             structure=self.structure,
             width=eps,
             return_indices=True,
             positions=self.positions,
@@ -424,14 +425,16 @@
             )
     if planes is not None:
         mat = np.asarray(planes).reshape(-1, 3)
         positions = np.einsum(
             "ij,i,nj->ni", mat, 1 / np.linalg.norm(mat, axis=-1), positions
         )
     if cluster_method is None:
+        from sklearn.cluster import AgglomerativeClustering
+
         cluster_method = AgglomerativeClustering(
             linkage="complete",
             n_clusters=None,
             distance_threshold=distance_threshold,
         )
     layers = []
     for ii, x in enumerate(positions.T):
@@ -489,14 +492,16 @@
 
     """
     voro = Voronoi(
         get_extended_positions(structure=structure, width=width_buffer) + epsilon
     )
     xx = voro.vertices
     if distance_threshold > 0:
+        from sklearn.cluster import AgglomerativeClustering
+
         cluster = AgglomerativeClustering(
             linkage="single", distance_threshold=distance_threshold, n_clusters=None
         )
         cluster.fit(xx)
         xx = get_average_of_unique_labels(cluster.labels_, xx)
     xx = xx[
         np.linalg.norm(
@@ -563,37 +568,37 @@
         structure=structure,
         position_interpreter=Delaunay,
         data_field="simplices",
         width_buffer=width_buffer,
     )
 
 
-def cluster_positions(
+def get_cluster_positions(
     structure, positions=None, eps=1, buffer_width=None, return_labels=False
 ):
     """
     Cluster positions according to the distances. Clustering algorithm uses DBSCAN:
 
     https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html
 
     Example I:
 
     ```
-    analyse = Analyze(some_pyiron_structure)
+    analyse = Analyze(some_ase_structure)
     positions = analyse.cluster_points(eps=2)
     ```
 
     This example should return the atom positions, if no two atoms lie within a distance of 2.
     If there are at least two atoms which lie within a distance of 2, their entries will be
     replaced by their mean position.
 
     Example II:
 
     ```
-    analyse = Analyze(some_pyiron_structure)
+    analyse = Analyze(some_ase_structure)
     print(analyse.cluster_positions([3*[0.], 3*[1.]], eps=3))
     ```
 
     This returns `[0.5, 0.5, 0.5]` (if the cell is large enough)
 
     Args:
         positions (numpy.ndarray): Positions to consider. Default: atom positions
@@ -605,14 +610,16 @@
         return_labels (bool): Whether to return the labels given according to the grouping
             together with the mean positions
 
     Returns:
         positions (numpy.ndarray): Mean positions
         label (numpy.ndarray): Labels of the positions (returned when `return_labels = True`)
     """
+    from sklearn.cluster import DBSCAN
+
     positions = structure.positions if positions is None else np.array(positions)
     if buffer_width is None:
         buffer_width = eps
     extended_positions, indices = get_extended_positions(
         structure=structure,
         width=buffer_width,
         return_indices=True,
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/strain.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/strain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.spatial.transform import Rotation
 from structuretoolkit.analyse.neighbors import get_neighbors
-from structuretoolkit.analyse.pyscal import analyse_cna_adaptive
+from structuretoolkit.analyse.pyscal import get_adaptive_cna_descriptors
 
 
 class Strain:
 
     """
     Calculate local strain of each atom following the Lagrangian strain tensor:
 
@@ -25,17 +25,17 @@
 
     def __init__(
         self, structure, ref_structure, num_neighbors=None, only_bulk_type=False
     ):
         """
 
         Args:
-            structure (pyiron_atomistics.atomistics.structure.Atoms): Structure to calculate the
+            structure (ase.atoms.Atoms): Structure to calculate the
                 strain values.
-            ref_structure (pyiron_atomistics.atomistics.structure.Atoms): Reference bulk structure
+            ref_structure (ase.atoms.Atoms): Reference bulk structure
                 (against which the strain is calculated)
             num_neighbors (int): Number of neighbors to take into account to calculate the local
                 frame. If not specified, it is estimated based on cna analysis (only available if
                 the bulk structure is bcc, fcc or hcp).
             only_bulk_type (bool): Whether to calculate the strain of all atoms or only for those
                 which cna considers has the same crystal structure as the bulk. Those which have
                 a different crystal structure will get 0 strain.
@@ -134,15 +134,15 @@
         distances = np.linalg.norm(
             coords[:, :, None, :] - ref_coord[None, None, :, :], axis=-1
         )
         return np.argmin(distances, axis=-1)
 
     @staticmethod
     def _get_majority_phase(structure):
-        cna = analyse_cna_adaptive(structure=structure)
+        cna = get_adaptive_cna_descriptors(structure=structure)
         return np.asarray([k for k in cna.keys()])[np.argmax([v for v in cna.values()])]
 
     @staticmethod
     def _get_number_of_neighbors(crystal_phase):
         if crystal_phase == "bcc":
             return 8
         elif crystal_phase == "fcc" or crystal_phase == "hcp":
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/analyse/symmetry.py` & `structuretoolkit-0.0.3/structuretoolkit/analyse/symmetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,33 +3,29 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from scipy.spatial import cKDTree
 import spglib
 import ast
 
-import structuretoolkit.helper
-from structuretoolkit.helper import get_structure_indices
+import structuretoolkit.common.helper
+from structuretoolkit.common.error import SymmetryError
 
 __author__ = "Joerg Neugebauer, Sam Waseda"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Sam Waseda"
 __email__ = "waseda@mpie.de"
 __status__ = "production"
 __date__ = "Sep 1, 2017"
 
 
-class SymmetryError(Exception):
-    pass
-
-
 class Symmetry(dict):
 
     """
 
     Return a class for operations related to box symmetries. Main attributes:
 
     - rotations: List of rotational matrices
@@ -46,15 +42,15 @@
         use_elements=True,
         symprec=1e-5,
         angle_tolerance=-1.0,
         epsilon=1.0e-8,
     ):
         """
         Args:
-            structure (:class:`pyiron.atomistics.structure.atoms.Atoms`): reference Atom structure.
+            structure (:class:`ase.atoms.Atoms`): reference Atom structure.
             use_magmoms (bool): Whether to consider magnetic moments (cf.
             get_initial_magnetic_moments())
             use_elements (bool): If False, chemical elements will be ignored
             symprec (float): Symmetry search precision
             angle_tolerance (float): Angle search tolerance
             epsilon (float): displacement to add to avoid wrapping of atoms at borders
         """
@@ -239,19 +235,25 @@
         )
         if use_elements is None:
             use_elements = self._use_elements
         if use_magmoms is None:
             use_magmoms = self._use_magmoms
         if use_elements:
             numbers = np.array(
-                get_structure_indices(structure=self._structure), dtype="intc"
+                structuretoolkit.common.helper.get_structure_indices(
+                    structure=self._structure
+                ),
+                dtype="intc",
             )
         else:
             numbers = np.ones_like(
-                get_structure_indices(structure=self._structure), dtype="intc"
+                structuretoolkit.common.helper.get_structure_indices(
+                    structure=self._structure
+                ),
+                dtype="intc",
             )
         if use_magmoms:
             return (
                 lattice,
                 positions,
                 numbers,
                 self._structure.get_initial_magnetic_moments(),
@@ -330,15 +332,15 @@
         Args:
             standardize (bool): Get orthogonal box
             use_magmoms (bool): Whether to consider magnetic moments (cf.
             get_initial_magnetic_moments())
             use_elements (bool): If False, chemical elements will be ignored
 
         Returns:
-            (pyiron_atomistics.atomistics.structure.atoms.Atoms): Primitive cell
+            (ase.atoms.Atoms): Primitive cell
 
         Example (assume `basis` is a primitive cell):
 
         >>> structure = basis.repeat(2)
         >>> symmetry = Symmetry(structure)
         >>> len(symmetry.get_primitive_cell()) == len(basis)
         True
@@ -350,15 +352,15 @@
         if ret is None:
             raise SymmetryError(spglib.spglib.spglib_error.message)
         cell, positions, indices = ret
         positions = (cell.T @ positions.T).T
         new_structure = self._structure.copy()
         new_structure.cell = cell
         new_structure = new_structure[: len(indices)]
-        new_structure = structuretoolkit.helper.set_indices(
+        new_structure = structuretoolkit.common.helper.set_indices(
             structure=new_structure, indices=indices
         )
         new_structure.positions = positions
         return new_structure
 
     def get_ir_reciprocal_mesh(
         self,
@@ -387,15 +389,15 @@
         use_magmoms (bool): Whether to consider magnetic moments (cf.
         get_initial_magnetic_moments())
         use_elements (bool): If False, chemical elements will be ignored
         symprec (float): Symmetry search precision
         angle_tolerance (float): Angle search tolerance
 
     Returns:
-        symmetry (:class:`pyiron.atomistics.structure.symmetry.Symmetry`): Symmetry class
+        symmetry (:class:`structuretoolkit.analyse.symmetry.Symmetry`): Symmetry class
 
 
     """
     return Symmetry(
         structure=structure,
         use_magmoms=use_magmoms,
         use_elements=use_elements,
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/build/aimsgb.py` & `structuretoolkit-0.0.3/structuretoolkit/build/aimsgb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from aimsgb import GrainBoundary, Grain, GBInformation
-from pymatgen.io.ase import AseAtomsAdaptor
+from structuretoolkit.common.pymatgen import ase_to_pymatgen, pymatgen_to_ase
 
 __author__ = "Ujjal Saikia"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Liam Huber"
 __email__ = "huber@mpie.de"
 __status__ = "production"
 __date__ = "Feb 26, 2021"
 
 
-def grainboundary_info(axis, max_sigma):
+def get_grainboundary_info(axis, max_sigma):
     """
     Provides a list of possible GB structures for a given rotational axis and upto the given maximum sigma value.
 
     Args:
         axis : Rotational axis for the GB you want to construct (for example, axis=[1,0,0])
         max_sigma (int) : The maximum value of sigma upto which you want to consider for your
         GB (for example, sigma=5)
@@ -33,18 +32,19 @@
             'plane': the GB planes")
             'rot_matrix': array([the rotational matrix]),
             'csl': [array([the csl matrix])]}}
 
     To construct the grain boundary select a GB plane and sigma value from the list and pass it to the
     GBBuilder.gb_build() function along with the rotational axis and initial bulk structure.
     """
+    from aimsgb import GBInformation
     return GBInformation(axis=axis, max_sigma=max_sigma)
 
 
-def grainboundary_build(
+def grainboundary(
     axis,
     sigma,
     plane,
     initial_struct,
     to_primitive=False,
     delete_layer="0b0t0b0t",
     add_if_dist=0.0,
@@ -54,15 +54,15 @@
     """
     Generate a grain boundary structure based on the aimsgb.GrainBoundary module.
 
     Args:
         axis : Rotational axis for the GB you want to construct (for example, axis=[1,0,0])
         sigma (int) : The sigma value of the GB you want to construct (for example, sigma=5)
         plane: The grain boundary plane of the GB you want to construct (for example, plane=[2,1,0])
-        initial_struct : Initial bulk structure from which you want to construct the GB (a pyiron
+        initial_struct : Initial bulk structure from which you want to construct the GB (a ase
                         structure object).
         delete_layer : To delete layers of the GB. For example, delete_layer='1b0t1b0t'. The first
                        4 characters is for first grain and the other 4 is for second grain. b means
                        bottom layer and t means top layer. Integer represents the number of layers
                        to be deleted. The first t and second b from the left hand side represents
                        the layers at the GB interface. Default value is delete_layer='0b0t0b0t', which
                        means no deletion of layers.
@@ -72,28 +72,28 @@
                         to_primitive=False
         uc_a (int): Number of unit cell of grain A. Default to 1.
         uc_b (int): Number of unit cell of grain B. Default to 1.
 
     Returns:
         :class:`.Atoms`: final grain boundary structure
     """
-    adapter = AseAtomsAdaptor()
-    basis_pymatgen = adapter.get_structure(atoms=initial_struct, cls=None)
+    from aimsgb import GrainBoundary, Grain
+    basis_pymatgen = ase_to_pymatgen(structure=initial_struct)
     grain_init = Grain(
         basis_pymatgen.lattice, basis_pymatgen.species, basis_pymatgen.frac_coords
     )
     gb_obj = GrainBoundary(
         axis=axis,
         sigma=sigma,
         plane=plane,
         initial_struct=grain_init,
         uc_a=uc_a,
         uc_b=uc_b,
     )
 
-    return adapter.get_atoms(
+    return pymatgen_to_ase(
         structure=gb_obj.build_gb(
             to_primitive=to_primitive,
             delete_layer=delete_layer,
             add_if_dist=add_if_dist,
         )
     )
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/build/compound.py` & `structuretoolkit-0.0.3/structuretoolkit/build/compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.2/structuretoolkit/build/sqs.py` & `structuretoolkit-0.0.3/structuretoolkit/build/sqs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import random
 import warnings
 import itertools
 from multiprocessing import cpu_count
 from ase.data import atomic_numbers
 from ase.atoms import Atoms
 import numpy as np
-from sqsgenerator import sqs_optimize
 from typing import Dict, Optional, Union, Iterable
 
 
 def chemical_formula(atoms: Atoms) -> str:
     def group_symbols():
         for species, same in itertools.groupby(atoms.get_chemical_symbols()):
             num_same = len(list(same))
@@ -97,15 +96,15 @@
     )
 
 
 def transpose(it):
     return zip(*it)
 
 
-def get_sqs_structures(
+def sqs_structures(
     structure: Atoms,
     mole_fractions: Dict[str, Union[float, int]],
     weights: Optional[Dict[int, float]] = None,
     objective: Union[float, np.ndarray] = 0.0,
     iterations: Union[float, int] = 1e6,
     output_structures: int = 10,
     mode: str = "random",
@@ -114,15 +113,17 @@
     pair_weights: Optional[np.ndarray] = None,
     rtol: Optional[float] = None,
     atol: Optional[float] = None,
     which: Optional[Iterable[int]] = None,
     shell_distances: Optional[Iterable[int]] = None,
     minimal: Optional[bool] = True,
     similar: Optional[bool] = True,
+    return_statistics: Optional[bool] = False,
 ):
+    from sqsgenerator import sqs_optimize
     composition = mole_fractions_to_composition(mole_fractions, len(structure))
 
     settings = dict(
         atol=atol,
         rtol=rtol,
         mode=mode,
         which=which,
@@ -147,8 +148,11 @@
         make_structures=True,
         structure_format="ase",
     )
 
     structures, sro_breakdown = transpose(map(remap_sqs_results, results.values()))
     num_iterations = iterations
     cycle_time = np.average(list(map_dict(np.average, timings).values()))
-    return structures, sro_breakdown, num_iterations, cycle_time
+    if not return_statistics:
+        return structures
+    else:
+        return structures, sro_breakdown, num_iterations, cycle_time
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/build/surface.py` & `structuretoolkit-0.0.3/structuretoolkit/build/surface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 from ase.build import bulk, surface
-from structuretoolkit.analyse.symmetry import get_symmetry
-from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-from pymatgen.io.ase import AseAtomsAdaptor
+from structuretoolkit.analyse import get_symmetry
+from structuretoolkit.common.pymatgen import ase_to_pymatgen, pymatgen_to_ase
 
 
-def high_index_surface_info(
+def get_high_index_surface_info(
         element,
         crystal_structure,
         lattice_constant,
         terrace_orientation=None,
         step_orientation=None,
         kink_orientation=None,
         step_down_vector=None,
@@ -130,35 +129,35 @@
         length_terrace (int): The length of the terrace along the kink direction in atoms. default: 3
         length_step (int): The length of the step along the step direction in atoms. default: 3
         length_kink (int): The length of the kink along the kink direction in atoms. default: 1
         layers (int): Number of layers of the high_index_surface. default: 60
         vacuum (float): Thickness of vacuum on the top of the slab. default:10
 
     Returns:
-        slab: pyiron_atomistics.atomistics.structure.atoms.Atoms instance Required surface
+        slab: ase.atoms.Atoms instance Required surface
     """
+    from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     basis = bulk(
         name=element,
         crystalstructure=crystal_structure,
         a=lattice_constant,
         cubic=True
     )
-    high_index_surface, _, _ = high_index_surface_info(
+    high_index_surface, _, _ = get_high_index_surface_info(
         element=element,
         crystal_structure=crystal_structure,
         lattice_constant=lattice_constant,
         terrace_orientation=terrace_orientation,
         step_orientation=step_orientation,
         kink_orientation=kink_orientation,
         step_down_vector=step_down_vector,
         length_step=length_step,
         length_terrace=length_terrace,
         length_kink=length_kink,
     )
     surf = surface(basis, high_index_surface, layers, vacuum)
-    adapter = AseAtomsAdaptor()
-    sga = SpacegroupAnalyzer(adapter.get_structure(atoms=surf))
-    pmg_refined = sga.get_refined_structure()
-    slab = adapter.get_atoms(structure=pmg_refined)
+    slab = pymatgen_to_ase(
+        SpacegroupAnalyzer(ase_to_pymatgen(structure=surf)).get_refined_structure()
+    )
     slab.positions[:, 2] = slab.positions[:, 2] - np.min(slab.positions[:, 2])
     slab.set_pbc(True)
     return slab
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/helper.py` & `structuretoolkit-0.0.3/structuretoolkit/common/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
     Args:
         structure (ase.atoms.Atoms):
         origin (float):  0 to confine between 0 and 1, -0.5 to confine between -0.5 and 0.5
         eps (float): Tolerance to detect atoms at cell edges
 
     Returns:
-        :class:`pyiron_atomistics.atomistics.structure.atoms.Atoms`: reference to this structure
+        :class:`ase.atoms.Atoms`: reference to this structure
     """
     if any(structure.pbc):
         structure.set_scaled_positions(
             np.mod(structure.get_scaled_positions(wrap=False) + eps, 1) - eps + origin
         )
     return structure
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit/visualize.py` & `structuretoolkit-0.0.3/structuretoolkit/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 import warnings
-from matplotlib.colors import rgb2hex
 from scipy.interpolate import interp1d
-from structuretoolkit.helper import get_atomic_numbers
+from structuretoolkit.common.helper import get_atomic_numbers
 
 __author__ = "Joerg Neugebauer, Sudarsan Surendralal"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -648,14 +647,16 @@
         end (float): Scalar value to map to the top of the colormap (values above are clipped).  (Default is
             None, use the maximal scalar value.)
         cmap (matplotlib.cm): The colormap to use. (Default is None, which gives a blue-red divergent map.)
 
     Returns:
         (list): The corresponding hex codes for each scalar value passed in.
     """
+    from matplotlib.colors import rgb2hex
+
     if start is None:
         start = np.amin(scalar_field)
     if end is None:
         end = np.amax(scalar_field)
     interp = interp1d([start, end], [0, 1])
     remapped_field = interp(np.clip(scalar_field, start, end))  # Map field onto [0,1]
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit.egg-info/PKG-INFO` & `structuretoolkit-0.0.3/structuretoolkit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.2
+Version: 0.0.3
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,10 +12,18 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: grainboundary
+Provides-Extra: pyscal
+Provides-Extra: nglview
+Provides-Extra: plotly
+Provides-Extra: clusters
+Provides-Extra: symmetry
+Provides-Extra: surface
+Provides-Extra: phonopy
 License-File: LICENSE
 
 http://pyiron.org
```

### Comparing `structuretoolkit-0.0.2/structuretoolkit.egg-info/SOURCES.txt` & `structuretoolkit-0.0.3/structuretoolkit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 structuretoolkit/__init__.py
 structuretoolkit/_version.py
-structuretoolkit/helper.py
 structuretoolkit/visualize.py
 structuretoolkit.egg-info/PKG-INFO
 structuretoolkit.egg-info/SOURCES.txt
 structuretoolkit.egg-info/dependency_links.txt
 structuretoolkit.egg-info/requires.txt
 structuretoolkit.egg-info/top_level.txt
 structuretoolkit/analyse/__init__.py
@@ -22,14 +21,19 @@
 structuretoolkit/analyse/strain.py
 structuretoolkit/analyse/symmetry.py
 structuretoolkit/build/__init__.py
 structuretoolkit/build/aimsgb.py
 structuretoolkit/build/compound.py
 structuretoolkit/build/sqs.py
 structuretoolkit/build/surface.py
+structuretoolkit/common/__init__.py
+structuretoolkit/common/error.py
+structuretoolkit/common/helper.py
+structuretoolkit/common/pymatgen.py
+structuretoolkit/common/pyscal.py
 tests/test_aimsgb.py
 tests/test_analyse.py
 tests/test_compound.py
 tests/test_high_index_surface.py
 tests/test_neighbors.py
 tests/test_pyscal.py
 tests/test_strain.py
```

### Comparing `structuretoolkit-0.0.2/tests/test_aimsgb.py` & `structuretoolkit-0.0.3/tests/test_aimsgb.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,31 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import unittest
 from ase.build import bulk
 import structuretoolkit as stk
 
+try:
+    import aimsgb
+    skip_aimsgb_test = False
+except ImportError:
+    skip_aimsgb_test = True
 
+
+@unittest.skipIf(skip_aimsgb_test, "aimsgb is not installed, so the aimsgb tests are skipped.")
 class TestAimsgb(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.fcc_basis = bulk('Al', cubic = True)
 
     def test_grain_thickness(self):
         axis = [0, 0, 1]
         sigma = 5
         plane = [1, 2, 0]
-        gb1 = stk.grainboundary_build(axis, sigma, plane, self.fcc_basis)  # Default thicknesses expected to be 1
+        gb1 = stk.build.grainboundary(axis, sigma, plane, self.fcc_basis)  # Default thicknesses expected to be 1
         uc_a, uc_b = 2, 3  # Make grains thicker
-        gb2 = stk.grainboundary_build(axis, sigma, plane, self.fcc_basis, uc_a=uc_a, uc_b=uc_b)
+        gb2 = stk.build.grainboundary(axis, sigma, plane, self.fcc_basis, uc_a=uc_a, uc_b=uc_b)
         self.assertEqual(
             ((uc_a + uc_b)/2)*len(gb1), len(gb2),
             msg="Expected structure to be bigger in proportion to grain thickness"
         )
```

### Comparing `structuretoolkit-0.0.2/tests/test_analyse.py` & `structuretoolkit-0.0.3/tests/test_analyse.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,134 +5,156 @@
 import unittest
 import numpy as np
 from ase.build import bulk
 from ase.atom import Atom
 from ase.atoms import Atoms
 from scipy.spatial import Voronoi
 from ase.lattice.cubic import BodyCenteredCubic
-from sklearn.cluster import AgglomerativeClustering, DBSCAN
 import structuretoolkit as stk
 
 
+try:
+    from sklearn.cluster import AgglomerativeClustering, DBSCAN
+    skip_cluster_test = False
+except ImportError:
+    skip_cluster_test = True
+
+
+try:
+    import pyscal
+    skip_pyscal_test = False
+except ImportError:
+    skip_pyscal_test = True
+
+
 class TestAtoms(unittest.TestCase):
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_layers(self):
         a_0 = 4
         struct = bulk(name='Al', a=a_0, crystalstructure='fcc', cubic=True).repeat(10)
         struct_pure = struct.copy()
-        layers = stk.get_layers(structure=struct)
+        layers = stk.analyse.get_layers(structure=struct)
         self.assertAlmostEqual(np.linalg.norm(layers-np.rint(2*struct.positions/a_0).astype(int)), 0)
         struct.append(Atom(symbol='C', position=np.random.random(3)))
         self.assertEqual(
-            np.linalg.norm(layers-stk.get_layers(structure=struct, id_list=stk.select_index(structure=struct, element='Al'))), 0
+            np.linalg.norm(layers-stk.analyse.get_layers(structure=struct, id_list=stk.common.select_index(structure=struct, element='Al'))), 0
         )
         self.assertEqual(
-            np.linalg.norm(layers-stk.get_layers(
+            np.linalg.norm(layers-stk.analyse.get_layers(
                 structure=struct,
-                id_list=stk.select_index(structure=struct, element='Al'),
+                id_list=stk.common.select_index(structure=struct, element='Al'),
                 wrap_atoms=False
             )), 0
         )
         with self.assertRaises(ValueError):
-            _ = stk.get_layers(structure=struct, distance_threshold=0)
+            _ = stk.analyse.get_layers(structure=struct, distance_threshold=0)
         with self.assertRaises(ValueError):
-            _ = stk.get_layers(structure=stk, id_list=[])
+            _ = stk.analyse.get_layers(structure=struct, id_list=[])
 
-        self.assertTrue(np.all(stk.get_layers(structure=struct) == stk.get_layers(
+        self.assertTrue(np.all(stk.analyse.get_layers(structure=struct) == stk.analyse.get_layers(
             structure=struct,
             cluster_method=AgglomerativeClustering(
                 linkage='complete',
                 n_clusters=None,
                 distance_threshold=0.01
             ))
         ), "Overriding cluster method with default parameters does not return the same results.")
         self.assertTrue(
             np.all(
-                stk.get_layers(structure=struct_pure) == stk.get_layers(
+                stk.analyse.get_layers(structure=struct_pure) == stk.analyse.get_layers(
                     structure=struct_pure,
                     cluster_method=DBSCAN(eps=0.01)
                 )
             ),
             "Overriding cluster method with DBSCAN does not return the same results for symmetric structure."
         )
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_layers_other_planes(self):
         structure = bulk(name='Fe', a=3.5, crystalstructure='fcc', cubic=True).repeat(2)
-        layers = stk.get_layers(structure=structure, planes=[1, 1, 1])
+        layers = stk.analyse.get_layers(structure=structure, planes=[1, 1, 1])
         self.assertEqual(np.unique(layers).tolist(), [0, 1, 2, 3, 4])
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_layers_with_strain(self):
         structure = bulk(name='Fe', a=2.8, crystalstructure='bcc', cubic=True).repeat(2)
-        layers = stk.get_layers(structure=structure).tolist()
-        stk.apply_strain(structure=structure, epsilon=0.1*(np.random.random((3, 3))-0.5))
+        layers = stk.analyse.get_layers(structure=structure).tolist()
+        stk.common.apply_strain(structure=structure, epsilon=0.1*(np.random.random((3, 3))-0.5))
         self.assertEqual(
-            layers, stk.get_layers(structure=structure, planes=np.linalg.inv(structure.cell).T).tolist()
+            layers, stk.analyse.get_layers(structure=structure, planes=np.linalg.inv(structure.cell).T).tolist()
         )
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_layers_across_pbc(self):
         structure = bulk(name='Fe', a=2.8, crystalstructure='bcc', cubic=True).repeat(2)
-        layers = stk.get_layers(structure=structure)
+        layers = stk.analyse.get_layers(structure=structure)
         structure.cell[1, 0] += 0.01
-        structure = stk.center_coordinates_in_unit_cell(structure=structure)
-        self.assertEqual(len(np.unique(layers[stk.get_layers(structure=structure)[:, 0] == 0, 0])), 1)
+        structure = stk.common.center_coordinates_in_unit_cell(structure=structure)
+        self.assertEqual(len(np.unique(layers[stk.analyse.get_layers(structure=structure)[:, 0] == 0, 0])), 1)
 
+    @unittest.skipIf(skip_pyscal_test, "pyscal is not installed, so the pyscal tests are skipped.")
     def test_pyscal_cna_adaptive(self):
         basis = Atoms(
             "FeFe", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=np.identity(3)
         )
         self.assertTrue(
-            stk.analyse_cna_adaptive(structure=basis)["bcc"] == 2
+            stk.analyse.get_adaptive_cna_descriptors(structure=basis)["bcc"] == 2
         )
 
+    @unittest.skipIf(skip_pyscal_test, "pyscal is not installed, so the pyscal tests are skipped.")
     def test_pyscal_centro_symmetry(self):
         basis = bulk(name='Fe', a=2.8, crystalstructure='bcc', cubic=True)
         self.assertTrue(
-            all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(structure=basis, num_neighbors=8)])
+            all([np.isclose(v, 0.0) for v in stk.analyse.get_centro_symmetry_descriptors(structure=basis, num_neighbors=8)])
         )
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_voronoi_vertices(self):
         basis = bulk(name='Al', a=4, crystalstructure='fcc', cubic=True)
-        self.assertEqual(len(stk.get_voronoi_vertices(structure=basis)), 12)
-        self.assertEqual(len(stk.get_voronoi_vertices(structure=basis, distance_threshold=2)), 1)
+        self.assertEqual(len(stk.analyse.get_voronoi_vertices(structure=basis)), 12)
+        self.assertEqual(len(stk.analyse.get_voronoi_vertices(structure=basis, distance_threshold=2)), 1)
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_interstitials_bcc(self):
         bcc = bulk('Fe', cubic=True)
         x_octa_ref = bcc.positions[:, None, :]+0.5*bcc.cell[None, :, :]
         x_octa_ref = x_octa_ref.reshape(-1, 3)
-        x_octa_ref = stk.get_wrapped_coordinates(structure=bcc, positions=x_octa_ref)
-        int_octa = stk.get_interstitials(structure=bcc, num_neighbors=6)
+        x_octa_ref = stk.common.get_wrapped_coordinates(structure=bcc, positions=x_octa_ref)
+        int_octa = stk.analyse.get_interstitials(structure=bcc, num_neighbors=6)
         self.assertEqual(len(int_octa.positions), len(x_octa_ref))
         self.assertAlmostEqual(
             np.linalg.norm(
                 x_octa_ref[:, None, :]-int_octa.positions[None, :, :], axis=-1
             ).min(axis=0).sum(), 0
         )
-        int_tetra = stk.get_interstitials(structure=bcc, num_neighbors=4)
-        x_tetra_ref = stk.get_wrapped_coordinates(structure=bcc, positions=stk.get_voronoi_vertices(structure=bcc))
+        int_tetra = stk.analyse.get_interstitials(structure=bcc, num_neighbors=4)
+        x_tetra_ref = stk.common.get_wrapped_coordinates(structure=bcc, positions=stk.analyse.get_voronoi_vertices(structure=bcc))
         self.assertEqual(len(int_tetra.positions), len(x_tetra_ref))
         self.assertAlmostEqual(
             np.linalg.norm(
                 x_tetra_ref[:, None, :]-int_tetra.positions[None, :, :], axis=-1
             ).min(axis=0).sum(), 0
         )
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_get_interstitials_fcc(self):
         fcc = bulk('Al', cubic=True)
         a_0 = fcc.cell[0, 0]
         x_tetra_ref = 0.25*a_0*np.ones(3)*np.array([[1], [-1]])+fcc.positions[:, None, :]
-        x_tetra_ref = stk.get_wrapped_coordinates(structure=fcc, positions=x_tetra_ref).reshape(-1, 3)
-        int_tetra = stk.get_interstitials(structure=fcc, num_neighbors=4)
+        x_tetra_ref = stk.common.get_wrapped_coordinates(structure=fcc, positions=x_tetra_ref).reshape(-1, 3)
+        int_tetra = stk.analyse.get_interstitials(structure=fcc, num_neighbors=4)
         self.assertEqual(len(int_tetra.positions), len(x_tetra_ref))
         self.assertAlmostEqual(
             np.linalg.norm(
                 x_tetra_ref[:, None, :]-int_tetra.positions[None, :, :], axis=-1
             ).min(axis=0).sum(), 0
         )
         x_octa_ref = 0.5*a_0*np.array([1, 0, 0])+fcc.positions
-        x_octa_ref = stk.get_wrapped_coordinates(structure=fcc, positions=x_octa_ref)
-        int_octa = stk.get_interstitials(structure=fcc, num_neighbors=6)
+        x_octa_ref = stk.common.get_wrapped_coordinates(structure=fcc, positions=x_octa_ref)
+        int_octa = stk.analyse.get_interstitials(structure=fcc, num_neighbors=6)
         self.assertEqual(len(int_octa.positions), len(x_octa_ref))
         self.assertAlmostEqual(
             np.linalg.norm(x_octa_ref[:, None, :]-int_octa.positions[None, :, :], axis=-1).min(axis=0).sum(), 0
         )
         self.assertTrue(
             np.allclose(int_octa.get_areas(), a_0**2*np.sqrt(3)),
             msg='Convex hull area comparison with analytical value failed'
@@ -162,44 +184,45 @@
             symbol='Fe', directions=[[-1, 0, 1], [1, -2, 1], [1, 1, 1]], latticeconstant=a_0
         )
         L = 100
         structure = structure.repeat((*np.rint(L/structure.cell.diagonal()[:2]).astype(int), 1))
         voro = Voronoi(structure.positions[:, :2])
         center = voro.vertices[np.linalg.norm(voro.vertices-structure.cell.diagonal()[:2]*0.5, axis=-1).argmin()]
         structure.positions[:, 2] += b/(2*np.pi)*np.arctan2(*(structure.positions[:, :2]-center).T[::-1])
-        structure = stk.center_coordinates_in_unit_cell(structure=structure)
+        structure = stk.common.center_coordinates_in_unit_cell(structure=structure)
         r_0 = 0.9*L/2
         r = np.linalg.norm(structure.positions[:, :2]-center, axis=-1)
         core_region = (r < r_0)*(r > 10)
-        strain = stk.get_strain(structure=structure, ref_structure=structure_bulk, num_neighbors=8)
+        strain = stk.analyse.get_strain(structure=structure, ref_structure=structure_bulk, num_neighbors=8)
         strain = strain[core_region]
         positions = structure.positions[core_region, :2]
         x = positions-center
         eps_yz = b/(4*np.pi)*x[:, 0]/np.linalg.norm(x, axis=-1)**2
         eps_xz = -b/(4*np.pi)*x[:, 1]/np.linalg.norm(x, axis=-1)**2
         self.assertLess(np.absolute(eps_yz-strain[:, 1, 2]).max(), 0.01)
         self.assertLess(np.absolute(eps_xz-strain[:, 0, 2]).max(), 0.01)
 
     def test_tessellations(self):
         structure_bulk = bulk('Fe', cubic=True)
         a_0 = structure_bulk.cell[0, 0]
         structure = structure_bulk.repeat(3)
-        self.assertAlmostEqual(np.linalg.norm(stk.find_mic(structure=structure, v=np.diff(
-            structure.positions[stk.get_delaunay_neighbors(structure=structure)], axis=-2
+        self.assertAlmostEqual(np.linalg.norm(stk.analyse.find_mic(structure=structure, v=np.diff(
+            structure.positions[stk.analyse.get_delaunay_neighbors(structure=structure)], axis=-2
         )), axis=-1).flatten().max(), a_0)
-        self.assertAlmostEqual(np.linalg.norm(stk.find_mic(structure=structure, v=np.diff(
-            structure.positions[stk.get_voronoi_neighbors(structure=structure)], axis=-2
+        self.assertAlmostEqual(np.linalg.norm(stk.analyse.find_mic(structure=structure, v=np.diff(
+            structure.positions[stk.analyse.get_voronoi_neighbors(structure=structure)], axis=-2
         )), axis=-1).flatten().max(), a_0)
 
+    @unittest.skipIf(skip_cluster_test, "sklearn is not installed, so the cluster tests are skipped.")
     def test_cluster_positions(self):
         structure_bulk = bulk('Fe', cubic=True)
-        self.assertEqual(len(stk.cluster_positions(structure=structure_bulk)), len(structure_bulk))
+        self.assertEqual(len(stk.analyse.get_cluster_positions(structure=structure_bulk)), len(structure_bulk))
         positions = np.append(structure_bulk.positions, structure_bulk.positions, axis=0)
-        self.assertEqual(len(stk.cluster_positions(structure=structure_bulk, positions=positions)), len(structure_bulk))
+        self.assertEqual(len(stk.analyse.get_cluster_positions(structure=structure_bulk, positions=positions)), len(structure_bulk))
         self.assertEqual(
-            stk.cluster_positions(structure=structure_bulk, positions=np.zeros((2, 3)), return_labels=True)[1].tolist(),
+            stk.analyse.get_cluster_positions(structure=structure_bulk, positions=np.zeros((2, 3)), return_labels=True)[1].tolist(),
             [0, 0]
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `structuretoolkit-0.0.2/tests/test_compound.py` & `structuretoolkit-0.0.3/tests/test_compound.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,87 +4,94 @@
 
 
 import unittest
 from ase.build import bulk
 import numpy as np
 import structuretoolkit as stk
 
+try:
+    import spglib
+    skip_spglib_test = False
+except ImportError:
+    skip_spglib_test = True
+
 
 class TestCompound(unittest.TestCase):
     def test_B2(self):
-        structure = stk.B2('Fe', 'Al')
+        structure = stk.build.B2('Fe', 'Al')
         self.assertAlmostEqual(bulk('Fe', cubic=True).cell[0, 0], structure.cell[0, 0],
                                msg="Docstring claims lattice constant defaults to primary species")
         self.assertEqual(2, len(structure))
-        neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
+        neigh = stk.analyse.get_neighbors(structure=structure, num_neighbors=8)
         symbols = np.array(structure.get_chemical_symbols())
         self.assertEqual(8, np.sum(symbols[neigh.indices[0]] == 'Al'),
                          msg="Expected the primary atom to have all secondary neighbors")
         self.assertEqual(8, np.sum(symbols[neigh.indices[1]] == 'Fe'),
                          msg="Expected the secondary atom to have all primary neighbors")
-        structure = stk.B2('Fe', 'Al', a=1)
+        structure = stk.build.B2('Fe', 'Al', a=1)
         self.assertTrue(np.allclose(np.diag(structure.cell.array), 1), "Expected cubic cell with specified size.")
 
     def test_C14(self):
         a_type = 'Mg'
         b_type = 'Cu'
-        c14 = stk.C14(a_type, b_type)
+        c14 = stk.build.C14(a_type, b_type)
         self.assertEqual(len(c14), 12, "Wrong number of atoms in C14 structure.")
         self.assertEqual(c14.get_chemical_formula(), "Cu8Mg4", "Wrong chemical formula.")
 
+    @unittest.skipIf(skip_spglib_test, "spglib is not installed, so the C15 tests are skipped.")
     def test_C15(self):
         """
         Tests based on Xie et al., JMR 2021 (DOI:10.1557/s43578-021-00237-y).
         """
 
         a_type = 'Mg'
         b_type = 'Cu'
-        structure = stk.C15(a_type, b_type)
+        structure = stk.build.C15(a_type, b_type)
 
         self.assertEqual(len(structure), 24, "Wrong number of atoms in C15 structure.")
         self.assertEqual(structure.get_chemical_formula(), "Cu16Mg8", "Wrong chemical formula.")
 
-        a_type_nn_distance = stk.get_neighbors(structure=bulk(a_type), num_neighbors=1).distances[0, 0]
+        a_type_nn_distance = stk.analyse.get_neighbors(structure=bulk(a_type), num_neighbors=1).distances[0, 0]
         self.assertAlmostEqual((4 / np.sqrt(3)) * a_type_nn_distance, structure.cell.array[0, 0],
                                msg="Default lattice constant should relate to NN distance of A-type element.")
 
-        unique_ids = np.unique(stk.get_symmetry(structure)['equivalent_atoms'])
+        unique_ids = np.unique(stk.analyse.get_symmetry(structure)['equivalent_atoms'])
         self.assertEqual(2, len(unique_ids), msg="Expected only A- and B1-type sites.")
         symbols = np.array(structure.get_chemical_symbols())
         a_id = unique_ids[np.argwhere(symbols[unique_ids] == a_type)[0, 0]]
         b_id = unique_ids[np.argwhere(symbols[unique_ids] == b_type)[0, 0]]
         unique_ids = [a_id, b_id]  # Now with guaranteed ordering
 
-        csa = stk.analyse_centro_symmetry(structure)[unique_ids]
+        csa = stk.analyse.get_centro_symmetry_descriptors(structure)[unique_ids]
         self.assertLess(1, csa[0], msg="A site for AB_2 C15 should be significantly non-centro-symmetric.")
         self.assertAlmostEqual(0, csa[1], msg="B site for AB_2 C15 should be nearly centro-symmetric.")
 
         num_a_neighs = 16
         num_b_neighs = 12
-        neigh = stk.get_neighbors(structure=structure, num_neighbors=num_a_neighs)
+        neigh = stk.analyse.get_neighbors(structure=structure, num_neighbors=num_a_neighs)
         a_neighs = neigh.indices[unique_ids[0]]
         b_neighs = neigh.indices[unique_ids[1], :num_b_neighs]
         symbols = np.array(structure.get_chemical_symbols())
         self.assertEqual(4, np.sum(symbols[a_neighs] == a_type))
         self.assertEqual(12, np.sum(symbols[a_neighs] == b_type))
         self.assertEqual(6, np.sum(symbols[b_neighs] == a_type))
         self.assertEqual(6, np.sum(symbols[b_neighs] == b_type))
 
     def test_C36(self):
         a_type = 'Mg'
         b_type = 'Cu'
-        c36 = stk.C36(a_type, b_type)
+        c36 = stk.build.C36(a_type, b_type)
         self.assertEqual(len(c36), 24, "Wrong number of atoms in C36 structure.")
         self.assertEqual(c36.get_chemical_formula(), "Cu16Mg8", "Wrong chemical formula.")
 
     def test_D03(self):
         element_a, element_b = 'Al', 'Fe'
-        structure = stk.D03(element_a, element_b)
+        structure = stk.build.D03(element_a, element_b)
         symbols = np.array(structure.get_chemical_symbols())
-        neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
+        neigh = stk.analyse.get_neighbors(structure=structure, num_neighbors=8)
 
         a_neighbors = neigh.indices[symbols == element_a]
         self.assertTrue(np.all(symbols[a_neighbors] == element_b), msg="A-type should only have B-type neighbors.")
 
         b_neighbors = neigh.indices[symbols == element_b]
         sorted_vals, counts = np.unique(np.mean(symbols[b_neighbors] == 'Al', axis=1), return_counts=True)
         self.assertAlmostEqual(0, sorted_vals[0], msg="Shared sub-lattice has no A-type neighbors.")
```

### Comparing `structuretoolkit-0.0.2/tests/test_neighbors.py` & `structuretoolkit-0.0.3/tests/test_neighbors.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,71 +5,84 @@
 import unittest
 import numpy as np
 from ase.build import bulk
 import structuretoolkit as stk
 from ase.atoms import Atoms
 import warnings
 
+try:
+    import pyscal
+    skip_pyscal_test = False
+except ImportError:
+    skip_pyscal_test = True
+
+
+try:
+    import sklearn
+    skip_sklearn_test = False
+except ImportError:
+    skip_sklearn_test = True
+
 
 class TestAtoms(unittest.TestCase):
     @classmethod
     def tearDownClass(cls):
         pass
 
     @classmethod
     def setUpClass(cls):
         pass
 
     def test_allow_ragged(self):
         struct = bulk('Al', a=4, cubic=True).repeat(10)
         del struct[0]
-        neigh = stk.get_neighbors(structure=struct, cutoff_radius=3, mode="ragged")
+        neigh = stk.analyse.get_neighbors(structure=struct, cutoff_radius=3, mode="ragged")
         self.assertTrue(neigh._mode["ragged"])
         self.assertTrue(isinstance(neigh.indices, list))
         indices = neigh.indices.copy()
         neigh._set_mode(neigh._allow_ragged_to_mode(False))
         self.assertTrue(isinstance(neigh.indices, np.ndarray))
         self.assertGreater(len(neigh.indices[0]), len(indices[0]))
         with self.assertRaises(IndexError):
             struct.positions[neigh.indices] = struct.positions[neigh.indices]
         neigh._set_mode(neigh._allow_ragged_to_mode(True))
         self.assertTrue(np.array_equal(neigh.indices[0], indices[0]))
-        neigh = stk.get_neighbors(structure=struct, cutoff_radius=3, num_neighbors=None)
+        neigh = stk.analyse.get_neighbors(structure=struct, cutoff_radius=3, num_neighbors=None)
         self.assertFalse(neigh._mode["ragged"])
         self.assertTrue(isinstance(neigh.indices, np.ndarray))
 
     def test_getter_and_ragged(self):
         struct = bulk('Al', a=4, cubic=True).repeat(2)
         del struct[0]
-        neigh = stk.get_neighbors(structure=struct, cutoff_radius=3, mode='filled')
+        neigh = stk.analyse.get_neighbors(structure=struct, cutoff_radius=3, mode='filled')
         vecs = neigh.filled.vecs
         distances = neigh.filled.distances
         indices = neigh.filled.indices
         self.assertTrue(np.array_equal(neigh.distances, distances))
         self.assertTrue(np.array_equal(neigh.indices, indices))
         self.assertTrue(np.array_equal(neigh.vecs, vecs))
 
     def test_get_neighborhood_single(self):
         struct = bulk('Al', a=4, cubic=True)
-        neigh = stk.get_neighborhood(structure=struct, positions=np.random.random(3), cutoff_radius=3)
+        neigh = stk.analyse.get_neighborhood(structure=struct, positions=np.random.random(3), cutoff_radius=3)
         distances = neigh.distances.copy()
         neigh.allow_ragged = False
         self.assertTrue(np.array_equal(neigh.distances, distances))
         neigh.allow_ragged = True
         self.assertTrue(np.array_equal(neigh.distances, distances))
         neigh.allow_ragged = False
         self.assertTrue(np.array_equal(neigh.distances, distances))
 
     def test_get_neighbors(self):
         struct = bulk('Fe', a=2.85, cubic=True).repeat(10)
         cell = struct.cell.copy()
         cell += np.random.random((3, 3))-0.5
         struct.positions += np.random.random((len(struct), 3))-0.5
         struct.set_cell(cell, scale_atoms=True)
-        neigh = stk.get_neighbors(structure=struct)
+        neigh = stk.analyse.get_neighbors(structure=struct)
         self.assertAlmostEqual(
             np.absolute(neigh.distances-np.linalg.norm(neigh.vecs, axis=-1)).max(), 0
         )
         myself = np.ones_like(neigh.indices)
         myself = myself*np.arange(len(myself))[:,np.newaxis]
         dist = struct.get_distances(myself.flatten(), neigh.indices.flatten(), mic=True)
         self.assertAlmostEqual(np.absolute(dist-neigh.distances.flatten()).max(), 0)
@@ -87,319 +100,339 @@
 
     def test_pbc_false(self):
         struct = bulk('Fe', a=2.85, cubic=True).repeat(10)
         struct.pbc = False
         cell = struct.cell.copy()
         cell += np.random.random((3, 3))-0.5
         struct.set_cell(cell, scale_atoms=True)
-        neigh = stk.get_neighbors(structure=struct)
+        neigh = stk.analyse.get_neighbors(structure=struct)
         self.assertAlmostEqual(
             np.absolute(neigh.distances-np.linalg.norm(neigh.vecs, axis=-1)).max(), 0
         )
         myself = np.ones_like(neigh.indices)
         myself = myself*np.arange(len(myself))[:,np.newaxis]
         dist = np.linalg.norm(
             struct.positions[myself]-struct.positions[neigh.indices], axis=-1
         )
         self.assertAlmostEqual(np.absolute(dist-neigh.distances).max(), 0)
 
     def test_fe_large(self):
         struct = bulk('Fe', a=2.85, cubic=True).repeat(10)
-        neigh = stk.get_neighbors(structure=struct)
+        neigh = stk.analyse.get_neighbors(structure=struct)
         self.assertAlmostEqual(
             np.absolute(neigh.distances-np.linalg.norm(neigh.vecs, axis=-1)).max(), 0
         )
         self.assertAlmostEqual(neigh.vecs[neigh.shells == 1].sum(), 0)
         self.assertAlmostEqual(neigh.vecs[0, neigh.shells[0] == 1].sum(), 0)
 
     def test_fe_small(self):
         struct = bulk('Fe', a=2.85, cubic=True)
-        neigh = stk.get_neighbors(structure=struct)
+        neigh = stk.analyse.get_neighbors(structure=struct)
         self.assertAlmostEqual(neigh.vecs[neigh.shells == 1].sum(), 0)
         with self.assertRaises(ValueError):
-            _ = stk.get_neighbors(structure=struct, num_neighbors=None)
+            _ = stk.analyse.get_neighbors(structure=struct, num_neighbors=None)
 
     def test_al_large(self):
         struct = bulk('Al', a=4.04, cubic=True).repeat(10)
-        neigh = stk.get_neighbors(structure=struct)
+        neigh = stk.analyse.get_neighbors(structure=struct)
         self.assertAlmostEqual(
             np.absolute(neigh.distances-np.linalg.norm(neigh.vecs, axis=-1)).max(), 0
         )
         self.assertAlmostEqual(neigh.vecs[neigh.shells == 1].sum(), 0)
         self.assertAlmostEqual(neigh.vecs[0, neigh.shells[0] == 1].sum(), 0)
 
     def test_al_small(self):
         struct = bulk('Al', a=4.04, cubic=True)
-        neigh = stk.get_neighbors(structure=struct)
+        neigh = stk.analyse.get_neighbors(structure=struct)
         self.assertAlmostEqual(
             np.absolute(neigh.distances-np.linalg.norm(neigh.vecs, axis=-1)).max(), 0
         )
         self.assertAlmostEqual(neigh.vecs[neigh.shells == 1].sum(), 0)
         with self.assertRaises(ValueError):
-            stk.get_neighbors(structure=struct, num_neighbors=0)
+            stk.analyse.get_neighbors(structure=struct, num_neighbors=0)
 
     def test_wrapped_positions(self):
         structure = bulk('Al', a=4, cubic=True).repeat(2)
-        neigh = stk.get_neighbors(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         distances = neigh.distances
         new_positions = structure.positions+structure.cell.diagonal()*2
         self.assertFalse(
             np.all(np.isclose(distances, neigh.get_neighborhood(new_positions, num_neighbors=13).distances[:,1:]))
         )
         neigh.wrap_positions = True
         self.assertTrue(
             np.all(np.isclose(distances, neigh.get_neighborhood(new_positions, num_neighbors=13).distances[:,1:]))
         )
 
+    @unittest.skipIf(
+        skip_sklearn_test,
+        "scikit-learn is not installed, so the clustering tests are skipped."
+    )
     def test_get_global_shells(self):
         structure = bulk('Al', a=4, cubic=True).repeat(2)
-        neigh = stk.get_neighbors(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         self.assertTrue(np.array_equal(neigh.shells, neigh.get_global_shells()))
         structure += Atoms(symbols='C', positions=[[0, 0, 0.5*4]])
-        neigh = stk.get_neighbors(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         self.assertFalse(np.array_equal(neigh.shells, neigh.get_global_shells()))
         structure = bulk('Al', a=4, cubic=True).repeat(2)
-        neigh = stk.get_neighbors(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         shells = neigh.get_global_shells()
         structure.positions += 0.01*(np.random.random((len(structure), 3))-0.5)
-        stk.center_coordinates_in_unit_cell(structure=structure)
-        neigh = stk.get_neighbors(structure=structure)
+        stk.common.center_coordinates_in_unit_cell(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         self.assertTrue(
             np.array_equal(
                 shells, neigh.get_global_shells(cluster_by_vecs=True, cluster_by_distances=True)
             )
         )
         neigh.reset_clusters()
         self.assertTrue(np.array_equal(shells, neigh.get_global_shells(cluster_by_vecs=True)))
         self.assertFalse(np.array_equal(shells, neigh.get_global_shells()))
 
+    @unittest.skipIf(
+        skip_sklearn_test,
+        "scikit-learn is not installed, so the clustering tests are skipped."
+    )
     def test_get_local_shells(self):
         structure = bulk('Al', a=4, cubic=True).repeat(2)
-        neigh = stk.get_neighbors(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         shells = neigh.get_local_shells()
         structure.positions += 0.01*(np.random.random((len(structure), 3))-0.5)
-        neigh = stk.get_neighbors(structure=structure)
+        neigh = stk.analyse.get_neighbors(structure=structure)
         self.assertTrue(
             np.array_equal(
                 shells, neigh.get_local_shells(cluster_by_vecs=True, cluster_by_distances=True)
             )
         )
         neigh.reset_clusters()
         self.assertTrue(np.array_equal(shells, neigh.get_local_shells(cluster_by_vecs=True)))
         self.assertFalse(np.array_equal(shells, neigh.get_local_shells()))
 
+    @unittest.skipIf(
+        skip_sklearn_test,
+        "scikit-learn is not installed, so the clustering tests are skipped."
+    )
     def test_get_global_shells_ragged(self):
         structure = bulk('Al', a=4, cubic=True).repeat(2)
         del structure[0]
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=3.5, num_neighbors=None)
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=3.5, num_neighbors=None)
         self.assertEqual(np.sum(neigh.get_global_shells() == -1), 12)
         self.assertEqual(np.sum(neigh.get_global_shells(cluster_by_distances=True) == -1), 12)
         self.assertEqual(np.sum(neigh.get_global_shells(cluster_by_vecs=True) == -1), 12)
         self.assertEqual(
             np.sum(neigh.get_global_shells(cluster_by_distances=True, cluster_by_vecs=True)==-1), 12
         )
         neigh._set_mode(neigh._allow_ragged_to_mode(True))
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_global_shells()]), 12)
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_global_shells(cluster_by_distances=True)]), 12)
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_global_shells(cluster_by_vecs=True)]), 12)
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_global_shells(cluster_by_distances=True, cluster_by_vecs=True)]), 12)
 
+    @unittest.skipIf(
+        skip_sklearn_test,
+        "scikit-learn is not installed, so the clustering tests are skipped."
+    )
     def test_get_local_shells_ragged(self):
         structure = bulk('Al', a=4, cubic=True).repeat(2)
         del structure[0]
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=3.5, num_neighbors=None)
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=3.5, num_neighbors=None)
         self.assertEqual(np.sum(neigh.shells == -1), 12)
         self.assertEqual(np.sum(neigh.get_local_shells(cluster_by_distances=True) == -1), 12)
         self.assertEqual(np.sum(neigh.get_local_shells(cluster_by_vecs=True) == -1), 12)
         self.assertEqual(
             np.sum(neigh.get_local_shells(cluster_by_distances=True, cluster_by_vecs=True) == -1), 12
         )
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=3.5, num_neighbors=None, mode='ragged')
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=3.5, num_neighbors=None, mode='ragged')
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.shells]), 12)
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_local_shells(cluster_by_distances=True)]), 12)
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_local_shells(cluster_by_vecs=True)]), 12)
         self.assertEqual(np.sum([len(s) == 11 for s in neigh.get_local_shells(cluster_by_distances=True, cluster_by_vecs=True)]), 12)
 
     def test_get_shells_flattened(self):
         structure = bulk('Al', cubic=True).repeat(2)
         del structure[0]
         r = structure.cell[0, 0]*0.49
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='flattened')
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='flattened')
         self.assertEqual(len(np.unique(neigh.shells)), 1)
         self.assertEqual(len(neigh.shells), 360)
         self.assertEqual(len(np.unique(neigh.get_local_shells())), 1)
         self.assertEqual(len(neigh.get_local_shells()), 360)
         self.assertEqual(len(np.unique(neigh.get_global_shells())), 1)
         self.assertEqual(len(neigh.get_global_shells()), 360)
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None)
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None)
         self.assertEqual(len(np.unique(neigh.flattened.shells)), 1)
         self.assertEqual(len(neigh.flattened.shells), 360)
 
     def test_get_distances_flattened(self):
         structure = bulk('Al', cubic=True).repeat(2)
         del structure[0]
         r = structure.cell[0, 0]*0.49
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='flattened')
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='flattened')
         self.assertAlmostEqual(np.std(neigh.distances), 0)
         self.assertEqual(len(neigh.distances), 360)
         self.assertEqual(neigh.vecs.shape, (360, 3, ))
 
     def test_atom_numbers(self):
         structure = bulk('Al', cubic=True).repeat(2)
         del structure[0]
         r = structure.cell[0, 0]*0.49
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='filled')
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='filled')
         n = len(structure)
         self.assertEqual(neigh.atom_numbers.sum(), int(n*(n-1)/2*12))
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='ragged')
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='ragged')
         for i, (a, d) in enumerate(zip(neigh.atom_numbers, neigh.distances)):
             self.assertEqual(np.sum(a-len(d)*[i]), 0)
-        neigh = stk.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='flattened')
+        neigh = stk.analyse.get_neighbors(structure=structure, cutoff_radius=r, num_neighbors=None, mode='flattened')
         labels, counts = np.unique(
             np.unique(neigh.atom_numbers, return_counts=True)[1], return_counts=True
         )
         self.assertEqual(labels.tolist(), [11, 12])
         self.assertEqual(counts.tolist(), [12, 19])
 
     def test_get_shell_matrix(self):
         structure = bulk('Fe', a=2.83, cubic=True).repeat(2)
         structure.symbols[0] = 'Ni'
-        neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
+        neigh = stk.analyse.get_neighbors(structure=structure, num_neighbors=8)
         mat = neigh.get_shell_matrix()
         self.assertEqual(mat[0].sum(), 8*len(structure))
         mat = neigh.get_shell_matrix(chemical_pair=['Fe', 'Ni'])
         self.assertEqual(mat[0].sum(), 16)
         mat = neigh.get_shell_matrix(chemical_pair=['Ni', 'Ni'])
         self.assertEqual(mat[0].sum(), 0)
 
     def test_cluster_analysis(self):
         basis = bulk('Al', a=4.2, cubic=True).repeat(10)
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=100)
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=100)
         key, counts = neigh.cluster_analysis(id_list=[0, 1], return_cluster_sizes=True)
         self.assertTrue(np.array_equal(key[1], [0, 1]))
         self.assertEqual(counts[0], 2)
         key, counts = neigh.cluster_analysis(
             id_list=[0, int(len(basis)/2)], return_cluster_sizes=True
         )
         self.assertTrue(np.array_equal(key[1], [0]))
         self.assertEqual(counts[0], 1)
 
     def test_get_bonds(self):
         basis = bulk('Al', a=4.2, cubic=True).repeat(5)
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=20)
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=20)
         bonds = neigh.get_bonds()
         self.assertTrue(np.array_equal(np.sort(bonds[0]['Al'][0]),
                         np.sort(neigh.indices[0, neigh.shells[0] == 1])))
 
     def test_find_neighbors_by_vector(self):
         basis = Atoms(symbols=2*["Fe"],
                       scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)],
                       cell=np.identity(3),
                       pbc=True)
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=14)
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=14)
         id_lst, dist = neigh.find_neighbors_by_vector([0, 0, 1],
                                                       return_deviation=True)
         self.assertEqual(len(np.unique(np.unique(id_lst, return_counts=True)[1])), 1)
         self.assertLess(np.linalg.norm(dist), 1.0e-4)
         id_lst = neigh.find_neighbors_by_vector([0, 0, 0])
         self.assertTrue(np.array_equal(id_lst, np.arange(len(basis))))
 
     def test_get_distances_arbitrary_array(self):
         basis = bulk('Al', a=4.2, cubic=True).repeat(3)
-        neigh = stk.get_neighbors(structure=basis, cutoff_radius=3.5, num_neighbors=None)
+        neigh = stk.analyse.get_neighbors(structure=basis, cutoff_radius=3.5, num_neighbors=None)
         self.assertEqual(len(neigh.get_neighborhood(np.random.random(3), num_neighbors=12).indices), 12)
         self.assertEqual(
             len(neigh.get_neighborhood(np.random.random(3), num_neighbors=12).ragged.distances), 12
         )
         self.assertLessEqual(
             len(neigh.get_neighborhood(np.random.random(3), num_neighbors=12, cutoff_radius=3.5).ragged.vecs), 12
         )
         self.assertTrue(neigh.get_neighborhood(np.random.random((2, 3)), num_neighbors=12).vecs.shape == (2, 12, 3))
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=50)
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=50)
         self.assertTrue(neigh.get_neighborhood(np.random.random(3)).distances.shape == (50,))
         self.assertTrue(neigh.get_neighborhood(np.random.random((2, 3))).indices.shape == (2, 50))
         self.assertTrue(neigh.get_neighborhood(np.random.random((2, 2, 3))).vecs.shape == (2, 2, 50, 3))
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter("always")
             _ = neigh.get_neighborhood(np.random.random(3), num_neighbors=51)
             self.assertEqual(len(w), 1)
             _ = neigh.get_neighborhood(np.random.random(3), num_neighbors=51).distances
             self.assertEqual(len(w), 2)
 
     def test_repr(self):
         basis = bulk('Al', a=4.2, cubic=True).repeat(3)
-        neigh = stk.get_neighbors(structure=basis, cutoff_radius=3.5, num_neighbors=None)
+        neigh = stk.analyse.get_neighbors(structure=basis, cutoff_radius=3.5, num_neighbors=None)
         self.assertTrue('each atom' in neigh.__repr__())
 
     def test_norm_order(self):
         a_0 = 2.8
         basis = bulk('Fe', a=a_0, cubic=True).repeat(10)
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=None, norm_order=np.inf, cutoff_radius=a_0+0.01)
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=None, norm_order=np.inf, cutoff_radius=a_0+0.01)
         self.assertEqual(len(neigh.indices[0]), 34)
         with self.assertRaises(ValueError):
             neigh.norm_order = 3
 
     def test_chemical_symbols(self):
         basis = bulk('Fe', cubic=True)
         basis.symbols[0] = 'Ni'
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=1)
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=1)
         self.assertEqual(neigh.chemical_symbols[0, 0], 'Fe')
         self.assertEqual(neigh.chemical_symbols[1, 0], 'Ni')
         vacancy = bulk('Fe', cubic=True).repeat(4)
         del vacancy[0]
-        neigh = stk.get_neighbors(structure=vacancy, num_neighbors=None, cutoff_radius=3)
+        neigh = stk.analyse.get_neighbors(structure=vacancy, num_neighbors=None, cutoff_radius=3)
         self.assertEqual(neigh.chemical_symbols[0, -1], 'v')
 
     def test_steinhardt_parameters(self):
-        neigh = stk.get_neighbors(structure=bulk('Al'), num_neighbors=12)
+        neigh = stk.analyse.get_neighbors(structure=bulk('Al'), num_neighbors=12)
         # values obtained with pyscal
         self.assertAlmostEqual(0, neigh.get_steinhardt_parameter(2)[0])
         self.assertAlmostEqual(0.19094065395649323, neigh.get_steinhardt_parameter(4)[0])
         self.assertAlmostEqual(0.5745242597140696, neigh.get_steinhardt_parameter(6)[0])
-        neigh = stk.get_neighbors(structure=bulk('Mg', a=1, c=np.sqrt(8/3)), num_neighbors=12)
+        neigh = stk.analyse.get_neighbors(structure=bulk('Mg', a=1, c=np.sqrt(8/3)), num_neighbors=12)
         self.assertAlmostEqual(0, neigh.get_steinhardt_parameter(2)[0])
         self.assertAlmostEqual(0.097222222, neigh.get_steinhardt_parameter(4)[0])
         self.assertAlmostEqual(0.484761685, neigh.get_steinhardt_parameter(6)[0])
-        neigh = stk.get_neighbors(structure=bulk('Fe'), num_neighbors=14)
+        neigh = stk.analyse.get_neighbors(structure=bulk('Fe'), num_neighbors=14)
         self.assertAlmostEqual(0.03636964837266537, neigh.get_steinhardt_parameter(4)[0])
         self.assertAlmostEqual(0.5106882308569508, neigh.get_steinhardt_parameter(6)[0])
         self.assertRaises(ValueError, neigh.get_steinhardt_parameter, 2, 2)
 
     def test_numbers_of_neighbors(self):
         basis = bulk('Al', cubic=True).repeat(2)
         del basis[0]
-        neigh = stk.get_neighbors(structure=basis, num_neighbors=None, cutoff_radius=0.45*basis.cell[0,0])
+        neigh = stk.analyse.get_neighbors(structure=basis, num_neighbors=None, cutoff_radius=0.45*basis.cell[0,0])
         n, c = np.unique(neigh.numbers_of_neighbors, return_counts=True)
         self.assertEqual(n.tolist(), [11, 12])
         self.assertEqual(c.tolist(), [12, 19])
 
     def test_modes(self):
         basis = bulk('Al', cubic=True)
-        neigh = stk.get_neighbors(structure=basis)
+        neigh = stk.analyse.get_neighbors(structure=basis)
         self.assertTrue(neigh.mode == 'filled')
         with self.assertRaises(KeyError):
-            neigh = stk.get_neighbors(structure=basis, mode='random_key')
+            neigh = stk.analyse.get_neighbors(structure=basis, mode='random_key')
 
+    @unittest.skipIf(
+        skip_pyscal_test,
+        "pyscal is not installed, so the centro symmetry descriptor based tests are skipped."
+    )
     def test_centrosymmetry(self):
         structure = bulk('Fe').repeat(4)
-        cs = stk.get_neighbors(structure=structure, num_neighbors=8).centrosymmetry
+        cs = stk.analyse.get_neighbors(structure=structure, num_neighbors=8).centrosymmetry
         self.assertAlmostEqual(cs.max(), 0)
         self.assertAlmostEqual(cs.min(), 0)
         structure.positions += 0.01*(2*np.random.random(structure.positions.shape)-1)
-        neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
+        neigh = stk.analyse.get_neighbors(structure=structure, num_neighbors=8)
         self.assertGreater(neigh.centrosymmetry.min(), 0)
         self.assertTrue(
             np.allclose(
-                neigh.centrosymmetry, stk.analyse_centro_symmetry(structure=structure, num_neighbors=8)
+                neigh.centrosymmetry, stk.analyse.get_centro_symmetry_descriptors(structure=structure, num_neighbors=8)
             )
         )
 
     def test_get_all_pairs(self):
         structure = bulk('Fe').repeat(4)
-        neigh = stk.get_neighbors(structure=structure, num_neighbors=8)
+        neigh = stk.analyse.get_neighbors(structure=structure, num_neighbors=8)
         for n in [2, 4, 6]:
             pairs = neigh._get_all_possible_pairs(n)
             self.assertEqual(
                 (np.prod(np.arange(int(n/2))*2+1), int(n/2), 2),
                 pairs.shape
             )
             for i in range(2**(n-2)):
```

### Comparing `structuretoolkit-0.0.2/tests/test_pyscal.py` & `structuretoolkit-0.0.3/tests/test_pyscal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import unittest
 import numpy as np
-import pyscal.core as pc
 from ase.build import bulk
 from ase.atoms import Atoms
 import structuretoolkit as stk
 
+try:
+    import pyscal
+    skip_pyscal_test = False
+except ImportError:
+    skip_pyscal_test = True
 
+
+@unittest.skipIf(skip_pyscal_test, "pyscal is not installed, so the pyscal tests are skipped.")
 class Testpyscal(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.structure = bulk('Al', a=4, cubic=True).repeat(4)
 
     def test_attributes(self):
         self.assertIsInstance(self.structure, Atoms)
 
     def test_simple_system(self):
         """
         Test a simple ase to pyscal conversion
         """
-        sysp = pc.System()
-        sysp.read_inputfile(self.structure, format="ase")
-        self.assertEqual(len(sysp.atoms), 256)
+        self.assertEqual(len(self.structure), 256)
+        self.assertEqual(len(stk.common.ase_to_pyscal(self.structure).atoms), 256)
 
     def test_steinhardt_parameters_returns(self):
-        self.assertEqual(2, len(stk.get_steinhardt_parameter_structure(self.structure)),
+        self.assertEqual(2, len(stk.analyse.get_steinhardt_parameters(self.structure)),
                          msg='Expected default return value to be a tuple of qs and cluster indices.')
-        self.assertIsInstance(stk.get_steinhardt_parameter_structure(self.structure, n_clusters=None), np.ndarray,
+        self.assertIsInstance(stk.analyse.get_steinhardt_parameters(self.structure, n_clusters=None), np.ndarray,
                               msg='Expected just the qs when no clustering is used.')
 
     def test_steinhardt_parameters_qs(self):
         """
         Test the calculation of Steinhardts parameters
         """
         perfect_vals = [0.00, 0.00, 0.190, 0.00, 0.575, 0.00, 0.404, 0.00,
                         0.013, 0.00, 0.600]
 
         qtest = np.random.randint(2, 13, size=2)
 
-        qs, _ = stk.get_steinhardt_parameter_structure(self.structure, cutoff=0, n_clusters=2, q=qtest)
+        qs, _ = stk.analyse.get_steinhardt_parameters(self.structure, cutoff=0, n_clusters=2, q=qtest)
         for c, q in enumerate(qs):
             self.assertLess(np.abs(np.mean(q) - perfect_vals[qtest[c]-2]), 1E-3)
 
     def test_steinhardt_parameters_clustering(self):
         noisy_structure = self.structure.copy()
         noisy_structure.positions += 0.5 * np.random.rand(*noisy_structure.positions.shape)
         n_clusters = 3
-        _, inds = stk.get_steinhardt_parameter_structure(noisy_structure, n_clusters=n_clusters)
+        _, inds = stk.analyse.get_steinhardt_parameters(noisy_structure, n_clusters=n_clusters)
         self.assertEqual(n_clusters, len(np.unique(inds)), msg='Expected to find one label for each cluster.')
 
     def test_centrosymmetry(self):
-        csm = stk.analyse_centro_symmetry(self.structure, num_neighbors=12)
+        csm = stk.analyse.get_centro_symmetry_descriptors(self.structure, num_neighbors=12)
         self.assertLess(np.mean(csm), 1E-5)
 
     def test_cna(self):
-        cna = stk.analyse_cna_adaptive(self.structure)
+        cna = stk.analyse.get_adaptive_cna_descriptors(self.structure)
         self.assertEqual(cna['fcc'], len(self.structure))
 
         rand = np.random.randint(0, len(self.structure))
 
-        cna = stk.analyse_cna_adaptive(self.structure, mode="numeric")
+        cna = stk.analyse.get_adaptive_cna_descriptors(self.structure, mode="numeric")
         self.assertEqual(cna[rand], 1)
 
-        cna = stk.analyse_cna_adaptive(self.structure, mode="str")
+        cna = stk.analyse.get_adaptive_cna_descriptors(self.structure, mode="str")
         self.assertEqual(cna[rand], "fcc")
 
     def test_volume(self):
-        vols = stk.analyse_voronoi_volume(self.structure)
+        vols = stk.analyse.get_voronoi_volumes(self.structure)
         self.assertLess(np.abs(np.mean(vols) - 16.0), 1E-3)
 
 
+@unittest.skipIf(skip_pyscal_test, "pyscal is not installed, so the pyscal tests are skipped.")
 class Testpyscalatoms(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.al_fcc = bulk("Al", cubic=True)
         cls.fe_bcc = bulk("Fe", cubic=True)
         cls.ti_hcp = bulk("Ti", orthorhombic=True)
         cls.si_dia = bulk("Si", cubic=True)
@@ -85,124 +91,124 @@
     def test_steinhardt_parameters(self):
         """ Test the calculation of Steinhardts parameters using the Analyse class. """
         perfect_vals = [0.00, 0.00, 0.190, 0.00, 0.575, 0.00, 0.404, 0.00,
                         0.013, 0.00, 0.600]
 
         qtest = np.random.randint(2, 13, size=2)
 
-        qs, _ = stk.get_steinhardt_parameter_structure(structure=self.al_fcc_4, cutoff=0, n_clusters=2, q=qtest)
+        qs, _ = stk.analyse.get_steinhardt_parameters(structure=self.al_fcc_4, cutoff=0, n_clusters=2, q=qtest)
         for c, q in enumerate(qs):
             self.assertLess(np.abs(np.mean(q) - perfect_vals[qtest[c]-2]), 1E-3)
 
     def test_analyse_pyscal_centro_symmetry(self):
-        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(structure=self.al_fcc, num_neighbors=12)]))
-        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse_centro_symmetry(structure=self.fe_bcc, num_neighbors=8)]))
-        self.assertTrue(all([np.isclose(v, 8.7025) for v in stk.analyse_centro_symmetry(structure=self.ti_hcp, num_neighbors=12)]))
-        self.assertTrue(all([np.isclose(v, 14.742449) for v in stk.analyse_centro_symmetry(structure=self.si_dia, num_neighbors=4)]))
-        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.al_fcc)), len(self.al_fcc))
-        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.fe_bcc)), len(self.fe_bcc))
-        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.ti_hcp)), len(self.ti_hcp))
-        self.assertEqual(len(stk.analyse_centro_symmetry(structure=self.si_dia)), len(self.si_dia))
+        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse.get_centro_symmetry_descriptors(structure=self.al_fcc, num_neighbors=12)]))
+        self.assertTrue(all([np.isclose(v, 0.0) for v in stk.analyse.get_centro_symmetry_descriptors(structure=self.fe_bcc, num_neighbors=8)]))
+        self.assertTrue(all([np.isclose(v, 8.7025) for v in stk.analyse.get_centro_symmetry_descriptors(structure=self.ti_hcp, num_neighbors=12)]))
+        self.assertTrue(all([np.isclose(v, 14.742449) for v in stk.analyse.get_centro_symmetry_descriptors(structure=self.si_dia, num_neighbors=4)]))
+        self.assertEqual(len(stk.analyse.get_centro_symmetry_descriptors(structure=self.al_fcc)), len(self.al_fcc))
+        self.assertEqual(len(stk.analyse.get_centro_symmetry_descriptors(structure=self.fe_bcc)), len(self.fe_bcc))
+        self.assertEqual(len(stk.analyse.get_centro_symmetry_descriptors(structure=self.ti_hcp)), len(self.ti_hcp))
+        self.assertEqual(len(stk.analyse.get_centro_symmetry_descriptors(structure=self.si_dia)), len(self.si_dia))
 
     def test_analyse_pyscal_voronoi_volume(self):
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.al_fcc)), 16.60753125)
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.fe_bcc)), 11.8199515)
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.ti_hcp)), 17.65294557)
-        self.assertAlmostEqual(np.mean(stk.analyse_voronoi_volume(structure=self.si_dia)), 20.01287587)
-        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.al_fcc)), len(self.al_fcc))
-        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.fe_bcc)), len(self.fe_bcc))
-        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.ti_hcp)), len(self.ti_hcp))
-        self.assertEqual(len(stk.analyse_voronoi_volume(structure=self.si_dia)), len(self.si_dia))
+        self.assertAlmostEqual(np.mean(stk.analyse.get_voronoi_volumes(structure=self.al_fcc)), 16.60753125)
+        self.assertAlmostEqual(np.mean(stk.analyse.get_voronoi_volumes(structure=self.fe_bcc)), 11.8199515)
+        self.assertAlmostEqual(np.mean(stk.analyse.get_voronoi_volumes(structure=self.ti_hcp)), 17.65294557)
+        self.assertAlmostEqual(np.mean(stk.analyse.get_voronoi_volumes(structure=self.si_dia)), 20.01287587)
+        self.assertEqual(len(stk.analyse.get_voronoi_volumes(structure=self.al_fcc)), len(self.al_fcc))
+        self.assertEqual(len(stk.analyse.get_voronoi_volumes(structure=self.fe_bcc)), len(self.fe_bcc))
+        self.assertEqual(len(stk.analyse.get_voronoi_volumes(structure=self.ti_hcp)), len(self.ti_hcp))
+        self.assertEqual(len(stk.analyse.get_voronoi_volumes(structure=self.si_dia)), len(self.si_dia))
 
     def test_analyse_pyscal_cna_adaptive(self):
         pyscal_keys = [
             'others', 'fcc', 'hcp', 'bcc', 'ico',
         ]
         ovito_keys = [
             'CommonNeighborAnalysis.counts.OTHER',
             'CommonNeighborAnalysis.counts.FCC',
             'CommonNeighborAnalysis.counts.HCP',
             'CommonNeighborAnalysis.counts.BCC',
              'CommonNeighborAnalysis.counts.ICO'
         ]
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.al_fcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[1]], len(self.al_fcc))
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.fe_bcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[3]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.ti_hcp, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[2]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.si_dia, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.si_dia, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.si_dia))
 
-        res_numeric = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.al_fcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 1 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.fe_bcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 3 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.ti_hcp, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 2 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(structure=self.si_dia, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.si_dia, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 0 for v in res_numeric]))
 
-        res_str = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.al_fcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'fcc' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.fe_bcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'bcc' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.ti_hcp, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'hcp' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(structure=self.si_dia, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.si_dia, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'others' for v in res_str]))
 
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.al_fcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[1]], len(self.al_fcc))
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.fe_bcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[3]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.ti_hcp, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[2]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_cna_adaptive(structure=self.si_dia, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_adaptive_cna_descriptors(structure=self.si_dia, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[0]], len(self.si_dia))
 
-        res_numeric = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.al_fcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 1 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.fe_bcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 3 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.ti_hcp, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 2 for v in res_numeric]))
-        res_numeric = stk.analyse_cna_adaptive(structure=self.si_dia, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_adaptive_cna_descriptors(structure=self.si_dia, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 0 for v in res_numeric]))
 
-        res_str = stk.analyse_cna_adaptive(structure=self.al_fcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.al_fcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'FCC' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(structure=self.fe_bcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.fe_bcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'BCC' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(structure=self.ti_hcp, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.ti_hcp, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'HCP' for v in res_str]))
-        res_str = stk.analyse_cna_adaptive(structure=self.si_dia, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_adaptive_cna_descriptors(structure=self.si_dia, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'Other' for v in res_str]))
 
     def test_analyse_pyscal_diamond_structure(self):
         pyscal_keys = [
             'others', 'fcc', 'hcp', 'bcc', 'ico',
             'cubic diamond', 'cubic diamond 1NN', 'cubic diamond 2NN',
@@ -213,88 +219,88 @@
             'IdentifyDiamond.counts.CUBIC_DIAMOND_FIRST_NEIGHBOR',
             'IdentifyDiamond.counts.CUBIC_DIAMOND_SECOND_NEIGHBOR',
             'IdentifyDiamond.counts.HEX_DIAMOND',
             'IdentifyDiamond.counts.HEX_DIAMOND_FIRST_NEIGHBOR',
             'IdentifyDiamond.counts.HEX_DIAMOND_SECOND_NEIGHBOR',
             'IdentifyDiamond.counts.OTHER'
         ]
-        res_dict_total = stk.analyse_diamond_structure(structure=self.al_fcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.al_fcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.al_fcc))
-        res_dict_total = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.fe_bcc, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.ti_hcp, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[0]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_diamond_structure(structure=self.si_dia, mode="total", ovito_compatibility=False)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.si_dia, mode="total", ovito_compatibility=False)
         self.assertEqual(sum([k in res_dict_total.keys() for k in pyscal_keys]), len(pyscal_keys))
         self.assertEqual(res_dict_total[pyscal_keys[5]], len(self.si_dia))
 
-        res_numeric = stk.analyse_diamond_structure(structure=self.al_fcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.al_fcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 0 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.fe_bcc, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 0 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.ti_hcp, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 0 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(structure=self.si_dia, mode="numeric", ovito_compatibility=False)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.si_dia, mode="numeric", ovito_compatibility=False)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 5 for v in res_numeric]))
 
-        res_str = stk.analyse_diamond_structure(structure=self.al_fcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.al_fcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'others' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.fe_bcc, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'others' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.ti_hcp, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'others' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(structure=self.si_dia, mode="str", ovito_compatibility=False)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.si_dia, mode="str", ovito_compatibility=False)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'cubic diamond' for v in res_str]))
 
-        res_dict_total = stk.analyse_diamond_structure(structure=self.al_fcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.al_fcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[6]], len(self.al_fcc))
-        res_dict_total = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.fe_bcc, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[6]], len(self.fe_bcc))
-        res_dict_total = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.ti_hcp, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[6]], len(self.ti_hcp))
-        res_dict_total = stk.analyse_diamond_structure(structure=self.si_dia, mode="total", ovito_compatibility=True)
+        res_dict_total = stk.analyse.get_diamond_structure_descriptors(structure=self.si_dia, mode="total", ovito_compatibility=True)
         self.assertEqual(sum([k in res_dict_total.keys() for k in ovito_keys]), len(ovito_keys))
         self.assertEqual(res_dict_total[ovito_keys[0]], len(self.si_dia))
 
-        res_numeric = stk.analyse_diamond_structure(structure=self.al_fcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.al_fcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.al_fcc))
         self.assertTrue(all([v == 6 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.fe_bcc, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.fe_bcc))
         self.assertTrue(all([v == 6 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.ti_hcp, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.ti_hcp))
         self.assertTrue(all([v == 6 for v in res_numeric]))
-        res_numeric = stk.analyse_diamond_structure(structure=self.si_dia, mode="numeric", ovito_compatibility=True)
+        res_numeric = stk.analyse.get_diamond_structure_descriptors(structure=self.si_dia, mode="numeric", ovito_compatibility=True)
         self.assertEqual(len(res_numeric), len(self.si_dia))
         self.assertTrue(all([v == 0 for v in res_numeric]))
 
-        res_str = stk.analyse_diamond_structure(structure=self.al_fcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.al_fcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.al_fcc))
         self.assertTrue(all([v == 'Other' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(structure=self.fe_bcc, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.fe_bcc, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.fe_bcc))
         self.assertTrue(all([v == 'Other' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(structure=self.ti_hcp, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.ti_hcp, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.ti_hcp))
         self.assertTrue(all([v == 'Other' for v in res_str]))
-        res_str = stk.analyse_diamond_structure(structure=self.si_dia, mode="str", ovito_compatibility=True)
+        res_str = stk.analyse.get_diamond_structure_descriptors(structure=self.si_dia, mode="str", ovito_compatibility=True)
         self.assertEqual(len(res_str), len(self.si_dia))
         self.assertTrue(all([v == 'Cubic diamond' for v in res_str]))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `structuretoolkit-0.0.2/tests/test_strain.py` & `structuretoolkit-0.0.3/tests/test_strain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # coding: utf-8
 import unittest
 import numpy as np
 from ase.build import bulk
 import structuretoolkit as stk
 
+try:
+    import pyscal
+    skip_pyscal_test = False
+except ImportError:
+    skip_pyscal_test = True
+
 
 class TestAtoms(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         bulk_structure = bulk('Fe', cubic=True)
-        cls.strain = stk.get_strain(structure=bulk_structure, ref_structure=bulk_structure, return_object=True)
+        cls.strain = stk.analyse.get_strain(structure=bulk_structure, ref_structure=bulk_structure, return_object=True)
 
+    @unittest.skipIf(skip_pyscal_test, "pyscal is not installed, so the pyscal tests are skipped.")
     def test_number_of_neighbors(self):
         self.assertEqual(self.strain.num_neighbors, 8)
         bulk_structure = bulk('Al', cubic=True)
-        strain = stk.get_strain(structure=bulk_structure, ref_structure=bulk_structure, return_object=True)
+        strain = stk.analyse.get_strain(structure=bulk_structure, ref_structure=bulk_structure, return_object=True)
         self.assertEqual(strain.num_neighbors, 12)
 
     def test_get_angle(self):
         self.assertAlmostEqual(self.strain._get_angle([1, 0, 0], [0, 1, 1]), 0.5*np.pi)
         self.assertAlmostEqual(self.strain._get_angle([1, 0, 0], [1, 1, 0]), 0.25*np.pi)
 
     def test_get_perpendicular_unit_vector(self):
```

### Comparing `structuretoolkit-0.0.2/tests/test_symmetry.py` & `structuretoolkit-0.0.3/tests/test_symmetry.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,162 +2,174 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import unittest
 import numpy as np
 from ase.build import bulk
 from ase.atoms import Atoms
-from structuretoolkit.analyse.symmetry import SymmetryError
 import structuretoolkit as stk
 
+try:
+    import pyscal
+    skip_pyscal_test = False
+except ImportError:
+    skip_pyscal_test = True
 
+
+try:
+    import spglib
+    skip_spglib_test = False
+except ImportError:
+    skip_spglib_test = True
+
+@unittest.skipIf(skip_spglib_test, "spglib is not installed, so the spglib tests are skipped.")
 class TestAtoms(unittest.TestCase):
     def test_get_arg_equivalent_sites(self):
         a_0 = 4.0
         structure = bulk('Al', cubic=True, a=a_0).repeat(2)
-        sites = stk.get_wrapped_coordinates(structure=structure, positions=structure.positions + np.array([0, 0, 0.5 * a_0]))
+        sites = stk.common.get_wrapped_coordinates(structure=structure, positions=structure.positions + np.array([0, 0, 0.5 * a_0]))
         v_position = structure.positions[0]
         del structure[0]
         pairs = np.stack((
-            stk.get_symmetry(structure=structure).get_arg_equivalent_sites(sites),
-            np.unique(np.round(stk.get_distances_array(structure=structure, p1=v_position, p2=sites), decimals=2), return_inverse=True)[1]
+            stk.analyse.get_symmetry(structure=structure).get_arg_equivalent_sites(sites),
+            np.unique(np.round(stk.analyse.get_distances_array(structure=structure, p1=v_position, p2=sites), decimals=2), return_inverse=True)[1]
         ), axis=-1)
         unique_pairs = np.unique(pairs, axis=0)
         self.assertEqual(len(unique_pairs), len(np.unique(unique_pairs[:, 0])))
         with self.assertRaises(ValueError):
-            stk.get_symmetry(structure=structure).get_arg_equivalent_sites([0, 0, 0])
+            stk.analyse.get_symmetry(structure=structure).get_arg_equivalent_sites([0, 0, 0])
 
     def test_generate_equivalent_points(self):
         a_0 = 4
         structure = bulk('Al', cubic=True, a=a_0)
-        sym = stk.get_symmetry(structure)
+        sym = stk.analyse.get_symmetry(structure)
         self.assertEqual(
             len(structure),
             len(sym.generate_equivalent_points([0, 0, 0.5 * a_0]))
         )
         x = np.array([[0, 0, 0.5 * a_0], 3 * [0.25 * a_0]])
         y = np.random.randn(2)
         sym_x = sym.generate_equivalent_points(x, return_unique=False)
         y = np.tile(y, len(sym_x))
         sym_x = sym_x.reshape(-1, 3)
         xy = np.round(
-            [stk.get_neighborhood(structure, sym_x, num_neighbors=1).distances.flatten(), y],
+            [stk.analyse.get_neighborhood(structure, sym_x, num_neighbors=1).distances.flatten(), y],
             decimals=8
         )
         self.assertEqual(
             np.unique(xy, axis=1).shape,
             (2, 2),
             msg="order of generated points does not match the original order"
         )
 
     def test_get_symmetry(self):
         cell = 2.2 * np.identity(3)
         Al = Atoms("AlAl", positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=cell, pbc=True).repeat(2)
-        self.assertEqual(len(set(stk.get_symmetry(structure=Al)["equivalent_atoms"])), 1)
-        self.assertEqual(len(stk.get_symmetry(structure=Al)["translations"]), 96)
+        self.assertEqual(len(set(stk.analyse.get_symmetry(structure=Al)["equivalent_atoms"])), 1)
+        self.assertEqual(len(stk.analyse.get_symmetry(structure=Al)["translations"]), 96)
         self.assertEqual(
-            len(stk.get_symmetry(structure=Al)["translations"]), len(stk.get_symmetry(structure=Al)["rotations"])
+            len(stk.analyse.get_symmetry(structure=Al)["translations"]), len(stk.analyse.get_symmetry(structure=Al)["rotations"])
         )
         cell = 2.2 * np.identity(3)
         Al = Atoms("AlAl", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=cell, pbc=True)
         v = np.random.rand(6).reshape(-1, 3)
-        self.assertAlmostEqual(np.linalg.norm(stk.get_symmetry(structure=Al).symmetrize_vectors(v)), 0)
+        self.assertAlmostEqual(np.linalg.norm(stk.analyse.get_symmetry(structure=Al).symmetrize_vectors(v)), 0)
         vv = np.random.rand(12).reshape(2, 2, 3)
-        for vvv in stk.get_symmetry(structure=Al).symmetrize_vectors(vv):
+        for vvv in stk.analyse.get_symmetry(structure=Al).symmetrize_vectors(vv):
             self.assertAlmostEqual(np.linalg.norm(vvv), 0)
         Al.positions[0, 0] += 0.01
-        w = stk.get_symmetry(structure=Al).symmetrize_vectors(v)
+        w = stk.analyse.get_symmetry(structure=Al).symmetrize_vectors(v)
         self.assertAlmostEqual(np.absolute(w[:, 0]).sum(), np.linalg.norm(w, axis=-1).sum())
 
     def test_get_symmetry_dataset(self):
         cell = 2.2 * np.identity(3)
         Al_sc = Atoms("AlAl", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=cell)
         Al_sc = Al_sc.repeat([2, 2, 2])
-        self.assertEqual(stk.get_symmetry(structure=Al_sc).info["number"], 229)
+        self.assertEqual(stk.analyse.get_symmetry(structure=Al_sc).info["number"], 229)
 
     def test_get_ir_reciprocal_mesh(self):
         cell = 2.2 * np.identity(3)
         Al_sc = Atoms("AlAl", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=cell)
-        self.assertEqual(len(stk.get_symmetry(structure=Al_sc).get_ir_reciprocal_mesh([3, 3, 3])[0]), 27)
+        self.assertEqual(len(stk.analyse.get_symmetry(structure=Al_sc).get_ir_reciprocal_mesh([3, 3, 3])[0]), 27)
 
     def test_get_primitive_cell(self):
         cell = 2.2 * np.identity(3)
         basis = Atoms("AlFe", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=cell)
         structure = basis.repeat([2, 2, 2])
-        sym = stk.get_symmetry(structure=structure)
+        sym = stk.analyse.get_symmetry(structure=structure)
         self.assertEqual(len(basis), len(sym.get_primitive_cell(standardize=True)))
-        self.assertEqual(stk.get_symmetry(structure=sym.get_primitive_cell()).spacegroup["Number"], 221)
+        self.assertEqual(stk.analyse.get_symmetry(structure=sym.get_primitive_cell()).spacegroup["Number"], 221)
 
     def test_get_equivalent_points(self):
         basis = Atoms("FeFe", positions=[[0.01, 0, 0], [0.5, 0.5, 0.5]], cell=np.identity(3))
-        arr = stk.get_symmetry(structure=basis).generate_equivalent_points([0, 0, 0.5])
+        arr = stk.analyse.get_symmetry(structure=basis).generate_equivalent_points([0, 0, 0.5])
         self.assertAlmostEqual(np.linalg.norm(arr - np.array([0.51, 0.5, 0]), axis=-1).min(), 0)
 
     def test_get_space_group(self):
         cell = 2.2 * np.identity(3)
         Al_sc = Atoms("AlAl", scaled_positions=[(0, 0, 0), (0.5, 0.5, 0.5)], cell=cell)
-        self.assertEqual(stk.get_symmetry(structure=Al_sc).spacegroup["InternationalTableSymbol"], "Im-3m")
-        self.assertEqual(stk.get_symmetry(structure=Al_sc).spacegroup["Number"], 229)
+        self.assertEqual(stk.analyse.get_symmetry(structure=Al_sc).spacegroup["InternationalTableSymbol"], "Im-3m")
+        self.assertEqual(stk.analyse.get_symmetry(structure=Al_sc).spacegroup["Number"], 229)
         cell = 4.2 * (0.5 * np.ones((3, 3)) - 0.5 * np.eye(3))
         Al_fcc = Atoms("Al", scaled_positions=[(0, 0, 0)], cell=cell)
-        self.assertEqual(stk.get_symmetry(structure=Al_fcc).spacegroup["InternationalTableSymbol"], "Fm-3m")
-        self.assertEqual(stk.get_symmetry(structure=Al_fcc).spacegroup["Number"], 225)
+        self.assertEqual(stk.analyse.get_symmetry(structure=Al_fcc).spacegroup["InternationalTableSymbol"], "Fm-3m")
+        self.assertEqual(stk.analyse.get_symmetry(structure=Al_fcc).spacegroup["Number"], 225)
         a = 3.18
         c = 1.623 * a
         cell = np.eye(3)
         cell[0, 0] = a
         cell[2, 2] = c
         cell[1, 0] = -a / 2.0
         cell[1, 1] = np.sqrt(3) * a / 2.0
         pos = np.array([[0.0, 0.0, 0.0], [1.0 / 3.0, 2.0 / 3.0, 1.0 / 2.0]])
         Mg_hcp = Atoms("Mg2", scaled_positions=pos, cell=cell)
-        self.assertEqual(stk.get_symmetry(structure=Mg_hcp).spacegroup["Number"], 194)
+        self.assertEqual(stk.analyse.get_symmetry(structure=Mg_hcp).spacegroup["Number"], 194)
         cell = np.eye(3)
         cell[0, 0] = a
         cell[2, 2] = c
         cell[1, 1] = np.sqrt(3) * a
         pos = np.array(
             [
                 [0.0, 0.0, 0.0],
                 [0.5, 0.5, 0.0],
                 [0.5, 1 / 6, 0.5],
                 [0.0, 2 / 3, 0.5],
             ]
         )
         Mg_hcp = Atoms("Mg4", scaled_positions=pos, cell=cell)
-        self.assertEqual(stk.get_symmetry(structure=Mg_hcp).spacegroup["Number"], 194)
+        self.assertEqual(stk.analyse.get_symmetry(structure=Mg_hcp).spacegroup["Number"], 194)
 
     def test_permutations(self):
         structure = bulk('Al', cubic=True).repeat(2)
         x_vacancy = structure.positions[0]
         del structure[0]
-        neigh = stk.get_neighborhood(structure=structure, positions=x_vacancy)
+        neigh = stk.analyse.get_neighborhood(structure=structure, positions=x_vacancy)
         vec = np.zeros_like(structure.positions)
         vec[neigh.indices[0]] = neigh.vecs[0]
-        sym = stk.get_symmetry(structure=structure)
+        sym = stk.analyse.get_symmetry(structure=structure)
         all_vectors = np.einsum('ijk,ink->inj', sym.rotations, vec[sym.permutations])
         for i, v in zip(neigh.indices, neigh.vecs):
             vec = np.zeros_like(structure.positions)
             vec[i] = v
             self.assertAlmostEqual(np.linalg.norm(all_vectors - vec, axis=(-1, -2)).min(), 0,)
 
     def test_arg_equivalent_vectors(self):
         structure = bulk('Al', cubic=True).repeat(2)
-        self.assertEqual(np.unique(stk.get_symmetry(structure=structure).arg_equivalent_vectors).squeeze(), 0)
+        self.assertEqual(np.unique(stk.analyse.get_symmetry(structure=structure).arg_equivalent_vectors).squeeze(), 0)
         x_v = structure.positions[0]
         del structure[0]
-        arg_v = stk.get_symmetry(structure=structure).arg_equivalent_vectors
-        dx = stk.get_distances_array(structure=structure, p1=structure.positions, p2=x_v, vectors=True)
+        arg_v = stk.analyse.get_symmetry(structure=structure).arg_equivalent_vectors
+        dx = stk.analyse.get_distances_array(structure=structure, p1=structure.positions, p2=x_v, vectors=True)
         dx_round = np.round(np.absolute(dx), decimals=3)
         self.assertEqual(len(np.unique(dx_round + arg_v)), len(np.unique(arg_v)))
 
     def test_error(self):
         """spglib errors should be wrapped in a SymmetryError."""
 
         structure = bulk('Al')
         structure += structure[-1]
-        with self.assertRaises(SymmetryError):
-            stk.get_symmetry(structure=structure)
+        with self.assertRaises(stk.common.SymmetryError):
+            stk.analyse.get_symmetry(structure=structure)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `structuretoolkit-0.0.2/tests/test_visualize.py` & `structuretoolkit-0.0.3/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.2/versioneer.py` & `structuretoolkit-0.0.3/versioneer.py`

 * *Files identical despite different names*

