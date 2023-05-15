# Comparing `tmp/steptools-20.0-cp37-abi3-win_amd64.whl.zip` & `tmp/steptools-20.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7354198 bytes, number of entries: 8
+Zip file size: 7353794 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        2 b- defN 22-Aug-19 14:38 steptools/py.typed
--rw-rw-rw-  2.0 fat 30841576 b- defN 23-May-11 20:37 steptools/step.pyd
--rw-rw-rw-  2.0 fat   107458 b- defN 23-May-04 20:43 steptools/step.pyi
--rw-rw-rw-  2.0 fat     3043 b- defN 23-May-11 20:37 steptools-20.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7015 b- defN 23-May-11 20:37 steptools-20.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-11 20:37 steptools-20.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-11 20:37 steptools-20.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-May-11 20:37 steptools-20.0.dist-info/RECORD
-8 files, 30959829 bytes uncompressed, 7353132 bytes compressed:  76.3%
+-rw-rw-rw-  2.0 fat 30832360 b- defN 23-May-15 22:31 steptools/step.pyd
+-rw-rw-rw-  2.0 fat   107772 b- defN 23-May-15 19:45 steptools/step.pyi
+-rw-rw-rw-  2.0 fat     3043 b- defN 23-May-15 22:32 steptools-20.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7014 b- defN 23-May-15 22:32 steptools-20.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-15 22:32 steptools-20.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-15 22:32 steptools-20.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-May-15 22:32 steptools-20.1.dist-info/RECORD
+8 files, 30950926 bytes uncompressed, 7352728 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: steptools/step.pyd
 Comment: 
 
 Filename: steptools/step.pyi
 Comment: 
 
-Filename: steptools-20.0.dist-info/LICENSE
+Filename: steptools-20.1.dist-info/LICENSE
 Comment: 
 
-Filename: steptools-20.0.dist-info/METADATA
+Filename: steptools-20.1.dist-info/METADATA
 Comment: 
 
-Filename: steptools-20.0.dist-info/WHEEL
+Filename: steptools-20.1.dist-info/WHEEL
 Comment: 
 
-Filename: steptools-20.0.dist-info/top_level.txt
+Filename: steptools-20.1.dist-info/top_level.txt
 Comment: 
 
-Filename: steptools-20.0.dist-info/RECORD
+Filename: steptools-20.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## steptools/step.pyi

```diff
@@ -144,26 +144,37 @@
 class Design:
     '''
     Class containing all data from a STEP exchange file.
     '''
     @overload    
     def name(self) -> str: ...
     @overload    
-    def name(self, nm: str) -> None:
+    def name(self, nm: StrOrBytesPath) -> None:
         '''Get or set design name'''
         pass
+
+    @overload    
+    def path(self) -> str: ...
+    @overload    
+    def path(self, nm: StrOrBytesPath) -> None:
+        '''Get or set design file path'''
+        pass
     
     def header_name(self) -> Object:
         '''Get header name object'''
         pass
 
     def header_description(self) -> Object:
         '''Get header description object'''
         pass
 
+    def find(self, id: str | int) -> Object:
+        '''Find an object by ANCHOR name or #123 entity id'''
+        pass
+
     def keys() -> Set[str]:
         '''Design name table keys'''
         pass
 
 
 class DesignCursor(Iterator[Object]):
     '''
```

## Comparing `steptools-20.0.dist-info/LICENSE` & `steptools-20.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `steptools-20.0.dist-info/METADATA` & `steptools-20.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steptools
-Version: 20.0
+Version: 20.1
 Summary: STEP and STEP-NC (ISO 10303) native extension for large CAD/CAM/CAE models and machine tool interfaces.
 Author-email: "STEP Tools, Inc" <support@steptools.com>
 License: 
         STEP Python Interface
         END USER LICENSE AGREEMENT
         REDISTRIBUTION NOT PERMITTED        
         STEP Tools, Inc. ("STI") grants you ("Customer") a non-exclusive,
@@ -98,15 +98,15 @@
 instance) definitions below.  Click on any definition to get a text
 description of its meaning.
 
 - [STEP Concepts - ARM](https://www.steptools.com/stds/stp_expg/arm.html)
 - [STEP Data Definition - AIM](https://www.steptools.com/stds/stp_expg/aim.html)
 
 The `steptools` package is built for Windows, Linux and MacOSX, on
-Python 3.10 and up.
+Python 3.7 and up.
 
 ## About
 
 STEP Tools, Inc. is a commercial software company that has been
 building software infrastructure for STEP CAD, STEP-NC CAM/CNC, and
 IFC BIM tools since 1991.  We have deep technical knowledge of the ISO
 10303 and related standards.
```

