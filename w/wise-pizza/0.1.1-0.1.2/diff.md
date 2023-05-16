# Comparing `tmp/wise-pizza-0.1.1.tar.gz` & `tmp/wise-pizza-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wise-pizza-0.1.1.tar", last modified: Mon May 15 17:04:32 2023, max compression
+gzip compressed data, was "wise-pizza-0.1.2.tar", last modified: Tue May 16 08:39:14 2023, max compression
```

## Comparing `wise-pizza-0.1.1.tar` & `wise-pizza-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-15 17:04:32.567055 wise-pizza-0.1.1/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10839 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/LICENSE
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5744 2023-05-15 17:04:32.566838 wise-pizza-0.1.1/PKG-INFO
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5218 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/README.md
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/pyproject.toml
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-15 17:04:32.567110 wise-pizza-0.1.1/setup.cfg
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-15 17:04:07.000000 wise-pizza-0.1.1/setup.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-15 17:04:32.565073 wise-pizza-0.1.1/wise_pizza/
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/__init__.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11404 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/explain.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/find_alpha.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/make_matrix.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/plotting.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/segment_data.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/slicer.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/solver.py
--rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-15 16:22:40.000000 wise-pizza-0.1.1/wise_pizza/utils.py
-drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-15 17:04:32.566360 wise-pizza-0.1.1/wise_pizza.egg-info/
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5744 2023-05-15 17:04:32.000000 wise-pizza-0.1.1/wise_pizza.egg-info/PKG-INFO
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-15 17:04:32.000000 wise-pizza-0.1.1/wise_pizza.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-15 17:04:32.000000 wise-pizza-0.1.1/wise_pizza.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-15 17:04:32.000000 wise-pizza-0.1.1/wise_pizza.egg-info/requires.txt
--rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-15 17:04:32.000000 wise-pizza-0.1.1/wise_pizza.egg-info/top_level.txt
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-16 08:39:14.928177 wise-pizza-0.1.2/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    10832 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/LICENSE
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5960 2023-05-16 08:39:14.927897 wise-pizza-0.1.2/PKG-INFO
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     5434 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/README.md
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      220 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/pyproject.toml
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       38 2023-05-16 08:39:14.928259 wise-pizza-0.1.2/setup.cfg
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     1232 2023-05-16 08:33:11.000000 wise-pizza-0.1.2/setup.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-16 08:39:14.920141 wise-pizza-0.1.2/wise_pizza/
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      118 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/__init__.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)    11404 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/explain.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7249 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/find_alpha.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     3799 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/make_matrix.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8974 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/plotting.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)      518 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/segment_data.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     7689 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/slicer.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     4005 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/solver.py
+-rw-rw-r--   0 alexander.polyakov   (503) staff       (20)     8527 2023-05-16 08:30:42.000000 wise-pizza-0.1.2/wise_pizza/utils.py
+drwxr-xr-x   0 alexander.polyakov   (503) staff       (20)        0 2023-05-16 08:39:14.927497 wise-pizza-0.1.2/wise_pizza.egg-info/
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)     5960 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      418 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)        1 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)      132 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/requires.txt
+-rw-r--r--   0 alexander.polyakov   (503) staff       (20)       11 2023-05-16 08:39:14.000000 wise-pizza-0.1.2/wise_pizza.egg-info/top_level.txt
```

### Comparing `wise-pizza-0.1.1/LICENSE` & `wise-pizza-0.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,20 +182,20 @@
    replaced with your own identifying information. (Don't include
    the brackets!)  The text should be enclosed in the appropriate
    comment syntax for the file format. We also recommend that a
    file or class name and description of purpose be included on the
    same "printed page" as the copyright notice for easier
    identification within third-party archives.
 
-Copyright 2023 TransferWise Ltd.
+Copyright 2023 Wise Plc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
-limitations under the License.
+limitations under the License.
```

### Comparing `wise-pizza-0.1.1/PKG-INFO` & `wise-pizza-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Wise Pizza: A library for automated figuring out most unusual segments
 
