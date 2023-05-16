# Comparing `tmp/maxtime-0.2.0-py3-none-win_amd64.whl.zip` & `tmp/maxtime-0.3.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 820570 bytes, number of entries: 4
--rw-r--r--  4.6 unx      682 b- defN 23-May-15 16:49 maxtime-0.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-May-15 16:49 maxtime-0.2.0.dist-info/WHEEL
--rwxr-xr-x  4.6 unx  2148352 b- defN 23-May-15 16:49 maxtime-0.2.0.data/scripts/maxtime.exe
--rw-r--r--  4.6 unx      303 b- defN 23-May-15 16:49 maxtime-0.2.0.dist-info/RECORD
-4 files, 2149431 bytes uncompressed, 819986 bytes compressed:  61.9%
+Zip file size: 820589 bytes, number of entries: 4
+-rw-r--r--  4.6 unx      695 b- defN 23-May-16 19:52 maxtime-0.3.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-May-16 19:52 maxtime-0.3.0.dist-info/WHEEL
+-rwxr-xr-x  4.6 unx  2148352 b- defN 23-May-16 19:52 maxtime-0.3.0.data/scripts/maxtime.exe
+-rw-r--r--  4.6 unx      303 b- defN 23-May-16 19:52 maxtime-0.3.0.dist-info/RECORD
+4 files, 2149444 bytes uncompressed, 820005 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: maxtime-0.2.0.dist-info/METADATA
+Filename: maxtime-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: maxtime-0.2.0.dist-info/WHEEL
+Filename: maxtime-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: maxtime-0.2.0.data/scripts/maxtime.exe
+Filename: maxtime-0.3.0.data/scripts/maxtime.exe
 Comment: 
 
-Filename: maxtime-0.2.0.dist-info/RECORD
+Filename: maxtime-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `maxtime-0.2.0.dist-info/METADATA` & `maxtime-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: maxtime
-Version: 0.2.0
+Version: 0.3.0
 Summary: Find the maximum mtime in a directory.
 Author: Tim Hutt <tdhutt@gmail.com>
 Author-email: Tim Hutt <tdhutt@gmail.com>
+License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 [![Build Status](https://github.com/timmmm/maxtime/actions/workflows/build.yml/badge.svg)](https://github.com/Timmmm/maxtime/actions/workflows/build.yml)
 
 # Maxtime
 
 This is a very simple tool to find the latest mtime of any file within a directory as fast as possible, but respecting `.gitignore` files.
```

## Comparing `maxtime-0.2.0.data/scripts/maxtime.exe` & `maxtime-0.3.0.data/scripts/maxtime.exe`

 * *Files 0% similar despite different names*

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014015b36c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon May 15 16:49:17 2023
+Time/Date		Tue May 16 19:52:55 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	35
 SizeOfCode		0000000000161200
 SizeOfInitializedData	00000000000ab600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000015b36c
@@ -2203,30 +2203,30 @@
  0000000140204d18:	00000001400b5e10 00000001400b5e39 00000001401ea424
  0000000140204d24:	00000001400b5e40 00000001400b5fb0 00000001401d5e34
  0000000140204d30:	00000001400b5fb0 00000001400b6048 00000001401ea480
  0000000140204d3c:	00000001400b6050 00000001400b6074 00000001401ea494
  0000000140204d48:	00000001400b6080 00000001400b60b9 00000001401ea4a0
  0000000140204d54:	00000001400b60d0 00000001400b613b 00000001401ea504
  0000000140204d60:	00000001400b6140 00000001400b616e 00000001401ea518
- 0000000140204d6c:	00000001400b6190 00000001400b61a5 00000001401d53b8
+ 0000000140204d6c:	00000001400b6180 00000001400b6195 00000001401d53b8
  0000000140204d78:	00000001400b6220 00000001400b62fd 00000001401d5474
  0000000140204d84:	00000001400b6300 00000001400b6342 00000001401d5428
  0000000140204d90:	00000001400b6350 00000001400b637f 00000001401d5474
  0000000140204d9c:	00000001400b6380 00000001400b66d0 00000001401ea568
  0000000140204da8:	00000001400b66d0 00000001400b66ee 00000001401ea588
- 0000000140204db4:	00000001400b66f0 00000001400b691b 00000001401ea5e4
- 0000000140204dc0:	00000001400b6920 00000001400b696d 00000001401ea604
- 0000000140204dcc:	00000001400b6970 00000001400b69b8 00000001401ea61c
- 0000000140204dd8:	00000001400b69c0 00000001400b69fd 00000001401d545c
+ 0000000140204db4:	00000001400b66f0 00000001400b672d 00000001401d545c
+ 0000000140204dc0:	00000001400b6730 00000001400b695b 00000001401ea5e4
+ 0000000140204dcc:	00000001400b6960 00000001400b69ad 00000001401ea604
+ 0000000140204dd8:	00000001400b69b0 00000001400b69f8 00000001401ea61c
  0000000140204de4:	00000001400b6a00 00000001400b6ad0 00000001401d5608
  0000000140204df0:	00000001400b6ad0 00000001400b6b78 00000001401ea684
- 0000000140204dfc:	00000001400b6bb0 00000001400b6bf3 00000001401d545c
- 0000000140204e08:	00000001400b6c00 00000001400b6c46 00000001401ea690
- 0000000140204e14:	00000001400b6c50 00000001400b6c70 00000001401ea6a4
- 0000000140204e20:	00000001400b6c70 00000001400b6c99 00000001401d545c
+ 0000000140204dfc:	00000001400b6bb0 00000001400b6bd9 00000001401d545c
+ 0000000140204e08:	00000001400b6be0 00000001400b6c23 00000001401d545c
+ 0000000140204e14:	00000001400b6c30 00000001400b6c76 00000001401ea690
+ 0000000140204e20:	00000001400b6c80 00000001400b6ca0 00000001401ea6a4
  0000000140204e2c:	00000001400b6d40 00000001400b6e02 00000001401ea6f8
  0000000140204e38:	00000001400b6e10 00000001400b6e30 00000001401ea70c
  0000000140204e44:	00000001400b6e30 00000001400b6e72 00000001401ea718
  0000000140204e50:	00000001400b6e80 00000001400b6f59 00000001401d53d0
  0000000140204e5c:	00000001400b6f80 00000001400b6fa0 00000001401d545c
  0000000140204e68:	00000001400b6fc0 00000001400b700f 00000001401d53ac
  0000000140204e74:	00000001400b7010 00000001400b7190 00000001401ea91c
@@ -4094,19 +4094,19 @@
  000000014020a5bc:	000000014015e3d0 000000014015e404 00000001401e2ebc
  000000014020a5c8:	000000014015e410 000000014015e441 00000001401dfaa4
  000000014020a5d4:	000000014015e450 000000014015ecb7 00000001401d5adc
  000000014020a5e0:	000000014015ecc0 000000014015ed82 00000001401d5608
  000000014020a5ec:	000000014015ed90 000000014015edc1 00000001401dfc68
  000000014020a5f8:	000000014015edd0 000000014015ee53 00000001401ea77c
  000000014020a604:	000000014015ee60 000000014015ee8d 00000001401ea794
- 000000014020a610:	000000014015ee90 000000014015ef5e 00000001401ea7e8
+ 000000014020a610:	000000014015ee90 000000014015ef52 00000001401ea7e8
  000000014020a61c:	000000014015ef60 000000014015ef81 00000001401ea7fc
  000000014020a628:	000000014015ef90 000000014015f052 00000001401ea84c
  000000014020a634:	000000014015f060 000000014015f081 00000001401ea860
- 000000014020a640:	000000014015f090 000000014015f152 00000001401ea8b0
+ 000000014020a640:	000000014015f090 000000014015f15e 00000001401ea8b0
  000000014020a64c:	000000014015f160 000000014015f181 00000001401ea8c4
  000000014020a658:	000000014015f190 000000014015f21b 00000001401ea914
  000000014020a664:	000000014015f220 000000014015f23f 00000001401dfaa4
  000000014020a670:	000000014015f240 000000014015f2a3 00000001401d53c0
  000000014020a67c:	000000014015f510 000000014015f577 00000001401d53c0
  000000014020a688:	000000014015f580 000000014015f5dc 00000001401d53c0
  000000014020a694:	000000014015f5e0 000000014015f6a3 00000001401d5608
@@ -29523,15 +29523,15 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 48 a5 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 50 a5 1e 00 28 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 40 61 0b 00
 	  030: d0 60 0b 00 ff ff ff ff fc 60 0b 00 00 00 00 00
 	  040: 02 61 0b 00 ff ff ff ff
- 00000001401d53b8 (rva: 001d53b8): 00000001400b6190 - 00000001400b61a5
+ 00000001401d53b8 (rva: 001d53b8): 00000001400b6180 - 00000001400b6195
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
  00000001401d5474 (rva: 001d5474): 00000001400b6220 - 00000001400b62fd
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: alloc large area: rsp = rsp - 0x88
@@ -29575,15 +29575,20 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 c4 a5 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 cc a5 1e 00 28 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff d0 66 0b 00
 	  030: 80 63 0b 00 ff ff ff ff 9d 66 0b 00 00 00 00 00
 	  040: b5 66 0b 00 ff ff ff ff
- 00000001401ea5e4 (rva: 001ea5e4): 00000001400b66f0 - 00000001400b691b
+ 00000001401d545c (rva: 001d545c): 00000001400b66f0 - 00000001400b672d
+	Version: 1, Flags: none
+	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
+	  pc+0x05: alloc small area: rsp = rsp - 0x20
+	  pc+0x01: push rsi
+ 00000001401ea5e4 (rva: 001ea5e4): 00000001400b6730 - 00000001400b695b
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 10, Prologue size: 0x15, Frame offset: 0x4, Frame reg: rbp
 	  pc+0x15: FPReg: rbp = rsp + 0x40 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x48
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rdi
 	  pc+0x0a: push rsi
@@ -29591,94 +29596,85 @@
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
 	Handler: 000000014015bb56.
 	User data:
 	  000: 34 a6 1e 00
- 00000001401ea604 (rva: 001ea604): 00000001400b6920 - 00000001400b696d
+ 00000001401ea604 (rva: 001ea604): 00000001400b6960 - 00000001400b69ad
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x19, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: alloc small area: rsp = rsp - 0x28
 	  pc+0x11: push rbx
 	  pc+0x10: push rdi
 	  pc+0x0f: push rsi
 	  pc+0x0e: push r12
 	  pc+0x0c: push r13
 	  pc+0x0a: push r14
 	  pc+0x08: push r15
 	  pc+0x06: push rbp
- 00000001401ea61c (rva: 001ea61c): 00000001400b6970 - 00000001400b69b8
+ 00000001401ea61c (rva: 001ea61c): 00000001400b69b0 - 00000001400b69f8
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x19, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: alloc small area: rsp = rsp - 0x28
 	  pc+0x11: push rbx
 	  pc+0x10: push rdi
 	  pc+0x0f: push rsi
 	  pc+0x0e: push r12
 	  pc+0x0c: push r13
 	  pc+0x0a: push r14
 	  pc+0x08: push r15
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 02 00 00 00 5c a6 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 6c a6 1e 00 40 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 70 69 0b 00
-	  030: 00 00 00 00 20 69 0b 00 f0 66 0b 00 ff ff ff ff
-	  040: 9b 68 0b 00 01 00 00 00 a4 68 0b 00 ff ff ff ff
- 00000001401d545c (rva: 001d545c): 00000001400b69c0 - 00000001400b69fd
-	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: alloc small area: rsp = rsp - 0x20
-	  pc+0x01: push rsi
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff b0 69 0b 00
+	  030: 00 00 00 00 60 69 0b 00 30 67 0b 00 ff ff ff ff
+	  040: db 68 0b 00 01 00 00 00 e4 68 0b 00 ff ff ff ff
  00000001401d5608 (rva: 001d5608): 00000001400b6a00 - 00000001400b6ad0
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x58
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
  00000001401ea684 (rva: 001ea684): 00000001400b6ad0 - 00000001400b6b78
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x70
 	  pc+0x03: push rbx
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
- 00000001401d545c (rva: 001d545c): 00000001400b6bb0 - 00000001400b6bf3
+ 00000001401d545c (rva: 001d545c): 00000001400b6bb0 - 00000001400b6bd9
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rsi
- 00000001401ea690 (rva: 001ea690): 00000001400b6c00 - 00000001400b6c46
+ 00000001401d545c also used for function at 00000001400b6be0
+ 00000001401ea690 (rva: 001ea690): 00000001400b6c30 - 00000001400b6c76
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0b, Frame offset: 0x3, Frame reg: rbp
 	  pc+0x0b: FPReg: rbp = rsp + 0x30 (info = 0x0)
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
 	Handler: 000000014015bb56.
 	User data:
 	  000: b0 a6 1e 00
- 00000001401ea6a4 (rva: 001ea6a4): 00000001400b6c50 - 00000001400b6c70
+ 00000001401ea6a4 (rva: 001ea6a4): 00000001400b6c80 - 00000001400b6ca0
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0b: alloc small area: rsp = rsp - 0x28
 	  pc+0x07: push rsi
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 d8 a6 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 e0 a6 1e 00 30 00 00 00
-	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 50 6c 0b 00
-	  030: 00 6c 0b 00 ff ff ff ff 28 6c 0b 00 00 00 00 00
-	  040: 2d 6c 0b 00 ff ff ff ff
- 00000001401d545c (rva: 001d545c): 00000001400b6c70 - 00000001400b6c99
-	Version: 1, Flags: none
-	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
-	  pc+0x05: alloc small area: rsp = rsp - 0x20
-	  pc+0x01: push rsi
+	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 80 6c 0b 00
+	  030: 30 6c 0b 00 ff ff ff ff 58 6c 0b 00 00 00 00 00
+	  040: 5d 6c 0b 00 ff ff ff ff
  00000001401ea6f8 (rva: 001ea6f8): 00000001400b6d40 - 00000001400b6e02
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0b, Frame offset: 0x4, Frame reg: rbp
 	  pc+0x0b: FPReg: rbp = rsp + 0x40 (info = 0x0)
 	  pc+0x06: alloc small area: rsp = rsp - 0x48
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
@@ -51796,15 +51792,15 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 c8 a7 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 d0 a7 1e 00 b0 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 60 ee 15 00
 	  030: d0 ed 15 00 ff ff ff ff 00 ee 15 00 00 00 00 00
 	  040: 49 ee 15 00 ff ff ff ff
