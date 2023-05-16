# Comparing `tmp/types-circuitpython-8.0.3.tar.gz` & `tmp/types-circuitpython-8.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-circuitpython-8.0.3.tar", last modified: Tue May 16 15:41:11 2023, max compression
+gzip compressed data, was "types-circuitpython-8.1.0a2.tar", last modified: Tue May 16 15:40:23 2023, max compression
```

## Comparing `types-circuitpython-8.0.3.tar` & `types-circuitpython-8.1.0a2.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.622103 types-circuitpython-8.0.3/
--rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.0.3/LICENSE
--rw-r--r--   0 timon      (501) staff       (20)     3382 2023-05-16 15:41:11.621739 types-circuitpython-8.0.3/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2327 2023-05-16 15:41:04.000000 types-circuitpython-8.0.3/README.md
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.566512 types-circuitpython-8.0.3/bindings/
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.569851 types-circuitpython-8.0.3/bindings/__future__/
--rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/__future__/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.570333 types-circuitpython-8.0.3/bindings/_bleio/
--rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/_bleio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.570868 types-circuitpython-8.0.3/bindings/_eve/
--rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/_eve/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.571410 types-circuitpython-8.0.3/bindings/_pew/
--rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/_pew/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.571998 types-circuitpython-8.0.3/bindings/_pixelmap/
--rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/_pixelmap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.572592 types-circuitpython-8.0.3/bindings/_stage/
--rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/_stage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.573188 types-circuitpython-8.0.3/bindings/adafruit_bus_device/
--rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.573842 types-circuitpython-8.0.3/bindings/adafruit_pixelbuf/
--rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-16 15:40:59.000000 types-circuitpython-8.0.3/bindings/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.574435 types-circuitpython-8.0.3/bindings/aesio/
--rw-r--r--   0 timon      (501) staff       (20)     2171 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/aesio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.576814 types-circuitpython-8.0.3/bindings/alarm/
--rw-r--r--   0 timon      (501) staff       (20)     7020 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/alarm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.577746 types-circuitpython-8.0.3/bindings/analogbufio/
--rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/analogbufio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.578749 types-circuitpython-8.0.3/bindings/analogio/
--rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/analogio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.579689 types-circuitpython-8.0.3/bindings/atexit/
--rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/atexit/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.580372 types-circuitpython-8.0.3/bindings/audiobusio/
--rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/audiobusio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.581215 types-circuitpython-8.0.3/bindings/audiocore/
--rw-r--r--   0 timon      (501) staff       (20)     4614 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/audiocore/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.581878 types-circuitpython-8.0.3/bindings/audioio/
--rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/audioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.582506 types-circuitpython-8.0.3/bindings/audiomixer/
--rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/audiomixer/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.583390 types-circuitpython-8.0.3/bindings/audiomp3/
--rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/audiomp3/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.584612 types-circuitpython-8.0.3/bindings/audiopwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4226 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/audiopwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.585804 types-circuitpython-8.0.3/bindings/bitbangio/
--rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/bitbangio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.586725 types-circuitpython-8.0.3/bindings/bitmaptools/
--rw-r--r--   0 timon      (501) staff       (20)    10928 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/bitmaptools/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.587357 types-circuitpython-8.0.3/bindings/bitops/
--rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/bitops/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.588084 types-circuitpython-8.0.3/bindings/board/
--rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/board/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.588767 types-circuitpython-8.0.3/bindings/busio/
--rw-r--r--   0 timon      (501) staff       (20)    20025 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/busio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.589272 types-circuitpython-8.0.3/bindings/camera/
--rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/camera/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.589702 types-circuitpython-8.0.3/bindings/canio/
--rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/canio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.590110 types-circuitpython-8.0.3/bindings/countio/
--rw-r--r--   0 timon      (501) staff       (20)     2782 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/countio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.590766 types-circuitpython-8.0.3/bindings/digitalio/
--rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/digitalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.591206 types-circuitpython-8.0.3/bindings/displayio/
--rw-r--r--   0 timon      (501) staff       (20)    38300 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/displayio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.591682 types-circuitpython-8.0.3/bindings/dualbank/
--rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/dualbank/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.592041 types-circuitpython-8.0.3/bindings/floppyio/
--rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:41:00.000000 types-circuitpython-8.0.3/bindings/floppyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.592502 types-circuitpython-8.0.3/bindings/fontio/
--rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/fontio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.592877 types-circuitpython-8.0.3/bindings/framebufferio/
--rw-r--r--   0 timon      (501) staff       (20)     3553 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/framebufferio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.593232 types-circuitpython-8.0.3/bindings/frequencyio/
--rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/frequencyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.593587 types-circuitpython-8.0.3/bindings/getpass/
--rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/getpass/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.593942 types-circuitpython-8.0.3/bindings/gifio/
--rw-r--r--   0 timon      (501) staff       (20)     1834 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/gifio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.594375 types-circuitpython-8.0.3/bindings/gnss/
--rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/gnss/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.594741 types-circuitpython-8.0.3/bindings/hashlib/
--rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/hashlib/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.595258 types-circuitpython-8.0.3/bindings/i2ctarget/
--rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/i2ctarget/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.595686 types-circuitpython-8.0.3/bindings/imagecapture/
--rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/imagecapture/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.596049 types-circuitpython-8.0.3/bindings/ipaddress/
--rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/ipaddress/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.596408 types-circuitpython-8.0.3/bindings/is31fl3741/
--rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/is31fl3741/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.596779 types-circuitpython-8.0.3/bindings/keypad/
--rw-r--r--   0 timon      (501) staff       (20)    13079 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/keypad/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.597153 types-circuitpython-8.0.3/bindings/math/
--rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/math/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.597793 types-circuitpython-8.0.3/bindings/mdns/
--rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/mdns/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.598328 types-circuitpython-8.0.3/bindings/memorymap/
--rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/memorymap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.598710 types-circuitpython-8.0.3/bindings/memorymonitor/
--rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/memorymonitor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.599136 types-circuitpython-8.0.3/bindings/microcontroller/
--rw-r--r--   0 timon      (501) staff       (20)     6055 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/microcontroller/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.599491 types-circuitpython-8.0.3/bindings/msgpack/
--rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/msgpack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.599837 types-circuitpython-8.0.3/bindings/neopixel_write/
--rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/neopixel_write/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.600183 types-circuitpython-8.0.3/bindings/nvm/
--rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/nvm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.600668 types-circuitpython-8.0.3/bindings/onewireio/
--rw-r--r--   0 timon      (501) staff       (20)     1646 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/onewireio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.601063 types-circuitpython-8.0.3/bindings/os/
--rw-r--r--   0 timon      (501) staff       (20)     3776 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/os/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.601514 types-circuitpython-8.0.3/bindings/paralleldisplay/
--rw-r--r--   0 timon      (501) staff       (20)     2415 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.602155 types-circuitpython-8.0.3/bindings/ps2io/
--rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/ps2io/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.602730 types-circuitpython-8.0.3/bindings/pulseio/
--rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/pulseio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.603145 types-circuitpython-8.0.3/bindings/pwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4872 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/pwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.603577 types-circuitpython-8.0.3/bindings/qrio/
--rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/qrio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.604033 types-circuitpython-8.0.3/bindings/rainbowio/
--rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/rainbowio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.604415 types-circuitpython-8.0.3/bindings/random/
--rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/random/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.604823 types-circuitpython-8.0.3/bindings/rgbmatrix/
--rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.605198 types-circuitpython-8.0.3/bindings/rotaryio/
--rw-r--r--   0 timon      (501) staff       (20)     2659 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/rotaryio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.605553 types-circuitpython-8.0.3/bindings/rtc/
--rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/rtc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.605922 types-circuitpython-8.0.3/bindings/sdcardio/
--rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/sdcardio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.606273 types-circuitpython-8.0.3/bindings/sdioio/
--rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/sdioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.606629 types-circuitpython-8.0.3/bindings/sharpdisplay/
--rw-r--r--   0 timon      (501) staff       (20)      276 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.607058 types-circuitpython-8.0.3/bindings/socketpool/
--rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/socketpool/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.607422 types-circuitpython-8.0.3/bindings/ssl/
--rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/ssl/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.607835 types-circuitpython-8.0.3/bindings/storage/
--rw-r--r--   0 timon      (501) staff       (20)     5556 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/storage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.608322 types-circuitpython-8.0.3/bindings/struct/
--rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/struct/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.609128 types-circuitpython-8.0.3/bindings/supervisor/
--rw-r--r--   0 timon      (501) staff       (20)     8633 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/supervisor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.610170 types-circuitpython-8.0.3/bindings/synthio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/synthio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.611068 types-circuitpython-8.0.3/bindings/terminalio/
--rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/terminalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.611865 types-circuitpython-8.0.3/bindings/time/
--rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/time/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.612767 types-circuitpython-8.0.3/bindings/touchio/
--rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/touchio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.613489 types-circuitpython-8.0.3/bindings/traceback/
--rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/traceback/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.614047 types-circuitpython-8.0.3/bindings/uheap/
--rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:41:01.000000 types-circuitpython-8.0.3/bindings/uheap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.614502 types-circuitpython-8.0.3/bindings/usb/
--rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/usb/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.615047 types-circuitpython-8.0.3/bindings/usb_cdc/
--rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/usb_cdc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.615582 types-circuitpython-8.0.3/bindings/usb_hid/
--rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/usb_hid/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.616186 types-circuitpython-8.0.3/bindings/usb_host/
--rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/usb_host/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.616602 types-circuitpython-8.0.3/bindings/usb_midi/
--rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/usb_midi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.616978 types-circuitpython-8.0.3/bindings/ustack/
--rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/ustack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.617360 types-circuitpython-8.0.3/bindings/vectorio/
--rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/vectorio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.617838 types-circuitpython-8.0.3/bindings/watchdog/
--rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/watchdog/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.618439 types-circuitpython-8.0.3/bindings/wifi/
--rw-r--r--   0 timon      (501) staff       (20)     9256 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/wifi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.619202 types-circuitpython-8.0.3/bindings/zlib/
--rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/bindings/zlib/__init__.pyi
--rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.0.3/pyproject.toml
--rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:41:11.622309 types-circuitpython-8.0.3/setup.cfg
--rw-r--r--   0 timon      (501) staff       (20)     2174 2023-05-16 15:41:02.000000 types-circuitpython-8.0.3/setup.py
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:41:11.621212 types-circuitpython-8.0.3/types_circuitpython.egg-info/
--rw-r--r--   0 timon      (501) staff       (20)     3382 2023-05-16 15:41:11.000000 types-circuitpython-8.0.3/types_circuitpython.egg-info/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:41:11.000000 types-circuitpython-8.0.3/types_circuitpython.egg-info/SOURCES.txt
--rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:41:11.000000 types-circuitpython-8.0.3/types_circuitpython.egg-info/dependency_links.txt
--rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:41:11.000000 types-circuitpython-8.0.3/types_circuitpython.egg-info/requires.txt
--rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:41:11.000000 types-circuitpython-8.0.3/types_circuitpython.egg-info/top_level.txt
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.917829 types-circuitpython-8.1.0a2/
+-rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.1.0a2/LICENSE
+-rw-r--r--   0 timon      (501) staff       (20)     3323 2023-05-16 15:40:23.917452 types-circuitpython-8.1.0a2/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2266 2023-05-16 15:40:00.000000 types-circuitpython-8.1.0a2/README.md
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.869443 types-circuitpython-8.1.0a2/bindings/
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.873667 types-circuitpython-8.1.0a2/bindings/__future__/
+-rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:40:11.000000 types-circuitpython-8.1.0a2/bindings/__future__/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.874189 types-circuitpython-8.1.0a2/bindings/_bleio/
+-rw-r--r--   0 timon      (501) staff       (20)    31085 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/_bleio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.874857 types-circuitpython-8.1.0a2/bindings/_eve/
+-rw-r--r--   0 timon      (501) staff       (20)    20379 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/_eve/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.875515 types-circuitpython-8.1.0a2/bindings/_pew/
+-rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/_pew/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.876069 types-circuitpython-8.1.0a2/bindings/_pixelmap/
+-rw-r--r--   0 timon      (501) staff       (20)     2572 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/_pixelmap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.876682 types-circuitpython-8.1.0a2/bindings/_stage/
+-rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/_stage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.877227 types-circuitpython-8.1.0a2/bindings/adafruit_bus_device/
+-rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.877752 types-circuitpython-8.1.0a2/bindings/adafruit_pixelbuf/
+-rw-r--r--   0 timon      (501) staff       (20)     4199 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.878290 types-circuitpython-8.1.0a2/bindings/aesio/
+-rw-r--r--   0 timon      (501) staff       (20)     2171 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/aesio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.878859 types-circuitpython-8.1.0a2/bindings/alarm/
+-rw-r--r--   0 timon      (501) staff       (20)     7020 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/alarm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.879450 types-circuitpython-8.1.0a2/bindings/analogbufio/
+-rw-r--r--   0 timon      (501) staff       (20)     2838 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/analogbufio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.879986 types-circuitpython-8.1.0a2/bindings/analogio/
+-rw-r--r--   0 timon      (501) staff       (20)     3769 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/analogio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.880500 types-circuitpython-8.1.0a2/bindings/atexit/
+-rw-r--r--   0 timon      (501) staff       (20)     1617 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/atexit/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.881124 types-circuitpython-8.1.0a2/bindings/audiobusio/
+-rw-r--r--   0 timon      (501) staff       (20)     7538 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/audiobusio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.881724 types-circuitpython-8.1.0a2/bindings/audiocore/
+-rw-r--r--   0 timon      (501) staff       (20)     4614 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/audiocore/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.882342 types-circuitpython-8.1.0a2/bindings/audioio/
+-rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/audioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.882946 types-circuitpython-8.1.0a2/bindings/audiomixer/
+-rw-r--r--   0 timon      (501) staff       (20)     4424 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/audiomixer/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.883511 types-circuitpython-8.1.0a2/bindings/audiomp3/
+-rw-r--r--   0 timon      (501) staff       (20)     3896 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/audiomp3/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.884050 types-circuitpython-8.1.0a2/bindings/audiopwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4226 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/audiopwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.884578 types-circuitpython-8.1.0a2/bindings/bitbangio/
+-rw-r--r--   0 timon      (501) staff       (20)    12567 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/bitbangio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.885100 types-circuitpython-8.1.0a2/bindings/bitmaptools/
+-rw-r--r--   0 timon      (501) staff       (20)    10928 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/bitmaptools/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.885808 types-circuitpython-8.1.0a2/bindings/bitops/
+-rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/bitops/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.886410 types-circuitpython-8.1.0a2/bindings/board/
+-rw-r--r--   0 timon      (501) staff       (20)     1562 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/board/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.887023 types-circuitpython-8.1.0a2/bindings/busio/
+-rw-r--r--   0 timon      (501) staff       (20)    19737 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/busio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.887721 types-circuitpython-8.1.0a2/bindings/camera/
+-rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/camera/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.888296 types-circuitpython-8.1.0a2/bindings/canio/
+-rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/canio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.888913 types-circuitpython-8.1.0a2/bindings/countio/
+-rw-r--r--   0 timon      (501) staff       (20)     2782 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/countio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.889391 types-circuitpython-8.1.0a2/bindings/digitalio/
+-rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:40:12.000000 types-circuitpython-8.1.0a2/bindings/digitalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.889948 types-circuitpython-8.1.0a2/bindings/displayio/
+-rw-r--r--   0 timon      (501) staff       (20)    38300 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/displayio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.890880 types-circuitpython-8.1.0a2/bindings/dualbank/
+-rw-r--r--   0 timon      (501) staff       (20)     1811 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/dualbank/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.891375 types-circuitpython-8.1.0a2/bindings/floppyio/
+-rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/floppyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.891741 types-circuitpython-8.1.0a2/bindings/fontio/
+-rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/fontio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.892091 types-circuitpython-8.1.0a2/bindings/framebufferio/
+-rw-r--r--   0 timon      (501) staff       (20)     3553 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/framebufferio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.892463 types-circuitpython-8.1.0a2/bindings/frequencyio/
+-rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/frequencyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.893039 types-circuitpython-8.1.0a2/bindings/getpass/
+-rw-r--r--   0 timon      (501) staff       (20)      545 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/getpass/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.893705 types-circuitpython-8.1.0a2/bindings/gifio/
+-rw-r--r--   0 timon      (501) staff       (20)     1834 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/gifio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.894278 types-circuitpython-8.1.0a2/bindings/gnss/
+-rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/gnss/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.894869 types-circuitpython-8.1.0a2/bindings/hashlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1011 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/hashlib/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.895389 types-circuitpython-8.1.0a2/bindings/i2ctarget/
+-rw-r--r--   0 timon      (501) staff       (20)     5397 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/i2ctarget/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.895982 types-circuitpython-8.1.0a2/bindings/imagecapture/
+-rw-r--r--   0 timon      (501) staff       (20)     2883 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/imagecapture/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.896542 types-circuitpython-8.1.0a2/bindings/ipaddress/
+-rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/ipaddress/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.896955 types-circuitpython-8.1.0a2/bindings/is31fl3741/
+-rw-r--r--   0 timon      (501) staff       (20)     3873 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/is31fl3741/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.897314 types-circuitpython-8.1.0a2/bindings/keypad/
+-rw-r--r--   0 timon      (501) staff       (20)    13079 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/keypad/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.897694 types-circuitpython-8.1.0a2/bindings/math/
+-rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/math/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.898140 types-circuitpython-8.1.0a2/bindings/mdns/
+-rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/mdns/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.898500 types-circuitpython-8.1.0a2/bindings/memorymap/
+-rw-r--r--   0 timon      (501) staff       (20)     1980 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/memorymap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.898839 types-circuitpython-8.1.0a2/bindings/memorymonitor/
+-rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/memorymonitor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.899191 types-circuitpython-8.1.0a2/bindings/microcontroller/
+-rw-r--r--   0 timon      (501) staff       (20)     6057 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/microcontroller/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.899531 types-circuitpython-8.1.0a2/bindings/msgpack/
+-rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/msgpack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.899865 types-circuitpython-8.1.0a2/bindings/neopixel_write/
+-rw-r--r--   0 timon      (501) staff       (20)     1372 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/neopixel_write/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.900203 types-circuitpython-8.1.0a2/bindings/nvm/
+-rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/nvm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.900533 types-circuitpython-8.1.0a2/bindings/onewireio/
+-rw-r--r--   0 timon      (501) staff       (20)     1646 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/onewireio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.900926 types-circuitpython-8.1.0a2/bindings/os/
+-rw-r--r--   0 timon      (501) staff       (20)     3776 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/os/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.901259 types-circuitpython-8.1.0a2/bindings/paralleldisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     2415 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.901603 types-circuitpython-8.1.0a2/bindings/ps2io/
+-rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/ps2io/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.901954 types-circuitpython-8.1.0a2/bindings/pulseio/
+-rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/pulseio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.902298 types-circuitpython-8.1.0a2/bindings/pwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4872 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/pwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.902639 types-circuitpython-8.1.0a2/bindings/qrio/
+-rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/qrio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.902975 types-circuitpython-8.1.0a2/bindings/rainbowio/
+-rw-r--r--   0 timon      (501) staff       (20)      332 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/rainbowio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.903300 types-circuitpython-8.1.0a2/bindings/random/
+-rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/random/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.903682 types-circuitpython-8.1.0a2/bindings/rgbmatrix/
+-rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.904012 types-circuitpython-8.1.0a2/bindings/rotaryio/
+-rw-r--r--   0 timon      (501) staff       (20)     2659 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/rotaryio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.904335 types-circuitpython-8.1.0a2/bindings/rtc/
+-rw-r--r--   0 timon      (501) staff       (20)     1962 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/rtc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.904672 types-circuitpython-8.1.0a2/bindings/sdcardio/
+-rw-r--r--   0 timon      (501) staff       (20)     2859 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/sdcardio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.905012 types-circuitpython-8.1.0a2/bindings/sdioio/
+-rw-r--r--   0 timon      (501) staff       (20)     3603 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/sdioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.905534 types-circuitpython-8.1.0a2/bindings/sharpdisplay/
+-rw-r--r--   0 timon      (501) staff       (20)      276 2023-05-16 15:40:13.000000 types-circuitpython-8.1.0a2/bindings/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.905911 types-circuitpython-8.1.0a2/bindings/socketpool/
+-rw-r--r--   0 timon      (501) staff       (20)     6132 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/socketpool/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.906422 types-circuitpython-8.1.0a2/bindings/ssl/
+-rw-r--r--   0 timon      (501) staff       (20)     4567 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/ssl/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.907045 types-circuitpython-8.1.0a2/bindings/storage/
+-rw-r--r--   0 timon      (501) staff       (20)     5556 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/storage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.907714 types-circuitpython-8.1.0a2/bindings/struct/
+-rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/struct/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.908178 types-circuitpython-8.1.0a2/bindings/supervisor/
+-rw-r--r--   0 timon      (501) staff       (20)    10816 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/supervisor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.908654 types-circuitpython-8.1.0a2/bindings/synthio/
+-rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/synthio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.909149 types-circuitpython-8.1.0a2/bindings/terminalio/
+-rw-r--r--   0 timon      (501) staff       (20)     1723 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/terminalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.909675 types-circuitpython-8.1.0a2/bindings/time/
+-rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/time/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.910095 types-circuitpython-8.1.0a2/bindings/touchio/
+-rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/touchio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.910461 types-circuitpython-8.1.0a2/bindings/traceback/
+-rw-r--r--   0 timon      (501) staff       (20)     3773 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/traceback/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.910858 types-circuitpython-8.1.0a2/bindings/uheap/
+-rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/uheap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.911203 types-circuitpython-8.1.0a2/bindings/usb/
+-rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/usb/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.911543 types-circuitpython-8.1.0a2/bindings/usb_cdc/
+-rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/usb_cdc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.911891 types-circuitpython-8.1.0a2/bindings/usb_hid/
+-rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/usb_hid/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.912255 types-circuitpython-8.1.0a2/bindings/usb_host/
+-rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/usb_host/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.912589 types-circuitpython-8.1.0a2/bindings/usb_midi/
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/usb_midi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.912938 types-circuitpython-8.1.0a2/bindings/ustack/
+-rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/ustack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.913289 types-circuitpython-8.1.0a2/bindings/vectorio/
+-rw-r--r--   0 timon      (501) staff       (20)     4828 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/vectorio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.913677 types-circuitpython-8.1.0a2/bindings/watchdog/
+-rw-r--r--   0 timon      (501) staff       (20)     3341 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/watchdog/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.914008 types-circuitpython-8.1.0a2/bindings/wifi/
+-rw-r--r--   0 timon      (501) staff       (20)     9256 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/wifi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.914546 types-circuitpython-8.1.0a2/bindings/zlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/bindings/zlib/__init__.pyi
+-rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.1.0a2/pyproject.toml
+-rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:40:23.917957 types-circuitpython-8.1.0a2/setup.cfg
+-rw-r--r--   0 timon      (501) staff       (20)     2182 2023-05-16 15:40:14.000000 types-circuitpython-8.1.0a2/setup.py
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:40:23.916860 types-circuitpython-8.1.0a2/types_circuitpython.egg-info/
+-rw-r--r--   0 timon      (501) staff       (20)     3323 2023-05-16 15:40:23.000000 types-circuitpython-8.1.0a2/types_circuitpython.egg-info/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2925 2023-05-16 15:40:23.000000 types-circuitpython-8.1.0a2/types_circuitpython.egg-info/SOURCES.txt
+-rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:40:23.000000 types-circuitpython-8.1.0a2/types_circuitpython.egg-info/dependency_links.txt
+-rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:40:23.000000 types-circuitpython-8.1.0a2/types_circuitpython.egg-info/requires.txt
+-rw-r--r--   0 timon      (501) staff       (20)      756 2023-05-16 15:40:23.000000 types-circuitpython-8.1.0a2/types_circuitpython.egg-info/top_level.txt
```

### Comparing `types-circuitpython-8.0.3/LICENSE` & `types-circuitpython-8.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/PKG-INFO` & `types-circuitpython-8.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.0.3
+Version: 8.1.0a2
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -42,17 +42,16 @@
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.1.x
-    - 8.1.0a2 (Corresponds 8.1.0-alpha.2 of CircuitPython's version)
+    - 8.1.0-alpha.2
   - 8.0.x
-    - 8.0.3
     - 8.0.2
     - 8.0.0
     - 8.0.0rc2 (Corresponds 8.0.0-rc.2 of CircuitPython's version)
     - 8.0.0rc1 (Corresponds 8.0.0-rc.1 of CircuitPython's version)
     - 8.0.0rc0 (Corresponds 8.0.0-rc.0 of CircuitPython's version)
     - 8.0.0b6 (Corresponds 8.0.0-beta.6 of CircuitPython's version)
     - 8.0.0b5 (Corresponds 8.0.0-beta.5 of CircuitPython's version)
```

### Comparing `types-circuitpython-8.0.3/README.md` & `types-circuitpython-8.1.0a2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.1.x
-    - 8.1.0a2 (Corresponds 8.1.0-alpha.2 of CircuitPython's version)
+    - 8.1.0-alpha.2
   - 8.0.x
-    - 8.0.3
     - 8.0.2
     - 8.0.0
     - 8.0.0rc2 (Corresponds 8.0.0-rc.2 of CircuitPython's version)
     - 8.0.0rc1 (Corresponds 8.0.0-rc.1 of CircuitPython's version)
     - 8.0.0rc0 (Corresponds 8.0.0-rc.0 of CircuitPython's version)
     - 8.0.0b6 (Corresponds 8.0.0-beta.6 of CircuitPython's version)
     - 8.0.0b5 (Corresponds 8.0.0-beta.5 of CircuitPython's version)
```

### Comparing `types-circuitpython-8.0.3/bindings/__future__/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/__future__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/_bleio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/_eve/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/_pew/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/_pixelmap/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/_stage/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/adafruit_pixelbuf/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/aesio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/aesio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/alarm/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/analogbufio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/analogio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/atexit/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/audiobusio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/audiocore/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/audioio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/audiomixer/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/audiomp3/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/audiopwmio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/bitbangio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/bitmaptools/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/bitops/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/board/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/busio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/busio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -356,21 +356,17 @@
     due to internal limitations."""
 
 class UART:
     """A bidirectional serial protocol"""
 
     def __init__(
         self,
-        tx: Optional[microcontroller.Pin] = None,
-        rx: Optional[microcontroller.Pin] = None,
+        tx: microcontroller.Pin,
+        rx: microcontroller.Pin,
         *,
-        rts: Optional[microcontroller.Pin] = None,
-        cts: Optional[microcontroller.Pin] = None,
-        rs485_dir: Optional[microcontroller.Pin] = None,
-        rs485_invert: bool = False,
         baudrate: int = 9600,
         bits: int = 8,
         parity: Optional[Parity] = None,
         stop: int = 1,
         timeout: float = 1,
         receiver_buffer_size: int = 64,
     ) -> None:
@@ -386,21 +382,19 @@
         :param int baudrate: the transmit and receive speed.
         :param int bits:  the number of bits per byte, 5 to 9.
         :param Parity parity:  the parity used for error checking.
         :param int stop:  the number of stop bits, 1 or 2.
         :param float timeout:  the timeout in seconds to wait for the first character and between subsequent characters when reading. Raises ``ValueError`` if timeout >100 seconds.
         :param int receiver_buffer_size: the character length of the read buffer (0 to disable). (When a character is 9 bits the buffer will be 2 * receiver_buffer_size bytes.)
 
-        ``tx`` and ``rx`` cannot both be ``None``.
-
         *New in CircuitPython 4.0:* ``timeout`` has incompatibly changed units from milliseconds to seconds.
         The new upper limit on ``timeout`` is meant to catch mistaken use of milliseconds.
 
         **Limitations:** RS485 is not supported on SAMD, nRF, Broadcom, Spresense, or STM.
-        On i.MX and Raspberry Pi RP2040, RS485 support is implemented in software:
+        On i.MX and Raspberry Pi RP2040 support is implemented in software:
         The timing for the ``rs485_dir`` pin signal is done on a best-effort basis, and may not meet
         RS485 specifications intermittently.
         """
         ...
     def deinit(self) -> None:
         """Deinitialises the UART and releases any hardware resources for reuse."""
         ...
```

### Comparing `types-circuitpython-8.0.3/bindings/camera/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/canio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/countio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/countio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/digitalio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/displayio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/dualbank/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/floppyio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/fontio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/framebufferio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/frequencyio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/getpass/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/gifio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/gnss/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/hashlib/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/i2ctarget/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/imagecapture/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/ipaddress/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/is31fl3741/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/keypad/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/math/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/mdns/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/memorymap/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/memorymonitor/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/microcontroller/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/microcontroller/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     Is `None` if the voltage is not available."""
 
 class ResetReason:
     """The reason the microntroller was last reset"""
 
     POWER_ON: object
-    """The microntroller was started from power off."""
+    """The microcontroller was started from power off."""
 
     BROWNOUT: object
     """The microntroller was reset due to too low a voltage."""
 
     SOFTWARE: object
     """The microntroller was reset from software."""
```

### Comparing `types-circuitpython-8.0.3/bindings/msgpack/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/neopixel_write/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/nvm/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/onewireio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/os/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/paralleldisplay/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/ps2io/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/pulseio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/pwmio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/qrio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/random/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/rgbmatrix/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/rotaryio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/rtc/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/sdcardio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/sdioio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/socketpool/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/ssl/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/storage/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/struct/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/supervisor/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/supervisor/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -167,15 +167,20 @@
     serial_connected: bool
     """Returns the USB serial communication status (read-only)."""
     serial_bytes_available: int
     """Returns the whether any bytes are available to read
     on the USB serial input.  Allows for polling to see whether
     to call the built-in input() or wait. (read-only)"""
     run_reason: RunReason
-    """Why CircuitPython started running this particular time."""
+    """Why CircuitPython started running this particular time (read-only)."""
+    safe_mode_reason: SafeModeReason
+    """Why CircuitPython went into safe mode this particular time (read-only).
+
+    **Limitations**: Raises ``NotImplementedError`` on builds that do not implement ``safemode.py``.
+    """
     autoreload: bool
     """Whether CircuitPython may autoreload based on workflow writes to the filesystem."""
 
     ble_workflow: bool
     """Enable/Disable ble workflow until a reset. This prevents BLE advertising outside of the VM and
     the services used for it."""
 
@@ -183,14 +188,75 @@
     """The size of the stack for the next vm run. If its too large, the default will be used."""
 
     rgb_status_brightness: int
     """Set brightness of status RGB LED from 0-255. This will take effect
     after the current code finishes and the status LED is used to show
     the finish state."""
 
+class SafeModeReason:
+    """The reason that CircuitPython went into safe mode.
+
+    **Limitations**: Class not available on builds that do not implement ``safemode.py``.
+    """
+
+    NONE: object
+    """CircuitPython is not in safe mode."""
+
+    BROWNOUT: object
+    """The microcontroller voltage dropped too low."""
+
+    FLASH_WRITE_FAIL: object
+    """Could not write to flash memory."""
+
+    GC_ALLOC_OUTSIDE_VM: object
+    """CircuitPython tried to allocate storage when its virtual machine was not running."""
+
+    HARD_FAULT: object
+    """The microcontroller detected a fault, such as an out-of-bounds memory write."""
+
+    INTERRUPT_ERROR: object
+    """Internal error related to interrupts."""
+
+    NLR_JUMP_FAIL: object
+    """An error occurred during exception handling, possibly due to memory corruption."""
+
+    NO_CIRCUITPY: object
+    """The CIRCUITPY drive was not available."""
+
+    NO_HEAP: object
+    """Heap storage was not present."""
+
+    PROGRAMMATIC: object
+    """The program entered safe mode using the `supervisor` module."""
+
+    SDK_FATAL_ERROR: object
+    """Third party firmware reported a fatal error."""
+
+    STACK_OVERFLOW: object
+    """The CircuitPython heap was corrupted because the stack was too small."""
+
+    USB_BOOT_DEVICE_NOT_INTERFACE_ZERO: object
+    """The USB HID boot device was not set up to be the first device, on interface #0."""
+
+    USB_TOO_MANY_ENDPOINTS: object
+    """USB devices need more endpoints than are available."""
+
+    USB_TOO_MANY_INTERFACE_NAMES: object
+    """USB devices specify too many interface names."""
+
+    USER: object
+    """The user pressed one or more buttons to enter safe mode.
+    This safe mode does **not** cause ``safemode.py`` to be run, since its purpose
+    is to prevent all user code from running.
+    This allows errors in ``safemode.py`` to be corrected easily.
+    """
+
+    SAFE_MODE_WATCHDOG: object
+    """An internal watchdog timer expired."""
+
 class StatusBar:
     """Current status of runtime objects.
 
     Usage::
 
        import supervisor
```

### Comparing `types-circuitpython-8.0.3/bindings/synthio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/terminalio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/time/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/touchio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/traceback/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/usb_cdc/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/usb_hid/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/usb_host/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/usb_midi/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/vectorio/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/watchdog/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/wifi/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/wifi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/bindings/zlib/__init__.pyi` & `types-circuitpython-8.1.0a2/bindings/zlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/setup.py` & `types-circuitpython-8.1.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir, path
 
 from setuptools import setup
 
 __name__ = "types-circuitpython"
-__version__ = "8.0.3"
+__version__ = "8.1.0-alpha.2"
 __repo__ = "https://github.com/hardfury-labs/types-circuitpython"
 __author__ = "HardFury"
 
 
 HERE = path.abspath(path.dirname(__file__))
 BINDINGS_DIR = path.join(HERE, "bindings")
```

### Comparing `types-circuitpython-8.0.3/types_circuitpython.egg-info/PKG-INFO` & `types-circuitpython-8.1.0a2/types_circuitpython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.0.3
+Version: 8.1.0a2
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -42,17 +42,16 @@
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
 - 8.x
   - 8.1.x
-    - 8.1.0a2 (Corresponds 8.1.0-alpha.2 of CircuitPython's version)
+    - 8.1.0-alpha.2
   - 8.0.x
-    - 8.0.3
     - 8.0.2
     - 8.0.0
     - 8.0.0rc2 (Corresponds 8.0.0-rc.2 of CircuitPython's version)
     - 8.0.0rc1 (Corresponds 8.0.0-rc.1 of CircuitPython's version)
     - 8.0.0rc0 (Corresponds 8.0.0-rc.0 of CircuitPython's version)
     - 8.0.0b6 (Corresponds 8.0.0-beta.6 of CircuitPython's version)
     - 8.0.0b5 (Corresponds 8.0.0-beta.5 of CircuitPython's version)
```

### Comparing `types-circuitpython-8.0.3/types_circuitpython.egg-info/SOURCES.txt` & `types-circuitpython-8.1.0a2/types_circuitpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.3/types_circuitpython.egg-info/top_level.txt` & `types-circuitpython-8.1.0a2/types_circuitpython.egg-info/top_level.txt`

 * *Files identical despite different names*

