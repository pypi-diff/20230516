# Comparing `tmp/pybdei-0.2.tar.gz` & `tmp/pybdei-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybdei-0.2.tar", last modified: Mon Nov  7 11:23:27 2022, max compression
+gzip compressed data, was "pybdei-0.3.tar", last modified: Mon Mar 20 11:16:53 2023, max compression
```

## Comparing `pybdei-0.2.tar` & `pybdei-0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-11-07 11:23:27.000000 pybdei-0.2/
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-11-07 11:23:27.000000 pybdei-0.2/bdei/
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)    55121 2022-11-07 11:13:36.000000 pybdei-0.2/bdei/BDEI.cpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     1053 2022-11-07 10:54:48.000000 pybdei-0.2/bdei/BDEI.hpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     3718 2022-10-04 11:46:46.000000 pybdei-0.2/bdei/pool.hpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)    17217 2022-10-04 11:46:46.000000 pybdei-0.2/bdei/queue.hpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     1745 2022-10-04 11:46:46.000000 pybdei-0.2/bdei/semaphore.hpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     5300 2022-11-07 11:23:27.000000 pybdei-0.2/PKG-INFO
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     2092 2022-11-07 11:05:54.000000 pybdei-0.2/setup.py
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei/
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     9566 2022-11-07 11:13:36.000000 pybdei-0.2/pybdei/__init__.py
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       84 2022-10-04 11:46:46.000000 pybdei-0.2/pybdei/_python.hpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     6639 2022-11-07 11:04:49.000000 pybdei-0.2/pybdei/inference.py
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     1205 2022-10-04 11:46:46.000000 pybdei-0.2/pybdei/_pybdei.hpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     4609 2022-11-07 10:54:48.000000 pybdei-0.2/pybdei/_pybdei.cpp
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     2836 2022-11-07 11:04:49.000000 pybdei-0.2/pybdei/loglikelihood.py
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       59 2022-10-04 11:46:46.000000 pybdei-0.2/MANIFEST.in
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       38 2022-11-07 11:23:27.000000 pybdei-0.2/setup.cfg
-drwxrwxr-x   0 azhukova  (1001) azhukova  (1001)        0 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)      101 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/entry_points.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)      408 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/SOURCES.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     5300 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/PKG-INFO
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       15 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/top_level.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)        1 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/dependency_links.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)       15 2022-11-07 11:23:27.000000 pybdei-0.2/pybdei.egg-info/requires.txt
--rw-rw-r--   0 azhukova  (1001) azhukova  (1001)     4625 2022-10-04 11:46:46.000000 pybdei-0.2/README.md
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-03-20 11:16:53.112319 pybdei-0.3/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       59 2022-12-22 13:19:09.000000 pybdei-0.3/MANIFEST.in
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     5264 2023-03-20 11:16:53.112319 pybdei-0.3/PKG-INFO
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4625 2022-12-22 13:19:09.000000 pybdei-0.3/README.md
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-03-20 11:16:53.112319 pybdei-0.3/bdei/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    55121 2022-12-22 13:19:09.000000 pybdei-0.3/bdei/BDEI.cpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1053 2022-12-22 13:19:09.000000 pybdei-0.3/bdei/BDEI.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3718 2022-12-22 13:19:09.000000 pybdei-0.3/bdei/pool.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)    17217 2022-12-22 13:19:09.000000 pybdei-0.3/bdei/queue.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1745 2022-12-22 13:19:09.000000 pybdei-0.3/bdei/semaphore.hpp
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-03-20 11:16:53.112319 pybdei-0.3/pybdei/
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     9566 2023-03-20 11:13:53.000000 pybdei-0.3/pybdei/__init__.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     4609 2022-12-22 13:19:10.000000 pybdei-0.3/pybdei/_pybdei.cpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     1205 2022-12-22 13:19:10.000000 pybdei-0.3/pybdei/_pybdei.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)       84 2022-12-22 13:19:10.000000 pybdei-0.3/pybdei/_python.hpp
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     6639 2022-12-22 13:19:10.000000 pybdei-0.3/pybdei/inference.py
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     3962 2023-03-20 11:13:53.000000 pybdei-0.3/pybdei/loglikelihood.py
+drwxrwxr-x   0 azhukova  (1000) azhukova  (1000)        0 2023-03-20 11:16:53.112319 pybdei-0.3/pybdei.egg-info/
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)     5264 2023-03-20 11:16:53.000000 pybdei-0.3/pybdei.egg-info/PKG-INFO
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      408 2023-03-20 11:16:53.000000 pybdei-0.3/pybdei.egg-info/SOURCES.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)        1 2023-03-20 11:16:53.000000 pybdei-0.3/pybdei.egg-info/dependency_links.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)      100 2023-03-20 11:16:53.000000 pybdei-0.3/pybdei.egg-info/entry_points.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-03-20 11:16:53.000000 pybdei-0.3/pybdei.egg-info/requires.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       15 2023-03-20 11:16:53.000000 pybdei-0.3/pybdei.egg-info/top_level.txt
+-rw-rw-r--   0 azhukova  (1000) azhukova  (1000)       38 2023-03-20 11:16:53.112319 pybdei-0.3/setup.cfg
+-rwxrwxr-x   0 azhukova  (1000) azhukova  (1000)     2092 2023-03-20 11:13:53.000000 pybdei-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pybdei-0.2/bdei/BDEI.cpp` & `pybdei-0.3/bdei/BDEI.cpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/bdei/BDEI.hpp` & `pybdei-0.3/bdei/BDEI.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/bdei/pool.hpp` & `pybdei-0.3/bdei/pool.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/bdei/queue.hpp` & `pybdei-0.3/bdei/queue.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/bdei/semaphore.hpp` & `pybdei-0.3/bdei/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/PKG-INFO` & `pybdei-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: pybdei
-Version: 0.2
+Version: 0.3
 Summary: Fast and accurate epidemiological parameter estimation from phylogenetic trees with the Birth-Death Exposed-Infectious (BDEI) model.
 Home-page: https://github.com/evolbioinfo/BDEI