- 00000001401ea7e8 (rva: 001ea7e8): 000000014015ee90 - 000000014015ef5e
+ 00000001401ea7e8 (rva: 001ea7e8): 000000014015ee90 - 000000014015ef52
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 3, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc small area: rsp = rsp - 0x80
 	  pc+0x01: push rbp
 	Handler: 000000014015bb56.
 	User data:
@@ -51814,16 +51810,16 @@
 	Nbr codes: 2, Prologue size: 0x11, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 2c a8 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 34 a8 1e 00 78 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 60 ef 15 00
-	  030: 90 ee 15 00 ff ff ff ff 4e ef 15 00 00 00 00 00
-	  040: 5d ef 15 00 ff ff ff ff
+	  030: 90 ee 15 00 ff ff ff ff 42 ef 15 00 00 00 00 00
+	  040: 51 ef 15 00 ff ff ff ff
  00000001401ea84c (rva: 001ea84c): 000000014015ef90 - 000000014015f052
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 3, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc small area: rsp = rsp - 0x80
 	  pc+0x01: push rbp
 	Handler: 000000014015bb56.
@@ -51836,15 +51832,15 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 90 a8 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 98 a8 1e 00 78 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 60 f0 15 00
 	  030: 90 ef 15 00 ff ff ff ff 42 f0 15 00 00 00 00 00
 	  040: 51 f0 15 00 ff ff ff ff
- 00000001401ea8b0 (rva: 001ea8b0): 000000014015f090 - 000000014015f152
+ 00000001401ea8b0 (rva: 001ea8b0): 000000014015f090 - 000000014015f15e
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 3, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc small area: rsp = rsp - 0x80
 	  pc+0x01: push rbp
 	Handler: 000000014015bb56.
 	User data:
@@ -51854,16 +51850,16 @@
 	Nbr codes: 2, Prologue size: 0x11, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 f4 a8 1e 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 fc a8 1e 00 78 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 60 f1 15 00
-	  030: 90 f0 15 00 ff ff ff ff 42 f1 15 00 00 00 00 00
-	  040: 51 f1 15 00 ff ff ff ff
+	  030: 90 f0 15 00 ff ff ff ff 4e f1 15 00 00 00 00 00
+	  040: 5d f1 15 00 ff ff ff ff
  00000001401ea914 (rva: 001ea914): 000000014015f190 - 000000014015f21b
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rsi
  00000001401dfaa4 (rva: 001dfaa4): 000000014015f220 - 000000014015f23f
 	Version: 1, Flags: none
@@ -239951,22 +239947,22 @@
    1400b4261:	call   *0xaf011(%rip)        # 0x140163278
    1400b4267:	mov    0x78(%r15),%rax
    1400b426b:	lock decq (%rax)
    1400b426f:	mov    %r15,-0x8(%rbp)
    1400b4273:	jne    0x1400b4282
    1400b4275:	mov    -0x8(%rbp),%rax
    1400b4279:	mov    0x78(%rax),%rcx
-   1400b427d:	call   0x1400b69c0
+   1400b427d:	call   0x1400b66f0
    1400b4282:	mov    -0x8(%rbp),%rax
    1400b4286:	mov    0x80(%rax),%rax
    1400b428d:	lock decq (%rax)
    1400b4291:	jne    0x1400b42a3
    1400b4293:	mov    -0x8(%rbp),%rax
    1400b4297:	mov    0x80(%rax),%rcx
-   1400b429e:	call   0x1400b66f0
+   1400b429e:	call   0x1400b6730
    1400b42a3:	mov    -0x8(%rbp),%rax
    1400b42a7:	mov    0x90(%rax),%rcx
    1400b42ae:	imul   $0x70,0x98(%rax),%rax
    1400b42b6:	mov    %rax,-0x10(%rbp)
    1400b42ba:	add    %rcx,%rax
    1400b42bd:	mov    %rax,-0x18(%rbp)
    1400b42c1:	data16 data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
@@ -241620,15 +241616,15 @@
    1400b599d:	int3
    1400b599e:	int3
    1400b599f:	int3
    1400b59a0:	mov    (%rcx),%rax
    1400b59a3:	lock decq (%rax)
    1400b59a7:	jne    0x1400b59b1
    1400b59a9:	mov    (%rcx),%rcx
-   1400b59ac:	jmp    0x1400b66f0
+   1400b59ac:	jmp    0x1400b6730
    1400b59b1:	ret
    1400b59b2:	int3
    1400b59b3:	int3
    1400b59b4:	int3
    1400b59b5:	int3
    1400b59b6:	int3
    1400b59b7:	int3
@@ -242273,81 +242269,81 @@
    1400b616f:	int3
    1400b6170:	lea    0xbe2f9(%rip),%rax        # 0x140174470
    1400b6177:	mov    $0x28,%edx
    1400b617c:	ret
    1400b617d:	int3
    1400b617e:	int3
    1400b617f:	int3
-   1400b6180:	lea    0x8(%rcx),%rax
-   1400b6184:	lea    0xbe85d(%rip),%rdx        # 0x1401749e8
-   1400b618b:	ret
-   1400b618c:	int3
-   1400b618d:	int3
-   1400b618e:	int3
-   1400b618f:	int3
-   1400b6190:	sub    $0x28,%rsp
-   1400b6194:	mov    (%rcx),%rax
-   1400b6197:	call   *0x8(%rax)
-   1400b619a:	mov    %rax,%rcx
-   1400b619d:	add    $0x28,%rsp
-   1400b61a1:	rex.W jmp *0x30(%rdx)
-   1400b61a5:	int3
-   1400b61a6:	int3
-   1400b61a7:	int3
-   1400b61a8:	int3
-   1400b61a9:	int3
-   1400b61aa:	int3
-   1400b61ab:	int3
+   1400b6180:	sub    $0x28,%rsp
+   1400b6184:	mov    (%rcx),%rax
+   1400b6187:	call   *0x8(%rax)
+   1400b618a:	mov    %rax,%rcx
+   1400b618d:	add    $0x28,%rsp
+   1400b6191:	rex.W jmp *0x30(%rdx)
+   1400b6195:	int3
+   1400b6196:	int3
+   1400b6197:	int3
+   1400b6198:	int3
+   1400b6199:	int3
+   1400b619a:	int3
+   1400b619b:	int3
+   1400b619c:	int3
+   1400b619d:	int3
+   1400b619e:	int3
+   1400b619f:	int3
+   1400b61a0:	lea    0x8(%rcx),%rax
+   1400b61a4:	lea    0xbe83d(%rip),%rdx        # 0x1401749e8
+   1400b61ab:	ret
    1400b61ac:	int3
    1400b61ad:	int3
    1400b61ae:	int3
    1400b61af:	int3
    1400b61b0:	movabs $0xfe13b116fa05e241,%rax
    1400b61ba:	ret
    1400b61bb:	int3
    1400b61bc:	int3
    1400b61bd:	int3
    1400b61be:	int3
    1400b61bf:	int3
-   1400b61c0:	movabs $0xc608023394b7e458,%rax
+   1400b61c0:	movabs $0x7e7ad0e78b585755,%rax
    1400b61ca:	ret
    1400b61cb:	int3
    1400b61cc:	int3
    1400b61cd:	int3
    1400b61ce:	int3
    1400b61cf:	int3
-   1400b61d0:	movabs $0xeb158e8aa62e55b0,%rax
+   1400b61d0:	movabs $0xc608023394b7e458,%rax
    1400b61da:	ret
    1400b61db:	int3
    1400b61dc:	int3
    1400b61dd:	int3
    1400b61de:	int3
    1400b61df:	int3
-   1400b61e0:	movabs $0xa74aae0519b3e2ba,%rax
+   1400b61e0:	movabs $0xf9f9c3c73610f9d9,%rax
    1400b61ea:	ret
    1400b61eb:	int3
    1400b61ec:	int3
    1400b61ed:	int3
    1400b61ee:	int3
    1400b61ef:	int3
-   1400b61f0:	movabs $0x7e7ad0e78b585755,%rax
+   1400b61f0:	movabs $0xeb158e8aa62e55b0,%rax
    1400b61fa:	ret
    1400b61fb:	int3
    1400b61fc:	int3
    1400b61fd:	int3
    1400b61fe:	int3
    1400b61ff:	int3
-   1400b6200:	movabs $0xf9f9c3c73610f9d9,%rax
+   1400b6200:	movabs $0x2896d79c8e65fb5b,%rax
    1400b620a:	ret
    1400b620b:	int3
    1400b620c:	int3
    1400b620d:	int3
    1400b620e:	int3
    1400b620f:	int3
-   1400b6210:	movabs $0x2896d79c8e65fb5b,%rax
+   1400b6210:	movabs $0xa74aae0519b3e2ba,%rax
    1400b621a:	ret
    1400b621b:	int3
    1400b621c:	int3
    1400b621d:	int3
    1400b621e:	int3
    1400b621f:	int3
    1400b6220:	push   %rsi
@@ -242668,248 +242664,248 @@
    1400b66de:	push   %rbx
    1400b66df:	sub    $0x20,%rsp
    1400b66e3:	lea    0x30(%rdx),%rbp
    1400b66e7:	call   0x1400041d0
    1400b66ec:	ud2
    1400b66ee:	int3
    1400b66ef:	int3
