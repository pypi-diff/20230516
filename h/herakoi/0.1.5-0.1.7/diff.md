# Comparing `tmp/herakoi-0.1.5.tar.gz` & `tmp/herakoi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herakoi-0.1.5.tar", last modified: Wed Dec 14 08:03:10 2022, max compression
+gzip compressed data, was "herakoi-0.1.7.tar", last modified: Tue May 16 17:16:20 2023, max compression
```

## Comparing `herakoi-0.1.5.tar` & `herakoi-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2022-12-14 08:03:10.008735 herakoi-0.1.5/
--rw-r--r--   0 lucadim    (501) staff       (20)     1072 2022-12-14 08:02:18.000000 herakoi-0.1.5/LICENSE.md
--rw-r--r--   0 lucadim    (501) staff       (20)     2978 2022-12-14 08:03:10.008615 herakoi-0.1.5/PKG-INFO
--rw-r--r--   0 lucadim    (501) staff       (20)     2361 2022-12-14 08:02:18.000000 herakoi-0.1.5/README.md
-drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2022-12-14 08:03:10.007688 herakoi-0.1.5/herakoi/
--rw-r--r--   0 lucadim    (501) staff       (20)      733 2022-12-14 08:02:18.000000 herakoi-0.1.5/herakoi/__init__.py
--rw-r--r--   0 lucadim    (501) staff       (20)       57 2022-12-14 08:02:18.000000 herakoi-0.1.5/herakoi/__main__.py
--rw-r--r--   0 lucadim    (501) staff       (20)     7381 2022-12-14 08:02:18.000000 herakoi-0.1.5/herakoi/core.py
-drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2022-12-14 08:03:10.008464 herakoi-0.1.5/herakoi.egg-info/
--rw-r--r--   0 lucadim    (501) staff       (20)     2978 2022-12-14 08:03:10.000000 herakoi-0.1.5/herakoi.egg-info/PKG-INFO
--rw-r--r--   0 lucadim    (501) staff       (20)      279 2022-12-14 08:03:10.000000 herakoi-0.1.5/herakoi.egg-info/SOURCES.txt
--rw-r--r--   0 lucadim    (501) staff       (20)        1 2022-12-14 08:03:10.000000 herakoi-0.1.5/herakoi.egg-info/dependency_links.txt
--rw-r--r--   0 lucadim    (501) staff       (20)       42 2022-12-14 08:03:10.000000 herakoi-0.1.5/herakoi.egg-info/entry_points.txt
--rw-r--r--   0 lucadim    (501) staff       (20)       60 2022-12-14 08:03:10.000000 herakoi-0.1.5/herakoi.egg-info/requires.txt
--rw-r--r--   0 lucadim    (501) staff       (20)        8 2022-12-14 08:03:10.000000 herakoi-0.1.5/herakoi.egg-info/top_level.txt
--rw-r--r--   0 lucadim    (501) staff       (20)      916 2022-12-14 08:02:18.000000 herakoi-0.1.5/pyproject.toml
--rw-r--r--   0 lucadim    (501) staff       (20)       38 2022-12-14 08:03:10.008769 herakoi-0.1.5/setup.cfg
+drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-05-16 17:16:20.207246 herakoi-0.1.7/
+-rw-r--r--   0 lucadim    (501) staff       (20)     1072 2023-05-16 17:15:39.000000 herakoi-0.1.7/LICENSE.md
+-rw-r--r--   0 lucadim    (501) staff       (20)     3048 2023-05-16 17:16:20.207098 herakoi-0.1.7/PKG-INFO
+-rw-r--r--   0 lucadim    (501) staff       (20)     2431 2023-05-16 17:15:39.000000 herakoi-0.1.7/README.md
+drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-05-16 17:16:20.205848 herakoi-0.1.7/herakoi/
+-rw-r--r--   0 lucadim    (501) staff       (20)     1056 2023-05-16 17:15:39.000000 herakoi-0.1.7/herakoi/__init__.py
+-rw-r--r--   0 lucadim    (501) staff       (20)       57 2023-05-16 17:15:39.000000 herakoi-0.1.7/herakoi/__main__.py
+-rw-r--r--   0 lucadim    (501) staff       (20)    11662 2023-05-16 17:15:39.000000 herakoi-0.1.7/herakoi/core.py
+drwxr-xr-x   0 lucadim    (501) staff       (20)        0 2023-05-16 17:16:20.206870 herakoi-0.1.7/herakoi.egg-info/
+-rw-r--r--   0 lucadim    (501) staff       (20)     3048 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/PKG-INFO
+-rw-r--r--   0 lucadim    (501) staff       (20)      279 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/SOURCES.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)        1 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/dependency_links.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)       42 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/entry_points.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)       72 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/requires.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)        8 2023-05-16 17:16:20.000000 herakoi-0.1.7/herakoi.egg-info/top_level.txt
+-rw-r--r--   0 lucadim    (501) staff       (20)     1054 2023-05-16 17:15:39.000000 herakoi-0.1.7/pyproject.toml
+-rw-r--r--   0 lucadim    (501) staff       (20)       38 2023-05-16 17:16:20.207292 herakoi-0.1.7/setup.cfg
```

### Comparing `herakoi-0.1.5/LICENSE.md` & `herakoi-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `herakoi-0.1.5/PKG-INFO` & `herakoi-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herakoi
-Version: 0.1.5
+Version: 0.1.7
 Summary: A sonification tool
 Author-email: Michele Ginolfi <micheleginolfi@gmail.com>, Luca Di Mascolo <lucadimascolo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucadimascolo/herakoi
 Project-URL: Bug Tracker, https://github.com/lucadimascolo/herakoi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -42,15 +42,15 @@
 ```
 pip install mediapipe-silicon
 ```
 
 ## Usage
 
 1. run `herakoi path_to_your_favorite_image`
-2. open your favorite MIDI virtual keyboard
+2. open your favorite MIDI player (e.g., if you run `herakoi` on an Apple computer, GarageBang is a good option) 
 3. have fun!
 
 You can customize your `herakoi` by using the following flags:
 * `--notes XX YY`, that will allow the pitch to span the range from the note `XX` and `YY` (with `XX` equal to, e.g., C4 for middle C)
 * `--volume ZZ`, that will set lower threshold for the note volume (with `ZZ` in percentage)
 * `--switch`, inverting the color-brightness mapping
```

