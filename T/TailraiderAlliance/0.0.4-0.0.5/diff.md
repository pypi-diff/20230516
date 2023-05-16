# Comparing `tmp/TailraiderAlliance-0.0.4.tar.gz` & `tmp/TailraiderAlliance-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TailraiderAlliance-0.0.4.tar", last modified: Tue May 16 10:02:11 2023, max compression
+gzip compressed data, was "TailraiderAlliance-0.0.5.tar", last modified: Tue May 16 10:12:01 2023, max compression
```

## Comparing `TailraiderAlliance-0.0.4.tar` & `TailraiderAlliance-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.632426 TailraiderAlliance-0.0.4/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      256 2023-05-16 10:02:11.631407 TailraiderAlliance-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.599375 TailraiderAlliance-0.0.4/TailraiderAlliance/
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.619251 TailraiderAlliance-0.0.4/TailraiderAlliance/Boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.620525 TailraiderAlliance-0.0.4/TailraiderAlliance/Bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.625221 TailraiderAlliance-0.0.4/TailraiderAlliance/Gajalaka/
--rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Gajalaka/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-16 09:59:03.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Gajalaka/catplot.py
--rw-rw-rw-   0        0        0      963 2023-05-16 09:03:16.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Gajalaka/relplot.py
--rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Palico.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.627513 TailraiderAlliance-0.0.4/TailraiderAlliance/Plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.628959 TailraiderAlliance-0.0.4/TailraiderAlliance/Protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.630366 TailraiderAlliance-0.0.4/TailraiderAlliance/Trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/Trouper/__init__.py
--rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.4/TailraiderAlliance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:02:11.617936 TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-16 10:02:10.000000 TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-05-16 10:02:11.000000 TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 10:02:10.000000 TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 10:02:11.000000 TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 10:02:11.000000 TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 10:02:11.633428 TailraiderAlliance-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-05-16 10:01:40.000000 TailraiderAlliance-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.523481 TailraiderAlliance-0.0.5/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      256 2023-05-16 10:12:01.522440 TailraiderAlliance-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.476699 TailraiderAlliance-0.0.5/TailraiderAlliance/
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.496703 TailraiderAlliance-0.0.5/TailraiderAlliance/Boaboa/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Boaboa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.498732 TailraiderAlliance-0.0.5/TailraiderAlliance/Bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.516111 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/
+-rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     1275 2023-05-16 10:07:35.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/catplot.py
+-rw-rw-rw-   0        0        0     1289 2023-05-16 10:07:33.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/relplot.py
+-rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Palico.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.519088 TailraiderAlliance-0.0.5/TailraiderAlliance/Plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.520209 TailraiderAlliance-0.0.5/TailraiderAlliance/Protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.521217 TailraiderAlliance-0.0.5/TailraiderAlliance/Trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/Trouper/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.5/TailraiderAlliance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:12:01.494704 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-16 10:12:00.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-05-16 10:12:01.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 10:12:00.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 10:12:00.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 10:12:01.000000 TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 10:12:01.524539 TailraiderAlliance-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      525 2023-05-16 10:10:54.000000 TailraiderAlliance-0.0.5/setup.py
```

### Comparing `TailraiderAlliance-0.0.4/LICENSE` & `TailraiderAlliance-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.4/TailraiderAlliance/Gajalaka/catplot.py` & `TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/catplot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 class CatPlot:
     """ Code for making catplots """
     def __init__(self, df, xlim_low = None, xlim_high = None):
-        self.df = df
+        self.data = df
         self.xlim_low = xlim_low
         self.xlim_high = xlim_high
+
     def catplot(self, x, y, hue = None, kind = 'bar'):
         """
         A function to make a catplot, based on the dataframe used for Gajalaka
 
         Parameters:
         --------------
         self :
```

### Comparing `TailraiderAlliance-0.0.4/TailraiderAlliance/Gajalaka/relplot.py` & `TailraiderAlliance-0.0.5/TailraiderAlliance/Gajalaka/relplot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 
-def relplot(self, x, y, hue = None, kind = 'scatter'):
-    """
-    A function to make a relplot, based on the dataframe used for Gajalaka
-
-    Parameters:
-    --------------
-    self :
-        The given name of the class
-
-    x : str
-        Column name for x parameter
-    
-    y : str
-        Column name for y parameter
-
-    hue : str (default = None)
-        A column name for differentiating per category
-
-    kind : str (default = 'bar')
-        The kind of plot you want to make, options are:
-            strip, swarm, box, violin, boxen, point, bar and count
-
-    Returns:
-    --------------
-    None :
-        Instead it shows the plot for which the parameters are given
-    """
-
-    sns.relplot(data = self.data, x = x, y = y, hue = hue, kind = kind)
-    plt.xlim(self.xlim_low, self.xlim_high)
-    plt.title(label = f'Value {y} over length of {x}')
-    plt.show()
+class RelPlot:
+    """ Code for making relplots """
+    def __init__(self, df, xlim_low = None, xlim_high = None):
+        self.data = df
+        self.xlim_low = xlim_low
+        self.xlim_high = xlim_high
+        
+    def relplot(self, x, y, hue = None, kind = 'scatter'):
+        """
+        A function to make a relplot, based on the dataframe used for Gajalaka
+
+        Parameters:
+        --------------
+        self :
+            The given name of the class
+
+        x : str
+            Column name for x parameter
+        
+        y : str
+            Column name for y parameter
+
+        hue : str (default = None)
+            A column name for differentiating per category
+
+        kind : str (default = 'bar')
+            The kind of plot you want to make, options are:
+                strip, swarm, box, violin, boxen, point, bar and count
+
+        Returns:
+        --------------
+        None :
+            Instead it shows the plot for which the parameters are given
+        """
+
+        sns.relplot(data = self.data, x = x, y = y, hue = hue, kind = kind)
+        plt.xlim(self.xlim_low, self.xlim_high)
+        plt.title(label = f'Value {y} over length of {x}')
+        plt.show()
```

### Comparing `TailraiderAlliance-0.0.4/TailraiderAlliance.egg-info/SOURCES.txt` & `TailraiderAlliance-0.0.5/TailraiderAlliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.4/setup.py` & `TailraiderAlliance-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier',
     name = 'TailraiderAlliance',
-    version = '0.0.4',
+    version = '0.0.5',
     packages = find_packages(include = ['TailraiderAlliance', 'TailraiderAlliance.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

