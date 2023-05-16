# Comparing `tmp/magyar-3.1.0.tar.gz` & `tmp/magyar-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.1.0.tar", last modified: Tue May 16 19:42:23 2023, max compression
+gzip compressed data, was "magyar-3.1.1.tar", last modified: Tue May 16 20:00:51 2023, max compression
```

## Comparing `magyar-3.1.0.tar` & `magyar-3.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-16 19:42:23.909774 magyar-3.1.0/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6754 2023-05-16 19:42:23.909774 magyar-3.1.0/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6344 2023-05-16 19:41:49.000000 magyar-3.1.0/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-16 19:42:23.909774 magyar-3.1.0/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6754 2023-05-16 19:42:23.000000 magyar-3.1.0/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-16 19:42:23.000000 magyar-3.1.0/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-16 19:42:23.000000 magyar-3.1.0/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-16 19:42:23.000000 magyar-3.1.0/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)   179728 2023-05-16 19:38:59.000000 magyar-3.1.0/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-16 19:42:23.909774 magyar-3.1.0/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-16 19:38:59.000000 magyar-3.1.0/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-16 20:00:51.859305 magyar-3.1.1/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6839 2023-05-16 20:00:51.859305 magyar-3.1.1/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6429 2023-05-16 20:00:36.000000 magyar-3.1.1/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-16 20:00:51.859305 magyar-3.1.1/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6839 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)   179728 2023-05-16 19:38:59.000000 magyar-3.1.1/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-16 20:00:51.859305 magyar-3.1.1/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-16 19:46:03.000000 magyar-3.1.1/setup.py
```

### Comparing `magyar-3.1.0/PKG-INFO` & `magyar-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.1.0
+Version: 3.1.1
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,14 +46,18 @@
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Listában Tuple:
 1. Magyarország összes települése + megye **telepules_megye**
+<br>
+
+![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/tuple.png)
+<br>
 
 
 1. Last names =  magyar.**vezeteknev**
 2. Female first names = magyar.**keresztnev_n**
 3. Male first names  = magyar.**keresztnev_f**
 4. Street names = magyar.**utca**
 5. City names = magyar.**telepules**
@@ -79,15 +83,15 @@
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
-6. 
+
 Tuple in List:
 1. All settlements in Hungary + county. = magyar.telepules_megye
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
```

### Comparing `magyar-3.1.0/README.md` & `magyar-3.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Listában Tuple:
 1. Magyarország összes települése + megye **telepules_megye**
+<br>
+
+![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/tuple.png)
+<br>
 
 
 1. Last names =  magyar.**vezeteknev**
 2. Female first names = magyar.**keresztnev_n**
 3. Male first names  = magyar.**keresztnev_f**
 4. Street names = magyar.**utca**
 5. City names = magyar.**telepules**
@@ -67,15 +71,15 @@
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
-6. 
+
 Tuple in List:
 1. All settlements in Hungary + county. = magyar.telepules_megye
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
```

### Comparing `magyar-3.1.0/magyar.egg-info/PKG-INFO` & `magyar-3.1.1/magyar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.1.0
+Version: 3.1.1
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,14 +46,18 @@
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Listában Tuple:
 1. Magyarország összes települése + megye **telepules_megye**
+<br>
+
+![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/tuple.png)
+<br>
 
 
 1. Last names =  magyar.**vezeteknev**
 2. Female first names = magyar.**keresztnev_n**
 3. Male first names  = magyar.**keresztnev_f**
 4. Street names = magyar.**utca**
 5. City names = magyar.**telepules**
@@ -79,15 +83,15 @@
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
-6. 
+
 Tuple in List:
 1. All settlements in Hungary + county. = magyar.telepules_megye
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
```

### Comparing `magyar-3.1.0/magyar.py` & `magyar-3.1.1/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-3.1.0/setup.py` & `magyar-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.1.0",
+    version="3.1.1",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

