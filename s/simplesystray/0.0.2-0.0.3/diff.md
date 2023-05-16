# Comparing `tmp/simplesystray-0.0.2.tar.gz` & `tmp/simplesystray-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesystray-0.0.2.tar", last modified: Tue May 16 21:13:13 2023, max compression
+gzip compressed data, was "simplesystray-0.0.3.tar", last modified: Tue May 16 21:27:19 2023, max compression
```

## Comparing `simplesystray-0.0.2.tar` & `simplesystray-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:13:13.604478 simplesystray-0.0.2/
--rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5315 2023-05-16 21:13:13.603478 simplesystray-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4740 2023-05-16 21:09:47.000000 simplesystray-0.0.2/README.md
--rw-rw-rw-   0        0        0      563 2023-05-16 21:13:02.000000 simplesystray-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 21:13:13.604478 simplesystray-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 21:13:13.591477 simplesystray-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:13:13.595478 simplesystray-0.0.2/src/infi/
--rw-rw-rw-   0        0        0       57 2023-05-16 20:57:09.000000 simplesystray-0.0.2/src/infi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:13:13.597478 simplesystray-0.0.2/src/infi/systray/
--rw-rw-rw-   0        0        0       91 2023-05-16 20:57:09.000000 simplesystray-0.0.2/src/infi/systray/__init__.py
--rw-rw-rw-   0        0        0    11495 2023-05-16 20:57:09.000000 simplesystray-0.0.2/src/infi/systray/traybar.py
--rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.2/src/infi/systray/win32_adapter.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:13:13.601481 simplesystray-0.0.2/src/simplesystray.egg-info/
--rw-rw-rw-   0        0        0     5315 2023-05-16 21:13:13.000000 simplesystray-0.0.2/src/simplesystray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-16 21:13:13.000000 simplesystray-0.0.2/src/simplesystray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 21:13:13.000000 simplesystray-0.0.2/src/simplesystray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-16 21:13:13.000000 simplesystray-0.0.2/src/simplesystray.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 21:13:13.602477 simplesystray-0.0.2/tests/
--rw-rw-rw-   0        0        0      582 2023-05-16 20:57:09.000000 simplesystray-0.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.574449 simplesystray-0.0.3/
+-rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5168 2023-05-16 21:27:19.573450 simplesystray-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4593 2023-05-16 21:24:31.000000 simplesystray-0.0.3/README.md
+-rw-rw-rw-   0        0        0      563 2023-05-16 21:27:01.000000 simplesystray-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 21:27:19.574449 simplesystray-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.562450 simplesystray-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.566450 simplesystray-0.0.3/src/infi/
+-rw-rw-rw-   0        0        0       57 2023-05-16 20:57:09.000000 simplesystray-0.0.3/src/infi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.568450 simplesystray-0.0.3/src/infi/systray/
+-rw-rw-rw-   0        0        0       91 2023-05-16 20:57:09.000000 simplesystray-0.0.3/src/infi/systray/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-05-16 21:18:52.000000 simplesystray-0.0.3/src/infi/systray/traybar.py
+-rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.3/src/infi/systray/win32_adapter.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.572450 simplesystray-0.0.3/src/simplesystray.egg-info/
+-rw-rw-rw-   0        0        0     5168 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.573450 simplesystray-0.0.3/tests/
+-rw-rw-rw-   0        0        0      756 2023-05-16 21:23:04.000000 simplesystray-0.0.3/tests/test.py
```

### Comparing `simplesystray-0.0.2/LICENSE` & `simplesystray-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.2/PKG-INFO` & `simplesystray-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: simplesystray
-Version: 0.0.2
+Version: 0.0.3
 Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
 Author-email: actorpus <alex@actorpus.com>
 Project-URL: Homepage, https://github.com/actorpus/systrayv2
 Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `infi.systray` [![](https://img.shields.io/pypi/v/simplesystray-actorpus)](https://pypi.org/project/simplesystray-actorpus/)
+# `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
 To install infi.systray, run:
 
 ```
-pip install infi.systray
+pip install simplesystray
 ```
 
 Alternatively, you can use easy_install.
 
 ## Usage
 
 Creating an icon with one option in the context menu:
 
 ```python
-from infi.systray import SysTrayIcon
+from simplesystray import SysTrayIcon
 
 def say_hello(systray):
     print("Hello, World!")
     
 menu_options = (("Say Hello", None, say_hello),)
 systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
 systray.start()
@@ -92,15 +92,15 @@
 the second value of the tuples. If None is passed, no icon is displayed for the option.
 The third value is the command to execute when the context menu is selected by the user.
 
 It is possible to create sub-menus in the context menu by recursively passing a list of 3-tuple options as the third
 value of an option, instead of passing a callback function. e.g.
 
 ```python
-from infi.systray import SysTrayIcon
+from simplesystray import SysTrayIcon
 
 hover_text = "SysTrayIcon Demo"
 
 
 def hello(sysTrayIcon):
     print("Hello World.")
     
@@ -130,18 +130,10 @@
 interrupts, some code must be written that will call systray.shutdown when the program should quit.
 Using SysTrayIcon as a context manager automates the start and shutdown of the tray.
 
 This module can only be used in Windows systems, otherwise the import statement will fail.
 
 ## Credit
 
-This module is adapted from an implementation by Simon Brunning, which in turn was adapted from Mark Hammond's
+This module is adapted from an implementation by Infinidat Ltd. this was a clone on Simon Brunning's version, which in turn was adapted from Mark Hammond's
 win32gui_taskbar.py and win32gui_menu.py demos from PyWin32.
 
-# Checking out the code
-
-To run this code from the repository for development purposes, run the following:
-
-```
-easy_install -U infi.projector
-projector devenv build
-```
```

### Comparing `simplesystray-0.0.2/README.md` & `simplesystray-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# `infi.systray` [![](https://img.shields.io/pypi/v/simplesystray-actorpus)](https://pypi.org/project/simplesystray-actorpus/)
+# `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
 To install infi.systray, run:
 
 ```
-pip install infi.systray
+pip install simplesystray
 ```
 
 Alternatively, you can use easy_install.
 
 ## Usage
 
 Creating an icon with one option in the context menu:
 
 ```python
-from infi.systray import SysTrayIcon
+from simplesystray import SysTrayIcon
 
 def say_hello(systray):
     print("Hello, World!")
     
 menu_options = (("Say Hello", None, say_hello),)
 systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
 systray.start()
@@ -78,15 +78,15 @@
 the second value of the tuples. If None is passed, no icon is displayed for the option.
 The third value is the command to execute when the context menu is selected by the user.
 
 It is possible to create sub-menus in the context menu by recursively passing a list of 3-tuple options as the third
 value of an option, instead of passing a callback function. e.g.
 
 ```python
-from infi.systray import SysTrayIcon
+from simplesystray import SysTrayIcon
 
 hover_text = "SysTrayIcon Demo"
 
 
 def hello(sysTrayIcon):
     print("Hello World.")
     
@@ -116,18 +116,10 @@
 interrupts, some code must be written that will call systray.shutdown when the program should quit.
 Using SysTrayIcon as a context manager automates the start and shutdown of the tray.
 
 This module can only be used in Windows systems, otherwise the import statement will fail.
 
 ## Credit
 
-This module is adapted from an implementation by Simon Brunning, which in turn was adapted from Mark Hammond's
+This module is adapted from an implementation by Infinidat Ltd. this was a clone on Simon Brunning's version, which in turn was adapted from Mark Hammond's
 win32gui_taskbar.py and win32gui_menu.py demos from PyWin32.
 
-# Checking out the code
-
-To run this code from the repository for development purposes, run the following:
-
-```
-easy_install -U infi.projector
-projector devenv build
-```
```

### Comparing `simplesystray-0.0.2/pyproject.toml` & `simplesystray-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simplesystray"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="actorpus", email="alex@actorpus.com" },
 ]
 description = "Adds support for a simple icon on the system tray, clone of infi-systray but maintained"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplesystray-0.0.2/src/infi/systray/traybar.py` & `simplesystray-0.0.3/src/infi/systray/traybar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from .win32_adapter import *
 import threading
 import uuid
 
+
 class SysTrayIcon(object):
     """
     menu_options: tuple of tuples (menu text, menu icon path or None, function name)
 
     menu text and tray hover text should be Unicode
     hover_text length is limited to 128; longer text will be truncated
 
@@ -20,47 +21,50 @@
 
     """
     QUIT = 'QUIT'
     SPECIAL_ACTIONS = [QUIT]
 
     FIRST_ID = 1023
 
-    def __init__(self,
-                 icon,
-                 hover_text,
-                 menu_options=None,
-                 on_quit=None,
-                 default_menu_index=None,
-                 window_class_name=None,
-                 auto_quit_button=True):
+    def __init__(
+            self,
+            icon,
+            hover_text,
+            menu_options=None,
+            on_quit=None,
+            default_menu_index=None,
+            window_class_name=None,
+            auto_quit_button=True
+    ):
 
         self._icon = icon
         self._icon_shared = False
         self._hover_text = hover_text
         self._on_quit = on_quit
 
         menu_options = menu_options or ()
-        
+
         if auto_quit_button:
             menu_options = menu_options + (('Quit', None, SysTrayIcon.QUIT),)
-        
+
+        self.menu_options_with_id = dict()
         self._next_action_id = SysTrayIcon.FIRST_ID
         self._menu_actions_by_id = set()
         self._menu_options = self._add_ids_to_menu_options(list(menu_options))
         self._menu_actions_by_id = dict(self._menu_actions_by_id)
 
         window_class_name = window_class_name or ("SysTrayIconPy-%s" % (str(uuid.uuid4())))
 
         self._default_menu_index = (default_menu_index or 0)
         self._window_class_name = encode_for_locale(window_class_name)
         self._message_dict = {RegisterWindowMessage("TaskbarCreated"): self._restart,
                               WM_DESTROY: self._destroy,
                               WM_CLOSE: self._destroy,
                               WM_COMMAND: self._command,
-                              WM_USER+20: self._notify}
+                              WM_USER + 20: self._notify}
         self._notify_id = None
         self._message_loop_thread = None
         self._hwnd = None
         self._hicon = 0
         self._hinst = None
         self._window_class = None
         self._menu = None
