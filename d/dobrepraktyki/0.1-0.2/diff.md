# Comparing `tmp/dobrepraktyki-0.1.tar.gz` & `tmp/dobrepraktyki-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dobrepraktyki-0.1.tar", last modified: Mon May 15 18:55:29 2023, max compression
+gzip compressed data, was "dobrepraktyki-0.2.tar", last modified: Tue May 16 07:52:15 2023, max compression
```

## Comparing `dobrepraktyki-0.1.tar` & `dobrepraktyki-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 18:55:29.965683 dobrepraktyki-0.1/
--rw-rw-rw-   0        0        0      208 2023-05-15 18:55:29.965683 dobrepraktyki-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6337 2023-05-15 17:07:40.000000 dobrepraktyki-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 18:55:29.936332 dobrepraktyki-0.1/Songs/
--rw-rw-rw-   0        0        0        0 2023-05-15 18:51:14.000000 dobrepraktyki-0.1/Songs/__init__.py
--rw-rw-rw-   0        0        0      660 2023-05-15 18:51:05.000000 dobrepraktyki-0.1/Songs/shazam.py
-drwxrwxrwx   0        0        0        0 2023-05-15 18:55:29.936332 dobrepraktyki-0.1/Weather/
--rw-rw-rw-   0        0        0        0 2023-05-15 17:25:21.000000 dobrepraktyki-0.1/Weather/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-05-15 17:51:44.000000 dobrepraktyki-0.1/Weather/weatherapi.py
--rw-rw-rw-   0        0        0      924 2023-05-15 18:07:04.000000 dobrepraktyki-0.1/Weather/weatherbit.py
-drwxrwxrwx   0        0        0        0 2023-05-15 18:55:29.965683 dobrepraktyki-0.1/dobrepraktyki.egg-info/
--rw-rw-rw-   0        0        0      208 2023-05-15 18:55:29.000000 dobrepraktyki-0.1/dobrepraktyki.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-15 18:55:29.000000 dobrepraktyki-0.1/dobrepraktyki.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 18:55:29.000000 dobrepraktyki-0.1/dobrepraktyki.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 18:55:29.000000 dobrepraktyki-0.1/dobrepraktyki.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-15 18:55:29.000000 dobrepraktyki-0.1/dobrepraktyki.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 18:55:29.965683 dobrepraktyki-0.1/setup.cfg
--rw-rw-rw-   0        0        0      255 2023-05-15 18:55:04.000000 dobrepraktyki-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:52:15.425504 dobrepraktyki-0.2/
+-rw-rw-rw-   0        0        0      208 2023-05-16 07:52:15.425504 dobrepraktyki-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6337 2023-05-15 17:07:40.000000 dobrepraktyki-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 07:52:15.394247 dobrepraktyki-0.2/Songs/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:51:09.000000 dobrepraktyki-0.2/Songs/__init__.py
+-rw-rw-rw-   0        0        0      660 2023-05-16 07:51:09.000000 dobrepraktyki-0.2/Songs/shazam.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:52:15.394247 dobrepraktyki-0.2/Weather/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:51:09.000000 dobrepraktyki-0.2/Weather/__init__.py
+-rw-rw-rw-   0        0        0     1469 2023-05-16 07:51:51.000000 dobrepraktyki-0.2/Weather/weatherapi.py
+-rw-rw-rw-   0        0        0      925 2023-05-16 07:51:51.000000 dobrepraktyki-0.2/Weather/weatherbit.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:52:15.425504 dobrepraktyki-0.2/dobrepraktyki.egg-info/
+-rw-rw-rw-   0        0        0      208 2023-05-16 07:52:15.000000 dobrepraktyki-0.2/dobrepraktyki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-16 07:52:15.000000 dobrepraktyki-0.2/dobrepraktyki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:52:15.000000 dobrepraktyki-0.2/dobrepraktyki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 07:52:15.000000 dobrepraktyki-0.2/dobrepraktyki.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 07:52:15.000000 dobrepraktyki-0.2/dobrepraktyki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:52:15.425504 dobrepraktyki-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      255 2023-05-16 07:51:51.000000 dobrepraktyki-0.2/setup.py
```

### Comparing `dobrepraktyki-0.1/README.md` & `dobrepraktyki-0.2/README.md`

 * *Files identical despite different names*

### Comparing `dobrepraktyki-0.1/Songs/shazam.py` & `dobrepraktyki-0.2/Songs/shazam.py`

 * *Files identical despite different names*

### Comparing `dobrepraktyki-0.1/Weather/weatherapi.py` & `dobrepraktyki-0.2/Weather/weatherapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,11 +29,11 @@
             for forecast in data["forecast"]["forecastday"]:
                 date = forecast["date"]
                 max_temp = forecast["day"]["maxtemp_c"]
                 min_temp = forecast["day"]["mintemp_c"]
                 condition = forecast["day"]["condition"]["text"]
 
                 tmp.update({date: {"max_temp": max_temp,
-                                   "min_tem": min_temp,
+                                   "min_temp": min_temp,
                                    "condition": condition}})
             return tmp
         return None
```

### Comparing `dobrepraktyki-0.1/Weather/weatherbit.py` & `dobrepraktyki-0.2/Weather/weatherbit.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,11 @@
             for forecast in data["data"]:
                 date = forecast["valid_date"]
                 max_temp = forecast["max_temp"]
                 min_temp = forecast["min_temp"]
                 condition = forecast["weather"]["description"]
 
                 tmp.update({date: {"max_temp": max_temp,
-                                   "min_tem": min_temp,
+                                   "min_temp": min_temp,
                                    "condition": condition}})
             return tmp
         return None
```

