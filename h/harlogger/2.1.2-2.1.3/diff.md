# Comparing `tmp/harlogger-2.1.2.tar.gz` & `tmp/harlogger-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlogger-2.1.2.tar", last modified: Sun Sep 18 16:24:44 2022, max compression
+gzip compressed data, was "harlogger-2.1.3.tar", last modified: Tue May 16 09:39:59 2023, max compression
```

## Comparing `harlogger-2.1.2.tar` & `harlogger-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 16:24:44.646498 harlogger-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-09-18 16:24:37.000000 harlogger-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-09-18 16:24:44.646498 harlogger-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-09-18 16:24:37.000000 harlogger-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 16:24:44.642497 harlogger-2.1.2/harlogger/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-18 16:24:37.000000 harlogger-2.1.2/harlogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2022-09-18 16:24:37.000000 harlogger-2.1.2/harlogger/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 16:24:44.646498 harlogger-2.1.2/harlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-09-18 16:24:44.000000 harlogger-2.1.2/harlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-18 16:24:44.000000 harlogger-2.1.2/harlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 16:24:44.000000 harlogger-2.1.2/harlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-18 16:24:44.000000 harlogger-2.1.2/harlogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-18 16:24:44.000000 harlogger-2.1.2/harlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-18 16:24:44.000000 harlogger-2.1.2/harlogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 16:24:44.646498 harlogger-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-09-18 16:24:37.000000 harlogger-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:59.263680 harlogger-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 09:39:43.000000 harlogger-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46960 2023-05-16 09:39:59.263680 harlogger-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-16 09:39:43.000000 harlogger-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:59.263680 harlogger-2.1.3/harlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:43.000000 harlogger-2.1.3/harlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-05-16 09:39:43.000000 harlogger-2.1.3/harlogger/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:59.263680 harlogger-2.1.3/harlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46960 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 09:39:43.000000 harlogger-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 09:39:43.000000 harlogger-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:39:59.263680 harlogger-2.1.3/setup.cfg
```

### Comparing `harlogger-2.1.2/LICENSE` & `harlogger-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `harlogger-2.1.2/PKG-INFO` & `harlogger-2.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: harlogger
-Version: 2.1.2
-Summary: Simple utility for sniffing decrypted HTTP/HTTPS traffic on an iDevice
-Home-page: https://github.com/doronz88/cfprefsmon
-Author: DoronZ
-Project-URL: pymobiledevice3, https://github.com/doronz88/cfprefsmon
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Description
 
 Simple pure python utility for sniffing HTTP/HTTPS decrypted traffic recorded by one of Apple's not-so-well documented
 APIs.
 
 # Installation
 
@@ -30,15 +15,15 @@
 framework. **This method doesn't include the request/response body.**
 
 ## Howto
 
 - Download Apple's CFNetwork profile which can be found here:
   https://developer.apple.com/services-account/download?path=/iOS/iOS_Logs/CFNetworkDiagnostics.mobileconfig
 
-- Install it via any way you prefer. I'm using `pymobiledevice3`:
+- Install it via any way you prefer. I'm using [`pymobiledevice3`](https://github.com/doronz88/pymobiledevice3):
 
     ```shell
     # if you don't already have it
     python3 -m pip install -U --user pymobiledevice3
     
     # install the profile
     pymobiledevice3 profile install CFNetworkDiagnostics.mobileconfig
@@ -118,7 +103,29 @@
 User-Agent: Mozilla/5.0 (iPhone; CPU iPhone OS 14_5_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.1 Mobile/15E148 Safari/604.1
 Referer: https://www.bing.com/
 Accept-Encoding: gzip, deflate, br
 Connection: keep-alive
 
 <ClientInstRequest><Events><E><T>Event.ClientInst</T><IG>EB94C422BC394F90A876D39A790BECBC</IG><TS>1634801882467</TS><D><![CDATA[[{"T":"CI.BoxModel","FID":"CI","Name":"v2.8","SV":"4","P":{"C":1,"N":5,"I":"5iv","S":"V","M":"V+L+M+MT+E+N+C+K+BD","T":1669960,"F":0},"V":"zrpx/////////visible/+zryw/////////hidden/@p"}]]]></D></E></Events><STS>1634801882467</STS></ClientInstRequest>
 ```
+
+# Enable HTTP instrumentation method
+
+Starting at iOS 15.0, the device will require the target process to have any of the following requirements:
+
+- `com.apple.private.cfnetwork.har-capture-delegation` entitlement
+- `get-task-allow` entitlement
+- `com.apple.security.get-task-allow` entitlement
+- OS build to be in `debug` mode
+
+In order to make the device enable HAR logging you may
+use [`pymobiledevice3`](https://github.com/doronz88/pymobiledevice3) as follows:
+
+```shell
+python3 -m pymobiledevice3 developer dvt har
+```
+
+Now you can start sniffing using the preference method:
+
+ ```shell
+python3 -m harlogger preference
+```
```

### Comparing `harlogger-2.1.2/harlogger/__main__.py` & `harlogger-2.1.3/harlogger/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,14 +192,15 @@
             },
             'entries': [],
         }
     }
 
     lockdown = LockdownClient(serial=udid)
     os_trace_service = OsTraceService(lockdown)
+    incomplete = ''
 
     try:
         for line in os_trace_service.syslog():
             if line.label is None:
                 continue
             if line.label.category != 'HAR':
                 continue
@@ -214,18 +215,24 @@
             if (len(images) > 0) and (image not in images):
                 continue
 
             if process_names and (posixpath.basename(line.filename) not in process_names):
                 continue
 
             try:
-                entry = json.loads(message)
+                entry = json.loads(incomplete + message)
+                incomplete = ''
             except json.decoder.JSONDecodeError:
-                print(f'failed to decode: {message}')
-                continue
+                if message.startswith('<incomplete>'):
+                    incomplete += message.split('<incomplete>', 1)[1]
+                    continue
+                elif len(incomplete) > 0:
+                    incomplete += message
+                    continue
+                raise
 
             # artificial HAR information extracted from syslog line
             entry['image'] = image
             entry['pid'] = pid
             entry['filename'] = line.filename
 
             if unique:
```

