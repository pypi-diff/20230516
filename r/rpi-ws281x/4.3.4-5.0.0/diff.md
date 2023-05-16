# Comparing `tmp/rpi_ws281x-4.3.4.tar.gz` & `tmp/rpi_ws281x-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_ws281x-4.3.4.tar", last modified: Mon Apr 11 13:30:08 2022, max compression
+gzip compressed data, was "rpi_ws281x-5.0.0.tar", last modified: Tue May 16 12:03:34 2023, max compression
```

## Comparing `rpi_ws281x-4.3.4.tar` & `rpi_ws281x-5.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-04-11 13:30:08.900964 rpi_ws281x-4.3.4/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1832 2022-04-11 13:27:32.000000 rpi_ws281x-4.3.4/CHANGELOG.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1290 2022-04-11 13:19:09.000000 rpi_ws281x-4.3.4/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)      211 2022-04-11 13:19:09.000000 rpi_ws281x-4.3.4/MANIFEST.in
--rw-rw-r--   0 phil      (1000) phil      (1000)    10161 2022-04-11 13:30:08.896964 rpi_ws281x-4.3.4/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     5798 2022-04-11 13:19:09.000000 rpi_ws281x-4.3.4/README.rst
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-04-11 13:30:08.896964 rpi_ws281x-4.3.4/lib/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1290 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3048 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/clk.h
--rw-rw-r--   0 phil      (1000) phil      (1000)     2362 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/dma.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     5633 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/dma.h
--rw-rw-r--   0 phil      (1000) phil      (1000)     4177 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/gpio.h
--rw-rw-r--   0 phil      (1000) phil      (1000)     7422 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/mailbox.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     2437 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/mailbox.h
--rw-rw-r--   0 phil      (1000) phil      (1000)    10101 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/main.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     3400 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/pcm.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     6929 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/pcm.h
--rw-rw-r--   0 phil      (1000) phil      (1000)     2856 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/pwm.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     4468 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/pwm.h
--rw-rw-r--   0 phil      (1000) phil      (1000)    15860 2022-04-11 13:20:38.000000 rpi_ws281x-4.3.4/lib/rpihw.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     2080 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/rpihw.h
--rw-rw-r--   0 phil      (1000) phil      (1000)    37448 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/ws2811.c
--rw-rw-r--   0 phil      (1000) phil      (1000)     7013 2022-04-11 13:20:27.000000 rpi_ws281x-4.3.4/lib/ws2811.h
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-04-11 13:30:08.896964 rpi_ws281x-4.3.4/rpi_ws281x/
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2022-04-11 13:27:57.000000 rpi_ws281x-4.3.4/rpi_ws281x/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     7438 2022-04-11 13:19:09.000000 rpi_ws281x-4.3.4/rpi_ws281x/rpi_ws281x.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2022-04-11 13:30:08.896964 rpi_ws281x-4.3.4/rpi_ws281x.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)    10161 2022-04-11 13:30:08.000000 rpi_ws281x-4.3.4/rpi_ws281x.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      447 2022-04-11 13:30:08.000000 rpi_ws281x-4.3.4/rpi_ws281x.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2022-04-11 13:30:08.000000 rpi_ws281x-4.3.4/rpi_ws281x.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       23 2022-04-11 13:30:08.000000 rpi_ws281x-4.3.4/rpi_ws281x.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)   170377 2022-04-11 13:19:09.000000 rpi_ws281x-4.3.4/rpi_ws281x_wrap.c
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2022-04-11 13:30:08.900964 rpi_ws281x-4.3.4/setup.cfg
--rwxrwxr-x   0 phil      (1000) phil      (1000)     1627 2022-04-11 13:27:41.000000 rpi_ws281x-4.3.4/setup.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      145 2022-04-11 13:19:09.000000 rpi_ws281x-4.3.4/version.h
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-16 12:03:34.830864 rpi_ws281x-5.0.0/
+-rw-r--r--   0 phil      (1000) phil      (1000)     2257 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/CHANGELOG.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)     1290 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)      211 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/MANIFEST.in
+-rw-r--r--   0 phil      (1000) phil      (1000)    11029 2023-05-16 12:03:34.830864 rpi_ws281x-5.0.0/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)     5798 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/README.rst
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-16 12:03:34.826864 rpi_ws281x-5.0.0/lib/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1290 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     3048 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/clk.h
+-rw-r--r--   0 phil      (1000) phil      (1000)     2362 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/dma.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     5633 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/dma.h
+-rw-r--r--   0 phil      (1000) phil      (1000)     4177 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/gpio.h
+-rw-r--r--   0 phil      (1000) phil      (1000)     7422 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/mailbox.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     2437 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/mailbox.h
+-rw-r--r--   0 phil      (1000) phil      (1000)    10101 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/main.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     3400 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/pcm.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     6929 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/pcm.h
+-rw-r--r--   0 phil      (1000) phil      (1000)     2856 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/pwm.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     4468 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/pwm.h
+-rw-r--r--   0 phil      (1000) phil      (1000)    17212 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/rpihw.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     2080 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/rpihw.h
+-rw-r--r--   0 phil      (1000) phil      (1000)    40200 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/ws2811.c
+-rw-r--r--   0 phil      (1000) phil      (1000)     7013 2023-05-16 12:02:29.000000 rpi_ws281x-5.0.0/lib/ws2811.h
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-16 12:03:34.830864 rpi_ws281x-5.0.0/rpi_ws281x/
+-rw-r--r--   0 phil      (1000) phil      (1000)      176 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/rpi_ws281x/__init__.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     7148 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/rpi_ws281x/rpi_ws281x.py
+drwxr-xr-x   0 phil      (1000) phil      (1000)        0 2023-05-16 12:03:34.830864 rpi_ws281x-5.0.0/rpi_ws281x.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)    11029 2023-05-16 12:03:34.000000 rpi_ws281x-5.0.0/rpi_ws281x.egg-info/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)      447 2023-05-16 12:03:34.000000 rpi_ws281x-5.0.0/rpi_ws281x.egg-info/SOURCES.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        1 2023-05-16 12:03:34.000000 rpi_ws281x-5.0.0/rpi_ws281x.egg-info/dependency_links.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       23 2023-05-16 12:03:34.000000 rpi_ws281x-5.0.0/rpi_ws281x.egg-info/top_level.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)   168837 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/rpi_ws281x_wrap.c
+-rw-r--r--   0 phil      (1000) phil      (1000)       38 2023-05-16 12:03:34.830864 rpi_ws281x-5.0.0/setup.cfg
+-rwxr-xr-x   0 phil      (1000) phil      (1000)     2061 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/setup.py
+-rw-r--r--   0 phil      (1000) phil      (1000)      145 2023-05-16 12:01:55.000000 rpi_ws281x-5.0.0/version.h
```

### Comparing `rpi_ws281x-4.3.4/CHANGELOG.txt` & `rpi_ws281x-5.0.0/CHANGELOG.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,20 @@
+5.0.0
+-----
+
+* Bumped to rpi_ws281x v1.0.0 (15330cb)
+* Full rpi_ws281x changes: https://github.com/jgarff/rpi_ws281x/compare/9be313f...15330cb
+* New: Added support for Revisions 0xa03141, 0xb03141, 0xc04141, 0xd03141 (CM4)
+* New: Added support for Revision 0xa32082 (Pi 3 B)
+* New: Added support for slices on PixelStrip
+* New: Regenerated SWIG bindings with v4.0.2
+* New: RGBW class for interfacing with pixel values
+
 4.3.4
+-----
 
 * New: Added support for Revision 0xa03115 (Pi 4, 1GB v1.5)
 
 4.3.3
 -----
 
 * New: Added support for Revision 0xc03115 (Pi 4, 4GB v1.5)
```

### Comparing `rpi_ws281x-4.3.4/LICENSE` & `rpi_ws281x-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/PKG-INFO` & `rpi_ws281x-5.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.2
 Name: rpi_ws281x
-Version: 4.3.4
+Version: 5.0.0
 Summary: Userspace Raspberry Pi PWM/PCM/SPI library for SK6812 and WS281X LEDs.
 Home-page: https://github.com/rpi-ws281x/rpi-ws281x-python/
 Author: Jeremy Garff <jer@jers.net>, Phil Howard <phil@pimoroni.com>
 Author-email: jer@jers.net, phil@pimoroni.com
 License: MIT
 Description: rpi\_ws281x
         ===========
@@ -183,15 +183,28 @@
         For transfers larger than 96 bytes the kernel driver also uses DMA. Of
         course there are practical limits on power and signal quality. These
         will be more constraining in practice than the theoretical limits above.
         
         When controlling a LED string of 240 LEDs the CPU load on the original
         Pi 2 (BCM2836) are: PWM 5% PCM 5% SPI 1%
         
+        
+        5.0.0
+        -----
+        
+        * Bumped to rpi_ws281x v1.0.0 (15330cb)
+        * Full rpi_ws281x changes: https://github.com/jgarff/rpi_ws281x/compare/9be313f...15330cb
+        * New: Added support for Revisions 0xa03141, 0xb03141, 0xc04141, 0xd03141 (CM4)
+        * New: Added support for Revision 0xa32082 (Pi 3 B)
+        * New: Added support for slices on PixelStrip
+        * New: Regenerated SWIG bindings with v4.0.2
+        * New: RGBW class for interfacing with pixel values
+        
         4.3.4
+        -----
         
         * New: Added support for Revision 0xa03115 (Pi 4, 1GB v1.5)
         
         4.3.3
         -----
         
         * New: Added support for Revision 0xc03115 (Pi 4, 4GB v1.5)
@@ -276,7 +289,15 @@
         
         3.0.7
         -----
         
         * New: Added support for Pi 3B+
         
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.6
```

### Comparing `rpi_ws281x-4.3.4/README.rst` & `rpi_ws281x-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/LICENSE` & `rpi_ws281x-5.0.0/lib/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/clk.h` & `rpi_ws281x-5.0.0/lib/clk.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/dma.c` & `rpi_ws281x-5.0.0/lib/dma.c`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/dma.h` & `rpi_ws281x-5.0.0/lib/dma.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/gpio.h` & `rpi_ws281x-5.0.0/lib/gpio.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/mailbox.c` & `rpi_ws281x-5.0.0/lib/mailbox.c`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/mailbox.h` & `rpi_ws281x-5.0.0/lib/mailbox.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/main.c` & `rpi_ws281x-5.0.0/lib/main.c`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -78,24 +78,24 @@
     .freq = TARGET_FREQ,
     .dmanum = DMA,
     .channel =
     {
         [0] =
         {
             .gpionum = GPIO_PIN,
-            .count = LED_COUNT,
             .invert = 0,
-            .brightness = 255,
+            .count = LED_COUNT,
             .strip_type = STRIP_TYPE,
+            .brightness = 255,
         },
         [1] =
         {
             .gpionum = 0,
-            .count = 0,
             .invert = 0,
+            .count = 0,
             .brightness = 0,
         },
     },
 };
 
 ws2811_led_t *matrix;
```

### Comparing `rpi_ws281x-4.3.4/lib/pcm.c` & `rpi_ws281x-5.0.0/lib/pcm.c`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/pcm.h` & `rpi_ws281x-5.0.0/lib/pcm.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/pwm.c` & `rpi_ws281x-5.0.0/lib/pwm.c`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/pwm.h` & `rpi_ws281x-5.0.0/lib/pwm.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/rpihw.c` & `rpi_ws281x-5.0.0/lib/rpihw.c`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     {
         .hwver = 0xc03131,
         .type = RPI_HWVER_TYPE_PI4,
         .periph_base = PERIPH_BASE_RPI4,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 400 - 4GB v1.1"
     },
+
     //
     // Raspberry Pi 4
     //
     {
         .hwver = 0xA03111,
         .type = RPI_HWVER_TYPE_PI4,
         .periph_base = PERIPH_BASE_RPI4,
@@ -152,21 +153,22 @@
     {
         .hwver = 0xc03115,
         .type = RPI_HWVER_TYPE_PI4,
         .periph_base = PERIPH_BASE_RPI4,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 4 Model B - 4GB v1.5"
     },
-    { 
+    {
         .hwver = 0xd03115,
         .type = RPI_HWVER_TYPE_PI4,
         .periph_base = PERIPH_BASE_RPI4,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 4 Model B - 8GB v1.5"
     },
+
     //
     // Compute Module 4
     //
     {
         .hwver = 0xa03140,
         .type = RPI_HWVER_TYPE_PI4,
         .periph_base = PERIPH_BASE_RPI4,
@@ -190,14 +192,43 @@
     {
         .hwver = 0xd03140,
         .type = RPI_HWVER_TYPE_PI4,
         .periph_base = PERIPH_BASE_RPI4,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Compute Module 4 v1.0 WiFi 8GB"
     },
+    {
+        .hwver = 0xa03141,
+        .type = RPI_HWVER_TYPE_PI4,
+        .periph_base = PERIPH_BASE_RPI4,
+        .videocore_base = VIDEOCORE_BASE_RPI2,
+        .desc = "Compute Module 4 Rev 1.1"
+    },
+    {
+        .hwver = 0xb03141,
+        .type = RPI_HWVER_TYPE_PI4,
+        .periph_base = PERIPH_BASE_RPI4,
+        .videocore_base = VIDEOCORE_BASE_RPI2,
+        .desc = "Compute Module 4 Rev 1.1"
+    },
+    {
+        .hwver = 0xc03141,
+        .type = RPI_HWVER_TYPE_PI4,
+        .periph_base = PERIPH_BASE_RPI4,
+        .videocore_base = VIDEOCORE_BASE_RPI2,
+        .desc = "Compute Module 4 Rev 1.1"
+    },
+    {
+        .hwver = 0xd03141,
+        .type = RPI_HWVER_TYPE_PI4,
+        .periph_base = PERIPH_BASE_RPI4,
+        .videocore_base = VIDEOCORE_BASE_RPI2,
+        .desc = "Compute Module 4 Rev 1.1"
+    },
+
     //
     // Model B Rev 1.0
     //
     {
         .hwver  = 0x02,
         .type = RPI_HWVER_TYPE_PI1,
         .periph_base = PERIPH_BASE_RPI,
@@ -325,14 +356,35 @@
     {
         .hwver  = 0x14,
         .type = RPI_HWVER_TYPE_PI1,
         .periph_base = PERIPH_BASE_RPI,
         .videocore_base = VIDEOCORE_BASE_RPI,
         .desc = "Compute Module 1",
     },
+    {
+        .hwver  = 0xa020a0,
+        .type = RPI_HWVER_TYPE_PI2,
+        .periph_base = PERIPH_BASE_RPI2,
+        .videocore_base = VIDEOCORE_BASE_RPI2,
+        .desc = "Compute Module 3/L3",
+    },
+    {
+        .hwver  = 0xa02100,
+        .type = RPI_HWVER_TYPE_PI2,
+        .periph_base = PERIPH_BASE_RPI2,
+        .videocore_base = VIDEOCORE_BASE_RPI2,
+        .desc = "Compute Module 3+",
+    },
+    {
+            .hwver  = 0xa220a0,
+            .type = RPI_HWVER_TYPE_PI2,
+            .periph_base = PERIPH_BASE_RPI2,
+            .videocore_base = VIDEOCORE_BASE_RPI2,
+            .desc = "Compute Module 3 Rev 1.0",
+    },
 
     //
     // Pi Zero
     //
     {
         .hwver  = 0x900092,
         .type = RPI_HWVER_TYPE_PI1,
@@ -365,17 +417,17 @@
         .hwver  = 0x9000c1,
         .type = RPI_HWVER_TYPE_PI1,
         .periph_base = PERIPH_BASE_RPI,
         .videocore_base = VIDEOCORE_BASE_RPI,
         .desc = "Pi Zero W v1.1",
     },
 
-    // 
+    //
     // Model Zero 2 W
-    // 
+    //
     {
         .hwver  = 0x902120,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi Zero 2 W v1.0",
     },
@@ -439,78 +491,69 @@
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 2",
     },
     //
     // Pi 3 Model B
     //
     {
-        .hwver  = 0xa020d3,
+        .hwver  = 0xa020d4,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 3 B+",
     },
     {
-        .hwver  = 0xa02082,
+        .hwver  = 0xa020d3,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
-        .desc = "Pi 3",
+        .desc = "Pi 3 B+",
     },
     {
-        .hwver  = 0xa02083,
+        .hwver  = 0xa32082,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
-        .desc = "Pi 3",
+        .desc = "Pi 3 B",
     },
     {
-        .hwver  = 0xa22082,
+        .hwver  = 0xa02082,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 3",
     },
     {
-        .hwver  = 0xa22083,
+        .hwver  = 0xa02083,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
         .desc = "Pi 3",
     },
     {
-        .hwver  = 0x9020e0,
+        .hwver  = 0xa22082,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
-        .desc = "Model 3 A+",
+        .desc = "Pi 3",
     },
-
-    //
-    // Pi Compute Module 3
-    //
     {
-        .hwver  = 0xa020a0,
+        .hwver  = 0xa22083,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
-        .desc = "Compute Module 3/L3",
+        .desc = "Pi 3",
     },
-    //
-    // Pi Compute Module 3+
-    //
     {
-        .hwver  = 0xa02100,
+        .hwver  = 0x9020e0,
         .type = RPI_HWVER_TYPE_PI2,
         .periph_base = PERIPH_BASE_RPI2,
         .videocore_base = VIDEOCORE_BASE_RPI2,
-        .desc = "Compute Module 3+",
-    },
-
-
+        .desc = "Model 3 A+",
+    }
 };
 
 
 const rpi_hw_t *rpi_hw_detect(void)
 {
     const rpi_hw_t *result = NULL;
     uint32_t rev;
@@ -588,8 +631,7 @@
     }
 #endif
 done:
     fclose(f);
 
     return result;
 }
-
```

### Comparing `rpi_ws281x-4.3.4/lib/rpihw.h` & `rpi_ws281x-5.0.0/lib/rpihw.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/lib/ws2811.c` & `rpi_ws281x-5.0.0/lib/ws2811.c`

 * *Files 17% similar despite different names*

```diff
@@ -68,22 +68,14 @@
 #define LED_RESET_WAIT_TIME                      300
 
 // Pad out to the nearest uint32 + 32-bits for idle low/high times the number of channels
 #define PWM_BYTE_COUNT(leds, freq)               (((((LED_BIT_COUNT(leds, freq) >> 3) & ~0x7) + 4) + 4) * \
                                                   RPI_PWM_CHANNELS)
 #define PCM_BYTE_COUNT(leds, freq)               ((((LED_BIT_COUNT(leds, freq) >> 3) & ~0x7) + 4) + 4)
 
-// Symbol definitions
-#define SYMBOL_HIGH                              0x6  // 1 1 0
-#define SYMBOL_LOW                               0x4  // 1 0 0
-
-// Symbol definitions for software inversion (PCM and SPI only)
-#define SYMBOL_HIGH_INV                          0x1  // 0 0 1
-#define SYMBOL_LOW_INV                           0x3  // 0 1 1
-
 // Driver mode definitions
 #define NONE	0
 #define PWM	1
 #define PCM	2
 #define SPI	3
 
 // We use the mailbox interface to request memory from the VideoCore.
