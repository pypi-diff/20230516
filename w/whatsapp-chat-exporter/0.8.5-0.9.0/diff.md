# Comparing `tmp/whatsapp-chat-exporter-0.8.5.tar.gz` & `tmp/whatsapp-chat-exporter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chat-exporter-0.8.5.tar", last modified: Tue Jan 31 10:08:24 2023, max compression
+gzip compressed data, was "whatsapp-chat-exporter-0.9.0.tar", last modified: Tue May 16 11:47:37 2023, max compression
```

## Comparing `whatsapp-chat-exporter-0.8.5.tar` & `whatsapp-chat-exporter-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:08:24.500593 whatsapp-chat-exporter-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-01-31 10:08:24.500593 whatsapp-chat-exporter-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:08:24.496593 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20016 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/extract_iphone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/extract_iphone_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/whatsapp.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 10:08:24.500593 whatsapp-chat-exporter-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-31 10:08:13.000000 whatsapp-chat-exporter-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:08:24.500593 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-01-31 10:08:24.000000 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-31 10:08:24.000000 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 10:08:24.000000 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 10:08:24.000000 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-31 10:08:24.000000 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-31 10:08:24.000000 whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/whatsapp.html
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/top_level.txt
```

### Comparing `whatsapp-chat-exporter-0.8.5/LICENSE` & `whatsapp-chat-exporter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.8.5/PKG-INFO` & `whatsapp-chat-exporter-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,24 @@
-Metadata-Version: 2.1
-Name: whatsapp-chat-exporter
-Version: 0.8.5
-Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
-Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
-Author: KnugiHK
-Author-email: info@knugi.com
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Utilities
-Classifier: Topic :: Database
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: android_backup
-Provides-Extra: crypt12
-Provides-Extra: crypt14
-Provides-Extra: crypt15
-License-File: LICENSE
-
 # Whatsapp-Chat-Exporter
 [![Latest in Pypi](https://img.shields.io/pypi/v/whatsapp-chat-exporter?label=Latest%20in%20Pypi)](https://pypi.org/project/whatsapp-chat-exporter/)
 ![License MIT](https://img.shields.io/pypi/l/whatsapp-chat-exporter)
 [![Python](https://img.shields.io/pypi/pyversions/Whatsapp-Chat-Exporter)](https://pypi.org/project/Whatsapp-Chat-Exporter/)
 
-A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.  
+A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Inspired by [Telegram Chat Export Tool](https://telegram.org/blog/export-and-more).  
 **If you plan to uninstall WhatsApp or delete your WhatsApp account, please make a backup of your WhatsApp database. You may want to use this exporter again on the same database in the future as the exporter develops**
 
 # Usage
 **Usage in README may be removed in the future. Check the usage in [Wiki](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/wiki)**.
 
 **If you want to use the old release (< 0.5) of the exporter, please follow the [old usage guide](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/wiki/Old-Usage#usage)**.
 
 First, install the exporter by:
 ```shell
 pip install whatsapp-chat-exporter
-pip install whatsapp-chat-exporter[android_backup]  & :: Optional, if you want it to support decrypting Android WhatsApp backup.
+pip install whatsapp-chat-exporter[android_backup]  :; # Optional, if you want it to support decrypting Android WhatsApp backup.
 ```
 Then, create a working directory in somewhere you want
 ```shell
 mkdir working_wts
 cd working_wts
 ```
 ## Working with Android
@@ -65,14 +38,15 @@
 
 ### Encrypted Android WhatsApp Backup
 In order to support the decryption, install pycryptodome if it is not installed
 ```sh
 pip install pycryptodome # Or 
 pip install whatsapp-chat-exporter["android_backup"] # install along with this software
 ```
+### Crypt15 is now the easiest way to decrypt a backup. If you have the 32 bytes hex key generated when you enable End-to-End encrypted backup, you can use it to decrypt the backup. If you do not have the 32 bytes hex key, you can still use the key file extracted just like extacting key file for Crypt12 and Crypt14 to decrypt the backup.
 #### Crypt12 or Crypt14
 Place the decryption key file (key) and the encrypted WhatsApp Backup (msgstore.db.crypt14) in the working directory. If you also want the name of your contacts, get the contact database, which is called wa.db. And copy the WhatsApp (Media) directory from your phone directly.
 
 And now, you should have something like this in the working directory.
 
 ![Android folder structure with WhatsApp Backup](imgs/android_structure_backup.png)
 #### Extracting
@@ -126,34 +100,41 @@
 #### Group Message
 ![Group Message](imgs/group.png)
 
 ## More options
 Invoke the wtsexporter with --help option will show you all options available.
 ```sh
 > wtsexporter --help
-Usage: wtsexporter [options]
+usage: wtsexporter [options]
 
-Options:
-  --version             show program's version number and exit
+options:
   -h, --help            show this help message and exit
   -a, --android         Define the target as Android
-  -i, --iphone          Define the target as iPhone
-  -w WA, --wa=WA        Path to contact database
-  -m MEDIA, --media=MEDIA
-                        Path to WhatsApp media folder
-  -b BACKUP, --backup=BACKUP
-                        Path to Android (must be used together with -k)/iPhone
-                        WhatsApp backup
-  -o OUTPUT, --output=OUTPUT
-                        Output to specific directory
-  -j, --json            Save the result to a single JSON file
-  -d DB, --db=DB        Path to database file
-  -k KEY, --key=KEY     Path to key file
-  -t TEMPLATE, --template=TEMPLATE
+  -i, --iphone, --ios   Define the target as iPhone
+  -w WA, --wa WA        Path to contact database (default: wa.db/ContactsV2.sqlite)
+  -m MEDIA, --media MEDIA
+                        Path to WhatsApp media folder (default: WhatsApp)
+  -b BACKUP, --backup BACKUP
+                        Path to Android (must be used together with -k)/iPhone WhatsApp backup
+  -o OUTPUT, --output OUTPUT
+                        Output to specific directory (default: result)
+  -j [JSON], --json [JSON]
+                        Save the result to a single JSON file (default if present: result.json)
+  -d DB, --db DB        Path to database file (default: msgstore.db/7c7fba66680ef796b916b067077cc246adacf01d)
+  -k KEY, --key KEY     Path to key file
+  -t TEMPLATE, --template TEMPLATE
                         Path to custom HTML template
+  -e, --embedded        Embed media into HTML file (not yet implemented)
+  -s, --showkey         Show the HEX key used to decrypt the database
+  -c, --move-media      Move the media directory to output directory if the flag is set, otherwise copy it
+  --offline OFFLINE     Relative path to offline static files
+  --size SIZE, --output-size SIZE
+                        Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
+  --no-html             Do not output html files
+  --check-update        Check for updates
 ```
 
 # To do
 1. Reply in iPhone
 
 # Copyright
 This is a MIT licensed project.
```

### Comparing `whatsapp-chat-exporter-0.8.5/README.md` & `whatsapp-chat-exporter-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,55 @@
+Metadata-Version: 2.1
+Name: whatsapp-chat-exporter
+Version: 0.9.0
+Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
+Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
+Author: KnugiHK
+Author-email: hello@knugi.com
+License: MIT
+Keywords: android,ios,parsing,history,iphone,whatsapp,messagecustomizable,android-backup,crypt12,whatsapp-chat-exporter,whatsapp-export,whatsapp-database,whatsapp-database-parser,whatsapp-conversations,iphone-backup,crypt14,crypt15,messages
+Platform: any
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Utilities
+Classifier: Topic :: Database
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: android_backup
+Provides-Extra: crypt12
+Provides-Extra: crypt14
+Provides-Extra: crypt15
+License-File: LICENSE
+
 # Whatsapp-Chat-Exporter
 [![Latest in Pypi](https://img.shields.io/pypi/v/whatsapp-chat-exporter?label=Latest%20in%20Pypi)](https://pypi.org/project/whatsapp-chat-exporter/)
 ![License MIT](https://img.shields.io/pypi/l/whatsapp-chat-exporter)
 [![Python](https://img.shields.io/pypi/pyversions/Whatsapp-Chat-Exporter)](https://pypi.org/project/Whatsapp-Chat-Exporter/)
 
-A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.  
+A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Inspired by [Telegram Chat Export Tool](https://telegram.org/blog/export-and-more).  
 **If you plan to uninstall WhatsApp or delete your WhatsApp account, please make a backup of your WhatsApp database. You may want to use this exporter again on the same database in the future as the exporter develops**
 
 # Usage
 **Usage in README may be removed in the future. Check the usage in [Wiki](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/wiki)**.
 
 **If you want to use the old release (< 0.5) of the exporter, please follow the [old usage guide](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/wiki/Old-Usage#usage)**.
 
 First, install the exporter by:
 ```shell
 pip install whatsapp-chat-exporter
-pip install whatsapp-chat-exporter[android_backup]  & :: Optional, if you want it to support decrypting Android WhatsApp backup.
+pip install whatsapp-chat-exporter[android_backup]  :; # Optional, if you want it to support decrypting Android WhatsApp backup.
 ```
 Then, create a working directory in somewhere you want
 ```shell
 mkdir working_wts
 cd working_wts
 ```
 ## Working with Android
@@ -38,14 +69,15 @@
 
 ### Encrypted Android WhatsApp Backup
 In order to support the decryption, install pycryptodome if it is not installed
 ```sh
 pip install pycryptodome # Or 
 pip install whatsapp-chat-exporter["android_backup"] # install along with this software
 ```
+### Crypt15 is now the easiest way to decrypt a backup. If you have the 32 bytes hex key generated when you enable End-to-End encrypted backup, you can use it to decrypt the backup. If you do not have the 32 bytes hex key, you can still use the key file extracted just like extacting key file for Crypt12 and Crypt14 to decrypt the backup.
 #### Crypt12 or Crypt14
 Place the decryption key file (key) and the encrypted WhatsApp Backup (msgstore.db.crypt14) in the working directory. If you also want the name of your contacts, get the contact database, which is called wa.db. And copy the WhatsApp (Media) directory from your phone directly.
 
 And now, you should have something like this in the working directory.
 
 ![Android folder structure with WhatsApp Backup](imgs/android_structure_backup.png)
 #### Extracting
@@ -99,34 +131,41 @@
 #### Group Message
 ![Group Message](imgs/group.png)
 
 ## More options
 Invoke the wtsexporter with --help option will show you all options available.
 ```sh
 > wtsexporter --help
-Usage: wtsexporter [options]
+usage: wtsexporter [options]
 
-Options:
-  --version             show program's version number and exit
+options:
   -h, --help            show this help message and exit
   -a, --android         Define the target as Android
-  -i, --iphone          Define the target as iPhone
-  -w WA, --wa=WA        Path to contact database
-  -m MEDIA, --media=MEDIA
-                        Path to WhatsApp media folder
-  -b BACKUP, --backup=BACKUP
-                        Path to Android (must be used together with -k)/iPhone
-                        WhatsApp backup
-  -o OUTPUT, --output=OUTPUT
-                        Output to specific directory
-  -j, --json            Save the result to a single JSON file
-  -d DB, --db=DB        Path to database file
-  -k KEY, --key=KEY     Path to key file
-  -t TEMPLATE, --template=TEMPLATE
+  -i, --iphone, --ios   Define the target as iPhone
+  -w WA, --wa WA        Path to contact database (default: wa.db/ContactsV2.sqlite)
+  -m MEDIA, --media MEDIA
+                        Path to WhatsApp media folder (default: WhatsApp)
+  -b BACKUP, --backup BACKUP
+                        Path to Android (must be used together with -k)/iPhone WhatsApp backup
+  -o OUTPUT, --output OUTPUT
+                        Output to specific directory (default: result)
+  -j [JSON], --json [JSON]
+                        Save the result to a single JSON file (default if present: result.json)
+  -d DB, --db DB        Path to database file (default: msgstore.db/7c7fba66680ef796b916b067077cc246adacf01d)
+  -k KEY, --key KEY     Path to key file
+  -t TEMPLATE, --template TEMPLATE
                         Path to custom HTML template
+  -e, --embedded        Embed media into HTML file (not yet implemented)
+  -s, --showkey         Show the HEX key used to decrypt the database
+  -c, --move-media      Move the media directory to output directory if the flag is set, otherwise copy it
+  --offline OFFLINE     Relative path to offline static files
+  --size SIZE, --output-size SIZE
+                        Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
+  --no-html             Do not output html files
+  --check-update        Check for updates
 ```
 
 # To do
 1. Reply in iPhone
 
 # Copyright
 This is a MIT licensed project.
```

### Comparing `whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/extract.py` & `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_new.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,45 +12,50 @@
 from bleach import clean as sanitize
 from markupsafe import Markup
 from datetime import datetime
 from enum import Enum
 from mimetypes import MimeTypes
 from hashlib import sha256
 
+from Whatsapp_Chat_Exporter.data_model import ChatStore, Message
+
 try:
     import zlib
     from Crypto.Cipher import AES
 except ModuleNotFoundError:
     support_backup = False
 else:
     support_backup = True
 try:
     import javaobj
 except ModuleNotFoundError:
     support_crypt15 = False
 else:
     support_crypt15 = True
 
+
 def sanitize_except(html):
     return Markup(sanitize(html, tags=["br"]))
 
 
 def determine_day(last, current):
     last = datetime.fromtimestamp(last).date()
     current = datetime.fromtimestamp(current).date()
     if last == current:
         return None
     else:
         return current
 
-CRYPT14_OFFSETS = [
+
+CRYPT14_OFFSETS = (
     {"iv": 67, "db": 191},
     {"iv": 67, "db": 190},
-    {"iv": 66, "db": 99}
-]
+    {"iv": 66, "db": 99},
+    {"iv": 67, "db": 193}
+)
 
 
 class Crypt(Enum):
     CRYPT15 = 15
     CRYPT14 = 14
     CRYPT12 = 12
 
@@ -67,26 +72,26 @@
             b'\x00' * 32,
             key_stream,
             sha256
         ).digest(),
         b"backup encryption\x01",
         sha256
     )
-    return key.digest()
+    return key.digest(), key_stream
 
 
 def _extract_encrypted_key(keyfile):
     key_stream = b""
     for byte in javaobj.loads(keyfile):
         key_stream += byte.to_bytes(1, "big", signed=True)
 
     return _generate_hmac_of_hmac(key_stream)
-    
 
-def decrypt_backup(database, key, output, crypt=Crypt.CRYPT14):
+
+def decrypt_backup(database, key, output, crypt=Crypt.CRYPT14, show_crypt15=False):
     if not support_backup:
         return 1
     if isinstance(key, io.IOBase):
         key = key.read()
         if crypt is not Crypt.CRYPT15:
             t1 = key[30:62]
     if crypt is not Crypt.CRYPT15 and len(key) != 158:
@@ -116,17 +121,20 @@
         db_ciphertext = database[db_offset:]
 
     if t1 != t2:
         raise ValueError("The signature of key file and backup file mismatch")
 
     if crypt == Crypt.CRYPT15:
         if len(key) == 32:
-            main_key = _generate_hmac_of_hmac(key)
+            main_key, hex_key = _generate_hmac_of_hmac(key)
         else:
-            main_key = _extract_encrypted_key(key)
+            main_key, hex_key = _extract_encrypted_key(key)
+        if show_crypt15:
+            hex_key = [hex_key.hex()[c:c+4] for c in range(0, len(hex_key.hex()), 4)]
+            print("The HEX key of the crypt15 backup is: " + ' '.join(hex_key))
     else:
         main_key = key[126:]
     decompressed = False
     while not decompressed:
         cipher = AES.new(main_key, AES.MODE_GCM, iv)
         db_compressed = cipher.decrypt(db_ciphertext)
         try:
@@ -180,165 +188,180 @@
     c.execute("""SELECT count() FROM wa_contacts""")
     total_row_number = c.fetchone()[0]
     print(f"Gathering contacts...({total_row_number})")
 
     c.execute("""SELECT jid, display_name FROM wa_contacts; """)
     row = c.fetchone()
     while row is not None:
-        data[row[0]] = {"name": row[1], "messages": {}}
+        data[row["jid"]] = ChatStore(row["display_name"])
         row = c.fetchone()
 
 
 def messages(db, data):
     # Get message history
     c = db.cursor()
-    c.execute("""SELECT count() FROM messages""")
+    c.execute("""SELECT count() FROM message""")
     total_row_number = c.fetchone()[0]
     print(f"Gathering messages...(0/{total_row_number})", end="\r")
 
     phone_number_re = re.compile(r"[0-9]+@s.whatsapp.net")
-    c.execute("""SELECT messages.key_remote_jid,
-                        messages._id,
-                        messages.key_from_me,
-                        messages.timestamp,
-                        messages.data,
-                        messages.status,
-                        messages.edit_version,
-                        messages.thumb_image,
-                        messages.remote_resource,
-                        messages.media_wa_type,
-                        messages.latitude,
-                        messages.longitude,
-                        messages_quotes.key_id as quoted,
-                        messages.key_id,
-                        messages_quotes.data,
-                        messages.media_caption
-                 FROM messages
-                    LEFT JOIN messages_quotes
-                        ON messages.quoted_row_id = messages_quotes._id
-                 WHERE messages.key_remote_jid <> '-1';""")
+    c.execute("""SELECT jid_global.raw_string as key_remote_jid,
+                        message._id,
+                        message.from_me as key_from_me,
+                        message.timestamp,
+                        message.text_data as data,
+                        message.status,
+                        message_future.version as edit_version,
+                        message_thumbnail.thumbnail as thumb_image,
+                        message_media.file_path as remote_resource,
+                        message_media.mime_type as media_wa_type,
+                        message_location.latitude,
+                        message_location.longitude,
+                        message_quoted.key_id as quoted,
+                        message.key_id,
+                        message_quoted.text_data as quoted_data,
+                        message.message_type,
+                        jid_group.raw_string as group_sender_jid,
+                        chat.subject as chat_subject
+                 FROM message
+                    LEFT JOIN message_quoted
+                        ON message_quoted.message_row_id = message._id
+                    LEFT JOIN message_location
+                        ON message_location.message_row_id = message._id
+                    LEFT JOIN message_media
+                        ON message_media.message_row_id = message._id
+                    LEFT JOIN message_thumbnail
+                        ON message_thumbnail.message_row_id = message._id
+                    LEFT JOIN message_future
+                        ON message_future.message_row_id = message._id
+                    LEFT JOIN chat
+                        ON chat._id = message.chat_row_id
+                    INNER JOIN jid jid_global
+                        ON jid_global._id = chat.jid_row_id
+                    LEFT JOIN jid jid_group
+                        ON jid_group._id = message.sender_jid_row_id
+                    WHERE key_remote_jid <> '-1';""")
     i = 0
     content = c.fetchone()
     while content is not None:
-        if content[0] not in data:
-            data[content[0]] = {"name": None, "messages": {}}
-        data[content[0]]["messages"][content[1]] = {
-            "from_me": bool(content[2]),
-            "timestamp": content[3]/1000,
-            "time": datetime.fromtimestamp(content[3]/1000).strftime("%H:%M"),
-            "media": False,
-            "key_id": content[13],
-            "meta": False,
-            "data": None
-        }
-        if "-" in content[0] and content[2] == 0:
+        if content["key_remote_jid"] not in data:
+            data[content["key_remote_jid"]] = ChatStore()
+        if content["key_remote_jid"] is None:
+            continue
+        data[content["key_remote_jid"]].add_message(content["_id"], Message(
+            from_me=content["key_from_me"],
+            timestamp=content["timestamp"],
+            time=content["timestamp"],
+            key_id=content["key_id"],
+        ))
+        if "-" in content["key_remote_jid"] and content["key_from_me"] == 0:
             name = None
-            if content[8] in data:
-                name = data[content[8]]["name"]
-                if "@" in content[8]:
-                    fallback = content[8].split('@')[0]
-                else:
-                    fallback = None
+            if content["chat_subject"] is not None:
+                _jid = content["group_sender_jid"]
+            else:
+                _jid = content["key_remote_jid"]
+            if _jid in data:
+                name = data[_jid].name
+                fallback = _jid.split('@')[0] if "@" in _jid else None
             else:
                 fallback = None
-
-            data[content[0]]["messages"][content[1]]["sender"] = name or fallback
+            data[content["key_remote_jid"]].messages[content["_id"]].sender = name or fallback
         else:
-            data[content[0]]["messages"][content[1]]["sender"] = None
+            data[content["key_remote_jid"]].messages[content["_id"]].sender = None
 
-        if content[12] is not None:
-            data[content[0]]["messages"][content[1]]["reply"] = content[12]
-            data[content[0]]["messages"][content[1]]["quoted_data"] = content[14]
+        if content["quoted"] is not None:
+            data[content["key_remote_jid"]].messages[content["_id"]].reply = content["quoted"]
+            data[content["key_remote_jid"]].messages[content["_id"]].quoted_data = content["quoted_data"]
         else:
-            data[content[0]]["messages"][content[1]]["reply"] = None
+            data[content["key_remote_jid"]].messages[content["_id"]].reply = None
 
-        if content[15] is not None:
-            data[content[0]]["messages"][content[1]]["caption"] = content[15]
+        if content["message_type"] == 1:
+            data[content["key_remote_jid"]].messages[content["_id"]].caption = content["data"]
         else:
-            data[content[0]]["messages"][content[1]]["caption"] = None
+            data[content["key_remote_jid"]].messages[content["_id"]].caption = None
 
-        if content[5] == 6:
-            if "-" in content[0]:
+        if content["status"] == 6:
+            if content["chat_subject"] is not None:
                 # Is Group
-                if content[4] is not None:
+                if content["data"] is not None:
                     try:
-                        int(content[4])
+                        int(content["data"])
                     except ValueError:
-                        msg = f"The group name changed to {content[4]}"
-                        data[content[0]]["messages"][content[1]]["data"] = msg
-                        data[content[0]]["messages"][content[1]]["meta"] = True
+                        msg = f"The group name changed to {content['data']}"
+                        data[content["key_remote_jid"]].messages[content["_id"]].data = msg
+                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
                     else:
-                        del data[content[0]]["messages"][content[1]]
+                        data[content["key_remote_jid"]].delete_message(content["_id"])
                 else:
-                    thumb_image = content[7]
+                    thumb_image = content["thumb_image"]
                     if thumb_image is not None:
                         if b"\x00\x00\x01\x74\x00\x1A" in thumb_image:
                             # Add user
                             added = phone_number_re.search(
                                 thumb_image.decode("unicode_escape"))[0]
                             if added in data:
                                 name_right = data[added]["name"]
                             else:
                                 name_right = added.split('@')[0]
-                            if content[8] is not None:
-                                if content[8] in data:
-                                    name_left = data[content[8]]["name"]
+                            if content["remote_resource"] is not None:
+                                if content["remote_resource"] in data:
+                                    name_left = data[content["remote_resource"]]["name"]
                                 else:
-                                    name_left = content[8].split('@')[0]
+                                    name_left = content["remote_resource"].split('@')[0]
                                 msg = f"{name_left} added {name_right or 'You'}"
                             else:
                                 msg = f"Added {name_right or 'You'}"
                         elif b"\xac\xed\x00\x05\x74\x00" in thumb_image:
                             # Changed number
-                            original = content[8].split('@')[0]
+                            original = content["remote_resource"].split('@')[0]
                             changed = thumb_image[7:].decode().split('@')[0]
                             msg = f"{original} changed to {changed}"
-                        data[content[0]]["messages"][content[1]]["data"] = msg
-                        data[content[0]]["messages"][content[1]]["meta"] = True
+                        data[content["key_remote_jid"]].messages[content["_id"]].data = msg
+                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
                     else:
-                        if content[4] is None:
-                            del data[content[0]]["messages"][content[1]]
+                        if content["data"] is None:
+                            data[content["key_remote_jid"]].delete_message(content["_id"])
             else:
                 # Private chat
-                if content[4] is None and content[7] is None:
-                    del data[content[0]]["messages"][content[1]]
+                if content["data"] is None and content["thumb_image"] is None:
+                    data[content["key_remote_jid"]].delete_message(content["_id"])
 
         else:
-            if content[2] == 1:
-                if content[5] == 5 and content[6] == 7:
+            if content["key_from_me"] == 1:
+                if content["status"] == 5 and content["edit_version"] == 7:
                     msg = "Message deleted"
-                    data[content[0]]["messages"][content[1]]["meta"] = True
+                    data[content["key_remote_jid"]].messages[content["_id"]].meta = True
                 else:
-                    if content[9] == "5":
+                    if content["media_wa_type"] == "5":
                         msg = f"Location shared: {content[10], content[11]}"
-                        data[content[0]]["messages"][content[1]]["meta"] = True
+                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
                     else:
-                        msg = content[4]
+                        msg = content["data"]
                         if msg is not None:
                             if "\r\n" in msg:
                                 msg = msg.replace("\r\n", "<br>")
                             if "\n" in msg:
                                 msg = msg.replace("\n", "<br>")
             else:
-                if content[5] == 0 and content[6] == 7:
+                if content["status"] == 0 and content["edit_version"] == 7:
                     msg = "Message deleted"
-                    data[content[0]]["messages"][content[1]]["meta"] = True
+                    data[content["key_remote_jid"]].messages[content["_id"]].meta = True
                 else:
-                    if content[9] == "5":
+                    if content["media_wa_type"] == "5":
                         msg = f"Location shared: {content[10], content[11]}"
-                        data[content[0]]["messages"][content[1]]["meta"] = True
+                        data[content["key_remote_jid"]].messages[content["_id"]].meta = True
                     else:
-                        msg = content[4]
+                        msg = content["data"]
                         if msg is not None:
                             if "\r\n" in msg:
                                 msg = msg.replace("\r\n", "<br>")
                             if "\n" in msg:
                                 msg = msg.replace("\n", "<br>")
 
-            data[content[0]]["messages"][content[1]]["data"] = msg
+            data[content["key_remote_jid"]].messages[content["_id"]].data = msg
 
         i += 1
         if i % 1000 == 0:
             print(f"Gathering messages...({i}/{total_row_number})", end="\r")
         content = c.fetchone()
     print(f"Gathering messages...({total_row_number}/{total_row_number})", end="\r")
 
@@ -346,93 +369,108 @@
 def media(db, data, media_folder):
     # Get media
     c = db.cursor()
     c.execute("""SELECT count() FROM message_media""")
     total_row_number = c.fetchone()[0]
     print(f"\nGathering media...(0/{total_row_number})", end="\r")
     i = 0
-    c.execute("""SELECT messages.key_remote_jid,
+    c.execute("""SELECT jid.raw_string,
                         message_row_id,
                         file_path,
                         message_url,
                         mime_type,
                         media_key
                  FROM message_media
-                    INNER JOIN messages
-                        ON message_media.message_row_id = messages._id
-                ORDER BY messages.key_remote_jid ASC""")
+                    INNER JOIN message
+                        ON message_media.message_row_id = message._id
+                    LEFT JOIN chat
+                        ON chat._id = message.chat_row_id
+                    INNER JOIN jid
+                        ON jid._id = chat.jid_row_id
+                 ORDER BY jid.raw_string ASC""")
     content = c.fetchone()
     mime = MimeTypes()
     while content is not None:
-        file_path = f"{media_folder}/{content[2]}"
-        data[content[0]]["messages"][content[1]]["media"] = True
+        file_path = f"{media_folder}/{content['file_path']}"
+        data[content["raw_string"]].messages[content["message_row_id"]].media = True
         if os.path.isfile(file_path):
-            data[content[0]]["messages"][content[1]]["data"] = file_path
-            if content[4] is None:
+            data[content["raw_string"]].messages[content["message_row_id"]].data = file_path
+            if content["mime_type"] is None:
                 guess = mime.guess_type(file_path)[0]
                 if guess is not None:
-                    data[content[0]]["messages"][content[1]]["mime"] = guess
+                    data[content["raw_string"]].messages[content["message_row_id"]].mime = guess
                 else:
-                    data[content[0]]["messages"][content[1]]["mime"] = "data/data"
+                    data[content["raw_string"]].messages[content["message_row_id"]].mime = "data/data"
             else:
-                data[content[0]]["messages"][content[1]]["mime"] = content[4]
+                data[content["raw_string"]].messages[content["message_row_id"]].mime = content["mime_type"]
         else:
-            # if "https://mmg" in content[4]:
+            # if "https://mmg" in content["mime_type"]:
             # try:
-            # r = requests.get(content[3])
+            # r = requests.get(content["message_url"])
             # if r.status_code != 200:
             # raise RuntimeError()
             # except:
-            # data[content[0]]["messages"][content[1]]["data"] = "{The media is missing}"
-            # data[content[0]]["messages"][content[1]]["media"] = True
-            # data[content[0]]["messages"][content[1]]["mime"] = "media"
+            # data[content["raw_string"]].messages[content["message_row_id"]].data = "{The media is missing}"
+            # data[content["raw_string"]].messages[content["message_row_id"]].media = True
+            # data[content["raw_string"]].messages[content["message_row_id"]].mime = "media"
             # else:
-            data[content[0]]["messages"][content[1]]["data"] = "The media is missing"
-            data[content[0]]["messages"][content[1]]["mime"] = "media"
-            data[content[0]]["messages"][content[1]]["meta"] = True
+            data[content["raw_string"]].messages[content["message_row_id"]].data = "The media is missing"
+            data[content["raw_string"]].messages[content["message_row_id"]].mime = "media"
+            data[content["raw_string"]].messages[content["message_row_id"]].meta = True
         i += 1
         if i % 100 == 0:
             print(f"Gathering media...({i}/{total_row_number})", end="\r")
         content = c.fetchone()
     print(
         f"Gathering media...({total_row_number}/{total_row_number})", end="\r")
 
 
 def vcard(db, data):
     c = db.cursor()
     c.execute("""SELECT message_row_id,
-                        messages.key_remote_jid,
+                        jid.raw_string,
                         vcard,
-                        messages.media_name
-                 FROM messages_vcards
-                    INNER JOIN messages
-                        ON messages_vcards.message_row_id = messages._id
-                 ORDER BY messages.key_remote_jid ASC;""")
+                        message.text_data
+                 FROM message_vcard
+                    INNER JOIN message
+                        ON message_vcard.message_row_id = message._id
+                    LEFT JOIN chat
+                        ON chat._id = message.chat_row_id
+                    INNER JOIN jid
+                        ON jid._id = chat.jid_row_id
+                 ORDER BY message.chat_row_id ASC;""")
     rows = c.fetchall()
     total_row_number = len(rows)
     print(f"\nGathering vCards...(0/{total_row_number})", end="\r")
     base = "WhatsApp/vCards"
     if not os.path.isdir(base):
         Path(base).mkdir(parents=True, exist_ok=True)
     for index, row in enumerate(rows):
-        media_name = row[3] if row[3] else ""
+        media_name = row["text_data"] if row["text_data"] else ""
         file_name = "".join(x for x in media_name if x.isalnum())
         file_path = f"{base}/{file_name}.vcf"
         if not os.path.isfile(file_path):
             with open(file_path, "w", encoding="utf-8") as f:
-                f.write(row[2])
-        data[row[1]]["messages"][row[0]]["data"] = media_name + \
+                f.write(row["vcard"])
+        data[row["raw_string"]].messages[row["message_row_id"]].data = media_name + \
             "The vCard file cannot be displayed here, " \
             f"however it should be located at {file_path}"
-        data[row[1]]["messages"][row[0]]["mime"] = "text/x-vcard"
-        data[row[1]]["messages"][row[0]]["meta"] = True
+        data[row["raw_string"]].messages[row["message_row_id"]].mime = "text/x-vcard"
+        data[row["raw_string"]].messages[row["message_row_id"]].meta = True
         print(f"Gathering vCards...({index + 1}/{total_row_number})", end="\r")
 
 
-def create_html(data, output_folder, template=None, embedded=False):
+def create_html(
+        data,
+        output_folder,
+        template=None,
+        embedded=False,
+        offline_static=False,
+        maximum_size=None
+    ):
     if template is None:
         template_dir = os.path.dirname(__file__)
         template_file = "whatsapp.html"
     else:
         template_dir = os.path.dirname(template)
         template_file = os.path.basename(template)
     templateLoader = jinja2.FileSystemLoader(searchpath=template_dir)
@@ -443,39 +481,52 @@
 
     total_row_number = len(data)
     print(f"\nCreating HTML...(0/{total_row_number})", end="\r")
 
     if not os.path.isdir(output_folder):
         os.mkdir(output_folder)
 
+    w3css = "https://www.w3schools.com/w3css/4/w3.css"
+    if offline_static:
+        import urllib.request
+        static_folder = os.path.join(output_folder, offline_static)
+        if not os.path.isdir(static_folder):
+            os.mkdir(static_folder)
+        w3css_path = os.path.join(static_folder, "w3.css")
+        if not os.path.isfile(w3css_path):
+            with urllib.request.urlopen(w3css) as resp:
+                with open(w3css_path, "wb") as f: f.write(resp.read())
+        w3css = os.path.join(offline_static, "w3.css")
+
     for current, contact in enumerate(data):
-        if len(data[contact]["messages"]) == 0:
+        if len(data[contact].messages) == 0:
             continue
         phone_number = contact.split('@')[0]
         if "-" in contact:
             file_name = ""
         else:
             file_name = phone_number
 
-        if data[contact]["name"] is not None:
+        if data[contact].name is not None:
             if file_name != "":
                 file_name += "-"
-            file_name += data[contact]["name"].replace("/", "-")
-            name = data[contact]["name"]
+            file_name += data[contact].name.replace("/", "-")
+            name = data[contact].name
         else:
             name = phone_number
-        safe_file_name = ''
+
         safe_file_name = "".join(x for x in file_name if x.isalnum() or x in "- ")
         with open(f"{output_folder}/{safe_file_name}.html", "w", encoding="utf-8") as f:
             f.write(
                 template.render(
                     name=name,
-                    msgs=data[contact]["messages"].values(),
+                    msgs=data[contact].messages.values(),
                     my_avatar=None,
-                    their_avatar=f"WhatsApp/Avatars/{contact}.j"
+                    their_avatar=f"WhatsApp/Avatars/{contact}.j",
+                    w3css=w3css
                 )
             )
         if current % 10 == 0:
             print(f"Creating HTML...({current}/{total_row_number})", end="\r")
 
     print(f"Creating HTML...({total_row_number}/{total_row_number})", end="\r")
```

### Comparing `whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/extract_iphone.py` & `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,33 +2,17 @@
 
 import sqlite3
 import json
 import jinja2
 import os
 import shutil
 from pathlib import Path
-from bleach import clean as sanitize
-from markupsafe import Markup
 from datetime import datetime
 from mimetypes import MimeTypes
-
-APPLE_TIME = datetime.timestamp(datetime(2001, 1, 1))
-
-
-def sanitize_except(html):
-    return Markup(sanitize(html, tags=["br"]))
-
-
-def determine_day(last, current):
-    last = datetime.fromtimestamp(last).date()
-    current = datetime.fromtimestamp(current).date()
-    if last == current:
-        return None
-    else:
-        return current
+from Whatsapp_Chat_Exporter.utility import sanitize_except, determine_day, APPLE_TIME
 
 
 def messages(db, data):
     c = db.cursor()
     # Get contacts
     c.execute("""SELECT count() FROM ZWACHATSESSION""")
     total_row_number = c.fetchone()[0]
@@ -224,15 +208,15 @@
             f"however it should be located at {file_path}"
         data[row[2]]["messages"][row[1]]["mime"] = "text/x-vcard"
         data[row[2]]["messages"][row[1]]["media"] = True
         data[row[2]]["messages"][row[1]]["meta"] = True
         print(f"Gathering vCards...({index + 1}/{total_row_number})", end="\r")
 
 
-def create_html(data, output_folder, template=None, embedded=False):
+def create_html(data, output_folder, template=None, embedded=False, offline_static=False):
     if template is None:
         template_dir = os.path.dirname(__file__)
         template_file = "whatsapp.html"
     else:
         template_dir = os.path.dirname(template)
         template_file = os.path.basename(template)
     templateLoader = jinja2.FileSystemLoader(searchpath=template_dir)
@@ -243,14 +227,26 @@
 
     total_row_number = len(data)
     print(f"\nCreating HTML...(0/{total_row_number})", end="\r")
 
     if not os.path.isdir(output_folder):
         os.mkdir(output_folder)
 
+    w3css = "https://www.w3schools.com/w3css/4/w3.css"
+    if offline_static:
+        import urllib.request
+        static_folder = os.path.join(output_folder, offline_static)
+        if not os.path.isdir(static_folder):
+            os.mkdir(static_folder)
+        w3css_path = os.path.join(static_folder, "w3.css")
+        if not os.path.isfile(w3css_path):
+            with urllib.request.urlopen(w3css) as resp:
+                with open(w3css_path, "wb") as f: f.write(resp.read())
+        w3css = os.path.join(offline_static, "w3.css")
+
     for current, contact in enumerate(data):
         if len(data[contact]["messages"]) == 0:
             continue
         phone_number = contact.split('@')[0]
         if "-" in contact:
             file_name = ""
         else:
@@ -268,15 +264,16 @@
         safe_file_name = "".join(x for x in file_name if x.isalnum() or x in "- ")
         with open(f"{output_folder}/{safe_file_name}.html", "w", encoding="utf-8") as f:
             f.write(
                 template.render(
                     name=name,
                     msgs=data[contact]["messages"].values(),
                     my_avatar=None,
-                    their_avatar=f"WhatsApp/Avatars/{contact}.j"
+                    their_avatar=f"WhatsApp/Avatars/{contact}.j",
+                    w3css=w3css
                 )
             )
         if current % 10 == 0:
             print(f"Creating HTML...({current}/{total_row_number})", end="\r")
 
     print(f"Creating HTML...({total_row_number}/{total_row_number})", end="\r")
```

### Comparing `whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/extract_iphone_media.py` & `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone_media.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.8.5/Whatsapp_Chat_Exporter/whatsapp.html` & `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/whatsapp.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 <!DOCTYPE html>
 <html>
 	<head>
 		<title>Whatsapp - {{ name }}</title> 
-		<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css"> 
+		<meta charset="UTF-8">
+		<link rel="stylesheet" href="{{w3css}}"> 
 		<style>
-		@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+HK:wght@300;400&display=swap');
-		html {
-			font-family: 'Noto Sans HK', sans-serif;
+		html, body {
 			font-size: 12px;
 			scroll-behavior: smooth;
 		}
 		header {
 			position: fixed;
 			z-index: 20;
 			border-bottom: 2px solid #e3e6e7;
@@ -135,19 +134,19 @@
 							{% else %}
 								{% if msg.media == false %}
 								{{ msg.data | sanitize_except() }}
 								{% else %}
 									{% if "image/" in msg.mime %}
 									<a href="{{ msg.data }}"><img src="{{ msg.data }}" /></a>
 									{% elif "audio/" in msg.mime %}
-									<audio controls="controls" autobuffer="autobuffer">
+									<audio controls preload="auto">
 										<source src="{{ msg.data }}" />
 									</audio>
 									{% elif "video/" in msg.mime %}
-									<video controls="controls" autobuffer="autobuffer">
+									<video controls preload="auto">
 										<source src="{{ msg.data }}" />
 									</video>
 									{% elif "/" in msg.mime %}
 										<div style="text-align: center;" class="w3-panel w3-border-blue w3-pale-blue w3-rightbar w3-leftbar">
 											<p>The file cannot be displayed here, however it should be located at <a href="./{{ msg.data }}">here</a></p>
 										</div>
 									{% else %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+
 Chat history with {{ name }}
 {% set last = {'last': 946688461.001} %} {% for msg in msgs -%}
  {% if determine_day(last.last, msg.timestamp) is not none %}
 {{ determine_day(last.last, msg.timestamp) }}
 {% if last.update({'last': msg.timestamp}) %}{% endif %} {% endif %} {% if
 msg.from_me == true %}
 {{ msg.time }}
```

### Comparing `whatsapp-chat-exporter-0.8.5/setup.py` & `whatsapp-chat-exporter-0.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,29 +7,38 @@
 with open("Whatsapp_Chat_Exporter/__init__.py", encoding="utf8") as f:
     version = search(r'__version__ = "(.*?)"', f.read()).group(1)
 
 setuptools.setup(
     name="whatsapp-chat-exporter",
     version=version,
     author="KnugiHK",
-    author_email="info@knugi.com",
+    author_email="hello@knugi.com",
     description="A Whatsapp database parser that will give you the "
                 "history of your Whatsapp conversations in HTML and JSON.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    license="MIT",
+    keywords=[
+        "android", "ios", "parsing", "history","iphone", "whatsapp", "message"
+        "customizable", "android-backup", "crypt12", "whatsapp-chat-exporter",
+        "whatsapp-export", "whatsapp-database", "whatsapp-database-parser",
+        "whatsapp-conversations", "iphone-backup", "crypt14", "crypt15", "messages"
+    ],
+    platforms=["any"],
     url="https://github.com/KnugiHK/Whatsapp-Chat-Exporter",
     packages=setuptools.find_packages(),
     package_data={
         '': ['whatsapp.html']
     },
     classifiers=[
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: End Users/Desktop",
         "Topic :: Communications :: Chat",
         "Topic :: Utilities",
```

### Comparing `whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/PKG-INFO` & `whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-exporter
-Version: 0.8.5
+Version: 0.9.0
 Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
 Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
 Author: KnugiHK
-Author-email: info@knugi.com
+Author-email: hello@knugi.com
+License: MIT
+Keywords: android,ios,parsing,history,iphone,whatsapp,messagecustomizable,android-backup,crypt12,whatsapp-chat-exporter,whatsapp-export,whatsapp-database,whatsapp-database-parser,whatsapp-conversations,iphone-backup,crypt14,crypt15,messages
+Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Utilities
@@ -26,26 +30,26 @@
 License-File: LICENSE
 
 # Whatsapp-Chat-Exporter
 [![Latest in Pypi](https://img.shields.io/pypi/v/whatsapp-chat-exporter?label=Latest%20in%20Pypi)](https://pypi.org/project/whatsapp-chat-exporter/)
 ![License MIT](https://img.shields.io/pypi/l/whatsapp-chat-exporter)
 [![Python](https://img.shields.io/pypi/pyversions/Whatsapp-Chat-Exporter)](https://pypi.org/project/Whatsapp-Chat-Exporter/)
 
-A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.  
+A customizable Android and iPhone Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON. Inspired by [Telegram Chat Export Tool](https://telegram.org/blog/export-and-more).  
 **If you plan to uninstall WhatsApp or delete your WhatsApp account, please make a backup of your WhatsApp database. You may want to use this exporter again on the same database in the future as the exporter develops**
 
 # Usage
 **Usage in README may be removed in the future. Check the usage in [Wiki](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/wiki)**.
 
 **If you want to use the old release (< 0.5) of the exporter, please follow the [old usage guide](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/wiki/Old-Usage#usage)**.
 
 First, install the exporter by:
 ```shell
 pip install whatsapp-chat-exporter
-pip install whatsapp-chat-exporter[android_backup]  & :: Optional, if you want it to support decrypting Android WhatsApp backup.
+pip install whatsapp-chat-exporter[android_backup]  :; # Optional, if you want it to support decrypting Android WhatsApp backup.
 ```
 Then, create a working directory in somewhere you want
 ```shell
 mkdir working_wts
 cd working_wts
 ```
 ## Working with Android
@@ -65,14 +69,15 @@
 
 ### Encrypted Android WhatsApp Backup
 In order to support the decryption, install pycryptodome if it is not installed
 ```sh
 pip install pycryptodome # Or 
 pip install whatsapp-chat-exporter["android_backup"] # install along with this software
 ```
+### Crypt15 is now the easiest way to decrypt a backup. If you have the 32 bytes hex key generated when you enable End-to-End encrypted backup, you can use it to decrypt the backup. If you do not have the 32 bytes hex key, you can still use the key file extracted just like extacting key file for Crypt12 and Crypt14 to decrypt the backup.
 #### Crypt12 or Crypt14
 Place the decryption key file (key) and the encrypted WhatsApp Backup (msgstore.db.crypt14) in the working directory. If you also want the name of your contacts, get the contact database, which is called wa.db. And copy the WhatsApp (Media) directory from your phone directly.
 
 And now, you should have something like this in the working directory.
 
 ![Android folder structure with WhatsApp Backup](imgs/android_structure_backup.png)
 #### Extracting
@@ -126,34 +131,41 @@
 #### Group Message
 ![Group Message](imgs/group.png)
 
 ## More options
 Invoke the wtsexporter with --help option will show you all options available.
 ```sh
 > wtsexporter --help
-Usage: wtsexporter [options]
+usage: wtsexporter [options]
 
-Options:
-  --version             show program's version number and exit
+options:
   -h, --help            show this help message and exit
   -a, --android         Define the target as Android
-  -i, --iphone          Define the target as iPhone
-  -w WA, --wa=WA        Path to contact database
-  -m MEDIA, --media=MEDIA
-                        Path to WhatsApp media folder
-  -b BACKUP, --backup=BACKUP
-                        Path to Android (must be used together with -k)/iPhone
-                        WhatsApp backup
-  -o OUTPUT, --output=OUTPUT
-                        Output to specific directory
-  -j, --json            Save the result to a single JSON file
-  -d DB, --db=DB        Path to database file
-  -k KEY, --key=KEY     Path to key file
-  -t TEMPLATE, --template=TEMPLATE
+  -i, --iphone, --ios   Define the target as iPhone
+  -w WA, --wa WA        Path to contact database (default: wa.db/ContactsV2.sqlite)
+  -m MEDIA, --media MEDIA
+                        Path to WhatsApp media folder (default: WhatsApp)
+  -b BACKUP, --backup BACKUP
+                        Path to Android (must be used together with -k)/iPhone WhatsApp backup
+  -o OUTPUT, --output OUTPUT
+                        Output to specific directory (default: result)
+  -j [JSON], --json [JSON]
+                        Save the result to a single JSON file (default if present: result.json)
+  -d DB, --db DB        Path to database file (default: msgstore.db/7c7fba66680ef796b916b067077cc246adacf01d)
+  -k KEY, --key KEY     Path to key file
+  -t TEMPLATE, --template TEMPLATE
                         Path to custom HTML template
+  -e, --embedded        Embed media into HTML file (not yet implemented)
+  -s, --showkey         Show the HEX key used to decrypt the database
+  -c, --move-media      Move the media directory to output directory if the flag is set, otherwise copy it
+  --offline OFFLINE     Relative path to offline static files
+  --size SIZE, --output-size SIZE
+                        Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
+  --no-html             Do not output html files
+  --check-update        Check for updates
 ```
 
 # To do
 1. Reply in iPhone
 
 # Copyright
 This is a MIT licensed project.
```

### Comparing `whatsapp-chat-exporter-0.8.5/whatsapp_chat_exporter.egg-info/SOURCES.txt` & `whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 README.md
 setup.py
 Whatsapp_Chat_Exporter/__init__.py
 Whatsapp_Chat_Exporter/__main__.py
+Whatsapp_Chat_Exporter/data_model.py
 Whatsapp_Chat_Exporter/extract.py
 Whatsapp_Chat_Exporter/extract_iphone.py
 Whatsapp_Chat_Exporter/extract_iphone_media.py
+Whatsapp_Chat_Exporter/extract_new.py
+Whatsapp_Chat_Exporter/utility.py
 Whatsapp_Chat_Exporter/whatsapp.html
 whatsapp_chat_exporter.egg-info/PKG-INFO
 whatsapp_chat_exporter.egg-info/SOURCES.txt
 whatsapp_chat_exporter.egg-info/dependency_links.txt
 whatsapp_chat_exporter.egg-info/entry_points.txt
 whatsapp_chat_exporter.egg-info/requires.txt
 whatsapp_chat_exporter.egg-info/top_level.txt
```

