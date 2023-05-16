# Comparing `tmp/FiReTiTiPyLib-1.5.2.tar.gz` & `tmp/FiReTiTiPyLib-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiReTiTiPyLib-1.5.2.tar", last modified: Wed Oct  5 04:34:28 2022, max compression
+gzip compressed data, was "FiReTiTiPyLib-1.5.4.tar", last modified: Tue May 16 18:44:13 2023, max compression
```

## Comparing `FiReTiTiPyLib-1.5.2.tar` & `FiReTiTiPyLib-1.5.4.tar`

### file list

```diff
@@ -1,82 +1,87 @@
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.065534 FiReTiTiPyLib-1.5.2/
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.039013 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.043944 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/
--rw-r--r--   0 firetiti   (501) staff       (20)    17914 2022-08-03 21:19:30.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py
--rw-r--r--   0 firetiti   (501) staff       (20)     3812 2022-09-27 18:24:16.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py
--rwxrwxrwx   0 firetiti   (501) staff       (20)    18824 2022-07-07 20:30:57.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py
--rw-r--r--   0 firetiti   (501) staff       (20)      732 2021-07-08 18:41:36.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py
--rw-r--r--   0 firetiti   (501) staff       (20)        1 2021-09-17 15:36:01.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)    14803 2022-08-08 22:26:45.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Evaluations.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.048844 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/
--rw-r--r--   0 firetiti   (501) staff       (20)    10139 2022-07-26 20:37:56.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py
--rw-r--r--   0 firetiti   (501) staff       (20)     9876 2022-10-04 22:11:12.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py
--rw-r--r--   0 firetiti   (501) staff       (20)     9988 2021-09-19 21:12:09.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py
--rw-r--r--   0 firetiti   (501) staff       (20)    11378 2022-08-04 06:45:51.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py
--rw-r--r--   0 firetiti   (501) staff       (20)     7372 2022-07-06 23:57:34.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py
--rw-r--r--   0 firetiti   (501) staff       (20)     1534 2019-11-02 07:53:49.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py
--rw-r--r--   0 firetiti   (501) staff       (20)    33168 2022-07-19 19:11:17.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py
--rw-r--r--   0 firetiti   (501) staff       (20)      358 2022-07-17 08:41:02.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Transformations.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10581 2022-05-06 19:56:26.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py
--rw-r--r--   0 firetiti   (501) staff       (20)      660 2022-08-08 19:41:02.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.049752 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/IO/
--rw-r--r--   0 firetiti   (501) staff       (20)      218 2022-07-07 20:25:41.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/IO/IOColors.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-07-07 20:24:41.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/IO/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)    48611 2021-09-19 21:40:03.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/ImageDataGenerator.py
--rw-r--r--   0 firetiti   (501) staff       (20)      814 2019-12-06 21:57:12.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/ImageTools.py
--rw-r--r--   0 firetiti   (501) staff       (20)    11946 2022-07-16 07:19:08.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/ImagesIO.py
--rw-r--r--   0 firetiti   (501) staff       (20)     3964 2021-09-19 21:40:24.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Metrics.py
--rw-r--r--   0 firetiti   (501) staff       (20)     8885 2022-07-20 07:25:42.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Normalizers.py
--rw-r--r--   0 firetiti   (501) staff       (20)      418 2019-10-10 23:12:13.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Processing.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.050090 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.051553 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Attentions/
--rw-r--r--   0 firetiti   (501) staff       (20)     9202 2021-09-19 21:46:32.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10798 2020-10-01 00:31:32.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Attentions/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.054286 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)    19971 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py
--rw-r--r--   0 firetiti   (501) staff       (20)    16797 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py
--rw-r--r--   0 firetiti   (501) staff       (20)     4706 2022-05-06 19:39:13.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py
--rw-r--r--   0 firetiti   (501) staff       (20)     2434 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py
--rw-r--r--   0 firetiti   (501) staff       (20)     3000 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.057727 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)     6671 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py
--rw-r--r--   0 firetiti   (501) staff       (20)    13047 2022-07-20 18:25:21.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py
--rw-r--r--   0 firetiti   (501) staff       (20)     4802 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py
--rw-r--r--   0 firetiti   (501) staff       (20)      390 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/metrics.py
--rw-r--r--   0 firetiti   (501) staff       (20)     5006 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py
--rw-r--r--   0 firetiti   (501) staff       (20)      746 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.059270 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/
--rw-r--r--   0 firetiti   (501) staff       (20)     3386 2022-07-27 08:46:54.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py
--rw-r--r--   0 firetiti   (501) staff       (20)     4934 2022-07-02 09:22:02.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py
--rw-r--r--   0 firetiti   (501) staff       (20)      715 2022-07-27 08:35:58.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.060858 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/
--rw-r--r--   0 firetiti   (501) staff       (20)    21520 2022-07-30 00:39:38.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py
--rw-r--r--   0 firetiti   (501) staff       (20)    10192 2020-08-25 21:18:24.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.061869 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/ResUnetA/
--rw-r--r--   0 firetiti   (501) staff       (20)    24635 2021-09-19 21:19:22.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 21:18:29.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/ResUnetA/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.062733 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/SegNet/
--rw-r--r--   0 firetiti   (501) staff       (20)     4974 2019-02-11 00:12:15.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/SegNet/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.063518 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/U-Net/
--rw-r--r--   0 firetiti   (501) staff       (20)    14940 2021-09-19 21:23:45.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/U-Net/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)     1032 2022-08-08 19:48:59.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.064419 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Tests/
--rw-r--r--   0 firetiti   (501) staff       (20)    23945 2021-09-20 07:02:02.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Tests/UnitTests.py
--rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:55:38.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Tests/__init__.py
--rw-r--r--   0 firetiti   (501) staff       (20)     2849 2022-07-09 22:24:02.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Tools.py
--rw-r--r--   0 firetiti   (501) staff       (20)    16078 2022-07-17 08:40:20.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Transformations.py
--rw-r--r--   0 firetiti   (501) staff       (20)       49 2022-10-04 22:44:20.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/__init__.py
-drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2022-10-05 04:34:28.041223 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/
--rw-r--r--   0 firetiti   (501) staff       (20)     1588 2022-10-05 04:34:27.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/PKG-INFO
--rw-r--r--   0 firetiti   (501) staff       (20)     2978 2022-10-05 04:34:27.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/SOURCES.txt
--rw-r--r--   0 firetiti   (501) staff       (20)        1 2022-10-05 04:34:27.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/dependency_links.txt
--rw-r--r--   0 firetiti   (501) staff       (20)      441 2022-10-05 04:34:27.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/requires.txt
--rw-r--r--   0 firetiti   (501) staff       (20)       14 2022-10-05 04:34:27.000000 FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/top_level.txt
--rw-r--r--   0 firetiti   (501) staff       (20)     1588 2022-10-05 04:34:28.064949 FiReTiTiPyLib-1.5.2/PKG-INFO
--rw-r--r--   0 firetiti   (501) staff       (20)       38 2022-10-05 04:34:28.065743 FiReTiTiPyLib-1.5.2/setup.cfg
--rw-r--r--   0 firetiti   (501) staff       (20)     2909 2022-07-26 08:53:22.000000 FiReTiTiPyLib-1.5.2/setup.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.938201 FiReTiTiPyLib-1.5.4/
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.909472 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.913098 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/
+-rw-r--r--   0 firetiti   (501) staff       (20)    17914 2022-08-03 21:19:30.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     3812 2022-09-27 18:24:16.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py
+-rwxrwxrwx   0 firetiti   (501) staff       (20)    18871 2023-05-16 18:40:45.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      732 2021-07-08 18:41:36.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        1 2021-09-17 15:36:01.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    14803 2022-08-08 22:26:45.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Evaluations.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.918174 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/
+-rw-r--r--   0 firetiti   (501) staff       (20)    10215 2023-03-29 22:50:57.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     9876 2022-10-04 22:11:12.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10045 2023-03-29 22:52:23.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    11378 2022-08-04 06:45:51.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     7372 2022-07-06 23:57:34.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1534 2019-11-02 07:53:49.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    33168 2022-07-19 19:11:17.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      358 2022-07-17 08:41:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Transformations.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10581 2022-05-06 19:56:26.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      660 2022-08-08 19:41:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.919178 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/
+-rw-r--r--   0 firetiti   (501) staff       (20)     7242 2022-10-25 08:02:30.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/Graphics.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-10-22 06:51:36.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Graphics/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.920026 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/IO/
+-rw-r--r--   0 firetiti   (501) staff       (20)      218 2022-07-07 20:25:41.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/IO/IOColors.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-07-07 20:24:41.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/IO/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    48611 2021-09-19 21:40:03.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageDataGenerator.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1686 2023-03-25 03:02:08.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageTools.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    16489 2023-05-15 18:15:00.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImagesIO.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     3964 2021-09-19 21:40:24.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Metrics.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     8885 2022-07-20 07:25:42.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Normalizers.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      418 2019-10-10 23:12:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Processing.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.920931 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.922570 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/
+-rw-r--r--   0 firetiti   (501) staff       (20)     9202 2021-09-19 21:46:32.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10798 2020-10-01 00:31:32.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.926461 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    19971 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    16797 2022-05-06 19:38:51.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     4706 2022-05-06 19:39:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     2434 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     3000 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     5900 2023-01-19 23:42:50.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CoCo.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.930020 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     6671 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    13047 2022-07-20 18:25:21.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     4802 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      390 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/metrics.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     5006 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      746 2022-05-06 19:36:04.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.931410 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/
+-rw-r--r--   0 firetiti   (501) staff       (20)     3386 2022-07-27 08:46:54.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     4934 2022-07-02 09:22:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py
+-rw-r--r--   0 firetiti   (501) staff       (20)      715 2022-07-27 08:35:58.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.932998 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/
+-rw-r--r--   0 firetiti   (501) staff       (20)    21854 2023-04-14 16:18:56.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    10192 2020-08-25 21:18:24.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.933959 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/
+-rw-r--r--   0 firetiti   (501) staff       (20)    24635 2021-09-19 21:19:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 21:18:29.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.934842 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/
+-rw-r--r--   0 firetiti   (501) staff       (20)     4974 2019-02-11 00:12:15.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.935772 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/
+-rw-r--r--   0 firetiti   (501) staff       (20)    14940 2021-09-19 21:23:45.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:52:22.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1032 2022-08-08 19:48:59.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.937044 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/
+-rw-r--r--   0 firetiti   (501) staff       (20)    23945 2021-09-20 07:02:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/ApiTests.py
+-rw-r--r--   0 firetiti   (501) staff       (20)        0 2021-09-19 20:55:38.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/__init__.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     1896 2023-03-25 07:44:55.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/test_ImageTools.py
+-rw-r--r--   0 firetiti   (501) staff       (20)     2849 2022-07-09 22:24:02.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tools.py
+-rw-r--r--   0 firetiti   (501) staff       (20)    16078 2022-07-17 08:40:20.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Transformations.py
+-rw-r--r--   0 firetiti   (501) staff       (20)       49 2023-05-15 20:29:08.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/__init__.py
+drwxr-xr-x   0 firetiti   (501) staff       (20)        0 2023-05-16 18:44:13.911065 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/
+-rw-r--r--   0 firetiti   (501) staff       (20)     1588 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/PKG-INFO
+-rw-r--r--   0 firetiti   (501) staff       (20)     3123 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/SOURCES.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)        1 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/dependency_links.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)      422 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/requires.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)       14 2023-05-16 18:44:13.000000 FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/top_level.txt
+-rw-r--r--   0 firetiti   (501) staff       (20)     1588 2023-05-16 18:44:13.937734 FiReTiTiPyLib-1.5.4/PKG-INFO
+-rw-r--r--   0 firetiti   (501) staff       (20)       38 2023-05-16 18:44:13.938404 FiReTiTiPyLib-1.5.4/setup.cfg
+-rw-r--r--   0 firetiti   (501) staff       (20)     2934 2023-05-16 18:41:29.000000 FiReTiTiPyLib-1.5.4/setup.py
```

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_JavaInterfacer.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_MarkersExclusiveness.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,19 +238,19 @@
 				height, width = Target.shape
 				for image in ToTransform:
 					print("	 -> Transforming '%s'." % (inputdir + "/" + image))
 					imRaw = self._LoadImage(inputdir + "/" + image, True, False)[0]
 					#warped_img = cv2.warpPerspective(imRaw, H, (width, height), borderMode=cv2.BORDER_CONSTANT, borderValue=0)
 					order = 1
 					#if "_c1_" not in image: order = 0
-					warped_img = warp(imRaw, Hinv, output_shape=(height, width), order=order)
+					warped_img = warp(imRaw, Hinv, output_shape=(height, width), order=order, preserve_range=True)
 					imIO.Write(warped_img.astype(np.uint16), True, outputdir + "/" + image)
 					del imRaw
 					del warped_img
-		
+			#sys.exit(0)
 		gc.collect()
 		return True
 
 
 
 	def _LastChance(self, inputdir: str, Target, Image, toTransform: list, outputdir: str) -> bool:
 		if self.Debug:
@@ -343,18 +343,18 @@
 		else:
 			raise Exception("Unknow features detector. Expected {SIFT, ORB}")
 
 
 
 	def _LoadImage(self, path: str, raw: bool, preprocess: bool):
 		print("Reading '" + str(path) + "'... ", end='')
-		image = imIO.Read(path, True, verbose=False) # Image.open(dapis[0])
+		image = imIO.Read(path, Channel="First", verbose=False) # Image.open(dapis[0])
 		print(str(image.shape) + " successfully.")
 		sys.stdout.flush()
-
+		
 		channel, height, width = image.shape
 		#if self.Safety < channel or self.Safety < height or self.Safety < width:
 		#	raise Exception("Image too big. Max accepted = " + str(self.Safety))
 		
 		if self.Warning <= channel or self.Warning <= height or self.Warning <= width:
 			print("WARNING - Not recommended to register such big images as the processing will likely generate an "
 					+ "error with Java if the number of pixels is higher than 2^31. "
```

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/CyclicIF/CyclicIF_Utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Evaluations.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Evaluations.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,17 +259,18 @@
 				if nInputs == 3:
 					print(self.previous_filenames[x] + "   ", end='')
 				print(self.image_filenames[x] + "   " + self.next_filenames[x])
 	
 	
 	def __getitem__(self, index):
 		# Input triplets