@@ -1133,25 +1125,92 @@
  *
  * @param    ws2811  ws2811 instance pointer.
  *
  * @returns  None
  */
 ws2811_return_t  ws2811_render(ws2811_t *ws2811)
 {
+	static uint8_t convert_table[3][256] =
+	{ 
+		{
+			0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92,  
+			0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 
+			0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x92, 0x93, 0x93, 0x93, 
+			0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 
+			0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 0x93, 
+			0x93, 0x93, 0x93, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 
+			0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 
+			0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9A, 0x9B, 0x9B, 0x9B, 0x9B, 
+			0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 
+			0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 0x9B, 
+			0x9B, 0x9B, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 
+			0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 
+			0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD2, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 
+			0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 
+			0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 0xD3, 
+			0xD3, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 
+			0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 
+			0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDA, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 
+			0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 
+			0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB, 0xDB 
+		},
+		{		 
+			0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x4D, 
+			0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 
+			0x69, 0x69, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x49, 0x49, 0x49, 
+			0x49, 0x49, 0x49, 0x49, 0x49, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 
+			0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 
+			0x6D, 0x6D, 0x6D, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x4D, 0x4D, 
+			0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 
+			0x69, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x49, 0x49, 0x49, 0x49, 
+			0x49, 0x49, 0x49, 0x49, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x69, 
+			0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 
+			0x6D, 0x6D, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x4D, 0x4D, 0x4D, 
+			0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 
+			0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x49, 0x49, 0x49, 0x49, 0x49, 
+			0x49, 0x49, 0x49, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x69, 0x69, 
+			0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 
+			0x6D, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 0x4D, 0x4D, 0x4D, 0x4D, 
+			0x4D, 0x4D, 0x4D, 0x4D, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x69, 0x6D, 
+			0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x49, 0x49, 0x49, 0x49, 0x49, 0x49, 
+			0x49, 0x49, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x4D, 0x69, 0x69, 0x69, 
+			0x69, 0x69, 0x69, 0x69, 0x69, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D, 0x6D 		
+		},		
+		{
+			0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 
+			0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 
+			0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 
+			0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 
+			0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 
+			0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 
+			0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 
+			0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 
+			0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 
+			0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 
+			0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 
+			0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 
+			0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 
+			0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 
+			0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 
+			0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 
+			0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 
+			0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 
+			0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 
+			0x36, 0xA4, 0xA6, 0xB4, 0xB6, 0x24, 0x26, 0x34, 0x36, 0xA4, 0xA6, 0xB4, 0xB6 
+		}
+	};
+
     volatile uint8_t *pxl_raw = ws2811->device->pxl_raw;
     int driver_mode = ws2811->device->driver_mode;
-    int bitpos;
-    int i, k, l, chan;
+    int i, l, chan;
     unsigned j;
     ws2811_return_t ret = WS2811_SUCCESS;
     uint32_t protocol_time = 0;
     static uint64_t previous_timestamp = 0;
 
-    bitpos = (driver_mode == SPI ? 7 : 31);
-
     for (chan = 0; chan < RPI_PWM_CHANNELS; chan++)         // Channel
     {
         ws2811_channel_t *channel = &ws2811->channel[chan];
 
         int wordpos = chan; // PWM & PCM
         int bytepos = 0;    // SPI
         const int scale = (channel->brightness & 0xff) + 1;
@@ -1180,65 +1239,27 @@
                 channel->gamma[(((channel->leds[i] >> channel->gshift) & 0xff) * scale) >> 8], // green
                 channel->gamma[(((channel->leds[i] >> channel->bshift) & 0xff) * scale) >> 8], // blue
                 channel->gamma[(((channel->leds[i] >> channel->wshift) & 0xff) * scale) >> 8], // white
             };
 
             for (j = 0; j < array_size; j++)               // Color
             {
-                for (k = 7; k >= 0; k--)                   // Bit
-                {
-                    // Inversion is handled by hardware for PWM, otherwise by software here
-                    uint8_t symbol = SYMBOL_LOW;
-                    if ((driver_mode != PWM) && channel->invert) symbol = SYMBOL_LOW_INV;
-
-                    if (color[j] & (1 << k))
-                    {
-                        symbol = SYMBOL_HIGH;
-                        if ((driver_mode != PWM) && channel->invert) symbol = SYMBOL_HIGH_INV;
-                    }
-
-                    for (l = 2; l >= 0; l--)               // Symbol
-                    {
-                        uint32_t *wordptr = &((uint32_t *)pxl_raw)[wordpos];   // PWM & PCM
-                        volatile uint8_t  *byteptr = &pxl_raw[bytepos];    // SPI
-
-                        if (driver_mode == SPI)
-                        {
-                            *byteptr &= ~(1 << bitpos);
-                            if (symbol & (1 << l))
-                            {
-                                *byteptr |= (1 << bitpos);
-                            }
-                        }
-                        else  // PWM & PCM
-                        {
-                            *wordptr &= ~(1 << bitpos);
-                            if (symbol & (1 << l))
-                            {
-                                *wordptr |= (1 << bitpos);
-                            }
-                        }
-
-                        bitpos--;
-                        if (bitpos < 0)
-                        {
-                            if (driver_mode == SPI)
-                            {
-                                bytepos++;
-                                bitpos = 7;
-                            }
-                            else  // PWM & PCM
-                            {
-                                // Every other word is on the same channel for PWM
-                                wordpos += (driver_mode == PWM ? 2 : 1);
-                                bitpos = 31;
-                            }
-                        }
-                    }
-                }
+				for(l = 0; l < 3; ++l)
+				{
+					uint8_t pos = driver_mode == SPI ? bytepos : 3 - bytepos;
+					uint8_t val = convert_table[l][color[j]];
+					if ((driver_mode != PWM) && channel->invert) val = ~val;
+					
+					pxl_raw[wordpos * 4 + pos] = val;
+					if(++bytepos == 4) 
+					{ 
+						bytepos = 0; 
+						wordpos += driver_mode == PWM ? 2 : 1; 
+					}
+				}
             }
         }
     }
 
     // Wait for any previous DMA operation to complete.
     if ((ret = ws2811_wait(ws2811)) != WS2811_SUCCESS)
     {
```

### Comparing `rpi_ws281x-4.3.4/lib/ws2811.h` & `rpi_ws281x-5.0.0/lib/ws2811.h`

 * *Files identical despite different names*

### Comparing `rpi_ws281x-4.3.4/rpi_ws281x/rpi_ws281x.py` & `rpi_ws281x-5.0.0/rpi_ws281x/rpi_ws281x.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,48 @@
 # Adafruit NeoPixel library port to the rpi_ws281x library.
 # Author: Tony DiCola (tony@tonydicola.com), Jeremy Garff (jer@jers.net)
 import _rpi_ws281x as ws
 import atexit
 
 
-try:
-    xrange(0)
-except NameError:
-    xrange = range
+class RGBW(int):
+    def __new__(self, r, g=None, b=None, w=None):
+        if (g, b, w) == (None, None, None):
+            return int.__new__(self, r)
+        else:
+            if w is None:
+                w = 0
+            return int.__new__(self, (w << 24) | (r << 16) | (g << 8) | b)
+
+    @property
+    def r(self):
+        return (self >> 16) & 0xff
+
+    @property
+    def g(self):
+        return (self >> 8) & 0xff
+
+    @property
+    def b(self):
+        return (self) & 0xff
+
+    @property
+    def w(self):
+        return (self >> 24) & 0xff
 
 
 def Color(red, green, blue, white=0):
     """Convert the provided red, green, blue color to a 24-bit color value.
     Each color component should be a value 0-255 where 0 is the lowest intensity
     and 255 is the highest intensity.
     """
-    return (white << 24) | (red << 16) | (green << 8) | blue
-
-
-class _LED_Data(object):
-    """Wrapper class which makes a SWIG LED color data array look and feel like
-    a Python list of integers.
-    """
-    def __init__(self, channel, size):
-        self.size = size
-        self.channel = channel
-
-    def __getitem__(self, pos):
-        """Return the 24-bit RGB color value at the provided position or slice
-        of positions.
-        """
-        # Handle if a slice of positions are passed in by grabbing all the values
-        # and returning them in a list.
-        if isinstance(pos, slice):
-            return [ws.ws2811_led_get(self.channel, n) for n in xrange(*pos.indices(self.size))]
-        # Else assume the passed in value is a number to the position.
-        else:
-            return ws.ws2811_led_get(self.channel, pos)
-
-    def __setitem__(self, pos, value):
-        """Set the 24-bit RGB color value at the provided position or slice of
-        positions.
-        """
-        # Handle if a slice of positions are passed in by setting the appropriate
-        # LED data values to the provided values.
-        if isinstance(pos, slice):
-            index = 0
-            for n in xrange(*pos.indices(self.size)):
-                ws.ws2811_led_set(self.channel, n, value[index])
-                index += 1
-        # Else assume the passed in value is a number to the position.
-        else:
-            return ws.ws2811_led_set(self.channel, pos, value)
+    return RGBW(red, green, blue, white)
 
 
-class PixelStrip(object):
+class PixelStrip:
     def __init__(self, num, pin, freq_hz=800000, dma=10, invert=False,
             brightness=255, channel=0, strip_type=None, gamma=None):
         """Class to represent a SK6812/WS281x LED display.  Num should be the
         number of pixels in the display, and pin should be the GPIO pin connected
         to the display signal line (must be a PWM pin like 18!).  Optional
         parameters are freq, the frequency of the display signal in hertz (default
         800khz), dma, the DMA channel to use (default 10), invert, a boolean
@@ -87,31 +71,59 @@
             ws.ws2811_channel_t_count_set(chan, 0)
             ws.ws2811_channel_t_gpionum_set(chan, 0)
             ws.ws2811_channel_t_invert_set(chan, 0)
             ws.ws2811_channel_t_brightness_set(chan, 0)
 
         # Initialize the channel in use
         self._channel = ws.ws2811_channel_get(self._leds, channel)
+
         ws.ws2811_channel_t_gamma_set(self._channel, gamma)
         ws.ws2811_channel_t_count_set(self._channel, num)
         ws.ws2811_channel_t_gpionum_set(self._channel, pin)
         ws.ws2811_channel_t_invert_set(self._channel, 0 if not invert else 1)
         ws.ws2811_channel_t_brightness_set(self._channel, brightness)
         ws.ws2811_channel_t_strip_type_set(self._channel, strip_type)
 
         # Initialize the controller
         ws.ws2811_t_freq_set(self._leds, freq_hz)
         ws.ws2811_t_dmanum_set(self._leds, dma)
 
-        # Grab the led data array.
-        self._led_data = _LED_Data(self._channel, num)
+        self.size = num
 
         # Substitute for __del__, traps an exit condition and cleans up properly
         atexit.register(self._cleanup)
 
+    def __getitem__(self, pos):
+        """Return the 24-bit RGB color value at the provided position or slice
+        of positions.
+        """
+        # Handle if a slice of positions are passed in by grabbing all the values
+        # and returning them in a list.
+        if isinstance(pos, slice):
+            return [ws.ws2811_led_get(self._channel, n) for n in range(*pos.indices(self.size))]
+        # Else assume the passed in value is a number to the position.
+        else:
+            return ws.ws2811_led_get(self._channel, pos)
+
+    def __setitem__(self, pos, value):
+        """Set the 24-bit RGB color value at the provided position or slice of
+        positions.
+        """
+        # Handle if a slice of positions are passed in by setting the appropriate
+        # LED data values to the provided value.
+        if isinstance(pos, slice):
+            for n in range(*pos.indices(self.size)):
+                ws.ws2811_led_set(self._channel, n, value)
+        # Else assume the passed in value is a number to the position.
+        else:
+            return ws.ws2811_led_set(self._channel, pos, value)
+
+    def __len__(self):
+        return ws.ws2811_channel_t_count_get(self._channel)
+
     def _cleanup(self):
         # Clean up memory used by the library when not needed anymore.
         if self._leds is not None:
             ws.ws2811_fini(self._leds)
             ws.delete_ws2811_t(self._leds)
             self._leds = None
             self._channel = None
@@ -136,15 +148,15 @@
         if resp != 0:
             str_resp = ws.ws2811_get_return_t_str(resp)
             raise RuntimeError('ws2811_render failed with code {0} ({1})'.format(resp, str_resp))
 
     def setPixelColor(self, n, color):
         """Set LED at position n to the provided 24-bit color value (in RGB order).
         """
-        self._led_data[n] = color
+        self[n] = color
 
     def setPixelColorRGB(self, n, red, green, blue, white=0):
         """Set LED at position n to the provided red, green, and blue color.
         Each color component should be a value from 0 to 255 (where 0 is the
         lowest intensity and 255 is the highest intensity).
         """
         self.setPixelColor(n, Color(red, green, blue, white))
@@ -158,35 +170,26 @@
         """
         ws.ws2811_channel_t_brightness_set(self._channel, brightness)
 
     def getPixels(self):
         """Return an object which allows access to the LED display data as if
         it were a sequence of 24-bit RGB values.
         """
-        return self._led_data
+        return self[:]
 
     def numPixels(self):
         """Return the number of pixels in the display."""
-        return ws.ws2811_channel_t_count_get(self._channel)
+        return len(self)
 
     def getPixelColor(self, n):
         """Get the 24-bit RGB color value for the LED at position n."""
-        return self._led_data[n]
+        return self[n]
 
     def getPixelColorRGB(self, n):
-        c = lambda: None
-        setattr(c, 'r', self._led_data[n] >> 16 & 0xff)
-        setattr(c, 'g', self._led_data[n] >> 8  & 0xff)
-        setattr(c, 'b', self._led_data[n]    & 0xff)
-        return c
-    
+        return RGBW(self[n])
+
     def getPixelColorRGBW(self, n):
-        c = lambda: None
-        setattr(c, 'w', self._led_data[n] >> 24 & 0xff)
-        setattr(c, 'r', self._led_data[n] >> 16 & 0xff)
-        setattr(c, 'g', self._led_data[n] >> 8  & 0xff)
-        setattr(c, 'b', self._led_data[n]    & 0xff)
-        return c
+        return RGBW(self[n])
 
 # Shim for back-compatibility
 class Adafruit_NeoPixel(PixelStrip):
     pass
```

### Comparing `rpi_ws281x-4.3.4/rpi_ws281x.egg-info/PKG-INFO` & `rpi_ws281x-5.0.0/rpi_ws281x.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.0
+Metadata-Version: 1.2
 Name: rpi-ws281x
-Version: 4.3.4
+Version: 5.0.0
 Summary: Userspace Raspberry Pi PWM/PCM/SPI library for SK6812 and WS281X LEDs.
 Home-page: https://github.com/rpi-ws281x/rpi-ws281x-python/
 Author: Jeremy Garff <jer@jers.net>, Phil Howard <phil@pimoroni.com>
 Author-email: jer@jers.net, phil@pimoroni.com
 License: MIT
 Description: rpi\_ws281x
         ===========
@@ -183,15 +183,28 @@
         For transfers larger than 96 bytes the kernel driver also uses DMA. Of
         course there are practical limits on power and signal quality. These
         will be more constraining in practice than the theoretical limits above.
         
         When controlling a LED string of 240 LEDs the CPU load on the original
         Pi 2 (BCM2836) are: PWM 5% PCM 5% SPI 1%
         
+        
+        5.0.0
+        -----
+        
+        * Bumped to rpi_ws281x v1.0.0 (15330cb)
+        * Full rpi_ws281x changes: https://github.com/jgarff/rpi_ws281x/compare/9be313f...15330cb
+        * New: Added support for Revisions 0xa03141, 0xb03141, 0xc04141, 0xd03141 (CM4)
+        * New: Added support for Revision 0xa32082 (Pi 3 B)
+        * New: Added support for slices on PixelStrip
+        * New: Regenerated SWIG bindings with v4.0.2
+        * New: RGBW class for interfacing with pixel values
+        
         4.3.4
+        -----
         
         * New: Added support for Revision 0xa03115 (Pi 4, 1GB v1.5)
         
         4.3.3
         -----
         
         * New: Added support for Revision 0xc03115 (Pi 4, 4GB v1.5)
@@ -276,7 +289,15 @@
         
         3.0.7
         -----
         
         * New: Added support for Pi 3B+
         
 Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.6
```

### Comparing `rpi_ws281x-4.3.4/rpi_ws281x_wrap.c` & `rpi_ws281x-5.0.0/rpi_ws281x_wrap.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 /* ----------------------------------------------------------------------------
  * This file was automatically generated by SWIG (http://www.swig.org).
- * Version 2.0.12
+ * Version 4.0.2
  *
  * This file is not intended to be easily readable and contains a number of
  * coding conventions designed to improve portability and efficiency. Do not make
  * changes to this file unless you know what you are doing--modify the SWIG
  * interface file instead.
  * ----------------------------------------------------------------------------- */
 
+
+#ifndef SWIGPYTHON
 #define SWIGPYTHON
+#endif
+
 #define SWIG_PYTHON_DIRECTOR_NO_VTABLE
 
 /* -----------------------------------------------------------------------------
  *  This section contains generic SWIG labels for method/variable
  *  declarations/attributes, and other compiler dependent labels.
  * ----------------------------------------------------------------------------- */
 
@@ -74,17 +78,19 @@
 
 /* internal inline SWIG method */
 #ifndef SWIGINTERNINLINE
 # define SWIGINTERNINLINE SWIGINTERN SWIGINLINE
 #endif
 
 /* exporting methods */
-#if (__GNUC__ >= 4) || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4)
-#  ifndef GCC_HASCLASSVISIBILITY
-#    define GCC_HASCLASSVISIBILITY
+#if defined(__GNUC__)
+#  if (__GNUC__ >= 4) || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4)
+#    ifndef GCC_HASCLASSVISIBILITY
+#      define GCC_HASCLASSVISIBILITY
+#    endif
 #  endif
 #endif
 
 #ifndef SWIGEXPORT
 # if defined(_WIN32) || defined(__WIN32__) || defined(__CYGWIN__)
 #   if defined(STATIC_LINKED)
 #     define SWIGEXPORT
@@ -115,21 +121,39 @@
 #endif
 
 /* Deal with Microsoft's attempt at deprecating methods in the standard C++ library */
 #if !defined(SWIG_NO_SCL_SECURE_NO_DEPRECATE) && defined(_MSC_VER) && !defined(_SCL_SECURE_NO_DEPRECATE)
 # define _SCL_SECURE_NO_DEPRECATE
 #endif
 
+/* Deal with Apple's deprecated 'AssertMacros.h' from Carbon-framework */
+#if defined(__APPLE__) && !defined(__ASSERT_MACROS_DEFINE_VERSIONS_WITHOUT_UNDERSCORES)
+# define __ASSERT_MACROS_DEFINE_VERSIONS_WITHOUT_UNDERSCORES 0
+#endif
+
+/* Intel's compiler complains if a variable which was never initialised is
+ * cast to void, which is a common idiom which we use to indicate that we
+ * are aware a variable isn't used.  So we just silence that warning.
+ * See: https://github.com/swig/swig/issues/192 for more discussion.
+ */
+#ifdef __INTEL_COMPILER
+# pragma warning disable 592
+#endif
 
 
+#if defined(__GNUC__) && defined(_WIN32) && !defined(SWIG_PYTHON_NO_HYPOT_WORKAROUND)
+/* Workaround for '::hypot' has not been declared', see https://bugs.python.org/issue11566 */
+# include <math.h>
+#endif
+
 #if defined(_DEBUG) && defined(SWIG_PYTHON_INTERPRETER_NO_DEBUG)
 /* Use debug wrappers with the Python release dll */
 # undef _DEBUG
 # include <Python.h>
-# define _DEBUG
+# define _DEBUG 1
 #else
 # include <Python.h>
 #endif
 
 /* -----------------------------------------------------------------------------
  * swigrun.swg
  *
@@ -171,14 +195,15 @@
 #ifndef SWIG_BUFFER_SIZE
 # define SWIG_BUFFER_SIZE 1024
 #endif
 
 /* Flags for pointer conversions */
 #define SWIG_POINTER_DISOWN        0x1
 #define SWIG_CAST_NEW_MEMORY       0x2
+#define SWIG_POINTER_NO_NULL       0x4
 
 /* Flags for new pointer objects */
 #define SWIG_POINTER_OWN           0x1
 
 
 /*
    Flags/methods for returning states.
@@ -532,22 +557,22 @@
 SWIGRUNTIME swig_type_info *
 SWIG_MangledTypeQueryModule(swig_module_info *start,
                             swig_module_info *end,
 		            const char *name) {
   swig_module_info *iter = start;
   do {
     if (iter->size) {
-      register size_t l = 0;
-      register size_t r = iter->size - 1;
+      size_t l = 0;
+      size_t r = iter->size - 1;
       do {
 	/* since l+r >= 0, we can (>> 1) instead (/ 2) */
-	register size_t i = (l + r) >> 1;
+	size_t i = (l + r) >> 1;
 	const char *iname = iter->types[i]->name;
 	if (iname) {
-	  register int compare = strcmp(name, iname);
+	  int compare = strcmp(name, iname);
 	  if (compare == 0) {
 	    return iter->types[i];
 	  } else if (compare < 0) {
 	    if (i) {
 	      r = i - 1;
 	    } else {
 	      break;
@@ -583,15 +608,15 @@
   if (ret) {
     return ret;
   } else {
     /* STEP 2: If the type hasn't been found, do a complete search
        of the str field (the human readable name) */
     swig_module_info *iter = start;
     do {
-      register size_t i = 0;
+      size_t i = 0;
       for (; i < iter->size; ++i) {
 	if (iter->types[i]->str && (SWIG_TypeEquiv(iter->types[i]->str, name)))
 	  return iter->types[i];
       }
       iter = iter->next;
     } while (iter != end);
   }
@@ -602,45 +627,45 @@
 
 /*
    Pack binary data into a string
 */
 SWIGRUNTIME char *
 SWIG_PackData(char *c, void *ptr, size_t sz) {
   static const char hex[17] = "0123456789abcdef";
-  register const unsigned char *u = (unsigned char *) ptr;
-  register const unsigned char *eu =  u + sz;
+  const unsigned char *u = (unsigned char *) ptr;
+  const unsigned char *eu =  u + sz;
   for (; u != eu; ++u) {
-    register unsigned char uu = *u;
+    unsigned char uu = *u;
     *(c++) = hex[(uu & 0xf0) >> 4];
     *(c++) = hex[uu & 0xf];
   }
   return c;
 }
 
 /*
    Unpack binary data from a string
 */
 SWIGRUNTIME const char *
 SWIG_UnpackData(const char *c, void *ptr, size_t sz) {
-  register unsigned char *u = (unsigned char *) ptr;
-  register const unsigned char *eu = u + sz;
+  unsigned char *u = (unsigned char *) ptr;
+  const unsigned char *eu = u + sz;
   for (; u != eu; ++u) {
-    register char d = *(c++);
-    register unsigned char uu;
+    char d = *(c++);
+    unsigned char uu;
     if ((d >= '0') && (d <= '9'))
-      uu = ((d - '0') << 4);
+      uu = (unsigned char)((d - '0') << 4);
     else if ((d >= 'a') && (d <= 'f'))
-      uu = ((d - ('a'-10)) << 4);
+      uu = (unsigned char)((d - ('a'-10)) << 4);
     else
       return (char *) 0;
     d = *(c++);
     if ((d >= '0') && (d <= '9'))
-      uu |= (d - '0');
+      uu |= (unsigned char)(d - '0');
     else if ((d >= 'a') && (d <= 'f'))
-      uu |= (d - ('a'-10));
+      uu |= (unsigned char)(d - ('a'-10));
     else
       return (char *) 0;
     *u = uu;
   }
   return c;
 }
 
@@ -755,192 +780,65 @@
 
 /* Warning: This function will allocate a new string in Python 3,
  * so please call SWIG_Python_str_DelForPy3(x) to free the space.
  */
 SWIGINTERN char*
 SWIG_Python_str_AsChar(PyObject *str)
 {
-#if PY_VERSION_HEX >= 0x03000000
-  char *cstr;
-  char *newstr;
-  Py_ssize_t len;
+#if PY_VERSION_HEX >= 0x03030000
+  return (char *)PyUnicode_AsUTF8(str);
+#elif PY_VERSION_HEX >= 0x03000000
+  char *newstr = 0;
   str = PyUnicode_AsUTF8String(str);
-  PyBytes_AsStringAndSize(str, &cstr, &len);
-  newstr = (char *) malloc(len+1);
-  memcpy(newstr, cstr, len+1);
-  Py_XDECREF(str);
+  if (str) {
+    char *cstr;
+    Py_ssize_t len;
+    if (PyBytes_AsStringAndSize(str, &cstr, &len) != -1) {
+      newstr = (char *) malloc(len+1);
+      if (newstr)
+        memcpy(newstr, cstr, len+1);
+    }
+    Py_XDECREF(str);
+  }
   return newstr;
 #else
   return PyString_AsString(str);
 #endif
 }
 
-#if PY_VERSION_HEX >= 0x03000000
-#  define SWIG_Python_str_DelForPy3(x) free( (void*) (x) )
+#if PY_VERSION_HEX >= 0x03030000 || PY_VERSION_HEX < 0x03000000
+#  define SWIG_Python_str_DelForPy3(x)
 #else
-#  define SWIG_Python_str_DelForPy3(x) 
+#  define SWIG_Python_str_DelForPy3(x) free( (void*) (x) )
 #endif
 
 
 SWIGINTERN PyObject*
 SWIG_Python_str_FromChar(const char *c)
 {
 #if PY_VERSION_HEX >= 0x03000000
   return PyUnicode_FromString(c); 
 #else
   return PyString_FromString(c);
 #endif
 }
 
-/* Add PyOS_snprintf for old Pythons */
-#if PY_VERSION_HEX < 0x02020000
-# if defined(_MSC_VER) || defined(__BORLANDC__) || defined(_WATCOM)
-#  define PyOS_snprintf _snprintf
-# else
-#  define PyOS_snprintf snprintf
-# endif
-#endif
-
-/* A crude PyString_FromFormat implementation for old Pythons */
-#if PY_VERSION_HEX < 0x02020000
-
-#ifndef SWIG_PYBUFFER_SIZE
-# define SWIG_PYBUFFER_SIZE 1024
-#endif
-
-static PyObject *
-PyString_FromFormat(const char *fmt, ...) {
-  va_list ap;
-  char buf[SWIG_PYBUFFER_SIZE * 2];
-  int res;
-  va_start(ap, fmt);
-  res = vsnprintf(buf, sizeof(buf), fmt, ap);
-  va_end(ap);
-  return (res < 0 || res >= (int)sizeof(buf)) ? 0 : PyString_FromString(buf);
-}
-#endif
-
-/* Add PyObject_Del for old Pythons */
-#if PY_VERSION_HEX < 0x01060000
-# define PyObject_Del(op) PyMem_DEL((op))
-#endif
 #ifndef PyObject_DEL
 # define PyObject_DEL PyObject_Del
 #endif
 
-/* A crude PyExc_StopIteration exception for old Pythons */
-#if PY_VERSION_HEX < 0x02020000
-# ifndef PyExc_StopIteration
-#  define PyExc_StopIteration PyExc_RuntimeError
-# endif
-# ifndef PyObject_GenericGetAttr
-#  define PyObject_GenericGetAttr 0
-# endif
-#endif
-
-/* Py_NotImplemented is defined in 2.1 and up. */
-#if PY_VERSION_HEX < 0x02010000
-# ifndef Py_NotImplemented
-#  define Py_NotImplemented PyExc_RuntimeError
-# endif
-#endif
-
-/* A crude PyString_AsStringAndSize implementation for old Pythons */
-#if PY_VERSION_HEX < 0x02010000
-# ifndef PyString_AsStringAndSize
-#  define PyString_AsStringAndSize(obj, s, len) {*s = PyString_AsString(obj); *len = *s ? strlen(*s) : 0;}
-# endif
-#endif
-
-/* PySequence_Size for old Pythons */
-#if PY_VERSION_HEX < 0x02000000
-# ifndef PySequence_Size
-#  define PySequence_Size PySequence_Length
-# endif
-#endif
-
-/* PyBool_FromLong for old Pythons */
-#if PY_VERSION_HEX < 0x02030000
-static
-PyObject *PyBool_FromLong(long ok)
-{
-  PyObject *result = ok ? Py_True : Py_False;
-  Py_INCREF(result);
-  return result;
-}
-#endif
-
-/* Py_ssize_t for old Pythons */
-/* This code is as recommended by: */
-/* http://www.python.org/dev/peps/pep-0353/#conversion-guidelines */
-#if PY_VERSION_HEX < 0x02050000 && !defined(PY_SSIZE_T_MIN)
-typedef int Py_ssize_t;
-# define PY_SSIZE_T_MAX INT_MAX
-# define PY_SSIZE_T_MIN INT_MIN
-typedef inquiry lenfunc;
-typedef intargfunc ssizeargfunc;
-typedef intintargfunc ssizessizeargfunc;
-typedef intobjargproc ssizeobjargproc;
-typedef intintobjargproc ssizessizeobjargproc;
-typedef getreadbufferproc readbufferproc;
-typedef getwritebufferproc writebufferproc;
-typedef getsegcountproc segcountproc;
-typedef getcharbufferproc charbufferproc;
-static long PyNumber_AsSsize_t (PyObject *x, void *SWIGUNUSEDPARM(exc))
-{
-  long result = 0;
-  PyObject *i = PyNumber_Int(x);
-  if (i) {
-    result = PyInt_AsLong(i);
-    Py_DECREF(i);
-  }
-  return result;
-}
-#endif
-
-#if PY_VERSION_HEX < 0x02050000
-#define PyInt_FromSize_t(x) PyInt_FromLong((long)x)
-#endif
-
-#if PY_VERSION_HEX < 0x02040000
-#define Py_VISIT(op)				\
-  do { 						\
-    if (op) {					\
-      int vret = visit((op), arg);		\
-      if (vret)					\
-        return vret;				\
-    }						\
-  } while (0)
-#endif
-
-#if PY_VERSION_HEX < 0x02030000
-typedef struct {
-  PyTypeObject type;
-  PyNumberMethods as_number;
-  PyMappingMethods as_mapping;
-  PySequenceMethods as_sequence;
-  PyBufferProcs as_buffer;
-  PyObject *name, *slots;
-} PyHeapTypeObject;
-#endif
-
-#if PY_VERSION_HEX < 0x02030000
-typedef destructor freefunc;
-#endif
-
-#if ((PY_MAJOR_VERSION == 2 && PY_MINOR_VERSION > 6) || \
-     (PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION > 0) || \
-     (PY_MAJOR_VERSION > 3))
+// SWIGPY_USE_CAPSULE is no longer used within SWIG itself, but some user
+// interface files check for it.
 # define SWIGPY_USE_CAPSULE
-# define SWIGPY_CAPSULE_NAME ((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION ".type_pointer_capsule" SWIG_TYPE_TABLE_NAME)
-#endif
+# define SWIGPY_CAPSULE_NAME ("swig_runtime_data" SWIG_RUNTIME_VERSION ".type_pointer_capsule" SWIG_TYPE_TABLE_NAME)
 
 #if PY_VERSION_HEX < 0x03020000
 #define PyDescr_TYPE(x) (((PyDescrObject *)(x))->d_type)
 #define PyDescr_NAME(x) (((PyDescrObject *)(x))->d_name)
+#define Py_hash_t long
 #endif
 
 /* -----------------------------------------------------------------------------
  * error manipulation
  * ----------------------------------------------------------------------------- */
 
 SWIGRUNTIME PyObject*
@@ -990,40 +888,72 @@
 SWIGRUNTIME void
 SWIG_Python_AddErrorMsg(const char* mesg)
 {
   PyObject *type = 0;
   PyObject *value = 0;
   PyObject *traceback = 0;
 
-  if (PyErr_Occurred()) PyErr_Fetch(&type, &value, &traceback);
+  if (PyErr_Occurred())
+    PyErr_Fetch(&type, &value, &traceback);
   if (value) {
-    char *tmp;
     PyObject *old_str = PyObject_Str(value);
+    const char *tmp = SWIG_Python_str_AsChar(old_str);
     PyErr_Clear();
     Py_XINCREF(type);
-
-    PyErr_Format(type, "%s %s", tmp = SWIG_Python_str_AsChar(old_str), mesg);
+    if (tmp)
+      PyErr_Format(type, "%s %s", tmp, mesg);
+    else
+      PyErr_Format(type, "%s", mesg);
     SWIG_Python_str_DelForPy3(tmp);
     Py_DECREF(old_str);
     Py_DECREF(value);
   } else {
     PyErr_SetString(PyExc_RuntimeError, mesg);
   }
 }
 
+SWIGRUNTIME int
+SWIG_Python_TypeErrorOccurred(PyObject *obj)
+{
+  PyObject *error;
+  if (obj)
+    return 0;
+  error = PyErr_Occurred();
+  return error && PyErr_GivenExceptionMatches(error, PyExc_TypeError);
+}
+
+SWIGRUNTIME void
+SWIG_Python_RaiseOrModifyTypeError(const char *message)
+{
+  if (SWIG_Python_TypeErrorOccurred(NULL)) {
+    /* Use existing TypeError to preserve stacktrace and enhance with given message */
+    PyObject *newvalue;
+    PyObject *type = NULL, *value = NULL, *traceback = NULL;
+    PyErr_Fetch(&type, &value, &traceback);
+#if PY_VERSION_HEX >= 0x03000000
+    newvalue = PyUnicode_FromFormat("%S\nAdditional information:\n%s", value, message);
+#else
+    newvalue = PyString_FromFormat("%s\nAdditional information:\n%s", PyString_AsString(value), message);
+#endif
+    Py_XDECREF(value);
+    PyErr_Restore(type, newvalue, traceback);
+  } else {
+    /* Raise TypeError using given message */
+    PyErr_SetString(PyExc_TypeError, message);
+  }
+}
+
 #if defined(SWIG_PYTHON_NO_THREADS)
 #  if defined(SWIG_PYTHON_THREADS)
 #    undef SWIG_PYTHON_THREADS
 #  endif
 #endif
 #if defined(SWIG_PYTHON_THREADS) /* Threading support is enabled */
 #  if !defined(SWIG_PYTHON_USE_GIL) && !defined(SWIG_PYTHON_NO_USE_GIL)
-#    if (PY_VERSION_HEX >= 0x02030000) /* For 2.3 or later, use the PyGILState calls */
-#      define SWIG_PYTHON_USE_GIL
-#    endif
+#    define SWIG_PYTHON_USE_GIL
 #  endif
 #  if defined(SWIG_PYTHON_USE_GIL) /* Use PyGILState threads calls */
 #    ifndef SWIG_PYTHON_INITIALIZE_THREADS
 #     define SWIG_PYTHON_INITIALIZE_THREADS  PyEval_InitThreads() 
 #    endif
 #    ifdef __cplusplus /* C++ code */
        class SWIG_Python_Thread_Block {
@@ -1092,52 +1022,43 @@
 /* Constant Types */
 #define SWIG_PY_POINTER 4
 #define SWIG_PY_BINARY  5
 
 /* Constant information structure */
 typedef struct swig_const_info {
   int type;
-  char *name;
+  const char *name;
   long lvalue;
   double dvalue;
   void   *pvalue;
   swig_type_info **ptype;
 } swig_const_info;
 
-
-/* -----------------------------------------------------------------------------
- * Wrapper of PyInstanceMethod_New() used in Python 3
- * It is exported to the generated module, used for -fastproxy
- * ----------------------------------------------------------------------------- */
-#if PY_VERSION_HEX >= 0x03000000
-SWIGRUNTIME PyObject* SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func)
-{
-  return PyInstanceMethod_New(func);
-}
-#else
-SWIGRUNTIME PyObject* SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *SWIGUNUSEDPARM(func))
-{
-  return NULL;
-}
-#endif
-
 #ifdef __cplusplus
 }
 #endif
 
 
 /* -----------------------------------------------------------------------------
  * pyrun.swg
  *
  * This file contains the runtime support for Python modules
  * and includes code for managing global variables and pointer
  * type checking.
  *
  * ----------------------------------------------------------------------------- */
 
+#if PY_VERSION_HEX < 0x02070000 /* 2.7.0 */
+# error "This version of SWIG only supports Python >= 2.7"
+#endif
+
+#if PY_VERSION_HEX >= 0x03000000 && PY_VERSION_HEX < 0x03020000
+# error "This version of SWIG only supports Python 3 >= 3.2"
+#endif
+
 /* Common SWIG API */
 
 /* for raw pointers */
 #define SWIG_Python_ConvertPtr(obj, pptr, type, flags)  SWIG_Python_ConvertPtrAndOwn(obj, pptr, type, flags, 0)
 #define SWIG_ConvertPtr(obj, pptr, type, flags)         SWIG_Python_ConvertPtr(obj, pptr, type, flags)
 #define SWIG_ConvertPtrAndOwn(obj,pptr,type,flags,own)  SWIG_Python_ConvertPtrAndOwn(obj, pptr, type, flags, own)
 
@@ -1213,43 +1134,34 @@
   PyObject *s = PyString_InternFromString(key);
   PyList_Append(seq, s);
   Py_DECREF(s);
 }
 
 SWIGINTERN void
 SWIG_Python_SetConstant(PyObject *d, PyObject *public_interface, const char *name, PyObject *obj) {   
-#if PY_VERSION_HEX < 0x02030000
-  PyDict_SetItemString(d, (char *)name, obj);
-#else
   PyDict_SetItemString(d, name, obj);
-#endif
   Py_DECREF(obj);
   if (public_interface)
     SwigPyBuiltin_AddPublicSymbol(public_interface, name);
 }
 
 #else
 
 SWIGINTERN void
 SWIG_Python_SetConstant(PyObject *d, const char *name, PyObject *obj) {   
-#if PY_VERSION_HEX < 0x02030000
-  PyDict_SetItemString(d, (char *)name, obj);
-#else
   PyDict_SetItemString(d, name, obj);
-#endif
   Py_DECREF(obj);                            
 }
 
 #endif
 
 /* Append a value to the result obj */
 
 SWIGINTERN PyObject*
 SWIG_Python_AppendOutput(PyObject* result, PyObject* obj) {
-#if !defined(SWIG_PYTHON_OUTPUT_TUPLE)
   if (!result) {
     result = obj;
   } else if (result == Py_None) {
     Py_DECREF(result);
     result = obj;
   } else {
     if (!PyList_Check(result)) {
@@ -1257,93 +1169,79 @@
       result = PyList_New(1);
       PyList_SetItem(result, 0, o2);
     }
     PyList_Append(result,obj);
     Py_DECREF(obj);
   }
   return result;
-#else
-  PyObject*   o2;
-  PyObject*   o3;
-  if (!result) {
-    result = obj;
-  } else if (result == Py_None) {
-    Py_DECREF(result);
-    result = obj;
-  } else {
-    if (!PyTuple_Check(result)) {
-      o2 = result;
-      result = PyTuple_New(1);
-      PyTuple_SET_ITEM(result, 0, o2);
-    }
-    o3 = PyTuple_New(1);
-    PyTuple_SET_ITEM(o3, 0, obj);
-    o2 = result;
-    result = PySequence_Concat(o2, o3);
-    Py_DECREF(o2);
-    Py_DECREF(o3);
-  }
-  return result;
-#endif
 }
 
 /* Unpack the argument tuple */
 
