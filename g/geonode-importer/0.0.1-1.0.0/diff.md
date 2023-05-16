# Comparing `tmp/geonode_importer-0.0.1-py3-none-any.whl.zip` & `tmp/geonode_importer-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 89159 bytes, number of entries: 77
--rw-r--r--  2.0 unx     1132 b- defN 23-May-16 14:04 importer/__init__.py
+Zip file size: 89160 bytes, number of entries: 77
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-16 15:09 importer/__init__.py
 -rw-r--r--  2.0 unx      891 b- defN 23-May-16 14:04 importer/apps.py
 -rw-r--r--  2.0 unx      301 b- defN 23-May-16 14:04 importer/celery_app.py
 -rw-r--r--  2.0 unx    25673 b- defN 23-May-16 14:04 importer/celery_tasks.py
 -rw-r--r--  2.0 unx     1142 b- defN 23-May-16 14:04 importer/datastore.py
 -rw-r--r--  2.0 unx     2137 b- defN 23-May-16 14:04 importer/db_router.py
 -rw-r--r--  2.0 unx     1533 b- defN 23-May-16 14:04 importer/models.py
 -rw-r--r--  2.0 unx    13953 b- defN 23-May-16 14:04 importer/orchestrator.py
@@ -67,13 +67,13 @@
 -rw-r--r--  2.0 unx     6095 b- defN 23-May-16 14:04 importer/tests/end2end/test_end2end.py
 -rw-r--r--  2.0 unx     7707 b- defN 23-May-16 14:04 importer/tests/end2end/test_end2end_copy.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/tests/unit/__init__.py
 -rw-r--r--  2.0 unx     1234 b- defN 23-May-16 14:04 importer/tests/unit/test_models.py
 -rw-r--r--  2.0 unx    13739 b- defN 23-May-16 14:04 importer/tests/unit/test_orchestrator.py
 -rw-r--r--  2.0 unx     3606 b- defN 23-May-16 14:04 importer/tests/unit/test_publisher.py
 -rw-r--r--  2.0 unx    23904 b- defN 23-May-16 14:04 importer/tests/unit/test_task.py
--rw-r--r--  2.0 unx     1069 b- defN 23-May-16 15:08 geonode_importer-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      712 b- defN 23-May-16 15:08 geonode_importer-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-16 15:08 geonode_importer-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-16 15:08 geonode_importer-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6809 b- defN 23-May-16 15:08 geonode_importer-0.0.1.dist-info/RECORD
-77 files, 293179 bytes uncompressed, 78221 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx     1069 b- defN 23-May-16 15:09 geonode_importer-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      712 b- defN 23-May-16 15:09 geonode_importer-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 15:09 geonode_importer-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-16 15:09 geonode_importer-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6809 b- defN 23-May-16 15:09 geonode_importer-1.0.0.dist-info/RECORD
+77 files, 293179 bytes uncompressed, 78222 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -210,23 +210,23 @@
 
 Filename: importer/tests/unit/test_publisher.py
 Comment: 
 
 Filename: importer/tests/unit/test_task.py
 Comment: 
 
-Filename: geonode_importer-0.0.1.dist-info/LICENSE
+Filename: geonode_importer-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: geonode_importer-0.0.1.dist-info/METADATA
+Filename: geonode_importer-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: geonode_importer-0.0.1.dist-info/WHEEL
+Filename: geonode_importer-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: geonode_importer-0.0.1.dist-info/top_level.txt
+Filename: geonode_importer-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: geonode_importer-0.0.1.dist-info/RECORD
+Filename: geonode_importer-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## importer/__init__.py

```diff
@@ -16,13 +16,13 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 #########################################################################
 import os
 
 project_dir = os.path.dirname(os.path.abspath(__file__))
 
-VERSION = (0, 0, 1)
+VERSION = (1, 0, 0)
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "geosolutions-it"
 __email__ = "info@geosolutionsgroup.com"
 __url__ = "https://github.com/GeoNode/geonode-importer"
 default_app_config = "importer.apps.ImporterConfig"
```

