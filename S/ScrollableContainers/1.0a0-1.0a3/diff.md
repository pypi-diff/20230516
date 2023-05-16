# Comparing `tmp/ScrollableContainers-1.0a0.tar.gz` & `tmp/ScrollableContainers-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScrollableContainers-1.0a0.tar", last modified: Sat Feb  4 16:24:35 2023, max compression
+gzip compressed data, was "ScrollableContainers-1.0a3.tar", last modified: Sat Mar  4 15:23:40 2023, max compression
```

## Comparing `ScrollableContainers-1.0a0.tar` & `ScrollableContainers-1.0a3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0 tfpf      (1000) tfpf      (1000)        0 2023-02-04 16:24:35.495633 ScrollableContainers-1.0a0/
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)     2329 2023-02-04 16:24:35.479976 ScrollableContainers-1.0a0/PKG-INFO
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)     1821 2023-02-04 13:19:51.000000 ScrollableContainers-1.0a0/README.md
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)      604 2023-02-04 16:22:57.000000 ScrollableContainers-1.0a0/pyproject.toml
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)       38 2023-02-04 16:24:35.495633 ScrollableContainers-1.0a0/setup.cfg
-drwxrwxrwx   0 tfpf      (1000) tfpf      (1000)        0 2023-02-04 16:24:34.993644 ScrollableContainers-1.0a0/src/
-drwxrwxrwx   0 tfpf      (1000) tfpf      (1000)        0 2023-02-04 16:24:35.213017 ScrollableContainers-1.0a0/src/ScrollableContainers/
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)     7088 2023-02-03 15:17:06.000000 ScrollableContainers-1.0a0/src/ScrollableContainers/Tk.py
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)      739 2023-01-31 09:54:02.000000 ScrollableContainers-1.0a0/src/ScrollableContainers/Wx.py
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)        0 2023-01-30 15:18:10.000000 ScrollableContainers-1.0a0/src/ScrollableContainers/__init__.py
-drwxrwxrwx   0 tfpf      (1000) tfpf      (1000)        0 2023-02-04 16:24:35.432658 ScrollableContainers-1.0a0/src/ScrollableContainers.egg-info/
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)     2329 2023-02-04 16:24:34.000000 ScrollableContainers-1.0a0/src/ScrollableContainers.egg-info/PKG-INFO
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)      315 2023-02-04 16:24:34.000000 ScrollableContainers-1.0a0/src/ScrollableContainers.egg-info/SOURCES.txt
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)        1 2023-02-04 16:24:34.000000 ScrollableContainers-1.0a0/src/ScrollableContainers.egg-info/dependency_links.txt
--rwxrwxrwx   0 tfpf      (1000) tfpf      (1000)       21 2023-02-04 16:24:34.000000 ScrollableContainers-1.0a0/src/ScrollableContainers.egg-info/top_level.txt
+drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-03-04 15:23:40.294310 ScrollableContainers-1.0a3/
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)     3086 2023-03-04 15:23:40.294310 ScrollableContainers-1.0a3/PKG-INFO
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)     2578 2023-03-04 08:09:35.000000 ScrollableContainers-1.0a3/README.md
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)      605 2023-03-02 10:16:09.000000 ScrollableContainers-1.0a3/pyproject.toml
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)       38 2023-03-04 15:23:40.294310 ScrollableContainers-1.0a3/setup.cfg
+drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-03-04 15:23:40.290976 ScrollableContainers-1.0a3/src/
+drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-03-04 15:23:40.294310 ScrollableContainers-1.0a3/src/ScrollableContainers/
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)      697 2023-03-04 08:09:35.000000 ScrollableContainers-1.0a3/src/ScrollableContainers/Qt5.py
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)     6328 2023-02-24 09:38:19.000000 ScrollableContainers-1.0a3/src/ScrollableContainers/Tk.py
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)      635 2023-03-02 10:03:21.000000 ScrollableContainers-1.0a3/src/ScrollableContainers/Wx.py
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)        0 2023-02-24 05:21:49.000000 ScrollableContainers-1.0a3/src/ScrollableContainers/__init__.py
+drwxr-xr-x   0 tfpf      (1000) tfpf      (1000)        0 2023-03-04 15:23:40.294310 ScrollableContainers-1.0a3/src/ScrollableContainers.egg-info/
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)     3086 2023-03-04 15:23:40.000000 ScrollableContainers-1.0a3/src/ScrollableContainers.egg-info/PKG-INFO
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)      347 2023-03-04 15:23:40.000000 ScrollableContainers-1.0a3/src/ScrollableContainers.egg-info/SOURCES.txt
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)        1 2023-03-04 15:23:40.000000 ScrollableContainers-1.0a3/src/ScrollableContainers.egg-info/dependency_links.txt
+-rw-r--r--   0 tfpf      (1000) tfpf      (1000)       21 2023-03-04 15:23:40.000000 ScrollableContainers-1.0a3/src/ScrollableContainers.egg-info/top_level.txt
```

### Comparing `ScrollableContainers-1.0a0/PKG-INFO` & `ScrollableContainers-1.0a3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScrollableContainers
-Version: 1.0a0
+Version: 1.0a3
 Summary: Scrollable containers for some GUI toolkits
 Author: Vishal Pankaj Chandratreya
 Project-URL: Homepage, https://github.com/tfpf/ScrollableContainers
 Project-URL: Bug Tracker, https://github.com/tfpf/ScrollableContainers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,38 +12,60 @@
 Description-Content-Type: text/markdown
 
 # Scrollable containers which *just work*!
 If you have developed GUI applications, you probably know the pain of designing a clean front-end only to find that
 your application window is too large for your client's screen. Making the content scrollable is not straightforward (at
 least in Tkinter). Especially not after you have already written a lot of code to draw the content.
 