@@ -92,65 +96,71 @@
         self._window_class.hCursor = LoadCursor(0, IDC_ARROW)
         self._window_class.hbrBackground = COLOR_WINDOW
         self._window_class.lpfnWndProc = LPFN_WNDPROC(self.WndProc)
         RegisterClass(ctypes.byref(self._window_class))
 
     def _create_window(self):
         style = WS_OVERLAPPED | WS_SYSMENU
-        self._hwnd = CreateWindowEx(0, self._window_class_name,
-                                      self._window_class_name,
-                                      style,
-                                      0,
-                                      0,
-                                      CW_USEDEFAULT,
-                                      CW_USEDEFAULT,
-                                      0,
-                                      0,
-                                      self._hinst,
-                                      None)
+        self._hwnd = CreateWindowEx(
+            0, self._window_class_name,
+            self._window_class_name,
+            style,
+            0, 0,
+            CW_USEDEFAULT,
+            CW_USEDEFAULT,
+            0, 0,
+            self._hinst,
+            None
+        )
         UpdateWindow(self._hwnd)
         self._refresh_icon()
 
     def _message_loop_func(self):
         self._create_window()
         PumpMessages()
 
     def start(self):
         if self._hwnd:
-            return      # already started
+            return  # already started
         self._message_loop_thread = threading.Thread(target=self._message_loop_func)
         self._message_loop_thread.start()
 
     def shutdown(self):
         if not self._hwnd:
