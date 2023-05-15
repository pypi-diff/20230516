# Comparing `tmp/hifi-5.0.0-py3.9.egg` & `tmp/hifi-6.0.0-py3.9.egg`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 83781 bytes, number of entries: 40
--rw-r--r--  2.0 unx     5145 b- defN 23-May-15 18:55 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      941 b- defN 23-May-15 18:55 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:55 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx     1519 b- defN 23-May-15 18:55 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-15 18:55 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:55 EGG-INFO/zip-safe
--rwxr-xr-x  2.0 unx     3192 b- defN 23-May-15 18:55 EGG-INFO/scripts/hifi
--rwxr-xr-x  2.0 unx     1538 b- defN 23-May-15 18:55 EGG-INFO/scripts/visbeats
+Zip file size: 210760 bytes, number of entries: 74
+-rw-r--r--  2.0 unx     5145 b- defN 23-May-15 19:03 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx     1222 b- defN 23-May-15 19:03 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 19:03 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 19:03 EGG-INFO/not-zip-safe
+-rw-r--r--  2.0 unx     1519 b- defN 23-May-15 19:03 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-15 19:03 EGG-INFO/top_level.txt
+-rwxr-xr-x  2.0 unx     3164 b- defN 23-May-15 19:03 EGG-INFO/scripts/hifi
+-rwxr-xr-x  2.0 unx     1510 b- defN 23-May-15 19:03 EGG-INFO/scripts/visbeats
 -rw-r--r--  2.0 unx    18598 b- defN 23-May-09 13:44 visbeats/__init__.py
 -rw-r--r--  2.0 unx       28 b- defN 23-May-09 07:48 visbeats/adefines.py
 -rw-r--r--  2.0 unx     7472 b- defN 23-May-09 08:40 visbeats/afilemanager.py
 -rw-r--r--  2.0 unx     4294 b- defN 23-May-09 08:40 visbeats/afuncdict.py
 -rw-r--r--  2.0 unx     5176 b- defN 23-May-09 08:40 visbeats/aimports.py
 -rw-r--r--  2.0 unx     4748 b- defN 23-May-09 09:29 visbeats/aobject.py
 -rw-r--r--  2.0 unx     3894 b- defN 23-May-09 08:41 visbeats/aparamdict.py
@@ -31,12 +31,46 @@
 -rw-r--r--  2.0 unx     3348 b- defN 23-May-09 08:42 visbeats/videoclip.py
 -rw-r--r--  2.0 unx    30746 b- defN 23-May-09 08:42 visbeats/videosource.py
 -rw-r--r--  2.0 unx       84 b- defN 23-May-09 07:54 visbeats/visbeatdefines.py
 -rw-r--r--  2.0 unx     5193 b- defN 23-May-09 08:26 visbeats/visbeatexamplevideo.py
 -rw-r--r--  2.0 unx     3676 b- defN 23-May-09 08:43 visbeats/visbeatimports.py
 -rw-r--r--  2.0 unx    10811 b- defN 23-May-09 08:43 visbeats/visualbeat.py
 -rw-r--r--  2.0 unx    28403 b- defN 23-May-09 09:38 visbeats/warp.py
