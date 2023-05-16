# Comparing `tmp/Econ_Windows-0.0.3.tar.gz` & `tmp/Econ_Windows-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.3.tar", last modified: Tue May 16 16:00:49 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.4.tar", last modified: Tue May 16 16:08:01 2023, max compression
```

## Comparing `Econ_Windows-0.0.3.tar` & `Econ_Windows-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 16:00:49.640071 Econ_Windows-0.0.3/
--rw-rw-rw-   0        0        0    10660 2023-05-16 15:59:30.000000 Econ_Windows-0.0.3/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-16 16:00:49.637070 Econ_Windows-0.0.3/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-16 16:00:49.000000 Econ_Windows-0.0.3/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-16 16:00:49.639071 Econ_Windows-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 16:00:49.641171 Econ_Windows-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-16 15:59:59.000000 Econ_Windows-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:08:01.048699 Econ_Windows-0.0.4/
+-rw-rw-rw-   0        0        0    10744 2023-05-16 16:07:16.000000 Econ_Windows-0.0.4/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-16 16:08:01.043214 Econ_Windows-0.0.4/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:08:01.046692 Econ_Windows-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:08:01.049700 Econ_Windows-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-16 16:07:44.000000 Econ_Windows-0.0.4/setup.py
```

### Comparing `Econ_Windows-0.0.3/Econ_Windows.cpp` & `Econ_Windows-0.0.4/Econ_Windows.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,18 @@
 
 					  if ((wcscmp(wcsupr(extrctd_vid), TOF_VID) == 0) && (wcscmp(wcsupr(extrctd_pid), TOF_PID) == 0))
 					  {
 						  printf("Before index list is fill  %d\n"+indexList);
 						  printf("count = %d\n"+ Count);
 						  indexList |= (1 << Count);
 						  printf("After index list is : %d\n"+indexList);
-						  printf("count = %d\n"+ Count);
+						  printf("Before count update = %d\n"+ Count);
 						  Count++;
-						  printf("count = %d\n"+ Count);
+						  printf("After count update = %d\n"+ Count);
+						  printf("After index list is : %d\n"+indexList);
 						  
 					  }
 
 				  }
 				  SysFreeString(var.bstrVal);
 			  }
 			  pM->AddRef();
```

### Comparing `Econ_Windows-0.0.3/setup.py` & `Econ_Windows-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.3',
+    version='0.0.4',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

