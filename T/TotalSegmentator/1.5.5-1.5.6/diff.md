# Comparing `tmp/TotalSegmentator-1.5.5.tar.gz` & `tmp/TotalSegmentator-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TotalSegmentator-1.5.5.tar", last modified: Wed Mar 29 15:38:08 2023, max compression
+gzip compressed data, was "dist/TotalSegmentator-1.5.6.tar", last modified: Tue May 16 14:04:08 2023, max compression
```

## Comparing `TotalSegmentator-1.5.5.tar` & `TotalSegmentator-1.5.6.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/
--rw-rw-r--   0 jakob     (1000) jakob     (1000)      565 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)    12818 2023-03-27 11:47:06.000000 TotalSegmentator-1.5.5/README.md
-drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/
--rw-rw-r--   0 jakob     (1000) jakob     (1000)      565 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/PKG-INFO
--rw-rw-r--   0 jakob     (1000) jakob     (1000)      880 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/SOURCES.txt
--rw-rw-r--   0 jakob     (1000) jakob     (1000)        1 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/dependency_links.txt
--rw-rw-r--   0 jakob     (1000) jakob     (1000)        1 2023-03-28 11:14:37.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/not-zip-safe
--rw-rw-r--   0 jakob     (1000) jakob     (1000)      138 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/requires.txt
--rw-rw-r--   0 jakob     (1000) jakob     (1000)       17 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/TotalSegmentator.egg-info/top_level.txt
-drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/bin/
--rw-rw-r--   0 jakob     (1000) jakob     (1000)     4960 2023-03-21 07:31:59.000000 TotalSegmentator-1.5.5/bin/TotalSegmentator
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3350 2023-03-22 14:10:31.000000 TotalSegmentator-1.5.5/bin/crop_to_body
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1799 2023-01-13 12:01:14.000000 TotalSegmentator-1.5.5/bin/totalseg_combine_masks
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1287 2023-03-28 11:43:02.000000 TotalSegmentator-1.5.5/bin/totalseg_download_weights
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1547 2023-03-21 07:45:59.000000 TotalSegmentator-1.5.5/bin/totalseg_import_weights
--rw-rw-r--   0 jakob     (1000) jakob     (1000)       38 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/setup.cfg
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1597 2023-03-29 15:37:34.000000 TotalSegmentator-1.5.5/setup.py
-drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-03-29 15:38:08.000000 TotalSegmentator-1.5.5/totalsegmentator/
--rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.5/totalsegmentator/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1447 2022-11-09 15:47:21.000000 TotalSegmentator-1.5.5/totalsegmentator/alignment.py
--rw-rw-r--   0 jakob     (1000) jakob     (1000)     3517 2023-03-29 15:32:11.000000 TotalSegmentator-1.5.5/totalsegmentator/config.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4910 2022-11-17 09:55:18.000000 TotalSegmentator-1.5.5/totalsegmentator/cropping.py
--rw-rw-r--   0 jakob     (1000) jakob     (1000)     3413 2023-03-17 08:42:38.000000 TotalSegmentator-1.5.5/totalsegmentator/dicom_io.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      262 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.5/totalsegmentator/download_pretrained_weights.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    12494 2023-03-22 13:35:04.000000 TotalSegmentator-1.5.5/totalsegmentator/libs.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    15859 2023-03-21 08:33:04.000000 TotalSegmentator-1.5.5/totalsegmentator/map_to_binary.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2840 2022-11-28 16:10:29.000000 TotalSegmentator-1.5.5/totalsegmentator/nifti_ext_header.py
--rw-rw-r--   0 jakob     (1000) jakob     (1000)    21697 2023-03-28 11:16:08.000000 TotalSegmentator-1.5.5/totalsegmentator/nnunet.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3131 2023-03-14 09:04:24.000000 TotalSegmentator-1.5.5/totalsegmentator/postprocessing.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     7211 2023-03-21 08:45:31.000000 TotalSegmentator-1.5.5/totalsegmentator/preview.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     9341 2023-03-29 14:42:51.000000 TotalSegmentator-1.5.5/totalsegmentator/python_api.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     9020 2023-02-13 12:30:29.000000 TotalSegmentator-1.5.5/totalsegmentator/resampling.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6478 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.5/totalsegmentator/statistics.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6126 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.5/totalsegmentator/vtk_utils.py
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)      565 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    13393 2023-04-03 14:41:05.000000 TotalSegmentator-1.5.6/README.md
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)      565 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/PKG-INFO
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)      908 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/SOURCES.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        1 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/dependency_links.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)        1 2023-03-28 11:14:37.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/not-zip-safe
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)      146 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/requires.txt
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)       17 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/TotalSegmentator.egg-info/top_level.txt
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/bin/
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     5117 2023-04-14 07:55:01.000000 TotalSegmentator-1.5.6/bin/TotalSegmentator
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3350 2023-03-22 14:10:31.000000 TotalSegmentator-1.5.6/bin/crop_to_body
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1799 2023-01-13 12:01:14.000000 TotalSegmentator-1.5.6/bin/totalseg_combine_masks
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1287 2023-03-28 11:43:02.000000 TotalSegmentator-1.5.6/bin/totalseg_download_weights
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1547 2023-03-21 07:45:59.000000 TotalSegmentator-1.5.6/bin/totalseg_import_weights
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      994 2023-03-31 11:51:32.000000 TotalSegmentator-1.5.6/bin/totalseg_setup_manually
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)       38 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/setup.cfg
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2082 2023-05-16 14:03:21.000000 TotalSegmentator-1.5.6/setup.py
+drwxrwxr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-16 14:04:08.000000 TotalSegmentator-1.5.6/totalsegmentator/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.6/totalsegmentator/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1447 2022-11-09 15:47:21.000000 TotalSegmentator-1.5.6/totalsegmentator/alignment.py
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     3569 2023-03-31 11:49:30.000000 TotalSegmentator-1.5.6/totalsegmentator/config.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4910 2022-11-17 09:55:18.000000 TotalSegmentator-1.5.6/totalsegmentator/cropping.py
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)     4383 2023-04-21 07:59:32.000000 TotalSegmentator-1.5.6/totalsegmentator/dicom_io.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      262 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.6/totalsegmentator/download_pretrained_weights.py
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)    13364 2023-04-14 12:49:15.000000 TotalSegmentator-1.5.6/totalsegmentator/libs.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    16041 2023-04-24 11:34:35.000000 TotalSegmentator-1.5.6/totalsegmentator/map_to_binary.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     2840 2022-11-28 16:10:29.000000 TotalSegmentator-1.5.6/totalsegmentator/nifti_ext_header.py
+-rw-rw-r--   0 jakob     (1000) jakob     (1000)    22548 2023-04-14 07:52:37.000000 TotalSegmentator-1.5.6/totalsegmentator/nnunet.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     3131 2023-03-14 09:04:24.000000 TotalSegmentator-1.5.6/totalsegmentator/postprocessing.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     7211 2023-03-21 08:45:31.000000 TotalSegmentator-1.5.6/totalsegmentator/preview.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     9607 2023-05-08 12:20:26.000000 TotalSegmentator-1.5.6/totalsegmentator/python_api.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     9100 2023-04-14 07:42:13.000000 TotalSegmentator-1.5.6/totalsegmentator/resampling.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6609 2023-03-31 14:24:39.000000 TotalSegmentator-1.5.6/totalsegmentator/statistics.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6126 2022-11-09 15:45:55.000000 TotalSegmentator-1.5.6/totalsegmentator/vtk_utils.py
```

### Comparing `TotalSegmentator-1.5.5/PKG-INFO` & `TotalSegmentator-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: TotalSegmentator
-Version: 1.5.5
+Version: 1.5.6
 Summary: Robust segmentation of 104 classes in CT images.
 Home-page: https://github.com/wasserth/TotalSegmentator
 Author: Jakob Wasserthal
 Author-email: jakob.wasserthal@usb.ch
 License: Apache 2.0
 Description: See Readme.md on github for more details.
 Platform: UNKNOWN
