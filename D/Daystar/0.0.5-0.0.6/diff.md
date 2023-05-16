# Comparing `tmp/Daystar-0.0.5.tar.gz` & `tmp/Daystar-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Daystar-0.0.5.tar", last modified: Tue May 16 19:40:08 2023, max compression
+gzip compressed data, was "Daystar-0.0.6.tar", last modified: Tue May 16 20:36:13 2023, max compression
```

## Comparing `Daystar-0.0.5.tar` & `Daystar-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:40:08.349299 Daystar-0.0.5/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:40:08.349299 Daystar-0.0.5/Daystar/
--rw-r--r--   0 runner    (1000) runner    (1000)     1391 2023-05-16 19:39:32.000000 Daystar-0.0.5/Daystar/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:40:08.349299 Daystar-0.0.5/Daystar.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1418 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-05-16 03:18:05.000000 Daystar-0.0.5/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1418 2023-05-16 19:40:08.349299 Daystar-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-05-16 19:39:23.000000 Daystar-0.0.5/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Daystar-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-16 19:40:08.349299 Daystar-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      658 2023-05-16 19:39:46.000000 Daystar-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 20:36:13.739254 Daystar-0.0.6/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 20:36:13.735254 Daystar-0.0.6/Daystar/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1391 2023-05-16 19:39:32.000000 Daystar-0.0.6/Daystar/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 20:36:13.739254 Daystar-0.0.6/Daystar.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1477 2023-05-16 20:36:13.000000 Daystar-0.0.6/Daystar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-05-16 20:36:13.000000 Daystar-0.0.6/Daystar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-16 20:36:13.000000 Daystar-0.0.6/Daystar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-16 20:36:13.000000 Daystar-0.0.6/Daystar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-05-16 20:36:13.000000 Daystar-0.0.6/Daystar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-05-16 03:18:05.000000 Daystar-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1477 2023-05-16 20:36:13.739254 Daystar-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1083 2023-05-16 20:35:52.000000 Daystar-0.0.6/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Daystar-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-16 20:36:13.739254 Daystar-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      648 2023-05-16 20:34:13.000000 Daystar-0.0.6/setup.py
```

### Comparing `Daystar-0.0.5/Daystar/__init__.py` & `Daystar-0.0.6/Daystar/__init__.py`

 * *Files identical despite different names*

### Comparing `Daystar-0.0.5/Daystar.egg-info/PKG-INFO` & `Daystar-0.0.6/Daystar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Daystar
-Version: 0.0.5
-Summary: Sun calculation class from Solarflare module
+Version: 0.0.6
+Summary: Solar calculation class for Python
 Author: Siddhu Pendyala
 Author-email: siddhu.pendyala@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -13,23 +13,24 @@
 
 # Daystar
 Daystar is a python library that provides a convenient class for Solar calculations based off of my other library _Solarflare_. Check out Solarflare at https://pypi.org/project/Solarflare/
 
 In order to use this library, just create an instance of the daystar class:
 
 ```python
+from Daystar import *
 sun = Daystar(latitude, longitude)
 ```
 
 The functions provided are (they all default to datetime.datetime.now()):
-  - risetime(date): returns the sunrise
-  - settime(date): returns the sunset
-  - solarnoon(date): returns the solar noon time
-  - hrangle(date): returns the hour angle for the time and date
-  - coordinates(date): returns a tuple with declination and right ascension
-  - mean(date): returns the mean anomaly
-  - true(date): returns the true anomaly
-  - ceq(date): returns the equation of center
-  - solar_julian(date): returns "rise" and "set" dictionary with sunrise and sunset julian dates
-  - alt(date): returns solar altitude
-  - azi(date): returns the solar azimuth
-  - nadir(date): returns the time of nadir
+  - `risetime(date)`: returns the sunrise 
+  - `settime(date)`: returns the sunset
+  - `solarnoon(date)`: returns the solar noon time
+  - `hrangle(date)`: returns the hour angle for the time and date
+  - `coordinates(date)`: returns a dictionary with declination and right ascension ("dec" and "ra")
+  - `mean(date)`: returns the mean anomaly
+  - `true(date)`: returns the true anomaly
+  - `ceq(date)`: returns the equation of center
+  - `solar_julian(date)`: returns "rise" and "set" dictionary with sunrise and sunset julian dates
+  - `alt(date)`: returns solar altitude
+  - `azi(date)`: returns the solar azimuth
+  - `nadir(date)`: returns the time of nadir
```

### Comparing `Daystar-0.0.5/LICENSE` & `Daystar-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Daystar-0.0.5/PKG-INFO` & `Daystar-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Daystar
-Version: 0.0.5
-Summary: Sun calculation class from Solarflare module
+Version: 0.0.6
+Summary: Solar calculation class for Python
 Author: Siddhu Pendyala
 Author-email: siddhu.pendyala@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -13,23 +13,24 @@
 
 # Daystar
 Daystar is a python library that provides a convenient class for Solar calculations based off of my other library _Solarflare_. Check out Solarflare at https://pypi.org/project/Solarflare/
 
 In order to use this library, just create an instance of the daystar class:
 
 ```python
+from Daystar import *
 sun = Daystar(latitude, longitude)
 ```
 
 The functions provided are (they all default to datetime.datetime.now()):