-		previm = ImagesIO.Read(self.previous_filenames[index], verbose=False) if self.nInputs == 3 else None
-		image = ImagesIO.Read(self.image_filenames[index], verbose=False)
-		nextim = ImagesIO.Read(self.next_filenames[index], verbose=False)
+		previm = ImagesIO.Read(self.previous_filenames[index], Channel="First", verbose=False) if self.nInputs == 3\
+																								else None
+		image = ImagesIO.Read(self.image_filenames[index], Channel="First", verbose=False)
+		nextim = ImagesIO.Read(self.next_filenames[index], Channel="First", verbose=False)
 		
 		if self.normalizer is not None: # Let's normalize
 			if self.nInputs == 3:
 				self.normalizer.Normalize(previm)
 			self.normalizer.Normalize(image)
 			self.normalizer.Normalize(nextim)
```

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Denoiser.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations copie.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,57 +78,59 @@
 		for i in range(nbImages):
 			prefix = os.path.commonprefix([DetectionsPaths[i], ForegroundPaths[i]])
 			name = os.path.basename(prefix)
 			dash = "" if SaveImagesIn is None or SaveImagesIn.endswith("/") else " - "
 			path = None if SaveImagesIn is None else SaveImagesIn + dash + name
 			print("Evaluating '" + prefix + "'.")
 			
-			if SegmentationOnly == False: det = imIO.Read(DetectionsPaths[i], True, False)
-			seg = imIO.Read(ForegroundPaths[i], True, False)
-			gt = imIO.Read(GT[i], True, False)
+			if not SegmentationOnly:
+				det = imIO.Read(DetectionsPaths[i], Channel="First", verbose=False)
+			seg = imIO.Read(ForegroundPaths[i], Channel="First", verbose=False)
+			gt = imIO.Read(GT[i], Channel="First", verbose=False)
 			segGT = numpy.where(0 < gt, 255, 0)
 			
-			if SegmentationOnly == False:
-				SegAcc, SegSens, SegSpec, SegPrec, SegDice, DetAcc, DetSens, DetPrec = self.EvaluateImage(seg, segGT, det, gt,
-														Threshold=Threshold, Overlap=Overlap, SaveImagesAs=path, SegmentationOnly=SegmentationOnly)
+			if not SegmentationOnly:
+				SegAcc, SegSens, SegSpec, SegPrec, SegDice, DetAcc, DetSens, DetPrec =\
+						self.EvaluateImage(seg, segGT, det, gt, Threshold=Threshold, Overlap=Overlap, SaveImagesAs=path,
+											SegmentationOnly=SegmentationOnly)
 			else:
 				SegAcc, SegSens, SegSpec, SegPrec, SegDice = self.EvaluateImage(seg, segGT, None, gt,
-														Threshold=Threshold, Overlap=Overlap, SaveImagesAs=path, SegmentationOnly=SegmentationOnly)
+							Threshold=Threshold, Overlap=Overlap, SaveImagesAs=path, SegmentationOnly=SegmentationOnly)
 			
 			if SaveEvalutationsAs is not None:
-				if SegmentationOnly == False:
+				if not SegmentationOnly:
 					evaluations.append({"Image": name,
-									   "Segmentation_Accuracy": SegAcc,
-									   "Segmentation_Sensitivity/Recall": SegSens,
-									   "Segmentation_Specificity": SegSpec,
-									   "Segmentation_Precision": SegPrec,
-									   "Segmentation_Dice": SegDice,
-									   "Detection_Accuracy": DetAcc,
-									   "Detection_Sensitivity/Recall": DetSens,
-									   "Detection_Precision": DetPrec})
+										"Segmentation_Accuracy": SegAcc,
+										"Segmentation_Sensitivity/Recall": SegSens,
+										"Segmentation_Specificity": SegSpec,
+										"Segmentation_Precision": SegPrec,
+										"Segmentation_Dice": SegDice,
+										"Detection_Accuracy": DetAcc,
+										"Detection_Sensitivity/Recall": DetSens,
+										"Detection_Precision": DetPrec})
 				else:
 					evaluations.append({"Image": name,
 										"Segmentation_Accuracy": SegAcc,
 										"Segmentation_Sensitivity/Recall": SegSens,
 										"Segmentation_Specificity": SegSpec,
 										"Segmentation_Precision": SegPrec,
 										"Segmentation_Dice": SegDice})
 				SegSumAcc  += SegAcc
 				SegSumSens += SegSens
 				SegSumSpec += SegSpec
 				SegSumPrec += SegPrec
 				SegSumDice += SegDice
-				if SegmentationOnly == False:
+				if not SegmentationOnly:
 					DetSumAcc  += DetAcc
 					DetSumSens += DetSens
 					DetSumPrec += DetPrec
 
 		
 		if SaveEvalutationsAs is not None:
-			if SegmentationOnly == False:
+			if not SegmentationOnly:
 				evaluations.append({"Image": "Average",
 									"Segmentation_Accuracy": SegSumAcc / nbImages,
 									"Segmentation_Sensitivity/Recall": SegSumSens / nbImages,
 									"Segmentation_Specificity": SegSumSpec / nbImages,
 									"Segmentation_Precision": SegSumPrec / nbImages,
 									"Segmentation_Dice": SegSumDice / nbImages,
 									"Detection_Accuracy": DetSumAcc / nbImages,
@@ -141,15 +143,15 @@
 									"Segmentation_Specificity": SegSumSpec / nbImages,
 									"Segmentation_Precision": SegSumPrec / nbImages,
 									"Segmentation_Dice": SegSumDice / nbImages})
 			
 			results = pandas.DataFrame(evaluations)
 			results.set_index("Image", inplace=True)
 			
-			if SegmentationOnly == False:
+			if not SegmentationOnly:
 				results.rename(columns={"Segmentation_Accuracy" : "Segmentation Accuracy",
 										"Segmentation_Sensitivity/Recall" : "Segmentation Sensitivity/Recall",
 										"Segmentation_Specificity" : "Segmentation Specificity",
 										"Segmentation_Precision" : "Segmentation Precision",
 										"Segmentation_Dice" : "Segmentation Dice",
 										"Detection_Accuracy" : "Detection Accuracy",
 										"Detection_Sensitivity/Recall" : "Detection Sensitivity/Recall",
@@ -186,19 +188,21 @@
 	
 	def EvaluateImage(self, SegPred, SegGT, DetPred, DetGT, Threshold: int=128, Overlap: float=0.51, SaveImagesAs: str=None,
 					SegmentationOnly: bool=False):
 		""" This function evaluates the segmentation and prediction results.
 			Args:
 				SegPred: The predicted/output/segmented image.
 				SegGT: The segmentation ground truth image.
-				DegPred: The predicted/output/detections image.
+				DetPred: The predicted/output/detections image.
 				DetGT: The detections ground truth image.
 				Threshold (int): The threshold to determine positive vs negative areaa for the segmentation.
 				Overlap (float32): What is the minimum overlap to consider that a pattern was detected?
-				SaveImageAs (str): The entire path and prefix name to save the result images. If None, no result images saved.
+				SaveImagesAs (str): The entire path and prefix name to save the result images.
+					If None, no result images saved.
+				SegmentationOnly (bool):
 			Returns:
 				Segmentation returns, Detection returns
 		"""
 		SaveSegmentationImageAs = None if SaveImagesAs is None else SaveImagesAs + " - Segmentation.png"
 		SaveDetectionImageAs = None if SaveImagesAs is None else SaveImagesAs + " - Detection.png"
 		
 		Acc, Sensitivity, Specificity, Precision, Dice = self.Segmentation(SegPred, SegGT, Threshold=Threshold, SaveImageAs=SaveSegmentationImageAs)
@@ -214,15 +218,16 @@
 
 	def Segmentation(self, Prediction, GroundTruth, Threshold: int=128, SaveImageAs: str=None):
 		""" This function evaluates the segmentation result for a single given image.
 			Args:
 				Prediction: The predicted/output image.
 				GroundTruth: The ground truth image.
 				Threshold: The threshold to determine positive vs negative areaa.
-				SaveImageAs (str): The entire path and name to save the result image. The result image is generated only if this path is not None.
+				SaveImageAs (str): The entire path and name to save the result image. The result image is generated
+					only if this path is not None.
 			Returns:
 				Accuracy
 				Sensitivity/Recall
 				Specificity
 				Precision
 				Dice
 		"""
@@ -232,15 +237,16 @@
 	
 	def Detection(self, Prediction, GroundTruth, Overlap: float=0.51, SaveImageAs: str=None):
 		""" This function evaluates the detection results for a single given image.
 			Args:
 				Prediction: The predicted labels.
 				GroundTruth: The ground truth labels.
 				Overlap (float32): What is the minimum overlap to consider that a pattern was detected?
-				SaveImageAs (str): The entire path and name to save the result image. The result image is generated only if this path is not None.
+				SaveImageAs (str): The entire path and name to save the result image. The result image is generated
+					only if this path is not None.
 			Returns:
 				Accuracy
 				Sensitivity/Recall
 				Precision
 		"""
 		return Evaluations.Detection(Prediction, GroundTruth, Overlap, SaveImageAs)
```

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/ImageDataGenerator.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/ImageDataGenerator.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Metrics.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Metrics.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Normalizers.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Normalizers.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/head.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/loss.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CEECNET/utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/losses.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/main.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/mask_gen.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/smallunet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/CrossPseudoSupervision/utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/Denoising.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/NRRN.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/Denoising/__init__.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,24 @@
 																box_score_thresh=box_score_thresh,
 																box_nms_thresh=box_nms_thresh,
 																box_detections_per_img=box_detections_per_img,
 																box_fg_iou_thresh=box_fg_iou_thresh,
 																box_bg_iou_thresh=box_bg_iou_thresh,
 																box_batch_size_per_image=box_batch_size_per_image,
 																box_positive_fraction=box_positive_fraction)
