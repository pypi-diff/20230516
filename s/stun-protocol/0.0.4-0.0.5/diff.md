# Comparing `tmp/stun-protocol-0.0.4.tar.gz` & `tmp/stun-protocol-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stun-protocol-0.0.4.tar", last modified: Wed Mar  9 01:12:29 2022, max compression
+gzip compressed data, was "stun-protocol-0.0.5.tar", last modified: Tue May 16 04:25:15 2023, max compression
```

## Comparing `stun-protocol-0.0.4.tar` & `stun-protocol-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2022-03-09 01:12:29.426061 stun-protocol-0.0.4/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2022-03-05 19:37:55.000000 stun-protocol-0.0.4/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4227 2022-03-09 01:12:29.426061 stun-protocol-0.0.4/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3613 2022-03-05 20:07:13.000000 stun-protocol-0.0.4/README.md
--rw-r--r--   0 nathan    (1000) nathan    (1000)      104 2022-03-05 20:03:02.000000 stun-protocol-0.0.4/pyproject.toml
--rw-r--r--   0 nathan    (1000) nathan    (1000)      698 2022-03-09 01:12:29.426061 stun-protocol-0.0.4/setup.cfg
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2022-03-09 01:12:29.416061 stun-protocol-0.0.4/stun_protocol/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2021-11-06 01:40:13.000000 stun-protocol-0.0.4/stun_protocol/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)    19748 2022-03-09 01:11:34.000000 stun-protocol-0.0.4/stun_protocol/attribute.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     6258 2022-03-09 01:11:34.000000 stun-protocol-0.0.4/stun_protocol/message.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2021-11-06 01:26:39.000000 stun-protocol-0.0.4/stun_protocol/stun.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2022-03-09 01:12:29.416061 stun-protocol-0.0.4/stun_protocol.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4227 2022-03-09 01:12:29.000000 stun-protocol-0.0.4/stun_protocol.egg-info/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)      298 2022-03-09 01:12:29.000000 stun-protocol-0.0.4/stun_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2022-03-09 01:12:29.000000 stun-protocol-0.0.4/stun_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)       14 2022-03-09 01:12:29.000000 stun-protocol-0.0.4/stun_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-16 04:25:15.053073 stun-protocol-0.0.5/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2022-03-05 19:37:55.000000 stun-protocol-0.0.5/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4190 2023-05-16 04:25:15.053073 stun-protocol-0.0.5/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3613 2022-03-05 20:07:13.000000 stun-protocol-0.0.5/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      104 2022-03-05 20:03:02.000000 stun-protocol-0.0.5/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      698 2023-05-16 04:25:15.053073 stun-protocol-0.0.5/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-16 04:25:15.053073 stun-protocol-0.0.5/stun_protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2021-11-06 01:40:13.000000 stun-protocol-0.0.5/stun_protocol/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    19748 2022-03-09 01:11:34.000000 stun-protocol-0.0.5/stun_protocol/attribute.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6925 2023-05-16 04:14:49.000000 stun-protocol-0.0.5/stun_protocol/message.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2021-11-06 01:26:39.000000 stun-protocol-0.0.5/stun_protocol/stun.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-16 04:25:15.053073 stun-protocol-0.0.5/stun_protocol.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4190 2023-05-16 04:25:15.000000 stun-protocol-0.0.5/stun_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      344 2023-05-16 04:25:15.000000 stun-protocol-0.0.5/stun_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-05-16 04:25:15.000000 stun-protocol-0.0.5/stun_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       14 2023-05-16 04:25:15.000000 stun-protocol-0.0.5/stun_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-05-16 04:25:15.053073 stun-protocol-0.0.5/tests/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    20003 2022-03-05 21:08:42.000000 stun-protocol-0.0.5/tests/test_attribute.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     9934 2023-05-16 04:15:54.000000 stun-protocol-0.0.5/tests/test_message.py
```

### Comparing `stun-protocol-0.0.4/LICENSE` & `stun-protocol-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stun-protocol-0.0.4/PKG-INFO` & `stun-protocol-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: stun-protocol
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for creating, parsing, and serializing STUN (RFC8489) packets
 Home-page: https://github.com/nbuckles13/python-stun-protocol
 Author: Carl Nathan Buckles
 Author-email: nbuckles@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/nbuckles13/python-stun-protocol/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -98,9 +96,7 @@
 # get a buffer from somewhere (perhaps received over a network)
 buffer = ...
 
 attr = create(buffer)
 ```
 
 There are various base classes for attributes starting with `Attribute` which is an abstract base class (`ABC`).  The module defines types for all attributes in the RFC, but the base classes allow for creating custom attributes as needed.
-
-
```