-            return      # not started
+            return  # not started
         PostMessage(self._hwnd, WM_CLOSE, 0, 0)
         self._message_loop_thread.join()
 
     def update(self, icon=None, hover_text=None):
         """ update icon image and/or hover text """
         if icon:
             self._icon = icon
             self._load_icon()
         if hover_text:
             self._hover_text = hover_text
         self._refresh_icon()
 
+    def get_options_menu_with_id(self):
+        return self.menu_options_with_id
+
     def _add_ids_to_menu_options(self, menu_options):
         result = []
         for menu_option in menu_options:
             option_text, option_icon, option_action = menu_option
             if callable(option_action) or option_action in SysTrayIcon.SPECIAL_ACTIONS:
                 self._menu_actions_by_id.add((self._next_action_id, option_action))
                 result.append(menu_option + (self._next_action_id,))
+                self.menu_options_with_id[option_text] = self._next_action_id
             elif non_string_iterable(option_action):
-                result.append((option_text,
-                               option_icon,
-                               self._add_ids_to_menu_options(option_action),
-                               self._next_action_id))
+                result.append((
+                    option_text,
+                    option_icon,
+                    self._add_ids_to_menu_options(option_action),
+                    self._next_action_id
+                ))
             else:
                 raise Exception('Unknown item', option_text, option_icon, option_action)
             self._next_action_id += 1
         return result
 
     def _load_icon(self):
         # release previous icon, if a custom one was loaded
@@ -180,20 +190,22 @@
             return
         if self._hicon == 0:
             self._load_icon()
         if self._notify_id:
             message = NIM_MODIFY
         else:
             message = NIM_ADD
-        self._notify_id = NotifyData(self._hwnd,
-                          0,
-                          NIF_ICON | NIF_MESSAGE | NIF_TIP,
-                          WM_USER+20,
-                          self._hicon,
-                          self._hover_text)
+        self._notify_id = NotifyData(
+            self._hwnd,
+            0,
+            NIF_ICON | NIF_MESSAGE | NIF_TIP,
+            WM_USER + 20,
+            self._hicon,
+            self._hover_text
+        )
         Shell_NotifyIcon(message, ctypes.byref(self._notify_id))
 
     def _restart(self, hwnd, msg, wparam, lparam):
         self._refresh_icon()
 
     def _destroy(self, hwnd, msg, wparam, lparam):
         if self._on_quit:
@@ -217,15 +229,15 @@
             pass
         return True
 
     def _show_menu(self):
         if self._menu is None:
             self._menu = CreatePopupMenu()
             self._create_menu(self._menu, self._menu_options)
-            #SetMenuDefaultItem(self._menu, 1000, 0)
+            # SetMenuDefaultItem(self._menu, 1000, 0)
 
         pos = POINT()
         GetCursorPos(ctypes.byref(pos))
         # See http://msdn.microsoft.com/library/default.asp?url=/library/en-us/winui/menus_0hdi.asp
         SetForegroundWindow(self._hwnd)
         TrackPopupMenu(self._menu,
                        TPM_LEFTALIGN,
@@ -248,15 +260,15 @@
                 InsertMenuItem(menu, 0, 1, ctypes.byref(item))
             else:
                 submenu = CreatePopupMenu()
                 self._create_menu(submenu, option_action)
                 item = PackMENUITEMINFO(text=option_text,
                                         hbmpItem=option_icon,
                                         hSubMenu=submenu)
-                InsertMenuItem(menu, 0, 1,  ctypes.byref(item))
+                InsertMenuItem(menu, 0, 1, ctypes.byref(item))
 
     def _prep_menu_icon(self, icon):
         icon = encode_for_locale(icon)
         # First load the icon.
         ico_x = GetSystemMetrics(SM_CXSMICON)
         ico_y = GetSystemMetrics(SM_CYSMICON)
         hicon = LoadImage(0, icon, IMAGE_ICON, ico_x, ico_y, LR_LOADFROMFILE)
@@ -283,15 +295,16 @@
         self._execute_menu_option(id)
 
     def _execute_menu_option(self, id):
         menu_action = self._menu_actions_by_id[id]
         if menu_action == SysTrayIcon.QUIT:
             DestroyWindow(self._hwnd)
         else:
-            menu_action(self)
+            menu_action(self, id)
+
 
 def non_string_iterable(obj):
     try:
         iter(obj)
     except TypeError:
         return False
     else:
```

### Comparing `simplesystray-0.0.2/src/infi/systray/win32_adapter.py` & `simplesystray-0.0.3/src/infi/systray/win32_adapter.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.2/src/simplesystray.egg-info/PKG-INFO` & `simplesystray-0.0.3/src/simplesystray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: simplesystray
-Version: 0.0.2
+Version: 0.0.3
 Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
 Author-email: actorpus <alex@actorpus.com>
 Project-URL: Homepage, https://github.com/actorpus/systrayv2
 Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `infi.systray` [![](https://img.shields.io/pypi/v/simplesystray-actorpus)](https://pypi.org/project/simplesystray-actorpus/)
+# `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
 To install infi.systray, run:
 
 ```
-pip install infi.systray
+pip install simplesystray
 ```
 
 Alternatively, you can use easy_install.
 
 ## Usage
 
 Creating an icon with one option in the context menu:
 
 ```python
-from infi.systray import SysTrayIcon
+from simplesystray import SysTrayIcon
 
 def say_hello(systray):
     print("Hello, World!")
     
 menu_options = (("Say Hello", None, say_hello),)
 systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
 systray.start()
@@ -92,15 +92,15 @@
 the second value of the tuples. If None is passed, no icon is displayed for the option.
 The third value is the command to execute when the context menu is selected by the user.
 
 It is possible to create sub-menus in the context menu by recursively passing a list of 3-tuple options as the third
 value of an option, instead of passing a callback function. e.g.
 
 ```python
-from infi.systray import SysTrayIcon
+from simplesystray import SysTrayIcon
 
 hover_text = "SysTrayIcon Demo"
 
 
 def hello(sysTrayIcon):
     print("Hello World.")
     
@@ -130,18 +130,10 @@
 interrupts, some code must be written that will call systray.shutdown when the program should quit.
 Using SysTrayIcon as a context manager automates the start and shutdown of the tray.
 
 This module can only be used in Windows systems, otherwise the import statement will fail.
 
 ## Credit
 
-This module is adapted from an implementation by Simon Brunning, which in turn was adapted from Mark Hammond's
+This module is adapted from an implementation by Infinidat Ltd. this was a clone on Simon Brunning's version, which in turn was adapted from Mark Hammond's
 win32gui_taskbar.py and win32gui_menu.py demos from PyWin32.
 
-# Checking out the code
-
-To run this code from the repository for development purposes, run the following:
-
-```
-easy_install -U infi.projector
-projector devenv build
-```
```

