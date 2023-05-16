# Comparing `tmp/vtmmpy-1.0.6.tar.gz` & `tmp/vtmmpy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtmmpy-1.0.6.tar", last modified: Fri Apr 28 10:56:14 2023, max compression
+gzip compressed data, was "vtmmpy-1.0.7.tar", max compression
```

## Comparing `vtmmpy-1.0.6.tar` & `vtmmpy-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,4 @@
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/
--rw-rw-r--   0 tony      (1000) tony      (1000)    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.6/LICENSE
--rw-rw-r--   0 tony      (1000) tony      (1000)     4115 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     3640 2023-04-28 10:46:41.000000 vtmmpy-1.0.6/README.md
--rw-r--r--   0 tony      (1000) tony      (1000)      103 2023-03-18 14:25:35.000000 vtmmpy-1.0.6/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      611 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/setup.cfg
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/src/
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/src/vtmmpy/
--rw-r--r--   0 tony      (1000) tony      (1000)     8697 2023-04-28 10:35:27.000000 vtmmpy-1.0.6/src/vtmmpy/__init__.py
-drwxrwxr-x   0 tony      (1000) tony      (1000)        0 2023-04-28 10:56:14.950293 vtmmpy-1.0.6/src/vtmmpy.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     4115 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      201 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        7 2023-04-28 10:56:14.000000 vtmmpy-1.0.6/src/vtmmpy.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.7/LICENSE
+-rw-r--r--   0        0        0      346 2023-05-16 13:29:19.315875 vtmmpy-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8869 2023-05-16 13:09:25.853982 vtmmpy-1.0.7/src/vtmmpy/__init__.py
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 vtmmpy-1.0.7/PKG-INFO
```

### Comparing `vtmmpy-1.0.6/LICENSE` & `vtmmpy-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.6/src/vtmmpy/__init__.py` & `vtmmpy-1.0.7/src/vtmmpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,22 @@
         print("  Angles of incidence:      ", np.rint(self.__theta[0]*180/np.pi), "-", np.rint(self.__theta[-1]*180/np.pi)) 
         print("  Incident medium:          ", self.__incident_medium) 
         print("  Transmitted medium:       ", self.__transmitted_medium) 
         print("") 
 
     def designs(self):
         try:
-            zipped = zip(self.__materials,self.__thicknesses) 
+            zipped = zip(self.__materials, self.__thicknesses) 
             for pair in zipped:
                 print(pair) 
         except:
             raise Exception("No designs found. Add designs with the addDesign() method.") 
             
+    def reset(self):
+        try:
+            del self.__materials
+            del self.__thicknesses
+        except:
+            print("No designs present")
+            
     def opticalProperties(self):
         return self.__opticalProperties
```