-	
-	if Anchors == "Nuclei":
-		anchor_generator = AnchorGenerator(sizes=tuple([(16, 32, 64) for _ in range(5)]),
-											aspect_ratios=tuple([(0.5, 1.0, 1.5) for _ in range(5)]))
+	if Anchors is not None:
+		anchors = Anchors.lower()
+		if anchors == "nuclei":
+			anchor_generator = AnchorGenerator(sizes=tuple([(16, 32, 64) for _ in range(5)]),
+												aspect_ratios=tuple([(0.5, 1.0, 1.5) for _ in range(5)]))
+		elif anchors == "axons":
+			anchor_generator = AnchorGenerator(sizes=tuple([(32, 64, 128, 256) for _ in range(5)]),
+												aspect_ratios=tuple([(0.5, 1.0, 1.5) for _ in range(5)]))
+		else:
+			raise Exception("Unknown anchors: '" + Anchors + "'. Expected Nuclei or Axons.")
 		model.rpn.anchor_generator = anchor_generator
 		model.rpn.head = RPNHead(256, anchor_generator.num_anchors_per_location()[0])
 	
 	# get number of input features for the classifier
 	in_features = model.roi_heads.box_predictor.cls_score.in_features
 	# replace the pre-trained head with a new one
 	model.roi_heads.box_predictor = FastRCNNPredictor(in_features, nbClasses)
