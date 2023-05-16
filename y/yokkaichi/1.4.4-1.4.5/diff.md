# Comparing `tmp/yokkaichi-1.4.4.tar.gz` & `tmp/yokkaichi-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.4.4.tar", last modified: Mon May 15 20:14:41 2023, max compression
+gzip compressed data, was "yokkaichi-1.4.5.tar", last modified: Tue May 16 21:24:53 2023, max compression
```

## Comparing `yokkaichi-1.4.4.tar` & `yokkaichi-1.4.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-15 20:14:41.965562 yokkaichi-1.4.4/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.4/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-15 20:14:41.965562 yokkaichi-1.4.4/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.4/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-15 20:14:41.965562 yokkaichi-1.4.4/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1547 2023-05-14 22:01:12.000000 yokkaichi-1.4.4/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-15 20:14:41.962229 yokkaichi-1.4.4/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.4/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6019 2023-05-15 20:13:39.000000 yokkaichi-1.4.4/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-15 20:13:39.000000 yokkaichi-1.4.4/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     8322 2023-05-14 21:45:54.000000 yokkaichi-1.4.4/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.4/yokkaichi/args_to_cfg.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3847 2023-05-15 20:13:39.000000 yokkaichi-1.4.4/yokkaichi/config_loader.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-15 20:14:41.962229 yokkaichi-1.4.4/yokkaichi/constants/
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.4/yokkaichi/constants/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.4.4/yokkaichi/constants/rich_console.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.4/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-15 20:14:41.962229 yokkaichi-1.4.4/yokkaichi/structs/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1053 2023-05-14 22:01:12.000000 yokkaichi-1.4.4/yokkaichi/structs/CFG.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.4/yokkaichi/structs/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-15 20:14:41.962229 yokkaichi-1.4.4/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-15 20:14:41.000000 yokkaichi-1.4.4/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      487 2023-05-15 20:14:41.000000 yokkaichi-1.4.4/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-15 20:14:41.000000 yokkaichi-1.4.4/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       63 2023-05-15 20:14:41.000000 yokkaichi-1.4.4/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-15 20:14:41.000000 yokkaichi-1.4.4/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.5/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.5/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1547 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.154572 yokkaichi-1.4.5/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.5/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     5835 2023-05-16 21:23:31.000000 yokkaichi-1.4.5/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-16 21:23:31.000000 yokkaichi-1.4.5/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     8949 2023-05-16 21:23:31.000000 yokkaichi-1.4.5/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.5/yokkaichi/args_to_cfg.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3847 2023-05-15 20:13:39.000000 yokkaichi-1.4.5/yokkaichi/config_loader.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/yokkaichi/constants/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/yokkaichi/constants/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.4.5/yokkaichi/constants/rich_console.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.5/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/yokkaichi/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1053 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/yokkaichi/structs/CFG.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/yokkaichi/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.154572 yokkaichi-1.4.5/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      487 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       63 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.4.4/LICENSE.txt` & `yokkaichi-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/PKG-INFO` & `yokkaichi-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.4
+Version: 1.4.5
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `yokkaichi-1.4.4/README.md` & `yokkaichi-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/setup.py` & `yokkaichi-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/yokkaichi/MasscanScan.py` & `yokkaichi-1.4.5/yokkaichi/MasscanScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/yokkaichi/ServerScan.py` & `yokkaichi-1.4.5/yokkaichi/ServerScan.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,20 +40,14 @@
 
         for thread in thread_list:
             thread.start()
 
         for thread in thread_list:
             thread.join()
 
-        # Show results
-        server_count = len(self.results)
-        console.print(
-            f"[bold white]{server_count}[/bold white] servers found", style="magenta"
-        )
-
     def scan_server(self):
         # Scan servers from masscan list
         if self.masscan_list != None:
             self.scan_masscan()
         if self.ip_list != None:
             self.scan_ip_list()
```

### Comparing `yokkaichi-1.4.4/yokkaichi/__main__.py` & `yokkaichi-1.4.5/yokkaichi/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Import modules
 from .constants.rich_console import console
 from .port_parser import parse_port_range
 from .args_to_cfg import args_to_cfg
 from .MasscanScan import MasscanScan
 from .ServerScan import ServerScan
 from yokkaichi import __version__
+from datetime import datetime
 from . import config_loader
 import IP2Location
 import platform
 import argparse
 import requests
 import pathlib
 import tomli
+import time
 
 
 def display_version():
     console.print(
         f"yokkaichi [bold cyan]{__version__}[/bold cyan] on [bold cyan]{platform.python_implementation()} {platform.python_version()}[/bold cyan]",
         style="green",
     )
@@ -110,14 +112,16 @@
             exit(0)
     else:
         # Touch the file
         pathlib.Path(cfg.output).touch()
 
     verify_ip2location(cfg.ip2location_db)
 
+    scan_start = time.time()
+
     if cfg.ip_list_scan:
         console.print("Loading IPs", style="cyan")
         ip_list = load_ip_list(cfg.ip_list)
         console.print(f"Loaded {len(ip_list)} IPs", style="green")
     else:
         ip_list = None
 
@@ -139,15 +143,27 @@
         masscan_results = masscan_scanner.start_scan()
     else:
         masscan_results = None
 
     # print(clr.Fore.CYAN + "Loading IPs")
     # ips = load_file()
 
-    ServerScan(cfg=cfg, masscan_list=masscan_results, ip_list=ip_list).start_scan()
+    scanner = ServerScan(cfg=cfg, masscan_list=masscan_results, ip_list=ip_list)
+    scanner.start_scan()
+
+    scan_end = time.time()
+
+    # Show results
+    scan_start_time = datetime.fromtimestamp(scan_start).isoformat()
+    scan_end_time = datetime.fromtimestamp(scan_end).isoformat()
+    scan_time = time.strftime("%H:%M:%S", time.gmtime(scan_end - scan_start))
+    console.print(
+        f"[bold white]{len(scanner.results)}[/bold white] servers found.\nStarted: [bold white]{scan_start_time}[/bold white].\nEnded: [bold white]{scan_end_time}[/bold white].\nTook [bold white]{scan_time}[/bold white].",
+        style="magenta",
+    )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(allow_abbrev=False)
     parser.add_argument(
         "-j", "--java", dest="java", help="Scan for Java servers", action="store_true"
     )
```

### Comparing `yokkaichi-1.4.4/yokkaichi/args_to_cfg.py` & `yokkaichi-1.4.5/yokkaichi/args_to_cfg.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/yokkaichi/config_loader.py` & `yokkaichi-1.4.5/yokkaichi/config_loader.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/yokkaichi/port_parser.py` & `yokkaichi-1.4.5/yokkaichi/port_parser.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/yokkaichi/structs/CFG.py` & `yokkaichi-1.4.5/yokkaichi/structs/CFG.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.4/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.4.5/yokkaichi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.4
+Version: 1.4.5
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