-   1400b66f0:	push   %rbp
-   1400b66f1:	push   %r15
-   1400b66f3:	push   %r14
-   1400b66f5:	push   %r13
-   1400b66f7:	push   %r12
-   1400b66f9:	push   %rsi
-   1400b66fa:	push   %rdi
-   1400b66fb:	push   %rbx
-   1400b66fc:	sub    $0x48,%rsp
-   1400b6700:	lea    0x40(%rsp),%rbp
-   1400b6705:	movq   $0xfffffffffffffffe,0x0(%rbp)
-   1400b670d:	mov    %rcx,%r13
-   1400b6710:	mov    0x40(%rcx),%rax
-   1400b6714:	test   %rax,%rax
-   1400b6717:	je     0x1400b67d3
-   1400b671d:	mov    0x38(%r13),%r12
-   1400b6721:	lea    (%rax,%rax,2),%r14
-   1400b6725:	shl    $0x4,%r14
-   1400b6729:	add    %r12,%r14
-   1400b672c:	mov    0xacb45(%rip),%r15        # 0x140163278
-   1400b6733:	jmp    0x1400b674c
-   1400b6735:	data16 cs nopw 0x0(%rax,%rax,1)
-   1400b6740:	mov    %rsi,%r12
-   1400b6743:	cmp    %r14,%rsi
-   1400b6746:	je     0x1400b67d3
-   1400b674c:	cmpq   $0x0,(%r12)
-   1400b6751:	je     0x1400b6764
-   1400b6753:	mov    0x8(%r12),%r8
-   1400b6758:	mov    0x147bf9(%rip),%rcx        # 0x1401fe358
-   1400b675f:	xor    %edx,%edx
-   1400b6761:	call   *%r15
-   1400b6764:	mov    0x28(%r12),%rax
-   1400b6769:	test   %rax,%rax
-   1400b676c:	je     0x1400b67b0
-   1400b676e:	mov    0x20(%r12),%rsi
-   1400b6773:	shl    $0x3,%rax
-   1400b6777:	lea    (%rax,%rax,2),%rdi
-   1400b677b:	xor    %ebx,%ebx
-   1400b677d:	jmp    0x1400b6789
-   1400b677f:	nop
-   1400b6780:	add    $0x18,%rbx
-   1400b6784:	cmp    %rbx,%rdi
-   1400b6787:	je     0x1400b67b0
-   1400b6789:	cmpq   $0x0,(%rsi,%rbx,1)
-   1400b678e:	je     0x1400b6780
-   1400b6790:	mov    0x8(%rsi,%rbx,1),%r8
-   1400b6795:	mov    0x147bbc(%rip),%rcx        # 0x1401fe358
-   1400b679c:	xor    %edx,%edx
-   1400b679e:	call   *%r15
-   1400b67a1:	jmp    0x1400b6780
-   1400b67a3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   1400b67b0:	lea    0x30(%r12),%rsi
-   1400b67b5:	cmpq   $0x0,0x18(%r12)
-   1400b67bb:	je     0x1400b6740
-   1400b67bd:	mov    0x20(%r12),%r8
-   1400b67c2:	mov    0x147b8f(%rip),%rcx        # 0x1401fe358
-   1400b67c9:	xor    %edx,%edx
-   1400b67cb:	call   *%r15
-   1400b67ce:	jmp    0x1400b6740
-   1400b67d3:	cmpq   $0x0,0x30(%r13)
-   1400b67d8:	je     0x1400b67ed
-   1400b67da:	mov    0x38(%r13),%r8
-   1400b67de:	mov    0x147b73(%rip),%rcx        # 0x1401fe358
-   1400b67e5:	xor    %edx,%edx
-   1400b67e7:	call   *0xaca8b(%rip)        # 0x140163278
-   1400b67ed:	mov    0x58(%r13),%rax
-   1400b67f1:	test   %rax,%rax
-   1400b67f4:	je     0x1400b6822
-   1400b67f6:	mov    0x50(%r13),%rcx
-   1400b67fa:	shl    $0x4,%rax
-   1400b67fe:	lea    (%rax,%rax,4),%rsi
-   1400b6802:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   1400b6810:	lea    0x50(%rcx),%rdi
-   1400b6814:	call   0x14009cde0
-   1400b6819:	mov    %rdi,%rcx
-   1400b681c:	add    $0xffffffffffffffb0,%rsi
-   1400b6820:	jne    0x1400b6810
-   1400b6822:	cmpq   $0x0,0x48(%r13)
-   1400b6827:	je     0x1400b683c
-   1400b6829:	mov    0x50(%r13),%r8
-   1400b682d:	mov    0x147b24(%rip),%rcx        # 0x1401fe358
-   1400b6834:	xor    %edx,%edx
-   1400b6836:	call   *0xaca3c(%rip)        # 0x140163278
-   1400b683c:	cmpq   $0x0,0x60(%r13)
-   1400b6841:	je     0x1400b6856
-   1400b6843:	mov    0x68(%r13),%r8
-   1400b6847:	mov    0x147b0a(%rip),%rcx        # 0x1401fe358
-   1400b684e:	xor    %edx,%edx
-   1400b6850:	call   *0xaca22(%rip)        # 0x140163278
-   1400b6856:	mov    0x20(%r13),%rcx
-   1400b685a:	mov    %r13,-0x10(%rbp)
-   1400b685e:	imul   $0x1b0,0x28(%r13),%rax
-   1400b6866:	mov    %rax,-0x8(%rbp)
-   1400b686a:	add    %rcx,%rax
-   1400b686d:	mov    %rax,-0x18(%rbp)
-   1400b6871:	data16 data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   1400b6880:	mov    -0x8(%rbp),%rax
-   1400b6884:	test   %rax,%rax
-   1400b6887:	je     0x1400b68a8
-   1400b6889:	lea    0x1b0(%rcx),%rsi
-   1400b6890:	add    $0xfffffffffffffe50,%rax
-   1400b6896:	mov    %rax,-0x8(%rbp)
-   1400b689a:	mov    %rsi,-0x20(%rbp)
-   1400b689e:	call   0x1400b4890
-   1400b68a3:	mov    %rsi,%rcx
-   1400b68a6:	jmp    0x1400b6880
-   1400b68a8:	mov    -0x10(%rbp),%rsi
-   1400b68ac:	cmpq   $0x0,0x18(%rsi)
-   1400b68b1:	je     0x1400b68c6
-   1400b68b3:	mov    0x20(%rsi),%r8
-   1400b68b7:	mov    0x147a9a(%rip),%rcx        # 0x1401fe358
-   1400b68be:	xor    %edx,%edx
-   1400b68c0:	call   *0xac9b2(%rip)        # 0x140163278
-   1400b68c6:	mov    0x78(%rsi),%rax
-   1400b68ca:	lock decq (%rax)
-   1400b68ce:	jne    0x1400b68d9
-   1400b68d0:	mov    0x78(%rsi),%rcx
-   1400b68d4:	call   0x14009e400
-   1400b68d9:	cmp    $0xffffffffffffffff,%rsi
-   1400b68dd:	je     0x1400b6909
-   1400b68df:	lock decq 0x8(%rsi)
-   1400b68e4:	jne    0x1400b6909
-   1400b68e6:	mov    0x147a6b(%rip),%rcx        # 0x1401fe358
-   1400b68ed:	xor    %edx,%edx
-   1400b68ef:	mov    %rsi,%r8
-   1400b68f2:	add    $0x48,%rsp
-   1400b68f6:	pop    %rbx
-   1400b68f7:	pop    %rdi
-   1400b68f8:	pop    %rsi
-   1400b68f9:	pop    %r12
-   1400b68fb:	pop    %r13
-   1400b68fd:	pop    %r14
-   1400b68ff:	pop    %r15
-   1400b6901:	pop    %rbp
-   1400b6902:	rex.W jmp *0xac96f(%rip)        # 0x140163278
-   1400b6909:	nop
-   1400b690a:	add    $0x48,%rsp
-   1400b690e:	pop    %rbx
-   1400b690f:	pop    %rdi
-   1400b6910:	pop    %rsi
-   1400b6911:	pop    %r12
-   1400b6913:	pop    %r13
-   1400b6915:	pop    %r14
-   1400b6917:	pop    %r15
-   1400b6919:	pop    %rbp
-   1400b691a:	ret
-   1400b691b:	nopl   0x0(%rax,%rax,1)
-   1400b6920:	mov    %rdx,0x10(%rsp)
-   1400b6925:	push   %rbp
-   1400b6926:	push   %r15
-   1400b6928:	push   %r14
-   1400b692a:	push   %r13
-   1400b692c:	push   %r12
-   1400b692e:	push   %rsi
-   1400b692f:	push   %rdi
-   1400b6930:	push   %rbx
-   1400b6931:	sub    $0x28,%rsp
-   1400b6935:	lea    0x40(%rdx),%rbp
-   1400b6939:	cmpq   $0x0,-0x8(%rbp)
-   1400b693e:	mov    -0x18(%rbp),%rsi
-   1400b6942:	mov    -0x20(%rbp),%rdi
-   1400b6946:	je     0x1400b695c
-   1400b6948:	mov    %rdi,%rcx
-   1400b694b:	call   0x1400b4890
-   1400b6950:	add    $0x1b0,%rdi
-   1400b6957:	cmp    %rsi,%rdi
-   1400b695a:	jne    0x1400b6948
-   1400b695c:	add    $0x28,%rsp
-   1400b6960:	pop    %rbx
-   1400b6961:	pop    %rdi
-   1400b6962:	pop    %rsi
-   1400b6963:	pop    %r12
-   1400b6965:	pop    %r13
-   1400b6967:	pop    %r14
-   1400b6969:	pop    %r15
-   1400b696b:	pop    %rbp
-   1400b696c:	ret
-   1400b696d:	nopl   (%rax)
-   1400b6970:	mov    %rdx,0x10(%rsp)
-   1400b6975:	push   %rbp
-   1400b6976:	push   %r15
-   1400b6978:	push   %r14
-   1400b697a:	push   %r13
-   1400b697c:	push   %r12
-   1400b697e:	push   %rsi
-   1400b697f:	push   %rdi
-   1400b6980:	push   %rbx
-   1400b6981:	sub    $0x28,%rsp
-   1400b6985:	lea    0x40(%rdx),%rbp
-   1400b6989:	mov    -0x10(%rbp),%rsi
-   1400b698d:	mov    0x18(%rsi),%rcx
-   1400b6991:	mov    0x20(%rsi),%rdx
-   1400b6995:	call   0x140003980
-   1400b699a:	add    $0x78,%rsi
-   1400b699e:	mov    %rsi,%rcx
-   1400b69a1:	call   0x1400998e0
-   1400b69a6:	nop
-   1400b69a7:	add    $0x28,%rsp
-   1400b69ab:	pop    %rbx
-   1400b69ac:	pop    %rdi
-   1400b69ad:	pop    %rsi
-   1400b69ae:	pop    %r12
-   1400b69b0:	pop    %r13
-   1400b69b2:	pop    %r14
-   1400b69b4:	pop    %r15
-   1400b69b6:	pop    %rbp
-   1400b69b7:	ret
-   1400b69b8:	int3
-   1400b69b9:	int3
-   1400b69ba:	int3
-   1400b69bb:	int3
-   1400b69bc:	int3
-   1400b69bd:	int3
-   1400b69be:	int3
-   1400b69bf:	int3
-   1400b69c0:	push   %rsi
-   1400b69c1:	sub    $0x20,%rsp
-   1400b69c5:	mov    %rcx,%rsi
-   1400b69c8:	add    $0x10,%rcx
-   1400b69cc:	call   0x1400b46e0
-   1400b69d1:	cmp    $0xffffffffffffffff,%rsi
-   1400b69d5:	je     0x1400b69f6
-   1400b69d7:	lock decq 0x8(%rsi)
-   1400b69dc:	jne    0x1400b69f6
-   1400b69de:	mov    0x147973(%rip),%rcx        # 0x1401fe358
-   1400b69e5:	xor    %edx,%edx
-   1400b69e7:	mov    %rsi,%r8
-   1400b69ea:	add    $0x20,%rsp
-   1400b69ee:	pop    %rsi
-   1400b69ef:	rex.W jmp *0xac882(%rip)        # 0x140163278
-   1400b69f6:	nop
-   1400b69f7:	add    $0x20,%rsp
-   1400b69fb:	pop    %rsi
-   1400b69fc:	ret
+   1400b66f0:	push   %rsi
+   1400b66f1:	sub    $0x20,%rsp
+   1400b66f5:	mov    %rcx,%rsi
+   1400b66f8:	add    $0x10,%rcx
+   1400b66fc:	call   0x1400b46e0
+   1400b6701:	cmp    $0xffffffffffffffff,%rsi
+   1400b6705:	je     0x1400b6726
+   1400b6707:	lock decq 0x8(%rsi)
+   1400b670c:	jne    0x1400b6726
+   1400b670e:	mov    0x147c43(%rip),%rcx        # 0x1401fe358
+   1400b6715:	xor    %edx,%edx
+   1400b6717:	mov    %rsi,%r8
+   1400b671a:	add    $0x20,%rsp
+   1400b671e:	pop    %rsi
+   1400b671f:	rex.W jmp *0xacb52(%rip)        # 0x140163278
+   1400b6726:	nop
+   1400b6727:	add    $0x20,%rsp
+   1400b672b:	pop    %rsi
+   1400b672c:	ret
+   1400b672d:	int3
+   1400b672e:	int3
+   1400b672f:	int3
+   1400b6730:	push   %rbp
+   1400b6731:	push   %r15
+   1400b6733:	push   %r14
+   1400b6735:	push   %r13
+   1400b6737:	push   %r12
+   1400b6739:	push   %rsi
+   1400b673a:	push   %rdi
+   1400b673b:	push   %rbx
+   1400b673c:	sub    $0x48,%rsp
+   1400b6740:	lea    0x40(%rsp),%rbp
+   1400b6745:	movq   $0xfffffffffffffffe,0x0(%rbp)
+   1400b674d:	mov    %rcx,%r13
+   1400b6750:	mov    0x40(%rcx),%rax
+   1400b6754:	test   %rax,%rax
+   1400b6757:	je     0x1400b6813
+   1400b675d:	mov    0x38(%r13),%r12
+   1400b6761:	lea    (%rax,%rax,2),%r14
+   1400b6765:	shl    $0x4,%r14
+   1400b6769:	add    %r12,%r14
+   1400b676c:	mov    0xacb05(%rip),%r15        # 0x140163278
+   1400b6773:	jmp    0x1400b678c
+   1400b6775:	data16 cs nopw 0x0(%rax,%rax,1)
+   1400b6780:	mov    %rsi,%r12
+   1400b6783:	cmp    %r14,%rsi
+   1400b6786:	je     0x1400b6813
+   1400b678c:	cmpq   $0x0,(%r12)
+   1400b6791:	je     0x1400b67a4
+   1400b6793:	mov    0x8(%r12),%r8
+   1400b6798:	mov    0x147bb9(%rip),%rcx        # 0x1401fe358
+   1400b679f:	xor    %edx,%edx
+   1400b67a1:	call   *%r15
+   1400b67a4:	mov    0x28(%r12),%rax
+   1400b67a9:	test   %rax,%rax
+   1400b67ac:	je     0x1400b67f0
+   1400b67ae:	mov    0x20(%r12),%rsi
+   1400b67b3:	shl    $0x3,%rax
+   1400b67b7:	lea    (%rax,%rax,2),%rdi
+   1400b67bb:	xor    %ebx,%ebx
+   1400b67bd:	jmp    0x1400b67c9
+   1400b67bf:	nop
+   1400b67c0:	add    $0x18,%rbx
+   1400b67c4:	cmp    %rbx,%rdi
+   1400b67c7:	je     0x1400b67f0
+   1400b67c9:	cmpq   $0x0,(%rsi,%rbx,1)
+   1400b67ce:	je     0x1400b67c0
+   1400b67d0:	mov    0x8(%rsi,%rbx,1),%r8
+   1400b67d5:	mov    0x147b7c(%rip),%rcx        # 0x1401fe358
+   1400b67dc:	xor    %edx,%edx
+   1400b67de:	call   *%r15
+   1400b67e1:	jmp    0x1400b67c0
+   1400b67e3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   1400b67f0:	lea    0x30(%r12),%rsi
+   1400b67f5:	cmpq   $0x0,0x18(%r12)
+   1400b67fb:	je     0x1400b6780
+   1400b67fd:	mov    0x20(%r12),%r8
+   1400b6802:	mov    0x147b4f(%rip),%rcx        # 0x1401fe358
+   1400b6809:	xor    %edx,%edx
+   1400b680b:	call   *%r15
+   1400b680e:	jmp    0x1400b6780
+   1400b6813:	cmpq   $0x0,0x30(%r13)
+   1400b6818:	je     0x1400b682d
+   1400b681a:	mov    0x38(%r13),%r8
+   1400b681e:	mov    0x147b33(%rip),%rcx        # 0x1401fe358
+   1400b6825:	xor    %edx,%edx
+   1400b6827:	call   *0xaca4b(%rip)        # 0x140163278
+   1400b682d:	mov    0x58(%r13),%rax
+   1400b6831:	test   %rax,%rax
+   1400b6834:	je     0x1400b6862
+   1400b6836:	mov    0x50(%r13),%rcx
+   1400b683a:	shl    $0x4,%rax
+   1400b683e:	lea    (%rax,%rax,4),%rsi
+   1400b6842:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   1400b6850:	lea    0x50(%rcx),%rdi
+   1400b6854:	call   0x14009cde0
+   1400b6859:	mov    %rdi,%rcx
+   1400b685c:	add    $0xffffffffffffffb0,%rsi
+   1400b6860:	jne    0x1400b6850
+   1400b6862:	cmpq   $0x0,0x48(%r13)
+   1400b6867:	je     0x1400b687c
+   1400b6869:	mov    0x50(%r13),%r8
+   1400b686d:	mov    0x147ae4(%rip),%rcx        # 0x1401fe358
+   1400b6874:	xor    %edx,%edx
+   1400b6876:	call   *0xac9fc(%rip)        # 0x140163278
+   1400b687c:	cmpq   $0x0,0x60(%r13)
+   1400b6881:	je     0x1400b6896
+   1400b6883:	mov    0x68(%r13),%r8
+   1400b6887:	mov    0x147aca(%rip),%rcx        # 0x1401fe358
+   1400b688e:	xor    %edx,%edx
+   1400b6890:	call   *0xac9e2(%rip)        # 0x140163278
+   1400b6896:	mov    0x20(%r13),%rcx
+   1400b689a:	mov    %r13,-0x10(%rbp)
+   1400b689e:	imul   $0x1b0,0x28(%r13),%rax
+   1400b68a6:	mov    %rax,-0x8(%rbp)
+   1400b68aa:	add    %rcx,%rax
+   1400b68ad:	mov    %rax,-0x18(%rbp)
+   1400b68b1:	data16 data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   1400b68c0:	mov    -0x8(%rbp),%rax
+   1400b68c4:	test   %rax,%rax
+   1400b68c7:	je     0x1400b68e8
+   1400b68c9:	lea    0x1b0(%rcx),%rsi
+   1400b68d0:	add    $0xfffffffffffffe50,%rax
+   1400b68d6:	mov    %rax,-0x8(%rbp)
+   1400b68da:	mov    %rsi,-0x20(%rbp)
+   1400b68de:	call   0x1400b4890
+   1400b68e3:	mov    %rsi,%rcx
+   1400b68e6:	jmp    0x1400b68c0
+   1400b68e8:	mov    -0x10(%rbp),%rsi
+   1400b68ec:	cmpq   $0x0,0x18(%rsi)
+   1400b68f1:	je     0x1400b6906
+   1400b68f3:	mov    0x20(%rsi),%r8
+   1400b68f7:	mov    0x147a5a(%rip),%rcx        # 0x1401fe358
+   1400b68fe:	xor    %edx,%edx
+   1400b6900:	call   *0xac972(%rip)        # 0x140163278
+   1400b6906:	mov    0x78(%rsi),%rax
+   1400b690a:	lock decq (%rax)
+   1400b690e:	jne    0x1400b6919
+   1400b6910:	mov    0x78(%rsi),%rcx
+   1400b6914:	call   0x14009e400
+   1400b6919:	cmp    $0xffffffffffffffff,%rsi
+   1400b691d:	je     0x1400b6949
+   1400b691f:	lock decq 0x8(%rsi)
+   1400b6924:	jne    0x1400b6949
+   1400b6926:	mov    0x147a2b(%rip),%rcx        # 0x1401fe358
+   1400b692d:	xor    %edx,%edx
+   1400b692f:	mov    %rsi,%r8
+   1400b6932:	add    $0x48,%rsp
+   1400b6936:	pop    %rbx
+   1400b6937:	pop    %rdi
+   1400b6938:	pop    %rsi
+   1400b6939:	pop    %r12
+   1400b693b:	pop    %r13
+   1400b693d:	pop    %r14
+   1400b693f:	pop    %r15
+   1400b6941:	pop    %rbp
+   1400b6942:	rex.W jmp *0xac92f(%rip)        # 0x140163278
+   1400b6949:	nop
+   1400b694a:	add    $0x48,%rsp
+   1400b694e:	pop    %rbx
+   1400b694f:	pop    %rdi
+   1400b6950:	pop    %rsi
+   1400b6951:	pop    %r12
+   1400b6953:	pop    %r13
+   1400b6955:	pop    %r14
+   1400b6957:	pop    %r15
+   1400b6959:	pop    %rbp
+   1400b695a:	ret
+   1400b695b:	nopl   0x0(%rax,%rax,1)
+   1400b6960:	mov    %rdx,0x10(%rsp)
+   1400b6965:	push   %rbp
+   1400b6966:	push   %r15
+   1400b6968:	push   %r14
+   1400b696a:	push   %r13
+   1400b696c:	push   %r12
+   1400b696e:	push   %rsi
+   1400b696f:	push   %rdi
+   1400b6970:	push   %rbx
+   1400b6971:	sub    $0x28,%rsp
+   1400b6975:	lea    0x40(%rdx),%rbp
+   1400b6979:	cmpq   $0x0,-0x8(%rbp)
+   1400b697e:	mov    -0x18(%rbp),%rsi
+   1400b6982:	mov    -0x20(%rbp),%rdi
+   1400b6986:	je     0x1400b699c
+   1400b6988:	mov    %rdi,%rcx
+   1400b698b:	call   0x1400b4890
+   1400b6990:	add    $0x1b0,%rdi
+   1400b6997:	cmp    %rsi,%rdi
+   1400b699a:	jne    0x1400b6988
+   1400b699c:	add    $0x28,%rsp
+   1400b69a0:	pop    %rbx
+   1400b69a1:	pop    %rdi
+   1400b69a2:	pop    %rsi
+   1400b69a3:	pop    %r12
+   1400b69a5:	pop    %r13
+   1400b69a7:	pop    %r14
+   1400b69a9:	pop    %r15
+   1400b69ab:	pop    %rbp
+   1400b69ac:	ret
+   1400b69ad:	nopl   (%rax)
+   1400b69b0:	mov    %rdx,0x10(%rsp)
+   1400b69b5:	push   %rbp
+   1400b69b6:	push   %r15
+   1400b69b8:	push   %r14
+   1400b69ba:	push   %r13
+   1400b69bc:	push   %r12
+   1400b69be:	push   %rsi
+   1400b69bf:	push   %rdi
+   1400b69c0:	push   %rbx
+   1400b69c1:	sub    $0x28,%rsp
+   1400b69c5:	lea    0x40(%rdx),%rbp
+   1400b69c9:	mov    -0x10(%rbp),%rsi
+   1400b69cd:	mov    0x18(%rsi),%rcx
+   1400b69d1:	mov    0x20(%rsi),%rdx
+   1400b69d5:	call   0x140003980
+   1400b69da:	add    $0x78,%rsi
+   1400b69de:	mov    %rsi,%rcx
+   1400b69e1:	call   0x1400998e0
+   1400b69e6:	nop
+   1400b69e7:	add    $0x28,%rsp
+   1400b69eb:	pop    %rbx
+   1400b69ec:	pop    %rdi
+   1400b69ed:	pop    %rsi
+   1400b69ee:	pop    %r12
+   1400b69f0:	pop    %r13
+   1400b69f2:	pop    %r14
+   1400b69f4:	pop    %r15
+   1400b69f6:	pop    %rbp
+   1400b69f7:	ret
+   1400b69f8:	int3
+   1400b69f9:	int3
+   1400b69fa:	int3
+   1400b69fb:	int3
+   1400b69fc:	int3
    1400b69fd:	int3
    1400b69fe:	int3
    1400b69ff:	int3
    1400b6a00:	push   %rsi
    1400b6a01:	push   %rdi
    1400b6a02:	sub    $0x58,%rsp
    1400b6a06:	inc    %rdx