```

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/MaskRCNN/MaskRCNN_Utils.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/PyTorch_Models/__init__.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/PyTorch_Models/__init__.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Tests/UnitTests.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tests/ApiTests.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Tools.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Tools.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib/Transformations.py` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib/Transformations.py`

 * *Files identical despite different names*

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/PKG-INFO` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FiReTiTiPyLib
-Version: 1.5.2
+Version: 1.5.4
 Summary: Python libraries used as support/tools.
-Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.2.tar.gz
+Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.4.tar.gz
 Author: Guillaume THIBAULT
 Author-email: thibaulg@ohsu.org
 Maintainer: Guillaume THIBAULT
 Maintainer-email: thibaulg@ohsu.edu
 License: MIT
 Keywords: cyclic Immunofluorescence,cycif,immunofluorescence,registration,segmentation,features,features extraction,nuclei,nucleus,cells,cell,cell analysis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FiReTiTiPyLib-1.5.2/FiReTiTiPyLib.egg-info/SOURCES.txt` & `FiReTiTiPyLib-1.5.4/FiReTiTiPyLib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Evaluations.py
 FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Losses.py
 FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Schedulers.py
 FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Segmentator.py
 FiReTiTiPyLib/FiReTiTiPyTorchLib/FiReTiTiPyTorchLib_Transformations.py
 FiReTiTiPyLib/FiReTiTiPyTorchLib/Segmentation_Datasets.py
 FiReTiTiPyLib/FiReTiTiPyTorchLib/__init__.py
