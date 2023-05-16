# Comparing `tmp/dagster_meltano-1.2.0.tar.gz` & `tmp/dagster_meltano-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_meltano-1.2.0.tar", max compression
+gzip compressed data, was "dagster_meltano-1.2.1.tar", max compression
```

## Comparing `dagster_meltano-1.2.0.tar` & `dagster_meltano-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/LICENSE
--rw-r--r--   0        0        0     2103 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/README.md
--rw-r--r--   0        0        0      313 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/__init__.py
--rw-r--r--   0        0        0       47 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/exceptions.py
--rw-r--r--   0        0        0     2187 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/generation.py
--rw-r--r--   0        0        0     1723 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/job.py
--rw-r--r--   0        0        0      592 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/logging.yaml
--rw-r--r--   0        0        0     5296 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/meltano_resource.py
--rw-r--r--   0        0        0     4040 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/ops.py
--rw-r--r--   0        0        0      859 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/schedule.py
--rw-r--r--   0        0        0     1011 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/dagster_meltano/utils.py
--rw-r--r--   0        0        0      643 2023-02-18 14:29:23.214447 dagster_meltano-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 dagster_meltano-1.2.0/setup.py
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 dagster_meltano-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2103 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/README.md
+-rw-r--r--   0        0        0      313 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/exceptions.py
+-rw-r--r--   0        0        0     2187 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/generation.py
+-rw-r--r--   0        0        0     1723 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/job.py
+-rw-r--r--   0        0        0      592 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/logging.yaml
+-rw-r--r--   0        0        0     5301 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/meltano_resource.py
+-rw-r--r--   0        0        0     4040 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/ops.py
+-rw-r--r--   0        0        0      859 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/schedule.py
+-rw-r--r--   0        0        0     1011 2023-05-16 12:00:48.846186 dagster_meltano-1.2.1/dagster_meltano/utils.py
+-rw-r--r--   0        0        0      643 2023-05-16 12:00:48.850186 dagster_meltano-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 dagster_meltano-1.2.1/PKG-INFO
```

### Comparing `dagster_meltano-1.2.0/LICENSE` & `dagster_meltano-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/README.md` & `dagster_meltano-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/dagster_meltano/generation.py` & `dagster_meltano-1.2.1/dagster_meltano/generation.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/dagster_meltano/job.py` & `dagster_meltano-1.2.1/dagster_meltano/job.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/dagster_meltano/logging.yaml` & `dagster_meltano-1.2.1/dagster_meltano/logging.yaml`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/dagster_meltano/meltano_resource.py` & `dagster_meltano-1.2.1/dagster_meltano/meltano_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         """The default environment to use when running Meltano commands.
 
         Returns:
             Dict[str, str]: The environment variables.
         """
         return {
             **os.environ.copy(),
-            "MELTANO_CLI_LOG_CONFIG": Path(__file__).parent / "logging.yaml",
+            "MELTANO_CLI_LOG_CONFIG": str(Path(__file__).parent / "logging.yaml"),
             "DBT_USE_COLORS": "false",
             "NO_COLOR": "1",
         }
 
     def execute_command(
         self,
         command: str,
```

### Comparing `dagster_meltano-1.2.0/dagster_meltano/ops.py` & `dagster_meltano-1.2.1/dagster_meltano/ops.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/dagster_meltano/schedule.py` & `dagster_meltano-1.2.1/dagster_meltano/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/dagster_meltano/utils.py` & `dagster_meltano-1.2.1/dagster_meltano/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.2.0/pyproject.toml` & `dagster_meltano-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-meltano"
-version = "1.2.0"
+version = "1.2.1"
 description = "A dagster plugin that allows you to run your Meltano project inside Dagster."
 authors = ["Jules Huisman"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "dagster_meltano" }
 ]
```

### Comparing `dagster_meltano-1.2.0/PKG-INFO` & `dagster_meltano-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-meltano
-Version: 1.2.0
+Version: 1.2.1
 Summary: A dagster plugin that allows you to run your Meltano project inside Dagster.
 License: Apache 2.0
 Author: Jules Huisman
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