@@ -243035,88 +243031,88 @@
    1400b6bae:	int3
    1400b6baf:	int3
    1400b6bb0:	push   %rsi
    1400b6bb1:	sub    $0x20,%rsp
    1400b6bb5:	mov    %rcx,%rsi
    1400b6bb8:	add    $0x8,%rcx
    1400b6bbc:	call   0x1400b5e40
-   1400b6bc1:	cmpq   $0x0,0x40(%rsi)
-   1400b6bc6:	je     0x1400b6bdb
-   1400b6bc8:	mov    0x48(%rsi),%r8
-   1400b6bcc:	mov    0x147785(%rip),%rcx        # 0x1401fe358
-   1400b6bd3:	xor    %edx,%edx
-   1400b6bd5:	call   *0xac69d(%rip)        # 0x140163278
-   1400b6bdb:	mov    0x147776(%rip),%rcx        # 0x1401fe358
-   1400b6be2:	xor    %edx,%edx
-   1400b6be4:	mov    %rsi,%r8
-   1400b6be7:	add    $0x20,%rsp
-   1400b6beb:	pop    %rsi
-   1400b6bec:	rex.W jmp *0xac685(%rip)        # 0x140163278
-   1400b6bf3:	int3
-   1400b6bf4:	int3
-   1400b6bf5:	int3
-   1400b6bf6:	int3
-   1400b6bf7:	int3
-   1400b6bf8:	int3
-   1400b6bf9:	int3
-   1400b6bfa:	int3
-   1400b6bfb:	int3
-   1400b6bfc:	int3
-   1400b6bfd:	int3
-   1400b6bfe:	int3
-   1400b6bff:	int3
-   1400b6c00:	push   %rbp
-   1400b6c01:	push   %rsi
-   1400b6c02:	sub    $0x38,%rsp
-   1400b6c06:	lea    0x30(%rsp),%rbp
-   1400b6c0b:	movq   $0xfffffffffffffffe,0x0(%rbp)
-   1400b6c13:	mov    %rcx,%rsi
-   1400b6c16:	add    $0x8,%rcx
-   1400b6c1a:	call   0x1400b5e40
-   1400b6c1f:	mov    %rsi,-0x8(%rbp)
-   1400b6c23:	lea    0x40(%rsi),%rcx
-   1400b6c27:	call   0x1400b5fb0
-   1400b6c2c:	mov    0x147725(%rip),%rcx        # 0x1401fe358
-   1400b6c33:	xor    %edx,%edx
-   1400b6c35:	mov    -0x8(%rbp),%r8
-   1400b6c39:	add    $0x38,%rsp
-   1400b6c3d:	pop    %rsi
-   1400b6c3e:	pop    %rbp
-   1400b6c3f:	rex.W jmp *0xac632(%rip)        # 0x140163278
-   1400b6c46:	cs nopw 0x0(%rax,%rax,1)
-   1400b6c50:	mov    %rdx,0x10(%rsp)
-   1400b6c55:	push   %rbp
-   1400b6c56:	push   %rsi
-   1400b6c57:	sub    $0x28,%rsp
-   1400b6c5b:	lea    0x30(%rdx),%rbp
-   1400b6c5f:	mov    -0x8(%rbp),%rcx
-   1400b6c63:	call   0x140003a30
-   1400b6c68:	nop
-   1400b6c69:	add    $0x28,%rsp
+   1400b6bc1:	mov    0x147790(%rip),%rcx        # 0x1401fe358
+   1400b6bc8:	xor    %edx,%edx
+   1400b6bca:	mov    %rsi,%r8
+   1400b6bcd:	add    $0x20,%rsp
+   1400b6bd1:	pop    %rsi
+   1400b6bd2:	rex.W jmp *0xac69f(%rip)        # 0x140163278
+   1400b6bd9:	int3
+   1400b6bda:	int3
+   1400b6bdb:	int3
+   1400b6bdc:	int3
+   1400b6bdd:	int3
+   1400b6bde:	int3
+   1400b6bdf:	int3
+   1400b6be0:	push   %rsi
+   1400b6be1:	sub    $0x20,%rsp
+   1400b6be5:	mov    %rcx,%rsi
+   1400b6be8:	add    $0x8,%rcx
+   1400b6bec:	call   0x1400b5e40
+   1400b6bf1:	cmpq   $0x0,0x40(%rsi)
+   1400b6bf6:	je     0x1400b6c0b
+   1400b6bf8:	mov    0x48(%rsi),%r8
+   1400b6bfc:	mov    0x147755(%rip),%rcx        # 0x1401fe358
+   1400b6c03:	xor    %edx,%edx
+   1400b6c05:	call   *0xac66d(%rip)        # 0x140163278
+   1400b6c0b:	mov    0x147746(%rip),%rcx        # 0x1401fe358
+   1400b6c12:	xor    %edx,%edx
+   1400b6c14:	mov    %rsi,%r8
+   1400b6c17:	add    $0x20,%rsp
+   1400b6c1b:	pop    %rsi
+   1400b6c1c:	rex.W jmp *0xac655(%rip)        # 0x140163278
+   1400b6c23:	int3
+   1400b6c24:	int3
+   1400b6c25:	int3
+   1400b6c26:	int3
+   1400b6c27:	int3
+   1400b6c28:	int3
+   1400b6c29:	int3
+   1400b6c2a:	int3
+   1400b6c2b:	int3
+   1400b6c2c:	int3
+   1400b6c2d:	int3
+   1400b6c2e:	int3
+   1400b6c2f:	int3
+   1400b6c30:	push   %rbp
+   1400b6c31:	push   %rsi
+   1400b6c32:	sub    $0x38,%rsp
+   1400b6c36:	lea    0x30(%rsp),%rbp
+   1400b6c3b:	movq   $0xfffffffffffffffe,0x0(%rbp)
+   1400b6c43:	mov    %rcx,%rsi
+   1400b6c46:	add    $0x8,%rcx
+   1400b6c4a:	call   0x1400b5e40
+   1400b6c4f:	mov    %rsi,-0x8(%rbp)
+   1400b6c53:	lea    0x40(%rsi),%rcx
+   1400b6c57:	call   0x1400b5fb0
+   1400b6c5c:	mov    0x1476f5(%rip),%rcx        # 0x1401fe358
+   1400b6c63:	xor    %edx,%edx
+   1400b6c65:	mov    -0x8(%rbp),%r8
+   1400b6c69:	add    $0x38,%rsp
    1400b6c6d:	pop    %rsi
    1400b6c6e:	pop    %rbp
