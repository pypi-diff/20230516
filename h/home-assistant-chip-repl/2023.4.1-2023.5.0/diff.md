# Comparing `tmp/home_assistant_chip_repl-2023.4.1-py3-none-any.whl.zip` & `tmp/home_assistant_chip_repl-2023.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 18071 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3939 b- defN 23-Apr-18 07:41 chip/ChipReplStartup.py
--rwxr-xr-x  2.0 unx    43771 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.data/scripts/chip-device-ctrl
--rwxr-xr-x  2.0 unx     1066 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.data/scripts/chip-repl
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      627 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      799 b- defN 23-Apr-18 07:41 home_assistant_chip_repl-2023.4.1.dist-info/RECORD
-8 files, 61656 bytes uncompressed, 16639 bytes compressed:  73.0%
+Zip file size: 29892 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    36797 b- defN 23-May-16 15:28 chip/ChipBluezMgr.py
+-rw-r--r--  2.0 unx    21363 b- defN 23-May-16 15:28 chip/ChipCoreBluetoothMgr.py
+-rw-r--r--  2.0 unx     3738 b- defN 23-May-16 15:28 chip/ChipReplStartup.py
+-rwxr-xr-x  2.0 unx    43792 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.data/scripts/chip-device-ctrl
+-rwxr-xr-x  2.0 unx     1051 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.data/scripts/chip-repl
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      690 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      963 b- defN 23-May-16 15:28 home_assistant_chip_repl-2023.5.0.dist-info/RECORD
+10 files, 119848 bytes uncompressed, 28212 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
+Filename: chip/ChipBluezMgr.py
+Comment: 
+
+Filename: chip/ChipCoreBluetoothMgr.py
+Comment: 
+
 Filename: chip/ChipReplStartup.py
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.data/scripts/chip-device-ctrl
+Filename: home_assistant_chip_repl-2023.5.0.data/scripts/chip-device-ctrl
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.data/scripts/chip-repl
+Filename: home_assistant_chip_repl-2023.5.0.data/scripts/chip-repl
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.dist-info/LICENSE
+Filename: home_assistant_chip_repl-2023.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.dist-info/METADATA
+Filename: home_assistant_chip_repl-2023.5.0.dist-info/METADATA
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.dist-info/WHEEL
+Filename: home_assistant_chip_repl-2023.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.dist-info/top_level.txt
+Filename: home_assistant_chip_repl-2023.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: home_assistant_chip_repl-2023.4.1.dist-info/RECORD
+Filename: home_assistant_chip_repl-2023.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chip/ChipReplStartup.py

```diff
@@ -1,26 +1,21 @@
-from rich import print
-from rich.pretty import pprint
-from rich import pretty
-from rich import inspect
-from rich.console import Console
-import logging
-from chip import ChipDeviceCtrl
-import chip.clusters as Clusters
-from chip.ChipStack import *
-import coloredlogs
-import chip.logging
 import argparse
+import atexit
 import builtins
-import chip.FabricAdmin
+import logging
+
 import chip.CertificateAuthority
-import chip.native
 import chip.discovery
-from chip.utils import CommissioningBuildingBlocks
-import atexit
+import chip.FabricAdmin
+import chip.logging
+import chip.native
+import coloredlogs
+from chip.ChipStack import *
+from rich import inspect, pretty
+from rich.console import Console
 
 _fabricAdmins = None
 
 
 def ReplInit(debug):
     #
     # Install the pretty printer that rich provides to replace the existing
@@ -29,22 +24,22 @@
     pretty.install(indent_guides=True, expand_all=True)
 
     console = Console()
 
     console.rule('Matter REPL')
     console.print('''
             [bold blue]
-    
+
             Welcome to the Matter Python REPL!
-    
+
             For help, please type [/][bold green]matterhelp()[/][bold blue]
-    
+
             To get more information on a particular object/class, you can pass
             that into [bold green]matterhelp()[/][bold blue] as well.
-    
+
             ''')
     console.rule()
 
     coloredlogs.install(level='DEBUG')
     chip.logging.RedirectToPythonLogging()
 
     if debug:
```

## Comparing `home_assistant_chip_repl-2023.4.1.data/scripts/chip-device-ctrl` & `home_assistant_chip_repl-2023.5.0.data/scripts/chip-device-ctrl`

 * *Files 2% similar despite different names*

