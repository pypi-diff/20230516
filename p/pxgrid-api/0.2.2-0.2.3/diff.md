# Comparing `tmp/pxgrid-api-0.2.2.tar.gz` & `tmp/pxgrid-api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgrid-api-0.2.2.tar", last modified: Tue May 16 03:38:00 2023, max compression
+gzip compressed data, was "pxgrid-api-0.2.3.tar", last modified: Tue May 16 03:55:36 2023, max compression
```

## Comparing `pxgrid-api-0.2.2.tar` & `pxgrid-api-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.106985 pxgrid-api-0.2.2/
--rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.2/LICENSE
--rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.2/MANIFEST.in
--rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:38:00.106573 pxgrid-api-0.2.2/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)    16165 2023-05-16 03:25:57.000000 pxgrid-api-0.2.2/README.rst
--rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-16 03:20:09.000000 pxgrid-api-0.2.2/pyproject.toml
--rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-16 03:38:00.107105 pxgrid-api-0.2.2/setup.cfg
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.095313 pxgrid-api-0.2.2/src/
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.100781 pxgrid-api-0.2.2/src/pxapi/
--rw-r--r--   0 vibobrov   (503) staff       (20)       82 2023-05-16 03:37:17.000000 pxgrid-api-0.2.2/src/pxapi/__init__.py
--rwxr-xr-x   0 vibobrov   (503) staff       (20)    20358 2023-05-16 03:15:00.000000 pxgrid-api-0.2.2/src/pxapi/__main__.py
--rw-r--r--   0 vibobrov   (503) staff       (20)    29184 2023-05-16 03:33:24.000000 pxgrid-api-0.2.2/src/pxapi/pxapi.py
--rw-r--r--   0 vibobrov   (503) staff       (20)     1488 2023-05-16 03:15:00.000000 pxgrid-api-0.2.2/src/pxapi/stompframe.py
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.105744 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/
--rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/SOURCES.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/dependency_links.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/entry_points.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/requires.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/top_level.txt
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.390559 pxgrid-api-0.2.3/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.3/LICENSE
+-rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.3/MANIFEST.in
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:55:36.390104 pxgrid-api-0.2.3/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)    16165 2023-05-16 03:25:57.000000 pxgrid-api-0.2.3/README.rst
+-rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-16 03:54:47.000000 pxgrid-api-0.2.3/pyproject.toml
+-rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-16 03:55:36.390679 pxgrid-api-0.2.3/setup.cfg
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.379358 pxgrid-api-0.2.3/src/
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.384460 pxgrid-api-0.2.3/src/pxapi/
+-rw-r--r--   0 vibobrov   (503) staff       (20)       82 2023-05-16 03:54:52.000000 pxgrid-api-0.2.3/src/pxapi/__init__.py
+-rwxr-xr-x   0 vibobrov   (503) staff       (20)    20351 2023-05-16 03:54:31.000000 pxgrid-api-0.2.3/src/pxapi/__main__.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29194 2023-05-16 03:48:27.000000 pxgrid-api-0.2.3/src/pxapi/pxapi.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)     1488 2023-05-16 03:15:00.000000 pxgrid-api-0.2.3/src/pxapi/stompframe.py
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:55:36.389059 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/entry_points.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/requires.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-16 03:55:36.000000 pxgrid-api-0.2.3/src/pxgrid_api.egg-info/top_level.txt
```

### Comparing `pxgrid-api-0.2.2/LICENSE` & `pxgrid-api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.2/PKG-INFO` & `pxgrid-api-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pxgrid-api-0.2.2/README.rst` & `pxgrid-api-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.2/pyproject.toml` & `pxgrid-api-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools","wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pxgrid-api"
-version = "0.2.2"
+version = "0.2.3"
 description = "pxGrid API library and command line tool"
 readme = "README.rst"
 authors = [{ name = "Viktor Bobrov", email = "vibobrov@cisco.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pxgrid-api-0.2.2/src/pxapi/__main__.py` & `pxgrid-api-0.2.3/src/pxapi/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
                 print("pxGrid Node is not defined. Use config show to verify.")
                 return
             if (self.config["client_cert_file"]=="" or self.config["client_key_file"]=="") and self.config["password"]=="":
                 print("Either client certificate/key or password is required. Use config show to verify.")
             if not hasattr(self,"api"):
                 print("API is not initialized. Use config apply.")
                 return
-        #try:
-        return(cmd.Cmd.onecmd(self, line))
-        #except Exception as e:
-        #    print("Error occured: {}".format(e))
+        try:
+            return(cmd.Cmd.onecmd(self, line))
+        except Exception as e:
+            print(f"Error occured: {e}")
 
     def print_json(self,value):
         print(json.dumps(value,indent=2))
 
     def show_topics(self,service):
         service_info=self.api.service_lookup(service)
         for service_property in service_info["services"][0]["properties"]:
```

### Comparing `pxgrid-api-0.2.2/src/pxapi/pxapi.py` & `pxgrid-api-0.2.3/src/pxapi/pxapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,23 +391,25 @@
         self.__check_mac(mac)
         self.__check_ip(nas_ip)
         return(self.__send_px_api(self.SERVICE_ANC,"getEndpointByNasIpAddress",{"mac":mac,"nasIpAddress":nas_ip}))
 
     def anc_apply_endpoint_by_mac_address(self,policy,mac):
         """Apply ANC Policy by MAC Address. Endpoint does not need to be online.\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlapplyendpointbymacaddress
+        
         :param policy: name of ANC Policy
         :param mac: MAC Address of endpoint
         """
         self.__check_mac(mac)
         return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointByMacAddress",{"policyName":policy,"mac":mac}))
 
     def anc_apply_endpoint_by_ip_address(self,policy,ip):
         """Apply ANC Policy by IP Address. Requires that the endpoint is connected to the network.\n
         Reference: https://github.com/cisco-pxgrid/pxgrid-rest-ws/wiki/ANC-configuration#post-restbaseurlapplyendpointbyipaddress
+
         :param policyName: name of ANC Policy
         :param ip: IP Address of endpoint
         """
         self.__check_ip(ip)
         return(self.__send_px_api(self.SERVICE_ANC,"applyEndpointByIpAddress",{"policyName":policy,"ip":ip}))
 
     def anc_apply_endpoint_policy(self,policy,mac,nas_ip):
```

### Comparing `pxgrid-api-0.2.2/src/pxapi/stompframe.py` & `pxgrid-api-0.2.3/src/pxapi/stompframe.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.2/src/pxgrid_api.egg-info/PKG-INFO` & `pxgrid-api-0.2.3/src/pxgrid_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgrid-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: pxGrid API library and command line tool
 Author-email: Viktor Bobrov <vibobrov@cisco.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

