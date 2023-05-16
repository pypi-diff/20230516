# Comparing `tmp/aotpy-0.6.1.tar.gz` & `tmp/aotpy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.6.1.tar", last modified: Tue May 16 13:56:07 2023, max compression
+gzip compressed data, was "aotpy-0.6.2.tar", last modified: Tue May 16 14:43:58 2023, max compression
```

## Comparing `aotpy-0.6.1.tar` & `aotpy-0.6.2.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:07.034304 aotpy-0.6.1/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     2991 2023-05-16 13:56:07.035281 aotpy-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:06.964977 aotpy-0.6.1/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.6.1/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:07.009890 aotpy-0.6.1/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.6.1/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.6.1/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     3967 2023-05-03 10:26:29.000000 aotpy-0.6.1/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 11:38:37.000000 aotpy-0.6.1/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0      618 2023-05-03 10:52:05.000000 aotpy-0.6.1/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.6.1/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-05-03 17:08:11.000000 aotpy-0.6.1/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.6.1/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.6.1/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-05-08 11:39:26.000000 aotpy-0.6.1/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.6.1/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3554 2023-05-08 11:39:26.000000 aotpy-0.6.1/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:07.010867 aotpy-0.6.1/aotpy/data/
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.6.1/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:07.015757 aotpy-0.6.1/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.6.1/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.6.1/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:07.022586 aotpy-0.6.1/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.6.1/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26711 2023-05-16 13:12:55.000000 aotpy-0.6.1/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    42036 2023-05-08 12:12:15.000000 aotpy-0.6.1/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     8760 2023-05-03 10:32:11.000000 aotpy-0.6.1/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31083 2023-05-08 11:41:08.000000 aotpy-0.6.1/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:07.033329 aotpy-0.6.1/aotpy/translators/
--rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.6.1/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0    11058 2023-05-16 13:51:26.000000 aotpy-0.6.1/aotpy/translators/aof.py
--rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.6.1/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     6842 2023-05-15 12:17:23.000000 aotpy-0.6.1/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    14290 2023-05-16 13:51:26.000000 aotpy-0.6.1/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0     9095 2023-05-15 14:15:02.000000 aotpy-0.6.1/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0     7181 2023-05-16 13:43:00.000000 aotpy-0.6.1/aotpy/translators/naomi.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:56:06.990361 aotpy-0.6.1/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2991 2023-05-16 13:56:06.000000 aotpy-0.6.1/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      856 2023-05-16 13:56:06.000000 aotpy-0.6.1/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:56:06.000000 aotpy-0.6.1/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-05-16 13:56:06.000000 aotpy-0.6.1/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 13:56:06.000000 aotpy-0.6.1/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0     1011 2023-05-16 13:56:07.044069 aotpy-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.205047 aotpy-0.6.2/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     2991 2023-05-16 14:43:58.205047 aotpy-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.138066 aotpy-0.6.2/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.6.2/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.174776 aotpy-0.6.2/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.6.2/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.6.2/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     3967 2023-05-03 10:26:29.000000 aotpy-0.6.2/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 11:38:37.000000 aotpy-0.6.2/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0      618 2023-05-03 10:52:05.000000 aotpy-0.6.2/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.6.2/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-05-03 17:08:11.000000 aotpy-0.6.2/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.6.2/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.6.2/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-05-08 11:39:26.000000 aotpy-0.6.2/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.6.2/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3554 2023-05-08 11:39:26.000000 aotpy-0.6.2/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.175753 aotpy-0.6.2/aotpy/data/
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.177709 aotpy-0.6.2/aotpy/data/AOF/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.6.2/aotpy/data/AOF/subap.fits
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.179659 aotpy-0.6.2/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.6.2/aotpy/data/ERIS/subap.fits
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.180636 aotpy-0.6.2/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.6.2/aotpy/data/NAOMI/zernike_control_modes.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.6.2/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.189424 aotpy-0.6.2/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.6.2/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.6.2/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.196259 aotpy-0.6.2/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.6.2/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26711 2023-05-16 13:12:55.000000 aotpy-0.6.2/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    42036 2023-05-08 12:12:15.000000 aotpy-0.6.2/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     8760 2023-05-03 10:32:11.000000 aotpy-0.6.2/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31083 2023-05-08 11:41:08.000000 aotpy-0.6.2/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.204072 aotpy-0.6.2/aotpy/translators/
+-rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.6.2/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0    11058 2023-05-16 13:51:26.000000 aotpy-0.6.2/aotpy/translators/aof.py
+-rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.6.2/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     6842 2023-05-15 12:17:23.000000 aotpy-0.6.2/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    14290 2023-05-16 13:51:26.000000 aotpy-0.6.2/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0     9095 2023-05-15 14:15:02.000000 aotpy-0.6.2/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0     7181 2023-05-16 13:43:00.000000 aotpy-0.6.2/aotpy/translators/naomi.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:43:58.158575 aotpy-0.6.2/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2991 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 14:43:58.000000 aotpy-0.6.2/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1019 2023-05-16 14:43:58.207979 aotpy-0.6.2/setup.cfg
```

### Comparing `aotpy-0.6.1/LICENSE` & `aotpy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/PKG-INFO` & `aotpy-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/kYwzor/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.6.1/README.md` & `aotpy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/__init__.py` & `aotpy-0.6.2/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/__init__.py` & `aotpy-0.6.2/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/aberration.py` & `aotpy-0.6.2/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/ao_system.py` & `aotpy-0.6.2/aotpy/core/ao_system.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/atmosphere.py` & `aotpy-0.6.2/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/base.py` & `aotpy-0.6.2/aotpy/core/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/image.py` & `aotpy-0.6.2/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/loop.py` & `aotpy-0.6.2/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/optical_sensor.py` & `aotpy-0.6.2/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/source.py` & `aotpy-0.6.2/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/telescope.py` & `aotpy-0.6.2/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/time.py` & `aotpy-0.6.2/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/core/wavefront_corrector.py` & `aotpy-0.6.2/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/io/base.py` & `aotpy-0.6.2/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/io/fits/_keywords.py` & `aotpy-0.6.2/aotpy/io/fits/_keywords.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/io/fits/reader.py` & `aotpy-0.6.2/aotpy/io/fits/reader.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/io/fits/utils.py` & `aotpy-0.6.2/aotpy/io/fits/utils.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/io/fits/writer.py` & `aotpy-0.6.2/aotpy/io/fits/writer.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/translators/aof.py` & `aotpy-0.6.2/aotpy/translators/aof.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/translators/base.py` & `aotpy-0.6.2/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/translators/ciao.py` & `aotpy-0.6.2/aotpy/translators/ciao.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/translators/eris.py` & `aotpy-0.6.2/aotpy/translators/eris.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/translators/eso.py` & `aotpy-0.6.2/aotpy/translators/eso.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy/translators/naomi.py` & `aotpy-0.6.2/aotpy/translators/naomi.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.6.1/aotpy.egg-info/PKG-INFO` & `aotpy-0.6.2/aotpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/kYwzor/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.6.1/aotpy.egg-info/SOURCES.txt` & `aotpy-0.6.2/aotpy.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 aotpy/core/loop.py
 aotpy/core/optical_sensor.py
 aotpy/core/source.py
 aotpy/core/telescope.py
 aotpy/core/time.py
 aotpy/core/wavefront_corrector.py
 aotpy/data/__init__.py
