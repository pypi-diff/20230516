# Comparing `tmp/ioddcomchecker-1.6.5.post4-cp39-cp39-win_amd64.whl.zip` & `tmp/ioddcomchecker-1.6.8-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 57161 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      732 b- defN 23-Apr-13 06:21 siogeen/LICENSE.txt
--rw-rw-rw-  2.0 fat   117760 b- defN 23-Apr-13 06:22 siogeen/tools/IoddComChecker.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      462 b- defN 23-Apr-13 06:21 siogeen/tools/__init__.py
--rw-rw-rw-  2.0 fat     1188 b- defN 23-Apr-13 06:21 siogeen/tools/cli/IoddComChecker.py
--rw-rw-rw-  2.0 fat      732 b- defN 23-Apr-13 06:22 IoddComChecker-1.6.5.post4.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     5625 b- defN 23-Apr-13 06:22 IoddComChecker-1.6.5.post4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 06:22 IoddComChecker-1.6.5.post4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-13 06:22 IoddComChecker-1.6.5.post4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      808 b- defN 23-Apr-13 06:22 IoddComChecker-1.6.5.post4.dist-info/RECORD
-9 files, 127415 bytes uncompressed, 55747 bytes compressed:  56.2%
+Zip file size: 57656 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      732 b- defN 23-May-16 04:32 siogeen/LICENSE.txt
+-rw-rw-rw-  2.0 fat   118784 b- defN 23-May-16 04:32 siogeen/tools/IoddComChecker.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      462 b- defN 23-May-16 04:32 siogeen/tools/__init__.py
+-rw-rw-rw-  2.0 fat     1401 b- defN 23-May-16 04:32 siogeen/tools/cli/IoddComChecker.py
+-rw-rw-rw-  2.0 fat      732 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5499 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      778 b- defN 23-May-16 04:32 ioddcomchecker-1.6.8.dist-info/RECORD
+9 files, 128496 bytes uncompressed, 56302 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: siogeen/tools/__init__.py
 Comment: 
 
 Filename: siogeen/tools/cli/IoddComChecker.py
 Comment: 
 
-Filename: IoddComChecker-1.6.5.post4.dist-info/LICENSE.txt
+Filename: ioddcomchecker-1.6.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: IoddComChecker-1.6.5.post4.dist-info/METADATA
+Filename: ioddcomchecker-1.6.8.dist-info/METADATA
 Comment: 
 
-Filename: IoddComChecker-1.6.5.post4.dist-info/WHEEL
+Filename: ioddcomchecker-1.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: IoddComChecker-1.6.5.post4.dist-info/top_level.txt
+Filename: ioddcomchecker-1.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: IoddComChecker-1.6.5.post4.dist-info/RECORD
+Filename: ioddcomchecker-1.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siogeen/tools/cli/IoddComChecker.py

```diff
@@ -5,31 +5,38 @@
 Created on 4.1.2023
 
 @author: Reimund Renner
 '''
 
 import argparse
 
-from siogeen.tools import IoddComChecker
-
-if __name__ == '__main__':
+def getParser():
     parser = argparse.ArgumentParser(
         description='Check for IO-Link masters and devices',
-        epilog='Example: %(prog)s -a 10.0.0.17 -a 10.0.0.19 --auto')
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        epilog='''Examples:
+  python -m siogeen.tools.cli.IoddComChecker
+  python -m siogeen.tools.cli.IoddComChecker -a 10.0.0.17 -a 10.0.0.19 --auto''')
     parser.add_argument("-a", "--address",action='append',
                         help="specify one or more master addresses (default all)")
     parser.add_argument("--auto", action='store_true',
                         help="activate master ports if all are disabled")
     parser.add_argument("--version", action='store_true',
         help="print version")
 
+    return parser
+
+if __name__ == '__main__':
+    parser = getParser()
     args = parser.parse_args()
     #args = parser.parse_args(['--auto'])
     #args = parser.parse_args(['-a', '/dev/ttyUSB0'])
     #args = parser.parse_args(['-a', '192.168.178.77'])
     #args = parser.parse_args(['-a', '192.168.178.77', '-a', '192.168.178.73'])
     #args = parser.parse_args(['-a', '192.168.178.77', '--auto'])
 
+    from siogeen.tools import IoddComChecker
+
     if args.version:
         print(f"IoddComChecker {IoddComChecker.__version__}")
     else:
         IoddComChecker.check(args.address, args.auto)
```

## Comparing `IoddComChecker-1.6.5.post4.dist-info/LICENSE.txt` & `ioddcomchecker-1.6.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `IoddComChecker-1.6.5.post4.dist-info/METADATA` & `ioddcomchecker-1.6.8.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: IoddComChecker
-Version: 1.6.5.post4
+Name: ioddcomchecker
+Version: 1.6.8
 Summary: IoddCom IO-Link master checker
 Home-page: https://siogeen.com
 Author: Reimund Renner
 Author-email: reimund@siogeen.com
 License: proprietary and confidential
 Project-URL: Documentation, https://siogeen.com/doc/
 Project-URL: Help Desk, https://siogeen.com/helpdesk/
@@ -28,15 +28,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: IoddComBase (>=1.6.4)
+Requires-Dist: ioddcombase (>=1.6.8)
 Requires-Dist: dict2obj
 
 IoddComChecker - IoddCom Checker
 ================================
 
 .. _IoddComCheckerGui: /project/IoddComCheckerGui
 
@@ -75,64 +75,60 @@
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

