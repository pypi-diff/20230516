# Comparing `tmp/sleepens-1.0.2.tar.gz` & `tmp/sleepens-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sleepens-1.0.2.tar", last modified: Mon May 15 22:38:34 2023, max compression
+gzip compressed data, was "dist\sleepens-1.0.3.tar", last modified: Mon May 15 22:44:28 2023, max compression
```

## Comparing `sleepens-1.0.2.tar` & `sleepens-1.0.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/
--rw-rw-rw-   0        0        0      722 2021-11-17 16:31:54.000000 sleepens-1.0.2/BUILDS.md
--rw-rw-rw-   0        0        0     3003 2023-05-15 22:30:02.000000 sleepens-1.0.2/CHANGES.md
--rw-rw-rw-   0        0        0     1549 2021-09-18 21:33:43.000000 sleepens-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       84 2021-09-18 21:33:43.000000 sleepens-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7293 2023-05-15 22:38:34.000000 sleepens-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6052 2023-05-15 22:30:02.000000 sleepens-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:33.000000 sleepens-1.0.2/doc/
--rw-rw-rw-   0        0        0      399 2021-09-18 21:33:43.000000 sleepens-1.0.2/doc/README.md
--rw-rw-rw-   0        0        0      111 2023-05-15 22:38:34.000000 sleepens-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1699 2023-05-15 21:45:14.000000 sleepens-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:33.000000 sleepens-1.0.2/sleepens/
--rw-rw-rw-   0        0        0       47 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/analysis/
--rw-rw-rw-   0        0        0      270 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/analysis/__init__.py
--rw-rw-rw-   0        0        0     2836 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/analysis/_confusion_matrix.py
--rw-rw-rw-   0        0        0     4968 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/analysis/_report.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/io/
--rw-rw-rw-   0        0        0      121 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/io/__init__.py
--rw-rw-rw-   0        0        0     3132 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/io/_dataobject.py
--rw-rw-rw-   0        0        0     5475 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/io/_dataset.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/io/interfaces/
--rw-rw-rw-   0        0        0      113 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/io/interfaces/__init__.py
--rw-rw-rw-   0        0        0     3136 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/io/interfaces/smrMAT.py
--rw-rw-rw-   0        0        0     6184 2023-04-14 17:03:39.000000 sleepens-1.0.2/sleepens/io/interfaces/son.py
--rw-rw-rw-   0        0        0     4394 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/io/interfaces/xls.py
--rw-rw-rw-   0        0        0    17246 2023-05-15 22:29:38.000000 sleepens-1.0.2/sleepens/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/ml/
--rw-rw-rw-   0        0        0      202 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/ml/__init__.py
--rw-rw-rw-   0        0        0    18272 2023-05-15 21:46:05.000000 sleepens-1.0.2/sleepens/ml/_base_model.py
--rw-rw-rw-   0        0        0     8288 2023-04-14 16:05:00.000000 sleepens-1.0.2/sleepens/ml/_cv.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/ml/models/
--rw-rw-rw-   0        0        0      246 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/ml/models/__init__.py
--rw-rw-rw-   0        0        0    12664 2023-05-15 21:56:32.000000 sleepens-1.0.2/sleepens/ml/models/_gb.py
--rw-rw-rw-   0        0        0     5366 2023-05-15 22:00:21.000000 sleepens-1.0.2/sleepens/ml/models/_stsens.py
--rw-rw-rw-   0        0        0     6666 2023-05-15 21:46:28.000000 sleepens-1.0.2/sleepens/ml/models/_tsens.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/postprocess/
--rw-rw-rw-   0        0        0      471 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1116 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_min_rem.py
--rw-rw-rw-   0        0        0     1591 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_rem_drop.py
--rw-rw-rw-   0        0        0     2431 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_rem_sensitivity.py
--rw-rw-rw-   0        0        0     2993 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_transition_fix.py
--rw-rw-rw-   0        0        0     1230 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_wake_max.py
--rw-rw-rw-   0        0        0     1291 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_wake_sensitivity.py
--rw-rw-rw-   0        0        0     1118 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/postprocess/_wake_to_rem.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/process/
--rw-rw-rw-   0        0        0        0 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/process/primary/
--rw-rw-rw-   0        0        0      230 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/primary/__init__.py
--rw-rw-rw-   0        0        0     2459 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/primary/_epoched_variance.py
--rw-rw-rw-   0        0        0     1553 2021-11-17 16:14:07.000000 sleepens-1.0.2/sleepens/process/primary/_fft.py
--rw-rw-rw-   0        0        0     1178 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/primary/_percentile_mean.py
--rw-rw-rw-   0        0        0     1003 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/primary/_rms.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/process/secondary/
--rw-rw-rw-   0        0        0      288 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/secondary/__init__.py
--rw-rw-rw-   0        0        0      731 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/secondary/_merge.py
--rw-rw-rw-   0        0        0      865 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/secondary/_ratio.py
--rw-rw-rw-   0        0        0     1163 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/secondary/_spectral_band.py
--rw-rw-rw-   0        0        0      849 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/secondary/_spectral_entropy.py
--rw-rw-rw-   0        0        0     1003 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/process/secondary/_transform.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/protocols/
--rw-rw-rw-   0        0        0       81 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/protocols/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/protocols/sleepens4/
--rw-rw-rw-   0        0        0       78 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/protocols/sleepens4/__init__.py
--rw-rw-rw-   0        0        0     1670 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/protocols/sleepens4/params.py
--rw-rw-rw-   0        0        0     4081 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/protocols/sleepens4/processor.py
--rw-rw-rw-   0        0        0     3457 2023-02-04 19:29:05.000000 sleepens-1.0.2/sleepens/protocols/sleepens4/sleepens4.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/utils/
--rw-rw-rw-   0        0        0      663 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/__init__.py
--rw-rw-rw-   0        0        0     3115 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/_calculate.py
--rw-rw-rw-   0        0        0     2554 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/_check.py
--rw-rw-rw-   0        0        0     3652 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/_data_mgmt.py
--rw-rw-rw-   0        0        0     2177 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/_misc.py
--rw-rw-rw-   0        0        0      825 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/_random.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens/utils/data/
--rw-rw-rw-   0        0        0        0 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/data/__init__.py
--rw-rw-rw-   0        0        0     3044 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/data/normalize.py
--rw-rw-rw-   0        0        0     8215 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/data/sampling.py
--rw-rw-rw-   0        0        0     5702 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/data/signal.py
--rw-rw-rw-   0        0        0     1885 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/data/smooth.py
--rw-rw-rw-   0        0        0     1812 2021-09-18 21:33:43.000000 sleepens-1.0.2/sleepens/utils/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:38:34.000000 sleepens-1.0.2/sleepens.egg-info/
--rw-rw-rw-   0        0        0     7293 2023-05-15 22:38:33.000000 sleepens-1.0.2/sleepens.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2103 2023-05-15 22:38:33.000000 sleepens-1.0.2/sleepens.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 22:38:33.000000 sleepens-1.0.2/sleepens.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-05-15 22:38:33.000000 sleepens-1.0.2/sleepens.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 22:38:33.000000 sleepens-1.0.2/sleepens.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2021-09-18 22:13:55.000000 sleepens-1.0.2/sleepens.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/
+-rw-rw-rw-   0        0        0      722 2021-11-17 16:31:54.000000 sleepens-1.0.3/BUILDS.md
+-rw-rw-rw-   0        0        0     3003 2023-05-15 22:44:19.000000 sleepens-1.0.3/CHANGES.md
+-rw-rw-rw-   0        0        0     1549 2021-09-18 21:33:43.000000 sleepens-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       84 2021-09-18 21:33:43.000000 sleepens-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7155 2023-05-15 22:44:28.000000 sleepens-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6016 2023-05-15 22:44:19.000000 sleepens-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/doc/
+-rw-rw-rw-   0        0        0      399 2021-09-18 21:33:43.000000 sleepens-1.0.3/doc/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-15 22:44:28.000000 sleepens-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2023-05-15 22:44:19.000000 sleepens-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/
+-rw-rw-rw-   0        0        0       47 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/analysis/
+-rw-rw-rw-   0        0        0      270 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2836 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/analysis/_confusion_matrix.py
+-rw-rw-rw-   0        0        0     4968 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/analysis/_report.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/io/
+-rw-rw-rw-   0        0        0      121 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/io/__init__.py
+-rw-rw-rw-   0        0        0     3132 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/io/_dataobject.py
+-rw-rw-rw-   0        0        0     5475 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/io/_dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/io/interfaces/
+-rw-rw-rw-   0        0        0      113 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/io/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     3136 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/io/interfaces/smrMAT.py
+-rw-rw-rw-   0        0        0     6184 2023-04-14 17:03:39.000000 sleepens-1.0.3/sleepens/io/interfaces/son.py
+-rw-rw-rw-   0        0        0     4394 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/io/interfaces/xls.py
+-rw-rw-rw-   0        0        0    17246 2023-05-15 22:44:19.000000 sleepens-1.0.3/sleepens/main.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/ml/
+-rw-rw-rw-   0        0        0      202 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/ml/__init__.py
+-rw-rw-rw-   0        0        0    18272 2023-05-15 21:46:05.000000 sleepens-1.0.3/sleepens/ml/_base_model.py
+-rw-rw-rw-   0        0        0     8288 2023-04-14 16:05:00.000000 sleepens-1.0.3/sleepens/ml/_cv.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/ml/models/
+-rw-rw-rw-   0        0        0      246 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/ml/models/__init__.py
+-rw-rw-rw-   0        0        0    12664 2023-05-15 21:56:32.000000 sleepens-1.0.3/sleepens/ml/models/_gb.py
+-rw-rw-rw-   0        0        0     5366 2023-05-15 22:00:21.000000 sleepens-1.0.3/sleepens/ml/models/_stsens.py
+-rw-rw-rw-   0        0        0     6666 2023-05-15 21:46:28.000000 sleepens-1.0.3/sleepens/ml/models/_tsens.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/postprocess/
+-rw-rw-rw-   0        0        0      471 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1116 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_min_rem.py
+-rw-rw-rw-   0        0        0     1591 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_rem_drop.py
+-rw-rw-rw-   0        0        0     2431 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_rem_sensitivity.py
+-rw-rw-rw-   0        0        0     2993 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_transition_fix.py
+-rw-rw-rw-   0        0        0     1230 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_wake_max.py
+-rw-rw-rw-   0        0        0     1291 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_wake_sensitivity.py
+-rw-rw-rw-   0        0        0     1118 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/postprocess/_wake_to_rem.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/process/
+-rw-rw-rw-   0        0        0        0 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/process/primary/
+-rw-rw-rw-   0        0        0      230 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/primary/__init__.py
+-rw-rw-rw-   0        0        0     2459 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/primary/_epoched_variance.py
+-rw-rw-rw-   0        0        0     1553 2021-11-17 16:14:07.000000 sleepens-1.0.3/sleepens/process/primary/_fft.py
+-rw-rw-rw-   0        0        0     1178 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/primary/_percentile_mean.py
+-rw-rw-rw-   0        0        0     1003 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/primary/_rms.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/process/secondary/
+-rw-rw-rw-   0        0        0      288 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/secondary/__init__.py
+-rw-rw-rw-   0        0        0      731 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/secondary/_merge.py
+-rw-rw-rw-   0        0        0      865 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/secondary/_ratio.py
+-rw-rw-rw-   0        0        0     1163 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/secondary/_spectral_band.py
+-rw-rw-rw-   0        0        0      849 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/secondary/_spectral_entropy.py
+-rw-rw-rw-   0        0        0     1003 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/process/secondary/_transform.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/protocols/
+-rw-rw-rw-   0        0        0       81 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/protocols/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/protocols/sleepens4/
+-rw-rw-rw-   0        0        0       78 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/protocols/sleepens4/__init__.py
+-rw-rw-rw-   0        0        0     1670 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/protocols/sleepens4/params.py
+-rw-rw-rw-   0        0        0     4081 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/protocols/sleepens4/processor.py
+-rw-rw-rw-   0        0        0     3457 2023-02-04 19:29:05.000000 sleepens-1.0.3/sleepens/protocols/sleepens4/sleepens4.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/utils/
+-rw-rw-rw-   0        0        0      663 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/__init__.py
+-rw-rw-rw-   0        0        0     3115 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/_calculate.py
+-rw-rw-rw-   0        0        0     2554 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/_check.py
+-rw-rw-rw-   0        0        0     3652 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/_data_mgmt.py
+-rw-rw-rw-   0        0        0     2177 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/_misc.py
+-rw-rw-rw-   0        0        0      825 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/_random.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens/utils/data/
+-rw-rw-rw-   0        0        0        0 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/data/__init__.py
+-rw-rw-rw-   0        0        0     3044 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/data/normalize.py
+-rw-rw-rw-   0        0        0     8215 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/data/sampling.py
+-rw-rw-rw-   0        0        0     5702 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/data/signal.py
+-rw-rw-rw-   0        0        0     1885 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/data/smooth.py
+-rw-rw-rw-   0        0        0     1812 2021-09-18 21:33:43.000000 sleepens-1.0.3/sleepens/utils/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens.egg-info/
+-rw-rw-rw-   0        0        0     7155 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2103 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 22:44:28.000000 sleepens-1.0.3/sleepens.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2021-09-18 22:13:55.000000 sleepens-1.0.3/sleepens.egg-info/zip-safe
```

### Comparing `sleepens-1.0.2/BUILDS.md` & `sleepens-1.0.3/BUILDS.md`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/CHANGES.md` & `sleepens-1.0.3/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - ![Feature](https://img.shields.io/badge/-Feature-blueviolet?style=flat-square) : Something that you couldn’t do before.
 - ![Enhancement](https://img.shields.io/badge/-Enhancement-purple?style=flat-square) : A miscellaneous minor improvement.
 - ![Efficiency](https://img.shields.io/badge/-Efficiency-indigo?style=flat-square) : An existing feature now may not require as much computation or memory.
 - ![Fix](https://img.shields.io/badge/-Fix-red?style=flat-square) : Something that previously didn’t work as documented or as expected should now work.
 - ![Documentation](https://img.shields.io/badge/-Documentation-blue?style=flat-square) : An update to the documentation.
 - ![Other](https://img.shields.io/badge/-Other-lightgrey?style=flat-square) : Miscellaneous updates such as package structure or GitHub quality of life updates.
 
-### Version 1.0.2
+### Version 1.0.3
 - ![Documentation](https://img.shields.io/badge/-Documentation-blue?style=flat-square) : Updated README to reflect freezing of dependencies.
 - ![Other](https://img.shields.io/badge/-Other-lightgrey?style=flat-square) : Specified exact versions of dependencies in `requirements.txt` and in `setup.py`.
 
 ### Version 1.0.1
 - ![Fix](https://img.shields.io/badge/-Fix-red?style=flat-square) : Remove `min_impurity_split` from `GradientBoostingClassifier` as it no longer exists in the underlying `sklearn` class.
 - ![Documentation](https://img.shields.io/badge/-Documentation-blue?style=flat-square) : Improve organization of the build directory.
```

