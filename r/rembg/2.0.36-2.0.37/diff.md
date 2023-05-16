# Comparing `tmp/rembg-2.0.36.tar.gz` & `tmp/rembg-2.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.36.tar", last modified: Tue May  9 04:22:46 2023, max compression
+gzip compressed data, was "rembg-2.0.37.tar", last modified: Tue May 16 01:12:04 2023, max compression
```

## Comparing `rembg-2.0.36.tar` & `rembg-2.0.37.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 04:22:33.000000 rembg-2.0.36/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 04:22:33.000000 rembg-2.0.36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-05-09 04:22:46.167957 rembg-2.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-05-09 04:22:33.000000 rembg-2.0.36/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-09 04:22:33.000000 rembg-2.0.36/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/dis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-09 04:22:33.000000 rembg-2.0.36/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:22:46.167957 rembg-2.0.36/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 04:22:46.000000 rembg-2.0.36/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 04:22:33.000000 rembg-2.0.36/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 04:22:33.000000 rembg-2.0.36/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-09 04:22:46.167957 rembg-2.0.36/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-09 04:22:33.000000 rembg-2.0.36/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-09 04:22:33.000000 rembg-2.0.36/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:12:04.186726 rembg-2.0.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 01:11:53.000000 rembg-2.0.37/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-16 01:11:53.000000 rembg-2.0.37/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-05-16 01:12:04.186726 rembg-2.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-05-16 01:11:53.000000 rembg-2.0.37/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-16 01:11:53.000000 rembg-2.0.37/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:12:04.186726 rembg-2.0.37/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 01:12:04.186726 rembg-2.0.37/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:12:04.186726 rembg-2.0.37/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:12:04.186726 rembg-2.0.37/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/dis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-16 01:11:53.000000 rembg-2.0.37/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:12:04.182726 rembg-2.0.37/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-05-16 01:12:04.000000 rembg-2.0.37/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-16 01:12:04.000000 rembg-2.0.37/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:12:04.000000 rembg-2.0.37/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 01:12:04.000000 rembg-2.0.37/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 01:12:04.000000 rembg-2.0.37/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 01:12:04.000000 rembg-2.0.37/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 01:11:53.000000 rembg-2.0.37/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-16 01:11:53.000000 rembg-2.0.37/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 01:12:04.186726 rembg-2.0.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-16 01:11:53.000000 rembg-2.0.37/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-16 01:11:53.000000 rembg-2.0.37/versioneer.py
```

### Comparing `rembg-2.0.36/LICENSE.txt` & `rembg-2.0.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/PKG-INFO` & `rembg-2.0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.36
+Version: 2.0.37
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.36 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.37 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `rembg-2.0.36/README.md` & `rembg-2.0.37/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/bg.py` & `rembg-2.0.37/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/commands/b_command.py` & `rembg-2.0.37/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/commands/i_command.py` & `rembg-2.0.37/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/commands/p_command.py` & `rembg-2.0.37/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/commands/s_command.py` & `rembg-2.0.37/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/session_factory.py` & `rembg-2.0.37/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/sessions/__init__.py` & `rembg-2.0.37/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/rembg/sessions/base.py` & `rembg-2.0.37/rembg/sessions/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,18 @@
             .astype(np.float32)
         }
 
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         raise NotImplementedError
 
     @classmethod
+    def checksum_disabled(cls, *args, **kwargs):
+        return os.getenv("MODEL_CHECKSUM_DISABLED", None) is not None
+
+    @classmethod
     def u2net_home(cls, *args, **kwargs):
         return os.path.expanduser(
             os.getenv(
                 "U2NET_HOME", os.path.join(os.getenv("XDG_DATA_HOME", "~"), ".u2net")
             )
         )
```

### Comparing `rembg-2.0.36/rembg/sessions/dis.py` & `rembg-2.0.37/rembg/sessions/u2netp.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
-class DisSession(BaseSession):
+class U2netpSession(BaseSession):
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
-            self.normalize(img, (0.485, 0.456, 0.406), (1.0, 1.0, 1.0), (1024, 1024)),
+            self.normalize(
+                img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
+            ),
         )
 
         pred = ort_outs[0][:, 0, :, :]
 
         ma = np.max(pred)
         mi = np.min(pred)
 
