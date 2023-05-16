# Comparing `tmp/pcf8591-library-0.0.1.tar.gz` & `tmp/pcf8591-library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcf8591-library-0.0.1.tar", last modified: Tue Apr 18 21:11:57 2023, max compression
+gzip compressed data, was "pcf8591-library-0.0.2.tar", last modified: Tue May 16 15:03:39 2023, max compression
```

## Comparing `pcf8591-library-0.0.1.tar` & `pcf8591-library-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 21:11:57.223689 pcf8591-library-0.0.1/
--rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 pcf8591-library-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     5747 2023-04-18 21:11:57.223689 pcf8591-library-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2803 2023-04-18 21:06:59.000000 pcf8591-library-0.0.1/README.md
--rw-rw-rw-   0        0        0     1531 2023-04-18 20:41:52.000000 pcf8591-library-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      759 2023-04-18 21:11:57.225673 pcf8591-library-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-04-18 20:45:05.000000 pcf8591-library-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 21:11:57.201673 pcf8591-library-0.0.1/src/
--rw-rw-rw-   0        0        0     3941 2023-04-18 20:23:00.000000 pcf8591-library-0.0.1/src/PCF8591.py
-drwxrwxrwx   0        0        0        0 2023-04-18 21:11:57.220674 pcf8591-library-0.0.1/src/pcf8591_library.egg-info/
--rw-rw-rw-   0        0        0     5747 2023-04-18 21:11:57.000000 pcf8591-library-0.0.1/src/pcf8591_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-18 21:11:57.000000 pcf8591-library-0.0.1/src/pcf8591_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 21:11:57.000000 pcf8591-library-0.0.1/src/pcf8591_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 21:11:57.000000 pcf8591-library-0.0.1/src/pcf8591_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 15:03:39.538125 pcf8591-library-0.0.2/
+-rw-rw-rw-   0        0        0     1281 2023-03-21 14:14:13.000000 pcf8591-library-0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     5911 2023-05-16 15:03:39.539125 pcf8591-library-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2967 2023-05-16 15:01:21.000000 pcf8591-library-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1531 2023-05-16 14:55:32.000000 pcf8591-library-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      759 2023-05-16 15:03:39.552120 pcf8591-library-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-05-16 14:55:32.000000 pcf8591-library-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:03:39.522119 pcf8591-library-0.0.2/src/
+-rw-rw-rw-   0        0        0     6796 2023-05-16 14:55:32.000000 pcf8591-library-0.0.2/src/PCF8591.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:03:39.536117 pcf8591-library-0.0.2/src/pcf8591_library.egg-info/
+-rw-rw-rw-   0        0        0     5911 2023-05-16 15:03:39.000000 pcf8591-library-0.0.2/src/pcf8591_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-16 15:03:39.000000 pcf8591-library-0.0.2/src/pcf8591_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:03:39.000000 pcf8591-library-0.0.2/src/pcf8591_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 15:03:39.000000 pcf8591-library-0.0.2/src/pcf8591_library.egg-info/top_level.txt
```

### Comparing `pcf8591-library-0.0.1/LICENSE.md` & `pcf8591-library-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pcf8591-library-0.0.1/PKG-INFO` & `pcf8591-library-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcf8591-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to use pcf8591 i2c analog IC with Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266. Can read analog value and write analog value with only 2 wire. 
 Home-page: https://github.com/xreef/PCF8591_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -59,14 +59,15 @@
 
 #
 #### www.mischianti.org
 
 ### MicroPython Library to use i2c analog IC with arduino and esp8266. Can read analog value and write analog value with only 2 wire (perfect for ESP-01).
 
 #### Changelog