+-rw-r--r--  2.0 unx    11483 b- defN 23-May-15 19:03 visbeats/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx      161 b- defN 23-May-15 19:03 visbeats/__pycache__/adefines.cpython-39.pyc
+-rw-r--r--  2.0 unx     6285 b- defN 23-May-15 19:03 visbeats/__pycache__/afilemanager.cpython-39.pyc
+-rw-r--r--  2.0 unx     4546 b- defN 23-May-15 19:03 visbeats/__pycache__/afuncdict.cpython-39.pyc
+-rw-r--r--  2.0 unx     6559 b- defN 23-May-15 19:03 visbeats/__pycache__/aimports.cpython-39.pyc
+-rw-r--r--  2.0 unx     4852 b- defN 23-May-15 19:03 visbeats/__pycache__/aobject.cpython-39.pyc
+-rw-r--r--  2.0 unx     4570 b- defN 23-May-15 19:03 visbeats/__pycache__/aparamdict.cpython-39.pyc
+-rw-r--r--  2.0 unx    23481 b- defN 23-May-15 19:03 visbeats/__pycache__/audio.cpython-39.pyc
+-rw-r--r--  2.0 unx     2347 b- defN 23-May-15 19:03 visbeats/__pycache__/audioclip.cpython-39.pyc
+-rw-r--r--  2.0 unx    17124 b- defN 23-May-15 19:03 visbeats/__pycache__/event.cpython-39.pyc
+-rw-r--r--  2.0 unx     5473 b- defN 23-May-15 19:03 visbeats/__pycache__/eventlist.cpython-39.pyc
+-rw-r--r--  2.0 unx    14460 b- defN 23-May-15 19:03 visbeats/__pycache__/image.cpython-39.pyc
+-rw-r--r--  2.0 unx     4180 b- defN 23-May-15 19:03 visbeats/__pycache__/image_cv.cpython-39.pyc
+-rw-r--r--  2.0 unx     1193 b- defN 23-May-15 19:03 visbeats/__pycache__/mediafiles.cpython-39.pyc
+-rw-r--r--  2.0 unx     6790 b- defN 23-May-15 19:03 visbeats/__pycache__/sourcelocationparser.cpython-39.pyc
+-rw-r--r--  2.0 unx     2442 b- defN 23-May-15 19:03 visbeats/__pycache__/timesignal.cpython-39.pyc
+-rw-r--r--  2.0 unx     2798 b- defN 23-May-15 19:03 visbeats/__pycache__/timesignal1d.cpython-39.pyc
+-rw-r--r--  2.0 unx     4815 b- defN 23-May-15 19:03 visbeats/__pycache__/vbmidi.cpython-39.pyc
+-rw-r--r--  2.0 unx     4981 b- defN 23-May-15 19:03 visbeats/__pycache__/vbobject.cpython-39.pyc
+-rw-r--r--  2.0 unx    24722 b- defN 23-May-15 19:03 visbeats/__pycache__/video.cpython-39.pyc
+-rw-r--r--  2.0 unx    23147 b- defN 23-May-15 19:03 visbeats/__pycache__/video_cv.cpython-39.pyc
+-rw-r--r--  2.0 unx     3345 b- defN 23-May-15 19:03 visbeats/__pycache__/videoclip.cpython-39.pyc
+-rw-r--r--  2.0 unx    18100 b- defN 23-May-15 19:03 visbeats/__pycache__/videosource.cpython-39.pyc
+-rw-r--r--  2.0 unx      245 b- defN 23-May-15 19:03 visbeats/__pycache__/visbeatdefines.cpython-39.pyc
+-rw-r--r--  2.0 unx     6213 b- defN 23-May-15 19:03 visbeats/__pycache__/visbeatexamplevideo.cpython-39.pyc
+-rw-r--r--  2.0 unx     3231 b- defN 23-May-15 19:03 visbeats/__pycache__/visbeatimports.cpython-39.pyc
+-rw-r--r--  2.0 unx     7690 b- defN 23-May-15 19:03 visbeats/__pycache__/visualbeat.cpython-39.pyc
+-rw-r--r--  2.0 unx    16843 b- defN 23-May-15 19:03 visbeats/__pycache__/warp.cpython-39.pyc
+-rw-rw-r--  2.0 unx    15866 b- defN 19-Jan-03 19:37 visbeats/assets/audio/hit.wav
+-rw-rw-r--  2.0 unx    40461 b- defN 23-May-10 01:08 visbeats/assets/images/VisBeatWatermark.png
 -rw-r--r--  2.0 unx     1435 b- defN 23-May-09 07:46 visbeats/fileui/__init__.py
 -rw-r--r--  2.0 unx     2922 b- defN 23-May-09 08:08 visbeats/fileui/uipath.py
+-rw-r--r--  2.0 unx     1655 b- defN 23-May-15 19:03 visbeats/fileui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     2784 b- defN 23-May-15 19:03 visbeats/fileui/__pycache__/uipath.cpython-39.pyc
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 07:48 visbeats/vbgui/__init__.py
 -rw-r--r--  2.0 unx    10355 b- defN 23-May-09 09:29 visbeats/vbgui/beatgui.py
-40 files, 333060 bytes uncompressed, 78971 bytes compressed:  76.3%
+-rw-r--r--  2.0 unx      151 b- defN 23-May-15 19:03 visbeats/vbgui/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--  2.0 unx     9641 b- defN 23-May-15 19:03 visbeats/vbgui/__pycache__/beatgui.cpython-39.pyc
+74 files, 635919 bytes uncompressed, 200274 bytes compressed:  68.5%
```

## zipnote «TEMP»/diffoscope_q0p3mq6n_/tmptv4t56f3_.zip

```diff
@@ -3,21 +3,21 @@
 
 Filename: EGG-INFO/SOURCES.txt
 Comment: 
 
 Filename: EGG-INFO/dependency_links.txt
 Comment: 
 
