# Comparing `tmp/backgroundremover-0.2.1.tar.gz` & `tmp/backgroundremover-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backgroundremover-0.2.1.tar", last modified: Fri May  5 19:51:39 2023, max compression
+gzip compressed data, was "dist/backgroundremover-0.2.2.tar", last modified: Tue May 16 04:26:44 2023, max compression
```

## Comparing `backgroundremover-0.2.1.tar` & `backgroundremover-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.1/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.1/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     6149 2023-05-05 19:20:58.000000 backgroundremover-0.2.1/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover/
--rw-rw-r--   0 john      (1000) john      (1000)      173 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     6793 2023-05-05 19:18:41.000000 backgroundremover-0.2.1/backgroundremover/bg.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/cmd/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/cmd/server.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.1/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)    12586 2023-05-05 19:18:06.000000 backgroundremover-0.2.1/backgroundremover/utilities.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     8101 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      654 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      364 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/backgroundremover.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.1/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)      364 2023-04-30 21:22:20.000000 backgroundremover-0.2.1/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-05 19:51:39.000000 backgroundremover-0.2.1/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1018 2023-05-05 19:51:38.000000 backgroundremover-0.2.1/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.2/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.2/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     6191 2023-05-15 23:12:59.000000 backgroundremover-0.2.2/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover/
+-rw-rw-r--   0 john      (1000) john      (1000)      175 2023-05-16 04:22:05.000000 backgroundremover-0.2.2/backgroundremover/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6962 2023-05-16 02:33:37.000000 backgroundremover-0.2.2/backgroundremover/bg.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/cmd/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12628 2023-05-15 23:12:59.000000 backgroundremover-0.2.2/backgroundremover/utilities.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      654 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       18 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.2/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-06 14:07:42.000000 backgroundremover-0.2.2/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1027 2023-05-16 04:26:22.000000 backgroundremover-0.2.2/setup.py
```

### Comparing `backgroundremover-0.2.1/LICENSE.txt` & `backgroundremover-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/PKG-INFO` & `backgroundremover-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.1
-Summary: Background remover from image and video
+Version: 0.2.2
+Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
-        ![Background Remover](/examplefiles/backgroundremoverexample.png)
-        <img alt="background remover video" src="/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
-        BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video), made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
+        ![Background Remover](https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverexample.png)
+        <img alt="background remover video" src="https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
+        BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video) using AI, made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
         
         
         ### Requirements
         
         * python >= 3.6
