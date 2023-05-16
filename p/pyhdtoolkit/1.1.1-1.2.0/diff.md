# Comparing `tmp/pyhdtoolkit-1.1.1.tar.gz` & `tmp/pyhdtoolkit-1.2.0.tar.gz`

## Comparing `pyhdtoolkit-1.1.1.tar` & `pyhdtoolkit-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/.codeclimate.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/.zenodo.json
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/Makefile
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/version.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/__init__.py
--rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/_generators.py
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/constants.py
--rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/coupling.py
--rw-r--r--   0        0        0    14264 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/matching.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/parameters.py
--rw-r--r--   0        0        0    15984 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/ptc.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/track.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/tune.py
--rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/twiss.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/utils.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/__init__.py
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_coupling.py
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_elements.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_errors.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_misc.py
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_powering.py
--rw-r--r--   0        0        0    12369 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_queries.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_routines.py
--rw-r--r--   0        0        0    21216 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_setup.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_twiss.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/maths/__init__.py
--rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/maths/nonconvex_phase_sync.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/maths/stats_fitting.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/maths/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/models/__init__.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/models/beam.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/models/htc.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/models/madx.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/optics/__init__.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/optics/beam.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/optics/ripken.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/optics/twiss.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/__init__.py
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/aperture.py
--rw-r--r--   0        0        0    10314 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/crossing.py
--rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/envelope.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/lattice.py
--rw-r--r--   0        0        0    13302 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/layout.py
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/phasespace.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/tune.py
--rw-r--r--   0        0        0    16622 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/utils.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/sbs/coupling.py
--rw-r--r--   0        0        0     8932 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/sbs/phase.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/styles/__init__.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/styles/paper.py
--rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/styles/thesis.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/_misc.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/cmdline.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/contexts.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/executors.py
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/htc_monitor.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/logging.py
--rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/operations.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyhdtoolkit/utils/printutil.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/LICENSE
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/README.md
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 pyhdtoolkit-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/.codeclimate.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/.zenodo.json
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/Makefile
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/version.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/__init__.py
+-rw-r--r--   0        0        0    15024 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/_generators.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/constants.py
+-rw-r--r--   0        0        0    14166 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/coupling.py
+-rw-r--r--   0        0        0    17947 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/matching.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/parameters.py
+-rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/ptc.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/track.py
+-rw-r--r--   0        0        0    15404 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/tune.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/twiss.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/utils.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/__init__.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_coupling.py
+-rw-r--r--   0        0        0    12990 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_elements.py
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_errors.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_misc.py
+-rw-r--r--   0        0        0    17925 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_powering.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_queries.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_routines.py
+-rw-r--r--   0        0        0    21324 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_setup.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_twiss.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/maths/__init__.py
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/maths/nonconvex_phase_sync.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/maths/stats_fitting.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/maths/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/models/__init__.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/models/beam.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/models/htc.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/models/madx.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/optics/__init__.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/optics/beam.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/optics/ripken.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/optics/twiss.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/__init__.py
+-rw-r--r--   0        0        0    14726 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/aperture.py
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/crossing.py
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/envelope.py
+-rw-r--r--   0        0        0    13069 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/lattice.py
+-rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/layout.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/phasespace.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/tune.py
+-rw-r--r--   0        0        0    19836 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/utils.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/sbs/coupling.py
+-rw-r--r--   0        0        0     8932 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/sbs/phase.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/styles/__init__.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/styles/paper.py
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/styles/thesis.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/_misc.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/cmdline.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/contexts.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/executors.py
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/htc_monitor.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/logging.py
+-rw-r--r--   0        0        0    32032 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/operations.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyhdtoolkit/utils/printutil.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/README.md
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 pyhdtoolkit-1.2.0/PKG-INFO
```

### Comparing `pyhdtoolkit-1.1.1/.codeclimate.yml` & `pyhdtoolkit-1.2.0/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/Makefile` & `pyhdtoolkit-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/__init__.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/version.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "1.1.1"
+VERSION = "1.2.0"
 
 
 def version_info() -> str:
     """Debug convenience function to give version, platform and runtime information."""
     import platform
     import sys
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/_generators.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/_generators.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/constants.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
                                     "beta21", "beta22"]
 MONITOR_TWISS_COLUMNS: List[str] = ["name", "s", "betx", "bety", "alfx", "alfy", "mux", "muy", "dx", "dy",
                                     "dpx", "dpy", "x", "y", "ddx", "ddy", "k1l", "k1sl", "k2l", "k3l", "k4l",
                                     "wx", "wy", "phix", "phiy", "dmux", "dmuy", "keyword", "dbx", "dby",
                                     "r11", "r12", "r21", "r22"]
 # fmt: on
 
