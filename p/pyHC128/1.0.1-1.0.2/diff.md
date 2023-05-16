# Comparing `tmp/pyHC128-1.0.1.tar.gz` & `tmp/pyHC128-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHC128-1.0.1.tar", last modified: Tue May 16 12:36:09 2023, max compression
+gzip compressed data, was "pyHC128-1.0.2.tar", last modified: Tue May 16 13:20:10 2023, max compression
```

## Comparing `pyHC128-1.0.1.tar` & `pyHC128-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:36:09.878791 pyHC128-1.0.1/
--rw-rw-rw-   0        0        0      429 2023-05-16 12:36:09.872286 pyHC128-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-16 12:34:23.000000 pyHC128-1.0.1/README.md
--rw-rw-rw-   0        0        0     3715 2023-05-15 18:53:02.000000 pyHC128-1.0.1/hc128.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:36:09.872286 pyHC128-1.0.1/pyHC128.egg-info/
--rw-rw-rw-   0        0        0      429 2023-05-16 12:36:09.000000 pyHC128-1.0.1/pyHC128.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-16 12:36:09.000000 pyHC128-1.0.1/pyHC128.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:36:09.000000 pyHC128-1.0.1/pyHC128.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 12:36:09.000000 pyHC128-1.0.1/pyHC128.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 12:36:09.878791 pyHC128-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      439 2023-05-16 12:33:40.000000 pyHC128-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:20:10.221126 pyHC128-1.0.2/
+-rw-rw-rw-   0        0        0      429 2023-05-16 13:20:10.221126 pyHC128-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-16 12:34:23.000000 pyHC128-1.0.2/README.md
+-rw-rw-rw-   0        0        0     3862 2023-05-16 13:15:40.000000 pyHC128-1.0.2/hc128.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:20:10.221126 pyHC128-1.0.2/pyHC128.egg-info/
+-rw-rw-rw-   0        0        0      429 2023-05-16 13:20:10.000000 pyHC128-1.0.2/pyHC128.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-05-16 13:20:10.000000 pyHC128-1.0.2/pyHC128.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:20:10.000000 pyHC128-1.0.2/pyHC128.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 13:20:10.000000 pyHC128-1.0.2/pyHC128.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:20:10.221126 pyHC128-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      439 2023-05-16 13:16:48.000000 pyHC128-1.0.2/setup.py
```

### Comparing `pyHC128-1.0.1/hc128.py` & `pyHC128-1.0.2/hc128.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,9 +97,12 @@
         keystream_bytes = self.generate_keystream_bytes(len(data))
         encrypted_data = bytearray(data)
         for i in range(len(data)):
             encrypted_data[i] ^= keystream_bytes[i]
         return bytes(encrypted_data)
 
     def decrypt(self, data: bytes) -> bytes:
-        # Todo: Optimization, extend and drink coffee
-        return self.encrypt(data)
+        keystream_bytes = self.generate_keystream_bytes(len(data))
+        decrypted_data = bytearray(data)
+        for i in range(len(data)):
+            decrypted_data[i] ^= keystream_bytes[i]
+        return bytes(decrypted_data)
```

