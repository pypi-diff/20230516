# Comparing `tmp/fastfft-0.2.2.tar.gz` & `tmp/fastfft-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfft-0.2.2.tar", last modified: Sat May 13 11:52:26 2023, max compression
+gzip compressed data, was "fastfft-0.2.3.tar", last modified: Tue May 16 08:05:52 2023, max compression
```

## Comparing `fastfft-0.2.2.tar` & `fastfft-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 11:52:26.707533 fastfft-0.2.2/
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-05-12 16:19:20.000000 fastfft-0.2.2/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)       45 2023-05-12 16:19:20.000000 fastfft-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2172 2023-05-13 11:52:26.707533 fastfft-0.2.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      574 2023-05-13 11:44:24.000000 fastfft-0.2.2/README.md
--rw-rw-r--   0 root         (0) root         (0)       27 2023-05-12 16:19:20.000000 fastfft-0.2.2/requirements-dev.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-05-12 16:19:20.000000 fastfft-0.2.2/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)     1543 2023-05-13 11:52:26.707533 fastfft-0.2.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1338 2023-05-12 16:33:00.000000 fastfft-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 11:52:26.703533 fastfft-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 11:52:26.703533 fastfft-0.2.2/src/fastfft/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-12 16:19:20.000000 fastfft-0.2.2/src/fastfft/__init__.py
--rw-r--r--   0 root         (0) root         (0)   271807 2023-05-13 11:51:07.000000 fastfft-0.2.2/src/fastfft/fft.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 11:52:26.707533 fastfft-0.2.2/src/fastfft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2172 2023-05-13 11:52:26.000000 fastfft-0.2.2/src/fastfft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      361 2023-05-13 11:52:26.000000 fastfft-0.2.2/src/fastfft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 11:52:26.000000 fastfft-0.2.2/src/fastfft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 11:52:26.000000 fastfft-0.2.2/src/fastfft.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-13 11:52:26.000000 fastfft-0.2.2/src/fastfft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-13 11:52:26.000000 fastfft-0.2.2/src/fastfft.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 11:52:26.707533 fastfft-0.2.2/tests/
--rw-rw-r--   0 root         (0) root         (0)      149 2023-05-13 11:44:24.000000 fastfft-0.2.2/tests/test_fft2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:05:52.776160 fastfft-0.2.3/
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-05-12 16:19:20.000000 fastfft-0.2.3/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       45 2023-05-12 16:19:20.000000 fastfft-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-05-16 08:05:52.776160 fastfft-0.2.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      574 2023-05-13 11:44:24.000000 fastfft-0.2.3/README.md
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-05-12 16:19:20.000000 fastfft-0.2.3/requirements-dev.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-05-12 16:19:20.000000 fastfft-0.2.3/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)     1543 2023-05-16 08:05:52.776160 fastfft-0.2.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1338 2023-05-12 16:33:00.000000 fastfft-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:05:52.760160 fastfft-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:05:52.776160 fastfft-0.2.3/src/fastfft/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-12 16:19:20.000000 fastfft-0.2.3/src/fastfft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   271807 2023-05-16 08:05:29.000000 fastfft-0.2.3/src/fastfft/fft.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:05:52.776160 fastfft-0.2.3/src/fastfft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-05-16 08:05:52.000000 fastfft-0.2.3/src/fastfft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      361 2023-05-16 08:05:52.000000 fastfft-0.2.3/src/fastfft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:05:52.000000 fastfft-0.2.3/src/fastfft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:05:52.000000 fastfft-0.2.3/src/fastfft.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-16 08:05:52.000000 fastfft-0.2.3/src/fastfft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 08:05:52.000000 fastfft-0.2.3/src/fastfft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:05:52.776160 fastfft-0.2.3/tests/
+-rw-rw-r--   0 root         (0) root         (0)      149 2023-05-13 11:44:24.000000 fastfft-0.2.3/tests/test_fft2.py
```

### Comparing `fastfft-0.2.2/LICENSE.txt` & `fastfft-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastfft-0.2.2/PKG-INFO` & `fastfft-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.2.2
+Version: 0.2.3
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.2.2/README.md` & `fastfft-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fastfft-0.2.2/setup.cfg` & `fastfft-0.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fastfft
-version = 0.2.2
+version = 0.2.3
 description = Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = Maxim Movshin
 author_email = maxim-movshin@yandex.ru
 url = https://github.com/BSaaber/fastfft