-SWIGINTERN int
+SWIGINTERN Py_ssize_t
 SWIG_Python_UnpackTuple(PyObject *args, const char *name, Py_ssize_t min, Py_ssize_t max, PyObject **objs)
 {
   if (!args) {
     if (!min && !max) {
       return 1;
     } else {
       PyErr_Format(PyExc_TypeError, "%s expected %s%d arguments, got none", 
 		   name, (min == max ? "" : "at least "), (int)min);
       return 0;
     }
   }  
   if (!PyTuple_Check(args)) {
     if (min <= 1 && max >= 1) {
-      register int i;
+      Py_ssize_t i;
       objs[0] = args;
       for (i = 1; i < max; ++i) {
 	objs[i] = 0;
       }
       return 2;
     }
     PyErr_SetString(PyExc_SystemError, "UnpackTuple() argument list is not a tuple");
     return 0;
   } else {
-    register Py_ssize_t l = PyTuple_GET_SIZE(args);
+    Py_ssize_t l = PyTuple_GET_SIZE(args);
     if (l < min) {
       PyErr_Format(PyExc_TypeError, "%s expected %s%d arguments, got %d", 
 		   name, (min == max ? "" : "at least "), (int)min, (int)l);
       return 0;
     } else if (l > max) {
       PyErr_Format(PyExc_TypeError, "%s expected %s%d arguments, got %d", 
 		   name, (min == max ? "" : "at most "), (int)max, (int)l);
       return 0;
     } else {
-      register int i;
+      Py_ssize_t i;
       for (i = 0; i < l; ++i) {
 	objs[i] = PyTuple_GET_ITEM(args, i);
       }
       for (; l < max; ++l) {
 	objs[l] = 0;
       }
       return i + 1;
     }    
   }
 }
 
+SWIGINTERN int
+SWIG_Python_CheckNoKeywords(PyObject *kwargs, const char *name) {
+  int no_kwargs = 1;
+  if (kwargs) {
+    assert(PyDict_Check(kwargs));
+    if (PyDict_Size(kwargs) > 0) {
+      PyErr_Format(PyExc_TypeError, "%s() does not take keyword arguments", name);
+      no_kwargs = 0;
+    }
+  }
+  return no_kwargs;
+}
+
 /* A functor is a function object with one single object argument */
-#if PY_VERSION_HEX >= 0x02020000
 #define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunctionObjArgs(functor, obj, NULL);
-#else
-#define SWIG_Python_CallFunctor(functor, obj)	        PyObject_CallFunction(functor, "O", obj);
-#endif
 
 /*
   Helper for static pointer initialization for both C and C++ code, for example
   static PyObject *SWIG_STATIC_POINTER(MyVar) = NewSomething(...);
 */
 #ifdef __cplusplus
 #define SWIG_STATIC_POINTER(var)  var
@@ -1364,43 +1262,14 @@
 #define SWIG_BUILTIN_TP_INIT	    (SWIG_POINTER_OWN << 2)
 #define SWIG_BUILTIN_INIT	    (SWIG_BUILTIN_TP_INIT | SWIG_POINTER_OWN)
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-/*  How to access Py_None */
-#if defined(_WIN32) || defined(__WIN32__) || defined(__CYGWIN__)
-#  ifndef SWIG_PYTHON_NO_BUILD_NONE
-#    ifndef SWIG_PYTHON_BUILD_NONE
-#      define SWIG_PYTHON_BUILD_NONE
-#    endif
-#  endif
-#endif
-
-#ifdef SWIG_PYTHON_BUILD_NONE
-#  ifdef Py_None
-#   undef Py_None
-#   define Py_None SWIG_Py_None()
-#  endif
-SWIGRUNTIMEINLINE PyObject * 
-_SWIG_Py_None(void)
-{
-  PyObject *none = Py_BuildValue((char*)"");
-  Py_DECREF(none);
-  return none;
-}
-SWIGRUNTIME PyObject * 
-SWIG_Py_None(void)
-{
-  static PyObject *SWIG_STATIC_POINTER(none) = _SWIG_Py_None();
-  return none;
-}
-#endif
-
 /* The python void return value */
 
 SWIGRUNTIMEINLINE PyObject * 
 SWIG_Py_Void(void)
 {
   PyObject *none = Py_None;
   Py_INCREF(none);
@@ -1419,15 +1288,18 @@
   PyTypeObject *pytype;
 } SwigPyClientData;
 
 SWIGRUNTIMEINLINE int 
 SWIG_Python_CheckImplicit(swig_type_info *ty)
 {
   SwigPyClientData *data = (SwigPyClientData *)ty->clientdata;
-  return data ? data->implicitconv : 0;
+  int fail = data ? data->implicitconv : 0;
+  if (fail)
+    PyErr_SetString(PyExc_TypeError, "Implicit conversion is prohibited for explicit constructors.");
+  return fail;
 }
 
 SWIGRUNTIMEINLINE PyObject *
 SWIG_Python_ExceptionType(swig_type_info *desc) {
   SwigPyClientData *data = desc ? (SwigPyClientData *) desc->clientdata : 0;
   PyObject *klass = data ? data->klass : 0;
   return (klass ? klass : PyExc_RuntimeError);
@@ -1446,43 +1318,35 @@
     Py_INCREF(data->klass);
     /* the newraw method and newargs arguments used to create a new raw instance */
     if (PyClass_Check(obj)) {
       data->newraw = 0;
       data->newargs = obj;
       Py_INCREF(obj);
     } else {
-#if (PY_VERSION_HEX < 0x02020000)
-      data->newraw = 0;
-#else
-      data->newraw = PyObject_GetAttrString(data->klass, (char *)"__new__");
-#endif
+      data->newraw = PyObject_GetAttrString(data->klass, "__new__");
       if (data->newraw) {
 	Py_INCREF(data->newraw);
 	data->newargs = PyTuple_New(1);
 	PyTuple_SetItem(data->newargs, 0, obj);
       } else {
 	data->newargs = obj;
       }
       Py_INCREF(data->newargs);
     }
     /* the destroy method, aka as the C++ delete method */
-    data->destroy = PyObject_GetAttrString(data->klass, (char *)"__swig_destroy__");
+    data->destroy = PyObject_GetAttrString(data->klass, "__swig_destroy__");
     if (PyErr_Occurred()) {
       PyErr_Clear();
       data->destroy = 0;
     }
     if (data->destroy) {
       int flags;
       Py_INCREF(data->destroy);
       flags = PyCFunction_GET_FLAGS(data->destroy);
-#ifdef METH_O
       data->delargs = !(flags & (METH_O));
-#else
-      data->delargs = 0;
-#endif
     } else {
       data->delargs = 0;
     }
     data->implicitconv = 0;
     data->pytype = 0;
     return data;
   }