@@ -29,19 +31,21 @@
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname = f"{cls.name()}.onnx"
         pooch.retrieve(
-            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx",
-            "md5:fc16ebd8b0c10d971d3513d564d01e29",
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:8e83ca70e441ab06c318d82300c84806",
             fname=fname,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return os.path.join(cls.u2net_home(), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
-        return "isnet-general-use"
+        return "u2netp"
```

### Comparing `rembg-2.0.36/rembg/sessions/sam.py` & `rembg-2.0.37/rembg/sessions/sam.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,25 +137,29 @@
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname_encoder = f"{cls.name()}_encoder.onnx"
         fname_decoder = f"{cls.name()}_decoder.onnx"
 
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx",
-            "md5:13d97c5c79ab13ef86d67cbde5f1b250",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:13d97c5c79ab13ef86d67cbde5f1b250",
             fname=fname_encoder,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx",
-            "md5:fa3d1c36a3187d3de1c8deebf33dd127",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:fa3d1c36a3187d3de1c8deebf33dd127",
             fname=fname_decoder,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return (
             os.path.join(cls.u2net_home(), fname_encoder),
             os.path.join(cls.u2net_home(), fname_decoder),
         )
```

### Comparing `rembg-2.0.36/rembg/sessions/silueta.py` & `rembg-2.0.37/rembg/sessions/silueta.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,17 +32,19 @@
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname = f"{cls.name()}.onnx"
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx",
-            "md5:55e59e0d8062d2f5d013f4725ee84782",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:55e59e0d8062d2f5d013f4725ee84782",
             fname=fname,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return os.path.join(cls.u2net_home(), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
```

### Comparing `rembg-2.0.36/rembg/sessions/u2net.py` & `rembg-2.0.37/rembg/sessions/u2net.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,19 @@
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname = f"{cls.name()}.onnx"
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx",
-            "md5:60024c5c889badc19c04ad937298a77b",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:60024c5c889badc19c04ad937298a77b",
             fname=fname,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return os.path.join(cls.u2net_home(), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
```

### Comparing `rembg-2.0.36/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.37/rembg/sessions/u2net_cloth_seg.py`

 * *Files 13% similar despite different names*

```diff
@@ -93,17 +93,19 @@
         return masks
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname = f"{cls.name()}.onnx"
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx",
-            "md5:2434d1f3cb744e0e49386c906e5a08bb",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:2434d1f3cb744e0e49386c906e5a08bb",
             fname=fname,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return os.path.join(cls.u2net_home(), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
```

### Comparing `rembg-2.0.36/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.37/rembg/sessions/dis.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
-class U2netHumanSegSession(BaseSession):
+class DisSession(BaseSession):
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
-            self.normalize(
-                img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
-            ),
+            self.normalize(img, (0.485, 0.456, 0.406), (1.0, 1.0, 1.0), (1024, 1024)),
         )
 
         pred = ort_outs[0][:, 0, :, :]
 
         ma = np.max(pred)
         mi = np.min(pred)
 
@@ -31,19 +29,21 @@
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname = f"{cls.name()}.onnx"
         pooch.retrieve(
-            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx",
-            "md5:c09ddc2e0104f800e3e1bb4652583d1f",
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:fc16ebd8b0c10d971d3513d564d01e29",
             fname=fname,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return os.path.join(cls.u2net_home(), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
-        return "u2net_human_seg"
+        return "isnet-general-use"
```

### Comparing `rembg-2.0.36/rembg/sessions/u2netp.py` & `rembg-2.0.37/rembg/sessions/u2net_human_seg.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
-class U2netpSession(BaseSession):
+class U2netHumanSegSession(BaseSession):
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
             self.normalize(
                 img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
             ),
         )
@@ -31,19 +31,21 @@
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
         fname = f"{cls.name()}.onnx"
         pooch.retrieve(
-            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx",
-            "md5:8e83ca70e441ab06c318d82300c84806",
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx",
+            None
+            if cls.checksum_disabled(*args, **kwargs)
+            else "md5:c09ddc2e0104f800e3e1bb4652583d1f",
             fname=fname,
-            path=cls.u2net_home(),
+            path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return os.path.join(cls.u2net_home(), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
-        return "u2netp"
+        return "u2net_human_seg"
```

### Comparing `rembg-2.0.36/rembg.egg-info/PKG-INFO` & `rembg-2.0.37/rembg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.36
+Version: 2.0.37
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rembg Version: 2.0.36 Summary: Remove image
+Metadata-Version: 2.1 Name: rembg Version: 2.0.37 Summary: Remove image
 background Home-page: https://github.com/danielgatis/rembg Author: Daniel Gatis
 Author-email: danielgatis@gmail.com License: UNKNOWN Keywords:
 remove,background,u2net Platform: UNKNOWN Classifier: License :: OSI Approved
 :: MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
```

### Comparing `rembg-2.0.36/rembg.egg-info/SOURCES.txt` & `rembg-2.0.37/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/setup.py` & `rembg-2.0.37/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.36/versioneer.py` & `rembg-2.0.37/versioneer.py`

 * *Files identical despite different names*

