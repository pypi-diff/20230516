# Comparing `tmp/quickdraw-0.2.0.tar.gz` & `tmp/quickdraw-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\quickdraw-0.2.0.tar", last modified: Wed Mar 10 21:26:16 2021, max compression
+gzip compressed data, was "quickdraw-1.0.0.tar", last modified: Tue May 16 12:02:16 2023, max compression
```

## Comparing `quickdraw-0.2.0.tar` & `quickdraw-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2021-03-10 21:26:16.019881 quickdraw-0.2.0/
--rw-rw-rw-   0        0        0     1608 2021-03-10 21:26:16.018879 quickdraw-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5400 2021-03-10 21:25:22.000000 quickdraw-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-03-10 21:26:15.974905 quickdraw-0.2.0/quickdraw/
--rw-rw-rw-   0        0        0       65 2021-03-10 20:34:52.000000 quickdraw-0.2.0/quickdraw/__init__.py
--rw-rw-rw-   0        0        0    20358 2021-03-10 21:09:08.000000 quickdraw-0.2.0/quickdraw/data.py
--rw-rw-rw-   0        0        0    16372 2021-03-10 20:34:52.000000 quickdraw-0.2.0/quickdraw/names.py
-drwxrwxrwx   0        0        0        0 2021-03-10 21:26:16.014883 quickdraw-0.2.0/quickdraw.egg-info/
--rw-rw-rw-   0        0        0     1608 2021-03-10 21:26:15.000000 quickdraw-0.2.0/quickdraw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2021-03-10 21:26:15.000000 quickdraw-0.2.0/quickdraw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-10 21:26:15.000000 quickdraw-0.2.0/quickdraw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-03-10 20:35:12.000000 quickdraw-0.2.0/quickdraw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2021-03-10 21:26:15.000000 quickdraw-0.2.0/quickdraw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-03-10 21:26:15.000000 quickdraw-0.2.0/quickdraw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-03-10 21:26:16.020880 quickdraw-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2724 2021-03-10 21:10:32.000000 quickdraw-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:02:16.788643 quickdraw-1.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-16 09:55:16.000000 quickdraw-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1239 2023-05-16 12:02:16.786686 quickdraw-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6113 2023-05-16 11:55:40.000000 quickdraw-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 12:02:16.724191 quickdraw-1.0.0/quickdraw/
+-rw-rw-rw-   0        0        0       85 2023-05-16 11:34:37.000000 quickdraw-1.0.0/quickdraw/__init__.py
+-rw-rw-rw-   0        0        0    24026 2023-05-16 11:58:43.000000 quickdraw-1.0.0/quickdraw/data.py
+-rw-rw-rw-   0        0        0    16372 2023-05-16 09:55:16.000000 quickdraw-1.0.0/quickdraw/names.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:02:16.774968 quickdraw-1.0.0/quickdraw.egg-info/
+-rw-rw-rw-   0        0        0     1239 2023-05-16 12:02:16.000000 quickdraw-1.0.0/quickdraw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-05-16 12:02:16.000000 quickdraw-1.0.0/quickdraw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:02:16.000000 quickdraw-1.0.0/quickdraw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 09:59:07.000000 quickdraw-1.0.0/quickdraw.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-05-16 12:02:16.000000 quickdraw-1.0.0/quickdraw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 12:02:16.000000 quickdraw-1.0.0/quickdraw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:02:16.788643 quickdraw-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2771 2023-05-16 11:39:43.000000 quickdraw-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:02:16.783767 quickdraw-1.0.0/tests/
+-rw-rw-rw-   0        0        0     4417 2023-05-16 11:38:16.000000 quickdraw-1.0.0/tests/test_quickdrawdata.py
+-rw-rw-rw-   0        0        0     4244 2023-05-16 11:38:48.000000 quickdraw-1.0.0/tests/test_quickdrawdatagroup.py
```

### Comparing `quickdraw-0.2.0/README.rst` & `quickdraw-1.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 quickdraw
 =========
 
 |pypibadge| |docsbadge|
 
+.. raw:: html
+
+    <iframe allowtransparency="true" style="background-color: white;" src="https://github.com/sponsors/martinohanlon/button" title="Sponsor martinohanlon" height="35" width="116" style="border: 0;"></iframe>
+
 `Quick Draw`_ is a drawing game which is training a neural network to recognise doodles.
 
 |quickdraw|
 
-``quickdraw`` is an API for accessing the `Quick Draw data`_ - it downloads the data files as and when needed, caches them locally and interprets them so they can be used.
+``quickdraw`` is a Python API for accessing the `Quick Draw data`_ - it downloads the data files as and when needed, caches them locally and interprets them so they can be used.
 
 |quickdrawpreview|
 
 Created by `Martin O'Hanlon`_ (`@martinohanlon`_, `stuffaboutco.de`_).
 
 Getting started
 ---------------
@@ -70,14 +74,22 @@
 
 .. code-block:: python
 
     anvil.image.save("my_anvil.gif")
 
 |myanvil|
 