-  - risetime(date): returns the sunrise
-  - settime(date): returns the sunset
-  - solarnoon(date): returns the solar noon time
-  - hrangle(date): returns the hour angle for the time and date
-  - coordinates(date): returns a tuple with declination and right ascension
-  - mean(date): returns the mean anomaly
-  - true(date): returns the true anomaly
-  - ceq(date): returns the equation of center
-  - solar_julian(date): returns "rise" and "set" dictionary with sunrise and sunset julian dates
-  - alt(date): returns solar altitude
-  - azi(date): returns the solar azimuth
-  - nadir(date): returns the time of nadir
+  - `risetime(date)`: returns the sunrise 
+  - `settime(date)`: returns the sunset
+  - `solarnoon(date)`: returns the solar noon time
+  - `hrangle(date)`: returns the hour angle for the time and date
+  - `coordinates(date)`: returns a dictionary with declination and right ascension ("dec" and "ra")
+  - `mean(date)`: returns the mean anomaly
+  - `true(date)`: returns the true anomaly
+  - `ceq(date)`: returns the equation of center
+  - `solar_julian(date)`: returns "rise" and "set" dictionary with sunrise and sunset julian dates
+  - `alt(date)`: returns solar altitude
+  - `azi(date)`: returns the solar azimuth
+  - `nadir(date)`: returns the time of nadir
```

### Comparing `Daystar-0.0.5/README.md` & `Daystar-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Daystar
 Daystar is a python library that provides a convenient class for Solar calculations based off of my other library _Solarflare_. Check out Solarflare at https://pypi.org/project/Solarflare/
 
 In order to use this library, just create an instance of the daystar class:
 
 ```python
+from Daystar import *
 sun = Daystar(latitude, longitude)
 ```
 
 The functions provided are (they all default to datetime.datetime.now()):
-  - risetime(date): returns the sunrise
-  - settime(date): returns the sunset
-  - solarnoon(date): returns the solar noon time
-  - hrangle(date): returns the hour angle for the time and date
-  - coordinates(date): returns a tuple with declination and right ascension
-  - mean(date): returns the mean anomaly
-  - true(date): returns the true anomaly
-  - ceq(date): returns the equation of center
-  - solar_julian(date): returns "rise" and "set" dictionary with sunrise and sunset julian dates
-  - alt(date): returns solar altitude
-  - azi(date): returns the solar azimuth
-  - nadir(date): returns the time of nadir
+  - `risetime(date)`: returns the sunrise 
+  - `settime(date)`: returns the sunset
+  - `solarnoon(date)`: returns the solar noon time
+  - `hrangle(date)`: returns the hour angle for the time and date
+  - `coordinates(date)`: returns a dictionary with declination and right ascension ("dec" and "ra")
+  - `mean(date)`: returns the mean anomaly
+  - `true(date)`: returns the true anomaly
+  - `ceq(date)`: returns the equation of center
+  - `solar_julian(date)`: returns "rise" and "set" dictionary with sunrise and sunset julian dates
+  - `alt(date)`: returns solar altitude
+  - `azi(date)`: returns the solar azimuth
+  - `nadir(date)`: returns the time of nadir
```

### Comparing `Daystar-0.0.5/setup.py` & `Daystar-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 with open("README.md", "r") as fh:
   long_description = fh.read()
 setuptools.setup(
   name="Daystar",
-  version="0.0.5",
+  version="0.0.6",
   author="Siddhu Pendyala",
   author_email="siddhu.pendyala@outlook.com",
-  description="Sun calculation class from Solarflare module",
+  description="Solar calculation class for Python",
   long_description=long_description,  # don't touch this, this is your README.md
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

