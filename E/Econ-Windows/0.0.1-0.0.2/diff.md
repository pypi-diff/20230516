# Comparing `tmp/Econ_Windows-0.0.1.tar.gz` & `tmp/Econ_Windows-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.1.tar", last modified: Tue May 16 15:04:05 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.2.tar", last modified: Tue May 16 15:52:21 2023, max compression
```

## Comparing `Econ_Windows-0.0.1.tar` & `Econ_Windows-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 15:04:05.412909 Econ_Windows-0.0.1/
--rw-rw-rw-   0        0        0    10497 2023-05-16 15:03:14.000000 Econ_Windows-0.0.1/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-16 15:04:05.410829 Econ_Windows-0.0.1/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-16 15:04:05.000000 Econ_Windows-0.0.1/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-16 15:04:05.000000 Econ_Windows-0.0.1/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 15:04:05.000000 Econ_Windows-0.0.1/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 15:02:47.000000 Econ_Windows-0.0.1/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-16 15:04:05.000000 Econ_Windows-0.0.1/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-16 15:04:05.411869 Econ_Windows-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 15:04:05.412909 Econ_Windows-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-16 14:48:41.000000 Econ_Windows-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:52:21.021198 Econ_Windows-0.0.2/
+-rw-rw-rw-   0        0        0    10620 2023-05-16 15:51:43.000000 Econ_Windows-0.0.2/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-16 15:52:21.018202 Econ_Windows-0.0.2/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-16 15:52:20.000000 Econ_Windows-0.0.2/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-16 15:52:21.020198 Econ_Windows-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 15:52:21.021198 Econ_Windows-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-16 15:49:02.000000 Econ_Windows-0.0.2/setup.py
```

### Comparing `Econ_Windows-0.0.1/Econ_Windows.cpp` & `Econ_Windows-0.0.2/Econ_Windows.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 	  //return DEPTHVISTAError::setErrno(Result::Ok);
   }
   
 	bool initialize() 
 	{
 		try
 		{
-	  		printf("initialize is statred");
+	  		printf("initialize is statred\n");
 	  		CoInitializeEx(NULL, COINIT_APARTMENTTHREADED);
 	  		TCHAR devicePath[MAX_PATH] = _T("");
 	  		TCHAR extrctd_vid[10] = _T("");
 	  		TCHAR extrctd_pid[10] = _T("");
 	  		TCHAR* vid_substr;
 	  		TCHAR* pid_substr;
 	  		HRESULT hr;
@@ -117,73 +117,76 @@
 	  		indexList = 0;
 	  
 	  		hr = CoCreateInstance(CLSID_SystemDeviceEnum, NULL, CLSCTX_INPROC_SERVER,
 		  	IID_ICreateDevEnum, (void**)&pCreateDevEnum);
 	  		if (hr != NO_ERROR)
 	  		{
 		 		SetLastError(0);
-		  		printf("NotInitialized Error");
+		  		printf("NotInitialized Error\n");
 		  		return false;
 		  		//return DEPTHVISTAError::setErrno(Result::NotInitialized);
 	  		}
 
 	  	hr = pCreateDevEnum->CreateClassEnumerator(CLSID_VideoInputDeviceCategory, &pEm, 0);
 	  	if (hr != NOERROR)
 	  	{
-		  	printf("NotInitialized Error");
+		  	printf("NotInitialized Error\n");
 		  	//return DEPTHVISTAError::setErrno(Result::NotInitialized);
 		  	return false;
 	  	}
 	  	pEm->Reset();
-	  	printf("Before While loop");
+	  	printf("Before While loop\n");
 	  	while (hr = pEm->Next(1, &pM, &cFetched), hr == S_OK)
 	  	{
-		  printf("Entered a While loop");
+		  printf("Entered a While loop\n");
 		  IPropertyBag* pBag = 0;
 		  hr = pM->BindToStorage(0, 0, IID_IPropertyBag, (void**)&pBag);
 
 		  if (SUCCEEDED(hr))
 		  {
-			  printf(" While loop hr successed");
+			  printf(" While loop hr successed\n");
 			  VARIANT var;
 			  var.vt = VT_BSTR;
 			  hr = pBag->Read(L"DevicePath", &var, 0);
 			  if (hr == S_OK)
 	 		  {
-				   printf(" While loop hr S_OK successed");
+				   printf(" While loop hr S_OK successed\n");
 				  StringCbPrintf(devicePath, MAX_PATH, L"%s", var.bstrVal);
 
 				  if (devicePath != NULL)
 				  {
-					  printf(" While loop hr devicePath != NULL successed");
+					  printf(" While loop hr devicePath != NULL successed\n");
 					  vid_substr = wcsstr(wcsupr(devicePath), TEXT("VID_"));
 
 					  if (vid_substr != NULL)
 					  {
 						  wcsncpy_s(extrctd_vid, vid_substr + 4, 4);
 						  extrctd_vid[5] = '\0';
-						  printf(" While loop hr wcsncpy_s(extrctd_vid, vid_substr + 4, 4) successed");
+						  printf(" While loop hr wcsncpy_s(extrctd_vid, vid_substr + 4, 4) successed\n");
 					  }
 
 					  pid_substr = wcsstr(wcsupr(devicePath), TEXT("PID_"));
 
 					  if (pid_substr != NULL)
 					  {
 						  wcsncpy_s(extrctd_pid, pid_substr + 4, 4);
 						  extrctd_pid[5] = '\0';
-						  printf("While loop - pid_substr != NULL - wcsncpy_s(extrctd_pid, pid_substr + 4, 4);");
+						  printf("While loop - pid_substr != NULL - wcsncpy_s(extrctd_pid, pid_substr + 4, 4);\n");
 					  }
-						printf("Before index list is fill \n");
+						
 
 					  if ((wcscmp(wcsupr(extrctd_vid), TOF_VID) == 0) && (wcscmp(wcsupr(extrctd_pid), TOF_PID) == 0))
 					  {
-						  
+						  printf("Before index list is fill  %d\n"+indexList);
 						  indexList |= (1 << Count);
-						  Count++;
 						  printf("After index list is : %d\n"+indexList);
+						  printf("count = %d\n"+ Count);
+						  Count++;
+						  printf("count = %d\n"+ Count);
+						  
 					  }
 
 				  }
 				  SysFreeString(var.bstrVal);
 			  }
 			  pM->AddRef();
```

### Comparing `Econ_Windows-0.0.1/setup.py` & `Econ_Windows-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.1',
+    version='0.0.2',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