+You can save an animation of the drawing using the ``animation`` property.
+
+.. code-block:: python
+
+    anvil.animation.save("my_anvil_animation.gif")
+
+|myanvilanimation|
+
 You can open a group of Quick Draw drawings using `QuickDrawDataGroup`_ passing the name of the drawing ("anvil", "aircraft", "baseball", etc).
 
 .. code-block:: python
 
     from quickdraw import QuickDrawDataGroup
 
     anvils = QuickDrawDataGroup("anvil")
@@ -132,27 +144,31 @@
 
 **Stable**. 
 
 Raise any `issues`_ in the `github repository`_.
 
 .. |quickdraw| image:: https://raw.githubusercontent.com/martinohanlon/quickdraw_python/master/docs/images/quickdraw.png
    :scale: 100 %
-   :alt: quickdraw
+   :alt: Quick Draw logo and banner
 
 .. |quickdrawpreview| image:: https://raw.githubusercontent.com/martinohanlon/quickdraw_python/master/docs/images/quickdraw_preview.jpg
    :scale: 100 %
-   :alt: quickdraw_preview
+   :alt: examples drawings created using Quick Draw
 
 .. |myanvil| image:: https://raw.githubusercontent.com/martinohanlon/quickdraw_python/master/docs/images/my_anvil.gif
    :scale: 100 %
-   :alt: quickdraw_preview
+   :alt: A Quick Draw drawing of a anvil
+
+.. |myanvilanimation| image:: https://raw.githubusercontent.com/martinohanlon/quickdraw_python/master/docs/images/my_anvil_animation.gif
+   :scale: 100 %
+   :alt: An animation of a Quick Draw drawing being drawn
 
 .. |pypibadge| image:: https://badge.fury.io/py/quickdraw.svg
    :target: https://badge.fury.io/py/quickdraw
-   :alt: Latest Version
+   :alt: Latest Version number
 
 .. |docsbadge| image:: https://readthedocs.org/projects/quickdraw/badge/
    :target: https://readthedocs.org/projects/quickdraw/
    :alt: Docs
 
 .. _Martin O'Hanlon: https://github.com/martinohanlon
 .. _stuffaboutco.de: http://stuffaboutco.de
@@ -165,8 +181,8 @@
 .. _quickdraw GitHub repository: https://github.com/martinohanlon/quickdraw_python
 .. _QuickDrawing: https://quickdraw.readthedocs.io/en/latest/api.html#quickdrawing
 .. _QuickDrawData: https://quickdraw.readthedocs.io/en/latest/api.html#quickdrawdata
 .. _QuickDrawDataGroup: https://quickdraw.readthedocs.io/en/latest/api.html#quickdrawdatagroup
 .. _drawing_names: https://quickdraw.readthedocs.io/en/latest/api.html#quickdraw.QuickDrawDataGroup.drawing_names
 .. _drawings: https://quickdraw.readthedocs.io/en/latest/api.html#quickdraw.QuickDrawDataGroup.drawings
 .. _issues: https://github.com/martinohanlon/quickdraw_python/issues
-.. _github repository: https://github.com/martinohanlon
+.. _github repository: https://github.com/martinohanlon/quickdraw_python
```

### Comparing `quickdraw-0.2.0/quickdraw/data.py` & `quickdraw-1.0.0/quickdraw/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .names import QUICK_DRAWING_FILES, QUICK_DRAWING_NAMES
 
 BINARY_URL = "https://storage.googleapis.com/quickdraw_dataset/full/binary/"
 CACHE_DIR = path.join(".",".quickdrawcache")
 
 
-class QuickDrawData():
+class QuickDrawData:
     """
     Allows interaction with the Google Quick, Draw! data set, downloads 
     Quick Draw data from 
     https://storage.googleapis.com/quickdraw_dataset/full/binary/ 
     and loads it into memory for easy access and processing.
 
     The following example will load the anvil drawings and get a single 
@@ -181,15 +181,15 @@
     def loaded_drawings(self):
         """
         Returns a list of drawing which have been loaded into memory.
         """
         return list(self._drawing_groups.keys())
 
 
-class QuickDrawDataGroup():
+class QuickDrawDataGroup:
     """
     Allows interaction with a group of Quick, Draw! drawings.
 
     The following example will load the ant group of drawings and get a 
     single drawing::
 
         from quickdraw import QuickDrawDataGroup
@@ -451,23 +451,24 @@
                     match = False
             
             if match:
                 results.append(drawing)
 
         return results
 
-class QuickDrawing():
+class QuickDrawing:
     """
     Represents a single Quick, Draw! drawing.
     """
     def __init__(self, name, drawing_data):
-        self._name =name
+        self._name = name
         self._drawing_data = drawing_data
         self._strokes = None
         self._image = None
+        self._animation = None
 
     @property
     def name(self):
         """
         Returns the name of the drawing (anvil, aircraft, ant, etc).
         """
         return self._name
@@ -598,11 +599,113 @@
         image = Image.new("RGB", (255,255), color=bg_color)
         image_draw = ImageDraw.Draw(image)
 
         for stroke in self.strokes:
             image_draw.line(stroke, fill=stroke_color, width=stroke_width)
 
         return image