+<img src="./docs/Wise_Logo.png" width=50% height=50%>
+
 **WisePizza** is a library to find and visualise the most interesting slices in multidimensional data based on Lasso and LP solvers, which provides different functions to find segments whose average is most different from the global one or find segments most useful in explaining the difference between two datasets.
 
 ## The approach
 WisePizza assumes you have a dataset with a number of discrete *dimensions* (could be currency, region, etc). For each
 combination of dimensions, the dataset must have a *total* value (total of the metric over that segment, for example
 the total volume in that region and currency), and an optional *size* value (set to 1 if not specified), this could for
 example be the total number of customers for that region and currency. The *average* value of the outcome for the segment
@@ -59,28 +61,32 @@
 
 
 ### 2. Understanding differences in two time periods or two dataframes
 If you have two time periods or two datasets, you can find segments that experience the largest change in the totals from previous period/dataset.
 
 
 ## Installation
-From the command line:
+You can always get the newest *wise_pizza* release using ``pip``:
+https://pypi.org/project/wise-pizza/
+```
+pip install wise-pizza
+```
+
+From the command line (another way):
 ```
 pip install git+https://github.com/transferwise/wise-pizza.git
 ```
 
-From Jupyter notebook:
+From Jupyter notebook (another way):
 ```
 !pip install git+https://github.com/transferwise/wise-pizza.git
 ```
 
 Or you can clone and run from source, in which case you should `pip -r requirements.txt` before running.
 
-A deployment to PyPi, to allow you to just *pip install wise-pizza* is coming soon!
-
 ## Quick Start
 The wisepizza package can be used for finding segments with unusual average:
 
 ```Python
 sf = explain_levels(
     df=data,
     dims=dims,
@@ -140,9 +146,13 @@
 
 ```Python
 sf.segments
 ```
 Please see the full example [here](https://github.com/transferwise/wise-pizza/blob/main/notebooks/Finding%20interesting%20segments.ipynb)
 
 ## For Developers
+
+
+Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.
+
 ### Testing
 We use [PyTest](https://docs.pytest.org/) for testing. If you want to contribute code, make sure that the tests in tests/ run without errors.
```

### Comparing `wise-pizza-0.1.1/README.md` & `wise-pizza-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Wise Pizza: A library for automated figuring out most unusual segments
 
+<img src="./docs/Wise_Logo.png" width=50% height=50%>
+
 **WisePizza** is a library to find and visualise the most interesting slices in multidimensional data based on Lasso and LP solvers, which provides different functions to find segments whose average is most different from the global one or find segments most useful in explaining the difference between two datasets.
 
 ## The approach
 WisePizza assumes you have a dataset with a number of discrete *dimensions* (could be currency, region, etc). For each
 combination of dimensions, the dataset must have a *total* value (total of the metric over that segment, for example
 the total volume in that region and currency), and an optional *size* value (set to 1 if not specified), this could for
 example be the total number of customers for that region and currency. The *average* value of the outcome for the segment
@@ -44,28 +46,32 @@
 
 
 ### 2. Understanding differences in two time periods or two dataframes
 If you have two time periods or two datasets, you can find segments that experience the largest change in the totals from previous period/dataset.
 
 
 ## Installation
-From the command line:
+You can always get the newest *wise_pizza* release using ``pip``:
+https://pypi.org/project/wise-pizza/
+```
+pip install wise-pizza
+```
+
+From the command line (another way):
 ```
 pip install git+https://github.com/transferwise/wise-pizza.git
 ```
 
-From Jupyter notebook:
+From Jupyter notebook (another way):
 ```
 !pip install git+https://github.com/transferwise/wise-pizza.git
 ```
 
 Or you can clone and run from source, in which case you should `pip -r requirements.txt` before running.
 
-A deployment to PyPi, to allow you to just *pip install wise-pizza* is coming soon!
-
 ## Quick Start
 The wisepizza package can be used for finding segments with unusual average:
 
 ```Python
 sf = explain_levels(
     df=data,
     dims=dims,
@@ -125,9 +131,13 @@
 
 ```Python
 sf.segments
 ```
 Please see the full example [here](https://github.com/transferwise/wise-pizza/blob/main/notebooks/Finding%20interesting%20segments.ipynb)
 
 ## For Developers
+
+
+Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.
+
 ### Testing
 We use [PyTest](https://docs.pytest.org/) for testing. If you want to contribute code, make sure that the tests in tests/ run without errors.
```