+FiReTiTiPyLib/Graphics/Graphics.py
+FiReTiTiPyLib/Graphics/__init__.py
 FiReTiTiPyLib/IO/IOColors.py
 FiReTiTiPyLib/IO/__init__.py
+FiReTiTiPyLib/PyTorch_Models/CoCo.py
 FiReTiTiPyLib/PyTorch_Models/__init__.py
 FiReTiTiPyLib/PyTorch_Models/Attentions/Attentions.py
 FiReTiTiPyLib/PyTorch_Models/Attentions/NonLocalBlock.py
 FiReTiTiPyLib/PyTorch_Models/Attentions/__init__.py
 FiReTiTiPyLib/PyTorch_Models/CEECNET/__init__.py
 FiReTiTiPyLib/PyTorch_Models/CEECNET/blocks.py
 FiReTiTiPyLib/PyTorch_Models/CEECNET/ceecnet.py
@@ -56,9 +59,10 @@
 FiReTiTiPyLib/PyTorch_Models/MaskRCNN/__init__.py
 FiReTiTiPyLib/PyTorch_Models/ResUnetA/ResUnetA.py
 FiReTiTiPyLib/PyTorch_Models/ResUnetA/__init__.py
 FiReTiTiPyLib/PyTorch_Models/SegNet/SegNet.py
 FiReTiTiPyLib/PyTorch_Models/SegNet/__init__.py
 FiReTiTiPyLib/PyTorch_Models/U-Net/UNet.py
 FiReTiTiPyLib/PyTorch_Models/U-Net/__init__.py
