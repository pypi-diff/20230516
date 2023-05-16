# Comparing `tmp/simplesystray-0.0.3.tar.gz` & `tmp/simplesystray-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesystray-0.0.3.tar", last modified: Tue May 16 21:27:19 2023, max compression
+gzip compressed data, was "simplesystray-0.0.4.tar", last modified: Tue May 16 21:43:35 2023, max compression
```

## Comparing `simplesystray-0.0.3.tar` & `simplesystray-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.574449 simplesystray-0.0.3/
--rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5168 2023-05-16 21:27:19.573450 simplesystray-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4593 2023-05-16 21:24:31.000000 simplesystray-0.0.3/README.md
--rw-rw-rw-   0        0        0      563 2023-05-16 21:27:01.000000 simplesystray-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 21:27:19.574449 simplesystray-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.562450 simplesystray-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.566450 simplesystray-0.0.3/src/infi/
--rw-rw-rw-   0        0        0       57 2023-05-16 20:57:09.000000 simplesystray-0.0.3/src/infi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.568450 simplesystray-0.0.3/src/infi/systray/
--rw-rw-rw-   0        0        0       91 2023-05-16 20:57:09.000000 simplesystray-0.0.3/src/infi/systray/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-05-16 21:18:52.000000 simplesystray-0.0.3/src/infi/systray/traybar.py
--rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.3/src/infi/systray/win32_adapter.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.572450 simplesystray-0.0.3/src/simplesystray.egg-info/
--rw-rw-rw-   0        0        0     5168 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-16 21:27:19.000000 simplesystray-0.0.3/src/simplesystray.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 21:27:19.573450 simplesystray-0.0.3/tests/
--rw-rw-rw-   0        0        0      756 2023-05-16 21:23:04.000000 simplesystray-0.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:43:35.114934 simplesystray-0.0.4/
+-rw-rw-rw-   0        0        0     1499 2023-05-16 20:57:09.000000 simplesystray-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5764 2023-05-16 21:43:35.113932 simplesystray-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5189 2023-05-16 21:39:36.000000 simplesystray-0.0.4/README.md
+-rw-rw-rw-   0        0        0      563 2023-05-16 21:42:44.000000 simplesystray-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 21:43:35.114934 simplesystray-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 21:43:35.102940 simplesystray-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:43:35.106941 simplesystray-0.0.4/src/infi/
+-rw-rw-rw-   0        0        0       57 2023-05-16 20:57:09.000000 simplesystray-0.0.4/src/infi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:43:35.108942 simplesystray-0.0.4/src/infi/systray/
+-rw-rw-rw-   0        0        0       91 2023-05-16 20:57:09.000000 simplesystray-0.0.4/src/infi/systray/__init__.py
+-rw-rw-rw-   0        0        0    12084 2023-05-16 21:40:55.000000 simplesystray-0.0.4/src/infi/systray/traybar.py
+-rw-rw-rw-   0        0        0     6321 2023-05-16 20:57:09.000000 simplesystray-0.0.4/src/infi/systray/win32_adapter.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:43:35.111943 simplesystray-0.0.4/src/simplesystray.egg-info/
+-rw-rw-rw-   0        0        0     5764 2023-05-16 21:43:35.000000 simplesystray-0.0.4/src/simplesystray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-16 21:43:35.000000 simplesystray-0.0.4/src/simplesystray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:43:35.000000 simplesystray-0.0.4/src/simplesystray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-16 21:43:35.000000 simplesystray-0.0.4/src/simplesystray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:43:35.112934 simplesystray-0.0.4/tests/
+-rw-rw-rw-   0        0        0      756 2023-05-16 21:23:04.000000 simplesystray-0.0.4/tests/test.py
```

### Comparing `simplesystray-0.0.3/LICENSE` & `simplesystray-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.3/PKG-INFO` & `simplesystray-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-Metadata-Version: 2.1
-Name: simplesystray
-Version: 0.0.3
-Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
-Author-email: actorpus <alex@actorpus.com>
-Project-URL: Homepage, https://github.com/actorpus/systrayv2
-Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
-To install infi.systray, run:
+To install simplesystray, run:
 
 ```
 pip install simplesystray
 ```
 
-Alternatively, you can use easy_install.
-
 ## Usage
 
-Creating an icon with one option in the context menu:
+### Creating an icon with one option in the context menu:
 
 ```python
 from simplesystray import SysTrayIcon
 
 def say_hello(systray):
     print("Hello, World!")
     
-menu_options = (("Say Hello", None, say_hello),)
+menu_options = (("Say Hello", "hello.ico", say_hello),)
 systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
 systray.start()
 ```
 
 The first parameter to SysTrayIcon is a path to the icon to show in the systray. If the icon is not found, or
 if None is specified, a default system icon will be displayed.
 The second parameter is the hover text to show when the mouse is hovered over the systray icon.
 The traybar will run in its own thread, so the using script can continue to run.
 
