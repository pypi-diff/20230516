# Comparing `tmp/iplocationchanger-0.0.3.tar.gz` & `tmp/iplocationchanger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iplocationchanger-0.0.3.tar", last modified: Mon Apr 24 17:45:37 2023, max compression
+gzip compressed data, was "iplocationchanger-0.0.4.tar", last modified: Tue May 16 19:11:37 2023, max compression
```

## Comparing `iplocationchanger-0.0.3.tar` & `iplocationchanger-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.936456 iplocationchanger-0.0.3/
--rw-r--r--   0 faaizz     (501) staff       (20)     1076 2023-03-01 19:20:31.000000 iplocationchanger-0.0.3/LICENSE
--rw-r--r--   0 faaizz     (501) staff       (20)     4234 2023-04-24 17:45:37.936014 iplocationchanger-0.0.3/PKG-INFO
--rw-r--r--   0 faaizz     (501) staff       (20)     2361 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/README.md
--rw-r--r--   0 faaizz     (501) staff       (20)      923 2023-04-24 17:45:08.000000 iplocationchanger-0.0.3/pyproject.toml
--rw-r--r--   0 faaizz     (501) staff       (20)       38 2023-04-24 17:45:37.936593 iplocationchanger-0.0.3/setup.cfg
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.920349 iplocationchanger-0.0.3/src/
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.923934 iplocationchanger-0.0.3/src/iplocationchanger/
--rw-r--r--   0 faaizz     (501) staff       (20)       22 2023-03-05 11:44:17.000000 iplocationchanger-0.0.3/src/iplocationchanger/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     2264 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/__main__.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.930791 iplocationchanger-0.0.3/src/iplocationchanger/exception/
--rw-r--r--   0 faaizz     (501) staff       (20)      106 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/iplocationchanger_exception.py
--rw-r--r--   0 faaizz     (501) staff       (20)      171 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/location_changer_service_exception.py
--rw-r--r--   0 faaizz     (501) staff       (20)      163 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/openvpn_service_exception.py
--rw-r--r--   0 faaizz     (501) staff       (20)      166 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/whatismyip_service_exception.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.931708 iplocationchanger-0.0.3/src/iplocationchanger/model/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/model/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)      570 2023-03-02 21:42:30.000000 iplocationchanger-0.0.3/src/iplocationchanger/model/openvpn_credentials.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.933725 iplocationchanger-0.0.3/src/iplocationchanger/service/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:19.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     2078 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/location_changer_service.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1839 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/openvpn_service.py
--rw-r--r--   0 faaizz     (501) staff       (20)     3013 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/whatismyip_service.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.935327 iplocationchanger-0.0.3/src/iplocationchanger/utils/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:22.000000 iplocationchanger-0.0.3/src/iplocationchanger/utils/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)      852 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/utils/utils.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.928283 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/
--rw-r--r--   0 faaizz     (501) staff       (20)     4234 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/PKG-INFO
--rw-r--r--   0 faaizz     (501) staff       (20)      951 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/SOURCES.txt
--rw-r--r--   0 faaizz     (501) staff       (20)        1 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/dependency_links.txt
--rw-r--r--   0 faaizz     (501) staff       (20)       40 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/requires.txt
--rw-r--r--   0 faaizz     (501) staff       (20)       18 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/top_level.txt
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.165633 iplocationchanger-0.0.4/
+-rw-r--r--   0 faaizz     (501) staff       (20)     1076 2023-03-01 19:20:31.000000 iplocationchanger-0.0.4/LICENSE
+-rw-r--r--   0 faaizz     (501) staff       (20)     4234 2023-05-16 19:11:37.165083 iplocationchanger-0.0.4/PKG-INFO
+-rw-r--r--   0 faaizz     (501) staff       (20)     2361 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/README.md
+-rw-r--r--   0 faaizz     (501) staff       (20)      923 2023-05-16 19:10:21.000000 iplocationchanger-0.0.4/pyproject.toml
+-rw-r--r--   0 faaizz     (501) staff       (20)       38 2023-05-16 19:11:37.165761 iplocationchanger-0.0.4/setup.cfg
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.141124 iplocationchanger-0.0.4/src/
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.144039 iplocationchanger-0.0.4/src/iplocationchanger/
+-rw-r--r--   0 faaizz     (501) staff       (20)       22 2023-03-05 11:44:17.000000 iplocationchanger-0.0.4/src/iplocationchanger/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     2264 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/__main__.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.160507 iplocationchanger-0.0.4/src/iplocationchanger/exception/
+-rw-r--r--   0 faaizz     (501) staff       (20)      106 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/exception/iplocationchanger_exception.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      171 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/exception/location_changer_service_exception.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      163 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/exception/openvpn_service_exception.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      166 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/exception/whatismyip_service_exception.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.161489 iplocationchanger-0.0.4/src/iplocationchanger/model/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/model/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      570 2023-03-02 21:42:30.000000 iplocationchanger-0.0.4/src/iplocationchanger/model/openvpn_credentials.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.163603 iplocationchanger-0.0.4/src/iplocationchanger/service/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:19.000000 iplocationchanger-0.0.4/src/iplocationchanger/service/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     2078 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/service/location_changer_service.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     1839 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/service/openvpn_service.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     3013 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/service/whatismyip_service.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.164471 iplocationchanger-0.0.4/src/iplocationchanger/utils/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:22.000000 iplocationchanger-0.0.4/src/iplocationchanger/utils/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      852 2023-04-24 17:44:14.000000 iplocationchanger-0.0.4/src/iplocationchanger/utils/utils.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-05-16 19:11:37.158071 iplocationchanger-0.0.4/src/iplocationchanger.egg-info/
+-rw-r--r--   0 faaizz     (501) staff       (20)     4234 2023-05-16 19:11:37.000000 iplocationchanger-0.0.4/src/iplocationchanger.egg-info/PKG-INFO
+-rw-r--r--   0 faaizz     (501) staff       (20)      951 2023-05-16 19:11:37.000000 iplocationchanger-0.0.4/src/iplocationchanger.egg-info/SOURCES.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)        1 2023-05-16 19:11:37.000000 iplocationchanger-0.0.4/src/iplocationchanger.egg-info/dependency_links.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)       40 2023-05-16 19:11:37.000000 iplocationchanger-0.0.4/src/iplocationchanger.egg-info/requires.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)       18 2023-05-16 19:11:37.000000 iplocationchanger-0.0.4/src/iplocationchanger.egg-info/top_level.txt
```

### Comparing `iplocationchanger-0.0.3/LICENSE` & `iplocationchanger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/PKG-INFO` & `iplocationchanger-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iplocationchanger
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reliable IP location changer using OpenVPN and WhatIsMyIP
 Author-email: Faizudeen Kajogbola <faizudeen@codecreek.cc>
 License: MIT License
         
         Copyright (c) 2023 Faizudeen Kajogbola
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `iplocationchanger-0.0.3/README.md` & `iplocationchanger-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/pyproject.toml` & `iplocationchanger-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iplocationchanger"
-version = "0.0.3"
+version = "0.0.4"
 description = "Reliable IP location changer using OpenVPN and WhatIsMyIP"
 readme = "README.md"
 authors = [{ name = "Faizudeen Kajogbola", email = "faizudeen@codecreek.cc" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
```

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger/__main__.py` & `iplocationchanger-0.0.4/src/iplocationchanger/__main__.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger/model/openvpn_credentials.py` & `iplocationchanger-0.0.4/src/iplocationchanger/model/openvpn_credentials.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger/service/location_changer_service.py` & `iplocationchanger-0.0.4/src/iplocationchanger/service/location_changer_service.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger/service/openvpn_service.py` & `iplocationchanger-0.0.4/src/iplocationchanger/service/openvpn_service.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger/service/whatismyip_service.py` & `iplocationchanger-0.0.4/src/iplocationchanger/service/whatismyip_service.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger/utils/utils.py` & `iplocationchanger-0.0.4/src/iplocationchanger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger.egg-info/PKG-INFO` & `iplocationchanger-0.0.4/src/iplocationchanger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iplocationchanger
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reliable IP location changer using OpenVPN and WhatIsMyIP
 Author-email: Faizudeen Kajogbola <faizudeen@codecreek.cc>
 License: MIT License
         
         Copyright (c) 2023 Faizudeen Kajogbola
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `iplocationchanger-0.0.3/src/iplocationchanger.egg-info/SOURCES.txt` & `iplocationchanger-0.0.4/src/iplocationchanger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

