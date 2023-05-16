# Comparing `tmp/t4flib-0.1.8-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8039 bytes, number of entries: 10
+Zip file size: 7974 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      892 b- defN 23-May-11 18:20 t4flib/config.py
--rw-rw-r--  2.0 unx     6286 b- defN 23-May-16 09:35 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     6145 b- defN 23-May-16 10:28 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     4508 b- defN 23-May-11 18:20 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     3259 b- defN 23-May-11 18:20 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      753 b- defN 23-May-11 18:20 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-May-16 09:44 t4flib-0.1.8.dist-info/RECORD
-10 files, 18320 bytes uncompressed, 6755 bytes compressed:  63.1%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      758 b- defN 23-May-16 10:36 t4flib-0.1.9.dist-info/RECORD
+10 files, 18179 bytes uncompressed, 6690 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.1.8.dist-info/METADATA
+Filename: t4flib-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.1.8.dist-info/WHEEL
+Filename: t4flib-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.1.8.dist-info/top_level.txt
+Filename: t4flib-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.1.8.dist-info/RECORD
+Filename: t4flib-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/file_helper.py

```diff
@@ -1,17 +1,18 @@
 import os
-from log_helper import logger
+from .log_helper import logger
 import shutil
 import fnmatch
 import datetime
 import pathlib
 import json
 import zipfile
 import glob
 import pandas as pd
+import csv
 
 
 def __validate_filemask__(filename, filemask):
     return fnmatch.fnmatch(filename, filemask)
 
 
 def zip_folder(source_dir, dest_dir, output_filename):
@@ -69,45 +70,40 @@
     except Exception as e:
         logger('ERROR', f'{str(e)}')
         raise
 
     logger('INFO', f'Fin du déplacement des fichiers commencant par {filemask} du dossier {source_dir} vers {dest_dir}')
 
 
-def concatenate_csv_files(source_dir, dest_dir, dest_file_path):
-    logger('INFO', 'Début de la concaténation des fichiers CSV')
-
+def read_and_concatenate_csv_files(source_dir, dest_dir, output_filename ,delimiter=';', isNeedSkipHeader=False):
+    
+    logger('INFO', f'Démarrage de la concaténation des CSV du dossier {source_dir}')
+    
     try:
-
-        # obtenir la liste de tous les fichiers .csv dans le dossier source
-        file_list = get_all_file_by_filemask(source_dir, '*.csv')
-
-        if len(file_list) == 0:
-            logger('WARNING', 'Pas de données CSV à concaténer')
-            return
-
-        liste_data = []
-
-        # Parcourez la liste des fichiers et lisez chaque fichier CSV
-        for fichier in file_list:
-            # Lisez le fichier CSV dans un DataFrame
-            donnees = pd.read_csv(str(fichier.absolute()), delimiter=';')
-
-            # Ajoutez les données du fichier actuel au DataFrame global
-            liste_data.append(donnees)
-
-        donnees_concatenees = pd.concat(liste_data, ignore_index=True)
-        # Écrivez le DataFrame global dans un fichier CSV
-        donnees_concatenees.to_csv(os.path.join(dest_dir, dest_file_path), index=False, sep=';')
-
+    
+        filenames=get_all_file_by_filemask(source_dir, '*.csv')
+        
+        if len(filenames) == 0:
+            logger('WARNING', 'Aucun fichier n\'a été detecté')
+            return None
+        
+        with open(os.path.join(dest_dir, output_filename), 'w', newline='') as output_file:
+            writer = csv.writer(output_file, delimiter=delimiter)
+            
+            for file in filenames:
+                with open(file, 'r') as input_file:
+                        reader = csv.reader(input_file, delimiter=delimiter)
+                        if isNeedSkipHeader:
+                            next(reader)
+                        writer.writerows(reader)
+   
     except Exception as e:
-        logger('ERROR', str(e))
-        raise
-    logger('INFO',
-           f'Le fichier {os.path.join(dest_dir, dest_file_path)} a bien été créé à partir de {len(file_list)} fichiers')
+        logger('ERROR', str(e))     
+    finally:    
+        logger('INFO', f'Fin de la concaténation des CSV du dossier {source_dir}')
 
 
 def is_file_older_than_nb_day(filepath, datetime_to_inspect):
     logger('INFO', f'Vérification que le fichier {filepath} soit plus ancien que {datetime_to_inspect} jour')
     try:
         if os.path.exists(filepath):
             modification_datetime = datetime.datetime.fromtimestamp(os.path.getmtime(filepath))
```

## Comparing `t4flib-0.1.8.dist-info/METADATA` & `t4flib-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.1.8.dist-info/RECORD` & `t4flib-0.1.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
-t4flib/file_helper.py,sha256=-n6JLN1NGBM3xbd27AkDLI6CHgW6FO-EW5ZqK56aRbU,6286
+t4flib/file_helper.py,sha256=NYIgOrA1iJBUcodtaRlDIsIHoivonLme4PmFZB1nQLw,6145
 t4flib/filetransfer_helper.py,sha256=mbi_R4cahDFTnPGO4zD_7txD8t1_SQrxPIIRSJvxCdg,4508
 t4flib/gcloud_helper.py,sha256=Y4u_y4fy4zDjXKEmwBV91Yl4x9FNJsSmDLEKLwzDqJ0,3259
 t4flib/log_helper.py,sha256=uRHKVgfhq6V4PY64lrRnrjzoA99OcyKI-bcr0vUnv_I,753
-t4flib-0.1.8.dist-info/METADATA,sha256=Oc57YOrPhHipD8shNqZuNnUjP15GggDDyNUnc7yzoSQ,1747
-t4flib-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.1.8.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.1.8.dist-info/RECORD,,
+t4flib-0.1.9.dist-info/METADATA,sha256=nii2sdyI7k5BI6XyM8DVYZYHIvQ5DvDHQ8yzkxekS08,1747
+t4flib-0.1.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.1.9.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.1.9.dist-info/RECORD,,
```