-The icon and/or hover text can be updated using the update() method with the appropriate `hover_text` or `icon` keyword argument:
+For the parameters of `menu_options`: cf the section **Menu** below
+
+### Updating : icon, hover text and/or menu options
+The icon and/or hover text and/or menu options can be updated using the update() method with the appropriate `hover_text` or `icon` or  `menu_options` keyword argument:
 
+#### Updating the hover_text:
 ```python
 for item in ['item1', 'item2', 'item3']:
     systray.update(hover_text=item)
     do_something(item)
 ```
 
+#### Updating the menu options:
+```python
+def say_hello(systray):
+    systray.update(menu_options=menu_optionsbye)
+    
+def say_bye(systray):
+    systray.update(menu_options=menu_optionshello)
+    
+menu_optionshello = (("Say Hello","hello.ico", say_hello),)
+menu_optionsbye = (("Say Bye", "bye.ico", say_bye),)
+systray = SysTrayIcon("icon.ico", "Hello/Bye", menu_optionshello)   
+systray.start()
+```
+
+### Shutting down
 To destroy the icon when the program ends, call
 
 ```python
 systray.shutdown()
 ```
 
 SysTrayIcon can be used as a context manager to start and shutdown the tray, which also prevents hung tray threads should the parent thread fail or otherwise not close the tray process:
```

### Comparing `simplesystray-0.0.3/README.md` & `simplesystray-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,80 @@
+Metadata-Version: 2.1
+Name: simplesystray
+Version: 0.0.4
+Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
+Author-email: actorpus <alex@actorpus.com>
+Project-URL: Homepage, https://github.com/actorpus/systrayv2
+Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
-To install infi.systray, run:
+To install simplesystray, run:
 
 ```
 pip install simplesystray
 ```
 
-Alternatively, you can use easy_install.
-
 ## Usage
 
-Creating an icon with one option in the context menu:
+### Creating an icon with one option in the context menu:
 
 ```python
 from simplesystray import SysTrayIcon
 
 def say_hello(systray):
     print("Hello, World!")
     
-menu_options = (("Say Hello", None, say_hello),)
+menu_options = (("Say Hello", "hello.ico", say_hello),)
 systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
 systray.start()
 ```
 
 The first parameter to SysTrayIcon is a path to the icon to show in the systray. If the icon is not found, or
 if None is specified, a default system icon will be displayed.
 The second parameter is the hover text to show when the mouse is hovered over the systray icon.
 The traybar will run in its own thread, so the using script can continue to run.
 
-The icon and/or hover text can be updated using the update() method with the appropriate `hover_text` or `icon` keyword argument:
+For the parameters of `menu_options`: cf the section **Menu** below
+
+### Updating : icon, hover text and/or menu options
+The icon and/or hover text and/or menu options can be updated using the update() method with the appropriate `hover_text` or `icon` or  `menu_options` keyword argument:
 
+#### Updating the hover_text:
 ```python
 for item in ['item1', 'item2', 'item3']:
     systray.update(hover_text=item)
     do_something(item)
 ```
 
+#### Updating the menu options:
+```python
+def say_hello(systray):
+    systray.update(menu_options=menu_optionsbye)
+    
+def say_bye(systray):
+    systray.update(menu_options=menu_optionshello)
+    
+menu_optionshello = (("Say Hello","hello.ico", say_hello),)
+menu_optionsbye = (("Say Bye", "bye.ico", say_bye),)
+systray = SysTrayIcon("icon.ico", "Hello/Bye", menu_optionshello)   
+systray.start()
+```
+
+### Shutting down
 To destroy the icon when the program ends, call
 
 ```python
 systray.shutdown()
 ```
 
 SysTrayIcon can be used as a context manager to start and shutdown the tray, which also prevents hung tray threads should the parent thread fail or otherwise not close the tray process:
```

### Comparing `simplesystray-0.0.3/pyproject.toml` & `simplesystray-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simplesystray"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="actorpus", email="alex@actorpus.com" },
 ]
 description = "Adds support for a simple icon on the system tray, clone of infi-systray but maintained"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplesystray-0.0.3/src/infi/systray/traybar.py` & `simplesystray-0.0.4/src/infi/systray/traybar.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,19 @@
             auto_quit_button=True
     ):
 
         self._icon = icon
         self._icon_shared = False
         self._hover_text = hover_text
         self._on_quit = on_quit
+        self._auto_quit_button = auto_quit_button
 
         menu_options = menu_options or ()
 
-        if auto_quit_button:
+        if self._auto_quit_button:
             menu_options = menu_options + (('Quit', None, SysTrayIcon.QUIT),)
 
         self.menu_options_with_id = dict()
         self._next_action_id = SysTrayIcon.FIRST_ID
         self._menu_actions_by_id = set()
         self._menu_options = self._add_ids_to_menu_options(list(menu_options))
         self._menu_actions_by_id = dict(self._menu_actions_by_id)
@@ -114,33 +115,48 @@
         UpdateWindow(self._hwnd)
         self._refresh_icon()
 
     def _message_loop_func(self):
         self._create_window()
         PumpMessages()
 