-   1400b6c6f:	ret
-   1400b6c70:	push   %rsi
-   1400b6c71:	sub    $0x20,%rsp
-   1400b6c75:	mov    %rcx,%rsi
-   1400b6c78:	add    $0x8,%rcx
-   1400b6c7c:	call   0x1400b5e40
-   1400b6c81:	mov    0x1476d0(%rip),%rcx        # 0x1401fe358
-   1400b6c88:	xor    %edx,%edx
-   1400b6c8a:	mov    %rsi,%r8
-   1400b6c8d:	add    $0x20,%rsp
-   1400b6c91:	pop    %rsi
-   1400b6c92:	rex.W jmp *0xac5df(%rip)        # 0x140163278
-   1400b6c99:	int3
-   1400b6c9a:	int3
-   1400b6c9b:	int3
-   1400b6c9c:	int3
-   1400b6c9d:	int3
-   1400b6c9e:	int3
-   1400b6c9f:	int3
+   1400b6c6f:	rex.W jmp *0xac602(%rip)        # 0x140163278
+   1400b6c76:	cs nopw 0x0(%rax,%rax,1)
+   1400b6c80:	mov    %rdx,0x10(%rsp)
+   1400b6c85:	push   %rbp
+   1400b6c86:	push   %rsi
+   1400b6c87:	sub    $0x28,%rsp
+   1400b6c8b:	lea    0x30(%rdx),%rbp
+   1400b6c8f:	mov    -0x8(%rbp),%rcx
+   1400b6c93:	call   0x140003a30
+   1400b6c98:	nop
+   1400b6c99:	add    $0x28,%rsp
+   1400b6c9d:	pop    %rsi
+   1400b6c9e:	pop    %rbp
+   1400b6c9f:	ret
    1400b6ca0:	mov    %rcx,%rax
    1400b6ca3:	lea    0xbdaee(%rip),%rdx        # 0x140174798
    1400b6caa:	ret
    1400b6cab:	int3
    1400b6cac:	int3
    1400b6cad:	int3
    1400b6cae:	int3
@@ -420264,15 +420260,15 @@
    14015ed9a:	mov    %rcx,%rdi
    14015ed9d:	lea    0x28(%rsp),%rbx
    14015eda2:	mov    %rbx,%rcx
    14015eda5:	call   0x14003f300
    14015edaa:	mov    %rdi,%rcx
    14015edad:	mov    %rsi,%rdx
    14015edb0:	mov    %rbx,%r8
-   14015edb3:	call   0x14015f090
+   14015edb3:	call   0x14015ee90
    14015edb8:	nop
    14015edb9:	add    $0x60,%rsp
    14015edbd:	pop    %rbx
    14015edbe:	pop    %rdi
    14015edbf:	pop    %rsi
    14015edc0:	ret
    14015edc1:	int3
@@ -420314,15 +420310,15 @@
    14015ee28:	mov    0x10(%rsi),%rax
    14015ee2c:	mov    %rax,-0x10(%rbp)
    14015ee30:	movups (%rsi),%xmm0
    14015ee33:	movaps %xmm0,-0x20(%rbp)
    14015ee37:	movb   $0x0,0x2f(%rbp)
    14015ee3b:	lea    -0x20(%rbp),%rcx
    14015ee3f:	lea    -0x60(%rbp),%rdx
-   14015ee43:	call   0x14015ee90
+   14015ee43:	call   0x14015f090
    14015ee48:	nop
    14015ee49:	add    $0xb8,%rsp
    14015ee50:	pop    %rsi
    14015ee51:	pop    %rbp
    14015ee52:	ret
    14015ee53:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
    14015ee60:	mov    %rdx,0x10(%rsp)
@@ -420343,67 +420339,63 @@
    14015ee8d:	int3
    14015ee8e:	int3
    14015ee8f:	int3
    14015ee90:	push   %rbp
    14015ee91:	sub    $0x80,%rsp
    14015ee98:	lea    0x80(%rsp),%rbp
    14015eea0:	movq   $0xfffffffffffffffe,-0x8(%rbp)
-   14015eea8:	lea    0x15a61(%rip),%rax        # 0x140174910
-   14015eeaf:	mov    %rax,-0x60(%rbp)
-   14015eeb3:	movups (%rdx),%xmm0
-   14015eeb6:	movups 0x10(%rdx),%xmm1
-   14015eeba:	movups 0x20(%rdx),%xmm2
-   14015eebe:	movups %xmm0,-0x58(%rbp)
-   14015eec2:	movups %xmm1,-0x48(%rbp)
-   14015eec6:	movups %xmm2,-0x38(%rbp)
-   14015eeca:	mov    0x30(%rdx),%rax
-   14015eece:	mov    %rax,-0x28(%rbp)
-   14015eed2:	movups (%rcx),%xmm0
-   14015eed5:	movups %xmm0,-0x20(%rbp)
-   14015eed9:	mov    0x10(%rcx),%rax
-   14015eedd:	mov    %rax,-0x10(%rbp)
-   14015eee1:	mov    0x9f470(%rip),%rcx        # 0x1401fe358
-   14015eee8:	test   %rcx,%rcx
-   14015eeeb:	jne    0x14015ef02
-   14015eeed:	call   *0x43cd(%rip)        # 0x1401632c0
-   14015eef3:	test   %rax,%rax
-   14015eef6:	je     0x14015ef4d
-   14015eef8:	mov    %rax,%rcx
-   14015eefb:	mov    %rax,0x9f456(%rip)        # 0x1401fe358
-   14015ef02:	mov    $0x58,%r8d
-   14015ef08:	xor    %edx,%edx
-   14015ef0a:	call   *0x43d8(%rip)        # 0x1401632e8
-   14015ef10:	test   %rax,%rax
-   14015ef13:	je     0x14015ef4d
-   14015ef15:	mov    -0x10(%rbp),%rcx
-   14015ef19:	mov    %rcx,0x50(%rax)
-   14015ef1d:	movups -0x20(%rbp),%xmm0
-   14015ef21:	movups %xmm0,0x40(%rax)
-   14015ef25:	movups -0x60(%rbp),%xmm0
-   14015ef29:	movups -0x50(%rbp),%xmm1
-   14015ef2d:	movups -0x40(%rbp),%xmm2
-   14015ef31:	movups -0x30(%rbp),%xmm3
-   14015ef35:	movups %xmm3,0x30(%rax)
-   14015ef39:	movups %xmm2,0x20(%rax)
-   14015ef3d:	movups %xmm1,0x10(%rax)
-   14015ef41:	movups %xmm0,(%rax)
-   14015ef44:	add    $0x80,%rsp
-   14015ef4b:	pop    %rbp
-   14015ef4c:	ret
-   14015ef4d:	mov    $0x58,%ecx
-   14015ef52:	mov    $0x8,%edx
-   14015ef57:	call   0x14015c420
-   14015ef5c:	ud2
-   14015ef5e:	xchg   %ax,%ax
+   14015eea8:	lea    0x15a31(%rip),%rax        # 0x1401748e0
+   14015eeaf:	mov    %rax,-0x58(%rbp)
+   14015eeb3:	movups (%r8),%xmm0
+   14015eeb7:	movups 0x10(%r8),%xmm1
+   14015eebc:	movups 0x20(%r8),%xmm2
+   14015eec1:	movups %xmm0,-0x50(%rbp)
+   14015eec5:	movups %xmm1,-0x40(%rbp)
+   14015eec9:	movups %xmm2,-0x30(%rbp)
+   14015eecd:	mov    0x30(%r8),%rax
+   14015eed1:	mov    %rax,-0x20(%rbp)
+   14015eed5:	mov    %rcx,-0x18(%rbp)
+   14015eed9:	mov    %rdx,-0x10(%rbp)
+   14015eedd:	mov    0x9f474(%rip),%rcx        # 0x1401fe358
+   14015eee4:	test   %rcx,%rcx
+   14015eee7:	jne    0x14015eefe
+   14015eee9:	call   *0x43d1(%rip)        # 0x1401632c0
+   14015eeef:	test   %rax,%rax
+   14015eef2:	je     0x14015ef41
+   14015eef4:	mov    %rax,%rcx
+   14015eef7:	mov    %rax,0x9f45a(%rip)        # 0x1401fe358
+   14015eefe:	mov    $0x50,%r8d
+   14015ef04:	xor    %edx,%edx
+   14015ef06:	call   *0x43dc(%rip)        # 0x1401632e8
+   14015ef0c:	test   %rax,%rax
+   14015ef0f:	je     0x14015ef41
+   14015ef11:	movups -0x18(%rbp),%xmm0
+   14015ef15:	movups %xmm0,0x40(%rax)
+   14015ef19:	movups -0x58(%rbp),%xmm0
+   14015ef1d:	movups -0x48(%rbp),%xmm1
+   14015ef21:	movups -0x38(%rbp),%xmm2
+   14015ef25:	movups -0x28(%rbp),%xmm3
+   14015ef29:	movups %xmm3,0x30(%rax)
+   14015ef2d:	movups %xmm2,0x20(%rax)
+   14015ef31:	movups %xmm1,0x10(%rax)
+   14015ef35:	movups %xmm0,(%rax)
+   14015ef38:	add    $0x80,%rsp
+   14015ef3f:	pop    %rbp
+   14015ef40:	ret
+   14015ef41:	mov    $0x50,%ecx
+   14015ef46:	mov    $0x8,%edx
+   14015ef4b:	call   0x14015c420
+   14015ef50:	ud2
+   14015ef52:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
    14015ef60:	mov    %rdx,0x10(%rsp)
    14015ef65:	push   %rbp
    14015ef66:	sub    $0x20,%rsp
    14015ef6a:	lea    0x80(%rdx),%rbp
-   14015ef71:	lea    -0x60(%rbp),%rcx
-   14015ef75:	call   0x1400b3be0
+   14015ef71:	lea    -0x58(%rbp),%rcx
+   14015ef75:	call   0x1400b60c0
    14015ef7a:	nop
    14015ef7b:	add    $0x20,%rsp
    14015ef7f:	pop    %rbp
    14015ef80:	ret
    14015ef81:	int3
    14015ef82:	int3
    14015ef83:	int3
@@ -420491,63 +420483,67 @@
    14015f08d:	int3
    14015f08e:	int3
    14015f08f:	int3
    14015f090:	push   %rbp
    14015f091:	sub    $0x80,%rsp
    14015f098:	lea    0x80(%rsp),%rbp
    14015f0a0:	movq   $0xfffffffffffffffe,-0x8(%rbp)
-   14015f0a8:	lea    0x15831(%rip),%rax        # 0x1401748e0
-   14015f0af:	mov    %rax,-0x58(%rbp)
-   14015f0b3:	movups (%r8),%xmm0
-   14015f0b7:	movups 0x10(%r8),%xmm1
-   14015f0bc:	movups 0x20(%r8),%xmm2
-   14015f0c1:	movups %xmm0,-0x50(%rbp)
-   14015f0c5:	movups %xmm1,-0x40(%rbp)
-   14015f0c9:	movups %xmm2,-0x30(%rbp)
-   14015f0cd:	mov    0x30(%r8),%rax
-   14015f0d1:	mov    %rax,-0x20(%rbp)
-   14015f0d5:	mov    %rcx,-0x18(%rbp)
-   14015f0d9:	mov    %rdx,-0x10(%rbp)
-   14015f0dd:	mov    0x9f274(%rip),%rcx        # 0x1401fe358
-   14015f0e4:	test   %rcx,%rcx
-   14015f0e7:	jne    0x14015f0fe
-   14015f0e9:	call   *0x41d1(%rip)        # 0x1401632c0
-   14015f0ef:	test   %rax,%rax
-   14015f0f2:	je     0x14015f141
-   14015f0f4:	mov    %rax,%rcx
-   14015f0f7:	mov    %rax,0x9f25a(%rip)        # 0x1401fe358
-   14015f0fe:	mov    $0x50,%r8d
-   14015f104:	xor    %edx,%edx
-   14015f106:	call   *0x41dc(%rip)        # 0x1401632e8
-   14015f10c:	test   %rax,%rax
-   14015f10f:	je     0x14015f141
-   14015f111:	movups -0x18(%rbp),%xmm0
-   14015f115:	movups %xmm0,0x40(%rax)
-   14015f119:	movups -0x58(%rbp),%xmm0
-   14015f11d:	movups -0x48(%rbp),%xmm1
-   14015f121:	movups -0x38(%rbp),%xmm2
-   14015f125:	movups -0x28(%rbp),%xmm3
-   14015f129:	movups %xmm3,0x30(%rax)
-   14015f12d:	movups %xmm2,0x20(%rax)
-   14015f131:	movups %xmm1,0x10(%rax)
-   14015f135:	movups %xmm0,(%rax)
-   14015f138:	add    $0x80,%rsp
-   14015f13f:	pop    %rbp
-   14015f140:	ret
-   14015f141:	mov    $0x50,%ecx
-   14015f146:	mov    $0x8,%edx
-   14015f14b:	call   0x14015c420
-   14015f150:	ud2
-   14015f152:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   14015f0a8:	lea    0x15861(%rip),%rax        # 0x140174910
+   14015f0af:	mov    %rax,-0x60(%rbp)
+   14015f0b3:	movups (%rdx),%xmm0
+   14015f0b6:	movups 0x10(%rdx),%xmm1
+   14015f0ba:	movups 0x20(%rdx),%xmm2
+   14015f0be:	movups %xmm0,-0x58(%rbp)
+   14015f0c2:	movups %xmm1,-0x48(%rbp)
+   14015f0c6:	movups %xmm2,-0x38(%rbp)
+   14015f0ca:	mov    0x30(%rdx),%rax
+   14015f0ce:	mov    %rax,-0x28(%rbp)
+   14015f0d2:	movups (%rcx),%xmm0
+   14015f0d5:	movups %xmm0,-0x20(%rbp)
+   14015f0d9:	mov    0x10(%rcx),%rax
+   14015f0dd:	mov    %rax,-0x10(%rbp)
+   14015f0e1:	mov    0x9f270(%rip),%rcx        # 0x1401fe358
+   14015f0e8:	test   %rcx,%rcx
+   14015f0eb:	jne    0x14015f102
+   14015f0ed:	call   *0x41cd(%rip)        # 0x1401632c0
+   14015f0f3:	test   %rax,%rax
+   14015f0f6:	je     0x14015f14d
+   14015f0f8:	mov    %rax,%rcx
+   14015f0fb:	mov    %rax,0x9f256(%rip)        # 0x1401fe358
+   14015f102:	mov    $0x58,%r8d
+   14015f108:	xor    %edx,%edx
+   14015f10a:	call   *0x41d8(%rip)        # 0x1401632e8
+   14015f110:	test   %rax,%rax
+   14015f113:	je     0x14015f14d
+   14015f115:	mov    -0x10(%rbp),%rcx
+   14015f119:	mov    %rcx,0x50(%rax)
+   14015f11d:	movups -0x20(%rbp),%xmm0
+   14015f121:	movups %xmm0,0x40(%rax)
+   14015f125:	movups -0x60(%rbp),%xmm0
+   14015f129:	movups -0x50(%rbp),%xmm1
+   14015f12d:	movups -0x40(%rbp),%xmm2
+   14015f131:	movups -0x30(%rbp),%xmm3
+   14015f135:	movups %xmm3,0x30(%rax)
+   14015f139:	movups %xmm2,0x20(%rax)
+   14015f13d:	movups %xmm1,0x10(%rax)
+   14015f141:	movups %xmm0,(%rax)
+   14015f144:	add    $0x80,%rsp
+   14015f14b:	pop    %rbp
+   14015f14c:	ret
+   14015f14d:	mov    $0x58,%ecx
+   14015f152:	mov    $0x8,%edx
+   14015f157:	call   0x14015c420
+   14015f15c:	ud2
+   14015f15e:	xchg   %ax,%ax
    14015f160:	mov    %rdx,0x10(%rsp)
    14015f165:	push   %rbp
    14015f166:	sub    $0x20,%rsp
    14015f16a:	lea    0x80(%rdx),%rbp