-Filename: EGG-INFO/requires.txt
+Filename: EGG-INFO/not-zip-safe
 Comment: 
 
-Filename: EGG-INFO/top_level.txt
+Filename: EGG-INFO/requires.txt
 Comment: 
 
-Filename: EGG-INFO/zip-safe
+Filename: EGG-INFO/top_level.txt
 Comment: 
 
 Filename: EGG-INFO/scripts/hifi
 Comment: 
 
 Filename: EGG-INFO/scripts/visbeats
 Comment: 
@@ -102,20 +102,122 @@
 
 Filename: visbeats/visualbeat.py
 Comment: 
 
 Filename: visbeats/warp.py
 Comment: 
 
+Filename: visbeats/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/adefines.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/afilemanager.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/afuncdict.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/aimports.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/aobject.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/aparamdict.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/audio.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/audioclip.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/event.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/eventlist.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/image.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/image_cv.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/mediafiles.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/sourcelocationparser.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/timesignal.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/timesignal1d.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/vbmidi.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/vbobject.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/video.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/video_cv.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/videoclip.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/videosource.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/visbeatdefines.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/visbeatexamplevideo.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/visbeatimports.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/visualbeat.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/__pycache__/warp.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/assets/audio/hit.wav
+Comment: 
+
+Filename: visbeats/assets/images/VisBeatWatermark.png
+Comment: 
+
 Filename: visbeats/fileui/__init__.py
 Comment: 
 
 Filename: visbeats/fileui/uipath.py
 Comment: 
 
+Filename: visbeats/fileui/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/fileui/__pycache__/uipath.cpython-39.pyc
+Comment: 
+
 Filename: visbeats/vbgui/__init__.py
 Comment: 
 
 Filename: visbeats/vbgui/beatgui.py
 Comment: 
 
+Filename: visbeats/vbgui/__pycache__/__init__.cpython-39.pyc
+Comment: 
+
+Filename: visbeats/vbgui/__pycache__/beatgui.cpython-39.pyc
+Comment: 
+
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hifi
-Version: 5.0.0
+Version: 6.0.0
 Summary: Command-line tool to find nearest store.
 Home-page: https://github.com/austinbrown34/hifi
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,11 +1,23 @@
 LICENSE
 MANIFEST.in
+Pipfile
 README.md
+environment.yml
+requirements.txt
 setup.py
+hifi/__init__,py
+hifi/engine.py
+hifi/hiphy.py
+hifi/live-encoder.sh
+hifi/out-ffmpeg.sh
+hifi/test-encoder.sh
+hifi/utils.py
+hifi/vidsnatch.py
+hifi/youtube-ffmpeg-mp4.sh
 hifi.egg-info/PKG-INFO
 hifi.egg-info/SOURCES.txt
 hifi.egg-info/dependency_links.txt
 hifi.egg-info/requires.txt
 hifi.egg-info/top_level.txt
 scripts/hifi
 scripts/visbeats
@@ -33,11 +45,13 @@
 visbeats/videoclip.py
 visbeats/videosource.py
 visbeats/visbeatdefines.py
 visbeats/visbeatexamplevideo.py
 visbeats/visbeatimports.py
 visbeats/visualbeat.py
 visbeats/warp.py
+visbeats/assets/audio/hit.wav
+visbeats/assets/images/VisBeatWatermark.png
 visbeats/fileui/__init__.py
 visbeats/fileui/uipath.py
 visbeats/vbgui/__init__.py
 visbeats/vbgui/beatgui.py
```

## EGG-INFO/scripts/hifi

```diff
@@ -1,8 +1,8 @@
-#!/Users/austinbrown/.local/share/virtualenvs/hifi-xpvT5RK6/bin/python
+#!/Users/austinbrown/miniforge3/bin/python
 
 import sys
 import argparse
 from hifi.hiphy import Hiphy
 from datetime import datetime
 import json
```

## EGG-INFO/scripts/visbeats

```diff
@@ -1,8 +1,8 @@
-#!/Users/austinbrown/.local/share/virtualenvs/hifi-xpvT5RK6/bin/python
+#!/Users/austinbrown/miniforge3/bin/python
 
 import sys
 import argparse
 import matplotlib
 matplotlib.use('PS')
 import visbeats as visbeats
 import os
```

