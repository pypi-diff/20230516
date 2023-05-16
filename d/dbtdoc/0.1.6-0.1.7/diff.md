# Comparing `tmp/dbtdoc-0.1.6-py3-none-any.whl.zip` & `tmp/dbtdoc-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11450 bytes, number of entries: 9
+Zip file size: 11407 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-04 16:02 dbtdoc/__init__.py
--rw-r--r--  2.0 unx       20 b- defN 23-Mar-25 12:18 dbtdoc/_version.py
--rw-r--r--  2.0 unx    16898 b- defN 23-Mar-25 12:42 dbtdoc/dbtdoc.py
--rw-r--r--  2.0 unx    11346 b- defN 23-Mar-25 12:45 dbtdoc-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2452 b- defN 23-Mar-25 12:45 dbtdoc-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-25 12:45 dbtdoc-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-25 12:45 dbtdoc-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-25 12:45 dbtdoc-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      694 b- defN 23-Mar-25 12:45 dbtdoc-0.1.6.dist-info/RECORD
-9 files, 31556 bytes uncompressed, 10254 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx       20 b- defN 23-May-16 14:42 dbtdoc/_version.py
+-rw-r--r--  2.0 unx    16369 b- defN 23-May-16 14:34 dbtdoc/dbtdoc.py
+-rw-r--r--  2.0 unx    11346 b- defN 23-May-16 14:44 dbtdoc-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2506 b- defN 23-May-16 14:44 dbtdoc-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 14:44 dbtdoc-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-May-16 14:44 dbtdoc-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-16 14:44 dbtdoc-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      694 b- defN 23-May-16 14:44 dbtdoc-0.1.7.dist-info/RECORD
+9 files, 31081 bytes uncompressed, 10211 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: dbtdoc/_version.py
 Comment: 
 
 Filename: dbtdoc/dbtdoc.py
 Comment: 
 
-Filename: dbtdoc-0.1.6.dist-info/LICENSE
+Filename: dbtdoc-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: dbtdoc-0.1.6.dist-info/METADATA
+Filename: dbtdoc-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: dbtdoc-0.1.6.dist-info/WHEEL
+Filename: dbtdoc-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: dbtdoc-0.1.6.dist-info/entry_points.txt
+Filename: dbtdoc-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: dbtdoc-0.1.6.dist-info/top_level.txt
+Filename: dbtdoc-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: dbtdoc-0.1.6.dist-info/RECORD
+Filename: dbtdoc-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbtdoc/_version.py

```diff
@@ -1 +1 @@
-__version__='0.1.6'
+__version__='0.1.7'
```

## dbtdoc/dbtdoc.py

