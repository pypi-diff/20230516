# Comparing `tmp/dghs-imgutils-0.0.3.tar.gz` & `tmp/dghs-imgutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs-imgutils-0.0.3.tar", last modified: Fri May 12 17:45:16 2023, max compression
+gzip compressed data, was "dghs-imgutils-0.0.4.tar", last modified: Tue May 16 11:00:05 2023, max compression
```

## Comparing `dghs-imgutils-0.0.3.tar` & `dghs-imgutils-0.0.4.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 17:45:16.000000 dghs-imgutils-0.0.3/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.453126 dghs-imgutils-0.0.3/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/utils/onnxruntime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 17:45:16.457126 dghs-imgutils-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-12 17:44:06.000000 dghs-imgutils-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 11:00:05.000000 dghs-imgutils-0.0.4/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.630635 dghs-imgutils-0.0.4/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/utils/onnxruntime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:00:05.634635 dghs-imgutils-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-16 10:59:09.000000 dghs-imgutils-0.0.4/setup.py
```

### Comparing `dghs-imgutils-0.0.3/LICENSE` & `dghs-imgutils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/PKG-INFO` & `dghs-imgutils-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
-Author: narugo1992
+Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `dghs-imgutils-0.0.3/README.md` & `dghs-imgutils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/dghs_imgutils.egg-info/PKG-INFO` & `dghs-imgutils-0.0.4/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
-Author: narugo1992
+Author: narugo1992, 7eu7d
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `dghs-imgutils-0.0.3/dghs_imgutils.egg-info/SOURCES.txt` & `dghs-imgutils-0.0.4/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 imgutils/detect/visual.py
 imgutils/edge/__init__.py
 imgutils/edge/_base.py
 imgutils/edge/canny.py
 imgutils/edge/lineart.py
 imgutils/edge/lineart_anime.py
 imgutils/metrics/__init__.py
+imgutils/metrics/aesthetic.py
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
 imgutils/segment/__init__.py
 imgutils/segment/isnetis.py
 imgutils/tagging/__init__.py
 imgutils/tagging/deepdanbooru.py
 imgutils/tagging/format.py
```

### Comparing `dghs-imgutils-0.0.3/dghs_imgutils.egg-info/requires.txt` & `dghs-imgutils-0.0.4/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/config/meta.py` & `dghs-imgutils-0.0.4/imgutils/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.0.3'
+__VERSION__ = '0.0.4'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
-__AUTHOR__ = 'narugo1992'
+__AUTHOR__ = 'narugo1992, 7eu7d'
 
 #: Email of the authors'.
 __AUTHOR_EMAIL__ = 'narugo@126.com'
```

### Comparing `dghs-imgutils-0.0.3/imgutils/data/background.py` & `dghs-imgutils-0.0.4/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/data/decode.py` & `dghs-imgutils-0.0.4/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/data/encode.py` & `dghs-imgutils-0.0.4/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/data/image.py` & `dghs-imgutils-0.0.4/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/data/layer.py` & `dghs-imgutils-0.0.4/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/detect/_yolo.py` & `dghs-imgutils-0.0.4/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/detect/face.py` & `dghs-imgutils-0.0.4/imgutils/detect/face.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 def _open_face_detect_model(level: str = 's'):
     return open_onnx_model(hf_hub_download(
         'deepghs/imgutils-models',
         f'face_detect/face_detect_best_{level}.onnx'
     ))
 
 