+aotpy/data/AOF/subap.fits
+aotpy/data/ERIS/subap.fits
+aotpy/data/NAOMI/zernike_control_modes.fits
 aotpy/io/__init__.py
 aotpy/io/base.py
 aotpy/io/fits/__init__.py
 aotpy/io/fits/_keywords.py
 aotpy/io/fits/reader.py
 aotpy/io/fits/utils.py
 aotpy/io/fits/writer.py
```

### Comparing `aotpy-0.6.1/setup.cfg` & `aotpy-0.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 362e 310d 0a61 7574 686f  n = 0.6.1..autho
+00000020: 6e20 3d20 302e 362e 320d 0a61 7574 686f  n = 0.6.2..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
@@ -44,21 +44,21 @@
 000002b0: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
 000002c0: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
 000002d0: 300d 0a69 6e73 7461 6c6c 5f72 6571 7569  0..install_requi
 000002e0: 7265 7320 3d20 0d0a 0961 7374 726f 7079  res = ...astropy
 000002f0: 3e3d 352e 312e 310d 0a09 6e75 6d70 793e  >=5.1.1...numpy>
 00000300: 3d31 2e32 300d 0a0d 0a5b 6f70 7469 6f6e  =1.20....[option
 00000310: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000320: 0a64 6174 6120 3d20 2a2e 6669 7473 0d0a  .data = *.fits..
-00000330: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
-00000340: 735f 7265 7175 6972 655d 0d0a 6573 6f61  s_require]..esoa
-00000350: 7263 6869 7665 203d 200d 0a09 7079 766f  rchive = ...pyvo
-00000360: 3e3d 312e 340d 0a73 6176 6669 6c65 7320  >=1.4..savfiles 
-00000370: 3d20 0d0a 0973 6369 7079 3e3d 312e 330d  = ...scipy>=1.3.
-00000380: 0a64 6f63 7320 3d20 0d0a 0973 7068 696e  .docs = ...sphin
-00000390: 780d 0a09 7370 6869 6e78 2d72 7464 2d74  x...sphinx-rtd-t
-000003a0: 6865 6d65 0d0a 616c 6c20 3d20 0d0a 0970  heme..all = ...p
-000003b0: 7976 6f3e 3d31 2e34 0d0a 0973 6369 7079  yvo>=1.4...scipy
-000003c0: 3e3d 312e 330d 0a0d 0a5b 6567 675f 696e  >=1.3....[egg_in
-000003d0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000003e0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000003f0: 0a0d 0a                                  ...
+00000320: 0a61 6f74 7079 2e64 6174 6120 3d20 2a2f  .aotpy.data = */
+00000330: 2a2e 6669 7473 0d0a 0d0a 5b6f 7074 696f  *.fits....[optio
+00000340: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
+00000350: 655d 0d0a 6573 6f61 7263 6869 7665 203d  e]..esoarchive =
+00000360: 200d 0a09 7079 766f 3e3d 312e 340d 0a73   ...pyvo>=1.4..s
+00000370: 6176 6669 6c65 7320 3d20 0d0a 0973 6369  avfiles = ...sci
+00000380: 7079 3e3d 312e 330d 0a64 6f63 7320 3d20  py>=1.3..docs = 
+00000390: 0d0a 0973 7068 696e 780d 0a09 7370 6869  ...sphinx...sphi
+000003a0: 6e78 2d72 7464 2d74 6865 6d65 0d0a 616c  nx-rtd-theme..al
+000003b0: 6c20 3d20 0d0a 0970 7976 6f3e 3d31 2e34  l = ...pyvo>=1.4
+000003c0: 0d0a 0973 6369 7079 3e3d 312e 330d 0a0d  ...scipy>=1.3...
+000003d0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000003e0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000003f0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

