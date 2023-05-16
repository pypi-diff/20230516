# Comparing `tmp/bgrm-8.tar.gz` & `tmp/bgrm-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgrm-8.tar", max compression
+gzip compressed data, was "bgrm-9.tar", max compression
```

## Comparing `bgrm-8.tar` & `bgrm-9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-11-11 19:21:59.408119 bgrm-8/LICENSE
--rw-r--r--   0        0        0     1582 2022-11-11 21:14:13.403195 bgrm-8/README.md
--rw-r--r--   0        0        0       66 2022-11-11 21:05:47.781506 bgrm-8/bgrm/__main__.py
--rwxr-xr-x   0        0        0      592 2022-11-11 21:05:47.781506 bgrm-8/bgrm/bgrm.py
--rw-r--r--   0        0        0     3769 2022-11-11 21:30:14.755363 bgrm-8/bgrm/cam.py
--rw-r--r--   0        0        0     2861 2022-11-11 21:05:47.781506 bgrm-8/bgrm/settings.py
--rw-r--r--   0        0        0     1340 2022-11-11 21:05:47.781506 bgrm-8/bgrm/virt_cam.py
--rw-r--r--   0        0        0      659 2022-11-11 21:30:57.547503 bgrm-8/pyproject.toml
--rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 bgrm-8/setup.py
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 bgrm-8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-11 19:21:59.408119 bgrm-9/LICENSE
+-rw-r--r--   0        0        0     1983 2022-11-11 22:50:40.184081 bgrm-9/README.md
+-rw-r--r--   0        0        0       66 2022-11-11 21:05:47.781506 bgrm-9/bgrm/__main__.py
+-rwxr-xr-x   0        0        0     1075 2022-11-11 22:50:40.184081 bgrm-9/bgrm/bgrm.py
+-rw-r--r--   0        0        0     3844 2022-11-11 22:50:40.184081 bgrm-9/bgrm/cam.py
+-rw-r--r--   0        0        0     3669 2022-11-11 22:50:40.184081 bgrm-9/bgrm/settings.py
+-rw-r--r--   0        0        0     1432 2022-11-11 22:50:40.184081 bgrm-9/bgrm/vid_file.py
+-rw-r--r--   0        0        0     1340 2022-11-11 21:05:47.781506 bgrm-9/bgrm/virt_cam.py
+-rw-r--r--   0        0        0      659 2022-11-11 22:50:40.184081 bgrm-9/pyproject.toml
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 bgrm-9/setup.py
+-rw-r--r--   0        0        0     2934 1970-01-01 00:00:00.000000 bgrm-9/PKG-INFO
```

### Comparing `bgrm-8/LICENSE` & `bgrm-9/LICENSE`

 * *Files identical despite different names*

### Comparing `bgrm-8/README.md` & `bgrm-9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 
 Well, I'm an engineer, so of course, I found a solution.
 
 Using OpenCV and a v4l2loopback device (basically a virtual webcam you can write data to), I threw together a Python application that takes your normal webcam input, removes and replaces the background, and outputs that to the created video device. Problem solved :)
 
 Note, this will work anywhere WebCams are used, not just Teams
 
+Now, the program can also be used to remove backgrounds from video files and save them as video files as well!
+
 ## How to Use
 
