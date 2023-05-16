# Comparing `tmp/xrdfit-1.2.0.tar.gz` & `tmp/xrdfit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrdfit-1.2.0.tar", last modified: Wed Dec 15 01:09:14 2021, max compression
+gzip compressed data, was "xrdfit-1.3.0.tar", last modified: Tue May 16 15:36:35 2023, max compression
```

## Comparing `xrdfit-1.2.0.tar` & `xrdfit-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.791807 xrdfit-1.2.0/
--rw-rw-rw-   0        0        0      367 2020-07-29 22:14:38.000000 xrdfit-1.2.0/.gitignore
--rw-rw-rw-   0        0        0     3434 2020-07-29 22:14:38.000000 xrdfit-1.2.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1437 2020-03-12 15:57:54.000000 xrdfit-1.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35823 2020-03-10 18:55:35.000000 xrdfit-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3922 2021-12-15 01:09:14.791807 xrdfit-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3356 2020-11-05 16:50:41.000000 xrdfit-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.638061 xrdfit-1.2.0/docs/
--rw-rw-rw-   0        0        0     1130 2020-03-10 18:55:35.000000 xrdfit-1.2.0/docs/README.md
--rw-rw-rw-   0        0        0       64 2020-03-10 18:55:35.000000 xrdfit-1.2.0/docs/index.html
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.653688 xrdfit-1.2.0/docs/source/
--rw-rw-rw-   0        0        0     2486 2021-12-15 01:03:41.000000 xrdfit-1.2.0/docs/source/conf.py
--rw-rw-rw-   0        0        0     4460 2020-11-05 16:50:41.000000 xrdfit-1.2.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       62 2020-03-10 18:55:35.000000 xrdfit-1.2.0/docs/source/modules.rst
--rw-rw-rw-   0        0        0      478 2020-03-12 15:57:54.000000 xrdfit-1.2.0/docs/source/xrdfit.rst
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.707100 xrdfit-1.2.0/example_data/
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00001.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00002.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00003.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00004.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00005.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00006.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00007.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00008.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00009.dat
--rw-rw-rw-   0        0        0   381114 2020-03-10 18:55:35.000000 xrdfit-1.2.0/example_data/adc_041_7Nb_NDload_700C_15mms_00010.dat
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.707100 xrdfit-1.2.0/example_data/instrument_data/
--rw-rw-rw-   0        0        0   194998 2020-03-12 15:57:54.000000 xrdfit-1.2.0/example_data/instrument_data/065_ETMT_data.txt
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.738355 xrdfit-1.2.0/paper/
--rw-rw-rw-   0        0        0  5410310 2020-07-29 22:14:38.000000 xrdfit-1.2.0/paper/figure1.eps
--rw-rw-rw-   0        0        0    65900 2020-11-05 16:50:41.000000 xrdfit-1.2.0/paper/figure2.eps
--rw-rw-rw-   0        0        0    13590 2021-12-10 11:27:30.000000 xrdfit-1.2.0/paper/paper.bib
--rw-rw-rw-   0        0        0     5434 2021-12-10 11:27:30.000000 xrdfit-1.2.0/paper/paper.md
--rw-rw-rw-   0        0        0      252 2020-03-10 18:55:35.000000 xrdfit-1.2.0/readthedocs.yaml
--rw-rw-rw-   0        0        0       74 2021-12-15 01:00:15.000000 xrdfit-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-12-15 01:09:14.791807 xrdfit-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1056 2021-12-15 01:04:04.000000 xrdfit-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.753972 xrdfit-1.2.0/tutorial notebooks/
--rw-rw-rw-   0        0        0    32025 2021-12-15 01:00:15.000000 xrdfit-1.2.0/tutorial notebooks/1 - Basic analysis workflow.ipynb
--rw-rw-rw-   0        0        0     8590 2021-12-10 15:09:56.000000 xrdfit-1.2.0/tutorial notebooks/2 - Analysis of multiple cakes.ipynb
--rw-rw-rw-   0        0        0    17228 2021-12-10 15:09:56.000000 xrdfit-1.2.0/tutorial notebooks/3 - Fitting peaks over time.ipynb
--rw-rw-rw-   0        0        0    37963 2021-12-10 15:09:56.000000 xrdfit-1.2.0/tutorial notebooks/4 - Working with larger data sets.ipynb
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.753972 xrdfit-1.2.0/tutorial notebooks/images/
--rw-rw-rw-   0        0        0    11979 2020-03-10 18:55:35.000000 xrdfit-1.2.0/tutorial notebooks/images/averaging_areas.svg
--rw-rw-rw-   0        0        0    11042 2020-03-10 18:55:35.000000 xrdfit-1.2.0/tutorial notebooks/images/cake_numbering.svg
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.776141 xrdfit-1.2.0/xrdfit/
--rw-rw-rw-   0        0        0        0 2020-03-10 18:55:35.000000 xrdfit-1.2.0/xrdfit/__init__.py
--rw-rw-rw-   0        0        0     9992 2020-11-05 16:50:41.000000 xrdfit-1.2.0/xrdfit/plotting.py
--rw-rw-rw-   0        0        0     6375 2020-07-29 22:14:38.000000 xrdfit-1.2.0/xrdfit/pv_fit.py
--rw-rw-rw-   0        0        0    38390 2021-12-15 01:00:15.000000 xrdfit-1.2.0/xrdfit/spectrum_fitting.py
--rw-rw-rw-   0        0        0      555 2021-12-10 14:03:56.000000 xrdfit-1.2.0/xrdfit/test.py
-drwxrwxrwx   0        0        0        0 2021-12-15 01:09:14.776141 xrdfit-1.2.0/xrdfit.egg-info/
--rw-rw-rw-   0        0        0     3922 2021-12-15 01:09:14.000000 xrdfit-1.2.0/xrdfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2021-12-15 01:09:14.000000 xrdfit-1.2.0/xrdfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-15 01:09:14.000000 xrdfit-1.2.0/xrdfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2021-12-15 01:09:14.000000 xrdfit-1.2.0/xrdfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-12-15 01:09:14.000000 xrdfit-1.2.0/xrdfit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 15:36:35.062644 xrdfit-1.3.0/
+-rw-rw-rw-   0        0        0    35823 2022-11-24 20:44:03.000000 xrdfit-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3525 2023-05-16 15:36:35.062644 xrdfit-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3000 2023-05-16 15:31:18.000000 xrdfit-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 15:36:35.062644 xrdfit-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-05-16 15:30:24.000000 xrdfit-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:36:35.056643 xrdfit-1.3.0/xrdfit/
+-rw-rw-rw-   0        0        0        0 2022-11-24 20:44:03.000000 xrdfit-1.3.0/xrdfit/__init__.py
+-rw-rw-rw-   0        0        0     9992 2022-11-24 20:44:03.000000 xrdfit-1.3.0/xrdfit/plotting.py
+-rw-rw-rw-   0        0        0     6378 2023-05-16 14:12:59.000000 xrdfit-1.3.0/xrdfit/pv_fit.py
+-rw-rw-rw-   0        0        0    38403 2022-11-24 20:44:03.000000 xrdfit-1.3.0/xrdfit/spectrum_fitting.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:36:35.061643 xrdfit-1.3.0/xrdfit.egg-info/
+-rw-rw-rw-   0        0        0     3525 2023-05-16 15:36:35.000000 xrdfit-1.3.0/xrdfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-16 15:36:35.000000 xrdfit-1.3.0/xrdfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:36:35.000000 xrdfit-1.3.0/xrdfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-05-16 15:36:35.000000 xrdfit-1.3.0/xrdfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 15:36:35.000000 xrdfit-1.3.0/xrdfit.egg-info/top_level.txt
```

### Comparing `xrdfit-1.2.0/LICENSE` & `xrdfit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xrdfit-1.2.0/PKG-INFO` & `xrdfit-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: xrdfit
-Version: 1.2.0
+Version: 1.3.0
 Summary: Automated fitting of XRD peaks using Pseudo-Voight fits
 Home-page: https://github.com/LightForm-group/xrdfit
 Author: Peter Crowther, Christopher Daniel
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: documentation_compilation
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/xrdfit.svg)](https://badge.fury.io/py/xrdfit)
 [![Documentation Status](https://readthedocs.org/projects/xrdfit/badge/?version=latest)](https://xrdfit.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/203145007.svg)](https://zenodo.org/badge/latestdoi/203145007)
@@ -52,17 +50,15 @@
 You can try out `xrdfit` directly in your browser with Binder by clicking [here](https://mybinder.org/v2/gh/LightForm-group/xrdfit/master).
 
 Note that `Tutorial Notebook 4` will not run correctly in Binder as it requires the download of a [supplementary dataset](https://zenodo.org/record/3630511#.XjHhJGj7SUl) which is not included in the source repository due to its size.
 
 Compatibility
 --------------
 
-The code was developed and tested with Python version 3.8. The minimum required Python version is 3.6. If you install the dependencies of xrdfit using the 
-specification in requirements.txt, this will use the same package versions used by the developers. While this is good for reproducibility, it is worth noting that
-if you are using a newer Python version (> 3.8), some of these packages may not have binary wheels for your version and may require compilation.
+The latest version of xrdfit was tested with Python version 3.10. The minimum required Python version is 3.7.
 
 Required libraries
 --------------------
 
 This module uses the Python libraries:
 * [NumPy](https://numpy.org/)
 * [matplotlib](https://matplotlib.org/)
@@ -70,9 +66,7 @@
 * [dill](https://pypi.org/project/dill/)
 * [tqdm ](https://tqdm.github.io/)
 * [SciPy](https://www.scipy.org/)
 * [lmfit](https://lmfit.github.io/lmfit-py/)
 
 The following libraries are required to use the tutorial documentation workbooks:
 * [Jupyter](https://jupyter.org/)
-
-
```

### Comparing `xrdfit-1.2.0/README.md` & `xrdfit-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,17 +36,15 @@
 You can try out `xrdfit` directly in your browser with Binder by clicking [here](https://mybinder.org/v2/gh/LightForm-group/xrdfit/master).
 
 Note that `Tutorial Notebook 4` will not run correctly in Binder as it requires the download of a [supplementary dataset](https://zenodo.org/record/3630511#.XjHhJGj7SUl) which is not included in the source repository due to its size.
 
 Compatibility
 --------------
 
-The code was developed and tested with Python version 3.8. The minimum required Python version is 3.6. If you install the dependencies of xrdfit using the 
-specification in requirements.txt, this will use the same package versions used by the developers. While this is good for reproducibility, it is worth noting that
-if you are using a newer Python version (> 3.8), some of these packages may not have binary wheels for your version and may require compilation.
+The latest version of xrdfit was tested with Python version 3.10. The minimum required Python version is 3.7.
 
 Required libraries
 --------------------
 
 This module uses the Python libraries:
 * [NumPy](https://numpy.org/)
 * [matplotlib](https://matplotlib.org/)
```

### Comparing `xrdfit-1.2.0/setup.py` & `xrdfit-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='xrdfit',
-    version='1.2.0',
+    version='1.3.0',
     description='Automated fitting of XRD peaks using Pseudo-Voight fits',
     author='Peter Crowther, Christopher Daniel',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LightForm-group/xrdfit",
     packages=find_packages(),
     install_requires=['numpy',
@@ -23,9 +23,9 @@
                       ],
     extras_require={"documentation_compilation": "sphinx"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
-)
+    python_requires='>=3.7',
+)
```

### Comparing `xrdfit-1.2.0/xrdfit/plotting.py` & `xrdfit-1.3.0/xrdfit/plotting.py`

 * *Files identical despite different names*

### Comparing `xrdfit-1.2.0/xrdfit/pv_fit.py` & `xrdfit-1.3.0/xrdfit/pv_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # Add one peak to the model for each maximum
     for maxima_num in range(num_maxima):
         prefix = f"maximum_{maxima_num}_"
         if model:
             model += lmfit.models.PseudoVoigtModel(prefix=prefix)
         else:
             model = lmfit.models.PseudoVoigtModel(prefix=prefix)
-    model += lmfit.Model(lambda background: background)
+    model += lmfit.Model(lambda x, background: background)
 
     two_theta = peak_data[:, 0]
     intensity = peak_data[:, 1]
 
     new_fit_parameters = guess_params(model, peak_param.previous_fit_parameters, two_theta,
                                       intensity, peak_param.maxima)
     # We can't use special characters in param names so have to save the user provided
```

### Comparing `xrdfit-1.2.0/xrdfit/spectrum_fitting.py` & `xrdfit-1.3.0/xrdfit/spectrum_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 
         self.first_cake_angle = first_cake_angle
         self.cake_order = cake_order
         self.fitted_peaks: List[PeakFit] = []
         self.num_evaluations = {}
         self.fit_time = {}
 
-        self.spectral_data = pd.read_table(file_path, delimiter=delimiter).to_numpy()
+        self.spectral_data = pd.read_table(file_path, delimiter=delimiter, header=None).to_numpy()
 
     def __str__(self):
         return f"FitSpectrum with {self.num_cakes} cakes. " \
                f"Num fitted peaks: {len(self.fitted_peaks)}"
 
     def __repr__(self):
         return f'<{str(self)}>'
```

### Comparing `xrdfit-1.2.0/xrdfit.egg-info/PKG-INFO` & `xrdfit-1.3.0/xrdfit.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: xrdfit
-Version: 1.2.0
+Version: 1.3.0
 Summary: Automated fitting of XRD peaks using Pseudo-Voight fits
 Home-page: https://github.com/LightForm-group/xrdfit
 Author: Peter Crowther, Christopher Daniel
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: documentation_compilation
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/xrdfit.svg)](https://badge.fury.io/py/xrdfit)
 [![Documentation Status](https://readthedocs.org/projects/xrdfit/badge/?version=latest)](https://xrdfit.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/203145007.svg)](https://zenodo.org/badge/latestdoi/203145007)
@@ -52,17 +50,15 @@
 You can try out `xrdfit` directly in your browser with Binder by clicking [here](https://mybinder.org/v2/gh/LightForm-group/xrdfit/master).
 
 Note that `Tutorial Notebook 4` will not run correctly in Binder as it requires the download of a [supplementary dataset](https://zenodo.org/record/3630511#.XjHhJGj7SUl) which is not included in the source repository due to its size.
 
 Compatibility
 --------------
 
-The code was developed and tested with Python version 3.8. The minimum required Python version is 3.6. If you install the dependencies of xrdfit using the 
-specification in requirements.txt, this will use the same package versions used by the developers. While this is good for reproducibility, it is worth noting that
-if you are using a newer Python version (> 3.8), some of these packages may not have binary wheels for your version and may require compilation.
+The latest version of xrdfit was tested with Python version 3.10. The minimum required Python version is 3.7.
 
 Required libraries
 --------------------
 
 This module uses the Python libraries:
 * [NumPy](https://numpy.org/)
 * [matplotlib](https://matplotlib.org/)
@@ -70,9 +66,7 @@
 * [dill](https://pypi.org/project/dill/)
 * [tqdm ](https://tqdm.github.io/)
 * [SciPy](https://www.scipy.org/)
 * [lmfit](https://lmfit.github.io/lmfit-py/)
 
 The following libraries are required to use the tutorial documentation workbooks:
 * [Jupyter](https://jupyter.org/)
-
-
```

