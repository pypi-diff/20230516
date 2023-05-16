# Comparing `tmp/wmwpy-0.1.1b0.tar.gz` & `tmp/wmwpy-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmwpy-0.1.1b0.tar", last modified: Tue Apr 25 17:18:19 2023, max compression
+gzip compressed data, was "wmwpy-0.2.0b0.tar", last modified: Tue May 16 03:17:25 2023, max compression
```

## Comparing `wmwpy-0.1.1b0.tar` & `wmwpy-0.2.0b0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.334036 wmwpy-0.1.1b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.334036 wmwpy-0.1.1b0/src/wmwpy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/Font/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Font/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/Utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Images.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/XMLTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/textures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/Utils/waltex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.338037 wmwpy-0.1.1b0/src/wmwpy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/Widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    22212 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/imagelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/sprite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.342037 wmwpy-0.1.1b0/src/wmwpy/classes/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_CANVAS.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_GROUP.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_LABEL.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_SLIDER.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/WT_TOGGLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/classes/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/gameobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-04-25 17:18:06.000000 wmwpy-0.1.1b0/src/wmwpy/gametemplate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:18:19.334036 wmwpy-0.1.1b0/src/wmwpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41984 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 17:18:19.000000 wmwpy-0.1.1b0/src/wmwpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.113730 wmwpy-0.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-16 03:17:25.113730 wmwpy-0.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 03:17:25.113730 wmwpy-0.2.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/wmwpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/wmwpy/Font/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Font/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/Utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/XMLTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/textures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/Utils/waltex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/Widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22504 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/imagelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/sprite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.109730 wmwpy-0.2.0b0/src/wmwpy/classes/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_CANVAS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_FINGER_CATCHER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_GROUP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_ICON_LIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_LABEL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_PROGRESS_BAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_PUSH_BUTTON.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_CAMERA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_SCROLLABLE_SET.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_SLIDER.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/WT_TOGGLE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/classes/widget/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/gameobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-16 03:17:12.000000 wmwpy-0.2.0b0/src/wmwpy/gametemplate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:17:25.105730 wmwpy-0.2.0b0/src/wmwpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42049 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 03:17:25.000000 wmwpy-0.2.0b0/src/wmwpy.egg-info/top_level.txt
```

### Comparing `wmwpy-0.1.1b0/LICENSE` & `wmwpy-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/PKG-INFO` & `wmwpy-0.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.1.1b0
+Version: 0.2.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,14 +676,15 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/wmw-modding/wmwpy
 Project-URL: Bug Tracker, https://github.com/wmw-modding/wmwpy/issues
+Project-URL: Documentation, https://wmw-modding.github.io/wmwpy/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wmwpy-0.1.1b0/README.md` & `wmwpy-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/pyproject.toml` & `wmwpy-0.2.0b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -25,10 +25,11 @@
   "filetype",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/wmw-modding/wmwpy"
 "Bug Tracker" = "https://github.com/wmw-modding/wmwpy/issues"
+"Documentation" = "https://wmw-modding.github.io/wmwpy/"
 
 [tool.setuptools.dynamic]
 version = { attr = "wmwpy.__version__" }
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/Game.py` & `wmwpy-0.2.0b0/src/wmwpy/game.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import typing
 
-from .Utils import Filesystem
+from .Utils.filesystem import *
 from .Utils import Texture
 from .classes import *
 
 class Game():
     _DB = '/Data/water.db'
     _BASEASSETS = '/'
     _PROFILE = None
@@ -54,33 +54,43 @@
         """
         Load level
 
         Args:
             xmlPath (str, optional): Path to xml file. Defaults to None.
             imagePath (str, optional): Path to image file. Defaults to None.
         """
-        split = os.path.splitext(xmlPath)
-        if split[1] == '':
-            imagePath = '.'.join([split[0], 'png'])
-            xmlPath = '.'.join([split[0], 'xml'])
-        
-        xml = None
-        if xmlPath:
-            xml = this.filesystem.get(xmlPath)
-        
-        image = None
-        if imagePath:
-            image = this.filesystem.get(imagePath)
+        if isinstance(xmlPath, File):
+            xml = xmlPath
+        else:
+            xml = None
+            if xmlPath:
+                split = os.path.splitext(xmlPath)
+                if split[1] == '':
+                    if imagePath in ['', None]:
+                        imagePath = '.'.join([split[0], 'png'])
+                    xmlPath = '.'.join([split[0], 'xml'])
+                
+                xml = this.filesystem.get(xmlPath)
+        
+        if isinstance(imagePath, File):
+            image = imagePath
+        else:
+            image = None
+            if imagePath:
+                image = this.filesystem.get(imagePath)
         
         level = Level(
             xml=xml,
             image=image,
             filesystem=this.filesystem,
         )
