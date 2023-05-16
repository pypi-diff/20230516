# Comparing `tmp/nso-oc-2.50.0.tar.gz` & `tmp/nso-oc-2.50.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-oc-2.50.0.tar", last modified: Mon May 15 14:50:23 2023, max compression
+gzip compressed data, was "nso-oc-2.50.1.tar", last modified: Mon May 15 19:19:54 2023, max compression
```

## Comparing `nso-oc-2.50.0.tar` & `nso-oc-2.50.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.741520 nso-oc-2.50.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-15 14:49:51.000000 nso-oc-2.50.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 14:49:51.000000 nso-oc-2.50.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 14:50:23.741520 nso-oc-2.50.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 14:49:51.000000 nso-oc-2.50.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.737519 nso-oc-2.50.0/nso_oc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 14:50:23.000000 nso-oc-2.50.0/nso_oc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.737519 nso-oc-2.50.0/package_nso_to_oc/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.741520 nso-oc-2.50.0/package_nso_to_oc/xe/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/common_xe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/main_xe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    63506 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_network_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_ospfv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_routing_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_static_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_stp.py
--rw-r--r--   0 runner    (1001) docker     (123)    93881 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xe/xe_vlans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:50:23.741520 nso-oc-2.50.0/package_nso_to_oc/xr/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/common_xr.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/main_xr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/xr_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/xr_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-15 14:49:51.000000 nso-oc-2.50.0/package_nso_to_oc/xr/xr_system.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 14:49:51.000000 nso-oc-2.50.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 14:50:23.741520 nso-oc-2.50.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-15 14:49:51.000000 nso-oc-2.50.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:19:54.931579 nso-oc-2.50.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-15 19:19:16.000000 nso-oc-2.50.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 19:19:16.000000 nso-oc-2.50.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 19:19:54.931579 nso-oc-2.50.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 19:19:16.000000 nso-oc-2.50.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:19:54.923579 nso-oc-2.50.1/nso_oc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-15 19:19:54.000000 nso-oc-2.50.1/nso_oc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-15 19:19:54.000000 nso-oc-2.50.1/nso_oc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:19:54.000000 nso-oc-2.50.1/nso_oc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 19:19:54.000000 nso-oc-2.50.1/nso_oc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 19:19:54.000000 nso-oc-2.50.1/nso_oc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 19:19:54.000000 nso-oc-2.50.1/nso_oc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:19:54.923579 nso-oc-2.50.1/package_nso_to_oc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3569 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:19:54.927579 nso-oc-2.50.1/package_nso_to_oc/xe/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/common_xe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/main_xe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30058 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36678 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63474 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42084 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_network_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39884 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_ospfv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_routing_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_static_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32957 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_stp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93881 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xe/xe_vlans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:19:54.931579 nso-oc-2.50.1/package_nso_to_oc/xr/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xr/common_xr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xr/main_xr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23665 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xr/xr_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xr/xr_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-15 19:19:16.000000 nso-oc-2.50.1/package_nso_to_oc/xr/xr_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-15 19:19:16.000000 nso-oc-2.50.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 19:19:54.931579 nso-oc-2.50.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-15 19:19:16.000000 nso-oc-2.50.1/setup.py
```

### Comparing `nso-oc-2.50.0/LICENSE` & `nso-oc-2.50.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/PKG-INFO` & `nso-oc-2.50.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.50.0
+Version: 2.50.1
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.50.0/README.md` & `nso-oc-2.50.1/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/nso_oc.egg-info/PKG-INFO` & `nso-oc-2.50.1/nso_oc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nso-oc
-Version: 2.50.0
+Version: 2.50.1
 Summary: Cisco NSO OpenConfig Tools
 Home-page: https://github.com/model-driven-devops/nso-oc-services
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NSO NED device configuration to OpenConfig
```

### Comparing `nso-oc-2.50.0/nso_oc.egg-info/SOURCES.txt` & `nso-oc-2.50.1/nso_oc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/README.md` & `nso-oc-2.50.1/package_nso_to_oc/README.md`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/common.py` & `nso-oc-2.50.1/package_nso_to_oc/common.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/main.py` & `nso-oc-2.50.1/package_nso_to_oc/main.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/common_xe.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/common_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/main_xe.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/main_xe.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_acls.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_bgp.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_bgp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_interfaces.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,17 +322,17 @@
             ip = ip_and_mask.get("address")
             ipv4_address_structure.update({f"{key_prefix}:ip": ip,
                                            f"{key_prefix}:config": {f"{key_prefix}:ip": ip,
                                                                        f"{key_prefix}:prefix-length": mask}})
         if len(ipv4_address_structure) > 0:
             openconfig_interface[f"{key_prefix}:ipv4"][f"{key_prefix}:addresses"][
                 f"{key_prefix}:address"].append(ipv4_address_structure)
-        
+
         process_vrrp_hsrp(vrrp_leftovers, hsrp_leftovers, index, nso_before_interface, nso_leftover_interface, ipv4_address_structure)
-    
+
     if len(vrrp_leftovers) > 0:
         nso_leftover_interface["vrrp"] = vrrp_leftovers
     elif "vrrp" in nso_leftover_interface and len(vrrp_leftovers) == 0:
         del nso_leftover_interface["vrrp"]
     if len(hsrp_leftovers) > 0:
         nso_leftover_interface["standby"]["standby-list"] = hsrp_leftovers
     elif "standby" in nso_leftover_interface and len(hsrp_leftovers) == 0:
@@ -444,15 +444,15 @@
                 "openconfig-if-ip-mdd-ext:nat-choice": "inside"}
             del nso_leftover_interface["ip"]["nat"]["inside"]
         elif nso_before_interface.get("ip", {}).get("nat", {}).get("outside"):
             openconfig_interface["openconfig-if-tunnel:ipv4"]["openconfig-if-tunnel:config"][
                 "openconfig-if-ip-mdd-ext:nat"] = {
                 "openconfig-if-ip-mdd-ext:nat-choice": "outside"}
             del nso_leftover_interface["ip"]["nat"]["outside"]
-        
+
 
 def configure_software_loopback(config_before: dict, config_leftover: dict, interface_data: dict) -> None:
     """Configure Loopbacks"""
     for interface_directory in interface_data.values():
         path_oc_sub_if = ["openconfig-interfaces:interfaces", "openconfig-interfaces:interface",
                           interface_directory["oc_interface_index"], "openconfig-interfaces:subinterfaces",
                           "openconfig-interfaces:subinterface", interface_directory["oc_sub_interface_place_counter"]]
@@ -796,15 +796,15 @@
 
             if len(current_vrrp["timers"]) == 0:
                 del current_vrrp["timers"]
         service_vrrp["openconfig-if-ip:vrrp"]["openconfig-if-ip:vrrp-group"].append(service_vrrp_group)
         # Keep object if it contains more properties
         if current_vrrp and len(current_vrrp) > 0:
             vrrp_leftover = current_vrrp
-    
+
     return (service_vrrp, vrrp_leftover)
 
 
 def xe_configure_hsrp_interfaces(nso_before_interface: dict, nso_leftover_interface: dict, index: int) -> tuple:
     """Configure HSRP"""
     service_hsrp = {"openconfig-if-ip-mdd-ext:hsrp": {"openconfig-if-ip-mdd-ext:hsrp-group": []}}
     hsrp_leftover = None
@@ -856,15 +856,15 @@
             del current_standby["timers"]["hold-time"]
 
             if len(current_standby["timers"]) == 0:
                 del current_standby["timers"]
 
         service_hsrp["openconfig-if-ip-mdd-ext:hsrp"]["openconfig-if-ip-mdd-ext:hsrp-group"].append(
             service_hsrp_group)
-        
+
         # Keep object if it contains more properties
         if current_standby and len(current_standby) > 0:
             hsrp_leftover = current_standby
 
     return (service_hsrp, hsrp_leftover)
```

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_network_instances.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_network_instances.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_ospfv2.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_ospfv2.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_routing_policy.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_routing_policy.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_static_route.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_static_route.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_stp.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_stp.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_system.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xe/xe_vlans.py` & `nso-oc-2.50.1/package_nso_to_oc/xe/xe_vlans.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xr/common_xr.py` & `nso-oc-2.50.1/package_nso_to_oc/xr/common_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xr/main_xr.py` & `nso-oc-2.50.1/package_nso_to_oc/xr/main_xr.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xr/xr_acls.py` & `nso-oc-2.50.1/package_nso_to_oc/xr/xr_acls.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xr/xr_interfaces.py` & `nso-oc-2.50.1/package_nso_to_oc/xr/xr_interfaces.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/package_nso_to_oc/xr/xr_system.py` & `nso-oc-2.50.1/package_nso_to_oc/xr/xr_system.py`

 * *Files identical despite different names*

### Comparing `nso-oc-2.50.0/setup.py` & `nso-oc-2.50.1/setup.py`

 * *Files identical despite different names*

