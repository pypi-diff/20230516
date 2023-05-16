# Comparing `tmp/thunder_toolbox-0.0.4-py3-none-any.whl.zip` & `tmp/thunder_toolbox-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2961 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      629 b- defN 23-May-10 18:28 tool_box/__init__.py
+Zip file size: 2781 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      406 b- defN 23-May-16 18:25 tool_box/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-10 17:53 tool_box/key_typer/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-10 18:28 tool_box/key_typer/keyboard_tools.py
--rw-rw-r--  2.0 unx     1065 b- defN 23-May-10 18:39 thunder_toolbox-0.0.4.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      805 b- defN 23-May-10 18:39 thunder_toolbox-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-10 18:39 thunder_toolbox-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-10 18:39 thunder_toolbox-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      678 b- defN 23-May-10 18:39 thunder_toolbox-0.0.4.dist-info/RECORD
-8 files, 3278 bytes uncompressed, 1753 bytes compressed:  46.5%
+-rw-rw-r--  2.0 unx     1065 b- defN 23-May-16 18:28 thunder_toolbox-0.0.5.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      370 b- defN 23-May-16 18:28 thunder_toolbox-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-16 18:28 thunder_toolbox-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-16 18:28 thunder_toolbox-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      678 b- defN 23-May-16 18:28 thunder_toolbox-0.0.5.dist-info/RECORD
+8 files, 2620 bytes uncompressed, 1573 bytes compressed:  40.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: tool_box/key_typer/__init__.py
 Comment: 
 
 Filename: tool_box/key_typer/keyboard_tools.py
 Comment: 
 
-Filename: thunder_toolbox-0.0.4.dist-info/LICENCE.txt
+Filename: thunder_toolbox-0.0.5.dist-info/LICENCE.txt
 Comment: 
 
-Filename: thunder_toolbox-0.0.4.dist-info/METADATA
+Filename: thunder_toolbox-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: thunder_toolbox-0.0.4.dist-info/WHEEL
+Filename: thunder_toolbox-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: thunder_toolbox-0.0.4.dist-info/top_level.txt
+Filename: thunder_toolbox-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: thunder_toolbox-0.0.4.dist-info/RECORD
+Filename: thunder_toolbox-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tool_box/__init__.py

```diff
@@ -1,27 +1,18 @@
 import pyautogui
 import time
+from pyautogui import typewrite, press, write
 
 
 class KeyBoardTools:
 
     @staticmethod
     def printer(text):
         return print(text)
 
-    @staticmethod
-    def type_write(text, interval=None):
-        if not interval:
-            return pyautogui.write(text)
-        else:
-            return pyautogui.write(text, interval)
-
-    @staticmethod
-    def press_key(key):
-        return pyautogui.press(key)
 
     @staticmethod
     def spammer(text, count=0, freeze_time=3):
         time.sleep(freeze_time)
         for ctr in range(count):
             pyautogui.typewrite(text)
             pyautogui.press('enter')
```

## Comparing `thunder_toolbox-0.0.4.dist-info/LICENCE.txt` & `thunder_toolbox-0.0.5.dist-info/LICENCE.txt`

 * *Files identical despite different names*