## Comparing `geonode_importer-0.0.1.dist-info/LICENSE` & `geonode_importer-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `geonode_importer-0.0.1.dist-info/METADATA` & `geonode_importer-1.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geonode-importer
-Version: 0.0.1
+Version: 1.0.0
 Home-page: https://github.com/GeoNode/geonode-importer
 Author: geosolutions-it
 Author-email: info@geosolutionsgroup.com
 Project-URL: Bug Tracker, https://github.com/geosolutions-it/geonode-importer/issues
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.0
```

## Comparing `geonode_importer-0.0.1.dist-info/RECORD` & `geonode_importer-1.0.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-importer/__init__.py,sha256=Mo-gfCGULxYMIbDFfBob8DoCS3y2Rfyxk--mRR1aIMM,1132
+importer/__init__.py,sha256=rh0F8FKX9TX5LTjIUEppJ1mol2ZjM5k699NcuaFGpP0,1132
 importer/apps.py,sha256=nym_44W069KBuqrWbDw64y7CetrA8xFPVgEBcP7F1_A,891
 importer/celery_app.py,sha256=vXVNHq_WntdNstgbKbVVJsOhTllf__ZWr-skmDohJvE,301
 importer/celery_tasks.py,sha256=rbx_r7w9K5MPJh_gIkdLF4lgDMgAh_D9Vcv7_0LoG_A,25673
 importer/datastore.py,sha256=OejV7R8G5fmvSGW3fJPGoE5DE3C_GZylYUIYOz2kbFg,1142
 importer/db_router.py,sha256=zY65wik8Z6ptJ3MggYxp4isFt11ohmk_5t2pIS9MBeA,2137
 importer/models.py,sha256=MuLxhMp8MnFT3J00dPX1gigk1K-ol6fmcpIJ1D6QvMg,1533
 importer/orchestrator.py,sha256=Lsljy5kA0VTeg1oS-0ok55CtFUNUt_L8hOLWxtvam00,13953
@@ -66,12 +66,12 @@
 importer/tests/end2end/test_end2end.py,sha256=Qh4P3o9LChneY-pKdpP459EzmBv1XwGwYfiWWXT1-_s,6095
 importer/tests/end2end/test_end2end_copy.py,sha256=QDmUCZOuhYcB8ie_NDWAw2NIJhcAenlnWimpWzzrIA8,7707
 importer/tests/unit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/tests/unit/test_models.py,sha256=cykml2VUVbiCmdeTTG7pqKAdZiCu0kAALxH7AVSWrC0,1234
 importer/tests/unit/test_orchestrator.py,sha256=M5KueNjjCC3hPfQRepZZD7oo58tDbM7sakmYx-ffUo8,13739
 importer/tests/unit/test_publisher.py,sha256=u6juJPEWoQoKGhfjt6h4D160PDkF8dKuZiiPwwN3XZU,3606
 importer/tests/unit/test_task.py,sha256=AYl0z7IvUMfHKt_bmIdsCaLL0Rn6M6pXHF4zxD8MdsI,23904
-geonode_importer-0.0.1.dist-info/LICENSE,sha256=gMS2YAekulHmzbeQAk-e6U1_unOcCszd6aKY5bQJXO0,1069
-geonode_importer-0.0.1.dist-info/METADATA,sha256=6XaARs0y6WGztPemZxECtklYh3WxQivd10TLSsFG6AU,712
-geonode_importer-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-geonode_importer-0.0.1.dist-info/top_level.txt,sha256=MRQ0MhtKdXF90IDYri2Z5uPJ8A9O0ITe5bEXA2ZLjM4,9
-geonode_importer-0.0.1.dist-info/RECORD,,
+geonode_importer-1.0.0.dist-info/LICENSE,sha256=gMS2YAekulHmzbeQAk-e6U1_unOcCszd6aKY5bQJXO0,1069
+geonode_importer-1.0.0.dist-info/METADATA,sha256=HFtnYav7OOCAF2rv5GXIYdBVzrmQ1Zv8UM_Aoj9Q_XU,712
+geonode_importer-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+geonode_importer-1.0.0.dist-info/top_level.txt,sha256=MRQ0MhtKdXF90IDYri2Z5uPJ8A9O0ITe5bEXA2ZLjM4,9
+geonode_importer-1.0.0.dist-info/RECORD,,
```