### Comparing `sleepens-1.0.2/LICENSE` & `sleepens-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/PKG-INFO` & `sleepens-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: sleepens
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sleep Classification using Ensemble Classification
 Home-page: http://github.com/paradoxysm/sleepens
 Author: paradoxysm
 Author-email: paradoxysm.dev@gmail.com
 License: BSD-3-Clause
-Download-URL: https://github.com/paradoxysm/sleepens/archive/1.0.2.tar.gz
+Download-URL: https://github.com/paradoxysm/sleepens/archive/1.0.3.tar.gz
 Keywords: python,ml,ensemble,sleep,classification
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,22 +29,22 @@
 
 [![CircleCI](https://img.shields.io/circleci/build/github/paradoxysm/sleepens?style=flat-square)](https://circleci.com/gh/paradoxysm/sleepens/tree/master)
 [![Codecov](https://flat.badgen.net/codecov/c/github/paradoxysm/sleepens?label=coverage&kill_cache=1)](https://codecov.io/gh/paradoxysm/sleepens)
 [![DOI](https://img.shields.io/badge/DOI-10.5821%2Fzenodo.7791521-blue?style=flat-square)](https://zenodo.org/badge/latestdoi/282098794)
 [![GitHub](https://img.shields.io/github/license/paradoxysm/sleepens?color=blue&style=flat-square)](https://github.com/paradoxysm/sleepens/blob/master/LICENSE)
 
 Sleep Ensemble is a framework for end-to-end sleep state classification using machine learning. It is designed to allow for modular data processing, classification, and further post-processing.
-Please see [here](https://academic.oup.com/sleep/advance-article-abstract/doi/10.1093/sleep/zsad101/7109541) for publication.
+Published in [SLEEP](https://academic.oup.com/sleep/advance-article-abstract/doi/10.1093/sleep/zsad101/7109541).
 
 ## Installation
 
 Install a suitable python environment from [python.org](https://www.python.org/downloads/release/python-378/).
-> Sleep Ensemble supports Python 3.7 to 3.9. It is extensively tested and developed with 64-bit Python 3.7.8 on Windows.
+> Sleep Ensemble supports Python 3.7 only. It is extensively tested and developed with 64-bit Python 3.7.8 on Windows.
 
-> Sleep Ensemble pre-trained builds are only useable for the specific OS and 32/64-bit Python environment. Its use may be possible with other Python 3.x versions but not guaranteed. The included pre-trained SleepEnsemble4 is built on 64-bit Python 3.7.8 on Windows.
+> Sleep Ensemble pre-trained builds are only useable for the specific OS and 32/64-bit Python environment. The included pre-trained SleepEnsemble4 is built on 64-bit Python 3.7.8 on Windows.
 
 Install the latest `sleepens` release using `pip` (on a terminal like command prompt):
 ```
 pip install sleepens
 ```
 Alternatively, download the source code for the latest release [here](https://github.com/paradoxysm/sleepens/releases). Unzip into desired location. Using the terminal, navigate to the top `sleepens` folder where `setup.py` is located and run the following:
 ```
@@ -102,28 +100,34 @@
 
 The underlying data processing pipelines and classification models are modular and can be adjusted to create different sleep ensemble models. `sleepens` currently contains one protocol, SleepEnsemble4, for 4-state sleep classification. New or modified protocols can be contributed to `sleepens.protocols` following the basic structure.
 
 Finally, `sleepens` uses `joblib` to store the pre-trained builds. This isn't the most secure method nor is the most data storage efficient. Ideally, a custom parameter export/load method is implemented that can reinstate a pre-trained build.
 
 ## Dependencies
 
-`sleepens` was developed using Python 3.7.8. Since development, `scikit-learn` has updated to a point that `sleepens` is not compatible with later versions of `scikit-learn` due to attribute name changes. At the same time, `sonpy` is limited to Python 3.7 to 3.9. For the sake of replicability (especially with pre-trained models provided on publication, the repository remains using the below dependencies at these versions.
+`sleepens` was developed using Python 3.7.8. Since development, `scikit-learn` has updated to a point that `sleepens` is not compatible with later versions of `scikit-learn` due to attribute name changes. At the same time, `sonpy` is limited to Python 3.7 to 3.9. For the sake of replicability (especially with pre-trained models provided on publication, the repository remains using the below dependencies at these versions. This also limits Python to 3.7.
 
 ```
 numpy==1.21.6
 scikit-learn==0.24.0
 joblib==1.0.0
 tqdm==4.55.0
 xlrd==2.0.1
 xlwt==1.3.0
 sonpy==1.7.5
 scipy==1.7.2
 ```
 
-Should one wish to upgrade these dependencies to the latest version of `scikit-learn`, change all references of `n_features_` to `n_features_in_` in `sleepens/sleepens/ml/_base_model.py`, `sleepens/sleepens/ml/models/_gb.py`, `sleepens/sleepens/ml/models/_tsens.py`, and `sleepens/sleepens/ml/models/_stsens.py`. Furthermore, change the loss parameter in `sleepens/sleepens/ml/_gb.py` line 220 to 'log_loss' (which replaces 'deviance' but is algorithmically the same). 
+Should one wish to upgrade these dependencies to the latest version of `scikit-learn`, change all references of `n_features_` to `n_features_in_` in the following:
+- `sleepens/sleepens/ml/_base_model.py`
+- `sleepens/sleepens/ml/models/_gb.py`
+- `sleepens/sleepens/ml/models/_tsens.py`
+- `sleepens/sleepens/ml/models/_stsens.py`
+
+Furthermore, change the loss parameter in `sleepens/sleepens/ml/_gb.py` line 220 to 'log_loss' (which replaces 'deviance' but is algorithmically the same). 
 
 ## Help and Support
 
 ### Documentation
 
 Documentation for `sleepens` can be found [here](https://github.com/paradoxysm/sleepens/tree/master/doc).
```

### Comparing `sleepens-1.0.2/README.md` & `sleepens-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 [![CircleCI](https://img.shields.io/circleci/build/github/paradoxysm/sleepens?style=flat-square)](https://circleci.com/gh/paradoxysm/sleepens/tree/master)
 [![Codecov](https://flat.badgen.net/codecov/c/github/paradoxysm/sleepens?label=coverage&kill_cache=1)](https://codecov.io/gh/paradoxysm/sleepens)
 [![DOI](https://img.shields.io/badge/DOI-10.5821%2Fzenodo.7791521-blue?style=flat-square)](https://zenodo.org/badge/latestdoi/282098794)
 [![GitHub](https://img.shields.io/github/license/paradoxysm/sleepens?color=blue&style=flat-square)](https://github.com/paradoxysm/sleepens/blob/master/LICENSE)
 
 Sleep Ensemble is a framework for end-to-end sleep state classification using machine learning. It is designed to allow for modular data processing, classification, and further post-processing.
-Please see [here](https://academic.oup.com/sleep/advance-article-abstract/doi/10.1093/sleep/zsad101/7109541) for publication.
+Published in [SLEEP](https://academic.oup.com/sleep/advance-article-abstract/doi/10.1093/sleep/zsad101/7109541).
 
 ## Installation
 
 Install a suitable python environment from [python.org](https://www.python.org/downloads/release/python-378/).
-> Sleep Ensemble supports Python 3.7 to 3.9. It is extensively tested and developed with 64-bit Python 3.7.8 on Windows.
+> Sleep Ensemble supports Python 3.7 only. It is extensively tested and developed with 64-bit Python 3.7.8 on Windows.
 
-> Sleep Ensemble pre-trained builds are only useable for the specific OS and 32/64-bit Python environment. Its use may be possible with other Python 3.x versions but not guaranteed. The included pre-trained SleepEnsemble4 is built on 64-bit Python 3.7.8 on Windows.
+> Sleep Ensemble pre-trained builds are only useable for the specific OS and 32/64-bit Python environment. The included pre-trained SleepEnsemble4 is built on 64-bit Python 3.7.8 on Windows.
 
 Install the latest `sleepens` release using `pip` (on a terminal like command prompt):
 ```
 pip install sleepens
 ```
 Alternatively, download the source code for the latest release [here](https://github.com/paradoxysm/sleepens/releases). Unzip into desired location. Using the terminal, navigate to the top `sleepens` folder where `setup.py` is located and run the following:
 ```
@@ -73,28 +73,34 @@
 
 The underlying data processing pipelines and classification models are modular and can be adjusted to create different sleep ensemble models. `sleepens` currently contains one protocol, SleepEnsemble4, for 4-state sleep classification. New or modified protocols can be contributed to `sleepens.protocols` following the basic structure.
 
 Finally, `sleepens` uses `joblib` to store the pre-trained builds. This isn't the most secure method nor is the most data storage efficient. Ideally, a custom parameter export/load method is implemented that can reinstate a pre-trained build.
 
 ## Dependencies
 
-`sleepens` was developed using Python 3.7.8. Since development, `scikit-learn` has updated to a point that `sleepens` is not compatible with later versions of `scikit-learn` due to attribute name changes. At the same time, `sonpy` is limited to Python 3.7 to 3.9. For the sake of replicability (especially with pre-trained models provided on publication, the repository remains using the below dependencies at these versions.
+`sleepens` was developed using Python 3.7.8. Since development, `scikit-learn` has updated to a point that `sleepens` is not compatible with later versions of `scikit-learn` due to attribute name changes. At the same time, `sonpy` is limited to Python 3.7 to 3.9. For the sake of replicability (especially with pre-trained models provided on publication, the repository remains using the below dependencies at these versions. This also limits Python to 3.7.
 
 ```
 numpy==1.21.6
 scikit-learn==0.24.0
 joblib==1.0.0
 tqdm==4.55.0
 xlrd==2.0.1
 xlwt==1.3.0
 sonpy==1.7.5
 scipy==1.7.2
 ```
 
-Should one wish to upgrade these dependencies to the latest version of `scikit-learn`, change all references of `n_features_` to `n_features_in_` in `sleepens/sleepens/ml/_base_model.py`, `sleepens/sleepens/ml/models/_gb.py`, `sleepens/sleepens/ml/models/_tsens.py`, and `sleepens/sleepens/ml/models/_stsens.py`. Furthermore, change the loss parameter in `sleepens/sleepens/ml/_gb.py` line 220 to 'log_loss' (which replaces 'deviance' but is algorithmically the same). 
+Should one wish to upgrade these dependencies to the latest version of `scikit-learn`, change all references of `n_features_` to `n_features_in_` in the following:
+- `sleepens/sleepens/ml/_base_model.py`
+- `sleepens/sleepens/ml/models/_gb.py`
+- `sleepens/sleepens/ml/models/_tsens.py`
+- `sleepens/sleepens/ml/models/_stsens.py`
+
+Furthermore, change the loss parameter in `sleepens/sleepens/ml/_gb.py` line 220 to 'log_loss' (which replaces 'deviance' but is algorithmically the same). 
 
 ## Help and Support
 
 ### Documentation
 
 Documentation for `sleepens` can be found [here](https://github.com/paradoxysm/sleepens/tree/master/doc).
```

### Comparing `sleepens-1.0.2/setup.py` & `sleepens-1.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 	Build a file path from *paths* and return the contents.
 	"""
 	with open(os.path.join(*paths), 'r') as f:
 		return f.read()
 
 setup(
 	name='sleepens',
-	version='1.0.2',
+	version='1.0.3',
 	description='Sleep Classification using Ensemble Classification',
 	long_description=(read('README.md') + '\n\n'),
 	long_description_content_type="text/markdown",
 	url='http://github.com/paradoxysm/sleepens',
-	download_url = 'https://github.com/paradoxysm/sleepens/archive/1.0.2.tar.gz',
+	download_url = 'https://github.com/paradoxysm/sleepens/archive/1.0.3.tar.gz',
 	author='paradoxysm',
 	author_email='paradoxysm.dev@gmail.com',
 	license='BSD-3-Clause',
 	packages=find_packages(exclude=['tests']),
 	include_package_data=True,
 	install_requires=[
 		'numpy==1.21.6',
@@ -37,16 +37,14 @@
 		'Intended Audience :: Developers',
 		'Natural Language :: English',
 		'License :: OSI Approved :: BSD License',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
 		'Topic :: Software Development :: Libraries :: Python Modules',
 		'Topic :: Scientific/Engineering :: Artificial Intelligence',
 		'Topic :: Scientific/Engineering :: Information Analysis',
 		'Intended Audience :: Science/Research',
 	],
 	keywords=['python', 'ml', 'ensemble', 'sleep', 'classification'],
 	zip_safe=True)
```

### Comparing `sleepens-1.0.2/sleepens/analysis/_confusion_matrix.py` & `sleepens-1.0.3/sleepens/analysis/_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/analysis/_report.py` & `sleepens-1.0.3/sleepens/analysis/_report.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/io/_dataobject.py` & `sleepens-1.0.3/sleepens/io/_dataobject.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/io/_dataset.py` & `sleepens-1.0.3/sleepens/io/_dataset.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/io/interfaces/smrMAT.py` & `sleepens-1.0.3/sleepens/io/interfaces/smrMAT.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/io/interfaces/son.py` & `sleepens-1.0.3/sleepens/io/interfaces/son.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/io/interfaces/xls.py` & `sleepens-1.0.3/sleepens/io/interfaces/xls.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/main.py` & `sleepens-1.0.3/sleepens/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sleepens.ml import cross_validate
 from sleepens.analysis import confusion_matrix, classification_report
 from sleepens.io.interfaces import interfaces
 
 from sleepens.protocols import protocols
 from sleepens.protocols.sleepens4 import SleepEnsemble4
 
-version = "1.0.2"
+version = "1.0.3"
 model = SleepEnsemble4()
 verbose = 4
 
 def displayMenu():
 	print("-"*30)
 	print("Sleep Ensemble", version)
 	print("Current model:", model.name)
```

### Comparing `sleepens-1.0.2/sleepens/ml/_base_model.py` & `sleepens-1.0.3/sleepens/ml/_base_model.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/ml/_cv.py` & `sleepens-1.0.3/sleepens/ml/_cv.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/ml/models/_gb.py` & `sleepens-1.0.3/sleepens/ml/models/_gb.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/ml/models/_stsens.py` & `sleepens-1.0.3/sleepens/ml/models/_stsens.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/ml/models/_tsens.py` & `sleepens-1.0.3/sleepens/ml/models/_tsens.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_min_rem.py` & `sleepens-1.0.3/sleepens/postprocess/_min_rem.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_rem_drop.py` & `sleepens-1.0.3/sleepens/postprocess/_rem_drop.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_rem_sensitivity.py` & `sleepens-1.0.3/sleepens/postprocess/_rem_sensitivity.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_transition_fix.py` & `sleepens-1.0.3/sleepens/postprocess/_transition_fix.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_wake_max.py` & `sleepens-1.0.3/sleepens/postprocess/_wake_max.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_wake_sensitivity.py` & `sleepens-1.0.3/sleepens/postprocess/_wake_sensitivity.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/postprocess/_wake_to_rem.py` & `sleepens-1.0.3/sleepens/postprocess/_wake_to_rem.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/primary/_epoched_variance.py` & `sleepens-1.0.3/sleepens/process/primary/_epoched_variance.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/primary/_fft.py` & `sleepens-1.0.3/sleepens/process/primary/_fft.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/primary/_percentile_mean.py` & `sleepens-1.0.3/sleepens/process/primary/_percentile_mean.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/primary/_rms.py` & `sleepens-1.0.3/sleepens/process/primary/_rms.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/secondary/_merge.py` & `sleepens-1.0.3/sleepens/process/secondary/_merge.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/secondary/_ratio.py` & `sleepens-1.0.3/sleepens/process/secondary/_ratio.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/secondary/_spectral_band.py` & `sleepens-1.0.3/sleepens/process/secondary/_spectral_band.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/secondary/_spectral_entropy.py` & `sleepens-1.0.3/sleepens/process/secondary/_spectral_entropy.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/process/secondary/_transform.py` & `sleepens-1.0.3/sleepens/process/secondary/_transform.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/protocols/sleepens4/params.py` & `sleepens-1.0.3/sleepens/protocols/sleepens4/params.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/protocols/sleepens4/processor.py` & `sleepens-1.0.3/sleepens/protocols/sleepens4/processor.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/protocols/sleepens4/sleepens4.py` & `sleepens-1.0.3/sleepens/protocols/sleepens4/sleepens4.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/__init__.py` & `sleepens-1.0.3/sleepens/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/_calculate.py` & `sleepens-1.0.3/sleepens/utils/_calculate.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/_check.py` & `sleepens-1.0.3/sleepens/utils/_check.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/_data_mgmt.py` & `sleepens-1.0.3/sleepens/utils/_data_mgmt.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/_misc.py` & `sleepens-1.0.3/sleepens/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/_random.py` & `sleepens-1.0.3/sleepens/utils/_random.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/data/normalize.py` & `sleepens-1.0.3/sleepens/utils/data/normalize.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/data/sampling.py` & `sleepens-1.0.3/sleepens/utils/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/data/signal.py` & `sleepens-1.0.3/sleepens/utils/data/signal.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/data/smooth.py` & `sleepens-1.0.3/sleepens/utils/data/smooth.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens/utils/data/transform.py` & `sleepens-1.0.3/sleepens/utils/data/transform.py`

 * *Files identical despite different names*

### Comparing `sleepens-1.0.2/sleepens.egg-info/PKG-INFO` & `sleepens-1.0.3/sleepens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: sleepens
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sleep Classification using Ensemble Classification
 Home-page: http://github.com/paradoxysm/sleepens
 Author: paradoxysm
 Author-email: paradoxysm.dev@gmail.com
 License: BSD-3-Clause
-Download-URL: https://github.com/paradoxysm/sleepens/archive/1.0.2.tar.gz
+Download-URL: https://github.com/paradoxysm/sleepens/archive/1.0.3.tar.gz
 Keywords: python,ml,ensemble,sleep,classification
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.9, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,22 +29,22 @@
 
 [![CircleCI](https://img.shields.io/circleci/build/github/paradoxysm/sleepens?style=flat-square)](https://circleci.com/gh/paradoxysm/sleepens/tree/master)
 [![Codecov](https://flat.badgen.net/codecov/c/github/paradoxysm/sleepens?label=coverage&kill_cache=1)](https://codecov.io/gh/paradoxysm/sleepens)
 [![DOI](https://img.shields.io/badge/DOI-10.5821%2Fzenodo.7791521-blue?style=flat-square)](https://zenodo.org/badge/latestdoi/282098794)
 [![GitHub](https://img.shields.io/github/license/paradoxysm/sleepens?color=blue&style=flat-square)](https://github.com/paradoxysm/sleepens/blob/master/LICENSE)
 
 Sleep Ensemble is a framework for end-to-end sleep state classification using machine learning. It is designed to allow for modular data processing, classification, and further post-processing.
-Please see [here](https://academic.oup.com/sleep/advance-article-abstract/doi/10.1093/sleep/zsad101/7109541) for publication.
+Published in [SLEEP](https://academic.oup.com/sleep/advance-article-abstract/doi/10.1093/sleep/zsad101/7109541).
 
 ## Installation
 
 Install a suitable python environment from [python.org](https://www.python.org/downloads/release/python-378/).
-> Sleep Ensemble supports Python 3.7 to 3.9. It is extensively tested and developed with 64-bit Python 3.7.8 on Windows.
+> Sleep Ensemble supports Python 3.7 only. It is extensively tested and developed with 64-bit Python 3.7.8 on Windows.
 
-> Sleep Ensemble pre-trained builds are only useable for the specific OS and 32/64-bit Python environment. Its use may be possible with other Python 3.x versions but not guaranteed. The included pre-trained SleepEnsemble4 is built on 64-bit Python 3.7.8 on Windows.
+> Sleep Ensemble pre-trained builds are only useable for the specific OS and 32/64-bit Python environment. The included pre-trained SleepEnsemble4 is built on 64-bit Python 3.7.8 on Windows.
 
 Install the latest `sleepens` release using `pip` (on a terminal like command prompt):
 ```
 pip install sleepens
 ```
 Alternatively, download the source code for the latest release [here](https://github.com/paradoxysm/sleepens/releases). Unzip into desired location. Using the terminal, navigate to the top `sleepens` folder where `setup.py` is located and run the following:
 ```
@@ -102,28 +100,34 @@
 
 The underlying data processing pipelines and classification models are modular and can be adjusted to create different sleep ensemble models. `sleepens` currently contains one protocol, SleepEnsemble4, for 4-state sleep classification. New or modified protocols can be contributed to `sleepens.protocols` following the basic structure.
 
 Finally, `sleepens` uses `joblib` to store the pre-trained builds. This isn't the most secure method nor is the most data storage efficient. Ideally, a custom parameter export/load method is implemented that can reinstate a pre-trained build.
 
 ## Dependencies
 
-`sleepens` was developed using Python 3.7.8. Since development, `scikit-learn` has updated to a point that `sleepens` is not compatible with later versions of `scikit-learn` due to attribute name changes. At the same time, `sonpy` is limited to Python 3.7 to 3.9. For the sake of replicability (especially with pre-trained models provided on publication, the repository remains using the below dependencies at these versions.
+`sleepens` was developed using Python 3.7.8. Since development, `scikit-learn` has updated to a point that `sleepens` is not compatible with later versions of `scikit-learn` due to attribute name changes. At the same time, `sonpy` is limited to Python 3.7 to 3.9. For the sake of replicability (especially with pre-trained models provided on publication, the repository remains using the below dependencies at these versions. This also limits Python to 3.7.
 
 ```
 numpy==1.21.6
 scikit-learn==0.24.0
 joblib==1.0.0
 tqdm==4.55.0
 xlrd==2.0.1
 xlwt==1.3.0
 sonpy==1.7.5
 scipy==1.7.2
 ```
 
-Should one wish to upgrade these dependencies to the latest version of `scikit-learn`, change all references of `n_features_` to `n_features_in_` in `sleepens/sleepens/ml/_base_model.py`, `sleepens/sleepens/ml/models/_gb.py`, `sleepens/sleepens/ml/models/_tsens.py`, and `sleepens/sleepens/ml/models/_stsens.py`. Furthermore, change the loss parameter in `sleepens/sleepens/ml/_gb.py` line 220 to 'log_loss' (which replaces 'deviance' but is algorithmically the same). 
+Should one wish to upgrade these dependencies to the latest version of `scikit-learn`, change all references of `n_features_` to `n_features_in_` in the following:
+- `sleepens/sleepens/ml/_base_model.py`
+- `sleepens/sleepens/ml/models/_gb.py`
+- `sleepens/sleepens/ml/models/_tsens.py`
+- `sleepens/sleepens/ml/models/_stsens.py`
+
+Furthermore, change the loss parameter in `sleepens/sleepens/ml/_gb.py` line 220 to 'log_loss' (which replaces 'deviance' but is algorithmically the same). 
 
 ## Help and Support
 
 ### Documentation
 
 Documentation for `sleepens` can be found [here](https://github.com/paradoxysm/sleepens/tree/master/doc).
```

### Comparing `sleepens-1.0.2/sleepens.egg-info/SOURCES.txt` & `sleepens-1.0.3/sleepens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

