# Comparing `tmp/UEVaultManager-1.1.1.7.tar.gz` & `tmp/UEVaultManager-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.1.1.7.tar", last modified: Thu May 11 17:12:09 2023, max compression
+gzip compressed data, was "UEVaultManager-1.3.0.tar", last modified: Tue May 16 17:12:04 2023, max compression
```

## Comparing `UEVaultManager-1.1.1.7.tar` & `UEVaultManager-1.3.0.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.988126 UEVaultManager-1.1.1.7/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.1.1.7/LICENSE
--rw-rw-rw-   0        0        0     5637 2023-05-11 17:12:09.987145 UEVaultManager-1.1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4865 2023-05-11 16:36:35.000000 UEVaultManager-1.1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.884325 UEVaultManager-1.1.1.7/UEVaultManager/
--rw-rw-rw-   0        0        0      721 2023-05-11 17:06:22.000000 UEVaultManager-1.1.1.7/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.914641 UEVaultManager-1.1.1.7/UEVaultManager/api/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    20251 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0      884 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/api/lgd.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.916640 UEVaultManager-1.1.1.7/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0    61539 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    42168 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.918639 UEVaultManager-1.1.1.7/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.921641 UEVaultManager-1.1.1.7/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38025 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.929000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6686 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    22112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/lgndry.py
--rw-rw-rw-   0        0        0     5528 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3040 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.945793 UEVaultManager-1.1.1.7/UEVaultManager/models/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     1351 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5078 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     1334 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/gql.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30499 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.948793 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.965164 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     4112 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6419 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    23010 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0     7778 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0     1124 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    10585 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2104 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     4910 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    24626 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0     2102 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9293 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     1471 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.984989 UEVaultManager-1.1.1.7/UEVaultManager/utils/
--rw-rw-rw-   0        0        0        0 2023-05-11 14:38:28.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3455 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5577 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1075 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10270 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      309 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      562 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     5891 2023-05-11 14:38:29.000000 UEVaultManager-1.1.1.7/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-05-11 17:12:09.905996 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     5637 2023-05-11 17:12:09.000000 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2104 2023-05-11 17:12:09.000000 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 17:12:09.000000 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-11 17:12:09.000000 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-11 17:12:09.000000 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-11 17:12:09.000000 UEVaultManager-1.1.1.7/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 17:12:09.988126 UEVaultManager-1.1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2174 2023-05-11 16:14:47.000000 UEVaultManager-1.1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.161909 UEVaultManager-1.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5779 2023-05-16 17:12:04.160909 UEVaultManager-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4948 2023-05-15 08:41:23.000000 UEVaultManager-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.002132 UEVaultManager-1.3.0/UEVaultManager/
+-rw-rw-rw-   0        0        0      780 2023-05-16 17:05:23.000000 UEVaultManager-1.3.0/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.038102 UEVaultManager-1.3.0/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25381 2023-05-16 09:42:26.000000 UEVaultManager-1.3.0/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3095 2023-05-16 14:13:33.000000 UEVaultManager-1.3.0/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.040471 UEVaultManager-1.3.0/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0    65456 2023-05-16 16:56:25.000000 UEVaultManager-1.3.0/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47084 2023-05-16 14:13:33.000000 UEVaultManager-1.3.0/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.041482 UEVaultManager-1.3.0/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.056504 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38030 2023-05-15 06:30:52.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.075255 UEVaultManager-1.3.0/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23055 2023-05-16 09:53:50.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3122 2023-05-15 06:51:32.000000 UEVaultManager-1.3.0/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.099423 UEVaultManager-1.3.0/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4478 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     1367 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5094 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0       72 2023-05-11 14:38:28.000000 UEVaultManager-1.3.0/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     1350 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/models/gql.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.3.0/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30505 2023-05-15 06:30:52.000000 UEVaultManager-1.3.0/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.107422 UEVaultManager-1.3.0/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:45:45.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0      949 2023-05-14 16:45:45.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.138059 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6042 2023-05-16 16:41:50.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4571 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6834 2023-05-16 13:36:33.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    24480 2023-05-16 16:57:32.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    10159 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0     1516 2023-05-15 10:14:37.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14228 2023-05-15 10:17:32.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2253 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     5056 2023-05-15 10:19:15.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    35352 2023-05-16 16:56:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-16 16:57:06.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-15 10:13:54.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-14 16:44:57.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0    12574 2023-05-16 15:35:58.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     1781 2023-05-16 14:18:21.000000 UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.159910 UEVaultManager-1.3.0/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3478 2023-05-15 08:49:51.000000 UEVaultManager-1.3.0/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5628 2023-05-16 07:17:45.000000 UEVaultManager-1.3.0/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.3.0/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10286 2023-05-15 06:33:02.000000 UEVaultManager-1.3.0/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.3.0/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.3.0/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7214 2023-05-15 10:15:19.000000 UEVaultManager-1.3.0/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:12:04.024092 UEVaultManager-1.3.0/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     5779 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2219 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 17:12:03.000000 UEVaultManager-1.3.0/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 17:12:04.161909 UEVaultManager-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2372 2023-05-16 08:14:34.000000 UEVaultManager-1.3.0/setup.py
```

### Comparing `UEVaultManager-1.1.1.7/LICENSE` & `UEVaultManager-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/PKG-INFO` & `UEVaultManager-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1.7
+Version: 1.3.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
+[![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
@@ -61,7 +62,10 @@
   * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
   * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
+
+
+ UEVaultManager ## version:1.3.0 ## codename: Andromeda
```

### Comparing `UEVaultManager-1.1.1.7/README.md` & `UEVaultManager-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Welcome to UEVaultManager
 ==========================================
+[![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/__init__.py` & `UEVaultManager-1.3.0/UEVaultManager/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-"""UEVaultManager"""
+# coding=utf-8
+"""
+UEVaultManager setup file.
+"""
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.1.1.7'
-# Pegasus Seiya
-# Dragon Shiryu
-# Cygnus Hyoga
-__codename__ = 'Cygnus+1'
-# Andromeda Shun
-# Phoenix Ikki
-# Leo Aiolia
-# Virgo Shaka
-# Libra Dohko
-# Scorpio Milo
-# Sagittarius Aiolos
-# Capricorn Shura
-# Aquarius Camus
-# Pisces Aphrodite
+__version__ = '1.3.0'
+# 0 Pegasus Seiya
+# 1 Dragon Shiryu
+# 2 Cygnus Hyoga
+# 3 Andromeda Shun
+__codename__ = 'Andromeda'
+# 4 Phoenix Ikki
+# 5 Leo Aiolia
+# 5 Virgo Shaka
+# 6 Libra Dohko
+# 7 Scorpio Milo
+# 8 Sagittarius Aiolos
+# 9 Capricorn Shura
+# 10 Aquarius Camus
+# 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
 __author_email__ = 'laurent@gameamea.com'
 __description__ = 'Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine'
 __copyright__ = f'{year} {__author__}'
 __license__ = 'GPL-3'
 __url__ = 'https://github.com/LaurentOngaro/UEVaultManager'
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/api/egs.py` & `UEVaultManager-1.3.0/UEVaultManager/api/egs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,66 @@
-# !/usr/bin/env python
 # coding: utf-8
-
+"""
+Implementation for:
+- EPCAPI : Epic Games Client API
+- GrabResult : Enum for the result of grabbing a page.
+- create_empty_assets_extras : Creates an empty asset extras dict.
+"""
 import logging
 import re
 import urllib.parse
 from enum import Enum
 
 import requests
 import requests.adapters
 from bs4 import BeautifulSoup
 from requests.auth import HTTPBasicAuth
 
 from UEVaultManager.models.exceptions import InvalidCredentialsError
 
 
 class GrabResult(Enum):
+    """
+    Enum for the result of grabbing a page.
+    """
     NO_ERROR = 0
     INCONSISTANT_DATA = 1
     PAGE_NOT_FOUND = 2
     CONTENT_NOT_FOUND = 3
+    TIMEOUT = 4
 
 
 def create_empty_assets_extras(asset_name: str) -> dict:
+    """
+    Creates an empty asset extras dict.
+    :param asset_name:  The name of the asset.
+    :return: The empty asset extras dict.
+     """
     return {
         'asset_name': asset_name,
         'asset_url': '',
         'asset_name_in_url': '',
         'price': 0,
+        'discount_price': 0,
         'review': 0,
         'purchased': False,
         'supported_versions': '',
         'page_title': '',
-        'grab_result': GrabResult.NO_ERROR.name
+        'grab_result': GrabResult.NO_ERROR.name,
+        'on_sale': False
     }
 
 
 class EPCAPI:
+    """
+    Epic Games Client API
+    :param lc: The language code.
+    :param cc: The country code.
+    :param timeout: The timeout for requests.
+    """
     _user_agent = 'UELauncher/11.0.1-14907503+++Portal+Release-Live Windows/10.0.19041.1.256.64bit'
     _store_user_agent = 'EpicGamesLauncher/14.0.8-22004686+++Portal+Release-Live'
     # required for the oauth request
     _user_basic = '34a02cf8f4414e29b15921876da36f9a'
     _pw_basic = 'daafbccc737745039dffe53d94fc76cf'
     _label = 'Live-EternalKnight'
 
@@ -76,36 +97,49 @@
         self.user = None
 
         self.language_code = lc
         self.country_code = cc
 
         self.request_timeout = timeout if timeout > 0 else None
 
-    def get_auth_url(self):
+    def _extract_price_from_elt(self, dom_elt=None, asset_name='NO NAME') -> float:
+        """
+        Extracts the price from a BeautifulSoup element.
+        :param dom_elt: The BeautifulSoup element.
+        :param asset_name: The name of the asset (for display purpose only).
+        :return: The price.
+        """
+        if dom_elt is None or dom_elt == '':
+            self.log.debug(f'Price not found for {asset_name}')
+            return 0.0
+        price = 0.0
+        try:
+            # asset base price when logged
+            price = dom_elt.text.strip('$')
+            price = price.strip('€')
+            price = float(price)
+        except Exception as error:
+            self.log.warning(f'Can not find the price for {asset_name}:{error!r}')
+        return price
+
+    def get_auth_url(self) -> str:
+        """
+        Returns the url for the oauth login.
+        :return: The url
+        """
         login_url = 'https://www.epicgames.com/id/login?redirectUrl='
         redirect_url = f'https://www.epicgames.com/id/api/redirect?clientId={self._user_basic}&responseType=code'
         return login_url + urllib.parse.quote(redirect_url)
 
-    def update_egs_params(self, egs_params):
-        # update user-agent
-        if version := egs_params['version']:
-            self._user_agent = f'UELauncher/{version} Windows/10.0.19041.1.256.64bit'
-            self._store_user_agent = f'EpicGamesLauncher/{version}'
-            self.session.headers['User-Agent'] = self._user_agent
-            self.unauth_session.headers['User-Agent'] = self._user_agent
-        # update label
-        if label := egs_params['label']:
-            self._label = label
-        # update client credentials
-        if 'client_id' in egs_params and 'client_secret' in egs_params:
-            self._user_basic = egs_params['client_id']
-            self._pw_basic = egs_params['client_secret']
-            self._oauth_basic = HTTPBasicAuth(self._user_basic, self._pw_basic)
-
-    def resume_session(self, session):
+    def resume_session(self, session: dict) -> dict:
+        """
+        Resumes a session.
+        :param session: The session.
+        :return: The session.
+        """
         self.session.headers['Authorization'] = f'bearer {session["access_token"]}'
         r = self.session.get(f'https://{self._oauth_host}/account/api/oauth/verify', timeout=self.request_timeout)
         if r.status_code >= 500:
             r.raise_for_status()
 
         j = r.json()
         if 'errorMessage' in j:
@@ -116,14 +150,22 @@
         session.update(j)
         self.user = session
         return self.user
 
     def start_session(
         self, refresh_token: str = None, exchange_token: str = None, authorization_code: str = None, client_credentials: bool = False
     ) -> dict:
+        """
+        Starts a session.
+        :param refresh_token: refresh token
+        :param exchange_token: exchange token
+        :param authorization_code: authorization code
+        :param client_credentials: client credentials
+        :return: The session.
+        """
         if refresh_token:
             params = dict(grant_type='refresh_token', refresh_token=refresh_token, token_type='eg1')
         elif exchange_token:
             params = dict(grant_type='exchange_code', exchange_code=exchange_token, token_type='eg1')
         elif authorization_code:
             params = dict(grant_type='authorization_code', code=authorization_code, token_type='eg1')
         elif client_credentials:
@@ -153,112 +195,183 @@
         self.session.headers['Authorization'] = f'bearer {j["access_token"]}'
         # only set user info when using non-anonymous login
         if not client_credentials:
             self.user = j
 
         return j
 
-    def invalidate_session(self):  # unused
-        _ = self.session.delete(f'https://{self._oauth_host}/account/api/oauth/sessions/kill/{self.access_token}', timeout=self.request_timeout)
-
-    def get_item_token(self):
+    def get_item_token(self) -> str:
+        """
+        Gets the item token.
+        Unused but kept for the global API reference.
+        :return: The item token using json format
+        """
         r = self.session.get(f'https://{self._oauth_host}/account/api/oauth/exchange', timeout=self.request_timeout)
         r.raise_for_status()
         return r.json()
 
-    def get_ownership_token(self, namespace, catalog_item_id):
+    def get_ownership_token(self, namespace: str, catalog_item_id: str) -> bytes:
+        """
+        Gets the ownership token.
+        Unused but kept for the global API reference.
+        :param namespace:  namespace
+        :param catalog_item_id: catalog item id
+        :return: The ownership token.
+        """
         user_id = self.user.get('account_id')
         r = self.session.post(
             f'https://{self._ecommerce_host}/ecommerceintegration/api/public/'
             f'platforms/EPIC/identities/{user_id}/ownershipToken',
             data=dict(nsCatalogItemId=f'{namespace}:{catalog_item_id}'),
             timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.content
 
-    def get_external_auths(self):
+    def get_external_auths(self) -> dict:
+        """
+        Gets the external auths.
+        Unused but kept for the global API reference.
+        :return: The external auths using json format.
+        """
         user_id = self.user.get('account_id')
         r = self.session.get(f'https://{self._oauth_host}/account/api/public/account/{user_id}/externalAuths', timeout=self.request_timeout)
         r.raise_for_status()
         return r.json()
 
     def get_item_assets(self, platform='Windows', label='Live'):
+        """
+        Gets the item assets.
+        :param platform: platform to get assets for
+        :param label: label of the assets
+        :return: The item assets using json format.
+        """
         r = self.session.get(
             f'https://{self._launcher_host}/launcher/api/public/assets/{platform}', params=dict(label=label), timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.json()
 
-    def get_item_manifest(self, namespace, catalog_item_id, app_name, platform='Windows', label='Live'):
+    def get_item_manifest(self, namespace, catalog_item_id, app_name, platform='Windows', label='Live') -> dict:
+        """
+        Gets the item manifest.
+        :param namespace:  namespace
+        :param catalog_item_id: catalog item id
+        :param app_name: app name
+        :param platform: platform to get manifest for
+        :param label: label of the manifest
+        :return: The item manifest using json format.
+        """
         r = self.session.get(
             f'https://{self._launcher_host}/launcher/api/public/assets/v2/platform'
             f'/{platform}/namespace/{namespace}/catalogItem/{catalog_item_id}/app'
             f'/{app_name}/label/{label}',
             timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.json()
 
-    def get_launcher_manifests(self, platform='Windows', label=None):
+    def get_launcher_manifests(self, platform='Windows', label: str = None) -> dict:
+        """
+        Gets the launcher manifests.
+        Unused but kept for the global API reference.
+        :param platform: platform to get manifests for
+        :param label: label of the manifests
+        :return: The launcher manifests using json format.
+        """
         r = self.session.get(
             f'https://{self._launcher_host}/launcher/api/public/assets/v2/platform/'
             f'{platform}/launcher',
             timeout=self.request_timeout,
             params=dict(label=label if label else self._label)
         )
         r.raise_for_status()
         return r.json()
 
-    def get_user_entitlements(self):
+    def get_user_entitlements(self) -> dict:
+        """
+        Gets the user entitlements.
+        Unused but kept for the global API reference.
+        :return: The user entitlements using json format.
+        """
         user_id = self.user.get('account_id')
         r = self.session.get(
             f'https://{self._entitlements_host}/entitlement/api/account/{user_id}/entitlements',
             params=dict(start=0, count=5000),
             timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.json()
 
-    def get_item_info(self, namespace, catalog_item_id, timeout=None):
+    def get_item_info(self, namespace: str, catalog_item_id: str, timeout: float = None) -> dict:
+        """
+        Gets the item info.
+        :param namespace: Namespace of the item
+        :param catalog_item_id: Catalog item id of the item
+        :param timeout: Timeout for the request
+        :return: The item info.
+        """
         r = self.session.get(
             f'https://{self._catalog_host}/catalog/api/shared/namespace/{namespace}/bulk/items',
             params=dict(
                 id=catalog_item_id, includeDLCDetails=True, includeMainGameDetails=True, country=self.country_code, locale=self.language_code
             ),
             timeout=timeout or self.request_timeout
         )
         r.raise_for_status()
         return r.json().get(catalog_item_id, None)
 
-    def get_artifact_service_ticket(self, sandbox_id: str, artifact_id: str, label='Live', platform='Windows'):
+    def get_artifact_service_ticket(self, sandbox_id: str, artifact_id: str, label='Live', platform='Windows') -> dict:
+        """
+        Gets the artifact service ticket.
+        Unused but kept for the global API reference.
+        :param sandbox_id: sandbox id
+        :param artifact_id: artifact id
+        :param label: label
+        :param platform: platform to get ticket for
+        :return: The artifact service ticket using json format.
+        """
         # Based on EOS Helper Windows service implementation. Only works with anonymous EOS Helper session.
         # sandbox_id is the same as the namespace, artifact_id is the same as the app name
         r = self.session.post(
             f'https://{self._artifact_service_host}/artifact-service/api/public/v1/dependency/'
             f'sandbox/{sandbox_id}/artifact/{artifact_id}/ticket',
             json=dict(label=label, expiresInSeconds=300, platform=platform),
             params=dict(useSandboxAwareLabel='false'),
             timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.json()
 
-    def get_item_manifest_by_ticket(self, artifact_id: str, signed_ticket: str, label='Live', platform='Windows'):
+    def get_item_manifest_by_ticket(self, artifact_id: str, signed_ticket: str, label='Live', platform='Windows') -> dict:
+        """
+        Gets the item manifest by ticket.
+        Unused but kept for the global API reference.
+        :param artifact_id: artifact id
+        :param signed_ticket: signed ticket
+        :param label: the label
+        :param platform: platform to get manifest for
+        :return: The item manifest by ticket using json format.
+        """
         # Based on EOS Helper Windows service implementation.
         r = self.session.post(
             f'https://{self._launcher_host}/launcher/api/public/assets/v2/'
             f'by-ticket/app/{artifact_id}',
             json=dict(platform=platform, label=label, signedTicket=signed_ticket),
             timeout=self.request_timeout
         )
         r.raise_for_status()
         return r.json()
 
-    def get_library_items(self, include_metadata=True):
+    def get_library_items(self, include_metadata=True) -> list:
+        """
+        Gets the library items.
+        :param include_metadata: Whether to include metadata
+        :return: The library items
+        """
         records = []
         r = self.session.get(
             f'https://{self._library_host}/library/api/public/items', params=dict(includeMetadata=include_metadata), timeout=self.request_timeout
         )
         r.raise_for_status()
         j = r.json()
         records.extend(j['records'])
@@ -273,14 +386,20 @@
             r.raise_for_status()
             j = r.json()
             records.extend(j['records'])
 
         return records
 
     def find_asset_url(self, asset_name: str, timeout=10.0) -> []:
+        """
+        Find the asset url from the asset name by searching the asset name in the unreal engine marketplace
+        :param asset_name: asset name to search
+        :param timeout: timeout for the request
+        :return: (The asset url, the asset name , the grab result code)
+        """
         # remove the suffix _EngineVersion (ex _4.27) at the end of the name to have a valid search value
         regex = r"_[4|5]\.\d{1,2}$"
         converted_name = re.sub(regex, '', asset_name, 0)
         # Replace ' ' by '%20'
         converted_name = converted_name.replace(' ', '%20')
         # SnakeCase
         # converted_name = inflection.underscore(converted_name)
@@ -294,16 +413,19 @@
         for entry in entry_list:
             converted_name = converted_name.replace(entry, '')
 
         url = ''
         asset_name_in_url = ''
         search_url_root = f'https://{self._search_url}/assets?keywords='
         search_url_full = search_url_root + converted_name
-        r = self.session.get(search_url_full, timeout=timeout)
-
+        try:
+            r = self.session.get(search_url_full, timeout=timeout)
+        except requests.exceptions.Timeout:
+            self.log.warning(f'Timeout for {asset_name}')
+            return [url, asset_name_in_url, GrabResult.TIMEOUT.name]
         if not r.ok:
             self.log.warning(f'Can not find the url for {asset_name}:{r.reason}')
             return [url, asset_name_in_url, GrabResult.PAGE_NOT_FOUND.name]
 
         soup = BeautifulSoup(r.content, 'html.parser')
         links = []
         group_elt = soup.find('div', attrs={'class': 'asset-list-group'})
@@ -321,14 +443,22 @@
         # return the first one (probably the best choice)
         asset_name_in_url = links[0].replace('/marketplace/en-US/product/', '')
         url = 'https://www.unrealengine.com' + links[0]
         return [url, asset_name_in_url, GrabResult.NO_ERROR.name]
 
     #  get the extras data of an asset (price, review...)
     def get_assets_extras(self, asset_name: str, asset_title: str, timeout=10.0, verbose_mode=False) -> dict:
+        """
+        Get the extras data of an asset (price, review...)
+        :param asset_name: name of the asset
+        :param asset_title: title of the asset
+        :param timeout: connection timeout
+        :param verbose_mode: verbose mode
+        :return: a dict with the extras data
+        """
         not_found_price = 0.0
         not_found_review = 0.0
         supported_versions = ''
         page_title = ''
         no_result = create_empty_assets_extras(asset_name=asset_name)
 
         # try to find the url of the asset by doing a search in the marketplace
@@ -344,14 +474,16 @@
             self.log.warning(f'Can not get extras data for {asset_name}:{error!r}')
             no_result['grab_result'] = error_code
             return no_result
 
         soup_logged = BeautifulSoup(response.text, 'html.parser')
 
         price = not_found_price
+        discount_price = not_found_price
+
         search_for_price = True
 
         # check if already purchased
         purchased = False
         purchased_elt = soup_logged.find('div', class_='purchase')
         if purchased_elt is not None:
             if 'Free' in purchased_elt.getText():
@@ -378,25 +510,34 @@
             if 'Sign in to Download' in purchased_elt.getText():
                 # free price when logged or not
                 price = 0.0
                 if verbose_mode:
                     self.log.info(f'{asset_name} is free (check 2)')
             else:
                 # get price using the logged or the not logged soup
-                asset_price = purchased_elt.find('span', class_='save-discount')
-                if asset_price is not None:
-                    try:
-                        # asset price when logged
-                        price = asset_price.text.strip('$')
-                        price = price.strip('€')
-                        price = float(price)
-                    except Exception as error:
-                        self.log.warning(f'Can not find the price for {asset_name}:{error!r}')
+                # notes:
+                #   when not discounted
+                #       base-price is not available
+                #       price is 'save-discount'
+                #       discount-price is 0.0
+                #   when discounted
+                #       price is 'base-price'
+                #       discount-price is 'save-discount'
+                elt = purchased_elt.find('span', class_='save-discount')
+                current_price = self._extract_price_from_elt(elt, asset_name)
+                elt = purchased_elt.find('span', class_='base-price')
+                base_price = self._extract_price_from_elt(elt, asset_name)
+                if elt is not None:
+                    # discounted
+                    price = base_price
+                    discount_price = current_price
                 else:
-                    self.log.debug(f'Price not found for {asset_name}')
+                    # not discounted
+                    price = current_price
+                    discount_price = current_price
 
         # get review
         reviews_elt = soup_logged.find('div', class_='asset-detail-rating')
         if reviews_elt is not None:
             reviews_elt = reviews_elt.find('div', class_='rating-board__pop__title')
         if reviews_elt is not None:
             try:
@@ -428,19 +569,23 @@
             try:
                 page_title = title_elt.text
             except Exception as error:
                 self.log.warning(f'Can not find the Page title for {asset_name}:{error!r}')
         else:
             self.log.debug(f'Can not find the Page title not found for {asset_name}')
             review = not_found_review
-        self.log.info(f'GRAB results: asset_name_in_url={asset_name_in_url} purchased={purchased} price={price} review={review}')
+        on_sale = 0.0 < discount_price < price and price > 0.0
+
+        self.log.info(f'GRAB results: asset_name_in_url={asset_name_in_url} on_sale={on_sale} purchased={purchased} price={price} review={review}')
         return {
             'asset_name': asset_name,
             'asset_url': asset_url,
             'asset_name_in_url': asset_name_in_url,
             'page_title': page_title,
             'price': price,
+            'discount_price': discount_price,
             'review': review,
             'purchased': purchased,
             'supported_versions': supported_versions,
-            'grab_result': error_code
+            'grab_result': error_code,
+            'on_sale': on_sale
         }
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.3.0/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/assets/main.ico` & `UEVaultManager-1.3.0/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/cli.py` & `UEVaultManager-1.3.0/UEVaultManager/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,132 @@
-#!/usr/bin/env python
-# coding: utf-8
-
+# coding=utf-8
+"""
+Implementation for:
+- UEVaultManagerCLI: command line interface for UEVaultManager
+"""
 import argparse
 import csv
 import json
 import logging
 import os
 import shutil
 import subprocess
+import time
 import webbrowser
 from collections import namedtuple
 from datetime import datetime
 from logging.handlers import QueueListener
 from multiprocessing import freeze_support, Queue as MPQueue
 from platform import platform
-from sys import exit, stdout, platform as sys_platform
+from sys import exit, stdout
+
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 # noinspection PyPep8Naming
-import UEVaultManager.tkgui.modules.UEVMGuiClass as gui_w  # using the shortest variable name for globals for convenience
 from UEVaultManager import __version__, __codename__
-from UEVaultManager.api.egs import create_empty_assets_extras
+from UEVaultManager.api.egs import create_empty_assets_extras, GrabResult
+from UEVaultManager.api.uevm import UpdateSeverity
 from UEVaultManager.core import AppCore, CSV_headings
 from UEVaultManager.models.exceptions import InvalidCredentialsError
+from UEVaultManager.tkgui.modules.DisplayContentWindowClass import DisplayContentWindow
+from UEVaultManager.tkgui.modules.functions import json_print_key_val
 from UEVaultManager.tkgui.modules.ProgressWindowsClass import ProgressWindow
-from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
+from UEVaultManager.tkgui.modules.UEVMGuiClass import UEVMGui
+from UEVaultManager.tkgui.modules.UEVMGuiHiddenRootClass import UEVMGuiHiddenRoot
 from UEVaultManager.utils.cli import str_to_bool, check_and_create_path, create_list_from_string
 from UEVaultManager.utils.custom_parser import HiddenAliasSubparsersAction
 
-# todo custom formatter for cli logger (clean info, highlighted error/warning)
 logging.basicConfig(format='[%(name)s] %(levelname)s: %(message)s', level=logging.INFO)
 
 
 class UEVaultManagerCLI:
+    """
+    Command line interface for UEVaultManager
+    :param override_config: path to a config file to use instead of the default one
+    :param api_timeout: timeout for API requests
+    """
 
     def __init__(self, override_config=None, api_timeout=None):
         self.core = AppCore(override_config, timeout=api_timeout)
         self.logger = logging.getLogger('Cli')
         self.logging_queue = None
 
-    def setup_threaded_logging(self):
+    def setup_threaded_logging(self) -> QueueListener:
+        """
+        Setup logging for the CLI
+        """
         self.logging_queue = MPQueue(-1)
         handler = logging.StreamHandler()
         formatter = logging.Formatter('[%(name)s] %(levelname)s: %(message)s')
         handler.setFormatter(formatter)
         ql = QueueListener(self.logging_queue, handler)
         ql.start()
         return ql
 
-    def _resolve_aliases(self, name):
+    def _resolve_aliases(self, name: str) -> str:
+        """
+        Resolve an alias
+        :param name: name to resolve
+        :return: real name
+        """
         # make sure aliases exist if not yet created
         self.core.update_aliases(force=False)
         name = name.strip()
         # resolve alias (if any) to real app name
-        return self.core.lgd.config.get(section='UEVaultManager.aliases', option=name, fallback=self.core.lgd.aliases.get(name.lower(), name))
+        return self.core.uevmlfs.config.get(section='UEVaultManager.aliases', option=name, fallback=self.core.uevmlfs.aliases.get(name.lower(), name))
 
     @staticmethod
     def _print_json(data, pretty=False):
         if pretty:
             print(json.dumps(data, indent=2, sort_keys=True))
         else:
             print(json.dumps(data))
 
-    def create_file_backup(self, file_src):
+    def create_file_backup(self, file_src: str) -> None:
+        """
+        Create a backup of a file
+        :param file_src: path to the file to back up
+        """
         # make a backup of the existing file
 
         # for files defined relatively to the config folder
-        file_src = file_src.replace('~/.config', self.core.lgd.path)
+        file_src = file_src.replace('~/.config', self.core.uevmlfs.path)
 
         if not file_src:
             return
         try:
             file_name_no_ext, file_ext = os.path.splitext(file_src)
             file_backup = f'{file_name_no_ext}.BACKUP_{datetime.now().strftime("%y-%m-%d_%H-%M-%S")}{file_ext}'
             shutil.copy(file_src, file_backup)
             self.logger.info(f'File {file_src} has been copied to {file_backup}')
         except FileNotFoundError:
             self.logger.info(f'File {file_src} has not been found')
 
-    def create_log_file_backup(self):
+    def create_log_file_backup(self) -> None:
+        """
+        Create a backup of the log files
+        """
         self.create_file_backup(self.core.ignored_assets_filename_log)
         self.create_file_backup(self.core.notfound_assets_filename_log)
         self.create_file_backup(self.core.bad_data_assets_filename_log)
 
-    def create_asset_from_data(self, item, asset_id, no_text_data, no_int_data, no_float_data, bool_true_data, bool_false_data):
+    def create_asset_from_data(
+        self, item, asset_id: str, no_text_data: str, no_int_data: int, no_float_data: float, bool_true_data: bool, bool_false_data: bool
+    ) -> (str, dict):
+        """
+        Create a dict containing all the data for an asset
+        :param item: item to get data from
+        :param asset_id: id of the asset
+        :param no_text_data: text to use if no text data is found
+        :param no_int_data: int value to use if no int data is found
+        :param no_float_data: float value to use if no float data is found
+        :param bool_true_data: bool (True) value to use if no bool data is found
+        :param bool_false_data: bool (False) value to use if no bool data is found
+        :return: (asset_id, dict containing all the data for an asset)
+        """
         record = {}
         metadata = item.metadata
         uid = metadata['id']
         category = metadata['categories'][0]['path']
         separator = ','
         try:
             tmp_list = [separator.join(item.get('compatibleApps')) for item in metadata['releaseInfo']]
@@ -99,34 +138,39 @@
         try:
             thumbnail_url = metadata['keyImages'][2]['url']  # 'Image' with 488 height
         except IndexError:
             self.logger.debug(f'asset {item.app_name} has no image')
         date_added = datetime.now().strftime(self.core.default_datetime_format)
         extras_data = None
         try:
-            extras_data = self.core.lgd.get_item_extras(item.app_name)
+            extras_data = self.core.uevmlfs.get_item_extras(item.app_name)
         except AttributeError as error:
             self.logger.warning(f'Error getting extra data for {item.app_name} : {error!r}')
         if extras_data is None:
             extras_data = create_empty_assets_extras(item.app_name)
         asset_url = no_text_data
         review = no_int_data
         price = no_float_data
         purchased = bool_false_data
+        discount_price = no_float_data
         supported_versions = no_text_data
         page_title = no_text_data
-        grab_result = no_int_data
+        grab_result = GrabResult.NO_ERROR.name
+        on_sale = bool_false_data
+
         try:
             asset_url = extras_data['asset_url']
             review = extras_data['review']
             price = extras_data['price']
+            discount_price = extras_data['discount_price']
             purchased = extras_data['purchased']
             supported_versions = extras_data['supported_versions']
             page_title = extras_data['page_title']
             grab_result = extras_data['grab_result']
+            on_sale = extras_data['on_sale']
         except (TypeError, KeyError) as error:
             self.logger.warning(f'Key not found in extra data for {item.app_name} : {error!r}')
 
         if self.core.engine_version_for_obsolete_assets == '' or supported_versions == '' or supported_versions == no_text_data:
             obsolete = bool_false_data
         else:
             supported_versions_list = supported_versions.lower().replace('UE_', '')
@@ -142,54 +186,58 @@
         try:
             values = (
                 # dans les infos
                 asset_id  # 'asset_id'
                 , item.app_name  # 'App name'
                 , item.app_title  # 'App title'
                 , category  # 'Category'
-                , thumbnail_url  # 'Image' with 488 height
-                , asset_url  # 'Url'
                 , item.app_version('Windows')  # 'UE Version'
-                , compatible_versions  # compatible_versions
                 , review  # 'Review'
                 , metadata['developer']  # 'Developer'
                 , metadata['description']  # 'Description'
-                , uid  # 'Uid'
-                , metadata['creationDate']  # 'Creation Date'
-                , metadata['lastModifiedDate']  # 'Update Date'
                 , metadata['status']  # 'status'
-                # Modified Fields when added into the file
-                , date_added  # 'Date Added'
-                , price  # 'Price'
-                , no_float_data  # 'Old Price'
-                , bool_false_data  # 'On Sale'
+                , discount_price  # 'Discount Price'
+                , on_sale  # 'On Sale'
                 , purchased  # 'Purchased'
                 , obsolete  # 'obsolete'
-                # Extracted from page, can be compared with value in metadata. Coud be used to if check data grabbing if OK
                 , supported_versions  # 'supported versions'
-                , page_title  # 'page title'
                 , grab_result  # 'grab result'
-                # Modified Fields when added into the file
+                , price  # 'Price'
+                , no_float_data  # 'Old Price'
+                # User Fields
                 , no_text_data  # 'Comment'
                 , no_float_data  # 'Stars'
-                , no_text_data  # 'Asset Folder'
                 , bool_false_data  # 'Must Buy'
                 , no_text_data  # 'Test result
                 , no_text_data  # 'Installed Folder'
                 , no_text_data  # 'Alternative'
+                , no_text_data  # 'Asset Folder'
+                # less important fields
+                , page_title  # 'page title'
+                , thumbnail_url  # 'Image' with 488 height
+                , asset_url  # 'Url'
+                , compatible_versions  # compatible_versions
+                , date_added  # 'Date Added'
+                , metadata['creationDate']  # 'Creation Date'
+                , metadata['lastModifiedDate']  # 'Update Date'
+                , uid  # 'Uid'
             )
             record = dict(zip(CSV_headings.keys(), values))
         except TypeError:
             self.logger.error(f'Could not create record for {item.app_name}')
 
         return asset_id, record
 
-    def auth(self, args):
+    def auth(self, args) -> None:
+        """
+        Handle authentication
+        :param args: options passed to the command
+        """
         if args.auth_delete:
-            self.core.lgd.invalidate_userdata()
+            self.core.uevmlfs.invalidate_userdata()
             self.logger.info('User data deleted.')
             return
 
         try:
             self.logger.info('Testing existing login data if present...')
             if self.core.login():
                 self.logger.info(
@@ -197,26 +245,26 @@
                     'account, run "UEVaultManager auth --delete" and try again.'
                 )
                 return
         except ValueError:
             pass
         except InvalidCredentialsError:
             self.logger.error('Stored credentials were found but were no longer valid. Continuing with login...')
-            self.core.lgd.invalidate_userdata()
+            self.core.uevmlfs.invalidate_userdata()
 
         # Force an update check and notice in case there are API changes
         self.core.check_for_updates(force=True)
         self.core.force_show_update = True
 
         if args.import_egs_auth:
             self.logger.info('Importing login session from the Epic Launcher...')
             try:
                 if self.core.auth_import():
                     self.logger.info('Successfully imported login session from EGS!')
-                    self.logger.info(f'Now logged in as user "{self.core.lgd.userdata["displayName"]}"')
+                    self.logger.info(f'Now logged in as user "{self.core.uevmlfs.userdata["displayName"]}"')
                     return
                 else:
                     self.logger.warning('Login session from EGS seems to no longer be valid.')
                     self.core.clean_exit(1)
             except Exception as error:
                 self.logger.error(f'No EGS login session found, please login manually. (Exception: {error!r})')
                 self.core.clean_exit(1)
@@ -238,15 +286,15 @@
                 if auth_code[0] == '{':
                     tmp = json.loads(auth_code)
                     auth_code = tmp['authorizationCode']
                 else:
                     auth_code = auth_code.strip('"')
             else:
                 if do_webview_login(callback_code=self.core.auth_ex_token):
-                    self.logger.info(f'Successfully logged in as "{self.core.lgd.userdata["displayName"]}" via WebView')
+                    self.logger.info(f'Successfully logged in as "{self.core.uevmlfs.userdata["displayName"]}" via WebView')
                 else:
                     self.logger.error('WebView login attempt failed, please see log for details.')
                 return
         elif args.session_id:
             exchange_token = self.core.auth_sid(args.session_id)
         elif args.auth_code:
             auth_code = args.auth_code
@@ -254,23 +302,34 @@
             exchange_token = args.ex_token
 
         if not exchange_token and not auth_code:
             self.logger.fatal('No exchange token/authorization code, cannot login.')
             return
 
         if exchange_token and self.core.auth_ex_token(exchange_token):
-            self.logger.info(f'Successfully logged in as "{self.core.lgd.userdata["displayName"]}"')
+            self.logger.info(f'Successfully logged in as "{self.core.uevmlfs.userdata["displayName"]}"')
         elif auth_code and self.core.auth_code(auth_code):
-            self.logger.info(f'Successfully logged in as "{self.core.lgd.userdata["displayName"]}"')
+            self.logger.info(f'Successfully logged in as "{self.core.uevmlfs.userdata["displayName"]}"')
         else:
             self.logger.error('Login attempt failed, please see log for details.')
 
-    def list_assets(self, args):
+    def list_assets(self, args) -> None:
+        """
+        List assets in the vault
+        :param args: options passed to the command
+        """
 
         def update_and_merge_csv_record_data(_asset, _items_in_file, _no_data_value) -> []:
+            """
+            Updates the data of the asset with the data from the items in the file
+            :param _asset: asset to update
+            :param _items_in_file: list of items in the file
+            :param _no_data_value: value to use when no data is available
+            :return: list of values to be written in the CSV file
+            """
             _asset_id = _asset[0]
             _csv_record = list(_asset[1].values())  # we need a list for the CSV comparison, not a dict
             # merge data from the items in the file (if exists) and those get by the application
             # items_in_file must be a dict of dicts
             if _items_in_file.get(_asset_id):
                 item_in_file = _items_in_file.get(_asset_id)
                 if len(item_in_file.keys()) != len(CSV_headings.keys()):
@@ -280,17 +339,16 @@
                     return _csv_record
                 else:
                     # loops through its columns
                     index = 0
                     price_index = 0
                     _price = float(_no_data_value)
                     old_price = float(_no_data_value)
-                    on_sale = _no_data_value
                     for key, keep_value_in_file in CSV_headings.items():
-                        if item_in_file[key] is None:
+                        if item_in_file.get(key, None) is None:
                             self.logger.error(
                                 f'In the existing file, asset {_asset_id} has no column named {key}. This asset is ignored and its values will be overwritten'
                             )
                             # print(f' CHECK for asset {_asset_id}')
                             return _csv_record
                         else:
                             if keep_value_in_file:
@@ -303,75 +361,71 @@
                                     old_price = float(
                                         item_in_file[key]
                                     )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
                                 except Exception as _error:
                                     self.logger.warning(f'Old Price value can not be converted for asset {_asset_id}\nError:{_error!r}')
                         index += 1
 
-                # compute the price related fields
-                if price_index > 0 and (isinstance(old_price, int) or isinstance(old_price, float)):
-                    on_sale = True if _price > old_price else False
                 _csv_record[price_index + 1] = old_price
-                _csv_record[price_index + 2] = on_sale
             return _csv_record
 
-        def update_and_merge_json_record_data(_asset, _items_in_file, _no_float_value, _no_bool_false_value) -> dict:
+        def update_and_merge_json_record_data(_asset, _items_in_file, _no_float_value: float, _no_bool_false_value: bool) -> dict:
+            """
+            Updates the data of the asset with the data from the items in the file
+            :param _asset: asset to update
+            :param _items_in_file: list of items in the file
+            :param _no_float_value:  value to use when no float data is available
+            :param _no_bool_false_value: value (False) to use when no bool data is available
+            :return:
+            """
             _asset_id = _asset[0]
             _json_record = _asset[1]
 
             # merge data from the items in the file (if exists) and those get by the application
             # items_in_file is a dict of dict
             if _items_in_file.get(_asset_id):
                 # loops through its columns
                 _price = float(_no_float_value)
                 old_price = float(_no_float_value)
-                on_sale = _no_bool_false_value
                 for key, keep_value_in_file in CSV_headings.items():
                     if keep_value_in_file and _items_in_file[_asset_id].get(key):
                         _json_record[key] = _items_in_file[_asset_id][key]
 
                 # Get the old price in the previous file
                 try:
                     _price = float(_json_record['Price'])
                     old_price = float(
                         _items_in_file[_asset_id]['Price']
                     )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
                 except Exception as _error:
                     self.logger.warning(f'Old Price values can not be converted for asset {_asset_id}\nError:{_error!r}')
-
-                # compute the price related fields
-                if isinstance(old_price, int) or isinstance(old_price, float):
-                    on_sale = True if _price > old_price else False
                 _json_record['Old Price'] = old_price
-                _json_record['On Sale'] = on_sale
             return _json_record
 
         self.logger.info('Logging in...')
         if not self.core.login():
             self.logger.error('Login failed, cannot continue!')
             self.core.clean_exit(1)
 
         if args.force_refresh:
             self.logger.info('Refreshing asset list, this may take a while...')
         else:
             self.logger.info('Getting asset list... (this may take a while)')
 
-        if args.filter_category:
+        if args.filter_category and args.filter_category != gui_g.s.default_category_for_all:
             gui_g.UEVM_filter_category = args.filter_category
-
-        if gui_g.UEVM_filter_category != '' and gui_g.UEVM_filter_category != gui_g.s.default_category_for_all:
-            self.logger.info(f'The String "{gui_g.UEVM_filter_category }" will be search in Assets category')
+            self.logger.info(f'The String "{args.filter_category}" will be search in Assets category')
 
         gui_g.progress_window_ref = None
         progress_window = None
         if args.gui:
             # check if the GUI is already running
             if gui_g.UEVM_gui_ref is None:
                 # create a fake root because ProgressWindow must always be a top level window
-                gui_g.UEVM_gui_ref = gui_w.UEVMGuiHiddenRoot()
+                gui_g.UEVM_gui_ref = UEVMGuiHiddenRoot()
                 uewm_gui_exists = False
             else:
                 uewm_gui_exists = True
             # create and use a progress window (as a top level window)
             gui_g.UEVM_log_ref = self.logger
             progress_window = ProgressWindow(
                 title="Updating Assets List",
@@ -418,15 +472,15 @@
         assets_to_output = {}
         # create a minimal and full dict of data from existing assets
         assets_in_file = {}
 
         cpt = 0
         cpt_max = len(items)
         if gui_g.progress_window_ref is not None:
-            gui_g.progress_window_ref.reset(new_value=0, new_text="Checking assets data...", new_max_value=len(items))
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Merging assets data...", new_max_value=len(items))
         for item in items:
             if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
                 return
             cpt += 1
             # notes:
             #   asset_id is not unique because somme assets can have the same asset_id but with several UE versions
             #   app_name is unique because it includes the unreal version
@@ -570,14 +624,19 @@
         print('\nAvailable UE Assets:')
         for asset in items:
             version = asset.app_version('Windows')
             print(f' * {asset.app_title.strip()} (App name: {asset.app_name} | Version: {version})')
         print(f'\nTotal: {len(items)}')
 
     def list_files(self, args):
+        """
+        List files for a given app name or manifest url/path
+        :param args: options passed to the command
+        :return:
+        """
         if not args.override_manifest and not args.app_name:
             print('You must provide either a manifest url/path or app name!')
             return
         elif args.app_name:
             args.app_name = self._resolve_aliases(args.app_name)
 
         # check if we even need to log in
@@ -618,51 +677,93 @@
                 print(fm.filename)
                 for t in fm.install_tags:
                     install_tags.add(t)
             if install_tags:
                 # use the log output so this isn't included when piping file list into file
                 self.logger.info(f'Install tags: {", ".join(sorted(install_tags))}')
 
-    def status(self, args):
+    def status(self, args) -> None:
+        """
+        Print the information about the vault and the available assets
+        :param args: options passed to the command
+        """
         if not args.offline:
             try:
                 if not self.core.login():
                     self.logger.error('Log in failed!')
                     self.core.clean_exit(1)
             except ValueError:
                 pass
             # if automatic checks are off force an update here
             self.core.check_for_updates(force=True)
 
-        if not self.core.lgd.userdata:
+        if not self.core.uevmlfs.userdata:
             user_name = '<not logged in>'
             args.offline = True
         else:
-            user_name = self.core.lgd.userdata['displayName']
+            user_name = self.core.uevmlfs.userdata['displayName']
+
+        cache_information = self.core.uevmlfs.get_ue_assets_cache_data()
+        update_information = self.core.uevmlfs.get_cached_version()
+        last_update = update_information.get('last_update', '')
+        update_information = update_information.get('data', None)
+        last_cache_update = cache_information.get('last_update', '')
+        if last_update != '':
+            last_update = time.strftime("%x", time.localtime(last_update))
+        if last_cache_update != '':
+            last_cache_update = time.strftime("%x", time.localtime(last_cache_update))
+
+        json_content = {
+            'Epic account': user_name,  #
+            'Last data update': last_update,
+            'Last cache update': last_cache_update,
+            'Config directory': self.core.uevmlfs.path,
+            'Platform': f'{platform()} ({os.name})',
+            'Current version': f'{__version__} - {__codename__}',
+        }
+        if not args.offline:
+            assets_available = len(self.core.get_asset_list(update_assets=not args.offline))
+            json_content['Assets available'] = assets_available
+            json_content['Update available'] = 'yes' if self.core.update_available else 'no'
+
+            if self.core.update_available and update_information is not None:
+                json_content['Update info'] = '\n\n'
+                json_content['New version'] = f'{update_information["version"]} - {update_information["codename"]}'
+                json_content['Release summary'] = update_information['summary']
+                json_content['Release Url'] = update_information['release_url']
+                json_content['Update recommendation'] = update_information['severity']
 
-        assets_available = len(self.core.get_asset_list(update_assets=not args.offline))
         if args.json:
-            return self._print_json(dict(account=user_name, assets_available=assets_available, config_directory=self.core.lgd.path), args.pretty_json)
+            return self._print_json(json_content, args.pretty_json)
+
+        if args.gui:
+            # check if the GUI is already running
+            if gui_g.UEVM_gui_ref is None:
+                # create a fake root because DisplayContentWindow must always be a top level window
+                gui_g.UEVM_gui_ref = UEVMGuiHiddenRoot()
+                uewm_gui_exists = False
+            else:
+                uewm_gui_exists = True
+            if gui_g.display_content_window_ref is None:
+                _ = DisplayContentWindow(title='UEVM: status command output', quit_on_close=not uewm_gui_exists)
 
-        print(f'Epic account: {user_name}')
-        print(f'Assets available: {assets_available}')
-        print(f'Config directory: {self.core.lgd.path}')
-        print(f'Platform (System): {platform()} ({os.name})')
-        print(f'\nUEVaultManager version: {__version__} - "{__codename__}"')
-        print(f'Update available: {"yes" if self.core.update_available else "no"}')
-        if self.core.update_available:
-            if update_info := self.core.get_update_info():
-                print(f'- New version: {update_info["version"]} - "{update_info["name"]}"')
-                print(f'- Release summary:\n{update_info["summary"]}\n- Release URL: {update_info["gh_url"]}')
-                if update_info['critical']:
-                    print('! This update is recommended as it fixes major issues.')
-            # prevent update message on close
-            self.core.update_available = False
+            json_print_key_val(json_content, output_on_gui=True)
+            if not uewm_gui_exists:
+                gui_g.UEVM_gui_ref.mainloop()
+        else:
+            json_print_key_val(json_content)
+
+        # prevent update message on close
+        self.core.update_available = False
 
-    def info(self, args):
+    def info(self, args) -> None:
+        """
+        Print information about a given app name or manifest url/path
+        :param args: options passed to the command
+        """
         name_or_path = args.app_name_or_manifest
         app_name = manifest_uri = None
         if os.path.exists(name_or_path) or name_or_path.startswith('http'):
             manifest_uri = name_or_path
         else:
             app_name = self._resolve_aliases(name_or_path)
 
@@ -801,15 +902,19 @@
                                                    f'(Chunks: {len(tag_chunk_guids)})')
 
             manifest_info.append(InfoItem('Disk size by install tag', 'tag_disk_size', tag_disk_size_human or 'N/A', tag_disk_size))
             manifest_info.append(InfoItem('Download size by install tag', 'tag_download_size', tag_download_size_human or 'N/A', tag_download_size))
 
         if not args.json:
 
-            def print_info_item(local_item: InfoItem):
+            def print_info_item(local_item: InfoItem) -> None:
+                """
+                Prints an info item to the console
+                :param local_item:  The info item to print
+                """
                 if local_item.value is None:
                     print(f'- {local_item.name}: (None)')
                 elif isinstance(local_item.value, list):
                     print(f'- {local_item.name}:')
                     for list_item in local_item.value:
                         print(' + ', list_item)
                 elif isinstance(local_item.value, dict):
@@ -847,41 +952,49 @@
                     json_out['manifest'][info_item.json_name] = info_item.json_value
             # set empty items to null
             for key, value in json_out.items():
                 if not value:
                     json_out[key] = None
             return self._print_json(json_out, args.pretty_json)
 
-    def cleanup(self, args):
-        before = self.core.lgd.get_dir_size()
+    def cleanup(self, args) -> None:
+        """
+        Cleans up the local assets data folders and logs
+        :param args: options passed to the command
+        """
+        before = self.core.uevmlfs.get_dir_size()
 
         # delete metadata
         if args.delete_metadata:
             self.logger.debug('Removing app metadata...')
-            self.core.lgd.clean_metadata()
+            self.core.uevmlfs.clean_metadata()
 
         # delete extras data
         if args.delete_extras_data:
             self.logger.debug('Removing app extras data...')
-            self.core.lgd.clean_extras()
+            self.core.uevmlfs.clean_extras()
 
         # delete log and backup
         self.logger.debug('Removing logs and backups...')
-        self.core.lgd.clean_logs_and_backups()
+        self.core.uevmlfs.clean_logs_and_backups()
 
         self.logger.debug('Removing manifests...')
-        self.core.lgd.clean_manifests()
+        self.core.uevmlfs.clean_manifests()
 
         self.logger.debug('Removing tmp data')
-        self.core.lgd.clean_tmp_data()
+        self.core.uevmlfs.clean_tmp_data()
 
-        after = self.core.lgd.get_dir_size()
+        after = self.core.uevmlfs.get_dir_size()
         self.logger.info(f'Cleanup complete! Removed {(before - after) / 1024 / 1024:.02f} MiB.')
 
-    def get_token(self, args):
+    def get_token(self, args) -> None:
+        """
+        Gets the access token for the current user
+        :param args: options passed to the command
+        """
         if not self.core.login(force_refresh=args.bearer):
             self.logger.error('Login failed!')
             return
 
         if args.bearer:
             args.json = True
             token = dict(
@@ -898,50 +1011,49 @@
             if args.pretty_json:
                 print(json.dumps(token, indent=2, sort_keys=True))
             else:
                 print(json.dumps(token))
             return
         self.logger.info(f'Exchange code: {token["code"]}')
 
-    def edit_assets(self, args):
+    def edit_assets(self, args) -> None:
+        """
+        Edit assets in the database using a GUI
+        :param args: options passed to the command
+        """
         if not args.input:
             input_filename = gui_g.s.csv_filename
             self.logger.warning('The file to read data from has not been precised by the --input command option. The default file name will be used.')
         else:
             input_filename = gui_f.path_from_relative_to_absolute(args.input)
 
         app_icon_filename = gui_f.path_from_relative_to_absolute(gui_g.s.app_icon_filename)
         gui_g.UEVM_log_ref = self.logger
         gui_g.UEVM_cli_ref = self
-        # args can not be used as it because it's an object that mainly run as a dict (but it's not)
-        # so we need to convert it to a dict first
-        temp_dict = vars(args)
+
         # set output file name from the input one. Used by the "rebuild file content" button (or rebuild_data method)
-        temp_dict['output'] = input_filename
-        temp_dict['csv'] = True  # force csv output
-        temp_dict['gui'] = True
-        # create a SaferDict object from the dict (it will avoid errors when trying to access non-existing keys)
-        gui_g.UEVM_cli_args = SaferDict({})
-        # copy the dict content to the SaferDict object
-        gui_g.UEVM_cli_args.copy_from(temp_dict)
+        gui_f.init_gui_args(args, additional_args={'output': input_filename})
 
-        gui_g.UEVM_gui_ref = gui_w.UEVMGui(
+        gui_g.UEVM_gui_ref = UEVMGui(
             title=gui_g.s.app_title,
             width=gui_g.s.app_width,
             height=gui_g.s.app_height,
             icon=app_icon_filename,
             screen_index=0,
             file=input_filename,
             show_open_file_dialog=not os.path.isfile(input_filename),
         )
         gui_g.UEVM_gui_ref.mainloop()
         # gui_g.UEVM_gui_ref.quit()
 
 
 def main():
+    """
+    Main function
+    """
     parser = argparse.ArgumentParser(description=f'UEVaultManager v{__version__} - "{__codename__}"')
     parser.register('action', 'parsers', HiddenAliasSubparsersAction)
 
     # general arguments
     parser.add_argument('-H', '--full-help', dest='full_help', action='store_true', help='Show full help (including individual command help)')
     parser.add_argument('-d', '--debug', dest='debug', action='store_true', help='Set loglevel to debug')
     parser.add_argument('-y', '--yes', dest='yes', action='store_true', help='Default to yes for all prompts')
@@ -1036,15 +1148,15 @@
     list_files_parser.add_argument(
         '--hashlist', dest='hashlist', action='store_true', help='Output file hash list in hashCheck/sha1sum -c compatible format'
     )
     list_files_parser.add_argument('-f', '--force-refresh', dest='force_refresh', action='store_true', help='Force a refresh of all assets metadata')
 
     status_parser.add_argument('--offline', dest='offline', action='store_true', help='Only print offline status information, do not login')
     status_parser.add_argument('--json', dest='json', action='store_true', help='Show status in JSON format')
-
+    status_parser.add_argument('-g', '--gui', dest='gui', action='store_true', help='Display the output in a windows instead of using the console')
     clean_parser.add_argument(
         '-m,'
         '--delete-metadata', dest='delete_metadata', action='store_true', help='Also delete metadata files. They are kept by default'
     )
     clean_parser.add_argument(
         '-e,'
         '--delete-extras-data', dest='delete_extras_data', action='store_true', help='Also delete extras data files. They are kept by default'
@@ -1094,32 +1206,32 @@
                 print('Follow https://github.com/LaurentOngaro/UEVaultManager#readme to set it up properly')
                 subprocess.Popen(['cmd', '/K', 'echo>nul'])
         return
 
     cli = UEVaultManagerCLI(override_config=args.config_file, api_timeout=args.api_timeout)
     ql = cli.setup_threaded_logging()
 
-    conf_log_level = cli.core.lgd.config.get('UEVaultManager', 'log_level', fallback='info')
+    conf_log_level = cli.core.uevmlfs.config.get('UEVaultManager', 'log_level', fallback='info')
     if conf_log_level == 'debug' or args.debug:
         cli.core.verbose_mode = True
         logging.getLogger().setLevel(level=logging.DEBUG)
         # keep requests quiet
         logging.getLogger('requests').setLevel(logging.WARNING)
         logging.getLogger('urllib3').setLevel(logging.WARNING)
 
-    cli.core.create_output_backup = str_to_bool(cli.core.lgd.config.get('UEVaultManager', 'create_output_backup', fallback=True))
-    cli.core.create_log_backup = str_to_bool(cli.core.lgd.config.get('UEVaultManager', 'create_log_backup', fallback=True))
-    cli.core.verbose_mode = str_to_bool(cli.core.lgd.config.get('UEVaultManager', 'verbose_mode', fallback=False))
-    cli.ue_assets_max_cache_duration = int(cli.core.lgd.config.get('UEVaultManager', 'ue_assets_max_cache_duration', fallback=1296000))
-
-    cli.core.ignored_assets_filename_log = cli.core.lgd.config.get('UEVaultManager', 'ignored_assets_filename_log', fallback='')
-    cli.core.notfound_assets_filename_log = cli.core.lgd.config.get('UEVaultManager', 'notfound_assets_filename_log', fallback='')
-    cli.core.bad_data_assets_filename_log = cli.core.lgd.config.get('UEVaultManager', 'bad_data_assets_filename_log', fallback='')
+    cli.core.create_output_backup = str_to_bool(cli.core.uevmlfs.config.get('UEVaultManager', 'create_output_backup', fallback=True))
+    cli.core.create_log_backup = str_to_bool(cli.core.uevmlfs.config.get('UEVaultManager', 'create_log_backup', fallback=True))
+    cli.core.verbose_mode = str_to_bool(cli.core.uevmlfs.config.get('UEVaultManager', 'verbose_mode', fallback=False))
+    cli.ue_assets_max_cache_duration = int(cli.core.uevmlfs.config.get('UEVaultManager', 'ue_assets_max_cache_duration', fallback=1296000))
+
+    cli.core.ignored_assets_filename_log = cli.core.uevmlfs.config.get('UEVaultManager', 'ignored_assets_filename_log', fallback='')
+    cli.core.notfound_assets_filename_log = cli.core.uevmlfs.config.get('UEVaultManager', 'notfound_assets_filename_log', fallback='')
+    cli.core.bad_data_assets_filename_log = cli.core.uevmlfs.config.get('UEVaultManager', 'bad_data_assets_filename_log', fallback='')
 
-    cli.core.engine_version_for_obsolete_assets = cli.core.lgd.config.get('UEVaultManager', 'engine_version_for_obsolete_assets', fallback='4.26')
+    cli.core.engine_version_for_obsolete_assets = cli.core.uevmlfs.config.get('UEVaultManager', 'engine_version_for_obsolete_assets', fallback='4.26')
 
     if cli.core.create_log_backup:
         cli.create_log_file_backup()
 
     # open log file for assets if necessary
     cli.core.setup_assets_logging()
     cli.core.egs.notfound_logger = cli.core.notfound_logger
@@ -1160,26 +1272,19 @@
     if not disable_update_message and hasattr(args, 'csv'):
         disable_update_message = args.csv
 
     # show note if update is available
     if not disable_update_message and cli.core.update_available and cli.core.update_notice_enabled():
         if update_info := cli.core.get_update_info():
             print(f'\nAn update available!')
-            print(f'- New version: {update_info["version"]} - "{update_info["name"]}"')
-            print(f'- Release summary:\n{update_info["summary"]}\n- Release URL: {update_info["gh_url"]}')
-            if update_info['critical']:
+            print(f'- New version: {update_info["version"]} - "{update_info["codename"]}"')
+            print(f'- Release summary:\n{update_info["summary"]}')
+            if update_info['severity'] == UpdateSeverity.HIGH.name:
                 print('! This update is recommended as it fixes major issues.')
-            elif 'downloads' in update_info:
-                dl_platform = 'windows'
-                if sys_platform == 'darwin':
-                    dl_platform = 'macos'
-                elif sys_platform == 'linux':
-                    dl_platform = 'linux'
-
-                print(f'\n- Download URL: {update_info["downloads"][dl_platform]}')
+                print(f'\n- Release URL: {update_info["release_url"]}')
 
     cli.core.clean_exit()
     ql.stop()
     exit(0)
 
 
 if __name__ == '__main__':
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/core.py` & `UEVaultManager-1.3.0/UEVaultManager/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-# coding: utf-8
-
+# coding=utf-8
+"""
+Implementation for:
+- AppCore: handles most of the lower level interaction with the downloader, lfs, and api components to make writing CLI/GUI code easier and cleaner and avoid duplication.
+- CSV_headings: contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
+"""
 import json
 import logging
 import os
 import time
-import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 from base64 import b64decode
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from hashlib import sha1
 from locale import getlocale, LC_CTYPE
 from platform import system
 from threading import current_thread, enumerate as thread_enumerate
 from urllib.parse import urlparse
 
 from requests import session, __version__
 from requests.exceptions import HTTPError, ConnectionError
 
+import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 from UEVaultManager.api.egs import EPCAPI, GrabResult
-from UEVaultManager.api.lgd import LGDAPI
+from UEVaultManager.api.uevm import UEVMAPI
 from UEVaultManager.lfs.egl import EPCLFS
-from UEVaultManager.lfs.lgndry import LGDLFS
+from UEVaultManager.lfs.uevmlfs import UEVMLFS
 from UEVaultManager.models.app import *
 from UEVaultManager.models.exceptions import *
 from UEVaultManager.models.json_manifest import JSONManifest
 from UEVaultManager.models.manifest import Manifest
 from UEVaultManager.utils.cli import check_and_create_path
 from UEVaultManager.utils.egl_crypt import decrypt_epic_data
 from UEVaultManager.utils.env import is_windows_mac_or_pyi
 
 # The heading dict contains the title of each column and a boolean value to know if its contents must be preserved if it already exists in the output file (To Avoid overwriting data changed by the user in the file)
 CSV_headings = {
     'Asset_id': False,  # ! important: Do not Rename => this field is used as main key for each asset
     'App name': False,
     'App title': False,
     'Category': False,
-    'Image': False,
-    'Url': True,  # could be kept if a better url that can be used to download the asset is found
     'UE Version': False,
-    'Compatible Versions': False,
     'Review': False,
     'Developer': False,
     'Description': False,
-    'Uid': False,
-    'Creation Date': False,
-    'Update Date': False,
     'Status': False,
-    # Modified Fields when added into the file (mainly from extras data)
-    'Date Added': True,
-    'Price': False,  # ! important: Rename Wisely => this field is searched by text in the next lines
-    'Old Price': False,  # ! important: always place it after the Price field in the list
-    'On Sale': False,  # ! important: always place it after the Old Price field in the list
+    'Discount Price': False,
+    'On sale': False,
     'Purchased': False,
     'Obsolete': True,
-    # Extracted from page, can be compared with value in metadata. Coud be used to if check data grabbing if OK
     'Supported Versions': False,
-    'Page title': False,
     'Grab result': False,
+    'Price': False,  # ! important: Rename Wisely => this field is searched by text in the next lines
+    'Old Price': False,  # ! important: always place it after the Price field in the list
     # User Fields
     'Comment': True,
     'Stars': True,
-    'Asset Folder': True,
     'Must Buy': True,
     'Test result': True,
     'Installed Folder': True,
-    'Alternative': True
+    'Alternative': True,
+    'Asset Folder': True,
+    # less important fields
+    'Page title': False,
+    'Image': False,
+    'Url': True,  # could be kept if a better url that can be used to download the asset is found
+    'Compatible Versions': False,
+    'Date Added': True,
+    'Creation Date': False,
+    'Update Date': False,
+    'Uid': False
 }
 
 # ToDo: instead of true/false return values for success/failure actually raise an exception that the CLI/GUI
 #  can handle to give the user more details. (Not required yet since there's no GUI so log output is fine)
 
 
 class AppCore:
     """
     AppCore handles most of the lower level interaction with
     the downloader, lfs, and api components to make writing CLI/GUI
     code easier and cleaner and avoid duplication.
+    :param override_config: path to a config file to use instead of the default
+    :param timeout: timeout in seconds for requests
     """
     _egl_version = '11.0.1-14907503+++Portal+Release-Live'
 
     def __init__(self, override_config=None, timeout=10.0):
         self.log = logging.getLogger('Core')
         self.egs = EPCAPI(timeout=timeout)
-        self.lgd = LGDLFS(config_file=override_config)
+        self.uevmlfs = UEVMLFS(config_file=override_config)
         self.egl = EPCLFS()
-        self.lgd_api = LGDAPI()
+        self.uevm_api = UEVMAPI()
 
         # on non-Windows load the programdata path from config
         if os.name != 'nt':
-            self.egl.programdata_path = self.lgd.config.get('UEVaultManager', 'egl_programdata', fallback=None)
+            self.egl.programdata_path = self.uevmlfs.config.get('UEVaultManager', 'egl_programdata', fallback=None)
             if self.egl.programdata_path and not os.path.exists(self.egl.programdata_path):
                 self.log.error(f'Config EGL path ("{self.egl.programdata_path}") is invalid! Disabling sync...')
                 self.egl.programdata_path = None
-                self.lgd.config.remove_option('UEVaultManager', 'egl_programdata')
-                self.lgd.save_config()
+                self.uevmlfs.config.remove_option('UEVaultManager', 'egl_programdata')
+                self.uevmlfs.save_config()
 
         self.local_timezone = datetime.now().astimezone().tzinfo
         self.language_code, self.country_code = ('en', 'US')
 
-        if locale := self.lgd.config.get('UEVaultManager', 'locale', fallback=getlocale(LC_CTYPE)[0]):
+        if locale := self.uevmlfs.config.get('UEVaultManager', 'locale', fallback=getlocale(LC_CTYPE)[0]):
             try:
                 self.language_code, self.country_code = locale.split('-' if '-' in locale else '_')
                 self.log.debug(f'Set locale to {self.language_code}-{self.country_code}')
                 # adjust egs api language as well
                 self.egs.language_code, self.egs.country_code = self.language_code, self.country_code
             except Exception as error:
                 self.log.warning(f'Getting locale failed: {error!r}, falling back to using en-US.')
@@ -135,40 +141,45 @@
         # new file loggers
         self.ignored_logger = None
         self.notfound_logger = None
         self.bad_data_logger = None
         # store time to process metadata and extras update
         self.process_time_average = {'time': 0.0, 'count': 0}
         self.use_threads = False
+        self.thread_executor = None
+        self.thread_executor_must_stop = False
         self.engine_version_for_obsolete_assets = '4.26'
 
-    def setup_assets_logging(self):
+    def setup_assets_logging(self) -> None:
+        """
+        Setup logging for ignored, not found and bad data assets
+        """
         formatter = logging.Formatter('%(message)s')
         message = f"-----\n{datetime.now().strftime(self.default_datetime_format)} Log Started\n-----\n"
 
         if self.ignored_assets_filename_log != '':
-            ignored_assets_filename_log = self.ignored_assets_filename_log.replace('~/.config', self.lgd.path)
+            ignored_assets_filename_log = self.ignored_assets_filename_log.replace('~/.config', self.uevmlfs.path)
             if check_and_create_path(ignored_assets_filename_log):
                 ignored_assets_handler = logging.FileHandler(ignored_assets_filename_log, mode='w')
                 ignored_assets_handler.setFormatter(formatter)
                 self.ignored_logger = logging.Logger('IgnoredAssets', 'INFO')
                 self.ignored_logger.addHandler(ignored_assets_handler)
                 self.ignored_logger.info(message)
 
         if self.notfound_assets_filename_log != '':
-            notfound_assets_filename_log = self.notfound_assets_filename_log.replace('~/.config', self.lgd.path)
+            notfound_assets_filename_log = self.notfound_assets_filename_log.replace('~/.config', self.uevmlfs.path)
             if check_and_create_path(notfound_assets_filename_log):
                 notfound_assets_handler = logging.FileHandler(notfound_assets_filename_log, mode='w')
                 notfound_assets_handler.setFormatter(formatter)
                 self.notfound_logger = logging.Logger('NotFoundAssets', 'INFO')
                 self.notfound_logger.addHandler(notfound_assets_handler)
                 self.notfound_logger.info(message)
 
         if self.bad_data_assets_filename_log != '':
-            bad_data_assets_filename_log = self.bad_data_assets_filename_log.replace('~/.config', self.lgd.path)
+            bad_data_assets_filename_log = self.bad_data_assets_filename_log.replace('~/.config', self.uevmlfs.path)
             if check_and_create_path(bad_data_assets_filename_log):
                 bad_data_assets_handler = logging.FileHandler(bad_data_assets_filename_log, mode='w')
                 bad_data_assets_handler.setFormatter(formatter)
                 self.bad_data_logger = logging.Logger('BadDataAssets', 'INFO')
                 self.bad_data_logger.addHandler(bad_data_assets_handler)
                 self.bad_data_logger.info(message)
 
@@ -213,26 +224,26 @@
         return ''
 
     def auth_code(self, code) -> bool:
         """
         Handles authentication via authorization code (either retrieved manually or automatically)
         """
         try:
-            self.lgd.userdata = self.egs.start_session(authorization_code=code)
+            self.uevmlfs.userdata = self.egs.start_session(authorization_code=code)
             return True
         except Exception as error:
             self.log.error(f'Logging in failed with {error!r}, please try again.')
             return False
 
     def auth_ex_token(self, code) -> bool:
         """
         Handles authentication via exchange token (either retrieved manually or automatically)
         """
         try:
-            self.lgd.userdata = self.egs.start_session(exchange_token=code)
+            self.uevmlfs.userdata = self.egs.start_session(exchange_token=code)
             return True
         except Exception as error:
             self.log.error(f'Logging in failed with {error!r}, please try again.')
             return False
 
     def auth_import(self) -> bool:
         """Import refresh token from EGL installation and use it for logging in"""
@@ -253,30 +264,30 @@
         else:
             re_data = json.loads(raw_data)[0]
 
         if 'Token' not in re_data:
             raise ValueError('No login session in config')
         refresh_token = re_data['Token']
         try:
-            self.lgd.userdata = self.egs.start_session(refresh_token=refresh_token)
+            self.uevmlfs.userdata = self.egs.start_session(refresh_token=refresh_token)
             return True
         except Exception as error:
             self.log.error(f'Logging in failed with {error!r}, please try again.')
             return False
 
     def login(self, force_refresh=False) -> bool:
         """
         Attempts logging in with existing credentials.
 
         raises ValueError if no existing credentials or InvalidCredentialsError if the API return an error
         """
-        if not self.lgd.userdata:
+        if not self.uevmlfs.userdata:
             raise ValueError('No saved credentials')
-        elif self.logged_in and self.lgd.userdata['expires_at']:
-            dt_exp = datetime.fromisoformat(self.lgd.userdata['expires_at'][:-1])
+        elif self.logged_in and self.uevmlfs.userdata['expires_at']:
+            dt_exp = datetime.fromisoformat(self.uevmlfs.userdata['expires_at'][:-1])
             dt_now = datetime.utcnow()
             td = dt_now - dt_exp
 
             # if session still has at least 10 minutes left we can re-use it.
             if dt_exp > dt_now and abs(td.total_seconds()) > 600:
                 return True
             else:
@@ -284,152 +295,200 @@
 
         # run update check
         if self.update_check_enabled():
             try:
                 self.check_for_updates()
             except Exception as error:
                 self.log.warning(f'Checking for UEVaultManager updates failed: {error!r}')
-        else:
-            self.apply_lgd_config()
 
-        if self.lgd.userdata['expires_at'] and not force_refresh:
-            dt_exp = datetime.fromisoformat(self.lgd.userdata['expires_at'][:-1])
+        if self.uevmlfs.userdata['expires_at'] and not force_refresh:
+            dt_exp = datetime.fromisoformat(self.uevmlfs.userdata['expires_at'][:-1])
             dt_now = datetime.utcnow()
             td = dt_now - dt_exp
 
             # if session still has at least 10 minutes left we can re-use it.
             if dt_exp > dt_now and abs(td.total_seconds()) > 600:
                 self.log.info('Trying to re-use existing login session...')
                 try:
-                    self.egs.resume_session(self.lgd.userdata)
+                    self.egs.resume_session(self.uevmlfs.userdata)
                     self.logged_in = True
                     return True
                 except InvalidCredentialsError as error:
                     self.log.warning(f'Resuming failed due to invalid credentials: {error!r}')
                 except Exception as error:
                     self.log.warning(f'Resuming failed for unknown reason: {error!r}')
                 # If verify fails just continue the normal authentication process
                 self.log.info('Falling back to using refresh token...')
 
         try:
             self.log.info('Logging in...')
-            userdata = self.egs.start_session(self.lgd.userdata['refresh_token'])
+            userdata = self.egs.start_session(self.uevmlfs.userdata['refresh_token'])
         except InvalidCredentialsError:
             self.log.error('Stored credentials are no longer valid! Please login again.')
-            self.lgd.invalidate_userdata()
+            self.uevmlfs.invalidate_userdata()
             return False
         except (HTTPError, ConnectionError) as error:
             self.log.error(f'HTTP request for login failed: {error!r}, please try again later.')
             return False
 
-        self.lgd.userdata = userdata
+        self.uevmlfs.userdata = userdata
         self.logged_in = True
         return True
 
-    def update_check_enabled(self):
-        return not self.lgd.config.getboolean('UEVaultManager', 'disable_update_check', fallback=False)
+    def update_check_enabled(self) -> bool:
+        """
+        Returns whether update checks are enabled or not
+        :return: True if update checks are enabled, False otherwise
+        """
+        return not self.uevmlfs.config.getboolean('UEVaultManager', 'disable_update_check', fallback=False)
 
-    def update_notice_enabled(self):
+    def update_notice_enabled(self) -> bool:
+        """
+        Returns whether update notices are enabled or not
+        :return: True if update notices are enabled, False otherwise
+        """
         if self.force_show_update:
             return True
-        return not self.lgd.config.getboolean('UEVaultManager', 'disable_update_notice', fallback=not is_windows_mac_or_pyi())
+        return not self.uevmlfs.config.getboolean('UEVaultManager', 'disable_update_notice', fallback=not is_windows_mac_or_pyi())
 
-    def check_for_updates(self, force=False):
+    def check_for_updates(self, force=False) -> None:
+        """
+        Checks for updates and sets the update_available flag accordingly
+        :param force: force update check
+        """
 
         def version_tuple(v):
+            """
+            Converts a version string to a tuple of ints
+            :param v: version string
+            :return:  tuple of ints
+            """
             return tuple(map(int, (v.split('.'))))
 
-        cached = self.lgd.get_cached_version()
+        cached = self.uevmlfs.get_cached_version()
         version_info = cached['data']
         if force or not version_info or (datetime.now().timestamp() - cached['last_update']) > 24 * 3600:
-            version_info = self.lgd_api.get_version_information()
-            self.lgd.set_cached_version(version_info)
-
-        web_version = version_info['release_info']['version']
+            version_info = self.uevm_api.get_version_information()
+            self.uevmlfs.set_cached_version(version_info)
 
+        web_version = version_info['version']
         self.update_available = version_tuple(web_version) > version_tuple(__version__)
-        # version check is disabled because it's checking for Legendary
-        # TODO: check UEVaultManager updates instead
         self.update_available = False
 
-        self.apply_lgd_config(version_info)
+    def get_update_info(self) -> dict:
+        """
+        Returns update info dict
+        :return: update info dict
+        """
+        return self.uevmlfs.get_cached_version()['data']
 
-    def apply_lgd_config(self, version_info=None):
-        """Applies configuration options returned by update API"""
-        if not version_info:
-            version_info = self.lgd.get_cached_version()['data']
-        # if cached data is invalid
-        if not version_info:
-            self.log.debug('No cached UEVaultManager config to apply.')
-            return
-
-        if 'egl_config' in version_info:
-            self.egs.update_egs_params(version_info['egl_config'])
-            self._egl_version = version_info['egl_config'].get('version', self._egl_version)
-            for data_key in version_info['egl_config'].get('data_keys', []):
-                if data_key not in self.egl.data_keys:
-                    self.egl.data_keys.append(data_key)
-
-        if lgd_config := version_info.get('legendary_config'):
-            self.webview_killswitch = lgd_config.get('webview_killswitch', False)
-
-    def get_update_info(self):
-        return self.lgd.get_cached_version()['data'].get('release_info')
-
-    def update_aliases(self, force=False):
-        _aliases_enabled = not self.lgd.config.getboolean('UEVaultManager', 'disable_auto_aliasing', fallback=False)
-        if _aliases_enabled and (force or not self.lgd.aliases):
-            self.lgd.generate_aliases()
+    def update_aliases(self, force=False) -> None:
+        """
+        Updates aliases if enabled
+        :param force: force alias update
+        """
+        _aliases_enabled = not self.uevmlfs.config.getboolean('UEVaultManager', 'disable_auto_aliasing', fallback=False)
+        if _aliases_enabled and (force or not self.uevmlfs.aliases):
+            self.uevmlfs.generate_aliases()
 
     def get_assets(self, update_assets=False, platform='Windows') -> List[AppAsset]:
+        """
+        Returns a list of assets for the given platform.
+        :param update_assets: if True, always fetches a new list of assets from the server
+        :param platform: platform to fetch assets for
+        :return: list of AppAsset objects
+        """
         # do not save and always fetch list when platform is overridden
-        if not self.lgd.assets or update_assets or platform not in self.lgd.assets:
+        if not self.uevmlfs.assets or update_assets or platform not in self.uevmlfs.assets:
             # if not logged in, return empty list
             if not self.egs.user:
                 return []
 
-            assets = self.lgd.assets.copy() if self.lgd.assets else dict()
+            assets = self.uevmlfs.assets.copy() if self.uevmlfs.assets else dict()
 
             assets.update({platform: [AppAsset.from_egs_json(a) for a in self.egs.get_item_assets(platform=platform)]})
 
             # only save (and write to disk) if there were changes
-            if self.lgd.assets != assets:
-                self.lgd.assets = assets
+            if self.uevmlfs.assets != assets:
+                self.uevmlfs.assets = assets
 
-        return self.lgd.assets[platform]
+        return self.uevmlfs.assets[platform]
 
-    def get_asset(self, app_name, platform='Windows', update=False) -> AppAsset:
-        if update or platform not in self.lgd.assets:
+    def get_asset(self, app_name: str, platform='Windows', update=False) -> AppAsset:
+        """
+        Returns an AppAsset object for the given app name and platform
+        :param app_name: app name to get
+        :param platform: platform to get asset for
+        :param update: force update of asset list
+        :return: AppAsset object
+        """
+        if update or platform not in self.uevmlfs.assets:
             self.get_assets(update_assets=True, platform=platform)
 
         try:
-            return next(i for i in self.lgd.assets[platform] if i.app_name == app_name)
+            return next(i for i in self.uevmlfs.assets[platform] if i.app_name == app_name)
         except StopIteration:
             raise ValueError
 
     def asset_available(self, item: App, platform='Windows') -> bool:
+        """
+        Returns whether an asset is available for the given item and platform
+        :param item: item to check
+        :param platform:
+        :return: True if asset is available, False otherwise
+        """
         # Just say yes for Origin titles
         if item.third_party_store:
             return True
 
         try:
             asset = self.get_asset(item.app_name, platform=platform)
             return asset is not None
         except ValueError:
             return False
 
     def get_item(self, app_name, update_meta=False, platform='Windows') -> App:
+        """
+        Returns an App object
+        :param app_name: name to get
+        :param update_meta: force update of metadata
+        :param platform: platform to get app for
+        :return: App object
+        """
         if update_meta:
             self.get_asset_list(True, platform=platform)
-        return self.lgd.get_item_meta(app_name)
+        return self.uevmlfs.get_item_meta(app_name)
 
     def get_asset_list(self, update_assets=True, platform='Windows', filter_category='', force_refresh=False) -> (List[App], Dict[str, List[App]]):
+        """
+        Returns a list of all available assets for the given platform
+        :param update_assets: force update of asset list
+        :param platform: platform to get assets for
+        :param filter_category: filter by category
+        :param force_refresh: force refresh of asset list
+        :return: Assets list
+        """
+
+        # Cancel all outstanding tasks and shut down the executor
+        def stop_executor(tasks) -> None:
+            """
+            Cancel all outstanding tasks and shut down the executor
+            :param tasks: tasks to cancel
+            """
+            for _, task in tasks.items():
+                task.cancel()
+            self.thread_executor.shutdown(wait=False)
 
         def fetch_asset_meta(name: str) -> bool:
-            if (name in currently_fetching or not fetch_list.get(name)) and ('Asset_Fetcher' in thread_enumerate()):
+            """
+            Fetches asset metadata for the given app name and adds it to the list of assets
+            :param name: app name
+            :return: True if successful, False otherwise
+            """
+            if (name in currently_fetching or not fetch_list.get(name)) and ('Asset_Fetcher' in thread_enumerate()) or self.thread_executor_must_stop:
                 return False
 
             thread_data = ''
             if self.use_threads:
                 thread = current_thread()
                 thread_data = f' ==> By Thread name={thread.name}'
 
@@ -438,21 +497,21 @@
             currently_fetching[name] = True
             start_time = datetime.now()
             name, namespace, catalog_item_id, _process_meta, _process_extras = fetch_list[name]
 
             if _process_meta:
                 eg_meta = self.egs.get_item_info(namespace, catalog_item_id, timeout=10.0)
                 app = App(app_name=name, app_title=eg_meta['title'], metadata=eg_meta, asset_infos=assets[name])
-                self.lgd.set_item_meta(app.app_name, app)
+                self.uevmlfs.set_item_meta(app.app_name, app)
                 apps[name] = app
 
             if _process_extras:
                 # we use title because it's less ambiguous than a name when searching an asset
                 eg_extras = self.egs.get_assets_extras(asset_name=name, asset_title=apps[name].app_title, verbose_mode=self.verbose_mode)
-                self.lgd.set_item_extras(app_name=name, extras=eg_extras, update_global_dict=True)
+                self.uevmlfs.set_item_extras(app_name=name, extras=eg_extras, update_global_dict=True)
 
                 # log the asset if the title in metadata and the title in the marketplace grabbed page are not identical
                 if eg_extras['page_title'] != '' and eg_extras['page_title'] != apps[name].app_title:
                     self.log.warning(f'{name} has incoherent data. It has been added to the bad_data_logger file')
                     eg_extras['grab_result'] = GrabResult.INCONSISTANT_DATA.name
                     if self.bad_data_logger:
                         self.bad_data_logger.info(name)
@@ -474,14 +533,17 @@
             if not self.use_threads:
                 process_average = self.process_time_average['time'] / self.process_time_average['count']
                 self.log.info(f'===Time Average={process_average:.3f} s # ({(len(fetch_list) * process_average):.3f} s time left)')
 
             self.log.info(
                 f'--- END fetching data in {name}{thread_data}. Time For Processing={process_time:.3f}s # Still {len(fetch_list)} assets to process'
             )
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                self.thread_executor_must_stop = True
+                return False
             return True
 
         _ret = []
         meta_updated = False
 
         # fetch asset information for Windows, all installed platforms, and the specified one
         platforms = {'Windows'}
@@ -489,21 +551,21 @@
         if gui_g.progress_window_ref is not None:
             gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching platforms...", new_max_value=len(platforms))
         for _platform in platforms:
             self.get_assets(update_assets=update_assets, platform=_platform)
             if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
                 return []
 
-        if not self.lgd.assets:
+        if not self.uevmlfs.assets:
             return _ret
 
         assets = {}
         if gui_g.progress_window_ref is not None:
-            gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching assets...", new_max_value=len(self.lgd.assets.items()))
-        for _platform, _assets in self.lgd.assets.items():
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching assets...", new_max_value=len(self.uevmlfs.assets.items()))
+        for _platform, _assets in self.uevmlfs.assets.items():
             for _asset in _assets:
                 if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
                     return []
                 if _asset.app_name in assets:
                     assets[_asset.app_name][_platform] = _asset
                 else:
                     assets[_asset.app_name] = {_platform: _asset}
@@ -561,15 +623,15 @@
                 return []
             item = valid_items[i]
             app_name = item['name']
             app_assets = item['asset']
             if self.verbose_mode:
                 self.log.info(f'Checking {app_name}....')
 
-            item_metadata = self.lgd.get_item_meta(app_name)
+            item_metadata = self.uevmlfs.get_item_meta(app_name)
             asset_updated = False
 
             if not item_metadata:
                 self.log.info(f'Metadata for {app_name} are missing. It Will be ADDED to the FETCH list')
             else:
                 category = str(item_metadata.metadata['categories'][0]['path']).lower()
                 if filter_category and filter_category.lower() not in category:
@@ -587,15 +649,15 @@
                 self.log.debug(f'{app_name} has been ADDED to the apps list with asset_updated={asset_updated}')
 
             # get extras data only in not filtered
             if force_refresh or asset_updated:
                 process_extras = True
             else:
                 # will read the extras data from file if necessary and put in the global dict
-                process_extras = self.lgd.get_item_extras(app_name) is None
+                process_extras = self.uevmlfs.get_item_extras(app_name) is None
 
             process_meta = not item_metadata or force_refresh or asset_updated
 
             if update_assets and (process_extras or process_meta):
                 self.log.debug(f'Scheduling metadata and extras update for {app_name}')
                 # namespace/catalog item are the same for all platforms, so we can just use the first one
                 _ga = next(iter(app_assets.values()))
@@ -606,30 +668,44 @@
             # end while i < len(valid_items):
 
         # setup and teardown of thread pool takes some time, so only do it when it makes sense.
         self.use_threads = len(fetch_list) > 5
         # self.use_threads = False  # test only
         if fetch_list:
             if gui_g.progress_window_ref is not None:
-                gui_g.progress_window_ref.reset(new_value=0, new_text="Fetching missing metadata...\nIt Could take a while !", new_max_value=0)
-                gui_g.progress_window_ref.hide_progress_bar()
-                gui_g.progress_window_ref.hide_stop_button()
+                gui_g.progress_window_ref.reset(
+                    new_value=0, new_text="Fetching missing metadata...\nIt could take some time. Be patient.", new_max_value=len(fetch_list)
+                )
+                # gui_g.progress_window_ref.hide_progress_bar()
+                # gui_g.progress_window_ref.hide_stop_button()
 
             self.log.info(f'Fetching metadata for {len(fetch_list)} app(s).')
             if self.use_threads:
                 # note:  unreal engine API limits the number of connection to 16. So no more than 16 threads !
-                with ThreadPoolExecutor(max_workers=min(16, os.cpu_count() + 2), thread_name_prefix="Asset_Fetcher") as executor:
-                    executor.map(fetch_asset_meta, fetch_list.keys(), timeout=30.0)
+
+                # with ThreadPoolExecutor(max_workers=min(16, os.cpu_count() - 2), thread_name_prefix="Asset_Fetcher") as executor:
+                #    executor.map(fetch_asset_meta, fetch_list.keys(), timeout=30.0)
+                self.thread_executor = ThreadPoolExecutor(max_workers=min(16, os.cpu_count() + 2), thread_name_prefix="Asset_Fetcher")
+                # Dictionary that maps each key to its corresponding Future object
+                futures = {}
+                for key in fetch_list.keys():
+                    # Submit the task and add its Future to the dictionary
+                    future = self.thread_executor.submit(fetch_asset_meta, key)
+                    futures[key] = future
+                    if self.thread_executor_must_stop:
+                        self.log.info(f'User stop has been pressed. Stopping running threads....')
+                        stop_executor(futures)
+                        return []
 
         self.log.info(f'A total of {bypass_count} on {len(valid_items)} assets have been bypassed in phase 2')
         self.log.info(f'======\nSTARTING phase 3: emptying the List of assets to be fetched \n')
         if gui_g.progress_window_ref is not None:
-            gui_g.progress_window_ref.show_progress_bar()  # show progress bar, must be before reset
+            # gui_g.progress_window_ref.show_progress_bar()  # show progress bar, must be before reset
             gui_g.progress_window_ref.show_stop_button()
-            gui_g.progress_window_ref.reset(new_value=0, new_text="Checking assets data...", new_max_value=len(filtered_items))
+            gui_g.progress_window_ref.reset(new_value=0, new_text="Checking and Fetching assets data...", new_max_value=len(filtered_items))
         # loop through valid and filtered items
         meta_updated = (bypass_count == 0) and meta_updated  # to avoid deleting metadata files or assets that have been filtered
         while len(filtered_items) > 0:
             if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
                 return []
             item = filtered_items.pop()
             app_name = item['name']
@@ -675,51 +751,74 @@
                 _ret.append(app_item)
 
         self.log.info(f'A total of {len(_ret)} assets have been analysed and kept in phase 3')
 
         self.update_aliases(force=meta_updated)
 
         if meta_updated:
+            if gui_g.progress_window_ref is not None:
+                gui_g.progress_window_ref.reset(new_value=0, new_text="Updating metadata files...", new_max_value=len(_ret))
             # delete old files
             self._prune_metadata()
             self._save_metadata(_ret)
         #  meta_updated = True  # test only
         if meta_updated:
+            if gui_g.progress_window_ref is not None:
+                gui_g.progress_window_ref.reset(new_value=0, new_text="Updating extras data files...", new_max_value=len(_ret))
             # save new ones
             self._prune_extras_data(update_global_dict=False)
-            self._save_extras_data(self.lgd.assets_extras_data, update_global_dict=False)
+            self._save_extras_data(self.uevmlfs.assets_extras_data, update_global_dict=False)
         return _ret
 
     # end def get_asset_list(self, update_assets=True, platform='Windows', filter_category='') -> (List[App], Dict[str, List[App]]):
 
-    def _prune_metadata(self):
+    def _prune_metadata(self) -> None:
+        """
+        Compile a list of assets without assets, then delete their metadata
+        """
         # compile list of assets without assets, then delete their metadata
         available_assets = set()
         available_assets |= {i.app_name for i in self.get_assets(platform='Windows')}
 
-        for app_name in self.lgd.get_item_app_names():
+        for app_name in self.uevmlfs.get_item_app_names():
             self.log.debug(f'Removing old/unused metadata for "{app_name}"')
-            self.lgd.delete_item_meta(app_name)
+            self.uevmlfs.delete_item_meta(app_name)
 
-    def _prune_extras_data(self, update_global_dict: True):
-        # compile list of assets without assets, then delete their extras data
+    def _prune_extras_data(self, update_global_dict: True) -> None:
+        """
+        Compile a list of assets without assets, then delete their extras data
+        :param update_global_dict:  if True, update the global dict
+        """
         available_assets = set()
         available_assets |= {i.app_name for i in self.get_assets(platform='Windows')}
 
-        for app_name in self.lgd.get_item_app_names():
+        for app_name in self.uevmlfs.get_item_app_names():
             self.log.debug(f'Removing old/unused extras data for "{app_name}"')
-            self.lgd.delete_item_extras(app_name, update_global_dict=update_global_dict)
+            self.uevmlfs.delete_item_extras(app_name, update_global_dict=update_global_dict)
 
-    def _save_metadata(self, assets):
+    def _save_metadata(self, assets) -> None:
+        """
+        Save the metadata for the given assets
+        :param assets:  List of assets to save
+        """
         for app in assets:
-            self.lgd.set_item_meta(app.app_name, app)
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return
+            self.uevmlfs.set_item_meta(app.app_name, app)
 
-    def _save_extras_data(self, extras: dict, update_global_dict: True):
+    def _save_extras_data(self, extras: dict, update_global_dict: True) -> None:
+        """
+        Save the extras data for the given assets
+        :param extras: Dict of extras data to save
+        :param update_global_dict: if True, update the global dict
+        """
         for app_name, eg_extras in extras.items():
-            self.lgd.set_item_extras(app_name=app_name, extras=eg_extras, update_global_dict=update_global_dict)
+            if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
+                return
+            self.uevmlfs.set_item_extras(app_name=app_name, extras=eg_extras, update_global_dict=update_global_dict)
 
     def get_non_asset_library_items(self, force_refresh=False, skip_ue=True) -> (List[App], Dict[str, List[App]]):
         """
         Gets a list of Items without assets for installation, for instance Items delivered via
         third-party stores that do not have assets for installation
 
         :param force_refresh: Force a metadata refresh
@@ -732,45 +831,46 @@
 
         for lib_item in self.egs.get_library_items():
             if lib_item['namespace'] == 'ue' and skip_ue:
                 continue
             if lib_item['appName'] in ignore:
                 continue
 
-            item = self.lgd.get_item_meta(lib_item['appName'])
+            item = self.uevmlfs.get_item_meta(lib_item['appName'])
             if not item or force_refresh:
                 eg_meta = self.egs.get_item_info(lib_item['namespace'], lib_item['catalogItemId'])
                 item = App(app_name=lib_item['appName'], app_title=eg_meta['title'], metadata=eg_meta)
-                self.lgd.set_item_meta(item.app_name, item)
+                self.uevmlfs.set_item_meta(item.app_name, item)
 
             if not any(i['path'] == 'mods' for i in item.metadata.get('categories', [])):
                 _ret.append(item)
 
         # Force refresh to make sure these titles are included in aliasing
         self.update_aliases(force=True)
         return _ret
 
-    def get_app_environment(self, app_name) -> dict:
-        # get environment overrides from config
-        env = dict()
-        if 'default.env' in self.lgd.config:
-            env |= {k: v for k, v in self.lgd.config['default.env'].items() if v and not k.startswith(';')}
-        if f'{app_name}.env' in self.lgd.config:
-            env |= {k: v for k, v in self.lgd.config[f'{app_name}.env'].items() if v and not k.startswith(';')}
-
-        return env
-
     @staticmethod
     def load_manifest(data: bytes) -> Manifest:
+        """
+        Load a manifest
+        :param data: Bytes object to load the manifest from
+        :return: Manifest object
+        """
         if data[0:1] == b'{':
             return JSONManifest.read_all(data)
         else:
             return Manifest.read_all(data)
 
     def get_cdn_urls(self, item, platform='Windows'):
+        """
+        Get the CDN URLs
+        :param item: Item to get the CDN URLs for
+        :param platform: Platform to get the CDN URLs for
+        :return: List of CDN URLs
+        """
         m_api_r = self.egs.get_item_manifest(item.namespace, item.catalog_item_id, item.app_name, platform)
 
         # never seen this outside the launcher itself, but if it happens: PANIC!
         if len(m_api_r['elements']) > 1:
             raise ValueError('Manifest response has more than one element!')
 
         manifest_hash = m_api_r['elements'][0]['hash']
@@ -786,14 +886,21 @@
                 manifest_urls.append(f'{manifest["uri"]}?{params}')
             else:
                 manifest_urls.append(manifest['uri'])
 
         return manifest_urls, base_urls, manifest_hash
 
     def get_cdn_manifest(self, item, platform='Windows', disable_https=False):
+        """
+        Get the CDN manifest
+        :param item: Item to get the CDN manifest for
+        :param platform: Platform to get the CDN manifest for
+        :param disable_https: Disable HTTPS for the manifest URLs
+        :return: list of base URLs, manifest hash
+        """
         manifest_urls, base_urls, manifest_hash = self.get_cdn_urls(item, platform)
         if not manifest_urls:
             raise ValueError('No manifest URLs returned by API')
 
         if disable_https:
             manifest_urls = [url.replace('https://', 'http://') for url in manifest_urls]
 
@@ -817,54 +924,59 @@
             raise ValueError(f'Unable to get manifest from any CDN URL, last result: {r.status_code} ({r.reason})')
 
         if sha1(manifest_bytes).hexdigest() != manifest_hash:
             raise ValueError('Manifest sha hash mismatch!')
 
         return manifest_bytes, base_urls
 
-    def get_uri_manifest(self, uri):
+    def get_uri_manifest(self, uri: str) -> (bytes, List[str]):
+        """
+        Get the manifest
+        :param uri: URI to get the manifest from
+        :return:  Manifest data and base URLs
+        """
         if uri.startswith('http'):
             r = self.egs.unauth_session.get(uri)
             r.raise_for_status()
             new_manifest_data = r.content
             base_urls = [r.url.rpartition('/')[0]]
         else:
             base_urls = []
             with open(uri, 'rb') as f:
                 new_manifest_data = f.read()
 
         return new_manifest_data, base_urls
 
-    def get_delta_manifest(self, base_url, old_build_id, new_build_id):
-        """Get optimized delta manifest (doesn't seem to exist for most games)"""
-        if old_build_id == new_build_id:
-            return None
-
-        r = self.egs.unauth_session.get(f'{base_url}/Deltas/{new_build_id}/{old_build_id}.delta')
-        return r.content if r.status_code == 200 else None
-
     # Check if the UE assets metadata cache must be updated
-    def check_for_ue_assets_updates(self, assets_count: int, force_refresh=False):
+    def check_for_ue_assets_updates(self, assets_count: int, force_refresh=False) -> None:
+        """
+        Check if the UE assets metadata cache must be updated
+        :param assets_count: assets count from the API
+        :param force_refresh: force the refresh of the cache
+        """
         self.cache_is_invalidate = False
-        cached = self.lgd.get_ue_assets_cache_data()
+        cached = self.uevmlfs.get_ue_assets_cache_data()
         cached_assets_count = cached['ue_assets_count']
 
         date_now = datetime.now().timestamp()
         date_diff = date_now - cached['last_update']
 
         if not cached_assets_count or cached_assets_count != assets_count:
             self.log.info(f'New assets are available. {assets_count} available VS {cached_assets_count} in cache')
-            self.lgd.set_ue_assets_cache_data(last_update=cached['last_update'], ue_assets_count=assets_count)
+            self.uevmlfs.set_ue_assets_cache_data(last_update=cached['last_update'], ue_assets_count=assets_count)
 
         if force_refresh or date_diff > self.ue_assets_max_cache_duration:
             self.cache_is_invalidate = True
-            self.lgd.set_ue_assets_cache_data(last_update=date_now, ue_assets_count=assets_count)
+            self.uevmlfs.set_ue_assets_cache_data(last_update=date_now, ue_assets_count=assets_count)
             if not force_refresh:
                 self.log.info(f'Data cache is outdated. Cache age is {date_diff:.1f} s OR {str(timedelta(seconds=date_diff))}')
         else:
             self.log.info(f'Data cache is still valid. Cache age is {str(timedelta(seconds=date_diff))}')
 
-    def clean_exit(self, code=0):
-        """ Do cleanup, config saving, and exit. """
-        self.lgd.save_config()
+    def clean_exit(self, code=0) -> None:
+        """
+        Do cleanup, config saving, and quit
+        :param code: exit code
+        """
+        self.uevmlfs.save_config()
         logging.shutdown()
         exit(code)
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.3.0/UEVaultManager/downloader/mp/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             self.log.info(f'Found {len(files_to_skip)} files to skip based on include prefix(es)')
             mc.added -= files_to_skip
             mc.changed -= files_to_skip
             mc.unchanged |= files_to_skip
 
         if file_prefix_filter or file_exclude_filter or file_install_tag:
             self.log.info(f'Remaining files after filtering: {len(mc.added) + len(mc.changed)}')
-            # correct install size after filtering
+            # correct instalation size after filtering
             analysis_res.install_size = sum(fm.file_size for fm in manifest.file_manifest_list.elements if fm.filename in mc.added)
 
         if mc.removed:
             analysis_res.removed = len(mc.removed)
             self.log.debug(f'{analysis_res.removed} removed files')
         if mc.added:
             analysis_res.added = len(mc.added)
@@ -227,15 +227,15 @@
         fmlist = sorted(manifest.file_manifest_list.elements, key=lambda a: a.filename.lower())
 
         # Create reference count for chunks and calculate additional/temporary disk size required for install
         current_tmp_size = 0
         for fm in fmlist:
             self.hash_map[fm.filename] = fm.sha_hash.hex()
 
-            # chunks of unchanged files are not downloaded so we can skip them
+            # chunks of unchanged files are not downloaded, so we can skip them
             if fm.filename in mc.unchanged:
                 analysis_res.unchanged += fm.file_size
                 continue
 
             for cp in fm.chunk_parts:
                 references[cp.guid_num] += 1
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.3.0/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.3.0/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.3.0/UEVaultManager/lfs/eos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,52 @@
+# coding=utf-8
+"""
+This package contains the API for interacting with the Epic Games Store.
+"""
 import logging
 import os
 
 from UEVaultManager.models.app import App
 
 if os.name == 'nt':
     from UEVaultManager.lfs.windows_helpers import *
 
 logger = logging.getLogger('EOSUtils')
 # Dummy Game objects to use with Core methods that expect them
 # Overlay
-EOSOverlayApp = App(app_name='98bc04bc842e4906993fd6d6644ffb8d',
-                    app_title='Epic Online Services Overlay',
-                    metadata=dict(namespace='302e5ede476149b1bc3e4fe6ae45e50e',
-                                  id='cc15684f44d849e89e9bf4cec0508b68'))
+EOSOverlayApp = App(
+    app_name='98bc04bc842e4906993fd6d6644ffb8d',
+    app_title='Epic Online Services Overlay',
+    metadata=dict(namespace='302e5ede476149b1bc3e4fe6ae45e50e', id='cc15684f44d849e89e9bf4cec0508b68')
+)
 # EOS Windows service
-EOSHApp = App(app_name='c9e2eb9993a1496c99dc529b49a07339',
-              app_title='Epic Online Services Helper (EOSH)',
-              metadata=dict(namespace='302e5ede476149b1bc3e4fe6ae45e50e',
-                            id='1108a9c0af47438da91331753b22ea21'))
+EOSHApp = App(
+    app_name='c9e2eb9993a1496c99dc529b49a07339',
+    app_title='Epic Online Services Helper (EOSH)',
+    metadata=dict(namespace='302e5ede476149b1bc3e4fe6ae45e50e', id='1108a9c0af47438da91331753b22ea21')
+)
 
 EOS_OVERLAY_KEY = r'SOFTWARE\Epic Games\EOS'
 WINE_EOS_OVERLAY_KEY = EOS_OVERLAY_KEY.replace('\\', '\\\\')
 EOS_OVERLAY_VALUE = 'OverlayPath'
 VULKAN_OVERLAY_KEY = r'SOFTWARE\Khronos\Vulkan\ImplicitLayers'
 
 
 def query_registry_entries(prefix=None):
     if os.name == 'nt':
         # Overlay location for the EOS SDK to load
         overlay_path = query_registry_value(HKEY_CURRENT_USER, EOS_OVERLAY_KEY, EOS_OVERLAY_VALUE)
         # Vulkan Layers
         # HKCU
-        vulkan_hkcu = [i[0] for i in
-                       list_registry_values(HKEY_CURRENT_USER, VULKAN_OVERLAY_KEY)
-                       if 'EOS' in i[0]]
+        vulkan_hkcu = [i[0] for i in list_registry_values(HKEY_CURRENT_USER, VULKAN_OVERLAY_KEY) if 'EOS' in i[0]]
         # HKLM 64 & 32 bit
-        vulkan_hklm = [i[0] for i in
-                       list_registry_values(HKEY_LOCAL_MACHINE, VULKAN_OVERLAY_KEY)
-                       if 'EOS' in i[0]]
-        vulkan_hklm += [i[0] for i in
-                        list_registry_values(HKEY_LOCAL_MACHINE, VULKAN_OVERLAY_KEY, use_32bit_view=True)
-                        if 'EOS' in i[0]]
-
-        return dict(overlay_path=overlay_path,
-                    vulkan_hkcu=vulkan_hkcu,
-                    vulkan_hklm=vulkan_hklm)
+        vulkan_hklm = [i[0] for i in list_registry_values(HKEY_LOCAL_MACHINE, VULKAN_OVERLAY_KEY) if 'EOS' in i[0]]
+        vulkan_hklm += [i[0] for i in list_registry_values(HKEY_LOCAL_MACHINE, VULKAN_OVERLAY_KEY, use_32bit_view=True) if 'EOS' in i[0]]
+
+        return dict(overlay_path=overlay_path, vulkan_hkcu=vulkan_hkcu, vulkan_hklm=vulkan_hklm)
     elif prefix:
         # Only read HKCU since we don't really care for the Vulkan stuff (doesn't work in WINE)
         use_reg_file = os.path.join(prefix, 'user.reg')
         if not os.path.exists(use_reg_file):
             raise ValueError('No user.reg file, invalid path')
 
         reg_lines = open(use_reg_file, 'r', encoding='utf-8').readlines()
@@ -61,26 +59,23 @@
 
         if overlay_path:
             if overlay_path.startswith('C:'):
                 overlay_path = os.path.join(prefix, 'drive_c', overlay_path[3:])
             elif overlay_path.startswith('Z:'):
                 overlay_path = overlay_path[2:]
 
-        return dict(overlay_path=overlay_path,
-                    vulkan_hkcu=list(),
-                    vulkan_hklm=list())
+        return dict(overlay_path=overlay_path, vulkan_hkcu=list(), vulkan_hklm=list())
     else:
         raise ValueError('No prefix specified on non-Windows platform')
 
 
 def add_registry_entries(overlay_path, prefix=None):
     if os.name == 'nt':
         logger.debug(f'Settings HKCU EOS Overlay Path: {overlay_path}')
-        set_registry_value(HKEY_CURRENT_USER, EOS_OVERLAY_KEY, EOS_OVERLAY_VALUE,
-                           overlay_path.replace('\\', '/'), TYPE_STRING)
+        set_registry_value(HKEY_CURRENT_USER, EOS_OVERLAY_KEY, EOS_OVERLAY_VALUE, overlay_path.replace('\\', '/'), TYPE_STRING)
         vk_32_path = os.path.join(overlay_path, 'EOSOverlayVkLayer-Win32.json').replace('/', '\\')
         vk_64_path = os.path.join(overlay_path, 'EOSOverlayVkLayer-Win64.json').replace('/', '\\')
         # the launcher only sets those in HKCU, th e service sets them in HKLM,
         # but it's not in use yet, so just do HKCU for now
         logger.debug(f'Settings HKCU 32-bit Vulkan Layer: {vk_32_path}')
         set_registry_value(HKEY_CURRENT_USER, VULKAN_OVERLAY_KEY, vk_32_path, 0, TYPE_DWORD)
         logger.debug(f'Settings HKCU 64-bit Vulkan Layer: {vk_32_path}')
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/lfs/lgndry.py` & `UEVaultManager-1.3.0/UEVaultManager/lfs/uevmlfs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # coding: utf-8
-
+"""
+Implementation for:
+- UEVMLFS: Local File System
+"""
 import json
 import logging
 import os
 from collections import defaultdict
 from pathlib import Path
 from time import time
 
 from UEVaultManager.models.app import *
 from UEVaultManager.models.config import LGDConf
 from UEVaultManager.utils.aliasing import generate_aliases
 from UEVaultManager.utils.env import is_windows_mac_or_pyi
 from .utils import clean_filename
 
 
-class LGDLFS:
+class UEVMLFS:
+    """
+    Class to handle all local filesystem related tasks
+    :param config_file: Path to config file to use instead of default
+    """
 
     def __init__(self, config_file=None):
-        self.log = logging.getLogger('LGDLFS')
+        self.log = logging.getLogger('UEVMLFS')
 
         if config_path := os.environ.get('XDG_CONFIG_HOME'):
             self.path = os.path.join(config_path, 'UEVaultManager')
         else:
             self.path = os.path.expanduser('~/.config/UEVaultManager')
 
         # EGS user info
@@ -182,192 +189,231 @@
                     for alias in aliases:
                         self.aliases[alias] = app_name
             except Exception as error:
                 self.log.debug(f'Loading aliases failed with {error!r}')
 
     @property
     def userdata(self):
+        """
+        Returns the user data as a dict
+        :return: User data
+        """
         if self._user_data is not None:
             return self._user_data
 
         try:
             self._user_data = json.load(open(os.path.join(self.path, 'user.json')))
             return self._user_data
         except Exception as error:
             self.log.debug(f'Failed to load user data: {error!r}')
             return None
 
     @userdata.setter
-    def userdata(self, userdata):
+    def userdata(self, userdata: dict) -> None:
+        """
+        Set the user data
+        :param userdata: User data
+        """
         if userdata is None:
             raise ValueError('Userdata is none!')
 
         self._user_data = userdata
         json.dump(userdata, open(os.path.join(self.path, 'user.json'), 'w'), indent=2, sort_keys=True)
 
-    def invalidate_userdata(self):
+    def invalidate_userdata(self) -> None:
+        """
+        Invalidate the user data
+        """
         self._user_data = None
         if os.path.exists(os.path.join(self.path, 'user.json')):
             os.remove(os.path.join(self.path, 'user.json'))
 
     @property
-    def entitlements(self):
-        if self._entitlements is not None:
-            return self._entitlements
-
-        try:
-            self._entitlements = json.load(open(os.path.join(self.path, 'entitlements.json')))
-            return self._entitlements
-        except Exception as error:
-            self.log.debug(f'Failed to load entitlements data: {error!r}')
-            return None
-
-    @entitlements.setter
-    def entitlements(self, entitlements):
-        if entitlements is None:
-            raise ValueError('Entitlements is none!')
-
-        self._entitlements = entitlements
-        json.dump(entitlements, open(os.path.join(self.path, 'entitlements.json'), 'w'), indent=2, sort_keys=True)
-
-    @property
     def assets(self):
+        """
+        Returns the assets data as a dict
+        :return: Assets data
+        """
         if self._assets is None:
             try:
                 tmp = json.load(open(os.path.join(self.path, 'assets.json')))
                 self._assets = {k: [AppAsset.from_json(j) for j in v] for k, v in tmp.items()}
             except Exception as error:
                 self.log.debug(f'Failed to load assets data: {error!r}')
                 return None
 
         return self._assets
 
     @assets.setter
-    def assets(self, assets):
+    def assets(self, assets) -> None:
+        """
+        Set the assets data
+        :param assets: data
+        """
         if assets is None:
             raise ValueError('Assets is none!')
 
         self._assets = assets
         json.dump(
             {platform: [a.__dict__ for a in assets] for platform, assets in self._assets.items()},
             open(os.path.join(self.path, 'assets.json'), 'w'),
             indent=2,
             sort_keys=True
         )
 
-    def _get_manifest_filename(self, app_name, version, platform=None):
-        if platform:
-            file_name = clean_filename(f'{app_name}_{platform}_{version}')
-        else:
-            file_name = clean_filename(f'{app_name}_{version}')
-        return os.path.join(self.path, self.manifests_folder, f'{file_name}.manifest')
-
-    def load_manifest(self, app_name, version, platform='Windows'):
-        try:
-            return open(self._get_manifest_filename(app_name, version, platform), 'rb').read()
-        except FileNotFoundError:  # all other errors should propagate
-            self.log.debug(f'Loading manifest failed, retrying without platform in filename...')
-            try:
-                return open(self._get_manifest_filename(app_name, version), 'rb').read()
-            except FileNotFoundError:  # all other errors should propagate
-                return None
-
-    def save_manifest(self, app_name, manifest_data, version, platform='Windows'):
-        with open(self._get_manifest_filename(app_name, version, platform), 'wb') as f:
-            f.write(manifest_data)
+    def delete_folder(self, folder: str, list_of_items_to_keep=None) -> bool:
+        """
+        Delete all the files in a folder that are not in the list_of_items_to_keep list
+        :param folder: The folder to clean
+        :param list_of_items_to_keep: The list of items to keep
+        """
+        if list_of_items_to_keep is None:
+            list_of_items_to_keep = []
+        for f in os.listdir(os.path.join(self.path, folder)):
+            app_name = f.rpartition('.')[0]
+            if list_of_items_to_keep is None or app_name not in list_of_items_to_keep:
+                try:
+                    os.remove(os.path.join(self.path, folder, f))
+                except Exception as error:
+                    self.log.warning(f'Failed to delete file "{f}": {error!r}')
+                    return False
+        return True
 
-    def get_item_meta(self, app_name):
+    def get_item_meta(self, app_name: str):
+        """
+        Get the metadata for an item
+        :param app_name: The name of the item
+        :return: an App object
+        """
         # note: self._assets_metadata is filled ay the start of the list command by reading all the json files in the metadata folder
         if _meta := self.assets_metadata.get(app_name, None):
             return App.from_json(_meta)  # create an object from the App class using the json data
         return None
 
-    def set_item_meta(self, app_name, meta):
+    def set_item_meta(self, app_name: str, meta) -> None:
+        """
+        Set the metadata for an item
+        :param app_name: The name of the item
+        :param meta: The metadata object
+        """
         json_meta = meta.__dict__
         self.assets_metadata[app_name] = json_meta
         meta_file = os.path.join(self.path, 'metadata', f'{app_name}.json')
         json.dump(json_meta, open(meta_file, 'w'), indent=2, sort_keys=True)
 
-    def delete_item_meta(self, app_name: str):
+    def delete_item_meta(self, app_name: str) -> None:
+        """
+        Delete the metadata for an item
+        :param app_name: The name of the item
+        """
         if app_name not in self.assets_metadata:
             raise ValueError(f'Item {app_name} does not exist in metadata DB!')
 
         del self.assets_metadata[app_name]
         meta_file = os.path.join(self.path, 'metadata', f'{app_name}.json')
         if os.path.exists(meta_file):
             os.remove(meta_file)
 
-    def get_item_extras(self, app_name: str):
+    def get_item_extras(self, app_name: str) -> dict:
+        """
+        Get the extras data for an app
+        :param app_name: The app name
+        :return: The extras data
+        """
         gm_file = app_name + '.json'
         extras = self.assets_extras_data.get(app_name, None)
         extras_file = os.path.join(self.path, self.extras_folder, f'{app_name}.json')
         if os.path.exists(extras_file):
-            extras = json.load(open(os.path.join(self.path, self.extras_folder, gm_file)))
-            self.assets_extras_data[extras['asset_name']] = extras
+            try:
+                extras = json.load(open(os.path.join(self.path, self.extras_folder, gm_file)))
+                self.assets_extras_data[extras['asset_name']] = extras
+            except json.decoder.JSONDecodeError:
+                self.log.warning(f'Failed to load extras data for {app_name}!. Deleting file...')
+                # delete the file
+                try:
+                    os.remove(extras_file)
+                except Exception as error:
+                    self.log.error(f'Failed to delete extras file {extras_file}: {error!r}')
+                return {}
         return extras
 
-    def set_item_extras(self, app_name: str, extras: dict, update_global_dict: True):
+    def set_item_extras(self, app_name: str, extras: dict, update_global_dict: True) -> None:
+        """
+        Save the extras data for an app
+        :param app_name: The app name
+        :param extras: The extras data
+        :param update_global_dict: Update the global dict with the new data
+        """
         extras_file = os.path.join(self.path, self.extras_folder, f'{app_name}.json')
         self.log.debug(f'--- SAVING {len(extras)} extras data for {app_name} in {extras_file}')
         json.dump(extras, open(extras_file, 'w'), indent=2, sort_keys=True)
         if update_global_dict:
             self.assets_extras_data[app_name] = extras
 
-    def delete_item_extras(self, app_name: str, update_global_dict: True):
+    def delete_item_extras(self, app_name: str, update_global_dict: True) -> None:
+        """
+        Delete the extras data for an app
+        :param app_name: The app name
+        :param update_global_dict: Update the global dict with the new data
+        """
         if update_global_dict and self.assets_extras_data.get(app_name):
             del self.assets_extras_data[app_name]
         extras_file = os.path.join(self.path, self.extras_folder, f'{app_name}.json')
         if os.path.exists(extras_file):
             os.remove(extras_file)
 
-    def get_item_app_names(self):
+    def get_item_app_names(self) -> list:
+        """
+        Get the list of app names
+        :return: The list of app names
+        """
         return sorted(self.assets_metadata.keys())
 
-    def clean_tmp_data(self):
-        for f in os.listdir(os.path.join(self.path, self.tmp_folder)):
-            try:
-                os.remove(os.path.join(self.path, self.tmp_folder, f))
-            except Exception as error:
-                self.log.warning(f'Failed to delete file "{f}": {error!r}')
-
-    def clean_metadata(self, app_names_to_keep):
-        for f in os.listdir(os.path.join(self.path, self.metadata_folder)):
-            app_name = f.rpartition('.')[0]
-            if app_name not in app_names_to_keep:
-                try:
-                    os.remove(os.path.join(self.path, self.metadata_folder, f))
-                except Exception as error:
-                    self.log.warning(f'Failed to delete file "{f}": {error!r}')
-
-    def clean_extras(self, app_names_to_keep):
-        for f in os.listdir(os.path.join(self.path, self.extras_folder)):
-            app_name = f.rpartition('.')[0]
-            if app_name not in app_names_to_keep:
-                try:
-                    os.remove(os.path.join(self.path, self.extras_folder, f))
-                except Exception as error:
-                    self.log.warning(f'Failed to delete file "{f}": {error!r}')
-
-    def clean_manifests(self):
-        for f in os.listdir(os.path.join(self.path, self.manifests_folder)):
-            try:
-                os.remove(os.path.join(self.path, self.manifests_folder, f))
-            except Exception as error:
-                self.log.warning(f'Failed to delete file "{f}": {error!r}')
-
-    def clean_logs_and_backups(self):
+    def clean_tmp_data(self) -> None:
+        """
+        Delete all the files in the tmp folder
+        """
+        self.delete_folder(self.tmp_folder)
+
+    def clean_metadata(self, app_names_to_keep: list) -> None:
+        """
+        Delete all the metadata files that are not in the app_names_to_keep list
+        :param app_names_to_keep: The list of app names to keep
+        """
+        self.delete_folder(self.metadata_folder, app_names_to_keep)
+
+    def clean_extras(self, app_names_to_keep: list) -> None:
+        """
+        Delete all the metadata files that are not in the app_names_to_keep list
+        :param app_names_to_keep: The list of app names to keep
+        """
+        self.delete_folder(self.extras_folder, app_names_to_keep)
+
+    def clean_manifests(self) -> None:
+        """
+        Delete all the metadata files that are not in the app_names_to_keep list
+        """
+        self.delete_folder(self.manifests_folder)
+
+    def clean_logs_and_backups(self) -> None:
+        """
+        Delete all the log and backup files
+        """
         for f in os.listdir(self.path):
             file_name_no_ext, file_ext = os.path.splitext(f)
             if '.log' in file_ext or '.bak' in file_ext:
                 try:
                     os.remove(os.path.join(self.path, f))
                 except Exception as error:
                     self.log.warning(f'Failed to delete file "{f}": {error!r}')
 
-    def save_config(self):
+    def save_config(self) -> None:
+        """
+        Save the config file
+        """
         # do not save if in read-only mode or file hasn't changed
         if self.config.read_only or not self.config.modified:
             return
         # if config file has been modified externally, back-up the user-modified version before writing
         if os.path.exists(self.config_path):
             if (mod_time := int(os.stat(self.config_path).st_mtime)) != self.config.mod_time:
                 new_filename = f'config.{mod_time}.ini'
@@ -376,53 +422,50 @@
                     f'user-modified config will be renamed to "{new_filename}"...'
                 )
                 os.rename(self.config_path, os.path.join(os.path.dirname(self.config_path), new_filename))
 
         with open(self.config_path, 'w') as cf:
             self.config.write(cf)
 
-    def get_dir_size(self):
+    def get_dir_size(self) -> int:
+        """
+        Get the size of the directory
+        :return: The size of the directory
+        """
         return sum(f.stat().st_size for f in Path(self.path).glob('**/*') if f.is_file())
 
-    def get_cached_version(self):
+    def get_cached_version(self) -> dict:
+        """
+        Get the cached version data
+        :return: version data
+        """
         if self._update_info:
             return self._update_info
-
         try:
             self._update_info = json.load(open(os.path.join(self.path, 'version.json')))
         except Exception as error:
             self.log.debug(f'Failed to load cached update data: {error!r}')
             self._update_info = dict(last_update=0, data=None)
 
         return self._update_info
 
-    def set_cached_version(self, version_data):
+    def set_cached_version(self, version_data: dict) -> None:
+        """
+        Set the cached version data
+        :param version_data: The version data
+        """
         if not version_data:
             return
         self._update_info = dict(last_update=time(), data=version_data)
         json.dump(self._update_info, open(os.path.join(self.path, 'version.json'), 'w'), indent=2, sort_keys=True)
 
-    def get_cached_sdl_data(self, app_name):
-        try:
-            return json.load(open(os.path.join(self.path, self.tmp_folder, f'{app_name}.json')))
-        except Exception as error:
-            self.log.debug(f'Failed to load cached SDL data: {error!r}')
-            return None
-
-    def set_cached_sdl_data(self, app_name, sdl_version, sdl_data):
-        if not app_name or not sdl_data:
-            return
-        json.dump(
-            dict(version=sdl_version, data=sdl_data),
-            open(os.path.join(self.path, self.tmp_folder, f'{app_name}.json'), 'w'),
-            indent=2,
-            sort_keys=True
-        )
-
-    def generate_aliases(self):
+    def generate_aliases(self) -> None:
+        """
+        Generate the list of aliases
+        """
         self.log.debug('Generating list of aliases...')
 
         self.aliases = dict()
         aliases = set()
         collisions = set()
         alias_map = defaultdict(set)
 
@@ -441,30 +484,42 @@
 
         # remove colliding aliases from map and add aliases to lookup table
         for app_name, aliases in alias_map.items():
             alias_map[app_name] -= collisions
             for alias in alias_map[app_name]:
                 self.aliases[alias] = app_name
 
-        def serialise_sets(obj):
-            """Turn sets into sorted lists for storage"""
+        def serialise_sets(obj) -> list:
+            """
+            Turn sets into sorted lists for storage
+            :param obj: The object to serialise
+            """
             return sorted(obj) if isinstance(obj, set) else obj
 
         json.dump(alias_map, open(os.path.join(self.path, 'aliases.json'), 'w', newline='\n'), indent=2, sort_keys=True, default=serialise_sets)
 
-    # Get UE assets metadata cache data
-    def get_ue_assets_cache_data(self):
+    def get_ue_assets_cache_data(self) -> dict:
+        """
+        Get UE assets metadata cache data
+        :return: dict {last_update, ue_assets_count}
+        """
         if self._ue_assets_cache_data:
             return self._ue_assets_cache_data
 
         try:
             self._ue_assets_cache_data = json.load(open(os.path.join(self.path, 'ue_assets_cache_data.json')))
         except Exception as error:
             self.log.debug(f'Failed to UE assets last update data: {error!r}')
             self._ue_assets_cache_data = dict(last_update=0, ue_assets_count=0)
 
         return self._ue_assets_cache_data
 
     # Set UE assets metadata cache data
-    def set_ue_assets_cache_data(self, last_update: float, ue_assets_count: int):
+    def set_ue_assets_cache_data(self, last_update: float, ue_assets_count: int) -> None:
+        """
+        Set UE assets metadata cache data
+        :param last_update: last update time
+        :param ue_assets_count: number of UE assets on last update
+        :return:
+        """
         self._ue_assets_cache_data = dict(last_update=last_update, ue_assets_count=ue_assets_count)
         json.dump(self._ue_assets_cache_data, open(os.path.join(self.path, 'ue_assets_cache_data.json'), 'w'), indent=2, sort_keys=True)
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.3.0/UEVaultManager/lfs/windows_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# coding=utf-8
+"""
+Windows specific helper functions for registry access.
+"""
 import ctypes
 import logging
 import winreg
 
 _logger = logging.getLogger('WindowsHelpers')
 
 HKEY_CURRENT_USER = winreg.HKEY_CURRENT_USER
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/app.py` & `UEVaultManager-1.3.0/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/chunk.py` & `UEVaultManager-1.3.0/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/config.py` & `UEVaultManager-1.3.0/UEVaultManager/models/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 import configparser
 import os
 import time
 
 
 class LGDConf(configparser.ConfigParser):
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/downloading.py` & `UEVaultManager-1.3.0/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/egl.py` & `UEVaultManager-1.3.0/UEVaultManager/models/egl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 from copy import deepcopy
 
 from UEVaultManager.utils.cli import str_to_bool
 
 _template = {
     'AppCategories'         : ['public', 'games', 'applications'],
     'AppName'               : '',
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/gql.py` & `UEVaultManager-1.3.0/UEVaultManager/models/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 # GQL queries needed for the EGS API
 
 uplay_codes_query = '''
 query partnerIntegrationQuery($accountId: String!) {
   PartnerIntegration {
     accountUplayCodes(accountId: $accountId) {
       epicAccountId
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.3.0/UEVaultManager/models/json_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def blob_to_num(in_str):
     """
     The JSON manifest use a rather strange format for storing numbers.
 
     It's essentially %03d for each char concatenated to a string.
     ...instead of just putting the fucking number in the JSON...
 
-    Also it's still little endian so we have to bitshift it.
+    Also, it's still little endian, so we have to bitshift it.
 
     """
     num = 0
     shift = 0
     for i in range(0, len(in_str), 3):
         num += (int(in_str[i:i + 3]) << shift)
         shift += 8
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/models/manifest.py` & `UEVaultManager-1.3.0/UEVaultManager/models/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         s = string.encode('utf-16le')
         bio.write(struct.pack('<i', -(len(string) + 1)))
         bio.write(s)
         bio.write(b'\x00\x00')
 
 
 def get_chunk_dir(version):
-    # The lowest version I've ever seen was 12 (Unreal Tournament), but for completeness sake leave all of them in
+    # The lowest version I've ever seen was 12 (Unreal Tournament), but for completeness’s sake leave all of them in
     if version >= 15:
         return 'ChunksV4'
     elif version >= 6:
         return 'ChunksV3'
     elif version >= 3:
         return 'ChunksV2'
     else:
@@ -247,15 +247,15 @@
         # this build id is used for something called "delta file" which I guess I'll have to implement eventually
         self._build_id = ''
 
     @property
     def build_id(self):
         if self._build_id:
             return self._build_id
-        # this took a while to figure out and get right and I'm still not sure if it'll work for all games :x
+        # this took a while to figure out and get right, and I'm still not sure if it'll work for all games :x
         s = hashlib.sha1()
         s.update(struct.pack('<I', self.app_id))
         s.update(self.app_name.encode('utf-8'))
         s.update(self.build_version.encode('utf-8'))
         s.update(self.launch_exe.encode('utf-8'))
         s.update(self.launch_command.encode('utf-8'))
         self._build_id = b64encode(s.digest()).decode('ascii').replace('+', '-').replace('/', '_').replace('=', '')
@@ -415,15 +415,15 @@
         for _ in range(_cdl.count):
             _cdl.elements.append(ChunkInfo(manifest_version=manifest_version))
 
         # guid, doesn't seem to be a standard like UUID but is fairly straightfoward, 4 bytes, 128 bit.
         for chunk in _cdl.elements:
             chunk.guid = struct.unpack('<IIII', bio.read(16))
 
-        # hash is a 64 bit integer, no idea how it's calculated but we don't need to know that.
+        # hash is a 64-bit integer, no idea how it's calculated, but we don't need to know that.
         for chunk in _cdl.elements:
             chunk.hash = struct.unpack('<Q', bio.read(8))[0]
 
         # sha1 hash
         for chunk in _cdl.elements:
             chunk.sha_hash = bio.read(20)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 """
 GUI module for UEVaultManager
 this can be run directly by executing this script
 or by the --edit command option for the UEVaultManager cli application, for instance by running `cli --edit --input <my_source_file>'
 """
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+# coding=utf-8
+"""
+Implementation for:
+- EditCellWindow: the window to edit a cell
+"""
 import os
 import tkinter as tk
 from tkinter import ttk
 
+from ttkbootstrap.constants import *
+
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 
 
 class EditCellWindow(tk.Toplevel):
     """
     The window to edit a cell
@@ -17,14 +24,16 @@
     :param screen_index: the index of the screen on which the window will be displayed
     :param editable_table: the table to edit
     """
 
     def __init__(self, parent, title: str, width: int = 600, height: int = 400, icon=None, screen_index=0, editable_table=None):
         super().__init__(parent)
         self.title(title)
+        style = gui_f.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
+        self.style = style
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
 
         if icon is None:
             self.attributes('-toolwindow', True)
         else:
             # windows only (remove the minimize/maximize buttons and the icon)
@@ -62,16 +71,19 @@
         The frame containing the control buttons of the window
         :param container: the container of the frame
         """
 
         def __init__(self, container):
             super().__init__(container)
             pack_def_options = {'ipadx': 3, 'ipady': 3, 'fill': tk.X}
-            ttk.Button(self, text='Cancel', command=container.on_close).pack(**pack_def_options, side=tk.RIGHT)
-            ttk.Button(self, text='Save Changes', command=container.save_change).pack(**pack_def_options, side=tk.RIGHT)
+            # (bootstyle is not recognized by PyCharm)
+            # noinspection PyArgumentList
+            ttk.Button(self, text='Close', command=container.on_close, bootstyle=WARNING).pack(**pack_def_options, side=tk.RIGHT)
+            # noinspection PyArgumentList
+            ttk.Button(self, text='Save Changes', command=container.save_change, bootstyle=INFO).pack(**pack_def_options, side=tk.RIGHT)
 
     def on_key_press(self, event) -> None:
         """
         Event when a key is pressed
         :param event: the event that triggered the call of this function
         """
         if event.keysym == 'Escape':
@@ -93,14 +105,15 @@
         self.close_window()
 
     def close_window(self) -> None:
         """
         Close the window
         """
         gui_g.edit_cell_window_ref = None
+        self.editable_table.reset_style()
         self.destroy()
 
     def save_change(self) -> None:
         """
         Save the changes made in the window  (Wrapper)
         """
         self.must_save = False
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+# coding=utf-8
+"""
+Implementation for:
+- EditRowWindow: the window to edit a row
+"""
 import os
 import tkinter as tk
 from tkinter import ttk
 
+from ttkbootstrap.constants import *
+
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 
 
 class EditRowWindow(tk.Toplevel):
     """
     The window to edit a row
@@ -17,40 +24,40 @@
     :param screen_index: the index of the screen on which the window will be displayed
     :param editable_table: the table to edit
     """
 
     def __init__(self, parent, title: str, width: int = 600, height: int = 800, icon=None, screen_index: int = 0, editable_table=None):
         super().__init__(parent)
         self.title(title)
+        style = gui_f.set_custom_style(gui_g.s.theme_name, gui_g.s.theme_font)
+        self.style = style
         geometry = gui_f.center_window_on_screen(screen_index, height, width)
         self.geometry(geometry)
-
         if icon is None:
             self.attributes('-toolwindow', True)
         else:
             # windows only (remove the minimize/maximize buttons and the icon)
             icon = gui_f.path_from_relative_to_absolute(icon)
             if icon != '' and os.path.isfile(icon):
                 self.iconbitmap(icon)
-
         self.resizable(True, False)
 
         self.editable_table = editable_table
         self.must_save = False
         self.initial_values = []
         self.width = width
         # the photoimage is stored is the variable to avoid garbage collection
         # see: https://stackoverflow.com/questions/30210618/image-not-getting-displayed-on-tkinter-through-label-widget
         self.canvas_image = None
 
-        self.content_frame = self.ContentFrame(self)
         self.control_frame = self.ControlFrame(self)
+        self.content_frame = self.ContentFrame(self)
 
-        self.content_frame.pack(ipadx=5, ipady=5, padx=5, pady=5, fill=tk.X)
         self.control_frame.pack(ipadx=5, ipady=5, fill=tk.X)
+        self.content_frame.pack(ipadx=5, ipady=5, padx=5, pady=5, fill=tk.X)
 
         self.bind('<Key>', self.on_key_press)
         self.protocol("WM_DELETE_WINDOW", self.on_close)
 
         gui_g.edit_row_window_ref = self
 
     class ContentFrame(ttk.Frame):
@@ -66,15 +73,15 @@
         """
         The frame containing the buttons
         :param container: the parent window
         """
 
         def __init__(self, container):
             super().__init__(container)
-            pack_def_options = {'ipadx': 2, 'ipady': 2, 'fill': tk.X}
+            pack_def_options = {'ipadx': 2, 'ipady': 2, 'fill': tk.X, 'anchor': tk.NW}
             grid_def_options = {'ipadx': 5, 'ipady': 5, 'padx': 2, 'pady': 2, 'sticky': tk.NSEW}
 
             lblf_navigation = ttk.LabelFrame(self, text='Navigation')
             lblf_navigation.grid(row=0, column=0, **grid_def_options)
             btn_prev = ttk.Button(lblf_navigation, text='Prev Asset', command=container.prev_asset)
             btn_prev.pack(**pack_def_options, side=tk.LEFT)
             btn_next = ttk.Button(lblf_navigation, text='Next Asset', command=container.next_asset)
@@ -86,18 +93,20 @@
             canvas_image.pack()
             canvas_image.create_rectangle((0, 0), (gui_g.s.preview_max_width, gui_g.s.preview_max_height), fill='black')
 
             lblf_actions = ttk.LabelFrame(self, text='Actions')
             lblf_actions.grid(row=0, column=2, **grid_def_options)
             btn_open_url = ttk.Button(lblf_actions, text="Open URL", command=container.open_asset_url)
             btn_open_url.pack(**pack_def_options, side=tk.LEFT)
-            bnt_save = ttk.Button(lblf_actions, text='Save Changes', command=container.save_change)
-            bnt_save.pack(**pack_def_options, side=tk.LEFT)
-            btn_on_close = ttk.Button(lblf_actions, text='Cancel', command=container.on_close)
+            # noinspection PyArgumentList
+            btn_on_close = ttk.Button(lblf_actions, text='Close', command=container.on_close, bootstyle=WARNING)
             btn_on_close.pack(**pack_def_options, side=tk.RIGHT)
+            # noinspection PyArgumentList
+            bnt_save = ttk.Button(lblf_actions, text='Save Changes', command=container.save_change, bootstyle=INFO)
+            bnt_save.pack(**pack_def_options, side=tk.RIGHT)
 
             # Configure the columns to take all the available width
             self.columnconfigure(0, weight=1)
             self.columnconfigure(1, weight=2)
             self.columnconfigure(2, weight=1)
 
             self.canvas_image = canvas_image
@@ -126,14 +135,15 @@
             self.save_change()
 
     def close_window(self) -> None:
         """
         Close the window
         """
         gui_g.edit_row_window_ref = None
+        self.editable_table.reset_style()
         self.destroy()
 
     def save_change(self) -> None:
         """
         Save the changes (Wrapper)
         """
         self.must_save = False
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+# coding=utf-8
+"""
+Implementation for:
+- EditableTable is a custom class that extends the pandastable.Table class, providing additional functionality
+"""
 import webbrowser
 from tkinter import ttk
 
 import pandas as pd
 from pandastable import Table, TableModel
 
 from UEVaultManager.tkgui.modules.EditCellWindowClass import EditCellWindow
 from UEVaultManager.tkgui.modules.EditRowWindowClass import EditRowWindow
+from UEVaultManager.tkgui.modules.ExtendedWidgetClasses import ExtendedText
 from UEVaultManager.tkgui.modules.functions import *
 from UEVaultManager.tkgui.modules.TaggedLabelFrameClass import TaggedLabelFrame
 
 
 class EditableTable(Table):
     """
     EditableTable is a custom class that extends the pandastable.Table class, providing additional functionality
@@ -137,65 +143,70 @@
         self.show_page(self.total_pages - 1)
 
     def load_data(self) -> None:
         """
         Loads data from the specified CSV file into the table.
         """
         csv_options = {
-            'converters'  : {
-                'Asset_id'  : str,  #
-                'App name'  : str,  #
-                'Review'    : float,  #
-                'Price'     : float,  #
-                'Old Price' : float,  #
-                'On Sale'   : convert_to_bool,  #
-                'Purchased' : convert_to_bool,  #
-                'Must Buy'  : convert_to_bool,  #
+            'converters': {
+                'Asset_id': str,  #
+                'App name': str,  #
+                'Review': float,  #
+                'Price': float,  #
+                'Old Price': float,  #
+                'Purchased': convert_to_bool,  #
+                'Must Buy': convert_to_bool,  #
                 'Date Added': convert_to_datetime,  #
             },
             'on_bad_lines': 'warn',
-            'encoding'    : "utf-8",
+            'encoding': "utf-8",
         }
         if not os.path.isfile(self.file):
             log_warning(f'File not found: {self.file}')
             return
 
         self.data = pd.read_csv(self.file, **csv_options)
         # log_debug("\nCOL TYPES AFTER LOADING CSV\n")
         # self.data.info() # direct print info
 
         self.total_pages = (len(self.data) - 1) // self.rows_per_page + 1
 
         for col in self.data.columns:
             try:
                 self.data[col] = self.data[col].astype(str)
-            except ValueError as error:
+            except (KeyError, ValueError) as error:
                 log_error(f'Could not convert column "{col}" to string. Error: {error}')
 
-        col_to_datetime = ['Creation Date', 'Update Date']
+        col_to_convert = ['Creation Date', 'Update Date']
         # note "date added" does not use the same format as the other date columns
-        for col in col_to_datetime:
-            try:
-                self.data[col] = pd.to_datetime(self.data[col], format='ISO8601')
-            except ValueError as error:
-                log_error(f'Could not convert column "{col}" to datetime. Error: {error}')
-
-        col_as_float = ['Review', 'Price', 'Old Price']
-        for col in col_as_float:
-            try:
-                self.data[col] = self.data[col].astype(float)
-            except ValueError as error:
-                log_error(f'Could not convert column "{col}" to float. Error: {error}')
-
-        col_as_category = ['Category']
-        for col in col_as_category:
-            try:
-                self.data[col] = self.data[col].astype("category")
-            except ValueError as error:
-                log_error(f'Could not convert column "{col}" to category. Error: {error}')
+        for col in col_to_convert:
+            col_type = self.data.get(col, None)
+            if col_type is not None:
+                try:
+                    self.data[col] = pd.to_datetime(self.data[col], format='ISO8601')
+                except (KeyError, ValueError) as error:
+                    log_error(f'Could not convert column "{col}" to datetime. Error: {error}')
+
+        col_to_convert = ['Review', 'Price', 'Old Price', 'Discount Price']
+        for col in col_to_convert:
+            col_type = self.data.get(col, None)
+            if col_type is not None:
+                try:
+                    self.data[col] = self.data[col].astype(float)
+                except (KeyError, ValueError) as error:
+                    log_error(f'Could not convert column "{col}" to float. Error: {error}')
+
+        col_to_convert = ['Category', 'Grab result']
+        for col in col_to_convert:
+            col_type = self.data.get(col, None)
+            if col_type is not None:
+                try:
+                    self.data[col] = self.data[col].astype('category')
+                except (KeyError, ValueError) as error:
+                    log_error(f'Could not convert column "{col}" to category. Error: {error}')
 
         # log_debug("\nCOL TYPES AFTER MANUAL CONVERSION\n")
         # self.data.info() # direct print info
 
         self.data_filtered = self.data
 
     def reload_data(self) -> None:
@@ -228,27 +239,37 @@
 
         data = self.data.iloc[0:len(self.data)]
         self.updateModel(TableModel(data))  # needed to restore all the data and not only the current page
         self.model.df.to_csv(self.file, index=False, na_rep='N/A', date_format=gui_g.s.csv_datetime_format)
         self.show_page(self.current_page)
         self.must_save = False
 
-    def search(self, category=gui_g.s.default_category_for_all, search_text=gui_g.s.default_search_text) -> None:
+    def apply_filters(self, filter_dict=None, global_search=None) -> None:
         """
-        Searches the table data based on the provided category and search text.
-        :param category: The category to filter the table data by.
-        :param search_text: The text to search for in the table data.
-        """
-        if category and category != gui_g.s.default_category_for_all:
-            self.data_filtered = self.data[self.data['Category'] == category]
-        if search_text and search_text != gui_g.s.default_search_text:
-            self.data_filtered = self.data_filtered[self.data_filtered.apply(lambda row: search_text.lower() in str(row).lower(), axis=1)]
+        Searches the table data based on the provided filter dictionary.
+        :param filter_dict: A dictionary containing the column names as keys and filter values as the values.
+        :param global_search: The text to search for in the table data.
+        """
+        if filter_dict is None:
+            filter_dict = {}
+        log_info(f'Filtering data with: {filter_dict} and global search: {global_search}')
+        self.data_filtered = self.data
+
+        for key, value in filter_dict.items():
+            if key == 'Category' and value == gui_g.s.default_category_for_all:
+                continue
+            if key == 'Grab result' and value == gui_g.s.default_category_for_all:
+                continue
+            self.data_filtered = self.data_filtered[self.data_filtered[key].apply(lambda x: str(value).lower() in str(x).lower())]
+
+        if global_search and global_search != gui_g.s.default_global_search:
+            self.data_filtered = self.data_filtered[self.data_filtered.apply(lambda row: global_search.lower() in str(row).lower(), axis=1)]
         self.show_page(0)
 
-    def reset_search(self) -> None:
+    def reset_filters(self) -> None:
         """
         Resets the table data filtering and sorting, displaying all rows.
         """
         self.data_filtered = self.data
         self.show_page(0)
 
     def expand_columns(self) -> None:
@@ -263,15 +284,20 @@
         """
         self.contractColumns(factor=gui_g.s.contract_columns_factor)
 
     def autofit_columns(self) -> None:
         """
         Automatically resizes the columns to fit their content.
         """
-        self.autoResizeColumns()
+        # note:
+        # autoResizeColumns() will not resize table with more than 30 columns
+        # same limit without settings the limit in adjustColumnWidths()
+        # self.autoResizeColumns()
+        self.adjustColumnWidths(limit=len(self.data.columns))
+        self.redraw()
 
     def zoom_in(self) -> None:
         """
         Increases the font size of the table.
         """
         self.zoomIn()
 
@@ -303,17 +329,17 @@
         """
         Creates the edit row window for the selected row in the table.
         """
         row_selected = self.getSelectedRow()
         if row_selected is None:
             return
 
-        title = 'Edit current row values'
+        title = 'Edit current row'
         width = 900
-        height = 900
+        height = 1000
         # window is displayed at mouse position
         # x = self.master.winfo_rootx()
         # y = self.master.winfo_rooty()
         edit_row_window = EditRowWindow(
             parent=self.master, title=title, width=width, height=height, icon=gui_g.s.app_icon_filename, editable_table=self
         )
         edit_row_window.grab_set()
@@ -355,15 +381,15 @@
                 entry = ttk.Entry(inner_frame_url)
                 entry.insert(0, value)
                 entry.pack(side=tk.LEFT, fill=tk.X, expand=True)
                 button = ttk.Button(inner_frame_url, text="Open URL", command=self.open_asset_url)
                 button.pack(side=tk.RIGHT)
             elif lower_key in ('description', 'comment'):
                 # description and comment fields are text
-                entry = tk.Text(edit_row_window.content_frame, height=3)
+                entry = ExtendedText(edit_row_window.content_frame, height=3)
                 entry.insert('1.0', value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
             else:
                 # other field is just a usual entry
                 entry = ttk.Entry(edit_row_window.content_frame)
                 entry.insert(0, value)
                 entry.grid(row=i, column=1, sticky=tk.EW)
@@ -423,15 +449,15 @@
         col_index = self.get_col_clicked(event)
         if row_index is None or col_index is None:
             return None
         cell_value = self.model.df.iat[row_index, col_index]
 
         title = 'Edit current cell values'
         width = 300
-        height = 80
+        height = 90
         # window is displayed at mouse position
         # x = self.master.winfo_rootx()
         # y = self.master.winfo_rooty()
         edit_cell_window = EditCellWindow(parent=self.master, title=title, width=width, height=height, editable_table=self)
         edit_cell_window.grab_set()
         edit_cell_window.minsize(width, height)
 
@@ -570,7 +596,14 @@
             asset_url = self.edit_row_entries['Url'].get()
         else:
             asset_url = url
         log_info(f'calling open_asset_url={asset_url}')
         if asset_url is None or asset_url == '' or asset_url == 'nan':
             return
         webbrowser.open(asset_url)
+
+    def reset_style(self) -> None:
+        """
+        Resets the table style. Usefull when style of the main ttk window has changed.
+        """
+        self.data.style.clear()
+        self.redraw()
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+# coding=utf-8
+"""
+Implementation for:
+- GUISettings: class containing all the settings for the GUI
+"""
+
+
 class GUISettings:
     """
     This class contains all the settings for the GUI.
     """
 
-    # todo: integrate these settings into the UEVM config file
     def __init__(self):
         self.debug_mode = False
 
         self.app_title = 'UEVM Gui'
         self.app_width = 1600
         self.app_height = 930
         self.app_monitor = 1
@@ -20,13 +26,19 @@
         self.cache_folder = "../cache"
         self.cache_max_time = 60 * 60 * 24 * 15  # 15 days
 
         self.default_image_filename = './assets/UEVM_200x200.png'
         self.preview_max_width = 150
         self.preview_max_height = 150
 
-        self.default_search_text = 'Text to search...'
+        self.default_global_search = 'Text to search...'
         self.default_category_for_all = 'All'
 
         self.table_font_size = 10
         self.expand_columns_factor = 20
         self.contract_columns_factor = 20
+
+        # ttkbootstrap themes:
+        # light themes : "cosmo", "flatly", "litera", "minty", "lumen", "sandstone", "yeti", "pulse", "united", "morph", "journal", "simplex", "cerculean"
+        # dark themes: "darkly", "superhero", "solar", "cyborg", "vapor"
+        self.theme_name = 'lumen'
+        self.theme_font = ('Verdana', 8)
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+# coding=utf-8
+"""
+Implementation for:
+- ProgressWindow: window to display the progress of a function
+"""
 import os
 import queue
 import threading
 import tkinter as tk
 from tkinter import ttk
 
 import UEVaultManager.tkgui.modules.functions as gui_f  # using the shortest variable name for globals for convenience
 import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
 
 
 # noinspection PyProtectedMember
 class ProgressWindow(tk.Toplevel):
+    """
+    The window to display the progress of a function
+    :param title: the title
+    :param width: the width
+    :param height: the height
+    :param icon: the icon
+    :param screen_index: the index of the screen on which the window will be displayed
+    :param max_value: the maximum value of the progress bar
+    :param show_start_button: whether to show the start button
+    :param show_stop_button: whether to show the stop button
+    :param show_progress: whether to show the progress bar
+    :param function: the function to execute
+    :param function_parameters: the parameters of the function
+    :param quit_on_close: whether to quit the application when the window is closed
+    """
 
     def __init__(
         self,
         title: str,
         width: 300,
         height: 150,
         icon=None,
@@ -72,14 +92,18 @@
             self.start_execution()
 
     def __del__(self):
         gui_f.log_debug(f'Destruction of {self.__class__.__name__} object')
         gui_g.progress_window_ref = None
 
     class ContentFrame(ttk.Frame):
+        """
+        The frame that contains the content of the window
+        :param container: the container
+        """
 
         def __init__(self, container):
             super().__init__(container)
             pack_def_options = {'ipadx': 3, 'ipady': 3, 'padx': 5, 'pady': 5, 'fill': tk.X}
             if container.function is None:
                 lbl_function = ttk.Label(self, text='No callable function set Yet')
             else:
@@ -88,14 +112,20 @@
             progress_bar = ttk.Progressbar(self, orient="horizontal", mode="determinate", maximum=container.max_value)
             progress_bar.pack(**pack_def_options)
             self.pack_def_options = pack_def_options
             self.progress_bar = progress_bar
             self.lbl_function = lbl_function
 
     class ControlFrame(ttk.Frame):
+        """
+        The frame that contains the control buttons
+        :param container: the container
+        :param show_start_button: whether to show the start button
+        :param show_stop_button: whether to show the stop button
+        """
 
         def __init__(self, container, show_start_button=True, show_stop_button=True):
             super().__init__(container)
             pack_def_options = {'ipadx': 3, 'ipady': 3, 'fill': tk.X}
             self.pack_def_options = pack_def_options
             self.button_start = None
             self.button_stop = None
@@ -104,84 +134,138 @@
                 button_start.pack(**pack_def_options, side=tk.LEFT)
                 self.button_start = button_start
             if show_stop_button:
                 button_stop = ttk.Button(self, text="Stop", command=container.stop_execution, state=tk.DISABLED)
                 button_stop.pack(**pack_def_options, side=tk.RIGHT)
                 self.button_stop = button_stop
 
-    def _function_result_wrapper(self, function, *args, **kwargs):
+    def _function_result_wrapper(self, function, *args, **kwargs) -> None:
+        """
+        Wraps the function call and puts the result in the queue
+        :param function: the function to execute
+        :param args: args to pass to the function
+        :param kwargs: kwargs to pass to the function
+        """
         gui_f.log_info(f'execution of {function.__name__} has started')
         result = function(*args, **kwargs)
         gui_f.log_info(f'execution of {function.__name__} has ended')
         self.result_queue.put(result)
 
-    # check if the function is still running, if not, quit the window
-    def _check_for_end(self, t):
+    def _check_for_end(self, t: threading) -> None:
+        """
+        Checks if the thread has ended, if not, schedules another check
+        :param t: the thread to check
+        """
         if t.is_alive():
             # Schedule another check in a few ms
             self.after(self._thread_check_delay, self._check_for_end, t)
         else:
             # The thread has finished; clean up
             gui_f.log_debug(f'Quitting {self.__class__.__name__}')
             self.function_return_value = self.result_queue.get()
             self.close_window(destroy_window=self.quit_on_close)  # the window is kept to allow further calls to the progress bar
 
-    def set_text(self, new_text):
+    def set_text(self, new_text: str) -> None:
+        """
+        Sets the text of the label
+        :param new_text: the new text
+        """
         if self.content_frame is None or self.content_frame.lbl_function is None:
             return
         self.content_frame.lbl_function.config(text=new_text)
 
-    def set_value(self, new_value):
+    def set_value(self, new_value: int) -> None:
+        """
+        Sets the value of the progress bar
+        :param new_value: the new value
+        """
         new_value = max(0, new_value)
         if self.content_frame is None or self.content_frame.progress_bar is None:
             return
         self.content_frame.progress_bar["value"] = new_value
 
-    def set_max_value(self, new_max_value):
+    def set_max_value(self, new_max_value: int) -> None:
+        """
+        Sets the maximum value of the progress bar
+        :param new_max_value: the new maximum value
+        """
         if self.content_frame is None or self.content_frame.progress_bar is None:
             return
         self.max_value = new_max_value
         self.content_frame.progress_bar["maximum"] = new_max_value
 
-    def set_function(self, new_function):
+    def set_function(self, new_function) -> None:
+        """
+        Sets the function to execute
+        :param new_function: the new function
+        """
         if new_function is None:
             return
         self.set_text('Running function: ' + new_function.__name__)
         self.function = new_function
 
-    def set_function_parameters(self, parameters: dict):
+    def set_function_parameters(self, parameters: dict) -> None:
+        """
+        Sets the parameters to pass to the function
+        :param parameters: the parameters
+        """
         self.function_params = parameters
 
-    def hide_progress_bar(self):
+    def hide_progress_bar(self) -> None:
+        """
+        Hides the progress bar
+        """
         self.content_frame.progress_bar.pack_forget()
 
-    def show_progress_bar(self):
+    def show_progress_bar(self) -> None:
+        """
+        Shows the progress bar
+        """
         self.content_frame.progress_bar.pack(self.content_frame.pack_def_options)
 
-    def hide_start_button(self):
+    def hide_start_button(self) -> None:
+        """
+        Hides the start button
+        """
         if self.control_frame is None or self.control_frame.button_start is None:
             return
         self.control_frame.button_start.pack_forget()
 
-    def show_start_button(self):
+    def show_start_button(self) -> None:
+        """
+        Shows the start button
+        """
         if self.control_frame is None or self.control_frame.button_start is None:
             return
         self.control_frame.button_start.pack(self.control_frame.pack_def_options)
 
-    def hide_stop_button(self):
+    def hide_stop_button(self) -> None:
+        """
+        Hides the stop button
+        """
         if self.control_frame is None or self.control_frame.button_stop is None:
             return
         self.control_frame.button_stop.pack_forget()
 
-    def show_stop_button(self):
+    def show_stop_button(self) -> None:
+        """
+        Shows the stop button
+        """
         if self.control_frame is None or self.control_frame.button_stop is None:
             return
         self.control_frame.button_stop.pack(self.control_frame.pack_def_options)
 
-    def reset(self, new_title=None, new_value=None, new_text=None, new_max_value=None):
+    def reset(self, new_title=None, new_value=None, new_text=None, new_max_value=None) -> None:
+        """
+        Resets the progress bar
+        :param new_title: the new title
+        :param new_value: the new value
+        :param new_text: the new text
+        :param new_max_value: the new maximum value
+        """
         self.must_end = False
         try:
             # sometimes the window is already destroyed
             if new_title is not None:
                 self.title(new_title)
             if new_text is not None:
                 self.set_text(new_text)
@@ -192,49 +276,69 @@
                 self.show_progress_bar()
                 self.set_max_value(new_max_value)
         except tk.TclError:
             gui_f.log_warning('Some tkinter elements are not set. The window is probably already destroyed')
         self.continue_execution = True
 
     def start_execution(self) -> None:
+        """
+        Starts the execution of the function
+        """
         if self.function is None:
             gui_f.log_warning('the function name to execute is not set')
             return
         self.continue_execution = True
         self.deactivate()
         # Run the function in a separate thread
         t = threading.Thread(target=self._function_result_wrapper, args=(self.function, self), kwargs=self.function_params)
         t.start()
         # Schedule GUI update while waiting for the thread to finish
         self.after(self._thread_check_delay, self._check_for_end, t)
 
     def stop_execution(self) -> None:
+        """
+        Stops the execution of the function
+        """
         self.continue_execution = False
         self.activate()
 
     def get_result(self):
+        """
+        Returns the result of the function
+        """
         return self.function_return_value
 
     def activate(self) -> None:
+        """
+        Activates the control buttons for starting
+        """
         if self.control_frame is None:
             return
         if self.control_frame.button_start is not None:
             self.control_frame.button_start.config(state=tk.NORMAL)
         if self.control_frame.button_stop is not None:
             self.control_frame.button_stop.config(state=tk.DISABLED)
 
     def deactivate(self) -> None:
+        """
+        Activates the control buttons for stopping
+        """
         if self.control_frame is None:
             return
         if self.control_frame.button_start is not None:
             self.control_frame.button_stop.config(state=tk.NORMAL)
         if self.control_frame.button_stop is not None:
             self.control_frame.button_start.config(state=tk.DISABLED)
 
     def update_and_continue(self, value=0, increment=0) -> bool:
+        """
+        Updates the progress bar and returns whether the execution should continue
+        :param value: the value to set
+        :param increment: the value to increment. If both value and increment are set, the value is ignored
+        """
         try:
             # sometimes the window is already destroyed
             progress_bar = self.content_frame.progress_bar
             if increment:
                 value = progress_bar["value"] + increment
 
             if value > self.max_value:
@@ -242,14 +346,19 @@
             progress_bar["value"] = value
             progress_bar.update_idletasks()
         except tk.TclError:
             gui_f.log_warning('Some tkinter elements are not set. The window is probably already destroyed')
         self.update_idletasks()
         return self.continue_execution
 
-    def close_window(self, destroy_window=True, _event=None):
+    def close_window(self, destroy_window=True, _event=None) -> None:
+        """
+        Closes the window
+        :param destroy_window: whether to destroy the window or just hide it
+        :param _event: the event that triggered the close
+        """
         self.must_end = True
         if destroy_window:
             if self.quit_on_close:
                 self.quit()
             else:
                 self.destroy()
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# coding=utf-8
+"""
+Implementation for:
+- SaferDict: a dictionary subclass that provides a safer alternative to handle non-existing keys
+"""
+
+
 class SaferDict(dict):
     """
     A dictionary subclass that provides a safer alternative to handle non-existing keys.
     It returns None or the specified default value when accessing non-existing keys, rather than raising a KeyError.
     """
 
     def __getitem__(self, key):
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# coding=utf-8
+"""
+Implementation for:
+- TaggedLabelFrame: a custom LabelFrame widget that allows child widgets to be identified by tags
+"""
 import tkinter as tk
 from tkinter import ttk
 
 from UEVaultManager.tkgui.modules.ExtendedWidgetClasses import WidgetType, ExtendedEntry, ExtendedText, ExtendedLabel, ExtendedCheckButton
 from UEVaultManager.tkgui.modules.functions import log_error, tag_to_label
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+# coding=utf-8
+"""
+Implementation for:
+- WebImage: class to download an image from an url and get it as a PhotoImage
+"""
 from io import BytesIO
 
 import requests
 from PIL import ImageTk, Image
+
 from UEVaultManager.tkgui.modules.functions import log_warning
 
 
 class WebImage:
     """
     Class to download an image from an url and get it as a PhotoImage
     :param url: the url of the image to download
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+# coding=utf-8
+"""
+Utilities functions and tools
+"""
 import datetime
 import os
 import time
 import tkinter as tk
 from io import BytesIO
 from tkinter import messagebox
 
 import requests
+import ttkbootstrap as ttk
 from PIL import ImageTk, Image
 from screeninfo import get_monitors
 from termcolor import colored
 
-import UEVaultManager.tkgui.modules.globals as gui_g  # using the shortest variable name for globals for convenience
+from UEVaultManager.tkgui.modules import globals as gui_g
+from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
 
 
 def log_format_message(name: str, levelname: str, message: str) -> str:
     """
     Format the log message
     :param name: the name of the logger
     :param levelname: the level of log
@@ -195,30 +201,29 @@
     if screen_index > len(monitors):
         log_warning(f'The screen #{screen_index} is not available. Using 0 as screen index.')
         screen_index = 0
     # Position the window in the center of the screen
     target_screen = monitors[screen_index]
     screen_width = target_screen.width
     screen_height = target_screen.height
-    x = target_screen.x + (screen_width - width) // 2
-    y = target_screen.y + (screen_height - height) // 2
+    x = target_screen.x + (screen_width-width) // 2
+    y = target_screen.y + (screen_height-height) // 2
     geometry: str = f'{width}x{height}+{x}+{y}'
     return geometry
 
 
 def show_asset_image(image_url: str, canvas_image=None) -> None:
     """
     Show the image of the given asset in the given canvas
     :param image_url: the url of the image to display
     :param canvas_image: the canvas to display the image in
     """
-    if canvas_image is None or image_url == '':
+    if canvas_image is None or image_url == '' or str(image_url).lower() == 'nan':
         return
     try:
-
         # noinspection DuplicatedCode
         if not os.path.isdir(gui_g.s.cache_folder):
             os.mkdir(gui_g.s.cache_folder)
         image_filename = os.path.join(gui_g.s.cache_folder, os.path.basename(image_url))
         # Check if the image is already cached
         if os.path.isfile(image_filename) and (time.time() - os.path.getmtime(image_filename)) < gui_g.s.cache_max_time:
             # Load the image from the cache folder
@@ -226,15 +231,14 @@
         else:
             response = requests.get(image_url)
             image = Image.open(BytesIO(response.content))
 
             with open(image_filename, "wb") as f:
                 f.write(response.content)
         resize_and_show_image(image, canvas_image)
-
     except Exception as error:
         log_error(f"Error showing image: {error}")
 
 
 def show_default_image(canvas_image=None) -> None:
     """
     Show the default image in the given canvas
@@ -258,7 +262,84 @@
     :param tag: the tag to convert
     :return: the label
     """
     if tag is None:
         return ''
 
     return tag.capitalize().replace('_', ' ')
+
+
+def set_custom_style(theme_name='lumen', font=('Arial', 10, 'normal')):
+    """
+    Set the custom style for the application
+    :return: the style object
+    """
+    style = ttk.Style(theme_name)
+    # option possible for ttk widgets:
+    # TButton, TCheckbutton, TCombobox, TEntry, TFrame, TLabel, TLabelFrame, TMenubutton, TNotebook, TProgressbar, TRadiobutton,
+    # TScale, TScrollbar, TSeparator, TSizegrip, Treeview, TPanedwindow,
+    # Horizontal.TProgressbar or Vertical.TProgressbar (depending on the orient option),
+    # Horizontal.TScale or Vertical.TScale (depending on the orient option),
+    # Horizontal.TScrollbar or Vertical.TScrollbar (depending on the orient option)
+    style.configure('TLabel', font=font, spacing=1, padding=2)
+    style.configure('TButton', font=font, spacing=1, padding=2)
+    style.configure('TEntry', font=font, spacing=1, padding=2)
+    style.configure('TFrame', font=font, spacing=1, padding=1)
+    return style
+
+
+def json_print_key_val(json_obj, indent=4, print_result=True, output_on_gui=False) -> None:
+    """
+    Pretty prints a JSON object in a simple 'key: value' format.
+    :param json_obj:  The JSON object to print.
+    :param indent: The number of spaces to indent each level.
+    :param print_result: Determines whether to print the result.
+    :param output_on_gui: Determines whether to print the result on the GUI.
+    :return: The pretty printed JSON object.
+    """
+
+    def _process(obj, level=0):
+        lines = []
+        indent_str = ' ' * indent * level
+
+        if isinstance(obj, dict):
+            for key, value in obj.items():
+                if isinstance(value, (dict, list)):
+                    lines.append(f'{indent_str}{key}:')
+                    lines.extend(_process(value, level + 1))
+                else:
+                    lines.append(f'{indent_str}{key}: {value}')
+        elif isinstance(obj, list):
+            for item in obj:
+                lines.extend(_process(item, level))
+        else:
+            lines.append(f'{indent_str}{obj}')
+
+        return lines
+
+    result = '\n'.join(_process(json_obj))
+
+    if print_result:
+        if output_on_gui and gui_g.display_content_window_ref is not None:
+            gui_g.display_content_window_ref.display(result)
+        else:
+            print(result)
+
+
+def init_gui_args(args, additional_args=None) -> None:
+    """
+    Initialize the GUI arguments using the CLI arguments
+    :param args:
+    :param additional_args: dict of additional arguments to add
+    """
+
+    # args can not be used as it because it's an object that mainly run as a dict (but it's not)
+    # so we need to convert it to a dict first
+    temp_dict = vars(args)
+    temp_dict['csv'] = True  # force csv output
+    temp_dict['gui'] = True
+    if additional_args is not None:
+        temp_dict.update(additional_args)
+    # create a SaferDict object from the dict (it will avoid errors when trying to access non-existing keys)
+    gui_g.UEVM_cli_args = SaferDict({})
+    # copy the dict content to the SaferDict object
+    gui_g.UEVM_cli_args.copy_from(temp_dict)
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.3.0/UEVaultManager/tkgui/modules/globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,25 @@
+# coding=utf-8
+"""
+global variables and references to global objects
+"""
+# circular import error
+# import UEVaultManager.tkgui.modules.DisplayContentWindowClass as DisplayContentWindow
 import UEVaultManager.tkgui.modules.EditCellWindowClass as EditCellWindow
 import UEVaultManager.tkgui.modules.EditRowWindowClass as EditRowWindow
 from UEVaultManager.tkgui.modules.GUISettingsClass import GUISettings
 from UEVaultManager.tkgui.modules.ProgressWindowsClass import ProgressWindow
 from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
 
 # references to global objects
 edit_cell_window_ref: EditCellWindow = None
 edit_row_window_ref: EditRowWindow = None
+# circular import error
+# display_content_window_ref: DisplayContentWindow = None
+display_content_window_ref = None
 # noinspection PyTypeChecker
 progress_window_ref: ProgressWindow = None
 # reference to the cli object of the UEVM main app (the main one, it gives all access to all the features)
 # if empty, direct access to its features from this script won't be available and a message will be displayed instead
 # noinspection PyTypeChecker
 UEVM_cli_ref = None  # avoid importing classes from the UEVM main app here because it can cause circular dependencies when importing the module
 # noinspection PyTypeChecker
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.3.0/UEVaultManager/utils/aliasing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# coding=utf-8
+"""
+Application aliases for the Epic Games Store.
+"""
 from string import ascii_lowercase, digits
 
 # Aliases generated:
 # - name lowercase (without TM etc.)
 # - same, but without spaces
 # - same, but roman numerals are replaced
 # if name has >= 2 parts:
@@ -12,48 +16,48 @@
 # - run previous recursively with everything before ":"
 # if single 'f' in long word:
 # - split word (this is mainly for cases like Battlfront -> BF)
 # the first word longer than 1 character that isn't "the", "for", or "of" will also be added
 
 allowed_characters = ascii_lowercase + digits
 roman = {
-    'i'    : '1',
-    'ii'   : '2',
-    'iii'  : '3',
-    'iv'   : '4',
-    'v'    : '5',
-    'vi'   : '6',
-    'vii'  : '7',
-    'viii' : '8',
-    'ix'   : '9',
-    'x'    : '10',
-    'xi'   : '11',
-    'xii'  : '12',
-    'xiii' : '13',
-    'xiv'  : '14',
-    'xv'   : '15',
-    'xvi'  : '16',
-    'xvii' : '17',
+    'i': '1',
+    'ii': '2',
+    'iii': '3',
+    'iv': '4',
+    'v': '5',
+    'vi': '6',
+    'vii': '7',
+    'viii': '8',
+    'ix': '9',
+    'x': '10',
+    'xi': '11',
+    'xii': '12',
+    'xiii': '13',
+    'xiv': '14',
+    'xv': '15',
+    'xvi': '16',
+    'xvii': '17',
     'xviii': '18',
-    'xix'  : '19',
-    'xx'   : '20'
+    'xix': '19',
+    'xx': '20'
 }
 
 
 def _filter(local_input):
     return ''.join(char for char in local_input if char in allowed_characters)
 
 
 def generate_aliases(game_name, item_folder=None, split_words=True, app_name=None):
     # normalise and split name, then filter for legal characters
     game_parts = [_filter(p) for p in game_name.lower().split()]
     # filter out empty parts
     game_parts = [p for p in game_parts if p]
 
-    _aliases = [game_name.lower().strip(), ' '.join(game_parts), ''.join(game_parts), ''.join(roman.get(p, p) for p in game_parts), ]
+    _aliases = [game_name.lower().strip(), ' '.join(game_parts), ''.join(game_parts), ''.join(roman.get(p, p) for p in game_parts)]
 
     # single word abbreviation
     try:
         first_word = next(i for i in game_parts if i not in ('for', 'the', 'of'))
         if len(first_word) > 1:
             _aliases.append(first_word)
     except StopIteration:
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/utils/cli.py` & `UEVaultManager-1.3.0/UEVaultManager/utils/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# coding=utf-8
+"""
+CLI interface functions
+"""
 import os
 
 
 def get_boolean_choice(prompt, default=True):
     """
     Prompts the user with a yes/no question and returns a boolean value based on their choice.
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.3.0/UEVaultManager/utils/custom_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+# coding=utf-8
+"""
+Class definitions for:
+- HiddenAliasSubparsersAction: Subclass of argparse._SubParsersAction that hides aliases from the help output.
+"""
 import argparse
 
 
 # noinspection PyUnresolvedReferences,PyProtectedMember
 class HiddenAliasSubparsersAction(argparse._SubParsersAction):
+    """
+    Subclass of argparse._SubParsersAction that hides aliases from the help output.
+    """
+
     def add_parser(self, name, **kwargs):
         # set prog from the existing prefix
         if kwargs.get('prog') is None:
             kwargs['prog'] = f'{self._prog_prefix} {name}'
 
         aliases = kwargs.pop('aliases', ())
         hide_aliases = kwargs.pop('hide_aliases', False)
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.3.0/UEVaultManager/utils/egl_crypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# coding=utf-8
 """
 Stripped down version of https://github.com/boppreh/aes which is in turn based
 on https://github.com/bozhu/AES-Python with ECB decryption added.
 
 You should practically never roll your own crypto like this.
 In this case it's just unimportant enough since all it needs to do is decrypt some data from the EGL config file.
 """
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.3.0/UEVaultManager/utils/rolling_hash.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,36 @@
-# this is the rolling hash Epic uses, it appears to be a variation on CRC-64-ECMA
+# coding=utf-8
+"""
+The rolling hash Epic uses, it appears to be a variation on CRC-64-ECMA
+"""
 
 hash_poly = 0xC96C5795D7870F42
 hash_table = []
 
 
 def _init():
+    """
+    Initializes the hash table.
+    """
     for i in range(256):
         for _ in range(8):
             if i & 1:
                 i >>= 1
                 i ^= hash_poly
             else:
                 i >>= 1
         hash_table.append(i)
 
 
-def get_hash(data):
+def get_hash(data) -> int:
+    """
+    Calculates the rolling hash of a string.
+    :param data: The string to hash.
+    :return:
+    """
     if not hash_table:
         _init()
 
     h = 0
     for i in range(len(data)):
         h = ((h << 1 | h >> 63) ^ hash_table[data[i]]) & 0xffffffffffffffff
     return h
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.3.0/UEVaultManager/utils/webview_login.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# coding=utf-8
+"""
+Implementation for:
+- MockLauncher: a mock launcher to handle the webview login
+- do_webview_login() : launch the webview login
+"""
 import json
 import logging
 import os
 import webbrowser
 
 from UEVaultManager import __version__
 
@@ -20,15 +26,15 @@
 except Exception as error:
     logger.debug(f'Webview unavailable, disabling webview login. Try to run "pip install pywebview" (Exception: {error!r}).')
     webview_available = False
 
 login_url = 'https://www.epicgames.com/id/login'
 sid_url = 'https://www.epicgames.com/id/api/redirect?'
 logout_url = f'https://www.epicgames.com/id/logout?productName=epic-games&redirectUrl={login_url}'
-goodbye_url = 'https://legendary.gl/goodbye'
+goodbye_url = 'https://laurentongaro.github.io/UEVaultManager/statics/goodbye/index.html'
 window_js = '''
 window.ue = {
     signinprompt: {
         requestexchangecodesignin: pywebview.api.set_exchange_code,
         registersignincompletecallback: pywebview.api.trigger_sid_exchange
     },
     common: {
@@ -46,24 +52,32 @@
 sid_req.addEventListener("load", on_loaded);
 sid_req.open("GET", "/id/api/redirect?");
 sid_req.send();
 '''
 
 
 class MockLauncher:
+    """
+    Mock launcher to handle the webview login.
+    :param callback_sid: callback function to handle the SID login
+    :param callback_code: callback function to handle the exchange code
+    """
 
     def __init__(self, callback_sid, callback_code):
         self.callback_sid = callback_sid
         self.callback_code = callback_code
         self.window = None
         self.inject_js = True
         self.destroy_on_load = False
         self.callback_result = None
 
-    def on_loaded(self):
+    def on_loaded(self) -> None:
+        """
+        Callback function called when the login page is loaded.
+        """
         url = self.window.get_current_url()
         logger.debug(f'Loaded url: {url.partition("?")[0]}')
 
         if self.destroy_on_load:
             logger.info('Closing login window...')
             self.window.destroy()
             return
@@ -74,22 +88,35 @@
 
         if 'logout' in url and self.callback_sid:
             # prepare to close browser after logout redirect
             self.destroy_on_load = True
         elif 'logout' in url:
             self.inject_js = True
 
-    def nop(self, *args, **kwargs):
+    def nop(self, *args, **kwargs) -> None:
+        """
+        No operation function.
+        :param args: arguments
+        :param kwargs: keyword arguments
+        """
         return
 
     @staticmethod
-    def open_url_external(url):
+    def open_url_external(url: str) -> None:
+        """
+        Open the given url in the default browser.
+        :param url: url to open
+        """
         webbrowser.open(url)
 
-    def set_exchange_code(self, exchange_code):
+    def set_exchange_code(self, exchange_code: str) -> None:
+        """
+        Callback function called when the exchange code is received.
+        :param exchange_code: exchange code
+        """
         self.inject_js = False
         logger.debug('Got exchange code (stage 1)!')
         # The default Windows webview retains cookies, GTK/Qt do not. Therefore, we can
         # skip logging out on those platforms and directly use the exchange code we're given.
         # On Windows we have to do a little dance with the SID to create a session that
         # remains valid after logging out in the embedded browser.
         #  Update: Epic broke SID login, we'll also do this on Windows now
@@ -100,22 +127,29 @@
         except Exception as _error:
             logger.error(f'Logging in via exchange-code failed with {_error!r}')
         finally:
             # We cannot destroy the browser from here,
             # so we'll load a small goodbye site first.
             self.window.load_url(goodbye_url)
 
-    def trigger_sid_exchange(self):
+    def trigger_sid_exchange(self) -> None:
+        """
+        Trigger the SID exchange.
+        """
         # check if code-based login hasn't already set the destroying flag
         if not self.destroy_on_load:
             logger.debug('Injecting SID JS')
             # inject JS to get SID API response and call our API
             self.window.evaluate_js(get_sid_js)
 
-    def login_sid(self, sid_json):
+    def login_sid(self, sid_json: str) -> None:
+        """
+        Login with the given SID.
+        :param sid_json: SID json
+        """
         # Try SID login, then log out
         try:
             j = json.loads(sid_json)
             sid = j['sid']
             logger.debug(f'Got SID (stage 2)! Executing sid login callback...')
             exchange_code = self.callback_sid(sid)
             if exchange_code:
@@ -123,15 +157,20 @@
         except Exception as _error:
             logger.error(f'SID login failed with {_error!r}')
         finally:
             logger.debug('Starting browser logout...')
             self.window.load_url(logout_url)
 
 
-def do_webview_login(callback_sid=None, callback_code=None):
+def do_webview_login(callback_sid=None, callback_code=None) -> None:
+    """
+    Open a webview window to log in to Epic Games.
+    :param callback_sid: callback function to handle the SID login
+    :param callback_code: callback function to handle the exchange code
+    """
     api = MockLauncher(callback_sid=callback_sid, callback_code=callback_code)
     url = login_url
 
     if os.name == 'nt':
         # On Windows we open the logout URL first to invalidate the current cookies (if any).
         # Additionally, we have to disable JS injection for the first load, as otherwise the user
         # will get an error for some reason.
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.3.0/UEVaultManager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.1.1.7
+Version: 1.3.0
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: webview
 Provides-Extra: webview_gtk
 License-File: LICENSE
 
 Welcome to UEVaultManager
 ==========================================
+[![Logo](https://laurentongaro.github.io/UEVaultManager/statics/UEVM_200x200.png)
 
 | pypi                                                                                                                 | py_versions                                                                                                          | github                                                                                                                         | docs                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
 | [![Current PyPi Version](https://img.shields.io/pypi/v/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![py_versions](https://img.shields.io/pypi/pyversions/uevaultmanager)](https://pypi.python.org/pypi/uevaultmanager) | [![github](https://img.shields.io/github/v/tag/LaurentOngaro/uevaultmanager)](https://github.com/LaurentOngaro/UEVaultManager) | [![docs](https://img.shields.io/readthedocs/uevaultmanager/latest)](https://uevaultmanager.readthedocs.io/en/latest/?badge=latest) |
 
 **UEVaultManager** is an open-source assets manager that can list assets and
 their data from the Epic Games Marketplace. It is developed in Python, so
@@ -61,7 +62,10 @@
   * [Log files and debug](https://uevaultmanager.readthedocs.io/en/latest/output.html#log-files-and-debug)
   * [The output file](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-output-file)
   * [The individual json files](https://uevaultmanager.readthedocs.io/en/latest/output.html#the-individual-json-files)
   * [how to fix invalid search result during the grabbing process](https://uevaultmanager.readthedocs.io/en/latest/output.html#how-to-fix-invalid-search-result-during-the-grabbing-process)
   * [possible values in the error Field](https://uevaultmanager.readthedocs.io/en/latest/output.html#possible-values-in-the-error-field)
 
 [Next](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
+
+
+ UEVaultManager ## version:1.3.0 ## codename: Andromeda
```

### Comparing `UEVaultManager-1.1.1.7/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.3.0/UEVaultManager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,48 +8,50 @@
 UEVaultManager.egg-info/SOURCES.txt
 UEVaultManager.egg-info/dependency_links.txt
 UEVaultManager.egg-info/entry_points.txt
 UEVaultManager.egg-info/requires.txt
 UEVaultManager.egg-info/top_level.txt
 UEVaultManager/api/__init__.py
 UEVaultManager/api/egs.py
-UEVaultManager/api/lgd.py
+UEVaultManager/api/uevm.py
 UEVaultManager/assets/UEVM_200x200.png
 UEVaultManager/assets/main.ico
 UEVaultManager/downloader/__init__.py
 UEVaultManager/downloader/mp/__init__.py
 UEVaultManager/downloader/mp/manager.py
 UEVaultManager/downloader/mp/workers.py
 UEVaultManager/lfs/__init__.py
 UEVaultManager/lfs/egl.py
 UEVaultManager/lfs/eos.py
-UEVaultManager/lfs/lgndry.py
+UEVaultManager/lfs/uevmlfs.py
 UEVaultManager/lfs/utils.py
 UEVaultManager/lfs/windows_helpers.py
 UEVaultManager/models/__init__.py
 UEVaultManager/models/app.py
 UEVaultManager/models/chunk.py
 UEVaultManager/models/config.py
 UEVaultManager/models/downloading.py
 UEVaultManager/models/egl.py
 UEVaultManager/models/exceptions.py
 UEVaultManager/models/gql.py
 UEVaultManager/models/json_manifest.py
 UEVaultManager/models/manifest.py
 UEVaultManager/tkgui/__init__.py
 UEVaultManager/tkgui/main.py
+UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
 UEVaultManager/tkgui/modules/EditCellWindowClass.py
 UEVaultManager/tkgui/modules/EditRowWindowClass.py
 UEVaultManager/tkgui/modules/EditableTableClass.py
 UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
 UEVaultManager/tkgui/modules/GUISettingsClass.py
 UEVaultManager/tkgui/modules/ProgressWindowsClass.py
 UEVaultManager/tkgui/modules/SaferDictClass.py
 UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
 UEVaultManager/tkgui/modules/UEVMGuiClass.py
+UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
 UEVaultManager/tkgui/modules/WebImageClass.py
 UEVaultManager/tkgui/modules/__init__.py
 UEVaultManager/tkgui/modules/functions.py
 UEVaultManager/tkgui/modules/globals.py
 UEVaultManager/utils/__init__.py
 UEVaultManager/utils/aliasing.py
 UEVaultManager/utils/cli.py
```

### Comparing `UEVaultManager-1.1.1.7/setup.py` & `UEVaultManager-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# !/usr/bin/env python
 # coding: utf-8
 
 import sys
 from pathlib import Path
 
 import setuptools
 from setuptools import setup
 
-from UEVaultManager import __name__, __version__, __license__, __author__, __author_email__, __copyright__, __description__, __url__
+from UEVaultManager import __name__, __version__, __codename__, __license__, __author__, __author_email__, __copyright__, __description__, __url__
 
 if sys.version_info < (3, 9):
     sys.exit('python 3.9 or higher is required for UEVaultManager')
 
 this_directory = Path(__file__).parent
 __long_description__ = Path.joinpath(this_directory, 'README.md').read_text()
+# add information about the version and codename in the PyPI page because codename s not available by default
+__long_description__ += f'\n\n {__name__} ## version:{__version__} ## codename: {__codename__}'
 # __long_description__ = ''.join(__long_description__[8:16])  # keep only description text
 
 setup(
     name=__name__,
     version=__version__,
     license=__license__,
     author=__author__,
```