+Download-URL: https://github.com/evolbioinfo/BDEI
 Author: Frédéric Heicht
 Author-email: frederic.hecht@sorbonne-universite.fr
 Maintainer: Anna Zhukova
 Maintainer-email: anna.zhukova@pasteur.fr
-License: UNKNOWN
-Download-URL: https://github.com/evolbioinfo/BDEI
 Keywords: BDEI,phylodynamics,epidemiological parameters
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # PyBDEI
@@ -119,8 +117,7 @@
 print('Inferred transmission rate is', result.la, result.la_CI)
 print('Inferred removal rate is', result.psi, result.psi_CI)
 print('Inferred reproductive number is', result.R_naught)
 print('Inferred incubation period is', result.incubation_period)
 print('Inferred infectious time is', result.infectious_time)
 print('Converged in', time.CPU_time, 's and', time.iterations, 'iterations')
 ```
-
```

### Comparing `pybdei-0.2/setup.py` & `pybdei-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ],
     packages=find_packages(),
     install_requires=['numpy', 'ete3', 'six'],
     setup_requires=['numpy'],
     include_package_data=True,
     package_data={'pybdei': ['*.hpp'],
                   'bdei': ['*.hpp']},
-    version='0.2',
+    version='0.3',
     description='Fast and accurate epidemiological parameter estimation from phylogenetic trees with the Birth-Death Exposed-Infectious (BDEI) model.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Frédéric Heicht',
     author_email='frederic.hecht@sorbonne-universite.fr',
     maintainer='Anna Zhukova',
     maintainer_email='anna.zhukova@pasteur.fr',
```

### Comparing `pybdei-0.2/pybdei/__init__.py` & `pybdei-0.3/pybdei/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ete3 import Tree
 
 ERRORS = 0
 WARNINGS = 1
 INFO = 2
 DEBUG = 3
 
-PYBDEI_VERSION = 0.2
+PYBDEI_VERSION = 0.3
 
 PS = (0.1, 0.4, 0.7)
 
 BDEI_result = namedtuple('BDEI_result', ['mu', 'la', 'psi', 'p', 'mu_CI', 'la_CI', 'psi_CI', 'p_CI',
                                          'R_naught', 'incubation_period', 'infectious_time'])
 BDEI_time = namedtuple('BDEI_time', ['CPU_time', 'iterations'])
