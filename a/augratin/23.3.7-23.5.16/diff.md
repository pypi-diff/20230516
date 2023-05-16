# Comparing `tmp/augratin-23.3.7.tar.gz` & `tmp/augratin-23.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augratin-23.3.7.tar", last modified: Tue Mar  7 16:07:08 2023, max compression
+gzip compressed data, was "augratin-23.5.16.tar", last modified: Tue May 16 19:45:37 2023, max compression
```

## Comparing `augratin-23.3.7.tar` & `augratin-23.5.16.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-07 16:07:08.786555 augratin-23.3.7/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.3.7/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4231 2023-03-07 16:07:08.786555 augratin-23.3.7/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3457 2023-03-07 16:05:13.000000 augratin-23.3.7/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-07 16:07:08.759555 augratin-23.3.7/augratin/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/__init__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    25079 2023-03-07 15:55:00.000000 augratin-23.3.7/augratin/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-07 16:07:08.783555 augratin-23.3.7/augratin/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24590 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/data/k6gte-augratin-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/data/k6gte-augratin-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/data/k6gte-augratin-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/data/k6gte-augratin.desktop
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-07 16:07:08.785555 augratin-23.3.7/augratin/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10244 2023-02-17 19:16:23.000000 augratin-23.3.7/augratin/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-03-07 15:55:15.000000 augratin-23.3.7/augratin/lib/version.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-07 16:07:08.765555 augratin-23.3.7/augratin.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4231 2023-03-07 16:07:08.000000 augratin-23.3.7/augratin.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      557 2023-03-07 16:07:08.000000 augratin-23.3.7/augratin.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-03-07 16:07:08.000000 augratin-23.3.7/augratin.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-03-07 16:07:08.000000 augratin-23.3.7/augratin.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       43 2023-03-07 16:07:08.000000 augratin-23.3.7/augratin.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-03-07 16:07:08.000000 augratin-23.3.7/augratin.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1107 2023-03-07 15:55:52.000000 augratin-23.3.7/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-03-07 16:07:08.786555 augratin-23.3.7/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.194069 augratin-23.5.16/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-02-19 00:59:20.000000 augratin-23.5.16/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4644 2023-05-16 19:45:37.194069 augratin-23.5.16/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3869 2023-05-16 19:43:59.000000 augratin-23.5.16/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.187069 augratin-23.5.16/augratin/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/__init__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    39551 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.193069 augratin-23.5.16/augratin/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    25586 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22040 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2015 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6303 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/data/k6gte-augratin.desktop
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.193069 augratin-23.5.16/augratin/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-17 19:16:23.000000 augratin-23.5.16/augratin/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2071 2023-03-28 14:10:04.000000 augratin-23.5.16/augratin/lib/omnirig_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-16 19:37:32.000000 augratin-23.5.16/augratin/lib/version.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-16 19:45:37.189069 augratin-23.5.16/augratin.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4644 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      591 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       71 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       31 2023-05-16 19:45:37.000000 augratin-23.5.16/augratin.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1142 2023-05-16 19:37:32.000000 augratin-23.5.16/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-16 19:45:37.194069 augratin-23.5.16/setup.cfg
```

### Comparing `augratin-23.3.7/LICENSE` & `augratin-23.5.16/LICENSE`

 * *Files identical despite different names*

### Comparing `augratin-23.3.7/PKG-INFO` & `augratin-23.5.16/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.3.7
+Version: 23.5.16
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -24,15 +24,15 @@
 
 ![logo](https://github.com/mbridak/augratin/raw/master/augratin/data/k6gte.augratin.svg)
 
 - [AuGratin](#augratin)
   - [Why AuGratin](#why-augratin)
   - [What is AuGratin](#what-is-augratin)
   - [Recent changes](#recent-changes)
-  - [Installing AuGratin](#installing-augratin)
+  - [Installing, Updating, Running, Removing](#installing-updating-running-removing)
   - [Features](#features)
   - [What to do if your map is blank](#what-to-do-if-your-map-is-blank)
   - [CAT control](#cat-control)
 
 ## Why AuGratin
 
 AuGratin is an extension to an earlier program called POTAto. And since it's made from POTAto, I called it AuGratin.
@@ -43,67 +43,80 @@
 [POTA](https://parksontheair.com) is Parks On The Air.
 A year round activity of many amateur radio operators or HAMS.
 The Activator, will set up a radio station in a state/national park and make as many contacts as they can.
 Other Radio Amateurs also known as Hunters or Chasers, will seek out and try to contact as many Activators as they can.
 
 AuGratin allows A [POTA](https://parksontheair.com) Hunter to easily log contacts with Activators.
 It pulls latest [POTA](https://parksontheair.com) spots. Displays them in a compact interface.
-Once a spot is clicked on AuGratin will talk to either rigctld or flrig to change the radio to the correct
+Once a spot is clicked on AuGratin will talk to either rigctld, flrig, or OmniRig to change the radio to the correct
 frequency and mode. It will pre-populate All the fields needed for logging the contact.
 All contacts are stored in an ADIF file in your home directory,
-which you can them import into your normal logging program.
+which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-15] Start big code changes to impliment better bandmap.
+- [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
-## Installing AuGratin
+## Installing, Updating, Running, Removing
 
 ```bash
+# install
 pip install augratin
+
+# update
+pip install -U augratin
+
+# remove
+pip uninstall augratin
+
+# running
+augratin
 ```
 
 ## Features
 
-- You can filter spots by band and or mode.
+- Shows spots on a band map
+- You can filter spots by mode.
 - Pulls in park and activator information.
-- Tunes your radio with flrig or rigctld to the activator and sets the mode automatically.
-- Double clicked spots adds Activator to a persistent watchlist.
+- Clicked spots, tune your radio with flrig, rigctld or OmniRig to the activator and sets the mode automatically.
+- ~~Double clicked spots adds Activator to a persistent watchlist.~~
 - Displays bearing to contact.
 
 When you press the "Log it" button the adif information is appended to `POTA_Contacts.adi` in your home folder.
 
 ## What to do if your map is blank
 
 Not sure why, but the map may not work if you let pip install PyQt5 and PyQtWebEngine automatically. If your map is blank, try:
 
 ```bash
 pip uninstall PyQt5
-Pip uninstall PyQtWebEngine
+pip uninstall PyQtWebEngine
 ```
 
 Then install them through your package manager.
 
 ```bash
 #fedora
 sudo dnf install python3-qt5 python3-qt5-webengine
 
 #ubuntu
 sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine
 ```
 
 ## CAT control
 
-If no command line options are given, the program will check if either flrig
-or rigctld are running on the computer. It will setup CAT control to which
-ever it finds first.
+If no command line options are given, the program will check if either flrig, rigctld or OmniRig are running on the computer. It will setup CAT control to whichever it finds first.
 
 You can force it to use either with commandline options.
 
 `-r` will force rigctld with default host:port of localhost:4532.
 
 `-f` will force flrig with default host:port of localhost:12345.
 
+`-2` will force 'Rig2' with OmniRig.
+
 `-s SERVER:PORT` will specify a non-standard host and port.
```

### Comparing `augratin-23.3.7/README.md` & `augratin-23.5.16/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ![logo](https://github.com/mbridak/augratin/raw/master/augratin/data/k6gte.augratin.svg)
 
 - [AuGratin](#augratin)
   - [Why AuGratin](#why-augratin)
   - [What is AuGratin](#what-is-augratin)
   - [Recent changes](#recent-changes)
-  - [Installing AuGratin](#installing-augratin)
+  - [Installing, Updating, Running, Removing](#installing-updating-running-removing)
   - [Features](#features)
   - [What to do if your map is blank](#what-to-do-if-your-map-is-blank)
   - [CAT control](#cat-control)
 
 ## Why AuGratin
 
 AuGratin is an extension to an earlier program called POTAto. And since it's made from POTAto, I called it AuGratin.
@@ -24,67 +24,80 @@
 [POTA](https://parksontheair.com) is Parks On The Air.
 A year round activity of many amateur radio operators or HAMS.
 The Activator, will set up a radio station in a state/national park and make as many contacts as they can.
 Other Radio Amateurs also known as Hunters or Chasers, will seek out and try to contact as many Activators as they can.
 
 AuGratin allows A [POTA](https://parksontheair.com) Hunter to easily log contacts with Activators.
 It pulls latest [POTA](https://parksontheair.com) spots. Displays them in a compact interface.
-Once a spot is clicked on AuGratin will talk to either rigctld or flrig to change the radio to the correct
+Once a spot is clicked on AuGratin will talk to either rigctld, flrig, or OmniRig to change the radio to the correct
 frequency and mode. It will pre-populate All the fields needed for logging the contact.
 All contacts are stored in an ADIF file in your home directory,
-which you can them import into your normal logging program.
+which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-15] Start big code changes to impliment better bandmap.
+- [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
-## Installing AuGratin
+## Installing, Updating, Running, Removing
 
 ```bash
+# install
 pip install augratin
+
+# update
+pip install -U augratin
+
+# remove
+pip uninstall augratin
+
+# running
+augratin
 ```
 
 ## Features
 
-- You can filter spots by band and or mode.
+- Shows spots on a band map
+- You can filter spots by mode.
 - Pulls in park and activator information.
-- Tunes your radio with flrig or rigctld to the activator and sets the mode automatically.
-- Double clicked spots adds Activator to a persistent watchlist.
+- Clicked spots, tune your radio with flrig, rigctld or OmniRig to the activator and sets the mode automatically.
+- ~~Double clicked spots adds Activator to a persistent watchlist.~~
 - Displays bearing to contact.
 
 When you press the "Log it" button the adif information is appended to `POTA_Contacts.adi` in your home folder.
 
 ## What to do if your map is blank
 
 Not sure why, but the map may not work if you let pip install PyQt5 and PyQtWebEngine automatically. If your map is blank, try:
 
 ```bash
 pip uninstall PyQt5
-Pip uninstall PyQtWebEngine
+pip uninstall PyQtWebEngine
 ```
 
 Then install them through your package manager.
 
 ```bash
 #fedora
 sudo dnf install python3-qt5 python3-qt5-webengine
 
 #ubuntu
 sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine
 ```
 
 ## CAT control
 
-If no command line options are given, the program will check if either flrig
-or rigctld are running on the computer. It will setup CAT control to which
-ever it finds first.
+If no command line options are given, the program will check if either flrig, rigctld or OmniRig are running on the computer. It will setup CAT control to whichever it finds first.
 
 You can force it to use either with commandline options.
 
 `-r` will force rigctld with default host:port of localhost:4532.
 
 `-f` will force flrig with default host:port of localhost:12345.
 
+`-2` will force 'Rig2' with OmniRig.
+
 `-s SERVER:PORT` will specify a non-standard host and port.
```

### Comparing `augratin-23.3.7/augratin/__main__.py` & `augratin-23.5.16/augratin/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 #!/usr/bin/env python3
 """AuGratin helps chasers hunt POTA activators. Find out more about POTA at https://pota.app"""
 
+# pylint: disable=unused-import, c-extension-no-member, no-member, invalid-name, too-many-lines
 # pylint: disable=no-name-in-module
-# pylint: disable=c-extension-no-member
 # pylint: disable=wildcard-import
 # pylint: disable=line-too-long
 
 # https://api.pota.app/park/K-0064
 # {"parkId": 64, "reference": "K-0064", "name": "Shenandoah", "latitude": 38.9068, "longitude": -78.1988, "grid4": "FM08", "grid6": "FM08vv", "parktypeId": 41, "active": 1, "parkComments": "Potentially co-located with K-4556 - Appalachian Trail NST.  Numerous SOTA locations.", "accessibility": null, "sensitivity": null, "accessMethods": "Automobile,Foot", "activationMethods": "Automobile,Cabin,Campground,Pedestrian,Shelter", "agencies": "National Park Service", "agencyURLs": "https://www.nps.gov/index.htm", "parkURLs": "https://www.nps.gov/shen/index.htm", "website": "https://www.nps.gov/shen/index.htm", "createdByAdmin": null, "parktypeDesc": "National Park", "locationDesc": "US-VA", "locationName": "Virginia", "entityId": 291, "entityName": "United States Of America", "referencePrefix": "K", "entityDeleted": 0, "firstActivator": "WX4TW", "firstActivationDate": "2015-08-27"}
 
 # https://api.pota.app/stats/user/K2EAG
 # {"callsign": "K2EAG", "name": "Matt Brown", "qth": "Amherst, New York", "gravatar": "bf8377378b67b265cbb2be687b13a23a", "activator": {"activations": 72, "parks": 33, "qsos": 3724}, "attempts": {"activations": 80, "parks": 33, "qsos": 3724}, "hunter": {"parks": 237, "qsos": 334}, "awards": 16, "endorsements": 32}
 
 import argparse
 import sys
+import sqlite3
 import os
 import io
 import logging
 from math import radians, sin, cos, atan2, sqrt, asin, pi
 import pkgutil
 from pathlib import Path
 from datetime import datetime, timezone
 from json import loads, dumps
 import re
 
 import psutil
-from PyQt5 import QtCore, QtWidgets, uic
+from PyQt5 import QtCore, QtWidgets, QtGui, uic
 from PyQt5.QtCore import QDir
 from PyQt5.QtGui import QFontDatabase, QBrush, QColor
 import PyQt5.QtWebEngineWidgets  # pylint: disable=unused-import
 
 # from PyQt5.QtWebEngineWidgets import QWebEngineView
 
 
 import requests
 import folium
 
 try:
     from augratin.lib.version import __version__
     from augratin.lib.cat_interface import CAT
+
+    if sys.platform == "win32":
+        from augratin.lib.omnirig_interface import OmniRigClient
 except ModuleNotFoundError:
     from lib.version import __version__
     from lib.cat_interface import CAT
 
+    if sys.platform == "win32":
+        from lib.omnirig_interface import OmniRigClient
+
 __author__ = "Michael C. Bridak, K6GTE"
 __license__ = "GNU General Public License v3.0"
 
 loader = pkgutil.get_loader("augratin")
 WORKING_PATH = os.path.dirname(loader.get_filename())
 
 logger = logging.getLogger("__name__")
@@ -82,36 +89,49 @@
     "-f",
     action=argparse.BooleanOptionalAction,
     dest="flrig",
     help="Force use of flrig",
 )
 
 parser.add_argument(
+    "-2",
+    action=argparse.BooleanOptionalAction,
+    dest="rig2",
+    help="Force use of rig2 in omnirig",
+)
+
+parser.add_argument(
     "-d",
     action=argparse.BooleanOptionalAction,
     dest="debug",
     help="Debug",
 )
 
 args = parser.parse_args()
 
+PIXELSPERSTEP = 10
+
 FORCED_INTERFACE = None
 SERVER_ADDRESS = None
+OMNI_RIGNUMBER = 1
 
 if args.rigctld:
     FORCED_INTERFACE = "rigctld"
     SERVER_ADDRESS = "localhost:4532"
 
 if args.flrig:
     FORCED_INTERFACE = "flrig"
     SERVER_ADDRESS = "localhost:12345"
 
 if args.server:
     SERVER_ADDRESS = args.server
 
+if args.rig2:
+    OMNI_RIGNUMBER = 2
+
 if args.debug:
     logger.setLevel(logging.DEBUG)
 
 logger.debug("Forces Interface: %s", FORCED_INTERFACE)
 logger.debug("Server Address: %s", SERVER_ADDRESS)
 
 
@@ -120,17 +140,168 @@
     font_families = set()
     for file_index in QDir(directory).entryInfoList(["*.ttf", "*.woff", "*.woff2"]):
         _id = QFontDatabase.addApplicationFont(file_index.absoluteFilePath())
         font_families |= set(QFontDatabase.applicationFontFamilies(_id))
     return font_families
 
 
+class Band:
+    """the band"""
+
+    bands = {
+        "160m": (1.8, 2),
+        "80m": (3.5, 4),
+        "60m": (5.102, 5.4065),
+        "40m": (7.0, 7.3),
+        "30m": (10.1, 10.15),
+        "20m": (14.0, 14.35),
+        "15m": (21.0, 21.45),
+        "10m": (28.0, 29.7),
+        "6m": (50.0, 54.0),
+        "4m": (70.0, 71.0),
+        "2m": (144.0, 148.0),
+    }
+
+    def __init__(self, band: str) -> None:
+        self.start, self.end = self.bands.get(band, (0.0, 1.0))
+        self.name = band
+
+
+class Database:
+    """spot database"""
+
+    def __init__(self) -> None:
+        self.db = sqlite3.connect(":memory:")
+        self.db.row_factory = self.row_factory
+        self.cursor = self.db.cursor()
+        sql_command = (
+            "create table spots("
+            "spotId INTEGER NOT NULL,"
+            "spotTime DATETIME NOT NULL, "
+            "activator VARCHAR(15) NOT NULL, "
+            "frequency REAL NOT NULL, "
+            "mode VARCHAR(6), "
+            "reference VARCHAR(8), "
+            "parkName VARCHAR(50), "
+            "spotter VARCHAR(15) NOT NULL, "
+            "comments VARCHAR(45), "
+            "source VARCHAR(8), "
+            "invalid INTEGER, "
+            "name VARCHAR(50), "
+            "locationDesc VARCHAR(10), "
+            "grid4 VARCHAR(4), "
+            "grid6 VARCHAR(6), "
+            "latitude REAL, "
+            "longitude REAL, "
+            "count INTEGER, "
+            "expire INTEGER "
+            ");"
+        )
+        self.cursor.execute(sql_command)
+        self.db.commit()
+
+    @staticmethod
+    def row_factory(cursor, row):
+        """
+        cursor.description:
+        (name, type_code, display_size,
+        internal_size, precision, scale, null_ok)
+        row: (value, value, ...)
+        """
+        return {
+            col[0]: row[idx]
+            for idx, col in enumerate(
+                cursor.description,
+            )
+        }
+
+    def addspot(self, spot):
+        """doc"""
+        try:
+            delete_call = (
+                f"delete from spots where activator = '{spot.get('activator')}';"
+            )
+            self.cursor.execute(delete_call)
+            self.db.commit()
+
+            pre = "INSERT INTO spots("
+            values = []
+            columns = ""
+            placeholders = ""
+            for key in spot.keys():
+                columns += f"{key},"
+                values.append(spot[key])
+                placeholders += "?,"
+            post = f") VALUES({placeholders[:-1]});"
+
+            sql = f"{pre}{columns[:-1]}{post}"
+            self.cursor.execute(sql, tuple(values))
+            self.db.commit()
+        except sqlite3.IntegrityError:
+            ...
+
+    def getspots(self) -> list:
+        """returns a list of dicts."""
+        try:
+            self.cursor.execute("select * from spots order by frequency ASC;")
+            return self.cursor.fetchall()
+        except sqlite3.OperationalError:
+            return ()
+
+    def getspotsinband(self, start: float, end: float) -> list:
+        """ "return a list of dict where freq range is defined"""
+        self.cursor.execute(
+            f"select * from spots where frequency >= {start} and frequency <= {end} order by frequency ASC;"
+        )
+        return self.cursor.fetchall()
+
+    def get_next_spot(self, current: float, limit: float) -> dict:
+        """ "return a list of dict where freq range is defined"""
+        self.cursor.execute(
+            f"select * from spots where frequency > {current} and frequency <= {limit} order by frequency ASC;"
+        )
+        return self.cursor.fetchone()
+
+    def get_prev_spot(self, current: float, limit: float) -> dict:
+        """ "return a list of dict where freq range is defined"""
+        self.cursor.execute(
+            f"select * from spots where frequency < {current} and frequency >= {limit} order by frequency DESC;"
+        )
+        return self.cursor.fetchone()
+
+    def getspot_byid(self, spot_id: int) -> dict:
+        """ "return dict of spot with the matching spotId"""
+        self.cursor.execute(f"select * from spots where spotId = {spot_id};")
+        return self.cursor.fetchone()
+
+    def delete_spots(self, minutes: int):
+        """doc"""
+        self.cursor.execute(
+            f"delete from spots where spotTime < datetime('now', '-{minutes} minutes');"
+        )
+
+
 class MainWindow(QtWidgets.QMainWindow):
     """The main window class"""
 
+    zoom = 5
+    currentBand = Band("20m")
+    txMark = []
+    rxMark = []
+    rx_freq = None
+    tx_freq = None
+    lineitemlist = []
+    textItemList = []
+    bandwidth = 0
+    bandwidth_mark = []
+    freq = 0.0
+    keepRXCenter = False
+    something = None
+    agetime = None
+
     potaurl = "https://api.pota.app/spot/activator"
     parkurl = "https://api.pota.app/park/"
     activatorurl = "https://api.pota.app/stats/user/"
     bw = {}
     lastclicked = ""
     workedlist = []
     spots = None
@@ -166,40 +337,50 @@
                     logger.debug("reading workedlist: %s", self.settings)
         except IOError as exception:
             logger.critical("%s", exception)
 
         self.cat_control = None
         local_flrig = self.check_process("flrig")
         local_rigctld = self.check_process("rigctld")
+        local_omnirig = self.check_process("omnirig.exe")
 
         if FORCED_INTERFACE:
             address, port = SERVER_ADDRESS.split(":")
             self.cat_control = CAT(FORCED_INTERFACE, address, int(port))
 
         if self.cat_control is None:
             if local_flrig:
                 if SERVER_ADDRESS:
                     address, port = SERVER_ADDRESS.split(":")
                 else:
                     address, port = "localhost", "12345"
-                self.cat_control = CAT("flrig", address, int(port))
+                    self.cat_control = CAT("flrig", address, int(port))
             if local_rigctld:
                 if SERVER_ADDRESS:
                     address, port = SERVER_ADDRESS.split(":")
                 else:
                     address, port = "localhost", "4532"
-                self.cat_control = CAT("rigctld", address, int(port))
+                    self.cat_control = CAT("rigctld", address, int(port))
+            if local_omnirig:
+                self.cat_control = OmniRigClient(OMNI_RIGNUMBER)
+                logging.debug("omnirig called")
 
         super().__init__(parent)
         data_path = WORKING_PATH + "/data/dialog.ui"
         uic.loadUi(data_path, self)
-        self.listWidget.clicked.connect(self.spotclicked)
-        self.listWidget.doubleClicked.connect(self.item_double_clicked)
+        self.zoom_in_button.clicked.connect(self.dec_zoom)
+        self.zoom_out_button.clicked.connect(self.inc_zoom)
+        self.bandmap_scene = QtWidgets.QGraphicsScene()
+        self.bandmap_scene.clear()
+        self.bandmap_scene.setFocusOnTouch(False)
+        self.bandmap_scene.selectionChanged.connect(self.spotclicked)
+        self.spotdb = Database()
         self.comboBox_mode.currentTextChanged.connect(self.getspots)
-        self.comboBox_band.currentTextChanged.connect(self.getspots)
+        self.comboBox_band.hide()
+        # self.comboBox_band.currentTextChanged.connect(self.getspots)
         self.mycall_field.textEdited.connect(self.save_call_and_grid)
         self.mygrid_field.textEdited.connect(self.save_call_and_grid)
         self.log_button.clicked.connect(self.log_contact)
         self.mycall_field.setText(self.settings.get("mycall", ""))
         self.mygrid_field.setText(self.settings.get("mygrid", ""))
         if self.settings.get("mygrid", "") == "":
             self.mygrid_field.setStyleSheet("border: 1px solid red;")
@@ -214,14 +395,33 @@
             zoom_start=3,
             max_zoom=19,
         )
         data = io.BytesIO()
         self.map.save(data, close_file=False)
         self.mapview.setHtml(data.getvalue().decode())
 
+    def poll_radio(self):
+        """Get Freq and Mode changes"""
+        if self.cat_control:
+            newfreq = float(self.cat_control.get_vfo()) / 1000000
+            # newmode = self.cat_control.get_mode()
+            if hasattr(self.cat_control, "get_bw"):
+                newbw = int(self.cat_control.get_bw())
+            else:
+                newbw = 0
+            if self.rx_freq != newfreq:
+                self.rx_freq = newfreq
+                self.set_band(f"{self.getband(str(int(newfreq * 1000)))}m")
+                step, _ = self.determine_step_digits()
+                self.drawTXRXMarks(step)
+            if self.bandwidth != newbw:
+                self.bandwidth = newbw
+                step, _ = self.determine_step_digits()
+                self.drawTXRXMarks(step)
+
     def save_call_and_grid(self):
         """Saves users callsign and gridsquare to json file."""
         self.settings["mycall"] = self.mycall_field.text().upper()
         self.settings["mygrid"] = self.mygrid_field.text().upper()
         try:
             home = os.path.expanduser("~")
             with open(
@@ -320,25 +520,25 @@
         dlon = lon2 - lon1
         dlat = lat2 - lat1
         aye = sin(dlat / 2) ** 2 + cos(lat1) * cos(lat2) * sin(dlon / 2) ** 2
         cee = 2 * asin(sqrt(aye))
         arrgh = 6372.8  # Radius of earth in kilometers.
         return cee * arrgh
 
-    def potasort(self, element):
-        """Sort list or dictionary items"""
-        return element["spotId"]
-
     def getspots(self):
         """Gets activator spots from pota.app"""
         self.time.setText(str(datetime.now(timezone.utc)).split()[1].split(".")[0][0:5])
         self.spots = self.getjson(self.potaurl)
         if self.spots:
-            self.spots.sort(reverse=True, key=self.potasort)
-            self.showspots()
+            for spot in self.spots:
+                spot["frequency"] = float(spot.get("frequency")) / 1000
+                self.spotdb.addspot(spot)
+            # self.spots.sort(reverse=True, key=self.potasort)
+            # self.showspots()
+            self.update()
 
     def log_contact(self):
         """Log the contact"""
         if self.loggable is False:
             return
         try:
             freq = str(int(self.freq_field.text()) / 1000000)
@@ -382,52 +582,115 @@
         with open(
             home + "/POTA_Contacts.adi", "a", encoding="utf-8"
         ) as file_descriptor:
             print(qso, file=file_descriptor)
         self.clear_fields()
         self.loggable = False
 
-    def showspots(self):
-        """Display spots in a list"""
-        self.listWidget.clear()
-        for i in self.spots:
-            mode_selection = self.comboBox_mode.currentText()
-            if mode_selection == "-FT*" and i["mode"][:2] == "FT":
-                continue
-            if (
-                mode_selection == "All"
-                or mode_selection == "-FT*"
-                or i["mode"] == mode_selection
-            ):
-                band_selection = self.comboBox_band.currentText()
+    def update(self):
+        """doc"""
+        # self.update_timer.setInterval(UPDATE_INTERVAL)
+        self.clear_all_callsign_from_scene()
+        self.clear_freq_mark(self.rxMark)
+        self.clear_freq_mark(self.txMark)
+        self.clear_freq_mark(self.bandwidth_mark)
+        self.bandmap_scene.clear()
+
+        step, _digits = self.determine_step_digits()
+        steps = int(round((self.currentBand.end - self.currentBand.start) / step))
+        self.graphicsView.setFixedSize(330, steps * PIXELSPERSTEP + 30)
+        self.graphicsView.setScene(self.bandmap_scene)
+        for i in range(steps):  # Draw tickmarks
+            length = 10
+            if i % 5 == 0:
+                length = 15
+            self.bandmap_scene.addLine(
+                10,
+                i * PIXELSPERSTEP,
+                length + 10,
+                i * PIXELSPERSTEP,
+                QtGui.QPen(QtGui.QColor(192, 192, 192)),
+            )
+            if i % 5 == 0:  # Add Frequency
+                freq = self.currentBand.start + step * i
+                text = f"{freq:.3f}"
+                self.something = self.bandmap_scene.addText(text)
+                self.something.setPos(
+                    -(self.something.boundingRect().width()) + 10,
+                    i * PIXELSPERSTEP - (self.something.boundingRect().height() / 2),
+                )
+
+        freq = self.currentBand.end + step * steps
+        endFreqDigits = f"{freq:.3f}"
+        self.bandmap_scene.setSceneRect(
+            160 - (len(endFreqDigits) * PIXELSPERSTEP), 0, 0, steps * PIXELSPERSTEP + 20
+        )
+
+        self.drawTXRXMarks(step)
+        self.update_stations()
+
+    def update_stations(self):
+        """doc"""
+        self.clear_all_callsign_from_scene()
+        self.spot_aging()
+        step, _digits = self.determine_step_digits()
+        mode_selection = self.comboBox_mode.currentText()
+        result = self.spotdb.getspotsinband(
+            self.currentBand.start, self.currentBand.end
+        )
+        if result:
+            min_y = 0.0
+            for items in result:
+                if mode_selection == "-FT*" and items["mode"][:2] == "FT":
+                    continue
                 if (
-                    band_selection == "All"
-                    or self.getband(i["frequency"].split(".")[0]) == band_selection
+                    mode_selection == "All"
+                    or mode_selection == "-FT*"
+                    or items["mode"] == mode_selection
                 ):
-                    spot = (
-                        f"{i['spotTime'].split('T')[1][0:5]} "
-                        f"{i['activator'].rjust(10)} "
-                        f"{i['reference'].ljust(7)} "
-                        f"{i['frequency'].split('.')[0].rjust(6)} "
-                        f"{i['mode']}"
-                    )
-
-                    self.listWidget.addItem(spot)
-                    if spot[5:] == self.lastclicked[5:]:
-                        founditem = self.listWidget.findItems(
-                            spot[5:],
-                            QtCore.Qt.MatchFlag.MatchContains,  # pylint: disable=no-member
+                    freq_y = (
+                        (items.get("frequency") - self.currentBand.start) / step
+                    ) * PIXELSPERSTEP
+                    text_y = max(min_y + 5, freq_y)
+                    self.lineitemlist.append(
+                        self.bandmap_scene.addLine(
+                            22,
+                            freq_y,
+                            55,
+                            text_y,
+                            QtGui.QPen(QtGui.QColor(192, 192, 192)),
                         )
-                        founditem[0].setSelected(True)
-                    if i["activator"] in self.workedlist:
-                        founditem = self.listWidget.findItems(
-                            i["activator"],
-                            QtCore.Qt.MatchFlag.MatchContains,  # pylint: disable=no-member
-                        )
-                        founditem[0].setBackground(QBrush(QColor.fromRgb(0, 128, 0)))
+                    )
+                    text = self.bandmap_scene.addText(
+                        items.get("activator")
+                        + " @ "
+                        + items.get("reference")
+                        + " "
+                        + items.get("mode")
+                        + " "
+                        + items.get("spotTime").split("T")[1][:-3]
+                    )
+                    text.document().setDocumentMargin(0)
+                    text.setPos(60, text_y - (text.boundingRect().height() / 2))
+                    text.setFlags(
+                        QtWidgets.QGraphicsItem.ItemIsFocusable
+                        | QtWidgets.QGraphicsItem.ItemIsSelectable
+                        | text.flags()
+                    )
+                    text.setProperty("freq", items.get("frequency"))
+                    text.setProperty("spotId", items.get("spotId"))
+                    text.setProperty("mode", items.get("mode"))
+                    text.setToolTip(items.get("comments"))
+
+                    min_y = text_y + text.boundingRect().height() / 2
+
+                    # textColor = Data::statusToColor(lower.value().status,
+                    # qApp->palette().color(QPalette::Text));
+                    # text->setDefaultTextColor(textColor);
+                    self.textItemList.append(text)
 
     def clear_fields(self):
         """Clear input fields and reset focus to RST TX."""
         self.activator_call.setText("")
         self.activator_name.setText("")
         self.park_designator.setText("")
         self.mode_field.setText("")
@@ -440,30 +703,178 @@
         self.park_grid.setText("")
         self.park_section.setText("")
         self.comments.setPlainText("")
         self.park_distance.setText("")
         self.park_direction.setText("")
         self.rst_sent.setFocus()
 
+    def spot_aging(self):
+        """doc"""
+        if self.agetime:
+            self.spots.delete_spots(self.agetime)
+
+    def inc_zoom(self):
+        """doc"""
+        self.zoom += 1
+        self.zoom = min(self.zoom, 7)
+        self.update()
+        self.center_on_rxfreq()
+
+    def dec_zoom(self):
+        """doc"""
+        self.zoom -= 1
+        self.zoom = max(self.zoom, 1)
+        self.update()
+        self.center_on_rxfreq()
+
+    def drawTXRXMarks(self, step):
+        """doc"""
+        if self.rx_freq:
+            self.clear_freq_mark(self.bandwidth_mark)
+            self.clear_freq_mark(self.rxMark)
+            self.draw_bandwidth(
+                self.rx_freq, step, QtGui.QColor(30, 30, 180, 180), self.bandwidth_mark
+            )
+            self.drawfreqmark(
+                self.rx_freq, step, QtGui.QColor(30, 180, 30, 180), self.rxMark
+            )
+
+    def Freq2ScenePos(self, freq: float):
+        """doc"""
+        if freq < self.currentBand.start or freq > self.currentBand.end:
+            return QtCore.QPointF()
+        step, _digits = self.determine_step_digits()
+        ret = QtCore.QPointF(
+            0, ((freq - self.currentBand.start) / step) * PIXELSPERSTEP
+        )
+        return ret
+
+    def center_on_rxfreq(self):
+        """doc"""
+        freq_pos = self.Freq2ScenePos(self.rx_freq).y()
+        self.scrollArea.verticalScrollBar().setValue(
+            int(freq_pos - (self.height() / 2) + 80)
+        )
+
+    def drawfreqmark(self, freq, _step, color, currentPolygon):
+        """doc"""
+
+        self.clear_freq_mark(currentPolygon)
+        # do not show the freq mark if it is outside the bandmap
+        if freq < self.currentBand.start or freq > self.currentBand.end:
+            return
+
+        Yposition = self.Freq2ScenePos(freq).y()
+
+        poly = QtGui.QPolygonF()
+
+        poly.append(QtCore.QPointF(21, Yposition))
+        poly.append(QtCore.QPointF(10, Yposition - 7))
+        poly.append(QtCore.QPointF(10, Yposition + 7))
+        pen = QtGui.QPen()
+        brush = QtGui.QBrush(color)
+        currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
+
+    def draw_bandwidth(self, freq, _step, color, currentPolygon):
+        """bandwidth"""
+        logger.debug("%s", f"mark:{currentPolygon} f:{freq} b:{self.bandwidth}")
+        self.clear_freq_mark(currentPolygon)
+        if freq < self.currentBand.start or freq > self.currentBand.end:
+            return
+        if freq and self.bandwidth:
+            # color = QtGui.QColor(30, 30, 180)
+            bw_start = freq - ((self.bandwidth / 2) / 1000000)
+            bw_end = freq + ((self.bandwidth / 2) / 1000000)
+            logger.debug("%s", f"s:{bw_start} e:{bw_end}")
+            Yposition_neg = self.Freq2ScenePos(bw_start).y()
+            Yposition_pos = self.Freq2ScenePos(bw_end).y()
+            poly = QtGui.QPolygonF()
+            poly.append(QtCore.QPointF(15, Yposition_neg))
+            poly.append(QtCore.QPointF(20, Yposition_neg))
+            poly.append(QtCore.QPointF(20, Yposition_pos))
+            poly.append(QtCore.QPointF(15, Yposition_pos))
+            pen = QtGui.QPen()
+            brush = QtGui.QBrush(color)
+            currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
+
+    def determine_step_digits(self):
+        """doc"""
+        return_zoom = {
+            1: (0.0001, 4),
+            2: (0.00025, 4),
+            3: (0.0005, 4),
+            4: (0.001, 3),
+            5: (0.0025, 3),
+            6: (0.005, 3),
+            7: (0.01, 2),
+        }
+        step, digits = return_zoom.get(self.zoom, (0.0001, 4))
+
+        if self.currentBand.start >= 28.0 and self.currentBand.start < 420.0:
+            step = step * 10
+            return (step, digits)
+
+        if self.currentBand.start >= 420.0 and self.currentBand.start < 2300.0:
+            step = step * 100
+
+        return (step, digits)
+
+    def set_band(self, band: str):
+        """doc"""
+        logger.debug("%s", f"{band}")
+        if band != self.currentBand.name:
+            # if savePrevBandZoom:
+            #     self.saveCurrentZoom()
+            self.currentBand = Band(band)
+            # self.zoom = self.savedZoom(band)
+            self.update()
+
+    def clear_all_callsign_from_scene(self):
+        """doc"""
+        for items in self.textItemList:
+            self.bandmap_scene.removeItem(items)
+        self.textItemList.clear()
+        for items in self.lineitemlist:
+            self.bandmap_scene.removeItem(items)
+        self.lineitemlist.clear()
+
+    def clear_freq_mark(self, currentPolygon):
+        """doc"""
+        if currentPolygon:
+            for mark in currentPolygon:
+                self.bandmap_scene.removeItem(mark)
+        currentPolygon.clear()
+
     def spotclicked(self):
         """
         If flrig/rigctld is running on this PC, tell it to tune to the spot freq and change mode.
         Otherwise die gracefully.
         """
+        # new stuff
+        selected_items = self.bandmap_scene.selectedItems()
+        if not selected_items:
+            return
+        selected = selected_items[0]
+        if selected:
+            spotId = selected.property("spotId")
+            spotfreq = int(selected.property("freq") * 1000000)
+            # spotmode = selected.property("mode")
 
+        # old stuff
         try:
+            spot = self.spotdb.getspot_byid(spotId)
+            item = f"xxx {spot.get('activator')} {spot.get('reference')} {int(spot.get('frequency')*1000)} {spot.get('mode')}"
             self.loggable = True
             dateandtime = datetime.utcnow().isoformat(" ")[:19]
             self.time_field.setText(dateandtime.split(" ")[1].replace(":", ""))
             the_date_fields = dateandtime.split(" ")[0].split("-")
             the_date = f"{the_date_fields[0]}{the_date_fields[1]}{the_date_fields[2]}"
             self.date_field.setText(the_date)
-            item = self.listWidget.currentItem()
-            line = item.text().split()
-            self.lastclicked = item.text()
+            line = item.split()
+            self.lastclicked = item
             self.activator_call.setText(line[1])
 
             if "/" in line[1]:
                 basecall = max(line[1].split("/")[0], line[1].split("/")[1], key=len)
             else:
                 basecall = line[1]
 
@@ -480,15 +891,15 @@
                     self.rst_sent.setText("599")
                     self.rst_recieved.setText("599")
                 else:
                     self.rst_sent.setText("59")
                     self.rst_recieved.setText("59")
             except IndexError:
                 self.mode_field.setText("")
-            self.freq_field.setText(f"{line[3]}000")
+            self.freq_field.setText(f"{spotfreq}")
             self.band_field.setText(f"{self.getband(line[3])}M")
             park_info = self.getjson(f"{self.parkurl}{line[2]}")
             if park_info:
                 self.park_name.setText(park_info["name"])
                 self.park_state.setText(park_info["locationName"])
                 self.park_grid.setText(park_info["grid6"])
                 self.park_section.setText(park_info["locationDesc"])
@@ -514,27 +925,28 @@
                     [park_info["latitude"], park_info["longitude"]],
                     popup=f"<i>{park_info['name']}</i>",
                 ).add_to(self.map)
                 data = io.BytesIO()
                 self.map.save(data, close_file=False)
                 self.mapview.setHtml(data.getvalue().decode())
             if self.cat_control is not None:
-                freq = line[3]
-                combfreq = f"{freq}000"
-                self.cat_control.set_vfo(combfreq)
+                combfreq = f"{spotfreq}"
                 try:
                     mode = line[4].upper()
                     if mode == "SSB":
-                        if int(combfreq) > 10000000:
+                        if spotfreq > 10000000:
                             mode = "USB"
                         else:
                             mode = "LSB"
                     self.cat_control.set_mode(mode)
                 except IndexError:
                     pass
+                self.cat_control.set_vfo(
+                    combfreq
+                )  # Set Mode first because some rigs offset vfo based on mode.
             else:
                 self.recheck_cat()
         except ConnectionRefusedError:
             pass
 
     def item_double_clicked(self):
         """If a list item is double clicked a green highlight will be toggled"""
@@ -587,21 +999,23 @@
             return "0"
 
     @staticmethod
     def check_process(name: str) -> bool:
         """checks to see if program of name is in the active process list"""
         for proc in psutil.process_iter():
             if bool(re.match(name, proc.name().lower())):
+                logger.debug("%s found!", name)
                 return True
         return False
 
     def recheck_cat(self):
         """Renegotiate CAT control."""
         local_flrig = self.check_process("flrig")
         local_rigctld = self.check_process("rigctld")
+        local_omnirig = self.check_process("omnirig.exe")
 
         if FORCED_INTERFACE:
             address, port = SERVER_ADDRESS.split(":")
             self.cat_control = CAT(FORCED_INTERFACE, address, int(port))
 
         if self.cat_control is None:
             if local_flrig:
@@ -612,14 +1026,16 @@
                 self.cat_control = CAT("flrig", address, int(port))
             if local_rigctld:
                 if SERVER_ADDRESS:
                     address, port = SERVER_ADDRESS.split(":")
                 else:
                     address, port = "localhost", "4532"
                 self.cat_control = CAT("rigctld", address, int(port))
+            if local_omnirig:
+                self.cat_control = OmniRigClient(OMNI_RIGNUMBER)
 
 
 def install_icons():
     """Install application icons"""
     os.system(
         "xdg-icon-resource install --size 128 --context apps --mode user "
         f"{WORKING_PATH}/data/k6gte-augratin-128.png k6gte-augratin"
@@ -642,18 +1058,21 @@
 logger.info(families)
 window = MainWindow()
 window.setWindowTitle(f"AuGratin v{__version__}")
 window.show()
 window.getspots()
 timer = QtCore.QTimer()
 timer.timeout.connect(window.getspots)
+timer2 = QtCore.QTimer()
+timer2.timeout.connect(window.poll_radio)
 
 
 def run():
     """Start the app"""
     install_icons()
     timer.start(30000)
+    timer2.start(100)
     sys.exit(app.exec())
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `augratin-23.3.7/augratin/data/JetBrainsMono-Regular.ttf` & `augratin-23.5.16/augratin/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `augratin-23.3.7/augratin/data/dialog.ui` & `augratin-23.5.16/augratin/data/dialog.ui`

 * *Files 0% similar despite different names*

#### Comparing `augratin-23.3.7/augratin/data/dialog.ui` & `augratin-23.5.16/augratin/data/dialog.ui`

```diff
@@ -26,31 +26,49 @@
       <string>K6GTE AuGratin</string>
     </property>
     <property name="styleSheet">
       <string notr="true">background-color:rgb(45,45,45);
 color: rgb(211, 215, 207);</string>
     </property>
     <widget class="QWidget" name="centralwidget">
-      <layout class="QGridLayout" name="gridLayout">
-        <item row="0" column="0">
+      <layout class="QVBoxLayout" name="verticalLayout_3">
+        <item>
           <layout class="QHBoxLayout" name="horizontalLayout" stretch="2,0,3">
             <property name="leftMargin">
               <number>9</number>
             </property>
             <property name="topMargin">
               <number>9</number>
             </property>
             <property name="rightMargin">
               <number>9</number>
             </property>
             <property name="bottomMargin">
               <number>9</number>
             </property>
             <item>
-              <layout class="QVBoxLayout" name="verticalLayout" stretch="0,1">
+              <layout class="QVBoxLayout" name="verticalLayout" stretch="0,0,0">
+                <item>
+                  <layout class="QHBoxLayout" name="horizontalLayout_12">
+                    <item>
+                      <widget class="QPushButton" name="zoom_in_button">
+                        <property name="text">
+                          <string>Zoom in</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="zoom_out_button">
+                        <property name="text">
+                          <string>Zoom out</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </item>
                 <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_2" stretch="1,0,0,0,1">
                     <property name="sizeConstraint">
                       <enum>QLayout::SetDefaultConstraint</enum>
                     </property>
                     <item>
                       <spacer name="horizontalSpacer_2">
@@ -229,32 +247,45 @@
                           </size>
                         </property>
                       </spacer>
                     </item>
                   </layout>
                 </item>
                 <item>
-                  <widget class="QListWidget" name="listWidget">
-                    <property name="sizePolicy">
-                      <sizepolicy hsizetype="MinimumExpanding" vsizetype="MinimumExpanding">
-                        <horstretch>0</horstretch>
-                        <verstretch>0</verstretch>
-                      </sizepolicy>
-                    </property>
-                    <property name="maximumSize">
-                      <size>
-                        <width>16777215</width>
-                        <height>16777215</height>
-                      </size>
-                    </property>
-                    <property name="font">
-                      <font>
-                        <family>JetBrains Mono</family>
-                      </font>
+                  <widget class="QScrollArea" name="scrollArea">
+                    <property name="widgetResizable">
+                      <bool>true</bool>
                     </property>
+                    <widget class="QWidget" name="scrollAreaWidgetContents">
+                      <property name="geometry">
+                        <rect>
+                          <x>0</x>
+                          <y>0</y>
+                          <width>393</width>
+                          <height>564</height>
+                        </rect>
+                      </property>
+                      <layout class="QVBoxLayout" name="verticalLayout_4">
+                        <item>
+                          <widget class="QGraphicsView" name="graphicsView">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="font">
+                              <font>
+                                <family>JetBrains Mono</family>
+                              </font>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </widget>
                   </widget>
                 </item>
               </layout>
             </item>
             <item>
               <widget class="Line" name="line">
                 <property name="orientation">
```

### Comparing `augratin-23.3.7/augratin/data/k6gte-augratin-128.png` & `augratin-23.5.16/augratin/data/k6gte-augratin-128.png`

 * *Files identical despite different names*

### Comparing `augratin-23.3.7/augratin/data/k6gte-augratin-32.png` & `augratin-23.5.16/augratin/data/k6gte-augratin-32.png`

 * *Files identical despite different names*

### Comparing `augratin-23.3.7/augratin/data/k6gte-augratin-64.png` & `augratin-23.5.16/augratin/data/k6gte-augratin-64.png`

 * *Files identical despite different names*

### Comparing `augratin-23.3.7/augratin/lib/cat_interface.py` & `augratin-23.5.16/augratin/lib/cat_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import logging
 import socket
 import xmlrpc.client
 
 if __name__ == "__main__":
     print("I'm not the program you are looking for.")
 
+logger = logging.getLogger("__main__")
+
 
 class CAT:
     """CAT control rigctld or flrig"""
 
     def __init__(self, interface: str, host: str, port: int) -> None:
         """
         Computer Aided Tranceiver abstraction class.
@@ -52,105 +54,145 @@
         self.rigctrlsocket = None
         self.interface = interface.lower()
         self.host = host
         self.port = port
         self.online = False
         if self.interface == "flrig":
             target = f"http://{host}:{port}"
-            logging.debug("%s", target)
+            logger.debug("%s", target)
             self.server = xmlrpc.client.ServerProxy(target)
+            self.online = True
         if self.interface == "rigctld":
             self.__initialize_rigctrld()
 
     def __initialize_rigctrld(self):
         try:
             self.rigctrlsocket = socket.socket()
             self.rigctrlsocket.settimeout(0.5)
             self.rigctrlsocket.connect((self.host, self.port))
-            logging.debug("Connected to rigctrld")
+            logger.debug("Connected to rigctrld")
             self.online = True
         except ConnectionRefusedError as exception:
             self.rigctrlsocket = None
             self.online = False
-            logging.debug("%s", exception)
+            logger.debug("%s", exception)
+        except TimeoutError as exception:
+            self.rigctrlsocket = None
+            self.online = False
+            logger.debug("%s", exception)
 
     def get_vfo(self) -> str:
         """Poll the radio for current vfo using the interface"""
         vfo = ""
         if self.interface == "flrig":
             vfo = self.__getvfo_flrig()
-            logging.debug("%s", vfo)
         if self.interface == "rigctld":
             vfo = self.__getvfo_rigctld()
-            logging.debug("%s", vfo)
             if "RPRT -" in vfo:
                 vfo = ""
         return vfo
 
     def __getvfo_flrig(self) -> str:
         """Poll the radio using flrig"""
         try:
             self.online = True
             return self.server.rig.get_vfo()
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("getvfo_flrig: %s", exception)
+            logger.debug("getvfo_flrig: %s", exception)
         return ""
 
     def __getvfo_rigctld(self) -> str:
         """Returns VFO freq returned from rigctld"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"\nf\n")
                 return self.rigctrlsocket.recv(1024).decode().strip()
             except socket.error as exception:
                 self.online = False
-                logging.debug("getvfo_rigctld: %s", exception)
+                logger.debug("getvfo_rigctld: %s", exception)
                 self.rigctrlsocket = None
             return ""
 
         self.__initialize_rigctrld()
         return ""
 
     def get_mode(self) -> str:
         """Returns the current mode filter width of the radio"""
         mode = ""
         if self.interface == "flrig":
             mode = self.__getmode_flrig()
         if self.interface == "rigctld":
             mode = self.__getmode_rigctld()
-        logging.debug("%s", mode)
         return mode
 
     def __getmode_flrig(self) -> str:
         """Returns mode via flrig"""
         try:
             self.online = True
             return self.server.rig.get_mode()
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("%s", exception)
+            logger.debug("%s", exception)
         return ""
 
     def __getmode_rigctld(self) -> str:
         """Returns mode vai rigctld"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"m\n")
                 mode = self.rigctrlsocket.recv(1024).decode()
-                logging.debug("%s", mode)
                 mode = mode.strip().split()[0]
+                logger.debug("%s", mode)
+                return mode
+            except IndexError as exception:
+                logger.debug("%s", exception)
+            except socket.error as exception:
+                self.online = False
+                logger.debug("%s", exception)
+                self.rigctrlsocket = None
+            return ""
+        self.__initialize_rigctrld()
+        return ""
+
+    def get_bw(self):
+        """Get current vfo bandwidth"""
+        if self.interface == "flrig":
+            return self.__getbw_flrig()
+        if self.interface == "rigctld":
+            return self.__getbw_rigctld()
+        return False
+
+    def __getbw_flrig(self):
+        """ccc"""
+        try:
+            self.online = True
+            return self.server.rig.get_bw()
+        except ConnectionRefusedError as exception:
+            self.online = False
+            logger.debug("getbw_flrig: %s", exception)
+            return ""
+
+    def __getbw_rigctld(self):
+        """ccc"""
+        if self.rigctrlsocket:
+            try:
+                self.online = True
+                self.rigctrlsocket.send(b"m\n")
+                mode = self.rigctrlsocket.recv(1024).decode()
+                mode = mode.strip().split()[1]
+                logger.debug("%s", mode)
                 return mode
             except IndexError as exception:
-                logging.debug("%s", exception)
+                logger.debug("%s", exception)
             except socket.error as exception:
                 self.online = False
-                logging.debug("%s", exception)
+                logger.debug("%s", exception)
                 self.rigctrlsocket = None
             return ""
         self.__initialize_rigctrld()
         return ""
 
     def get_power(self):
         """Get power level from rig"""
@@ -162,26 +204,26 @@
 
     def __getpower_flrig(self):
         try:
             self.online = True
             return self.server.rig.get_power()
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("getpower_flrig: %s", exception)
+            logger.debug("getpower_flrig: %s", exception)
             return ""
 
     def __getpower_rigctld(self):
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"l RFPOWER\n")
                 return int(float(self.rigctrlsocket.recv(1024).decode().strip()) * 100)
             except socket.error as exception:
                 self.online = False
-                logging.debug("getpower_rigctld: %s", exception)
+                logger.debug("getpower_rigctld: %s", exception)
                 self.rigctrlsocket = None
             return ""
 
     def get_ptt(self):
         """Get PTT state"""
         if self.interface == "flrig":
             return self.__getptt_flrig()
@@ -192,30 +234,30 @@
     def __getptt_flrig(self):
         """Returns ptt state via flrig"""
         try:
             self.online = True
             return self.server.rig.get_ptt()
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("%s", exception)
+            logger.debug("%s", exception)
         return "0"
 
     def __getptt_rigctld(self):
         """Returns ptt state via rigctld"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(b"t\n")
                 ptt = self.rigctrlsocket.recv(1024).decode()
-                logging.debug("%s", ptt)
+                logger.debug("%s", ptt)
                 ptt = ptt.strip()
                 return ptt
             except socket.error as exception:
                 self.online = False
-                logging.debug("%s", exception)
+                logger.debug("%s", exception)
                 self.rigctrlsocket = None
         return "0"
 
     def set_vfo(self, freq: str) -> bool:
         """Sets the radios vfo"""
         if self.interface == "flrig":
             return self.__setvfo_flrig(freq)
@@ -226,28 +268,28 @@
     def __setvfo_flrig(self, freq: str) -> bool:
         """Sets the radios vfo"""
         try:
             self.online = True
             return self.server.rig.set_frequency(float(freq))
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("setvfo_flrig: %s", exception)
+            logger.debug("setvfo_flrig: %s", exception)
         return False
 
     def __setvfo_rigctld(self, freq: str) -> bool:
         """sets the radios vfo"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(bytes(f"F {freq}\n", "utf-8"))
                 _ = self.rigctrlsocket.recv(1024).decode().strip()
                 return True
             except socket.error as exception:
                 self.online = False
-                logging.debug("setvfo_rigctld: %s", exception)
+                logger.debug("setvfo_rigctld: %s", exception)
                 self.rigctrlsocket = None
                 return False
         self.__initialize_rigctrld()
         return False
 
     def set_mode(self, mode: str) -> bool:
         """Sets the radios mode"""
@@ -260,28 +302,28 @@
     def __setmode_flrig(self, mode: str) -> bool:
         """Sets the radios mode"""
         try:
             self.online = True
             return self.server.rig.set_mode(mode)
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("setmode_flrig: %s", exception)
+            logger.debug("setmode_flrig: %s", exception)
         return False
 
     def __setmode_rigctld(self, mode: str) -> bool:
         """sets the radios mode"""
         if self.rigctrlsocket:
             try:
                 self.online = True
                 self.rigctrlsocket.send(bytes(f"M {mode} 0\n", "utf-8"))
                 _ = self.rigctrlsocket.recv(1024).decode().strip()
                 return True
             except socket.error as exception:
                 self.online = False
-                logging.debug("setmode_rigctld: %s", exception)
+                logger.debug("setmode_rigctld: %s", exception)
                 self.rigctrlsocket = None
                 return False
         self.__initialize_rigctrld()
         return False
 
     def set_power(self, power):
         """Sets the radios power"""
@@ -293,20 +335,89 @@
 
     def __setpower_flrig(self, power):
         try:
             self.online = True
             return self.server.rig.set_power(power)
         except ConnectionRefusedError as exception:
             self.online = False
-            logging.debug("setmode_flrig: %s", exception)
+            logger.debug("setmode_flrig: %s", exception)
             return False
 
     def __setpower_rigctld(self, power):
         if power.isnumeric() and int(power) >= 1 and int(power) <= 100:
             rig_cmd = bytes(f"L RFPOWER {str(float(power) / 100)}\n", "utf-8")
             try:
                 self.online = True
                 self.rigctrlsocket.send(rig_cmd)
                 _ = self.rigctrlsocket.recv(1024).decode().strip()
             except socket.error:
                 self.online = False
                 self.rigctrlsocket = None
+
+    def ptt_on(self):
+        """turn ptt on/off"""
+        if self.interface == "flrig":
+            return self.__ptt_on_flrig()
+        if self.interface == "rigctld":
+            return self.__ptt_on_rigctld()
+        return False
+
+    def __ptt_on_rigctld(self):
+        """Toggle PTT state on"""
+
+        # T, set_ptt 'PTT'
+        # Set 'PTT'.
+        # PTT is a value: ‘0’ (RX), ‘1’ (TX), ‘2’ (TX mic), or ‘3’ (TX data).
+
+        # t, get_ptt
+        # Get 'PTT' status.
+        # Returns PTT as a value in set_ptt above.
+
+        rig_cmd = bytes("T 1\n", "utf-8")
+        logger.debug("%s", f"{rig_cmd}")
+        try:
+            self.online = True
+            self.rigctrlsocket.send(rig_cmd)
+            _ = self.rigctrlsocket.recv(1024).decode().strip()
+        except socket.error:
+            self.online = False
+            self.rigctrlsocket = None
+
+    def __ptt_on_flrig(self):
+        """Toggle PTT state on"""
+        try:
+            self.online = True
+            return self.server.rig.set_ptt(1)
+        except ConnectionRefusedError as exception:
+            self.online = False
+            logger.debug("%s", exception)
+        return "0"
+
+    def ptt_off(self):
+        """turn ptt on/off"""
+        if self.interface == "flrig":
+            return self.__ptt_off_flrig()
+        if self.interface == "rigctld":
+            return self.__ptt_off_rigctld()
+        return False
+
+    def __ptt_off_rigctld(self):
+        """Toggle PTT state off"""
+        rig_cmd = bytes("T 0\n", "utf-8")
+        logger.debug("%s", f"{rig_cmd}")
+        try:
+            self.online = True
+            self.rigctrlsocket.send(rig_cmd)
+            _ = self.rigctrlsocket.recv(1024).decode().strip()
+        except socket.error:
+            self.online = False
+            self.rigctrlsocket = None
+
+    def __ptt_off_flrig(self):
+        """Toggle PTT state off"""
+        try:
+            self.online = True
+            return self.server.rig.set_ptt(0)
+        except ConnectionRefusedError as exception:
+            self.online = False
+            logger.debug("%s", exception)
+        return "0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `augratin-23.3.7/augratin.egg-info/PKG-INFO` & `augratin-23.5.16/augratin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augratin
-Version: 23.3.7
+Version: 23.5.16
 Summary: An aid for POTA hunters
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/augratin
 Project-URL: Bug Tracker, https://github.com/mbridak/augratin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -24,15 +24,15 @@
 
 ![logo](https://github.com/mbridak/augratin/raw/master/augratin/data/k6gte.augratin.svg)
 
 - [AuGratin](#augratin)
   - [Why AuGratin](#why-augratin)
   - [What is AuGratin](#what-is-augratin)
   - [Recent changes](#recent-changes)
-  - [Installing AuGratin](#installing-augratin)
+  - [Installing, Updating, Running, Removing](#installing-updating-running-removing)
   - [Features](#features)
   - [What to do if your map is blank](#what-to-do-if-your-map-is-blank)
   - [CAT control](#cat-control)
 
 ## Why AuGratin
 
 AuGratin is an extension to an earlier program called POTAto. And since it's made from POTAto, I called it AuGratin.
@@ -43,67 +43,80 @@
 [POTA](https://parksontheair.com) is Parks On The Air.
 A year round activity of many amateur radio operators or HAMS.
 The Activator, will set up a radio station in a state/national park and make as many contacts as they can.
 Other Radio Amateurs also known as Hunters or Chasers, will seek out and try to contact as many Activators as they can.
 
 AuGratin allows A [POTA](https://parksontheair.com) Hunter to easily log contacts with Activators.
 It pulls latest [POTA](https://parksontheair.com) spots. Displays them in a compact interface.
-Once a spot is clicked on AuGratin will talk to either rigctld or flrig to change the radio to the correct
+Once a spot is clicked on AuGratin will talk to either rigctld, flrig, or OmniRig to change the radio to the correct
 frequency and mode. It will pre-populate All the fields needed for logging the contact.
 All contacts are stored in an ADIF file in your home directory,
-which you can them import into your normal logging program.
+which you can then import into your normal logging program.
 
 ![screenshot](https://github.com/mbridak/augratin/raw/master/pic/screenshot.png)
 
 ## Recent changes
 
+- [23-5-15] Start big code changes to impliment better bandmap.
+- [23-3-28] Merged in changes from @barryshaffer KK7JXG to add support for Omnirig on windows.
 - [23-3-7] Reduced network timeout for spot pulls from 15 to 5 seconds. Safer dictionary key access.
 - [23-2-17] Repackaged for PyPi and pip install
 
-## Installing AuGratin
+## Installing, Updating, Running, Removing
 
 ```bash
+# install
 pip install augratin
+
+# update
+pip install -U augratin
+
+# remove
+pip uninstall augratin
+
+# running
+augratin
 ```
 
 ## Features
 
-- You can filter spots by band and or mode.
+- Shows spots on a band map
+- You can filter spots by mode.
 - Pulls in park and activator information.
-- Tunes your radio with flrig or rigctld to the activator and sets the mode automatically.
-- Double clicked spots adds Activator to a persistent watchlist.
+- Clicked spots, tune your radio with flrig, rigctld or OmniRig to the activator and sets the mode automatically.
+- ~~Double clicked spots adds Activator to a persistent watchlist.~~
 - Displays bearing to contact.
 
 When you press the "Log it" button the adif information is appended to `POTA_Contacts.adi` in your home folder.
 
 ## What to do if your map is blank
 
 Not sure why, but the map may not work if you let pip install PyQt5 and PyQtWebEngine automatically. If your map is blank, try:
 
 ```bash
 pip uninstall PyQt5
-Pip uninstall PyQtWebEngine
+pip uninstall PyQtWebEngine
 ```
 
 Then install them through your package manager.
 
 ```bash
 #fedora
 sudo dnf install python3-qt5 python3-qt5-webengine
 
 #ubuntu
 sudo apt install python3-pyqt5 python3-pyqt5.qtwebengine
 ```
 
 ## CAT control
 
-If no command line options are given, the program will check if either flrig
-or rigctld are running on the computer. It will setup CAT control to which
-ever it finds first.
+If no command line options are given, the program will check if either flrig, rigctld or OmniRig are running on the computer. It will setup CAT control to whichever it finds first.
 
 You can force it to use either with commandline options.
 
 `-r` will force rigctld with default host:port of localhost:4532.
 
 `-f` will force flrig with default host:port of localhost:12345.
 
+`-2` will force 'Rig2' with OmniRig.
+
 `-s SERVER:PORT` will specify a non-standard host and port.
```

### Comparing `augratin-23.3.7/augratin.egg-info/SOURCES.txt` & `augratin-23.5.16/augratin.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 augratin/data/dialog.ui
 augratin/data/k6gte-augratin-128.png
 augratin/data/k6gte-augratin-32.png
 augratin/data/k6gte-augratin-64.png
 augratin/data/k6gte-augratin.desktop
 augratin/lib/__init__.py
 augratin/lib/cat_interface.py
+augratin/lib/omnirig_interface.py
 augratin/lib/version.py
```

### Comparing `augratin-23.3.7/pyproject.toml` & `augratin-23.5.16/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "augratin" 
-version = "23.3.7"
+version = "23.5.16"
 description = "An aid for POTA hunters"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
+
 dependencies = [
     "PyQt5",
     "PyQtWebEngine",
     "requests",
     "psutil",
     "folium",
+    "pywin32; os_name == 'nt'",
 ]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Environment :: X11 Applications :: Qt",
     "Operating System :: POSIX :: Linux",
     "Intended Audience :: End Users/Desktop",
```