+### WebCam Replacement
+
 Dependencies:
     - python >= 3.8 (3.10 is what's supported officially)
     - pip
     - v4l2loopback
 
 Setup:
 1. Configure v4l2loopback (may not be necessary):
@@ -28,14 +32,20 @@
     ```
 2. Install with `pip install bgrm`
 
 Then, you can run: 
 - Run with `python -m bgrm <options>` (use `--help` to see all options)
 - Example: `python -m bgrm -b ~/Pictures/Wallpapers/ni-skyline-wallpaper.png -w 320 -H 240 -s 2.0`
 
+### File Replacement
+
+You can also remove the background from video files. It works just like the WebCam, but instead of setting the `--camera` cli arg, you call the program like this:
+
+`python -m bgrm --file_mode -i <input file> -o <output file> <other options>`
+
 ## Build from Repo
 
 You can also build the package yourself from source (or grab the latest version from the releases tab)
 
 To do that you need the "poetry" build system.
 
 Run `poetry build` and install the whl from the dist/ folder
```

### Comparing `bgrm-8/bgrm/cam.py` & `bgrm-9/bgrm/cam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Author: Dylan Turner
 # Description: Handle OpenCV processing of images
 
 from cv2 import \
     VideoCapture, resize, namedWindow, moveWindow, imshow, waitKey, \
     destroyAllWindows, imread, BORDER_CONSTANT, copyMakeBorder, resize, imread, \
     GaussianBlur
-from numpy import shape
+from numpy import shape, uint8
 from cvzone import stackImages
 from cvzone.SelfiSegmentationModule import SelfiSegmentation
 from time import sleep
 
 WIN_TITLE = 'Feed'
 
 class Cam:
     def __init__(self, settings):
         # Set up WebCam access and output
         self._settings = settings
 
-        self._vidFeed = VideoCapture(settings.camera)
-        self._vidFeed.set(3, settings.screen_width)
-        self._vidFeed.set(4, settings.screen_height)
+        self._vid_feed = VideoCapture(settings.camera)
+        self._vid_feed.set(3, settings.screen_width)
+        self._vid_feed.set(4, settings.screen_height)
 
-        _success, baseFrame = self._vidFeed.read()
+        _success, baseFrame = self._vid_feed.read()
         if not _success:
             print('Failed to read from camera!')
             quit()
         _height, _width, self.channels = baseFrame.shape
 
         if not settings.disable_win:
             namedWindow(WIN_TITLE)
@@ -38,20 +38,23 @@
         else:
             self._bg_img = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        self._vidFeed.release()
+        self._vid_feed.release()
         destroyAllWindows()
 
     # Return regular camera frame and with the bg removal applied, as well as them put together
     def frames(self):
-        _success, frame = self._vidFeed.read()
+        success, frame = self._vid_feed.read()
+
+        if not success:
+            return (None, None, None)
 
         if shape(self._bg_img) == ():
             no_bg_frame = self._segmentor.removeBG(
                 frame, self._settings.fill_color,
                 threshold = self._settings.rm_thresh
             )
         else:
```

### Comparing `bgrm-8/bgrm/settings.py` & `bgrm-9/bgrm/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     screen_height: int
     view_scale: float
     rm_thresh: float
     fill_color: tuple[float, float, float]
     bg_img: str
     blur: bool
     disable_win: bool
+    file_mode: bool
+    input_file: str
+    output_file: str
+    fps: int
 
     @staticmethod
     def from_cli():
         virt_dev = pull_virt_dev()
         args = cli_args()
 
         # Convert fill color from string to tuple
@@ -28,15 +32,16 @@
         if len(fill_col) != 3:
             print('Failed to parse fill color argument \'' + args.color + '\'')
             raise SettingsError
         fill_col = tuple([ float(e) for e in fill_col ])
 
         return AppSettings(
             virt_dev, args.camera, args.width, args.height, args.scale,
-            args.thresh, fill_col, args.bg, args.blur, args.disable_window
+            args.thresh, fill_col, args.bg, args.blur, args.disable_window,
+            args.file_mode, args.input, args.output, args.fps
         )
 
 # Get video settings from command line
 def pull_virt_dev():
     shell_result = run(
         [ 'ls', '/sys/devices/virtual/video4linux' ],
         stderr = PIPE, stdout = PIPE, text = True
@@ -87,14 +92,33 @@
         action = 'store_true'
     )
     parser.add_argument(
         '-C', '--color', type = str, default = '0,0,0',
         help = 'List of R, G, B to replace background with',
     )
 
+    # File versions
+    parser.add_argument(
+        '--file_mode',
+        help = 'Remove the background from video files instead of cameras (overrides --camera)',
+        action = 'store_true'
+    )
+    parser.add_argument(
+        '-i', '--input', type = str, default = '',
+        help = 'Only used with file mode. Input file to remove background',
+    )
+    parser.add_argument(
+        '-o', '--output', type = str, default = '',
+        help = 'Only used with file mode. Output file to store removed background feed.'
+    )
+    parser.add_argument(
+        '-f', '--fps', type = int, default = 30,
+        help = 'Only used with file mode. Output file fps'
+    )
+
     # Mostly useless window options
     parser.add_argument(
         '-s', '--scale', type = float, default = 0.5,
         help = 'Scale factor from camera size to window.'
     )
 
     return parser.parse_args()
```

### Comparing `bgrm-8/bgrm/virt_cam.py` & `bgrm-9/bgrm/virt_cam.py`

 * *Files identical despite different names*

### Comparing `bgrm-8/pyproject.toml` & `bgrm-9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bgrm"
-version = "8"
+version = "9"
 description = "Remove backgrounds from video feeds in your web cam applications."
 authors = [ "Dylan Turner <dylantdmt@gmail.com>" ]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/blueOkiris/bgrm"
 repository = "https://github.com/blueOkiris/bgrm"
 keywords = [ "bgrm", "background", "removal", "teams", "linux", "mediapipe", "opencv", "bg", "rm" ]
```

### Comparing `bgrm-8/setup.py` & `bgrm-9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'mediapipe==0.8.11',
  'opencv-python==4.6.0.66',
  'protobuf==3.19.0',
  'v4l2-python3==0.3.1']
 
 setup_kwargs = {
     'name': 'bgrm',
-    'version': '8',
+    'version': '9',
     'description': 'Remove backgrounds from video feeds in your web cam applications.',
-    'long_description': '# Background Remover\n\n## The Need\n\nIt\'s been good long while since Microsoft first released a Teams version for Linux and yet, one of Teams\' coolest features doesn\'t exist in said Linux version: removable backgrounds. As someone who uses Linux for their daily driver, this annoys me.\n\nWell, I\'m an engineer, so of course, I found a solution.\n\nUsing OpenCV and a v4l2loopback device (basically a virtual webcam you can write data to), I threw together a Python application that takes your normal webcam input, removes and replaces the background, and outputs that to the created video device. Problem solved :)\n\nNote, this will work anywhere WebCams are used, not just Teams\n\n## How to Use\n\nDependencies:\n    - python >= 3.8 (3.10 is what\'s supported officially)\n    - pip\n    - v4l2loopback\n\nSetup:\n1. Configure v4l2loopback (may not be necessary):\n    - Recommended something like this:\n    ```\n    export DEVICE_ARR=(`ls /sys/devices/virtual/video4linux | tr -d \'video\'`); \\\n    sudo modprobe v4l2loopback \\\n        devices=1 exclusive_caps=1 video_nr=${DEVICE_ARR[1]} max_buffers=2 \\\n        card_label=v4l2lo\n    ```\n2. Install with `pip install bgrm`\n\nThen, you can run: \n- Run with `python -m bgrm <options>` (use `--help` to see all options)\n- Example: `python -m bgrm -b ~/Pictures/Wallpapers/ni-skyline-wallpaper.png -w 320 -H 240 -s 2.0`\n\n## Build from Repo\n\nYou can also build the package yourself from source (or grab the latest version from the releases tab)\n\nTo do that you need the "poetry" build system.\n\nRun `poetry build` and install the whl from the dist/ folder\n',
+    'long_description': '# Background Remover\n\n## The Need\n\nIt\'s been good long while since Microsoft first released a Teams version for Linux and yet, one of Teams\' coolest features doesn\'t exist in said Linux version: removable backgrounds. As someone who uses Linux for their daily driver, this annoys me.\n\nWell, I\'m an engineer, so of course, I found a solution.\n\nUsing OpenCV and a v4l2loopback device (basically a virtual webcam you can write data to), I threw together a Python application that takes your normal webcam input, removes and replaces the background, and outputs that to the created video device. Problem solved :)\n\nNote, this will work anywhere WebCams are used, not just Teams\n\nNow, the program can also be used to remove backgrounds from video files and save them as video files as well!\n\n## How to Use\n\n### WebCam Replacement\n\nDependencies:\n    - python >= 3.8 (3.10 is what\'s supported officially)\n    - pip\n    - v4l2loopback\n\nSetup:\n1. Configure v4l2loopback (may not be necessary):\n    - Recommended something like this:\n    ```\n    export DEVICE_ARR=(`ls /sys/devices/virtual/video4linux | tr -d \'video\'`); \\\n    sudo modprobe v4l2loopback \\\n        devices=1 exclusive_caps=1 video_nr=${DEVICE_ARR[1]} max_buffers=2 \\\n        card_label=v4l2lo\n    ```\n2. Install with `pip install bgrm`\n\nThen, you can run: \n- Run with `python -m bgrm <options>` (use `--help` to see all options)\n- Example: `python -m bgrm -b ~/Pictures/Wallpapers/ni-skyline-wallpaper.png -w 320 -H 240 -s 2.0`\n\n### File Replacement\n\nYou can also remove the background from video files. It works just like the WebCam, but instead of setting the `--camera` cli arg, you call the program like this:\n\n`python -m bgrm --file_mode -i <input file> -o <output file> <other options>`\n\n## Build from Repo\n\nYou can also build the package yourself from source (or grab the latest version from the releases tab)\n\nTo do that you need the "poetry" build system.\n\nRun `poetry build` and install the whl from the dist/ folder\n',
     'author': 'Dylan Turner',
     'author_email': 'dylantdmt@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/blueOkiris/bgrm',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bgrm-8/PKG-INFO` & `bgrm-9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgrm
-Version: 8
+Version: 9
 Summary: Remove backgrounds from video feeds in your web cam applications.
 Home-page: https://github.com/blueOkiris/bgrm
 License: GPL-3.0-only
 Keywords: bgrm,background,removal,teams,linux,mediapipe,opencv,bg,rm
 Author: Dylan Turner
 Author-email: dylantdmt@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -30,16 +30,20 @@
 
 Well, I'm an engineer, so of course, I found a solution.
 
 Using OpenCV and a v4l2loopback device (basically a virtual webcam you can write data to), I threw together a Python application that takes your normal webcam input, removes and replaces the background, and outputs that to the created video device. Problem solved :)
 
 Note, this will work anywhere WebCams are used, not just Teams
 
+Now, the program can also be used to remove backgrounds from video files and save them as video files as well!
+
 ## How to Use
 
+### WebCam Replacement
+
 Dependencies:
     - python >= 3.8 (3.10 is what's supported officially)
     - pip
     - v4l2loopback
 
 Setup:
 1. Configure v4l2loopback (may not be necessary):
@@ -52,14 +56,20 @@
     ```
 2. Install with `pip install bgrm`
 
 Then, you can run: 
 - Run with `python -m bgrm <options>` (use `--help` to see all options)
 - Example: `python -m bgrm -b ~/Pictures/Wallpapers/ni-skyline-wallpaper.png -w 320 -H 240 -s 2.0`
 
+### File Replacement
+
+You can also remove the background from video files. It works just like the WebCam, but instead of setting the `--camera` cli arg, you call the program like this:
+
+`python -m bgrm --file_mode -i <input file> -o <output file> <other options>`
+
 ## Build from Repo
 
 You can also build the package yourself from source (or grab the latest version from the releases tab)
 
 To do that you need the "poetry" build system.
 
 Run `poetry build` and install the whl from the dist/ folder
```

