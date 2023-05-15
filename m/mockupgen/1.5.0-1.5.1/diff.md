# Comparing `tmp/mockupgen-1.5.0.tar.gz` & `tmp/mockupgen-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockupgen-1.5.0.tar", last modified: Sun May 14 00:35:22 2023, max compression
+gzip compressed data, was "mockupgen-1.5.1.tar", last modified: Mon May 15 21:57:21 2023, max compression
```

## Comparing `mockupgen-1.5.0.tar` & `mockupgen-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:35:22.533907 mockupgen-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-14 00:35:05.000000 mockupgen-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-14 00:35:22.533907 mockupgen-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-14 00:35:05.000000 mockupgen-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:35:22.529906 mockupgen-1.5.0/mockupgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 00:35:05.000000 mockupgen-1.5.0/mockupgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-14 00:35:05.000000 mockupgen-1.5.0/mockupgen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-14 00:35:05.000000 mockupgen-1.5.0/mockupgen/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-14 00:35:05.000000 mockupgen-1.5.0/mockupgen/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-05-14 00:35:05.000000 mockupgen-1.5.0/mockupgen/mockupgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 00:35:22.533907 mockupgen-1.5.0/mockupgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-14 00:35:22.000000 mockupgen-1.5.0/mockupgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-14 00:35:22.000000 mockupgen-1.5.0/mockupgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 00:35:22.000000 mockupgen-1.5.0/mockupgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 00:35:22.000000 mockupgen-1.5.0/mockupgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-14 00:35:22.000000 mockupgen-1.5.0/mockupgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 00:35:22.000000 mockupgen-1.5.0/mockupgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-14 00:35:05.000000 mockupgen-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-14 00:35:22.533907 mockupgen-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-14 00:35:05.000000 mockupgen-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:21.628849 mockupgen-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-15 21:57:08.000000 mockupgen-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-15 21:57:21.628849 mockupgen-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-15 21:57:08.000000 mockupgen-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:21.628849 mockupgen-1.5.1/mockupgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:08.000000 mockupgen-1.5.1/mockupgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 21:57:08.000000 mockupgen-1.5.1/mockupgen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-15 21:57:08.000000 mockupgen-1.5.1/mockupgen/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-15 21:57:08.000000 mockupgen-1.5.1/mockupgen/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-15 21:57:08.000000 mockupgen-1.5.1/mockupgen/mockupgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:21.628849 mockupgen-1.5.1/mockupgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-15 21:57:21.000000 mockupgen-1.5.1/mockupgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 21:57:21.000000 mockupgen-1.5.1/mockupgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:57:21.000000 mockupgen-1.5.1/mockupgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 21:57:21.000000 mockupgen-1.5.1/mockupgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 21:57:21.000000 mockupgen-1.5.1/mockupgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 21:57:21.000000 mockupgen-1.5.1/mockupgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 21:57:08.000000 mockupgen-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-15 21:57:21.628849 mockupgen-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 21:57:08.000000 mockupgen-1.5.1/setup.py
```

### Comparing `mockupgen-1.5.0/LICENSE.md` & `mockupgen-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mockupgen-1.5.0/PKG-INFO` & `mockupgen-1.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: mockupgen
-Version: 1.5.0
-Summary: A tool that generates a 3D device mockup from a screenshot.
-Home-page: https://github.com/rmenon1008/mockupgen
-Author: Rohan Menon
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # mockupgen
 A tool that generates a 3D device mockup from a screenshot.
 
 <br>
 
 ![](https://www.rohanmenon.com/media/example.png)
 
@@ -68,14 +59,16 @@
 
             // Only one of the two options below must be specified
             "mask_file": "mask.png",  // An image used to mask the screenshot (alpha channel used)
             // OR
             "mask_aspect_ratio": 1.0, // Aspect ratio to mask the screenshot (assumes rectangular)
 
             // Optional fields
+            "black_white_point": ["292826", "D9DCDD"], // Black and white points
+                                                       // for color correction
             "brightness": 1.0,        // Brightness adjustment of the screenshot
             "contrast": 1.0           // Contrast adjustment of the screenshot
         },
         ...
     ]
 }
 ```
```

### Comparing `mockupgen-1.5.0/mockupgen/helpers.py` & `mockupgen-1.5.1/mockupgen/helpers.py`

 * *Files identical despite different names*

### Comparing `mockupgen-1.5.0/mockupgen/image_processing.py` & `mockupgen-1.5.1/mockupgen/image_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,33 @@
         int(center[1] - crop_height / 2):int(center[1] + crop_height / 2),
         int(center[0] - crop_width / 2):int(center[0] + crop_width / 2)
     ]
 
     return image
 
 
