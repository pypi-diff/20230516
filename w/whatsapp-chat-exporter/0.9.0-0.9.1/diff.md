# Comparing `tmp/whatsapp-chat-exporter-0.9.0.tar.gz` & `tmp/whatsapp-chat-exporter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chat-exporter-0.9.0.tar", last modified: Tue May 16 11:47:37 2023, max compression
+gzip compressed data, was "whatsapp-chat-exporter-0.9.1.tar", last modified: Tue May 16 16:15:20 2023, max compression
```

## Comparing `whatsapp-chat-exporter-0.9.0.tar` & `whatsapp-chat-exporter-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/whatsapp.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 11:47:23.000000 whatsapp-chat-exporter-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:47:37.849467 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 11:47:37.000000 whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:15:20.332943 whatsapp-chat-exporter-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-16 16:15:20.332943 whatsapp-chat-exporter-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:15:20.328943 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/whatsapp.html
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:15:20.332943 whatsapp-chat-exporter-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 16:15:07.000000 whatsapp-chat-exporter-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:15:20.328943 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 16:15:20.000000 whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/top_level.txt
```

### Comparing `whatsapp-chat-exporter-0.9.0/LICENSE` & `whatsapp-chat-exporter-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/PKG-INFO` & `whatsapp-chat-exporter-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-exporter
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
 Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
 Author: KnugiHK
 Author-email: hello@knugi.com
 License: MIT
 Keywords: android,ios,parsing,history,iphone,whatsapp,messagecustomizable,android-backup,crypt12,whatsapp-chat-exporter,whatsapp-export,whatsapp-database,whatsapp-database-parser,whatsapp-conversations,iphone-backup,crypt14,crypt15,messages
 Platform: any
@@ -161,13 +161,13 @@
   --size SIZE, --output-size SIZE
                         Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
   --no-html             Do not output html files
   --check-update        Check for updates
 ```
 
 # To do
-1. Reply in iPhone
+See [issues](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues).
 
 # Copyright
 This is a MIT licensed project.
 
 The Telegram Desktop's export is the reference for whatsapp.html in this repo
```

### Comparing `whatsapp-chat-exporter-0.9.0/README.md` & `whatsapp-chat-exporter-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -130,13 +130,13 @@
   --size SIZE, --output-size SIZE
                         Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
   --no-html             Do not output html files
   --check-update        Check for updates
 ```
 
 # To do
-1. Reply in iPhone
+See [issues](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues).
 
 # Copyright
 This is a MIT licensed project.
 
 The Telegram Desktop's export is the reference for whatsapp.html in this repo
```

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/__main__.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     parser.add_argument(
         '-i',
         '--iphone',
         '--ios',
         dest='iphone',
         default=False,
         action='store_true',
-        help="Define the target as iPhone")
+        help="Define the target as iPhone/iPad")
     parser.add_argument(
         "-w",
         "--wa",
         dest="wa",
         default=None,
         help="Path to contact database (default: wa.db/ContactsV2.sqlite)")
     parser.add_argument(
```

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/data_model.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/data_model.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             f"however it should be located at {file_path}"
         data[row[2]]["messages"][row[1]]["mime"] = "text/x-vcard"
         data[row[2]]["messages"][row[1]]["media"] = True
         data[row[2]]["messages"][row[1]]["meta"] = True
         print(f"Gathering vCards...({index + 1}/{total_row_number})", end="\r")
 
 
-def create_html(data, output_folder, template=None, embedded=False, offline_static=False):
+def create_html(data, output_folder, template=None, embedded=False, offline_static=False, maximum_size=None):
     if template is None:
         template_dir = os.path.dirname(__file__)
         template_file = "whatsapp.html"
     else:
         template_dir = os.path.dirname(template)
         template_file = os.path.basename(template)
     templateLoader = jinja2.FileSystemLoader(searchpath=template_dir)
```

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_iphone_media.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_iphone_media.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/extract_new.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/extract_new.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/utility.py` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/utility.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/Whatsapp_Chat_Exporter/whatsapp.html` & `whatsapp-chat-exporter-0.9.1/Whatsapp_Chat_Exporter/whatsapp.html`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/setup.py` & `whatsapp-chat-exporter-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/PKG-INFO` & `whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-exporter
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Whatsapp database parser that will give you the history of your Whatsapp conversations in HTML and JSON.
 Home-page: https://github.com/KnugiHK/Whatsapp-Chat-Exporter
 Author: KnugiHK
 Author-email: hello@knugi.com
 License: MIT
 Keywords: android,ios,parsing,history,iphone,whatsapp,messagecustomizable,android-backup,crypt12,whatsapp-chat-exporter,whatsapp-export,whatsapp-database,whatsapp-database-parser,whatsapp-conversations,iphone-backup,crypt14,crypt15,messages
 Platform: any
@@ -161,13 +161,13 @@
   --size SIZE, --output-size SIZE
                         Maximum size of a single output file in bytes, 0 for auto (not yet implemented)
   --no-html             Do not output html files
   --check-update        Check for updates
 ```
 
 # To do
-1. Reply in iPhone
+See [issues](https://github.com/KnugiHK/Whatsapp-Chat-Exporter/issues).
 
 # Copyright
 This is a MIT licensed project.
 
 The Telegram Desktop's export is the reference for whatsapp.html in this repo
```

### Comparing `whatsapp-chat-exporter-0.9.0/whatsapp_chat_exporter.egg-info/SOURCES.txt` & `whatsapp-chat-exporter-0.9.1/whatsapp_chat_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

