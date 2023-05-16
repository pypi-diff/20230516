# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230513-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230514-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 2386383 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-May-14 04:51 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6787480 b- defN 23-May-14 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-May-14 04:51 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-May-14 04:51 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-May-14 04:51 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-May-14 04:53 tflite_runtime_nightly-2.14.0.dev20230513.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-May-14 04:53 tflite_runtime_nightly-2.14.0.dev20230513.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-May-14 04:53 tflite_runtime_nightly-2.14.0.dev20230513.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-May-14 04:53 tflite_runtime_nightly-2.14.0.dev20230513.dist-info/RECORD
+-rw-rw-r--  2.0 unx       80 b- defN 23-May-15 04:51 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6787480 b- defN 23-May-15 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-May-15 04:51 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-May-15 04:51 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-May-15 04:51 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-May-15 04:53 tflite_runtime_nightly-2.14.0.dev20230514.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-May-15 04:53 tflite_runtime_nightly-2.14.0.dev20230514.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-15 04:53 tflite_runtime_nightly-2.14.0.dev20230514.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-May-15 04:53 tflite_runtime_nightly-2.14.0.dev20230514.dist-info/RECORD
 9 files, 6832369 bytes uncompressed, 2384837 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230513.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230514.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230513.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230514.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230513.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230514.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230513.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230514.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230513'
-__git_version__ = '0.6.0-147793-g852f109317b'
+__version__ = '2.14.0dev20230514'
+__git_version__ = '0.6.0-147797-g07913c4ab49'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230513.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230514.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230513
+Version: 2.14.0.dev20230514
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230513.dist-info/RECORD` & `tflite_runtime_nightly-2.14.0.dev20230514.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=7MdmL2qz1Uvs2csJxjdJSg_Dpap1rf_EgcceGPkQh6Q,80
+tflite_runtime/__init__.py,sha256=z9-fHwv0lUUuVtN0iGQSHGngTZ6GG5xlRI0ym47G_Bg,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=nRtqfUlOKem_9gJfDIUazZRDBpbtq1Exap3Q3ltGgBs,6787480
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.14.0.dev20230513.dist-info/METADATA,sha256=w2acpJobnWAvCz976bfQSp4d0c3GlB25xfALAUw5y7I,1440
-tflite_runtime_nightly-2.14.0.dev20230513.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
-tflite_runtime_nightly-2.14.0.dev20230513.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.14.0.dev20230513.dist-info/RECORD,,
+tflite_runtime_nightly-2.14.0.dev20230514.dist-info/METADATA,sha256=vhHMSK8TMdRT2ZoUmGC0sv9Q0e57y8xdKqwD5rfF_Us,1440
+tflite_runtime_nightly-2.14.0.dev20230514.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
+tflite_runtime_nightly-2.14.0.dev20230514.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.14.0.dev20230514.dist-info/RECORD,,
```