-    def start(self):
+    def start(self, daemon=False):
         if self._hwnd:
             return  # already started
-        self._message_loop_thread = threading.Thread(target=self._message_loop_func)
+        self._message_loop_thread = threading.Thread(target=self._message_loop_func, daemon=daemon)
         self._message_loop_thread.start()
 
     def shutdown(self):
         if not self._hwnd:
             return  # not started
         PostMessage(self._hwnd, WM_CLOSE, 0, 0)
         self._message_loop_thread.join()
 
-    def update(self, icon=None, hover_text=None):
-        """ update icon image and/or hover text """
+    def update(self, icon=None, hover_text=None, menu_options=None):
+        """
+        update icon image and/or hover text and/or menu options
+        updating menu_options might be leaky, use with caution
+        """
         if icon:
             self._icon = icon
             self._load_icon()
+
         if hover_text:
             self._hover_text = hover_text
+
+        if menu_options:
+            if self._auto_quit_button:
+                menu_options = menu_options + (('Quit', None, SysTrayIcon.QUIT),)
+            self._next_action_id = SysTrayIcon.FIRST_ID
+            self._menu_actions_by_id = set()
+            self._menu_options = self._add_ids_to_menu_options(list(menu_options))
+            self._menu_actions_by_id = dict(self._menu_actions_by_id)
+            ctypes.windll.user32.DestroyMenu(self._menu)
+            self._menu = None
+
         self._refresh_icon()
 
     def get_options_menu_with_id(self):
         return self.menu_options_with_id
 
     def _add_ids_to_menu_options(self, menu_options):
         result = []
```

### Comparing `simplesystray-0.0.3/src/infi/systray/win32_adapter.py` & `simplesystray-0.0.4/src/infi/systray/win32_adapter.py`

 * *Files identical despite different names*

### Comparing `simplesystray-0.0.3/src/simplesystray.egg-info/PKG-INFO` & `simplesystray-0.0.4/src/simplesystray.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplesystray
-Version: 0.0.3
+Version: 0.0.4
 Summary: Adds support for a simple icon on the system tray, clone of infi-systray but maintained
 Author-email: actorpus <alex@actorpus.com>
 Project-URL: Homepage, https://github.com/actorpus/systrayv2
 Project-URL: Bug Tracker, https://github.com/actorpus/systrayv2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,50 +14,67 @@
 
 # `simplesystray` [![](https://img.shields.io/pypi/v/simplesystray)](https://pypi.org/project/simplesystray/)
 
 This module implements a Windows system tray icon with a right-click context menu.
 
 ## Installation
 
-To install infi.systray, run:
+To install simplesystray, run:
 
 ```
 pip install simplesystray
 ```
 
-Alternatively, you can use easy_install.
-
 ## Usage
 
-Creating an icon with one option in the context menu:
+### Creating an icon with one option in the context menu:
 
 ```python
 from simplesystray import SysTrayIcon
 
 def say_hello(systray):
     print("Hello, World!")
     
-menu_options = (("Say Hello", None, say_hello),)
+menu_options = (("Say Hello", "hello.ico", say_hello),)
 systray = SysTrayIcon("icon.ico", "Example tray icon", menu_options)
 systray.start()
 ```
 
 The first parameter to SysTrayIcon is a path to the icon to show in the systray. If the icon is not found, or
 if None is specified, a default system icon will be displayed.
 The second parameter is the hover text to show when the mouse is hovered over the systray icon.
 The traybar will run in its own thread, so the using script can continue to run.
 
-The icon and/or hover text can be updated using the update() method with the appropriate `hover_text` or `icon` keyword argument:
+For the parameters of `menu_options`: cf the section **Menu** below
+
+### Updating : icon, hover text and/or menu options
+The icon and/or hover text and/or menu options can be updated using the update() method with the appropriate `hover_text` or `icon` or  `menu_options` keyword argument:
 
+#### Updating the hover_text:
 ```python
 for item in ['item1', 'item2', 'item3']:
     systray.update(hover_text=item)
     do_something(item)
 ```
 
+#### Updating the menu options:
+```python
+def say_hello(systray):
+    systray.update(menu_options=menu_optionsbye)
+    
+def say_bye(systray):
+    systray.update(menu_options=menu_optionshello)
+    
+menu_optionshello = (("Say Hello","hello.ico", say_hello),)
+menu_optionsbye = (("Say Bye", "bye.ico", say_bye),)
+systray = SysTrayIcon("icon.ico", "Hello/Bye", menu_optionshello)   
+systray.start()
+```
+
+### Shutting down
 To destroy the icon when the program ends, call
 
 ```python
 systray.shutdown()
 ```
 
 SysTrayIcon can be used as a context manager to start and shutdown the tray, which also prevents hung tray threads should the parent thread fail or otherwise not close the tray process:
```

### Comparing `simplesystray-0.0.3/tests/test.py` & `simplesystray-0.0.4/tests/test.py`

 * *Files identical despite different names*

