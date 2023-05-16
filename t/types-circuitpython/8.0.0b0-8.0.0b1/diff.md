# Comparing `tmp/types-circuitpython-8.0.0b0.tar.gz` & `tmp/types-circuitpython-8.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-circuitpython-8.0.0b0.tar", last modified: Thu Sep 15 20:29:34 2022, max compression
+gzip compressed data, was "types-circuitpython-8.0.0b1.tar", last modified: Tue May 16 15:29:11 2023, max compression
```

## Comparing `types-circuitpython-8.0.0b0.tar` & `types-circuitpython-8.0.0b1.tar`

### file list

```diff
@@ -1,186 +1,188 @@
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.174642 types-circuitpython-8.0.0b0/
--rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.0.0b0/LICENSE
--rw-r--r--   0 timon      (501) staff       (20)     2432 2022-09-15 20:29:34.174358 types-circuitpython-8.0.0b0/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     1375 2022-09-15 19:48:13.000000 types-circuitpython-8.0.0b0/README.md
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.128408 types-circuitpython-8.0.0b0/bindings/
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.130624 types-circuitpython-8.0.0b0/bindings/__future__/
--rw-r--r--   0 timon      (501) staff       (20)      579 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/__future__/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.131081 types-circuitpython-8.0.0b0/bindings/_bleio/
--rw-r--r--   0 timon      (501) staff       (20)    31099 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/_bleio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.131646 types-circuitpython-8.0.0b0/bindings/_eve/
--rw-r--r--   0 timon      (501) staff       (20)    20014 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/_eve/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.132109 types-circuitpython-8.0.0b0/bindings/_pew/
--rw-r--r--   0 timon      (501) staff       (20)     1288 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/_pew/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.132445 types-circuitpython-8.0.0b0/bindings/_stage/
--rw-r--r--   0 timon      (501) staff       (20)     3833 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/_stage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.132896 types-circuitpython-8.0.0b0/bindings/adafruit_bus_device/
--rw-r--r--   0 timon      (501) staff       (20)      370 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.133262 types-circuitpython-8.0.0b0/bindings/adafruit_pixelbuf/
--rw-r--r--   0 timon      (501) staff       (20)     4136 2022-09-15 20:29:26.000000 types-circuitpython-8.0.0b0/bindings/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.133581 types-circuitpython-8.0.0b0/bindings/aesio/
--rw-r--r--   0 timon      (501) staff       (20)     2046 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/aesio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.133904 types-circuitpython-8.0.0b0/bindings/alarm/
--rw-r--r--   0 timon      (501) staff       (20)     5464 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/alarm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.134236 types-circuitpython-8.0.0b0/bindings/analogio/
--rw-r--r--   0 timon      (501) staff       (20)     3580 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/analogio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.134810 types-circuitpython-8.0.0b0/bindings/atexit/
--rw-r--r--   0 timon      (501) staff       (20)     1619 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/atexit/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.135461 types-circuitpython-8.0.0b0/bindings/audiobusio/
--rw-r--r--   0 timon      (501) staff       (20)     7424 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/audiobusio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.136046 types-circuitpython-8.0.0b0/bindings/audiocore/
--rw-r--r--   0 timon      (501) staff       (20)     4555 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/audiocore/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.136649 types-circuitpython-8.0.0b0/bindings/audioio/
--rw-r--r--   0 timon      (501) staff       (20)     4323 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/audioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.137353 types-circuitpython-8.0.0b0/bindings/audiomixer/
--rw-r--r--   0 timon      (501) staff       (20)     4418 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/audiomixer/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.137984 types-circuitpython-8.0.0b0/bindings/audiomp3/
--rw-r--r--   0 timon      (501) staff       (20)     3675 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/audiomp3/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.138470 types-circuitpython-8.0.0b0/bindings/audiopwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4227 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/audiopwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.138923 types-circuitpython-8.0.0b0/bindings/bitbangio/
--rw-r--r--   0 timon      (501) staff       (20)    12037 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/bitbangio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.139465 types-circuitpython-8.0.0b0/bindings/bitmaptools/
--rw-r--r--   0 timon      (501) staff       (20)    10918 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/bitmaptools/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.139967 types-circuitpython-8.0.0b0/bindings/bitops/
--rw-r--r--   0 timon      (501) staff       (20)     1236 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/bitops/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.140441 types-circuitpython-8.0.0b0/bindings/board/
--rw-r--r--   0 timon      (501) staff       (20)     1547 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/board/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.140908 types-circuitpython-8.0.0b0/bindings/busio/
--rw-r--r--   0 timon      (501) staff       (20)    19265 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/busio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.141551 types-circuitpython-8.0.0b0/bindings/camera/
--rw-r--r--   0 timon      (501) staff       (20)     1549 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/camera/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.142046 types-circuitpython-8.0.0b0/bindings/canio/
--rw-r--r--   0 timon      (501) staff       (20)    10887 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/canio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.142499 types-circuitpython-8.0.0b0/bindings/countio/
--rw-r--r--   0 timon      (501) staff       (20)     2505 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/countio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.142989 types-circuitpython-8.0.0b0/bindings/digitalio/
--rw-r--r--   0 timon      (501) staff       (20)     5165 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/digitalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.143506 types-circuitpython-8.0.0b0/bindings/displayio/
--rw-r--r--   0 timon      (501) staff       (20)    38226 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/displayio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.144476 types-circuitpython-8.0.0b0/bindings/dotenv/
--rw-r--r--   0 timon      (501) staff       (20)     1345 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/dotenv/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.144940 types-circuitpython-8.0.0b0/bindings/dualbank/
--rw-r--r--   0 timon      (501) staff       (20)     1225 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/dualbank/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.145374 types-circuitpython-8.0.0b0/bindings/floppyio/
--rw-r--r--   0 timon      (501) staff       (20)     1573 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/floppyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.145879 types-circuitpython-8.0.0b0/bindings/fontio/
--rw-r--r--   0 timon      (501) staff       (20)     3049 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/fontio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.146328 types-circuitpython-8.0.0b0/bindings/framebufferio/
--rw-r--r--   0 timon      (501) staff       (20)     3532 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/framebufferio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.146760 types-circuitpython-8.0.0b0/bindings/frequencyio/
--rw-r--r--   0 timon      (501) staff       (20)     3462 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/frequencyio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.147203 types-circuitpython-8.0.0b0/bindings/getpass/
--rw-r--r--   0 timon      (501) staff       (20)      546 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/getpass/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.147629 types-circuitpython-8.0.0b0/bindings/gifio/
--rw-r--r--   0 timon      (501) staff       (20)     1834 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/gifio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.148098 types-circuitpython-8.0.0b0/bindings/gnss/
--rw-r--r--   0 timon      (501) staff       (20)     2457 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/gnss/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.148549 types-circuitpython-8.0.0b0/bindings/hashlib/
--rw-r--r--   0 timon      (501) staff       (20)      989 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/hashlib/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.148972 types-circuitpython-8.0.0b0/bindings/i2ctarget/
--rw-r--r--   0 timon      (501) staff       (20)     5397 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/i2ctarget/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.149396 types-circuitpython-8.0.0b0/bindings/imagecapture/
--rw-r--r--   0 timon      (501) staff       (20)     2886 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/imagecapture/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.149838 types-circuitpython-8.0.0b0/bindings/ipaddress/
--rw-r--r--   0 timon      (501) staff       (20)      991 2022-09-15 20:29:27.000000 types-circuitpython-8.0.0b0/bindings/ipaddress/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.150282 types-circuitpython-8.0.0b0/bindings/is31fl3741/
--rw-r--r--   0 timon      (501) staff       (20)     3870 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/is31fl3741/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.150712 types-circuitpython-8.0.0b0/bindings/keypad/
--rw-r--r--   0 timon      (501) staff       (20)    13077 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/keypad/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.151300 types-circuitpython-8.0.0b0/bindings/math/
--rw-r--r--   0 timon      (501) staff       (20)     4805 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/math/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.151860 types-circuitpython-8.0.0b0/bindings/mdns/
--rw-r--r--   0 timon      (501) staff       (20)     3234 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/mdns/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.152367 types-circuitpython-8.0.0b0/bindings/memorymonitor/
--rw-r--r--   0 timon      (501) staff       (20)     3321 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/memorymonitor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.152952 types-circuitpython-8.0.0b0/bindings/microcontroller/
--rw-r--r--   0 timon      (501) staff       (20)     5739 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/microcontroller/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.153579 types-circuitpython-8.0.0b0/bindings/msgpack/
--rw-r--r--   0 timon      (501) staff       (20)     2898 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/msgpack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.154187 types-circuitpython-8.0.0b0/bindings/multiterminal/
--rw-r--r--   0 timon      (501) staff       (20)     1112 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/multiterminal/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.154776 types-circuitpython-8.0.0b0/bindings/neopixel_write/
--rw-r--r--   0 timon      (501) staff       (20)     1367 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/neopixel_write/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.155249 types-circuitpython-8.0.0b0/bindings/nvm/
--rw-r--r--   0 timon      (501) staff       (20)     1500 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/nvm/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.155746 types-circuitpython-8.0.0b0/bindings/onewireio/
--rw-r--r--   0 timon      (501) staff       (20)     1646 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/onewireio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.156300 types-circuitpython-8.0.0b0/bindings/os/
--rw-r--r--   0 timon      (501) staff       (20)     2962 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/os/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.156844 types-circuitpython-8.0.0b0/bindings/paralleldisplay/
--rw-r--r--   0 timon      (501) staff       (20)     2415 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.157395 types-circuitpython-8.0.0b0/bindings/ps2io/
--rw-r--r--   0 timon      (501) staff       (20)     3619 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/ps2io/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.157975 types-circuitpython-8.0.0b0/bindings/pulseio/
--rw-r--r--   0 timon      (501) staff       (20)     6309 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/pulseio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.158445 types-circuitpython-8.0.0b0/bindings/pwmio/
--rw-r--r--   0 timon      (501) staff       (20)     4873 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/pwmio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.159002 types-circuitpython-8.0.0b0/bindings/qrio/
--rw-r--r--   0 timon      (501) staff       (20)     2571 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/qrio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.159510 types-circuitpython-8.0.0b0/bindings/rainbowio/
--rw-r--r--   0 timon      (501) staff       (20)      327 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/rainbowio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.160588 types-circuitpython-8.0.0b0/bindings/random/
--rw-r--r--   0 timon      (501) staff       (20)     1670 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/random/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.161575 types-circuitpython-8.0.0b0/bindings/rgbmatrix/
--rw-r--r--   0 timon      (501) staff       (20)     3385 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.162114 types-circuitpython-8.0.0b0/bindings/rotaryio/
--rw-r--r--   0 timon      (501) staff       (20)     2517 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/rotaryio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.162620 types-circuitpython-8.0.0b0/bindings/rtc/
--rw-r--r--   0 timon      (501) staff       (20)     1873 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/rtc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.162996 types-circuitpython-8.0.0b0/bindings/sdcardio/
--rw-r--r--   0 timon      (501) staff       (20)     2861 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/sdcardio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.163320 types-circuitpython-8.0.0b0/bindings/sdioio/
--rw-r--r--   0 timon      (501) staff       (20)     3695 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/sdioio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.163633 types-circuitpython-8.0.0b0/bindings/sharpdisplay/
--rw-r--r--   0 timon      (501) staff       (20)      276 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.164031 types-circuitpython-8.0.0b0/bindings/socketpool/
--rw-r--r--   0 timon      (501) staff       (20)     5114 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/socketpool/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.164350 types-circuitpython-8.0.0b0/bindings/ssl/
--rw-r--r--   0 timon      (501) staff       (20)     4124 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/ssl/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.164679 types-circuitpython-8.0.0b0/bindings/storage/
--rw-r--r--   0 timon      (501) staff       (20)     4888 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/storage/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.165027 types-circuitpython-8.0.0b0/bindings/struct/
--rw-r--r--   0 timon      (501) staff       (20)     1589 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/struct/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.165480 types-circuitpython-8.0.0b0/bindings/supervisor/
--rw-r--r--   0 timon      (501) staff       (20)     6782 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/supervisor/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.165864 types-circuitpython-8.0.0b0/bindings/synthio/
--rw-r--r--   0 timon      (501) staff       (20)     2781 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/synthio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.166186 types-circuitpython-8.0.0b0/bindings/terminalio/
--rw-r--r--   0 timon      (501) staff       (20)     1712 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/terminalio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.166508 types-circuitpython-8.0.0b0/bindings/time/
--rw-r--r--   0 timon      (501) staff       (20)     3466 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/time/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.166983 types-circuitpython-8.0.0b0/bindings/touchio/
--rw-r--r--   0 timon      (501) staff       (20)     2387 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/touchio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.167564 types-circuitpython-8.0.0b0/bindings/traceback/
--rw-r--r--   0 timon      (501) staff       (20)     2870 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/traceback/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.168138 types-circuitpython-8.0.0b0/bindings/uheap/
--rw-r--r--   0 timon      (501) staff       (20)      199 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/uheap/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.168691 types-circuitpython-8.0.0b0/bindings/usb/
--rw-r--r--   0 timon      (501) staff       (20)      152 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/usb/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.169236 types-circuitpython-8.0.0b0/bindings/usb_cdc/
--rw-r--r--   0 timon      (501) staff       (20)     5682 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/usb_cdc/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.169778 types-circuitpython-8.0.0b0/bindings/usb_hid/
--rw-r--r--   0 timon      (501) staff       (20)     8353 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/usb_hid/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.170305 types-circuitpython-8.0.0b0/bindings/usb_host/
--rw-r--r--   0 timon      (501) staff       (20)     1124 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/usb_host/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.170681 types-circuitpython-8.0.0b0/bindings/usb_midi/
--rw-r--r--   0 timon      (501) staff       (20)     2802 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/usb_midi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.171006 types-circuitpython-8.0.0b0/bindings/ustack/
--rw-r--r--   0 timon      (501) staff       (20)      503 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/ustack/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.171326 types-circuitpython-8.0.0b0/bindings/vectorio/
--rw-r--r--   0 timon      (501) staff       (20)     4648 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/vectorio/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.171667 types-circuitpython-8.0.0b0/bindings/watchdog/
--rw-r--r--   0 timon      (501) staff       (20)     3269 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/watchdog/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.172095 types-circuitpython-8.0.0b0/bindings/wifi/
--rw-r--r--   0 timon      (501) staff       (20)     8823 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/wifi/__init__.pyi
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.172424 types-circuitpython-8.0.0b0/bindings/zlib/
--rw-r--r--   0 timon      (501) staff       (20)     1339 2022-09-15 20:29:28.000000 types-circuitpython-8.0.0b0/bindings/zlib/__init__.pyi
--rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.0.0b0/pyproject.toml
--rw-r--r--   0 timon      (501) staff       (20)       38 2022-09-15 20:29:34.174738 types-circuitpython-8.0.0b0/setup.cfg
--rw-r--r--   0 timon      (501) staff       (20)     2181 2022-09-15 20:29:29.000000 types-circuitpython-8.0.0b0/setup.py
-drwxr-xr-x   0 timon      (501) staff       (20)        0 2022-09-15 20:29:34.173959 types-circuitpython-8.0.0b0/types_circuitpython.egg-info/
--rw-r--r--   0 timon      (501) staff       (20)     2432 2022-09-15 20:29:34.000000 types-circuitpython-8.0.0b0/types_circuitpython.egg-info/PKG-INFO
--rw-r--r--   0 timon      (501) staff       (20)     2892 2022-09-15 20:29:34.000000 types-circuitpython-8.0.0b0/types_circuitpython.egg-info/SOURCES.txt
--rw-r--r--   0 timon      (501) staff       (20)        1 2022-09-15 20:29:34.000000 types-circuitpython-8.0.0b0/types_circuitpython.egg-info/dependency_links.txt
--rw-r--r--   0 timon      (501) staff       (20)       30 2022-09-15 20:29:34.000000 types-circuitpython-8.0.0b0/types_circuitpython.egg-info/requires.txt
--rw-r--r--   0 timon      (501) staff       (20)      745 2022-09-15 20:29:34.000000 types-circuitpython-8.0.0b0/types_circuitpython.egg-info/top_level.txt
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.897533 types-circuitpython-8.0.0b1/
+-rw-r--r--   0 timon      (501) staff       (20)    35149 2022-09-11 11:33:25.000000 types-circuitpython-8.0.0b1/LICENSE
+-rw-r--r--   0 timon      (501) staff       (20)     2694 2023-05-16 15:29:11.897201 types-circuitpython-8.0.0b1/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     1637 2023-05-16 15:24:44.000000 types-circuitpython-8.0.0b1/README.md
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.853282 types-circuitpython-8.0.0b1/bindings/
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.856433 types-circuitpython-8.0.0b1/bindings/__future__/
+-rw-r--r--   0 timon      (501) staff       (20)      579 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/__future__/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.856847 types-circuitpython-8.0.0b1/bindings/_bleio/
+-rw-r--r--   0 timon      (501) staff       (20)    31068 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/_bleio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.857302 types-circuitpython-8.0.0b1/bindings/_eve/
+-rw-r--r--   0 timon      (501) staff       (20)    20082 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/_eve/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.857688 types-circuitpython-8.0.0b1/bindings/_pew/
+-rw-r--r--   0 timon      (501) staff       (20)     1288 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/_pew/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.858029 types-circuitpython-8.0.0b1/bindings/_stage/
+-rw-r--r--   0 timon      (501) staff       (20)     3833 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/_stage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.858374 types-circuitpython-8.0.0b1/bindings/adafruit_bus_device/
+-rw-r--r--   0 timon      (501) staff       (20)      370 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.858703 types-circuitpython-8.0.0b1/bindings/adafruit_pixelbuf/
+-rw-r--r--   0 timon      (501) staff       (20)     4132 2023-05-16 15:28:59.000000 types-circuitpython-8.0.0b1/bindings/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.859033 types-circuitpython-8.0.0b1/bindings/aesio/
+-rw-r--r--   0 timon      (501) staff       (20)     2171 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/aesio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.859374 types-circuitpython-8.0.0b1/bindings/alarm/
+-rw-r--r--   0 timon      (501) staff       (20)     6891 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/alarm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.859741 types-circuitpython-8.0.0b1/bindings/analogbufio/
+-rw-r--r--   0 timon      (501) staff       (20)     3271 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/analogbufio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.860220 types-circuitpython-8.0.0b1/bindings/analogio/
+-rw-r--r--   0 timon      (501) staff       (20)     3579 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/analogio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.860553 types-circuitpython-8.0.0b1/bindings/atexit/
+-rw-r--r--   0 timon      (501) staff       (20)     1619 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/atexit/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.860900 types-circuitpython-8.0.0b1/bindings/audiobusio/
+-rw-r--r--   0 timon      (501) staff       (20)     7346 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/audiobusio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.861307 types-circuitpython-8.0.0b1/bindings/audiocore/
+-rw-r--r--   0 timon      (501) staff       (20)     4614 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/audiocore/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.861652 types-circuitpython-8.0.0b1/bindings/audioio/
+-rw-r--r--   0 timon      (501) staff       (20)     4505 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/audioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.862141 types-circuitpython-8.0.0b1/bindings/audiomixer/
+-rw-r--r--   0 timon      (501) staff       (20)     4415 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/audiomixer/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.862547 types-circuitpython-8.0.0b1/bindings/audiomp3/
+-rw-r--r--   0 timon      (501) staff       (20)     3897 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/audiomp3/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.862913 types-circuitpython-8.0.0b1/bindings/audiopwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4226 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/audiopwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.863267 types-circuitpython-8.0.0b1/bindings/bitbangio/
+-rw-r--r--   0 timon      (501) staff       (20)    12038 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/bitbangio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.863611 types-circuitpython-8.0.0b1/bindings/bitmaptools/
+-rw-r--r--   0 timon      (501) staff       (20)    10928 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/bitmaptools/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.863941 types-circuitpython-8.0.0b1/bindings/bitops/
+-rw-r--r--   0 timon      (501) staff       (20)     1236 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/bitops/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.864265 types-circuitpython-8.0.0b1/bindings/board/
+-rw-r--r--   0 timon      (501) staff       (20)     1547 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/board/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.864589 types-circuitpython-8.0.0b1/bindings/busio/
+-rw-r--r--   0 timon      (501) staff       (20)    19547 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/busio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.864988 types-circuitpython-8.0.0b1/bindings/camera/
+-rw-r--r--   0 timon      (501) staff       (20)     1549 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/camera/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.865305 types-circuitpython-8.0.0b1/bindings/canio/
+-rw-r--r--   0 timon      (501) staff       (20)    11023 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/canio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.865637 types-circuitpython-8.0.0b1/bindings/countio/
+-rw-r--r--   0 timon      (501) staff       (20)     2681 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/countio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.865966 types-circuitpython-8.0.0b1/bindings/digitalio/
+-rw-r--r--   0 timon      (501) staff       (20)     5162 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/digitalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.866291 types-circuitpython-8.0.0b1/bindings/displayio/
+-rw-r--r--   0 timon      (501) staff       (20)    38193 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/displayio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.866701 types-circuitpython-8.0.0b1/bindings/dotenv/
+-rw-r--r--   0 timon      (501) staff       (20)     1345 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/dotenv/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.867024 types-circuitpython-8.0.0b1/bindings/dualbank/
+-rw-r--r--   0 timon      (501) staff       (20)     1224 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/dualbank/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.867346 types-circuitpython-8.0.0b1/bindings/floppyio/
+-rw-r--r--   0 timon      (501) staff       (20)     1573 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/floppyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.867675 types-circuitpython-8.0.0b1/bindings/fontio/
+-rw-r--r--   0 timon      (501) staff       (20)     3048 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/fontio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.868001 types-circuitpython-8.0.0b1/bindings/framebufferio/
+-rw-r--r--   0 timon      (501) staff       (20)     3526 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/framebufferio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.868337 types-circuitpython-8.0.0b1/bindings/frequencyio/
+-rw-r--r--   0 timon      (501) staff       (20)     3461 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/frequencyio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.868814 types-circuitpython-8.0.0b1/bindings/getpass/
+-rw-r--r--   0 timon      (501) staff       (20)      546 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/getpass/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.869187 types-circuitpython-8.0.0b1/bindings/gifio/
+-rw-r--r--   0 timon      (501) staff       (20)     1834 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/gifio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.869682 types-circuitpython-8.0.0b1/bindings/gnss/
+-rw-r--r--   0 timon      (501) staff       (20)     2453 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/gnss/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.870186 types-circuitpython-8.0.0b1/bindings/hashlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1002 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/hashlib/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.870701 types-circuitpython-8.0.0b1/bindings/i2ctarget/
+-rw-r--r--   0 timon      (501) staff       (20)     5394 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/i2ctarget/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.871296 types-circuitpython-8.0.0b1/bindings/imagecapture/
+-rw-r--r--   0 timon      (501) staff       (20)     2886 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/imagecapture/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.871821 types-circuitpython-8.0.0b1/bindings/ipaddress/
+-rw-r--r--   0 timon      (501) staff       (20)      989 2023-05-16 15:29:00.000000 types-circuitpython-8.0.0b1/bindings/ipaddress/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.872342 types-circuitpython-8.0.0b1/bindings/is31fl3741/
+-rw-r--r--   0 timon      (501) staff       (20)     3868 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/is31fl3741/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.872863 types-circuitpython-8.0.0b1/bindings/keypad/
+-rw-r--r--   0 timon      (501) staff       (20)    13070 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/keypad/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.873385 types-circuitpython-8.0.0b1/bindings/math/
+-rw-r--r--   0 timon      (501) staff       (20)     4805 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/math/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.873902 types-circuitpython-8.0.0b1/bindings/mdns/
+-rw-r--r--   0 timon      (501) staff       (20)     3226 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/mdns/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.874381 types-circuitpython-8.0.0b1/bindings/memorymonitor/
+-rw-r--r--   0 timon      (501) staff       (20)     3320 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/memorymonitor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.874837 types-circuitpython-8.0.0b1/bindings/microcontroller/
+-rw-r--r--   0 timon      (501) staff       (20)     5733 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/microcontroller/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.875302 types-circuitpython-8.0.0b1/bindings/msgpack/
+-rw-r--r--   0 timon      (501) staff       (20)     2897 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/msgpack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.875733 types-circuitpython-8.0.0b1/bindings/multiterminal/
+-rw-r--r--   0 timon      (501) staff       (20)     1112 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/multiterminal/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.876267 types-circuitpython-8.0.0b1/bindings/neopixel_write/
+-rw-r--r--   0 timon      (501) staff       (20)     1367 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/neopixel_write/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.876900 types-circuitpython-8.0.0b1/bindings/nvm/
+-rw-r--r--   0 timon      (501) staff       (20)     1499 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/nvm/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.877579 types-circuitpython-8.0.0b1/bindings/onewireio/
+-rw-r--r--   0 timon      (501) staff       (20)     1646 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/onewireio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.878208 types-circuitpython-8.0.0b1/bindings/os/
+-rw-r--r--   0 timon      (501) staff       (20)     3569 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/os/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.878843 types-circuitpython-8.0.0b1/bindings/paralleldisplay/
+-rw-r--r--   0 timon      (501) staff       (20)     2415 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.879666 types-circuitpython-8.0.0b1/bindings/ps2io/
+-rw-r--r--   0 timon      (501) staff       (20)     3619 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/ps2io/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.880535 types-circuitpython-8.0.0b1/bindings/pulseio/
+-rw-r--r--   0 timon      (501) staff       (20)     6307 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/pulseio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.881369 types-circuitpython-8.0.0b1/bindings/pwmio/
+-rw-r--r--   0 timon      (501) staff       (20)     4872 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/pwmio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.882055 types-circuitpython-8.0.0b1/bindings/qrio/
+-rw-r--r--   0 timon      (501) staff       (20)     2570 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/qrio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.882668 types-circuitpython-8.0.0b1/bindings/rainbowio/
+-rw-r--r--   0 timon      (501) staff       (20)      327 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/rainbowio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.883249 types-circuitpython-8.0.0b1/bindings/random/
+-rw-r--r--   0 timon      (501) staff       (20)     1670 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/random/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.883800 types-circuitpython-8.0.0b1/bindings/rgbmatrix/
+-rw-r--r--   0 timon      (501) staff       (20)     3383 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.884333 types-circuitpython-8.0.0b1/bindings/rotaryio/
+-rw-r--r--   0 timon      (501) staff       (20)     2659 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/rotaryio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.885145 types-circuitpython-8.0.0b1/bindings/rtc/
+-rw-r--r--   0 timon      (501) staff       (20)     1872 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/rtc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.885601 types-circuitpython-8.0.0b1/bindings/sdcardio/
+-rw-r--r--   0 timon      (501) staff       (20)     2861 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/sdcardio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.886192 types-circuitpython-8.0.0b1/bindings/sdioio/
+-rw-r--r--   0 timon      (501) staff       (20)     3605 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/sdioio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.886674 types-circuitpython-8.0.0b1/bindings/sharpdisplay/
+-rw-r--r--   0 timon      (501) staff       (20)      276 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.887048 types-circuitpython-8.0.0b1/bindings/socketpool/
+-rw-r--r--   0 timon      (501) staff       (20)     5473 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/socketpool/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.887515 types-circuitpython-8.0.0b1/bindings/ssl/
+-rw-r--r--   0 timon      (501) staff       (20)     4123 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/ssl/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.887907 types-circuitpython-8.0.0b1/bindings/storage/
+-rw-r--r--   0 timon      (501) staff       (20)     4889 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/storage/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.888285 types-circuitpython-8.0.0b1/bindings/struct/
+-rw-r--r--   0 timon      (501) staff       (20)     1589 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/struct/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.888693 types-circuitpython-8.0.0b1/bindings/supervisor/
+-rw-r--r--   0 timon      (501) staff       (20)     8703 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/supervisor/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.889255 types-circuitpython-8.0.0b1/bindings/synthio/
+-rw-r--r--   0 timon      (501) staff       (20)     2781 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/synthio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.889940 types-circuitpython-8.0.0b1/bindings/terminalio/
+-rw-r--r--   0 timon      (501) staff       (20)     1713 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/terminalio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.890556 types-circuitpython-8.0.0b1/bindings/time/
+-rw-r--r--   0 timon      (501) staff       (20)     3466 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/time/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.890929 types-circuitpython-8.0.0b1/bindings/touchio/
+-rw-r--r--   0 timon      (501) staff       (20)     2385 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/touchio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.891277 types-circuitpython-8.0.0b1/bindings/traceback/
+-rw-r--r--   0 timon      (501) staff       (20)     2870 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/traceback/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.891623 types-circuitpython-8.0.0b1/bindings/uheap/
+-rw-r--r--   0 timon      (501) staff       (20)      199 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/uheap/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.891971 types-circuitpython-8.0.0b1/bindings/usb/
+-rw-r--r--   0 timon      (501) staff       (20)      152 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/usb/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.892332 types-circuitpython-8.0.0b1/bindings/usb_cdc/
+-rw-r--r--   0 timon      (501) staff       (20)     5696 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/usb_cdc/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.892682 types-circuitpython-8.0.0b1/bindings/usb_hid/
+-rw-r--r--   0 timon      (501) staff       (20)     8198 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/usb_hid/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.893037 types-circuitpython-8.0.0b1/bindings/usb_host/
+-rw-r--r--   0 timon      (501) staff       (20)     1124 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/usb_host/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.893381 types-circuitpython-8.0.0b1/bindings/usb_midi/
+-rw-r--r--   0 timon      (501) staff       (20)     2802 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/usb_midi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.893715 types-circuitpython-8.0.0b1/bindings/ustack/
+-rw-r--r--   0 timon      (501) staff       (20)      503 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/ustack/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.894059 types-circuitpython-8.0.0b1/bindings/vectorio/
+-rw-r--r--   0 timon      (501) staff       (20)     4641 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/vectorio/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.894414 types-circuitpython-8.0.0b1/bindings/watchdog/
+-rw-r--r--   0 timon      (501) staff       (20)     3268 2023-05-16 15:29:01.000000 types-circuitpython-8.0.0b1/bindings/watchdog/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.894761 types-circuitpython-8.0.0b1/bindings/wifi/
+-rw-r--r--   0 timon      (501) staff       (20)     8804 2023-05-16 15:29:02.000000 types-circuitpython-8.0.0b1/bindings/wifi/__init__.pyi
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.895121 types-circuitpython-8.0.0b1/bindings/zlib/
+-rw-r--r--   0 timon      (501) staff       (20)     1339 2023-05-16 15:29:02.000000 types-circuitpython-8.0.0b1/bindings/zlib/__init__.pyi
+-rw-r--r--   0 timon      (501) staff       (20)      235 2022-09-15 19:24:03.000000 types-circuitpython-8.0.0b1/pyproject.toml
+-rw-r--r--   0 timon      (501) staff       (20)       38 2023-05-16 15:29:11.897632 types-circuitpython-8.0.0b1/setup.cfg
+-rw-r--r--   0 timon      (501) staff       (20)     2181 2023-05-16 15:29:02.000000 types-circuitpython-8.0.0b1/setup.py
+drwxr-xr-x   0 timon      (501) staff       (20)        0 2023-05-16 15:29:11.896797 types-circuitpython-8.0.0b1/types_circuitpython.egg-info/
+-rw-r--r--   0 timon      (501) staff       (20)     2694 2023-05-16 15:29:11.000000 types-circuitpython-8.0.0b1/types_circuitpython.egg-info/PKG-INFO
+-rw-r--r--   0 timon      (501) staff       (20)     2926 2023-05-16 15:29:11.000000 types-circuitpython-8.0.0b1/types_circuitpython.egg-info/SOURCES.txt
+-rw-r--r--   0 timon      (501) staff       (20)        1 2023-05-16 15:29:11.000000 types-circuitpython-8.0.0b1/types_circuitpython.egg-info/dependency_links.txt
+-rw-r--r--   0 timon      (501) staff       (20)       30 2023-05-16 15:29:11.000000 types-circuitpython-8.0.0b1/types_circuitpython.egg-info/requires.txt
+-rw-r--r--   0 timon      (501) staff       (20)      757 2023-05-16 15:29:11.000000 types-circuitpython-8.0.0b1/types_circuitpython.egg-info/top_level.txt
```

### Comparing `types-circuitpython-8.0.0b0/LICENSE` & `types-circuitpython-8.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/PKG-INFO` & `types-circuitpython-8.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.0.0b0
+Version: 8.0.0b1
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -26,39 +26,44 @@
 # types-circuitpython
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-circuitpython?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/types-circuitpython?style=flat-square)
 
 Type Support (typings) for [CircuitPython](https://github.com/adafruit/circuitpython) built-in binding packages.
 
-Coding with adafruit-circuitpython-typing:
+Coding with `adafruit-circuitpython-typing`:
 
 ![adafruit-circuitpython-typing](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/adafruit-circuitpython-typing.gif)
 
-Coding with types-circuitpython:
+Coding with `types-circuitpython`:
 
 ![types-circuitpython](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/types-circuitpython.gif)
 
 ## Long term support versions
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
+- 8.x
+  - 8.0.0b0 (Corresponds 8.0.0-beta.0 of CircuitPython)
+  - 8.0.0a1 (Corresponds 8.0.0-alpha.1 of CircuitPython)
+  - 8.0.0a0 (Corresponds 8.0.0-alpha.0 of CircuitPython)
 - 7.x
   - 7.3.3
-- 8.x
-  - 8.0.0-beta.0
+  - 7.3.2
+  - 7.3.1
+  - 7.3.0
 
 ## Usage
 
 ```bash
 $ pip install types-circuitpython==7.3.3
 # or
-$ pip install types-circuitpython==8.0.0-beta.0
+$ pip install types-circuitpython==8.0.0b0
 ```
 
 ## Development
 
 ## Initialization
 
 ```bash
@@ -66,14 +71,20 @@
 $ . ./.venv/bin/activate
 $ pip install -r requirements.txt
 $ python setup.py develop
 # or
 $ pip install -e .
 ```
 
+## Update CircuitPython submodule
+
+```bash
+$ git submodule update --remote
+```
+
 ## Generate bindings
 
 ```bash
 $ make generate version=<CIRCUITPYTHON VERSION>
 ```
 
 ## Code styles
```

### Comparing `types-circuitpython-8.0.0b0/README.md` & `types-circuitpython-8.0.0b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # types-circuitpython
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-circuitpython?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/types-circuitpython?style=flat-square)
 
 Type Support (typings) for [CircuitPython](https://github.com/adafruit/circuitpython) built-in binding packages.
 
-Coding with adafruit-circuitpython-typing:
+Coding with `adafruit-circuitpython-typing`:
 
 ![adafruit-circuitpython-typing](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/adafruit-circuitpython-typing.gif)
 
-Coding with types-circuitpython:
+Coding with `types-circuitpython`:
 
 ![types-circuitpython](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/types-circuitpython.gif)
 
 ## Long term support versions
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
+- 8.x
+  - 8.0.0b0 (Corresponds 8.0.0-beta.0 of CircuitPython)
+  - 8.0.0a1 (Corresponds 8.0.0-alpha.1 of CircuitPython)
+  - 8.0.0a0 (Corresponds 8.0.0-alpha.0 of CircuitPython)
 - 7.x
   - 7.3.3
-- 8.x
-  - 8.0.0-beta.0
+  - 7.3.2
+  - 7.3.1
+  - 7.3.0
 
 ## Usage
 
 ```bash
 $ pip install types-circuitpython==7.3.3
 # or
-$ pip install types-circuitpython==8.0.0-beta.0
+$ pip install types-circuitpython==8.0.0b0
 ```
 
 ## Development
 
 ## Initialization
 
 ```bash
@@ -41,14 +46,20 @@
 $ . ./.venv/bin/activate
 $ pip install -r requirements.txt
 $ python setup.py develop
 # or
 $ pip install -e .
 ```
 
+## Update CircuitPython submodule
+
+```bash
+$ git submodule update --remote
+```
+
 ## Generate bindings
 
 ```bash
 $ make generate version=<CIRCUITPYTHON VERSION>
 ```
 
 ## Code styles
```

### Comparing `types-circuitpython-8.0.0b0/bindings/__future__/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/__future__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/_bleio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/_bleio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -80,23 +80,20 @@
         On boards with native BLE, you cannot create an instance of `_bleio.Adapter`;
         this constructor will raise `NotImplementedError`.
         Use `_bleio.adapter` to access the sole instance already available.
         """
         ...
     enabled: bool
     """State of the BLE adapter."""
-
     address: Address
     """MAC address of the BLE adapter."""
-
     name: str
     """name of the BLE adapter used once connected.
     The name is "CIRCUITPY" + the last four hex digits of ``adapter.address``,
     to make it easy to distinguish multiple CircuitPython boards."""
-
     def start_advertising(
         self,
         data: ReadableBuffer,
         *,
         scan_response: Optional[ReadableBuffer] = None,
         connectable: bool = True,
         anonymous: bool = False,
@@ -157,23 +154,20 @@
         :rtype: iterable"""
         ...
     def stop_scan(self) -> None:
         """Stop the current scan."""
         ...
     advertising: bool
     """True when the adapter is currently advertising. (read-only)"""
-
     connected: bool
     """True when the adapter is connected to another device regardless of who initiated the
     connection. (read-only)"""
-
     connections: Tuple[Connection]
     """Tuple of active connections including those initiated through
     :py:meth:`_bleio.Adapter.connect`. (read-only)"""
-
     def connect(self, address: Address, *, timeout: float) -> Connection:
         """Attempts a connection to the device with the given address.
 
         :param Address address: The address of the peripheral to connect to
         :param float/int timeout: Try to connect for timeout seconds."""
         ...
     def erase_bonding(self) -> None:
@@ -203,21 +197,19 @@
     .. code-block:: python
 
       >>> import _bleio
       >>> _bleio.adapter.address
       <Address c8:1d:f5:ed:a8:35>
       >>> _bleio.adapter.address.address_bytes
       b'5\\xa8\\xed\\xf5\\x1d\\xc8'"""
-
     type: int
     """The address type (read-only).
 
     One of the integer values: `PUBLIC`, `RANDOM_STATIC`, `RANDOM_PRIVATE_RESOLVABLE`,
     or `RANDOM_PRIVATE_NON_RESOLVABLE`."""
-
     def __eq__(self, other: object) -> bool:
         """Two Address objects are equal if their addresses and address types are equal."""
         ...
     def __hash__(self) -> int:
         """Returns a hash for the Address data."""
         ...
     PUBLIC: int
@@ -310,32 +302,26 @@
 
         :return: the new Characteristic."""
         ...
     properties: int
     """An int bitmask representing which properties are set, specified as bitwise or'ing of
     of these possible values.
     `BROADCAST`, `INDICATE`, `NOTIFY`, `READ`, `WRITE`, `WRITE_NO_RESPONSE`."""
-
     uuid: Optional[UUID]
     """The UUID of this characteristic. (read-only)
 
     Will be ``None`` if the 128-bit UUID for this characteristic is not known."""
-
     value: bytearray
     """The value of this characteristic."""
-
     max_length: int
     """The max length of this characteristic."""
-
     descriptors: Descriptor
     """A tuple of :py:class:`Descriptor` objects related to this characteristic. (read-only)"""
-
     service: Service
     """The Service this Characteristic is a part of."""
-
     def set_cccd(self, *, notify: bool = False, indicate: bool = False) -> None:
         """Set the remote characteristic's CCCD to enable or disable notification and indication.
 
         :param bool notify: True if Characteristic should receive notifications of remote writes
         :param float indicate: True if Characteristic should receive indications of remote writes"""
         ...
     BROADCAST: int
@@ -392,15 +378,14 @@
         """Read a line, ending in a newline character.
 
         :return: the line read
         :rtype: int or None"""
         ...
     in_waiting: int
     """The number of bytes in the input buffer, available to be read"""
-
     def reset_input_buffer(self) -> None:
         """Discard any unread characters in the input buffer."""
         ...
     def deinit(self) -> None:
         """Disable permanently."""
         ...
 
@@ -457,28 +442,25 @@
           service or characteristic to be discovered. Creating the UUID causes the UUID to be
           registered for use. (This restriction may be lifted in the future.)
 
         :return: A tuple of `_bleio.Service` objects provided by the remote peripheral."""
         ...
     connected: bool
     """True if connected to the remote peer."""
-
     paired: bool
     """True if paired to the remote peer."""
-
     connection_interval: float
     """Time between transmissions in milliseconds. Will be multiple of 1.25ms. Lower numbers
     increase speed and decrease latency but increase power consumption.
 
     When setting connection_interval, the peer may reject the new interval and
     `connection_interval` will then remain the same.
 
     Apple has additional guidelines that dictate should be a multiple of 15ms except if HID is
     available. When HID is available Apple devices may accept 11.25ms intervals."""
-
     max_packet_length: int
     """The maximum number of data bytes that can be sent in a single transmission,
     not including overhead bytes.
 
     This is the maximum number of bytes that can be sent in a notification,
     which must be sent in a single packet.
     But for a regular characteristic read or write, may be sent in multiple packets,
@@ -523,18 +505,16 @@
         :param bool fixed_length: True if the descriptor value is of fixed length.
         :param ~circuitpython_typing.ReadableBuffer initial_value: The initial value for this descriptor.
 
         :return: the new Descriptor."""
         ...
     uuid: UUID
     """The descriptor uuid. (read-only)"""
-
     characteristic: Characteristic
     """The Characteristic this Descriptor is a part of."""
-
     value: bytearray
     """The value of this descriptor."""
 
 class PacketBuffer:
     """Accumulates a Characteristic's incoming packets in a FIFO buffer and facilitates packet aware
     outgoing writes. A packet's size is either the characteristic length or the maximum transmission
     unit (MTU) minus overhead, whichever is smaller. The MTU can change so check `incoming_packet_length`
@@ -581,15 +561,14 @@
         :rtype: int"""
         ...
     def deinit(self) -> None:
         """Disable permanently."""
         ...
     incoming_packet_length: int
     """Maximum length in bytes of a packet we are reading."""
-
     outgoing_packet_length: int
     """Maximum length in bytes of a packet we are writing."""
 
 class ScanEntry:
     """Encapsulates information about a device that was received during scanning. It can be
     advertisement or scan response data. This object may only be created by a `_bleio.ScanResults`:
     it has no user-visible constructor."""
@@ -600,24 +579,20 @@
     def matches(self, prefixes: ScanEntry, *, match_all: bool = True) -> bool:
         """Returns True if the ScanEntry matches all prefixes when ``match_all`` is True. This is stricter
         than the scan filtering which accepts any advertisements that match any of the prefixes
         where ``match_all`` is False."""
         ...
     address: Address
     """The address of the device (read-only), of type `_bleio.Address`."""
-
     advertisement_bytes: bytes
     """All the advertisement data present in the packet, returned as a ``bytes`` object. (read-only)"""
-
     rssi: int
     """The signal strength of the device at the time of the scan, in integer dBm. (read-only)"""
-
     connectable: bool
     """True if the device can be connected to. (read-only)"""
-
     scan_response: bool
     """True if the entry was a scan response. (read-only)"""
 
 class ScanResults:
     """Iterates over advertising data received while scanning. This object is always created
     by a `_bleio.Adapter`: it has no user-visible constructor."""
 
@@ -646,21 +621,18 @@
         :param bool secondary: If the service is a secondary one
 
         :return: the new Service"""
         ...
     characteristics: Tuple[Characteristic, ...]
     """A tuple of :py:class:`Characteristic` designating the characteristics that are offered by
     this service. (read-only)"""
-
     remote: bool
     """True if this is a service provided by a remote device. (read-only)"""
-
     secondary: bool
     """True if this is a secondary service. (read-only)"""
-
     uuid: Optional[UUID]
     """The UUID of this service. (read-only)
 
     Will be ``None`` if the 128-bit UUID for this service is not known."""
 
 class UUID:
     """A 16-bit or 128-bit UUID. Can be used for services, characteristics, descriptors and more."""
@@ -679,26 +651,23 @@
         :param value: The uuid value to encapsulate
         :type value: int, ~circuitpython_typing.ReadableBuffer or str"""
         ...
     uuid16: int
     """The 16-bit part of the UUID. (read-only)
 
     :type: int"""
-
     uuid128: bytes
     """The 128-bit value of the UUID
     Raises AttributeError if this is a 16-bit UUID. (read-only)
 
     :type: bytes"""
-
     size: int
     """128 if this UUID represents a 128-bit vendor-specific UUID. 16 if this UUID represents a
     16-bit Bluetooth SIG assigned UUID. (read-only) 32-bit UUIDs are not currently supported.
 
     :type: int"""
-
     def pack_into(self, buffer: WriteableBuffer, offset: int = 0) -> None:
         """Packs the UUID into the given buffer at the given offset."""
         ...
     def __eq__(self, other: object) -> bool:
         """Two UUID objects are equal if their values match and they are both 128-bit or both 16-bit."""
         ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/_eve/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/_eve/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from __future__ import annotations
 
 from typing import Tuple
 
 from circuitpython_typing import ReadableBuffer
 
 class _EVE:
+    def __init__(self) -> None:
+        """Create an _EVE object"""
     def register(self, o: object) -> None: ...
     def flush(self) -> None:
         """Send any queued drawing commands directly to the hardware.
 
         :param int width: The width of the grid in tiles, or 1 for sprites."""
         ...
     def cc(self, b: ReadableBuffer) -> None:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/_pew/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/_stage/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/adafruit_pixelbuf/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/adafruit_pixelbuf/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -41,27 +41,23 @@
         :param float brightness: Brightness (0 to 1.0, default 1.0)
         :param bool auto_write: Whether to automatically write pixels (Default False)
         :param ~circuitpython_typing.ReadableBuffer header: Sequence of bytes to always send before pixel values.
         :param ~circuitpython_typing.ReadableBuffer trailer: Sequence of bytes to always send after pixel values."""
         ...
     bpp: int
     """The number of bytes per pixel in the buffer (read-only)"""
-
     brightness: float
     """Float value between 0 and 1.  Output brightness.
 
     When brightness is less than 1.0, a second buffer will be used to store the color values
     before they are adjusted for brightness."""
-
     auto_write: bool
     """Whether to automatically write the pixels after each update."""
-
     byteorder: str
     """byteorder string for the buffer (read-only)"""
-
     def show(self) -> None:
         """Transmits the color data to the pixels so that they are shown. This is done automatically
         when `auto_write` is True."""
         ...
     def fill(
         self, color: Union[int, Tuple[int, int, int], Tuple[int, int, int, float]]
     ) -> None:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/aesio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/aesio/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """AES encryption routines
 
 The `AES` module contains classes used to implement encryption
-and decryption. It aims to be low overhead in terms of memory."""
+and decryption. It aims to be low overhead in terms of memory.
+
+For more information on AES, refer to `the Wikipedia entry
+<https://en.wikipedia.org/wiki/Advanced_Encryption_Standard>`_.
+"""
 
 from __future__ import annotations
 
 from typing import Optional
 
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
```

### Comparing `types-circuitpython-8.0.0b0/bindings/alarm/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/alarm/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 For more information about working with alarms and light/deep sleep in CircuitPython,
 see `this Learn guide <https://learn.adafruit.com/deep-sleep-with-circuitpython>`_.
 """
 
 from __future__ import annotations
 
-from typing import Optional, overload
+from typing import Optional, Sequence, overload
 
 import circuitpython_typing
+import digitalio
 from circuitpython_typing import ReadableBuffer
 
 sleep_memory: SleepMemory
 """Memory that persists during deep sleep.
 This object is the sole instance of `alarm.SleepMemory`."""
-
 wake_alarm: Optional[circuitpython_typing.Alarm]
 """The most recently triggered alarm. If CircuitPython was sleeping, the alarm that woke it from sleep.
 If no alarm occured since the last hard reset or soft restart, value is ``None``.
 """
 
 def light_sleep_until_alarms(
     *alarms: circuitpython_typing.Alarm,
@@ -51,52 +51,79 @@
     This allows the user to interrupt an existing program with ctrl-C,
     and to edit the files in CIRCUITPY, which would not be possible in true light sleep.
     Thus, to use light sleep and save significant power,
     it may be necessary to disconnect from the host.
     """
     ...
 
-def exit_and_deep_sleep_until_alarms(*alarms: circuitpython_typing.Alarm) -> None:
+def exit_and_deep_sleep_until_alarms(
+    *alarms: circuitpython_typing.Alarm,
+    preserve_dios: Sequence[digitalio.DigitalInOut] = (),
+) -> None:
     """Exit the program and go into a deep sleep, until awakened by one of the alarms.
     This function does not return.
 
     When awakened, the microcontroller will restart and will run ``boot.py`` and ``code.py``
     from the beginning.
 
     After restart, an alarm *equivalent* to the one that caused the wake-up
     will be available as `alarm.wake_alarm`.
     Its type and/or attributes may not correspond exactly to the original alarm.
     For time-base alarms, currently, an `alarm.time.TimeAlarm()` is created.
 
     If no alarms are specified, the microcontroller will deep sleep until reset.
 
+    :param circuitpython_typing.Alarm alarms: the alarms that can wake the microcontroller.
+    :param Sequence[digitalio.DigitalInOut] preserve_dios: A sequence of `DigitalInOut` objects
+      whose state should be preserved during deep sleep.
+      If a `DigitalInOut` in the sequence is set to be an output,
+      its current `DigitalInOut.value` (``True`` or ``False``)
+      will be preserved during the deep sleep.
+      If a `DigitalInOut` in the sequence is set to be an input,
+      its current `DigitalInOut.pull` value (``DOWN``, ``UP``, or ``None``)
+      will be preserved during deep sleep.
+
+    Preserving `DigitalInOut` states during deep sleep can be used to ensure that
+    external or on-board devices are powered or unpowered during sleep, among other purposes.
+
+    On some microcontrollers, some pins cannot remain in their original state for hardware reasons.
+
+    .. note::
+      On Espressif chips, preserving pin settings during deep sleep may consume extra current.
+      On ESP32, this was measured to be 250 uA or more.
+      Consider not preserving pins unless you need to.
+      Measure power consumption carefully both with no pins preserved and with the pins you might want to
+      preserve to achieve the lowest consumption.
+
     **If CircuitPython is connected to a host computer via USB or BLE
     the first time a deep sleep is requested,
     the connection will be maintained and the system will not go into deep sleep.**
     This allows the user to interrupt an existing program with ctrl-C,
     and to edit the files in CIRCUITPY, which would not be possible in true deep sleep.
 
     If CircuitPython goes into a true deep sleep, and USB or BLE is reconnected,
     the next deep sleep will still be a true deep sleep. You must do a hard reset
     or power-cycle to exit a true deep sleep loop.
 
-    Here is skeletal example that deep-sleeps and restarts every 60 seconds:
+    Here is a skeletal example:
 
     .. code-block:: python
 
         import alarm
         import time
+        import board
 
         print("Waking up")
 
-        # Set an alarm for 60 seconds from now.
+        # Create an alarm for 60 seconds from now, and also a pin alarm.
         time_alarm = alarm.time.TimeAlarm(monotonic_time=time.monotonic() + 60)
+        pin_alarm = alarm.pin.PinAlarm(board.D7, False)
 
-        # Deep sleep until the alarm goes off. Then restart the program.
-        alarm.exit_and_deep_sleep_until_alarms(time_alarm)
+        # Deep sleep until one of the alarm goes off. Then restart the program.
+        alarm.exit_and_deep_sleep_until_alarms(time_alarm, pin_alarm)
     """
     ...
 
 class SleepMemory:
     """Store raw bytes in RAM that persists during deep sleep.
     The class acts as a ``bytearray``.
     If power is lost, the memory contents are lost.
```

### Comparing `types-circuitpython-8.0.0b0/bindings/analogio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/analogio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     value: int
     """The value on the analog pin between 0 and 65535 inclusive (16-bit). (read-only)
 
     Even if the underlying analog to digital converter (ADC) is lower
     resolution, the value is 16-bit."""
-
     reference_voltage: float
     """The maximum voltage measurable (also known as the reference voltage) as a
     `float` in Volts.  Note the ADC value may not scale to the actual voltage linearly
     at ends of the analog range."""
 
 class AnalogOut:
     """Output analog values (a specific voltage).
```

### Comparing `types-circuitpython-8.0.0b0/bindings/atexit/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/audiobusio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/audiobusio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,14 @@
         The sample itself should consist of 8 bit or 16 bit samples."""
         ...
     def stop(self) -> None:
         """Stops playback."""
         ...
     playing: bool
     """True when the audio sample is being output. (read-only)"""
-
     def pause(self) -> None:
         """Stops playback temporarily while remembering the position. Use `resume` to resume playback."""
         ...
     def resume(self) -> None:
         """Resumes sample playback after :py:func:`pause`."""
         ...
     paused: bool
@@ -136,39 +135,38 @@
           Minimum sample_rate is about 16000 Hz.
         :param int bit_depth: Final number of bits per sample. Must be divisible by 8
         :param bool mono: True when capturing a single channel of audio, captures two channels otherwise
         :param int oversample: Number of single bit samples to decimate into a final sample. Must be divisible by 8
         :param float startup_delay: seconds to wait after starting microphone clock
          to allow microphone to turn on. Most require only 0.01s; some require 0.1s. Longer is safer.
          Must be in range 0.0-1.0 seconds."""
+    """Record 8-bit unsigned samples to buffer::
 
-        """Record 8-bit unsigned samples to buffer::
-
-          import audiobusio
-          import board
+      import audiobusio
+      import board
 
-          # Prep a buffer to record into
-          b = bytearray(200)
-          with audiobusio.PDMIn(board.MICROPHONE_CLOCK, board.MICROPHONE_DATA, sample_rate=16000) as mic:
-              mic.record(b, len(b))
-
-        Record 16-bit unsigned samples to buffer::
-
-          import audiobusio
-          import board
-
-          # Prep a buffer to record into. The array interface doesn't allow for
-          # constructing with a set size so we append to it until we have the size
-          # we want.
-          b = array.array("H")
-          for i in range(200):
-              b.append(0)
-          with audiobusio.PDMIn(board.MICROPHONE_CLOCK, board.MICROPHONE_DATA, sample_rate=16000, bit_depth=16) as mic:
-              mic.record(b, len(b))"""
-        ...
+      # Prep a buffer to record into
+      b = bytearray(200)
+      with audiobusio.PDMIn(board.MICROPHONE_CLOCK, board.MICROPHONE_DATA, sample_rate=16000) as mic:
+          mic.record(b, len(b))
+
+    Record 16-bit unsigned samples to buffer::
+
+      import audiobusio
+      import board
+
+      # Prep a buffer to record into. The array interface doesn't allow for
+      # constructing with a set size so we append to it until we have the size
+      # we want.
+      b = array.array("H")
+      for i in range(200):
+          b.append(0)
+      with audiobusio.PDMIn(board.MICROPHONE_CLOCK, board.MICROPHONE_DATA, sample_rate=16000, bit_depth=16) as mic:
+          mic.record(b, len(b))"""
+    ...
     def deinit(self) -> None:
         """Deinitialises the PDMIn and releases any hardware resources for reuse."""
         ...
     def __enter__(self) -> PDMIn:
         """No-op used by Context Managers."""
         ...
     def __exit__(self) -> None:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/audiocore/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/audiocore/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Support for audio samples"""
 
 from __future__ import annotations
 
 import typing
-from typing import Optional
+from typing import Optional, Union
 
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
 
 class RawSample:
     """A raw audio sample buffer in memory"""
 
     def __init__(
@@ -62,44 +62,45 @@
 class WaveFile:
     """Load a wave file for audio playback
 
     A .wav file prepped for audio playback. Only mono and stereo files are supported. Samples must
     be 8 bit unsigned or 16 bit signed. If a buffer is provided, it will be used instead of allocating
     an internal buffer, which can prevent memory fragmentation."""
 
-    def __init__(self, file: typing.BinaryIO, buffer: WriteableBuffer) -> None:
+    def __init__(
+        self, file: Union[str, typing.BinaryIO], buffer: WriteableBuffer
+    ) -> None:
         """Load a .wav file for playback with `audioio.AudioOut` or `audiobusio.I2SOut`.
 
-        :param typing.BinaryIO file: Already opened wave file
+        :param Union[str, typing.BinaryIO] file: The name of a wave file (preferred) or an already opened wave file
         :param ~circuitpython_typing.WriteableBuffer buffer: Optional pre-allocated buffer,
           that will be split in half and used for double-buffering of the data.
           The buffer must be 8 to 1024 bytes long.
           If not provided, two 256 byte buffers are initially allocated internally.
 
-
         Playing a wave file from flash::
 
           import board
           import audiocore
           import audioio
           import digitalio
 
           # Required for CircuitPlayground Express
           speaker_enable = digitalio.DigitalInOut(board.SPEAKER_ENABLE)
           speaker_enable.switch_to_output(value=True)
 
-          data = open("cplay-5.1-16bit-16khz.wav", "rb")
-          wav = audiocore.WaveFile(data)
+          wav = audiocore.WaveFile("cplay-5.1-16bit-16khz.wav")
           a = audioio.AudioOut(board.A0)
 
           print("playing")
           a.play(wav)
           while a.playing:
             pass
-          print("stopped")"""
+          print("stopped")
+        """
         ...
     def deinit(self) -> None:
         """Deinitialises the WaveFile and releases all memory resources for reuse."""
         ...
     def __enter__(self) -> WaveFile:
         """No-op used by Context Managers."""
         ...
@@ -107,13 +108,11 @@
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     sample_rate: int
     """32 bit value that dictates how quickly samples are loaded into the DAC
     in Hertz (cycles per second). When the sample is looped, this can change
     the pitch output without changing the underlying sample."""
-
     bits_per_sample: int
     """Bits per sample. (read only)"""
-
     channel_count: int
     """Number of audio channels. (read only)"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/audioio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/audioio/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 The `audioio` module contains classes to provide access to audio IO.
 
 All classes change hardware state and should be deinitialized when they
 are no longer needed if the program continues after use. To do so, either
 call :py:meth:`!deinit` or use a context manager. See
 :ref:`lifetime-and-contextmanagers` for more info.
 
+For more information on working with this module, refer to the
+`CircuitPython Essentials Learn Guide
+<https://learn.adafruit.com/circuitpython-essentials/circuitpython-audio-out>`_.
+
 Since CircuitPython 5, `RawSample` and `WaveFile` are moved
 to :mod:`audiocore`, and `Mixer` is moved to :mod:`audiomixer`.
 
 For compatibility with CircuitPython 4.x, some builds allow the items in
 `audiocore` to be imported from `audioio`.  This will be removed for all
 boards in a future build of CircuitPython."""
 
@@ -103,15 +107,14 @@
         DAC that ignores the lowest 6 bits when playing 16 bit samples."""
         ...
     def stop(self) -> None:
         """Stops playback and resets to the start of the sample."""
         ...
     playing: bool
     """True when an audio sample is being output even if `paused`. (read-only)"""
-
     def pause(self) -> None:
         """Stops playback temporarily while remembering the position. Use `resume` to resume playback."""
         ...
     def resume(self) -> None:
         """Resumes sample playback after :py:func:`pause`."""
         ...
     paused: bool
```

### Comparing `types-circuitpython-8.0.0b0/bindings/audiomixer/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/audiomixer/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -61,18 +61,16 @@
         ...
     def __exit__(self) -> None:
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     playing: bool
     """True when any voice is being output. (read-only)"""
-
     sample_rate: int
     """32 bit value that dictates how quickly samples are played in Hertz (cycles per second)."""
-
     voice: Tuple[MixerVoice, ...]
     """A tuple of the mixer's `audiomixer.MixerVoice` object(s).
 
     .. code-block:: python
 
        >>> mixer.voice
        (<MixerVoice>,)"""
@@ -113,10 +111,9 @@
         The sample must match the `audiomixer.Mixer`'s encoding settings given in the constructor."""
         ...
     def stop(self) -> None:
         """Stops playback of the sample on this voice."""
         ...
     level: float
     """The volume level of a voice, as a floating point number between 0 and 1."""
-
     playing: bool
     """True when this voice is being output. (read-only)"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/audiomp3/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/audiomp3/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,35 @@
 see `this CircuitPython Essentials Learn guide page
 <https://learn.adafruit.com/circuitpython-essentials/circuitpython-mp3-audio>`_.
 """
 
 from __future__ import annotations
 
 import typing
+from typing import Union
 
 from circuitpython_typing import WriteableBuffer
 
 class MP3Decoder:
     """Load a mp3 file for audio playback
 
     .. note::
 
         ``MP3Decoder`` uses a lot of contiguous memory, so care should be given to
         optimizing memory usage.  More information and recommendations can be found here:
         https://learn.adafruit.com/Memory-saving-tips-for-CircuitPython/reducing-memory-fragmentation
     """
 
-    def __init__(self, file: typing.BinaryIO, buffer: WriteableBuffer) -> None:
+    def __init__(
+        self, file: Union[str, typing.BinaryIO], buffer: WriteableBuffer
+    ) -> None:
 
         """Load a .mp3 file for playback with `audioio.AudioOut` or `audiobusio.I2SOut`.
 
-        :param typing.BinaryIO file: Already opened mp3 file
+        :param Union[str, typing.BinaryIO] file: The name of a mp3 file (preferred) or an already opened mp3 file
         :param ~circuitpython_typing.WriteableBuffer buffer: Optional pre-allocated buffer, that will be split in half and used for double-buffering of the data. If not provided, two buffers are allocated internally.  The specific buffer size required depends on the mp3 file.
 
         Playback of mp3 audio is CPU intensive, and the
         exact limit depends on many factors such as the particular
         microcontroller, SD card or flash performance, and other
         code in use such as displayio. If playback is garbled,
         skips, or plays as static, first try using a "simpler" mp3:
@@ -50,46 +53,44 @@
           import audioio
           import digitalio
 
           # Required for CircuitPlayground Express
           speaker_enable = digitalio.DigitalInOut(board.SPEAKER_ENABLE)
           speaker_enable.switch_to_output(value=True)
 
-          data = open("cplay-16bit-16khz-64kbps.mp3", "rb")
-          mp3 = audiomp3.MP3Decoder(data)
+          mp3 = audiomp3.MP3Decoder("cplay-16bit-16khz-64kbps.mp3")
           a = audioio.AudioOut(board.A0)
 
           print("playing")
           a.play(mp3)
           while a.playing:
             pass
-          print("stopped")"""
+          print("stopped")
+        """
         ...
     def deinit(self) -> None:
         """Deinitialises the MP3 and releases all memory resources for reuse."""
         ...
     def __enter__(self) -> MP3Decoder:
         """No-op used by Context Managers."""
         ...
     def __exit__(self) -> None:
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     file: typing.BinaryIO
     """File to play back."""
-
+    def open(self, filepath: str) -> None:
+        """Takes in the name of a mp3 file, opens it, and replaces the old playback file."""
+        ...
     sample_rate: int
     """32 bit value that dictates how quickly samples are loaded into the DAC
     in Hertz (cycles per second). When the sample is looped, this can change
     the pitch output without changing the underlying sample."""
-
     bits_per_sample: int
     """Bits per sample. (read only)"""
-
     channel_count: int
     """Number of audio channels. (read only)"""
-
     rms_level: float
     """The RMS audio level of a recently played moment of audio. (read only)"""
-
     samples_decoded: int
     """The number of audio samples decoded from the current file. (read only)"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/audiopwmio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/audiopwmio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         resolution will use the highest order bits to output."""
         ...
     def stop(self) -> None:
         """Stops playback and resets to the start of the sample."""
         ...
     playing: bool
     """True when an audio sample is being output even if `paused`. (read-only)"""
-
     def pause(self) -> None:
         """Stops playback temporarily while remembering the position. Use `resume` to resume playback."""
         ...
     def resume(self) -> None:
         """Resumes sample playback after :py:func:`pause`."""
         ...
     paused: bool
```

### Comparing `types-circuitpython-8.0.0b0/bindings/bitbangio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/bitbangio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         If ``out_start`` or ``out_end`` is provided, then the buffer will be sliced
         as if ``out_buffer[out_start:out_end]`` were passed, but without copying the data.
         The number of bytes written will be the length of ``out_buffer[start:end]``.
 
         If ``in_start`` or ``in_end`` is provided, then the input buffer will be sliced
         as if ``in_buffer[in_start:in_end]`` were passed,
         The number of bytes read will be the length of ``out_buffer[in_start:in_end]``.
+
         :param int address: 7-bit device address
         :param ~circuitpython_typing.ReadableBuffer out_buffer: buffer containing the bytes to write
         :param ~circuitpython_typing.WriteableBuffer in_buffer: buffer to write into
         :param int out_start: beginning of ``out_buffer`` slice
         :param int out_end: end of ``out_buffer`` slice; if not specified, use ``len(out_buffer)``
         :param int in_start: beginning of ``in_buffer`` slice
         :param int in_end: end of ``in_buffer slice``; if not specified, use ``len(in_buffer)``
```

### Comparing `types-circuitpython-8.0.0b0/bindings/bitmaptools/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/bitmaptools/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 def alphablend(
     dest_bitmap: displayio.Bitmap,
     source_bitmap_1: displayio.Bitmap,
     source_bitmap_2: displayio.Bitmap,
     colorspace: displayio.Colorspace,
     factor1: float = 0.5,
-    factor2: float = None,
+    factor2: Optional[float] = None,
 ) -> None:
     """Alpha blend the two source bitmaps into the destination.
 
     It is permitted for the destination bitmap to be one of the two
     source bitmaps.
 
     :param bitmap dest_bitmap: Destination bitmap that will be written into
```

### Comparing `types-circuitpython-8.0.0b0/bindings/bitops/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/board/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/busio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/busio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         If ``out_start`` or ``out_end`` is provided, then the buffer will be sliced
         as if ``out_buffer[out_start:out_end]`` were passed, but without copying the data.
         The number of bytes written will be the length of ``out_buffer[start:end]``.
 
         If ``in_start`` or ``in_end`` is provided, then the input buffer will be sliced
         as if ``in_buffer[in_start:in_end]`` were passed,
         The number of bytes read will be the length of ``out_buffer[in_start:in_end]``.
+
         :param int address: 7-bit device address
         :param ~circuitpython_typing.ReadableBuffer out_buffer: buffer containing the bytes to write
         :param ~circuitpython_typing.WriteableBuffer in_buffer: buffer to write into
         :param int out_start: beginning of ``out_buffer`` slice
         :param int out_end: end of ``out_buffer`` slice; if not specified, use ``len(out_buffer)``
         :param int in_start: beginning of ``in_buffer`` slice
         :param int in_end: end of ``in_buffer slice``; if not specified, use ``len(in_buffer)``
@@ -399,55 +400,57 @@
         """No-op used by Context Managers."""
         ...
     def __exit__(self) -> None:
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     def read(self, nbytes: Optional[int] = None) -> Optional[bytes]:
-        """Read characters.  If ``nbytes`` is specified then read at most that many
+        """Read bytes.  If ``nbytes`` is specified then read at most that many
         bytes. Otherwise, read everything that arrives until the connection
         times out. Providing the number of bytes expected is highly recommended
-        because it will be faster.
+        because it will be faster. If no bytes are read, return ``None``.
+
+        .. note:: When no bytes are read due to a timeout, this function returns ``None``.
+          This matches the behavior of `io.RawIOBase.read` in Python 3, but
+          differs from pyserial which returns ``b''`` in that situation.
 
         :return: Data read
         :rtype: bytes or None"""
         ...
     def readinto(self, buf: WriteableBuffer) -> Optional[int]:
         """Read bytes into the ``buf``. Read at most ``len(buf)`` bytes.
 
         :return: number of bytes read and stored into ``buf``
         :rtype: int or None (on a non-blocking error)
 
         *New in CircuitPython 4.0:* No length parameter is permitted."""
         ...
     def readline(self) -> bytes:
         """Read a line, ending in a newline character, or
-           return None if a timeout occurs sooner, or
-           return everything readable if no newline is found and timeout=0
+        return ``None`` if a timeout occurs sooner, or
+        return everything readable if no newline is found and
+        ``timeout=0``
 
         :return: the line read
         :rtype: bytes or None"""
         ...
-    def write(self, buf: WriteableBuffer) -> Optional[int]:
+    def write(self, buf: ReadableBuffer) -> Optional[int]:
         """Write the buffer of bytes to the bus.
 
         *New in CircuitPython 4.0:* ``buf`` must be bytes, not a string.
 
           :return: the number of bytes written
           :rtype: int or None"""
         ...
     baudrate: int
     """The current baudrate."""
-
     in_waiting: int
     """The number of bytes in the input buffer, available to be read"""
-
     timeout: float
     """The current timeout, in seconds (float)."""
-
     def reset_input_buffer(self) -> None:
         """Discard any unread characters in the input buffer."""
         ...
 
 class Parity:
     """Enum-like class to define the parity used to verify correct data transfer."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/camera/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/canio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/canio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 A CAN bus involves a transceiver, which is often a separate chip with a "standby" pin.
 If your board has a CAN_STANDBY pin, ensure to set it to an output with the value False
 to enable the transceiver.
 
 Other implementations of the CAN device may exist (for instance, attached
 via an SPI bus).  If so their constructor arguments may differ, but
 otherwise we encourage implementors to follow the API that the core uses.
+
+For more information on working with this module, refer to
+`this Learn Guide on using it <https://learn.adafruit.com/using-canio-circuitpython>`_.
 """
 
 from __future__ import annotations
 
 from types import TracebackType
 from typing import Optional, Sequence, Type, Union
 
@@ -84,24 +87,20 @@
         :param bool loopback: When True  the ``rx`` pin's value is ignored, and the device receives the packets it sends.
         :param bool silent: When True the ``tx`` pin is always driven to the high logic level.  This mode can be used to "sniff" a CAN bus without interfering.
         :param bool auto_restart: If True, will restart communications after entering bus-off state
         """
         ...
     auto_restart: bool
     """If True, will restart communications after entering bus-off state"""
-
     baudrate: int
     """The baud rate (read-only)"""
-
     transmit_error_count: int
     """The number of transmit errors (read-only).  Increased for a detected transmission error, decreased for successful transmission.  Limited to the range from 0 to 255 inclusive.  Also called TEC."""
-
     receive_error_count: int
     """The number of receive errors (read-only).  Increased for a detected reception error, decreased for successful reception.  Limited to the range from 0 to 255 inclusive.  Also called REC."""
-
     state: BusState
     """The current state of the bus. (read-only)"""
     def restart(self) -> None:
         """If the device is in the bus off state, restart it."""
         ...
     def listen(
         self, matches: Optional[Sequence[Match]] = None, *, timeout: float = 10
@@ -136,24 +135,22 @@
         ESP32S2 supports one Listener.  There is a single filter block, which can either match a
         standard address with mask or an extended address with mask.
         """
         ...
     loopback: bool
     """True if the device was created in loopback mode, False
     otherwise (read-only)"""
-
     def send(self, message: Union[RemoteTransmissionRequest, Message]) -> None:
         """Send a message on the bus with the given data and id.
         If the message could not be sent due to a full fifo or a bus error condition, RuntimeError is raised.
         """
         ...
     silent: bool
     """True if the device was created in silent mode, False
     otherwise (read-only)"""
-
     def deinit(self) -> None:
         """Deinitialize this object, freeing its hardware resources"""
         ...
     def __enter__(self) -> CAN:
         """Returns self, to allow the object to be used in a `with` statement for resource control"""
         ...
     def __exit__(
@@ -227,18 +224,16 @@
 
         If mask is not None, then the filter is for any id which matches all
         the nonzero bits in mask. Otherwise, it matches exactly the given id.
         If extended is true then only extended ids are matched, otherwise
         only standard ids are matched."""
     id: int
     """The id to match"""
-
     mask: int
     """The optional mask of ids to match"""
-
     extended: bool
     """True to match extended ids, False to match standard ides"""
 
 class Message:
     def __init__(self, id: int, data: bytes, *, extended: bool = False) -> None:
         """Construct a Message to send on a CAN bus.
 
@@ -247,18 +242,16 @@
         :param bool extended: True if the message has an extended identifier, False if it has a standard identifier
 
         In CAN, messages can have a length from 0 to 8 bytes.
         """
         ...
     id: int
     """The numeric ID of the message"""
-
     data: bytes
     """The content of the message"""
-
     extended: bool
     """True if the message's id is an extended id"""
 
 class RemoteTransmissionRequest:
     def __init__(self, id: int, length: int, *, extended: bool = False) -> None:
         """Construct a RemoteTransmissionRequest to send on a CAN bus.
 
@@ -267,13 +260,11 @@
         :param bool extended: True if the message has an extended identifier, False if it has a standard identifier
 
         In CAN, messages can have a length from 0 to 8 bytes.
         """
         ...
     id: int
     """The numeric ID of the message"""
-
     extended: bool
     """True if the message's id is an extended id"""
-
     length: int
     """The length of the requested message."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/countio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/countio/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """Support for edge counting
 
 The `countio` module contains logic to read and count edge transistions
 
+For more information on the applications of counting edges, see
+`this Learn Guide on sequential circuits
+<https://learn.adafruit.com/digital-circuits-4-sequential-circuits>`_.
+
 All classes change hardware state and should be deinitialized when they
 are no longer needed if the program continues after use. To do so, either
 call :py:meth:`!deinit` or use a context manager. See
 :ref:`lifetime-and-contextmanagers` for more info."""
 
 from __future__ import annotations
 
@@ -67,10 +71,9 @@
     def __enter__(self) -> Counter:
         """No-op used by Context Managers."""
     def __exit__(self) -> None:
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
     count: int
     """The current count in terms of pulses."""
-
     def reset(self) -> None:
         """Resets the count back to 0."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/digitalio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/digitalio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -113,24 +113,21 @@
     direction: Direction
     """The direction of the pin.
 
     Setting this will use the defaults from the corresponding
     :py:meth:`switch_to_input` or :py:meth:`switch_to_output` method. If
     you want to set pull, value or drive mode prior to switching, then use
     those methods instead."""
-
     value: bool
     """The digital logic level of the pin."""
-
     drive_mode: DriveMode
     """The pin drive mode. One of:
 
     - `digitalio.DriveMode.PUSH_PULL`
     - `digitalio.DriveMode.OPEN_DRAIN`"""
-
     pull: Optional[Pull]
     """The pin pull direction. One of:
 
     - `digitalio.Pull.UP`
     - `digitalio.Pull.DOWN`
     - `None`
```

### Comparing `types-circuitpython-8.0.0b0/bindings/displayio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/displayio/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,16 @@
 
         :param int width: The number of values wide
         :param int height: The number of values high
         :param int value_count: The number of possible pixel values."""
         ...
     width: int
     """Width of the bitmap. (read only)"""
-
     height: int
     """Height of the bitmap. (read only)"""
-
     def __getitem__(self, index: Union[Tuple[int, int], int]) -> int:
         """Returns the value at the given index. The index can either be an x,y tuple or an int equal
         to ``y * width + x``.
 
         This allows you to::
 
           print(bitmap[0,1])"""
@@ -155,15 +153,14 @@
         ...
     def convert(self, color: int) -> int:
         """Converts the given color to RGB565 according to the Colorspace"""
         ...
     dither: bool
     """When `True` the ColorConverter dithers the output by adding random noise when
     truncating to display bitdepth"""
-
     def make_transparent(self, color: int) -> None:
         """Set the transparent color or index for the ColorConverter. This will
         raise an Exception if there is already a selected transparent index.
 
         :param int color: The color to be transparent"""
     def make_opaque(self, color: int) -> None:
         """Make the ColorConverter be opaque and have no transparent pixels.
@@ -298,33 +295,26 @@
 
         :param Optional[int] target_frames_per_second: The target frame rate that :py:func:`refresh` should try to
             achieve. Set to `None` for immediate refresh.
         :param int minimum_frames_per_second: The minimum number of times the screen should be updated per second."""
         ...
     auto_refresh: bool
     """True when the display is refreshed automatically."""
-
     brightness: float
     """The brightness of the display as a float. 0.0 is off and 1.0 is full brightness."""
-
     width: int
     """Gets the width of the board"""
-
     height: int
     """Gets the height of the board"""
-
     rotation: int
     """The rotation of the display as an int in degrees."""
-
     bus: _DisplayBus
     """The bus being used by the display"""
-
     root_group: Group
     """The root group on the display."""
-
     def fill_row(self, y: int, buffer: WriteableBuffer) -> WriteableBuffer:
         """Extract the pixels from a single row
 
         :param int y: The top edge of the area
         :param ~circuitpython_typing.WriteableBuffer buffer: The buffer in which to place the pixel data"""
         ...
 
@@ -421,28 +411,23 @@
         varying the refresh mode of the display."""
     def refresh(self) -> None:
         """Refreshes the display immediately or raises an exception if too soon. Use
         ``time.sleep(display.time_to_refresh)`` to sleep until a refresh can occur."""
         ...
     time_to_refresh: float
     """Time, in fractional seconds, until the ePaper display can be refreshed."""
-
     busy: bool
     """True when the display is refreshing. This uses the ``busy_pin`` when available or the
        ``refresh_time`` otherwise."""
-
     width: int
     """Gets the width of the display in pixels"""
-
     height: int
     """Gets the height of the display in pixels"""
-
     rotation: int
     """The rotation of the display as an int in degrees."""
-
     bus: _DisplayBus
     """The bus being used by the display"""
 
 class FourWire:
     """Manage updating a display over SPI four wire protocol in the background while Python code runs.
     It doesn't handle display initialization."""
 
@@ -499,25 +484,21 @@
         :param int scale: Scale of layer pixels in one dimension.
         :param int x: Initial x position within the parent.
         :param int y: Initial y position within the parent."""
         ...
     hidden: bool
     """True when the Group and all of it's layers are not visible. When False, the Group's layers
     are visible if they haven't been hidden."""
-
     scale: int
     """Scales each pixel within the Group in both directions. For example, when scale=2 each pixel
     will be represented by 2x2 pixels."""
-
     x: int
     """X position of the Group in the parent."""
-
     y: int
     """Y position of the Group in the parent."""
-
     def append(
         self,
         layer: Union[
             vectorio.Circle, vectorio.Rectangle, vectorio.Polygon, Group, TileGrid
         ],
     ) -> None:
         """Append a layer to the group. It will be drawn above other layers."""
@@ -663,18 +644,16 @@
         mode. CircuitPython 7.0 modified OnDiskBitmap so that it takes a
         filename instead, and opens the file internally.  A future version
         of CircuitPython will remove the ability to pass in an opened file.
         """
         ...
     width: int
     """Width of the bitmap. (read only)"""
-
     height: int
     """Height of the bitmap. (read only)"""
-
     pixel_shader: Union[ColorConverter, Palette]
     """The image's pixel_shader.  The type depends on the underlying
     bitmap's structure.  The pixel shader can be modified (e.g., to set the
     transparent pixel or, for palette shaded images, to update the palette.)"""
 
 class Palette:
     """Map a pixel palette_index to a full color. Colors are transformed to the display's format internally to
@@ -769,52 +748,40 @@
         :param int tile_width: Width of a single tile in pixels. Defaults to the full Bitmap and must evenly divide into the Bitmap's dimensions.
         :param int tile_height: Height of a single tile in pixels. Defaults to the full Bitmap and must evenly divide into the Bitmap's dimensions.
         :param int default_tile: Default tile index to show.
         :param int x: Initial x position of the left edge within the parent.
         :param int y: Initial y position of the top edge within the parent."""
     hidden: bool
     """True when the TileGrid is hidden. This may be False even when a part of a hidden Group."""
-
     x: int
     """X position of the left edge in the parent."""
-
     y: int
     """Y position of the top edge in the parent."""
-
     width: int
     """Width of the tilegrid in tiles."""
-
     height: int
     """Height of the tilegrid in tiles."""
-
     tile_width: int
     """Width of a single tile in pixels."""
-
     tile_height: int
     """Height of a single tile in pixels."""
-
     flip_x: bool
     """If true, the left edge rendered will be the right edge of the right-most tile."""
-
     flip_y: bool
     """If true, the top edge rendered will be the bottom edge of the bottom-most tile."""
-
     transpose_xy: bool
     """If true, the TileGrid's axis will be swapped. When combined with mirroring, any 90 degree
     rotation can be achieved along with the corresponding mirrored version."""
-
     def contains(self, touch_tuple: tuple) -> bool:
         """Returns True if the first two values in ``touch_tuple`` represent an x,y coordinate
         inside the tilegrid rectangle bounds."""
     pixel_shader: Union[ColorConverter, Palette]
     """The pixel shader of the tilegrid."""
-
     bitmap: Union[Bitmap, OnDiskBitmap, Shape]
     """The bitmap of the tilegrid."""
-
     def __getitem__(self, index: Union[Tuple[int, int], int]) -> int:
         """Returns the tile index at the given index. The index can either be an x,y tuple or an int equal
         to ``y * width + x``.
 
         This allows you to::
 
           print(grid[0])"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/dotenv/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/dotenv/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/dualbank/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/dualbank/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from __future__ import annotations
 
 from circuitpython_typing import ReadableBuffer
 
 ...
 
-def flash(*buffer: ReadableBuffer, offset: int = 0) -> None:
+def flash(buffer: ReadableBuffer, offset: int = 0) -> None:
     """Writes one of two app partitions at the given offset.
 
     This can be called multiple times when flashing the firmware
     in small chunks.
     """
     ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/floppyio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/fontio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/fontio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         `Adafruit_CircuitPython_Bitmap_Font <https://github.com/adafruit/Adafruit_CircuitPython_Bitmap_Font>`_
         library for dynamically loaded fonts."""
         ...
     bitmap: displayio.Bitmap
     """Bitmap containing all font glyphs starting with ASCII and followed by unicode. Use
     `get_glyph` in most cases. This is useful for use with `displayio.TileGrid` and
     `terminalio.Terminal`."""
-
     def get_bounding_box(self) -> Tuple[int, int]:
         """Returns the maximum bounds of all glyphs in the font in a tuple of two values: width, height."""
         ...
     def get_glyph(self, codepoint: int) -> Glyph:
         """Returns a `fontio.Glyph` for the given codepoint or None if no glyph is available."""
         ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/framebufferio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/framebufferio/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,30 +53,24 @@
         without calls to this.)
 
         :param int target_frames_per_second: How many times a second `refresh` should be called and the screen updated.
         :param int minimum_frames_per_second: The minimum number of times the screen should be updated per second."""
         ...
     auto_refresh: bool
     """True when the display is refreshed automatically."""
-
     brightness: float
     """The brightness of the display as a float. 0.0 is off and 1.0 is full brightness."""
-
     width: int
     """Gets the width of the framebuffer"""
-
     height: int
     """Gets the height of the framebuffer"""
-
     rotation: int
     """The rotation of the display as an int in degrees."""
-
     framebuffer: circuitpython_typing.FrameBuffer
     """The framebuffer being used by the display"""
-
     def fill_row(self, y: int, buffer: WriteableBuffer) -> WriteableBuffer:
         """Extract the pixels from a single row
 
         :param int y: The top edge of the area
         :param ~circuitpython_typing.WriteableBuffer buffer: The buffer in which to place the pixel data"""
         ...
     root_group: displayio.Group
```

### Comparing `types-circuitpython-8.0.0b0/bindings/frequencyio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/frequencyio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -85,11 +85,10 @@
     capture_period: int
     """The capture measurement period. Lower incoming frequencies will be measured
     more accurately with longer capture periods. Higher frequencies are more
     accurate with shorter capture periods.
 
     .. note:: When setting a new ``capture_period``, all previous capture information is
               cleared with a call to ``clear()``."""
-
     def __get__(self, index: int) -> int:
         """Returns the value of the last frequency captured."""
         ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/getpass/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/gifio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/gifio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/gnss/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/gnss/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,24 +37,20 @@
         """Turn off the GNSS."""
         ...
     def update(self) -> None:
         """Update GNSS positioning information."""
         ...
     latitude: float
     """Latitude of current position in degrees (float)."""
-
     longitude: float
     """Longitude of current position in degrees (float)."""
-
     altitude: float
     """Altitude of current position in meters (float)."""
-
     timestamp: time.struct_time
     """Time when the position data was updated."""
-
     fix: PositionFix
     """Fix mode."""
 
 class PositionFix:
     """Position fix mode"""
 
     def __init__(self) -> None:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/hashlib/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/hashlib/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 
 from __future__ import annotations
 
 import hashlib
 
 from circuitpython_typing import ReadableBuffer
 
-def new(name, data=b"") -> hashlib.Hash:
+def new(name: str, data: bytes = b"") -> hashlib.Hash:
     """Returns a Hash object setup for the named algorithm. Raises ValueError when the named
        algorithm is unsupported.
 
     :return: a hash object for the given algorithm
     :rtype: hashlib.Hash"""
     ...
 
 class Hash:
     """In progress hash algorithm. This object is always created by a `hashlib.new()`. It has no
     user-visible constructor."""
 
     digest_size: int
     """Digest size in bytes"""
-
     def update(self, data: ReadableBuffer) -> None:
         """Update the hash with the given bytes.
 
         :param ~circuitpython_typing.ReadableBuffer data: Update the hash from data in this buffer"""
         ...
     def digest(self) -> bytes:
         """Returns the current digest as bytes() with a length of `hashlib.Hash.digest_size`."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/i2ctarget/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/i2ctarget/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -114,21 +114,18 @@
         """No-op used in Context Managers."""
         ...
     def __exit__(self) -> None:
         """Close the request."""
         ...
     address: int
     """The I2C address of the request."""
-
     is_read: bool
     """The I2C main controller is reading from this target."""
-
     is_restart: bool
     """Is Repeated Start Condition."""
-
     def read(self, n: int = -1, ack: bool = True) -> bytearray:
         """Read data.
         If ack=False, the caller is responsible for calling :py:meth:`I2CTargetRequest.ack`.
 
         :param n: Number of bytes to read (negative means all)
         :param ack: Whether or not to send an ACK after the n'th byte
         :return: Bytes read"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/imagecapture/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/ipaddress/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/ipaddress/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     def __init__(self, address: Union[int, str, bytes]) -> None:
         """Create a new IPv4Address object encapsulating the address value.
 
         The value itself can either be bytes or a string formatted address."""
         ...
     packed: bytes
     """The bytes that make up the address (read-only)."""
-
     version: int
     """4 for IPv4, 6 for IPv6"""
-
     def __eq__(self, other: object) -> bool:
         """Two Address objects are equal if their addresses and address types are equal."""
         ...
     def __hash__(self) -> int:
         """Returns a hash for the IPv4Address data."""
         ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/is31fl3741/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/is31fl3741/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -44,22 +44,20 @@
         """Free the resources associated with this
         IS31FL3741 instance.  After deinitialization, no further operations
         may be performed."""
         ...
     brightness: float
     """In the current implementation, 0.0 turns the display off entirely
     and any other value up to 1.0 turns the display on fully."""
-
     def refresh(self) -> None:
         """Transmits the color data in the buffer to the pixels so that
         they are shown."""
         ...
     width: int
     """The width of the display, in pixels"""
-
     height: int
     """The height of the display, in pixels"""
 
 class IS31FL3741:
     """Driver for an IS31FL3741 device."""
 
     def __init__(self, i2c: busio.I2C, *, addr: int = 0x30) -> None:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/keypad/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/keypad/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,28 +26,24 @@
         :param int key_number: The key number.
         :param bool pressed: ``True`` if the key was pressed; ``False`` if it was released.
         :param int timestamp: The time in milliseconds that the keypress occurred in the `supervisor.ticks_ms` time system.  If specified as None, the current value of `supervisor.ticks_ms` is used.
         """
         ...
     key_number: int
     """The key number."""
-
     pressed: bool
     """``True`` if the event represents a key down (pressed) transition.
     The opposite of `released`.
     """
-
     released: bool
     """``True`` if the event represents a key up (released) transition.
     The opposite of `pressed`.
     """
-
     timestamp: int
     """The timestamp."""
-
     def __eq__(self, other: object) -> bool:
         """Two `Event` objects are equal if their `key_number`
         and `pressed`/`released` values are equal.
         Note that this does not compare the event timestamps.
         """
         ...
     def __hash__(self) -> int:
@@ -157,15 +153,14 @@
         Any key that is already pressed at the time of this call will therefore immediately cause
         a new key-pressed event to occur.
         """
         ...
     key_count: int
     """The number of keys that are being scanned. (read-only)
     """
-
     def key_number_to_row_column(self, key_number: int) -> Tuple[int]:
         """Return the row and column for the given key number.
         The row is ``key_number // len(column_pins)``.
         The column is ``key_number % len(column_pins)``.
 
         :return: ``(row, column)``
         :rtype: Tuple[int]
@@ -232,15 +227,14 @@
         Any key that is already pressed at the time of this call will therefore immediately cause
         a new key-pressed event to occur.
         """
         ...
     key_count: int
     """The number of keys that are being scanned. (read-only)
     """
-
     events: EventQueue
     """The `EventQueue` associated with this `Keys` object. (read-only)
     """
 
 class ShiftRegisterKeys:
     """Manage a set of keys attached to an incoming shift register."""
 
@@ -302,11 +296,10 @@
         Any key that is already pressed at the time of this call will therefore immediately cause
         a new key-pressed event to occur.
         """
         ...
     key_count: int
     """The number of keys that are being scanned. (read-only)
     """
-
     events: EventQueue
     """The `EventQueue` associated with this `Keys` object. (read-only)
     """
```

### Comparing `types-circuitpython-8.0.0b0/bindings/math/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/mdns/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/mdns/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,30 +17,24 @@
     object may only be created by a `mdns.Server`. It has no user-visible constructor."""
 
     def __init__(self) -> None:
         """Cannot be instantiated directly. Use `mdns.Server.find`."""
         ...
     hostname: str
     """The hostname of the device (read-only),."""
-
     instance_name: str
     """The human readable instance name for the service. (read-only)"""
-
     service_type: str
     """The service type string such as ``_http``. (read-only)"""
-
     protocol: str
     """The protocol string such as ``_tcp``. (read-only)"""
-
     port: int
     """Port number used for the service. (read-only)"""
-
     ipv4_address: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the remote service. None if no A records are found."""
-
     def __del__(self) -> None:
         """Deletes the RemoteService object."""
         ...
 
 class Server:
     """The MDNS Server responds to queries for this device's information and allows for querying
     other devices."""
@@ -54,18 +48,16 @@
     def deinit(self) -> None:
         """Stops the server"""
         ...
     hostname: str
     """Hostname resolvable as ``<hostname>.local`` in addition to ``circuitpython.local``. Make
        sure this is unique across all devices on the network. It defaults to ``cpy-######``
        where ``######`` is the hex digits of the last three bytes of the mac address."""
-
     instance_name: str
     """Human readable name to describe the device."""
-
     def find(
         self, service_type: str, protocol: str, *, timeout: float = 1
     ) -> Tuple[RemoteService]:
         """Find all locally available remote services with the given service type and protocol.
 
         This doesn't allow for direct hostname lookup. To do that, use
         `socketpool.SocketPool.getaddrinfo()`.
```

### Comparing `types-circuitpython-8.0.0b0/bindings/memorymonitor/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/memorymonitor/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         ...
     def __exit__(self) -> None:
         """Automatically pauses allocation tracking when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     bytes_per_block: int
     """Number of bytes per block"""
-
     def __len__(self) -> int:
         """Returns the number of allocation buckets.
 
         This allows you to::
 
           mm = memorymonitor.AllocationSize()
           print(len(mm))"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/microcontroller/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/microcontroller/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from nvm import ByteArray
 from watchdog import WatchDogTimer
 
 cpu: Processor
 """CPU information and control, such as ``cpu.temperature`` and ``cpu.frequency``
 (clock frequency).
 This object is an instance of `microcontroller.Processor`."""
-
 cpus: Processor
 """CPU information and control, such as ``cpus[0].temperature`` and ``cpus[1].frequency``
 (clock frequency) on chips with more than 1 cpu. The index selects which cpu.
 This object is an instance of `microcontroller.Processor`."""
 
 def delay_us(delay: int) -> None:
     """Dedicated delay method used for very short delays. **Do not** do long delays
@@ -56,15 +55,14 @@
     ...
 
 nvm: Optional[ByteArray]
 """Available non-volatile memory.
 This object is the sole instance of `nvm.ByteArray` when available or ``None`` otherwise.
 
 :type: nvm.ByteArray or None"""
-
 watchdog: Optional[WatchDogTimer]
 """Available watchdog timer.
 This object is the sole instance of `watchdog.WatchDogTimer` when available or ``None`` otherwise."""
 
 class Pin:
     """Identifies an IO pin on the microcontroller."""
 
@@ -96,26 +94,22 @@
 
     def __init__(self) -> None:
         """You cannot create an instance of `microcontroller.Processor`.
         Use `microcontroller.cpu` to access the sole instance available."""
         ...
     frequency: int
     """The CPU operating frequency in Hertz. (read-only)"""
-
     reset_reason: microcontroller.ResetReason
     """The reason the microcontroller started up from reset state."""
-
     temperature: Optional[float]
     """The on-chip temperature, in Celsius, as a float. (read-only)
 
     Is `None` if the temperature is not available."""
-
     uid: bytearray
     """The unique id (aka serial number) of the chip as a `bytearray`. (read-only)"""
-
     voltage: Optional[float]
     """The input voltage to the microcontroller, as a float. (read-only)
 
     Is `None` if the voltage is not available."""
 
 class ResetReason:
     """The reason the microntroller was last reset"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/msgpack/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/msgpack/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -95,11 +95,10 @@
     def __init__(self, code: int, data: bytes) -> None:
         """Constructor
         :param int code: type code in range 0~127.
         :param bytes data: representation."""
     code: int
     """The type code, in range 0~127."""
     ...
-
     data: bytes
     """Data."""
     ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/multiterminal/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/multiterminal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/neopixel_write/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/nvm/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/nvm/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     all values to change at once.
 
     Usage::
 
        import microcontroller
        microcontroller.nvm[0:3] = b"\xcc\x10\x00"
     """
-
     def __init__(self) -> None:
         """Not currently dynamically supported. Access the sole instance through `microcontroller.nvm`."""
         ...
     def __bool__(self) -> bool: ...
     def __len__(self) -> int:
         """Return the length. This is used by (`len`)"""
         ...
```

### Comparing `types-circuitpython-8.0.0b0/bindings/onewireio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/os/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/os/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,28 @@
 def rename(old_path: str, new_path: str) -> str:
     """Rename a file."""
     ...
 
 def stat(path: str) -> Tuple[int, int, int, int, int, int, int, int, int, int]:
     """Get the status of a file or directory.
 
+       Returns a tuple with the status of a file or directory in the following order:
+
+
+       * ``st_mode`` -- File type, regular or directory
+       * ``st_ino``  -- Set to 0
+       * ``st_dev`` -- Set to 0
+       * ``st_nlink`` -- Set to 0
+       * ``st_uid`` -- Set to 0
+       * ``st_gid`` -- Set to 0
+       * ``st_size`` -- Size of the file in bytes
+       * ``st_atime`` -- Time of most recent access expressed in seconds
+       * ``st_mtime`` -- Time of most recent content modification expressed in seconds.
+       * ``st_ctime`` -- Time of most recent content modification expressed in seconds.
+
     .. note:: On builds without long integers, the number of seconds
        for contemporary dates will not fit in a small integer.
        So the time fields return 946684800,
        which is the number of seconds corresponding to 1999-12-31."""
     ...
 
 def statvfs(path: str) -> Tuple[int, int, int, int, int, int, int, int, int, int]:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/paralleldisplay/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/ps2io/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/pulseio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/pulseio/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,19 +86,17 @@
         ...
     def popleft(self) -> int:
         """Removes and returns the oldest read pulse."""
         ...
     maxlen: int
     """The maximum length of the PulseIn. When len() is equal to maxlen,
     it is unclear which pulses are active and which are idle."""
-
     paused: bool
     """True when pulse capture is paused as a result of :py:func:`pause` or an error during capture
     such as a signal that is too fast."""
-
     def __bool__(self) -> bool: ...
     def __len__(self) -> int:
         """Returns the number of pulse durations currently stored.
 
         This allows you to::
 
           pulses = pulseio.PulseIn(pin)
```

### Comparing `types-circuitpython-8.0.0b0/bindings/pwmio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/pwmio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     (0). 0xffff will always be high, 0 will always be low and 0x7fff will
     be half high and then half low.
 
     Depending on how PWM is implemented on a specific board, the internal
     representation for duty cycle might have less than 16 bits of resolution.
     Reading this property will return the value from the internal representation,
     so it may differ from the value set."""
-
     frequency: int
     """32 bit value that dictates the PWM frequency in Hertz (cycles per
     second). Only writeable when constructed with ``variable_frequency=True``.
 
     Depending on how PWM is implemented on a specific board, the internal value
     for the PWM's duty cycle may need to be recalculated when the frequency
     changes. In these cases, the duty cycle is automatically recalculated
```

### Comparing `types-circuitpython-8.0.0b0/bindings/qrio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/qrio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         ...
     def decode(
         self, buffer: ReadableBuffer, pixel_policy: PixelPolicy = PixelPolicy.EVERY_BYTE
     ) -> List[QRInfo]:
         """Decode zero or more QR codes from the given image.  The size of the buffer must be at least ``length``×``width`` bytes for `EVERY_BYTE`, and 2×``length``×``width`` bytes for `EVEN_BYTES` or `ODD_BYTES`."""
     width: int
     """The width of image the decoder expects"""
-
     height: int
     """The height of image the decoder expects"""
 
 class QRInfo:
     """Information about a decoded QR code"""
 
     payload: bytes
```

### Comparing `types-circuitpython-8.0.0b0/bindings/random/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/rgbmatrix/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/rgbmatrix/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,15 @@
         """Free the resources (pins, timers, etc.) associated with this
         rgbmatrix instance.  After deinitialization, no further operations
         may be performed."""
         ...
     brightness: float
     """In the current implementation, 0.0 turns the display off entirely
     and any other value up to 1.0 turns the display on fully."""
-
     def refresh(self) -> None:
         """Transmits the color data in the buffer to the pixels so that
         they are shown."""
         ...
     width: int
     """The width of the display, in pixels"""
-
     height: int
     """The height of the display, in pixels"""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/rotaryio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/rotaryio/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Support for reading rotation sensors
 
 The `rotaryio` module contains classes to read different rotation encoding schemes. See
 `Wikipedia's Rotary Encoder page <https://en.wikipedia.org/wiki/Rotary_encoder>`_ for more
 background.
 
+For more information on working with rotary encoders using this library, see
+`this Learn Guide <https://learn.adafruit.com/rotary-encoder>`_.
+
 All classes change hardware state and should be deinitialized when they
 are no longer needed if the program continues after use. To do so, either
 call :py:meth:`!deinit` or use a context manager. See
 :ref:`lifetime-and-contextmanagers` for more info."""
 
 from __future__ import annotations
 
@@ -51,11 +54,10 @@
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     divisor: int
     """The divisor of the quadrature signal.  Use 1 for encoders without
     detents, or encoders with 4 detents per cycle.  Use 2 for encoders with 2
     detents per cycle.  Use 4 for encoders with 1 detent per cycle."""
-
     position: int
     """The current position in terms of pulses. The number of pulses per rotation is defined by the
     specific hardware and by the divisor."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/rtc/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/rtc/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     Once set, the RTC will automatically update this value as time passes. You can read this
     property to get a snapshot of the current time::
 
       current_time = r.datetime
       print(current_time)
       # struct_time(tm_year=2019, tm_month=5, ...)"""
-
     calibration: int
     """The RTC calibration value as an `int`.
 
     A positive value speeds up the clock and a negative value slows it down.
     Range and value is hardware specific, but one step is often approximately 1 ppm::
 
       import rtc
```

### Comparing `types-circuitpython-8.0.0b0/bindings/sdcardio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/sdioio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/sdioio/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -74,23 +74,19 @@
 
         """Write one or more blocks to the card
 
         :param int start_block: The block to start writing from
         :param ~circuitpython_typing.ReadableBuffer buf: The buffer to read from.  Length must be multiple of 512.
 
         :return: None"""
-    @property
-    def frequency(self) -> int:
-        """The actual SDIO bus frequency. This may not match the frequency
-        requested due to internal limitations."""
-        ...
-    @property
-    def width(self) -> int:
-        """The actual SDIO bus width, in bits"""
-        ...
+    frequency: int
+    """The actual SDIO bus frequency. This may not match the frequency
+    requested due to internal limitations."""
+    width: int
+    """The actual SDIO bus width, in bits"""
     def deinit(self) -> None:
         """Disable permanently.
 
         :return: None"""
     def __enter__(self) -> SDCard:
         """No-op used by Context Managers.
         Provided by context manager helper."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/socketpool/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/socketpool/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from __future__ import annotations
 
 from typing import Optional, Tuple
 
 import socketpool
+import wifi
 from circuitpython_typing import ReadableBuffer, WriteableBuffer
 
 class Socket:
     """TCP, UDP and RAW socket. Cannot be created directly. Instead, call
     `SocketPool.socket()`.
 
     Provides a subset of CPython's `socket.socket` API. It only implements the versions of
@@ -98,16 +99,25 @@
         ...
 
 class SocketPool:
     """A pool of socket resources available for the given radio. Only one
     SocketPool can be created for each radio.
 
     SocketPool should be used in place of CPython's socket which provides
-    a pool of sockets provided by the underlying OS."""
+    a pool of sockets provided by the underlying OS.
+    """
 
+    def __init__(self, radio: wifi.Radio) -> None:
+        """Create a new SocketPool object for the provided radio
+
+        :param wifi.Radio radio: The (connected) network hardware to associate
+            with this SocketPool; currently, this will always be the object
+            returned by :py:attr:`wifi.radio`
+        """
+        ...
     AF_INET: int
     AF_INET6: int
     SOCK_STREAM: int
     SOCK_DGRAM: int
     SOCK_RAW: int
 
     def socket(
```

### Comparing `types-circuitpython-8.0.0b0/bindings/ssl/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/ssl/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     def load_verify_locations(self, cadata: Optional[str] = None) -> None:
         """Load a set of certification authority (CA) certificates used to validate
         other peers' certificates."""
     def set_default_verify_paths(self) -> None:
         """Load a set of default certification authority (CA) certificates."""
     check_hostname: bool
     """Whether to match the peer certificate's hostname."""
-
     def wrap_socket(
         self,
         sock: socketpool.Socket,
         *,
         server_side: bool = False,
         server_hostname: Optional[str] = None,
     ) -> ssl.SSLSocket:
```

### Comparing `types-circuitpython-8.0.0b0/bindings/storage/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/storage/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Storage management
 
 The `storage` provides storage management functionality such as mounting and
 unmounting which is typically handled by the operating system hosting Python.
 CircuitPython does not have an OS, so this module provides this functionality
 directly.
+
 For more information regarding using the `storage` module, refer to the `CircuitPython
 Essentials Learn guide
 <https://learn.adafruit.com/circuitpython-essentials/circuitpython-storage>`_.
 """
 
 from __future__ import annotations
```

### Comparing `types-circuitpython-8.0.0b0/bindings/struct/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/supervisor/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/supervisor/__init__.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 from typing import Optional
 
 runtime: Runtime
 """Runtime information, such as ``runtime.serial_connected``
 (USB serial connection status).
 This object is the sole instance of `supervisor.Runtime`."""
+status_bar: StatusBar
+"""The status bar, shown on an attached display, and also sent to
+an attached terminal via OSC escape codes over the REPL serial connection.
+The status bar reports the current IP or BLE connection, what file is running,
+the last exception name and location, and firmware version information.
+This object is the sole instance of `supervisor.StatusBar`."""
 
 def set_rgb_status_brightness(brightness: int) -> None:
     """Set brightness of status RGB LED from 0-255. This will take effect
     after the current code finishes and the status LED is used to show
     the finish state."""
     ...
 
@@ -121,14 +127,31 @@
     the services used for it."""
     ...
 
 def reset_terminal(x_pixels: int, y_pixels: int) -> None:
     """Reset the CircuitPython serial terminal with new dimensions."""
     ...
 
+def set_usb_identification(
+    manufacturer: Optional[str] = None,
+    product: Optional[str] = None,
+    vid: int = -1,
+    pid: int = -1,
+) -> None:
+    """Override identification constants in the USB Device Descriptor.
+
+    If passed, `manufacturer` and `product` must be ASCII strings (or buffers) of at most 126
+    characters. Any omitted arguments will be left at their default values.
+
+    This method must be called in boot.py to have any effect.
+
+    Not available on boards without native USB support.
+    """
+    ...
+
 class RunReason:
     """The reason that CircuitPython started running."""
 
     STARTUP: object
     """CircuitPython started the microcontroller started up. See `microcontroller.Processor.reset_reason`
        for more detail on why the microcontroller was started."""
 
@@ -152,21 +175,44 @@
 
     def __init__(self) -> None:
         """You cannot create an instance of `supervisor.Runtime`.
         Use `supervisor.runtime` to access the sole instance available."""
         ...
     usb_connected: bool
     """Returns the USB enumeration status (read-only)."""
-
     serial_connected: bool
     """Returns the USB serial communication status (read-only)."""
-
     serial_bytes_available: int
     """Returns the whether any bytes are available to read
     on the USB serial input.  Allows for polling to see whether
     to call the built-in input() or wait. (read-only)"""
-
     run_reason: RunReason
     """Why CircuitPython started running this particular time."""
-
     autoreload: bool
     """Whether CircuitPython may autoreload based on workflow writes to the filesystem."""
+
+class StatusBar:
+    """Current status of runtime objects.
+
+    Usage::
+
+       import supervisor
+
+       supervisor.status_bar.console = False
+    """
+
+    def __init__(self) -> None:
+        """You cannot create an instance of `supervisor.StatusBar`.
+        Use `supervisor.status_bar` to access the sole instance available."""
+        ...
+    console: bool
+    """Whether status bar information is sent over the console (REPL) serial connection,
+    using OSC terminal escape codes that change the terminal's title. Default is ``True``.
+    If set to ``False``, status bar will be cleared and then disabled.
+    May be set in ``boot.py`` or later. Persists across soft restarts.
+    """
+    display: bool
+    """Whether status bar information is displayed on the top line of the display.
+    Default is ``True``. If set to ``False``, status bar will be cleared and then disabled.
+    May be set in ``boot.py`` or later.  Persists across soft restarts.
+    Not available if `terminalio` is not available.
+    """
```

### Comparing `types-circuitpython-8.0.0b0/bindings/synthio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/terminalio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/terminalio/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     """
 
     def __init__(
         self,
         scroll_area: displayio.TileGrid,
         font: fontio.BuiltinFont,
         *,
-        title_bar: displayio.TileGrid = None,
+        status_bar: displayio.TileGrid = None,
     ) -> None:
         """Terminal manages tile indices and cursor position based on VT100 commands. The font should be
         a `fontio.BuiltinFont` and the TileGrid's bitmap should match the font's bitmap."""
         ...
     def write(self, buf: ReadableBuffer) -> Optional[int]:
         """Write the buffer of bytes to the bus.
```

### Comparing `types-circuitpython-8.0.0b0/bindings/time/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/touchio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/touchio/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -56,18 +56,16 @@
         """Automatically deinitializes the hardware when exiting a context. See
         :ref:`lifetime-and-contextmanagers` for more info."""
         ...
     value: bool
     """Whether the touch pad is being touched or not. (read-only)
 
     True when `raw_value` > `threshold`."""
-
     raw_value: int
     """The raw touch measurement as an `int`. (read-only)"""
-
     threshold: Optional[int]
     """Minimum `raw_value` needed to detect a touch (and for `value` to be `True`).
 
     When the **TouchIn** object is created, an initial `raw_value` is read from the pin,
     and then `threshold` is set to be 100 + that value.
 
     You can adjust `threshold` to make the pin more or less sensitive::
```

### Comparing `types-circuitpython-8.0.0b0/bindings/traceback/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/usb_cdc/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/usb_cdc/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -66,19 +66,20 @@
         and fewer than ``size`` bytes are available, keep waiting until the timeout
         expires or ``size`` bytes are available.
 
         :return: Data read
         :rtype: bytes"""
         ...
     def readinto(self, buf: WriteableBuffer) -> int:
-        """Read bytes into the ``buf``.  If ``nbytes`` is specified then read at most
-        that many bytes, subject to `timeout`.  Otherwise, read at most ``len(buf)`` bytes.
+        """Read bytes into the ``buf``. Read at most ``len(buf)`` bytes. If `timeout`
+        is > 0 or ``None``, keep waiting until the timeout expires or ``len(buf)``
+        bytes are available.
 
         :return: number of bytes read and stored into ``buf``
-        :rtype: bytes"""
+        :rtype: int"""
         ...
     def readline(self, size: int = -1) -> Optional[bytes]:
         r"""Read a line ending in a newline character ("\\n"), including the newline.
         Return everything readable if no newline is found and ``timeout`` is 0.
         Return ``None`` in case of error.
 
         This is a binary stream: the newline character "\\n" cannot be changed.
@@ -109,28 +110,24 @@
     connected: bool
     """True if this Serial is connected to a host. (read-only)
 
     .. note:: The host is considered to be connected if it is asserting DTR (Data Terminal Ready).
       Most terminal programs and ``pyserial`` assert DTR when opening a serial connection.
       However, the C# ``SerialPort`` API does not. You must set ``SerialPort.DtrEnable``.
     """
-
     in_waiting: int
     """Returns the number of bytes waiting to be read on the USB serial input. (read-only)"""
-
     out_waiting: int
     """Returns the number of bytes waiting to be written on the USB serial output. (read-only)"""
-
     def reset_input_buffer(self) -> None:
         """Clears any unread bytes."""
         ...
     def reset_output_buffer(self) -> None:
         """Clears any unwritten bytes."""
         ...
     timeout: Optional[float]
     """The initial value of `timeout` is ``None``. If ``None``, wait indefinitely to satisfy
     the conditions of a read operation. If 0, do not wait. If > 0, wait only ``timeout`` seconds."""
-
     write_timeout: Optional[float]
     """The initial value of `write_timeout` is ``None``. If ``None``, wait indefinitely to finish
     writing all the bytes passed to ``write()``.If 0, do not wait.
     If > 0, wait only ``write_timeout`` seconds."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/usb_hid/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/usb_hid/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -142,37 +142,31 @@
     in each report, and a relative mouse wheel change from -127 to 127 in each report.
     Uses Report ID 2 for its IN report.
     """
 
     CONSUMER_CONTROL: Device
     """Consumer Control device supporting sent values from 1-652, with no rollover.
     Uses Report ID 3 for its IN report."""
-
     def send_report(
         self, report: ReadableBuffer, report_id: Optional[int] = None
     ) -> None:
         """Send an HID report. If the device descriptor specifies zero or one report id's,
         you can supply `None` (the default) as the value of ``report_id``.
         Otherwise you must specify which report id to use when sending the report.
         """
         ...
-    def get_last_received_report(self, report_id: Optional[int] = None) -> bytes:
+    def get_last_received_report(
+        self, report_id: Optional[int] = None
+    ) -> Optional[bytes]:
         """Get the last received HID OUT or feature report for the given report ID.
         The report ID may be omitted if there is no report ID, or only one report ID.
-        Return `None` if nothing received.
+        Return `None` if nothing received. After returning a report, subsequent calls
+        will return `None` until next report is received.
         """
         ...
-    last_received_report: bytes
-    """The HID OUT report as a `bytes` (read-only). `None` if nothing received.
-    Same as `get_last_received_report()` with no argument.
-
-    Deprecated: will be removed in CircutPython 8.0.0. Use `get_last_received_report()` instead.
-    """
-
     usage_page: int
     """The device usage page identifier, which designates a category of device. (read-only)"""
-
     usage: int
     """The device usage identifier, which designates a specific kind of device. (read-only)
 
     For example, Keyboard is 0x06 within the generic desktop usage page 0x01.
     Mouse is 0x02 within the same usage page."""
```

### Comparing `types-circuitpython-8.0.0b0/bindings/usb_host/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/usb_midi/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/bindings/vectorio/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/vectorio/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,18 +41,16 @@
         :param Union[~displayio.ColorConverter,~displayio.Palette] pixel_shader: The pixel shader that produces colors from values
         :param int radius: The radius of the circle in pixels
         :param int x: Initial x position of the axis.
         :param int y: Initial y position of the axis.
         :param int color_index: Initial color_index to use when selecting color from the palette."""
     radius: int
     """The radius of the circle in pixels."""
-
     color_index: int
     """The color_index of the circle as 0 based index of the palette."""
-
     x: int
     """X position of the center point of the circle in the parent."""
 
     y: int
     """Y position of the center point of the circle in the parent."""
 
     location: Tuple[int, int]
@@ -76,18 +74,16 @@
             shader that produces colors from values
         :param List[Tuple[int,int]] points: Vertices for the polygon
         :param int x: Initial screen x position of the 0,0 origin in the points list.
         :param int y: Initial screen y position of the 0,0 origin in the points list.
         :param int color_index: Initial color_index to use when selecting color from the palette."""
     points: List[Tuple[int, int]]
     """Vertices for the polygon."""
-
     color_index: int
     """The color_index of the polygon as 0 based index of the palette."""
-
     x: int
     """X position of the 0,0 origin in the points list."""
 
     y: int
     """Y position of the 0,0 origin in the points list."""
 
     location: Tuple[int, int]
@@ -111,21 +107,18 @@
         :param int width: The number of pixels wide
         :param int height: The number of pixels high
         :param int x: Initial x position of the top left corner.
         :param int y: Initial y position of the top left corner.
         :param int color_index: Initial color_index to use when selecting color from the palette."""
     width: int
     """The width of the rectangle in pixels."""
-
     height: int
     """The height of the rectangle in pixels."""
-
     color_index: int
     """The color_index of the rectangle in 1 based index of the palette."""
-
     x: int
     """X position of the top left corner of the rectangle in the parent."""
 
     y: int
     """Y position of the top left corner of the rectangle in the parent."""
 
     location: Tuple[int, int]
```

### Comparing `types-circuitpython-8.0.0b0/bindings/watchdog/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/watchdog/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def deinit(self) -> None:
         """Stop the watchdog timer. This may raise an error if the watchdog
         timer cannot be disabled on this platform."""
         ...
     timeout: float
     """The maximum number of seconds that can elapse between calls
     to feed()"""
-
     mode: WatchDogMode
     """The current operating mode of the WatchDogTimer `watchdog.WatchDogMode`.
 
     Setting a WatchDogMode activates the WatchDog::
 
       import microcontroller
       import watchdog
```

### Comparing `types-circuitpython-8.0.0b0/bindings/wifi/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/wifi/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     :param int queue: The queue size for buffering the packet.
 
     """
     ...
 
 channel: int
 """The WiFi channel to scan."""
-
 queue: int
 """The queue size for buffering the packet."""
 
 def deinit(self) -> None:
     """De-initialize `wifi.Monitor` singleton."""
     ...
 
@@ -75,27 +74,22 @@
     """A wifi network provided by a nearby access point."""
 
     def __init__(self) -> None:
         """You cannot create an instance of `wifi.Network`. They are returned by `wifi.Radio.start_scanning_networks`."""
         ...
     ssid: str
     """String id of the network"""
-
     bssid: bytes
     """BSSID of the network (usually the AP's MAC address)"""
-
     rssi: int
     """Signal strength of the network"""
-
     channel: int
     """Channel number the network is operating on"""
-
     country: str
     """String id of the country code"""
-
     authmode: str
     """String id of the authmode"""
 
 class Packet:
     """The packet parameters."""
 
     CH: object
@@ -122,30 +116,25 @@
         """You cannot create an instance of `wifi.Radio`.
         Use `wifi.radio` to access the sole instance available."""
         ...
     enabled: bool
     """``True`` when the wifi radio is enabled.
     If you set the value to ``False``, any open sockets will be closed.
     """
-
     hostname: Union[str | ReadableBuffer]
     """Hostname for wifi interface. When the hostname is altered after interface started/connected
        the changes would only be reflected once the interface restarts/reconnects."""
-
     mac_address: ReadableBuffer
     """MAC address for the station. When the address is altered after interface is connected
        the changes would only be reflected once the interface reconnects."""
-
     tx_power: float
     """Wifi transmission power, in dBm."""
-
     mac_address_ap: ReadableBuffer
     """MAC address for the AP. When the address is altered after interface is started
        the changes would only be reflected once the interface restarts."""
-
     def start_scanning_networks(
         self, *, start_channel: int = 1, stop_channel: int = 11
     ) -> Iterable[Network]:
         """Scans for available wifi networks over the given channel range. Make sure the channels are allowed in your country."""
         ...
     def stop_scanning_networks(self) -> None:
         """Stop scanning for Wifi networks and free any resources used to do it."""
@@ -201,47 +190,39 @@
         significantly because a full scan doesn't occur.
 
         If ``bssid`` is given, the scan will start at the first channel or the one given and
         connect to the AP with the given ``bssid`` and ``ssid``."""
         ...
     ipv4_gateway: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the station gateway when connected to an access point. None otherwise."""
-
     ipv4_gateway_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point gateway, when enabled. None otherwise."""
-
     ipv4_subnet: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the station subnet when connected to an access point. None otherwise."""
-
     ipv4_subnet_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point subnet, when enabled. None otherwise."""
-
     def set_ipv4_address(
         self,
         *,
         ipv4: ipaddress.IPv4Address,
         netmask: ipaddress.IPv4Address,
         gateway: ipaddress.IPv4Address,
         ipv4_dns: Optional[ipaddress.IPv4Address],
     ) -> None:
         """Sets the IP v4 address of the station. Must include the netmask and gateway. DNS address is optional.
         Setting the address manually will stop the DHCP client."""
         ...
     ipv4_address: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the station when connected to an access point. None otherwise."""
-
     ipv4_address_ap: Optional[ipaddress.IPv4Address]
     """IP v4 Address of the access point, when enabled. None otherwise."""
-
     ipv4_dns: ipaddress.IPv4Address
     """IP v4 Address of the DNS server to be used."""
-
     ap_info: Optional[Network]
     """Network object containing BSSID, SSID, authmode, channel, country and RSSI when connected to an access point. None otherwise."""
-
     def start_dhcp(self) -> None:
         """Starts the DHCP client."""
         ...
     def stop_dhcp(self) -> None:
         """Stops the DHCP client. Needed to assign a static IP address."""
         ...
     def ping(
```

### Comparing `types-circuitpython-8.0.0b0/bindings/zlib/__init__.pyi` & `types-circuitpython-8.0.0b1/bindings/zlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-circuitpython-8.0.0b0/setup.py` & `types-circuitpython-8.0.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import listdir, path
 
 from setuptools import setup
 
 __name__ = "types-circuitpython"
-__version__ = "8.0.0-beta.0"
+__version__ = "8.0.0-beta.1"
 __repo__ = "https://github.com/hardfury-labs/types-circuitpython"
 __author__ = "HardFury"
 
 
 HERE = path.abspath(path.dirname(__file__))
 BINDINGS_DIR = path.join(HERE, "bindings")
```

### Comparing `types-circuitpython-8.0.0b0/types_circuitpython.egg-info/PKG-INFO` & `types-circuitpython-8.0.0b1/types_circuitpython.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-circuitpython
-Version: 8.0.0b0
+Version: 8.0.0b1
 Summary: Type support (typings) for CircuitPython built-in binding packages.
 Home-page: https://github.com/hardfury-labs/types-circuitpython
 Author: HardFury
 License: GNU General Public License v3 (GPLv3)
 Keywords: circuitpython,micropython,adafruit
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
@@ -26,39 +26,44 @@
 # types-circuitpython
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-circuitpython?style=flat-square)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/types-circuitpython?style=flat-square)
 
 Type Support (typings) for [CircuitPython](https://github.com/adafruit/circuitpython) built-in binding packages.
 
-Coding with adafruit-circuitpython-typing:
+Coding with `adafruit-circuitpython-typing`:
 
 ![adafruit-circuitpython-typing](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/adafruit-circuitpython-typing.gif)
 
-Coding with types-circuitpython:
+Coding with `types-circuitpython`:
 
 ![types-circuitpython](https://raw.githubusercontent.com/hardfury-labs/types-circuitpython/master/screen-records/types-circuitpython.gif)
 
 ## Long term support versions
 
 Following [CircuitPython release versions](https://github.com/adafruit/circuitpython/releases)
 
 [Pypi versions](https://pypi.org/project/types-circuitpython/#history)
 
+- 8.x
+  - 8.0.0b0 (Corresponds 8.0.0-beta.0 of CircuitPython)
+  - 8.0.0a1 (Corresponds 8.0.0-alpha.1 of CircuitPython)
+  - 8.0.0a0 (Corresponds 8.0.0-alpha.0 of CircuitPython)
 - 7.x
   - 7.3.3
-- 8.x
-  - 8.0.0-beta.0
+  - 7.3.2
+  - 7.3.1
+  - 7.3.0
 
 ## Usage
 
 ```bash
 $ pip install types-circuitpython==7.3.3
 # or
-$ pip install types-circuitpython==8.0.0-beta.0
+$ pip install types-circuitpython==8.0.0b0
 ```
 
 ## Development
 
 ## Initialization
 
 ```bash
@@ -66,14 +71,20 @@
 $ . ./.venv/bin/activate
 $ pip install -r requirements.txt
 $ python setup.py develop
 # or
 $ pip install -e .
 ```
 
+## Update CircuitPython submodule
+
+```bash
+$ git submodule update --remote
+```
+
 ## Generate bindings
 
 ```bash
 $ make generate version=<CIRCUITPYTHON VERSION>
 ```
 
 ## Code styles
```

### Comparing `types-circuitpython-8.0.0b0/types_circuitpython.egg-info/SOURCES.txt` & `types-circuitpython-8.0.0b1/types_circuitpython.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 bindings/_eve/__init__.pyi
 bindings/_pew/__init__.pyi
 bindings/_stage/__init__.pyi
 bindings/adafruit_bus_device/__init__.pyi
 bindings/adafruit_pixelbuf/__init__.pyi
 bindings/aesio/__init__.pyi
 bindings/alarm/__init__.pyi
+bindings/analogbufio/__init__.pyi
 bindings/analogio/__init__.pyi
 bindings/atexit/__init__.pyi
 bindings/audiobusio/__init__.pyi
 bindings/audiocore/__init__.pyi
 bindings/audioio/__init__.pyi
 bindings/audiomixer/__init__.pyi
 bindings/audiomp3/__init__.pyi
```

### Comparing `types-circuitpython-8.0.0b0/types_circuitpython.egg-info/top_level.txt` & `types-circuitpython-8.0.0b1/types_circuitpython.egg-info/top_level.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 _eve
 _pew
 _stage
 adafruit_bus_device
 adafruit_pixelbuf
 aesio
 alarm
+analogbufio
 analogio
 atexit
 audiobusio
 audiocore
 audioio
 audiomixer
 audiomp3
```

