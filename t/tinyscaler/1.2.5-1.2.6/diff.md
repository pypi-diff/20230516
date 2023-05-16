# Comparing `tmp/tinyscaler-1.2.5.tar.gz` & `tmp/tinyscaler-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyscaler-1.2.5.tar", last modified: Tue May 16 02:00:37 2023, max compression
+gzip compressed data, was "tinyscaler-1.2.6.tar", last modified: Tue May 16 03:44:41 2023, max compression
```

## Comparing `tinyscaler-1.2.5.tar` & `tinyscaler-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-05-16 02:00:37.254712 tinyscaler-1.2.5/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1078 2023-05-15 22:23:42.000000 tinyscaler-1.2.5/LICENSE
--rw-r--r--   0 ericl     (1000) ericl     (1001)      133 2023-05-15 22:23:42.000000 tinyscaler-1.2.5/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4211 2023-05-16 02:00:37.254712 tinyscaler-1.2.5/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3113 2023-05-16 01:59:07.000000 tinyscaler-1.2.5/README.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1324 2023-05-16 01:57:58.000000 tinyscaler-1.2.5/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-05-16 02:00:37.254712 tinyscaler-1.2.5/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)      776 2023-05-15 22:23:42.000000 tinyscaler-1.2.5/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-05-16 02:00:37.251378 tinyscaler-1.2.5/src/
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17345 2023-05-15 22:23:42.000000 tinyscaler-1.2.5/src/scaler.c
--rw-r--r--   0 ericl     (1000) ericl     (1001)      762 2023-05-15 22:23:42.000000 tinyscaler-1.2.5/src/scaler.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)   928720 2023-05-16 02:00:37.000000 tinyscaler-1.2.5/src/tinyscaler.c
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-05-16 02:00:37.254712 tinyscaler-1.2.5/src/tinyscaler.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4211 2023-05-16 02:00:37.000000 tinyscaler-1.2.5/src/tinyscaler.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      304 2023-05-16 02:00:37.000000 tinyscaler-1.2.5/src/tinyscaler.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-05-16 02:00:37.000000 tinyscaler-1.2.5/src/tinyscaler.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)       14 2023-05-16 02:00:37.000000 tinyscaler-1.2.5/src/tinyscaler.egg-info/requires.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-05-16 02:00:37.000000 tinyscaler-1.2.5/src/tinyscaler.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)     5227 2023-05-15 22:23:42.000000 tinyscaler-1.2.5/src/tinyscaler.pyx
+drwxrwxrwx   0        0        0        0 2023-05-16 03:44:41.048887 tinyscaler-1.2.6/
+-rw-rw-rw-   0        0        0     1099 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4297 2023-05-16 03:44:41.048887 tinyscaler-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3174 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/README.md
+-rw-rw-rw-   0        0        0     1360 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:44:41.048887 tinyscaler-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:44:41.033317 tinyscaler-1.2.6/src/
+-rw-rw-rw-   0        0        0    17793 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/src/scaler.c
+-rw-rw-rw-   0        0        0      790 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/src/scaler.h
+-rw-rw-rw-   0        0        0   928725 2023-05-16 03:44:40.000000 tinyscaler-1.2.6/src/tinyscaler.c
+drwxrwxrwx   0        0        0        0 2023-05-16 03:44:41.048887 tinyscaler-1.2.6/src/tinyscaler.egg-info/
+-rw-rw-rw-   0        0        0     4297 2023-05-16 03:44:41.000000 tinyscaler-1.2.6/src/tinyscaler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-05-16 03:44:41.000000 tinyscaler-1.2.6/src/tinyscaler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:44:41.000000 tinyscaler-1.2.6/src/tinyscaler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 03:44:41.000000 tinyscaler-1.2.6/src/tinyscaler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 03:44:41.000000 tinyscaler-1.2.6/src/tinyscaler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5371 2023-05-16 03:43:54.000000 tinyscaler-1.2.6/src/tinyscaler.pyx
```

### Comparing `tinyscaler-1.2.5/PKG-INFO` & `tinyscaler-1.2.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-Metadata-Version: 2.1
-Name: tinyscaler
-Version: 1.2.5
-Summary: A tiny, simple image scaler.
-Author-email: Farama Foundation <contact@farama.org>
-License: MIT License
-Project-URL: Homepage, https://farama.org
-Project-URL: Repository, https://github.com/Farama-Foundation/TinyScaler
-Project-URL: Documentation, https://github.com/Farama-Foundation/TinyScaler
-Project-URL: Bug Report, https://github.com/Farama-Foundation/TinyScaler/issues
-Keywords: Reinforcement Learning,Gymnasium,PettingZoo
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Farama-Foundation/TinyScaler/main/tinyscaler-text.png" width="500px"/>
-</p>
-
-A small CPU image scaling library with SIMD support on x86_64 and Arm (Neon). This project is aimed to replace OpenCV for image resizing, resolving installation inconveniences and compatibility issues. We developed this for future use in Gymnasium and PettingZoo wrappers.
-
-## Installation
-You can install from PyPI using `pip install tinyscaler`. Linux and macOS with Python 3.7, 3.8, 3.9, 3.10 and 3.11 are supported.
-
-## Usage
-Tinyscaler contains a single external function, `scale` that using a numpy array input for the image and the new resized shape, returns the resized image. 
-
-```python
-import numpy as np
-import tinyscaler
-
-img = np.random.rand(64, 64, 4).astype(np.float32)
-
-resize_img = tinyscaler.scale(img, (32, 32))
-print(resize_img.shape, resize_img.dtype)  # (32, 32) np.float32
-```
-
-TinyScaler supports mode='area', mode='bilinear', and mode='nearest' filtering. It also allows one to pass a destination buffer in order to avoid duplicate memory allocations.
-
-Area filtering is only really useful for downscaling, bilinear will be used even when area filtering is set if upscaling. Area filtering is also likely not worth it when downscaling less than or equal to 2x.
-
-TinyScaler is used through a single function. The full signature is:
-
-```python
-scale(src : np.ndarray, size : tuple, mode='area', dst : np.ndarray = None)
-```
-
-Note that the `size` tuple parameter is (width, height). However, the numpy arrays have dimensions ordered as (height, width, channels). This is similar to OpenCV.
-
-TinyScaler expects a contiguous numpy array. If it is not contiguous, it will throw an error. You can make a non-contiguous numpy array contiguous by calling `np.ascontiguousarray`. Usually a numpy array will already be contiguous.
-
-If the final array dimension is not 4 (RGBA), it will automatically convert to it. Further, if the array is uint8, it will be converted to float32. So the prefered array has a shape `(height, width, 4)` and `dtype=np.float32`.
-
-Finally, downscaling is the focus of TinyScaler. It can also upscale, but it will not be as fast as a more complex separable algorithm in that case.
-
-## Performance
-In a [simple benchmark](./examples/benchmark.py), we resized the same image (4928x3279) down to (852x567) 100 times using bilinear filtering with several libraries. Here are the times (in seconds) spent (measured with Python's perf_counter) on a AMD 1950x:
-
-```
-Time elapsed for tinyscaler: 0.7968465110002398
-Time elapsed for OpenCV: 0.48667862100001
-Time elapsed for Pillow: 12.672875003999707
-Time elapsed for skimage: 164.45401711399973
-```
-
-And with area filtering (just TinyScaler and OpenCV):
-
-```
-Time elapsed for tinyscaler: 4.34793155800071
-Time elapsed for OpenCV: 8.118138265999733
-```
-
-All methods were forced to use a single thread. OpenCV is slightly faster than TinyScaler for bilinear filtering, but TinyScaler remains very fast regardless.
-
-Interestingly, for area filtering, TinyScaler is faster (almost 2x).
-
+Metadata-Version: 2.1
+Name: tinyscaler
+Version: 1.2.6
+Summary: A tiny, simple image scaler.
+Author-email: Farama Foundation <contact@farama.org>
+License: MIT License
+Project-URL: Homepage, https://farama.org
+Project-URL: Repository, https://github.com/Farama-Foundation/TinyScaler
+Project-URL: Documentation, https://github.com/Farama-Foundation/TinyScaler
+Project-URL: Bug Report, https://github.com/Farama-Foundation/TinyScaler/issues
+Keywords: Reinforcement Learning,Gymnasium,PettingZoo
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Farama-Foundation/TinyScaler/main/tinyscaler-text.png" width="500px"/>
+</p>
+
+A small CPU image scaling library with SIMD support on x86_64 and Arm (Neon). This project is aimed to replace OpenCV for image resizing, resolving installation inconveniences and compatibility issues. We developed this for future use in Gymnasium and PettingZoo wrappers.
+
+## Installation
+You can install from PyPI using `pip install tinyscaler`. Linux and macOS with Python 3.7, 3.8, 3.9, 3.10 and 3.11 are supported.
+
+## Usage
+Tinyscaler contains a single external function, `scale` that using a numpy array input for the image and the new resized shape, returns the resized image. 
+
+```python
+import numpy as np
+import tinyscaler
+
+img = np.random.rand(64, 64, 4).astype(np.float32)
+
+resize_img = tinyscaler.scale(img, (32, 32))
+print(resize_img.shape, resize_img.dtype)  # (32, 32) np.float32
+```
+
+TinyScaler supports mode='area', mode='bilinear', and mode='nearest' filtering. It also allows one to pass a destination buffer in order to avoid duplicate memory allocations.
+
+Area filtering is only really useful for downscaling, bilinear will be used even when area filtering is set if upscaling. Area filtering is also likely not worth it when downscaling less than or equal to 2x.
+
+TinyScaler is used through a single function. The full signature is:
+
+```python
+scale(src : np.ndarray, size : tuple, mode='area', dst : np.ndarray = None)
+```
+
+Note that the `size` tuple parameter is (width, height). However, the numpy arrays have dimensions ordered as (height, width, channels). This is similar to OpenCV.
+
+TinyScaler expects a contiguous numpy array. If it is not contiguous, it will throw an error. You can make a non-contiguous numpy array contiguous by calling `np.ascontiguousarray`. Usually a numpy array will already be contiguous.
+
+If the final array dimension is not 4 (RGBA), it will automatically convert to it. Further, if the array is uint8, it will be converted to float32. So the prefered array has a shape `(height, width, 4)` and `dtype=np.float32`.
+
+Finally, downscaling is the focus of TinyScaler. It can also upscale, but it will not be as fast as a more complex separable algorithm in that case.
+
+## Performance
+In a [simple benchmark](./examples/benchmark.py), we resized the same image (4928x3279) down to (852x567) 100 times using bilinear filtering with several libraries. Here are the times (in seconds) spent (measured with Python's perf_counter) on a AMD 1950x:
+
+```
+Time elapsed for tinyscaler: 0.7968465110002398
+Time elapsed for OpenCV: 0.48667862100001
+Time elapsed for Pillow: 12.672875003999707
+Time elapsed for skimage: 164.45401711399973
+```
+
+And with area filtering (just TinyScaler and OpenCV):
+
+```
+Time elapsed for tinyscaler: 4.34793155800071
+Time elapsed for OpenCV: 8.118138265999733
+```
+
+All methods were forced to use a single thread. OpenCV is slightly faster than TinyScaler for bilinear filtering, but TinyScaler remains very fast regardless.
+
+Interestingly, for area filtering, TinyScaler is faster (almost 2x).
+
```

### Comparing `tinyscaler-1.2.5/README.md` & `tinyscaler-1.2.6/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Farama-Foundation/TinyScaler/main/tinyscaler-text.png" width="500px"/>
-</p>
-
-A small CPU image scaling library with SIMD support on x86_64 and Arm (Neon). This project is aimed to replace OpenCV for image resizing, resolving installation inconveniences and compatibility issues. We developed this for future use in Gymnasium and PettingZoo wrappers.
-
-## Installation
-You can install from PyPI using `pip install tinyscaler`. Linux and macOS with Python 3.7, 3.8, 3.9, 3.10 and 3.11 are supported.
-
-## Usage
-Tinyscaler contains a single external function, `scale` that using a numpy array input for the image and the new resized shape, returns the resized image. 
-
-```python
-import numpy as np
-import tinyscaler
-
-img = np.random.rand(64, 64, 4).astype(np.float32)
-
-resize_img = tinyscaler.scale(img, (32, 32))
-print(resize_img.shape, resize_img.dtype)  # (32, 32) np.float32
-```
-
-TinyScaler supports mode='area', mode='bilinear', and mode='nearest' filtering. It also allows one to pass a destination buffer in order to avoid duplicate memory allocations.
-
-Area filtering is only really useful for downscaling, bilinear will be used even when area filtering is set if upscaling. Area filtering is also likely not worth it when downscaling less than or equal to 2x.
-
-TinyScaler is used through a single function. The full signature is:
-
-```python
-scale(src : np.ndarray, size : tuple, mode='area', dst : np.ndarray = None)
-```
-
-Note that the `size` tuple parameter is (width, height). However, the numpy arrays have dimensions ordered as (height, width, channels). This is similar to OpenCV.
-
-TinyScaler expects a contiguous numpy array. If it is not contiguous, it will throw an error. You can make a non-contiguous numpy array contiguous by calling `np.ascontiguousarray`. Usually a numpy array will already be contiguous.
-
-If the final array dimension is not 4 (RGBA), it will automatically convert to it. Further, if the array is uint8, it will be converted to float32. So the prefered array has a shape `(height, width, 4)` and `dtype=np.float32`.
-
-Finally, downscaling is the focus of TinyScaler. It can also upscale, but it will not be as fast as a more complex separable algorithm in that case.
-
-## Performance
-In a [simple benchmark](./examples/benchmark.py), we resized the same image (4928x3279) down to (852x567) 100 times using bilinear filtering with several libraries. Here are the times (in seconds) spent (measured with Python's perf_counter) on a AMD 1950x:
-
-```
-Time elapsed for tinyscaler: 0.7968465110002398
-Time elapsed for OpenCV: 0.48667862100001
-Time elapsed for Pillow: 12.672875003999707
-Time elapsed for skimage: 164.45401711399973
-```
-
-And with area filtering (just TinyScaler and OpenCV):
-
-```
-Time elapsed for tinyscaler: 4.34793155800071
-Time elapsed for OpenCV: 8.118138265999733
-```
-
-All methods were forced to use a single thread. OpenCV is slightly faster than TinyScaler for bilinear filtering, but TinyScaler remains very fast regardless.
-
-Interestingly, for area filtering, TinyScaler is faster (almost 2x).
-
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Farama-Foundation/TinyScaler/main/tinyscaler-text.png" width="500px"/>
+</p>
+
+A small CPU image scaling library with SIMD support on x86_64 and Arm (Neon). This project is aimed to replace OpenCV for image resizing, resolving installation inconveniences and compatibility issues. We developed this for future use in Gymnasium and PettingZoo wrappers.
+
+## Installation
+You can install from PyPI using `pip install tinyscaler`. Linux and macOS with Python 3.7, 3.8, 3.9, 3.10 and 3.11 are supported.
+
+## Usage
+Tinyscaler contains a single external function, `scale` that using a numpy array input for the image and the new resized shape, returns the resized image. 
+
+```python
+import numpy as np
+import tinyscaler
+
+img = np.random.rand(64, 64, 4).astype(np.float32)
+
+resize_img = tinyscaler.scale(img, (32, 32))
+print(resize_img.shape, resize_img.dtype)  # (32, 32) np.float32
+```
+
+TinyScaler supports mode='area', mode='bilinear', and mode='nearest' filtering. It also allows one to pass a destination buffer in order to avoid duplicate memory allocations.
+
+Area filtering is only really useful for downscaling, bilinear will be used even when area filtering is set if upscaling. Area filtering is also likely not worth it when downscaling less than or equal to 2x.
+
+TinyScaler is used through a single function. The full signature is:
+
+```python
+scale(src : np.ndarray, size : tuple, mode='area', dst : np.ndarray = None)
+```
+
+Note that the `size` tuple parameter is (width, height). However, the numpy arrays have dimensions ordered as (height, width, channels). This is similar to OpenCV.
+
+TinyScaler expects a contiguous numpy array. If it is not contiguous, it will throw an error. You can make a non-contiguous numpy array contiguous by calling `np.ascontiguousarray`. Usually a numpy array will already be contiguous.
+
+If the final array dimension is not 4 (RGBA), it will automatically convert to it. Further, if the array is uint8, it will be converted to float32. So the prefered array has a shape `(height, width, 4)` and `dtype=np.float32`.
+
+Finally, downscaling is the focus of TinyScaler. It can also upscale, but it will not be as fast as a more complex separable algorithm in that case.
+
+## Performance
+In a [simple benchmark](./examples/benchmark.py), we resized the same image (4928x3279) down to (852x567) 100 times using bilinear filtering with several libraries. Here are the times (in seconds) spent (measured with Python's perf_counter) on a AMD 1950x:
+
+```
+Time elapsed for tinyscaler: 0.7968465110002398
+Time elapsed for OpenCV: 0.48667862100001
+Time elapsed for Pillow: 12.672875003999707
+Time elapsed for skimage: 164.45401711399973
+```
+
+And with area filtering (just TinyScaler and OpenCV):
+
+```
+Time elapsed for tinyscaler: 4.34793155800071
+Time elapsed for OpenCV: 8.118138265999733
+```
+
+All methods were forced to use a single thread. OpenCV is slightly faster than TinyScaler for bilinear filtering, but TinyScaler remains very fast regardless.
+
+Interestingly, for area filtering, TinyScaler is faster (almost 2x).
+
```

### Comparing `tinyscaler-1.2.5/pyproject.toml` & `tinyscaler-1.2.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# Package ######################################################################
-
-[build-system]
-requires = ["setuptools", "wheel", "Cython"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "tinyscaler"
-description = "A tiny, simple image scaler."
-readme = "README.md"
-requires-python = ">= 3.7, < 3.12"
-authors = [{ name = "Farama Foundation", email = "contact@farama.org" }]
-license = { text = "MIT License" }
-keywords = ["Reinforcement Learning", "Gymnasium", "PettingZoo"]
-classifiers = [
-    "Development Status :: 4 - Beta",  # change to `5 - Production/Stable` when ready
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    'Intended Audience :: Science/Research',
-    'Topic :: Scientific/Engineering :: Artificial Intelligence',
-]
-version="1.2.5"
-dependencies = [
-    "numpy >=1.21.0",
-]
-
-[project.urls]
-Homepage = "https://farama.org"
-Repository = "https://github.com/Farama-Foundation/TinyScaler"
-Documentation = "https://github.com/Farama-Foundation/TinyScaler"
-"Bug Report" = "https://github.com/Farama-Foundation/TinyScaler/issues"
+# Package ######################################################################
+
+[build-system]
+requires = ["setuptools", "wheel", "Cython"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "tinyscaler"
+description = "A tiny, simple image scaler."
+readme = "README.md"
+requires-python = ">= 3.7, < 3.12"
+authors = [{ name = "Farama Foundation", email = "contact@farama.org" }]
+license = { text = "MIT License" }
+keywords = ["Reinforcement Learning", "Gymnasium", "PettingZoo"]
+classifiers = [
+    "Development Status :: 4 - Beta",  # change to `5 - Production/Stable` when ready
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    'Intended Audience :: Science/Research',
+    'Topic :: Scientific/Engineering :: Artificial Intelligence',
+]
+version="1.2.6"
+dependencies = [
+    "numpy >=1.21.0",
+]
+
+[project.urls]
+Homepage = "https://farama.org"
+Repository = "https://github.com/Farama-Foundation/TinyScaler"
+Documentation = "https://github.com/Farama-Foundation/TinyScaler"
+"Bug Report" = "https://github.com/Farama-Foundation/TinyScaler/issues"
```

### Comparing `tinyscaler-1.2.5/setup.py` & `tinyscaler-1.2.6/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import platform
-
-from Cython.Build import cythonize
-from setuptools import Extension, setup
-
-ext_modules = []
-
-if platform.system() == "Windows":  # Windows
-    ext_modules = [Extension("tinyscaler", ["src/*.pyx"])]
-else:  # Not Windows
-    if platform.machine() == "x86_64":  # Detect x86_64 platform
-        ext_modules = [Extension("tinyscaler", ["src/*.pyx"])]
-    else:  # Arm assumed
-        ext_modules = [
-            Extension(
-                "tinyscaler",
-                ["src/*.pyx"],
-                extra_compile_args=["-mfpu=neon"],
-                extra_link_args=["-mfpu=neon"],
-            )
-        ]
-
-setup(
-    name="tinyscaler",
-    ext_modules=cythonize(
-        ext_modules, language_level=3, compiler_directives={"annotation_typing": False}
-    ),
-)
+import platform
+
+from Cython.Build import cythonize
+from setuptools import Extension, setup
+
+ext_modules = []
+
+if platform.system() == "Windows":  # Windows
+    ext_modules = [Extension("tinyscaler", ["src/*.pyx"])]
+else:  # Not Windows
+    if platform.machine() == "x86_64":  # Detect x86_64 platform
+        ext_modules = [Extension("tinyscaler", ["src/*.pyx"])]
+    else:  # Arm assumed
+        ext_modules = [
+            Extension(
+                "tinyscaler",
+                ["src/*.pyx"],
+                extra_compile_args=["-mfpu=neon"],
+                extra_link_args=["-mfpu=neon"],
+            )
+        ]
+
+setup(
+    name="tinyscaler",
+    ext_modules=cythonize(
+        ext_modules, language_level=3, compiler_directives={"annotation_typing": False}
+    ),
+)
```

### Comparing `tinyscaler-1.2.5/src/scaler.c` & `tinyscaler-1.2.6/src/scaler.c`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,448 +1,448 @@
-#include "scaler.h"
-
-// Nearest does not use SIMD
-void scale_nearest_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)src_width / (f32)dst_width;
-    f32 ratio_y = (f32)src_height / (f32)dst_height;
-    i32 dst_width4 = dst_width << 2;
-    i32 src_width4 = src_width << 2;
-
-    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-        i32 src_y = (i32)((dst_y + 0.5f) * ratio_y);
-
-        i32 dst_offset4 = dst_width4 * dst_y;
-        i32 src_offset4 = src_width4 * src_y;
-
-        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-            i32 src_x = (i32)((dst_x + 0.5f) * ratio_x);
-
-            memcpy(&dst[(dst_x << 2) + dst_offset4], &src[(src_x << 2) + src_offset4], RGBA32F_SIZE);
-        }
-    }
-}
-
-#if defined(__x86_64__) // SSE implementation
-
-void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)(src_width - 1) / (f32)dst_width;
-    f32 ratio_y = (f32)(src_height - 1) / (f32)dst_height;
-    i32 dst_width4 = dst_width << 2;
-    i32 src_width4 = src_width << 2;
-    i32 src_width4_4 = src_width4 + 4;
-
-    if ((((size_t)src | (size_t)dst) & 0x0f) == 0) { // Aligned memory
-        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-            f32 src_y_f = (dst_y + 0.5f) * ratio_y;
-            i32 src_y = (i32)src_y_f;
-            f32 interp_y = src_y_f - src_y;
-
-            __m128 iy = _mm_set1_ps(interp_y);
-            __m128 iy1 = _mm_set1_ps(1.0f - interp_y);
-
-            i32 dst_offset4 = dst_width4 * dst_y;
-            i32 src_offset4 = src_width4 * src_y;
-
-            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-                f32 src_x_f = (dst_x + 0.5f) * ratio_x;
-                i32 src_x = (i32)src_x_f;
-                f32 interp_x = src_x_f - src_x;
-
-                i32 dst_start = (dst_x << 2) + dst_offset4;
-
-                f32* src_start00 = src + (src_x << 2) + src_offset4;
-
-                __m128 ix = _mm_set1_ps(interp_x);
-                __m128 ix1 = _mm_set1_ps(1.0f - interp_x);
-
-                __m128 p00 = _mm_load_ps(src_start00);
-                __m128 p01 = _mm_load_ps(src_start00 + 4);
-                __m128 p10 = _mm_load_ps(src_start00 + src_width4);
-                __m128 p11 = _mm_load_ps(src_start00 + src_width4_4);
-
-                p00 = _mm_add_ps(_mm_mul_ps(p00, iy1), _mm_mul_ps(p10, iy));
-                p01 = _mm_add_ps(_mm_mul_ps(p01, iy1), _mm_mul_ps(p11, iy));
-
-                p00 = _mm_add_ps(_mm_mul_ps(p00, ix1), _mm_mul_ps(p01, ix));
-
-                _mm_store_ps(dst + dst_start, p00);
-            }
-        }
-    }
-    else { // Unaligned memory
-        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-            f32 src_y_f = (dst_y + 0.5f) * ratio_y;
-            i32 src_y = (i32)src_y_f;
-            f32 interp_y = src_y_f - src_y;
-
-            __m128 iy = _mm_set1_ps(interp_y);
-            __m128 iy1 = _mm_set1_ps(1.0f - interp_y);
-
-            i32 dst_offset4 = dst_width4 * dst_y;
-            i32 src_offset4 = src_width4 * src_y;
-
-            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-                f32 src_x_f = (dst_x + 0.5f) * ratio_x;
-                i32 src_x = (i32)src_x_f;
-                f32 interp_x = src_x_f - src_x;
-
-                i32 dst_start = (dst_x << 2) + dst_offset4;
-
-                f32* src_start00 = src + (src_x << 2) + src_offset4;
-
-                __m128 ix = _mm_set1_ps(interp_x);
-                __m128 ix1 = _mm_set1_ps(1.0f - interp_x);
-
-                __m128 p00 = _mm_loadu_ps(src_start00);
-                __m128 p01 = _mm_loadu_ps(src_start00 + 4);
-                __m128 p10 = _mm_loadu_ps(src_start00 + src_width4);
-                __m128 p11 = _mm_loadu_ps(src_start00 + src_width4_4);
-
-                p00 = _mm_add_ps(_mm_mul_ps(p00, iy1), _mm_mul_ps(p10, iy));
-                p01 = _mm_add_ps(_mm_mul_ps(p01, iy1), _mm_mul_ps(p11, iy));
-
-                p00 = _mm_add_ps(_mm_mul_ps(p00, ix1), _mm_mul_ps(p01, ix));
-
-                _mm_storeu_ps(dst + dst_start, p00);
-            }
-        }
-    }
-}
-
-void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)src_width / (f32)dst_width;
-    f32 ratio_y = (f32)src_height / (f32)dst_height;
-    i32 src_width4 = src_width << 2;
-    i32 dst_width4 = dst_width << 2;
-
-    if ((((size_t)src | (size_t)dst) & 0x0f) == 0) { // Aligned memory
-        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-            f32 src_lower_y_f = dst_y * ratio_y;
-            f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
-
-            i32 src_lower_y = max(0, (i32)src_lower_y_f);
-            i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
-
-            f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
-            f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
-
-            i32 dst_offset4 = dst_width4 * dst_y;
-
-            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-                f32 src_lower_x_f = dst_x * ratio_x;
-                f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
-
-                i32 src_lower_x = max(0, (i32)src_lower_x_f);
-                i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
-
-                f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
-                f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
-
-                i32 dst_start = (dst_x << 2) + dst_offset4;
-
-                __m128 res = _mm_set1_ps(0.0f);
-
-                f32 weight_total = 0.0f;
-
-                for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
-                    i32 src_offset4 = src_width4 * area_y;
-
-                    for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
-                        f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
-                            (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
-
-                        i32 src_start = (area_x << 2) + src_offset4;
-
-                        __m128 p = _mm_load_ps(src + src_start);
-
-                        res = _mm_add_ps(res, _mm_mul_ps(p, _mm_set1_ps(weight)));
-                        weight_total += weight;
-                    }
-                }
-
-                f32 div = 1.0f / weight_total;
-
-                res = _mm_mul_ps(res, _mm_set1_ps(div));
-
-                _mm_store_ps(dst + dst_start, res);
-            }
-        }
-    }
-    else { // Unaligned memory
-        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-            f32 src_lower_y_f = dst_y * ratio_y;
-            f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
-
-            i32 src_lower_y = max(0, (i32)src_lower_y_f);
-            i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
-
-            f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
-            f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
-
-            i32 dst_offset4 = dst_width4 * dst_y;
-
-            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-                f32 src_lower_x_f = dst_x * ratio_x;
-                f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
-
-                i32 src_lower_x = max(0, (i32)src_lower_x_f);
-                i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
-
-                f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
-                f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
-
-                i32 dst_start = (dst_x << 2) + dst_offset4;
-
-                __m128 res = _mm_set1_ps(0.0f);
-
-                f32 weight_total = 0.0f;
-
-                for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
-                    i32 src_offset4 = src_width4 * area_y;
-
-                    for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
-                        f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
-                            (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
-
-                        i32 src_start = (area_x << 2) + src_offset4;
-
-                        __m128 p = _mm_loadu_ps(src + src_start);
-
-                        res = _mm_add_ps(res, _mm_mul_ps(p, _mm_set1_ps(weight)));
-                        weight_total += weight;
-                    }
-                }
-
-                f32 div = 1.0f / weight_total;
-
-                res = _mm_mul_ps(res, _mm_set1_ps(div));
-
-                _mm_storeu_ps(dst + dst_start, res);
-            }
-        }
-    }
-}
-
-#elif defined(__arm__) // ARM Neon implementation
-
-void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)(src_width - 1) / (f32)dst_width;
-    f32 ratio_y = (f32)(src_height - 1) / (f32)dst_height;
-    i32 dst_width4 = dst_width << 2;
-    i32 src_width4 = src_width << 2;
-    i32 src_width4_4 = src_width4 + 4;
-
-    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-        f32 src_y_f = (dst_y + 0.5f) * ratio_y;
-        i32 src_y = (i32)src_y_f;
-        f32 interp_y = src_y_f - src_y;
-
-        float32x4_t iy = vdupq_n_f32(interp_y);
-        float32x4_t iy1 = vdupq_n_f32(1.0f - interp_y);
-
-        i32 dst_offset4 = dst_width4 * dst_y;
-        i32 src_offset4 = src_width4 * src_y;
-
-        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-            f32 src_x_f = (dst_x + 0.5f) * ratio_x;
-            i32 src_x = (i32)src_x_f;
-            f32 interp_x = src_x_f - src_x;
-
-            i32 dst_start = (dst_x << 2) + dst_offset4;
-
-            f32* src_start00 = src + (src_x << 2) + src_offset4;
-
-            float32x4_t ix = vdupq_n_f32(interp_x); // Use q versions (128 bit)
-            float32x4_t ix1 = vdupq_n_f32(1.0f - interp_x);
-
-            float32x4_t p00 = vld1q_f32(src_start00);
-            float32x4_t p01 = vld1q_f32(src_start00 + 4);
-            float32x4_t p10 = vld1q_f32(src_start00 + src_width4);
-            float32x4_t p11 = vld1q_f32(src_start00 + src_width4_4);
-
-            p00 = vaddq_f32(vmulq_f32(p00, iy1), vmulq_f32(p10, iy));
-            p01 = vaddq_f32(vmulq_f32(p01, iy1), vmulq_f32(p11, iy));
-
-            p00 = vaddq_f32(vmulq_f32(p00, ix1), vmulq_f32(p01, ix));
-
-            vst1q_f32(dst + dst_start, p00);
-        }
-    }
-}
-
-void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)src_width / (f32)dst_width;
-    f32 ratio_y = (f32)src_height / (f32)dst_height;
-    i32 src_width4 = src_width << 2;
-    i32 dst_width4 = dst_width << 2;
-
-    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-        f32 src_lower_y_f = dst_y * ratio_y;
-        f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
-
-        i32 src_lower_y = max(0, (i32)src_lower_y_f);
-        i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
-
-        f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
-        f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
-
-        i32 dst_offset4 = dst_width4 * dst_y;
-
-        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-            f32 src_lower_x_f = dst_x * ratio_x;
-            f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
-
-            i32 src_lower_x = max(0, (i32)src_lower_x_f);
-            i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
-
-            f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
-            f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
-
-            i32 dst_start = (dst_x << 2) + dst_offset4;
-
-            float32x4_t res = vdupq_n_f32(0.0f);
-
-            f32 weight_total = 0.0f;
-
-            for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
-                i32 src_offset4 = src_width4 * area_y;
-
-                for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
-                    f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
-                        (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
-
-                    i32 src_start = (area_x << 2) + src_offset4;
-
-                    float32x4_t p = vld1q_f32(src + src_start);
-
-                    res = vaddq_f32(res, vmulq_f32(p, vdupq_n_f32(weight)));
-                    weight_total += weight;
-                }
-            }
-
-            f32 div = 1.0f / weight_total;
-
-            res = vmulq_f32(res, vdupq_n_f32(div));
-
-            vst1q_f32(dst + dst_start, res);
-        }
-    }
-}
-
-#else // No SIMD implementation
-
-void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)(src_width - 1) / (f32)dst_width;
-    f32 ratio_y = (f32)(src_height - 1) / (f32)dst_height;
-    i32 dst_width4 = dst_width << 2;
-
-    i32 src_width4s[8];
-    src_width4s[0] = src_width << 2;
-    
-    for (i32 i = 1; i < 8; i++)
-        src_width4s[i] = src_width4s[0] + i;
-
-    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-        f32 src_y_f = (dst_y + 0.5f) * ratio_y;
-        i32 src_y = (i32)src_y_f;
-        f32 interp_y = src_y_f - src_y;
-        f32 interp_y1 = 1.0f - interp_y;
-
-        i32 dst_offset4 = dst_width4 * dst_y;
-        i32 src_offset4 = src_width4s[0] * src_y;
-
-        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-            f32 src_x_f = (dst_x + 0.5f) * ratio_x;
-            i32 src_x = (i32)src_x_f;
-            f32 interp_x = src_x_f - src_x;
-
-            i32 dst_start = (dst_x << 2) + dst_offset4;
-
-            i32 src_start00 = (src_x << 2) + src_offset4;
-
-            f32 interp_x1 = 1.0f - interp_x;
-
-            f32 pr0 = interp_y1 * src[src_start00    ] + interp_y * src[src_start00 + src_width4s[0]];
-            f32 pr1 = interp_y1 * src[src_start00 + 4] + interp_y * src[src_start00 + src_width4s[4]];
-
-            f32 pg0 = interp_y1 * src[src_start00 + 1] + interp_y * src[src_start00 + src_width4s[1]];
-            f32 pg1 = interp_y1 * src[src_start00 + 5] + interp_y * src[src_start00 + src_width4s[5]];
-
-            f32 pb0 = interp_y1 * src[src_start00 + 2] + interp_y * src[src_start00 + src_width4s[2]];
-            f32 pb1 = interp_y1 * src[src_start00 + 6] + interp_y * src[src_start00 + src_width4s[6]];
-
-            f32 pa0 = interp_y1 * src[src_start00 + 3] + interp_y * src[src_start00 + src_width4s[3]];
-            f32 pa1 = interp_y1 * src[src_start00 + 7] + interp_y * src[src_start00 + src_width4s[7]];
-
-            dst[dst_start    ] = interp_x1 * pr0 + interp_x * pr1;
-            dst[dst_start + 1] = interp_x1 * pg0 + interp_x * pg1;
-            dst[dst_start + 2] = interp_x1 * pb0 + interp_x * pb1;
-            dst[dst_start + 3] = interp_x1 * pa0 + interp_x * pa1;
-        }
-    }
-}
-
-void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
-    f32 ratio_x = (f32)src_width / (f32)dst_width;
-    f32 ratio_y = (f32)src_height / (f32)dst_height;
-    i32 src_width4 = src_width << 2;
-    i32 dst_width4 = dst_width << 2;
-
-    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
-        f32 src_lower_y_f = dst_y * ratio_y;
-        f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
-
-        i32 src_lower_y = max(0, (i32)src_lower_y_f);
-        i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
-
-        f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
-        f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
-
-        i32 dst_offset4 = dst_width4 * dst_y;
-
-        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
-            f32 src_lower_x_f = dst_x * ratio_x;
-            f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
-
-            i32 src_lower_x = max(0, (i32)src_lower_x_f);
-            i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
-
-            f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
-            f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
-
-            i32 dst_start = (dst_x << 2) + dst_offset4;
-
-            f32 r = 0.0f;
-            f32 g = 0.0f;
-            f32 b = 0.0f;
-            f32 a = 0.0f;
-
-            f32 weight_total = 0.0f;
-
-            for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
-                i32 src_offset4 = src_width4 * area_y;
-
-                for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
-                    f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
-                        (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
-
-                    i32 src_start = (area_x << 2) + src_offset4;
-
-                    r += weight * src[src_start    ];
-                    g += weight * src[src_start + 1];
-                    b += weight * src[src_start + 2];
-                    a += weight * src[src_start + 3];
-                    weight_total += weight;
-                }
-            }
-
-            f32 div = 1.0f / weight_total;
-
-            dst[dst_start    ] = r * div;
-            dst[dst_start + 1] = g * div;
-            dst[dst_start + 2] = b * div;
-            dst[dst_start + 3] = a * div;
-        }
-    }
-}
-
-#endif
+#include "scaler.h"
+
+// Nearest does not use SIMD
+void scale_nearest_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)src_width / (f32)dst_width;
+    f32 ratio_y = (f32)src_height / (f32)dst_height;
+    i32 dst_width4 = dst_width << 2;
+    i32 src_width4 = src_width << 2;
+
+    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+        i32 src_y = (i32)((dst_y + 0.5f) * ratio_y);
+
+        i32 dst_offset4 = dst_width4 * dst_y;
+        i32 src_offset4 = src_width4 * src_y;
+
+        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+            i32 src_x = (i32)((dst_x + 0.5f) * ratio_x);
+
+            memcpy(&dst[(dst_x << 2) + dst_offset4], &src[(src_x << 2) + src_offset4], RGBA32F_SIZE);
+        }
+    }
+}
+
+#if defined(__x86_64__) // SSE implementation
+
+void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)(src_width - 1) / (f32)dst_width;
+    f32 ratio_y = (f32)(src_height - 1) / (f32)dst_height;
+    i32 dst_width4 = dst_width << 2;
+    i32 src_width4 = src_width << 2;
+    i32 src_width4_4 = src_width4 + 4;
+
+    if ((((size_t)src | (size_t)dst) & 0x0f) == 0) { // Aligned memory
+        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+            f32 src_y_f = (dst_y + 0.5f) * ratio_y;
+            i32 src_y = (i32)src_y_f;
+            f32 interp_y = src_y_f - src_y;
+
+            __m128 iy = _mm_set1_ps(interp_y);
+            __m128 iy1 = _mm_set1_ps(1.0f - interp_y);
+
+            i32 dst_offset4 = dst_width4 * dst_y;
+            i32 src_offset4 = src_width4 * src_y;
+
+            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+                f32 src_x_f = (dst_x + 0.5f) * ratio_x;
+                i32 src_x = (i32)src_x_f;
+                f32 interp_x = src_x_f - src_x;
+
+                i32 dst_start = (dst_x << 2) + dst_offset4;
+
+                f32* src_start00 = src + (src_x << 2) + src_offset4;
+
+                __m128 ix = _mm_set1_ps(interp_x);
+                __m128 ix1 = _mm_set1_ps(1.0f - interp_x);
+
+                __m128 p00 = _mm_load_ps(src_start00);
+                __m128 p01 = _mm_load_ps(src_start00 + 4);
+                __m128 p10 = _mm_load_ps(src_start00 + src_width4);
+                __m128 p11 = _mm_load_ps(src_start00 + src_width4_4);
+
+                p00 = _mm_add_ps(_mm_mul_ps(p00, iy1), _mm_mul_ps(p10, iy));
+                p01 = _mm_add_ps(_mm_mul_ps(p01, iy1), _mm_mul_ps(p11, iy));
+
+                p00 = _mm_add_ps(_mm_mul_ps(p00, ix1), _mm_mul_ps(p01, ix));
+
+                _mm_store_ps(dst + dst_start, p00);
+            }
+        }
+    }
+    else { // Unaligned memory
+        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+            f32 src_y_f = (dst_y + 0.5f) * ratio_y;
+            i32 src_y = (i32)src_y_f;
+            f32 interp_y = src_y_f - src_y;
+
+            __m128 iy = _mm_set1_ps(interp_y);
+            __m128 iy1 = _mm_set1_ps(1.0f - interp_y);
+
+            i32 dst_offset4 = dst_width4 * dst_y;
+            i32 src_offset4 = src_width4 * src_y;
+
+            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+                f32 src_x_f = (dst_x + 0.5f) * ratio_x;
+                i32 src_x = (i32)src_x_f;
+                f32 interp_x = src_x_f - src_x;
+
+                i32 dst_start = (dst_x << 2) + dst_offset4;
+
+                f32* src_start00 = src + (src_x << 2) + src_offset4;
+
+                __m128 ix = _mm_set1_ps(interp_x);
+                __m128 ix1 = _mm_set1_ps(1.0f - interp_x);
+
+                __m128 p00 = _mm_loadu_ps(src_start00);
+                __m128 p01 = _mm_loadu_ps(src_start00 + 4);
+                __m128 p10 = _mm_loadu_ps(src_start00 + src_width4);
+                __m128 p11 = _mm_loadu_ps(src_start00 + src_width4_4);
+
+                p00 = _mm_add_ps(_mm_mul_ps(p00, iy1), _mm_mul_ps(p10, iy));
+                p01 = _mm_add_ps(_mm_mul_ps(p01, iy1), _mm_mul_ps(p11, iy));
+
+                p00 = _mm_add_ps(_mm_mul_ps(p00, ix1), _mm_mul_ps(p01, ix));
+
+                _mm_storeu_ps(dst + dst_start, p00);
+            }
+        }
+    }
+}
+
+void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)src_width / (f32)dst_width;
+    f32 ratio_y = (f32)src_height / (f32)dst_height;
+    i32 src_width4 = src_width << 2;
+    i32 dst_width4 = dst_width << 2;
+
+    if ((((size_t)src | (size_t)dst) & 0x0f) == 0) { // Aligned memory
+        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+            f32 src_lower_y_f = dst_y * ratio_y;
+            f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
+
+            i32 src_lower_y = max(0, (i32)src_lower_y_f);
+            i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
+
+            f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
+            f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
+
+            i32 dst_offset4 = dst_width4 * dst_y;
+
+            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+                f32 src_lower_x_f = dst_x * ratio_x;
+                f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
+
+                i32 src_lower_x = max(0, (i32)src_lower_x_f);
+                i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
+
+                f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
+                f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
+
+                i32 dst_start = (dst_x << 2) + dst_offset4;
+
+                __m128 res = _mm_set1_ps(0.0f);
+
+                f32 weight_total = 0.0f;
+
+                for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
+                    i32 src_offset4 = src_width4 * area_y;
+
+                    for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
+                        f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
+                            (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
+
+                        i32 src_start = (area_x << 2) + src_offset4;
+
+                        __m128 p = _mm_load_ps(src + src_start);
+
+                        res = _mm_add_ps(res, _mm_mul_ps(p, _mm_set1_ps(weight)));
+                        weight_total += weight;
+                    }
+                }
+
+                f32 div = 1.0f / weight_total;
+
+                res = _mm_mul_ps(res, _mm_set1_ps(div));
+
+                _mm_store_ps(dst + dst_start, res);
+            }
+        }
+    }
+    else { // Unaligned memory
+        for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+            f32 src_lower_y_f = dst_y * ratio_y;
+            f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
+
+            i32 src_lower_y = max(0, (i32)src_lower_y_f);
+            i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
+
+            f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
+            f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
+
+            i32 dst_offset4 = dst_width4 * dst_y;
+
+            for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+                f32 src_lower_x_f = dst_x * ratio_x;
+                f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
+
+                i32 src_lower_x = max(0, (i32)src_lower_x_f);
+                i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
+
+                f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
+                f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
+
+                i32 dst_start = (dst_x << 2) + dst_offset4;
+
+                __m128 res = _mm_set1_ps(0.0f);
+
+                f32 weight_total = 0.0f;
+
+                for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
+                    i32 src_offset4 = src_width4 * area_y;
+
+                    for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
+                        f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
+                            (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
+
+                        i32 src_start = (area_x << 2) + src_offset4;
+
+                        __m128 p = _mm_loadu_ps(src + src_start);
+
+                        res = _mm_add_ps(res, _mm_mul_ps(p, _mm_set1_ps(weight)));
+                        weight_total += weight;
+                    }
+                }
+
+                f32 div = 1.0f / weight_total;
+
+                res = _mm_mul_ps(res, _mm_set1_ps(div));
+
+                _mm_storeu_ps(dst + dst_start, res);
+            }
+        }
+    }
+}
+
+#elif defined(__arm__) // ARM Neon implementation
+
+void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)(src_width - 1) / (f32)dst_width;
+    f32 ratio_y = (f32)(src_height - 1) / (f32)dst_height;
+    i32 dst_width4 = dst_width << 2;
+    i32 src_width4 = src_width << 2;
+    i32 src_width4_4 = src_width4 + 4;
+
+    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+        f32 src_y_f = (dst_y + 0.5f) * ratio_y;
+        i32 src_y = (i32)src_y_f;
+        f32 interp_y = src_y_f - src_y;
+
+        float32x4_t iy = vdupq_n_f32(interp_y);
+        float32x4_t iy1 = vdupq_n_f32(1.0f - interp_y);
+
+        i32 dst_offset4 = dst_width4 * dst_y;
+        i32 src_offset4 = src_width4 * src_y;
+
+        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+            f32 src_x_f = (dst_x + 0.5f) * ratio_x;
+            i32 src_x = (i32)src_x_f;
+            f32 interp_x = src_x_f - src_x;
+
+            i32 dst_start = (dst_x << 2) + dst_offset4;
+
+            f32* src_start00 = src + (src_x << 2) + src_offset4;
+
+            float32x4_t ix = vdupq_n_f32(interp_x); // Use q versions (128 bit)
+            float32x4_t ix1 = vdupq_n_f32(1.0f - interp_x);
+
+            float32x4_t p00 = vld1q_f32(src_start00);
+            float32x4_t p01 = vld1q_f32(src_start00 + 4);
+            float32x4_t p10 = vld1q_f32(src_start00 + src_width4);
+            float32x4_t p11 = vld1q_f32(src_start00 + src_width4_4);
+
+            p00 = vaddq_f32(vmulq_f32(p00, iy1), vmulq_f32(p10, iy));
+            p01 = vaddq_f32(vmulq_f32(p01, iy1), vmulq_f32(p11, iy));
+
+            p00 = vaddq_f32(vmulq_f32(p00, ix1), vmulq_f32(p01, ix));
+
+            vst1q_f32(dst + dst_start, p00);
+        }
+    }
+}
+
+void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)src_width / (f32)dst_width;
+    f32 ratio_y = (f32)src_height / (f32)dst_height;
+    i32 src_width4 = src_width << 2;
+    i32 dst_width4 = dst_width << 2;
+
+    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+        f32 src_lower_y_f = dst_y * ratio_y;
+        f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
+
+        i32 src_lower_y = max(0, (i32)src_lower_y_f);
+        i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
+
+        f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
+        f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
+
+        i32 dst_offset4 = dst_width4 * dst_y;
+
+        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+            f32 src_lower_x_f = dst_x * ratio_x;
+            f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
+
+            i32 src_lower_x = max(0, (i32)src_lower_x_f);
+            i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
+
+            f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
+            f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
+
+            i32 dst_start = (dst_x << 2) + dst_offset4;
+
+            float32x4_t res = vdupq_n_f32(0.0f);
+
+            f32 weight_total = 0.0f;
+
+            for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
+                i32 src_offset4 = src_width4 * area_y;
+
+                for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
+                    f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
+                        (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
+
+                    i32 src_start = (area_x << 2) + src_offset4;
+
+                    float32x4_t p = vld1q_f32(src + src_start);
+
+                    res = vaddq_f32(res, vmulq_f32(p, vdupq_n_f32(weight)));
+                    weight_total += weight;
+                }
+            }
+
+            f32 div = 1.0f / weight_total;
+
+            res = vmulq_f32(res, vdupq_n_f32(div));
+
+            vst1q_f32(dst + dst_start, res);
+        }
+    }
+}
+
+#else // No SIMD implementation
+
+void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)(src_width - 1) / (f32)dst_width;
+    f32 ratio_y = (f32)(src_height - 1) / (f32)dst_height;
+    i32 dst_width4 = dst_width << 2;
+
+    i32 src_width4s[8];
+    src_width4s[0] = src_width << 2;
+    
+    for (i32 i = 1; i < 8; i++)
+        src_width4s[i] = src_width4s[0] + i;
+
+    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+        f32 src_y_f = (dst_y + 0.5f) * ratio_y;
+        i32 src_y = (i32)src_y_f;
+        f32 interp_y = src_y_f - src_y;
+        f32 interp_y1 = 1.0f - interp_y;
+
+        i32 dst_offset4 = dst_width4 * dst_y;
+        i32 src_offset4 = src_width4s[0] * src_y;
+
+        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+            f32 src_x_f = (dst_x + 0.5f) * ratio_x;
+            i32 src_x = (i32)src_x_f;
+            f32 interp_x = src_x_f - src_x;
+
+            i32 dst_start = (dst_x << 2) + dst_offset4;
+
+            i32 src_start00 = (src_x << 2) + src_offset4;
+
+            f32 interp_x1 = 1.0f - interp_x;
+
+            f32 pr0 = interp_y1 * src[src_start00    ] + interp_y * src[src_start00 + src_width4s[0]];
+            f32 pr1 = interp_y1 * src[src_start00 + 4] + interp_y * src[src_start00 + src_width4s[4]];
+
+            f32 pg0 = interp_y1 * src[src_start00 + 1] + interp_y * src[src_start00 + src_width4s[1]];
+            f32 pg1 = interp_y1 * src[src_start00 + 5] + interp_y * src[src_start00 + src_width4s[5]];
+
+            f32 pb0 = interp_y1 * src[src_start00 + 2] + interp_y * src[src_start00 + src_width4s[2]];
+            f32 pb1 = interp_y1 * src[src_start00 + 6] + interp_y * src[src_start00 + src_width4s[6]];
+
+            f32 pa0 = interp_y1 * src[src_start00 + 3] + interp_y * src[src_start00 + src_width4s[3]];
+            f32 pa1 = interp_y1 * src[src_start00 + 7] + interp_y * src[src_start00 + src_width4s[7]];
+
+            dst[dst_start    ] = interp_x1 * pr0 + interp_x * pr1;
+            dst[dst_start + 1] = interp_x1 * pg0 + interp_x * pg1;
+            dst[dst_start + 2] = interp_x1 * pb0 + interp_x * pb1;
+            dst[dst_start + 3] = interp_x1 * pa0 + interp_x * pa1;
+        }
+    }
+}
+
+void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height) {
+    f32 ratio_x = (f32)src_width / (f32)dst_width;
+    f32 ratio_y = (f32)src_height / (f32)dst_height;
+    i32 src_width4 = src_width << 2;
+    i32 dst_width4 = dst_width << 2;
+
+    for (i32 dst_y = 0; dst_y < dst_height; dst_y++) {
+        f32 src_lower_y_f = dst_y * ratio_y;
+        f32 src_upper_y_f = (dst_y + 1.0f) * ratio_y;
+
+        i32 src_lower_y = max(0, (i32)src_lower_y_f);
+        i32 src_upper_y = min(src_height, (i32)src_upper_y_f + 1);
+
+        f32 over_height = src_lower_y_f - (i32)src_lower_y_f;
+        f32 over_height1 = 1.0f - (src_upper_y_f - (i32)src_lower_y_f);
+
+        i32 dst_offset4 = dst_width4 * dst_y;
+
+        for (i32 dst_x = 0; dst_x < dst_width; dst_x++) {
+            f32 src_lower_x_f = dst_x * ratio_x;
+            f32 src_upper_x_f = (dst_x + 1.0f) * ratio_x;
+
+            i32 src_lower_x = max(0, (i32)src_lower_x_f);
+            i32 src_upper_x = min(src_width, (i32)src_upper_x_f + 1);
+
+            f32 over_width = src_lower_x_f - (i32)src_lower_x_f;
+            f32 over_width1 = 1.0f - (src_upper_x_f - (i32)src_lower_x_f);
+
+            i32 dst_start = (dst_x << 2) + dst_offset4;
+
+            f32 r = 0.0f;
+            f32 g = 0.0f;
+            f32 b = 0.0f;
+            f32 a = 0.0f;
+
+            f32 weight_total = 0.0f;
+
+            for (i32 area_y = src_lower_y; area_y < src_upper_y; area_y++) {
+                i32 src_offset4 = src_width4 * area_y;
+
+                for (i32 area_x = src_lower_x; area_x < src_upper_x; area_x++) {
+                    f32 weight = (1.0f - (area_y == src_lower_y) * over_height) * (1.0f - (area_x == src_lower_x) * over_width) +
+                        (1.0f - (area_y == src_upper_y) * over_height1) * (1.0f - (area_x == src_upper_x) * over_width1);
+
+                    i32 src_start = (area_x << 2) + src_offset4;
+
+                    r += weight * src[src_start    ];
+                    g += weight * src[src_start + 1];
+                    b += weight * src[src_start + 2];
+                    a += weight * src[src_start + 3];
+                    weight_total += weight;
+                }
+            }
+
+            f32 div = 1.0f / weight_total;
+
+            dst[dst_start    ] = r * div;
+            dst[dst_start + 1] = g * div;
+            dst[dst_start + 2] = b * div;
+            dst[dst_start + 3] = a * div;
+        }
+    }
+}
+
+#endif
```

### Comparing `tinyscaler-1.2.5/src/scaler.h` & `tinyscaler-1.2.6/src/scaler.h`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#pragma once
-
-#include <stdlib.h>
-#include <math.h>
-#include <memory.h>
-
-#if defined(__x86_64__)
-#include <pmmintrin.h> // SSE
-#elif defined(__arm__)
-#include <arm_neon.h> // Neon
-#endif
-
-#define RGBA32F_SIZE 16 // Byte size of a pixel
-
-#ifndef max
-#define max(a,b) (((a) > (b)) ? (a) : (b))
-#define min(a,b) (((a) < (b)) ? (a) : (b))
-#endif
-
-typedef unsigned char u8;
-typedef int i32;
-typedef float f32;
-typedef double f64;
-
-// Scalers
-void scale_nearest_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height);
-void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height);
-void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height);
+#pragma once
+
+#include <stdlib.h>
+#include <math.h>
+#include <memory.h>
+
+#if defined(__x86_64__)
+#include <pmmintrin.h> // SSE
+#elif defined(__arm__)
+#include <arm_neon.h> // Neon
+#endif
+
+#define RGBA32F_SIZE 16 // Byte size of a pixel
+
+#ifndef max
+#define max(a,b) (((a) > (b)) ? (a) : (b))
+#define min(a,b) (((a) < (b)) ? (a) : (b))
+#endif
+
+typedef unsigned char u8;
+typedef int i32;
+typedef float f32;
+typedef double f64;
+
+// Scalers
+void scale_nearest_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height);
+void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height);
+void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height);
```

### Comparing `tinyscaler-1.2.5/src/tinyscaler.c` & `tinyscaler-1.2.6/src/tinyscaler.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 /* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "src/scaler.c",
-            "src/scaler.h"
+            "src\\scaler.c",
+            "src\\scaler.h"
         ],
         "include_dirs": [
             "src"
         ],
         "name": "tinyscaler",
         "sources": [
-            "src/tinyscaler.pyx"
+            "src\\tinyscaler.pyx"
         ]
     },
     "module_name": "tinyscaler"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -972,15 +972,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "src/tinyscaler.pyx",
+  "src\\tinyscaler.pyx",
   "stringsource",
 };
 /* MemviewSliceStruct.proto */
 struct __pyx_memoryview_obj;
 typedef struct {
   struct __pyx_memoryview_obj *memview;
   char *data;
@@ -2088,15 +2088,15 @@
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_ascontiguousarray[] = "ascontiguousarray";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_Incorrect_dst_size[] = "Incorrect dst size!";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_src_tinyscaler_pyx[] = "src/tinyscaler.pyx";
+static const char __pyx_k_src_tinyscaler_pyx[] = "src\\tinyscaler.pyx";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
```

### Comparing `tinyscaler-1.2.5/src/tinyscaler.egg-info/PKG-INFO` & `tinyscaler-1.2.6/src/tinyscaler.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-Metadata-Version: 2.1
-Name: tinyscaler
-Version: 1.2.5
-Summary: A tiny, simple image scaler.
-Author-email: Farama Foundation <contact@farama.org>
-License: MIT License
-Project-URL: Homepage, https://farama.org
-Project-URL: Repository, https://github.com/Farama-Foundation/TinyScaler
-Project-URL: Documentation, https://github.com/Farama-Foundation/TinyScaler
-Project-URL: Bug Report, https://github.com/Farama-Foundation/TinyScaler/issues
-Keywords: Reinforcement Learning,Gymnasium,PettingZoo
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.12,>=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-    <img src="https://raw.githubusercontent.com/Farama-Foundation/TinyScaler/main/tinyscaler-text.png" width="500px"/>
-</p>
-
-A small CPU image scaling library with SIMD support on x86_64 and Arm (Neon). This project is aimed to replace OpenCV for image resizing, resolving installation inconveniences and compatibility issues. We developed this for future use in Gymnasium and PettingZoo wrappers.
-
-## Installation
-You can install from PyPI using `pip install tinyscaler`. Linux and macOS with Python 3.7, 3.8, 3.9, 3.10 and 3.11 are supported.
-
-## Usage
-Tinyscaler contains a single external function, `scale` that using a numpy array input for the image and the new resized shape, returns the resized image. 
-
-```python
-import numpy as np
-import tinyscaler
-
-img = np.random.rand(64, 64, 4).astype(np.float32)
-
-resize_img = tinyscaler.scale(img, (32, 32))
-print(resize_img.shape, resize_img.dtype)  # (32, 32) np.float32
-```
-
-TinyScaler supports mode='area', mode='bilinear', and mode='nearest' filtering. It also allows one to pass a destination buffer in order to avoid duplicate memory allocations.
-
-Area filtering is only really useful for downscaling, bilinear will be used even when area filtering is set if upscaling. Area filtering is also likely not worth it when downscaling less than or equal to 2x.
-
-TinyScaler is used through a single function. The full signature is:
-
-```python
-scale(src : np.ndarray, size : tuple, mode='area', dst : np.ndarray = None)
-```
-
-Note that the `size` tuple parameter is (width, height). However, the numpy arrays have dimensions ordered as (height, width, channels). This is similar to OpenCV.
-
-TinyScaler expects a contiguous numpy array. If it is not contiguous, it will throw an error. You can make a non-contiguous numpy array contiguous by calling `np.ascontiguousarray`. Usually a numpy array will already be contiguous.
-
-If the final array dimension is not 4 (RGBA), it will automatically convert to it. Further, if the array is uint8, it will be converted to float32. So the prefered array has a shape `(height, width, 4)` and `dtype=np.float32`.
-
-Finally, downscaling is the focus of TinyScaler. It can also upscale, but it will not be as fast as a more complex separable algorithm in that case.
-
-## Performance
-In a [simple benchmark](./examples/benchmark.py), we resized the same image (4928x3279) down to (852x567) 100 times using bilinear filtering with several libraries. Here are the times (in seconds) spent (measured with Python's perf_counter) on a AMD 1950x:
-
-```
-Time elapsed for tinyscaler: 0.7968465110002398
-Time elapsed for OpenCV: 0.48667862100001
-Time elapsed for Pillow: 12.672875003999707
-Time elapsed for skimage: 164.45401711399973
-```
-
-And with area filtering (just TinyScaler and OpenCV):
-
-```
-Time elapsed for tinyscaler: 4.34793155800071
-Time elapsed for OpenCV: 8.118138265999733
-```
-
-All methods were forced to use a single thread. OpenCV is slightly faster than TinyScaler for bilinear filtering, but TinyScaler remains very fast regardless.
-
-Interestingly, for area filtering, TinyScaler is faster (almost 2x).
-
+Metadata-Version: 2.1
+Name: tinyscaler
+Version: 1.2.6
+Summary: A tiny, simple image scaler.
+Author-email: Farama Foundation <contact@farama.org>
+License: MIT License
+Project-URL: Homepage, https://farama.org
+Project-URL: Repository, https://github.com/Farama-Foundation/TinyScaler
+Project-URL: Documentation, https://github.com/Farama-Foundation/TinyScaler
+Project-URL: Bug Report, https://github.com/Farama-Foundation/TinyScaler/issues
+Keywords: Reinforcement Learning,Gymnasium,PettingZoo
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: <3.12,>=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/Farama-Foundation/TinyScaler/main/tinyscaler-text.png" width="500px"/>
+</p>
+
+A small CPU image scaling library with SIMD support on x86_64 and Arm (Neon). This project is aimed to replace OpenCV for image resizing, resolving installation inconveniences and compatibility issues. We developed this for future use in Gymnasium and PettingZoo wrappers.
+
+## Installation
+You can install from PyPI using `pip install tinyscaler`. Linux and macOS with Python 3.7, 3.8, 3.9, 3.10 and 3.11 are supported.
+
+## Usage
+Tinyscaler contains a single external function, `scale` that using a numpy array input for the image and the new resized shape, returns the resized image. 
+
+```python
+import numpy as np
+import tinyscaler
+
+img = np.random.rand(64, 64, 4).astype(np.float32)
+
+resize_img = tinyscaler.scale(img, (32, 32))
+print(resize_img.shape, resize_img.dtype)  # (32, 32) np.float32
+```
+
+TinyScaler supports mode='area', mode='bilinear', and mode='nearest' filtering. It also allows one to pass a destination buffer in order to avoid duplicate memory allocations.
+
+Area filtering is only really useful for downscaling, bilinear will be used even when area filtering is set if upscaling. Area filtering is also likely not worth it when downscaling less than or equal to 2x.
+
+TinyScaler is used through a single function. The full signature is:
+
+```python
+scale(src : np.ndarray, size : tuple, mode='area', dst : np.ndarray = None)
+```
+
+Note that the `size` tuple parameter is (width, height). However, the numpy arrays have dimensions ordered as (height, width, channels). This is similar to OpenCV.
+
+TinyScaler expects a contiguous numpy array. If it is not contiguous, it will throw an error. You can make a non-contiguous numpy array contiguous by calling `np.ascontiguousarray`. Usually a numpy array will already be contiguous.
+
+If the final array dimension is not 4 (RGBA), it will automatically convert to it. Further, if the array is uint8, it will be converted to float32. So the prefered array has a shape `(height, width, 4)` and `dtype=np.float32`.
+
+Finally, downscaling is the focus of TinyScaler. It can also upscale, but it will not be as fast as a more complex separable algorithm in that case.
+
+## Performance
+In a [simple benchmark](./examples/benchmark.py), we resized the same image (4928x3279) down to (852x567) 100 times using bilinear filtering with several libraries. Here are the times (in seconds) spent (measured with Python's perf_counter) on a AMD 1950x:
+
+```
+Time elapsed for tinyscaler: 0.7968465110002398
+Time elapsed for OpenCV: 0.48667862100001
+Time elapsed for Pillow: 12.672875003999707
+Time elapsed for skimage: 164.45401711399973
+```
+
+And with area filtering (just TinyScaler and OpenCV):
+
+```
+Time elapsed for tinyscaler: 4.34793155800071
+Time elapsed for OpenCV: 8.118138265999733
+```
+
+All methods were forced to use a single thread. OpenCV is slightly faster than TinyScaler for bilinear filtering, but TinyScaler remains very fast regardless.
+
+Interestingly, for area filtering, TinyScaler is faster (almost 2x).
+
```

### Comparing `tinyscaler-1.2.5/src/tinyscaler.pyx` & `tinyscaler-1.2.6/src/tinyscaler.pyx`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import cython
-
-
-cdef extern from "scaler.c":
-    pass
-
-cdef extern from "scaler.h":
-    ctypedef unsigned char u8;
-    ctypedef int i32;
-    ctypedef float f32;
-    ctypedef double f64;
-
-    void scale_nearest_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height)
-    void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height)
-    void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height)
-
-import numpy as np
-
-auto_convert = True # Global controlling whether automatic channel/type conversions take place
-
-def _scale_4f32(src: np.ndarray, size: tuple, mode: str = 'area', dst: np.ndarray = None) -> np.ndarray:
-    assert(len(src.shape) == 3 and src.shape[2] == 4) # Must be 4 channel
-
-    if not src.flags['C_CONTIGUOUS']:
-        src = np.ascontiguousarray(src)
-
-    cdef float[:, :, ::1] src_memview = src
-
-    if dst is None:
-        dst = np.empty((size[1], size[0], 4), dtype=np.float32)
-    else:
-        if len(dst.shape) != 3 or dst.shape[0] != size[1] or dst.shape[1] != size[0] or dst.shape[2] != 4:
-            raise Exception('Incorrect dst size!')
-        elif dst.dtype != np.float32:
-            raise Exception('Incorrect dst type (must be float32)!')
-
-    if not dst.flags['C_CONTIGUOUS']:
-        dst = np.ascontiguousarray(dst)
-
-    cdef float[:, :, ::1] dst_memview = dst
-
-    if mode == 'bilinear':
-        scale_bilinear_4f32(&src_memview[0][0][0], &dst_memview[0][0][0], src.shape[1], src.shape[0], size[0], size[1])
-    elif mode == 'area':
-        scale_area_4f32(&src_memview[0][0][0], &dst_memview[0][0][0], src.shape[1], src.shape[0], size[0], size[1])
-    else:
-        scale_nearest_4f32(&src_memview[0][0][0], &dst_memview[0][0][0], src.shape[1], src.shape[0], size[0], size[1])
-
-    return dst.reshape((size[1], size[0], 4))
-
-@cython.binding(True)
-def scale(src: np.ndarray, size: tuple, mode: str = 'area', dst: np.ndarray = None) -> np.ndarray:
-    '''
-    scale (resize) a source image to a specified size
-
-    Parameters
-    ----------
-    src : numpy.ndarray
-        the source array, must have len(src.shape) == 2 or len(src.shape) == 3. Must be contiguous (using numpy.ascontiguousarray if not already).
-        Ideally (most efficient) the shape is (width, height, 4) with dtype=numpy.float32 (others will cause a conversion to occur)
-    size :
-        target size, a tuple of two positive integers (width, height)
-    mode : {'area', 'bilinear', 'nearest'}, optional
-        interpolation method to use. Defaults to area, can also be bilinear or nearest
-    dst : {None}, optional
-        destination buffer to put resized image in. Leaving this = None will result in an allocation.
-        For efficient code, set dst to a buffer of shape (size[0], size[1], 4) with dtype=numpy.float32
-
-    Returns
-    -------
-    numpy.ndarray
-        the scaled image
-
-    Raises
-    ------
-    Exception
-        when src is not contiguous or the wrong shape
-    '''
-
-    if not src.data.contiguous:
-        raise Exception('Input image must be contiguous! Use np.ascontiguousarray(image) maybe?')
-
-    src_dims = len(src.shape)
-    src_channels = 4
-    src_type = src.dtype
-
-    if mode == 'area' and (src.shape[1] < size[0] or src.shape[0] < size[1]):
-        mode = 'bilinear' # Switch to bilinear if upscaling with area filter, as area filter only applies to downscaling
-
-    # Automatic conversion
-    if auto_convert:
-        if len(src.shape) != 2 and len(src.shape) != 3:
-            raise Exception('Incorrect number of dimensions - need 2 or 3, received ' + str(len(src.shape)))
-
-        if src.dtype != np.float32:
-            if src.dtype == np.uint8:
-                src = src.astype(np.float32)
-
-                src *= float(1.0 / 255.0)
-            else:
-                src = src.astype(np.float32)
-
-        if len(src.shape) == 2 or src.shape[2] == 1: # Gray
-            if len(src.shape) == 3:
-                src = src.reshape((src.shape[0], src.shape[1]))
-
-            src_channels = 1
-
-            src_new = np.empty((src.shape[0], src.shape[1], 4), dtype=np.float32)
-            src_new[:, :, 0] = src
-            src_new[:, :, 1] = src
-            src_new[:, :, 2] = src
-            src_new[:, :, 3] = src
-
-            src = src_new
-        elif src.shape[2] == 3: # RGB
-            src_channels = 3
-
-            src_new = np.empty((src.shape[0], src.shape[1], 4), dtype=np.float32)
-            src_new[:, :, :3] = src
-            src_new[:, :, 3] = np.ones((src.shape[0], src.shape[1]))
-
-            src = src_new
-        elif src.shape[2] != 4:
-            raise Exception('Passed an invalid number of channels, must be 1, 3, or 4 (received ' + str(src.shape[2]) + ')!')
-        
-    result = None
-
-    try:
-        result = _scale_4f32(src, size, mode, dst)
-    except Exception as e:
-        raise e
-
-    # Covert back
-    if auto_convert:
-        if src_type == np.uint8:
-            result = (result * float(255.0)).astype(np.uint8)[:, :, :src_channels]
-        else:
-            result = result[:, :, :src_channels].astype(src_type)
-
-        if src_dims == 2:
-            result = result.reshape((size[1], size[0]))
-
-    return result
+import cython
+
+
+cdef extern from "scaler.c":
+    pass
+
+cdef extern from "scaler.h":
+    ctypedef unsigned char u8;
+    ctypedef int i32;
+    ctypedef float f32;
+    ctypedef double f64;
+
+    void scale_nearest_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height)
+    void scale_bilinear_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height)
+    void scale_area_4f32(f32 src[], f32 dst[], i32 src_width, i32 src_height, i32 dst_width, i32 dst_height)
+
+import numpy as np
+
+auto_convert = True # Global controlling whether automatic channel/type conversions take place
+
+def _scale_4f32(src: np.ndarray, size: tuple, mode: str = 'area', dst: np.ndarray = None) -> np.ndarray:
+    assert(len(src.shape) == 3 and src.shape[2] == 4) # Must be 4 channel
+
+    if not src.flags['C_CONTIGUOUS']:
+        src = np.ascontiguousarray(src)
+
+    cdef float[:, :, ::1] src_memview = src
+
+    if dst is None:
+        dst = np.empty((size[1], size[0], 4), dtype=np.float32)
+    else:
+        if len(dst.shape) != 3 or dst.shape[0] != size[1] or dst.shape[1] != size[0] or dst.shape[2] != 4:
+            raise Exception('Incorrect dst size!')
+        elif dst.dtype != np.float32:
+            raise Exception('Incorrect dst type (must be float32)!')
+
+    if not dst.flags['C_CONTIGUOUS']:
+        dst = np.ascontiguousarray(dst)
+
+    cdef float[:, :, ::1] dst_memview = dst
+
+    if mode == 'bilinear':
+        scale_bilinear_4f32(&src_memview[0][0][0], &dst_memview[0][0][0], src.shape[1], src.shape[0], size[0], size[1])
+    elif mode == 'area':
+        scale_area_4f32(&src_memview[0][0][0], &dst_memview[0][0][0], src.shape[1], src.shape[0], size[0], size[1])
+    else:
+        scale_nearest_4f32(&src_memview[0][0][0], &dst_memview[0][0][0], src.shape[1], src.shape[0], size[0], size[1])
+
+    return dst.reshape((size[1], size[0], 4))
+
+@cython.binding(True)
+def scale(src: np.ndarray, size: tuple, mode: str = 'area', dst: np.ndarray = None) -> np.ndarray:
+    '''
+    scale (resize) a source image to a specified size
+
+    Parameters
+    ----------
+    src : numpy.ndarray
+        the source array, must have len(src.shape) == 2 or len(src.shape) == 3. Must be contiguous (using numpy.ascontiguousarray if not already).
+        Ideally (most efficient) the shape is (width, height, 4) with dtype=numpy.float32 (others will cause a conversion to occur)
+    size :
+        target size, a tuple of two positive integers (width, height)
+    mode : {'area', 'bilinear', 'nearest'}, optional
+        interpolation method to use. Defaults to area, can also be bilinear or nearest
+    dst : {None}, optional
+        destination buffer to put resized image in. Leaving this = None will result in an allocation.
+        For efficient code, set dst to a buffer of shape (size[0], size[1], 4) with dtype=numpy.float32
+
+    Returns
+    -------
+    numpy.ndarray
+        the scaled image
+
+    Raises
+    ------
+    Exception
+        when src is not contiguous or the wrong shape
+    '''
+
+    if not src.data.contiguous:
+        raise Exception('Input image must be contiguous! Use np.ascontiguousarray(image) maybe?')
+
+    src_dims = len(src.shape)
+    src_channels = 4
+    src_type = src.dtype
+
+    if mode == 'area' and (src.shape[1] < size[0] or src.shape[0] < size[1]):
+        mode = 'bilinear' # Switch to bilinear if upscaling with area filter, as area filter only applies to downscaling
+
+    # Automatic conversion
+    if auto_convert:
+        if len(src.shape) != 2 and len(src.shape) != 3:
+            raise Exception('Incorrect number of dimensions - need 2 or 3, received ' + str(len(src.shape)))
+
+        if src.dtype != np.float32:
+            if src.dtype == np.uint8:
+                src = src.astype(np.float32)
+
+                src *= float(1.0 / 255.0)
+            else:
+                src = src.astype(np.float32)
+
+        if len(src.shape) == 2 or src.shape[2] == 1: # Gray
+            if len(src.shape) == 3:
+                src = src.reshape((src.shape[0], src.shape[1]))
+
+            src_channels = 1
+
+            src_new = np.empty((src.shape[0], src.shape[1], 4), dtype=np.float32)
+            src_new[:, :, 0] = src
+            src_new[:, :, 1] = src
+            src_new[:, :, 2] = src
+            src_new[:, :, 3] = src
+
+            src = src_new
+        elif src.shape[2] == 3: # RGB
+            src_channels = 3
+
+            src_new = np.empty((src.shape[0], src.shape[1], 4), dtype=np.float32)
+            src_new[:, :, :3] = src
+            src_new[:, :, 3] = np.ones((src.shape[0], src.shape[1]))
+
+            src = src_new
+        elif src.shape[2] != 4:
+            raise Exception('Passed an invalid number of channels, must be 1, 3, or 4 (received ' + str(src.shape[2]) + ')!')
+        
+    result = None
+
+    try:
+        result = _scale_4f32(src, size, mode, dst)
+    except Exception as e:
+        raise e
+
+    # Covert back
+    if auto_convert:
+        if src_type == np.uint8:
+            result = (result * float(255.0)).astype(np.uint8)[:, :, :src_channels]
+        else:
+            result = result[:, :, :src_channels].astype(src_type)
+
+        if src_dims == 2:
+            result = result.reshape((size[1], size[0]))
+
+    return result
```