@@ -1504,14 +1368,31 @@
   int own;
   PyObject *next;
 #ifdef SWIGPYTHON_BUILTIN
   PyObject *dict;
 #endif
 } SwigPyObject;
 
+
+#ifdef SWIGPYTHON_BUILTIN
+
+SWIGRUNTIME PyObject *
+SwigPyObject_get___dict__(PyObject *v, PyObject *SWIGUNUSEDPARM(args))
+{
+  SwigPyObject *sobj = (SwigPyObject *)v;
+
+  if (!sobj->dict)
+    sobj->dict = PyDict_New();
+
+  Py_INCREF(sobj->dict);
+  return sobj->dict;
+}
+
+#endif
+
 SWIGRUNTIME PyObject *
 SwigPyObject_long(SwigPyObject *v)
 {
   return PyLong_FromVoidPtr(v->ptr);
 }
 
 SWIGRUNTIME PyObject *
@@ -1545,40 +1426,40 @@
 SWIGRUNTIME PyObject *
 SwigPyObject_hex(SwigPyObject *v)
 {
   return SwigPyObject_format("%x",v);
 }
 
 SWIGRUNTIME PyObject *
-#ifdef METH_NOARGS
 SwigPyObject_repr(SwigPyObject *v)
-#else
-SwigPyObject_repr(SwigPyObject *v, PyObject *args)
-#endif
 {
   const char *name = SWIG_TypePrettyName(v->ty);
   PyObject *repr = SWIG_Python_str_FromFormat("<Swig Object of type '%s' at %p>", (name ? name : "unknown"), (void *)v);
   if (v->next) {
-# ifdef METH_NOARGS
     PyObject *nrep = SwigPyObject_repr((SwigPyObject *)v->next);
-# else
-    PyObject *nrep = SwigPyObject_repr((SwigPyObject *)v->next, args);
-# endif
 # if PY_VERSION_HEX >= 0x03000000
     PyObject *joined = PyUnicode_Concat(repr, nrep);
     Py_DecRef(repr);
     Py_DecRef(nrep);
     repr = joined;
 # else
     PyString_ConcatAndDel(&repr,nrep);
 # endif
   }
   return repr;  
 }
 
+/* We need a version taking two PyObject* parameters so it's a valid
+ * PyCFunction to use in swigobject_methods[]. */
+SWIGRUNTIME PyObject *
+SwigPyObject_repr2(PyObject *v, PyObject *SWIGUNUSEDPARM(args))
+{
+  return SwigPyObject_repr((SwigPyObject*)v);
+}
+
 SWIGRUNTIME int
 SwigPyObject_compare(SwigPyObject *v, SwigPyObject *w)
 {
   void *i = v->ptr;
   void *j = w->ptr;
   return (i < j) ? -1 : ((i > j) ? 1 : 0);
 }
@@ -1642,24 +1523,40 @@
   if (sobj->own == SWIG_POINTER_OWN) {
     swig_type_info *ty = sobj->ty;
     SwigPyClientData *data = ty ? (SwigPyClientData *) ty->clientdata : 0;
     PyObject *destroy = data ? data->destroy : 0;
     if (destroy) {
       /* destroy is always a VARARGS method */
       PyObject *res;
+
+      /* PyObject_CallFunction() has the potential to silently drop
+         the active exception.  In cases of unnamed temporary
+         variable or where we just finished iterating over a generator
+         StopIteration will be active right now, and this needs to
+         remain true upon return from SwigPyObject_dealloc.  So save
+         and restore. */
+      
+      PyObject *type = NULL, *value = NULL, *traceback = NULL;
+      PyErr_Fetch(&type, &value, &traceback);
+
       if (data->delargs) {
-	/* we need to create a temporary object to carry the destroy operation */
-	PyObject *tmp = SwigPyObject_New(sobj->ptr, ty, 0);
-	res = SWIG_Python_CallFunctor(destroy, tmp);
-	Py_DECREF(tmp);
+        /* we need to create a temporary object to carry the destroy operation */
+        PyObject *tmp = SwigPyObject_New(sobj->ptr, ty, 0);
+        res = SWIG_Python_CallFunctor(destroy, tmp);
+        Py_DECREF(tmp);
       } else {
-	PyCFunction meth = PyCFunction_GET_FUNCTION(destroy);
-	PyObject *mself = PyCFunction_GET_SELF(destroy);
-	res = ((*meth)(mself, v));
+        PyCFunction meth = PyCFunction_GET_FUNCTION(destroy);
+        PyObject *mself = PyCFunction_GET_SELF(destroy);
+        res = ((*meth)(mself, v));
       }
+      if (!res)
+        PyErr_WriteUnraisable(destroy);
+
+      PyErr_Restore(type, value, traceback);
+
       Py_XDECREF(res);
     } 
 #if !defined(SWIG_PYTHON_SILENT_MEMLEAK)
     else {
       const char *name = SWIG_TypePrettyName(ty);
       printf("swig/python detected a memory leak of type '%s', no destructor found.\n", (name ? name : "unknown"));
     }
@@ -1669,135 +1566,81 @@
   PyObject_DEL(v);
 }
 
 SWIGRUNTIME PyObject* 
 SwigPyObject_append(PyObject* v, PyObject* next)
 {
   SwigPyObject *sobj = (SwigPyObject *) v;
-#ifndef METH_O
-  PyObject *tmp = 0;
-  if (!PyArg_ParseTuple(next,(char *)"O:append", &tmp)) return NULL;
-  next = tmp;
-#endif
   if (!SwigPyObject_Check(next)) {
+    PyErr_SetString(PyExc_TypeError, "Attempt to append a non SwigPyObject");
     return NULL;
   }
   sobj->next = next;
   Py_INCREF(next);
   return SWIG_Py_Void();
 }
 
 SWIGRUNTIME PyObject* 
-#ifdef METH_NOARGS
-SwigPyObject_next(PyObject* v)
-#else
 SwigPyObject_next(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
-#endif
 {
   SwigPyObject *sobj = (SwigPyObject *) v;
   if (sobj->next) {    
     Py_INCREF(sobj->next);
     return sobj->next;
   } else {
     return SWIG_Py_Void();
   }
 }
 
 SWIGINTERN PyObject*
-#ifdef METH_NOARGS
-SwigPyObject_disown(PyObject *v)
-#else
 SwigPyObject_disown(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
-#endif
 {
   SwigPyObject *sobj = (SwigPyObject *)v;
   sobj->own = 0;
   return SWIG_Py_Void();
 }
 
 SWIGINTERN PyObject*
-#ifdef METH_NOARGS
-SwigPyObject_acquire(PyObject *v)
-#else
 SwigPyObject_acquire(PyObject* v, PyObject *SWIGUNUSEDPARM(args))
-#endif
 {
   SwigPyObject *sobj = (SwigPyObject *)v;
   sobj->own = SWIG_POINTER_OWN;
   return SWIG_Py_Void();
 }
 
 SWIGINTERN PyObject*
 SwigPyObject_own(PyObject *v, PyObject *args)
 {
   PyObject *val = 0;
-#if (PY_VERSION_HEX < 0x02020000)
-  if (!PyArg_ParseTuple(args,(char *)"|O:own",&val))
-#elif (PY_VERSION_HEX < 0x02050000)
-  if (!PyArg_UnpackTuple(args, (char *)"own", 0, 1, &val)) 
-#else
-  if (!PyArg_UnpackTuple(args, "own", 0, 1, &val)) 
-#endif
-    {
-      return NULL;
+  if (!PyArg_UnpackTuple(args, "own", 0, 1, &val)) {
+    return NULL;
+  } else {
+    SwigPyObject *sobj = (SwigPyObject *)v;
+    PyObject *obj = PyBool_FromLong(sobj->own);
+    if (val) {
+      if (PyObject_IsTrue(val)) {
+        SwigPyObject_acquire(v,args);
+      } else {
+        SwigPyObject_disown(v,args);
+      }
     } 
-  else
-    {
-      SwigPyObject *sobj = (SwigPyObject *)v;
-      PyObject *obj = PyBool_FromLong(sobj->own);
-      if (val) {
-#ifdef METH_NOARGS
-	if (PyObject_IsTrue(val)) {
-	  SwigPyObject_acquire(v);
-	} else {
-	  SwigPyObject_disown(v);
-	}
-#else
-	if (PyObject_IsTrue(val)) {
-	  SwigPyObject_acquire(v,args);
-	} else {
-	  SwigPyObject_disown(v,args);
-	}
-#endif
-      } 
-      return obj;
-    }
+    return obj;
+  }
 }
 
-#ifdef METH_O
 static PyMethodDef
 swigobject_methods[] = {
-  {(char *)"disown",  (PyCFunction)SwigPyObject_disown,  METH_NOARGS,  (char *)"releases ownership of the pointer"},
-  {(char *)"acquire", (PyCFunction)SwigPyObject_acquire, METH_NOARGS,  (char *)"acquires ownership of the pointer"},
-  {(char *)"own",     (PyCFunction)SwigPyObject_own,     METH_VARARGS, (char *)"returns/sets ownership of the pointer"},
-  {(char *)"append",  (PyCFunction)SwigPyObject_append,  METH_O,       (char *)"appends another 'this' object"},
-  {(char *)"next",    (PyCFunction)SwigPyObject_next,    METH_NOARGS,  (char *)"returns the next 'this' object"},
-  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,    METH_NOARGS,  (char *)"returns object representation"},
+  {"disown",  SwigPyObject_disown,  METH_NOARGS,  "releases ownership of the pointer"},
+  {"acquire", SwigPyObject_acquire, METH_NOARGS,  "acquires ownership of the pointer"},
+  {"own",     SwigPyObject_own,     METH_VARARGS, "returns/sets ownership of the pointer"},
+  {"append",  SwigPyObject_append,  METH_O,       "appends another 'this' object"},
+  {"next",    SwigPyObject_next,    METH_NOARGS,  "returns the next 'this' object"},
+  {"__repr__",SwigPyObject_repr2,   METH_NOARGS,  "returns object representation"},
   {0, 0, 0, 0}  
 };
-#else
-static PyMethodDef
-swigobject_methods[] = {
-  {(char *)"disown",  (PyCFunction)SwigPyObject_disown,  METH_VARARGS,  (char *)"releases ownership of the pointer"},
-  {(char *)"acquire", (PyCFunction)SwigPyObject_acquire, METH_VARARGS,  (char *)"aquires ownership of the pointer"},
-  {(char *)"own",     (PyCFunction)SwigPyObject_own,     METH_VARARGS,  (char *)"returns/sets ownership of the pointer"},
-  {(char *)"append",  (PyCFunction)SwigPyObject_append,  METH_VARARGS,  (char *)"appends another 'this' object"},
-  {(char *)"next",    (PyCFunction)SwigPyObject_next,    METH_VARARGS,  (char *)"returns the next 'this' object"},
-  {(char *)"__repr__",(PyCFunction)SwigPyObject_repr,   METH_VARARGS,  (char *)"returns object representation"},
-  {0, 0, 0, 0}  
-};
-#endif
-
-#if PY_VERSION_HEX < 0x02020000
-SWIGINTERN PyObject *
-SwigPyObject_getattr(SwigPyObject *sobj,char *name)
-{
-  return Py_FindMethod(swigobject_methods, (PyObject *)sobj, name);
-}
-#endif
 
 SWIGRUNTIME PyTypeObject*
 SwigPyObject_TypeOnce(void) {
   static char swigobject_doc[] = "Swig object carries a C/C++ instance pointer";
 
   static PyNumberMethods SwigPyObject_as_number = {
     (binaryfunc)0, /*nb_add*/
@@ -1830,69 +1673,61 @@
     0, /*nb_reserved*/
 #endif
     (unaryfunc)0,                 /*nb_float*/
 #if PY_VERSION_HEX < 0x03000000
     (unaryfunc)SwigPyObject_oct,  /*nb_oct*/
     (unaryfunc)SwigPyObject_hex,  /*nb_hex*/
 #endif
-#if PY_VERSION_HEX >= 0x03000000 /* 3.0 */
+#if PY_VERSION_HEX >= 0x03050000 /* 3.5 */
+    0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_matrix_multiply */
+#elif PY_VERSION_HEX >= 0x03000000 /* 3.0 */
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_index, nb_inplace_divide removed */
-#elif PY_VERSION_HEX >= 0x02050000 /* 2.5.0 */
+#else
     0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_index */
-#elif PY_VERSION_HEX >= 0x02020000 /* 2.2.0 */
-    0,0,0,0,0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_true_divide */
-#elif PY_VERSION_HEX >= 0x02000000 /* 2.0.0 */
-    0,0,0,0,0,0,0,0,0,0,0 /* nb_inplace_add -> nb_inplace_or */
 #endif
   };
 
   static PyTypeObject swigpyobject_type;
   static int type_init = 0;
   if (!type_init) {
     const PyTypeObject tmp = {
-      /* PyObject header changed in Python 3 */
 #if PY_VERSION_HEX >= 0x03000000
       PyVarObject_HEAD_INIT(NULL, 0)
 #else
       PyObject_HEAD_INIT(NULL)
       0,                                    /* ob_size */
 #endif
-      (char *)"SwigPyObject",               /* tp_name */
+      "SwigPyObject",                       /* tp_name */
       sizeof(SwigPyObject),                 /* tp_basicsize */
       0,                                    /* tp_itemsize */
       (destructor)SwigPyObject_dealloc,     /* tp_dealloc */
-      0,				    /* tp_print */
-#if PY_VERSION_HEX < 0x02020000
-      (getattrfunc)SwigPyObject_getattr,    /* tp_getattr */
-#else
+      0,                                    /* tp_print */
       (getattrfunc)0,                       /* tp_getattr */
-#endif
       (setattrfunc)0,                       /* tp_setattr */
 #if PY_VERSION_HEX >= 0x03000000
-    0, /* tp_reserved in 3.0.1, tp_compare in 3.0.0 but not used */
+      0, /* tp_reserved in 3.0.1, tp_compare in 3.0.0 but not used */
 #else
       (cmpfunc)SwigPyObject_compare,        /* tp_compare */
 #endif
       (reprfunc)SwigPyObject_repr,          /* tp_repr */
       &SwigPyObject_as_number,              /* tp_as_number */
       0,                                    /* tp_as_sequence */
       0,                                    /* tp_as_mapping */
       (hashfunc)0,                          /* tp_hash */
       (ternaryfunc)0,                       /* tp_call */
-      0,				    /* tp_str */
+      0,                                    /* tp_str */
       PyObject_GenericGetAttr,              /* tp_getattro */
       0,                                    /* tp_setattro */
       0,                                    /* tp_as_buffer */
       Py_TPFLAGS_DEFAULT,                   /* tp_flags */
       swigobject_doc,                       /* tp_doc */
       0,                                    /* tp_traverse */
       0,                                    /* tp_clear */
       (richcmpfunc)SwigPyObject_richcompare,/* tp_richcompare */
       0,                                    /* tp_weaklistoffset */
-#if PY_VERSION_HEX >= 0x02020000
       0,                                    /* tp_iter */
       0,                                    /* tp_iternext */
       swigobject_methods,                   /* tp_methods */
       0,                                    /* tp_members */
       0,                                    /* tp_getset */
       0,                                    /* tp_base */
       0,                                    /* tp_dict */
@@ -1905,33 +1740,37 @@
       0,                                    /* tp_free */
       0,                                    /* tp_is_gc */
       0,                                    /* tp_bases */
       0,                                    /* tp_mro */
       0,                                    /* tp_cache */
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
-#endif
-#if PY_VERSION_HEX >= 0x02030000
       0,                                    /* tp_del */
+      0,                                    /* tp_version_tag */
+#if PY_VERSION_HEX >= 0x03040000
+      0,                                    /* tp_finalize */
 #endif
-#if PY_VERSION_HEX >= 0x02060000
-      0,                                    /* tp_version */
+#if PY_VERSION_HEX >= 0x03080000
+      0,                                    /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+      0,                                    /* tp_print */
 #endif
 #ifdef COUNT_ALLOCS
-      0,0,0,0                               /* tp_alloc -> tp_next */
+      0,                                    /* tp_allocs */
+      0,                                    /* tp_frees */
+      0,                                    /* tp_maxalloc */
+      0,                                    /* tp_prev */
+      0                                     /* tp_next */
 #endif
     };
     swigpyobject_type = tmp;
     type_init = 1;
-#if PY_VERSION_HEX < 0x02020000
-    swigpyobject_type.ob_type = &PyType_Type;
-#else
     if (PyType_Ready(&swigpyobject_type) < 0)
       return NULL;
-#endif
   }
   return &swigpyobject_type;
 }
 
 SWIGRUNTIME PyObject *
 SwigPyObject_New(void *ptr, swig_type_info *ty, int own)
 {
@@ -1952,28 +1791,14 @@
 typedef struct {
   PyObject_HEAD
   void *pack;
   swig_type_info *ty;
   size_t size;
 } SwigPyPacked;
 
-SWIGRUNTIME int
-SwigPyPacked_print(SwigPyPacked *v, FILE *fp, int SWIGUNUSEDPARM(flags))
-{
-  char result[SWIG_BUFFER_SIZE];
-  fputs("<Swig Packed ", fp); 
-  if (SWIG_PackDataName(result, v->pack, v->size, 0, sizeof(result))) {
-    fputs("at ", fp); 
-    fputs(result, fp); 
-  }
-  fputs(v->ty->name,fp); 
-  fputs(">", fp);
-  return 0; 
-}
-  
 SWIGRUNTIME PyObject *
 SwigPyPacked_repr(SwigPyPacked *v)
 {
   char result[SWIG_BUFFER_SIZE];
   if (SWIG_PackDataName(result, v->pack, v->size, 0, sizeof(result))) {
     return SWIG_Python_str_FromFormat("<Swig Packed at %s%s>", result, v->ty->name);
   } else {
@@ -1994,15 +1819,15 @@
 
 SWIGRUNTIME int
 SwigPyPacked_compare(SwigPyPacked *v, SwigPyPacked *w)
 {
   size_t i = v->size;
   size_t j = w->size;
   int s = (i < j) ? -1 : ((i > j) ? 1 : 0);
-  return s ? s : strncmp((char *)v->pack, (char *)w->pack, 2*v->size);
+  return s ? s : strncmp((const char *)v->pack, (const char *)w->pack, 2*v->size);
 }
 
 SWIGRUNTIME PyTypeObject* SwigPyPacked_TypeOnce(void);
 
 SWIGRUNTIME PyTypeObject*
 SwigPyPacked_type(void) {
   static PyTypeObject *SWIG_STATIC_POINTER(type) = SwigPyPacked_TypeOnce();
@@ -2028,26 +1853,25 @@
 SWIGRUNTIME PyTypeObject*
 SwigPyPacked_TypeOnce(void) {
   static char swigpacked_doc[] = "Swig object carries a C/C++ instance pointer";
   static PyTypeObject swigpypacked_type;
   static int type_init = 0;
   if (!type_init) {
     const PyTypeObject tmp = {
-      /* PyObject header changed in Python 3 */
 #if PY_VERSION_HEX>=0x03000000
       PyVarObject_HEAD_INIT(NULL, 0)
 #else
       PyObject_HEAD_INIT(NULL)
       0,                                    /* ob_size */
 #endif
-      (char *)"SwigPyPacked",               /* tp_name */
+      "SwigPyPacked",                       /* tp_name */
       sizeof(SwigPyPacked),                 /* tp_basicsize */
       0,                                    /* tp_itemsize */
       (destructor)SwigPyPacked_dealloc,     /* tp_dealloc */
-      (printfunc)SwigPyPacked_print,        /* tp_print */
+      0,                                    /* tp_print */
       (getattrfunc)0,                       /* tp_getattr */
       (setattrfunc)0,                       /* tp_setattr */
 #if PY_VERSION_HEX>=0x03000000
       0, /* tp_reserved in 3.0.1 */
 #else
       (cmpfunc)SwigPyPacked_compare,        /* tp_compare */
 #endif
@@ -2063,15 +1887,14 @@
       0,                                    /* tp_as_buffer */
       Py_TPFLAGS_DEFAULT,                   /* tp_flags */
       swigpacked_doc,                       /* tp_doc */
       0,                                    /* tp_traverse */
       0,                                    /* tp_clear */
       0,                                    /* tp_richcompare */
       0,                                    /* tp_weaklistoffset */
-#if PY_VERSION_HEX >= 0x02020000
       0,                                    /* tp_iter */
       0,                                    /* tp_iternext */
       0,                                    /* tp_methods */
       0,                                    /* tp_members */
       0,                                    /* tp_getset */
       0,                                    /* tp_base */
       0,                                    /* tp_dict */
@@ -2084,33 +1907,37 @@
       0,                                    /* tp_free */
       0,                                    /* tp_is_gc */
       0,                                    /* tp_bases */
       0,                                    /* tp_mro */
       0,                                    /* tp_cache */
       0,                                    /* tp_subclasses */
       0,                                    /* tp_weaklist */
-#endif
-#if PY_VERSION_HEX >= 0x02030000
       0,                                    /* tp_del */
+      0,                                    /* tp_version_tag */
+#if PY_VERSION_HEX >= 0x03040000
+      0,                                    /* tp_finalize */
 #endif
-#if PY_VERSION_HEX >= 0x02060000
-      0,                                    /* tp_version */
+#if PY_VERSION_HEX >= 0x03080000
+      0,                                    /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+      0,                                    /* tp_print */
 #endif
 #ifdef COUNT_ALLOCS
-      0,0,0,0                               /* tp_alloc -> tp_next */
+      0,                                    /* tp_allocs */
+      0,                                    /* tp_frees */
+      0,                                    /* tp_maxalloc */
+      0,                                    /* tp_prev */
+      0                                     /* tp_next */
 #endif
     };
     swigpypacked_type = tmp;
     type_init = 1;
-#if PY_VERSION_HEX < 0x02020000
-    swigpypacked_type.ob_type = &PyType_Type;
-#else
     if (PyType_Ready(&swigpypacked_type) < 0)
       return NULL;
-#endif
   }
   return &swigpypacked_type;
 }
 
 SWIGRUNTIME PyObject *
 SwigPyPacked_New(void *ptr, size_t size, swig_type_info *ty)
 {
@@ -2143,28 +1970,22 @@
   }
 }
 
 /* -----------------------------------------------------------------------------
  * pointers/data manipulation
  * ----------------------------------------------------------------------------- */
 
-SWIGRUNTIMEINLINE PyObject *
-_SWIG_This(void)
-{
-    return SWIG_Python_str_FromChar("this");
-}
-
-static PyObject *swig_this = NULL;
+static PyObject *Swig_This_global = NULL;
 
 SWIGRUNTIME PyObject *
 SWIG_This(void)
 {
-  if (swig_this == NULL)
-    swig_this = _SWIG_This();
-  return swig_this;
+  if (Swig_This_global == NULL)
+    Swig_This_global = SWIG_Python_str_FromChar("this");
+  return Swig_This_global;
 }
 
 /* #define SWIG_PYTHON_SLOW_GETSET_THIS */
 
 /* TODO: I don't know how to implement the fast getset in Python 3 right now */
 #if PY_VERSION_HEX>=0x03000000
 #define SWIG_PYTHON_SLOW_GETSET_THIS 
@@ -2188,15 +2009,15 @@
   }
 # endif
   return NULL;
 #else
 
   obj = 0;
 
-#if (!defined(SWIG_PYTHON_SLOW_GETSET_THIS) && (PY_VERSION_HEX >= 0x02030000))
+#if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
   if (PyInstance_Check(pyobj)) {
     obj = _PyInstance_Lookup(pyobj, SWIG_This());      
   } else {
     PyObject **dictptr = _PyObject_GetDictPtr(pyobj);
     if (dictptr != NULL) {
       PyObject *dict = *dictptr;
       obj = dict ? PyDict_GetItem(dict, SWIG_This()) : 0;
@@ -2258,15 +2079,15 @@
   int implicit_conv = (flags & SWIG_POINTER_IMPLICIT_CONV) != 0;
 
   if (!obj)
     return SWIG_ERROR;
   if (obj == Py_None && !implicit_conv) {
     if (ptr)
       *ptr = 0;
-    return SWIG_OK;
+    return (flags & SWIG_POINTER_NO_NULL) ? SWIG_NullReferenceError : SWIG_OK;
   }
 
   res = SWIG_ERROR;
 
   sobj = SWIG_Python_GetSwigThis(obj);
   if (own)
     *own = 0;
@@ -2338,59 +2159,56 @@
                 }
               }
             }
             Py_DECREF(impconv);
           }
         }
       }