```

### Comparing `fastfft-0.2.2/setup.py` & `fastfft-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `fastfft-0.2.2/src/fastfft/fft.cpp` & `fastfft-0.2.3/src/fastfft/fft.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2356,61 +2356,61 @@
       __pyx_t_5 = 0;
 
       /* "fastfft/fft.pyx":76
  *     for i in range(half_n):
  *         for j in range(half_n):
  *             v00 = matrix00[i][j]             # <<<<<<<<<<<<<<
  *             vW10 = matrix10[i][j] * W(n, i)
- *             vW01 = matrix10[i][j] * W(n, j)
+ *             vW01 = matrix01[i][j] * W(n, j)
  */
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
       __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
       __pyx_v_v00 = ((__pyx_v_matrix00[__pyx_t_12])[__pyx_t_13]);
 
       /* "fastfft/fft.pyx":77
  *         for j in range(half_n):
  *             v00 = matrix00[i][j]
  *             vW10 = matrix10[i][j] * W(n, i)             # <<<<<<<<<<<<<<
- *             vW01 = matrix10[i][j] * W(n, j)
- *             vW11 = matrix10[i][j] * W(n, i + i)
+ *             vW01 = matrix01[i][j] * W(n, j)
+ *             vW11 = matrix11[i][j] * W(n, i + j)
  */
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_i); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       __pyx_v_vW10 = (((__pyx_v_matrix10[__pyx_t_12])[__pyx_t_13]) * __pyx_f_7fastfft_3fft_W(__pyx_v_n, __pyx_t_15));
 
       /* "fastfft/fft.pyx":78
  *             v00 = matrix00[i][j]
  *             vW10 = matrix10[i][j] * W(n, i)
- *             vW01 = matrix10[i][j] * W(n, j)             # <<<<<<<<<<<<<<
- *             vW11 = matrix10[i][j] * W(n, i + i)
+ *             vW01 = matrix01[i][j] * W(n, j)             # <<<<<<<<<<<<<<
+ *             vW11 = matrix11[i][j] * W(n, i + j)
  * 
  */
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L1_error)
       __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L1_error)
       __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_v_j); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L1_error)
-      __pyx_v_vW01 = (((__pyx_v_matrix10[__pyx_t_12])[__pyx_t_13]) * __pyx_f_7fastfft_3fft_W(__pyx_v_n, __pyx_t_15));
+      __pyx_v_vW01 = (((__pyx_v_matrix01[__pyx_t_12])[__pyx_t_13]) * __pyx_f_7fastfft_3fft_W(__pyx_v_n, __pyx_t_15));
 
       /* "fastfft/fft.pyx":79
  *             vW10 = matrix10[i][j] * W(n, i)
- *             vW01 = matrix10[i][j] * W(n, j)
- *             vW11 = matrix10[i][j] * W(n, i + i)             # <<<<<<<<<<<<<<
+ *             vW01 = matrix01[i][j] * W(n, j)
+ *             vW11 = matrix11[i][j] * W(n, i + j)             # <<<<<<<<<<<<<<
  * 
  *             matrix[i][j] = v00 + vW10 + vW01 + vW11
  */
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
       __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
-      __pyx_t_5 = PyNumber_Add(__pyx_v_i, __pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
+      __pyx_t_5 = PyNumber_Add(__pyx_v_i, __pyx_v_j); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_15 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_15 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __pyx_v_vW11 = (((__pyx_v_matrix10[__pyx_t_12])[__pyx_t_13]) * __pyx_f_7fastfft_3fft_W(__pyx_v_n, __pyx_t_15));
+      __pyx_v_vW11 = (((__pyx_v_matrix11[__pyx_t_12])[__pyx_t_13]) * __pyx_f_7fastfft_3fft_W(__pyx_v_n, __pyx_t_15));
 
       /* "fastfft/fft.pyx":81
- *             vW11 = matrix10[i][j] * W(n, i + i)
+ *             vW11 = matrix11[i][j] * W(n, i + j)
  * 
  *             matrix[i][j] = v00 + vW10 + vW01 + vW11             # <<<<<<<<<<<<<<
  *             matrix[i + half_n][j] = v00 - vW10 + vW01 - vW11
  *             matrix[i][j + half_n] = v00 + vW10 - vW01 - vW11
  */
       __pyx_t_12 = __Pyx_PyInt_As_size_t(__pyx_v_i); if (unlikely((__pyx_t_12 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
       __pyx_t_13 = __Pyx_PyInt_As_size_t(__pyx_v_j); if (unlikely((__pyx_t_13 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
```

### Comparing `fastfft-0.2.2/src/fastfft.egg-info/PKG-INFO` & `fastfft-0.2.3/src/fastfft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfft
-Version: 0.2.2
+Version: 0.2.3
 Summary: Discrete Fourier transform implementation by the analog of the Cooley-Tukey algorithm.
 Home-page: https://github.com/BSaaber/fastfft
 Author: Maxim Movshin
 Author-email: maxim-movshin@yandex.ru
 License: MIT
 Project-URL: Documentation, https://github.com/BSaaber/fastfft
 Project-URL: Code, https://github.com/BSaaber/fastfft
```