-You can use `ScrollableContainers` to reduce headaches. Run the following command to install the package.
+You can use `ScrollableContainers` to reduce headaches.
+[It's available on PyPI!](https://pypi.org/project/ScrollableContainers/)
 
 ```shell
 pip install ScrollableContainers
 ```
 
-## `ScrollableFrameTk`
-A full implementation of a scrollable frame in Tkinter.
+Scrollable containers are currently available for the following GUI toolkits.
+* [Tkinter](#Tkinter)
+* [wxPython](#wxPython)
+* [PyQt5](#PyQt5)
+
+# Tkinter
+`ScrollableContainers.Tk.ScrollableFrameTk`: a comprehensive implementation of a scrollable frame, and the flagship
+class of this project. (I wrote the other classes just for completeness.)
+
+### Usage
+Add widgets to the `frame` attribute of a `ScrollableFrameTk` object.
+[See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableFrameTk.py)
+
+### Features
 * Handles resize events correctly.
-* Horizontally centres the contents if the window is wider.
 * Supports scrolling with the mouse wheel and touchpad.
   * Scrolling the mouse wheel or swiping vertically with two fingers on the touchpad triggers a vertical scroll.
   * Scrolling the mouse wheel while holding down Shift or swiping horizontally with two fingers on the touchpad
     triggers a horizontal scroll.
-
-### Usage
-Add widgets to the `frame` attribute of a `ScrollableFrameTk` object.
-[See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableFrameTk.py)
+* Horizontally centres the contents if the window is wider.
 
 ### Notes
 `'<Button-4>'`, `'<Button-5>'` and `'<MouseWheel>'` are bound to all widgets using `bind_all` to handle mouse wheel
 scroll events. Do not `unbind_all` (or `bind_all` another function to) these three sequences!
 
-## `ScrollablePanelWx`
-A thin wrapper around `wx.lib.scrolledpanel.ScrolledPanel`.
-* Does everything the aforementioned class does.
-* Horizontally centres the contents if the window is wider.
+# wxPython
+`ScrollableContainers.Wx.ScrollablePanelWx`: a thin wrapper around `wx.lib.scrolledpanel.ScrolledPanel`.
 
 ### Usage
 Add widgets to the `panel` attribute of a `ScrollablePanelWx` object.
 [See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollablePanelWx.py)
+
+### Features
+* Does everything the wrapped class does.
+* Horizontally centres the contents if the window is wider.
+
+# PyQt5
+`ScrollableContainers.Qt5.ScrollableAreaQt5`: a thin wrapper around `PyQt5.QtWidgets.QScrollArea`.
+
+### Usage
+Add widgets to the `area` attribute of a `ScrollableAreaQt5` object.
+[See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableAreaQt5.py)
+
+### Features
+* Does everything the wrapped class does.
+* Horizontally centres the contents if the window is wider.
```

### Comparing `ScrollableContainers-1.0a0/README.md` & `ScrollableContainers-1.0a3/src/ScrollableContainers.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,71 @@
+Metadata-Version: 2.1
+Name: ScrollableContainers
+Version: 1.0a3
+Summary: Scrollable containers for some GUI toolkits
+Author: Vishal Pankaj Chandratreya
+Project-URL: Homepage, https://github.com/tfpf/ScrollableContainers
+Project-URL: Bug Tracker, https://github.com/tfpf/ScrollableContainers/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # Scrollable containers which *just work*!
 If you have developed GUI applications, you probably know the pain of designing a clean front-end only to find that
 your application window is too large for your client's screen. Making the content scrollable is not straightforward (at
 least in Tkinter). Especially not after you have already written a lot of code to draw the content.
 
-You can use `ScrollableContainers` to reduce headaches. Run the following command to install the package.
+You can use `ScrollableContainers` to reduce headaches.
+[It's available on PyPI!](https://pypi.org/project/ScrollableContainers/)
 
 ```shell
 pip install ScrollableContainers
 ```
 
-## `ScrollableFrameTk`
-A full implementation of a scrollable frame in Tkinter.
+Scrollable containers are currently available for the following GUI toolkits.
+* [Tkinter](#Tkinter)
+* [wxPython](#wxPython)
+* [PyQt5](#PyQt5)
+
+# Tkinter
+`ScrollableContainers.Tk.ScrollableFrameTk`: a comprehensive implementation of a scrollable frame, and the flagship
+class of this project. (I wrote the other classes just for completeness.)
+
+### Usage
+Add widgets to the `frame` attribute of a `ScrollableFrameTk` object.
+[See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableFrameTk.py)
+
+### Features
 * Handles resize events correctly.
-* Horizontally centres the contents if the window is wider.
 * Supports scrolling with the mouse wheel and touchpad.
   * Scrolling the mouse wheel or swiping vertically with two fingers on the touchpad triggers a vertical scroll.
   * Scrolling the mouse wheel while holding down Shift or swiping horizontally with two fingers on the touchpad
     triggers a horizontal scroll.
-
-### Usage
-Add widgets to the `frame` attribute of a `ScrollableFrameTk` object.
-[See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableFrameTk.py)
+* Horizontally centres the contents if the window is wider.
 
 ### Notes
 `'<Button-4>'`, `'<Button-5>'` and `'<MouseWheel>'` are bound to all widgets using `bind_all` to handle mouse wheel
 scroll events. Do not `unbind_all` (or `bind_all` another function to) these three sequences!
 
-## `ScrollablePanelWx`
-A thin wrapper around `wx.lib.scrolledpanel.ScrolledPanel`.
-* Does everything the aforementioned class does.
-* Horizontally centres the contents if the window is wider.
+# wxPython
+`ScrollableContainers.Wx.ScrollablePanelWx`: a thin wrapper around `wx.lib.scrolledpanel.ScrolledPanel`.
 
 ### Usage
 Add widgets to the `panel` attribute of a `ScrollablePanelWx` object.
 [See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollablePanelWx.py)
+
+### Features
+* Does everything the wrapped class does.
+* Horizontally centres the contents if the window is wider.
+
+# PyQt5
+`ScrollableContainers.Qt5.ScrollableAreaQt5`: a thin wrapper around `PyQt5.QtWidgets.QScrollArea`.
+
+### Usage
+Add widgets to the `area` attribute of a `ScrollableAreaQt5` object.
+[See examples.](https://github.com/tfpf/ScrollableContainers/blob/main/examples/examples_ScrollableAreaQt5.py)
+
+### Features
+* Does everything the wrapped class does.
+* Horizontally centres the contents if the window is wider.
```

### Comparing `ScrollableContainers-1.0a0/pyproject.toml` & `ScrollableContainers-1.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ScrollableContainers"
-version = "1.0a"
+version = "1.0a3"
 authors = [
     { name="Vishal Pankaj Chandratreya" },
 ]
 description = "Scrollable containers for some GUI toolkits"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ScrollableContainers-1.0a0/src/ScrollableContainers/Tk.py` & `ScrollableContainers-1.0a3/src/ScrollableContainers/Tk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-#! /usr/bin/python3 -B
+__all__ = ['ScrollableFrameTk']
 
 import platform
 import tkinter as tk
 import tkinter.ttk as ttk
 
-__all__ = ['ScrollableFrameTk']
-
 _system = platform.system()
 
-###############################################################################
 
 class ScrollableFrameTk(ttk.Frame):
-    '''
+    """
 Container with horizontal and vertical scrolling capabilities. Widgets must be
 added to its `frame` attribute.
-    '''
+    """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Scrollable canvas. This is the widget which actually manages
         # scrolling. Using the grid geometry manager ensures that the
         # horizontal and vertical scrollbars do not meet.
@@ -44,140 +41,116 @@
 
         # Initially, the vertical scrollbar is a hair below its topmost
         # position. Move it to said position. No harm in doing the equivalent
         # for the horizontal scrollbar.
         self._canvas.xview_moveto(0.0)
         self._canvas.yview_moveto(0.0)
 
-    ###########################################################################
-
     def _xview(self, *args, width=None):
-        '''
+        """
 Called when a horizontal scroll is requested. Called by some other callbacks
 (`_on_canvas_configure` and `_on_frame_configure`) whenever it is necessary to
 horizontally realign the contents of the canvas. Scroll the view only if the
 contents are not completely visible. Otherwise, move the scrollbar to such a
 position that they are horizontally centred.
 
 :param args: Tuple which can be passed to `tkinter.Canvas.xview`.
 :param width: Width of the canvas.
-        '''
-
+        """
         if self._canvas.xview() != (0.0, 1.0):
             self._canvas.xview(*args)
         else:
             width = width or self._canvas.winfo_width()
 
             # To move the contents of the canvas to the centre, I call this
             # function with a negative argument. I don't know if this hack is
             # supported (because the Tcl/Tk manual pages say that it must be a
             # fraction between 0 and 1), but it works!
             self._canvas.xview_moveto((1 - width / self.frame.winfo_width()) / 2)
 
-    ###########################################################################
-
     def _yview(self, *args):
-        '''
+        """
 Called when a vertical scroll is requested. Scroll the view only if the
 contents are not completely visible.
 
 :param args: Tuple which can be passed to `tkinter.Canvas.yview`.
-        '''
-
+        """
         if self._canvas.yview() != (0.0, 1.0):
             self._canvas.yview(*args)
 
-    ###########################################################################
-
     def _on_canvas_configure(self, event):
-        '''
+        """
 Called when the canvas is resized. Update the scrollable region.
 
 :param event: Configure event.
-        '''
-
+        """
         self._canvas.configure(scrollregion=self._canvas.bbox(tk.ALL))
         self._xview(tk.SCROLL, 0, tk.UNITS, width=event.width)
 
-    ###########################################################################
-
     def _on_frame_configure(self, event=None):
-        '''
+        """
 Called when the frame is resized or the canvas is scrolled. Update the
 scrollable region.
 
 This method is necessary to handle updates which may occur after the GUI loop
 has started.
 
 :param event: Configure event.
-        '''
-
+        """
         self._canvas.configure(scrollregion=self._canvas.bbox(tk.ALL))
         self._xview(tk.SCROLL, 0, tk.UNITS)
 
-    ###########################################################################
-
     def _on_frame_expose(self, event=None):
-        '''
+        """
 Called when the frame becomes visible. Call `_on_frame_configure` and then
 disable this callback.
 
 This method is necessary because if a scrollable frame is put into, say, a
 notebook (as opposed to a toplevel window), and the canvas is wider than its
 contents, then (on Linux) the contents are not initially horizontally centred.
 (This issue is not observed on Windows, probably because its frame configure
 events work differently.) Hence, I try to centre the contents again upon an
 expose event.
 
 :param event: Expose event.
-        '''
-
+        """
         self._on_frame_configure()
         self.frame.unbind('<Expose>', self._on_frame_expose_id)
 
-    ###########################################################################
-
     def _on_canvas_enter(self, event=None):
-        '''
+        """
 Called when the mouse pointer enters the canvas. Set up vertical scrolling with
 the mouse wheel.
 
 :param event: Enter event.
-        '''
-
+        """
         self.bind_all('<Button-4>', self._on_mouse_scroll)
         self.bind_all('<Button-5>', self._on_mouse_scroll)
         self.bind_all('<MouseWheel>', self._on_mouse_scroll)
 
-    ###########################################################################
-
     def _on_canvas_leave(self, event=None):
-        '''
+        """
 Called when the mouse pointer leaves the canvas. Unset vertical scrolling with
 the mouse wheel.
 
 :param event: Leave event.
-        '''
-
+        """
         self.unbind_all('<Button-4>')
         self.unbind_all('<Button-5>')
         self.unbind_all('<MouseWheel>')
 
-    ###########################################################################
-
     def _on_mouse_scroll(self, event):
-        '''
+        """
 Called when the mouse wheel is scrolled or a two-finger swipe gesture is
 performed on the touchpad. Ask to scroll the view horizontally if the mouse
 wheel is scrolled with Shift held down (equivalent to a horizontal two-finger
 swipe) and vertically otherwise (equivalent to a vertical two-finger swipe).
 
 :param event: Scroll event.
-        '''
-
+        """
         # Select which method to call based on whether Shift was held down.
         # This is indicated by the LSB of the state.
         if event.state & 1:
             callee = self._xview
         else:
             callee = self._yview
```

### Comparing `ScrollableContainers-1.0a0/src/ScrollableContainers/Wx.py` & `ScrollableContainers-1.0a3/src/ScrollableContainers/Wx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-#! /usr/bin/python3 -B
+__all__ = ['ScrollablePanelWx']
 
 import wx
 import wx.lib.scrolledpanel as scrolledpanel
 
-__all__ = ['ScrollablePanelWx']
-
-###############################################################################
 
 class ScrollablePanelWx(scrolledpanel.ScrolledPanel):
-    '''
+    """
 Container with horizontal and vertical scrolling capabilities. Widgets must be
 added to its `panel` attribute.
-    '''
+    """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # According to the documentation, a sizer is required to calculate the
         # minimum virtual size of the panel.
         vbox = wx.BoxSizer(wx.VERTICAL)
```