### Comparing `wise-pizza-0.1.1/setup.py` & `wise-pizza-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="wise-pizza",
-    version="0.1.1",
+    version="0.1.2",
     description="A library to find and visualise the most interesting slices in multidimensional data",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Wise",
     url='https://github.com/transferwise/wise-pizza',
     classifiers=[
         'Programming Language :: Python :: 3 :: Only',
```

### Comparing `wise-pizza-0.1.1/wise_pizza/explain.py` & `wise-pizza-0.1.2/wise_pizza/explain.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/find_alpha.py` & `wise-pizza-0.1.2/wise_pizza/find_alpha.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/make_matrix.py` & `wise-pizza-0.1.2/wise_pizza/make_matrix.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/plotting.py` & `wise-pizza-0.1.2/wise_pizza/plotting.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/segment_data.py` & `wise-pizza-0.1.2/wise_pizza/segment_data.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/slicer.py` & `wise-pizza-0.1.2/wise_pizza/slicer.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/solver.py` & `wise-pizza-0.1.2/wise_pizza/solver.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza/utils.py` & `wise-pizza-0.1.2/wise_pizza/utils.py`

 * *Files identical despite different names*

### Comparing `wise-pizza-0.1.1/wise_pizza.egg-info/PKG-INFO` & `wise-pizza-0.1.2/wise_pizza.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: wise-pizza
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to find and visualise the most interesting slices in multidimensional data
 Home-page: https://github.com/transferwise/wise-pizza
 Author: Wise
 Keywords: wise-pizza
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Wise Pizza: A library for automated figuring out most unusual segments
 
+<img src="./docs/Wise_Logo.png" width=50% height=50%>
+
 **WisePizza** is a library to find and visualise the most interesting slices in multidimensional data based on Lasso and LP solvers, which provides different functions to find segments whose average is most different from the global one or find segments most useful in explaining the difference between two datasets.
 
 ## The approach
 WisePizza assumes you have a dataset with a number of discrete *dimensions* (could be currency, region, etc). For each
 combination of dimensions, the dataset must have a *total* value (total of the metric over that segment, for example
 the total volume in that region and currency), and an optional *size* value (set to 1 if not specified), this could for
 example be the total number of customers for that region and currency. The *average* value of the outcome for the segment
@@ -59,28 +61,32 @@
 
 
 ### 2. Understanding differences in two time periods or two dataframes
 If you have two time periods or two datasets, you can find segments that experience the largest change in the totals from previous period/dataset.
 
 
 ## Installation
-From the command line:
+You can always get the newest *wise_pizza* release using ``pip``:
+https://pypi.org/project/wise-pizza/
+```
+pip install wise-pizza
+```
+
+From the command line (another way):
 ```
 pip install git+https://github.com/transferwise/wise-pizza.git
 ```
 
-From Jupyter notebook:
+From Jupyter notebook (another way):
 ```
 !pip install git+https://github.com/transferwise/wise-pizza.git
 ```
 
 Or you can clone and run from source, in which case you should `pip -r requirements.txt` before running.
 
-A deployment to PyPi, to allow you to just *pip install wise-pizza* is coming soon!
-
 ## Quick Start
 The wisepizza package can be used for finding segments with unusual average:
 
 ```Python
 sf = explain_levels(
     df=data,
     dims=dims,
@@ -140,9 +146,13 @@
 
 ```Python
 sf.segments
 ```
 Please see the full example [here](https://github.com/transferwise/wise-pizza/blob/main/notebooks/Finding%20interesting%20segments.ipynb)
 
 ## For Developers
+
+
+Wise-pizza is open sourced and maintained by Wise Plc. Copyright 2023 Wise Plc.
+
 ### Testing
 We use [PyTest](https://docs.pytest.org/) for testing. If you want to contribute code, make sure that the tests in tests/ run without errors.
```

