# Comparing `tmp/TailraiderAlliance-0.0.5.tar.gz` & `tmp/TailraiderAlliance-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TailraiderAlliance-0.0.5.tar", last modified: Tue May 16 10:12:01 2023, max compression
+gzip compressed data, was "TailraiderAlliance-0.0.6.tar", last modified: Tue May 16 10:29:13 2023, max compression
```

## Comparing `TailraiderAlliance-0.0.5.tar` & `TailraiderAlliance-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.523481 TailraiderAlliance-0.0.5/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      256 2023-05-16 10:12:01.522440 TailraiderAlliance-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.476699 TailraiderAlliance-0.0.5/TailraiderAlliance/
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.496703 TailraiderAlliance-0.0.5/TailraiderAlliance/Boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.498732 TailraiderAlliance-0.0.5/TailraiderAlliance/Bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.516111 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/
--rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/__init__.py
--rw-rw-rw-   0        0        0     1275 2023-05-16 10:07:35.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/catplot.py
--rw-rw-rw-   0        0        0     1289 2023-05-16 10:07:33.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/relplot.py
--rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Palico.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.519088 TailraiderAlliance-0.0.5/TailraiderAlliance/Plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.520209 TailraiderAlliance-0.0.5/TailraiderAlliance/Protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.521217 TailraiderAlliance-0.0.5/TailraiderAlliance/Trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Trouper/__init__.py
--rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.494704 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-16 10:12:00.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-05-16 10:12:01.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 10:12:00.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 10:12:00.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 10:12:01.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 10:12:01.524539 TailraiderAlliance-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-05-16 10:10:54.000000 TailraiderAlliance-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.320946 TailraiderAlliance-0.0.6/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      256 2023-05-16 10:29:13.319712 TailraiderAlliance-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.279615 TailraiderAlliance-0.0.6/TailraiderAlliance/
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.305008 TailraiderAlliance-0.0.6/TailraiderAlliance/Boaboa/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Boaboa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.307266 TailraiderAlliance-0.0.6/TailraiderAlliance/Bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Bugtrapper/__init__.py
+-rw-rw-rw-   0        0        0     2602 2023-05-16 10:27:54.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/GaJaLaKa.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.314833 TailraiderAlliance-0.0.6/TailraiderAlliance/Gajalaka/
+-rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-05-16 10:27:58.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Gajalaka/catplot.py
+-rw-rw-rw-   0        0        0     1302 2023-05-16 10:28:01.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Gajalaka/relplot.py
+-rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Palico.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.317089 TailraiderAlliance-0.0.6/TailraiderAlliance/Plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.317089 TailraiderAlliance-0.0.6/TailraiderAlliance/Protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.318507 TailraiderAlliance-0.0.6/TailraiderAlliance/Trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/Trouper/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.6/TailraiderAlliance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:29:13.303498 TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-16 10:29:12.000000 TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2023-05-16 10:29:13.000000 TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 10:29:12.000000 TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 10:29:12.000000 TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 10:29:12.000000 TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 10:29:13.321957 TailraiderAlliance-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      525 2023-05-16 10:28:54.000000 TailraiderAlliance-0.0.6/setup.py
```

### Comparing `TailraiderAlliance-0.0.5/LICENSE` & `TailraiderAlliance-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/catplot.py` & `TailraiderAlliance-0.0.6/TailraiderAlliance/Gajalaka/catplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,9 +34,9 @@
         --------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
         sns.catplot(data = self.data, x = x, y = y, hue = hue, kind = kind)
         plt.xlim(self.xlim_low, self.xlim_high)
-        plt.title(label = f'Value {y} per category {x}')
+        plt.title(label = f'{kind}plot with x: {x} and y: {y}')
         plt.show()
```

### Comparing `TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/relplot.py` & `TailraiderAlliance-0.0.6/TailraiderAlliance/Gajalaka/relplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,12 +31,12 @@
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
         --------------
         None :
             Instead it shows the plot for which the parameters are given
         """
-
+        
         sns.relplot(data = self.data, x = x, y = y, hue = hue, kind = kind)
         plt.xlim(self.xlim_low, self.xlim_high)
-        plt.title(label = f'Value {y} over length of {x}')
+        plt.title(label = f'{kind}plot with x: {x} and y: {y}')
         plt.show()
```

### Comparing `TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/SOURCES.txt` & `TailraiderAlliance-0.0.6/TailraiderAlliance.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+TailraiderAlliance/GaJaLaKa.py
 TailraiderAlliance/Palico.py
 TailraiderAlliance/__init__.py
 TailraiderAlliance.egg-info/PKG-INFO
 TailraiderAlliance.egg-info/SOURCES.txt
 TailraiderAlliance.egg-info/dependency_links.txt
 TailraiderAlliance.egg-info/requires.txt
 TailraiderAlliance.egg-info/top_level.txt
```

### Comparing `TailraiderAlliance-0.0.5/setup.py` & `TailraiderAlliance-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier',
     name = 'TailraiderAlliance',
-    version = '0.0.5',
+    version = '0.0.6',
     packages = find_packages(include = ['TailraiderAlliance', 'TailraiderAlliance.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

