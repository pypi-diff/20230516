# Comparing `tmp/ioddcomcheckergui-1.6.5.post4-py3-none-any.whl.zip` & `tmp/ioddcomcheckergui-1.6.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 5874 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     5727 b- defN 23-Apr-13 06:04 siogeen/tools/gui/IoddComChecker.py
--rw-rw-r--  2.0 unx      468 b- defN 23-Apr-13 06:04 siogeen/tools/gui/__init__.py
--rw-rw-r--  2.0 unx      732 b- defN 23-Apr-13 06:04 IoddComCheckerGui-1.6.5.post4.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     5197 b- defN 23-Apr-13 06:04 IoddComCheckerGui-1.6.5.post4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 06:04 IoddComCheckerGui-1.6.5.post4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-13 06:04 IoddComCheckerGui-1.6.5.post4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      645 b- defN 23-Apr-13 06:04 IoddComCheckerGui-1.6.5.post4.dist-info/RECORD
-7 files, 12869 bytes uncompressed, 4706 bytes compressed:  63.4%
+Zip file size: 6382 bytes, number of entries: 11
+drwx------  2.0 unx        0 b- stor 23-May-16 03:57 ioddcomcheckergui-1.6.8.dist-info/
+-rw-rw-r--  2.0 unx     5069 b- defF 23-May-16 01:50 ioddcomcheckergui-1.6.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defF 23-May-16 01:50 ioddcomcheckergui-1.6.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      615 b- defF 23-May-16 03:58 ioddcomcheckergui-1.6.8.dist-info/RECORD
+-rw-rw-r--  2.0 unx        8 b- defF 23-May-16 01:50 ioddcomcheckergui-1.6.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      732 b- defF 23-May-16 01:50 ioddcomcheckergui-1.6.8.dist-info/LICENSE.txt
+drwx------  2.0 unx        0 b- stor 23-May-16 03:57 siogeen/
+drwx------  2.0 unx        0 b- stor 23-May-16 03:57 siogeen/tools/
+drwx------  2.0 unx        0 b- stor 23-May-16 03:57 siogeen/tools/gui/
+-rw-rw-r--  2.0 unx     5771 b- defF 23-May-16 01:50 siogeen/tools/gui/IoddComChecker.py
+-rw-rw-r--  2.0 unx      468 b- defF 23-May-16 01:50 siogeen/tools/gui/__init__.py
+11 files, 12755 bytes uncompressed, 4822 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
-Filename: siogeen/tools/gui/IoddComChecker.py
+Filename: ioddcomcheckergui-1.6.8.dist-info/
 Comment: 
 
-Filename: siogeen/tools/gui/__init__.py
+Filename: ioddcomcheckergui-1.6.8.dist-info/METADATA
+Comment: 
+
+Filename: ioddcomcheckergui-1.6.8.dist-info/WHEEL
+Comment: 
+
+Filename: ioddcomcheckergui-1.6.8.dist-info/RECORD
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post4.dist-info/LICENSE.txt
+Filename: ioddcomcheckergui-1.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post4.dist-info/METADATA
+Filename: ioddcomcheckergui-1.6.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post4.dist-info/WHEEL
+Filename: siogeen/
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post4.dist-info/top_level.txt
+Filename: siogeen/tools/
 Comment: 
 
-Filename: IoddComCheckerGui-1.6.5.post4.dist-info/RECORD
+Filename: siogeen/tools/gui/
+Comment: 
+
+Filename: siogeen/tools/gui/IoddComChecker.py
+Comment: 
+
+Filename: siogeen/tools/gui/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## siogeen/tools/gui/IoddComChecker.py

```diff
@@ -4,17 +4,20 @@
 
 Created on 14.11.2022
 
 @author: Reimund Renner
 '''
 
 import webbrowser
+import os
 
 from threading import Thread
 
+os.environ["KIVY_NO_CONSOLELOG"] = "1"
+
 from kivymd.app import MDApp as App
 from kivymd.uix.button import MDFillRoundFlatButton as Button
 #from kivymd.uix.tooltip.tooltip import MDTooltip
 from kivymd.uix.button import MDFloatingActionButtonSpeedDial as FloatingButton
 from kivymd.uix.textfield.textfield import MDTextFieldRect as TextInput
 from kivymd.uix.selectioncontrol.selectioncontrol import MDCheckbox as CheckBox
 #from kivymd.uix.behaviors.toggle_behavior import MDToggleButton as ToggleButton
@@ -26,15 +29,15 @@
 from kivymd.uix.floatlayout import MDFloatLayout as FloatLayout
 from kivymd.uix.stacklayout import MDStackLayout as StackLayout
 from kivy.core.clipboard import Clipboard
 from kivy.clock import Clock
 
 from siogeen.tools import IoddComChecker
 
-__version__ = "1.6.5.post4"
+__version__ = "1.6.8"
 
 class IoddComCheckerGui(App):
     def build(self):
         if __version__ == IoddComChecker.__version__:
             self.title = 'IoddComChecker ' + IoddComChecker.__version__
         else:
             self.title = f'IoddComChecker {IoddComChecker.__version__}' \
```

