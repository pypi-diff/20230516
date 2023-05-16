# Comparing `tmp/dgpost-2.0a4.tar.gz` & `tmp/dgpost-2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgpost-2.0a4.tar", last modified: Thu Aug 18 07:22:54 2022, max compression
+gzip compressed data, was "dgpost-2.0rc1.tar", last modified: Fri Dec  2 11:12:43 2022, max compression
```

## Comparing `dgpost-2.0a4.tar` & `dgpost-2.0rc1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.535759 dgpost-2.0a4/
--rw-rw-rw-   0        0        0    35823 2022-06-28 12:08:21.000000 dgpost-2.0a4/LICENSE
--rw-rw-rw-   0        0        0       55 2022-06-28 12:08:21.000000 dgpost-2.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     3063 2022-08-18 07:22:54.536723 dgpost-2.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     2313 2022-06-28 12:08:21.000000 dgpost-2.0a4/README.md
--rw-rw-rw-   0        0        0      217 2022-08-18 07:22:54.541711 dgpost-2.0a4/setup.cfg
--rw-rw-rw-   0        0        0     1783 2022-08-17 11:22:11.000000 dgpost-2.0a4/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.394197 dgpost-2.0a4/src/
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.543703 dgpost-2.0a4/src/dgpost/
--rw-rw-rw-   0        0        0      179 2022-06-28 12:08:21.000000 dgpost-2.0a4/src/dgpost/__init__.py
--rw-rw-rw-   0        0        0      518 2022-08-18 07:22:54.543703 dgpost-2.0a4/src/dgpost/_version.py
--rw-rw-rw-   0        0        0     5360 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/main.py
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.500951 dgpost-2.0a4/src/dgpost/transform/
--rw-rw-rw-   0        0        0        0 2022-06-28 12:08:21.000000 dgpost-2.0a4/src/dgpost/transform/__init__.py
--rw-rw-rw-   0        0        0    19059 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/transform/catalysis.py
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.509794 dgpost-2.0a4/src/dgpost/transform/circuit_utils/
--rw-rw-rw-   0        0        0        0 2022-06-28 12:08:21.000000 dgpost-2.0a4/src/dgpost/transform/circuit_utils/__init__.py
--rw-rw-rw-   0        0        0     5924 2022-06-28 12:08:21.000000 dgpost-2.0a4/src/dgpost/transform/circuit_utils/circuit_components.py
--rw-rw-rw-   0        0        0     5988 2022-06-28 12:08:21.000000 dgpost-2.0a4/src/dgpost/transform/circuit_utils/circuit_parser.py
--rw-rw-rw-   0        0        0    10188 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/transform/electrochemistry.py
--rw-rw-rw-   0        0        0    13827 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/transform/impedance.py
--rw-rw-rw-   0        0        0     6215 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/transform/rates.py
--rw-rw-rw-   0        0        0     4262 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/transform/table.py
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.533731 dgpost-2.0a4/src/dgpost/utils/
--rw-rw-rw-   0        0        0      162 2022-06-28 12:08:21.000000 dgpost-2.0a4/src/dgpost/utils/__init__.py
--rw-rw-rw-   0        0        0    11124 2022-08-18 07:09:52.000000 dgpost-2.0a4/src/dgpost/utils/extract.py
--rw-rw-rw-   0        0        0    21821 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/utils/helpers.py
--rw-rw-rw-   0        0        0     2330 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/utils/load.py
--rw-rw-rw-   0        0        0     1298 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/utils/parse.py
--rw-rw-rw-   0        0        0     7061 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/utils/plot.py
--rw-rw-rw-   0        0        0     3205 2022-08-17 11:22:11.000000 dgpost-2.0a4/src/dgpost/utils/save.py
--rw-rw-rw-   0        0        0     1275 2022-08-17 11:22:12.000000 dgpost-2.0a4/src/dgpost/utils/transform.py
-drwxrwxrwx   0        0        0        0 2022-08-18 07:22:54.487854 dgpost-2.0a4/src/dgpost.egg-info/
--rw-rw-rw-   0        0        0     3063 2022-08-18 07:22:54.000000 dgpost-2.0a4/src/dgpost.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2022-08-18 07:22:54.000000 dgpost-2.0a4/src/dgpost.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-18 07:22:54.000000 dgpost-2.0a4/src/dgpost.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-08-18 07:22:54.000000 dgpost-2.0a4/src/dgpost.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      235 2022-08-18 07:22:54.000000 dgpost-2.0a4/src/dgpost.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-18 07:22:54.000000 dgpost-2.0a4/src/dgpost.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    83320 2022-06-28 12:08:22.000000 dgpost-2.0a4/versioneer.py
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:43.224933 dgpost-2.0rc1/
+-rw-rw-rw-   0        0        0    35823 2022-11-10 12:13:22.000000 dgpost-2.0rc1/LICENSE
+-rw-rw-rw-   0        0        0       55 2022-11-10 12:13:22.000000 dgpost-2.0rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3064 2022-12-02 11:12:43.226000 dgpost-2.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     2313 2022-11-10 12:13:22.000000 dgpost-2.0rc1/README.md
+-rw-rw-rw-   0        0        0      217 2022-12-02 11:12:43.231473 dgpost-2.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1801 2022-11-10 12:13:22.000000 dgpost-2.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:42.922384 dgpost-2.0rc1/src/
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:43.234474 dgpost-2.0rc1/src/dgpost/
+-rw-rw-rw-   0        0        0      179 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/__init__.py
+-rw-rw-rw-   0        0        0      519 2022-12-02 11:12:43.235478 dgpost-2.0rc1/src/dgpost/_version.py
+-rw-rw-rw-   0        0        0     6397 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/main.py
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:43.114477 dgpost-2.0rc1/src/dgpost/transform/
+-rw-rw-rw-   0        0        0        0 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/__init__.py
+-rw-rw-rw-   0        0        0    19178 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/catalysis.py
+-rw-rw-rw-   0        0        0    11331 2022-12-02 11:11:42.000000 dgpost-2.0rc1/src/dgpost/transform/chromatography.py
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:43.169499 dgpost-2.0rc1/src/dgpost/transform/circuit_utils/
+-rw-rw-rw-   0        0        0        0 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/circuit_utils/__init__.py
+-rw-rw-rw-   0        0        0     6036 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/circuit_utils/circuit_components.py
+-rw-rw-rw-   0        0        0     6092 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/circuit_utils/circuit_parser.py
+-rw-rw-rw-   0        0        0    10330 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/electrochemistry.py
+-rw-rw-rw-   0        0        0    13936 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/impedance.py
+-rw-rw-rw-   0        0        0     6303 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/rates.py
+-rw-rw-rw-   0        0        0    15976 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/transform/reflection.py
+-rw-rw-rw-   0        0        0     7535 2022-11-10 17:08:25.000000 dgpost-2.0rc1/src/dgpost/transform/table.py
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:43.222933 dgpost-2.0rc1/src/dgpost/utils/
+-rw-rw-rw-   0        0        0      162 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/__init__.py
+-rw-rw-rw-   0        0        0    11124 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/extract.py
+-rw-rw-rw-   0        0        0    23481 2022-12-01 16:59:16.000000 dgpost-2.0rc1/src/dgpost/utils/helpers.py
+-rw-rw-rw-   0        0        0     2346 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/load.py
+-rw-rw-rw-   0        0        0     1298 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/parse.py
+-rw-rw-rw-   0        0        0     7061 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/plot.py
+-rw-rw-rw-   0        0        0     3253 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/save.py
+-rw-rw-rw-   0        0        0     1275 2022-11-10 12:13:22.000000 dgpost-2.0rc1/src/dgpost/utils/transform.py
+drwxrwxrwx   0        0        0        0 2022-12-02 11:12:43.034474 dgpost-2.0rc1/src/dgpost.egg-info/
+-rw-rw-rw-   0        0        0     3064 2022-12-02 11:12:42.000000 dgpost-2.0rc1/src/dgpost.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2022-12-02 11:12:42.000000 dgpost-2.0rc1/src/dgpost.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-02 11:12:42.000000 dgpost-2.0rc1/src/dgpost.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2022-12-02 11:12:42.000000 dgpost-2.0rc1/src/dgpost.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      241 2022-12-02 11:12:42.000000 dgpost-2.0rc1/src/dgpost.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2022-12-02 11:12:42.000000 dgpost-2.0rc1/src/dgpost.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    83320 2022-11-10 12:13:23.000000 dgpost-2.0rc1/versioneer.py
```

### Comparing `dgpost-2.0a4/LICENSE` & `dgpost-2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dgpost-2.0a4/PKG-INFO` & `dgpost-2.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgpost
-Version: 2.0a4
+Version: 2.0rc1
 Summary: datagram post-processing toolkit
 Home-page: https://github.com/dgbowl/dgpost
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/dgpost/issues
 Project-URL: Documentation, https://dgbowl.github.io/dgpost/
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dgpost-2.0a4/README.md` & `dgpost-2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dgpost-2.0a4/setup.py` & `dgpost-2.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,18 +36,19 @@
     install_requires=[
         "numpy",
         "uncertainties",
         "pandas",
         "openpyxl",
         "pint>=0.18",
         "chemicals>=1.0.0",
-        "rdkit-pypi>=2022",
+        "rdkit>=2022.3",
         "yadg>=4.1",
         "dgbowl-schemas>=106",
         "matplotlib>=3.5.0",
+        "requests",
     ],
     extras_require={
         "testing": [
             "pytest",
             "Pillow"
         ],
         "docs": [
```

### Comparing `dgpost-2.0a4/src/dgpost/_version.py` & `dgpost-2.0rc1/src/dgpost/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-08-18T09:08:18+0200",
+ "date": "2022-12-02T12:10:36+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "d259b0db4e9ccca8426a77919ba4164978bc165c",
- "version": "2.0a4"
+ "full-revisionid": "06c0b3399f5eb65422357e6f7be3e338baaa2e06",
+ "version": "2.0rc1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `dgpost-2.0a4/src/dgpost/main.py` & `dgpost-2.0rc1/src/dgpost/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,47 @@
 Module containing the execution functions for dgpost.
 
 """
 import argparse
 import logging
 from importlib import metadata
 import copy
+import requests
+import json
+from packaging import version
 
 from dgpost.utils import parse, load, extract, transform, save, plot
 from dgpost.utils.helpers import combine_tables
 
 logger = logging.getLogger(__name__)
 
 
+def version_check(project="dgpost"):
+    url = f"https://pypi.org/pypi/{project}/json"
+    try:
+        res = requests.get(url, timeout=1)
+    except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as e:
+        logger.debug(f"Version check could not proceed due to Exception={e}.")
+        return
+    jsdata = json.loads(res.text)
+    versions = sorted([version.parse(i) for i in jsdata["releases"].keys()])
+    latest = versions[-1]
+    current = version.parse(metadata.version(project))
+    if latest > current:
+        logger.warning("You are using an out-of-date version of '%s'. ", project)
+        logger.info(
+            "The latest version is '%s', the current version is '%s'.", latest, current
+        )
+        logger.info(
+            "Consider updating using: pip install --upgrade %s==%s", project, latest
+        )
+    else:
+        logger.debug("Your version of '%s' is up-to-date.", project)
+
+
 def run(path: str, patch: str = None) -> tuple[dict, dict]:
     """
     Main API execution function. Loads the `recipe` from the provided ``path``,
     patches the file paths specified within the `recipe`, if necessary, and
     processes the following entries, in order:
 
     - :mod:`~dgpost.utils.load`,
@@ -175,8 +201,9 @@
 
     args = parser.parse_args()
 
     loglevel = min(max(30 - (10 * args.verbose) + (10 * args.quiet), 10), 50)
     logging.basicConfig(level=loglevel)
     logging.debug(f"loglevel set to '{logging._levelToName[loglevel]}'")
 
+    version_check()
     run(args.infile, patch=args.patch)
```

### Comparing `dgpost-2.0a4/src/dgpost/transform/catalysis.py` & `dgpost-2.0rc1/src/dgpost/transform/catalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 
 Includes functions to calculate the reactant- and product-based 
 :func:`~dgpost.transform.catalysis.conversion`, atom-based 
 :func:`~dgpost.transform.catalysis.selectivity`,  
 :func:`~dgpost.transform.catalysis.catalytic_yield`, and 
 :func:`~dgpost.transform.catalysis.atom_balance`.
 
+.. rubric:: Functions
+
+.. autosummary::
+
+    atom_balance
+    catalytic_yield
+    conversion
+    selectivity
+
 Names of compounds within the specified mixtures are parsed to SMILES, and the
 cross-matching of the ``feestock``, internal ``standard``, and the components of 
 ``xin`` and ``xout`` (or ``rin`` and ``rout``) is performed using these SMILES.
 
 .. note::
 
     This module assumes that the provided inlet and outlet compositions, whether
```

### Comparing `dgpost-2.0a4/src/dgpost/transform/circuit_utils/circuit_components.py` & `dgpost-2.0rc1/src/dgpost/transform/circuit_utils/circuit_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+dgpost.transform.circuit_utils.circuit_components
+=================================================
+"""
 from typing import Type
 
 import numpy as np
 
 
 def create_parameter(name: str, bounds: tuple[float, float], unit: str):
     """
```

### Comparing `dgpost-2.0a4/src/dgpost/transform/circuit_utils/circuit_parser.py` & `dgpost-2.0rc1/src/dgpost/transform/circuit_utils/circuit_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+dgpost.transform.circuit_utils.circuit_parser
+=============================================
+"""
 import re
 import warnings
 import logging
 from typing import Callable, Tuple
 from scipy.optimize import least_squares, minimize
```

### Comparing `dgpost-2.0a4/src/dgpost/transform/electrochemistry.py` & `dgpost-2.0rc1/src/dgpost/transform/electrochemistry.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 Includes functions for calculating applied voltage correction via the 
 :func:`~dgpost.transform.electrochemistry.nernst` equation, calculation of the 
 Faradaic efficiency (:func:`~dgpost.transform.electrochemistry.fe`), as well as 
 the calculation of total :func:`~dgpost.transform.electrochemistry.charge`, and 
 the :func:`~dgpost.transform.electrochemistry.average_current` from the total 
 charge and timestamps.
 
+.. rubric:: Functions
+
+.. autosummary::
+
+    average_current
+    charge
+    fe
+    nernst
+
 """
 import pint
 from yadg.dgutils import ureg
 import numpy as np
 import pandas as pd
 from typing import Iterable
 from uncertainties import UFloat
@@ -182,15 +191,16 @@
     -------
     dict(output, E) : dict[str, pint.Quantity]
         Returns the calculated Faradaic efficiencies.
 
     """
     etot = abs(I) / (ureg("elementary_charge") * ureg("avogadro_constant"))
     if isinstance(etot.m, Iterable):
-        etot.m[etot.m == 0] = np.NaN
+        etotn, _, _ = separate_data(etot)
+        etot.m[etotn == 0] = np.NaN
     pretag = "fe" if output is None else output
     ret = {}
     for k, v in rate.items():
         kchem = name_to_chem(k)
         n = electrons_from_smiles(kchem.smiles, ions=charges)
         ek = v * n
         fek = ek / etot
```

### Comparing `dgpost-2.0a4/src/dgpost/transform/impedance.py` & `dgpost-2.0rc1/src/dgpost/transform/impedance.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 
 Including functions relevant for Electrochemical Impedance Spectroscopy (EIS):
 evaluation of an equivalent circuit as well as the fitting of the circuit to data 
 (:func:`~dgpost.transform.impedance.calc_circuit` and 
 :func:`~dgpost.transform.impedance.fit_circuit`), and an interpolation function 
 to find the :func:`~dgpost.transform.impedance.lowest_real_impedance` in the data.
 
+.. rubric:: Functions
+
+.. autosummary::
+
+    calc_circuit
+    fit_circuit
+    lowest_real_impedance
+
 .. note::
     The functions in this module expect the whole EIS trace as input - the 
     :math:`\\text{Re}(Z)`, :math:`-\\text{Im}(Z)` and :math:`f` are expected to
     be :class:`pint.Quantity` containing an :class:`np.ndarray` (or similar 
     :class:`list`-like object), which is then processed to a (set of) scalar 
     values. This means that for processing time resolved data, the functions
     in this module have to be called on each timestep individually.
```

### Comparing `dgpost-2.0a4/src/dgpost/transform/rates.py` & `dgpost-2.0rc1/src/dgpost/transform/rates.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 Includes functions to convert mixture compositions (concentration, mol fraction) 
 from instantaneous flow data or continuous batch data to rates (dimension of 
 ``[quantity]/[time]``). The :func:`~dgpost.transform.rates.flow_to_molar` function
 is useful for converting gas-phase or liquid flows, while 
 :func:`~dgpost.transform.rates.batch_to_molar` can be used to determine formation 
 rates from the concentration profile of a batch mixture.
 
+.. rubric:: Functions
+
+.. autosummary::
+  
+    batch_to_molar
+    flow_to_molar
+
 """
 import pint
 from yadg.dgutils import ureg
 import pandas as pd
 import numpy as np
 from typing import Iterable
```

### Comparing `dgpost-2.0a4/src/dgpost/utils/extract.py` & `dgpost-2.0rc1/src/dgpost/utils/extract.py`

 * *Files identical despite different names*

### Comparing `dgpost-2.0a4/src/dgpost/utils/helpers.py` & `dgpost-2.0rc1/src/dgpost/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import pint
 import functools
 import pandas as pd
 import numpy as np
 from uncertainties import unumpy as unp
 from rdkit import Chem
+from inspect import signature
 
 from collections import defaultdict
 from typing import Any, Union, Sequence
 from chemicals.elements import periodic_table, simple_formula_parser
 from chemicals.identifiers import search_chemical
 from yadg.dgutils import ureg
 import logging
@@ -141,14 +142,16 @@
     -------
     Quantity: pint.Quantity
         Unit-aware :class:`ping.Quantity` object containing the data from ``df[col]``.
 
     """
     if df.columns.nlevels == 1:
         vals = df[col].array
+    elif isinstance(col, tuple) and len(col) == df.columns.nlevels:
+        vals = df[col].array
     else:
         vals = df[col].squeeze().array
     if unit is not None:
         pass
     else:
         unit = get_units(col, df)
     return ureg.Quantity(vals, unit)
@@ -257,17 +260,20 @@
                 # Check if the dataframe has a units attribute. If not, the quantities
                 # in the dataframe are unitless and need to be converted.
                 if "units" in df.attrs:
                     uconv = False
                 else:
                     uconv = True
 
+                # keep original kwargs cname-cval keypairs in orig_kwargs
+                orig_kwargs = {}
                 data_kwargs = {}
                 for cname, cunit, ctype in fcols:
                     cval = kwargs.pop(cname, None)
+                    orig_kwargs[cname] = cval
                     if ctype is pd.Index and cval is None:
                         # if ctype is pd.Index, it can still be overriden by cval
                         # otherwise send the df.index wrapped in cunit
                         data_kwargs[cname] = ureg.Quantity(df.index, cunit)
                     elif cval is None:
                         # cval is optional -> we want to let func use its default
                         continue
@@ -306,33 +312,59 @@
                             c = key[-1]
                             if uconv:
                                 temp[c] = pQ(df, key, unit=cunit)
                             else:
                                 temp[c] = pQ(df, key)
                         data_kwargs[cname] = temp
 
+                # if the called function requires the names of columns,
+                # it can ask for them by having _inp in its signature
+                if "_inp" in signature(func).parameters:
+                    kwargs["_inp"] = orig_kwargs
+
                 units = {}
                 # if a "list" is specified as type, we need to transpose the input:
                 if list in {col[2] for col in fcols}:
-                    row_k = data_kwargs.keys()
-                    row_v = data_kwargs.values()
+                    if all([col[2] is list for col in fcols]):
+                        row_k = data_kwargs.keys()
+                        row_v = data_kwargs.values()
+                    else:
+                        row_k = []
+                        row_v = []
+                        to_pad = []
+                        for k, v in data_kwargs.items():
+                            for col in fcols:
+                                if k == col[0] and col[2] is list:
+                                    row_k.append(k)
+                                    row_v.append(v)
+                                elif k == col[0] and col[2] is None:
+                                    row_k.append(k)
+                                    row_v.append([v])
+                                    to_pad.append(len(row_k) - 1)
+                        l = max([len(i) for i in row_v])
+                        for i in to_pad:
+                            row_v[i] = row_v[i] * l
                     ret_data = {}
-                    for r in zip(*row_v):
+                    for ri, r in enumerate(zip(*row_v)):
                         row_data = {k: v for k, v in zip(row_k, r)}
                         retvals = func(**row_data, **kwargs)
                         for name, qty in retvals.items():
                             if name not in ret_data:
-                                ret_data[name] = []
+                                ret_data[name] = [None] * ri
                             if isinstance(qty, pint.Quantity):
                                 qty.ito_reduced_units()
                                 ret_data[name].append(qty.m)
                                 if not uconv and not qty.unitless:
                                     units[name] = f"{qty.u:~P}"
                             else:
                                 ret_data[name].append(qty)
+                        for name in ret_data.keys():
+                            if name not in retvals:
+                                ret_data[name].append(None)
+                    print(f"{ret_data}=")
                 else:
                     retvals = func(**data_kwargs, **kwargs)
                     ret_data = {}
                     for name, qty in retvals.items():
                         if isinstance(qty, pint.Quantity):
                             qty.ito_reduced_units()
                             ret_data[name] = qty.m
```

### Comparing `dgpost-2.0a4/src/dgpost/utils/load.py` & `dgpost-2.0rc1/src/dgpost/utils/load.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,25 +18,27 @@
 
 """
 import os
 import json
 import pandas as pd
 from yadg.core import validate_datagram
 from uncertainties import ufloat_fromstr, UFloat
-import re
 from typing import Union, Any
 import logging
 from dgpost.utils.helpers import arrow_to_multiindex
 
 logger = logging.getLogger(__name__)
 
 
 def _parse_ufloat(v: Union[str, Any]) -> Union[UFloat, Any]:
-    if isinstance(v, str) and re.match(r"[0-9\.]+\+/-[0-9\.]+", v):
-        return ufloat_fromstr(v)
+    if isinstance(v, str):
+        try:
+            return ufloat_fromstr(v)
+        except ValueError:
+            return v
     else:
         return v
 
 
 def load(
     path: str,
     check: bool = True,
```

### Comparing `dgpost-2.0a4/src/dgpost/utils/parse.py` & `dgpost-2.0rc1/src/dgpost/utils/parse.py`

 * *Files identical despite different names*

### Comparing `dgpost-2.0a4/src/dgpost/utils/plot.py` & `dgpost-2.0rc1/src/dgpost/utils/plot.py`

 * *Files identical despite different names*

### Comparing `dgpost-2.0a4/src/dgpost/utils/save.py` & `dgpost-2.0rc1/src/dgpost/utils/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
             names.append((col[0] + f" [{ureg.Unit(unit):~P}]", *col[1:]))
 
     savedf = table.copy()
     if all([isinstance(name, str) for name in names]):
         savedf.columns = pd.Index(names)
     else:
         savedf.columns = pd.MultiIndex.from_tuples(names)
+    savedf = savedf.sort_index(axis="columns")
     if type == "csv":
         logger.debug("Writing csv into '%s'." % path)
         savedf.to_csv(path)
     elif type == "xlsx":
         logger.debug("Writing xlsx into '%s'." % path)
         savedf.to_excel(path)
     else:
```

### Comparing `dgpost-2.0a4/src/dgpost/utils/transform.py` & `dgpost-2.0rc1/src/dgpost/utils/transform.py`

 * *Files identical despite different names*

### Comparing `dgpost-2.0a4/src/dgpost.egg-info/PKG-INFO` & `dgpost-2.0rc1/src/dgpost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgpost
-Version: 2.0a4
+Version: 2.0rc1
 Summary: datagram post-processing toolkit
 Home-page: https://github.com/dgbowl/dgpost
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/dgpost/issues
 Project-URL: Documentation, https://dgbowl.github.io/dgpost/
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dgpost-2.0a4/src/dgpost.egg-info/SOURCES.txt` & `dgpost-2.0rc1/src/dgpost.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 src/dgpost.egg-info/SOURCES.txt
 src/dgpost.egg-info/dependency_links.txt
 src/dgpost.egg-info/entry_points.txt
 src/dgpost.egg-info/requires.txt
 src/dgpost.egg-info/top_level.txt
 src/dgpost/transform/__init__.py
 src/dgpost/transform/catalysis.py
+src/dgpost/transform/chromatography.py
 src/dgpost/transform/electrochemistry.py
 src/dgpost/transform/impedance.py
 src/dgpost/transform/rates.py
+src/dgpost/transform/reflection.py
 src/dgpost/transform/table.py
 src/dgpost/transform/circuit_utils/__init__.py
 src/dgpost/transform/circuit_utils/circuit_components.py
 src/dgpost/transform/circuit_utils/circuit_parser.py
 src/dgpost/utils/__init__.py
 src/dgpost/utils/extract.py
 src/dgpost/utils/helpers.py
```

### Comparing `dgpost-2.0a4/versioneer.py` & `dgpost-2.0rc1/versioneer.py`

 * *Files identical despite different names*