-    }
-    if (!SWIG_IsOK(res) && obj == Py_None) {
-      if (ptr)
-        *ptr = 0;
-      if (PyErr_Occurred())
-        PyErr_Clear();
-      res = SWIG_OK;
+      if (!SWIG_IsOK(res) && obj == Py_None) {
+        if (ptr)
+          *ptr = 0;
+        if (PyErr_Occurred())
+          PyErr_Clear();
+        res = SWIG_OK;
+      }
     }
   }
   return res;
 }
 
 /* Convert a function ptr value */
 
 SWIGRUNTIME int
 SWIG_Python_ConvertFunctionPtr(PyObject *obj, void **ptr, swig_type_info *ty) {
   if (!PyCFunction_Check(obj)) {
     return SWIG_ConvertPtr(obj, ptr, ty, 0);
   } else {
     void *vptr = 0;
-    
+    swig_cast_info *tc;
+
     /* here we get the method pointer for callbacks */
     const char *doc = (((PyCFunctionObject *)obj) -> m_ml -> ml_doc);
     const char *desc = doc ? strstr(doc, "swig_ptr: ") : 0;
     if (desc)
       desc = ty ? SWIG_UnpackVoidPtr(desc + 10, &vptr, ty->name) : 0;
-    if (!desc) 
+    if (!desc)
       return SWIG_ERROR;
-    if (ty) {
-      swig_cast_info *tc = SWIG_TypeCheck(desc,ty);
-      if (tc) {
-        int newmemory = 0;
-        *ptr = SWIG_TypeCast(tc,vptr,&newmemory);
-        assert(!newmemory); /* newmemory handling not yet implemented */
-      } else {
-        return SWIG_ERROR;
-      }
+    tc = SWIG_TypeCheck(desc,ty);
+    if (tc) {
+      int newmemory = 0;
+      *ptr = SWIG_TypeCast(tc,vptr,&newmemory);
+      assert(!newmemory); /* newmemory handling not yet implemented */
     } else {
-      *ptr = vptr;
+      return SWIG_ERROR;
     }
     return SWIG_OK;
   }
 }
 
-/* Convert a packed value value */
+/* Convert a packed pointer value */
 
 SWIGRUNTIME int
 SWIG_Python_ConvertPacked(PyObject *obj, void *ptr, size_t sz, swig_type_info *ty) {
   swig_type_info *to = SwigPyPacked_UnpackData(obj, ptr, sz);
   if (!to) return SWIG_ERROR;
   if (ty) {
     if (to != ty) {
@@ -2410,15 +2228,14 @@
   Create a new instance object, without calling __init__, and set the
   'this' attribute.
 */
 
 SWIGRUNTIME PyObject* 
 SWIG_Python_NewShadowInstance(SwigPyClientData *data, PyObject *swig_this)
 {
-#if (PY_VERSION_HEX >= 0x02020000)
   PyObject *inst = 0;
   PyObject *newraw = data->newraw;
   if (newraw) {
     inst = PyObject_Call(newraw, data->newargs, NULL);
     if (inst) {
 #if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
       PyObject **dictptr = _PyObject_GetDictPtr(inst);
@@ -2427,102 +2244,81 @@
 	if (dict == NULL) {
 	  dict = PyDict_New();
 	  *dictptr = dict;
 	  PyDict_SetItem(dict, SWIG_This(), swig_this);
 	}
       }
 #else
-      PyObject *key = SWIG_This();
-      PyObject_SetAttr(inst, key, swig_this);
+      if (PyObject_SetAttr(inst, SWIG_This(), swig_this) == -1) {
+        Py_DECREF(inst);
+        inst = 0;
+      }
 #endif
     }
   } else {
 #if PY_VERSION_HEX >= 0x03000000
-    inst = PyBaseObject_Type.tp_new((PyTypeObject*) data->newargs, Py_None, Py_None);
-    if (inst) {
-      PyObject_SetAttr(inst, SWIG_This(), swig_this);
-      Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
+    PyObject *empty_args = PyTuple_New(0);
+    if (empty_args) {
+      PyObject *empty_kwargs = PyDict_New();
+      if (empty_kwargs) {
+        inst = ((PyTypeObject *)data->newargs)->tp_new((PyTypeObject *)data->newargs, empty_args, empty_kwargs);
+        Py_DECREF(empty_kwargs);
+        if (inst) {
+          if (PyObject_SetAttr(inst, SWIG_This(), swig_this) == -1) {
+            Py_DECREF(inst);
+            inst = 0;
+          } else {
+            Py_TYPE(inst)->tp_flags &= ~Py_TPFLAGS_VALID_VERSION_TAG;
+          }
+        }
+      }
+      Py_DECREF(empty_args);
     }
 #else
     PyObject *dict = PyDict_New();
     if (dict) {
       PyDict_SetItem(dict, SWIG_This(), swig_this);
       inst = PyInstance_NewRaw(data->newargs, dict);
       Py_DECREF(dict);
     }
 #endif
   }
   return inst;
-#else
-#if (PY_VERSION_HEX >= 0x02010000)
-  PyObject *inst = 0;
-  PyObject *dict = PyDict_New();
-  if (dict) {
-    PyDict_SetItem(dict, SWIG_This(), swig_this);
-    inst = PyInstance_NewRaw(data->newargs, dict);
-    Py_DECREF(dict);
-  }
-  return (PyObject *) inst;
-#else
-  PyInstanceObject *inst = PyObject_NEW(PyInstanceObject, &PyInstance_Type);
-  if (inst == NULL) {
-    return NULL;
-  }
-  inst->in_class = (PyClassObject *)data->newargs;
-  Py_INCREF(inst->in_class);
-  inst->in_dict = PyDict_New();
-  if (inst->in_dict == NULL) {
-    Py_DECREF(inst);
-    return NULL;
-  }
-#ifdef Py_TPFLAGS_HAVE_WEAKREFS
-  inst->in_weakreflist = NULL;
-#endif
-#ifdef Py_TPFLAGS_GC
-  PyObject_GC_Init(inst);
-#endif
-  PyDict_SetItem(inst->in_dict, SWIG_This(), swig_this);
-  return (PyObject *) inst;
-#endif
-#endif
 }
 
-SWIGRUNTIME void
+SWIGRUNTIME int
 SWIG_Python_SetSwigThis(PyObject *inst, PyObject *swig_this)
 {
- PyObject *dict;
-#if (PY_VERSION_HEX >= 0x02020000) && !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
- PyObject **dictptr = _PyObject_GetDictPtr(inst);
- if (dictptr != NULL) {
-   dict = *dictptr;
-   if (dict == NULL) {
-     dict = PyDict_New();
-     *dictptr = dict;
-   }
-   PyDict_SetItem(dict, SWIG_This(), swig_this);
-   return;
- }
-#endif
- dict = PyObject_GetAttrString(inst, (char*)"__dict__");
- PyDict_SetItem(dict, SWIG_This(), swig_this);
- Py_DECREF(dict);
+#if !defined(SWIG_PYTHON_SLOW_GETSET_THIS)
+  PyObject **dictptr = _PyObject_GetDictPtr(inst);
+  if (dictptr != NULL) {
+    PyObject *dict = *dictptr;
+    if (dict == NULL) {
+      dict = PyDict_New();
+      *dictptr = dict;
+    }
+    return PyDict_SetItem(dict, SWIG_This(), swig_this);
+  }
+#endif
+  return PyObject_SetAttr(inst, SWIG_This(), swig_this);
 } 
 
 
 SWIGINTERN PyObject *
 SWIG_Python_InitShadowInstance(PyObject *args) {
   PyObject *obj[2];
   if (!SWIG_Python_UnpackTuple(args, "swiginit", 2, 2, obj)) {
     return NULL;
   } else {
     SwigPyObject *sthis = SWIG_Python_GetSwigThis(obj[0]);
     if (sthis) {
       SwigPyObject_append((PyObject*) sthis, obj[1]);
     } else {
-      SWIG_Python_SetSwigThis(obj[0], obj[1]);
+      if (SWIG_Python_SetSwigThis(obj[0], obj[1]) != 0)
+        return NULL;
     }
     return SWIG_Py_Void();
   }
 }
 
 /* Create a new pointer object */
 
@@ -2543,26 +2339,29 @@
       newobj = (SwigPyObject*) self;
       if (newobj->ptr) {
         PyObject *next_self = clientdata->pytype->tp_alloc(clientdata->pytype, 0);
         while (newobj->next)
 	  newobj = (SwigPyObject *) newobj->next;
         newobj->next = next_self;
         newobj = (SwigPyObject *)next_self;
+#ifdef SWIGPYTHON_BUILTIN
+        newobj->dict = 0;
+#endif
       }
     } else {
       newobj = PyObject_New(SwigPyObject, clientdata->pytype);
+#ifdef SWIGPYTHON_BUILTIN
+      newobj->dict = 0;
+#endif
     }
     if (newobj) {
       newobj->ptr = ptr;
       newobj->ty = type;
       newobj->own = own;
       newobj->next = 0;
-#ifdef SWIGPYTHON_BUILTIN
-      newobj->dict = 0;
-#endif
       return (PyObject*) newobj;
     }
     return SWIG_Py_Void();
   }
 
   assert(!(flags & SWIG_BUILTIN_TP_INIT));
 
@@ -2594,110 +2393,56 @@
 SWIG_Python_GetModule(void *SWIGUNUSEDPARM(clientdata)) {
   static void *type_pointer = (void *)0;
   /* first check if module already created */
   if (!type_pointer) {
 #ifdef SWIG_LINK_RUNTIME
     type_pointer = SWIG_ReturnGlobalTypeList((void *)0);
 #else
-# ifdef SWIGPY_USE_CAPSULE
     type_pointer = PyCapsule_Import(SWIGPY_CAPSULE_NAME, 0);
-# else
-    type_pointer = PyCObject_Import((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION,
-				    (char*)"type_pointer" SWIG_TYPE_TABLE_NAME);
-# endif
     if (PyErr_Occurred()) {
       PyErr_Clear();
       type_pointer = (void *)0;
     }
 #endif
   }
   return (swig_module_info *) type_pointer;
 }
 
-#if PY_MAJOR_VERSION < 2
-/* PyModule_AddObject function was introduced in Python 2.0.  The following function
-   is copied out of Python/modsupport.c in python version 2.3.4 */
-SWIGINTERN int
-PyModule_AddObject(PyObject *m, char *name, PyObject *o)
-{
-  PyObject *dict;
-  if (!PyModule_Check(m)) {
-    PyErr_SetString(PyExc_TypeError,
-		    "PyModule_AddObject() needs module as first arg");
-    return SWIG_ERROR;
-  }
-  if (!o) {
-    PyErr_SetString(PyExc_TypeError,
-		    "PyModule_AddObject() needs non-NULL value");
-    return SWIG_ERROR;
-  }
-  
-  dict = PyModule_GetDict(m);
-  if (dict == NULL) {
-    /* Internal error -- modules must have a dict! */
-    PyErr_Format(PyExc_SystemError, "module '%s' has no __dict__",
-		 PyModule_GetName(m));
-    return SWIG_ERROR;
-  }
-  if (PyDict_SetItemString(dict, name, o))
-    return SWIG_ERROR;
-  Py_DECREF(o);
-  return SWIG_OK;
-}
-#endif
-
 SWIGRUNTIME void
-#ifdef SWIGPY_USE_CAPSULE
 SWIG_Python_DestroyModule(PyObject *obj)
-#else
-SWIG_Python_DestroyModule(void *vptr)
-#endif
 {
-#ifdef SWIGPY_USE_CAPSULE
   swig_module_info *swig_module = (swig_module_info *) PyCapsule_GetPointer(obj, SWIGPY_CAPSULE_NAME);
-#else
-  swig_module_info *swig_module = (swig_module_info *) vptr;
-#endif
   swig_type_info **types = swig_module->types;
   size_t i;
   for (i =0; i < swig_module->size; ++i) {
     swig_type_info *ty = types[i];
     if (ty->owndata) {
       SwigPyClientData *data = (SwigPyClientData *) ty->clientdata;
       if (data) SwigPyClientData_Del(data);
     }
   }
   Py_DECREF(SWIG_This());
-  swig_this = NULL;
+  Swig_This_global = NULL;
 }
 
 SWIGRUNTIME void
 SWIG_Python_SetModule(swig_module_info *swig_module) {
 #if PY_VERSION_HEX >= 0x03000000
  /* Add a dummy module object into sys.modules */
-  PyObject *module = PyImport_AddModule((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION);
+  PyObject *module = PyImport_AddModule("swig_runtime_data" SWIG_RUNTIME_VERSION);
 #else
   static PyMethodDef swig_empty_runtime_method_table[] = { {NULL, NULL, 0, NULL} }; /* Sentinel */
-  PyObject *module = Py_InitModule((char*)"swig_runtime_data" SWIG_RUNTIME_VERSION, swig_empty_runtime_method_table);
+  PyObject *module = Py_InitModule("swig_runtime_data" SWIG_RUNTIME_VERSION, swig_empty_runtime_method_table);
 #endif
-#ifdef SWIGPY_USE_CAPSULE
   PyObject *pointer = PyCapsule_New((void *) swig_module, SWIGPY_CAPSULE_NAME, SWIG_Python_DestroyModule);
   if (pointer && module) {
-    PyModule_AddObject(module, (char*)"type_pointer_capsule" SWIG_TYPE_TABLE_NAME, pointer);
-  } else {
-    Py_XDECREF(pointer);
-  }
-#else
-  PyObject *pointer = PyCObject_FromVoidPtr((void *) swig_module, SWIG_Python_DestroyModule);
-  if (pointer && module) {
-    PyModule_AddObject(module, (char*)"type_pointer" SWIG_TYPE_TABLE_NAME, pointer);
+    PyModule_AddObject(module, "type_pointer_capsule" SWIG_TYPE_TABLE_NAME, pointer);
   } else {
     Py_XDECREF(pointer);
   }
-#endif
 }
 
 /* The python cached type query */
 SWIGRUNTIME PyObject *
 SWIG_Python_TypeCache(void) {
   static PyObject *SWIG_STATIC_POINTER(cache) = PyDict_New();
   return cache;
@@ -2707,28 +2452,20 @@
 SWIG_Python_TypeQuery(const char *type)
 {
   PyObject *cache = SWIG_Python_TypeCache();
   PyObject *key = SWIG_Python_str_FromChar(type); 
   PyObject *obj = PyDict_GetItem(cache, key);
   swig_type_info *descriptor;
   if (obj) {
-#ifdef SWIGPY_USE_CAPSULE
     descriptor = (swig_type_info *) PyCapsule_GetPointer(obj, NULL);
-#else
-    descriptor = (swig_type_info *) PyCObject_AsVoidPtr(obj);
-#endif
   } else {
     swig_module_info *swig_module = SWIG_GetModule(0);
     descriptor = SWIG_TypeQueryModule(swig_module, swig_module, type);
     if (descriptor) {
-#ifdef SWIGPY_USE_CAPSULE
       obj = PyCapsule_New((void*) descriptor, NULL, NULL);
-#else
-      obj = PyCObject_FromVoidPtr(descriptor, NULL);
-#endif
       PyDict_SetItem(cache, key, obj);
       Py_DECREF(obj);
     }
   }
   Py_DECREF(key);
   return descriptor;
 }
@@ -2745,22 +2482,23 @@
 {  
   if (PyErr_Occurred()) {
     PyObject *type = 0;
     PyObject *value = 0;
     PyObject *traceback = 0;
     PyErr_Fetch(&type, &value, &traceback);
     if (value) {
-      char *tmp;
       PyObject *old_str = PyObject_Str(value);
+      const char *tmp = SWIG_Python_str_AsChar(old_str);
+      const char *errmesg = tmp ? tmp : "Invalid error message";
       Py_XINCREF(type);
       PyErr_Clear();
       if (infront) {
-	PyErr_Format(type, "%s %s", mesg, tmp = SWIG_Python_str_AsChar(old_str));
+	PyErr_Format(type, "%s %s", mesg, errmesg);
       } else {
-	PyErr_Format(type, "%s %s", tmp = SWIG_Python_str_AsChar(old_str), mesg);
+	PyErr_Format(type, "%s %s", errmesg, mesg);
       }
       SWIG_Python_str_DelForPy3(tmp);
       Py_DECREF(old_str);
     }
     return 1;
   } else {
     return 0;
@@ -2878,14 +2616,16 @@
     f = descr->ob_type->tp_descr_set;
   if (!f) {
     if (PyString_Check(name)) {
       encoded_name = name;
       Py_INCREF(name);
     } else {
       encoded_name = PyUnicode_AsUTF8String(name);
+      if (!encoded_name)
+        return -1;
     }
     PyErr_Format(PyExc_AttributeError, "'%.100s' object has no attribute '%.200s'", tp->tp_name, PyString_AsString(encoded_name));
     Py_DECREF(encoded_name);
   } else {
     res = f(descr, obj, value);
   }
   
@@ -2904,14 +2644,29 @@
 
 #define SWIG_exception_fail(code, msg) do { SWIG_Error(code, msg); SWIG_fail; } while(0) 
 
 #define SWIG_contract_assert(expr, msg) if (!(expr)) { SWIG_Error(SWIG_RuntimeError, msg); SWIG_fail; } else 
 
 
 
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+/* Method creation and docstring support functions */
+
+SWIGINTERN PyMethodDef *SWIG_PythonGetProxyDoc(const char *name);
+SWIGINTERN PyObject *SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func);
+SWIGINTERN PyObject *SWIG_PyStaticMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func);
+
+#ifdef __cplusplus
+}
+#endif
+
+
 /* -------- TYPES TABLE (BEGIN) -------- */
 
 #define SWIGTYPE_p_char swig_types[0]
 #define SWIGTYPE_p_int swig_types[1]
 #define SWIGTYPE_p_long_long swig_types[2]
 #define SWIGTYPE_p_rpi_hw_t swig_types[3]
 #define SWIGTYPE_p_short swig_types[4]
@@ -2927,33 +2682,32 @@
 static swig_type_info *swig_types[15];
 static swig_module_info swig_module = {swig_types, 14, 0, 0, 0, 0};
 #define SWIG_TypeQuery(name) SWIG_TypeQueryModule(&swig_module, &swig_module, name)
 #define SWIG_MangledTypeQuery(name) SWIG_MangledTypeQueryModule(&swig_module, &swig_module, name)
 
 /* -------- TYPES TABLE (END) -------- */
 
-#if (PY_VERSION_HEX <= 0x02000000)
-# if !defined(SWIG_PYTHON_CLASSIC)
-#  error "This python version requires swig to be run with the '-classic' option"
-# endif
+#ifdef SWIG_TypeQuery
+# undef SWIG_TypeQuery
 #endif
+#define SWIG_TypeQuery SWIG_Python_TypeQuery
 
 /*-----------------------------------------------
               @(target):= _rpi_ws281x.so
   ------------------------------------------------*/
 #if PY_VERSION_HEX >= 0x03000000
 #  define SWIG_init    PyInit__rpi_ws281x
 
 #else
 #  define SWIG_init    init_rpi_ws281x
 
 #endif
 #define SWIG_name    "_rpi_ws281x"
 
-#define SWIGVERSION 0x020012 
+#define SWIGVERSION 0x040002 
 #define SWIG_VERSION SWIGVERSION
 
 
 #define SWIG_as_voidptr(a) (void *)((const void *)(a)) 
 #define SWIG_as_voidptrptr(a) ((void)SWIG_as_voidptr(*a),(void**)(a)) 
 
 
@@ -3007,17 +2761,19 @@
 SWIGINTERN int
 SWIG_AsVal_double (PyObject *obj, double *val)
 {
   int res = SWIG_TypeError;
   if (PyFloat_Check(obj)) {
     if (val) *val = PyFloat_AsDouble(obj);
     return SWIG_OK;
+#if PY_VERSION_HEX < 0x03000000
   } else if (PyInt_Check(obj)) {
-    if (val) *val = PyInt_AsLong(obj);
+    if (val) *val = (double) PyInt_AsLong(obj);
     return SWIG_OK;
+#endif
   } else if (PyLong_Check(obj)) {
     double v = PyLong_AsDouble(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
@@ -3083,24 +2839,28 @@
   return 0;
 }
 
 
 SWIGINTERN int
 SWIG_AsVal_long (PyObject *obj, long* val)
 {
+#if PY_VERSION_HEX < 0x03000000
   if (PyInt_Check(obj)) {
     if (val) *val = PyInt_AsLong(obj);
     return SWIG_OK;
-  } else if (PyLong_Check(obj)) {
+  } else
+#endif
+  if (PyLong_Check(obj)) {
     long v = PyLong_AsLong(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
+      return SWIG_OverflowError;
     }
   }
 #ifdef SWIG_PYTHON_CAST_MODE
   {
     int dispatch = 0;
     long v = PyInt_AsLong(obj);
     if (!PyErr_Occurred()) {
@@ -3156,26 +2916,15 @@
   if (PyLong_Check(obj)) {
     unsigned long v = PyLong_AsUnsignedLong(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
-#if PY_VERSION_HEX >= 0x03000000
-      {
-        long v = PyLong_AsLong(obj);
-        if (!PyErr_Occurred()) {
-          if (v < 0) {
-            return SWIG_OverflowError;
-          }
-        } else {
-          PyErr_Clear();
-        }
-      }
-#endif
+      return SWIG_OverflowError;
     }
   }
 #ifdef SWIG_PYTHON_CAST_MODE
   {
     int dispatch = 0;
     unsigned long v = PyLong_AsUnsignedLong(obj);
     if (!PyErr_Occurred()) {
@@ -3210,82 +2959,86 @@
       if (val) *val = (unsigned char)(v);
     }
   }  
   return res;
 }
 
 
-  #define SWIG_From_long   PyLong_FromLong 
+  #define SWIG_From_long   PyInt_FromLong 
 
 
 SWIGINTERNINLINE PyObject* 
 SWIG_From_unsigned_SS_long  (unsigned long value)
 {
   return (value > LONG_MAX) ?
-    PyLong_FromUnsignedLong(value) : PyLong_FromLong((long)(value)); 
+    PyLong_FromUnsignedLong(value) : PyInt_FromLong((long)(value));
 }
 
 
 SWIGINTERNINLINE PyObject *
 SWIG_From_unsigned_SS_char  (unsigned char value)
 {    
   return SWIG_From_unsigned_SS_long  (value);
 }
 
 
+#if defined(LLONG_MAX) && !defined(SWIG_LONG_LONG_AVAILABLE)
+#  define SWIG_LONG_LONG_AVAILABLE
+#endif
+
+
+#ifdef SWIG_LONG_LONG_AVAILABLE
 SWIGINTERN int
 SWIG_AsVal_unsigned_SS_long_SS_long (PyObject *obj, unsigned long long *val)
 {
   int res = SWIG_TypeError;
   if (PyLong_Check(obj)) {
     unsigned long long v = PyLong_AsUnsignedLongLong(obj);
     if (!PyErr_Occurred()) {
       if (val) *val = v;
       return SWIG_OK;
     } else {
       PyErr_Clear();
+      res = SWIG_OverflowError;
     }
   } else {
     unsigned long v;
     res = SWIG_AsVal_unsigned_SS_long (obj,&v);
     if (SWIG_IsOK(res)) {
       if (val) *val = v;
       return res;
     }
   }
 #ifdef SWIG_PYTHON_CAST_MODE
   {
     const double mant_max = 1LL << DBL_MANT_DIG;
     double d;
     res = SWIG_AsVal_double (obj,&d);
+    if (SWIG_IsOK(res) && !SWIG_CanCastAsInteger(&d, 0, mant_max))
+      return SWIG_OverflowError;
     if (SWIG_IsOK(res) && SWIG_CanCastAsInteger(&d, 0, mant_max)) {
       if (val) *val = (unsigned long long)(d);
       return SWIG_AddCast(res);
     }
     res = SWIG_TypeError;
   }
 #endif
   return res;
 }
+#endif
 
 
-SWIGINTERNINLINE PyObject* 
-SWIG_From_long_SS_long  (long long value)
-{
-  return ((value < LONG_MIN) || (value > LONG_MAX)) ?
-    PyLong_FromLongLong(value) : PyLong_FromLong((long)(value)); 
-}
-
-
+#ifdef SWIG_LONG_LONG_AVAILABLE
 SWIGINTERNINLINE PyObject* 
 SWIG_From_unsigned_SS_long_SS_long  (unsigned long long value)
 {
   return (value > LONG_MAX) ?
-    PyLong_FromUnsignedLongLong(value) : PyLong_FromLong((long)(value)); 
+    PyLong_FromUnsignedLongLong(value) : PyInt_FromLong((long)(value));
 }
+#endif
 
 
 SWIGINTERN int
 SWIG_AsVal_unsigned_SS_int (PyObject * obj, unsigned int *val)
 {
   unsigned long v;
   int res = SWIG_AsVal_unsigned_SS_long (obj, &v);
@@ -3326,17 +3079,21 @@
   if (carray) {
     if (size > INT_MAX) {
       swig_type_info* pchar_descriptor = SWIG_pchar_descriptor();
       return pchar_descriptor ? 
 	SWIG_InternalNewPointerObj((char *)(carray), pchar_descriptor, 0) : SWIG_Py_Void();
     } else {
 #if PY_VERSION_HEX >= 0x03000000
-      return PyUnicode_FromStringAndSize(carray, (int)(size));
+#if defined(SWIG_PYTHON_STRICT_BYTE_CHAR)
+      return PyBytes_FromStringAndSize(carray, (Py_ssize_t)(size));
+#else
+      return PyUnicode_DecodeUTF8(carray, (Py_ssize_t)(size), "surrogateescape");
+#endif
 #else
-      return PyString_FromStringAndSize(carray, (int)(size));
+      return PyString_FromStringAndSize(carray, (Py_ssize_t)(size));
 #endif
     }
   } else {
     return SWIG_Py_Void();
   }
 }
 
@@ -3376,581 +3133,581 @@
     }
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_gpionum_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_gpionum_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_gpionum_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gpionum_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gpionum_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_gpionum_set" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   if (arg1) (arg1)->gpionum = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_gpionum_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   int result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_gpionum_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gpionum_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gpionum_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (int) ((arg1)->gpionum);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_invert_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_invert_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_invert_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_invert_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_invert_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_invert_set" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   if (arg1) (arg1)->invert = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_invert_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   int result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_invert_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_invert_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_invert_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (int) ((arg1)->invert);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_count_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_count_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_count_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_count_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_count_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_count_set" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   if (arg1) (arg1)->count = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_count_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   int result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_count_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_count_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_count_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (int) ((arg1)->count);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_strip_type_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_strip_type_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_strip_type_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_strip_type_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_strip_type_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_strip_type_set" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   if (arg1) (arg1)->strip_type = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_strip_type_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   int result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_strip_type_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_strip_type_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_strip_type_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (int) ((arg1)->strip_type);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_leds_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   ws2811_led_t *arg2 = (ws2811_led_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   void *argp2 = 0 ;
   int res2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_leds_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_leds_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_leds_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_leds_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  res2 = SWIG_ConvertPtr(obj1, &argp2,SWIGTYPE_p_unsigned_int, SWIG_POINTER_DISOWN |  0 );
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_unsigned_int, SWIG_POINTER_DISOWN |  0 );
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ws2811_channel_t_leds_set" "', argument " "2"" of type '" "ws2811_led_t *""'"); 
   }
   arg2 = (ws2811_led_t *)(argp2);
   if (arg1) (arg1)->leds = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_leds_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   ws2811_led_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_leds_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_leds_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_leds_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (ws2811_led_t *) ((arg1)->leds);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_unsigned_int, 0 |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_brightness_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   uint8_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned char val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_brightness_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_brightness_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_brightness_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_brightness_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_char(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_char(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_brightness_set" "', argument " "2"" of type '" "uint8_t""'");
   } 
   arg2 = (uint8_t)(val2);
   if (arg1) (arg1)->brightness = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_brightness_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint8_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_brightness_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_brightness_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_brightness_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (uint8_t) ((arg1)->brightness);
   resultobj = SWIG_From_unsigned_SS_char((unsigned char)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_wshift_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   uint8_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned char val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_wshift_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_wshift_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_wshift_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_wshift_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_char(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_char(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_wshift_set" "', argument " "2"" of type '" "uint8_t""'");
   } 
   arg2 = (uint8_t)(val2);
   if (arg1) (arg1)->wshift = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_wshift_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint8_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_wshift_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_wshift_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_wshift_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (uint8_t) ((arg1)->wshift);
   resultobj = SWIG_From_unsigned_SS_char((unsigned char)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_rshift_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   uint8_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned char val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_rshift_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_rshift_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_rshift_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_rshift_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_char(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_char(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_rshift_set" "', argument " "2"" of type '" "uint8_t""'");
   } 
   arg2 = (uint8_t)(val2);
   if (arg1) (arg1)->rshift = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_rshift_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint8_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_rshift_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_rshift_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_rshift_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (uint8_t) ((arg1)->rshift);
   resultobj = SWIG_From_unsigned_SS_char((unsigned char)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_gshift_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   uint8_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned char val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_gshift_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_gshift_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gshift_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gshift_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_char(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_char(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_gshift_set" "', argument " "2"" of type '" "uint8_t""'");
   } 
   arg2 = (uint8_t)(val2);
   if (arg1) (arg1)->gshift = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_gshift_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint8_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_gshift_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gshift_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gshift_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (uint8_t) ((arg1)->gshift);
   resultobj = SWIG_From_unsigned_SS_char((unsigned char)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_bshift_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   uint8_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned char val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_bshift_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_bshift_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_bshift_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_bshift_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_char(obj1, &val2);
+  arg1 = (struct ws2811_channel_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_char(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_t_bshift_set" "', argument " "2"" of type '" "uint8_t""'");
   } 
   arg2 = (uint8_t)(val2);
   if (arg1) (arg1)->bshift = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_bshift_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint8_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_bshift_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_bshift_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_bshift_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (uint8_t) ((arg1)->bshift);
   resultobj = SWIG_From_unsigned_SS_char((unsigned char)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_gamma_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   uint8_t *arg2 = (uint8_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_t_gamma_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_t_gamma_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gamma_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gamma_set" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   {
     /* As a consequence of this malloc, I believe there's a potential memory leak
        /  which would occur if gamma is set more than once.
        /  The gamma value is only freed once at cleanup.
        /  Using a typemap is also risky here, since it would apply to all *uint8_t,
        /  this type is presently only used for the gamma table.
        */
     arg2 = malloc(sizeof(uint8_t) * 256);
-    if (!convert_iarray(obj1,arg2,256)) {
+    if (!convert_iarray(swig_obj[1],arg2,256)) {
       return NULL;
     }
   }
   if (arg1) (arg1)->gamma = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_channel_t_gamma_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint8_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_channel_t_gamma_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gamma_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_t_gamma_get" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   result = (uint8_t *) ((arg1)->gamma);
   {
     resultobj = PyList_New(256);
     int x;
     for(x = 0; x < 256; x++){
       PyList_SetItem(resultobj, x, PyInt_FromLong(result[x]));
     }
@@ -3959,423 +3716,434 @@
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_new_ws2811_channel_t(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *result = 0 ;
+  struct ws2811_channel_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)":new_ws2811_channel_t")) SWIG_fail;
-  result = (ws2811_channel_t *)calloc(1, sizeof(ws2811_channel_t));
+  if (!SWIG_Python_UnpackTuple(args, "new_ws2811_channel_t", 0, 0, 0)) SWIG_fail;
+  result = (struct ws2811_channel_t *)calloc(1, sizeof(struct ws2811_channel_t));
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ws2811_channel_t, SWIG_POINTER_NEW |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_delete_ws2811_channel_t(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
+  struct ws2811_channel_t *arg1 = (struct ws2811_channel_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:delete_ws2811_channel_t",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, SWIG_POINTER_DISOWN |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, SWIG_POINTER_DISOWN |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ws2811_channel_t" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ws2811_channel_t" "', argument " "1"" of type '" "struct ws2811_channel_t *""'"); 
   }
-  arg1 = (ws2811_channel_t *)(argp1);
+  arg1 = (struct ws2811_channel_t *)(argp1);
   free((char *) arg1);
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *ws2811_channel_t_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *obj;
-  if (!PyArg_ParseTuple(args,(char*)"O:swigregister", &obj)) return NULL;
+  if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
   SWIG_TypeNewClientData(SWIGTYPE_p_ws2811_channel_t, SWIG_NewClientData(obj));
   return SWIG_Py_Void();
 }
 
+SWIGINTERN PyObject *ws2811_channel_t_swiginit(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  return SWIG_Python_InitShadowInstance(args);
+}
+
 SWIGINTERN PyObject *_wrap_ws2811_t_render_wait_time_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   uint64_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned long long val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_t_render_wait_time_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_t_render_wait_time_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_render_wait_time_set" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_render_wait_time_set" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_long_SS_long(obj1, &val2);
+  arg1 = (struct ws2811_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_long_SS_long(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_t_render_wait_time_set" "', argument " "2"" of type '" "uint64_t""'");
   } 
   arg2 = (uint64_t)(val2);
   if (arg1) (arg1)->render_wait_time = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_render_wait_time_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint64_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_t_render_wait_time_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_render_wait_time_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_render_wait_time_get" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   result = (uint64_t) ((arg1)->render_wait_time);
   resultobj = SWIG_From_unsigned_SS_long_SS_long((unsigned long long)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_device_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   struct ws2811_device *arg2 = (struct ws2811_device *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   void *argp2 = 0 ;
   int res2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_t_device_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_t_device_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_device_set" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_device_set" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
-  res2 = SWIG_ConvertPtr(obj1, &argp2,SWIGTYPE_p_ws2811_device, SWIG_POINTER_DISOWN |  0 );
+  arg1 = (struct ws2811_t *)(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_ws2811_device, SWIG_POINTER_DISOWN |  0 );
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ws2811_t_device_set" "', argument " "2"" of type '" "struct ws2811_device *""'"); 
   }
   arg2 = (struct ws2811_device *)(argp2);
   if (arg1) (arg1)->device = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_device_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   struct ws2811_device *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_t_device_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_device_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_device_get" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   result = (struct ws2811_device *) ((arg1)->device);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ws2811_device, 0 |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_rpi_hw_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   rpi_hw_t *arg2 = (rpi_hw_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   void *argp2 = 0 ;
   int res2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_t_rpi_hw_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_t_rpi_hw_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_rpi_hw_set" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_rpi_hw_set" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
-  res2 = SWIG_ConvertPtr(obj1, &argp2,SWIGTYPE_p_rpi_hw_t, SWIG_POINTER_DISOWN |  0 );
+  arg1 = (struct ws2811_t *)(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_rpi_hw_t, SWIG_POINTER_DISOWN |  0 );
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ws2811_t_rpi_hw_set" "', argument " "2"" of type '" "rpi_hw_t const *""'"); 
   }
   arg2 = (rpi_hw_t *)(argp2);
   if (arg1) (arg1)->rpi_hw = (rpi_hw_t const *)arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_rpi_hw_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   rpi_hw_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_t_rpi_hw_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_rpi_hw_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_rpi_hw_get" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   result = (rpi_hw_t *) ((arg1)->rpi_hw);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_rpi_hw_t, 0 |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_freq_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   uint32_t arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   unsigned int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_t_freq_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_t_freq_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_freq_set" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_freq_set" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
-  ecode2 = SWIG_AsVal_unsigned_SS_int(obj1, &val2);
+  arg1 = (struct ws2811_t *)(argp1);
+  ecode2 = SWIG_AsVal_unsigned_SS_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_t_freq_set" "', argument " "2"" of type '" "uint32_t""'");
   } 
   arg2 = (uint32_t)(val2);
   if (arg1) (arg1)->freq = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_freq_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   uint32_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_t_freq_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_freq_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_freq_get" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   result = (uint32_t) ((arg1)->freq);
   resultobj = SWIG_From_unsigned_SS_int((unsigned int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_dmanum_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_t_dmanum_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_t_dmanum_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_dmanum_set" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_dmanum_set" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  arg1 = (struct ws2811_t *)(argp1);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_t_dmanum_set" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   if (arg1) (arg1)->dmanum = arg2;
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_dmanum_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   int result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_t_dmanum_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_dmanum_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_dmanum_get" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   result = (int) ((arg1)->dmanum);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_channel_set(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   ws2811_channel_t *arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   void *argp2 = 0 ;
   int res2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_t_channel_set",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_t_channel_set", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_channel_set" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_channel_set" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
-  res2 = SWIG_ConvertPtr(obj1, &argp2,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  arg1 = (struct ws2811_t *)(argp1);
+  res2 = SWIG_ConvertPtr(swig_obj[1], &argp2,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res2)) {
     SWIG_exception_fail(SWIG_ArgError(res2), "in method '" "ws2811_t_channel_set" "', argument " "2"" of type '" "ws2811_channel_t [RPI_PWM_CHANNELS]""'"); 
   } 
   arg2 = (ws2811_channel_t *)(argp2);
   {
     if (arg2) {
       size_t ii = 0;
-      for (; ii < (size_t)RPI_PWM_CHANNELS; ++ii) arg1->channel[ii] = arg2[ii];
+      for (; ii < (size_t)RPI_PWM_CHANNELS; ++ii) *(ws2811_channel_t *)&arg1->channel[ii] = *((ws2811_channel_t *)arg2 + ii);
     } else {
       SWIG_exception_fail(SWIG_ValueError, "invalid null reference " "in variable '""channel""' of type '""ws2811_channel_t [RPI_PWM_CHANNELS]""'");
     }
   }
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_ws2811_t_channel_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   ws2811_channel_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_t_channel_get",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_channel_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_t_channel_get" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   result = (ws2811_channel_t *)(ws2811_channel_t *) ((arg1)->channel);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_new_ws2811_t(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *result = 0 ;
+  struct ws2811_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)":new_ws2811_t")) SWIG_fail;
-  result = (ws2811_t *)calloc(1, sizeof(ws2811_t));
+  if (!SWIG_Python_UnpackTuple(args, "new_ws2811_t", 0, 0, 0)) SWIG_fail;
+  result = (struct ws2811_t *)calloc(1, sizeof(struct ws2811_t));
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ws2811_t, SWIG_POINTER_NEW |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *_wrap_delete_ws2811_t(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
-  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  struct ws2811_t *arg1 = (struct ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:delete_ws2811_t",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, SWIG_POINTER_DISOWN |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, SWIG_POINTER_DISOWN |  0 );
   if (!SWIG_IsOK(res1)) {
-    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ws2811_t" "', argument " "1"" of type '" "ws2811_t *""'"); 
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "delete_ws2811_t" "', argument " "1"" of type '" "struct ws2811_t *""'"); 
   }
-  arg1 = (ws2811_t *)(argp1);
+  arg1 = (struct ws2811_t *)(argp1);
   free((char *) arg1);
   resultobj = SWIG_Py_Void();
   return resultobj;
 fail:
   return NULL;
 }
 
 
 SWIGINTERN PyObject *ws2811_t_swigregister(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *obj;
-  if (!PyArg_ParseTuple(args,(char*)"O:swigregister", &obj)) return NULL;
+  if (!SWIG_Python_UnpackTuple(args, "swigregister", 1, 1, &obj)) return NULL;
   SWIG_TypeNewClientData(SWIGTYPE_p_ws2811_t, SWIG_NewClientData(obj));
   return SWIG_Py_Void();
 }
 
+SWIGINTERN PyObject *ws2811_t_swiginit(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  return SWIG_Python_InitShadowInstance(args);
+}
+
 SWIGINTERN PyObject *_wrap_ws2811_init(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   ws2811_t *arg1 = (ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   ws2811_return_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_init",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_init" "', argument " "1"" of type '" "ws2811_t *""'"); 
   }
   arg1 = (ws2811_t *)(argp1);
   result = (ws2811_return_t)ws2811_init(arg1);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
@@ -4385,18 +4153,19 @@
 
 
 SWIGINTERN PyObject *_wrap_ws2811_fini(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   ws2811_t *arg1 = (ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_fini",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_fini" "', argument " "1"" of type '" "ws2811_t *""'"); 
   }
   arg1 = (ws2811_t *)(argp1);
   ws2811_fini(arg1);
   resultobj = SWIG_Py_Void();
   return resultobj;
@@ -4406,19 +4175,20 @@
 
 
 SWIGINTERN PyObject *_wrap_ws2811_render(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   ws2811_t *arg1 = (ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   ws2811_return_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_render",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_render" "', argument " "1"" of type '" "ws2811_t *""'"); 
   }
   arg1 = (ws2811_t *)(argp1);
   result = (ws2811_return_t)ws2811_render(arg1);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
@@ -4428,19 +4198,20 @@
 
 
 SWIGINTERN PyObject *_wrap_ws2811_wait(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   ws2811_t *arg1 = (ws2811_t *) 0 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   ws2811_return_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_wait",&obj0)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_wait" "', argument " "1"" of type '" "ws2811_t *""'"); 
   }
   arg1 = (ws2811_t *)(argp1);
   result = (ws2811_return_t)ws2811_wait(arg1);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
@@ -4450,50 +4221,79 @@
 
 
 SWIGINTERN PyObject *_wrap_ws2811_get_return_t_str(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   ws2811_return_t arg1 ;
   int val1 ;
   int ecode1 = 0 ;
-  PyObject * obj0 = 0 ;
+  PyObject *swig_obj[1] ;
   char *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"O:ws2811_get_return_t_str",&obj0)) SWIG_fail;
-  ecode1 = SWIG_AsVal_int(obj0, &val1);
+  if (!args) SWIG_fail;
+  swig_obj[0] = args;
+  ecode1 = SWIG_AsVal_int(swig_obj[0], &val1);
   if (!SWIG_IsOK(ecode1)) {
     SWIG_exception_fail(SWIG_ArgError(ecode1), "in method '" "ws2811_get_return_t_str" "', argument " "1"" of type '" "ws2811_return_t""'");
   } 
   arg1 = (ws2811_return_t)(val1);
   result = (char *)ws2811_get_return_t_str(arg1);
   resultobj = SWIG_FromCharPtr((const char *)result);
   return resultobj;
 fail:
   return NULL;
 }
 
 
+SWIGINTERN PyObject *_wrap_ws2811_set_custom_gamma_factor(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
+  PyObject *resultobj = 0;
+  ws2811_t *arg1 = (ws2811_t *) 0 ;
+  double arg2 ;
+  void *argp1 = 0 ;
+  int res1 = 0 ;
+  double val2 ;
+  int ecode2 = 0 ;
+  PyObject *swig_obj[2] ;
+  
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_set_custom_gamma_factor", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_IsOK(res1)) {
+    SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_set_custom_gamma_factor" "', argument " "1"" of type '" "ws2811_t *""'"); 
+  }
+  arg1 = (ws2811_t *)(argp1);
+  ecode2 = SWIG_AsVal_double(swig_obj[1], &val2);
+  if (!SWIG_IsOK(ecode2)) {
+    SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_set_custom_gamma_factor" "', argument " "2"" of type '" "double""'");
+  } 
+  arg2 = (double)(val2);
+  ws2811_set_custom_gamma_factor(arg1,arg2);
+  resultobj = SWIG_Py_Void();
+  return resultobj;
+fail:
+  return NULL;
+}
+
+
 SWIGINTERN PyObject *_wrap_ws2811_led_get(PyObject *SWIGUNUSEDPARM(self), PyObject *args) {
   PyObject *resultobj = 0;
   ws2811_channel_t *arg1 = (ws2811_channel_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   uint32_t result;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_led_get",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_led_get", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_led_get" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
   }
   arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_led_get" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   result = (uint32_t)ws2811_led_get(arg1,arg2);
   resultobj = SWIG_From_unsigned_SS_int((unsigned int)(result));
   return resultobj;
@@ -4509,31 +4309,29 @@
   uint32_t arg3 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
   unsigned int val3 ;
   int ecode3 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
-  PyObject * obj2 = 0 ;
+  PyObject *swig_obj[3] ;
   int result;
   
-  if (!PyArg_ParseTuple(args,(char *)"OOO:ws2811_led_set",&obj0,&obj1,&obj2)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_led_set", 3, 3, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_led_set" "', argument " "1"" of type '" "ws2811_channel_t *""'"); 
   }
   arg1 = (ws2811_channel_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_led_set" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
-  ecode3 = SWIG_AsVal_unsigned_SS_int(obj2, &val3);
+  ecode3 = SWIG_AsVal_unsigned_SS_int(swig_obj[2], &val3);
   if (!SWIG_IsOK(ecode3)) {
     SWIG_exception_fail(SWIG_ArgError(ecode3), "in method '" "ws2811_led_set" "', argument " "3"" of type '" "uint32_t""'");
   } 
   arg3 = (uint32_t)(val3);
   result = (int)ws2811_led_set(arg1,arg2,arg3);
   resultobj = SWIG_From_int((int)(result));
   return resultobj;
@@ -4546,87 +4344,93 @@
   PyObject *resultobj = 0;
   ws2811_t *arg1 = (ws2811_t *) 0 ;
   int arg2 ;
   void *argp1 = 0 ;
   int res1 = 0 ;
   int val2 ;
   int ecode2 = 0 ;
-  PyObject * obj0 = 0 ;
-  PyObject * obj1 = 0 ;
+  PyObject *swig_obj[2] ;
   ws2811_channel_t *result = 0 ;
   
-  if (!PyArg_ParseTuple(args,(char *)"OO:ws2811_channel_get",&obj0,&obj1)) SWIG_fail;
-  res1 = SWIG_ConvertPtr(obj0, &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
+  if (!SWIG_Python_UnpackTuple(args, "ws2811_channel_get", 2, 2, swig_obj)) SWIG_fail;
+  res1 = SWIG_ConvertPtr(swig_obj[0], &argp1,SWIGTYPE_p_ws2811_t, 0 |  0 );
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "ws2811_channel_get" "', argument " "1"" of type '" "ws2811_t *""'"); 
   }
   arg1 = (ws2811_t *)(argp1);
-  ecode2 = SWIG_AsVal_int(obj1, &val2);
+  ecode2 = SWIG_AsVal_int(swig_obj[1], &val2);
   if (!SWIG_IsOK(ecode2)) {
     SWIG_exception_fail(SWIG_ArgError(ecode2), "in method '" "ws2811_channel_get" "', argument " "2"" of type '" "int""'");
   } 
   arg2 = (int)(val2);
   result = (ws2811_channel_t *)ws2811_channel_get(arg1,arg2);
   resultobj = SWIG_NewPointerObj(SWIG_as_voidptr(result), SWIGTYPE_p_ws2811_channel_t, 0 |  0 );
   return resultobj;
 fail:
   return NULL;
 }
 
 
 static PyMethodDef SwigMethods[] = {
-	 { (char *)"SWIG_PyInstanceMethod_New", (PyCFunction)SWIG_PyInstanceMethod_New, METH_O, NULL},
-	 { (char *)"ws2811_channel_t_gpionum_set", _wrap_ws2811_channel_t_gpionum_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_gpionum_get", _wrap_ws2811_channel_t_gpionum_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_invert_set", _wrap_ws2811_channel_t_invert_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_invert_get", _wrap_ws2811_channel_t_invert_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_count_set", _wrap_ws2811_channel_t_count_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_count_get", _wrap_ws2811_channel_t_count_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_strip_type_set", _wrap_ws2811_channel_t_strip_type_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_strip_type_get", _wrap_ws2811_channel_t_strip_type_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_leds_set", _wrap_ws2811_channel_t_leds_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_leds_get", _wrap_ws2811_channel_t_leds_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_brightness_set", _wrap_ws2811_channel_t_brightness_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_brightness_get", _wrap_ws2811_channel_t_brightness_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_wshift_set", _wrap_ws2811_channel_t_wshift_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_wshift_get", _wrap_ws2811_channel_t_wshift_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_rshift_set", _wrap_ws2811_channel_t_rshift_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_rshift_get", _wrap_ws2811_channel_t_rshift_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_gshift_set", _wrap_ws2811_channel_t_gshift_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_gshift_get", _wrap_ws2811_channel_t_gshift_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_bshift_set", _wrap_ws2811_channel_t_bshift_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_bshift_get", _wrap_ws2811_channel_t_bshift_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_gamma_set", _wrap_ws2811_channel_t_gamma_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_gamma_get", _wrap_ws2811_channel_t_gamma_get, METH_VARARGS, NULL},
-	 { (char *)"new_ws2811_channel_t", _wrap_new_ws2811_channel_t, METH_VARARGS, NULL},
-	 { (char *)"delete_ws2811_channel_t", _wrap_delete_ws2811_channel_t, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_t_swigregister", ws2811_channel_t_swigregister, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_render_wait_time_set", _wrap_ws2811_t_render_wait_time_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_render_wait_time_get", _wrap_ws2811_t_render_wait_time_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_device_set", _wrap_ws2811_t_device_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_device_get", _wrap_ws2811_t_device_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_rpi_hw_set", _wrap_ws2811_t_rpi_hw_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_rpi_hw_get", _wrap_ws2811_t_rpi_hw_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_freq_set", _wrap_ws2811_t_freq_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_freq_get", _wrap_ws2811_t_freq_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_dmanum_set", _wrap_ws2811_t_dmanum_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_dmanum_get", _wrap_ws2811_t_dmanum_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_channel_set", _wrap_ws2811_t_channel_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_channel_get", _wrap_ws2811_t_channel_get, METH_VARARGS, NULL},
-	 { (char *)"new_ws2811_t", _wrap_new_ws2811_t, METH_VARARGS, NULL},
-	 { (char *)"delete_ws2811_t", _wrap_delete_ws2811_t, METH_VARARGS, NULL},
-	 { (char *)"ws2811_t_swigregister", ws2811_t_swigregister, METH_VARARGS, NULL},
-	 { (char *)"ws2811_init", _wrap_ws2811_init, METH_VARARGS, NULL},
-	 { (char *)"ws2811_fini", _wrap_ws2811_fini, METH_VARARGS, NULL},
-	 { (char *)"ws2811_render", _wrap_ws2811_render, METH_VARARGS, NULL},
-	 { (char *)"ws2811_wait", _wrap_ws2811_wait, METH_VARARGS, NULL},
-	 { (char *)"ws2811_get_return_t_str", _wrap_ws2811_get_return_t_str, METH_VARARGS, NULL},
-	 { (char *)"ws2811_led_get", _wrap_ws2811_led_get, METH_VARARGS, NULL},
-	 { (char *)"ws2811_led_set", _wrap_ws2811_led_set, METH_VARARGS, NULL},
-	 { (char *)"ws2811_channel_get", _wrap_ws2811_channel_get, METH_VARARGS, NULL},
+	 { "SWIG_PyInstanceMethod_New", SWIG_PyInstanceMethod_New, METH_O, NULL},
+	 { "ws2811_channel_t_gpionum_set", _wrap_ws2811_channel_t_gpionum_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_gpionum_get", _wrap_ws2811_channel_t_gpionum_get, METH_O, NULL},
+	 { "ws2811_channel_t_invert_set", _wrap_ws2811_channel_t_invert_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_invert_get", _wrap_ws2811_channel_t_invert_get, METH_O, NULL},
+	 { "ws2811_channel_t_count_set", _wrap_ws2811_channel_t_count_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_count_get", _wrap_ws2811_channel_t_count_get, METH_O, NULL},
+	 { "ws2811_channel_t_strip_type_set", _wrap_ws2811_channel_t_strip_type_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_strip_type_get", _wrap_ws2811_channel_t_strip_type_get, METH_O, NULL},
+	 { "ws2811_channel_t_leds_set", _wrap_ws2811_channel_t_leds_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_leds_get", _wrap_ws2811_channel_t_leds_get, METH_O, NULL},
+	 { "ws2811_channel_t_brightness_set", _wrap_ws2811_channel_t_brightness_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_brightness_get", _wrap_ws2811_channel_t_brightness_get, METH_O, NULL},
+	 { "ws2811_channel_t_wshift_set", _wrap_ws2811_channel_t_wshift_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_wshift_get", _wrap_ws2811_channel_t_wshift_get, METH_O, NULL},
+	 { "ws2811_channel_t_rshift_set", _wrap_ws2811_channel_t_rshift_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_rshift_get", _wrap_ws2811_channel_t_rshift_get, METH_O, NULL},
+	 { "ws2811_channel_t_gshift_set", _wrap_ws2811_channel_t_gshift_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_gshift_get", _wrap_ws2811_channel_t_gshift_get, METH_O, NULL},
+	 { "ws2811_channel_t_bshift_set", _wrap_ws2811_channel_t_bshift_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_bshift_get", _wrap_ws2811_channel_t_bshift_get, METH_O, NULL},
+	 { "ws2811_channel_t_gamma_set", _wrap_ws2811_channel_t_gamma_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_t_gamma_get", _wrap_ws2811_channel_t_gamma_get, METH_O, NULL},
+	 { "new_ws2811_channel_t", _wrap_new_ws2811_channel_t, METH_NOARGS, NULL},
+	 { "delete_ws2811_channel_t", _wrap_delete_ws2811_channel_t, METH_O, NULL},
+	 { "ws2811_channel_t_swigregister", ws2811_channel_t_swigregister, METH_O, NULL},
+	 { "ws2811_channel_t_swiginit", ws2811_channel_t_swiginit, METH_VARARGS, NULL},
+	 { "ws2811_t_render_wait_time_set", _wrap_ws2811_t_render_wait_time_set, METH_VARARGS, NULL},
+	 { "ws2811_t_render_wait_time_get", _wrap_ws2811_t_render_wait_time_get, METH_O, NULL},
+	 { "ws2811_t_device_set", _wrap_ws2811_t_device_set, METH_VARARGS, NULL},
+	 { "ws2811_t_device_get", _wrap_ws2811_t_device_get, METH_O, NULL},
+	 { "ws2811_t_rpi_hw_set", _wrap_ws2811_t_rpi_hw_set, METH_VARARGS, NULL},
+	 { "ws2811_t_rpi_hw_get", _wrap_ws2811_t_rpi_hw_get, METH_O, NULL},
+	 { "ws2811_t_freq_set", _wrap_ws2811_t_freq_set, METH_VARARGS, NULL},
+	 { "ws2811_t_freq_get", _wrap_ws2811_t_freq_get, METH_O, NULL},
+	 { "ws2811_t_dmanum_set", _wrap_ws2811_t_dmanum_set, METH_VARARGS, NULL},
+	 { "ws2811_t_dmanum_get", _wrap_ws2811_t_dmanum_get, METH_O, NULL},
+	 { "ws2811_t_channel_set", _wrap_ws2811_t_channel_set, METH_VARARGS, NULL},
+	 { "ws2811_t_channel_get", _wrap_ws2811_t_channel_get, METH_O, NULL},
+	 { "new_ws2811_t", _wrap_new_ws2811_t, METH_NOARGS, NULL},
+	 { "delete_ws2811_t", _wrap_delete_ws2811_t, METH_O, NULL},
+	 { "ws2811_t_swigregister", ws2811_t_swigregister, METH_O, NULL},
+	 { "ws2811_t_swiginit", ws2811_t_swiginit, METH_VARARGS, NULL},
+	 { "ws2811_init", _wrap_ws2811_init, METH_O, NULL},
+	 { "ws2811_fini", _wrap_ws2811_fini, METH_O, NULL},
+	 { "ws2811_render", _wrap_ws2811_render, METH_O, NULL},
+	 { "ws2811_wait", _wrap_ws2811_wait, METH_O, NULL},
+	 { "ws2811_get_return_t_str", _wrap_ws2811_get_return_t_str, METH_O, NULL},
+	 { "ws2811_set_custom_gamma_factor", _wrap_ws2811_set_custom_gamma_factor, METH_VARARGS, NULL},
+	 { "ws2811_led_get", _wrap_ws2811_led_get, METH_VARARGS, NULL},
+	 { "ws2811_led_set", _wrap_ws2811_led_set, METH_VARARGS, NULL},
+	 { "ws2811_channel_get", _wrap_ws2811_channel_get, METH_VARARGS, NULL},
+	 { NULL, NULL, 0, NULL }
+};
+
+static PyMethodDef SwigMethods_proxydocs[] = {
 	 { NULL, NULL, 0, NULL }
 };
 
 
 /* -------- TYPE CONVERSION AND EQUIVALENCE RULES (BEGIN) -------- */
 
 static swig_type_info _swigt__p_char = {"_p_char", "char *", 0, 0, (void*)0, 0};
@@ -4635,18 +4439,18 @@
 static swig_type_info _swigt__p_rpi_hw_t = {"_p_rpi_hw_t", "rpi_hw_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_short = {"_p_short", "short *|int_least16_t *|int16_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_signed_char = {"_p_signed_char", "signed char *|int_least8_t *|int_fast8_t *|int8_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_unsigned_char = {"_p_unsigned_char", "unsigned char *|uint_least8_t *|uint_fast8_t *|uint8_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_unsigned_int = {"_p_unsigned_int", "uintptr_t *|uint_least32_t *|uint_fast32_t *|uint32_t *|unsigned int *|ws2811_led_t *|uint_fast16_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_unsigned_long_long = {"_p_unsigned_long_long", "uint_least64_t *|uint_fast64_t *|uint64_t *|unsigned long long *|uintmax_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_unsigned_short = {"_p_unsigned_short", "unsigned short *|uint_least16_t *|uint16_t *", 0, 0, (void*)0, 0};
-static swig_type_info _swigt__p_ws2811_channel_t = {"_p_ws2811_channel_t", "ws2811_channel_t *", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_ws2811_channel_t = {"_p_ws2811_channel_t", "struct ws2811_channel_t *|ws2811_channel_t *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_ws2811_device = {"_p_ws2811_device", "struct ws2811_device *", 0, 0, (void*)0, 0};
 static swig_type_info _swigt__p_ws2811_return_t = {"_p_ws2811_return_t", "enum ws2811_return_t *|ws2811_return_t *", 0, 0, (void*)0, 0};
-static swig_type_info _swigt__p_ws2811_t = {"_p_ws2811_t", "ws2811_t *", 0, 0, (void*)0, 0};
+static swig_type_info _swigt__p_ws2811_t = {"_p_ws2811_t", "struct ws2811_t *|ws2811_t *", 0, 0, (void*)0, 0};
 
 static swig_type_info *swig_type_initial[] = {
   &_swigt__p_char,
   &_swigt__p_int,
   &_swigt__p_long_long,
   &_swigt__p_rpi_hw_t,
   &_swigt__p_short,
@@ -4711,15 +4515,15 @@
  * The idea is that swig generates all the structures that are needed.
  * The runtime then collects these partially filled structures.
  * The SWIG_InitializeModule function takes these initial arrays out of
  * swig_module, and does all the lookup, filling in the swig_module.types
  * array with the correct data and linking the correct swig_cast_info
  * structures together.
  *
- * The generated swig_type_info structures are assigned staticly to an initial
+ * The generated swig_type_info structures are assigned statically to an initial
  * array. We just loop through that array, and handle each type individually.
  * First we lookup if this type has been already loaded, and if so, use the
  * loaded structure instead of the generated one. Then we have to fill in the
  * cast linked list. The cast data is initially stored in something like a
  * two-dimensional array. Each row corresponds to a type (there are the same
  * number of rows as there are in the swig_type_initial array). Each entry in
  * a column is one of the swig_cast_info structures for that type.
@@ -4755,15 +4559,15 @@
 #endif
 
 
 SWIGRUNTIME void
 SWIG_InitializeModule(void *clientdata) {
   size_t i;
   swig_module_info *module_head, *iter;
-  int found, init;
+  int init;
   
   /* check to see if the circular list has been setup, if not, set it up */
   if (swig_module.next==0) {
     /* Initialize the swig_module */
     swig_module.type_initial = swig_type_initial;
     swig_module.cast_initial = swig_cast_initial;
     swig_module.next = &swig_module;
@@ -4774,51 +4578,47 @@
   
   /* Try and load any already created modules */
   module_head = SWIG_GetModule(clientdata);
   if (!module_head) {
     /* This is the first module loaded for this interpreter */
     /* so set the swig module into the interpreter */
     SWIG_SetModule(clientdata, &swig_module);
-    module_head = &swig_module;
   } else {
     /* the interpreter has loaded a SWIG module, but has it loaded this one? */
-    found=0;
     iter=module_head;
     do {
       if (iter==&swig_module) {
-        found=1;
-        break;
+        /* Our module is already in the list, so there's nothing more to do. */
+        return;
       }
       iter=iter->next;
     } while (iter!= module_head);
     
-    /* if the is found in the list, then all is done and we may leave */
-    if (found) return;
-    /* otherwise we must add out module into the list */
+    /* otherwise we must add our module into the list */
     swig_module.next = module_head->next;
     module_head->next = &swig_module;
   }
   
   /* When multiple interpreters are used, a module could have already been initialized in
        a different interpreter, but not yet have a pointer in this interpreter.
        In this case, we do not want to continue adding types... everything should be
        set up already */
   if (init == 0) return;
   
   /* Now work on filling in swig_module.types */
 #ifdef SWIGRUNTIME_DEBUG
-  printf("SWIG_InitializeModule: size %d\n", swig_module.size);
+  printf("SWIG_InitializeModule: size %lu\n", (unsigned long)swig_module.size);
 #endif
   for (i = 0; i < swig_module.size; ++i) {
     swig_type_info *type = 0;
     swig_type_info *ret;
     swig_cast_info *cast;
     
 #ifdef SWIGRUNTIME_DEBUG
-    printf("SWIG_InitializeModule: type %d %s\n", i, swig_module.type_initial[i]->name);
+    printf("SWIG_InitializeModule: type %lu %s\n", (unsigned long)i, swig_module.type_initial[i]->name);
 #endif
     
     /* if there is another module already loaded */
     if (swig_module.next != &swig_module) {
       type = SWIG_MangledTypeQueryModule(swig_module.next, &swig_module, swig_module.type_initial[i]->name);
     }
     if (type) {
@@ -4885,15 +4685,15 @@
   swig_module.types[i] = 0;
   
 #ifdef SWIGRUNTIME_DEBUG
   printf("**** SWIG_InitializeModule: Cast List ******\n");
   for (i = 0; i < swig_module.size; ++i) {
     int j = 0;
     swig_cast_info *cast = swig_module.cast_initial[i];
-    printf("SWIG_InitializeModule: type %d %s\n", i, swig_module.type_initial[i]->name);
+    printf("SWIG_InitializeModule: type %lu %s\n", (unsigned long)i, swig_module.type_initial[i]->name);
     while (cast->type) {
       printf("SWIG_InitializeModule: cast type %s\n", cast->type->name);
       cast++;
       ++j;
     }
     printf("---- Total casts: %d\n",j);
   }
@@ -5007,25 +4807,14 @@
       if (var->next) PyString_ConcatAndDel(&str,PyString_FromString(", "));
     }
     PyString_ConcatAndDel(&str,PyString_FromString(")"));
 #endif
     return str;
   }
   
-  SWIGINTERN int
-  swig_varlink_print(swig_varlinkobject *v, FILE *fp, int SWIGUNUSEDPARM(flags)) {
-    char *tmp;
-    PyObject *str = swig_varlink_str(v);
-    fprintf(fp,"Swig global variables ");
-    fprintf(fp,"%s\n", tmp = SWIG_Python_str_AsChar(str));
-    SWIG_Python_str_DelForPy3(tmp);
-    Py_DECREF(str);
-    return 0;
-  }
-  
   SWIGINTERN void
   swig_varlink_dealloc(swig_varlinkobject *v) {
     swig_globalvar *var = v->vars;
     while (var) {
       swig_globalvar *n = var->next;
       free(var->name);
       free(var);
@@ -5041,15 +4830,15 @@
       if (strcmp(var->name,n) == 0) {
         res = (*var->get_attr)();
         break;
       }
       var = var->next;
     }
     if (res == NULL && !PyErr_Occurred()) {
-      PyErr_SetString(PyExc_NameError,"Unknown C global variable");
+      PyErr_Format(PyExc_AttributeError, "Unknown C global variable '%s'", n);
     }
     return res;
   }
   
   SWIGINTERN int
   swig_varlink_setattr(swig_varlinkobject *v, char *n, PyObject *p) {
     int res = 1;
@@ -5058,38 +4847,37 @@
       if (strcmp(var->name,n) == 0) {
         res = (*var->set_attr)(p);
         break;
       }
       var = var->next;
     }
     if (res == 1 && !PyErr_Occurred()) {
-      PyErr_SetString(PyExc_NameError,"Unknown C global variable");
+      PyErr_Format(PyExc_AttributeError, "Unknown C global variable '%s'", n);
     }
     return res;
   }
   
   SWIGINTERN PyTypeObject*
   swig_varlink_type(void) {
     static char varlink__doc__[] = "Swig var link object";
     static PyTypeObject varlink_type;
     static int type_init = 0;
     if (!type_init) {
       const PyTypeObject tmp = {
-        /* PyObject header changed in Python 3 */
 #if PY_VERSION_HEX >= 0x03000000
         PyVarObject_HEAD_INIT(NULL, 0)
 #else
         PyObject_HEAD_INIT(NULL)
         0,                                  /* ob_size */
 #endif
-        (char *)"swigvarlink",              /* tp_name */
+        "swigvarlink",                      /* tp_name */
         sizeof(swig_varlinkobject),         /* tp_basicsize */
         0,                                  /* tp_itemsize */
         (destructor) swig_varlink_dealloc,  /* tp_dealloc */
-        (printfunc) swig_varlink_print,     /* tp_print */
+        0,                                  /* tp_print */
         (getattrfunc) swig_varlink_getattr, /* tp_getattr */
         (setattrfunc) swig_varlink_setattr, /* tp_setattr */
         0,                                  /* tp_compare */
         (reprfunc) swig_varlink_repr,       /* tp_repr */
         0,                                  /* tp_as_number */
         0,                                  /* tp_as_sequence */
         0,                                  /* tp_as_mapping */
@@ -5101,35 +4889,38 @@
         0,                                  /* tp_as_buffer */
         0,                                  /* tp_flags */
         varlink__doc__,                     /* tp_doc */
         0,                                  /* tp_traverse */
         0,                                  /* tp_clear */
         0,                                  /* tp_richcompare */
         0,                                  /* tp_weaklistoffset */
-#if PY_VERSION_HEX >= 0x02020000
         0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0, /* tp_iter -> tp_weaklist */
-#endif
-#if PY_VERSION_HEX >= 0x02030000
         0,                                  /* tp_del */
+        0,                                  /* tp_version_tag */
+#if PY_VERSION_HEX >= 0x03040000
+        0,                                  /* tp_finalize */
 #endif
-#if PY_VERSION_HEX >= 0x02060000
-        0,                                  /* tp_version */
+#if PY_VERSION_HEX >= 0x03080000
+        0,                                  /* tp_vectorcall */
+#endif
+#if (PY_VERSION_HEX >= 0x03080000) && (PY_VERSION_HEX < 0x03090000)
+        0,                                  /* tp_print */
 #endif
 #ifdef COUNT_ALLOCS
-        0,0,0,0                             /* tp_alloc -> tp_next */
+        0,                                  /* tp_allocs */
+        0,                                  /* tp_frees */
+        0,                                  /* tp_maxalloc */
+        0,                                  /* tp_prev */
+        0                                   /* tp_next */
 #endif
       };
       varlink_type = tmp;
       type_init = 1;
-#if PY_VERSION_HEX < 0x02020000
-      varlink_type.ob_type = &PyType_Type;
-#else
       if (PyType_Ready(&varlink_type) < 0)
       return NULL;
-#endif
     }
     return &varlink_type;
   }
   
   /* Create a variable linking object for use later */
   SWIGINTERN PyObject *
   SWIG_Python_newvarlink(void) {
@@ -5137,35 +4928,37 @@
     if (result) {
       result->vars = 0;
     }
     return ((PyObject*) result);
   }
   
   SWIGINTERN void 
-  SWIG_Python_addvarlink(PyObject *p, char *name, PyObject *(*get_attr)(void), int (*set_attr)(PyObject *p)) {
+  SWIG_Python_addvarlink(PyObject *p, const char *name, PyObject *(*get_attr)(void), int (*set_attr)(PyObject *p)) {
     swig_varlinkobject *v = (swig_varlinkobject *) p;
     swig_globalvar *gv = (swig_globalvar *) malloc(sizeof(swig_globalvar));
     if (gv) {
       size_t size = strlen(name)+1;
       gv->name = (char *)malloc(size);
       if (gv->name) {
-        strncpy(gv->name,name,size);
+        memcpy(gv->name, name, size);
         gv->get_attr = get_attr;
         gv->set_attr = set_attr;
         gv->next = v->vars;
       }
     }
     v->vars = gv;
   }
   
   SWIGINTERN PyObject *
   SWIG_globals(void) {
-    static PyObject *_SWIG_globals = 0; 
-    if (!_SWIG_globals) _SWIG_globals = SWIG_newvarlink();  
-    return _SWIG_globals;
+    static PyObject *globals = 0;
+    if (!globals) {
+      globals = SWIG_newvarlink();
+    }
+    return globals;
   }
   
   /* -----------------------------------------------------------------------------
    * constants/methods manipulation
    * ----------------------------------------------------------------------------- */
   
   /* Install Constants */
@@ -5200,15 +4993,17 @@
   SWIG_Python_FixMethods(PyMethodDef *methods,
     swig_const_info *const_table,
     swig_type_info **types,
     swig_type_info **types_initial) {
     size_t i;
     for (i = 0; methods[i].ml_name; ++i) {
       const char *c = methods[i].ml_doc;
-      if (c && (c = strstr(c, "swig_ptr: "))) {
+      if (!c) continue;
+      c = strstr(c, "swig_ptr: ");
+      if (c) {
         int j;
         swig_const_info *ci = 0;
         const char *name = c + 10;
         for (j = 0; const_table[j].type; ++j) {
           if (strncmp(const_table[j].name, name, 
               strlen(const_table[j].name)) == 0) {
             ci = &(const_table[j]);
@@ -5221,27 +5016,85 @@
             size_t shift = (ci->ptype) - types;
             swig_type_info *ty = types_initial[shift];
             size_t ldoc = (c - methods[i].ml_doc);
             size_t lptr = strlen(ty->name)+2*sizeof(void*)+2;
             char *ndoc = (char*)malloc(ldoc + lptr + 10);
             if (ndoc) {
               char *buff = ndoc;
-              strncpy(buff, methods[i].ml_doc, ldoc);
+              memcpy(buff, methods[i].ml_doc, ldoc);
               buff += ldoc;
-              strncpy(buff, "swig_ptr: ", 10);
+              memcpy(buff, "swig_ptr: ", 10);
               buff += 10;
               SWIG_PackVoidPtr(buff, ptr, ty->name, lptr);
               methods[i].ml_doc = ndoc;
             }
           }
         }
       }
     }
   } 
   
+  /* -----------------------------------------------------------------------------
+   * Method creation and docstring support functions
+   * ----------------------------------------------------------------------------- */
+  
+  /* -----------------------------------------------------------------------------
+   * Function to find the method definition with the correct docstring for the
+   * proxy module as opposed to the low-level API
+   * ----------------------------------------------------------------------------- */
+  
+  SWIGINTERN PyMethodDef *SWIG_PythonGetProxyDoc(const char *name) {
+    /* Find the function in the modified method table */
+    size_t offset = 0;
+    int found = 0;
+    while (SwigMethods_proxydocs[offset].ml_meth != NULL) {
+      if (strcmp(SwigMethods_proxydocs[offset].ml_name, name) == 0) {
+        found = 1;
+        break;
+      }
+      offset++;
+    }
+    /* Use the copy with the modified docstring if available */
+    return found ? &SwigMethods_proxydocs[offset] : NULL;
+  }
+  
+  /* -----------------------------------------------------------------------------
+   * Wrapper of PyInstanceMethod_New() used in Python 3
+   * It is exported to the generated module, used for -fastproxy
+   * ----------------------------------------------------------------------------- */
+  
+  SWIGINTERN PyObject *SWIG_PyInstanceMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func) {
+    if (PyCFunction_Check(func)) {
+      PyCFunctionObject *funcobj = (PyCFunctionObject *)func;
+      PyMethodDef *ml = SWIG_PythonGetProxyDoc(funcobj->m_ml->ml_name);
+      if (ml)
+      func = PyCFunction_NewEx(ml, funcobj->m_self, funcobj->m_module);
+    }
+#if PY_VERSION_HEX >= 0x03000000
+    return PyInstanceMethod_New(func);
+#else
+    return PyMethod_New(func, NULL, NULL);
+#endif
+  }
+  
+  /* -----------------------------------------------------------------------------
+   * Wrapper of PyStaticMethod_New()
+   * It is exported to the generated module, used for -fastproxy
+   * ----------------------------------------------------------------------------- */
+  
+  SWIGINTERN PyObject *SWIG_PyStaticMethod_New(PyObject *SWIGUNUSEDPARM(self), PyObject *func) {
+    if (PyCFunction_Check(func)) {
+      PyCFunctionObject *funcobj = (PyCFunctionObject *)func;
+      PyMethodDef *ml = SWIG_PythonGetProxyDoc(funcobj->m_ml->ml_name);
+      if (ml)
+      func = PyCFunction_NewEx(ml, funcobj->m_self, funcobj->m_module);
+    }
+    return PyStaticMethod_New(func);
+  }
+  
 #ifdef __cplusplus
 }
 #endif
 
 /* -----------------------------------------------------------------------------*
  *  Partial Init method
  * -----------------------------------------------------------------------------*/
@@ -5253,28 +5106,20 @@
 SWIGEXPORT 
 #if PY_VERSION_HEX >= 0x03000000
 PyObject*
 #else
 void
 #endif
 SWIG_init(void) {
-  PyObject *m, *d, *md;
+  PyObject *m, *d, *md, *globals;
+  
 #if PY_VERSION_HEX >= 0x03000000
   static struct PyModuleDef SWIG_module = {
-# if PY_VERSION_HEX >= 0x03020000
     PyModuleDef_HEAD_INIT,
-# else
-    {
-      PyObject_HEAD_INIT(NULL)
-      NULL, /* m_init */
-      0,    /* m_index */
-      NULL, /* m_copy */
-    },
-# endif
-    (char *) SWIG_name,
+    SWIG_name,
     NULL,
     -1,
     SwigMethods,
     NULL,
     NULL,
     NULL,
     NULL
@@ -5285,70 +5130,80 @@
   static SwigPyClientData SwigPyObject_clientdata = {
     0, 0, 0, 0, 0, 0, 0
   };
   static PyGetSetDef this_getset_def = {
     (char *)"this", &SwigPyBuiltin_ThisClosure, NULL, NULL, NULL
   };
   static SwigPyGetSet thisown_getset_closure = {
-    (PyCFunction) SwigPyObject_own,
-    (PyCFunction) SwigPyObject_own
+    SwigPyObject_own,
+    SwigPyObject_own
   };
   static PyGetSetDef thisown_getset_def = {
     (char *)"thisown", SwigPyBuiltin_GetterClosure, SwigPyBuiltin_SetterClosure, NULL, &thisown_getset_closure
   };
-  PyObject *metatype_args;
   PyTypeObject *builtin_pytype;
   int builtin_base_count;
   swig_type_info *builtin_basetype;
   PyObject *tuple;
   PyGetSetDescrObject *static_getset;
   PyTypeObject *metatype;
+  PyTypeObject *swigpyobject;
   SwigPyClientData *cd;
   PyObject *public_interface, *public_symbol;
   PyObject *this_descr;
   PyObject *thisown_descr;
+  PyObject *self = 0;
   int i;
   
   (void)builtin_pytype;
   (void)builtin_base_count;
   (void)builtin_basetype;
   (void)tuple;
   (void)static_getset;
+  (void)self;
   
-  /* metatype is used to implement static member variables. */
-  metatype_args = Py_BuildValue("(s(O){})", "SwigPyObjectType", &PyType_Type);
-  assert(metatype_args);
-  metatype = (PyTypeObject *) PyType_Type.tp_call((PyObject *) &PyType_Type, metatype_args, NULL);
+  /* Metaclass is used to implement static member variables */
+  metatype = SwigPyObjectType();
   assert(metatype);
-  Py_DECREF(metatype_args);
-  metatype->tp_setattro = (setattrofunc) &SwigPyObjectType_setattro;
-  assert(PyType_Ready(metatype) >= 0);
+#endif
+  
+  (void)globals;
+  
+  /* Create singletons now to avoid potential deadlocks with multi-threaded usage after module initialization */
+  SWIG_This();
+  SWIG_Python_TypeCache();
+  SwigPyPacked_type();
+#ifndef SWIGPYTHON_BUILTIN
+  SwigPyObject_type();
 #endif
   
   /* Fix SwigMethods to carry the callback ptrs when needed */
   SWIG_Python_FixMethods(SwigMethods, swig_const_table, swig_types, swig_type_initial);
   
 #if PY_VERSION_HEX >= 0x03000000
   m = PyModule_Create(&SWIG_module);
 #else
-  m = Py_InitModule((char *) SWIG_name, SwigMethods);
+  m = Py_InitModule(SWIG_name, SwigMethods);
 #endif
+  
   md = d = PyModule_GetDict(m);
   (void)md;
   
   SWIG_InitializeModule(0);
   
 #ifdef SWIGPYTHON_BUILTIN
+  swigpyobject = SwigPyObject_TypeOnce();
+  
   SwigPyObject_stype = SWIG_MangledTypeQuery("_p_SwigPyObject");
   assert(SwigPyObject_stype);
   cd = (SwigPyClientData*) SwigPyObject_stype->clientdata;
   if (!cd) {
     SwigPyObject_stype->clientdata = &SwigPyObject_clientdata;
-    SwigPyObject_clientdata.pytype = SwigPyObject_TypeOnce();
-  } else if (SwigPyObject_TypeOnce()->tp_basicsize != cd->pytype->tp_basicsize) {
+    SwigPyObject_clientdata.pytype = swigpyobject;
+  } else if (swigpyobject->tp_basicsize != cd->pytype->tp_basicsize) {
     PyErr_SetString(PyExc_RuntimeError, "Import error: attempted to load two incompatible swig-generated modules.");
 # if PY_VERSION_HEX >= 0x03000000
     return NULL;
 # else
     return;
 # endif
   }
```

### Comparing `rpi_ws281x-4.3.4/setup.py` & `rpi_ws281x-5.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,32 @@
 from setuptools.command.build_py import build_py
 
 class CustomInstallCommand(build_py):
     def run(self):
         print("Compiling ws281x library...")
         build_py.run(self)
 
+classifiers = ['Development Status :: 4 - Beta',
+               'Operating System :: POSIX :: Linux',
+               'License :: OSI Approved :: MIT License',
+               'Intended Audience :: Developers',
+               'Programming Language :: Python :: 3',
+               'Topic :: Software Development',
+               'Topic :: System :: Hardware']
+
 setup(name              = 'rpi_ws281x',
-      version           = '4.3.4',
+      version           = '5.0.0',
       author            = 'Jeremy Garff <jer@jers.net>, Phil Howard <phil@pimoroni.com>',
       author_email      = 'jer@jers.net, phil@pimoroni.com',
       description       = 'Userspace Raspberry Pi PWM/PCM/SPI library for SK6812 and WS281X LEDs.',
-      long_description  = open('README.rst').read() + "\n" + open('CHANGELOG.txt').read(),
+      long_description  = open('README.rst').read() + "\n\n" + open('CHANGELOG.txt').read(),
       license           = 'MIT',
       url               = 'https://github.com/rpi-ws281x/rpi-ws281x-python/',
+      classifiers       = classifiers,
+      python_requires   = '>=3.6',
       cmdclass          = {'build_py':CustomInstallCommand},
       packages          = ['rpi_ws281x'],
       ext_modules       = [Extension('_rpi_ws281x',
                                      include_dirs = ['.'],
                                      sources = ['rpi_ws281x_wrap.c',
                                               'lib/dma.c',
                                               'lib/mailbox.c',
```

