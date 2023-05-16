# Comparing `tmp/types-circuitpython-8.0.0b6.tar.gz` & `tmp/types-circuitpython-8.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-circuitpython-8.0.0b6.tar", last modified: Tue May 16 15:34:37 2023, max compression
+gzip compressed data, was "types-circuitpython-8.0.0rc0.tar", last modified: Tue May 16 15:35:32 2023, max compression
```

## Comparing `types-circuitpython-8.0.0b6.tar` & `types-circuitpython-8.0.0rc0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.261736 types-circuitpython-8.0.0b6/
--rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.0.0b6/LICENSE
--rw-r--r--   0 timon      (501) staff       (20)     2978 2023-05-16 15:34:37.260931 types-circuitpython-8.0.0b6/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     1921 2023-05-16 15:34:17.000000 types-circuitpython-8.0.0b6/README.md
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.122850 types-circuitpython-8.0.0b6/bindings/
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.126971 types-circuitpython-8.0.0b6/bindings/__future__/
--rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/__future__/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.127681 types-circuitpython-8.0.0b6/bindings/_bleio/
--rw-r--r--   0 timon      (501) staff       (20)    31068 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/_bleio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.128530 types-circuitpython-8.0.0b6/bindings/_eve/
--rw-r--r--   0 timon      (501) staff       (20)    20082 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/_eve/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.129468 types-circuitpython-8.0.0b6/bindings/_pew/
--rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/_pew/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.130258 types-circuitpython-8.0.0b6/bindings/_pixelmap/
--rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/_pixelmap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.130983 types-circuitpython-8.0.0b6/bindings/_stage/
--rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/_stage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.131675 types-circuitpython-8.0.0b6/bindings/adafruit_bus_device/
--rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.132294 types-circuitpython-8.0.0b6/bindings/adafruit_pixelbuf/
--rw-r--r--   0 timon      (501) staff       (20)     4190 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.132925 types-circuitpython-8.0.0b6/bindings/aesio/
--rw-r--r--   0 timon      (501) staff       (20)     2171 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/aesio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.133516 types-circuitpython-8.0.0b6/bindings/alarm/
--rw-r--r--   0 timon      (501) staff       (20)     7020 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/alarm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.134283 types-circuitpython-8.0.0b6/bindings/analogbufio/
--rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/analogbufio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.135371 types-circuitpython-8.0.0b6/bindings/analogio/
--rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/analogio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.136744 types-circuitpython-8.0.0b6/bindings/atexit/
--rw-r--r--   0 timon      (501) staff       (20)     1619 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/atexit/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.137634 types-circuitpython-8.0.0b6/bindings/audiobusio/
--rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/audiobusio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.138185 types-circuitpython-8.0.0b6/bindings/audiocore/
--rw-r--r--   0 timon      (501) staff       (20)     4614 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/audiocore/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.138654 types-circuitpython-8.0.0b6/bindings/audioio/
--rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:34:24.000000 types-circuitpython-8.0.0b6/bindings/audioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.139113 types-circuitpython-8.0.0b6/bindings/audiomixer/
--rw-r--r--   0 timon      (501) staff       (20)     4415 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/audiomixer/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.139570 types-circuitpython-8.0.0b6/bindings/audiomp3/
--rw-r--r--   0 timon      (501) staff       (20)     3897 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/audiomp3/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.140499 types-circuitpython-8.0.0b6/bindings/audiopwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4226 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/audiopwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.141225 types-circuitpython-8.0.0b6/bindings/bitbangio/
--rw-r--r--   0 timon      (501) staff       (20)    12038 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/bitbangio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.141839 types-circuitpython-8.0.0b6/bindings/bitmaptools/
--rw-r--r--   0 timon      (501) staff       (20)    10928 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/bitmaptools/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.142295 types-circuitpython-8.0.0b6/bindings/bitops/
--rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/bitops/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.142737 types-circuitpython-8.0.0b6/bindings/board/
--rw-r--r--   0 timon      (501) staff       (20)     1547 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/board/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.143176 types-circuitpython-8.0.0b6/bindings/busio/
--rw-r--r--   0 timon      (501) staff       (20)    19739 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/busio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.143646 types-circuitpython-8.0.0b6/bindings/camera/
--rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/camera/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.144006 types-circuitpython-8.0.0b6/bindings/canio/
--rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/canio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.144355 types-circuitpython-8.0.0b6/bindings/countio/
--rw-r--r--   0 timon      (501) staff       (20)     2782 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/countio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.144725 types-circuitpython-8.0.0b6/bindings/digitalio/
--rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/digitalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.145077 types-circuitpython-8.0.0b6/bindings/displayio/
--rw-r--r--   0 timon      (501) staff       (20)    38264 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/displayio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.145525 types-circuitpython-8.0.0b6/bindings/dualbank/
--rw-r--r--   0 timon      (501) staff       (20)     1224 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/dualbank/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.145870 types-circuitpython-8.0.0b6/bindings/floppyio/
--rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/floppyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.146222 types-circuitpython-8.0.0b6/bindings/fontio/
--rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/fontio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.146574 types-circuitpython-8.0.0b6/bindings/framebufferio/
--rw-r--r--   0 timon      (501) staff       (20)     3526 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/framebufferio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.209221 types-circuitpython-8.0.0b6/bindings/frequencyio/
--rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/frequencyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.210436 types-circuitpython-8.0.0b6/bindings/getpass/
--rw-r--r--   0 timon      (501) staff       (20)      546 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/getpass/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.211606 types-circuitpython-8.0.0b6/bindings/gifio/
--rw-r--r--   0 timon      (501) staff       (20)     1834 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/gifio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.212133 types-circuitpython-8.0.0b6/bindings/gnss/
--rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/gnss/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.212555 types-circuitpython-8.0.0b6/bindings/hashlib/
--rw-r--r--   0 timon      (501) staff       (20)     1002 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/hashlib/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.213145 types-circuitpython-8.0.0b6/bindings/i2ctarget/
--rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/i2ctarget/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.213657 types-circuitpython-8.0.0b6/bindings/imagecapture/
--rw-r--r--   0 timon      (501) staff       (20)     2886 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/imagecapture/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.214494 types-circuitpython-8.0.0b6/bindings/ipaddress/
--rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/ipaddress/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.215890 types-circuitpython-8.0.0b6/bindings/is31fl3741/
--rw-r--r--   0 timon      (501) staff       (20)     3868 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/is31fl3741/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.217043 types-circuitpython-8.0.0b6/bindings/keypad/
--rw-r--r--   0 timon      (501) staff       (20)    13070 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/keypad/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.217842 types-circuitpython-8.0.0b6/bindings/math/
--rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/math/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.218342 types-circuitpython-8.0.0b6/bindings/mdns/
--rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/mdns/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.218858 types-circuitpython-8.0.0b6/bindings/memorymap/
--rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:34:25.000000 types-circuitpython-8.0.0b6/bindings/memorymap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.219669 types-circuitpython-8.0.0b6/bindings/memorymonitor/
--rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/memorymonitor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.220233 types-circuitpython-8.0.0b6/bindings/microcontroller/
--rw-r--r--   0 timon      (501) staff       (20)     5928 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/microcontroller/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.220994 types-circuitpython-8.0.0b6/bindings/msgpack/
--rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/msgpack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.221630 types-circuitpython-8.0.0b6/bindings/neopixel_write/
--rw-r--r--   0 timon      (501) staff       (20)     1367 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/neopixel_write/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.222338 types-circuitpython-8.0.0b6/bindings/nvm/
--rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/nvm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.223022 types-circuitpython-8.0.0b6/bindings/onewireio/
--rw-r--r--   0 timon      (501) staff       (20)     1646 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/onewireio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.223882 types-circuitpython-8.0.0b6/bindings/os/
--rw-r--r--   0 timon      (501) staff       (20)     3776 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/os/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.226014 types-circuitpython-8.0.0b6/bindings/paralleldisplay/
--rw-r--r--   0 timon      (501) staff       (20)     2415 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.227466 types-circuitpython-8.0.0b6/bindings/ps2io/
--rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/ps2io/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.228595 types-circuitpython-8.0.0b6/bindings/pulseio/
--rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/pulseio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.230017 types-circuitpython-8.0.0b6/bindings/pwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4872 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/pwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.231167 types-circuitpython-8.0.0b6/bindings/qrio/
--rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/qrio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.232223 types-circuitpython-8.0.0b6/bindings/rainbowio/
--rw-r--r--   0 timon      (501) staff       (20)      327 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/rainbowio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.233189 types-circuitpython-8.0.0b6/bindings/random/
--rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/random/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.234027 types-circuitpython-8.0.0b6/bindings/rgbmatrix/
--rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.235027 types-circuitpython-8.0.0b6/bindings/rotaryio/
--rw-r--r--   0 timon      (501) staff       (20)     2659 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/rotaryio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.236694 types-circuitpython-8.0.0b6/bindings/rtc/
--rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/rtc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.237824 types-circuitpython-8.0.0b6/bindings/sdcardio/
--rw-r--r--   0 timon      (501) staff       (20)     2861 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/sdcardio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.238564 types-circuitpython-8.0.0b6/bindings/sdioio/
--rw-r--r--   0 timon      (501) staff       (20)     3605 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/sdioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.239139 types-circuitpython-8.0.0b6/bindings/sharpdisplay/
--rw-r--r--   0 timon      (501) staff       (20)      276 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.239808 types-circuitpython-8.0.0b6/bindings/socketpool/
--rw-r--r--   0 timon      (501) staff       (20)     6123 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/socketpool/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.241102 types-circuitpython-8.0.0b6/bindings/ssl/
--rw-r--r--   0 timon      (501) staff       (20)     4558 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/ssl/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.242112 types-circuitpython-8.0.0b6/bindings/storage/
--rw-r--r--   0 timon      (501) staff       (20)     5394 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/storage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.242881 types-circuitpython-8.0.0b6/bindings/struct/
--rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/struct/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.243620 types-circuitpython-8.0.0b6/bindings/supervisor/
--rw-r--r--   0 timon      (501) staff       (20)     8633 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/supervisor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.244519 types-circuitpython-8.0.0b6/bindings/synthio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/synthio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.245394 types-circuitpython-8.0.0b6/bindings/terminalio/
--rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/terminalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.246781 types-circuitpython-8.0.0b6/bindings/time/
--rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/time/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.248290 types-circuitpython-8.0.0b6/bindings/touchio/
--rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/touchio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.249090 types-circuitpython-8.0.0b6/bindings/traceback/
--rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/traceback/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.249564 types-circuitpython-8.0.0b6/bindings/uheap/
--rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/uheap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.250037 types-circuitpython-8.0.0b6/bindings/usb/
--rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/usb/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.250995 types-circuitpython-8.0.0b6/bindings/usb_cdc/
--rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:34:26.000000 types-circuitpython-8.0.0b6/bindings/usb_cdc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.251778 types-circuitpython-8.0.0b6/bindings/usb_hid/
--rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/usb_hid/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.252658 types-circuitpython-8.0.0b6/bindings/usb_host/
--rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/usb_host/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.253373 types-circuitpython-8.0.0b6/bindings/usb_midi/
--rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/usb_midi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.254329 types-circuitpython-8.0.0b6/bindings/ustack/
--rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/ustack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.255041 types-circuitpython-8.0.0b6/bindings/vectorio/
--rw-r--r--   0 timon      (501) staff       (20)     4801 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/vectorio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.255575 types-circuitpython-8.0.0b6/bindings/watchdog/
--rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/watchdog/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.256026 types-circuitpython-8.0.0b6/bindings/wifi/
--rw-r--r--   0 timon      (501) staff       (20)     9090 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/wifi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.256440 types-circuitpython-8.0.0b6/bindings/zlib/
--rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:34:27.000000 types-circuitpython-8.0.0b6/bindings/zlib/__init__.pyi
--rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.0.0b6/pyproject.toml
--rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:34:37.261956 types-circuitpython-8.0.0b6/setup.cfg
--rw-r--r--   0 timon      (501) staff       (20)     2181 2023-05-16 15:34:28.000000 types-circuitpython-8.0.0b6/setup.py
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:34:37.259449 types-circuitpython-8.0.0b6/types_circuitpython.egg-info/
--rw-r--r--   0 timon      (501) staff       (20)     2978 2023-05-16 15:34:37.000000 types-circuitpython-8.0.0b6/types_circuitpython.egg-info/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:34:37.000000 types-circuitpython-8.0.0b6/types_circuitpython.egg-info/SOURCES.txt
--rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:34:37.000000 types-circuitpython-8.0.0b6/types_circuitpython.egg-info/dependency_links.txt
--rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:34:37.000000 types-circuitpython-8.0.0b6/types_circuitpython.egg-info/requires.txt
--rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:34:37.000000 types-circuitpython-8.0.0b6/types_circuitpython.egg-info/top_level.txt
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.181711 types-circuitpython-8.0.0rc0/
+-rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.0.0rc0/LICENSE
+-rw-r--r--   0 timon      (501) staff       (20)     3038 2023-05-16 15:35:32.181088 types-circuitpython-8.0.0rc0/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:35:28.000000 types-circuitpython-8.0.0rc0/README.md
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.124650 types-circuitpython-8.0.0rc0/bindings/
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.129072 types-circuitpython-8.0.0rc0/bindings/__future__/
+-rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/__future__/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.130375 types-circuitpython-8.0.0rc0/bindings/_bleio/
+-rw-r--r--   0 timon      (501) staff       (20)    31068 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/_bleio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.131464 types-circuitpython-8.0.0rc0/bindings/_eve/
+-rw-r--r--   0 timon      (501) staff       (20)    20082 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/_eve/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.132513 types-circuitpython-8.0.0rc0/bindings/_pew/
+-rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/_pew/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.133758 types-circuitpython-8.0.0rc0/bindings/_pixelmap/
+-rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/_pixelmap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.134741 types-circuitpython-8.0.0rc0/bindings/_stage/
+-rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/_stage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.135451 types-circuitpython-8.0.0rc0/bindings/adafruit_bus_device/
+-rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.136101 types-circuitpython-8.0.0rc0/bindings/adafruit_pixelbuf/
+-rw-r--r--   0 timon      (501) staff       (20)     4190 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.136732 types-circuitpython-8.0.0rc0/bindings/aesio/
+-rw-r--r--   0 timon      (501) staff       (20)     2171 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/aesio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.137304 types-circuitpython-8.0.0rc0/bindings/alarm/
+-rw-r--r--   0 timon      (501) staff       (20)     7020 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/alarm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.137775 types-circuitpython-8.0.0rc0/bindings/analogbufio/
+-rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/analogbufio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.138216 types-circuitpython-8.0.0rc0/bindings/analogio/
+-rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/analogio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.138749 types-circuitpython-8.0.0rc0/bindings/atexit/
+-rw-r--r--   0 timon      (501) staff       (20)     1619 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/atexit/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.139397 types-circuitpython-8.0.0rc0/bindings/audiobusio/
+-rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/audiobusio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.139931 types-circuitpython-8.0.0rc0/bindings/audiocore/
+-rw-r--r--   0 timon      (501) staff       (20)     4614 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/audiocore/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.140491 types-circuitpython-8.0.0rc0/bindings/audioio/
+-rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/audioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.140948 types-circuitpython-8.0.0rc0/bindings/audiomixer/
+-rw-r--r--   0 timon      (501) staff       (20)     4415 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/audiomixer/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.141488 types-circuitpython-8.0.0rc0/bindings/audiomp3/
+-rw-r--r--   0 timon      (501) staff       (20)     3897 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/audiomp3/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.142051 types-circuitpython-8.0.0rc0/bindings/audiopwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4226 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/audiopwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.142498 types-circuitpython-8.0.0rc0/bindings/bitbangio/
+-rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/bitbangio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.142952 types-circuitpython-8.0.0rc0/bindings/bitmaptools/
+-rw-r--r--   0 timon      (501) staff       (20)    10928 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/bitmaptools/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.143437 types-circuitpython-8.0.0rc0/bindings/bitops/
+-rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/bitops/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.143892 types-circuitpython-8.0.0rc0/bindings/board/
+-rw-r--r--   0 timon      (501) staff       (20)     1547 2023-05-16 15:35:21.000000 types-circuitpython-8.0.0rc0/bindings/board/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.144296 types-circuitpython-8.0.0rc0/bindings/busio/
+-rw-r--r--   0 timon      (501) staff       (20)    19739 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/busio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.144818 types-circuitpython-8.0.0rc0/bindings/camera/
+-rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/camera/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.145228 types-circuitpython-8.0.0rc0/bindings/canio/
+-rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/canio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.145761 types-circuitpython-8.0.0rc0/bindings/countio/
+-rw-r--r--   0 timon      (501) staff       (20)     2782 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/countio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.146229 types-circuitpython-8.0.0rc0/bindings/digitalio/
+-rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/digitalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.146756 types-circuitpython-8.0.0rc0/bindings/displayio/
+-rw-r--r--   0 timon      (501) staff       (20)    38264 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/displayio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.147528 types-circuitpython-8.0.0rc0/bindings/dualbank/
+-rw-r--r--   0 timon      (501) staff       (20)     1224 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/dualbank/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.148185 types-circuitpython-8.0.0rc0/bindings/floppyio/
+-rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/floppyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.148983 types-circuitpython-8.0.0rc0/bindings/fontio/
+-rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/fontio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.149649 types-circuitpython-8.0.0rc0/bindings/framebufferio/
+-rw-r--r--   0 timon      (501) staff       (20)     3526 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/framebufferio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.150073 types-circuitpython-8.0.0rc0/bindings/frequencyio/
+-rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/frequencyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.150615 types-circuitpython-8.0.0rc0/bindings/getpass/
+-rw-r--r--   0 timon      (501) staff       (20)      546 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/getpass/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.151070 types-circuitpython-8.0.0rc0/bindings/gifio/
+-rw-r--r--   0 timon      (501) staff       (20)     1834 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/gifio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.151630 types-circuitpython-8.0.0rc0/bindings/gnss/
+-rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/gnss/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.152073 types-circuitpython-8.0.0rc0/bindings/hashlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1002 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/hashlib/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.152492 types-circuitpython-8.0.0rc0/bindings/i2ctarget/
+-rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/i2ctarget/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.152891 types-circuitpython-8.0.0rc0/bindings/imagecapture/
+-rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/imagecapture/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.153289 types-circuitpython-8.0.0rc0/bindings/ipaddress/
+-rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/ipaddress/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.153781 types-circuitpython-8.0.0rc0/bindings/is31fl3741/
+-rw-r--r--   0 timon      (501) staff       (20)     3868 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/is31fl3741/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.154324 types-circuitpython-8.0.0rc0/bindings/keypad/
+-rw-r--r--   0 timon      (501) staff       (20)    13070 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/keypad/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.154748 types-circuitpython-8.0.0rc0/bindings/math/
+-rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/math/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.155176 types-circuitpython-8.0.0rc0/bindings/mdns/
+-rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/mdns/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.155627 types-circuitpython-8.0.0rc0/bindings/memorymap/
+-rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/memorymap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.156077 types-circuitpython-8.0.0rc0/bindings/memorymonitor/
+-rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/memorymonitor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.156537 types-circuitpython-8.0.0rc0/bindings/microcontroller/
+-rw-r--r--   0 timon      (501) staff       (20)     6055 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/microcontroller/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.157311 types-circuitpython-8.0.0rc0/bindings/msgpack/
+-rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/msgpack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.157845 types-circuitpython-8.0.0rc0/bindings/neopixel_write/
+-rw-r--r--   0 timon      (501) staff       (20)     1367 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/neopixel_write/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.158279 types-circuitpython-8.0.0rc0/bindings/nvm/
+-rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/nvm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.158788 types-circuitpython-8.0.0rc0/bindings/onewireio/
+-rw-r--r--   0 timon      (501) staff       (20)     1646 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/onewireio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.159428 types-circuitpython-8.0.0rc0/bindings/os/
+-rw-r--r--   0 timon      (501) staff       (20)     3776 2023-05-16 15:35:22.000000 types-circuitpython-8.0.0rc0/bindings/os/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.159913 types-circuitpython-8.0.0rc0/bindings/paralleldisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     2415 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.160386 types-circuitpython-8.0.0rc0/bindings/ps2io/
+-rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/ps2io/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.160821 types-circuitpython-8.0.0rc0/bindings/pulseio/
+-rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/pulseio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.161337 types-circuitpython-8.0.0rc0/bindings/pwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4872 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/pwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.161817 types-circuitpython-8.0.0rc0/bindings/qrio/
+-rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/qrio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.162370 types-circuitpython-8.0.0rc0/bindings/rainbowio/
+-rw-r--r--   0 timon      (501) staff       (20)      327 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/rainbowio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.162853 types-circuitpython-8.0.0rc0/bindings/random/
+-rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/random/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.163310 types-circuitpython-8.0.0rc0/bindings/rgbmatrix/
+-rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.163745 types-circuitpython-8.0.0rc0/bindings/rotaryio/
+-rw-r--r--   0 timon      (501) staff       (20)     2659 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/rotaryio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.164192 types-circuitpython-8.0.0rc0/bindings/rtc/
+-rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/rtc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.164637 types-circuitpython-8.0.0rc0/bindings/sdcardio/
+-rw-r--r--   0 timon      (501) staff       (20)     2861 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/sdcardio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.165120 types-circuitpython-8.0.0rc0/bindings/sdioio/
+-rw-r--r--   0 timon      (501) staff       (20)     3605 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/sdioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.165716 types-circuitpython-8.0.0rc0/bindings/sharpdisplay/
+-rw-r--r--   0 timon      (501) staff       (20)      276 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.166230 types-circuitpython-8.0.0rc0/bindings/socketpool/
+-rw-r--r--   0 timon      (501) staff       (20)     6123 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/socketpool/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.166633 types-circuitpython-8.0.0rc0/bindings/ssl/
+-rw-r--r--   0 timon      (501) staff       (20)     4558 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/ssl/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.167026 types-circuitpython-8.0.0rc0/bindings/storage/
+-rw-r--r--   0 timon      (501) staff       (20)     5394 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/storage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.167554 types-circuitpython-8.0.0rc0/bindings/struct/
+-rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/struct/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.168098 types-circuitpython-8.0.0rc0/bindings/supervisor/
+-rw-r--r--   0 timon      (501) staff       (20)     8633 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/supervisor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.168545 types-circuitpython-8.0.0rc0/bindings/synthio/
+-rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/synthio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.168940 types-circuitpython-8.0.0rc0/bindings/terminalio/
+-rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/terminalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.169340 types-circuitpython-8.0.0rc0/bindings/time/
+-rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/time/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.169777 types-circuitpython-8.0.0rc0/bindings/touchio/
+-rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/touchio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.170193 types-circuitpython-8.0.0rc0/bindings/traceback/
+-rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/traceback/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.170746 types-circuitpython-8.0.0rc0/bindings/uheap/
+-rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/uheap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.171346 types-circuitpython-8.0.0rc0/bindings/usb/
+-rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/usb/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.172038 types-circuitpython-8.0.0rc0/bindings/usb_cdc/
+-rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/usb_cdc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.172752 types-circuitpython-8.0.0rc0/bindings/usb_hid/
+-rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/usb_hid/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.173438 types-circuitpython-8.0.0rc0/bindings/usb_host/
+-rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/usb_host/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.174157 types-circuitpython-8.0.0rc0/bindings/usb_midi/
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/usb_midi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.174800 types-circuitpython-8.0.0rc0/bindings/ustack/
+-rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/ustack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.175459 types-circuitpython-8.0.0rc0/bindings/vectorio/
+-rw-r--r--   0 timon      (501) staff       (20)     4801 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/vectorio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.176086 types-circuitpython-8.0.0rc0/bindings/watchdog/
+-rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:35:23.000000 types-circuitpython-8.0.0rc0/bindings/watchdog/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.176687 types-circuitpython-8.0.0rc0/bindings/wifi/
+-rw-r--r--   0 timon      (501) staff       (20)     9256 2023-05-16 15:35:24.000000 types-circuitpython-8.0.0rc0/bindings/wifi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.177322 types-circuitpython-8.0.0rc0/bindings/zlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:35:24.000000 types-circuitpython-8.0.0rc0/bindings/zlib/__init__.pyi
+-rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.0.0rc0/pyproject.toml
+-rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:35:32.181935 types-circuitpython-8.0.0rc0/setup.cfg
+-rw-r--r--   0 timon      (501) staff       (20)     2179 2023-05-16 15:35:24.000000 types-circuitpython-8.0.0rc0/setup.py
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:35:32.180381 types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/
+-rw-r--r--   0 timon      (501) staff       (20)     3038 2023-05-16 15:35:32.000000 types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:35:32.000000 types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/SOURCES.txt
+-rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:35:32.000000 types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/dependency_links.txt
+-rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:35:32.000000 types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/requires.txt
+-rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:35:32.000000 types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/top_level.txt
```

### Comparing `types-circuitpython-8.0.0b6/LICENSE` & `types-circuitpython-8.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/PKG-INFO` & `types-circuitpython-8.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.0.0b6
+Version: 8.0.0rc0
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,15 @@
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.0.x
+    - 8.0.0-rc.0 (Corresponds 8.0.0-rc.0 of CircuitPython)
     - 8.0.0b6 (Corresponds 8.0.0-beta.6 of CircuitPython)
     - 8.0.0b5 (Corresponds 8.0.0-beta.5 of CircuitPython)
     - 8.0.0b4 (Corresponds 8.0.0-beta.4 of CircuitPython)
     - 8.0.0b3 (Corresponds 8.0.0-beta.3 of CircuitPython)
     - 8.0.0b2 (Corresponds 8.0.0-beta.2 of CircuitPython)
     - 8.0.0b1 (Corresponds 8.0.0-beta.1 of CircuitPython)
     - 8.0.0b0 (Corresponds 8.0.0-beta.0 of CircuitPython)