```diff
@@ -32,14 +32,15 @@
 LOGGER.setLevel(logging.ERROR) # only display errors
 stream_handler = StreamHandler()
 stream_handler.setLevel(logging.DEBUG)
 handler_format = Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 stream_handler.setFormatter(handler_format)
 LOGGER.addHandler(stream_handler)
 
+SINGLE_FILE=''
 
 class Dumper(yaml.Dumper):
     """ A workaround to indent list more friendly
         See https://github.com/yaml/pyyaml/issues/234 for details
     """
     def increase_indent(self, flow=False, *ARGS, **kwARGS):
         return super().increase_indent(flow=flow, indentless=False)
@@ -64,14 +65,22 @@
         return dumper.represent_scalar("tag:yaml.org,2002:str", instance)
 yaml.add_representer(str, _represent_str)
 
 
 def _get_dirs(dbt_dir):
     """ Return the value of `model-paths` and `macro-path`from dbt_project.yml
     """
+    global SINGLE_FILE
+
+    if os.path.isfile(dbt_dir):
+        LOGGER.warning(f"{dbt_dir} is a file")
+        SINGLE_FILE = os.path.normpath(dbt_dir)
+        dirname, _ = os.path.split(dbt_dir)
+        return [dirname]
+
     dbt_project_file = os.path.join(dbt_dir, "dbt_project.yml")
     if not os.path.isfile(dbt_project_file):
         LOGGER.warning(f"dbt_project.yml not found in {dbt_dir}")
         return [dbt_dir]
 
     try:
         with open(dbt_project_file, "r") as f:
@@ -91,45 +100,14 @@
     except Exception as e:
         LOGGER.error(f"invalid project file in {dbt_dir}")
         exit(1)
 
     return result
 
 
-def _read_blocks(sql_file):
-    """ Extract doc, dbt block from comments
-        doc block: everything from the beginning to dbt block
-        dbt block: evertyhing inside ```dbt block
-        everything after the dbt block is ignored by dbtdocstr
-    """
-    with open(sql_file, "r") as f:
-        sql = f.read()
-    doc_start = sql.find("/*")
-    doc_end = sql.find("*/")
-    doc = sql[doc_start + 2:doc_end] if doc_start > -1 else ""
-
-    dbt = {}
-    if doc:
-        dbt_start = doc.find(DBT_BLOCK_START_KEY)
-        dbt_end = doc.find("```", dbt_start + len(DBT_BLOCK_START_KEY))
-
-        if dbt_start > -1:
-            dbt_block = doc[dbt_start + len(DBT_BLOCK_START_KEY):dbt_end]
-            try:
-                dbt = yaml.load(dbt_block, Loader=yaml.FullLoader)
-                dbt = yaml.safe_load(dbt_block)
-            except Exception as e:
-                LOGGER.error(f"invalid dbt block in {sql_file}")
-                LOGGER.debug(dbt_block)
-
-        doc = doc[0:dbt_start].strip()
-
-    return doc, dbt
-
-
 def _quote_item(d):
     """ Scan an item and quote string if it is necessary
     """
     if d is None:
         return None
 
     if isinstance(d, str):
@@ -166,14 +144,21 @@
         for fname in files:
             # Parse the table name from the SQL file name
             if fname[-3:] != "sql":
                 LOGGER.info("Skipping non-sql file: " + fname)
                 continue
 
             sql_file = os.path.join(cdir, fname)
+
+            # ignore if SINGLE_FILE is a valid path and not equal to sql_file
+            if SINGLE_FILE != '' and SINGLE_FILE != sql_file:
+                LOGGER.info(f"Skipping file {sql_file} because it is not {SINGLE_FILE}")
+                continue
+
+
             with open(sql_file, 'r') as f:
                 sql = f.read()
 
             # split into macro/test blocks
             # using a simple rule, need to be enhanced
             r = re.findall('((?:/\*.*?\*/)*.+?(?:macro|test|materialization) .*?end(?:macro|test|materialization))', sql, re.DOTALL)
             if len(r) == 0:
```

## Comparing `dbtdoc-0.1.6.dist-info/LICENSE` & `dbtdoc-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dbtdoc-0.1.6.dist-info/METADATA` & `dbtdoc-0.1.7.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: dbtdoc
-Version: 0.1.6
+Version: 0.1.7
 Summary: Document tool for dbt
 Home-page: https://github.com/bachng2017/dbtdoc
 Author: bachng
 Author-email: bachng@gmail.com
 License: Apache
 Keywords: dbt doc sql
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools (>=40.3.0)
 
+![Downloads](https://static.pepy.tech/badge/dbtdoc)
+
+
 # dbtdoc
 Create dbt document from SQL files
 
 ## Install
 ```
 pip install dbtdoc
 ```
```

## Comparing `dbtdoc-0.1.6.dist-info/RECORD` & `dbtdoc-0.1.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 dbtdoc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dbtdoc/_version.py,sha256=Yr-urKBBkTSlDbB9sQHA80VCYo7fQWd8NNEJDukz9Ew,20
-dbtdoc/dbtdoc.py,sha256=ecHgUntBi56XDd7YDfUiDjlpG8mAwQZiVIQA9cnlmCQ,16898
-dbtdoc-0.1.6.dist-info/LICENSE,sha256=bwQF4GDyH6Fbv-3PsoNGZ9v_Hg5YuGzSFLIZqYn7wZo,11346
-dbtdoc-0.1.6.dist-info/METADATA,sha256=06SyTs8LqzgPoIUjax9yKXuwTrLZpoZldEUWur2nLI8,2452
-dbtdoc-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dbtdoc-0.1.6.dist-info/entry_points.txt,sha256=FFtYiRyNfj03_4IV8djschstbsLYN5TLkIOooj8luhY,47
-dbtdoc-0.1.6.dist-info/top_level.txt,sha256=Ryrb84PzaV3b6MpPvPO_EVuHE7-9N_gyD96Ey19hpp4,7
-dbtdoc-0.1.6.dist-info/RECORD,,
+dbtdoc/_version.py,sha256=iAZZvdXy5MtXjWzFJe-oSZfUbo01gSpOwRHNM7Id4F8,20
+dbtdoc/dbtdoc.py,sha256=1k5c3s9VEbNifgoH2Lw7nR6qZ9LuA3CDSIK-Gz3CExQ,16369
+dbtdoc-0.1.7.dist-info/LICENSE,sha256=bwQF4GDyH6Fbv-3PsoNGZ9v_Hg5YuGzSFLIZqYn7wZo,11346
+dbtdoc-0.1.7.dist-info/METADATA,sha256=M1pav0FAFSFfMWfV_YhY5-4BxclYKJAUbW4GOxVNxF0,2506
+dbtdoc-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dbtdoc-0.1.7.dist-info/entry_points.txt,sha256=FFtYiRyNfj03_4IV8djschstbsLYN5TLkIOooj8luhY,47
+dbtdoc-0.1.7.dist-info/top_level.txt,sha256=Ryrb84PzaV3b6MpPvPO_EVuHE7-9N_gyD96Ey19hpp4,7
+dbtdoc-0.1.7.dist-info/RECORD,,
```