-        * python3.6-dev #or what ever version of python you using
+        * python3.6-dev #or what ever version of python you use
         * torch and torchvision stable version (https://pytorch.org)
         * ffmpeg 4.4+
         
         #### How to install torch and fmpeg
         
         Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
         
@@ -36,34 +36,31 @@
         To install ffmpeg and python-dev
         
         ```
         sudo apt install ffmpeg python3.6-dev
         ```
         
         ### Installation
+        To Install backgroundremover, install it from pypi
         
-        To run code without installation:
+        ```bash
+        pip install --upgrade pip
+        pip install backgroundremover
+        ```
+        Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will pull them from this repo
         
+        It is also possible to run this without installing it via pip, just clone the git to local start a virtual env and install requirements and run
         ```bash
         python -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
         ```
         and for windows
         ```bash
         python.exe -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
         ```
-        ### Installation
-        
-        To Install backgroundremover, install it from pypi
-        
-        ```bash
-        pip install --upgrade pip
-        pip install backgroundremover
-        ```
-        Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will get them from u2net's google drive, as they say too [here](https://github.com/xuebinqin/U-2-Net#usage-for-salient-object-detection), and in this repo the code that pulls it is [here](https://github.com/nadermx/backgroundremover/blob/main/src/backgroundremover/utilities.py#L289)
-        # Usage as a cli
+        ### Usage as a cli
         ## Image
         
         Remove the background from a local file image
         
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -o "output.png"
         ```
@@ -71,15 +68,15 @@
         ### Advance usage for image background removal
         
         Sometimes it is possible to achieve better results by turning on alpha matting. Example:
         
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -a -ae 15 -o "output.png"
         ```
-        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
+        change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -m "u2net_human_seg" -o "output.png"
         ```
         ## Video
         
         ### remove background from video and make transparent mov
         
@@ -99,15 +96,15 @@
         
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -tg -o "output.gif"
         ```
         ### Make matte key file (green screen overlay)
         
-        Make a matte file for premier
+        Make a matte file for premiere
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -mk -o "output.matte.mp4"
         ```
         
         ### Advance usage for video
         
@@ -130,27 +127,27 @@
         ```
         
         Change the number of workers working on video (default is set to 1)
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
         ```
-        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
+        change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
         ```bash
         backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
         ```
         
         ## Todo
         
         - convert logic from video to image to utilize more GPU on image removal
         - clean up documentation a bit more
         - add ability to adjust and give feedback images or videos to datasets
         - add ability to realtime background removal for videos, for streaming
         - finish flask server api
-        - add ability to use other models than u2net, ie your own.
+        - add ability to use other models than u2net, ie your own
         - other
         
         ### Pull requests
         
         Accepted
         
         ### If you like this library
@@ -181,15 +178,16 @@
         ### License
         
         - Copyright (c) 2021-present [Johnathan Nader](https://github.com/nadermx)
         - Copyright (c) 2020-present [Lucas Nestler](https://github.com/ClashLuke)
         - Copyright (c) 2020-present [Dr. Tim Scarfe](https://github.com/ecsplendid)
         - Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
         
-        Licensed under [MIT License](./LICENSE.txt)
+        Code Licensed under [MIT License](./LICENSE.txt)
+        Models Licensed under [Apache License 2.0](./models/license)
         
 Keywords: remove,background,u2net,remove background,background remover
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

### Comparing `backgroundremover-0.2.1/README.md` & `backgroundremover-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # BackgroundRemover
-![Background Remover](/examplefiles/backgroundremoverexample.png)
-<img alt="background remover video" src="/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
-BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video), made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
+![Background Remover](https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverexample.png)
+<img alt="background remover video" src="https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
+BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video) using AI, made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
 
 
 ### Requirements
 
 * python >= 3.6