-def detect_faces(image: ImageTyping, level: str = 's', max_infer_size=1216,
+def detect_faces(image: ImageTyping, level: str = 's', max_infer_size=640,
                  conf_threshold: float = 0.25, iou_threshold: float = 0.7) \
         -> List[Tuple[Tuple[int, int, int, int], str, float]]:
     """
     Overview:
         Detect human faces (including the entire head) in anime images.
 
     :param image: Image to detect.
     :param level: The model level being used can be either `s` or `n`.
         The `n` model runs faster with smaller system overhead, while the `s` model achieves higher accuracy.
         The default value is `s`.
     :param max_infer_size: The maximum image size used for model inference, if the image size exceeds this limit,
-        the image will be resized and used for inference. The default value is `1216` pixels.
+        the image will be resized and used for inference. The default value is `640` pixels.
     :param conf_threshold: The confidence threshold, only detection results with confidence scores above
         this threshold will be returned. The default value is `0.25`.
     :param iou_threshold: The detection area coverage overlap threshold, areas with overlaps above this threshold
         will be discarded. The default value is `0.7`.
     :return: The detection results list, each item includes the detected area `(x0, y0, x1, y1)`,
         the target type (always `head`) and the target confidence score.
```

### Comparing `dghs-imgutils-0.0.3/imgutils/detect/person.py` & `dghs-imgutils-0.0.4/imgutils/detect/person.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,35 +18,42 @@
 
 from huggingface_hub import hf_hub_download
 
 from ._yolo import _image_preprocess, _data_postprocess
 from ..data import ImageTyping, load_image, rgb_encode
 from ..utils import open_onnx_model
 
+_VERSIONS = {
+    'v0': '',
+    'v1': 'plus_',
+    'v1.1': 'plus_v1.1_',
+}
+
 
 @lru_cache()
-def _open_person_detect_model(level: str = 's'):
+def _open_person_detect_model(level: str, version: str):
     return open_onnx_model(hf_hub_download(
         'deepghs/imgutils-models',
-        f'person_detect/person_detect_best_{level}.onnx'
+        f'person_detect/person_detect_{_VERSIONS[version]}best_{level}.onnx'
     ))
 
 
-def detect_person(image: ImageTyping, level: str = 's', max_infer_size=1216,
+def detect_person(image: ImageTyping, level: str = 'm', version: str = 'v1.1', max_infer_size=640,
                   conf_threshold: float = 0.3, iou_threshold: float = 0.5):
     """
     Overview:
         Detect human bodies (including the entire body) in anime images.
 
     :param image: Image to detect.
-    :param level: The model level being used can be either `s`, `m` or `x`.
-        The `s` model runs faster with smaller system overhead, while the `m` model achieves higher accuracy.
-        The default value is `s`.
+    :param level: The model level being used can be either ``n``, ``s``, ``m`` or ``x``.
+        The ``n`` model runs faster with smaller system overhead, while the ``m`` model achieves higher accuracy.
+        The default value is ``m``.
+    :param version: Version of model, default is ``v1.1``. Available versions are ``v0``, ``v1`` and ``v1.1``.
     :param max_infer_size: The maximum image size used for model inference, if the image size exceeds this limit,
-        the image will be resized and used for inference. The default value is `1216` pixels.
+        the image will be resized and used for inference. The default value is ``640`` pixels.
     :param conf_threshold: The confidence threshold, only detection results with confidence scores above
         this threshold will be returned. The default value is `0.3`.
     :param iou_threshold: The detection area coverage overlap threshold, areas with overlaps above this threshold
         will be discarded. The default value is `0.5`.
     :return: The detection results list, each item includes the detected area `(x0, y0, x1, y1)`,
         the target type (always `person`) and the target confidence score.
 
@@ -63,14 +70,20 @@
             ((614, 3, 1275, 654), 'person', 0.4047100841999054)
         ]
         >>>
         >>> # visualize it
         >>> from matplotlib import pyplot as plt
         >>> plt.imshow(detection_visualize(image, result))
         >>> plt.show()
+
+    .. note::
+        Please note that certain combinations of versions and levels may not have corresponding models.
+        When using them, please refer to the performance chart at the top of that page, which lists
+        the versions and models included.
+
     """
     image = load_image(image, mode='RGB')
     new_image, old_size, new_size = _image_preprocess(image, max_infer_size)
 
     data = rgb_encode(new_image)[None, ...]
-    output, = _open_person_detect_model(level).run(['output0'], {'images': data})
+    output, = _open_person_detect_model(level, version).run(['output0'], {'images': data})
     return _data_postprocess(output[0], conf_threshold, iou_threshold, old_size, new_size, ['person'])
```

### Comparing `dghs-imgutils-0.0.3/imgutils/detect/visual.py` & `dghs-imgutils-0.0.4/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/edge/__init__.py` & `dghs-imgutils-0.0.4/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/edge/_base.py` & `dghs-imgutils-0.0.4/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/edge/canny.py` & `dghs-imgutils-0.0.4/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/edge/lineart.py` & `dghs-imgutils-0.0.4/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/edge/lineart_anime.py` & `dghs-imgutils-0.0.4/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/metrics/lpips.py` & `dghs-imgutils-0.0.4/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/metrics/psnr_.py` & `dghs-imgutils-0.0.4/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/segment/isnetis.py` & `dghs-imgutils-0.0.4/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/tagging/deepdanbooru.py` & `dghs-imgutils-0.0.4/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/tagging/format.py` & `dghs-imgutils-0.0.4/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/tagging/mldanbooru.py` & `dghs-imgutils-0.0.4/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/tagging/wd14.py` & `dghs-imgutils-0.0.4/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/utils/onnxruntime.py` & `dghs-imgutils-0.0.4/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/validate/color.py` & `dghs-imgutils-0.0.4/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/validate/monochrome.py` & `dghs-imgutils-0.0.4/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/imgutils/validate/truncate.py` & `dghs-imgutils-0.0.4/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs-imgutils-0.0.3/setup.py` & `dghs-imgutils-0.0.4/setup.py`

 * *Files identical despite different names*