+# Needs to be formatted
+LHC_IR_BPM_REGEX = r"BPM\S?\S?\.[0-{max_index}][LR][1258]\.*"
+
 # MQX + maybe F (1/3 in HLLHC) + A (1/3) or B (2) + . + maybe A or B (2) + triplet number (1/2/3) + side (R/L) + IP number (1/2/5/8)
 LHC_TRIPLETS_REGEX = "^MQXF?[AB].[AB]?[123][RL][1258]"
 
 # This might not be accurate anymore
 LHC_CROSSING_SCHEMES: Dict[str, Dict[str, float]] = {
     "flat": {},
     "lhc_inj": {
@@ -151,40 +154,40 @@
     for sector in [1, 2, 3, 4, 5, 6, 7, 8]
 ]
 
 HLLHC_CORRECTOR_LIMITS: Dict[str, float] = {  # All values are defined as multiples of 0.3/Energy
     "MQSX1": 0.600 / 0.050,  # 0.6 T.m @ 50 mm in IR1&IR5
     "MQSX2": 1.360 / 0.017,  # 1.36 T @ 17 mm in IR2&IR8
     # ------------- #
-    "MCSX1": 0.050 * 2 / (0.050 ** 2),  # 0.050 Tm @ 50 mm in IR1&IR5
-    "MCSX2": 0.028 * 2 / (0.017 ** 2),  # 0.028 T @ 17 mm in IR2&IR8
+    "MCSX1": 0.050 * 2 / (0.050**2),  # 0.050 Tm @ 50 mm in IR1&IR5
+    "MCSX2": 0.028 * 2 / (0.017**2),  # 0.028 T @ 17 mm in IR2&IR8
     # ------------- #
-    "MCSSX1": 0.050 * 2 / (0.050 ** 2),  # 0.050 Tm @ 50 mm in IR1&IR5
-    "MCSSX2": 0.11 * 2 / (0.017 ** 2),  # 0.11 T @ 17 mm in IR2&IR8
+    "MCSSX1": 0.050 * 2 / (0.050**2),  # 0.050 Tm @ 50 mm in IR1&IR5
+    "MCSSX2": 0.11 * 2 / (0.017**2),  # 0.11 T @ 17 mm in IR2&IR8
     # ------------- #
-    "MCOX1": 0.030 * 6 / (0.050 ** 3),  # 0.030 Tm @ 50 mm in IR1&IR5
-    "MCOX2": 0.045 * 6 / (0.017 ** 3),  # 0.045 T @ 17 mm in IR2&IR8
+    "MCOX1": 0.030 * 6 / (0.050**3),  # 0.030 Tm @ 50 mm in IR1&IR5
+    "MCOX2": 0.045 * 6 / (0.017**3),  # 0.045 T @ 17 mm in IR2&IR8
     # ------------- #
-    "MCOSX1": 0.030 * 6 / (0.050 ** 3),  # 0.030 Tm @ 50 mm in IR1&IR5
-    "MCOSX2": 0.048 * 6 / (0.017 ** 3),  # 0.048 T @ 17 mm in IR2&IR8
+    "MCOSX1": 0.030 * 6 / (0.050**3),  # 0.030 Tm @ 50 mm in IR1&IR5
+    "MCOSX2": 0.048 * 6 / (0.017**3),  # 0.048 T @ 17 mm in IR2&IR8
     # ------------- #
-    "MCDX1": 0.030 * 24 / (0.050 ** 4),  # 0.030 Tm @ 50 mm in IR1&IR5
+    "MCDX1": 0.030 * 24 / (0.050**4),  # 0.030 Tm @ 50 mm in IR1&IR5
     # ------------- #
-    "MCDSX1": 0.030 * 24 / (0.050 ** 4),  # 0.030 Tm @ 50 mm in IR1&IR5
+    "MCDSX1": 0.030 * 24 / (0.050**4),  # 0.030 Tm @ 50 mm in IR1&IR5
     # ------------- #
-    "MCTX1": 0.07 * 120 / (0.050 ** 5),  # 0.070 Tm @ 50 mm in IR1&IR5
-    "MCTX2": 0.01 * 120 / (0.017 ** 5),  # 0.010 Tm @ 17 mm in IR1&IR5
+    "MCTX1": 0.07 * 120 / (0.050**5),  # 0.070 Tm @ 50 mm in IR1&IR5
+    "MCTX2": 0.01 * 120 / (0.017**5),  # 0.010 Tm @ 17 mm in IR1&IR5
     # ------------- #
-    "MCTSX1": 0.07 * 120 / (0.050 ** 5),  # 0.070 Tm @ 50 mm in IR1&IR5
+    "MCTSX1": 0.07 * 120 / (0.050**5),  # 0.070 Tm @ 50 mm in IR1&IR5
     "MQT": 120,  # 120 T/m
     "MQS": 120,  # 120 T/m
-    "MS": 1.280 * 2 / (0.017 ** 2),  # 1.28 T @ 17 mm
-    "MSS": 1.280 * 2 / (0.017 ** 2),  # 1.28 T @ 17 mm
-    "MCS": 0.471 * 2 / (0.017 ** 2),  # 0.471 T @ 17 mm
-    "MCO": 0.040 * 6 / (0.017 ** 3),  # 0.04 T @ 17 mm
-    "MCD": 0.100 * 24 / (0.017 ** 4),  # 0.1 T @ 17 mm
-    "MO": 0.29 * 6 / (0.017 ** 3),  # 0.29 T @ 17 mm
+    "MS": 1.280 * 2 / (0.017**2),  # 1.28 T @ 17 mm
+    "MSS": 1.280 * 2 / (0.017**2),  # 1.28 T @ 17 mm
+    "MCS": 0.471 * 2 / (0.017**2),  # 0.471 T @ 17 mm
+    "MCO": 0.040 * 6 / (0.017**3),  # 0.04 T @ 17 mm
+    "MCD": 0.100 * 24 / (0.017**4),  # 0.1 T @ 17 mm
+    "MO": 0.29 * 6 / (0.017**3),  # 0.29 T @ 17 mm
 }
 
 FD_FAMILIES: Set[str] = {"MO", "MS", "MQT"}  # Magnets that have F and D families
 TWO_FAMILIES: Set[str] = {"MS"}  # Magnets that have 1 and 2 families
 SPECIAL_FAMILIES: Set[str] = {"MQS"}  # Magnets in every second arc
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/coupling.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/coupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from pyhdtoolkit.cpymadtools.twiss import get_pattern_twiss, get_twiss_tfs
 
 # ----- General Use ----- #
 
 
 def get_closest_tune_approach(
     madx: Madx,
+    /,
     accelerator: str = None,
     sequence: str = None,
     varied_knobs: Sequence[str] = None,
     telescopic_squeeze: bool = True,
     run3: bool = False,
     explicit_targets: Tuple[float, float] = None,
     step: float = 1e-7,
@@ -48,15 +49,15 @@
     under the hood.
 
     .. note::
         This assumes the sequence has previously been matched to the user's desired working point, as if not
         explicitely given, the appropriate targets will be determined from the ``MAD-X`` internal tables.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         accelerator (Optional[str]): name of the accelerator, used to determmine knobs if *variables* is not given.
             Automatic determination will only work for `LHC` and `HLLHC`.
         sequence (str): name of the sequence you want to activate for the tune matching.
         varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH`` routine. An input
             could be ``["kqf", "ksd", "kqf", "kqd"]`` as they are common names used for quadrupole and sextupole
             strengths (focusing / defocusing) in most examples.
         telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for Telescopic
@@ -139,14 +140,15 @@
     madx.command.twiss()  # make sure TWISS and SUMM tables are returned to their original state
 
     return cminus
 
 
 def get_cminus_from_coupling_rdts(
     madx: Madx,
+    /,
     patterns: Sequence[str] = [""],
     method: str = "teapot",
     qx: float = None,
     qy: float = None,
     filtering: float = 0,
 ) -> float:
     """
@@ -162,15 +164,15 @@
         normalizations, which is the use-case of this functions.
 
     .. note::
         If using the “calaga”, “teapot”, “teapot_franchi” or “franchi” method, then the returned
         value will be a real number.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         patterns (Sequence[str]): the different patterns (such as ``MQX`` or ``BPM``) of elements
             to use when computing the coupling RDTs. Defaults to `[""]` which will select and use
             all elements in the ``TWISS`` outputs.
         method (str): the method to use for the calculation of the :math:`C^{-}`. Defaults to
             `teapot`, which is the default of `~optics_functions.coupling.closest_tune_approach`.
         qx (float): the horizontal tune. Defaults to `None`, in which case the value will be taken
             from the ``SUMM`` table.
@@ -227,24 +229,24 @@
         dqmin_df = dqmin_df.abs()
 
     # Now we can take the mean of the DELTAQMIN column
     return dqmin_df.DELTAQMIN.mean()
 
 
 def match_no_coupling_through_ripkens(
-    madx: Madx, sequence: str = None, location: str = None, vary_knobs: Sequence[str] = None
+    madx: Madx, /, sequence: str = None, location: str = None, vary_knobs: Sequence[str] = None
 ) -> None:
     """
     .. versionadded:: 0.16.0
 
     Matching routine to get cross-term Ripken parameters :math:`\\beta_{12}` and :math:`\\beta_{21}`
     to be 0 at a given location.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         sequence (str): name of the sequence to activate for the matching.
         location (str): the name of the element at which one wants the cross-term Ripkens to be 0.
         vary_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` routine.
 
     Example:
         .. code-block:: python
 
@@ -263,23 +265,23 @@
     madx.command.use_macro(name="do_ripken")
     madx.input(f"constraint, expr=table(twiss, {location}, beta12)=0")  # need input else includes " and fails
     madx.input(f"constraint, expr=table(twiss, {location}, beta21)=0")  # need input else includes " and fails
     madx.command.lmdif(calls=500, tolerance=1e-21)
     madx.command.endmatch()
 
 
-def get_coupling_rdts(madx: Madx, **kwargs) -> tfs.TfsDataFrame:
+def get_coupling_rdts(madx: Madx, /, **kwargs) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.20.0
 
-    Computed the coupling Resonance Driving Tensors (RDTs) :math:`f_{1001}` and :math:`f_{1010}`
+    Computed the coupling Resonance Driving Terms (RDTs) :math:`f_{1001}` and :math:`f_{1010}`
     at all elements in the currently active sequence from a ``TWISS`` call.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         **kwargs: any keyword argument will be transmitted to the ``TWISS`` command in ``MAD-X``.
 
     Returns:
         A `~tfs.TfsDataFrame` with columns of the ``TWISS`` table, and two complex columns for the
         ``F1001`` and ``f1010`` RDTs.
 
     Example:
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/matching.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/matching.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pyhdtoolkit.cpymadtools.lhc import get_lhc_tune_and_chroma_knobs
 
 # ----- Workhorse ----- #
 
 
 def match_tunes_and_chromaticities(
     madx: Madx,
+    /,
     accelerator: str = None,
     sequence: Optional[str] = None,
     q1_target: float = None,
     q2_target: float = None,
     dq1_target: float = None,
     dq2_target: float = None,
     varied_knobs: Sequence[str] = None,
@@ -41,49 +42,57 @@
     `MAD-X manual <http://madx.web.cern.ch/madx/releases/last-rel/madxuguide.pdf>`_.
 
     One can find example use of this function in the :ref:`lattice plotting <demo-accelerator-lattice>`,
     :ref:`rigid waist shift <demo-rigid-waist-shift>` or :ref:`phase space <demo-phase-space>` example
     galleries.
 
     .. important::
-        If target tune values only are provided, then tune matching is performed with the provided knobs.
-        If target chromaticity values only are provided, then chromaticity matching is performed with the
-        provided knobs. If targets for both types are provided, then both are matched in a single call with
-        the provided knobs.
+        If target tune values only are provided, then tune matching is performed with the
+        provided knobs. If target chromaticity values only are provided, then chromaticity
+        matching is performed with the provided knobs. If targets for both types are provided,
+        then both are matched in a single call with the provided knobs.
 
     .. note::
-        If the user wishes to perform different matching calls for each, then it is recommended to call this
-        function as many times as necessary, with the appropriate targets.
+        If the user wishes to perform different matching calls for each, then it is recommended
+        to call this function as many times as necessary, with the appropriate targets.
 
-        For instance, in some cases and machines some prefer to do a tune matching followed by a chromaticity matching,
-        then followed by a combined matching. In this case the function should be called three times, once with tune
-        targets and knobs, another time with chromaticity targets and knobs, then a final time with all of the above.
-        For this, simple wrappers are provided: the :func:`match_tunes` and :func:`match_chromaticities` functions.
+        For instance, in some cases and machines some prefer to do a tune matching followed by
+        a chromaticity matching, then followed by a combined matching. In this case the function
+        should be called three times, once with tune targets and knobs, another time with
+        chromaticity targets and knobs, then a final time with all of the above. For this, simple
+        wrappers are provided: the :func:`match_tunes` and :func:`match_chromaticities` functions.
 
     .. hint::
-        When acting of either the ``LHC`` or ``HLLHC`` machines, the accelerator name can be provided and the vary
-        knobs will be automatically set accordingly to the provided targets. Note that only the relevant knobs are
-        set, so if tune targets only are provided, then tune knobs only will be used, and not chromaticity knobs.
-        If explicit knobs are provided, these will always be used. On other machines the knobs should be provided
-        explicitly, always.
+        When acting of either the ``LHC`` or ``HLLHC`` machines, the accelerator name can be
+        provided and the vary knobs will be automatically set accordingly to the provided targets.
+        Note that only the relevant knobs are set, so if tune targets only are provided, then tune
+        knobs only will be used, and not chromaticity knobs. If explicit knobs are provided, these
+        will always be used. On other machines the knobs should be provided explicitly, always.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
-        accelerator (Optional[str]): name of the accelerator, used to determmine knobs if *variables* is not given.
-            Automatic determination will only work for ``LHC`` and ``HLLHC``.
-        sequence (str): name of the sequence you want to perform the matching for.
-        q1_target (float): horizontal tune to match to.
-        q2_target (float): vertical tune to match to.
-        dq1_target (float): horizontal chromaticity to match to.
-        dq2_target (float): vertical chromaticity to match to.
-        varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH`` routine. An input
-            could be ``["kqf", "ksd", "kqf", "kqd"]`` as they are common names used for quadrupole and sextupole
-            strengths (focusing / defocusing) in most examples.
-        telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for Telescopic
-            Squeeze configuration. Defaults to `True` since `v0.9.0`.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
+        accelerator (Optional[str]): name of the accelerator, used to determmine knobs if
+            *variables* is not given. Automatic determination will only work for ``LHC`` and
+            ``HLLHC``. Defaults to `None`, in which case the knobs must be provided explicitly
+            through ``varied_knobs``.
+        sequence (str): name of the sequence you want to perform the matching for. Defaults to
+            `None`, in which case the currently active sequence will be used for the matching.
+        q1_target (float): horizontal tune to match to. Defaults to `None`, in which case it will
+            not be a target and will be excluded from the matching.
+        q2_target (float): vertical tune to match to. Defaults to `None`, in which case it will
+            not be a target and will be excluded from the matching.
+        dq1_target (float): horizontal chromaticity to match to. Defaults to `None`, in which case
+            it will not be a target and will be excluded from the matching.
+        dq2_target (float): vertical chromaticity to match to. Defaults to `None`, in which case it
+            will not be a target and will be excluded from the matching.
+        varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH``
+            routine. An example input could be ``["kqf", "ksd", "kqf", "kqd"]`` as they are common
+            names used for quadrupole and sextupole strengths (focusing / defocusing) in most examples.
+        telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for
+            Telescopic Squeeze configuration. Defaults to `True` since `v0.9.0`.
         run3 (bool): if set to `True`, uses the ``LHC`` Run 3 `*_op` knobs. Defaults to `False`.
         step (float): step size to use when varying knobs.
         calls (int): max number of varying calls to perform. Defaults to 100.
         tolerance (float): tolerance for successfull matching. Defaults to :math:`10^{-21}`.
 
     Examples:
         Matching a dummy lattice (not LHC or HLLHC):
@@ -97,15 +106,30 @@
             ...     q1_target=6.335,
             ...     q2_target=6.29,
             ...     dq1_target=100,
             ...     dq2_target=100,
             ...     varied_knobs=["kqf", "kqd", "ksf", "ksd"],
             ... )
 
-        Matching the LHC lattice:
+        Note that since the ``accelerator`` and ``sequence`` arguments default to `None`,
+        they can be omitted. In this case the sequence currently in use will be used for
+        the matching, and ``varied_knobs`` must be provided.
+
+        .. code-block:: python
+
+            >>> matching.match_tunes_and_chromaticities(
+            ...     madx,
+            ...     q1_target=6.335,
+            ...     q2_target=6.29,
+            ...     dq1_target=100,
+            ...     dq2_target=100,
+            ...     varied_knobs=["kqf", "kqd", "ksf", "ksd"],
+            ... )
+
+        Matching the ``lhcb1`` sequence of the ``LHC`` lattice:
 
         .. code-block:: python
 
             >>> matching.match_tunes_and_chromaticities(
             ...     madx,
             ...     "lhc",                    # will find the knobs automatically
             ...     sequence="lhcb1",
@@ -163,49 +187,57 @@
 
 
 # ----- Convenient Wrappers ----- #
 
 
 def match_tunes(
     madx: Madx,
+    /,
     accelerator: str = None,
     sequence: Optional[str] = None,
     q1_target: float = None,
     q2_target: float = None,
     varied_knobs: Sequence[str] = None,
     telescopic_squeeze: bool = True,
     run3: bool = False,
     step: float = 1e-7,
     calls: int = 100,
     tolerance: float = 1e-21,
 ):
     """
     .. versionadded:: 0.17.0
 
-    Provided with an active `~cpymad.madx.Madx` object, will run relevant commands to match tunes to
-    the desired target values.
+    Provided with an active `~cpymad.madx.Madx` object, will run relevant commands
+    to match tunes to the desired target values.
 
     .. note::
-        This is a wrapper around the `~.match_tunes_and_chromaticities` function. Refer to its documentation
-        for usage details.
+        This is a wrapper around the `~.match_tunes_and_chromaticities` function. Refer
+        to its documentation for usage details.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
-        accelerator (Optional[str]): name of the accelerator, used to determmine knobs if *variables* is not given.
-            Automatic determination will only work for `LHC` and `HLLHC`.
-        sequence (str): name of the sequence you want to perform the matching for.
-        q1_target (float): horizontal tune to match to.
-        q2_target (float): vertical tune to match to.
-        varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH`` routine.
-        telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for Telescopic
-            Squeeze configuration. Defaults to `True` since `v0.9.0`.
-        run3 (bool): if set to `True`, uses the `LHC` Run 3 `*_op` knobs. Defaults to `False`.
-        step (float): step size to use when varying knobs. Defaults to `1E-7`.
-        calls (int): max number of varying calls to perform. Defaults to `100`.
-        tolerance (float): tolerance for successfull matching. Defaults to `1E-21`.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
+        accelerator (Optional[str]): name of the accelerator, used to determmine knobs if
+            *variables* is not given. Automatic determination will only work for ``LHC`` and
+            ``HLLHC``. Defaults to `None`, in which case the knobs must be provided explicitly
+            through ``varied_knobs``.
+        sequence (str): name of the sequence you want to perform the matching for. Defaults to
+            `None`, in which case the currently active sequence will be used for the matching.
+        q1_target (float): horizontal tune to match to. Defaults to `None`, in which case it will
+            not be a target and will be excluded from the matching.
+        q2_target (float): vertical tune to match to. Defaults to `None`, in which case it will
+            not be a target and will be excluded from the matching.
+        varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH``
+            routine. An example input could be ``["kqf", "ksd", "kqf", "kqd"]`` as they are common
+            names used for quadrupole and sextupole strengths (focusing / defocusing) in most examples.
+        telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for
+            Telescopic Squeeze configuration. Defaults to `True` since `v0.9.0`.
+        run3 (bool): if set to `True`, uses the ``LHC`` Run 3 `*_op` knobs. Defaults to `False`.
+        step (float): step size to use when varying knobs.
+        calls (int): max number of varying calls to perform. Defaults to 100.
+        tolerance (float): tolerance for successfull matching. Defaults to :math:`10^{-21}`.
 
     Examples:
         Matching a dummy lattice (not LHC or HLLHC):
 
         .. code-block:: python
 
             >>> matching.match_tunes(
@@ -213,28 +245,41 @@
             ...     None,              # this is not LHC or HLLHC
             ...     sequence="CAS3",
             ...     q1_target=6.335,
             ...     q2_target=6.29,
             ...     varied_knobs=["kqf", "kqd"],  # only tune knobs
             ... )
 
+        Note that since the ``accelerator`` and ``sequence`` arguments default to `None`,
+        they can be omitted. In this case the sequence currently in use will be used for
+        the matching, and ``varied_knobs`` must be provided.
+
+        .. code-block:: python
+
+            >>> matching.match_tunes_and_chromaticities(
+            ...     madx,
+            ...     q1_target=6.335,
+            ...     q2_target=6.29,
+            ...     varied_knobs=["kqf", "kqd"],  # only tune knobs
+            ... )
+
         Matching the LHC lattice:
 
         .. code-block:: python
 
             >>> matching.match_tunes(
             ...     madx,
             ...     "lhc",                    # will find the knobs automatically
             ...     sequence="lhcb1",
             ...     q1_target=62.31,
             ...     q2_target=60.32,
             ... )
     """
     match_tunes_and_chromaticities(
-        madx=madx,
+        madx,
         accelerator=accelerator,
         sequence=sequence,
         q1_target=q1_target,
         q2_target=q2_target,
         dq1_target=None,
         dq2_target=None,
         varied_knobs=varied_knobs,
@@ -244,49 +289,57 @@
         calls=calls,
         tolerance=tolerance,
     )
 
 
 def match_chromaticities(
     madx: Madx,
+    /,
     accelerator: str = None,
     sequence: Optional[str] = None,
     dq1_target: float = None,
     dq2_target: float = None,
     varied_knobs: Sequence[str] = None,
     telescopic_squeeze: bool = True,
     run3: bool = False,
     step: float = 1e-7,
     calls: int = 100,
     tolerance: float = 1e-21,
 ):
     """
     .. versionadded:: 0.17.0
 
-    Provided with an active `~cpymad.madx.Madx` object, will run relevant commands to match chromaticities
-    to the desired target values.
+    Provided with an active `~cpymad.madx.Madx` object, will run relevant commands
+    to match chromaticities to the desired target values.
 
     .. note::
-        This is a wrapper around the `~.match_tunes_and_chromaticities` function. Refer to its documentation
-        for usage details.
+        This is a wrapper around the `~.match_tunes_and_chromaticities` function.
+        Refer to its documentation for usage details.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
-        accelerator (Optional[str]): name of the accelerator, used to determmine knobs if *variables* is not given.
-            Automatic determination will only work for `LHC` and `HLLHC`.
-        sequence (str): name of the sequence you want to perform the matching for.
-        q1_target (float): horizontal tune to match to.
-        q2_target (float): vertical tune to match to.
-        varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH`` routine.
-        telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for Telescopic
-            Squeeze configuration. Defaults to `True` since `v0.9.0`.
-        run3 (bool): if set to `True`, uses the `LHC` Run 3 `*_op` knobs. Defaults to `False`.
-        step (float): step size to use when varying knobs. Defaults to `1E-7`.
-        calls (int): max number of varying calls to perform. Defaults to `100`.
-        tolerance (float): tolerance for successfull matching. Defaults to `1E-21`.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
+        accelerator (Optional[str]): name of the accelerator, used to determmine knobs if
+            *variables* is not given. Automatic determination will only work for ``LHC`` and
+            ``HLLHC``. Defaults to `None`, in which case the knobs must be provided explicitly
+            through ``varied_knobs``.
+        sequence (str): name of the sequence you want to perform the matching for. Defaults to
+            `None`, in which case the currently active sequence will be used for the matching.
+        dq1_target (float): horizontal chromaticity to match to. Defaults to `None`, in which case
+            it will not be a target and will be excluded from the matching.
+        dq2_target (float): vertical chromaticity to match to. Defaults to `None`, in which case it
+            will not be a target and will be excluded from the matching.
+        varied_knobs (Sequence[str]): the variables names to ``VARY`` in the ``MAD-X`` ``MATCH``
+            routine. An example input could be ``["kqf", "ksd", "kqf", "kqd"]`` as they are common
+            names used for quadrupole and sextupole strengths (focusing / defocusing) in most examples.
+        telescopic_squeeze (bool): ``LHC`` specific. If set to `True`, uses the ``(HL)LHC`` knobs for
+            Telescopic Squeeze configuration. Defaults to `True` since `v0.9.0`.
+        run3 (bool): if set to `True`, uses the ``LHC`` Run 3 `*_op` knobs. Defaults to `False`.
+        step (float): step size to use when varying knobs.
+        calls (int): max number of varying calls to perform. Defaults to 100.
+        tolerance (float): tolerance for successfull matching. Defaults to :math:`10^{-21}`.
 
     Examples:
         Matching a dummy lattice (not LHC or HLLHC):
 
         .. code-block:: python
 
             >>> matching.match_chromaticities(
@@ -294,28 +347,41 @@
             ...     None,              # this is not LHC or HLLHC
             ...     sequence="CAS3",
             ...     dq1_target=100,
             ...     dq2_target=100,
             ...     varied_knobs=["ksf", "ksd"],  # only chroma knobs
             ... )
 
+        Note that since the ``accelerator`` and ``sequence`` arguments default to `None`,
+        they can be omitted. In this case the sequence currently in use will be used for
+        the matching, and ``varied_knobs`` must be provided.
+
+        .. code-block:: python
+
+            >>> matching.match_tunes_and_chromaticities(
+            ...     madx,
+            ...     dq1_target=100,
+            ...     dq2_target=100,
+            ...     varied_knobs=["ksf", "ksd"],  # only chroma knobs
+            ... )
+
         Matching the LHC lattice:
 
         .. code-block:: python
 
             >>> matching.match_chromaticities(
             ...     madx,
             ...     "lhc",                    # will find the knobs automatically
             ...     sequence="lhcb1",
             ...     dq1_target=2.0,
             ...     dq2_target=2.0,
             ... )
     """
     match_tunes_and_chromaticities(
-        madx=madx,
+        madx,
         accelerator=accelerator,
         sequence=sequence,
         q1_target=None,
         q2_target=None,
         dq1_target=dq1_target,
         dq2_target=dq2_target,
         varied_knobs=varied_knobs,
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/parameters.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 from loguru import logger
 
 from pyhdtoolkit.models.madx import MADXBeam
 
 # ----- Utilities ----- #
 
 
-def query_beam_attributes(madx: Madx) -> MADXBeam:
+def query_beam_attributes(madx: Madx, /) -> MADXBeam:
     """
     .. versionadded:: 0.12.0
 
     Returns all ``BEAM`` attributes from the ``MAD-X`` process based on the currently defined
     beam. If no beam has been defined at function call, then ``MAD-X`` will return all the default
     values. See the `MAD-X manual <http://madx.web.cern.ch/madx/releases/last-rel/madxuguide.pdf>`_
     for details.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
 
     Returns:
         A validated `~.models.madx.MADXBeam` object.
 
     Example:
         .. code-block:: python
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/track.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/track.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from loguru import logger
 
 # ----- Utlites ----- #
 
 
 def track_single_particle(
     madx: Madx,
+    /,
     initial_coordinates: Tuple[float, float, float, float, float, float],
     nturns: int,
     sequence: Optional[str] = None,
     observation_points: Sequence[str] = None,
     **kwargs,
 ) -> Dict[str, pd.DataFrame]:
     """
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/tune.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/tune.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 import tfs
 
 from cpymad.madx import Madx
 from loguru import logger
 
 
 def make_footprint_table(
-    madx: Madx, sigma: float = 5, dense: bool = False, file: str = None, cleanup: bool = True, **kwargs
+    madx: Madx, /, sigma: float = 5, dense: bool = False, file: str = None, cleanup: bool = True, **kwargs
 ) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.9.0
 
     Instantiates an ensemble of particles up to the desired bunch :math:`\\sigma` amplitude to be tracked for
     the ``DYNAP`` command, letting ``MAD-X`` infer their tunes. Particules are instantiated for different angle
     variables for each amplitude, creating an ensemble able to represent the tune footprint.
 
     .. warning::
         Since the ``DYNAP`` command makes use of tracking, your sequence needs to be sliced before calling
         this function.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         sigma (float): the maximum amplitude of the tracked particles, in bunch :math:`\\sigma`. Defaults
             to 5.
         dense (bool): if set to `True`, an increased number of particles will be tracked. Defaults to `False`.
         file (str): If given, the ``dynaptune`` table will be exported as a ``TFS`` file with the provided name.
         cleanup (bool): If `True`, the **fort.69** and **lyapunov.data** files are cleared before returning the
             ``dynaptune`` table. Defaults to `True`.
         **kwargs: any keyword argument will be transmitted to the ``DYNAP`` command in ``MAD-X``.
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/twiss.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/twiss.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pyhdtoolkit.cpymadtools.constants import DEFAULT_TWISS_COLUMNS
 
 # ----- Utlites ----- #
 
 
 def get_pattern_twiss(
     madx: Madx,
+    /,
     columns: Sequence[str] = None,
     patterns: Sequence[str] = [""],
     **kwargs,
 ) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.8.0
 
@@ -38,15 +39,15 @@
 
     .. warning::
         Although the *patterns* parameter should accept a regex, ``MAD-X`` does not implement actual regexes.
         Please refer to the `MAD-X manual <http://madx.web.cern.ch/madx/releases/last-rel/madxuguide.pdf>`_,
         section `Regular Expressions` for details on what is implemented in ``MAD-X`` itself.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         columns (Sequence[str]): the variables to be returned, as columns in the `~tfs.frame.TfsDataFrame`.
             Defaults to `None`, which will return all available columns.
         patterns (Sequence[str]): the different element patterns (such as ``MQX`` or ``BPM``) to be applied
             to the ``TWISS`` command, which will determine the rows in the returned `~tfs.frame.TfsDataFrame`.
             Defaults to `[""]` which will select all elements.
         **kwargs: Any keyword argument that can be given to the ``MAD-X`` ``TWISS`` command, such as ``chrom``,
             ``ripken``, ``centre``; or starting coordinates with ``betx``, ``bety`` etc.
@@ -91,25 +92,25 @@
     twiss_df = twiss_df[madx.table.twiss.selected_columns()].iloc[madx.table.twiss.selected_rows()]
 
     logger.trace("Clearing 'TWISS' flag")
     madx.select(flag="twiss", clear=True)
     return twiss_df
 
 
-def get_twiss_tfs(madx: Madx, **kwargs) -> tfs.TfsDataFrame:
+def get_twiss_tfs(madx: Madx, /, **kwargs) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.8.3
 
     Returns a `~tfs.frame.TfsDataFrame` from the `~cpymad.madx.Madx` instance's ``TWISS`` table,
     typically in the way we're used to getting it from ``MAD-X`` outputting the `TWISS` (uppercase
     names, colnames, ``SUMM`` table in headers). This will call the `TWISS` command first before
     returning the dframe to you.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         **kwargs: Any keyword argument that can be given to the ``MAD-X`` ``TWISS`` command, such as ``chrom``,
             ``ripken``, ``centre``; or starting coordinates with ``betx``, ``bety`` etc.    Keyword Args:
 
     Returns:
         A `~tfs.frame.TfsDataFrame` of the ``TWISS`` table.
 
     Example:
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/utils.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,36 @@
 import tfs
 
 from cpymad.madx import Madx
 from loguru import logger
 
 
 def export_madx_table(
-    madx: Madx, table_name: str, file_name: Union[Path, str], pattern: str = None, headers_table: str = "SUMM", **kwargs
+    madx: Madx,
+    /,
+    table_name: str,
+    file_name: Union[Path, str],
+    pattern: str = None,
+    headers_table: str = "SUMM",
+    **kwargs,
 ) -> None:
     """
     .. versionadded:: 0.17.0
 
     Exports an internal table from the ``MAD-X`` process into a `~tfs.frame.TfsDataFrame` on disk.
 
     .. important::
         Tables can only be correctly read back in ``MAD-X`` (through ``READTABLE``) if the written
         file has a ``NAME`` and a ``TYPE`` entries in its headers.
 
         If these entries are not  (see below for their usage), then
         they will be given default values so the **TFS** file can be read by ``MAD-X``.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         table_name (str): the name of the internal table to retrieve.
         file_name (str): the name of the file to export to.
         pattern (str): if given, will be used as a regular expression to filter the extracted
             table, by passing it as the *regex* parameter of `pandas.DataFrame.filter`.
         headers_table (str): the name of the internal table to use for headers.
             Defaults to ``SUMM``.
         **kwargs: any keyword arguments will be passed to `~tfs.writer.write_tfs`.
@@ -59,22 +65,22 @@
     if "TYPE" not in dframe.headers:
         logger.debug(f"No 'TYPE' header found, adding a default value 'EXPORT'")
         dframe.headers["TYPE"] = "EXPORT"
     logger.debug("Writing to disk")
     tfs.write(file_path, dframe, **kwargs)
 
 
-def get_table_tfs(madx: Madx, table_name: str, headers_table: str = "SUMM") -> tfs.TfsDataFrame:
+def get_table_tfs(madx: Madx, /, table_name: str, headers_table: str = "SUMM") -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.11.0
 
     Turns an internal table from the ``MAD-X`` process into a `~tfs.frame.TfsDataFrame`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         table_name (str): the name of the internal table to retrieve.
         headers_table (str): the name of the internal table to use for headers.
             Defaults to ``SUMM``.
 
     Returns:
         A `~tfs.frame.TfsDataFrame` object with the *table_name* data, and the desired
         *headers_table* (usually ``SUMM``) as headers.
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/__init__.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_coupling.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_coupling.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 from loguru import logger
 from optics_functions.coupling import coupling_via_cmatrix
 
 from pyhdtoolkit.cpymadtools import twiss
 from pyhdtoolkit.cpymadtools.constants import MONITOR_TWISS_COLUMNS
 
 
+# This is a duplicate of the function in _routines.py, merge at some point
 def correct_lhc_global_coupling(
-    madx: Madx, beam: int = 1, telescopic_squeeze: bool = True, calls: int = 100, tolerance: float = 1.0e-21
+    madx: Madx, /, beam: int = 1, telescopic_squeeze: bool = True, calls: int = 100, tolerance: float = 1.0e-21
 ) -> None:
     """
     .. versionadded:: 0.20.0
 
     A littly tricky matching routine to perform a decent global coupling correction using
     the ``LHC`` coupling knobs.
 
     .. important::
         This routine makes use of some matching tricks and uses the ``SUMM`` table's
         ``dqmin`` variable for the matching. It should be considered a helpful little
         trick, but it is not a perfect solution.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         beam (int): which beam you want to perform the matching for, should be `1` or
             `2`. Defaults to `1`.
         telescopic_squeeze (bool): If set to `True`, uses the coupling knobs
             for Telescopic Squeeze configuration. Defaults to `True`.
         calls (int): max number of varying calls to perform when matching. Defaults to 100.
         tolerance (float): tolerance for successfull matching. Defaults to :math:`10^{-21}`.
 
@@ -54,23 +55,23 @@
     madx.command.global_(dqmin=0, Q1=62.28)
     madx.command.vary(name=real_knob, step=1.0e-8)
     madx.command.vary(name=imag_knob, step=1.0e-8)
     madx.command.lmdif(calls=calls, tolerance=tolerance)
     madx.command.endmatch()
 
 
-def get_lhc_bpms_twiss_and_rdts(madx: Madx) -> tfs.TfsDataFrame:
+def get_lhc_bpms_twiss_and_rdts(madx: Madx, /) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.19.0
 
     Runs a ``TWISS`` on the currently active sequence for all ``LHC`` BPMs. The coupling RDTs
     are also computed through a CMatrix approach via  `optics_functions.coupling.coupling_via_cmatrix`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
 
     Returns:
         A `~tfs.frame.TfsDataFrame` of the ``TWISS`` table with basic default columns, as well as one
         new column for each of the coupling RDTs. The coupling RDTs are returned as complex numbers.
 
     Example:
         .. code-block:: python
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_elements.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_elements.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,53 +7,77 @@
 """
 from cpymad.madx import Madx
 from loguru import logger
 
 
 def install_ac_dipole_as_kicker(
     madx: Madx,
+    /,
     deltaqx: float,
     deltaqy: float,
     sigma_x: float,
     sigma_y: float,
     beam: int = 1,
     start_turn: int = 100,
     ramp_turns: int = 2000,
     top_turns: int = 6600,
 ) -> None:
     """
     .. versionadded:: 0.15.0
 
-    Installs an AC dipole as a kicker element in (HL)LHC beam 1 or 2, for tracking. This function
-    assumes that you have already defined lhcb1/lhcb2 sequence, made a beam for it (``BEAM``
-    command or `~lhc.make_lhc_beams` function), matched to your desired working point and made
-    a ``TWISS`` call.
+    Installs an AC dipole as a kicker element in (HL)LHC beam 1 or 2, for
+    tracking. This function assumes that you have already defined lhcb1/lhcb2
+    sequence, made a beam for it (``BEAM`` command or `~lhc.make_lhc_beams`
+    function), matched to your desired working point and made a ``TWISS`` call.
 
     .. important::
-        In a real machine, the AC Dipole does impact the orbit as well as the betatron
-        functions when turned on (:cite:t:`Miyamoto:ACD:2008`, part III). In ``MAD-X``
-        however, it cannot be modeled to do both at the same time. This routine introduces
-        an AC Dipole as a kicker element so that its effect can be seen on particle trajectory
+        In a real machine, the AC Dipole does impact the orbit as well as
+        the betatron functions when turned on (:cite:t:`Miyamoto:ACD:2008`,
+        part III). In ``MAD-X`` however, it cannot be modeled to do both at
+        the same time. This routine introduces an AC Dipole as a kicker
+        element so that its effect can be seen on particle trajectory
         in tracking. It **does not** affect ``TWISS`` functions.
 
     One can find a full example use of the function for tracking in the
     :ref:`AC Dipole Tracking <demo-ac-dipole-tracking>` example gallery.
 
+    .. warning::
+        Installing the AC Dipole modifies the sequence, which will then be
+        ``USE``d at the end of this function. This will remove any errors
+        that were installed in the sequence.
+
+        As the errors impact the optics functions which are used during the
+        installation of the AC Dipole, it would not be correct to implement
+        them only after installing the element.
+
+        Therefore, it is recommended to install the errors and save them with
+        the ``ESAVE`` or ``ETABLE`` command, call this function, then
+        re-implement the errors with the ``SETERR`` command.
+
     Args:
         madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
-        deltaqx (float): the deltaQx (horizontal tune excitation) used by the AC dipole.
-        deltaqy (float): the deltaQy (vertical tune excitation) used by the AC dipole.
-        sigma_x (float): the horizontal amplitude to drive the beam to, in bunch sigma.
-        sigma_y (float): the vertical amplitude to drive the beam to, in bunch sigma.
-        beam (int): the LHC beam to install the AC Dipole into, either 1 or 2. Defaults to 1.
-        start_turn (int): the turn at which to start ramping up the AC dipole. Defaults to 100.
-        ramp_turns (int): the number of turns to use for the ramp-up and the ramp-down of the AC dipole.
-            This number is important in order to preserve the adiabaticity of the cycle. Defaults to 2000
-            as in the LHC.
-        top_turns (int): the number of turns to drive the beam for. Defaults to 6600 as in the LHC.
+            Positional only.
+        deltaqx (float): the deltaQx (horizontal tune excitation) used by the
+            AC dipole.
+        deltaqy (float): the deltaQy (vertical tune excitation) used by the
+            AC dipole.
+        sigma_x (float): the horizontal amplitude to drive the beam to, in
+            bunch sigma.
+        sigma_y (float): the vertical amplitude to drive the beam to, in
+            bunch sigma.
+        beam (int): the LHC beam to install the AC Dipole into, either 1 or 2.
+            Defaults to 1.
+        start_turn (int): the turn at which to start ramping up the AC dipole.
+            Defaults to 100.
+        ramp_turns (int): the number of turns to use for the ramp-up and the
+            ramp-down of the AC dipole. This number is important in order to
+            preserve the adiabaticity of the cycle. Defaults to 2000 as in the
+            LHC.
+        top_turns (int): the number of turns to drive the beam for. Defaults
+            to 6600 as in the LHC.
 
     Example:
         .. code-block:: python
 
             >>> install_ac_dipole_as_kicker(
             ...     madx,
             ...     deltaqx=-0.01,  # driven horizontal tune to Qxd = 62.31 - 0.01 = 62.30
@@ -114,37 +138,57 @@
     logger.warning(
         f"Sequence LHCB{beam:d} is now re-USEd for changes to take effect. Beware that this will reset it, "
         "remove errors etc."
     )
     madx.use(sequence=f"lhcb{beam:d}")
 
 
-def install_ac_dipole_as_matrix(madx: Madx, deltaqx: float, deltaqy: float, beam: int = 1) -> None:
+def install_ac_dipole_as_matrix(madx: Madx, /, deltaqx: float, deltaqy: float, beam: int = 1) -> None:
     """
     .. versionadded:: 0.15.0
 
-    Installs an AC dipole as a matrix element in (HL)LHC beam 1 or 2, to see its effect on TWISS functions
-    This function assumes that you have already defined lhcb1/lhcb2 sequence, made a beam for it (``BEAM``
-    command or `~lhc.make_lhc_beams` function), matched to your desired working point and made a ``TWISS``
-    call.
+    Installs an AC dipole as a matrix element in (HL)LHC beam 1 or 2, to
+    see its effect on TWISS functions This function assumes that you have
+    already defined lhcb1/lhcb2 sequence, made a beam for it (``BEAM``
+    command or `~lhc.make_lhc_beams` function), matched to your desired
+    working point and made a ``TWISS`` call.
 
-    This function's use is very similar to that of `~.lhc.install_ac_dipole_as_kicker`.
+    This function's use is very similar to that of
+    `~.lhc.install_ac_dipole_as_kicker`.
 
     .. important::
-        In a real machine, the AC Dipole does impact the orbit as well as the betatron
-        functions when turned on (:cite:t:`Miyamoto:ACD:2008`, part III). In ``MAD-X``
-        however, it cannot be modeled to do both at the same time. This routine introduces
-        an AC Dipole as a matrix element so that its effect can be seen on ``TWISS`` functions.
-        It **does not** affect tracking.
+        In a real machine, the AC Dipole does impact the orbit as well as the
+        betatron functions when turned on (:cite:t:`Miyamoto:ACD:2008`, part
+        III). In ``MAD-X`` however, it cannot be modeled to do both at the
+        same time. This routine introduces an AC Dipole as a matrix element
+        so that its effect can be seen on ``TWISS`` functions. It **does not**
+        affect tracking.
+
+    .. warning::
+        Installing the AC Dipole modifies the sequence, which will then be
+        ``USE``d at the end of this function. This will remove any errors
+        that were installed in the sequence.
+
+        As the errors impact the optics functions which are used during the
+        installation of the AC Dipole, it would not be correct to implement
+        them only after installing the element.
+
+        Therefore, it is recommended to install the errors and save them with
+        the ``ESAVE`` or ``ETABLE`` command, call this function, then
+        re-implement the errors with the ``SETERR`` command.
 
     Args:
         madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
-        deltaqx (float): the deltaQx (horizontal tune excitation) used by the AC dipole.
-        deltaqy (float): the deltaQy (vertical tune excitation) used by the AC dipole.
-        beam (int): the LHC beam to install the AC Dipole into, either 1 or 2. Defaults to 1.
+            Positional only.
+        deltaqx (float): the deltaQx (horizontal tune excitation) used by the
+            AC dipole.
+        deltaqy (float): the deltaQy (vertical tune excitation) used by the
+            AC dipole.
+        beam (int): the LHC beam to install the AC Dipole into, either 1 or 2.
+            Defaults to 1.
 
     Example:
         .. code-block:: python
 
             >>> install_ac_dipole_as_matrix(madx, deltaqx=-0.01, deltaqy=0.012, beam=1)
     """
     logger.warning("This AC Dipole is implemented as a matrix and will not affect particle tracking!")
@@ -179,38 +223,47 @@
     logger.warning(
         f"Sequence LHCB{beam:d} is now re-USEd for changes to take effect. Beware that this will reset it, "
         "remove errors etc."
     )
     madx.use(sequence=f"lhcb{beam:d}")
 
 
-def add_markers_around_lhc_ip(madx: Madx, sequence: str, ip: int, n_markers: int, interval: float) -> None:
+def add_markers_around_lhc_ip(madx: Madx, /, sequence: str, ip: int, n_markers: int, interval: float) -> None:
     """
     .. versionadded:: 1.0.0
 
-    Adds some simple marker elements left and right of an IP point, to increase the granularity of optics
-    functions returned from a ``TWISS`` call.
+    Adds some simple marker elements left and right of an IP point, to
+    increase the granularity of optics functions returned from a ``TWISS``
+    call.
 
     .. warning::
-        You will most likely need to have sliced the sequence before calling this function,
-        as otherwise there is a risk on getting a negative drift depending on the affected
-        IP. This would lead to the remote ``MAD-X`` process to crash.
+        You will most likely need to have sliced the sequence before calling
+        this function, as otherwise there is a risk on getting a negative
+        drift depending on the affected IP. This would lead to the remote
+        ``MAD-X`` process to crash.
 
     .. warning::
-        After editing the *sequence* to add markers, the ``USE`` command will be run for the changes to apply.
-        This means the caveats of ``USE`` apply, for instance the erasing of previously defined errors, orbits
+        After editing the *sequence* to add markers, the ``USE`` command will
+        be run for the changes to apply. This means the caveats of ``USE``
+        apply, for instance the erasing of previously defined errors, orbits
         corrections etc.
+        
+        Therefore, it is recommended to install the errors and save them with
+        the ``ESAVE`` or ``ETABLE`` command, call this function, then
+        re-implement the errors with the ``SETERR`` command.
 
     Args:
         madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+            Positional only.
         sequence (str): which sequence to use the routine on.
         ip (int): The interaction point around which to add markers.
         n_markers (int): how many markers to add on each side of the IP.
-        interval (float): the distance between markers, in [m]. Giving ``interval=0.05`` will
-            place a marker every 5cm (starting 5cm away from the IP on each side).
+        interval (float): the distance between markers, in [m]. Giving
+            ``interval=0.05`` will place a marker every 5cm (starting 5cm
+            away from the IP on each side).
 
     Example:
         .. code-block:: python
 
             >>> add_markers_around_lhc_ip(
             ...     madx, sequence=f"lhcb1", ip=1, n_markers=1000, interval=0.001
             ... )
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_errors.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     8: ["^MQML.8{side}{ip:d}.B{beam:d}"],  # Q8 LHC & HL-LHC
     9: ["^MQM.9{side}{ip:d}.B{beam:d}", "^MQMC.9{side}{ip:d}.B{beam:d}"],  # Q9 3.4m then 2.4m LHC & HL-LHC
     10: ["^MQML.10{side}{ip:d}.B{beam:d}"],  # Q10 4.8m LHC & HL-LHC
 }
 
 
 def misalign_lhc_triplets(
-    madx: Madx, ip: int, sides: Sequence[str] = ("r", "l"), table: str = "triplet_errors", **kwargs
+    madx: Madx, /, ip: int, sides: Sequence[str] = ("r", "l"), table: str = "triplet_errors", **kwargs
 ) -> None:
     """
     .. versionadded:: 0.9.0
 
     Apply misalignment errors to IR triplet quadrupoles on a given side of a given IP. In case of a
     sliced lattice, this will misalign all slices of each magnet together. This is a convenience wrapper
     around the `~.misalign_lhc_ir_quadrupoles` function, see that function's docstring for more
     information.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         ip (int): the interaction point around which to apply errors.
         sides (Sequence[str]): sides of the IP to apply error on the triplets, either L or R or both.
             Case-insensitive. Defaults to both.
         table (str): the name of the internal table that will save the assigned errors. Defaults to
             `triplet_errors`.
         **kwargs: Any keyword argument is given to the ``EALIGN`` command, including the error to apply
             (`DX`, `DY`, `DPSI` etc) as a string, like it would be given directly into ``MAD-X``.
@@ -60,14 +60,15 @@
             >>> misalign_lhc_triplets(madx, ip=5, sides="RL", dpsi="0.001 * TGAUSS(2.5)")
     """
     misalign_lhc_ir_quadrupoles(madx, ips=[ip], beam=None, quadrupoles=(1, 2, 3), sides=sides, table=table, **kwargs)
 
 
 def misalign_lhc_ir_quadrupoles(
     madx: Madx,
+    /,
     ips: Sequence[int],
     beam: int,
     quadrupoles: Sequence[int],
     sides: Sequence[str] = ("r", "l"),
     table: str = "ir_quads_errors",
     **kwargs,
 ) -> None:
@@ -88,15 +89,15 @@
 
     .. warning::
         One should avoid issuing different errors with several uses of this command as it is unclear to me
         how ``MAD-X`` chooses to handle this internally. Instead, it is advised to give all errors in the same
         command, which is guaranteed to work. See the last provided example below.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         ips (Sequence[int]): the interaction point(s) around which to apply errors.
         beam (int): beam number to apply the errors to. Unlike triplet quadrupoles which are single
             aperture, Q4 to Q10 are not and will need this information.
         quadrupoles (Sequence[int]): the number of the quadrupoles to apply errors to.
         sides (Sequence[str]): sides of the IP to apply error on the triplets, either L or R or both.
             Case-insensitive. Defaults to both.
         table (str): the name of the internal table that will save the assigned errors. Defaults to
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_misc.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,23 @@
     LHC_IP2_SPECIAL_FLAG,
     LHC_IP_OFFSET_FLAGS,
     LHC_PARALLEL_SEPARATION_FLAGS,
 )
 from pyhdtoolkit.optics.ripken import _add_beam_size_to_df
 
 
-def make_sixtrack_output(madx: Madx, energy: int) -> None:
+def make_sixtrack_output(madx: Madx, /, energy: int) -> None:
     """
     .. versionadded:: 0.15.0
 
     Prepare output for a ``SixTrack`` run. Initial implementation credits go to
     :user:`Joschua Dilly <joschd>`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         energy (float): beam energy, in [GeV].
 
     Example:
         .. code-block:: python
 
             >>> make_sixtrack_output(madx, energy=6800)
     """
@@ -46,22 +46,22 @@
     madx.globals["LAGRF400.B2"] = 0.0
 
     logger.debug("Executing TWISS and SIXTRACK commands")
     madx.twiss()  # used by sixtrack
     madx.sixtrack(cavall=True, radius=0.017)  # this value is only ok for HL(LHC) magnet radius
 
 
-def reset_lhc_bump_flags(madx: Madx) -> None:
+def reset_lhc_bump_flags(madx: Madx, /) -> None:
     """
     .. versionadded:: 0.15.0
 
     Resets all LHC IP bump flags to 0.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
 
     Example:
         .. code-block:: python
 
             >>> reset_lhc_bump_flags(madx)
     """
     logger.debug("Resetting all LHC IP bump flags")
@@ -138,15 +138,15 @@
             f"kqtd.b{beam}{suffix}",
             f"ksf.b{beam}{suffix}",
             f"ksd.b{beam}{suffix}",
         ),
     }[accelerator.upper()]
 
 
-def get_lhc_bpms_list(madx: Madx) -> List[str]:
+def get_lhc_bpms_list(madx: Madx, /) -> List[str]:
     """
     .. versionadded:: 0.16.0
 
     Returns the list of monitoring BPMs for the current LHC sequence in use.
     The BPMs are queried through a regex in the result of a ``TWISS`` command.
 
     .. note::
@@ -165,22 +165,24 @@
             >>> observation_bpms = get_lhc_bpms_list(madx)
     """
     twiss_df = twiss.get_twiss_tfs(madx).reset_index()
     bpms_df = twiss_df[twiss_df.NAME.str.contains("^bpm.*B[12]$", case=False, regex=True)]
     return bpms_df.NAME.tolist()
 
 
-def get_sizes_at_ip(madx: Madx, ip: int, geom_emit_x: float = None, geom_emit_y: float = None) -> Tuple[float, float]:
+def get_sizes_at_ip(
+    madx: Madx, /, ip: int, geom_emit_x: float = None, geom_emit_y: float = None
+) -> Tuple[float, float]:
     """
     .. versionadded:: 1.0.0
 
     Get the Lebedev beam sizes (horizontal and vertical) at the provided LHC *ip*.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         ip (int): the IP to get the sizes at.
         geom_emit_x (float): the horizontal geometrical emittance to use for the
             calculation. If not provided, will look for the values of the
             ``geometric_emit_x`` variable in ``MAD-X``.
         geom_emit_y (float): the vertical geometrical emittance to use for the
             calculation. If not provided, will look for the values of the
             ``geometric_emit_y`` variable in ``MAD-X``.
@@ -189,14 +191,14 @@
         A tuple of the horizontal and vertical beam sizes at the provided *IP*.
 
     Example:
         .. code-block:: python
 
             >>> ip5_x, ip5_y = get_size_at_ip(madx, ip=5)
     """
-    logger.debug(f"Getting horizotnal and vertical sizes at IP{ip:d} through Ripken parameters")
+    logger.debug(f"Getting horizontal and vertical sizes at IP{ip:d} through Ripken parameters")
     geom_emit_x = geom_emit_x or madx.globals["geometric_emit_x"]
     geom_emit_y = geom_emit_y or madx.globals["geometric_emit_y"]
 
     twiss_tfs = twiss.get_twiss_tfs(madx, ripken=True)
     twiss_tfs = _add_beam_size_to_df(twiss_tfs, geom_emit_x, geom_emit_y)
     return twiss_tfs.loc[f"IP{ip:d}"].SIZE_X, twiss_tfs.loc[f"IP{ip:d}"].SIZE_Y
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_powering.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_powering.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 """
 from typing import Dict, List, Sequence
 
 from cpymad.madx import Madx
 from loguru import logger
 
 
-def apply_lhc_colinearity_knob(madx: Madx, colinearity_knob_value: float = 0, ir: int = None) -> None:
+def apply_lhc_colinearity_knob(madx: Madx, /, colinearity_knob_value: float = 0, ir: int = None) -> None:
     """
     .. versionadded:: 0.15.0
 
     Applies the a trim of the LHC colinearity knob.
 
     .. note::
         If you don't know what this is, you really should not be using this function.
 
     .. tip::
         The convention, which is also the one I implemented in ``LSA`` for the ``LHC``, is that a
         positive value of the colinearity knob results in a powering increase of the ``MQSX`` *right*
         of the IP, and a powering decrease of the ``MQSX`` *left* of the IP.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         colinearity_knob_value (float): Units of the colinearity knob to apply. Defaults to 0 so users
             don't mess up local IR coupling by mistake. This should be a positive integer, normally between 1
             and 10.
         ir (int): The Interaction Region to apply the knob to, should be one of [1, 2, 5, 8].
             Classically 1 or 5.
 
     Example:
@@ -45,26 +45,26 @@
 
     madx.globals[right_knob] = colinearity_knob_value * 1e-4
     logger.debug(f"Set '{right_knob}' to {madx.globals[right_knob]}")
     madx.globals[left_knob] = -1 * colinearity_knob_value * 1e-4
     logger.debug(f"Set '{left_knob}' to {madx.globals[left_knob]}")
 
 
-def apply_lhc_colinearity_knob_delta(madx: Madx, colinearity_knob_delta: float = 0, ir: int = None) -> None:
+def apply_lhc_colinearity_knob_delta(madx: Madx, /, colinearity_knob_delta: float = 0, ir: int = None) -> None:
     """
     .. versionadded:: 0.21.0
 
     This is essentially the same as `.apply_lhc_colinearity_knob`, but instead of a applying fixed powering
     value, it applies a delta to the (potentially) existing value.
 
     .. note::
         If you don't know what this is, you really should not be using this function.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         colinearity_knob_delta (float): Units of the colinearity knob to vary the existing powerings with.
             Defaults to 0.
         ir (int): The Interaction Region to apply the knob to, should be one of [1, 2, 5, 8].
             Classically 1 or 5.
 
     Example:
         .. code-block:: python
@@ -85,15 +85,15 @@
     madx.globals[right_knob] = current_right + colinearity_knob_delta * 1e-4
     logger.debug(f"Set '{right_knob}' to {madx.globals[right_knob]}")
     madx.globals[left_knob] = current_left - colinearity_knob_delta * 1e-4
     logger.debug(f"Set '{left_knob}' to {madx.globals[left_knob]}")
 
 
 def apply_lhc_rigidity_waist_shift_knob(
-    madx: Madx, rigidty_waist_shift_value: float = 0, ir: int = None, side: str = "left"
+    madx: Madx, /, rigidty_waist_shift_value: float = 0, ir: int = None, side: str = "left"
 ) -> None:
     """
     .. versionadded:: 0.15.0
 
     Applies a trim of the LHC rigidity waist shift knob, moving the waist left or right of IP.
     The waist shift is achieved by moving all four betatron waists simltaneously: unbalancing
     the triplet powering knobs of the left and right-hand sides of the IP.
@@ -105,15 +105,15 @@
         Applying the shift will modify your tunes and is likely to flip them, making a subsequent matching
         impossible if your lattice has coupling. To avoid this, one should match to tunes split further apart
         before applying the waist shift knob, and then match to the desired working point. For instance for
         the LHC, matching to (62.27, 60.36) before applying and afterwards rematching to (62.31, 60.32) usually
         works well.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         rigidty_waist_shift_value (float): Units of the rigidity waist shift knob (positive values only).
         ir (int): The Interaction Region to apply the knob to, should be one of [1, 2, 5, 8].
             Classically 1 or 5.
         side (str): Which side of the IP to move the waist to, determines a sign in the calculation.
             Defaults to `left`, which means :math:`s_{\\mathrm{waist}} \\lt s_{\\mathrm{ip}}` (and
             setting it to `right` would move the waist such that
             :math:`s_{\\mathrm{waist}} \\gt s_{\\mathrm{ip}}`).
@@ -144,23 +144,23 @@
         raise ValueError("Invalid value for parameter 'side'.")
 
     logger.debug(f"Set '{right_knob}' to {madx.globals[right_knob]}")
     logger.debug(f"Set '{left_knob}' to {madx.globals[left_knob]}")
 
 
 def apply_lhc_coupling_knob(
-    madx: Madx, coupling_knob: float = 0, beam: int = 1, telescopic_squeeze: bool = True
+    madx: Madx, /, coupling_knob: float = 0, beam: int = 1, telescopic_squeeze: bool = True
 ) -> None:
     """
     .. versionadded:: 0.15.0
 
     Applies a trim of the LHC coupling knob to reach the desired :math:`|C^{-}|` value.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         coupling_knob (float): Desired value for the Cminus, typically a few units of ``1E-3``.
             Defaults to 0 so users don't mess up coupling by mistake.
         beam (int): beam to apply the knob to. Defaults to beam 1.
         telescopic_squeeze (bool): if set to `True`, uses the knobs for Telescopic Squeeze configuration.
             Defaults to `True` since `v0.9.0`.
 
     Example:
@@ -177,23 +177,23 @@
     knob_name = f"CMRS.b{beam:d}{suffix}"
 
     logger.debug(f"Knob '{knob_name}' is {madx.globals[knob_name]} before implementation")
     madx.globals[knob_name] = coupling_knob
     logger.debug(f"Set '{knob_name}' to {madx.globals[knob_name]}")
 
 
-def carry_colinearity_knob_over(madx: Madx, ir: int, to_left: bool = True) -> None:
+def carry_colinearity_knob_over(madx: Madx, /, ir: int, to_left: bool = True) -> None:
     """
     .. versionadded:: 0.20.0
 
     Removes the powering setting on one side of the colinearty knob and applies it to the
     other side.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         ir (int): The Interaction Region around which to apply the change, should be
             one of [1, 2, 5, 8].
         to_left (bool): If `True`, the magnet right of IP is de-powered of and its powering
             is transferred to the magnet left of IP. If `False`, then the opposite happens.
             Defaults to `True`.
 
     Example:
@@ -212,22 +212,22 @@
     new_right = 0 if to_left else left_powering + right_powering
     logger.debug(f"New powering values are: '{left_variable}'={new_left} | '{right_variable}'={new_right}")
     madx.globals[left_variable] = new_left
     madx.globals[right_variable] = new_right
     logger.debug("New powerings applied")
 
 
-def power_landau_octupoles(madx: Madx, beam: int, mo_current: float, defective_arc: bool = False) -> None:
+def power_landau_octupoles(madx: Madx, /, beam: int, mo_current: float, defective_arc: bool = False) -> None:
     """
     .. versionadded:: 0.15.0
 
     Powers the Landau octupoles in the (HL)LHC.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         beam (int): beam to use.
         mo_current (float): `MO` powering, in [A].
         defective_arc: If set to `True`, the ``KOD`` in Arc 56 are powered for less ``Imax``.
 
     Example:
         .. code-block:: python
 
@@ -249,22 +249,22 @@
             logger.debug(f"Powering element '{octupole}' at {strength} Amps")
             madx.globals[octupole] = strength
 
     if defective_arc and (beam == 1):
         madx.globals["KOD.A56B1"] = strength * 4.65 / 6  # defective MO group
 
 
-def deactivate_lhc_arc_sextupoles(madx: Madx, beam: int) -> None:
+def deactivate_lhc_arc_sextupoles(madx: Madx, /, beam: int) -> None:
     """
     .. versionadded:: 0.15.0
 
     Deactivates all arc sextupoles in the (HL)LHC.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         beam (int): beam to use.
 
     Example:
         .. code-block:: python
 
             >>> deactivate_lhc_arc_sextupoles(madx, beam=1)
     """
@@ -279,29 +279,29 @@
             for i in (1, 2):
                 sextupole = f"KS{fd}{i:d}.{arc}"
                 logger.debug(f"De-powering element '{sextupole}'")
                 madx.globals[sextupole] = 0.0
 
 
 def vary_independent_ir_quadrupoles(
-    madx: Madx, quad_numbers: Sequence[int], ip: int, sides: Sequence[str] = ("r", "l"), beam: int = 1
+    madx: Madx, /, quad_numbers: Sequence[int], ip: int, sides: Sequence[str] = ("r", "l"), beam: int = 1
 ) -> None:
     """
     .. versionadded:: 0.15.0
 
     Sends the ``VARY`` commands for the desired quadrupoles in the IR surrounding the provided *ip*.
     The independent quadrupoles for which this is implemented are Q4 to Q13 included. This is useful
     to setup some specific matching involving these elements.
 
     .. important::
         It is necessary to have defined a ``brho`` variable when creating your beams. If one has used
         `make_lhc_beams` to create the beams, this has already been done automatically.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         quad_numbers (Sequence[int]): quadrupoles to be varied, by number (aka position from IP).
         ip (int): the IP around which to apply the instructions.
         sides (Sequence[str]): the sides of IP to act on. Should be `R` for right and `L` for left,
             accepts these letters case-insensitively. Defaults to both sides of the IP.
         beam (int): the beam for which to apply the instructions. Defaults to 1.
 
     Example:
@@ -341,23 +341,23 @@
                 name=f"kq{'t' if quad >= 11 else ''}{'l' if quad == 11 else ''}{quad}.{side}{ip}b{beam}",
                 step=1e-7,
                 lower=f"-{circuit}.{'b' if quad == 7 else ''}{quad}{side}{ip}.b{beam}->kmax/brho",
                 upper=f"+{circuit}.{'b' if quad == 7 else ''}{quad}{side}{ip}.b{beam}->kmax/brho",
             )
 
 
-def switch_magnetic_errors(madx: Madx, **kwargs) -> None:
+def switch_magnetic_errors(madx: Madx, /, **kwargs) -> None:
     """
     .. versionadded:: 0.7.0
 
     Applies magnetic field orders. This will only work for LHC and HLLHC machines.
     Initial implementation credits go to :user:`Joschua Dilly <joschd>`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         **kwargs: The setting works through keyword arguments, and several specific
             kwargs are expected. `default` sets global default to this value (defaults to `False`).
             `AB#` sets the default for all of that order, the order being the `#` number. `A#` or
             `B#` sets the default for systematic and random of this id. `A#s`, `B#r`, etc. sets the
             specific value for this given order. In all kwargs, the order # should be in the range
             [1...15], where 1 == dipolar field.
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_queries.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     LHC_KSS_KNOBS,
 )
 from pyhdtoolkit.cpymadtools.lhc._setup import lhc_orbit_variables
 from pyhdtoolkit.cpymadtools.utils import _get_k_strings
 
 
 def get_magnets_powering(
-    madx: Madx, patterns: Sequence[str] = [r"^mb\.", r"^mq\.", r"^ms\."], brho: Union[str, float] = None, **kwargs
+    madx: Madx, /, patterns: Sequence[str] = [r"^mb\.", r"^mq\.", r"^ms\."], brho: Union[str, float] = None, **kwargs
 ) -> tfs.TfsDataFrame:
     r"""
     .. versionadded:: 0.17.0
 
     Gets the twiss table with additional defined columns for the given *patterns*.
 
     .. note::
@@ -58,15 +58,15 @@
         the results for *all* elements. One can also give a specific magnet's exact
         name to include it in the results.
 
     .. note::
         The ``TWISS`` flag will be fully cleared after running this function.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         patterns (Sequence[str]): a list of regex patterns to define which elements
             should be selected and included in the returned table. Defaults to selecting
             the main bends, quads and sextupoles. See the note admonition above for
             useful patterns to select specific ``LHC`` magnet families.
         brho (Union[str, float]): optional, an explicit definition for the magnetic
             rigidity in :math:`Tm^{-1}`. If not given, it will be assumed that
             a ``brho`` quantity is defined in the ``MAD-X`` globals.
@@ -85,15 +85,15 @@
     logger.debug("Computing magnets field and powering limits proportions")
     NEW_COLNAMES = ["name", "keyword", "ampere", "imax", "percent", "kn", "kmax", "integrated_field", "L"]
     NEW_COLNAMES = list(set(NEW_COLNAMES + kwargs.pop("columns", [])))  # in case user gives explicit columns
     _list_field_currents(madx, brho=brho)
     return twiss.get_pattern_twiss(madx, columns=NEW_COLNAMES, patterns=patterns, **kwargs)
 
 
-def query_arc_correctors_powering(madx: Madx) -> Dict[str, float]:
+def query_arc_correctors_powering(madx: Madx, /) -> Dict[str, float]:
     """
     .. versionadded:: 0.15.0
 
     Queries for the arc corrector strengths and returns their values as a percentage of
     their max powering. This is a port of one of the **corr_value.madx** file's macros
 
     Args:
@@ -116,40 +116,40 @@
     result.update({knob: 100 * _knob_value(madx, knob) / k_mqt_max for knob in LHC_KQTF_KNOBS})
 
     logger.debug("Querying arc short straight sections skew quadrupole correctors (MQSs) powering")
     k_mqs_max = 120 / madx.globals.brho  # 120 T/m
     result.update({knob: 100 * _knob_value(madx, knob) / k_mqs_max for knob in LHC_KQS_KNOBS})
 
     logger.debug("Querying arc sextupole correctors (MSs) powering")
-    k_ms_max = 1.280 * 2 / 0.017 ** 2 / madx.globals.brho  # 1.28 T @ 17 mm
+    k_ms_max = 1.280 * 2 / 0.017**2 / madx.globals.brho  # 1.28 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_ms_max for knob in LHC_KSF_KNOBS})
 
     logger.debug("Querying arc skew sextupole correctors (MSSs) powering")
-    k_mss_max = 1.280 * 2 / 0.017 ** 2 / madx.globals.brho  # 1.28 T @ 17 mm
+    k_mss_max = 1.280 * 2 / 0.017**2 / madx.globals.brho  # 1.28 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mss_max for knob in LHC_KSS_KNOBS})
 
     logger.debug("Querying arc spool piece (skew) sextupole correctors (MCSs) powering")
-    k_mcs_max = 0.471 * 2 / 0.017 ** 2 / madx.globals.brho  # 0.471 T @ 17 mm
+    k_mcs_max = 0.471 * 2 / 0.017**2 / madx.globals.brho  # 0.471 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mcs_max for knob in LHC_KCS_KNOBS})
 
     logger.debug("Querying arc spool piece (skew) octupole correctors (MCOs) powering")
-    k_mco_max = 0.040 * 6 / 0.017 ** 3 / madx.globals.brho  # 0.04 T @ 17 mm
+    k_mco_max = 0.040 * 6 / 0.017**3 / madx.globals.brho  # 0.04 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mco_max for knob in LHC_KCO_KNOBS})
 
     logger.debug("Querying arc spool piece (skew) decapole correctors (MCDs) powering")
-    k_mcd_max = 0.100 * 24 / 0.017 ** 4 / madx.globals.brho  # 0.1 T @ 17 mm
+    k_mcd_max = 0.100 * 24 / 0.017**4 / madx.globals.brho  # 0.1 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mcd_max for knob in LHC_KCD_KNOBS})
 
     logger.debug("Querying arc short straight sections octupole correctors (MOs) powering")
-    k_mo_max = 0.29 * 6 / 0.017 ** 3 / madx.globals.brho  # 0.29 T @ 17 mm
+    k_mo_max = 0.29 * 6 / 0.017**3 / madx.globals.brho  # 0.29 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mo_max for knob in LHC_KO_KNOBS})
     return result
 
 
-def query_triplet_correctors_powering(madx: Madx) -> Dict[str, float]:
+def query_triplet_correctors_powering(madx: Madx, /) -> Dict[str, float]:
     """
     .. versionadded:: 0.15.0
 
     Queries for the triplet corrector strengths and returns their values as a percentage of
     their max powering. This is a port of one of the **corr_value.madx** file's macros.
 
     Args:
@@ -168,44 +168,44 @@
     result: Dict[str, float] = {}
 
     logger.debug("Querying triplet skew quadrupole correctors (MQSXs) powering")
     k_mqsx_max = 1.360 / 0.017 / madx.globals.brho  # 1.36 T @ 17mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mqsx_max for knob in LHC_KQSX_KNOBS})
 
     logger.debug("Querying triplet sextupole correctors (MCSXs) powering")
-    k_mcsx_max = 0.028 * 2 / 0.017 ** 2 / madx.globals.brho  # 0.028 T @ 17 mm
+    k_mcsx_max = 0.028 * 2 / 0.017**2 / madx.globals.brho  # 0.028 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mcsx_max for knob in LHC_KCSX_KNOBS})
 
     logger.debug("Querying triplet skew sextupole correctors (MCSSXs) powering")
-    k_mcssx_max = 0.11 * 2 / 0.017 ** 2 / madx.globals.brho  # 0.11 T @ 17 mm
+    k_mcssx_max = 0.11 * 2 / 0.017**2 / madx.globals.brho  # 0.11 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mcssx_max for knob in LHC_KCSSX_KNOBS})
 
     logger.debug("Querying triplet octupole correctors (MCOXs) powering")
-    k_mcox_max = 0.045 * 6 / 0.017 ** 3 / madx.globals.brho  # 0.045 T @ 17 mm
+    k_mcox_max = 0.045 * 6 / 0.017**3 / madx.globals.brho  # 0.045 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mcox_max for knob in LHC_KCOX_KNOBS})
 
     logger.debug("Querying triplet skew octupole correctors (MCOSXs) powering")
-    k_mcosx_max = 0.048 * 6 / 0.017 ** 3 / madx.globals.brho  # 0.048 T @ 17 mm
+    k_mcosx_max = 0.048 * 6 / 0.017**3 / madx.globals.brho  # 0.048 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mcosx_max for knob in LHC_KCOSX_KNOBS})
 
     logger.debug("Querying triplet decapole correctors (MCTXs) powering")
-    k_mctx_max = 0.01 * 120 / 0.017 ** 5 / madx.globals.brho  # 0.010 T @ 17 mm
+    k_mctx_max = 0.01 * 120 / 0.017**5 / madx.globals.brho  # 0.010 T @ 17 mm
     result.update({knob: 100 * _knob_value(madx, knob) / k_mctx_max for knob in LHC_KCTX_KNOBS})
     return result
 
 
-def get_current_orbit_setup(madx: Madx) -> Dict[str, float]:
+def get_current_orbit_setup(madx: Madx, /) -> Dict[str, float]:
     """
     .. versionadded:: 0.8.0
 
     Get the current values for the (HL)LHC orbit variables. Initial implementation credits go to
     :user:`Joschua Dilly <joschd>`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
 
     Returns:
         A `dict` of all orbit variables set, and their values as set in the ``MAD-X`` globals.
 
     Example:
         .. code-block:: python
 
@@ -215,29 +215,29 @@
     variables, specials = lhc_orbit_variables()
     return {orbit_variable: madx.globals[orbit_variable] for orbit_variable in variables + list(specials.keys())}
 
 
 # ----- Helpers ----- #
 
 
-def _list_field_currents(madx: Madx, brho: Union[str, float] = None) -> None:
+def _list_field_currents(madx: Madx, /, brho: Union[str, float] = None) -> None:
     """
     Creates additional columns for the ``TWISS`` table with the magnets' total fields
     and currents, to help later on determine which proportion of their maximum powering
     the current setting is using. This is an implementation of the old utility script
     located at **/afs/cern.ch/eng/lhc/optics/V6.503/toolkit/list_fields_currents.madx**.
 
     .. important::
         Certain quantities are assumed to be defined in the ``MAD-X`` globals, such as
         ``brho``, or available in the magnets definition, such as ``calib``. For this
         reason, this script most likely only works for the ``(HL)LHC`` sequences where
         those are defined.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         brho (Union[str, float]): optional, an explicit definition for the magnetic
             rigidity in :math:`Tm^{-1}`. If not given, it will be assumed that
             a ``brho`` quantity is defined in the ``MAD-X`` globals and this one will
             be used.
     """
     logger.debug("Creating additional TWISS table columns for magnets' fields and currents")
 
@@ -262,21 +262,21 @@
     madx.globals["field"] = "kn * brho"
     madx.globals["percent"] = "field * 100 / (kmaxx + epsilon)"
     madx.globals["ampere"] = "field / calibration"
     madx.globals["imax"] = "kmaxx / calibration"
     madx.globals["integrated_field"] = "field * length"
 
 
-def _knob_value(madx: Madx, knob: str) -> float:
+def _knob_value(madx: Madx, /, knob: str) -> float:
     """
     Queryies the current value of a given *knob* name in the ``MAD-X`` process, and defaults
     to 0 (as ``MAD-X`` does) in case that knob has not been defined in the current process.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         knob (str): the name the knob.
 
     Returns:
         The knob value if it was defined, otherwise 0.
 
     Example:
         .. code-block:: python
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_routines.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_routines.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from cpymad.madx import Madx
 from loguru import logger
 
 from pyhdtoolkit.cpymadtools.lhc._twiss import get_ir_twiss
 
 
 def do_kmodulation(
-    madx: Madx, ir: int = 1, side: str = "right", steps: int = 100, stepsize: float = 3e-8, **kwargs
+    madx: Madx, /, ir: int = 1, side: str = "right", steps: int = 100, stepsize: float = 3e-8, **kwargs
 ) -> tfs.TfsDataFrame:
     r"""
     .. versionadded:: 0.20.0
 
     Simulates a K-Modulation measurement by varying the powering of Q1 left or
     right of the IP, and returning the tune variations resulting from this
     modulation.
@@ -31,15 +31,15 @@
 
     .. tip::
         From these, one can then calculate the :math:`\beta`-functions at the Q1
         and then at the IP, plus the possible waist shift, according to
         :cite:t:`Carlier:AccuracyFeasibilityMeasurement2017`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         ir (int): the IR in which to perform the modulation. Defaults to 1.
         side (str): which side of the IP to use the Q1 to perform the modulation.
             Should be either ``right`` or ``left``, case-insensitive. Defaults to
             ``right``.
         steps (int): the number of steps to perform in the modulations, aka the number
             of "measurements". Defaults to 100.
         stepsize (float): the increment in powering for Q1, in direct values of the
@@ -91,30 +91,31 @@
 
     results.index.name = powering_variable
     results.ERRTUNEX = 0  # No measurement error from MAD-X
     results.ERRTUNEY = 0  # No measurement error from MAD-X
     return results
 
 
+# This is a duplicate of the function in _coupling.py, merge at some point
 def correct_lhc_global_coupling(
-    madx: Madx, beam: int = 1, telescopic_squeeze: bool = True, calls: int = 100, tolerance: float = 1.0e-21
+    madx: Madx, /, beam: int = 1, telescopic_squeeze: bool = True, calls: int = 100, tolerance: float = 1.0e-21
 ) -> None:
     """
     .. versionadded:: 0.20.0
 
     A littly tricky matching routine to perform a decent global coupling correction using
     the ``LHC`` coupling knobs.
 
     .. important::
         This routine makes use of some matching tricks and uses the ``SUMM`` table's
         ``dqmin`` variable for the matching. It should be considered a helpful little
         trick, but it is not a perfect solution.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         beam (int): which beam you want to perform the matching for, should be `1` or
             `2`. Defaults to `1`.
         telescopic_squeeze (bool): If set to `True`, uses the coupling knobs
             for Telescopic Squeeze configuration. Defaults to `True`.
         calls (int): max number of varying calls to perform when matching. Defaults to 100.
         tolerance (float): tolerance for successfull matching. Defaults to :math:`10^{-21}`.
 
@@ -136,14 +137,15 @@
     madx.command.vary(name=imag_knob, step=1.0e-8)
     madx.command.lmdif(calls=calls, tolerance=tolerance)
     madx.command.endmatch()
 
 
 def correct_lhc_orbit(
     madx: Madx,
+    /,
     sequence: str,
     orbit_tolerance: float = 1e-14,
     iterations: int = 3,
     mode: str = "micado",
     **kwargs,
 ) -> None:
     """
@@ -151,15 +153,15 @@
 
     Routine for orbit correction using ``MCB.*`` elements in the LHC. This uses the
     ``CORRECT`` command in ``MAD-X`` behind the scenes, refer to the
     `MAD-X manual <http://madx.web.cern.ch/madx/releases/last-rel/madxuguide.pdf>`_ for
     usage information.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         sequence (str): which sequence to use the routine on.
         orbit_tolerance (float): the tolerance for the correction. Defaults to 1e-14.
         iterations (int): the number of iterations of the correction to perform.
             Defaults to 3.
         mode (str): the method to use for the correction. Defaults to ``micado`` as in
             the `CORRECT` command.
         **kwargs: Any keyword argument that can be given to the ``MAD-X`` ``CORRECT``
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_setup.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
     .. note::
         Matching is **not** performed by this function and should be taken care of by the user, but the working point
         should be set by the definitions in the *opticsfile*. Beware that passing specific variables as keyword arguments
         might change that working point.
 
     Args:
-        opticsfile (str): name of the optics file to be used. Can be the string path to the file or only the opticsfile
-            name itself, which would be looked for at the **acc-models-lhc/operation/optics/** path.
+        opticsfile (str): the relative string path or a `Path` object to the opticsfile location. This will 
+            be used to determine the location of the sequence file, see the admonition above.
         beam (int): which beam to set up for. Defaults to beam 1.
         use_b4 (bool): if `True`, the lhcb4 sequence file will be used. This is the beam 2 sequence but for tracking
             purposes. Defaults to `False`.
         energy (float): beam energy to set up for, in GeV. Defaults to 6500.
         slicefactor (int): if provided, the sequence will be sliced and made thin. Defaults to `None`,
             which leads to an unsliced sequence.
         **kwargs: if `echo` or `warn` are found in the keyword arguments they will be transmitted as options
@@ -65,14 +65,15 @@
         raise ValueError("Cannot use beam 4 sequence file for beam 1")
 
     def _run2_sequence_from_opticsfile(opticsfile: Path, use_b4: bool = False) -> Path:
         filename = "lhc_as-built.seq" if not use_b4 else "lhcb4_as-built.seq"
         seqfile_path = opticsfile.parent.parent / filename
         if not seqfile_path.is_file():
             logger.error(f"Could not find sequence file '{filename}' at expected location '{seqfile_path}'")
+            raise ValueError(f"No sequence file found at '{seqfile_path}'")
         return seqfile_path
 
     logger.debug("Creating Run 2 setup MAD-X instance")
     echo, warn = kwargs.pop("echo", False), kwargs.pop("warn", False)
 
     madx = Madx(**kwargs)
     madx.option(echo=echo, warn=warn)
@@ -259,27 +260,28 @@
 
 
 # ----- Configuration Utlites ----- #
 
 
 def make_lhc_beams(
     madx: Madx,
+    /,
     energy: float = 7000,
     emittance_x: float = 3.75e-6,
     emittance_y: float = 3.75e-6,
     b4: bool = False,
     **kwargs,
 ) -> None:
     """
     .. versionadded:: 0.15.0
 
     Defines beams with default configuratons for ``LHCB1`` and ``LHCB2`` sequences.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         energy (float): beam energy, in [GeV]. Defaults to 6500.
         emittance_x (float): horizontal emittance in [m]. Will be used to calculate
             geometric emittance which is then fed to the ``BEAM`` command.
         emittance_y (float): vertical emittance in [m]. Will be used to calculate
             geometric emittance which is then fed to the ``BEAM`` command.
         b4 (bool): if `True`, will consider one is using ``lhb4`` to do tracking on beam 2,
             and will properly set the ``bv`` flag to 1. Defaults to `False`.
@@ -316,15 +318,15 @@
             ex=geometric_emit_x,
             ey=geometric_emit_y,
             sige=4.5e-4,
             **kwargs,
         )
 
 
-def make_lhc_thin(madx: Madx, sequence: str, slicefactor: int = 1, **kwargs) -> None:
+def make_lhc_thin(madx: Madx, /, sequence: str, slicefactor: int = 1, **kwargs) -> None:
     """
     .. versionadded:: 0.15.0
 
     Executes the ``MAKETHIN`` command for the LHC sequence as previously done in ``MAD-X`` macros.
     This will use the ``teapot`` style and will enforce ``makedipedge``.
 
     One can find an exemple use of this function in the :ref:`AC Dipole Tracking <demo-ac-dipole-tracking>`
@@ -378,15 +380,15 @@
 
     madx.use(sequence=sequence)
     style = kwargs.get("style", "teapot")
     makedipedge = kwargs.get("makedipedge", False)  # defaults to False to compensate default TEAPOT style
     madx.command.makethin(sequence=sequence, style=style, makedipedge=makedipedge)
 
 
-def re_cycle_sequence(madx: Madx, sequence: str = "lhcb1", start: str = "IP3") -> None:
+def re_cycle_sequence(madx: Madx, /, sequence: str = "lhcb1", start: str = "IP3") -> None:
     """
     .. versionadded:: 0.15.0
 
     Re-cycles the provided *sequence* from a different starting point, given as *start*.
 
     One can find an exemple use of this function in the :ref:`AC Dipole Tracking <demo-ac-dipole-tracking>`
     and :ref:`Free Tracking <demo-free-tracking>` example galleries.
@@ -465,24 +467,24 @@
         "on_xx1": "on_x1",
         "on_ssep5": "on_sep5",
         "on_xx5": "on_x5",
     }
     return variables, special
 
 
-def setup_lhc_orbit(madx: Madx, scheme: str = "flat", **kwargs) -> Dict[str, float]:
+def setup_lhc_orbit(madx: Madx, /, scheme: str = "flat", **kwargs) -> Dict[str, float]:
     """
     .. versionadded:: 0.8.0
 
     Automated orbit setup for (HL)LHC runs, for some default schemes. It is assumed that at
     least sequence and optics files have been called. Initial implementation credits go to
     :user:`Joschua Dilly <joschd>`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         scheme (str): the default scheme to apply, as defined in the ``LHC_CROSSING_SCHEMES``
             constant. Accepted values are keys of `LHC_CROSSING_SCHEMES`. Defaults to *flat*
             (every orbit variable to 0).
         **kwargs: Any standard crossing scheme variables (``on_x1``, ``phi_IR1``, etc). Values
             given here override the values in the default scheme configurations.
 
     Returns:
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/cpymadtools/lhc/_twiss.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/cpymadtools/lhc/_twiss.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,49 +12,49 @@
 from cpymad.madx import Madx
 from loguru import logger
 
 from pyhdtoolkit.cpymadtools import twiss
 from pyhdtoolkit.cpymadtools.constants import DEFAULT_TWISS_COLUMNS
 
 
-def get_ips_twiss(madx: Madx, columns: Sequence[str] = DEFAULT_TWISS_COLUMNS, **kwargs) -> tfs.TfsDataFrame:
+def get_ips_twiss(madx: Madx, /, columns: Sequence[str] = DEFAULT_TWISS_COLUMNS, **kwargs) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.9.0
 
     Quickly get the ``TWISS`` table for certain variables at IP locations only. The ``SUMM`` table will be
     included as the `~tfs.frame.TfsDataFrame`'s header dictionary.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         columns (Sequence[str]): the variables to be returned, as columns in the DataFrame.
         **kwargs: Any keyword argument that can be given to the ``MAD-X`` ``TWISS`` command, such as ``chrom``,
             ``ripken``, ``centre``; or starting coordinates with ``betx``, ``bety`` etc.
 
     Returns:
         A `~tfs.frame.TfsDataFrame` of the ``TWISS`` table's sub-selection.
 
     Example:
         .. code-block:: python
 
             >>> ips_df = get_ips_twiss(madx, chrom=True, ripken=True)
     """
     logger.debug("Getting Twiss at IPs")
-    return twiss.get_pattern_twiss(madx=madx, columns=columns, patterns=["IP"], **kwargs)
+    return twiss.get_pattern_twiss(madx, columns=columns, patterns=["IP"], **kwargs)
 
 
-def get_ir_twiss(madx: Madx, ir: int, columns: Sequence[str] = DEFAULT_TWISS_COLUMNS, **kwargs) -> tfs.TfsDataFrame:
+def get_ir_twiss(madx: Madx, /, ir: int, columns: Sequence[str] = DEFAULT_TWISS_COLUMNS, **kwargs) -> tfs.TfsDataFrame:
     """
     .. versionadded:: 0.9.0
 
     Quickly get the ``TWISS`` table for certain variables for one Interaction Region, meaning at the IP and
     Q1 to Q3 both left and right of the IP. The ``SUMM`` table will be included as the `~tfs.frame.TfsDataFrame`'s
     header dictionary.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         ir (int): which interaction region to get the TWISS for.
         columns (Sequence[str]): the variables to be returned, as columns in the DataFrame.
         **kwargs: Any keyword argument that can be given to the ``MAD-X`` ``TWISS`` command, such as ``chrom``,
             ``ripken``, ``centre``; or starting coordinates with ``betx``, ``bety`` etc.
 
     Returns:
         A `~tfs.frame.TfsDataFrame` of the ``TWISS`` table's sub-selection.
@@ -62,15 +62,15 @@
     Example:
         .. code-block:: python
 
             >>> ir_df = get_ir_twiss(madx, chrom=True, ripken=True)
     """
     logger.debug(f"Getting Twiss for IR{ir:d}")
     return twiss.get_pattern_twiss(
-        madx=madx,
+        madx,
         columns=columns,
         patterns=[
             f"IP{ir:d}",
             f"MQXA.[12345][RL]{ir:d}",  # Q1 and Q3 LHC
             f"MQXB.[AB][12345][RL]{ir:d}",  # Q2A and Q2B LHC
             f"MQXF[AB].[AB][12345][RL]{ir:d}",  # Q1 to Q3 A and B HL-LHC
         ],
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/maths/nonconvex_phase_sync.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/maths/nonconvex_phase_sync.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/maths/stats_fitting.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/maths/stats_fitting.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/maths/utils.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/maths/utils.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/models/beam.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/models/beam.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/models/htc.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/models/htc.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/models/madx.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/models/madx.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/optics/beam.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/optics/beam.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/optics/ripken.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/optics/ripken.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/optics/twiss.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/optics/twiss.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/crossing.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/crossing.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import tfs
 
 from cpymad.madx import Madx
 from loguru import logger
 
 
 def plot_two_lhc_ips_crossings(
-    madx: Madx, first_ip: int, second_ip: int, ir_limit: float = 275, highlight_mqx_and_mbx: bool = True
+    madx: Madx, /, first_ip: int, second_ip: int, ir_limit: float = 275, highlight_mqx_and_mbx: bool = True
 ) -> None:
     """
     .. versionadded:: 1.0.0
 
     Creates a plot representing the crossing schemes at the two provided IPs. One can find an example
     use of this function in the :ref:`LHC crossing schemes <demo-crossing-schemes>` example gallery.
 
@@ -40,15 +40,15 @@
     .. warning::
         This function will get ``TWISS`` tables for both beams, which means it will ``USE`` both the
         ``lhcb1`` and ``lhcb2`` sequences, erasing previously defined errors or orbit corrections. The
         second sequence ``USE`` will be called on is ``lhcb2``, which may not be the one you were using
         before. Please re-``use`` your wanted sequence after calling this function!
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         first_ip (int): the first of the two IPs to plot crossing schemes for.
         second_ip (int): the second of the two IPs to plot crossing schemes for.
         ir_limit (float): the amount of meters to keep left and right of the IP point. Will also
             determine the ``xlimits`` of the plots. Defaults to 275.
         highlight_mqx_and_mbx (bool): if `True`, will add patches highlighting the zones corresponding
             to ``MBX`` and ``MQX`` elements. Defaults to `True`.
         **kwargs: If either `ax` or `axis` is found in the kwargs, the corresponding value is used as the
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/lattice.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/lattice.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 .. _plotting-lattice:
 
 Lattice Plotters
 ----------------
 
 Module with functions to create lattice plots through a `~cpymad.madx.Madx` object.
 """
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import matplotlib
 import matplotlib.axes
 import matplotlib.pyplot as plt
-import pandas as pd
 
 from cpymad.madx import Madx
 from loguru import logger
 
-from pyhdtoolkit.plotting.layout import plot_machine_layout
+from pyhdtoolkit.plotting.layout import _ylim_from_input, plot_machine_layout
 from pyhdtoolkit.plotting.utils import (
     _get_twiss_table_with_offsets_and_limits,
     make_survey_groups,
     maybe_get_ax,
 )
 
 
 def plot_latwiss(
     madx: Madx,
+    /,
     title: Optional[str] = None,
     xoffset: float = 0,
     xlimits: Tuple[float, float] = None,
     plot_dipoles: bool = True,
     plot_dipole_k1: bool = False,
     plot_quadrupoles: bool = True,
     plot_bpms: bool = False,
-    disp_ylim: Tuple[float, float] = None,
-    beta_ylim: Tuple[float, float] = None,
-    k0l_lim: Tuple[float, float] = None,
-    k1l_lim: Tuple[float, float] = None,
-    k2l_lim: Tuple[float, float] = None,
+    disp_ylim: Union[Tuple[float, float], float, int] = None,
+    beta_ylim: Union[Tuple[float, float], float, int] = None,
+    k0l_lim: Union[Tuple[float, float], float, int] = None,
+    k1l_lim: Union[Tuple[float, float], float, int] = None,
+    k2l_lim: Union[Tuple[float, float], float, int] = None,
+    k3l_lim: Union[Tuple[float, float], float, int] = None,
     **kwargs,
 ) -> None:
     """
     .. versionadded:: 1.0.0
 
     Creates a plot on the current figure (`~matplotlib.pyplot.gcf`) representing the lattice layout and
     the :math:`\\beta`-functions along with the horizontal dispertion function. This is a *very, very heavily
@@ -61,15 +62,15 @@
     .. warning::
         Currently the function tries to plot legends for the different layout patches. The position of the
         different legends has been hardcoded in corners and might require users to tweak the axis limits
         (through ``k0l_lim``, ``k1l_lim`` and ``k2l_lim``) to ensure legend labels and plotted elements don't
         overlap.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         title (Optional[str]): if provided, is set as title of the plot. Defaults to `None`.
         xoffset (float): An offset applied to the ``S`` coordinate before plotting. This is useful if
             you want to center a plot around a specific point or element, which would then become located
             at :math:`s = 0`. Beware this offset is applied before applying the *xlimits*. Defaults to 0.
         xlimits (Tuple[float, float]): will implement xlim (for the ``s`` coordinate) if this is
             not ``None``, using the tuple passed.
         plot_dipoles (bool): if `True`, dipole patches will be plotted on the layout subplot of
@@ -77,39 +78,69 @@
         plot_dipole_k1 (bool): if `True`, dipole elements with a quadrupolar gradient will have this
             gradient plotted as a quadrupole patch. Defaults to `False`.
         plot_quadrupoles (bool): if `True`, quadrupole patches will be plotted on the layout
             subplot of the figure. Defaults to `True`. Quadrupoles are plotted in red.
         plot_bpms (bool): if `True`, additional patches will be plotted on the layout subplot to
             represent Beam Position Monitors. BPMs are plotted in dark grey.
         disp_ylim (Tuple[float, float]): vertical axis limits for the dispersion values.
-            Defaults to `None`.
+            Can be given as a single value (float, int) or a tuple (in which case it should be
+            symmetric). Defaults to (-10, 125).
         beta_ylim (Tuple[float, float]): vertical axis limits for the betatron function values.
-            Defaults to None, to be determined by matplotlib based on the provided beta values.
-        k0l_lim (Tuple[float, float]): vertical axis limits for the ``k0l`` values used for the
-            height of dipole patches. Defaults to `None`.
-        k1l_lim (Tuple[float, float]): vertical axis limits for the ``k1l`` values used for the
-            height of quadrupole patches. Defaults to `None`.
-        k2l_lim (Tuple[float, float]): if given, sextupole patches will be plotted on the layout subplot of
-            the figure, and the provided values act as vertical axis limits for the k2l values used for the
-            height of sextupole patches.
-        **kwargs: any keyword argument will be transmitted to `~.plotting.utils.plot_machine_layout`, later on
-            to `~.plotting.utils._plot_lattice_series`, and then `~matplotlib.patches.Rectangle`, such as ``lw`` etc.
+            Can be given as a single value (float, int) or a tuple (in which case it should be
+            symmetric). Defaults to `None`, to be determined by `~matplotlib` based on the
+            plotted beta values.
+        k0l_lim (Union[Tuple[float, float], float, int]): vertical axis limits for the ``k0l``
+            values used for the height of dipole patches. Can be given as a single value (float,
+            int) or a tuple (in which case it should be symmetric). If `None` (default) is given,
+            then the limits will be auto-determined based on the ``k0l`` values of the dipoles in
+            the plot.
+        k1l_lim (Union[Tuple[float, float], float, int]): vertical axis limits for the ``k1l``
+            values used for the height of quadrupole patches. Can be given as a single value (float,
+            int) or a tuple (in which case it should be symmetric). If `None` (default) is given,
+            then the limits will be auto-determined based on the ``k0l`` values of the quadrupoles
+            in the plot.
+        k2l_lim (Union[Tuple[float, float], float, int]): if given, sextupole patches will be plotted
+            on the layout subplot of the figure. If given, acts as vertical axis limits for the k2l
+            values used for the height of sextupole patches. Can be given as a single value (float,
+            int) or a tuple (in which case it should be symmetric).
+        k3l_lim (Union[Tuple[float, float], float, int]): if given, octupole patches will be plotted
+            on the layout subplot of the figure. If given, acts as vertical axis limits for the k3l
+            values used for the height of octupole patches. Can be given as a single value (float,
+            int) or a tuple (in which case it should be symmetric).
+        **kwargs: any keyword argument will be transmitted to `~.plotting.utils.plot_machine_layout`,
+            later on to `~.plotting.utils._plot_lattice_series`, and then `~matplotlib.patches.Rectangle`,
+            such as ``lw`` etc.
 
     Example:
         .. code-block:: python
 
             >>> title = "Machine Layout"
             >>> plt.figure(figsize=(16, 11))
             >>> plot_latwiss(
             ...     madx,
-                    title=title,
-                    k0l_lim=(-0.15, 0.15),
-                    k1l_lim=(-0.08, 0.08),
-                    disp_ylim=(-10, 125),
-                    lw=3,
+            ...     title=title,
+            ...     k0l_lim=(-0.15, 0.15),
+            ...     k1l_lim=(-0.08, 0.08),
+            ...     disp_ylim=(-10, 125),
+            ...     lw=3,
+            ... )
+
+        One can provide ylimits for the machine layout patches as single values:
+
+        .. code-block:: python
+
+            >>> title = "Machine Layout"
+            >>> plt.figure(figsize=(16, 11))
+            >>> plot_latwiss(
+            ...     madx,
+            ...     title=title,
+            ...     k0l_lim=0.15,  # identical to k0l_lim=(-0.15, 0.15)
+            ...     k1l_lim=0.08,  # identical to k1l_lim=(-0.08, 0.08)
+            ...     disp_ylim=(-10, 125),
+            ...     lw=3,
             ... )
     """
     # pylint: disable=too-many-arguments
     # Restrict the span of twiss_df to avoid plotting all elements then cropping when xlimits is given
     logger.debug("Plotting optics functions and machine layout")
     twiss_df = _get_twiss_table_with_offsets_and_limits(madx, xoffset, xlimits)
     xlimits = (twiss_df.s.min(), twiss_df.s.max()) if xlimits is None else xlimits
@@ -126,14 +157,15 @@
         plot_dipoles=plot_dipoles,
         plot_dipole_k1=plot_dipole_k1,
         plot_quadrupoles=plot_quadrupoles,
         plot_bpms=plot_bpms,
         k0l_lim=k0l_lim,
         k1l_lim=k1l_lim,
         k2l_lim=k2l_lim,
+        k3l_lim=k3l_lim,
         **kwargs,
     )
 
     # Plotting beta functions on remaining two thirds of the figure
     logger.debug("Plotting beta functions")
     betatron_axis = plt.subplot2grid((3, 3), (1, 0), colspan=3, rowspan=2, sharex=quadrupole_patches_axis)
     betatron_axis.plot(twiss_df.s, twiss_df.betx, label="$\\beta_x$")
@@ -149,42 +181,45 @@
     dispertion_axis.legend(loc=1)
     dispertion_axis.set_ylabel("$D_{x,y}$ $[m]$", color="brown")
     dispertion_axis.tick_params(axis="y", labelcolor="brown")
     dispertion_axis.grid(False)
 
     if beta_ylim:
         logger.debug("Setting ylim for betatron functions plot")
+        beta_ylim = _ylim_from_input(beta_ylim, "beta_ylim")
         betatron_axis.set_ylim(beta_ylim)
 
     if disp_ylim:
         logger.debug("Setting ylim for dispersion plot")
+        disp_ylim = _ylim_from_input(disp_ylim, "beta_ylim")
         dispertion_axis.set_ylim(disp_ylim)
 
     if xlimits:
         logger.debug("Setting xlim for longitudinal coordinate")
         plt.xlim(xlimits)
 
 
 def plot_machine_survey(
     madx: Madx,
+    /,
     title: str = None,
     show_elements: bool = False,
     high_orders: bool = False,
     **kwargs,
 ) -> matplotlib.axes.Axes:
     """
     .. versionadded:: 1.0.0
 
     Creates a plot representing the lattice layout and the machine geometry in 2D. This is a very,
     very heavily refactored version of an initial implementation by :user:`Guido Sterbini <sterbini>`.
     One can find an example use of this function in the :ref:`machine survey <demo-machine-survey>`
     example gallery.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         title (Optional[str]): if provided, is set as title of the plot. Defaults to `None`.
         show_elements (bool): if `True`, will try to plot by differentiating elements.
             Defaults to `False`.
         high_orders (bool): if `True`, plots sextupoles and octupoles if *show_elements* is `True`,
             otherwise only up to quadrupoles. Defaults to `False`.
         **kwargs: any keyword argument will be transmitted to `~matplotlib.pyplot.scatter` calls
             later on. If either `ax` or `axis` is found in the kwargs, the corresponding value is
@@ -215,21 +250,29 @@
             element_dfs["dipoles"].z,
             element_dfs["dipoles"].x,
             marker=".",
             c=element_dfs["dipoles"].s,
             label="Dipoles",
             **kwargs,
         )
-        plt.scatter(element_dfs["quad_foc"].z, element_dfs["quad_foc"].x, marker="o", color="blue", label="QF")
-        plt.scatter(element_dfs["quad_defoc"].z, element_dfs["quad_defoc"].x, marker="o", color="red", label="QD")
+        plt.scatter(
+            element_dfs["quad_foc"].z, element_dfs["quad_foc"].x, marker="o", color="blue", label="QF"
+        )
+        plt.scatter(
+            element_dfs["quad_defoc"].z, element_dfs["quad_defoc"].x, marker="o", color="red", label="QD"
+        )
 
         if high_orders:
             logger.debug("Plotting high order magnetic elements (up to octupoles)")
-            plt.scatter(element_dfs["sextupoles"].z, element_dfs["sextupoles"].x, marker=".", color="m", label="MS")
-            plt.scatter(element_dfs["octupoles"].z, element_dfs["octupoles"].x, marker=".", color="cyan", label="MO")
+            plt.scatter(
+                element_dfs["sextupoles"].z, element_dfs["sextupoles"].x, marker=".", color="m", label="MS"
+            )
+            plt.scatter(
+                element_dfs["octupoles"].z, element_dfs["octupoles"].x, marker=".", color="cyan", label="MO"
+            )
         plt.legend(loc=2)
 
     else:
         logger.debug("Plotting survey without elements differentiation")
         plt.scatter(survey.z, survey.x, c=survey.s, marker=".", **kwargs)
 
     # Trying a trick to ensure the colorbar scales values properly up to the max S value and not 1
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/layout.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/layout.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 Layout Plotters
 ---------------
 
 Module with functions used to represent a machine' elements in an `~matplotlib.axes.Axes`
 object, mostly used in different `~pyhdtoolkit.plotting` modules.
 """
-from cmath import log
-from typing import Tuple
+from typing import Tuple, Union
 
 import matplotlib
 import matplotlib.axes
 import matplotlib.patches as patches
 import pandas as pd
 
 from cpymad.madx import Madx
@@ -23,107 +22,145 @@
     make_elements_groups,
     maybe_get_ax,
 )
 
 
 def plot_machine_layout(
     madx: Madx,
+    /,
     title: str = None,
     xoffset: float = 0,
     xlimits: Tuple[float, float] = None,
     plot_dipoles: bool = True,
     plot_dipole_k1: bool = False,
     plot_quadrupoles: bool = True,
     plot_bpms: bool = False,
-    k0l_lim: Tuple[float, float] = None,
-    k1l_lim: Tuple[float, float] = None,
-    k2l_lim: Tuple[float, float] = None,
+    k0l_lim: Union[Tuple[float, float], float, int] = None,
+    k1l_lim: Union[Tuple[float, float], float, int] = None,
+    k2l_lim: Union[Tuple[float, float], float, int] = None,
+    k3l_lim: Union[Tuple[float, float], float, int] = None,
     **kwargs,
 ) -> None:
     """
     .. versionadded:: 1.0.0
 
-    Draws patches elements representing the lattice layout on the given *axis*. This is
-    the function that takes care of the machine layout axis in `~.plotting.lattice.plot_latwiss`
-    and `~.plotting.aperture.plot_aperture`. Its results can be seen in the
-    :ref:`machine lattice <demo-accelerator-lattice>` and :ref:`machine aperture <demo-accelerator-aperture>`
-    example galleries.
+    Draws patches elements representing the lattice layout on the given
+    *axis*. This is the function that takes care of the machine layout axis
+    in `~.plotting.lattice.plot_latwiss` and
+    `~.plotting.aperture.plot_aperture`. Its results can be seen in the
+    :ref:`machine lattice <demo-accelerator-lattice>` and
+    :ref:`machine aperture <demo-accelerator-aperture>` example galleries.
 
     .. note::
-        This current implementation can plot dipoles, quadrupoles, sextupoles and BPMs.
+        This current implementation can plot dipoles, quadrupoles, sextupoles,
+        octupoles and BPMs.
 
     .. important::
-        If not provided, the limits for the ``k0l_lim``, ``k1l_lim`` will be auto-determined, which might
-        not be the perfect choice for you plot. When providing these limits (also for ``k2l_lim``), make
-        sure to provide symmetric values around 0 (so [-x, x]) otherwise the element patches will show up
-        vertically displaced from the axis' center line.
+        If not provided, the limits for the ``k0l_lim``, ``k1l_lim`` will be
+        auto-determined, which might not be the perfect choice for you plot.
+        When providing these limits (also for ``k2l_lim``), make sure to
+        provide symmetric values around 0 (so [-x, x]) otherwise the element
+        patches will show up vertically displaced from the axis' center line.
 
     .. warning::
-        Currently the function tries to plot legends for the different layout patches. The position of the
-        different legends has been hardcoded in corners of the `~matplotlib.axes.Axes` and might require users
-        to tweak the axis limits (through ``k0l_lim``, ``k1l_lim`` and ``k2l_lim``) to ensure legend labels and
-        plotted elements don't overlap.
+        Currently the function tries to plot legends for the different layout
+        patches. The position of the different legends has been hardcoded in
+        corners of the `~matplotlib.axes.Axes` and might require users to tweak
+        the axis limits (through ``k0l_lim``, ``k1l_lim`` and ``k2l_lim``) to
+        ensure legend labels and plotted elements don't overlap.
 
     Args:
         madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
-        title (Optional[str]): if provided, is set as title of the plot. Defaults to `None`.
-        xoffset (float): An offset applied to the ``S`` coordinate before plotting. This is useful if
-            you want to center a plot around a specific point or element, which would then become located
-            at :math:`s = 0`. Beware this offset is applied before applying the *xlimits*. Defaults to 0.
-        xlimits (Tuple[float, float]): will implement xlim (for the ``s`` coordinate) if this is
-            not ``None``, using the tuple passed.
-        plot_dipoles (bool): if `True`, dipole patches will be plotted on the layout subplot of
-            the figure. Defaults to `True`. Dipoles are plotted in blue.
-        plot_dipole_k1 (bool): if `True`, dipole elements with a quadrupolar gradient will have this
-            gradient plotted as a quadrupole patch. Defaults to `False`.
-        plot_quadrupoles (bool): if `True`, quadrupole patches will be plotted on the layout
-            subplot of the figure. Defaults to `True`. Quadrupoles are plotted in red.
-        plot_bpms (bool): if `True`, additional patches will be plotted on the layout subplot to
-            represent Beam Position Monitors. BPMs are plotted in dark grey.
-        disp_ylim (Tuple[float, float]): vertical axis limits for the dispersion values.
-            Defaults to (-10, 125).
-        beta_ylim (Tuple[float, float]): vertical axis limits for the betatron function values.
-            Defaults to None, to be determined by matplotlib based on the provided beta values.
-        k0l_lim (Tuple[float, float]): vertical axis limits for the ``k0l`` values used for the
-            height of dipole patches, should be symmetric. If `None` (default) is provided, then
-            the limits will be auto-determined based on the ``k0l`` values of the dipoles in the
-            plot.
-        k1l_lim (Tuple[float, float]): vertical axis limits for the ``k1l`` values used for the
-            height of quadrupole patches, should be symmetric. If `None` (default) is provided,
-            then the limits will be auto-determined based on the ``k0l`` values of the dipoles
-            in the plot.
-        k2l_lim (Tuple[float, float]): if given, sextupole patches will be plotted on the layout subplot of
-            the figure, and the provided values act as vertical axis limits for the k2l values used for the
-            height of sextupole patches.
-        **kwargs: any keyword argument will be transmitted to `~.plotting.utils.plot_machine_layout`, later on
-            to `~.plotting.utils._plot_lattice_series`, and then `~matplotlib.patches.Rectangle`, such as ``lw``
-            etc. If either `ax` or `axis` is found in the kwargs, the corresponding value is used as the axis
-            object to plot on. By definition, the quadrupole elements will be drawn on said axis, and for each
-            new element type to plot a call to `~matplotlib.axes.Axes.twinx` is made and the new elements will
-            be drawn on the newly created twin `~matplotlib.axes.Axes`.
+            Positional only.
+        title (Optional[str]): if provided, is set as title of the plot.
+            Defaults to `None`.
+        xoffset (float): An offset applied to the ``S`` coordinate before
+            plotting. This is useful if you want to center a plot around a
+                specific point or element, which would then become located
+            at :math:`s = 0`. Beware this offset is applied before applying
+            the *xlimits*. Defaults to 0.
+        xlimits (Tuple[float, float]): will implement xlim (for the ``s``
+            coordinate) if this is not ``None``, using the tuple passed.
+        plot_dipoles (bool): if `True`, dipole patches will be plotted on
+            the layout subplot of the figure. Defaults to `True`. Dipoles
+            are plotted in blue.
+        plot_dipole_k1 (bool): if `True`, dipole elements with a quadrupolar
+            gradient will have this gradient plotted as a quadrupole patch.
+            Defaults to `False`.
+        plot_quadrupoles (bool): if `True`, quadrupole patches will be plotted
+            on the layout subplot of the figure. Defaults to `True`.
+            Quadrupoles are plotted in red.
+        plot_bpms (bool): if `True`, additional patches will be plotted on the
+            layout subplot to represent Beam Position Monitors. BPMs are
+            plotted in dark grey.
+        k0l_lim (Union[Tuple[float, float], float, int]): vertical axis limits
+            for the ``k0l`` values used for the height of dipole patches. Can
+            be given as a single value (float, int) or a tuple (in which case
+            it should be symmetric). If `None` (default) is given, then the
+            limits will be auto-determined based on the ``k0l`` values of the
+            dipoles in the plot.
+        k1l_lim (Union[Tuple[float, float], float, int]): vertical axis limits
+            for the ``k1l`` values used for the height of quadrupole patches.
+            Can be given as a single value (float, int) or a tuple (in which
+            case it should be symmetric). If `None` (default) is given, then
+            the limits will be auto-determined based on the ``k0l`` values of
+            the quadrupoles in the plot.
+        k2l_lim (Union[Tuple[float, float], float, int]): if given, sextupole
+            patches will be plotted on the layout subplot of the figure. If
+            given, acts as vertical axis limits for the k2l values used for
+            the height of sextupole patches. Can be given as a single value
+            (float, int) or a tuple (in which case it should be symmetric).
+        k3l_lim (Union[Tuple[float, float], float, int]): if given, octupole
+            patches will be plotted on the layout subplot of the figure. If
+            given, acts as vertical axis limits for the k3l values used for
+            the height of octupole patches. Can be given as a single value
+            (float, int) or a tuple (in which case it should be symmetric).
+        **kwargs: any keyword argument will be transmitted to
+            `~.plotting.utils.plot_machine_layout`, later on to
+            `~.plotting.utils._plot_lattice_series`, and then
+            `~matplotlib.patches.Rectangle`, such as ``lw`` etc. If either
+            `ax` or `axis` is found in the kwargs, the corresponding value
+            is used as the axis object to plot on. By definition, the
+            quadrupole elements will be drawn on said axis, and for each
+            new element type to plot a call to `~matplotlib.axes.Axes.twinx`
+            is made and the new elements will be drawn on the newly created
+            twin `~matplotlib.axes.Axes`. If ``bpms_legend`` is given as
+            `False` and BPMs are plotted, the BPM legend will not be plotted
+            on the layout axis.
 
     Example:
         .. code-block:: python
 
             >>> fig, ax = plt.subplots(figsize=(6, 2))
             >>> plot_machine_layout(madx, title="Machine Elements", lw=3)
     """
     # pylint: disable=too-many-arguments
     axis, kwargs = maybe_get_ax(**kwargs)
+    bpms_legend = kwargs.pop("bpms_legend", True)
     twiss_df = _get_twiss_table_with_offsets_and_limits(madx, xoffset, xlimits)
 
     logger.trace("Extracting element-specific dataframes")
     element_dfs = make_elements_groups(madx, xoffset, xlimits)
     dipoles_df = element_dfs["dipoles"]
     quadrupoles_df = element_dfs["quadrupoles"]
     sextupoles_df = element_dfs["sextupoles"]
+    octupoles_df = element_dfs["octupoles"]
     bpms_df = element_dfs["bpms"]
 
-    k0l_lim = k0l_lim or _determine_default_knl_lim(dipoles_df, col="k0l", coeff=2)
-    k1l_lim = k1l_lim or _determine_default_knl_lim(quadrupoles_df, col="k1l", coeff=1.3)
+    logger.trace("Determining the ylimits for k0l and k1l patches")
+    k0l_lim = (
+        _ylim_from_input(k0l_lim, "k0l_lim")
+        if k0l_lim is not None
+        else _determine_default_knl_lim(dipoles_df, col="k0l", coeff=2)
+    )
+    k1l_lim = (
+        _ylim_from_input(k1l_lim, "k1l_lim")
+        if k1l_lim is not None
+        else _determine_default_knl_lim(quadrupoles_df, col="k1l", coeff=1.3)
+    )
 
     logger.debug("Plotting machine layout")
     logger.trace(f"Plotting from axis '{axis}'")
     axis.set_ylabel("$1/f=K_{1}L$ $[m^{-1}]$", color="red")  # quadrupole in red
     axis.tick_params(axis="y", labelcolor="red")
     axis.set_ylim(k1l_lim)
     if xlimits is not None:
@@ -160,15 +197,17 @@
                     dipole,
                     height=dipole.k1l,
                     v_offset=dipole.k1l / 2,
                     color="r",
                     **kwargs,
                 )
             plotted_elements += 1
-        dipole_patches_axis.legend(loc=1)
+        logger.debug(f"Plotted {plotted_elements} dipole elements")
+        if plotted_elements > 0:  # If we plotted at least one dipole, we need to plot the legend
+            dipole_patches_axis.legend(loc=1)
 
     if plot_quadrupoles:
         logger.trace("Plotting quadrupole patches")
         plotted_elements = 0
         for quadrupole_name, quadrupole in quadrupoles_df.iterrows():
             logger.trace(f"Plotting quadrupole element '{quadrupole_name}'")
             _plot_lattice_series(
@@ -177,38 +216,71 @@
                 height=quadrupole.k1l,
                 v_offset=quadrupole.k1l / 2,
                 color="r",
                 label="MQ" if plotted_elements == 0 else None,  # avoid duplicating legend labels
                 **kwargs,
             )
             plotted_elements += 1
-        axis.legend(loc=2)
+        logger.debug(f"Plotted {plotted_elements} quadrupole elements")
+        if plotted_elements > 0:  # If we plotted at least one quadrupole, we need to plot the legend
+            axis.legend(loc=2)
 
     if k2l_lim:
         logger.trace("Plotting sextupole patches")
         sextupoles_patches_axis = axis.twinx()
         sextupoles_patches_axis.set_ylabel("$K_{2}L$ $[m^{-2}]$", color="darkgoldenrod")
         sextupoles_patches_axis.tick_params(axis="y", labelcolor="darkgoldenrod")
-        sextupoles_patches_axis.spines["right"].set_position(("axes", 1.1))
+        sextupoles_patches_axis.spines["right"].set_position(("axes", 1.12))
+        k2l_lim = _ylim_from_input(k2l_lim, "k2l_lim")
         sextupoles_patches_axis.set_ylim(k2l_lim)
         plotted_elements = 0
         for sextupole_name, sextupole in sextupoles_df.iterrows():
             logger.trace(f"Plotting sextupole element '{sextupole_name}'")
             _plot_lattice_series(
                 sextupoles_patches_axis,
                 sextupole,
                 height=sextupole.k2l,
                 v_offset=sextupole.k2l / 2,
                 color="goldenrod",
                 label="MS" if plotted_elements == 0 else None,  # avoid duplicating legend labels
                 **kwargs,
             )
             plotted_elements += 1
-        sextupoles_patches_axis.legend(loc=3)
+        logger.debug(f"Plotted {plotted_elements} sextupole elements")
         sextupoles_patches_axis.grid(False)
+        if plotted_elements > 0:  # If we plotted at least one sextupole, we need to plot the legend
+            sextupoles_patches_axis.legend(loc=3)
+
+    if k3l_lim:
+        logger.trace("Plotting octupole patches")
+        octupoles_patches_axis = axis.twinx()
+        octupoles_patches_axis.set_ylabel("$K_{3}L$ $[m^{-3}]$", color="forestgreen")
+        octupoles_patches_axis.tick_params(axis="y", labelcolor="forestgreen")
+        octupoles_patches_axis.yaxis.set_label_position("left")
+        octupoles_patches_axis.yaxis.tick_left()
+        octupoles_patches_axis.spines["left"].set_position(("axes", -0.14))
+        k3l_lim = _ylim_from_input(k3l_lim, "k3l_lim")
+        octupoles_patches_axis.set_ylim(k3l_lim)
+        plotted_elements = 0
+        for octupole_name, octupole in octupoles_df.iterrows():
+            logger.trace(f"Plotting octupole element '{octupole_name}'")
+            _plot_lattice_series(
+                octupoles_patches_axis,
+                octupole,
+                height=octupole.k3l,
+                v_offset=octupole.k3l / 2,
+                color="forestgreen",
+                label="MO" if plotted_elements == 0 else None,  # avoid duplicating legend labels
+                **kwargs,
+            )
+            plotted_elements += 1
+        logger.debug(f"Plotted {plotted_elements} octupole elements")
+        octupoles_patches_axis.grid(False)
+        if plotted_elements > 0:  # If we plotted at least one octupole, we need to plot the legend
+            octupoles_patches_axis.legend(loc=4)
 
     if plot_bpms:
         logger.trace("Plotting BPM patches")
         bpm_patches_axis = axis.twinx()
         bpm_patches_axis.set_axis_off()  # hide yticks, labels etc
         bpm_patches_axis.set_ylim(-1.6, 1.6)
         plotted_elements = 0
@@ -220,15 +292,29 @@
                 height=2,
                 v_offset=0,
                 color="dimgrey",
                 label="BPM" if plotted_elements == 0 else None,  # avoid duplicating legend labels
                 **kwargs,
             )
             plotted_elements += 1
-        bpm_patches_axis.legend(loc=4)
+        logger.debug(f"Plotted {plotted_elements} BPMs")
+        logger.trace("Determining BPM legend location")
+        if bpms_legend is True:
+            if k2l_lim is not None and k3l_lim is not None:
+                bpm_legend_loc = 8  # all corners are taken, we go bottom center
+            elif k2l_lim is not None:
+                bpm_legend_loc = 4  # sextupoles are here but not octupoles, we go bottom left
+            elif k3l_lim is not None:
+                bpm_legend_loc = 3  # octuoles are here but not sextupoles, we go bottom right
+            else:
+                bpm_legend_loc = (
+                    "best"  # can't easily determine the best position, go automatic and leave to the user
+                )
+            if plotted_elements > 0:  # If we plotted at least one BPM, we need to plot the legend
+                bpm_patches_axis.legend(loc=bpm_legend_loc)
         bpm_patches_axis.grid(False)
 
 
 # ----- Helpers ----- #
 
 
 def _plot_lattice_series(
@@ -239,49 +325,89 @@
     color: str = "r",
     alpha: float = 0.5,
     **kwargs,
 ) -> None:
     """
     .. versionadded:: 1.0.0
 
-    Plots a `~matplotlib.patches.Rectangle` element on the provided `~matplotlib.axes.Axes` to
-    represent an element of the machine. Original code from :user:`Guido Sterbini <sterbini>`.
+    Plots a `~matplotlib.patches.Rectangle` element on the provided
+    `~matplotlib.axes.Axes` to represent an element of the machine.
+    Original code from :user:`Guido Sterbini <sterbini>`.
 
     Args:
-        ax (matplotlib.axes.Axes): an existing  `~matplotlib.axes.Axes` object to draw on.
+        ax (matplotlib.axes.Axes): an existing  `~matplotlib.axes.Axes`
+            object to draw on.
         series (pd.DataFrame): a `pandas.DataFrame` with the elements' data.
         height (float): value to reach for the patch on the y axis.
         v_offset (float): vertical offset for the patch.
         color (str): color kwarg to transmit to `~matplotlib.pyplot`.
         alpha (float): alpha kwarg to transmit to `~matplotlib.pyplot`.
-        **kwargs: any keyword argument will be transmitted to `~matplotlib.patches.Rectangle`,
-            for instance ``lw`` for the edge line width.
+        **kwargs: any keyword argument will be transmitted to
+            `~matplotlib.patches.Rectangle`, for instance ``lw`` for the
+            edge line width.
     """
     ax.add_patch(
         patches.Rectangle(
             (series.s - series.l, v_offset - height / 2.0),  # anchor point
             series.l,  # width
             height,  # height
             color=color,
             alpha=alpha,
             **kwargs,
         )
     )
 
 
+def _ylim_from_input(
+    ylim: Union[Tuple[float, float], float, int], name_for_error: str = "knl_lim"
+) -> Tuple[float, float]:
+    """
+    .. versionadded:: 1.2.0
+
+    Determines the ylimits for a given axis from the input provided by the
+    user. This is used in `~.plotting.utils.plot_machine_layout` and handles
+    different inputs from the user, such as a tuple, a float and an int.
+
+    Args:
+        ylim (Tuple[float, float], float, int): the input provided by
+            the user.
+        name_for_error (str): the name of the variable to use in the
+            error message.
+
+    Returns:
+        A tuple for the ylimits from the input.
+
+    Raises:
+        TypeError: if the input is not a tuple, a float or an int.
+    """
+    if isinstance(ylim, tuple):
+        return ylim
+    elif isinstance(ylim, (float, int)):
+        if ylim >= 0:
+            return (-ylim, ylim)
+        else:
+            return (ylim, -ylim)
+    else:
+        raise TypeError(
+            f"Invalid type for '{name_for_error}': {type(ylim)}. "
+            "Should be a tuple, a float or an int. Can also be give as None."
+        )
+
+
 def _determine_default_knl_lim(df: pd.DataFrame, col: str, coeff: float) -> Tuple[float, float]:
     """
     .. versionadded:: 1.0.0
 
-    Determine the default limits for the ``knl`` axis, when plotting machine layout.
-    This is in case `None` are provided by the user, to make sure the plot still
-    looks coherent and symmetric in `~.plotting.utils.plot_machine_layout`.
+    Determine the default limits for the ``knl`` axis, when plotting machine
+    layout. This is in case `None` are provided by the user, to make sure the
+    plot still looks coherent and symmetric in 
+    `~.plotting.utils.plot_machine_layout`.
 
-    The limits are determined symmetric, using the maximum absolute value of the
-    knl column in the provided dataframe and a 1.25 scaling factor.
+    The limits are determined symmetric, using the maximum absolute value of
+    the knl column in the provided dataframe and a 1.25 scaling factor.
 
     Args:
         df (pd.DataFrame): a `pandas.DataFrame` with the multipoles' data.
             The ``knl`` column is used to determine the limits.
         col (str): the 'knl' column to query in the dataframe.
         coeff (float): a scaling factor to apply to the max absolute value
             when determining the limits.
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/phasespace.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/phasespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 COLORS_DICT = dict(mcolors.BASE_COLORS, **mcolors.CSS4_COLORS)
 BY_HSV = sorted((tuple(mcolors.rgb_to_hsv(mcolors.to_rgba(color)[:3])), name) for name, color in COLORS_DICT.items())
 SORTED_COLORS = [name for hsv, name in BY_HSV]
 
 
 def plot_courant_snyder_phase_space(
     madx: Madx,
+    /,
     u_coordinates: np.ndarray,
     pu_coordinates: np.ndarray,
     plane: str = "Horizontal",
     title: str = None,
     **kwargs,
 ) -> matplotlib.axes.Axes:
     """
     .. versionadded:: 1.0.0
 
     Creates a plot representing the normalized Courant-Snyder phase space of a particle distribution
     when provided by position and momentum coordinates for a specific plane. One can find an example
     use of this function in the :ref:`phase space <demo-phase-space>` example gallery.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         u_coordinates (np.ndarray): `~numpy.ndarray` of particles' coordinates for the given plane. Here
             ``u_coordinates[0]`` should be the tracked coordinates for the first particle and so on.
         pu_coordinates (np.ndarray): `~numpy.ndarray` of particles' momentum coordinates for the
             given plane. Here ``pu_coordinates[0]`` should be the tracked momenta for the first particle
             and so on.
         plane (str): the physical plane to plot, should be either ``Horizontal`` or ``Vertical``, and is
             case-insensitive. Defaults to ``Horizontal``.
@@ -86,14 +87,15 @@
             axis.set_ylabel(r"$\bar{py} \ [rad]$")
 
     return axis
 
 
 def plot_courant_snyder_phase_space_colored(
     madx: Madx,
+    /,
     u_coordinates: np.ndarray,
     pu_coordinates: np.ndarray,
     plane: str = "Horizontal",
     title: str = None,
     **kwargs,
 ) -> matplotlib.figure.Figure:
     """
@@ -102,15 +104,15 @@
     Creates a plot representing the normalized Courant-Snyder phase space of a particle distribution
     when provided by position and momentum coordinates for a specific plane. Each particle trajectory
     has its own color on the plot, within the limit of `~matplotlib.pyplot`'s 156 named colors, after
     the function loops back to the first color again. One can find an example use of this function in
     the :ref:`phase space <demo-phase-space>` example gallery.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         u_coordinates (np.ndarray): `~numpy.ndarray` of particles' coordinates for the given plane. Here
             ``u_coordinates[0]`` should be the tracked coordinates for the first particle and so on.
         pu_coordinates (np.ndarray): `~numpy.ndarray` of particles' momentum coordinates for the
             given plane. Here ``pu_coordinates[0]`` should be the tracked momenta for the first particle
             and so on.
         savefig (str): if not `None`, will save the figure to file using the string value passed.
         plane (str): the physical plane to plot, should be either ``Horizontal`` or ``Vertical``, and is
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/tune.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/tune.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/utils.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 .. _plotting-utils:
 
 Plotting Utility Functions
 --------------------------
 
 Module with functions to used throught the different `~pyhdtoolkit.plotting` modules.
 """
-from typing import Dict, Tuple
+from __future__ import annotations  # important for Sphinx to generate short type signatures!
 
 import matplotlib
 import matplotlib.axes
 import matplotlib.pyplot as plt
+import matplotlib.transforms as transforms
+import numpy as np
 import pandas as pd
 import tfs
 
 from cpymad.madx import Madx
 from loguru import logger
+from matplotlib.patches import Ellipse
+from numpy.typing import ArrayLike
 
 # ------ General Utilities ----- #
 
 
 def maybe_get_ax(**kwargs):
     """
     .. versionadded:: 1.0.0
@@ -46,15 +50,15 @@
             ...     ax, kwargs = maybe_get_ax(**kwargs)
             ...     # do stuff with ax
             ...     ax.plot(*args, **kwargs)
             ... )
     """
     logger.debug("Looking for axis object to plot on")
     if "ax" in kwargs:
-        logger.debug("Using the provided kwargs 'ax' as the axis to plot one")
+        logger.debug("Using the provided kwargs 'ax' as the axis to plot on")
         ax = kwargs.pop("ax")
     elif "axis" in kwargs:
         logger.debug("Using the provided kwargs 'axis' as the axis to plot on")
         ax = kwargs.pop("axis")
     else:
         logger.debug("No axis provided, using `plt.gca()`")
         ax = plt.gca()
@@ -93,15 +97,15 @@
         logger.debug("IP{ip:d} segment seems cut off by end of sequence, looping around to determine IP location")
         distance = (model_df.S.to_numpy().max() - first_element_s_in_model) + ip_s_in_model
     else:  # just the difference
         distance = ip_s_in_model - first_element_s_in_model
     return distance
 
 
-def get_lhc_ips_positions(dataframe: pd.DataFrame) -> Dict[str, float]:
+def get_lhc_ips_positions(dataframe: pd.DataFrame) -> dict[str, float]:
     """
     .. versionadded:: 1.0.0
 
     Returns a `dict` of LHC IPs and their positions from the provided *dataframe*.
 
     .. important::
         This function expects the IP names to be in the dataframe's index,
@@ -131,27 +135,27 @@
         ip_names = [f"ip{i:d}" for i in range(1, 9)]
         ip_pos = dataframe.loc[ip_names, "s"].to_numpy()
     ip_names = [name.upper() for name in ip_names]  # make sure to uppercase now
     return dict(zip(ip_names, ip_pos))
 
 
 def make_elements_groups(
-    madx: Madx, xoffset: float = 0, xlimits: Tuple[float, float] = None
-) -> Dict[str, pd.DataFrame]:
+    madx: Madx, /, xoffset: float = 0, xlimits: tuple[float, float] = None
+) -> dict[str, pd.DataFrame]:
     """
     .. versionadded:: 1.0.0
 
     Provided with an active `cpymad` instance after having ran a script, will returns different portions of
     the twiss table's dataframe for different magnetic elements.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         xoffset (float): An offset applied to the S coordinate before plotting. This is useful is you want
             to center a plot around a specific point or element, which would then become located at s = 0.
-        xlimits (Tuple[float, float]): will only consider elements within xlim (for the s coordinate) if this
+        xlimits (tuple[float, float]): will only consider elements within xlim (for the s coordinate) if this
             is not None, using the tuple passed.
 
     Returns:
         A `dict` containing a `pd.DataFrame` for dipoles, focusing quadrupoles, defocusing
         quadrupoles, sextupoles and octupoles. The keys are self-explanatory.
 
     Example:
@@ -171,23 +175,23 @@
         "quadrupoles": twiss_df[twiss_df.keyword.isin(["multipole", "quadrupole"])].query("k1l != 0 or k1sl != 0"),
         "sextupoles": twiss_df[twiss_df.keyword.isin(["multipole", "sextupole"])].query("k2l != 0 or k2sl " "!= 0"),
         "octupoles": twiss_df[twiss_df.keyword.isin(["multipole", "octupole"])].query("k3l != 0 or k3sl != " "0"),
         "bpms": twiss_df[(twiss_df.keyword.isin(["monitor"])) & (twiss_df.name.str.contains("BPM", case=False))],
     }
 
 
-def make_survey_groups(madx: Madx) -> Dict[str, pd.DataFrame]:
+def make_survey_groups(madx: Madx, /) -> dict[str, pd.DataFrame]:
     """
     .. versionadded:: 1.0.0
 
     Provided with an active `cpymad` instance after having ran a script, will returns different portions of
     the survey table's dataframe for different magnetic elements.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
 
     Returns:
         A `dict` containing a `pd.DataFrame` for dipoles, focusing quadrupoles, defocusing
         quadrupoles, sextupoles and octupoles. The keys are self-explanatory.
 
     Example:
         .. code-block:: python
@@ -211,15 +215,15 @@
     }
 
 
 # ----- Plotting Utilities -----#
 
 
 def draw_ip_locations(
-    ip_positions: Dict[str, float] = None,
+    ip_positions: dict[str, float] = None,
     lines: bool = True,
     location: str = "outside",
     **kwargs,
 ) -> None:
     """
     .. versionadded:: 1.0.0
 
@@ -267,34 +271,33 @@
             logger.debug(f"Skipping {ip_name} as its position is outside of the plot's xlimits")
 
     axis.set_xlim(xlimits)
     axis.set_ylim(ylimits)
 
 
 def set_arrow_label(
-    axis: matplotlib.axes.Axes,
     label: str,
-    arrow_position: Tuple[float, float],
-    label_position: Tuple[float, float],
+    arrow_position: tuple[float, float],
+    label_position: tuple[float, float],
     color: str = "k",
     arrow_arc_rad: float = -0.2,
     fontsize: int = 20,
     **kwargs,
 ) -> matplotlib.text.Annotation:
     """
     .. versionadded:: 0.6.0
 
     Adds on the provided `matplotlib.axes.Axes` a label box with text and an arrow from the box to a specified position.
     Original code from :user:`Guido Sterbini <sterbini>`.
 
     Args:
         axis (matplotlib.axes.Axes): a `matplotlib.axes.Axes` to plot on.
         label (str): label text to print on the axis.
-        arrow_position (Tuple[float, float]): where on the plot to point the tip of the arrow.
-        label_position (Tuple[float, float]): where on the plot the text label (and thus start
+        arrow_position (tuple[float, float]): where on the plot to point the tip of the arrow.
+        label_position (tuple[float, float]): where on the plot the text label (and thus start
             of the arrow) is.
         color (str): color parameter for your arrow and label. Defaults to "k".
         arrow_arc_rad (float): angle value defining the upwards / downwards shape of and
             bending of the arrow.
         fontsize (int): text size in the box.
         **kwargs: additional keyword arguments are transmitted to `~matplotlib.axes.Axes.annotate`.
             If either `ax` or `axis` is found in the kwargs, the corresponding value is used as the
@@ -328,38 +331,104 @@
         ha="center",
         bbox=dict(boxstyle="round4", fc="w", color=color),
         arrowprops=dict(arrowstyle="-|>", connectionstyle="arc3,rad=" + str(arrow_arc_rad), fc="w", color=color),
         **kwargs,
     )
 
 
+def draw_confidence_ellipse(x: ArrayLike, y: ArrayLike, n_std: float = 3.0, facecolor="none", **kwargs) -> Ellipse:
+    """
+    .. versionadded:: 1.2.0
+
+    Plot the covariance confidence ellipse of *x* and *y*. This code is taken from the
+    `matplotlib gallery <https://matplotlib.org/stable/gallery/statistics/confidence_ellipse.html>`_.
+
+    .. note::
+        One might want to provide the `edgecolor` to this function.
+
+    Args:
+        x (ArrayLike): array-like, should be of shape (n,).
+        y (ArrayLike): array-like, should be of shape (n,).
+        n_std (float): The number of standard deviations of the data to
+            highlight, to determine the ellipse's radiuses.
+        facecolor (str): The facecolor of the ellipse.
+        **kwargs: Any keyword argument will be forwarded to `~matplotlib.patches.Ellipse`.
+            If either `ax` or `axis` is found in the kwargs, the corresponding value is
+            used as the axis object to plot on.
+
+    Returns:
+        The corresponding `~matplotlib.patches.Ellipse` object added to the axis.
+
+    Example:
+        .. code-block:: python
+
+            >>> x = np.random.normal(size=1000)
+            >>> y = np.random.normal(size=1000)
+            >>> plt.plot(x, y, ".", markersize=0.8)
+            >>> draw_confidence_ellipse(x, y, n_std=2.5, edgecolor="red")
+    """
+    axis, kwargs = maybe_get_ax(**kwargs)
+    x = np.array(x)
+    y = np.array(y)
+
+    if x.size != y.size:
+        logger.error(f"x and y must be the same size, but shapes {x.shape} and {y.shape} were given.")
+        raise ValueError(f"x and y must be the same size, but shapes {x.shape} and {y.shape} were given.")
+
+    logger.debug("Computing covariance matrix and pearson correlation coefficient")
+    covariance_matrix = np.cov(x, y)
+    pearson = covariance_matrix[0, 1] / np.sqrt(covariance_matrix[0, 0] * covariance_matrix[1, 1])
+
+    # Using a special case to obtain the eigenvalues of this two-dimensionl dataset.
+    logger.debug("Computing radiuses of the ellipse")
+    radius_x = np.sqrt(1 + pearson)
+    radius_y = np.sqrt(1 - pearson)
+    ellipse = Ellipse((0, 0), width=radius_x * 2, height=radius_y * 2, facecolor=facecolor, **kwargs)
+
+    # Calculating the stdev of x from the square root of the variance and multiplying
+    # with the given number of standard deviations.
+    scale_x = np.sqrt(covariance_matrix[0, 0]) * n_std
+    mean_x = np.mean(x)
+
+    # Calculating the stdev of y from the square root of the variance and multiplying
+    # with the given number of standard deviations.
+    scale_y = np.sqrt(covariance_matrix[1, 1]) * n_std
+    mean_y = np.mean(y)
+
+    logger.debug("Preparing and drawing ellipse patch")
+    transf = transforms.Affine2D().rotate_deg(45).scale(scale_x, scale_y).translate(mean_x, mean_y)
+    ellipse.set_transform(transf + axis.transData)
+    return axis.add_patch(ellipse)
+
+
 # ----- Private Helpers ----- #
 
 
 def _get_twiss_table_with_offsets_and_limits(
-    madx: Madx, xoffset: float = 0, xlimits: Tuple[float, float] = None
+    madx: Madx, /, xoffset: float = 0, xlimits: tuple[float, float] = None, **kwargs
 ) -> pd.DataFrame:
     """
     .. versionadded:: 1.0.0
 
     Get the twiss dataframe from madx, only within the provided `xlimits` and with the s axis shifted by
     the given `xoffset`.
 
     Args:
-        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object.
+        madx (cpymad.madx.Madx): an instanciated `~cpymad.madx.Madx` object. Positional only.
         xoffset (float): An offset applied to the S coordinate in the dataframe.
-        xlimits (Tuple[float, float]): will only consider elements within xlimits (for the s coordinate) if
+        xlimits (tuple[float, float]): will only consider elements within xlimits (for the s coordinate) if
             this is not `None`, using the tuple passed.
+        **kwargs: any keyword argument will be transmitted to the ``MAD-X`` ``TWISS` command.
 
     Returns:
         The ``TWISS`` dataframe from ``MAD-X``, with the limits and offset applied, if any.
     """
     # Restrict the span of twiss_df to avoid plotting all elements then cropping when xlimits is given
     logger.trace("Getting TWISS table from MAD-X")
-    madx.command.twiss()
+    madx.command.twiss(**kwargs)
     twiss_df = madx.table.twiss.dframe()
     twiss_df.s = twiss_df.s - xoffset
     twiss_df = twiss_df[twiss_df.s.between(*xlimits)] if xlimits else twiss_df
     return twiss_df
 
 
 def _determine_default_sbs_coupling_ylabel(rdt: str, component: str) -> str:
```

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/sbs/coupling.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/sbs/coupling.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/sbs/phase.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/sbs/phase.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/styles/__init__.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/styles/paper.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/styles/paper.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/plotting/styles/thesis.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/plotting/styles/thesis.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/__init__.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/cmdline.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/contexts.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/executors.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/executors.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/htc_monitor.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/htc_monitor.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/logging.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/operations.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/operations.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyhdtoolkit/utils/printutil.py` & `pyhdtoolkit-1.2.0/pyhdtoolkit/utils/printutil.py`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/.gitignore` & `pyhdtoolkit-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/LICENSE` & `pyhdtoolkit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/README.md` & `pyhdtoolkit-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyhdtoolkit-1.1.1/pyproject.toml` & `pyhdtoolkit-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Utilities",
 ]
 
 dependencies = [
-  "numpy >= 1.21",
+  "numpy >= 1.21,!=1.24",
   "pandas >= 1.4",
   "matplotlib >=3.3",
   "scipy >= 1.6",
   "tfs-pandas >= 3.2",
   "loguru < 1.0",
   "cpymad >= 1.9",
   "rich >= 12.0",
@@ -86,14 +86,15 @@
   "sphinx-rtd-theme >= 1.0",
   "sphinx-issues >= 3.0",
   "sphinx_copybutton < 1.0",
   "sphinxcontrib-bibtex >= 2.4",
   "sphinx-panels < 1.0",
   "sphinx-gallery < 1.0",
   "sphinx-prompt >= 1.5",
+  "sphinx_codeautolink>=0.14",
 ]
 
 [project.urls]
 homepage = "https://github.com/fsoubelet/PyhDToolkit"
 repository = "https://github.com/fsoubelet/PyhDToolkit"
 documentation = "https://fsoubelet.github.io/PyhDToolkit"
 changelog = "https://fsoubelet.github.io/PyhDToolkit/release.html"
@@ -144,14 +145,15 @@
   | \.tox
   | \.venv
   | _build
   | buck-out
   | build
   | dist
   | tests/.*/setup.py
+  | acc-models-lhc
 )/
 '''
 
 [tool.mypy]
 pretty = true
 strict_optional = false
 show_error_codes = true
```

### Comparing `pyhdtoolkit-1.1.1/PKG-INFO` & `pyhdtoolkit-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyhdtoolkit
-Version: 1.1.1
+Version: 1.2.0
 Summary: An all-in-one toolkit package to ease my Python work in my PhD.
 Project-URL: homepage, https://github.com/fsoubelet/PyhDToolkit
 Project-URL: repository, https://github.com/fsoubelet/PyhDToolkit
 Project-URL: documentation, https://fsoubelet.github.io/PyhDToolkit
 Project-URL: changelog, https://fsoubelet.github.io/PyhDToolkit/release.html
 Author-email: Felix Soubelet <felix.soubelet@cern.ch>
+License-Expression: MIT
 License-File: LICENSE
 Keywords: Accelerator Physics,Docker,PHD,Physics Simulation,Visualisation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -23,27 +24,28 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: cpymad>=1.9
 Requires-Dist: loguru<1.0
 Requires-Dist: matplotlib>=3.3
-Requires-Dist: numpy>=1.21
+Requires-Dist: numpy!=1.24,>=1.21
 Requires-Dist: optics-functions>=0.1
 Requires-Dist: pandas>=1.4
 Requires-Dist: pendulum>=2.0
 Requires-Dist: pydantic>=1.0
 Requires-Dist: rich>=12.0
 Requires-Dist: scipy>=1.6
 Requires-Dist: tfs-pandas>=3.2
 Provides-Extra: dev
 Requires-Dist: black>=22.1; extra == 'dev'
 Requires-Dist: isort>=5.10; extra == 'dev'
 Requires-Dist: pylint>=2.4; extra == 'dev'
 Provides-Extra: docs
+Requires-Dist: sphinx-codeautolink>=0.14; extra == 'docs'
 Requires-Dist: sphinx-copybutton<1.0; extra == 'docs'
 Requires-Dist: sphinx-gallery<1.0; extra == 'docs'
 Requires-Dist: sphinx-issues>=3.0; extra == 'docs'
 Requires-Dist: sphinx-panels<1.0; extra == 'docs'
 Requires-Dist: sphinx-prompt>=1.5; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme>=1.0; extra == 'docs'
 Requires-Dist: sphinx>=4.4; extra == 'docs'
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: pyhdtoolkit Version: 1.1.1 Summary: An all-in-one
+Metadata-Version: 2.1 Name: pyhdtoolkit Version: 1.2.0 Summary: An all-in-one
 toolkit package to ease my Python work in my PhD. Project-URL: homepage, https:
 //github.com/fsoubelet/PyhDToolkit Project-URL: repository, https://github.com/
 fsoubelet/PyhDToolkit Project-URL: documentation, https://fsoubelet.github.io/
 PyhDToolkit Project-URL: changelog, https://fsoubelet.github.io/PyhDToolkit/
 release.html Author-email: Felix Soubelet
-soubelet@cern.ch> License-File: LICENSE Keywords: Accelerator
-Physics,Docker,PHD,Physics Simulation,Visualisation Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
-Implementation :: CPython Classifier: Topic :: Scientific/Engineering
+soubelet@cern.ch> License-Expression: MIT License-File: LICENSE Keywords:
+Accelerator Physics,Docker,PHD,Physics Simulation,Visualisation Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
+Research Classifier: License :: OSI Approved :: MIT License Classifier: Natural
+Language :: English Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: Implementation :: CPython Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Scientific/Engineering :: Visualization Classifier: Topic :: Utilities
 Requires-Python: >=3.8 Requires-Dist: cpymad>=1.9 Requires-Dist: loguru<1.0
-Requires-Dist: matplotlib>=3.3 Requires-Dist: numpy>=1.21 Requires-Dist:
+Requires-Dist: matplotlib>=3.3 Requires-Dist: numpy!=1.24,>=1.21 Requires-Dist:
 optics-functions>=0.1 Requires-Dist: pandas>=1.4 Requires-Dist: pendulum>=2.0
 Requires-Dist: pydantic>=1.0 Requires-Dist: rich>=12.0 Requires-Dist:
 scipy>=1.6 Requires-Dist: tfs-pandas>=3.2 Provides-Extra: dev Requires-Dist:
 black>=22.1; extra == 'dev' Requires-Dist: isort>=5.10; extra == 'dev'
 Requires-Dist: pylint>=2.4; extra == 'dev' Provides-Extra: docs Requires-Dist:
-sphinx-copybutton<1.0; extra == 'docs' Requires-Dist: sphinx-gallery<1.0; extra
-== 'docs' Requires-Dist: sphinx-issues>=3.0; extra == 'docs' Requires-Dist:
+sphinx-codeautolink>=0.14; extra == 'docs' Requires-Dist: sphinx-
+copybutton<1.0; extra == 'docs' Requires-Dist: sphinx-gallery<1.0; extra ==
+'docs' Requires-Dist: sphinx-issues>=3.0; extra == 'docs' Requires-Dist:
 sphinx-panels<1.0; extra == 'docs' Requires-Dist: sphinx-prompt>=1.5; extra ==
 'docs' Requires-Dist: sphinx-rtd-theme>=1.0; extra == 'docs' Requires-Dist:
 sphinx>=4.4; extra == 'docs' Requires-Dist: sphinxcontrib-bibtex>=2.4; extra ==
 'docs' Provides-Extra: test Requires-Dist: coverage[toml]>=5.2; extra == 'test'
 Requires-Dist: flaky>=3.5; extra == 'test' Requires-Dist: pytest-cov>=3.0;
 extra == 'test' Requires-Dist: pytest-mpl>=0.12; extra == 'test' Requires-Dist:
 pytest-randomly>=3.3; extra == 'test' Requires-Dist: pytest-xdist>=2.5; extra
```