-        level.filename = xmlPath
+        if isinstance(xmlPath, File):
+            level.filename = xmlPath.path
+        else:
+            level.filename = xmlPath
         
         return level
     
     def Object(
         this,
         object : str,
         **kwargs
@@ -91,16 +101,20 @@
         Args:
             object (str): Path to `.hs` object file.
 
         Returns:
             classes.object.Object: Where's My Water? object.
         """
         
+        
+        if not isinstance(object, File):
+            object = this.filesystem.get(object)
+        
         obj = Object(
-            this.filesystem.get(object),
+            object,
             filesystem = this.filesystem,
             **kwargs
         )
         obj.filename = object
         return obj
     
     def Imagelist(
@@ -115,16 +129,19 @@
             imagelist (str): Path to `.imagelist` file. Defaults to None
             HD (bool, optional): Whether to use HD textures. Defaults to False.
 
         Returns:
             classes.imagelist.Imagelist: Imagelist object.
         """
         
+        if not isinstance(imagelist, File):
+            imagelist = this.filesystem.get(imagelist)
+        
         imagelistObject = Imagelist(
-            this.filesystem.get(imagelist),
+            imagelist,
             filesystem = this.filesystem,
             HD = False,
         )
         imagelistObject.filename = imagelist
         return imagelistObject
     
     def Sprite(
@@ -138,16 +155,19 @@
         Args:
             sprite (str): Path to `.sprite` file.`
 
         Returns:
             classes.sprite.Sprite: Sprite object.
         """
         
+        if not isinstance(sprite, File):
+            sprite = this.filesystem.get(sprite)
+        
         spriteObject = Sprite(
-            this.filesystem.get(sprite),
+            sprite,
             filesystem = this.filesystem,
             **kwargs
         )
         spriteObject.filename = sprite
         return spriteObject
     
     def Texture(
@@ -160,16 +180,19 @@
         Args:
             texture (str): Path to image file.
 
         Returns:
             Utils.textures.Texture: Texture object.
         """
         
+        if not isinstance(texture, File):
+            texture = this.filesystem.get(texture)
+        
         return Texture(
-            this.filesystem.get(texture)
+            texture
         )
     
     def Layout(this, layout : str):
         raise NotImplementedError('load layout is not implemented yet.')
     
     def generateFileManifest(this, writeFile : bool = True, filename : str = '/FileManifest.txt'):
         """Generate the `FileManifest.txt` file needed for some games, such as WMM. This just generates a text file with the paths to every file in the `assets` folder (which includes the `FileManifest.txt` file).
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Documents.py` & `wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Documents.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/Utils/Types/Images.py` & `wmwpy-0.2.0b0/src/wmwpy/Utils/Types/Images.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/Utils/filesystem.py` & `wmwpy-0.2.0b0/src/wmwpy/Utils/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,19 @@
         #     # print('file-like')
         # else:
         #     raise TypeError(f"file can only 'str', 'bytes', or file-like object.")
         
         return this.root.add(path = path, content = file, replace = replace)
     
     def remove(this, path : str):
+        """Remove a file or folder
+
+        Args:
+            path (str): Path to file or folder to remove.
+        """
         return this.root.remove(path)
     
     def getAssets(
         this,
         extract_zip = False,
         split_imagelist = False,
         hook : typing.Callable[[int, str, int], typing.Any] = None
@@ -112,16 +117,16 @@
                 if file.is_dir():
                     count += dirlength(file.path)
                 else:
                     count += 1
             return count
 
         
-        print(this.gamepath)
-        print(f'{this.gamepath = }\n{this.assets = }')
+        # print(this.gamepath)
+        # print(f'{this.gamepath = }\n{this.assets = }')
         
         assets = pathlib.Path(joinPath(this.gamepath, this.assets))
         
         if not assets.exists():
             raise FileNotFoundError(f'Folder {assets} does not exist')
         
         total = dirlength(assets.resolve().as_posix())
@@ -163,34 +168,39 @@
 
         Returns:
             list: List of files and subfolders.
         """
         return this.get(path).listdir(recursive = recursive)
     
     def dump(this, output : str = None):
+        """Dump the contents of the filesystem to the specified directory
+
+        Args:
+            output (str, optional): Path to output directory. Defaults to original path.
+        """
         if output == None:
             output = joinPath(this.gamepath, this.assets)
         
-        print(f'output: {output}')
+        # print(f'output: {output}')
         
         files = this.listdir(recursive=True)
         for path in files:
             file = this.get(path)
             if file.is_dir():
                 continue
             parts = pathlib.Path(path).parts
             
             if parts[0] in ['/', '\\', '']:
                 parts = parts[1::]
             
-            print(f'new: {parts}')
+            # print(f'new: {parts}')
             
             newpath = pathlib.Path(output, *parts)
             
-            print(f'writing: {newpath.as_posix()}')
+            # print(f'writing: {newpath.as_posix()}')
             
             newpath.parent.mkdir(exist_ok=True)
             
             data = file.rawdata.getvalue()
             
             with open(newpath, 'wb') as f:
                 f.write(data)
@@ -244,33 +254,53 @@
         """Detatch this file or folder from it's parent.
         """
         if self.parent == None:
             return
         self.parent.files.remove(self)
         self.parent = None
     
-    def is_dir(this):
+    def is_dir(this) -> bool:
+        """Check whether this is a folder.
+
+        Returns:
+            bool
+        """
         return this._type.value == this._Type.FOLDER
         
     @property
-    def path(this):
+    def path(this) -> str:
+        """Path to this file or folder from the root.
+
+        Returns:
+            str: Path this file or folder.
+        """
         if this.parent == None or isinstance(this.parent, Filesystem):
             if isinstance(this, File) and not isinstance(this.parent, Filesystem):
                 return this.name
             return '/'
         return pathlib.Path(this.parent.path, this.name).as_posix()
     
     @property
-    def root(this):
+    def root(this) -> 'Folder':
+        """Root Folder for this File or Folder.
+
+        Returns:
+            Folder: Root Folder for this File or Folder
+        """
         if this.parent == None or this.name == '':
             return this
         return this.parent.root
     
     @property
-    def filesystem(this):
+    def filesystem(this) -> Filesystem:
+        """Returns the Filesystem or root Folder for this File or Folder.
+
+        Returns:
+            Filesystem | Folder: Root Filesystem or Folder
+        """
         if isinstance(this.parent, Filesystem):
             return this.parent
         if this.parent == None or this.name == '':
             return this
         return this.parent.filesystem
         
     class _Type():
@@ -295,41 +325,52 @@
             path (str): File path.
             content (bytes): Contents of file as bytes.
         """
         super().__init__(parent, path)
         this._type.value = this._Type.FILE
         
         this._datatype = 'raw'
+        this._original_filename = ''
         
         if isinstance(data, bytes):
             this._rawcontent = data
         elif isinstance(data, str):
             if os.path.exists(data):
                 this._rawcontent = data
                 this._datatype = 'path'
+                this._original_filename = data
             else:
                 this._rawcontent = data.encode()
         elif isinstance(data, io.BytesIO):
             this._rawcontent = data.getvalue()
         elif isinstance(data, File):
             this._rawcontent = data._rawcontent
             this._datatype = data._datatype
+            this._original_filename = data._original_filename
         elif hasattr(data, 'read'):
+            data.seek(0)
+            if hasattr(data, 'name'):
+                this._original_filename = data.name
+            
+            data.seek(0)
+            
             this._rawcontent = data.read()
             if isinstance(this._rawcontent, str):
                 this._rawcontent = this._rawcontent.encode()
         else:
             this._rawcontent = bytes(data)
         
         this.content = None
         
         if this._datatype == 'raw':
             this._getdata()
         
     def _getdata(this):
+        """Get data from file path
+        """
         if this._datatype == 'path':
             with open(this._rawcontent, 'rb') as file:
                 this._rawcontent = file.read()
             this._datatype = 'raw'
         
         this.rawdata = io.BytesIO(this._rawcontent)
         # seek back to the start to be able to read the data later.
@@ -353,24 +394,34 @@
             this.mime = this.type.mime
             this.extension = this.type.extension
             
         return this.mime
     
     @property
     def rawdata(this) -> io.BytesIO:
+        """Returns the raw data of the file as a `BytesIO` object.
+
+        Returns:
+            io.BytesIO: Raw data of file.
+        """
         if this._datatype == 'path':
             this._getdata()
         
         return this._rawdata
     @rawdata.setter
     def rawdata(this, value : io.BytesIO):
         this._rawdata : io.BytesIO = value
     
     @property
-    def extension(this):
+    def extension(this) -> str:
+        """The file extension
+
+        Returns:
+            str: File extension
+        """
         if this._datatype == 'path':
             return os.path.splitext(this._rawcontent)[1::]
         else:
             this._extension
     @extension.setter
     def extension(this, value):
         this._extension = value
@@ -386,15 +437,15 @@
             this._getdata()
         
         this.rawdata.seek(0)
         
         reader = Reader()
         
         for r in FILE_READERS:
-            print(r)
+            # print(r)
             if r.check(this.mime, this.extension, this.rawdata, filesystem = this.filesystem, **kwargs):
                 reader = r
                 break
         
         this.content = reader.read(this.mime, this.extension, this.rawdata, **kwargs)
         
         # if this.mime == 'image/waltex':
@@ -530,15 +581,15 @@
                 raise NotADirectoryError(f"{file.path} is not a directory.")
             
             return file.add(pathlib.Path(*parts[1::]).as_posix(), content, replace=replace)
         else:
             if file != None:
                 if  not replace:
                     raise FileExistsError(f'File {file.path} already exists.')
-                print(f'File {file.path} already exists. Now replacing it.')
+                # print(f'File {file.path} already exists. Now replacing it.')
                 this.files.remove(file)
             
             file = File(this, parts[0], data = content)
             this.files.append(file)
             
             return file
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/Utils/textures.py` & `wmwpy-0.2.0b0/src/wmwpy/Utils/textures.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,14 +77,27 @@
                 _cachedWaltextImages[path] = image.copy()
     else:
         image = Image.open(path).convert('RGBA')
         
     return image
     
 def getTextueSettings(gamepath : str, assets : str, textureSettings : str, name : str, ) -> dict:
+    """Get the texture settings of a texture.
+    
+    Really needs an update, as now I can reliably get the path to the file using the `baseassets` property in the `Game` object.
+
+    Args:
+        gamepath (str): Path to game
+        assets (str): Relative path from the gamepath to the assets folder.
+        textureSettings (str): Path to `TextureSettings.xml` file
+        name (str): Name of image to look for.
+
+    Returns:
+        dict: The texture settings as a dict.
+    """
     fullpath = joinPath(gamepath, assets, textureSettings)
     xml = etree.parse(fullpath).getroot()
     
     Texture = etree.ElementBase()
     for i in xml:
         if not i.tag is etree.Comment:
             if i.tag == 'Texture' and i.get('name') == name:
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/Utils/waltex.py` & `wmwpy-0.2.0b0/src/wmwpy/Utils/waltex.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     import filetype
 
     class _WaltexFile(filetype.Type):
         MIME = 'image/waltex'
         EXTENSION = 'waltex'
 
         def __init__(self):
+            """Waltex file extension class for the `filetype` module
+            """
             super(_WaltexFile, self).__init__(
                 mime=_WaltexFile.MIME,
                 extension=_WaltexFile.EXTENSION,
             )
 
         def match(self, buf):
             return (len(buf) > 3 and
@@ -142,15 +144,23 @@
         this._byte_order = byte_order
         
         this.file = file
         this.rawdata = io.BytesIO(rawdata)
         
         this.read(byte_order=this._byte_order)
     
-    def read(this, byte_order : str = None):
+    def read(this, byte_order : str = None) -> Image.Image:
+        """Read the waltex image.
+
+        Args:
+            byte_order (str, optional): The byte order. Can be 'little' or 'big'. Defaults to None.
+
+        Returns:
+            PIL.Image.Image: PIL Image object
+        """
         if byte_order:
             this._byte_order = byte_order
             
         header = this.rawdata.getvalue()[0:16]
             
         this.format = int(header[5])
         this.colorspec = this._colorspecs[this.format]
@@ -168,14 +178,19 @@
         
         this.image.format = _WaltexImageFile.format
         this.image.format_description = _WaltexImageFile.format_description
         return this.image
     
     @property
     def size(this):
+        """Return size of image
+
+        Returns:
+            tuple[int,int]: tuple(width, height)
+        """
         return this.image.size
 
 # legacy functions for reading waltex image
 def WaltexImage(path : str | bytes | io.BytesIO, premultiplyAlpha : bool = False, dePremultiplyAlpha : bool = False, endian : str = 'little') -> Image.Image:
     """
     ### Depracted
     Use `Image.load()` instead.
@@ -213,15 +228,15 @@
         rawdata = path
     elif hasattr(path, 'read'):
         rawdata = path.read()
     else:
         raise TypeError(f"file has to be a 'str', 'bytes' or file-like object.")
     
         
-    print(filetype.guess(rawdata))
+    # print(filetype.guess(rawdata))
         
     if filetype.guess(rawdata).MIME != 'image/waltex':
         raise TypeError('File is not a waltex')
     version = int(rawdata[4])
     format = int(rawdata[5])
     w = int.from_bytes(rawdata[6:8], byteorder='little')
     h = int.from_bytes(rawdata[8:10], byteorder='little')
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/__init__.py` & `wmwpy-0.2.0b0/src/wmwpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-__version__ = "0.1.1-beta"
+__version__ = "0.2.0-beta"
 __author__ = 'ego-lay-atman-bay'
 
 import typing
 
-from .Game import Game
+from .game import Game
 from . import classes
 from . import Font
 from .classes import widget
 from . import Utils
 from .gametemplate import GAMES
+from .Utils import filesystem
 
 def load(
     gamepath : str,
     platform : typing.Literal['android', 'ios'] = 'android',
     game : str = 'WMW',
     assets : str = None,
     db : str = None,
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/Widgets.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/Widgets.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/curves.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/curves.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/imagelist.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/imagelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,16 @@
             else:
                 file = this.filesystem.add(path, output)
         
         
         return output
     
     def combinePages(this):
+        """Combine all the pages in this Imagelist into 1 Page
+        """
         if this.type == this.Type.IMAGELIST:
             return
         
         main = this.pages[0]
         for i in range(len(this.pages) - 1):
             page : this.Page = this.pages[i + 1]
             for name in page.images:
@@ -345,15 +347,20 @@
                     this.name,
                     file = this.rawdata.getvalue(),
                     replace = replace
                 )
             
             
             @property
-            def filename(this):
+            def filename(this) -> str:
+                """Image filepath in the Filesystem
+
+                Returns:
+                    str: Full filepath in the Filesystem
+                """
                 return this.filesystem.get(this.name).path
 
         
         def read(this):
             """Read xml.
             """
             this.properties = deepcopy(this.xml.attrib)
@@ -371,15 +378,15 @@
                 if this.filesystem.exists(hd):
                     this.file = hd
     
             this.fullAtlasPath = ''
     
             if this.gamepath:
                 this.fullAtlasPath = joinPath(this.gamepath, this.assets, this.file)
-                print(this.fullAtlasPath)
+                # print(this.fullAtlasPath)
     
             this.getAtlas()
             this.getImages()
     
         def getAtlas(this):
             """Get atlas image.
             """
@@ -452,15 +459,15 @@
                 properties (dict, optional): Additional properties for image. Defaults to {}.
                 replace (bool, optional): Whether to replace existing image if there is a conflict. Defaults to False.
 
             Raises:
                 NameError: Image already exists.
             """
             if name in this.images:
-                print(f'Warning: "{name}" already in imagelist.')
+                # print(f'Warning: "{name}" already in imagelist.')
                 if not replace:
                     raise NameError(f'Image "{name}" already exists.')
             properties['name'] = name
             properties['rect'] = ' '.join([str(_) for _ in (0,0) + image.size])
             
             texture = this.Image(
                 image,
@@ -501,15 +508,15 @@
         
         def updateProperties(this):
             """Updates all the properties dict.
             """
             this.properties['textureBasePath'] = this.textureBasePath
             this.properties['imgSize'] = ' '.join([str(n) for n in this.size])
             this.properties['file'] = this.file
-            print(this.properties['file'])
+            # print(this.properties['file'])
             if this.id == None:
                 if 'id' in this.properties:
                    del this.properties['id']
             else:
                 this.properties['id'] = str(this.id)
                 
         
@@ -593,14 +600,16 @@
                 image.atlas = atlas
                 atlas.paste(image.image, image.rect[0:2])
             
             this.atlas = atlas
             return this.atlas
     
         def getNO_TEX(this):
+            """## NEED TO UPDATE
+            """
             NO_TEX_settings = getTextueSettings(
                 this.gamepath,
                 this.assets,
                 joinPath(os.path.dirname(os.path.dirname(this.textureBasePath)), 'Data/textureSettings.xml'),
                 os.path.join(this.textureBasePath, 'NO_TEX.png')
             )
             NO_TEX_image = PIL.Image.open(joinPath(this.gamepath, this.assets, this.textureBasePath, 'NO_TEX.png')).convert('RGBA')
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/layout.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/layout.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/level.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/level.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 from lxml import etree
-from PIL import Image
+from PIL import Image, ImageTk
+import numpy
 
 from ..Utils.filesystem import *
 from .object import Object
 from ..gameobject import GameObject
 
 class Level(GameObject):
     XML_TEMPLATE = b"""<?xml version="1.0"?>
@@ -54,21 +55,76 @@
             this.image = Image.open(this.image_file).quantize(colors=256)
         
         this.objects = []
         this.properties = {}
         this.room = (0,0)
         
         this.read()
+        
+        this.scale = 5
+    
+    @property
+    def size(this) -> tuple[int,int]:
+        """Level image size
+
+        Returns:
+            tuple[int,int]: (width,height)
+        """
+        return this._image.size
+    
+    @property
+    def image(this) -> Image.Image:
+        """Scaled up Level image
+
+        Returns:
+            PIL.Image.Image: PIL Image
+        """
+        image = this._image.copy()
+        
+        size = numpy.array(image.size)
+        size = size * this.scale
+        
+        image = image.resize(size, resample = Image.NEAREST)
+        
+        return image
+        
+    @image.setter
+    def image(this, value : Image.Image):
+        this._image = value
+    
+    @property
+    def PhotoImage(this) -> ImageTk.PhotoImage:
+        """Tkinter PhotoImage of the Level image
+
+        Returns:
+            ImageTk.PhotoImage: Tkinter PhotoImage
+        """
+        this._PhotoImage = ImageTk.PhotoImage(this.image)
+        return this._PhotoImage
+
+    @property
+    def scale(this) -> int:
+        """Level size scale
+        """
+        return this._scale
+    @scale.setter
+    def scale(this, value : int):
+        this._scale = value
+        
+        for obj in this.objects:
+            obj.scale = this._scale
     
     def read(this):
         """Read level XML
         """
         this.objects : list[Object] = []
         this.properties = {}
         
+        id = 0
+        
         for element in this.xml:
             # comment safe-guard
             if element is etree.Comment:
                 continue
             
             if element.tag == 'Object':
                 properties = {}
@@ -89,15 +145,19 @@
                     this.filesystem.get(properties['Filename']), # get file because `Object` does not take filepath
                     filesystem = this.filesystem,
                     properties = properties,
                     pos = pos,
                     name = name,
                 )
                 
+                obj.id = id
+                
                 this.objects.append(obj)
+                
+                id += 1
             
             if element.tag == 'Properties':
                 for el in element:
                     if el is etree.Comment:
                         continue
                     
                     if el.tag == 'Property':
@@ -183,39 +243,59 @@
             name (str, optional): Name of object. May get renamed if object with name alread exists. Defaults to 'Obj'.
 
         Returns:
             Object: wmwpy Object.
         """
         if not isinstance(filename, Object):
             filename = Object(
-                this.filesystem.get(filename),
+                filename,
                 filesystem = this.filesystem,
                 properties = properties,
                 pos = pos,
                 name = name,
             )
         else:
             filename.name = name
             filename.pos = pos
             filename.setProperty(properties)
         
         obj = filename
         
+        id = 0
+        while this.getObjectById(id) != None:
+            id += 1
+        
         if this.getObject(obj.name) != None:
             objnum = 0
             name = obj.name
             
             while this.getObject(obj.name) != None:
                 objnum += 1
                 obj.name = f'{name}{str(objnum)}'
         
+        obj.id = id
         this.objects.append(obj)
+        obj.scale = this.scale
         
         return obj
     
+    def getObjectById(this, id : int) -> Object:
+        """Get an Object by it's id
+
+        Args:
+            id (int): Object id to find
+
+        Returns:
+            Object: wmwpy Object
+        """
+        for obj in this.objects:
+            if obj.id == id:
+                return obj
+        return None
+    
     def getObject(this, name : str):
         """
         Get object by name
 
         Args:
             name (str): Object name.
         """
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/object.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/sprite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,417 +1,503 @@
-import lxml
 from lxml import etree
-import io
-from copy import deepcopy
 from PIL import Image, ImageTk
 import numpy
+from copy import deepcopy
 import math
 
-from ..gameobject import GameObject
-from .sprite import Sprite
+from .imagelist import Imagelist
 from ..Utils.filesystem import *
-
 from ..Utils.XMLTools import strbool
-class Object(GameObject):
+from ..gameobject import GameObject
+
+class Sprite(GameObject):
     def __init__(
         this,
         file : str | bytes | File,
-        filesystem : Filesystem | Folder = None,
-        gamepath : str = None,
-        assets : str = '/assets',
+        filesystem: Filesystem | Folder = None,
+        gamepath: str = None, assets: str = '/assets',
         baseassets : str = '/',
         properties : dict = {},
-        pos : tuple | str = (0,0),
-        name : str = 'Obj',
         scale : int = 10,
     ) -> None:
-        """Get game object. Game object is `.hs` file.
+        """Game sprite.
 
         Args:
-            file (str | bytes | File): Object file.
+            this (_type_): _description_
+            file (str | bytes | File): Sprite file.
             filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
             gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
             assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
             baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
-            properties (dict, optional): Object properties that override default properties. Defaults to {}.
-            pos (tuple | str, optional): Position of object. Defaults to (0,0).
-            name (str, optional): Name of object. Defaults to 'Obj'.
-            scale (int, optional): The image scale. Defaults to 10.
+            properties (dict, optional): Sprite properties. Defaults to {}.
+            scale (int, optional): Sprite image scale. Defaults to 10.
         """
         
         super().__init__(filesystem, gamepath, assets, baseassets)
-        
         this.file = super().get_file(file)
         
-        this._properties = deepcopy(properties)
-        if isinstance(pos, str):
-            this.pos = tuple([float(a) for a in pos.split()])
-        else:
-            this.pos = tuple(pos)
-        
         this.xml : etree.ElementBase = etree.parse(this.file).getroot()
-        this.sprites : list[Sprite] = []
-        this.shapes : list[Shape] = []
-        this.UVs : list[tuple[int,int]] = []
-        this.VertIndices : list[int] = []
-        this.defaultProperties = {}
-        this.properties = {}
-        this.name = name
         
-        this.offset = [0,0]
+        this.properties = deepcopy(properties)
+        this.animations : list[Sprite.Animation] = []
+        
         this.scale = scale
         
         this.readXML()
-        
+        this.animation = 0
+    
+    def setAnimation(this, animation : str | int):
+        """Set the current animation for the Sprite
+
+        Args:
+            animation (str | int): Animation name or index.
+        """
+        this.animation = animation
     
     @property
     def image(this) -> Image.Image:
+        """Image of sprite
+
+        Returns:
+            PIL.Image.Image: PIL Image
+        """
+        image = this.animation.image.copy()
+        gridSize = numpy.array(this.gridSize)
+        size = gridSize * this.scale
+        size = [abs(round(x)) for x in size]
+        image = image.resize(size)
         
-        rects = []
-        background = []
-        foreground = []
-        
-        image = Image.new('RGBA', (1,1), (0,0,0,0))
-        for sprite in this.sprites:
-            if 'visible' in sprite.properties:
-                if not strbool(sprite.properties['visible']):
-                    continue
-            if ('isBackground' in sprite.properties) and strbool(sprite.properties['isBackground']):
-                background.append(sprite)
-            else:
-                foreground.append(sprite)
-                
-            pos = numpy.array(sprite.pos)
-            size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
-            
-            rects.append(
-                tuple(pos - (size / 2))
-            )
-            rects.append(
-                tuple(pos + (size / 2))
-            )
-            
-        rects = numpy.array(rects).swapaxes(0,1)
-        
-        min = numpy.array([math.floor(v.min()) for v in rects])
-        max = numpy.array([math.ceil(v.max()) for v in rects])
-        
-        maxSize = max - min
-        
-        this.offset = [a.mean() for a in numpy.array([min,max]).swapaxes(0,1)]
-        
-        print(f'{min = }')
-        print(f'{max = }')
-        print(rects)
-        print(maxSize)
-        print(f'{this.offset = }')
-        
-        
-        image = Image.new('RGBA', tuple(maxSize * this.scale), (0,0,0,0))
-        
-        sprites = list(reversed(background)) + foreground
+        image = image.rotate(this.angle, Image.BILINEAR, expand=True)
         
-        for sprite in sprites:
-            size = (numpy.array(sprite.image.size) / sprite.scale) * [1,-1]
-            pos = this.truePos(
-                sprite.pos,
-                size,
-                maxSize,
-                scale = this.scale,
-                offset = this.offset
-            )
-            
-            print(f'{pos = }')
-            
-            image.alpha_composite(
-                sprite.image,
-                tuple([round(x) for x in pos]),
-            )
-            
         return image
     
     @property
-    def PhotoImage(this):
-        this._PhotoImage = ImageTk.PhotoImage(this.image)
-        return this._PhotoImage
+    def animation(this) -> 'Sprite.Animation':
+        """Returns the current animation
+
+        Returns:
+            Sprite.Animation: A Sprite.Animation class
+        """
+        return this._currentAnimation
+    @animation.setter
+    def animation(this, animation : str | int):
+        if isinstance(animation, (int, float)):
+            animation = int(animation)
+            this._currentAnimation = this.animations[animation]
+        elif isinstance(animation, str):
+            for a in this.animations:
+                if a.name == animation:
+                    this._currentAnimation = a
+                    break
+        elif isinstance(animation, this.Animation):
+            this._currentAnimation = animation
     
     @property
-    def scale(this):
-        return this._scale
-    @scale.setter
-    def scale(this, value : int):
-        this._scale = value
-        for sprite in this.sprites:
-            sprite.scale = this._scale
+    def frame(this) -> int:
+        """The current animation frame.
+
+        Returns:
+            int: Current animation frame index.
+        """
+        return this.animation.frame
+    @frame.setter
+    def frame(this, value : int):
+        this.animation.frame = value
+    
+    @property
+    def filename(this) -> str:
+        """Sprite filename
+        """
+        if 'filename' in this.properties:
+            return this.properties['filename']
+        else:
+            return None
+    @filename.setter
+    def filename(this, value):
+        this.properties['filename'] = value
         
     def readXML(this):
-        """Read object XML
+        """Read Sprite XML
         """
-        
-        # specifically specifying type so it's easier to use in vscode
-        tags = {
-            'Shapes': this._getShapes,
-            'Sprites': this._getSprites,
-            'UVs': this._getUVs,
-            'VertIndices': this._getVertIndices,
-            'DefaultProperties': this._getDefaultProperties,
-        }
-        
+        this.animations = []
         for element in this.xml:
-            if element is etree.Comment:
-                continue
-            if element.tag in tags:
-                tags[element.tag](element)
-        
-        this.getProperties()
+            if (not element is etree.Comment) or element.tag == 'Animation':
+                animation = this.Animation(
+                    element,
+                    this.filesystem
+                )
+                
+                this.animations.append(animation)
     
-    def export(this, path : str = None) -> bytes:
-        """Export object XML
+    def export(this, path : str = None):
+        """Export the Sprite XML file
 
         Args:
-            path (str, optional): Filename for object. Defaults to Object.filename.
+            path (str, optional): Path to export into the filesystem. Defaults to the original filename.
 
         Raises:
-            TypeError: Path is not a file
+            TypeError: Path is not a file.
 
         Returns:
-            bytes: XML file.
+            str: Contents of saved file.
         """
-        xml : etree.ElementBase = etree.Element('InteractiveObject')
-        
-        shapes = etree.Element('Shapes')
-        
-        for shape in this.shapes:
-            shape : Shape
-            shapes.append(shape.getXML())
-        
-        if len(shapes) > 0:
-            xml.append(shapes)
-        
-        sprites : etree.ElementBase = etree.Element('Sprites')
-        
-        for sprite in this.sprites:
-            sprite : Sprite
-            sprite.export()
-            etree.SubElement(sprites, 'Sprite', sprite.properties)
-        
-        if len(sprites) > 0:
-            xml.append(sprites)
-        
-        UVs : etree.ElementBase = etree.Element('UVs')
-        
-        for UV in this.UVs:
-            pos = ' '.join([str(_) for _ in UV])
-            etree.SubElement(UVs, 'UV', {'pos': pos})
+        xml : etree.ElementBase = etree.Element('Sprite')
         
-        if len(UVs) > 0:
-            xml.append(UVs)
-        
-        VertIndices : etree.ElementBase = etree.Element('VertIndices')
-        
-        for index in this.VertIndices:
-            etree.SubElement(VertIndices, 'Vert', {'index': str(index)})
-        
-        if len(VertIndices) > 0:
-            xml.append(VertIndices)
-        
-        DefaultProperties : etree.ElementBase = etree.Element('DefaultProperties')
-        
-        for name in this.defaultProperties:
-            etree.SubElement(DefaultProperties, 'Property', {
-                'name': name,
-                'value': this.defaultProperties[name]
-            })
-        
-        if len(DefaultProperties) > 0:
-            xml.append(DefaultProperties)
+        for animation in this.animations:
+            xml.append(animation.getXML())
         
         this.xml = xml
+        
         output = etree.tostring(xml, pretty_print=True, xml_declaration=True, encoding='utf-8')
         
         if path == None:
             if this.filename:
                 path = this.filename
         
         if path != None:
             if (file := this.filesystem.get(path)) != None:
                 if isinstance(file, File):
                     file.write(output)
                 else:
                     raise TypeError(f'Path {path} is not a file.')
-                    
             else:
                 this.filesystem.add(path, output)
         
         return output
     
-    def updateProperties(this):
-        """Update properties. Deletes any properties that are the same as defaultProperties.
+    @property
+    def visible(this) -> bool:
+        """Whether this Sprite is visible or not
         """
-        properties = list(this.properties.keys())
-        
-        for property in properties:
-            if property in this.defaultProperties:
-                if this.properties[property] == this.defaultProperties[property]:
-                    del this.properties[property]
+        if 'visible' in this.properties:
+            return strbool(this.properties['visible'])
+        return False
+    @visible.setter
+    def visible(this, value : bool | str):
+        this.properties['visible'] = str(strbool(value)).lower()
+    
+    @property
+    def isBackground(this):
+        """Whether this Sprite is a background
+        """
+        if 'isBackground' in this.properties:
+            return strbool(this.properties['isBackground'])
+        return False
+    @isBackground.setter
+    def isBackground(this, value : bool | str):
+        this.properties['isBackground'] = str(strbool(value)).lower()
+    
+    @property
+    def gridSize(this) -> tuple[float,float]:
+        """The gridSize (size) of this Sprite
 
-    def getLevelXML(
-        this,
-        filename : str = None,
-    ) -> etree.ElementBase:
-        """Gets XML to be used in levels.
+        Returns:
+            tuple[float,float]: (width,height)
+        """
+        if 'gridSize' in this.properties:
+            return tuple([float(x) for x in this.properties['gridSize'].split()])
+        return (1,1)
+    @gridSize.setter
+    def gridSize(this, value : tuple[int,int] | str):
+        if isinstance(value, str):
+            this.properties['gridSize'] = value
+        elif isinstance(value, (tuple, list)):
+            this.properties['gridSize'] = ' '.join([str(x) for x in value])
+    
+    @property
+    def pos(this) -> tuple[float,float]:
+        """Position of Sprite relative to the center of the Object
 
-        Args:
-            filename (str, optional): Object filename. Defaults to Object.filename.
+        Returns:
+            tuple[float,float]: (x,y)
+        """
+        if 'pos' in this.properties:
+            return tuple([float(x) for x in this.properties['pos'].split()])
+        return (0,0)
+    @pos.setter
+    def pos(this, value : tuple[int,int] | str):
+        if isinstance(value, str):
+            this.properties['pos'] = value
+        elif isinstance(value, (tuple, list)):
+            this.properties['pos'] = ' '.join([str(x) for x in value])
+    
+    @property
+    def angle(this) -> float:
+        """Sprite rotation angle
 
         Returns:
-            etree.Element: lxml Element
+            float: Angle as degrees
         """
-        if filename == None:
-            if this.filename:
-                filename = this.filename
-        else:
-            this.filename = filename
-        
-        xml = etree.Element('Object', name = this.name)
-        etree.SubElement(xml, 'AbsoluteLocation', value = ' '.join([str(_) for _ in this.pos]))
-        
-        properties = etree.SubElement(xml, 'Properties')
-        
-        this.updateProperties()
+        if 'angle' in this.properties:
+            return float(this.properties['angle'])
+        return 0
+    @angle.setter
+    def angle(this, value : int | float):
+        this.properties['angle'] = str(value)
+
+    class Animation(GameObject):
+        def __init__(
+            this,
+            xml : str | etree.ElementBase,
+            filesystem: Filesystem | Folder = None,
+            gamepath: str = None,
+            assets: str = '/assets',
+            baseassets: str = '/',
+        ) -> None:
+            """Animation for Sprite.
+
+            Args:
+                xml (str | etree.Element): lxml.etree Element xml element for sprite.
+                filesystem (Filesystem | Folder, optional): Filesystem to use. Defaults to None.
+                gamepath (str, optional): Game path. Only used if filesystem not specified. Defaults to None.
+                assets (str, optional): Assets path relative to game path. Only used if filesystem not specified. Defaults to '/assets'.
+                baseassets (str, optional): Base assets path within the assets folder, e.g. `/perry/` in wmp. Defaults to `/`
+            """
+            super().__init__(filesystem, gamepath, assets, baseassets)
+            
+            if isinstance(xml, str):
+                this.xml : etree.ElementBase = etree.parse(xml).getroot()
+            else:
+                this.xml = xml
+            
+            this.properties = {}
+            this.name = ''
+            this.textureBasePath = '/Textures/'
+            this.atlas : Imagelist = None
+            this.fps = 30
+            this.playbackMode = 'ONCE'
+            this.loopCount = 1
+            
+            this._PhotoImage = None
+            
+            this.frame = 0
+            
+            this.frames : list[Sprite.Animation.Frame] = []
+            
+            this.readXML()
         
-        for name in this.properties:
-            value = this.properties[name]
+        @property
+        def image(this) -> Image.Image:
+            """Current Animation image
+
+            Returns:
+                PIL.Image.Image: PIL Image
+            """
+            if this.frame > len(this.frames):
+                this.frame = 0
+            if this.frame < 0:
+                this.frame = len(this.frames)
             
-            etree.SubElement(properties, 'Property', name = name, value = value)
+            return this.frames[this.frame].image
         
-        return xml
-    
-    @property
-    def filename(this):
-        if 'Filename' in this.properties:
-            return this.properties['Filename']
-        else:
-            return None
-    @filename.setter
-    def filename(this, value : str):
-        this.properties['Filename'] = value
-    
-    @property
-    def type(this):
-        if 'Type' in this.properties:
-            return this.properties['Type']
-        elif 'Type' in this.defaultProperties:
-            return this.defaultProperties['Type']
-        else:
-            return None
-    @type.setter
-    def type(this, value : str):
-        if not isinstance(value, str):
-            raise TypeError('type is not a string')
-        
-        if not 'Type' in this.defaultProperties:
-            this.defaultProperties['Type'] = value
-        this.properties['Type'] = value
-    
-    def _getShapes(this, xml : etree.ElementBase):
-        for element in xml:
-            shape = Shape(element)
-            this.shapes.append(shape)
-        
-    def _getSprites(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            
-            if element.tag == 'Sprite':
-                attributes = element.attrib
-                sprite = Sprite(
-                    file = this.filesystem.get(attributes['filename']),
-                    filesystem = this.filesystem,
-                    properties = attributes,
-                    scale = this.scale,
+        @property
+        def PhotoImage(this) -> ImageTk.PhotoImage:
+            """Tkinter PhotoImage for the Animation
+            """
+            this._PhotoImage = ImageTk.PhotoImage(this.image)
+            return this._PhotoImage
+            
+        def readXML(this):
+            """Read the xml for this Animation
+            """
+            this.getAttributes()
+            this.getFrames()
+        
+        def getAttributes(this):
+            """Get all the attributes of this Animation
+            """
+            this.properties = this.xml.attrib
+            
+            if 'name' in this.properties:
+                this.name = this.properties['name']
+            if 'textureBasePath' in this.properties:
+                this.textureBasePath = this.properties['textureBasePath']
+            if 'atlas' in this.properties:
+                this.atlasPath = this.properties['atlas']
+                this.atlas = Imagelist(
+                    this.filesystem.get(this.properties['atlas']),
+                    this.filesystem,
+                    HD=False
                 )
-                this.sprites.append(sprite)
-    
-    def _getUVs(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'UV':
-                pos = element.get('pos')
-                this.UVs.append(tuple([float(_) for _ in pos.split()]))
-    
-    def _getVertIndices(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'Vert':
-                index = element.get('index')
-                this.VertIndices.append(int(index))
-    
-    def getProperties(this):
-        for prop in this.defaultProperties:
-            this.properties[prop] = this.defaultProperties[prop]
-        for prop in this._properties:
-            this.properties[prop] = this._properties[prop]
-        return this.properties
-    
-    def _getDefaultProperties(this, xml : etree.ElementBase):
-        for element in xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'Property':
-                name = element.get('name')
-                value = element.get('value')
                 
-                this.defaultProperties[name] = value
-    
-    def setProperty(this, property : str | dict, value : str = ''):
-        """Set object property.
+                # this.atlasHD = Imagelist(
+                #     this.filesystem.get(this.properties['atlas']),
+                #     this.filesystem,
+                #     HD=True
+                # )
+                
+            if 'fps' in this.properties:
+                this.fps = float(this.properties['fps'])
+            if 'playbackMode' in this.properties:
+                this.playbackMode = this.properties['playbackMode']
+            if 'loopCount' in this.properties:
+                this.loopCount = int(this.properties['loopCount'])
+            
+            
+        def getFrames(this) -> list['Sprite.Animation.Frame']:
+            """Get a list of all the Animation `Frame`s
 
-        Args:
-            property (str | dict): Property name to set. If value is dict, it will combine the properties in the dict with the current properties.
-            value (str, optional): Property value. Defaults to ''.
-        """
-        if isinstance(property, dict):
-            for name in property:
-                this.properties[name] = property[name]
-            return
-        this.properties[property] = value
-
-class Shape():
-    def __init__(this, xml : etree.ElementBase = None) -> None:
-        """Shape for Object
+            Returns:
+                list[Sprite.Animation.Frame]: List of all the Frames in this Animation.
+            """
+            this.frames = []
+            
+            if this.xml == None:
+                return None
+            for f in this.xml:
+                if (not f is etree.Comment) and f.tag == 'Frame':
+                    this.frames.append(this.Frame(
+                        f.attrib,
+                        this.atlas,
+                        this.textureBasePath
+                    ))
+            
+            return this.frames
 
-        Args:
-            xml (etree.Element, optional): lxml Element. Defaults to None.
-        """
-        this.points = []
-        this.xml = xml
+        def updateProperties(this):
+            """Update the Sprite properties
+            """
+            def updateProperty(property : str, value, default = None):
+                if default != None and value == default:
+                    if property in this.properties:
+                        del this.properties[property]
+                else:
+                    this.properties[property] = value
+            
+            updateProperty('name', this.name)
+            updateProperty('textureBasePath', this.textureBasePath)
+            this.atlas.export(this.atlasPath, exportImage=True)
+            updateProperty('atlas', this.atlasPath)
+            updateProperty('fps', str(this.fps))
+            updateProperty('playbackMode', this.playbackMode)
+            updateProperty('loopCount', str(this.loopCount))
+        
+        def getXML(this):
+            """Get the XML of this Animation
+
+            Returns:
+                etree.Element: etree Element
+            """
+            this.updateProperties()
+            xml : etree.ElementBase = etree.Element('Animation', **this.properties)
+            
+            for frame in this.frames:
+                xml.append(frame.getXML())
+            
+            this.xml = xml
+            return this.xml
         
-        this.readXML()
-    
-    def readXML(this):
-        """Read XML if any.
-        """
-        if this.xml == None:
-            return
-        for element in this.xml:
-            if element is etree.Comment:
-                continue
-            if element.tag == 'Point':
-                pos : str = element.get('pos')
-                point = tuple([float(_) for _ in pos.split()])
-                this.points.append(point)
-    
-    def getXML(this) -> etree.ElementBase:
-        """Gets Shape XML for Object.
+        
+        # Frame
+        class Frame():
+            _offset = (0,0)
+            _scale = (1,1)
+            _angleDeg = 0
+            _repeat = 1
+            def __init__(
+                this,
+                properties : dict,
+                atlas : Imagelist = None,
+                textureBasePath : str = None,
+            ) -> None:
+                """Frame for Sprite.Animation.
+
+                Args:
+                    this (_type_): _description_
+                    properties (dict): Image properties.
+                    atlas (Imagelist, optional): Image atlas for Image. Defaults to None.
+                    textureBasePath (str, optional): Directory to put image in. Defaults to None.
+                """
+                this.atlas = atlas
+                this.textueBasePath = textureBasePath
+                this.properties = properties
+                
+                this.name = ''
+                this.offset = this._offset
+                this.scale = this._scale
+                this.angleDeg = this._angleDeg
+                this.repeat = this._repeat
+                
+                
+                
+                this.getData()
+                this.getImage()
+            
+            def getData(this):
+                """Get the Frame data
+                """
+                if 'name' in this.properties:
+                    this.name = this.properties['name']
+                if 'offset' in this.properties:
+                    this.offset = tuple([float(x) for x in this.properties['offset'].split()])
+                if 'scale' in this.properties:
+                    this.scale = tuple([float(x) for x in this.properties['scale'].split()])
+                if 'angleDeg' in this.properties:
+                    this.angleDeg = float(this.properties['angleDeg'])
+                if 'repeat' in this.properties:
+                    this.repeat = int(this.properties['repeat'])
+                
+            def getImage(this):
+                this._image = this.atlas.getImage(this.name)
+            
+            @property
+            def image(this) -> Image.Image:
+                """Image of this Image
+
+                Returns:
+                    PIL.Image.Image: PIL Image
+                """
+                if this._image:
+                    image = this._image.image.copy()
+                    image = image.resize(tuple([round(_) for _ in (numpy.array(this._image.size) * numpy.array(this.scale))]))
+                    image = image.rotate(this.angleDeg, expand = True)
+                else:
+                    image = Image.new('RGBA', (1,1), (0,0,0,0))
+                return image
+            @image.setter
+            def image(this, image : Image.Image):
+                this._image = image
+            
+            def updateProperties(this):
+                """Update Image properties
+                """
+                def updateProperty(property : str, value, default):
+                    if value == default:
+                        if property in this.properties:
+                            del this.properties[property]
+                    else:
+                        this.properties[property] = value
+                
+                this.properties['name'] = this.name
+                
+                updateProperty(
+                    'offset',
+                    ' '.join([str(_) for _ in this.offset]),
+                    ' '.join([str(_) for _ in this._offset])
+                )
+                
+                updateProperty(
+                    'scale',
+                    ' '.join([str(_) for _ in this.scale]),
+                    ' '.join([str(_) for _ in this._scale])
+                )
+                
+                updateProperty(
+                    'angleDeg',
+                    str(this.angleDeg),
+                    str(this._angleDeg)
+                )
+                
+                updateProperty(
+                    'repeat',
+                    str(this.repeat),
+                    str(this._repeat)
+                )
 
-        Returns:
-            etree.Element: lxml Element.
-        """
-        xml : etree.ElementBase = etree.Element('Shape')
-        for point in this.points:
-            etree.SubElement(xml, 'Point', {'pos': ' '.join([str(_) for _ in point])})
-        this.xml = xml
-        return xml
+            def getXML(this) -> etree.ElementBase:
+                """Get the XML for the Frame
+
+                Returns:
+                    etree.Element: XML of this Frame
+                """
+                this.updateProperties()
+                return etree.Element('Frame', **this.properties)
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/widget/__init__.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/classes/widget/widget.py` & `wmwpy-0.2.0b0/src/wmwpy/classes/widget/widget.py`

 * *Files identical despite different names*

### Comparing `wmwpy-0.1.1b0/src/wmwpy/gameobject.py` & `wmwpy-0.2.0b0/src/wmwpy/gameobject.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         #     print(f'Error: {str(e)}')
         #     raise FileNotFoundError('Must have a valid `filesystem` or `gamepath`')
     
     def get_file(
         this,
         file : bytes | File | io.BytesIO | str,
         template : str | io.BytesIO = None,
-        ) -> io.BytesIO | str:
+    ) -> io.BytesIO | str:
         """Get file
 
         Args:
             file (bytes | wmwpy.Utils.filesystem.File | io.BytesIO | str): Content of file. Can be bytes, wmwpy File, str (contents of file) or file-like object.
             template (str | io.BytesIO, optional): Fallback for file if file == None. Defaults to ''
 
         Raises:
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy/gametemplate.py` & `wmwpy-0.2.0b0/src/wmwpy/gametemplate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 
-from .Game import Game
+from .game import Game
 
 # Where's My Water?
 class WMW(Game):
     _DB = '/Data/water.db'
     _BASEASSETS = '/'
     _PROFILE = None
     
@@ -177,15 +177,21 @@
         db: str = '/Data/water-Lite.db',
         profile: str = None,
         baseassets: str = '/',
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
         super().__init__(gamepath, assets, db, profile, baseassets, hook)
     
-    def mode(this, mode = 'wmw'):
+    def mode(this, mode : typing.Literal['wmw', 'wmp'] = 'wmw'):
+        """Switch game mode from 'wmw' to 'wmp' and vice verca.
+
+        Args:
+            mode (str, optional): Mode. Can be 'wmw' or 'wmp'. Defaults to 'wmw'.
+        """
+        
         mode = mode.lower()
         if mode == 'wmw':
             this.db = '/Data/water-Lite.db'
             this.baseassets = '/'
             
             this._DB = '/Data/water-Lite.db'
             this._BASEASSETS = '/'
@@ -211,14 +217,25 @@
         hook: typing.Callable[[int, str, int], typing.Any] = None
     ) -> None:
         super().__init__(gamepath, assets, db, profile, baseassets, hook)
 
 GAMES : dict[str, Game] = {}
 
 def register_game(name : str, class_ : Game):
+    """Register a game template
+
+    Args:
+        name (str): Name of the game. E.G. 'WMW'
+        class_ (Game): A class that has been inherited by the `Game` object.
+
+    Raises:
+        TypeError: class has to be inherited by Game
+        TypeError: name must be a string
+        NameError: game already exists
+    """
     
     if not isinstance(class_, type):
         class_ = class_.__class__
     
     if not isinstance(class_(None), Game):
         raise TypeError('class has to be inherited by Game')
     if not isinstance(name, str):
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy.egg-info/PKG-INFO` & `wmwpy-0.2.0b0/src/wmwpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmwpy
-Version: 0.1.1b0
+Version: 0.2.0b0
 Summary: Python module to work with Where's My...? games files.
 Author: ego-lay-atman-bay
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,14 +676,15 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/wmw-modding/wmwpy
 Project-URL: Bug Tracker, https://github.com/wmw-modding/wmwpy/issues
+Project-URL: Documentation, https://wmw-modding.github.io/wmwpy/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wmwpy-0.1.1b0/src/wmwpy.egg-info/SOURCES.txt` & `wmwpy-0.2.0b0/src/wmwpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
-src/wmwpy/Game.py
 src/wmwpy/__init__.py
+src/wmwpy/game.py
 src/wmwpy/gameobject.py
 src/wmwpy/gametemplate.py
 src/wmwpy.egg-info/PKG-INFO
 src/wmwpy.egg-info/SOURCES.txt
 src/wmwpy.egg-info/dependency_links.txt
 src/wmwpy.egg-info/requires.txt
 src/wmwpy.egg-info/top_level.txt
 src/wmwpy/Font/__init__.py
 src/wmwpy/Utils/XMLTools.py
 src/wmwpy/Utils/__init__.py
 src/wmwpy/Utils/filesystem.py
 src/wmwpy/Utils/path.py
+src/wmwpy/Utils/rotate.py
 src/wmwpy/Utils/textures.py
 src/wmwpy/Utils/waltex.py
 src/wmwpy/Utils/Types/Documents.py
 src/wmwpy/Utils/Types/Images.py
 src/wmwpy/Utils/Types/__init__.py
 src/wmwpy/classes/Widgets.py
 src/wmwpy/classes/__init__.py
```

