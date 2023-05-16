# Comparing `tmp/t4flib-0.1.7-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8011 bytes, number of entries: 10
+Zip file size: 8039 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      892 b- defN 23-May-11 18:20 t4flib/config.py
--rw-rw-r--  2.0 unx     6122 b- defN 23-May-15 15:30 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     6286 b- defN 23-May-16 09:35 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     4508 b- defN 23-May-11 18:20 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     3259 b- defN 23-May-11 18:20 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      753 b- defN 23-May-11 18:20 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-15 15:37 t4flib-0.1.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-15 15:37 t4flib-0.1.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-15 15:37 t4flib-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-May-15 15:37 t4flib-0.1.7.dist-info/RECORD
-10 files, 18156 bytes uncompressed, 6727 bytes compressed:  62.9%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      758 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/RECORD
+10 files, 18320 bytes uncompressed, 6755 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.1.7.dist-info/METADATA
+Filename: t4flib-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.1.7.dist-info/WHEEL
+Filename: t4flib-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.1.7.dist-info/top_level.txt
+Filename: t4flib-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.1.7.dist-info/RECORD
+Filename: t4flib-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/file_helper.py

```diff
@@ -1,9 +1,9 @@
 import os
-from .log_helper import logger
+from log_helper import logger
 import shutil
 import fnmatch
 import datetime
 import pathlib
 import json
 import zipfile
 import glob
@@ -11,20 +11,26 @@
 
 
 def __validate_filemask__(filename, filemask):
     return fnmatch.fnmatch(filename, filemask)
 
 
 def zip_folder(source_dir, dest_dir, output_filename):
-    logger('INFO', f'Zippage du dossier {source_dir}')
+    logger('INFO', f'Zippage du dossier de ouf {source_dir}')
     try:
         with zipfile.ZipFile(os.path.join(dest_dir, output_filename), 'w', zipfile.ZIP_DEFLATED) as zipf:
-            for root, dirs, files in os.walk(source_dir):
-                for file in files:
-                    zipf.write(os.path.join(root, file), os.path.relpath(os.path.join(root, file), source_dir))
+            files=get_all_file_by_filemask(source_dir, '*')
+            if len(files) == 0:
+                logger('WARNING', 'Pas de fichier à zipper')
+                return
+            
+            for file in files:
+                file_path=str(file.absolute())
+            
+                zipf.write(file_path, os.path.relpath(file_path, source_dir))
 
         logger('INFO', f'Le dossier {source_dir} a été zippé avec succès dans {output_filename}')
     except Exception as e:
         logger('ERROR', f'{str(e)}')
         raise
 
 
@@ -173,7 +179,11 @@
 
         for file in files:
             shutil.copyfile(str(file.absolute()), os.path.join(dest_dir, file.name))
     except Exception as e:
         logger('ERROR', str(e))
         raise
     logger('INFO', 'L\'ensemble des fichiers ont été copiés')
+
+
+
+
```

## Comparing `t4flib-0.1.7.dist-info/METADATA` & `t4flib-0.1.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.1.7.dist-info/RECORD` & `t4flib-0.1.8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
-t4flib/file_helper.py,sha256=ISSI07izV5tgo-HR2bG63Vs14AEorVdGNkIoaua-FKg,6122
+t4flib/file_helper.py,sha256=-n6JLN1NGBM3xbd27AkDLI6CHgW6FO-EW5ZqK56aRbU,6286
 t4flib/filetransfer_helper.py,sha256=mbi_R4cahDFTnPGO4zD_7txD8t1_SQrxPIIRSJvxCdg,4508
 t4flib/gcloud_helper.py,sha256=Y4u_y4fy4zDjXKEmwBV91Yl4x9FNJsSmDLEKLwzDqJ0,3259
 t4flib/log_helper.py,sha256=uRHKVgfhq6V4PY64lrRnrjzoA99OcyKI-bcr0vUnv_I,753
-t4flib-0.1.7.dist-info/METADATA,sha256=t6CyJGVFi95iJ3I2qGl93m9qXZKcHQtPZ6d7kQ4h5S8,1747
-t4flib-0.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.1.7.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.1.7.dist-info/RECORD,,
+t4flib-0.1.8.dist-info/METADATA,sha256=Oc57YOrPhHipD8shNqZuNnUjP15GggDDyNUnc7yzoSQ,1747
+t4flib-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.1.8.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.1.8.dist-info/RECORD,,
```