### Comparing `stun-protocol-0.0.4/README.md` & `stun-protocol-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stun-protocol-0.0.4/setup.cfg` & `stun-protocol-0.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stun-protocol
-version = 0.0.4
+version = 0.0.5
 author = Carl Nathan Buckles
 author_email = nbuckles@gmail.com
 description = A package for creating, parsing, and serializing STUN (RFC8489) packets
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nbuckles13/python-stun-protocol
 project_urls =
```

### Comparing `stun-protocol-0.0.4/stun_protocol/attribute.py` & `stun-protocol-0.0.5/stun_protocol/attribute.py`

 * *Files identical despite different names*

### Comparing `stun-protocol-0.0.4/stun_protocol/message.py` & `stun-protocol-0.0.5/stun_protocol/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import struct
 
 from enum import IntEnum
 from hashlib import sha1, sha256
 from typing import List, Type
 from stun_protocol import attribute
 
-from stun_protocol.attribute import Attribute, FingerprintAttribute, MessageIntegrityAttribute, MessageIntegritySha256Attribute
+from stun_protocol.attribute import Attribute, FingerprintAttribute, MessageIntegrityAttribute, \
+    MessageIntegritySha256Attribute, XorMappedAddressAttribute, MappedAddressAttributeBase
 
 
 class MessageClass(IntEnum):
     'https://datatracker.ietf.org/doc/html/rfc8489#section-5'
     REQUEST = 0b00
     INDICATION = 0b01
     SUCCESS_RESPONSE = 0b10
@@ -154,7 +155,19 @@
 
         # 2. pack the stun message
         packed_message = self.pack()
 
         # 3. run crc32 over the packed stun message, up to the start of the fingerprint attribute itself
         fpa_value = binascii.crc32(packed_message[0:-fpa.packed_length()], 0) ^ 0x5354554e
         self.attributes[-1].fingerprint = fpa_value
+
+    def add_xor_mapped_address_attribute_v4(self, port: int, address: int) -> None:
+        # 1. xor the port with the most 16 significant bits of the cookie
+        port = port ^ ((self.MAGIC_COOKIE & 0xFFFF0000) >> 16)
+
+        # 2. xor the address with the magic cookie and convert to bytes
+        address = address ^ self.MAGIC_COOKIE
+        address = address.to_bytes(length=4, byteorder='big')
+
+        # 3. add an XorMappedAddressAttribute with the calculated values
+        xmaa = XorMappedAddressAttribute(MappedAddressAttributeBase.family_ipv4, port, address)
+        self.add_attribute(xmaa)
```

### Comparing `stun-protocol-0.0.4/stun_protocol.egg-info/PKG-INFO` & `stun-protocol-0.0.5/stun_protocol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: stun-protocol
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for creating, parsing, and serializing STUN (RFC8489) packets
 Home-page: https://github.com/nbuckles13/python-stun-protocol
 Author: Carl Nathan Buckles
 Author-email: nbuckles@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/nbuckles13/python-stun-protocol/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -98,9 +96,7 @@
 # get a buffer from somewhere (perhaps received over a network)
 buffer = ...
 
 attr = create(buffer)
 ```
 
 There are various base classes for attributes starting with `Attribute` which is an abstract base class (`ABC`).  The module defines types for all attributes in the RFC, but the base classes allow for creating custom attributes as needed.
-
-
```