-   14015f171:	lea    -0x58(%rbp),%rcx
-   14015f175:	call   0x1400b60c0
+   14015f171:	lea    -0x60(%rbp),%rcx
+   14015f175:	call   0x1400b3be0
    14015f17a:	nop
    14015f17b:	add    $0x20,%rsp
    14015f17f:	pop    %rbp
    14015f180:	ret
    14015f181:	int3
    14015f182:	int3
    14015f183:	int3
@@ -452531,174 +452527,169 @@
    1401745fa:	add    %al,(%rax)
    1401745fc:	and    $0x0,%al
    1401745fe:	add    %al,(%rax)
    140174600:	lock rex (bad)
    140174603:	rex add %eax,(%rax)
 	...
    14017460e:	add    %al,(%rax)
-   140174610:	cmpb   $0x0,(%rbx)
-   140174613:	rex add %eax,(%rax)
+   140174610:	rolb   $0x40,0x0(%rcx)
+   140174614:	add    %eax,(%rax)
    140174616:	add    %al,(%rax)
-   140174618:	sbb    %al,(%rax)
+   140174618:	adc    %al,(%rax)
    14017461a:	add    %al,(%rax)
    14017461c:	add    %al,(%rax)
    14017461e:	add    %al,(%rax)
    140174620:	or     %al,(%rax)
    140174622:	add    %al,(%rax)
    140174624:	add    %al,(%rax)
    140174626:	add    %al,(%rax)
-   140174628:	adc    $0x3,%cl
-   14017462b:	rex add %eax,(%rax)
+   140174628:	lock sub $0x14000,%eax
    14017462e:	add    %al,(%rax)
-   140174630:	cmpb   $0x0,(%rbx)
-   140174633:	rex add %eax,(%rax)
+   140174630:	rolb   $0x40,0x0(%rcx)
+   140174634:	add    %eax,(%rax)
    140174636:	add    %al,(%rax)
-   140174638:	sbb    %al,(%rax)
+   140174638:	adc    %al,(%rax)
    14017463a:	add    %al,(%rax)
    14017463c:	add    %al,(%rax)
    14017463e:	add    %al,(%rax)
    140174640:	or     %al,(%rax)
    140174642:	add    %al,(%rax)
    140174644:	add    %al,(%rax)
    140174646:	add    %al,(%rax)
-   140174648:	movabs 0x80000000014003d1,%al
-   140174651:	roll   (%rbx)
-   140174653:	rex add %eax,(%rax)
+   140174648:	movabs 0xf000000001400b6f,%al
+   140174651:	sub    $0x14000,%eax
    140174656:	add    %al,(%rax)
    140174658:	adc    %al,0x17(%rsi)
    14017465b:	rex add %eax,(%rax)
    14017465e:	add    %al,(%rax)
    140174660:	jo     0x1401745f8
    140174662:	add    0x1(%rax),%eax
    140174665:	add    %al,(%rax)
-   140174667:	add    %dl,(%rax)
+   140174667:	add    %dh,%al
    140174669:	(bad)
    14017466a:	or     0x1(%rax),%eax
    14017466d:	add    %al,(%rax)
    14017466f:	add    %dh,0x61(%rax)
    140174672:	or     0x1(%rax),%eax
    140174675:	add    %al,(%rax)
    140174677:	add    %dh,-0x6a(%rax)
    14017467a:	add    0x1(%rax),%eax
    14017467d:	add    %al,(%rax)
    14017467f:	add    %al,%al
    140174681:	add    %al,0x1(%r8)
    140174685:	add    %al,(%rax)
-   140174687:	add    %al,%al
-   140174689:	add    %al,0x1(%r8)
+   140174687:	add    %dh,0x1400b5f(%rax)
    14017468d:	add    %al,(%rax)
    14017468f:	add    %dl,(%rax)
    140174691:	add    %al,(%rax)
    140174693:	add    %al,(%rax)
    140174695:	add    %al,(%rax)
    140174697:	add    %cl,(%rax)
    140174699:	add    %al,(%rax)
    14017469b:	add    %al,(%rax)
    14017469d:	add    %al,(%rax)
-   14017469f:	add    %dh,%al
-   1401746a1:	sub    $0x14000,%eax
-   1401746a6:	add    %al,(%rax)
-   1401746a8:	rolb   $0x40,0x0(%rcx)
-   1401746ac:	add    %eax,(%rax)
-   1401746ae:	add    %al,(%rax)
-   1401746b0:	adc    %al,(%rax)
-   1401746b2:	add    %al,(%rax)
-   1401746b4:	add    %al,(%rax)
-   1401746b6:	add    %al,(%rax)
-   1401746b8:	or     %al,(%rax)
-   1401746ba:	add    %al,(%rax)
-   1401746bc:	add    %al,(%rax)
-   1401746be:	add    %al,(%rax)
-   1401746c0:	movabs 0xf000000001400b6f,%al
-   1401746c9:	sub    $0x14000,%eax
-   1401746ce:	add    %al,(%rax)
-   1401746d0:	mov    %al,0x17(%rsi)
-   1401746d3:	rex add %eax,(%rax)
-   1401746d6:	add    %al,(%rax)
-   1401746d8:	jo     0x140174670
-   1401746da:	add    0x1(%rax),%eax
+   14017469f:	add    %ah,0x6f(%rax)
+   1401746a2:	or     0x1(%rax),%eax
+   1401746a5:	add    %al,(%rax)
+   1401746a7:	add    %dh,0x1400b5f(%rax)
+   1401746ad:	add    %al,(%rax)
+   1401746af:	add    %dl,(%rax)
+   1401746b1:	add    %al,(%rax)
+   1401746b3:	add    %al,(%rax)
+   1401746b5:	add    %al,(%rax)
+   1401746b7:	add    %cl,(%rax)
+   1401746b9:	add    %al,(%rax)
+   1401746bb:	add    %al,(%rax)
+   1401746bd:	add    %al,(%rax)
+   1401746bf:	add    %al,0x1400b6e(%rax)
+   1401746c5:	add    %al,(%rax)
+   1401746c7:	add    %ah,0x6f(%rax)
+   1401746ca:	or     0x1(%rax),%eax
+   1401746cd:	add    %al,(%rax)
+   1401746cf:	add    %cl,0x1401746(%rax)
+   1401746d5:	add    %al,(%rax)
+   1401746d7:	add    %ah,0x1400b61(%rax)
    1401746dd:	add    %al,(%rax)
-   1401746df:	add    %dl,%al
+   1401746df:	add    %ah,%al
    1401746e1:	(bad)
    1401746e2:	or     0x1(%rax),%eax
    1401746e5:	add    %al,(%rax)
    1401746e7:	add    %dh,0x61(%rax)
    1401746ea:	or     0x1(%rax),%eax
    1401746ed:	add    %al,(%rax)
-   1401746ef:	add    %dh,-0x6a(%rax)
-   1401746f2:	add    0x1(%rax),%eax
+   1401746ef:	add    %ah,0x1400b61(%rax)
    1401746f5:	add    %al,(%rax)
    1401746f7:	add    %al,%al
    1401746f9:	add    %al,0x1(%r8)
    1401746fd:	add    %al,(%rax)
-   1401746ff:	add    %dh,0x1400b5f(%rax)
+   1401746ff:	add    %al,0x140003b(%rax)
    140174705:	add    %al,(%rax)
-   140174707:	add    %dl,(%rax)
+   140174707:	add    %bl,(%rax)
    140174709:	add    %al,(%rax)
    14017470b:	add    %al,(%rax)
    14017470d:	add    %al,(%rax)
    14017470f:	add    %cl,(%rax)
    140174711:	add    %al,(%rax)
    140174713:	add    %al,(%rax)
    140174715:	add    %al,(%rax)
-   140174717:	add    %ah,0x6f(%rax)
-   14017471a:	or     0x1(%rax),%eax
+   140174717:	add    %al,0x14003d1(%rax)
    14017471d:	add    %al,(%rax)
-   14017471f:	add    %dh,0x1400b5f(%rax)
+   14017471f:	add    %al,0x140003b(%rax)
    140174725:	add    %al,(%rax)
-   140174727:	add    %dl,(%rax)
+   140174727:	add    %bl,(%rax)
    140174729:	add    %al,(%rax)
    14017472b:	add    %al,(%rax)
    14017472d:	add    %al,(%rax)
    14017472f:	add    %cl,(%rax)
    140174731:	add    %al,(%rax)
    140174733:	add    %al,(%rax)
    140174735:	add    %al,(%rax)
-   140174737:	add    %al,0x1400b6e(%rax)
+   140174737:	add    %ah,0x14003d1(%rax)
    14017473d:	add    %al,(%rax)
-   14017473f:	add    %ah,0x6f(%rax)
-   140174742:	or     0x1(%rax),%eax
+   14017473f:	add    %al,0x14003d1(%rax)
    140174745:	add    %al,(%rax)
    140174747:	add    %al,(%rax)
    140174749:	rex.RXB (bad)
    14017474b:	rex add %eax,(%rax)
    14017474e:	add    %al,(%rax)
-   140174750:	andb   $0x40,0xb(%rcx)
-   140174754:	add    %eax,(%rax)
-   140174756:	add    %al,(%rax)
-   140174758:	add    %ah,0xb(%rdx)
-   14017475b:	rex add %eax,(%rax)
-   14017475e:	add    %al,(%rax)
-   140174760:	jo     0x1401747c3
+   140174750:	jo     0x1401746e8
+   140174752:	add    0x1(%rax),%eax
+   140174755:	add    %al,(%rax)
+   140174757:	add    %al,(%rax)
+   140174759:	(bad)
+   14017475a:	or     0x1(%rax),%eax
+   14017475d:	add    %al,(%rax)
+   14017475f:	add    %dh,0x61(%rax)
    140174762:	or     0x1(%rax),%eax
    140174765:	add    %al,(%rax)
-   140174767:	add    %al,0x1400b61(%rax)
+   140174767:	add    %dh,-0x6a(%rax)
+   14017476a:	add    0x1(%rax),%eax
    14017476d:	add    %al,(%rax)
    14017476f:	add    %al,%al
    140174771:	add    %al,0x1(%r8)
    140174775:	add    %al,(%rax)
-   140174777:	add    %ah,%al
-   140174779:	cmp    (%rbx),%ecx
+   140174777:	add    %ah,(%rax)
+   140174779:	cmp    $0xb,%al
    14017477b:	rex add %eax,(%rax)
    14017477e:	add    %al,(%rax)
-   140174780:	pop    %rax
+   140174780:	push   %rax
    140174781:	add    %al,(%rax)
    140174783:	add    %al,(%rax)
    140174785:	add    %al,(%rax)
    140174787:	add    %cl,(%rax)
    140174789:	add    %al,(%rax)
    14017478b:	add    %al,(%rax)
    14017478d:	add    %al,(%rax)
    14017478f:	add    %al,0x1400b6f(%rax)
    140174795:	add    %al,(%rax)
-   140174797:	add    %ah,%al
-   140174799:	cmp    (%rbx),%ecx
+   140174797:	add    %ah,(%rax)
+   140174799:	cmp    $0xb,%al
    14017479b:	rex add %eax,(%rax)
    14017479e:	add    %al,(%rax)
-   1401747a0:	pop    %rax
+   1401747a0:	push   %rax
    1401747a1:	add    %al,(%rax)
    1401747a3:	add    %al,(%rax)
    1401747a5:	add    %al,(%rax)
    1401747a7:	add    %cl,(%rax)
    1401747a9:	add    %al,(%rax)
    1401747ab:	add    %al,(%rax)
    1401747ad:	add    %al,(%rax)