```diff
@@ -19,47 +19,38 @@
 #
 
 #
 #    @file
 #      This file implements the Python-based Chip Device Controller Shell.
 #
 
-from __future__ import absolute_import
-from __future__ import print_function
-from sqlite3 import adapt
-from chip import ChipDeviceCtrl
-from chip import clusters as Clusters
-from chip import FabricAdmin
-from chip import ChipStack
-from chip import ChipCommissionableNodeCtrl
-from chip import exceptions
-from chip import native
+from __future__ import absolute_import, print_function
+
 import argparse
+import base64
 import ctypes
-import sys
+import logging
 import os
 import platform
 import random
-from optparse import OptionParser, OptionValueError
 import shlex
-import base64
+import string
+import sys
 import textwrap
 import time
-import string
 import traceback
-from cmd import Cmd
-from chip.setup_payload import SetupPayload
-import deprecation
 import warnings
-import logging
-from rich import print
-from rich.pretty import pprint
-from rich import pretty
-import coloredlogs
+from cmd import Cmd
+from optparse import OptionParser, OptionValueError
+
 import chip.logging
+import coloredlogs
+from chip import ChipCommissionableNodeCtrl, ChipStack, FabricAdmin, exceptions, native
+from chip.setup_payload import SetupPayload
+from rich import pretty, print
 
 # Extend sys.path with one or more directories, relative to the location of the
 # running script, in which the chip package might be found .  This makes it
 # possible to run the device manager shell from a non-standard install location,
 # as well as directly from its location the CHIP source tree.
 #
 # Note that relative package locations are prepended to sys.path so as to give
@@ -181,15 +172,17 @@
 
         DeviceMgrCmd.command_names.sort()
 
         self.bleMgr = None
 
         self.chipStack = ChipStack.ChipStack(
             bluetoothAdapter=bluetoothAdapter, persistentStoragePath='/tmp/chip-device-ctrl-storage.json')
-        self.fabricAdmin = FabricAdmin.FabricAdmin(0xFFF1)
+        self.certificateAuthorityManager = chip.CertificateAuthority.CertificateAuthorityManager(chipStack=self.chipStack)
+        self.certificateAuthority = self.certificateAuthorityManager.NewCertificateAuthority()
+        self.fabricAdmin = self.certificateAuthority.NewFabricAdmin(vendorId=0xFFF1, fabricId=1)
         self.devCtrl = self.fabricAdmin.NewController(
             nodeId=controllerNodeId, useTestCommissioner=True)
 
         self.commissionableNodeCtrl = ChipCommissionableNodeCtrl.ChipCommissionableNodeController(
             self.chipStack)
 
         # If we are on Linux and user selects non-default bluetooth adapter.
@@ -890,15 +883,15 @@
             if len(args) == 1 and args[0] == '?':
                 print('\n'.join(all_attrs.keys()))
             elif len(args) == 2 and args[0] == '?':
                 if args[1] not in all_attrs:
                     raise exceptions.UnknownCluster(args[1])
                 cluster_attrs = all_attrs.get(args[1], {})
                 print('\n'.join(["{}: {}".format(key, cluster_attrs[key]["type"])
-                      for key in cluster_attrs.keys() if cluster_attrs[key].get("writable", False)]))
+                                 for key in cluster_attrs.keys() if cluster_attrs[key].get("writable", False)]))
             elif len(args) == 6:
                 if args[0] not in all_attrs:
                     raise exceptions.UnknownCluster(args[0])
                 attribute_type = all_attrs.get(args[0], {}).get(
                     args[1], {}).get("type", None)
                 self.replHint = f"await devCtrl.WriteAttribute({int(args[2])}, [({int(args[3])}, Clusters.{args[0]}.Attributes.{args[1]}(value={repr(ParseValueWithType(args[5], attribute_type))}))])"
                 res = self.devCtrl.ZCLWriteAttribute(args[0], args[1], int(
```

## Comparing `home_assistant_chip_repl-2023.4.1.data/scripts/chip-repl` & `home_assistant_chip_repl-2023.5.0.data/scripts/chip-repl`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 
+import sys
+
 import IPython
 from traitlets.config import Config
-import builtins
-import sys
 
 
 def main():
     c = Config()
     c.InteractiveShellApp.exec_lines = [
         "import pkgutil",
         "module = pkgutil.get_loader('chip.ChipReplStartup')",
```

## Comparing `home_assistant_chip_repl-2023.4.1.dist-info/LICENSE` & `home_assistant_chip_repl-2023.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_repl-2023.4.1.dist-info/METADATA` & `home_assistant_chip_repl-2023.5.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: home-assistant-chip-repl
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Python-base APIs and tools for CHIP.
 Home-page: https://github.com/project-chip/connectedhomeip
 License: Apache
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Requires-Dist: coloredlogs
+Requires-Dist: dbus-python (==1.2.18)
 Requires-Dist: ipykernel
 Requires-Dist: ipython (!=8.1.0)
 Requires-Dist: mobly
+Requires-Dist: pygobject
 Requires-Dist: rich
 
 UNKNOWN
```

