# Comparing `tmp/pywebgo-0.0.3.tar.gz` & `tmp/pywebgo-0.0.4.tar.gz`

## Comparing `pywebgo-0.0.3.tar` & `pywebgo-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.3/src/pywebgo/__init__.py
--rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 pywebgo-0.0.3/src/pywebgo/controller.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.3/src/pywebgo/data.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.3/src/pywebgo/elements.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.3/src/pywebgo/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pywebgo-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pywebgo-0.0.3/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pywebgo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/pywebgo.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/__init__.py
+-rw-r--r--   0        0        0    13828 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/controller.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/data.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/elements.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.4/src/pywebgo/utils.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 pywebgo-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pywebgo-0.0.4/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pywebgo-0.0.4/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.4/PKG-INFO
```

### Comparing `pywebgo-0.0.3/src/pywebgo/controller.py` & `pywebgo-0.0.4/src/pywebgo/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,29 @@
     - :class:`list` urls --> non-linked web pages to traverse through
     - :class:`bool` teardown --> closes the browser after execution if true
     - :class:`float` wait --> time delay for executing each action
     - :class:`ElementsHandler` elem_handler --> instance of ElementsHandler class to manage elements
     - :class:`DataHandler` data_handler --> instance of DataHandler class to manage data associated with the elements
     """
 
-    def __init__(self, urls: list, teardown: bool = True, wait: float = 0):
+    def __init__(self, urls: list, teardown: bool = True, wait: float = 0, options: list = None):
         """
         Initialize a new instance of the WebController class.
 
         :param urls: non-linked web pages to traverse through
         :param teardown: closes the browser after execution if true
         :param wait: time delay for executing each action
         """
-        super(WebController, self).__init__()
+        chrome_options = webdriver.ChromeOptions()
+        chrome_options.add_experimental_option("excludeSwitches", ["disable-popup-blocking"])
+        if options:
+            for option in options:
+                chrome_options.add_argument(option)
+
+        super(WebController, self).__init__(chrome_options=chrome_options)
 
         # ---- Private Variables ----- #
         self.urls = urls
         self.wait = wait
         self.teardown = teardown
         self.elem_handler = ElementsHandler()
         self.data_handler = DataHandler()
```

### Comparing `pywebgo-0.0.3/src/pywebgo/data.py` & `pywebgo-0.0.4/src/pywebgo/data.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.3/src/pywebgo/elements.py` & `pywebgo-0.0.4/src/pywebgo/elements.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.3/src/pywebgo/utils.py` & `pywebgo-0.0.4/src/pywebgo/utils.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.3/LICENSE.txt` & `pywebgo-0.0.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018 The Python Packaging Authority
+MIT License
+
+Copyright (c) 2022 Adil Zafar Khan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `pywebgo-0.0.3/pyproject.toml` & `pywebgo-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pywebgo"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Adil Zafar Khan", email="adilzafar66@gmail.com" },
 ]
 description = "A selenium client that automates web surfing with simple commands."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywebgo-0.0.3/PKG-INFO` & `pywebgo-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pywebgo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A selenium client that automates web surfing with simple commands.
 Project-URL: Homepage, https://github.com/adilzafar66/pywebgo
 Project-URL: Bug Tracker, https://github.com/adilzafar66/pywebgo/issues
 Author-email: Adil Zafar Khan <adilzafar66@gmail.com>
-License-File: LICENSE.txt
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyWebGo
-
-To be updated.
+A selenium client that automates web surfing using simple dictionary commands.
```