### Comparing `herakoi-0.1.5/README.md` & `herakoi-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 pip install mediapipe-silicon
 ```
 
 ## Usage
 
 1. run `herakoi path_to_your_favorite_image`
-2. open your favorite MIDI virtual keyboard
+2. open your favorite MIDI player (e.g., if you run `herakoi` on an Apple computer, GarageBang is a good option) 
 3. have fun!
 
 You can customize your `herakoi` by using the following flags:
 * `--notes XX YY`, that will allow the pitch to span the range from the note `XX` and `YY` (with `XX` equal to, e.g., C4 for middle C)
 * `--volume ZZ`, that will set lower threshold for the note volume (with `ZZ` in percentage)
 * `--switch`, inverting the color-brightness mapping
```

### Comparing `herakoi-0.1.5/herakoi/__init__.py` & `herakoi-0.1.7/herakoi/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,13 +6,18 @@
                     help='Input image',
                     nargs='?')
   pars.add_argument('--notes',
                     help='Define the pitch range (as note+octave format; e.g., C4)',
                     nargs=2,default=['C1','B8'],metavar=('low','high'))
   pars.add_argument('--volume',
                     help='Change the low volume threshold (in percentage)',
-                    nargs=1,default=['20'],metavar=('volume',))
+                    default=20,metavar=('volume'),type=float)
+  pars.add_argument('--mode',
+                    help='Select herakoi mode [single/adaptive/scan]',
+                    default='single',metavar=('mode'))
+  pars.add_argument('--box',
+                    help='sonification box size in units of frame percentage',
+                    default=2,metavar=('box'),type=float)
   pars.add_argument('--switch',action='store_true')
-
   args = pars.parse_args()
 
-  start(image=args.image,mode='single',notes=(args.notes[0],args.notes[1]),volume=float(args.volume[0]),switch=args.switch)
+  start(image=args.image,mode=args.mode,notes=(args.notes[0],args.notes[1]),volume=args.volume,box=args.box,switch=args.switch)
```

### Comparing `herakoi-0.1.5/herakoi.egg-info/PKG-INFO` & `herakoi-0.1.7/herakoi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herakoi
-Version: 0.1.5
+Version: 0.1.7
 Summary: A sonification tool
 Author-email: Michele Ginolfi <micheleginolfi@gmail.com>, Luca Di Mascolo <lucadimascolo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/lucadimascolo/herakoi
 Project-URL: Bug Tracker, https://github.com/lucadimascolo/herakoi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -42,15 +42,15 @@
 ```
 pip install mediapipe-silicon
 ```
 
 ## Usage
 
 1. run `herakoi path_to_your_favorite_image`
-2. open your favorite MIDI virtual keyboard
+2. open your favorite MIDI player (e.g., if you run `herakoi` on an Apple computer, GarageBang is a good option) 
 3. have fun!
 
 You can customize your `herakoi` by using the following flags:
 * `--notes XX YY`, that will allow the pitch to span the range from the note `XX` and `YY` (with `XX` equal to, e.g., C4 for middle C)
 * `--volume ZZ`, that will set lower threshold for the note volume (with `ZZ` in percentage)
 * `--switch`, inverting the color-brightness mapping
```

### Comparing `herakoi-0.1.5/pyproject.toml` & `herakoi-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-  [build-system]
+[build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.isort]
 known_third_party = ["mediapipe","mediapipe-silicon"]
 
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+include = ["herakoi*"]
+exclude = ["images*"]
+
 [project]
 name = "herakoi"
-version = "0.1.5"
+version = "0.1.7"
 authors = [
   { name="Michele Ginolfi", email="micheleginolfi@gmail.com" },
   { name="Luca Di Mascolo", email="lucadimascolo@gmail.com" },
 ]
 description = "A sonification tool"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { text = "MIT License" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
 ]
-dependencies = ["mido>=1.2","python-rtmidi>=1.4","opencv-python>=4.6","numpy>=1.23"]
+dependencies = ["mido>=1.2","python-rtmidi>=1.4","opencv-python>=4.6","numpy>=1.23","pynput>=1.7"]
 
 [project.urls]
 "Homepage" = "https://github.com/lucadimascolo/herakoi"
 "Bug Tracker" = "https://github.com/lucadimascolo/herakoi/issues"
 
 [project.scripts]
 herakoi = "herakoi:basic"
```