-* python3.6-dev #or what ever version of python you using
+* python3.6-dev #or what ever version of python you use
 * torch and torchvision stable version (https://pytorch.org)
 * ffmpeg 4.4+
 
 #### How to install torch and fmpeg
 
 Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
 
@@ -28,34 +28,31 @@
 To install ffmpeg and python-dev
 
 ```
 sudo apt install ffmpeg python3.6-dev
 ```
 
 ### Installation
+To Install backgroundremover, install it from pypi
 
-To run code without installation:
+```bash
+pip install --upgrade pip
+pip install backgroundremover
+```
+Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will pull them from this repo
 
+It is also possible to run this without installing it via pip, just clone the git to local start a virtual env and install requirements and run
 ```bash
 python -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
 ```
 and for windows
 ```bash
 python.exe -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
 ```
-### Installation
-
-To Install backgroundremover, install it from pypi
-
-```bash
-pip install --upgrade pip
-pip install backgroundremover
-```
-Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will get them from u2net's google drive, as they say too [here](https://github.com/xuebinqin/U-2-Net#usage-for-salient-object-detection), and in this repo the code that pulls it is [here](https://github.com/nadermx/backgroundremover/blob/main/src/backgroundremover/utilities.py#L289)
-# Usage as a cli
+### Usage as a cli
 ## Image
 
 Remove the background from a local file image
 
 ```bash
 backgroundremover -i "/path/to/image.jpeg" -o "output.png"
 ```
@@ -63,15 +60,15 @@
 ### Advance usage for image background removal
 
 Sometimes it is possible to achieve better results by turning on alpha matting. Example:
 
 ```bash
 backgroundremover -i "/path/to/image.jpeg" -a -ae 15 -o "output.png"
 ```
-change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
+change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
 ```bash
 backgroundremover -i "/path/to/image.jpeg" -m "u2net_human_seg" -o "output.png"
 ```
 ## Video
 
 ### remove background from video and make transparent mov
 
@@ -91,15 +88,15 @@
 
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -tg -o "output.gif"
 ```
 ### Make matte key file (green screen overlay)
 
-Make a matte file for premier
+Make a matte file for premiere
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -mk -o "output.matte.mp4"
 ```
 
 ### Advance usage for video
 
@@ -122,27 +119,27 @@
 ```
 
 Change the number of workers working on video (default is set to 1)
 
 ```bash
 backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
 ```
-change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
+change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
 ```bash
 backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
 ```
 
 ## Todo
 
 - convert logic from video to image to utilize more GPU on image removal
 - clean up documentation a bit more
 - add ability to adjust and give feedback images or videos to datasets
 - add ability to realtime background removal for videos, for streaming
 - finish flask server api
-- add ability to use other models than u2net, ie your own.
+- add ability to use other models than u2net, ie your own
 - other
 
 ### Pull requests
 
 Accepted
 
 ### If you like this library
@@ -173,8 +170,9 @@
 ### License
 
 - Copyright (c) 2021-present [Johnathan Nader](https://github.com/nadermx)
 - Copyright (c) 2020-present [Lucas Nestler](https://github.com/ClashLuke)
 - Copyright (c) 2020-present [Dr. Tim Scarfe](https://github.com/ecsplendid)
 - Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
 
-Licensed under [MIT License](./LICENSE.txt)
+Code Licensed under [MIT License](./LICENSE.txt)
+Models Licensed under [Apache License 2.0](./models/license)
```

### Comparing `backgroundremover-0.2.1/backgroundremover/bg.py` & `backgroundremover-0.2.2/backgroundremover/bg.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 import torch
 import torch.nn.functional
 import torch.nn.functional
 from hsh.library.hash import Hasher
 from .u2net import detect, u2net
 from . import utilities
 
-DEVICE = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-
+# closes https://github.com/nadermx/backgroundremover/issues/18
+if torch.cuda.is_available():
+    DEVICE = torch.device('cuda:0')
+elif torch.backends.mps.is_available():
+    DEVICE = torch.device('mps')
+else:
+    DEVICE = torch.device('cpu')
 
 class Net(torch.nn.Module):
     def __init__(self, model_name):
         super(Net, self).__init__()
         hasher = Hasher()
         model = {
             'u2netp': (u2net.U2NETP,
```

### Comparing `backgroundremover-0.2.1/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.2/backgroundremover/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/backgroundremover/cmd/server.py` & `backgroundremover-0.2.2/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.2/backgroundremover/u2net/data_loader.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.2/backgroundremover/u2net/detect.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.2/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/backgroundremover/utilities.py` & `backgroundremover-0.2.2/backgroundremover/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     print(F"FRAME RATE: {framerate} TOTAL FRAMES: {total_frames}")
 
     p = multiprocessing.Process(target=capture_frames,
                                 args=(file_path, frames_dict, gpu_batchsize * prefetched_batches, total_frames))
     p.start()
 
-    # note I am deliberatley not using pool
+    # note I am deliberately not using pool
     # we can't trust it to run all the threads concurrently (or at all)
     workers = [multiprocessing.Process(target=worker,
                                        args=(worker_nodes, wn, results_dict, model_name, gpu_batchsize, total_frames,
                                              frames_dict))
                for wn in range(worker_nodes)]
     for w in workers:
         w.start()
@@ -180,15 +180,15 @@
     matte_key(temp_file, file_path,
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
-    cmd = "nice -10 ffmpeg -y -i %s -i %s -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest %s" % (
+    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest '%s'" % (
         file_path, temp_file, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
 
     return
 
 
@@ -206,15 +206,15 @@
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -i %s -i %s -i %s -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[fg];[2][fg]overlay=(main_w-overlay_w)/2:(main_h-overlay_h)/2:format=auto,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest %s" % (
+    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[fg];[2][fg]overlay=(main_w-overlay_w)/2:(main_h-overlay_h)/2:format=auto,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest '%s'" % (
         file_path, temp_file, overlay, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
@@ -235,15 +235,15 @@
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -nostats -loglevel 0 -i %s -i %s -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1' -c:v qtrle -shortest %s" % (
+    cmd = "nice -10 ffmpeg -y -nostats -loglevel 0 -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1' -c:v qtrle -shortest '%s'" % (
         file_path, temp_file, output)
     process = sp.Popen(cmd, shell=True, stdout=sp.PIPE, stderr=sp.PIPE)
     stdout, stderr = process.communicate()
     print('after call')
 
     if stderr:
         return "ERROR: %s" % stderr.decode("utf-8")
@@ -269,15 +269,15 @@
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -i %s -i %s -i %s -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[vid];[vid][2:v]scale2ref[fg][bg];[bg][fg]overlay=shortest=1[out]' -map [out] -shortest %s" % (
+    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[vid];[vid][2:v]scale2ref[fg][bg];[bg][fg]overlay=shortest=1[out]' -map [out] -shortest '%s'" % (
         file_path, temp_file, overlay, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
@@ -299,19 +299,19 @@
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Scale image")
     temp_image = os.path.abspath("%s/new.jpg" % tmpdirname)
-    cmd = "nice -10 ffmpeg -i %s -i %s -filter_complex 'scale2ref[img][vid];[img]setsar=1;[vid]nullsink' -q:v 2 %s" % (
+    cmd = "nice -10 ffmpeg -i '%s' -i '%s' -filter_complex 'scale2ref[img][vid];[img]setsar=1;[vid]nullsink' -q:v 2 '%s'" % (
         overlay, file_path, temp_image)
     sp.run(shlex.split(cmd))
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -i %s -i %s -i %s -filter_complex '[0:v]scale2ref=oh*mdar:ih[bg];[1:v]scale2ref=oh*mdar:ih[fg];[bg][fg]overlay=(W-w)/2:(H-h)/2:shortest=1[out]' -map [out] -shortest %s" % (
+    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[0:v]scale2ref=oh*mdar:ih[bg];[1:v]scale2ref=oh*mdar:ih[fg];[bg][fg]overlay=(W-w)/2:(H-h)/2:shortest=1[out]' -map [out] -shortest '%s'" % (
         temp_image, file_path, temp_file, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
```

### Comparing `backgroundremover-0.2.1/backgroundremover.egg-info/PKG-INFO` & `backgroundremover-0.2.2/backgroundremover.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.1
-Summary: Background remover from image and video
+Version: 0.2.2
+Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
-        ![Background Remover](/examplefiles/backgroundremoverexample.png)
-        <img alt="background remover video" src="/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
-        BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video), made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
+        ![Background Remover](https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverexample.png)
+        <img alt="background remover video" src="https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverprocessed.gif" height="200" /><br>
+        BackgroundRemover is a command line tool to remove background from [image](https://github.com/nadermx/backgroundremover#image) and [video](https://github.com/nadermx/backgroundremover#video) using AI, made by [nadermx](https://john.nader.mx) to power [https://BackgroundRemoverAI.com](https://backgroundremoverai.com). If you wonder why it was made read this [short blog post](https://johnathannader.com/my-first-open-source-project/).<br>
         
         
         ### Requirements
         
         * python >= 3.6
-        * python3.6-dev #or what ever version of python you using
+        * python3.6-dev #or what ever version of python you use
         * torch and torchvision stable version (https://pytorch.org)
         * ffmpeg 4.4+
         
         #### How to install torch and fmpeg
         
         Go to https://pytorch.org and scroll down to `INSTALL PYTORCH` section and follow the instructions.
         
@@ -36,34 +36,31 @@
         To install ffmpeg and python-dev
         
         ```
         sudo apt install ffmpeg python3.6-dev
         ```
         
         ### Installation
+        To Install backgroundremover, install it from pypi
         
-        To run code without installation:
+        ```bash
+        pip install --upgrade pip
+        pip install backgroundremover
+        ```
+        Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will pull them from this repo
         
+        It is also possible to run this without installing it via pip, just clone the git to local start a virtual env and install requirements and run
         ```bash
         python -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
         ```
         and for windows
         ```bash
         python.exe -m backgroundremover.cmd.cli -i "video.mp4" -mk -o "output.mov"
         ```
-        ### Installation
-        
-        To Install backgroundremover, install it from pypi
-        
-        ```bash
-        pip install --upgrade pip
-        pip install backgroundremover
-        ```
-        Please note that when you first run the program, it will check to see if you have the u2net models, if you do not, it will get them from u2net's google drive, as they say too [here](https://github.com/xuebinqin/U-2-Net#usage-for-salient-object-detection), and in this repo the code that pulls it is [here](https://github.com/nadermx/backgroundremover/blob/main/src/backgroundremover/utilities.py#L289)
-        # Usage as a cli
+        ### Usage as a cli
         ## Image
         
         Remove the background from a local file image
         
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -o "output.png"
         ```
@@ -71,15 +68,15 @@
         ### Advance usage for image background removal
         
         Sometimes it is possible to achieve better results by turning on alpha matting. Example:
         
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -a -ae 15 -o "output.png"
         ```
-        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
+        change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg`
         ```bash
         backgroundremover -i "/path/to/image.jpeg" -m "u2net_human_seg" -o "output.png"
         ```
         ## Video
         
         ### remove background from video and make transparent mov
         
@@ -99,15 +96,15 @@
         
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -tg -o "output.gif"
         ```
         ### Make matte key file (green screen overlay)
         
-        Make a matte file for premier
+        Make a matte file for premiere
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -mk -o "output.matte.mp4"
         ```
         
         ### Advance usage for video
         
@@ -130,27 +127,27 @@
         ```
         
         Change the number of workers working on video (default is set to 1)
         
         ```bash
         backgroundremover -i "/path/to/video.mp4" -wn 4 -tv -o "output.mov"
         ```
-        change the model for diferent background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
+        change the model for different background removal methods between `u2netp`, `u2net`, or `u2net_human_seg` and limit the frames to 150
         ```bash
         backgroundremover -i "/path/to/video.mp4" -m "u2net_human_seg" -fl 150 -tv -o "output.mov"
         ```
         
         ## Todo
         
         - convert logic from video to image to utilize more GPU on image removal
         - clean up documentation a bit more
         - add ability to adjust and give feedback images or videos to datasets
         - add ability to realtime background removal for videos, for streaming
         - finish flask server api
-        - add ability to use other models than u2net, ie your own.
+        - add ability to use other models than u2net, ie your own
         - other
         
         ### Pull requests
         
         Accepted
         
         ### If you like this library
@@ -181,15 +178,16 @@
         ### License
         
         - Copyright (c) 2021-present [Johnathan Nader](https://github.com/nadermx)
         - Copyright (c) 2020-present [Lucas Nestler](https://github.com/ClashLuke)
         - Copyright (c) 2020-present [Dr. Tim Scarfe](https://github.com/ecsplendid)
         - Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
         
-        Licensed under [MIT License](./LICENSE.txt)
+        Code Licensed under [MIT License](./LICENSE.txt)
+        Models Licensed under [Apache License 2.0](./models/license)
         
 Keywords: remove,background,u2net,remove background,background remover
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

### Comparing `backgroundremover-0.2.1/backgroundremover.egg-info/SOURCES.txt` & `backgroundremover-0.2.2/backgroundremover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.1/setup.py` & `backgroundremover-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.2.1",
-    description="Background remover from image and video",
+    version="0.2.2",
+    description="Background remover from image and video using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