-FiReTiTiPyLib/Tests/UnitTests.py
-FiReTiTiPyLib/Tests/__init__.py
+FiReTiTiPyLib/Tests/ApiTests.py
+FiReTiTiPyLib/Tests/__init__.py
+FiReTiTiPyLib/Tests/test_ImageTools.py
```

### Comparing `FiReTiTiPyLib-1.5.2/PKG-INFO` & `FiReTiTiPyLib-1.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FiReTiTiPyLib
-Version: 1.5.2
+Version: 1.5.4
 Summary: Python libraries used as support/tools.
-Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.2.tar.gz
+Download-URL: https://www.thibault.biz/Doc/FiReTiTiPyLib/FiReTiTiPyLib-1.5.4.tar.gz
 Author: Guillaume THIBAULT
 Author-email: thibaulg@ohsu.org
 Maintainer: Guillaume THIBAULT
 Maintainer-email: thibaulg@ohsu.edu
 License: MIT
 Keywords: cyclic Immunofluorescence,cycif,immunofluorescence,registration,segmentation,features,features extraction,nuclei,nucleus,cells,cell,cell analysis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FiReTiTiPyLib-1.5.2/setup.py` & `FiReTiTiPyLib-1.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,20 @@
 						"opencv-contrib-python-headless>=4.5.5",
 						"opencv-python-headless>=4.5.5",
 						"pandas>=1.2.4",
 						"Pillow>=8.2.0",
 						"psutil>=5.8.0",
 						"qtconsole>=5.1.0",
 						"QtPy>=1.9.0",
-						"scikit-image>=0.18.3,<0.19",
+						"scikit-image>=0.18.3",#"scikit-image>=0.18.3,<0.19",
 						"scikit-learn>=0.24.2",
 						"scipy>=1.6.3",
 						"seaborn>=0.11.1",
 						#"six>=1.15.0",
-						"sklearn>=0.0",
+						#"sklearn>=0.0",
 						"spams>=2.6.2.5",
 						"tifffile>=2021.4.8",
 						"torch",
 						"torchvision>=0.8.2",
 						"tornado>=6.1",
 						"wheel>=0.37.0"],
 	python_requires=">=3.8,<3.10",
```