```

### Comparing `types-circuitpython-8.0.0b6/README.md` & `types-circuitpython-8.0.0rc0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.0.x
+    - 8.0.0-rc.0 (Corresponds 8.0.0-rc.0 of CircuitPython)
     - 8.0.0b6 (Corresponds 8.0.0-beta.6 of CircuitPython)
     - 8.0.0b5 (Corresponds 8.0.0-beta.5 of CircuitPython)
     - 8.0.0b4 (Corresponds 8.0.0-beta.4 of CircuitPython)
     - 8.0.0b3 (Corresponds 8.0.0-beta.3 of CircuitPython)
     - 8.0.0b2 (Corresponds 8.0.0-beta.2 of CircuitPython)
     - 8.0.0b1 (Corresponds 8.0.0-beta.1 of CircuitPython)
     - 8.0.0b0 (Corresponds 8.0.0-beta.0 of CircuitPython)
```

### Comparing `types-circuitpython-8.0.0b6/bindings/__future__/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/__future__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/_bleio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/_eve/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/_pew/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/_pixelmap/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/_stage/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/adafruit_pixelbuf/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/aesio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/alarm/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/analogbufio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/analogio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/atexit/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/audiobusio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/audiocore/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/audioio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/audiomixer/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/audiomp3/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/audiopwmio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/bitbangio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/bitbangio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -229,17 +229,29 @@
 
         :return: True when lock has been grabbed
         :rtype: bool"""
         ...
     def unlock(self) -> None:
         """Releases the SPI lock."""
         ...
-    def write(self, buf: ReadableBuffer) -> None:
+    import sys
+    def write(
+        self, buf: ReadableBuffer, *, start: int = 0, end: int = sys.maxsize
+    ) -> None:
         """Write the data contained in ``buf``. Requires the SPI being locked.
