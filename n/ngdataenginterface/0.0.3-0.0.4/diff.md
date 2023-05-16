# Comparing `tmp/ngdataenginterface-0.0.3.tar.gz` & `tmp/ngdataenginterface-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngdataenginterface-0.0.3.tar", max compression
+gzip compressed data, was "ngdataenginterface-0.0.4.tar", max compression
```

## Comparing `ngdataenginterface-0.0.3.tar` & `ngdataenginterface-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/README.md
--rw-r--r--   0        0        0      142 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/__init__.py
--rw-r--r--   0        0        0       81 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/analytical/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/analytical/core.py
--rw-r--r--   0        0        0      320 2023-05-15 15:46:09.063485 ngdataenginterface-0.0.3/ngdataenginterface/core/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/aws_interface.py
--rw-r--r--   0        0        0     1555 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/partition.py
--rw-r--r--   0        0        0     5623 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/read.py
--rw-r--r--   0        0        0     2779 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/schema.py
--rw-r--r--   0        0        0     2187 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/utils_emr.py
--rw-r--r--   0        0        0     1424 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/validations.py
--rw-r--r--   0        0        0     4362 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/core/write.py
--rw-r--r--   0        0        0      174 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/__init__.py
--rw-r--r--   0        0        0     4027 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/cleansing.py
--rw-r--r--   0        0        0      408 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/export_redshift.py
--rw-r--r--   0        0        0     6859 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/ngdataenginterface/process/pismo.py
--rw-r--r--   0        0        0      422 2023-05-15 15:46:09.064485 ngdataenginterface-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/README.md
+-rw-r--r--   0        0        0      142 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/analytical/__init__.py
+-rw-r--r--   0        0        0     2429 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/analytical/core.py
+-rw-r--r--   0        0        0      320 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/aws_interface.py
+-rw-r--r--   0        0        0     1558 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/partition.py
+-rw-r--r--   0        0        0     5627 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/read.py
+-rw-r--r--   0        0        0     2787 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/schema.py
+-rw-r--r--   0        0        0     6726 2023-05-16 14:17:19.997272 ngdataenginterface-0.0.4/ngdataenginterface/core/utils_emr.py
+-rw-r--r--   0        0        0     1424 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/core/validations.py
+-rw-r--r--   0        0        0     4362 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/core/write.py
+-rw-r--r--   0        0        0      174 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/__init__.py
+-rw-r--r--   0        0        0     4027 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/cleansing.py
+-rw-r--r--   0        0        0      408 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/export_redshift.py
+-rw-r--r--   0        0        0     6859 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/ngdataenginterface/process/pismo.py
+-rw-r--r--   0        0        0      399 2023-05-16 14:17:19.998272 ngdataenginterface-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 ngdataenginterface-0.0.4/PKG-INFO
```

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/analytical/core.py` & `ngdataenginterface-0.0.4/ngdataenginterface/analytical/core.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/core/aws_interface.py` & `ngdataenginterface-0.0.4/ngdataenginterface/core/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/core/partition.py` & `ngdataenginterface-0.0.4/ngdataenginterface/core/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,21 @@
     for part in partition.split("/"):
         # constructs the partition path from 'ref_date'
         partition_path += part + "=" + PARTITION_MAP[part](date) + "/"
 
     # returns the partition_path without last '/' charactere
     return partition_path[:-1]
 
+
 def get_year_month_day(execution_date: datetime):
     year = execution_date.strftime("%Y")
     month = execution_date.strftime("%m")
     day = execution_date.strftime("%d")
     return year, month, day
 
+
 def get_last_partition(execution_date: datetime):
     previous_year, previous_month, previous_day = get_year_month_day(
         datetime(execution_date.year, execution_date.month, execution_date.day)
         - timedelta(days=1)
     )
-    return datetime(int(previous_year), int(previous_month), int(previous_day))
+    return datetime(int(previous_year), int(previous_month), int(previous_day))
```

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/core/read.py` & `ngdataenginterface-0.0.4/ngdataenginterface/core/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     object_path = read_params["object_path"]
     partition = read_params["partition"]
     file_type = read_params["file_type"]
     schema_path = read_params["schema_path"]
 
     return {
         "path": {
-            "bucket_name": f"s3://ngcash-datalake-{env}-{layer}",
+            "bucket_name": f"s3a://ngcash-datalake-{env}-{layer}",
             "object_path": object_path,
             "partition": partition,
             "file_type": file_type,
         },
         "schema": {
             "bucket_name": f"s3://ngcash-datalake-{env}-repository",
             "object_path": schema_path,
@@ -103,25 +103,22 @@
 def read_data(
     spark: SparkSession,
     type_file: string,
     path,
     schema: StructType,
     header: bool = False,
 ):
-
     if type_file == CSV:
-
         return (
             spark.read.option("header", header)
             .format(type_file)
             .schema(schema)
             .load(path)
         )
     elif type_file == JSON:
-
         return spark.read.format(type_file).schema(schema).load(path)
 
     elif type_file == PARQUET:
         sql = SQLContext(spark)
         return sql.read.schema(schema).parquet(path)
 
     return spark.read.format(type_file).schema(schema).load(path)
@@ -179,10 +176,10 @@
     DataFrame
         the pyspark dataframe
     """
 
     # validate input
     read_input_validation(self)
     # get schema
-    schema = retrive_schema(self["schema"])
+    schema = retrive_schema(self["schema"], meta)
     # read table
     return read_table(self, schema, meta)
```

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/core/schema.py` & `ngdataenginterface-0.0.4/ngdataenginterface/core/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,29 +50,29 @@
         elif "format" in field_metadata.keys():
             field_format = field_metadata["format"]
             if field_format in ("date-time", "date"):
                 field.dataType = TimestampType()
     return pyspark_schema
 
 
-def retrive_schema(self: dict) -> StructType:
+def retrive_schema(self: dict, meta: dict) -> StructType:
     """Constructs the schema from schema path information and boto3 client
 
     Parameters
     ----------
     self : dict
         Dictionary that contains the `bucket_name` and `object_path` of the schema
 
     Returns
     -------
     StructType
         the schema in pyspark StructType format
     """
 
-    datalake_client = boto3.client("s3")
+    datalake_client = meta["client"]
 
     print(f"""Bucket Name : {self["bucket_name"][5:]}""")
     print(f"""Object Path : {self["object_path"]}""")
     # get object from aws s3 bucket
     object = get_object_aws(
         datalake_client,
         self["bucket_name"][5:],
```

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/core/validations.py` & `ngdataenginterface-0.0.4/ngdataenginterface/core/validations.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/core/write.py` & `ngdataenginterface-0.0.4/ngdataenginterface/core/write.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/process/cleansing.py` & `ngdataenginterface-0.0.4/ngdataenginterface/process/cleansing.py`

 * *Files identical despite different names*

### Comparing `ngdataenginterface-0.0.3/ngdataenginterface/process/pismo.py` & `ngdataenginterface-0.0.4/ngdataenginterface/process/pismo.py`

 * *Files identical despite different names*