+ - 16/05/2023: v0.0.2 Minor fix on read and write [#Forum](https://www.mischianti.org/forums/topic/micropython-i2c-pcf8591-round-value-problem-raspberry-pi-pico/)
  - 18/04/2023: v0.0.1 Initial commit of stable version.
 
 I try to simplify the use of this IC, with a minimal set of operation.
 
 #### Installation
 To install the library execute the following command:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcf8591-library Version: 0.0.1 Summary: Library to
+Metadata-Version: 2.1 Name: pcf8591-library Version: 0.0.2 Summary: Library to
 use pcf8591 i2c analog IC with Arduino, Raspberry Pi Pico and rp2040 boards,
 esp32, SMT32 and ESP8266. Can read analog value and write analog value with
 only 2 wire. Home-page: https://github.com/xreef/PCF8591_micropython_library
 Author: Renzo Mischianti Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -34,21 +34,23 @@
 Implementation :: MicroPython Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE.md
 [Support_forum_pcf8591_English]
 [Forum_supporto_pcf8591_italiano]
 # #### www.mischianti.org ### MicroPython Library to use i2c analog IC with
 arduino and esp8266. Can read analog value and write analog value with only 2
-wire (perfect for ESP-01). #### Changelog - 18/04/2023: v0.0.1 Initial commit
-of stable version. I try to simplify the use of this IC, with a minimal set of
-operation. #### Installation To install the library execute the following
-command: ```bash pip install pcf8591-library ``` **Constructor:** Pass the
-address of I2C ```python from PCF8591 import PCF8591 from machine import I2C,
-Pin # Initialize the I2C bus i2c = I2C(0, scl=Pin(22), sda=Pin(21)) #
-Initialize the PCF8591 pcf8591 = PCF8591(0x48, i2c) if pcf8591.begin(): print
+wire (perfect for ESP-01). #### Changelog - 16/05/2023: v0.0.2 Minor fix on
+read and write [#Forum](https://www.mischianti.org/forums/topic/micropython-
+i2c-pcf8591-round-value-problem-raspberry-pi-pico/) - 18/04/2023: v0.0.1
+Initial commit of stable version. I try to simplify the use of this IC, with a
+minimal set of operation. #### Installation To install the library execute the
+following command: ```bash pip install pcf8591-library ``` **Constructor:**
+Pass the address of I2C ```python from PCF8591 import PCF8591 from machine
+import I2C, Pin # Initialize the I2C bus i2c = I2C(0, scl=Pin(22), sda=Pin(21))
+# Initialize the PCF8591 pcf8591 = PCF8591(0x48, i2c) if pcf8591.begin(): print
 ("PCF8591 found") ``` or ```python from PCF8591 import PCF8591 pcf8591 =
 PCF8591(0x48, sda=21, scl=22) if pcf8591.begin(): print("PCF8591 found") ``` To
 read all analog input in one ```python # Main loop while True: # Read all
 analog input channels ain0, ain1, ain2, ain3 = pcf8591.analog_read_all() #
 Print the results print("AIN0:", ain0, "AIN1:", ain1, "AIN2:", ain2, "AIN3:",
 ain3) # Wait for 1 second utime.sleep(1) ``` If you want to read a single
 input: ```python print("AIN0 ", pcf8591.analog_read(PCF8591.AIN0)) print("AIN1
```

### Comparing `pcf8591-library-0.0.1/README.md` & `pcf8591-library-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 #
 #### www.mischianti.org
 
 ### MicroPython Library to use i2c analog IC with arduino and esp8266. Can read analog value and write analog value with only 2 wire (perfect for ESP-01).
 
 #### Changelog
+ - 16/05/2023: v0.0.2 Minor fix on read and write [#Forum](https://www.mischianti.org/forums/topic/micropython-i2c-pcf8591-round-value-problem-raspberry-pi-pico/)
  - 18/04/2023: v0.0.1 Initial commit of stable version.
 
 I try to simplify the use of this IC, with a minimal set of operation.
 
 #### Installation
 To install the library execute the following command:
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
 [Support_forum_pcf8591_English]
 [Forum_supporto_pcf8591_italiano]
 # #### www.mischianti.org ### MicroPython Library to use i2c analog IC with
 arduino and esp8266. Can read analog value and write analog value with only 2
-wire (perfect for ESP-01). #### Changelog - 18/04/2023: v0.0.1 Initial commit
-of stable version. I try to simplify the use of this IC, with a minimal set of
-operation. #### Installation To install the library execute the following
-command: ```bash pip install pcf8591-library ``` **Constructor:** Pass the
-address of I2C ```python from PCF8591 import PCF8591 from machine import I2C,
-Pin # Initialize the I2C bus i2c = I2C(0, scl=Pin(22), sda=Pin(21)) #
-Initialize the PCF8591 pcf8591 = PCF8591(0x48, i2c) if pcf8591.begin(): print
+wire (perfect for ESP-01). #### Changelog - 16/05/2023: v0.0.2 Minor fix on
+read and write [#Forum](https://www.mischianti.org/forums/topic/micropython-
+i2c-pcf8591-round-value-problem-raspberry-pi-pico/) - 18/04/2023: v0.0.1
+Initial commit of stable version. I try to simplify the use of this IC, with a
+minimal set of operation. #### Installation To install the library execute the
+following command: ```bash pip install pcf8591-library ``` **Constructor:**
+Pass the address of I2C ```python from PCF8591 import PCF8591 from machine
+import I2C, Pin # Initialize the I2C bus i2c = I2C(0, scl=Pin(22), sda=Pin(21))
+# Initialize the PCF8591 pcf8591 = PCF8591(0x48, i2c) if pcf8591.begin(): print
 ("PCF8591 found") ``` or ```python from PCF8591 import PCF8591 pcf8591 =
 PCF8591(0x48, sda=21, scl=22) if pcf8591.begin(): print("PCF8591 found") ``` To
 read all analog input in one ```python # Main loop while True: # Read all
 analog input channels ain0, ain1, ain2, ain3 = pcf8591.analog_read_all() #
 Print the results print("AIN0:", ain0, "AIN1:", ain1, "AIN2:", ain2, "AIN3:",
 ain3) # Wait for 1 second utime.sleep(1) ``` If you want to read a single
 input: ```python print("AIN0 ", pcf8591.analog_read(PCF8591.AIN0)) print("AIN1
```

### Comparing `pcf8591-library-0.0.1/pyproject.toml` & `pcf8591-library-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 6366 3835 3931 2d6c 6962 7261  = "pcf8591-libra
 00000020: 7279 220d 0a76 6572 7369 6f6e 203d 2022  ry"..version = "
-00000030: 302e 302e 3122 0d0a 6175 7468 6f72 7320  0.0.1"..authors 
+00000030: 302e 302e 3222 0d0a 6175 7468 6f72 7320  0.0.2"..authors 
 00000040: 3d20 5b0d 0a20 207b 206e 616d 653d 2252  = [..  { name="R
 00000050: 656e 7a6f 204d 6973 6368 6961 6e74 6922  enzo Mischianti"
 00000060: 2c20 656d 6169 6c3d 2272 656e 7a6f 406d  , email="renzo@m
 00000070: 6973 6368 6961 6e74 692e 6f72 6722 207d  ischianti.org" }
 00000080: 2c0d 0a5d 0d0a 6d61 696e 7461 696e 6572  ,..]..maintainer
 00000090: 7320 3d20 5b0d 0a20 207b 206e 616d 653d  s = [..  { name=
 000000a0: 2252 656e 7a6f 204d 6973 6368 6961 6e74  "Renzo Mischiant
```

### Comparing `pcf8591-library-0.0.1/setup.cfg` & `pcf8591-library-0.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6366 3835 3931 2d6c 6962 7261   = pcf8591-libra
 00000020: 7279 0d0a 7665 7273 696f 6e20 3d20 302e  ry..version = 0.
-00000030: 302e 310d 0a61 7574 686f 7220 3d20 5265  0.1..author = Re
+00000030: 302e 320d 0a61 7574 686f 7220 3d20 5265  0.2..author = Re
 00000040: 6e7a 6f20 4d69 7363 6869 616e 7469 0d0a  nzo Mischianti..
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 5043  description = PC
 00000060: 4638 3539 3120 6d69 6372 6f70 7974 686f  F8591 micropytho
 00000070: 6e20 6c69 6272 6172 7920 666f 7220 4172  n library for Ar
 00000080: 6475 696e 6f2c 2052 6173 7062 6572 7279  duino, Raspberry
 00000090: 2050 6920 5069 636f 2061 6e64 2072 7032   Pi Pico and rp2
 000000a0: 3034 3020 626f 6172 6473 2c20 6573 7033  040 boards, esp3
```

### Comparing `pcf8591-library-0.0.1/setup.py` & `pcf8591-library-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 sys.path.pop(0)
 from setuptools import setup
 
 setup(
     name="pcf8591-library",
     package_dir={'': 'src'},
     py_modules=["PCF8591"],
-    version="0.0.1",
+    version="0.0.2",
     description="PCF8591, library for Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266",
     long_description="Library to use pcf8591 i2c analog IC with Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266. Can read analog value and write analog value with only 2 wire. ",
     keywords="micropython, digital, i2c, expander, pcf8591, pcf8591a, esp32, esp8266, stm32, SAMD, Arduino, wire, rp2040, Raspberry",
     url="https://github.com/xreef/PCF8591_micropython_library",
     author="Renzo Mischianti",
     author_email="renzo.mischianti@gmail.com",
     maintainer="Renzo Mischianti",
```

### Comparing `pcf8591-library-0.0.1/src/pcf8591_library.egg-info/PKG-INFO` & `pcf8591-library-0.0.2/src/pcf8591_library.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcf8591-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library to use pcf8591 i2c analog IC with Arduino, Raspberry Pi Pico and rp2040 boards, esp32, SMT32 and ESP8266. Can read analog value and write analog value with only 2 wire. 
 Home-page: https://github.com/xreef/PCF8591_micropython_library
 Author: Renzo Mischianti
 Author-email: Renzo Mischianti <renzo@mischianti.org>
 Maintainer: Renzo Mischianti
 Maintainer-email: Renzo Mischianti <renzo@mischianti.org>
 License: The MIT License (MIT)
@@ -59,14 +59,15 @@
 
 #
 #### www.mischianti.org
 
 ### MicroPython Library to use i2c analog IC with arduino and esp8266. Can read analog value and write analog value with only 2 wire (perfect for ESP-01).
 
 #### Changelog
+ - 16/05/2023: v0.0.2 Minor fix on read and write [#Forum](https://www.mischianti.org/forums/topic/micropython-i2c-pcf8591-round-value-problem-raspberry-pi-pico/)
  - 18/04/2023: v0.0.1 Initial commit of stable version.
 
 I try to simplify the use of this IC, with a minimal set of operation.
 
 #### Installation
 To install the library execute the following command:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcf8591-library Version: 0.0.1 Summary: Library to
+Metadata-Version: 2.1 Name: pcf8591-library Version: 0.0.2 Summary: Library to
 use pcf8591 i2c analog IC with Arduino, Raspberry Pi Pico and rp2040 boards,
 esp32, SMT32 and ESP8266. Can read analog value and write analog value with
 only 2 wire. Home-page: https://github.com/xreef/PCF8591_micropython_library
 Author: Renzo Mischianti Author-email: Renzo Mischianti
 mischianti.org> Maintainer: Renzo Mischianti Maintainer-email: Renzo Mischianti
 mischianti.org> License: The MIT License (MIT) Copyright (c) 2017 Renzo
 Mischianti www.mischianti.org All right reserved. You may copy, alter and reuse
@@ -34,21 +34,23 @@
 Implementation :: MicroPython Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE.md
 [Support_forum_pcf8591_English]
 [Forum_supporto_pcf8591_italiano]
 # #### www.mischianti.org ### MicroPython Library to use i2c analog IC with
 arduino and esp8266. Can read analog value and write analog value with only 2
-wire (perfect for ESP-01). #### Changelog - 18/04/2023: v0.0.1 Initial commit
-of stable version. I try to simplify the use of this IC, with a minimal set of
-operation. #### Installation To install the library execute the following
-command: ```bash pip install pcf8591-library ``` **Constructor:** Pass the
-address of I2C ```python from PCF8591 import PCF8591 from machine import I2C,
-Pin # Initialize the I2C bus i2c = I2C(0, scl=Pin(22), sda=Pin(21)) #
-Initialize the PCF8591 pcf8591 = PCF8591(0x48, i2c) if pcf8591.begin(): print
+wire (perfect for ESP-01). #### Changelog - 16/05/2023: v0.0.2 Minor fix on
+read and write [#Forum](https://www.mischianti.org/forums/topic/micropython-
+i2c-pcf8591-round-value-problem-raspberry-pi-pico/) - 18/04/2023: v0.0.1
+Initial commit of stable version. I try to simplify the use of this IC, with a
+minimal set of operation. #### Installation To install the library execute the
+following command: ```bash pip install pcf8591-library ``` **Constructor:**
+Pass the address of I2C ```python from PCF8591 import PCF8591 from machine
+import I2C, Pin # Initialize the I2C bus i2c = I2C(0, scl=Pin(22), sda=Pin(21))
+# Initialize the PCF8591 pcf8591 = PCF8591(0x48, i2c) if pcf8591.begin(): print
 ("PCF8591 found") ``` or ```python from PCF8591 import PCF8591 pcf8591 =
 PCF8591(0x48, sda=21, scl=22) if pcf8591.begin(): print("PCF8591 found") ``` To
 read all analog input in one ```python # Main loop while True: # Read all
 analog input channels ain0, ain1, ain2, ain3 = pcf8591.analog_read_all() #
 Print the results print("AIN0:", ain0, "AIN1:", ain1, "AIN2:", ain2, "AIN3:",
 ain3) # Wait for 1 second utime.sleep(1) ``` If you want to read a single
 input: ```python print("AIN0 ", pcf8591.analog_read(PCF8591.AIN0)) print("AIN1
```