-        If the buffer is empty, nothing happens."""
+        If the buffer is empty, nothing happens.
+
+        If ``start`` or ``end`` is provided, then the buffer will be sliced
+        as if ``buffer[start:end]`` were passed, but without copying the data.
+        The number of bytes written will be the length of ``buffer[start:end]``.
+
+        :param ReadableBuffer buffer: buffer containing the bytes to write
+        :param int start: beginning of buffer slice
+        :param int end: end of buffer slice; if not specified, use ``len(buffer)``
+        """
         ...
     import sys
     def readinto(
         self,
         buffer: WriteableBuffer,
         *,
         start: int = 0,
```

### Comparing `types-circuitpython-8.0.0b6/bindings/bitmaptools/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/bitops/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/board/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/busio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/camera/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/canio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/countio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/digitalio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/displayio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/dualbank/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/floppyio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/fontio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/framebufferio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/frequencyio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/getpass/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/gifio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/gnss/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/hashlib/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/i2ctarget/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/imagecapture/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/imagecapture/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Support for "Parallel capture" interfaces
 
 .. seealso::
 
-    Espressif microcontrollers use the `esp32_camera` module together.
+    Espressif microcontrollers use the `espcamera` module together.
 
 """
 
 from __future__ import annotations
 
 from typing import List, Optional
```

### Comparing `types-circuitpython-8.0.0b6/bindings/ipaddress/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/is31fl3741/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/keypad/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/math/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/mdns/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/memorymap/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/memorymonitor/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/microcontroller/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/microcontroller/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,19 @@
        print(microcontroller.cpus[1].frequency)"""
 
     def __init__(self) -> None:
         """You cannot create an instance of `microcontroller.Processor`.
         Use `microcontroller.cpu` to access the sole instance available."""
         ...
     frequency: int
-    """The CPU operating frequency in Hertz. (read-only)"""
+    """The CPU operating frequency in Hertz.
+
+    **Limitations:** Setting the ``frequency`` is possible only on some i.MX boards.
+    On most boards, ``frequency`` is read-only.
+    """
     reset_reason: microcontroller.ResetReason
     """The reason the microcontroller started up from reset state."""
     temperature: Optional[float]
     """The on-chip temperature, in Celsius, as a float. (read-only)
 
     Is `None` if the temperature is not available.
```

### Comparing `types-circuitpython-8.0.0b6/bindings/msgpack/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/neopixel_write/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/nvm/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/onewireio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/os/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/paralleldisplay/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/ps2io/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/pulseio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/pwmio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/qrio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/random/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/rgbmatrix/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/rotaryio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/rtc/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/sdcardio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/sdioio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/socketpool/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/ssl/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/storage/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/struct/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/supervisor/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/synthio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/terminalio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/time/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/touchio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/traceback/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/usb_cdc/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/usb_hid/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/usb_host/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/usb_midi/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/vectorio/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/watchdog/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/bindings/wifi/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/wifi/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,26 @@
     If you set the value to ``False``, any open sockets will be closed.
     """
     hostname: Union[str | ReadableBuffer]
     """Hostname for wifi interface. When the hostname is altered after interface started/connected
        the changes would only be reflected once the interface restarts/reconnects."""
     mac_address: ReadableBuffer
     """MAC address for the station. When the address is altered after interface is connected
-       the changes would only be reflected once the interface reconnects."""
+       the changes would only be reflected once the interface reconnects.
+
+    **Limitations:** Not settable on RP2040 CYW43 boards, such as Pi Pico W.
+    """
     tx_power: float
     """Wifi transmission power, in dBm."""
     mac_address_ap: ReadableBuffer
     """MAC address for the AP. When the address is altered after interface is started
-       the changes would only be reflected once the interface restarts."""
+       the changes would only be reflected once the interface restarts.
+
+    **Limitations:** Not settable on RP2040 CYW43 boards, such as Pi Pico W.
+    """
     def start_scanning_networks(
         self, *, start_channel: int = 1, stop_channel: int = 11
     ) -> Iterable[Network]:
         """Scans for available wifi networks over the given channel range. Make sure the channels are allowed in your country.
 
         .. note::
```

### Comparing `types-circuitpython-8.0.0b6/bindings/zlib/__init__.pyi` & `types-circuitpython-8.0.0rc0/bindings/zlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/setup.py` & `types-circuitpython-8.0.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir, path
 
 from setuptools import setup
 
 __name__ = "types-circuitpython"
-__version__ = "8.0.0-beta.6"
+__version__ = "8.0.0-rc.0"
 __repo__ = "https://github.com/hardfury-labs/types-circuitpython"
 __author__ = "HardFury"
 
 
 HERE = path.abspath(path.dirname(__file__))
 BINDINGS_DIR = path.join(HERE, "bindings")
```

### Comparing `types-circuitpython-8.0.0b6/types_circuitpython.egg-info/PKG-INFO` & `types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.0.0b6
+Version: 8.0.0rc0
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -42,14 +42,15 @@
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.0.x
+    - 8.0.0-rc.0 (Corresponds 8.0.0-rc.0 of CircuitPython)
     - 8.0.0b6 (Corresponds 8.0.0-beta.6 of CircuitPython)
     - 8.0.0b5 (Corresponds 8.0.0-beta.5 of CircuitPython)
     - 8.0.0b4 (Corresponds 8.0.0-beta.4 of CircuitPython)
     - 8.0.0b3 (Corresponds 8.0.0-beta.3 of CircuitPython)
     - 8.0.0b2 (Corresponds 8.0.0-beta.2 of CircuitPython)
     - 8.0.0b1 (Corresponds 8.0.0-beta.1 of CircuitPython)
     - 8.0.0b0 (Corresponds 8.0.0-beta.0 of CircuitPython)
```

### Comparing `types-circuitpython-8.0.0b6/types_circuitpython.egg-info/SOURCES.txt` & `types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b6/types_circuitpython.egg-info/top_level.txt` & `types-circuitpython-8.0.0rc0/types_circuitpython.egg-info/top_level.txt`

 * *Files identical despite different names*