## Comparing `IoddComCheckerGui-1.6.5.post4.dist-info/LICENSE.txt` & `ioddcomcheckergui-1.6.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComCheckerGui-1.6.5.post4.dist-info/METADATA` & `ioddcomcheckergui-1.6.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoddComCheckerGui
-Version: 1.6.5.post4
+Version: 1.6.8
 Summary: IoddCom IO-Link master checker Gui
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: IoddComChecker (>=1.6.5.post4)
+Requires-Dist: IoddComChecker (>=1.6.8)
 Requires-Dist: kivymd
 
 IoddComCheckerGui - IoddComChecker GUI
 ======================================
 
 .. _IoddComChecker: /project/IoddComChecker
 
@@ -67,64 +67,60 @@
 **Copyright 2017-2023 Siogeen UG** (limited liability)
 
 .. _request: https://siogeen.com/#contact
 
 Supported Platforms
 ~~~~~~~~~~~~~~~~~~~
 
-============= ===================== ===================
-**OS**         Python 2.7, 3.4-3.5   Python 3.6 - 3.11
-============= ===================== ===================
-**Windows**     [1]_                   x
-**Linux**       [1]_                   x
-**Raspberry**   [1]_                  3.7, 3.9
-**macOS**       [1]_                  3.8-3.11 [2]_
-============= ===================== ===================
+========================= ===================== ===================
+**OS**                    Python 2.7, 3.4-3.5   Python 3.6 - 3.11
+========================= ===================== ===================
+**Windows**                 [1]_                   x
+**Linux x86/x64**           [1]_                   x
+**Linux Arm (Raspberry)**   [1]_                  3.7-3.11
+**macOS**                   [1]_                  3.8-3.11
+========================= ===================== ===================
 
 .. [1] IoddCom for Python 2.7, 3.4 - 3.5 on request_.
-.. [2] IoddCom for macOS: Intel chip only, yet
 
 Support for other platforms on request_.
 
 Supported operating systems and IO-Link masters
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Table of supported IO-Link masters for specific operating systems (OS):
 
 +---------------------------------+---------------------------------------------------+
 | Master                          | supported OS                                      |
 |                                 +---------+----------+--------------+---------------+
-|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [3]_ |
+|                                 | Windows |  Linux   | Raspberry Pi | macOS 64 [2]_ |
 +=================================+=========+==========+==============+===============+
-| TMG-USB based masters [4]_ [5]_ |   x     |    x     |    x         |    x          |
+| TMG-USB based masters [3]_      |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
-| TMG ethernet based masters [6]_ |   x     |    x     |    x         |    x          |
+| TMG ethernet based masters [4]_ |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
-| ifm ethernet based masters [7]_ |   x     |    x     |    x         |    x          |
+| ifm ethernet based masters [5]_ |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
-| ifm USB based masters [8]_      |   x     |    x     |    x         |    x          |
+| ifm USB based masters [6]_      |   x     |    x     |    x         |    x          |
 +---------------------------------+---------+----------+--------------+---------------+
 
 For Windows, Linux and Raspberry Pi both, 32-bit and 64-bit versions are available.
 
-.. [3] For macOS 10.15+ Python 3.8-3.11 with Intel chip (others on request)
+.. [2] For macOS 13+
 
-.. [4] Driver not included. Need driver from manufacturer or install DTM driver
-       for the device.
+.. [3] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
 
-.. [5] For example: Baumer, Leuze, Pepperl+Fuchs, SICK AG, Turck
+.. [4] For Example: Balluff, Belden, Murrelektronik, Pepperl+Fuchs, Wenglor
 
-.. [6] For Example: Balluff, Belden, Murrelektronik, Pepperl+Fuchs, Wenglor
-
-.. [7] All ifm IO-Link masters AL1xxx should be supported. Functionality depends on
+.. [5] All ifm IO-Link masters AL1xxx should be supported. Functionality depends on
        master type.
        The following functions are missing yet: PD streaming, master data storage read/write,
        master commands, PD valid status
 
-.. [8] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
-       like for [7]_
+.. [6] Experimental ifm USB IO-Link master AL1060 support. Special functions missing
+       like for [5]_
 
 Not supported masters:
 
 * RevolutionPi RevPi masters
 * Pepperl & Fuchs comtrol masters
 * Baumer USB-C and senscontrol masters
 * Germbedded masters
```