@@ -452707,49 +452698,47 @@
    1401747b5:	add    %al,(%rax)
    1401747b7:	add    %al,0x1400b6f(%rax)
    1401747bd:	add    %al,(%rax)
    1401747bf:	add    %bh,0x47(%rax)
    1401747c2:	(bad)
    1401747c3:	rex add %eax,(%rax)
    1401747c6:	add    %al,(%rax)
-   1401747c8:	nop
-   1401747c9:	(bad)
-   1401747ca:	or     0x1(%rax),%eax
-   1401747cd:	add    %al,(%rax)
-   1401747cf:	add    %al,%al
-   1401747d1:	(bad)
-   1401747d2:	or     0x1(%rax),%eax
-   1401747d5:	add    %al,(%rax)
-   1401747d7:	add    %dh,0x61(%rax)
+   1401747c8:	andb   $0x40,0xb(%rcx)
+   1401747cc:	add    %eax,(%rax)
+   1401747ce:	add    %al,(%rax)
+   1401747d0:	shlb   $0x40,0xb(%rcx)
+   1401747d4:	add    %eax,(%rax)
+   1401747d6:	add    %al,(%rax)
+   1401747d8:	jo     0x14017483b
    1401747da:	or     0x1(%rax),%eax
    1401747dd:	add    %al,(%rax)
-   1401747df:	add    %dl,0x1400b61(%rax)
+   1401747df:	add    %al,0x1400b61(%rax)
    1401747e5:	add    %al,(%rax)
    1401747e7:	add    %al,%al
    1401747e9:	add    %al,0x1(%r8)
    1401747ed:	add    %al,(%rax)
-   1401747ef:	add    %ah,(%rax)
-   1401747f1:	cmp    $0xb,%al
+   1401747ef:	add    %ah,%al
+   1401747f1:	cmp    (%rbx),%ecx
    1401747f3:	rex add %eax,(%rax)
    1401747f6:	add    %al,(%rax)
-   1401747f8:	push   %rax
+   1401747f8:	pop    %rax
    1401747f9:	add    %al,(%rax)
    1401747fb:	add    %al,(%rax)
    1401747fd:	add    %al,(%rax)
    1401747ff:	add    %cl,(%rax)
    140174801:	add    %al,(%rax)
    140174803:	add    %al,(%rax)
    140174805:	add    %al,(%rax)
    140174807:	add    %al,0x1400b6f(%rax)
    14017480d:	add    %al,(%rax)
-   14017480f:	add    %ah,(%rax)
-   140174811:	cmp    $0xb,%al
+   14017480f:	add    %ah,%al
+   140174811:	cmp    (%rbx),%ecx
    140174813:	rex add %eax,(%rax)
    140174816:	add    %al,(%rax)
-   140174818:	push   %rax
+   140174818:	pop    %rax
    140174819:	add    %al,(%rax)
    14017481b:	add    %al,(%rax)
    14017481d:	add    %al,(%rax)
    14017481f:	add    %cl,(%rax)
    140174821:	add    %al,(%rax)
    140174823:	add    %al,(%rax)
    140174825:	add    %al,(%rax)
@@ -452758,26 +452747,24 @@
    14017482d:	add    %al,(%rax)
    14017482f:	add    %al,0x1400b6f(%rax)
    140174835:	add    %al,(%rax)
    140174837:	add    %dh,%al
    140174839:	rex.RXB (bad)
    14017483b:	rex add %eax,(%rax)
    14017483e:	add    %al,(%rax)
-   140174840:	nop
-   140174841:	(bad)
-   140174842:	or     0x1(%rax),%eax
-   140174845:	add    %al,(%rax)
-   140174847:	add    %dh,%al
-   140174849:	(bad)
-   14017484a:	or     0x1(%rax),%eax
-   14017484d:	add    %al,(%rax)
-   14017484f:	add    %dh,0x61(%rax)
+   140174840:	andb   $0x40,0xb(%rcx)
+   140174844:	add    %eax,(%rax)
+   140174846:	add    %al,(%rax)
+   140174848:	shlb   0xb(%rcx)
+   14017484b:	rex add %eax,(%rax)
+   14017484e:	add    %al,(%rax)
+   140174850:	jo     0x1401748b3
    140174852:	or     0x1(%rax),%eax
    140174855:	add    %al,(%rax)
-   140174857:	add    %dl,0x1400b61(%rax)
+   140174857:	add    %al,0x1400b61(%rax)
    14017485d:	add    %al,(%rax)
    14017485f:	add    %al,%al
    140174861:	add    %al,0x1(%r8)
    140174865:	add    %al,(%rax)
    140174867:	add    %al,%al
    140174869:	(bad)
    14017486a:	or     0x1(%rax),%eax
@@ -452809,70 +452796,69 @@
    1401748a5:	add    %al,(%rax)
    1401748a7:	add    %al,0x1400b6f(%rax)
    1401748ad:	add    %al,(%rax)
    1401748af:	add    %ch,0x48(%rax)
    1401748b2:	(bad)
    1401748b3:	rex add %eax,(%rax)
    1401748b6:	add    %al,(%rax)
-   1401748b8:	nop
-   1401748b9:	(bad)
-   1401748ba:	or     0x1(%rax),%eax
-   1401748bd:	add    %al,(%rax)
-   1401748bf:	add    %dh,0x1400b61(%rax)
+   1401748b8:	andb   $0x40,0xb(%rcx)
+   1401748bc:	add    %eax,(%rax)
+   1401748be:	add    %al,(%rax)
+   1401748c0:	mov    $0x61,%al
+   1401748c2:	or     0x1(%rax),%eax
    1401748c5:	add    %al,(%rax)
    1401748c7:	add    %dh,0x61(%rax)
    1401748ca:	or     0x1(%rax),%eax
    1401748cd:	add    %al,(%rax)
-   1401748cf:	add    %dl,0x1400b61(%rax)
+   1401748cf:	add    %al,0x1400b61(%rax)
    1401748d5:	add    %al,(%rax)
    1401748d7:	add    %al,%al
    1401748d9:	add    %al,0x1(%r8)
    1401748dd:	add    %al,(%rax)
-   1401748df:	add    %dh,0x6c(%rax)
-   1401748e2:	or     0x1(%rax),%eax
+   1401748df:	add    %dh,0x1400b6b(%rax)
    1401748e5:	add    %al,(%rax)
-   1401748e7:	add    %dl,0x1400b6b(%rax)
+   1401748e7:	add    %al,0x1400b6b(%rax)
    1401748ed:	add    %al,(%rax)
    1401748ef:	add    %al,%al
    1401748f1:	insb   (%dx),%es:(%rdi)
    1401748f2:	or     0x1(%rax),%eax
    1401748f5:	add    %al,(%rax)
    1401748f7:	add    %dl,%al
    1401748f9:	insb   (%dx),%es:(%rdi)
    1401748fa:	or     0x1(%rax),%eax
    1401748fd:	add    %al,(%rax)
-   1401748ff:	add    %dh,0x6c(%rax)
-   140174902:	or     0x1(%rax),%eax
+   1401748ff:	add    %dh,0x1400b6b(%rax)
    140174905:	add    %al,(%rax)
    140174907:	add    %dh,-0x6a(%rax)
    14017490a:	add    0x1(%rax),%eax
    14017490d:	add    %al,(%rax)
-   14017490f:	add    %dh,0x1400b6b(%rax)
-   140174915:	add    %al,(%rax)
-   140174917:	add    %al,0x1400b6b(%rax)
-   14017491d:	add    %al,(%rax)
-   14017491f:	add    %ah,0x1400b6c(%rax)
+   14017490f:	add    %ah,%al
+   140174911:	imul   $0x40,(%rbx),%ecx
+   140174914:	add    %eax,(%rax)
+   140174916:	add    %al,(%rax)
+   140174918:	movabs 0xb000000001400b6b,%al
+   140174921:	insb   (%dx),%es:(%rdi)
+   140174922:	or     0x1(%rax),%eax
    140174925:	add    %al,(%rax)
    140174927:	add    %dh,%al
    140174929:	insb   (%dx),%es:(%rdi)
    14017492a:	or     0x1(%rax),%eax
    14017492d:	add    %al,(%rax)
-   14017492f:	add    %dh,0x6c(%rax)
-   140174932:	or     0x1(%rax),%eax
+   14017492f:	add    %dh,0x1400b6b(%rax)
    140174935:	add    %al,(%rax)
    140174937:	add    %dh,-0x6a(%rax)
    14017493a:	add    0x1(%rax),%eax
    14017493d:	add    %al,(%rax)
-   14017493f:	add    %al,(%rax)
+   14017493f:	add    %dh,(%rax)
    140174941:	insb   (%dx),%es:(%rdi)
    140174942:	or     0x1(%rax),%eax
    140174945:	add    %al,(%rax)
-   140174947:	add    %ah,0x1400b6b(%rax)
+   140174947:	add    %dl,0x1400b6b(%rax)
    14017494d:	add    %al,(%rax)
-   14017494f:	add    %dh,0x1400b6c(%rax)
+   14017494f:	add    %ah,0x1400b6c(%rax)
    140174955:	add    %al,(%rax)
    140174957:	add    %dl,(%rax)
    140174959:	insl   (%dx),%es:(%rdi)
    14017495a:	or     0x1(%rax),%eax
    14017495d:	add    %al,(%rax)
    14017495f:	add    %al,0x6d(%rax)
    140174962:	or     0x1(%rax),%eax
@@ -452952,24 +452938,19 @@
    140174a13:	rex add %eax,(%rax)
    140174a16:	add    %al,(%rax)
    140174a18:	nop
    140174a19:	cmpsb  %es:(%rdi),%ds:(%rsi)
    140174a1a:	adc    $0x40,%al
    140174a1c:	add    %eax,(%rax)
    140174a1e:	add    %al,(%rax)
-   140174a20:	loopne 0x140174a83
-   140174a22:	or     0x1(%rax),%eax
-   140174a25:	add    %al,(%rax)
-   140174a27:	add    %al,%al
-   140174a29:	movsl  %ds:(%rsi),%es:(%rdi)
-   140174a2a:	adc    $0x40,%al
-   140174a2c:	add    %eax,(%rax)
-   140174a2e:	add    %al,(%rax)
-   140174a30:	(bad)
-   140174a31:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   140174a20:	adc    %ah,0xb(%rdx)
+   140174a23:	rex add %eax,(%rax)
+   140174a26:	add    %al,(%rax)
+   140174a28:	shlb   $0x0,0x14014(%rbp)
+   140174a2f:	add    %ah,-0x5a(%rax)
    140174a32:	adc    $0x40,%al
    140174a34:	add    %eax,(%rax)
    140174a36:	add    %al,(%rax)
    140174a38:	rolb   $0x40,0x0(%rcx)
    140174a3c:	add    %eax,(%rax)
    140174a3e:	add    %al,(%rax)
    140174a40:	push   %rax
@@ -453198,15 +453179,15 @@
    140174c5f:	gs push %rsp
    140174c61:	imul   $0x74747548,0x20(%rbp),%ebp
    140174c68:	and    %bh,(%rsp,%rsi,2)
    140174c6b:	fs push $0x40747475
    140174c71:	insl   (%dx),%es:(%edi)
    140174c73:	(bad)
    140174c74:	imul   $0x303e6d6f,0x63(%rsi,%rbp,1),%ebp
-   140174c7c:	cs xor (%rsi),%ch
+   140174c7c:	cs xor (%rsi),%ebp
    140174c7f:	xor    %al,0x69(%rsi)
    140174c82:	outsb  %ds:(%rsi),(%dx)
    140174c83:	and    %dh,%fs:0x65(%rax,%rbp,2)
    140174c88:	and    %ch,0x61(%rbp)
    140174c8b:	js     0x140174cf6
    140174c8d:	insl   (%dx),%es:(%rdi)
    140174c8e:	jne    0x140174cfd
@@ -624326,15 +624307,15 @@
    1401d4a9c:	add    %al,(%rax)
    1401d4a9e:	add    %al,(%rax)
    1401d4aa0:	movabs 0xd00000000140149c,%al
    1401d4aa9:	movabs 0x4a68000000014014,%al
    1401d4ab2:	sbb    $0x140,%eax
    1401d4ab7:	add    %dl,0x14014a6(%rax)
    1401d4abd:	add    %al,(%rax)
-   1401d4abf:	add    %ah,%al
+   1401d4abf:	add    %dl,(%rax)
    1401d4ac1:	(bad)
    1401d4ac2:	or     0x1(%rax),%eax
    1401d4ac5:	add    %al,(%rax)
    1401d4ac7:	add    %al,%al
    1401d4ac9:	movsl  %ds:(%rsi),%es:(%rdi)
    1401d4aca:	adc    $0x40,%al
    1401d4acc:	add    %eax,(%rax)
@@ -624611,16 +624592,17 @@
    1401d4e46:	add    %al,(%rax)
    1401d4e48:	js     0x1401d4e7d
    1401d4e4a:	(bad)
    1401d4e4b:	rex add %eax,(%rax)
    1401d4e4e:	add    %al,(%rax)
    1401d4e50:	add    %al,(%rax)
    1401d4e52:	add    %al,(%rax)
-   1401d4e54:	lea    0x62(%rdx),%esp
-   1401d4e57:	add    %al,%fs:(%rax)
+   1401d4e54:	(bad)
+   1401d4e55:	fbld   0x64(%rbx)
+   1401d4e58:	add    %al,(%rax)
    1401d4e5a:	add    %al,(%rax)
    1401d4e5c:	or     $0x44000000,%eax
    1401d4e61:	add    (%rax),%eax
    1401d4e63:	add    %ah,0x1d(%rdi,%rcx,2)
    1401d4e67:	add    %ah,0x1d(%rbp,%rsi,1)
 	...
    1401d4e7f:	add    %cl,%al