```

### Comparing `TotalSegmentator-1.5.5/README.md` & `TotalSegmentator-1.5.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,42 +11,45 @@
 ### Installation
 
 TotalSegmentator works on Ubuntu, Mac and Windows and on CPU and GPU (on CPU it is slow).
 
 Install dependencies:  
 * Python >= 3.7
 * [Pytorch](http://pytorch.org/)
-* if you use the option `--preview` you have to install xvfb (`apt-get install xvfb`)
 * You should not have any nnU-Net installation in your python environment since TotalSegmentator will install its own custom installation.
 
-* optionally: for faster resampling you can use `cucim` (`pip install cupy-cuda11x cucim`)
+optionally:
+* if you input DICOM images and run on MacOS you have to install [dcm2niix](https://github.com/rordenlab/dcm2niix)
+* if you use the option `--preview` you have to install xvfb (`apt-get install xvfb`)
+* for faster resampling you can use `cucim` (`pip install cupy-cuda11x cucim`)
+
 
 Install Totalsegmentator
 ```
 pip install TotalSegmentator
 ```
 
 
 ### Usage
 ```
 TotalSegmentator -i ct.nii.gz -o segmentations
 ```
-> Note: A Nifti file or a folder of Dicom images is allowed as input
+> Note: A Nifti file or a folder of DICOM images is allowed as input
 
 > Note: If a CUDA compatible GPU is available TotalSegmentator will automatically use it. Otherwise it will use the CPU, which is a lot slower and should only be used with the `--fast` option.  
 
 > Note: You can also try it online: [www.totalsegmentator.com](https://totalsegmentator.com/) (supports dicom files)
 
 > Note: This is not a medical device and not intended for clinical usage.
 
 
 ### Advanced settings
 * `--fast`: For faster runtime and less memory requirements use this option. It will run a lower resolution model (3mm instead of 1.5mm). 
 * `--preview`: This will generate a 3D rendering of all classes, giving you a quick overview if the segmentation worked and where it failed (see `preview.png` in output directory).
-* `--ml`: This will save one nifti file containing all labels instead of one file for each class. Saves runtime during saving of nifti files.
+* `--ml`: This will save one nifti file containing all labels instead of one file for each class. Saves runtime during saving of nifti files. (see [here](https://github.com/wasserth/TotalSegmentator#class-details) for index to class name mapping).
 * `--roi_subset`: Takes a space separated list of class names (e.g. `spleen colon brain`) and only saves those classes. Saves runtime during saving of nifti files.
 * `--statistics`: This will generate a file `statistics.json` with volume (in mm³) and mean intensity of each class.
 * `--radiomics`: This will generate a file `statistics_radiomics.json` with radiomics features of each class. You have to install pyradiomics to use this (`pip install pyradiomics`).
  
 
 ### Subtasks
 
@@ -164,128 +167,113 @@
 ### Class details
 
 The following table shows a list of all classes.
 
 TA2 is a standardised way to name anatomy. Mostly the TotalSegmentator names follow this standard. 
 For some classes they differ which you can see in the table below.
 
-|TotalSegmentator name|TA2 name|
-|:-----|:-----|
-spleen ||
-kidney_right ||
-kidney_left ||
-gallbladder ||
-liver ||
-stomach ||
-aorta ||
-inferior_vena_cava ||
-portal_vein_and_splenic_vein | hepatic portal vein |
-pancreas ||
-adrenal_gland_right | suprarenal gland |
-adrenal_gland_left | suprarenal gland |
-lung_upper_lobe_left | superior lobe of left lung |
-lung_lower_lobe_left | inferior lobe of left lung |
-lung_upper_lobe_right | superior lobe of right lung |
-lung_middle_lobe_right | middle lobe of right lung |
-lung_lower_lobe_right | inferior lobe of right lung |
-vertebrae_L5 ||
-vertebrae_L4 ||
-vertebrae_L3 ||
-vertebrae_L2 ||
-vertebrae_L1 ||
-vertebrae_T12 ||
-vertebrae_T11 ||
-vertebrae_T10 ||
-vertebrae_T9 ||
-vertebrae_T8 ||
-vertebrae_T7 ||
-vertebrae_T6 ||
-vertebrae_T5 ||
-vertebrae_T4 ||
-vertebrae_T3 ||
-vertebrae_T2 ||
-vertebrae_T1 ||
-vertebrae_C7 ||
-vertebrae_C6 ||
-vertebrae_C5 ||
-vertebrae_C4 ||
-vertebrae_C3 ||
-vertebrae_C2 ||
-vertebrae_C1 ||
-esophagus ||
-trachea ||
-heart_myocardium ||
-heart_atrium_left ||
-heart_ventricle_left ||
-heart_atrium_right ||
-heart_ventricle_right ||
-pulmonary_artery | pulmonary arteries |
-brain ||
-iliac_artery_left | common iliac artery |
-iliac_artery_right | common iliac artery |
-iliac_vena_left | common iliac vein |
-iliac_vena_right | common iliac vein |
-small_bowel | small intestine |
-duodenum ||
-colon ||
-rib_left_1 ||
-rib_left_2 ||
-rib_left_3 ||
-rib_left_4 ||
-rib_left_5 ||
-rib_left_6 ||
-rib_left_7 ||
-rib_left_8 ||
-rib_left_9 ||
-rib_left_10 ||
-rib_left_11 ||
-rib_left_12 ||
-rib_right_1 ||
-rib_right_2 ||
-rib_right_3 ||
-rib_right_4 ||
-rib_right_5 ||
-rib_right_6 ||
-rib_right_7 ||
-rib_right_8 ||
-rib_right_9 ||
-rib_right_10 ||
-rib_right_11 ||
-rib_right_12 ||
-scapula_left ||
-scapula_right ||
-clavicula_left | clavicle |
-clavicula_right | clavicle |
-hip_left | hip bone |
-hip_right | hip bone |
-sacrum ||
-face ||
-gluteus_maximus_left | gluteus maximus muscle |
-gluteus_maximus_right | gluteus maximus muscle |
-gluteus_medius_left | gluteus medius muscle |
-gluteus_medius_right | gluteus medius muscle |
-gluteus_minimus_left | gluteus minimus muscle |
-gluteus_minimus_right | gluteus minimus muscle |
-autochthon_left ||
-autochthon_right ||
-iliopsoas_left | iliopsoas muscle |
-iliopsoas_right | iliopsoas muscle |
-urinary_bladder ||
-femur ||
-patella ||
-tibia ||
-fibula ||
-tarsal ||
-metatarsal ||
-phalanges_feet ||
-humerus ||
-ulna ||
-radius ||
-carpal ||
-metacarpal ||
-phalanges_hand ||
-sternum ||
-skull ||
-subcutaneous_fat ||
-skeletal_muscle ||
-torso_fat ||
-spinal_cord ||
+|Index|TotalSegmentator name|TA2 name|
+|:-----|:-----|:-----|
+1 | spleen ||
+2 | kidney_right ||
+3 | kidney_left ||
+4 | gallbladder ||
+5 | liver ||
+6 | stomach ||
+7 | aorta ||
+8 | inferior_vena_cava ||
+9 | portal_vein_and_splenic_vein | hepatic portal vein |
+10 | pancreas ||
+11 | adrenal_gland_right | suprarenal gland |
+12 | adrenal_gland_left | suprarenal gland |
+13 | lung_upper_lobe_left | superior lobe of left lung |
+14 | lung_lower_lobe_left | inferior lobe of left lung |
+15 | lung_upper_lobe_right | superior lobe of right lung |
+16 | lung_middle_lobe_right | middle lobe of right lung |
+17 | lung_lower_lobe_right | inferior lobe of right lung |
+18 | vertebrae_L5 ||
+19 | vertebrae_L4 ||
+20 | vertebrae_L3 ||
+21 | vertebrae_L2 ||
+22 | vertebrae_L1 ||
+23 | vertebrae_T12 ||
+24 | vertebrae_T11 ||
+25 | vertebrae_T10 ||
+26 | vertebrae_T9 ||
+27 | vertebrae_T8 ||
+28 | vertebrae_T7 ||
+29 | vertebrae_T6 ||
+30 | vertebrae_T5 ||
+31 | vertebrae_T4 ||
+32 | vertebrae_T3 ||
+33 | vertebrae_T2 ||
+34 | vertebrae_T1 ||
+35 | vertebrae_C7 ||
+36 | vertebrae_C6 ||
+37 | vertebrae_C5 ||
+38 | vertebrae_C4 ||
+39 | vertebrae_C3 ||
+40 | vertebrae_C2 ||
+41 | vertebrae_C1 ||
+42 | esophagus ||
+43 | trachea ||
+44 | heart_myocardium ||
+45 | heart_atrium_left ||
+46 | heart_ventricle_left ||
+47 | heart_atrium_right ||
+48 | heart_ventricle_right ||
+49 | pulmonary_artery | pulmonary arteries |
+50 | brain ||
+51 | iliac_artery_left | common iliac artery |
+52 | iliac_artery_right | common iliac artery |
+53 | iliac_vena_left | common iliac vein |
+54 | iliac_vena_right | common iliac vein |
+55 | small_bowel | small intestine |
+56 | duodenum ||
+57 | colon ||
+58 | rib_left_1 ||
+59 | rib_left_2 ||
+60 | rib_left_3 ||
+61 | rib_left_4 ||
+62 | rib_left_5 ||
+63 | rib_left_6 ||
+64 | rib_left_7 ||
+65 | rib_left_8 ||
+66 | rib_left_9 ||
+67 | rib_left_10 ||
+68 | rib_left_11 ||
+69 | rib_left_12 ||
+70 | rib_right_1 ||
+71 | rib_right_2 ||
+72 | rib_right_3 ||
+73 | rib_right_4 ||
+74 | rib_right_5 ||
+75 | rib_right_6 ||
+76 | rib_right_7 ||
+77 | rib_right_8 ||
+78 | rib_right_9 ||
+79 | rib_right_10 ||
+80 | rib_right_11 ||
+81 | rib_right_12 ||
+82 | humerus left ||
+83 | humerus right ||
+84 | scapula_left ||
+85 | scapula_right ||
+86 | clavicula_left | clavicle |
+87 | clavicula_right | clavicle |
+88 | femur left ||
+89 | femur right ||
+90 | hip_left | hip bone |
+91 | hip_right | hip bone |
+92 | sacrum ||
+93 | face ||
+94 | gluteus_maximus_left | gluteus maximus muscle |
+95 | gluteus_maximus_right | gluteus maximus muscle |
+96 | gluteus_medius_left | gluteus medius muscle |
+97 | gluteus_medius_right | gluteus medius muscle |
+98 | gluteus_minimus_left | gluteus minimus muscle |
+99 | gluteus_minimus_right | gluteus minimus muscle |
+100 | autochthon_left ||
+101 | autochthon_right ||
+102 | iliopsoas_left | iliopsoas muscle |
+103 | iliopsoas_right | iliopsoas muscle |
+104 | urinary_bladder ||
```

### Comparing `TotalSegmentator-1.5.5/TotalSegmentator.egg-info/PKG-INFO` & `TotalSegmentator-1.5.6/TotalSegmentator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: TotalSegmentator
-Version: 1.5.5
+Version: 1.5.6
 Summary: Robust segmentation of 104 classes in CT images.
 Home-page: https://github.com/wasserth/TotalSegmentator
 Author: Jakob Wasserthal
 Author-email: jakob.wasserthal@usb.ch
 License: Apache 2.0
 Description: See Readme.md on github for more details.
 Platform: UNKNOWN
```

### Comparing `TotalSegmentator-1.5.5/TotalSegmentator.egg-info/SOURCES.txt` & `TotalSegmentator-1.5.6/TotalSegmentator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 TotalSegmentator.egg-info/requires.txt
 TotalSegmentator.egg-info/top_level.txt
 bin/TotalSegmentator
 bin/crop_to_body
 bin/totalseg_combine_masks
 bin/totalseg_download_weights
 bin/totalseg_import_weights
+bin/totalseg_setup_manually
 totalsegmentator/__init__.py
 totalsegmentator/alignment.py
 totalsegmentator/config.py
 totalsegmentator/cropping.py
 totalsegmentator/dicom_io.py
 totalsegmentator/download_pretrained_weights.py
 totalsegmentator/libs.py
```

### Comparing `TotalSegmentator-1.5.5/bin/TotalSegmentator` & `TotalSegmentator-1.5.6/bin/TotalSegmentator`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,20 @@
 
     parser.add_argument("-q", "--quiet", action="store_true", help="Print no intermediate outputs",
                         default=False)
 
     parser.add_argument("-v", "--verbose", action="store_true", help="Show more intermediate output",
                         default=False)
 
-    parser.add_argument("--test", metavar="0|1|2|3", choices=[0, 1, 2, 3], type=int,
+    # Tests:
+    # 0: no testing behaviour activated
+    # 1: total normal
+    # 2: total fast -> removed because can run normally with cpu
+    # 3: lung_vessels
+    parser.add_argument("--test", metavar="0|1|3", choices=[0, 1, 3], type=int,
                         help="Only needed for unittesting.",
                         default=0)
 
     parser.add_argument('--version', action='version', version=require("TotalSegmentator")[0].version)
 
     args = parser.parse_args()
```

### Comparing `TotalSegmentator-1.5.5/bin/crop_to_body` & `TotalSegmentator-1.5.6/bin/crop_to_body`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/bin/totalseg_combine_masks` & `TotalSegmentator-1.5.6/bin/totalseg_combine_masks`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/bin/totalseg_download_weights` & `TotalSegmentator-1.5.6/bin/totalseg_download_weights`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/bin/totalseg_import_weights` & `TotalSegmentator-1.5.6/bin/totalseg_import_weights`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/setup.py` & `TotalSegmentator-1.5.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+import sys
 from setuptools import setup, find_packages
 
+if sys.version_info < (3, 10):
+    # Specify the fixed version for Python < 3.10. Because using the latest
+    # requests would also install the latest urllib3 which does not work
+    # properly on python < 3.10.
+    requests_version = '==2.27.1'  #requires: urllib3>=1.21.1,<1.27 
+    # 2.27.1 somehow not available in dockerfile
+else:
+    requests_version = ''  # No fixed version for Python 3.10 and higher
+
+
 setup(name='TotalSegmentator',
-        version='1.5.5',
+        version='1.5.6',
         description='Robust segmentation of 104 classes in CT images.',
         long_description="See Readme.md on github for more details.",
         url='https://github.com/wasserth/TotalSegmentator',
         author='Jakob Wasserthal',
         author_email='jakob.wasserthal@usb.ch',
         python_requires='>=3.5',
         license='Apache 2.0',
@@ -21,23 +32,24 @@
             'p_tqdm',
             'xvfbwrapper',
             'fury',
             'batchgenerators==0.21',
             # This does not work if want to upload to pypi
             # 'nnunet @ git+https://github.com/wasserth/nnUNet_cust@working_2022_03_18#egg=nnUNet'
             'nnunet-customized==1.2',
-            'requests',
+            f'requests{requests_version}',
             'rt_utils'
         ],
         zip_safe=False,
         classifiers=[
             'Intended Audience :: Science/Research',
             'Programming Language :: Python',
             'Topic :: Scientific/Engineering',
             'Operating System :: Unix',
             'Operating System :: MacOS'
         ],
         scripts=[
             'bin/TotalSegmentator', 'bin/totalseg_combine_masks', 'bin/crop_to_body', 
-            'bin/totalseg_import_weights', 'bin/totalseg_download_weights'
+            'bin/totalseg_import_weights', 'bin/totalseg_download_weights',
+            'bin/totalseg_setup_manually'
         ]
     )
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/alignment.py` & `TotalSegmentator-1.5.6/totalsegmentator/alignment.py`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/config.py` & `TotalSegmentator-1.5.6/totalsegmentator/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,24 +23,25 @@
     # This variables will only be active during the python script execution. Therefore
     # we do not have to unset them in the end.
     os.environ["nnUNet_raw_data_base"] = str(weights_dir)  # not needed, just needs to be an existing directory
     os.environ["nnUNet_preprocessed"] = str(weights_dir)  # not needed, just needs to be an existing directory
     os.environ["RESULTS_FOLDER"] = str(weights_dir)
 
 
-def setup_totalseg():
+def setup_totalseg(totalseg_id=None):
     home_path = Path("/tmp") if str(Path.home()) == "/" else Path.home()
     totalseg_path = home_path / ".totalsegmentator"
     totalseg_path.mkdir(exist_ok=True)
     totalseg_config_file = totalseg_path / "config.json"
 
     if totalseg_config_file.exists():
         config = json.load(open(totalseg_config_file, "r"))
     else:
-        totalseg_id = "totalseg_" + ''.join(random.Random().choices(string.ascii_uppercase + string.digits, k=8))
+        if totalseg_id is None:
+            totalseg_id = "totalseg_" + ''.join(random.Random().choices(string.ascii_uppercase + string.digits, k=8))
         config = {
             "totalseg_id": totalseg_id,
             "send_usage_stats": True,
             "prediction_counter": 0
         }
         json.dump(config, open(totalseg_config_file, "w"), indent=4)
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/cropping.py` & `TotalSegmentator-1.5.6/totalsegmentator/cropping.py`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/dicom_io.py` & `TotalSegmentator-1.5.6/totalsegmentator/dicom_io.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,25 +10,33 @@
 
 import numpy as np
 import nibabel as nib
 
 from totalsegmentator.libs import get_config_dir
 
 
+
+def command_exists(command):
+    return shutil.which(command) is not None
+
+
 def download_dcm2niix():
     import urllib.request
     print("  Downloading dcm2niix...")
 
     if platform.system() == "Windows":
         url = "https://github.com/rordenlab/dcm2niix/releases/latest/download/dcm2niix_win.zip"
     elif platform.system() == "Darwin":  # Mac
-        if platform.machine().startswith("arm") or platform.machine().startswith("aarch"):  # arm
-            url = "https://github.com/rordenlab/dcm2niix/releases/latest/download/dcm2niix_mac_arm.pkg"
-        else:  # intel
-            url = "https://github.com/rordenlab/dcm2niix/releases/latest/download/dcm2niix_mac.zip"
+        raise ValueError("For MacOS automatic installation of dcm2niix not possible. Install it manually.")
+        # Problem: not zip files
+        # if platform.machine().startswith("arm") or platform.machine().startswith("aarch"):  # arm
+        #     url = "https://github.com/rordenlab/dcm2niix/releases/latest/download/macos_dcm2niix.pkg"
+        # else:  # intel
+        #     # unclear if this is the right link (is the same as for arm)
+        #     url = "https://github.com/rordenlab/dcm2niix/releases/latest/download/macos_dcm2niix.pkg"
     elif platform.system() == "Linux":
         url = "https://github.com/rordenlab/dcm2niix/releases/latest/download/dcm2niix_lnx.zip"
     else:
         raise ValueError("Unknown operating system. Can not download the right version of dcm2niix.")
 
     config_dir = get_config_dir()
 
@@ -48,22 +56,39 @@
     """
     input_path: a directory of dicom slices
     output_path: a nifti file path
     """
     verbose_str = "" if verbose else "> /dev/null"
 
     config_dir = get_config_dir()
-    dcm2niix = config_dir / "dcm2niix"
 
-    if not dcm2niix.exists():
-        download_dcm2niix()
+    if command_exists("dcm2niix"):
+        dcm2niix = "dcm2niix"
+    else:
+        if platform.system() == "Windows":
+            dcm2niix = config_dir / "dcm2niix.exe"
+        else:
+            dcm2niix = config_dir / "dcm2niix"
+        if not dcm2niix.exists():
+            download_dcm2niix()
 
     subprocess.call(f"{dcm2niix} -o {output_path.parent} -z y -f {output_path.name[:-7]} {input_path} {verbose_str}", shell=True)
 
     nii_files = list(output_path.parent.glob("*.nii.gz"))
+
+    if len(nii_files) > 1:
+        print("WARNING: Dicom to nifti resulted in several nifti files. Skipping files which contain ROI in filename.")
+        for nii_file in nii_files:
+            # output file name is "converted_dcm.nii.gz" so if ROI in name, then this can be deleted
+            if "ROI" in nii_file.name:
+                os.remove(nii_file)
+                print(f"Skipped: {nii_file.name}")
+
+    nii_files = list(output_path.parent.glob("*.nii.gz"))
+
     if len(nii_files) > 1:
         print("WARNING: Dicom to nifti resulted in several nifti files. Only using first one.")
         print([f.name for f in nii_files])
         for nii_file in nii_files[1:]:
             os.remove(nii_file)
         # todo: have to rename first file to not contain any counter which is automatically added by dcm2niix
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/libs.py` & `TotalSegmentator-1.5.6/totalsegmentator/libs.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,23 @@
 #     r = requests.get(url, stream=True)
 #     with open(save_path, 'wb') as f:
 #         for chunk in r.iter_content(chunk_size=chunk_size):
 #             f.write(chunk)
 
 
 def download_url_and_unpack(url, config_dir):
-    import http.client
-    # helps to solve incomplete read erros
-    # https://stackoverflow.com/questions/37816596/restrict-request-to-only-ask-for-http-1-0-to-prevent-chunking-error
-    http.client.HTTPConnection._http_vsn = 10
-    http.client.HTTPConnection._http_vsn_str = 'HTTP/1.0'
+
+    if "TOTALSEG_DISABLE_HTTP1" in os.environ and os.environ["TOTALSEG_DISABLE_HTTP1"]:
+        print("Disabling HTTP/1.0")
+    else:
+        import http.client
+        # helps to solve incomplete read erros
+        # https://stackoverflow.com/questions/37816596/restrict-request-to-only-ask-for-http-1-0-to-prevent-chunking-error
+        http.client.HTTPConnection._http_vsn = 10
+        http.client.HTTPConnection._http_vsn_str = 'HTTP/1.0'
 
     tempfile = config_dir / "tmp_download_file.zip"
 
     try:
         st = time.time()
         with open(tempfile, 'wb') as f:
             # session = requests.Session()  # making it slower
@@ -95,35 +99,41 @@
     old_weights = [
         "Task223_my_test"
     ]
 
     if task_id == 251:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task251_TotalSegmentator_part1_organs_1139subj"
-        WEIGHTS_URL = "https://zenodo.org/record/6802342/files/Task251_TotalSegmentator_part1_organs_1139subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/6802342/files/Task251_TotalSegmentator_part1_organs_1139subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task251_TotalSegmentator_part1_organs_1139subj.zip"
     elif task_id == 252:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task252_TotalSegmentator_part2_vertebrae_1139subj"
-        WEIGHTS_URL = "https://zenodo.org/record/6802358/files/Task252_TotalSegmentator_part2_vertebrae_1139subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/6802358/files/Task252_TotalSegmentator_part2_vertebrae_1139subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task252_TotalSegmentator_part2_vertebrae_1139subj.zip"
     elif task_id == 253:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task253_TotalSegmentator_part3_cardiac_1139subj"
-        WEIGHTS_URL = "https://zenodo.org/record/6802360/files/Task253_TotalSegmentator_part3_cardiac_1139subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/6802360/files/Task253_TotalSegmentator_part3_cardiac_1139subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task253_TotalSegmentator_part3_cardiac_1139subj.zip"
     elif task_id == 254:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task254_TotalSegmentator_part4_muscles_1139subj"
-        WEIGHTS_URL = "https://zenodo.org/record/6802366/files/Task254_TotalSegmentator_part4_muscles_1139subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/6802366/files/Task254_TotalSegmentator_part4_muscles_1139subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task254_TotalSegmentator_part4_muscles_1139subj.zip"
     elif task_id == 255:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task255_TotalSegmentator_part5_ribs_1139subj"
-        WEIGHTS_URL = "https://zenodo.org/record/6802452/files/Task255_TotalSegmentator_part5_ribs_1139subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/6802452/files/Task255_TotalSegmentator_part5_ribs_1139subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task255_TotalSegmentator_part5_ribs_1139subj.zip"
     elif task_id == 256:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task256_TotalSegmentator_3mm_1139subj"
-        WEIGHTS_URL = "https://zenodo.org/record/6802052/files/Task256_TotalSegmentator_3mm_1139subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/6802052/files/Task256_TotalSegmentator_3mm_1139subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task256_TotalSegmentator_3mm_1139subj.zip"
     elif task_id == 258:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task258_lung_vessels_248subj"
         WEIGHTS_URL = "https://zenodo.org/record/7064718/files/Task258_lung_vessels_248subj.zip?download=1"
     elif task_id == 200:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task200_covid_challenge"
@@ -143,15 +153,16 @@
     elif task_id == 260:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task260_hip_implant_71subj"
         WEIGHTS_URL = "https://zenodo.org/record/7234263/files/Task260_hip_implant_71subj.zip?download=1"
     elif task_id == 269:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task269_Body_extrem_6mm_1200subj"
-        WEIGHTS_URL = "https://zenodo.org/record/7334272/files/Task269_Body_extrem_6mm_1200subj.zip?download=1"
+        # WEIGHTS_URL = "https://zenodo.org/record/7334272/files/Task269_Body_extrem_6mm_1200subj.zip?download=1"
+        WEIGHTS_URL = "http://94.16.105.223/static/Task269_Body_extrem_6mm_1200subj.zip"
     elif task_id == 503:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task503_cardiac_motion"
         WEIGHTS_URL = "https://zenodo.org/record/7271576/files/Task503_cardiac_motion.zip?download=1"
     elif task_id == 273:
         config_dir = config_dir / "3d_fullres"
         weights_path = config_dir / "Task273_Body_extrem_1259subj"
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/map_to_binary.py` & `TotalSegmentator-1.5.6/totalsegmentator/map_to_binary.py`

 * *Files 3% similar despite different names*

```diff
@@ -487,34 +487,35 @@
         17: "gluteus_minimus_right",
         18: "autochthon_left",
         19: "autochthon_right",
         20: "iliopsoas_left",
         21: "iliopsoas_right"
     },
 
+    # --roi_subset does not work anymore with this
     # without humerus and femur
-    "class_map_part_muscles_v2": {
-        1: "scapula_left",
-        2: "scapula_right",
-        3: "clavicula_left",
-        4: "clavicula_right",
-        5: "hip_left",
-        6: "hip_right",
-        7: "sacrum",
-        8: "gluteus_maximus_left",
-        9: "gluteus_maximus_right",
-        10: "gluteus_medius_left",
-        11: "gluteus_medius_right",
-        12: "gluteus_minimus_left",
-        13: "gluteus_minimus_right",
-        14: "autochthon_left",
-        15: "autochthon_right",
-        16: "iliopsoas_left",
-        17: "iliopsoas_right"
-    },
+    # "class_map_part_muscles_v2": {
+    #     1: "scapula_left",
+    #     2: "scapula_right",
+    #     3: "clavicula_left",
+    #     4: "clavicula_right",
+    #     5: "hip_left",
+    #     6: "hip_right",
+    #     7: "sacrum",
+    #     8: "gluteus_maximus_left",
+    #     9: "gluteus_maximus_right",
+    #     10: "gluteus_medius_left",
+    #     11: "gluteus_medius_right",
+    #     12: "gluteus_minimus_left",
+    #     13: "gluteus_minimus_right",
+    #     14: "autochthon_left",
+    #     15: "autochthon_right",
+    #     16: "iliopsoas_left",
+    #     17: "iliopsoas_right"
+    # },
 
     # 24 classes
     # 12. ribs start from vertebrae T12
     # Small subset of population (roughly 8%) have 13. rib below 12. rib
     #  (would start from L1 then)
     #  -> this has label rib_12
     # Even smaller subset (roughly 1%) has extra rib above 1. rib   ("Halsrippe")
@@ -546,35 +547,36 @@
         20: "rib_right_8",
         21: "rib_right_9",
         22: "rib_right_10",
         23: "rib_right_11",
         24: "rib_right_12"
     },
 
-    "class_map_part_bones" : {
-        1: "femur",
-        2: "patella",
-        3: "tibia",
-        4: "fibula",
-        5: "tarsal",
-        6: "metatarsal",
-        7: "phalanges_feet",
-        8: "humerus",
-        9: "ulna",
-        10: "radius",
-        11: "carpal",
-        12: "metacarpal",
-        13: "phalanges_hand",
-        14: "sternum",
-        15: "skull",
-        16: "subcutaneous_fat",
-        17: "skeletal_muscle",
-        18: "torso_fat",
-        19: "spinal_cord"
-    },
+    # --roi_subset does not work anymore with this
+    # "class_map_part_bones" : {
+    #     1: "femur",
+    #     2: "patella",
+    #     3: "tibia",
+    #     4: "fibula",
+    #     5: "tarsal",
+    #     6: "metatarsal",
+    #     7: "phalanges_feet",
+    #     8: "humerus",
+    #     9: "ulna",
+    #     10: "radius",
+    #     11: "carpal",
+    #     12: "metacarpal",
+    #     13: "phalanges_hand",
+    #     14: "sternum",
+    #     15: "skull",
+    #     16: "subcutaneous_fat",
+    #     17: "skeletal_muscle",
+    #     18: "torso_fat",
+    #     19: "spinal_cord"
+    # },
 
     "test": class_map["test"]
 }
 
 
 map_taskid_to_partname = {
     251: "class_map_part_organs",
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/nifti_ext_header.py` & `TotalSegmentator-1.5.6/totalsegmentator/nifti_ext_header.py`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/nnunet.py` & `TotalSegmentator-1.5.6/totalsegmentator/nnunet.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from totalsegmentator.resampling import change_spacing
 from totalsegmentator.libs import combine_masks, compress_nifti, check_if_shape_and_affine_identical
 from totalsegmentator.dicom_io import dcm_to_nifti, save_mask_as_rtstruct
 from totalsegmentator.cropping import crop_to_mask_nifti, undo_crop_nifti
 from totalsegmentator.cropping import crop_to_mask, undo_crop
 from totalsegmentator.postprocessing import remove_outside_of_mask, extract_skin
 from totalsegmentator.nifti_ext_header import save_multilabel_nifti
+from totalsegmentator.statistics import get_basic_statistics_for_entire_dir
 
 
 def _get_full_task_name(task_id: int, src: str="raw"):
     if src == "raw":
         base = Path(os.environ['nnUNet_raw_data_base']) / "nnUNet_raw_data"
     elif src == "preprocessed":
         base = Path(os.environ['nnUNet_preprocessed'])
@@ -134,15 +135,15 @@
 
 
 def nnUNet_predict_image(file_in, file_out, task_id, model="3d_fullres", folds=None,
                          trainer="nnUNetTrainerV2", tta=False, multilabel_image=True, 
                          resample=None, crop=None, crop_path=None, task_name="total", nora_tag="None", preview=False, 
                          save_binary=False, nr_threads_resampling=1, nr_threads_saving=6, force_split=False,
                          crop_addon=[3,3,3], roi_subset=None, output_type="nifti", 
-                         quiet=False, verbose=False, test=0):
+                         statistics=False, quiet=False, verbose=False, test=0):
     """
     crop: string or a nibabel image
     resample: None or float  (target spacing for all dimensions)
     """
     file_in = Path(file_in)
     if file_out is not None:
         file_out = Path(file_out)
@@ -276,15 +277,15 @@
                 for img_part in img_parts:
                     nib.save(nib.Nifti1Image(seg_combined[img_part], img_in_rsp.affine), tmp_dir / f"{img_part}.nii.gz")
             elif test == 1:
                 print("WARNING: Using reference seg instead of prediction for testing.")
                 shutil.copy(Path("tests") / "reference_files" / "example_seg.nii.gz", tmp_dir / f"s01.nii.gz")
         else:
             if not quiet: print(f"Predicting...")
-            if test == 0 or test == 2:
+            if test == 0:
                 with nostdout(verbose):
                     nnUNet_predict(tmp_dir, tmp_dir, task_id, model, folds, trainer, tta,
                                    nr_threads_resampling, nr_threads_saving)
             # elif test == 2:
             #     print("WARNING: Using reference seg instead of prediction for testing.")
             #     shutil.copy(Path("tests") / "reference_files" / "example_seg_fast.nii.gz", tmp_dir / f"s01.nii.gz")
             elif test == 3:
@@ -308,14 +309,29 @@
             if not quiet: print("Generating preview...")
             st = time.time()
             smoothing = 20
             preview_dir = file_out.parent if multilabel_image else file_out
             generate_preview(img_in_rsp, preview_dir / f"preview_{task_name}.png", img_pred.get_fdata(), smoothing, task_name)
             if not quiet: print("  Generated in {:.2f}s".format(time.time() - st))
 
+        # Statistics calculated on the 3mm downsampled image are very similar to statistics
+        # calculated on the original image. Volume often completely identical. For intensity
+        # some more change but still minor.
+        #
+        # Speed: 
+        # stats on 1.5mm: 37s
+        # stats on 3.0mm: 4s    -> great improvement
+        if statistics:
+            if not quiet: print("Calculating statistics fast...")
+            st = time.time()
+            stats_dir = file_out.parent if multilabel_image else file_out
+            stats_dir.mkdir(exist_ok=True)
+            get_basic_statistics_for_entire_dir(img_pred.get_fdata(), img_in_rsp, stats_dir / "statistics.json", quiet)
+            if not quiet: print(f"  calculated in {time.time()-st:.2f}s")
+
         if resample is not None:
             if not quiet: print("Resampling...")
             if verbose: print(f"  back to original shape: {img_in_shape}")    
             # Use force_affine otherwise output affine sometimes slightly off (which then is even increased
             # by undo_canonical)
             img_pred = change_spacing(img_pred, [resample, resample, resample], img_in_shape,
                                         order=0, dtype=np.uint8, nr_cpus=nr_threads_resampling,
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/postprocessing.py` & `TotalSegmentator-1.5.6/totalsegmentator/postprocessing.py`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/preview.py` & `TotalSegmentator-1.5.6/totalsegmentator/preview.py`

 * *Files identical despite different names*

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/python_api.py` & `TotalSegmentator-1.5.6/totalsegmentator/python_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
     For explanation of the arguments see description of command line 
     arguments in bin/TotalSegmentator.
     """
     input = Path(input)
     output = Path(output)
 
+    nora_tag = "None" if nora_tag is None else nora_tag
+
     if not quiet: 
         print("\nIf you use this tool please cite: https://doi.org/10.48550/arXiv.2208.05868\n")
 
     if not torch.cuda.is_available():
         print("No GPU detected. Running on CPU. This can be very slow. The '--fast' option can help to some extend.")
 
     setup_nnunet()
@@ -165,14 +167,21 @@
         trainer = "nnUNetTrainerV2"
         crop = "body"
         model = "3d_fullres"
         folds = [0]
 
     crop_path = output if crop_path is None else crop_path
 
+    # fast statistics are calculated on the downsampled image
+    if statistics and fast:
+        statistics_fast = True  
+        statistics = False
+    else:
+        statistics_fast = False
+
     if type(task_id) is list:
         for tid in task_id:
             download_pretrained_weights(tid)
     else:
         download_pretrained_weights(task_id)
 
     # Generate rough body segmentation (speedup for big images; not useful in combination with --fast option)
@@ -180,47 +189,46 @@
         download_pretrained_weights(269)
         st = time.time()
         if not quiet: print("Generating rough body segmentation...")
         body_seg = nnUNet_predict_image(input, None, 269, model="3d_fullres", folds=[0],
                             trainer="nnUNetTrainerV2", tta=False, multilabel_image=True, resample=6.0,
                             crop=None, crop_path=None, task_name="body", nora_tag="None", preview=False, 
                             save_binary=True, nr_threads_resampling=nr_thr_resamp, nr_threads_saving=1, 
-                            crop_addon=crop_addon, output_type=output_type, quiet=quiet, 
-                            verbose=verbose, test=0)
+                            crop_addon=crop_addon, output_type=output_type, statistics=False,
+                            quiet=quiet, verbose=verbose, test=0)
         crop = body_seg
         if verbose: print(f"Rough body segmentation generated in {time.time()-st:.2f}s")
 
     folds = [0]  # None
     seg_img = nnUNet_predict_image(input, output, task_id, model=model, folds=folds,
                          trainer=trainer, tta=False, multilabel_image=ml, resample=resample,
                          crop=crop, crop_path=crop_path, task_name=task, nora_tag=nora_tag, preview=preview, 
                          nr_threads_resampling=nr_thr_resamp, nr_threads_saving=nr_thr_saving, 
                          force_split=force_split, crop_addon=crop_addon, roi_subset=roi_subset,
-                         output_type=output_type, quiet=quiet, verbose=verbose, test=test)
-    if verbose: print("Predict returned...")
+                         output_type=output_type, statistics=statistics_fast, 
+                         quiet=quiet, verbose=verbose, test=test)
     seg = seg_img.get_fdata().astype(np.uint8)
 
-    if verbose: print("Setting up config...")
     config = setup_totalseg()
-    if verbose: print("Increasing counter...")
     increase_prediction_counter()
-    if verbose: print("Sending stats...")
     send_usage_stats(config, {"task": task, "fast": fast, "preview": preview,
                               "multilabel": ml, "roi_subset": roi_subset, 
                               "statistics": statistics, "radiomics": radiomics})
 
     if statistics:
         if not quiet: print("Calculating statistics...")
         st = time.time()
         stats_dir = output.parent if ml else output
         get_basic_statistics_for_entire_dir(seg, input, stats_dir / "statistics.json", quiet)
         # get_radiomics_features_for_entire_dir(input, output, output / "statistics_radiomics.json")
         if not quiet: print(f"  calculated in {time.time()-st:.2f}s")
 
     if radiomics:
+        if ml:
+            raise ValueError("Radiomics not supported for multilabel segmentation. Use without --ml option.")
         if not quiet: print("Calculating radiomics...")  
         st = time.time()
         stats_dir = output.parent if ml else output
         get_radiomics_features_for_entire_dir(input, output, stats_dir / "statistics_radiomics.json")
         if not quiet: print(f"  calculated in {time.time()-st:.2f}s")
 
     return seg_img
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/resampling.py` & `TotalSegmentator-1.5.6/totalsegmentator/resampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 def resample_img_cucim(img, zoom=0.5, order=0, nr_cpus=-1):
     """
     Completely speedup of resampling compare to non-gpu version not as big, because much time is lost in 
     loading the file and then in copying to the GPU.
 
     For small image no significant speedup.
     For large images reducing resampling time by over 50%.
+
+    On our slurm gpu cluster it is actually slower with cucim than without it.
     """
     import cupy as cp
     from cucim.skimage.transform import resize
 
     img = cp.asarray(img)  # slow
     new_shape = (np.array(img.shape) * zoom).round().astype(np.int32)
     resampled_img = resize(img, output_shape=new_shape, order=order, mode="edge", anti_aliasing=False)  # very fast
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/statistics.py` & `TotalSegmentator-1.5.6/totalsegmentator/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pathlib
 from pathlib import Path
 import json
 from functools import partial
 import time
 
 import numpy as np
 import pandas as pd
@@ -58,16 +59,19 @@
     stats = p_map(partial(get_radiomics_features, img_file=ct_file),
                     masks, num_cpus=1, disable=False)
     stats = {mask_name: stats for mask_name, stats in stats}
     with open(file_out, "w") as f:
         json.dump(stats, f, indent=4)
 
 
-def get_basic_statistics_for_entire_dir(seg: np.array, ct_file:Path, file_out:Path, quiet:bool=False):
-    ct_img = nib.load(ct_file)
+def get_basic_statistics_for_entire_dir(seg: np.array, ct_file, file_out:Path, quiet:bool=False):
+    """
+    ct_file: path to a ct_file or a nifti file object
+    """
+    ct_img = nib.load(ct_file) if type(ct_file) == pathlib.PosixPath else ct_file
     ct = ct_img.get_fdata()
     spacing = ct_img.header.get_zooms()
     vox_vol = spacing[0] * spacing[1] * spacing[2]
     stats = {}
     for k, mask_name in tqdm(class_map["total"].items(), disable=quiet):
         stats[mask_name] = {}
         # data = nib.load(mask).get_fdata()  # loading: 0.6s
```

### Comparing `TotalSegmentator-1.5.5/totalsegmentator/vtk_utils.py` & `TotalSegmentator-1.5.6/totalsegmentator/vtk_utils.py`

 * *Files identical despite different names*