+def _adjust_image(image, black_point, white_point):
+    a = image[:,:,3]
+    image = image[:,:,0:3]
+
+    # The white point and black point are hex strings, so convert them to RGB
+    white_point = tuple(int(white_point[i:i+2], 16) for i in (4, 2, 0))
+    black_point = tuple(int(black_point[i:i+2], 16) for i in (4, 2, 0))
+
+    # Scale and offset colors so that each color goes from black_point to white_point
+    scale = (np.array(white_point) - np.array(black_point)) / 255.0
+    offset = np.array(black_point)
+
+    # Apply the scale and offset
+    image = np.clip(image * scale + offset, 0, 255).astype(np.uint8)
+    image = np.dstack((image, a))
+
+    return image
+
+
 def _read_image(image_path_or_url, fmt=cv2.IMREAD_UNCHANGED):
     if image_path_or_url.startswith('http'):
         try:
             resp = urllib.request.urlopen(image_path_or_url)
             image = np.asarray(bytearray(resp.read()), dtype="uint8")
             image = cv2.imdecode(image, fmt)
         except urllib.error.HTTPError:
@@ -73,15 +92,17 @@
     for color in range(0, 3):
         background[:,:,color] = alpha_foreground * foreground[:,:,color] + background[:,:,color] * (1 - alpha_foreground)
     return background
 
 
 def _warn_for_different_aspect_ratios(ar1, ar2):
     if ar1 / ar2 > 1.1 or ar2 / ar1 > 1.1:
-        print(_r(f'Warning: The screenshot was stretched significantly to fit the template. Use --crop to crop the screenshot instead.'))
+        print(_r(f'Warning: The screenshot was stretched significantly to fit the template.)'))
+        print(_r( "         Use --crop to crop the screenshot instead."))
+        print()
 
 
 def _mask_image(image, mask):
     # Set the alpha channel of the image to the alpha channel of the mask
     image[:,:,3] = mask[:,:,3]
     return image
 
@@ -155,14 +176,16 @@
         mockup_img = cv2.resize(mockup_img, (0, 0), fx=mockup_upscale_factor, fy=mockup_upscale_factor, interpolation=cv2.INTER_CUBIC)
 
     # Always upscale by 4 to improve the quality after the perspective warp 
     mockup_img = cv2.resize(mockup_img, (0, 0), fx=4, fy=4, interpolation=cv2.INTER_CUBIC)
     mockup_upscale_factor *= 4
 
     # Adjust the screenshot based on the mockup options
+    if "black_white_point" in mockup:
+        screenshot = _adjust_image(screenshot, mockup['black_white_point'][0], mockup['black_white_point'][1])
     if "contrast" in mockup:
         screenshot = _contrast(screenshot, mockup['contrast'])
     if "brightness" in mockup:
         screenshot = _brightness(screenshot, mockup['brightness'])
     
     # Now adjust the screenshot based on the CLI options
     if contrast:
@@ -227,20 +250,16 @@
 
     matrix = cv2.getPerspectiveTransform(screenshot_points, mockup_points)
 
     warped_screenshot = cv2.warpPerspective(
         masked_screenshot,
         matrix,
         (mockup_img.shape[1], mockup_img.shape[0]),
-        borderMode=cv2.BORDER_TRANSPARENT
+        flags=cv2.INTER_NEAREST
     )
-    
-    # Blur the screenshot slightly
-    warped_screenshot = cv2.blur(warped_screenshot, (2, 2))
-
 
 
     ### STEP 5: Composite the screenshot onto the mockup and resize
     
     # Composite
     mockup_img = _over_composite(mockup_img, warped_screenshot)
```

### Comparing `mockupgen-1.5.0/mockupgen/mockupgen.py` & `mockupgen-1.5.1/mockupgen/mockupgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     # Accept a template URL or path
     if args.custom_templates:
         template_list, template_version, template_dir = get_template_index(args.custom_templates)
         print(f'Using custom template directory: {_b(args.custom_templates)} (version {_b(template_version)})')
     else:
         template_list, template_version, template_dir = get_template_index(DEFAULT_TEMPLATE_DIR)
-        print(f'Template index version {_b(template_version)}')
+        print(f'Using {_b("mockupgen-templates")} (version {_b(template_version)})')
 
     # List the templates if requested
     if args.list:
         print_template_list(template_list)
         exit(0)
 
     # Ensure the screenshot exists
```

### Comparing `mockupgen-1.5.0/mockupgen.egg-info/PKG-INFO` & `mockupgen-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockupgen
-Version: 1.5.0
+Version: 1.5.1
 Summary: A tool that generates a 3D device mockup from a screenshot.
 Home-page: https://github.com/rmenon1008/mockupgen
 Author: Rohan Menon
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # mockupgen
@@ -68,14 +68,16 @@
 
             // Only one of the two options below must be specified
             "mask_file": "mask.png",  // An image used to mask the screenshot (alpha channel used)
             // OR
             "mask_aspect_ratio": 1.0, // Aspect ratio to mask the screenshot (assumes rectangular)
 
             // Optional fields
+            "black_white_point": ["292826", "D9DCDD"], // Black and white points
+                                                       // for color correction
             "brightness": 1.0,        // Brightness adjustment of the screenshot
             "contrast": 1.0           // Contrast adjustment of the screenshot
         },
         ...
     ]
 }
 ```
```

