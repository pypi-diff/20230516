# Comparing `tmp/Daystar-0.0.4.tar.gz` & `tmp/Daystar-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Daystar-0.0.4.tar", last modified: Tue May 16 19:32:22 2023, max compression
+gzip compressed data, was "Daystar-0.0.5.tar", last modified: Tue May 16 19:40:08 2023, max compression
```

## Comparing `Daystar-0.0.4.tar` & `Daystar-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:32:22.493972 Daystar-0.0.4/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:32:22.493972 Daystar-0.0.4/Daystar/
--rw-r--r--   0 runner    (1000) runner    (1000)     1092 2023-05-16 16:45:08.000000 Daystar-0.0.4/Daystar/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:32:22.493972 Daystar-0.0.4/Daystar.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1071 2023-05-16 19:32:22.000000 Daystar-0.0.4/Daystar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-05-16 19:32:22.000000 Daystar-0.0.4/Daystar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-16 19:32:22.000000 Daystar-0.0.4/Daystar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-16 19:32:22.000000 Daystar-0.0.4/Daystar.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-05-16 19:32:22.000000 Daystar-0.0.4/Daystar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-05-16 03:18:05.000000 Daystar-0.0.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1071 2023-05-16 19:32:22.493972 Daystar-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      668 2023-05-16 03:33:27.000000 Daystar-0.0.4/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Daystar-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-16 19:32:22.493972 Daystar-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      658 2023-05-16 16:45:12.000000 Daystar-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:40:08.349299 Daystar-0.0.5/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:40:08.349299 Daystar-0.0.5/Daystar/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1391 2023-05-16 19:39:32.000000 Daystar-0.0.5/Daystar/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 19:40:08.349299 Daystar-0.0.5/Daystar.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1418 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-05-16 19:40:08.000000 Daystar-0.0.5/Daystar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-05-16 03:18:05.000000 Daystar-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1418 2023-05-16 19:40:08.349299 Daystar-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1014 2023-05-16 19:39:23.000000 Daystar-0.0.5/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Daystar-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-16 19:40:08.349299 Daystar-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      658 2023-05-16 19:39:46.000000 Daystar-0.0.5/setup.py
```

### Comparing `Daystar-0.0.4/Daystar/__init__.py` & `Daystar-0.0.5/Daystar/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,7 +33,16 @@
     return equation(date)
 
   def solar_julian(self, date=datetime.datetime.now()):
     return {
       "rise": julian_date(sunrise(self.lat, self.long, date)),
       "set": julian_date(sunset(self.lat, self.long, date))
     }
+
+  def alt(self, date=datetime.datetime.now()):
+    return altitude(self.lat, self.long, date)
+
+  def azi(self, date=datetime.datetime.now()):
+    return azimuth(self.lat, self.long, date)
+
+  def nadir(self, date=datetime.datetime.now()):
+    return fromJulian(solar_transit(self.long, date) - 0.5)
```

### Comparing `Daystar-0.0.4/LICENSE` & `Daystar-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Daystar-0.0.4/setup.py` & `Daystar-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
   long_description = fh.read()
 setuptools.setup(
   name="Daystar",
-  version="0.0.4",
+  version="0.0.5",
   author="Siddhu Pendyala",
   author_email="siddhu.pendyala@outlook.com",
   description="Sun calculation class from Solarflare module",
   long_description=long_description,  # don't touch this, this is your README.md
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

