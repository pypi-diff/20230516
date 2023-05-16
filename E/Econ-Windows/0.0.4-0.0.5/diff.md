# Comparing `tmp/Econ_Windows-0.0.4.tar.gz` & `tmp/Econ_Windows-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.4.tar", last modified: Tue May 16 16:08:01 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.5.tar", last modified: Tue May 16 16:13:10 2023, max compression
```

## Comparing `Econ_Windows-0.0.4.tar` & `Econ_Windows-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 16:08:01.048699 Econ_Windows-0.0.4/
--rw-rw-rw-   0        0        0    10744 2023-05-16 16:07:16.000000 Econ_Windows-0.0.4/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-16 16:08:01.043214 Econ_Windows-0.0.4/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-16 16:08:00.000000 Econ_Windows-0.0.4/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-16 16:08:01.046692 Econ_Windows-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 16:08:01.049700 Econ_Windows-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-16 16:07:44.000000 Econ_Windows-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:13:10.504791 Econ_Windows-0.0.5/
+-rw-rw-rw-   0        0        0    10922 2023-05-16 16:12:35.000000 Econ_Windows-0.0.5/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-16 16:13:10.501144 Econ_Windows-0.0.5/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:13:10.502834 Econ_Windows-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:13:10.504791 Econ_Windows-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-16 16:09:58.000000 Econ_Windows-0.0.5/setup.py
```

### Comparing `Econ_Windows-0.0.4/Econ_Windows.cpp` & `Econ_Windows-0.0.5/Econ_Windows.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -227,16 +227,20 @@
 	  {
 		 // return DEPTHVISTAError::setErrno(Result::NoDeviceConnected);
 		 printf("Device is not connected");
 		 return false;
 	  }
 	  while (list)
 	  {
+		  printf("Before list =  %d\n",list);
 		  list &= (list - 1);
+		  printf("After list =  %d\n",list);
+		  printf("Before list =  %d\n",gDeviceCount);
 		  *gDeviceCount += 1;
+		  printf("After list =  %d\n",gDeviceCount);
 	  }
 	  return true;
   }
   
 	bool getDeviceListInfo(uint32_t deviceCount,DeviceInfo* gDevicesList) 
 	{
 	  for (uint32_t index = 0; index < deviceCount; index++)
```

### Comparing `Econ_Windows-0.0.4/setup.py` & `Econ_Windows-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.4',
+    version='0.0.5',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

