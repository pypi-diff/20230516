# Comparing `tmp/Econ_Windows-0.0.2.tar.gz` & `tmp/Econ_Windows-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.2.tar", last modified: Tue May 16 15:52:21 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.3.tar", last modified: Tue May 16 16:00:49 2023, max compression
```

## Comparing `Econ_Windows-0.0.2.tar` & `Econ_Windows-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 15:52:21.021198 Econ_Windows-0.0.2/
--rw-rw-rw-   0        0        0    10620 2023-05-16 15:51:43.000000 Econ_Windows-0.0.2/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-16 15:52:21.018202 Econ_Windows-0.0.2/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-16 15:52:21.020198 Econ_Windows-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 15:52:21.021198 Econ_Windows-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-16 15:49:02.000000 Econ_Windows-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:00:49.640071 Econ_Windows-0.0.3/
+-rw-rw-rw-   0        0        0    10660 2023-05-16 15:59:30.000000 Econ_Windows-0.0.3/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-16 16:00:49.637070 Econ_Windows-0.0.3/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:00:49.639071 Econ_Windows-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:00:49.641171 Econ_Windows-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-16 15:59:59.000000 Econ_Windows-0.0.3/setup.py
```

### Comparing `Econ_Windows-0.0.2/Econ_Windows.cpp` & `Econ_Windows-0.0.3/Econ_Windows.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 						  printf("While loop - pid_substr != NULL - wcsncpy_s(extrctd_pid, pid_substr + 4, 4);\n");
 					  }
 						
 
 					  if ((wcscmp(wcsupr(extrctd_vid), TOF_VID) == 0) && (wcscmp(wcsupr(extrctd_pid), TOF_PID) == 0))
 					  {
 						  printf("Before index list is fill  %d\n"+indexList);
+						  printf("count = %d\n"+ Count);
 						  indexList |= (1 << Count);
 						  printf("After index list is : %d\n"+indexList);
 						  printf("count = %d\n"+ Count);
 						  Count++;
 						  printf("count = %d\n"+ Count);
 						  
 					  }
```

### Comparing `Econ_Windows-0.0.2/setup.py` & `Econ_Windows-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.2',
+    version='0.0.3',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

