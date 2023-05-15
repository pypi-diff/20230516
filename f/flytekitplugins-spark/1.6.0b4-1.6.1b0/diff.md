# Comparing `tmp/flytekitplugins-spark-1.6.0b4.tar.gz` & `tmp/flytekitplugins-spark-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-spark-1.6.0b4.tar", last modified: Tue May  9 00:42:40 2023, max compression
+gzip compressed data, was "flytekitplugins-spark-1.6.1b0.tar", last modified: Mon May 15 22:07:10 2023, max compression
```

## Comparing `flytekitplugins-spark-1.6.0b4.tar` & `flytekitplugins-spark-1.6.1b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/pyspark_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/sd_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:40.000000 flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-09 00:42:15.000000 flytekitplugins-spark-1.6.0b4/scripts/flytekit_install_spark3.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:40.312776 flytekitplugins-spark-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-09 00:42:30.000000 flytekitplugins-spark-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:10.475781 flytekitplugins-spark-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 22:07:10.475781 flytekitplugins-spark-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:10.471781 flytekitplugins-spark-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:10.475781 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/pyspark_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/sd_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:10.475781 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:10.000000 flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:10.475781 flytekitplugins-spark-1.6.1b0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-15 22:06:44.000000 flytekitplugins-spark-1.6.1b0/scripts/flytekit_install_spark3.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:10.475781 flytekitplugins-spark-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-15 22:07:00.000000 flytekitplugins-spark-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-spark-1.6.0b4/PKG-INFO` & `flytekitplugins-spark-1.6.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b4/README.md` & `flytekitplugins-spark-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/__init__.py` & `flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/models.py` & `flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/pyspark_transformers.py` & `flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/pyspark_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/schema.py` & `flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/sd_transformers.py` & `flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins/spark/task.py` & `flytekitplugins-spark-1.6.1b0/flytekitplugins/spark/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,22 @@
     """
     Use this to configure a SparkContext for a your task. Task's marked with this will automatically execute
     natively onto K8s as a distributed execution of spark
 
     Args:
         spark_conf: Dictionary of spark config. The variables should match what spark expects
         hadoop_conf: Dictionary of hadoop conf. The variables should match a typical hadoop configuration for spark
+        executor_path: Python binary executable to use for PySpark in driver and executor.
+        applications_path: MainFile is the path to a bundled JAR, Python, or R file of the application to execute.
     """
 
     spark_conf: Optional[Dict[str, str]] = None
     hadoop_conf: Optional[Dict[str, str]] = None
+    executor_path: Optional[str] = None
+    applications_path: Optional[str] = None
 
     def __post_init__(self):
         if self.spark_conf is None:
             self.spark_conf = {}
 
         if self.hadoop_conf is None:
             self.hadoop_conf = {}
@@ -103,16 +107,16 @@
         self,
         task_config: Spark,
         task_function: Callable,
         container_image: Optional[Union[str, ImageSpec]] = None,
         **kwargs,
     ):
         self.sess: Optional[SparkSession] = None
-        self._default_executor_path: Optional[str] = None
-        self._default_applications_path: Optional[str] = None
+        self._default_executor_path: Optional[str] = task_config.executor_path
+        self._default_applications_path: Optional[str] = task_config.applications_path
 
         if isinstance(container_image, ImageSpec):
             if container_image.base_image is None:
                 img = f"cr.flyte.org/flyteorg/flytekit:spark-{DefaultImages.get_version_suffix()}"
                 container_image.base_image = img
                 # default executor path and applications path in apache/spark-py:3.3.1
                 self._default_executor_path = "/usr/bin/python3"
```

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/PKG-INFO` & `flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.6.0b4/flytekitplugins_spark.egg-info/SOURCES.txt` & `flytekitplugins-spark-1.6.1b0/flytekitplugins_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/scripts/flytekit_install_spark3.sh` & `flytekitplugins-spark-1.6.1b0/scripts/flytekit_install_spark3.sh`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.6.0b4/setup.py` & `flytekitplugins-spark-1.6.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "spark"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pyspark>=3.0.0"]
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Spark 3 plugin for flytekit",
```