@@ -662125,27 +662107,28 @@
    1401ea654:	add    %al,(%rax)
    1401ea656:	add    %al,(%rax)
    1401ea658:	add    %eax,(%rax)
    1401ea65a:	add    %al,(%rax)
    1401ea65c:	(bad)
    1401ea65d:	(bad)
    1401ea65e:	(bad)
-   1401ea65f:	push   0x69(%rax)
-   1401ea662:	or     (%rax),%eax
-   1401ea664:	add    %al,(%rax)
-   1401ea666:	add    %al,(%rax)
-   1401ea668:	and    %ch,0xb(%rcx)
-   1401ea66b:	add    %dh,%al
-   1401ea66d:	or     (%rax),%ax
-   1401ea670:	(bad)
+   1401ea65f:	push   0xb69(%rax)
+   1401ea665:	add    %al,(%rax)
+   1401ea667:	add    %ah,0x69(%rax)
+   1401ea66a:	or     (%rax),%eax
+   1401ea66c:	xor    %ah,0xb(%rdi)
+   1401ea66f:	add    %bh,%bh
    1401ea671:	(bad)
    1401ea672:	(bad)
-   1401ea673:	lcall  *0x1000b68(%rbx)
+   1401ea673:	(bad)
+   1401ea674:	fldt   0xb(%rax)
+   1401ea677:	add    %al,(%rcx)
    1401ea679:	add    %al,(%rax)
-   1401ea67b:	add    %ah,-0xfff5(%rax,%rbp,2)
+   1401ea67b:	add    %ah,%ah
+   1401ea67d:	push   $0xffffffffffff000b
    1401ea682:	(bad)
    1401ea683:	incl   (%rcx)
    1401ea685:	(bad)
    1401ea686:	add    $0x0,%al
    1401ea688:	(bad)
    1401ea689:	rolb   %cl,(%rbx)
    1401ea68b:	xor    %al,(%rdx)
@@ -662182,26 +662165,28 @@
    1401ea6cf:	add    %al,(%rax)
    1401ea6d1:	add    %al,(%rax)
    1401ea6d3:	add    %al,(%rcx)
    1401ea6d5:	add    %al,(%rax)
    1401ea6d7:	add    %bh,%bh
    1401ea6d9:	(bad)
    1401ea6da:	(bad)
-   1401ea6db:	call   *0x6c(%rax)
-   1401ea6de:	or     (%rax),%eax
-   1401ea6e0:	add    %ch,0x0(%rbx,%rcx,1)
+   1401ea6db:	incl   0x30000b6c(%rax)
+   1401ea6e1:	insb   (%dx),%es:(%rdi)
+   1401ea6e2:	or     (%rax),%eax
    1401ea6e4:	(bad)
    1401ea6e5:	(bad)
    1401ea6e6:	(bad)
-   1401ea6e7:	ljmp   *(%rax)
-   1401ea6e9:	insb   (%dx),%es:(%rdi)
+   1401ea6e7:	lcall  *0x6c(%rax)
    1401ea6ea:	or     (%rax),%eax
    1401ea6ec:	add    %al,(%rax)
    1401ea6ee:	add    %al,(%rax)
-   1401ea6f0:	sub    $0xff000b6c,%eax
+   1401ea6f0:	pop    %rbp
+   1401ea6f1:	insb   (%dx),%es:(%rdi)
+   1401ea6f2:	or     (%rax),%eax
+   1401ea6f4:	(bad)
    1401ea6f5:	(bad)
    1401ea6f6:	(bad)
    1401ea6f7:	lcall  *(%rcx)
    1401ea6f9:	or     -0x7df9fcf5(,%rax,2),%eax
    1401ea700:	add    0x1(%rax),%ah
    1401ea703:	push   %rax
    1401ea704:	push   %rsi
@@ -662336,17 +662321,17 @@
    1401ea82d:	(bad)
    1401ea82e:	(bad)
    1401ea82f:	jmp    *-0x11(%rax)
    1401ea832:	adc    $0x15ee9000,%eax
    1401ea837:	add    %bh,%bh
    1401ea839:	(bad)
    1401ea83a:	(bad)
-   1401ea83b:	decl   -0x11(%rsi)
+   1401ea83b:	incl   -0x11(%rdx)
    1401ea83e:	adc    $0x0,%eax
-   1401ea843:	add    %bl,-0x11(%rbp)
+   1401ea843:	add    %dl,-0x11(%rcx)
    1401ea846:	adc    $0xffffff00,%eax
    1401ea84b:	lcall  *(%rcx)
    1401ea84d:	adc    %al,(%rbx)
    1401ea84f:	test   %edx,(%rax)
    1401ea851:	add    (%rax),%ecx
    1401ea853:	repnz add %edx,0x0(%rax)
    1401ea857:	add    %dl,-0x45(%rsi)
@@ -662412,17 +662397,17 @@
    1401ea8f5:	(bad)
    1401ea8f6:	(bad)
    1401ea8f7:	jmp    *-0xf(%rax)
    1401ea8fa:	adc    $0x15f09000,%eax
    1401ea8ff:	add    %bh,%bh
    1401ea901:	(bad)
    1401ea902:	(bad)
-   1401ea903:	incl   -0xf(%rdx)
+   1401ea903:	decl   -0xf(%rsi)
    1401ea906:	adc    $0x0,%eax
-   1401ea90b:	add    %dl,-0xf(%rcx)
+   1401ea90b:	add    %bl,-0xf(%rbp)
    1401ea90e:	adc    $0xffffff00,%eax
    1401ea913:	incl   (%rcx)
    1401ea915:	add    $0xd2050002,%eax
    1401ea91a:	add    %esp,0x19(%rax)
    1401ea91d:	adc    $0x315450a,%eax
    1401ea922:	adc    %al,0x700b300c(%rdx)
    1401ea928:	or     0x9(%rax),%ah
@@ -705246,17 +705231,17 @@
    140204d5c:	add    $0xa5,%al
    140204d5e:	(bad)
    140204d5f:	add    %al,0x61(%rax)
    140204d62:	or     (%rax),%eax
    140204d64:	outsb  %ds:(%rsi),(%dx)
    140204d65:	(bad)
    140204d66:	or     (%rax),%eax
-   140204d68:	sbb    %ah,0x6190001e(%rbp)
+   140204d68:	sbb    %ah,0x6180001e(%rbp)
    140204d6e:	or     (%rax),%eax
-   140204d70:	movsl  %ds:(%rsi),%es:(%rdi)
+   140204d70:	xchg   %eax,%ebp
    140204d71:	(bad)
    140204d72:	or     (%rax),%eax
    140204d74:	mov    $0x20001d53,%eax
    140204d79:	(bad)
    140204d7a:	or     (%rax),%eax
    140204d7c:	std
    140204d7d:	(bad)
@@ -705276,69 +705261,61 @@
    140204da1:	or     (%rax),%ax
    140204da4:	push   $0xffffffffd0001ea5
    140204da9:	or     (%rax),%ax
    140204dac:	out    %al,(%dx)
    140204dad:	or     (%rax),%ax
    140204db0:	mov    %ah,0x66f0001e(%rbp)
    140204db6:	or     (%rax),%eax
-   140204db8:	sbb    0xb(%rcx),%ebp
-   140204dbb:	add    %ah,%ah
-   140204dbd:	movsl  %ds:(%rsi),%es:(%rdi)
-   140204dbe:	(bad)
-   140204dbf:	add    %ah,(%rax)
-   140204dc1:	imul   $0xb696d00,(%rbx),%ecx
-   140204dc7:	add    %al,(%rsi,%riz,4)
+   140204db8:	sub    $0x5c000b67,%eax
+   140204dbd:	push   %rsp
+   140204dbe:	sbb    $0xb673000,%eax
+   140204dc3:	add    %bl,0x69(%rbx)
+   140204dc6:	or     (%rax),%eax
+   140204dc8:	in     $0xa5,%al
    140204dca:	(bad)
-   140204dcb:	add    %dh,0x69(%rax)
+   140204dcb:	add    %ah,0x69(%rax)
    140204dce:	or     (%rax),%eax
-   140204dd0:	mov    $0x1c000b69,%eax
-   140204dd5:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   140204dd6:	(bad)
-   140204dd7:	add    %al,%al
-   140204dd9:	imul   $0xb69fd00,(%rbx),%ecx
-   140204ddf:	add    %bl,0x1d(%rsp,%rdx,2)
+   140204dd0:	lods   %ds:(%rsi),%eax
+   140204dd1:	imul   $0x1ea60400,(%rbx),%ecx
+   140204dd7:	add    %dh,-0x7fff497(%rax)
+   140204ddd:	imul   $0x1ea61c00,(%rbx),%ecx
    140204de3:	add    %al,(%rax)
    140204de5:	push   $0xb
    140204de7:	add    %dl,%al
    140204de9:	push   $0xb
    140204deb:	add    %cl,(%rax)
    140204ded:	push   %rsi
    140204dee:	sbb    $0xb6ad000,%eax
    140204df3:	add    %bh,0x6b(%rax)
    140204df6:	or     (%rax),%eax
    140204df8:	test   %ah,0x6bb0001e(%rsi)
    140204dfe:	or     (%rax),%eax
-   140204e00:	repz imul $0x0,(%rbx),%ecx
-   140204e04:	pop    %rsp
-   140204e05:	push   %rsp
-   140204e06:	sbb    $0xb6c0000,%eax
-   140204e0b:	add    %al,0x6c(%rsi)
-   140204e0e:	or     (%rax),%eax
-   140204e10:	nop
-   140204e11:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   140204e12:	(bad)
-   140204e13:	add    %dl,0x6c(%rax)
-   140204e16:	or     (%rax),%eax
-   140204e18:	jo     0x140204e86
+   140204e00:	fldcw  0xb(%rbx)
+   140204e03:	add    %bl,0x1d(%rsp,%rdx,2)
+   140204e07:	add    %ah,%al
+   140204e09:	imul   $0x0,(%rbx),%ecx
+   140204e0c:	and    0x0(%rbx,%rcx,1),%ebp
+   140204e10:	pop    %rsp
+   140204e11:	push   %rsp
+   140204e12:	sbb    $0xb6c3000,%eax
+   140204e17:	add    %dh,0x6c(%rsi)
    140204e1a:	or     (%rax),%eax
-   140204e1c:	movsb  %ds:(%rsi),%es:(%rdi)
+   140204e1c:	nop
    140204e1d:	cmpsb  %es:(%rdi),%ds:(%rsi)
    140204e1e:	(bad)
-   140204e1f:	add    %dh,0x6c(%rax)
-   140204e22:	or     (%rax),%eax
-   140204e24:	cltd
+   140204e1f:	add    %al,-0x5ffff494(%rax)
    140204e25:	insb   (%dx),%es:(%rdi)
    140204e26:	or     (%rax),%eax
-   140204e28:	pop    %rsp
-   140204e29:	push   %rsp
-   140204e2a:	sbb    $0xb6d4000,%eax
-   140204e2f:	add    %al,(%rdx)
-   140204e31:	outsb  %ds:(%rsi),(%dx)
-   140204e32:	or     (%rax),%eax
-   140204e34:	clc
+   140204e28:	movsb  %ds:(%rsi),%es:(%rdi)
+   140204e29:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   140204e2a:	(bad)
+   140204e2b:	add    %al,0x6d(%rax)
+   140204e2e:	or     (%rax),%eax
+   140204e30:	add    0xb(%rsi),%ch
+   140204e33:	add    %bh,%al
    140204e35:	cmpsb  %es:(%rdi),%ds:(%rsi)
    140204e36:	(bad)
    140204e37:	add    %dl,(%rax)
    140204e39:	outsb  %ds:(%rsi),(%dx)
    140204e3a:	or     (%rax),%eax
    140204e3c:	xor    %ch,0xb(%rsi)
    140204e3f:	add    %cl,(%rdi,%riz,4)
@@ -713700,30 +713677,30 @@
    14020a5f7:	add    %dl,%al
    14020a5f9:	in     (%dx),%eax
    14020a5fa:	adc    $0x15ee5300,%eax
    14020a5ff:	add    %bh,0x1e(%rdi,%riz,4)
    14020a603:	add    %ah,-0x12(%rax)
    14020a606:	adc    $0x15ee8d00,%eax
    14020a60b:	add    %dl,-0x116fffe2(%rdi,%riz,4)
-   14020a612:	adc    $0x15ef5e00,%eax
+   14020a612:	adc    $0x15ef5200,%eax
    14020a617:	add    %ch,%al
    14020a619:	cmpsl  %es:(%rdi),%ds:(%rsi)
    14020a61a:	(bad)
    14020a61b:	add    %ah,-0x11(%rax)
    14020a61e:	adc    $0x15ef8100,%eax
    14020a623:	add    %bh,%ah
    14020a625:	cmpsl  %es:(%rdi),%ds:(%rsi)
    14020a626:	(bad)
    14020a627:	add    %dl,0x520015ef(%rax)
    14020a62d:	lock adc $0x1ea84c00,%eax
    14020a633:	add    %ah,-0x10(%rax)
    14020a636:	adc    $0x15f08100,%eax
    14020a63b:	add    %ah,-0x58(%rax)
    14020a63e:	(bad)
-   14020a63f:	add    %dl,0x520015f0(%rax)
+   14020a63f:	add    %dl,0x5e0015f0(%rax)
    14020a645:	int1
    14020a646:	adc    $0x1ea8b000,%eax
    14020a64b:	add    %ah,-0xf(%rax)
    14020a64e:	adc    $0x15f18100,%eax
    14020a653:	add    %al,%ah
    14020a655:	test   $0x1e,%al
    14020a657:	add    %dl,0x1b0015f1(%rax)
```