+    
+    @property
+    def animation(self):
+        """
+        Returns a :class:`QuickDrawAnimation` instance representing the an 
+        animation of the QuickDrawing on a white background with a black 
+        drawing. Alternative image parameters can be set using 
+        ``get_animation()``.
+
+        To save the animation you would use the ``save`` method::
+
+            from quickdraw import QuickDrawData
+
+            qd = QuickDrawData()
+
+            anvil = qd.get_drawing("anvil")
+            anvil.animation.save("my_anvil_animation.gif")
+            
+        """
+        if self._animation is None:
+            self._animation = self.get_animation()
+
+        return self._animation
+
+    def get_animation(self, stroke_color=(0,0,0), stroke_width=2, bg_color=(255,255,255)):
+        """
+        Returns a :class:`QuickDrawAnimation` instance representing the an 
+        animation of the QuickDrawing being created.
+
+        :param list stroke_color:
+            A list of RGB (red, green, blue) values for the stroke color,
+            defaults to (0,0,0).
+
+        :param int stroke_color:
+            A width of the stroke, defaults to 2.
+
+        :param list bg_color:
+            A list of RGB (red, green, blue) values for the background color,
+            defaults to (255,255,255).
+        """
+        return QuickDrawAnimation(self, stroke_color, stroke_width, bg_color)
 
     def __str__(self):
         return "QuickDrawing key_id={}".format(self.key_id)
 
+class QuickDrawAnimation:
+    """
+    Represents an animation of a :class:`QuickDrawing`.
+
+    While an instance can be created directly it is typically returned by 
+    :meth:`QuickDrawing.get_animation` or :meth:`QuickDrawing.animation`.
+
+    To save the animation you would use the ``save`` method::
+
+        from quickdraw import QuickDrawData
+
+        qd = QuickDrawData()
+
+        anvil = qd.get_drawing("anvil")
+        anvil.animation.save("my_anvil_animation.gif")
+    """
+    def __init__(self, quick_drawing, stroke_color, stroke_width, bg_color): 
+        self._quick_drawing = quick_drawing
+        self._frames = []
+
+        image = Image.new("RGB", (255,255), color=bg_color)
+        image_draw = ImageDraw.Draw(image)
+
+        for stroke in self._quick_drawing.strokes:
+            for point in range(len(stroke)-1):
+                image_draw.line(
+                    (stroke[point], stroke[point+1]), 
+                    fill=stroke_color, 
+                    width=stroke_width
+                    )
+                self._frames.append(image.copy())
+
+    @property
+    def frames(self):
+        """
+        Returns a list `PIL Image <https://pillow.readthedocs.io/en/3.0.x/reference/Image.html>`_ 
+        objects of the animation.
+        """
+        return self._frames
+    
+    def save(self, filename, frame_length=0.1, loop_times=0):
+        """
+        Save's the animation to a given filename.
+
+        :param string filename:
+            The filename or path to save the animation. The filetype must be 
+            ``gif``.
+
+        :param int frame_length:
+            The time in seconds between each frame, defaults to 0.1.
+
+        :param int loop_times:
+            The number of times the animation should loop. A value of 0
+            will result in the animation looping forever. A value of ``None``
+            will result in the animation not looping. The default is 0.
+        """
+        kwargs = {}
+        if loop_times is not None:
+            kwargs["loop"] = loop_times
+
+        self._frames[0].save(filename, save_all=True, append_images=self._frames[1:], duration=frame_length*1000, **kwargs)
```

### Comparing `quickdraw-0.2.0/quickdraw/names.py` & `quickdraw-1.0.0/quickdraw/names.py`

 * *Files identical despite different names*

### Comparing `quickdraw-0.2.0/setup.py` & `quickdraw-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     if not sys.version_info >= (3, 3):
         raise ValueError('This package requires Python 3.3 or newer')
 else:
     raise ValueError('Unrecognized major version of Python')
 
 __project__ = 'quickdraw'
 __desc__ = 'An API for downloading and reading the google quickdraw data.'
-__version__ = '0.2.0'
+__version__ = '1.0.0'
 __author__ = "Martin O'Hanlon"
 __author_email__ = 'martin@ohanlonweb.com'
 __license__ = 'MIT'
 __url__ = 'https://github.com/martinohanlon/quickdraw_python'
 __requires__ = ['pillow', 'requests', ]
 __long_description__ = """# quickdraw
 
@@ -60,29 +60,30 @@
 
 [quickdraw.readthedocs.io](https://quickdraw.readthedocs.io)
 
 """
 
 __classifiers__ = [
 #   "Development Status :: 3 - Alpha",
-   "Development Status :: 4 - Beta",
-#   "Development Status :: 5 - Production/Stable",
+#   "Development Status :: 4 - Beta",
+   "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Education",
     "Intended Audience :: Developers",
     "Topic :: Education",
     "Topic :: Scientific/Engineering :: Image Recognition",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.3",
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 
 if __name__ == '__main__':
     setup(
         name='quickdraw',
         version = __version__,
         description = __desc__,
```