```

### Comparing `pybdei-0.2/pybdei/inference.py` & `pybdei-0.3/pybdei/inference.py`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/pybdei/_pybdei.hpp` & `pybdei-0.3/pybdei/_pybdei.hpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/pybdei/_pybdei.cpp` & `pybdei-0.3/pybdei/_pybdei.cpp`

 * *Files identical despite different names*

### Comparing `pybdei-0.2/pybdei/loglikelihood.py` & `pybdei-0.3/pybdei/loglikelihood.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pybdei import get_loglikelihood, ERRORS, WARNINGS, INFO, DEBUG
+from pybdei import get_loglikelihood, ERRORS, WARNINGS, INFO, DEBUG, PYBDEI_VERSION
 
 
 def main():
     """
     Entry point, calling :py:func:`pydbei.infer` with command-line arguments.
     :return: void
     """
@@ -29,14 +29,26 @@
     parameter_group.add_argument('-p', '--p', required=True, type=float, default=None,
                                   help="Value to fix BDEI sampling probability. "
                                        "If not given, will be estimated.")
     parameter_group.add_argument('--pi_E', required=False, type=float, default=-1,
                                  help="Frequency of E at time 0, "
                                       "should be between 0 and 1. "
                                       "If not given, will be estimated from the model parameters.")
+    parameter_group.add_argument('--T', default=0, type=float,
+                                  help="Total time between the tree roots and the end of the epidemic "
+                                       "(to be given if all trees start at the same time). "
+                                       "If a positive value is given, the total time will be set to the maximum "
+                                       "between this value and the maximal time between the start "
+                                       "and the last sampled tip of all the trees. "
+                                       "If a zero or negative value is given, the time will be tree-specific "
+                                       "and estimated as the time between the root "
+                                       "and the last sampled tip for each tree."
+                                       "Note that if the number of unobserved trees (u) is given, "
+                                       "all the trees are assumed to have started at the same time, "
+                                       "hence T must be non-negative.")
     parser.add_argument('--log_level',
                         help="level of logging information "
                              "(the lower, the less information will be printed to the output). "
                              "Possible levels are: {} (errors only), {} (errors+warnings), {} (errors+warnings+info), "
                              "{} (errors+warnings+info+debug).".format(ERRORS, WARNINGS, INFO, DEBUG), type=int,
                         default=INFO)
     parser.add_argument('-v', '--version', action='version', version='%(prog)s {version}'.format(version=PYBDEI_VERSION))
```

### Comparing `pybdei-0.2/pybdei.egg-info/PKG-INFO` & `pybdei-0.3/pybdei.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: pybdei
-Version: 0.2
+Version: 0.3
 Summary: Fast and accurate epidemiological parameter estimation from phylogenetic trees with the Birth-Death Exposed-Infectious (BDEI) model.
 Home-page: https://github.com/evolbioinfo/BDEI
+Download-URL: https://github.com/evolbioinfo/BDEI
 Author: Frédéric Heicht
 Author-email: frederic.hecht@sorbonne-universite.fr
 Maintainer: Anna Zhukova
 Maintainer-email: anna.zhukova@pasteur.fr
-License: UNKNOWN
-Download-URL: https://github.com/evolbioinfo/BDEI
 Keywords: BDEI,phylodynamics,epidemiological parameters
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # PyBDEI
@@ -119,8 +117,7 @@
 print('Inferred transmission rate is', result.la, result.la_CI)
 print('Inferred removal rate is', result.psi, result.psi_CI)
 print('Inferred reproductive number is', result.R_naught)
 print('Inferred incubation period is', result.incubation_period)
 print('Inferred infectious time is', result.infectious_time)
 print('Converged in', time.CPU_time, 's and', time.iterations, 'iterations')
 ```
-
```

### Comparing `pybdei-0.2/README.md` & `pybdei-0.3/README.md`

 * *Files identical despite different names*

