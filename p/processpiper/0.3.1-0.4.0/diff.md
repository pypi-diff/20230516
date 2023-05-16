# Comparing `tmp/processpiper-0.3.1.tar.gz` & `tmp/processpiper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processpiper-0.3.1.tar", last modified: Fri Apr 28 09:04:09 2023, max compression
+gzip compressed data, was "processpiper-0.4.0.tar", last modified: Tue May 16 08:20:34 2023, max compression
```

## Comparing `processpiper-0.3.1.tar` & `processpiper-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.940065 processpiper-0.3.1/
--rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     6365 2023-04-28 09:04:09.940065 processpiper-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5810 2023-04-28 09:03:44.000000 processpiper-0.3.1/README.md
--rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 09:04:09.941065 processpiper-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.905741 processpiper-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.922059 processpiper-0.3.1/src/processpiper/
--rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.3.1/src/processpiper/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-04-09 09:57:23.000000 processpiper-0.3.1/src/processpiper/activity.py
--rw-rw-rw-   0        0        0    11673 2023-04-17 09:21:44.000000 processpiper-0.3.1/src/processpiper/colourtheme.py
--rw-rw-rw-   0        0        0     1753 2023-04-21 08:48:40.000000 processpiper-0.3.1/src/processpiper/constants.py
--rw-rw-rw-   0        0        0     4978 2023-04-16 00:55:33.000000 processpiper-0.3.1/src/processpiper/event.py
--rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.3.1/src/processpiper/footer.py
--rw-rw-rw-   0        0        0     2800 2023-04-09 09:10:50.000000 processpiper-0.3.1/src/processpiper/gateway.py
--rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.3.1/src/processpiper/helper.py
--rw-rw-rw-   0        0        0    10689 2023-04-21 08:45:10.000000 processpiper-0.3.1/src/processpiper/lane.py
--rw-rw-rw-   0        0        0    35665 2023-04-21 04:25:43.000000 processpiper-0.3.1/src/processpiper/painter.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 09:21:44.000000 processpiper-0.3.1/src/processpiper/pool.py
--rw-rw-rw-   0        0        0    18885 2023-04-28 08:53:46.000000 processpiper-0.3.1/src/processpiper/processmap.py
--rw-rw-rw-   0        0        0    19242 2023-04-21 08:51:52.000000 processpiper-0.3.1/src/processpiper/shape.py
--rw-rw-rw-   0        0        0     9395 2023-04-28 08:56:59.000000 processpiper-0.3.1/src/processpiper/text2diagram.py
--rw-rw-rw-   0        0        0     2267 2023-04-09 09:14:12.000000 processpiper-0.3.1/src/processpiper/title.py
--rw-rw-rw-   0        0        0     1189 2023-04-28 08:23:04.000000 processpiper-0.3.1/src/processpiper/version.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.937064 processpiper-0.3.1/src/processpiper.egg-info/
--rw-rw-rw-   0        0        0     6365 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-28 09:04:09.000000 processpiper-0.3.1/src/processpiper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 09:04:09.939064 processpiper-0.3.1/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.3.1/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.3.1/src/tests/github_action_test.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.402413 processpiper-0.4.0/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     6817 2023-05-16 08:20:34.402413 processpiper-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6262 2023-05-16 08:18:24.000000 processpiper-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:20:34.402413 processpiper-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.350463 processpiper-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.381407 processpiper-0.4.0/src/processpiper/
+-rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.4.0/src/processpiper/__init__.py
+-rw-rw-rw-   0        0        0     2386 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/activity.py
+-rw-rw-rw-   0        0        0    11673 2023-05-16 08:03:51.000000 processpiper-0.4.0/src/processpiper/colourtheme.py
+-rw-rw-rw-   0        0        0     1753 2023-04-21 08:48:40.000000 processpiper-0.4.0/src/processpiper/constants.py
+-rw-rw-rw-   0        0        0    12143 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/event.py
+-rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.4.0/src/processpiper/footer.py
+-rw-rw-rw-   0        0        0     4359 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/gateway.py
+-rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.4.0/src/processpiper/helper.py
+-rw-rw-rw-   0        0        0    11631 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/lane.py
+-rw-rw-rw-   0        0        0    39008 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/painter.py
+-rw-rw-rw-   0        0        0     5518 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/pool.py
+-rw-rw-rw-   0        0        0    26293 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/processmap.py
+-rw-rw-rw-   0        0        0    19377 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/shape.py
+-rw-rw-rw-   0        0        0    10307 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/text2diagram.py
+-rw-rw-rw-   0        0        0     2263 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/title.py
+-rw-rw-rw-   0        0        0     1189 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/version.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.399413 processpiper-0.4.0/src/processpiper.egg-info/
+-rw-rw-rw-   0        0        0     6817 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.401413 processpiper-0.4.0/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.4.0/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.4.0/src/tests/github_action_test.py
```

### Comparing `processpiper-0.3.1/LICENSE` & `processpiper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/PKG-INFO` & `processpiper-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: processpiper
-Version: 0.3.1
-Summary: Processpiper. An open source python library to generate business process diagram using code.
-Author: CS Goh
-Project-URL: Homepage, https://github.com/csgoh/processpiper
-Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
 ![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
@@ -37,44 +23,56 @@
 * Generate business process diagrams with Python code
 * Alternatively business process diagram can be generated by using plain text
 * Business process diagrams contains
   * Diagram title
   * Pool(s)
   * Lane(s)
   * Elements:
-    * Event: Start, End, Timer, Intermediate
+    * Event: Start, End, Timer, Intermediate, Message, Signal, Conditional and Link
     * Activity: Task, Subprocess
-    * Gateway: Inclusive, Exclusive, Parallel
+    * Gateway: Inclusive, Exclusive, Parallel, Event
 * Support for different colour themes
   * Default
   * GREYWOOF
   * BLUEMOUNTAIN
   * ORANGEPEEL
   * GREENTURTLE
 * Save diagram as PNG file
 
+## Change Logs
+Refer to this [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) page for the latest updates.
+
+
+
 ## Installation
 ### Install from PyPI
 ```bash
 pip install processpiper
 ```
+<br>
+
+## Frontend Application
+Two frontend applications have been developed to showcase ProcessPiper capability.
+* [Piperoni](https://github.com/csgoh/Piperoni) - A desktop application
+* [Piperita](https://piperita.streamlit.app/) - A Streamlit web application 
+<br>
 
 ### Python version requirements:
 * Python 3.10, 3.11
   
 ### Library Dependencies
-* Pillow 9.4.0
+* Pillow 9.5.0
 
 ### Supported Platforms
 * Windows
 * Ubuntu
 * MacOS
 
 ## Documentation
-Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this RaC library.
+Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this library.
 
 ## Examples
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
 from processpiper.text2diagram import render
```

### Comparing `processpiper-0.3.1/README.md` & `processpiper-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: processpiper
+Version: 0.4.0
+Summary: Processpiper. An open source python library to generate business process diagram using code.
+Author: CS Goh
+Project-URL: Homepage, https://github.com/csgoh/processpiper
+Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![release](https://img.shields.io/pypi/v/processpiper?style=plastic)
 ![Wheel](https://img.shields.io/pypi/wheel/processpiper?style=plastic)
 ![Downloads](https://img.shields.io/pypi/dm/processpiper?style=plastic)
 ![Platforms](https://img.shields.io/badge/Platform%3A-win%20%7C%20ubuntu%20%7C%20osx-brightgreen?style=plastic)
 [![license](https://img.shields.io/badge/license-mit-brightgreen.svg?style=plastic)](https://en.wikipedia.org/wiki/MIT_License)
 [![CodeFactor](https://www.codefactor.io/repository/github/csgoh/processpiper/badge?style=plastic)](https://www.codefactor.io/repository/github/csgoh/processpiper)
 ![code size](https://img.shields.io/github/languages/code-size/csgoh/processmapper?style=plastic)
@@ -23,44 +37,56 @@
 * Generate business process diagrams with Python code
 * Alternatively business process diagram can be generated by using plain text
 * Business process diagrams contains
   * Diagram title
   * Pool(s)
   * Lane(s)
   * Elements:
-    * Event: Start, End, Timer, Intermediate
+    * Event: Start, End, Timer, Intermediate, Message, Signal, Conditional and Link
     * Activity: Task, Subprocess
-    * Gateway: Inclusive, Exclusive, Parallel
+    * Gateway: Inclusive, Exclusive, Parallel, Event
 * Support for different colour themes
   * Default
   * GREYWOOF
   * BLUEMOUNTAIN
   * ORANGEPEEL
   * GREENTURTLE
 * Save diagram as PNG file
 
+## Change Logs
+Refer to this [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) page for the latest updates.
+
+
+
 ## Installation
 ### Install from PyPI
 ```bash
 pip install processpiper
 ```
+<br>
+
+## Frontend Application
+Two frontend applications have been developed to showcase ProcessPiper capability.
+* [Piperoni](https://github.com/csgoh/Piperoni) - A desktop application
+* [Piperita](https://piperita.streamlit.app/) - A Streamlit web application 
+<br>
 
 ### Python version requirements:
 * Python 3.10, 3.11
   
 ### Library Dependencies
-* Pillow 9.4.0
+* Pillow 9.5.0
 
 ### Supported Platforms
 * Windows
 * Ubuntu
 * MacOS
 
 ## Documentation
-Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this RaC library.
+Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this library.
 
 ## Examples
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
 from processpiper.text2diagram import render
```

### Comparing `processpiper-0.3.1/pyproject.toml` & `processpiper-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/src/processpiper/activity.py` & `processpiper-0.4.0/src/processpiper/activity.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,7 +50,17 @@
             subprocess_x_pos,
             self.y + self.height - subprocess_height,
             "[+]",
             painter.element_font,
             14,
             painter.element_font_colour,
         )
+
+
+class ServiceTask(Activity):
+    def draw(self, painter: Painter):
+        super().draw(painter)
+
+        raise NotImplementedError("ServiceTask is not implemented yet.")
+
+
+### To implement: User Task,Script Task,Business Rule Task, Manual Task, Received Task,Send Task, Receive Task
```

### Comparing `processpiper-0.3.1/src/processpiper/colourtheme.py` & `processpiper-0.4.0/src/processpiper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/src/processpiper/constants.py` & `processpiper-0.4.0/src/processpiper/constants.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/src/processpiper/footer.py` & `processpiper-0.4.0/src/processpiper/footer.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/src/processpiper/gateway.py` & `processpiper-0.4.0/src/processpiper/gateway.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+import math
 from .shape import Diamond
 from .painter import Painter
 
 SYMBOL_SIZE = 23
 
 
 class Gateway(Diamond):
     """A gateway is a diamond shape with a symbol in the middle"""
 
     def draw_symbol(self, symbol: str, painter: Painter):
         """Draw a symbol in the middle of the gateway"""
-        symbol_w, symbol_h = painter.get_text_dimension(symbol, "Arial", SYMBOL_SIZE)
+        symbol_w, symbol_h = painter.get_text_dimension(
+            symbol, painter.element_font, SYMBOL_SIZE
+        )
         painter.draw_text(
             self.x + (self.width / 2) - (symbol_w / 2),
             self.y + (self.height / 2) - (symbol_h / 2),
             symbol,
             painter.element_font,
             SYMBOL_SIZE,
             painter.element_font_colour,
@@ -66,7 +69,47 @@
     """An inclusive gateway is a diamond shape with a circle in the middle"""
 
     def draw(self, painter: Painter):
         """Draw the gateway and the symbol in the middle of the gateway"""
         super().draw(painter)
         symbol = "O"
         super().draw_symbol(symbol, painter)
+
+
+class EventGateway(Gateway):
+    """An event gateway is a diamond shape with a pentagon in the middle"""
+
+    def draw(self, painter: Painter):
+        """Draw the gateway and the symbol in the middle of the gateway"""
+        super().draw(painter)
+        # symbol = "O"
+        # super().draw_symbol(symbol, painter)
+
+        # Define the pentagon's properties
+        num_sides = 5
+        side_length = 7
+        center_x, center_y = self.x + self.width // 2, self.y + self.height // 2
+        angle = 2 * math.pi / num_sides
+        starting_angle = -math.pi / 2
+
+        # Calculate the coordinates of the pentagon's vertices
+        vertices = []
+        for i in range(num_sides):
+            x = center_x + side_length * math.cos(i * angle + starting_angle)
+            y = center_y + side_length * math.sin(i * angle + starting_angle)
+            vertices.append((x, y))
+
+        # Draw two circles
+        radius = 13
+        painter.draw_circle(center_x, center_y, radius, "black")
+        painter.draw_circle(center_x, center_y, radius - 1, self.fill_colour)
+        painter.draw_circle(center_x, center_y, radius - 3, "black")
+        painter.draw_circle(center_x, center_y, radius - 4, self.fill_colour)
+
+        # Draw the pentagon
+        print(f"vertices: {vertices}")
+        painter.draw_polygon(
+            vertices,
+            fill_colour=painter.element_fill_colour,
+            outline_colour="black",
+            outline_width=2,
+        )
```

### Comparing `processpiper-0.3.1/src/processpiper/helper.py` & `processpiper-0.4.0/src/processpiper/helper.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/src/processpiper/lane.py` & `processpiper-0.4.0/src/processpiper/lane.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,39 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from dataclasses import dataclass, field
 from enum import Enum
 from itertools import count
 from .shape import Shape
 from .painter import Painter
-from .event import Event, Start, End, Timer, Intermediate
-from .activity import Activity, Task, Subprocess
-from .gateway import Gateway, Exclusive, Parallel, Inclusive
+from .event import *
+from .activity import *
+from .gateway import *
 from .constants import Configs
 from .helper import Helper
 
 # from .helper import Helper
 
 
 class EventType:
     """Event types"""
 
     START = "Start"
     END = "End"
     TIMER = "Timer"
     INTERMEDIATE = "Intermediate"
+    MESSAGE = "Message"
+    MESSAGE_INTERMEDIATE = "MessageIntermediate"
+    MESSAGE_END = "MessageEnd"
+    SIGNAL = "Signal"
+    SIGNAL_INTERMEDIATE = "SignalIntermediate"
+    SIGNAL_END = "SignalEnd"
+    CONDITIONAL = "Conditional"
+    CONDITIONAL_INTERMEDIATE = "ConditionalIntermediate"
+    LINK = "Link"
 
 
 class ActivityType:
     """Activity types"""
 
     TASK = "Task"
     SUBPROCESS = "Subprocess"
@@ -51,28 +60,39 @@
 
 class GatewayType:
     """Gateway types"""
 
     EXCLUSIVE = "Exclusive"
     PARALLEL = "Parallel"
     INCLUSIVE = "Inclusive"
+    EVENT = "EventGateway"
 
 
 class ElementType(str, Enum):
     """Element types"""
 
     START = "Start"
     END = "End"
     TIMER = "Timer"
     INTERMEDIATE = "Intermediate"
+    MESSAGE = "Message"
+    MESSAGE_INTERMEDIATE = "MessageIntermediate"
+    MESSAGE_END = "MessageEnd"
+    SIGNAL = "Signal"
+    SIGNAL_INTERMEDIATE = "SignalIntermediate"
+    SIGNAL_END = "SignalEnd"
+    CONDITIONAL = "Conditional"
+    CONDITIONAL_INTERMEDIATE = "ConditionalIntermediate"
+    LINK = "Link"
     TASK = "Task"
     SUBPROCESS = "Subprocess"
     EXCLUSIVE = "Exclusive"
     PARALLEL = "Parallel"
     INCLUSIVE = "Inclusive"
+    EVENT = "Event"
 
 
 @dataclass
 class Lane:
     """A lane is a container for elements in a process diagram."""
 
     name: str = field(init=True)
@@ -106,24 +126,30 @@
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
         fill_colour: str = "",
         text_alignment: str = "",
     ) -> Shape:
         """Add an element to the lane"""
-        if font == "":
-            font = self.painter.element_font
-        if font_size == 0:
-            font_size = self.painter.element_font_size
-        if font_colour == "":
-            font_colour = self.painter.element_font_colour
-        if fill_colour == "":
-            fill_colour = self.painter.element_fill_colour
-        if text_alignment == "":
-            text_alignment = self.painter.element_text_alignment
+        # if font == "":
+        #     font = self.painter.element_font
+        # if font_size == 0:
+        #     font_size = self.painter.element_font_size
+        # if font_colour == "":
+        #     font_colour = self.painter.element_font_colour
+        # if fill_colour == "":
+        #     fill_colour = self.painter.element_fill_colour
+        # if text_alignment == "":
+        #     text_alignment = self.painter.element_text_alignment
+
+        font = font or self.painter.element_font
+        font_size = font_size or self.painter.element_font_size
+        font_colour = font_colour or self.painter.element_font_colour
+        fill_colour = fill_colour or self.painter.element_fill_colour
+        text_alignment = text_alignment or self.painter.element_text_alignment
 
         event_class = globals()[type]
         element = event_class(name, self.name)
         element.lane_id = self.id
         element.pool_name = self.pool_text
         element.font = font
         element.font_size = font_size
@@ -264,15 +290,14 @@
             #### Mark for removal
             # shape.draw_position_set = True
 
             shape.x_pos_traversed = True
 
             ### Set next elements' position
             for index, next_shape in enumerate(shape.connection_to.target):
-
                 ### Check whether the position has been set, if yes, skipped.
                 ### This is needed to avoid infinite recursion
                 if next_shape.traversed == True:
                     continue
 
                 if index == 0:
                     next_shape_y = y
```

### Comparing `processpiper-0.3.1/src/processpiper/painter.py` & `processpiper-0.4.0/src/processpiper/painter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 import math
 import os
 import sys
-from PIL import Image, ImageDraw, ImageFont, ImageColor
+from PIL import Image, ImageDraw, ImageFont, ImageColor, ImageFilter, ImageEnhance
 import textwrap
 from .colourtheme import ColourTheme
 from .helper import Helper
 
 
 class Painter:
     """Painter class to draw the diagram"""
@@ -73,15 +73,18 @@
     footer_font_colour: str
     ### Colour scheme attributes - End
 
     def __init__(self, width: int = 500, height: int = 500) -> None:
         """Initialise the painter"""
         self.output_type = "PNG"
         self.__surface = Image.new("RGBA", (width, height), (0, 0, 0, 0))
+        ### Set DPI
+        # self.__surface.info["dpi"] = (1600, 1600)
         self.__cr = ImageDraw.Draw(self.__surface)
+
         self.width = width
         self.height = height
 
     def set_colour_theme(self, colour_theme: str) -> None:
         """Set colour palette
 
         Args:
@@ -138,23 +141,30 @@
         if sys.platform.startswith("win"):  # Windows
             return os.path.join("C:\\", "Windows", "Fonts", f"{font_name}.ttf")
         elif sys.platform.startswith("darwin"):  # macOS
             return os.path.join(
                 "/", "System", "Library", "Fonts", "Supplemental", f"{font_name}.ttf"
             )
         elif sys.platform.startswith("linux"):  # Linux
-            return os.path.join(
-                "/",
-                "usr",
-                "share",
-                "fonts",
-                "truetype",
-                "msttcorefonts",
-                f"{font_name}.ttf",
-            )
+            font_dir = f"/usr/share/fonts/truetype/msttcorefonts"
+
+            if os.path.exists(os.path.join(font_dir, f"{font_name}.ttf")):
+                return os.path.join(font_dir, f"{font_name}.ttf")
+            else:
+                ### This is cater for cases where msttcorefonts is not installed
+                linux_font_name = "DejaVuSans"  # Default font for Linux
+                return os.path.join(
+                    "/",
+                    "usr",
+                    "share",
+                    "fonts",
+                    "truetype",
+                    "dejavu",  # Use the DejaVu font directory instead of msttcorefonts
+                    f"{linux_font_name}.ttf",
+                )
         else:
             raise Exception("Unsupported operating system")
 
     def draw_grid(self):
         """Draw a grid of dots to help with alignment"""
         ### Set the dot size and spacing
         spacing = 10
@@ -184,14 +194,42 @@
             width (int): Rectangle width
             height (int): Rectangle height
             box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
         """
         shape = [(x, y), (x + width, y + height)]
         self.__cr.rectangle(shape, fill=box_fill_colour)
 
+    def draw_box_with_outline(
+        self,
+        x: int,
+        y: int,
+        width: int,
+        height: int,
+        box_outline_colour: str,
+        box_outline_transparency: int,
+        box_outline_width: int,
+        box_fill_colour: str,
+    ) -> None:
+        """Draw a rectagle
+
+        Args:
+            x (int): X coordinate
+            y (int): Y coordinate
+            width (int): Rectangle width
+            height (int): Rectangle height
+            box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
+        """
+        shape = [(x, y), (x + width, y + height)]
+        self.__cr.rectangle(
+            shape,
+            fill=box_fill_colour,
+            outline=box_outline_colour,
+            width=box_outline_width,
+        )
+
     def draw_rounded_box(
         self, x: int, y: int, width: int, height: int, box_fill_colour: str
     ) -> None:
         """Draw a rounded rectagle
 
         Args:
             x (int): X coordinate
@@ -405,14 +443,25 @@
             ### Rotate text
             rotated_img = Image.new("RGBA", (font_width, font_height))
             rotated_draw = ImageDraw.Draw(rotated_img)
             rotated_draw.text((0, 0), line, font=font, fill=(text_font_colour))
             rotated_img = rotated_img.rotate(90, expand=1)
             self.__surface.paste(rotated_img, (int(x), int(y)), rotated_img)
 
+    def draw_polygon(
+        self,
+        points: list,
+        outline_colour: str = "",
+        outline_width: int = 1,
+        fill_colour: str = "",
+    ):
+        self.__cr.polygon(
+            points, fill=fill_colour, outline=outline_colour, width=outline_width
+        )
+
     def draw_diamond(
         self, x: int, y: int, width: int, height: int, fill_colour: str
     ) -> None:
         """Draw a diamond
 
         Args:
             x (int): X coordinate
@@ -430,29 +479,47 @@
             (x, y + height / 2),
         ]
 
         ### Use Pillow's ImageDraw module to draw a polygon with the given points and fill color.
         self.__cr.polygon(points, fill=fill_colour)
 
     def draw_circle(
-        self, x: int, y: int, radius: float, outline_colour: str, fill_colour: str = ""
+        self,
+        x: int,
+        y: int,
+        radius: float,
+        outline_colour: str,
+        outline_width: int = 1,
+        fill_colour: str = "",
     ) -> None:
         """Draw a circle"""
+        outline_red, outline_green, outline_blue = ImageColor.getrgb(outline_colour)
         if fill_colour == "":
             ### If no fill colour is specified, use the outline colour as the fill colour.
-            outline_red, outline_green, outline_blue = ImageColor.getrgb(outline_colour)
             fill_red, fill_green, fill_blue = outline_red, outline_green, outline_blue
+            self.__cr.ellipse(
+                (x - radius, y - radius, x + radius, y + radius),
+                fill=(fill_red, fill_green, fill_blue),
+                outline=(outline_red, outline_green, outline_blue),
+                width=outline_width,
+            )
+        elif fill_colour == "transparent":
+            self.__cr.ellipse(
+                (x - radius, y - radius, x + radius, y + radius),
+                outline=(outline_red, outline_green, outline_blue),
+                width=outline_width,
+            )
         else:
-            outline_red, outline_green, outline_blue = ImageColor.getrgb(outline_colour)
             fill_red, fill_green, fill_blue = ImageColor.getrgb(fill_colour)
-        self.__cr.ellipse(
-            (x - radius, y - radius, x + radius, y + radius),
-            fill=(fill_red, fill_green, fill_blue),
-            outline=(outline_red, outline_green, outline_blue),
-        )
+            self.__cr.ellipse(
+                (x - radius, y - radius, x + radius, y + radius),
+                fill=(fill_red, fill_green, fill_blue),
+                outline=(outline_red, outline_green, outline_blue),
+                width=outline_width,
+            )
 
     def draw_dot(self, x: int, y: int, colour: str) -> None:
         """Draw a dot"""
         r, g, b = ImageColor.getrgb(colour)
         self.__cr.point((x, y), fill=(r, g, b))
 
     def draw_line(
@@ -819,15 +886,15 @@
             connection_style,
             connector_line_width,
             connector_line_colour,
         )
 
         label_x_pos, label_y_pos = right_angle_point
 
-        label_w, label_h = self.get_multitext_dimension(label, "Arial", 12)
+        label_w, label_h = self.get_multitext_dimension(label, connector_font, 12)
         if label_x_pos == x1 and label_y_pos == y1:
             ### There is no right angle point
             label_x_pos = max(x1 + 5, x1 + (((x2 - x1) - label_w) / 2))
             label_y_pos = y1 - label_h - 3
         else:
             label_x_pos += 5
             label_y_pos = label_y_pos - label_h - 3
@@ -839,15 +906,21 @@
             connector_font,
             connector_font_size,
             connector_font_color,
         )
 
         if connection_style == "dashed":
             ### Draw round circle at the beginning of the line
-            self.draw_circle(x1, y1, 6, connector_arrow_colour, "white")
+            self.draw_circle(
+                x1,
+                y1,
+                radius=6,
+                outline_colour=connector_arrow_colour,
+                fill_colour="white",
+            )
 
             ### Draw white arrow head at the end of the line
 
             self.draw_arrow_head(
                 right_angle_point[0],
                 right_angle_point[1],
                 x2,
@@ -1010,8 +1083,28 @@
         """Save surface to PNG file
 
         Args:
             filename (str): PNG file name
         """
         if self.output_type == "PNG":
             if self.__surface is not None:
-                self.__surface.save(filename)
+                # anti_alias_image = self.__surface.filter(ImageFilter.SMOOTH_MORE)
+                # anti_alias_image.save(filename)
+                # Set the DPI to 300
+                # info = self.__surface.info.copy()
+                # info["dpi"] = (600, 600)
+
+                # Save the image with the new DPI
+                # self.__surface.save(filename, **info)
+
+                length_x, width_y = self.__surface.size
+                factor = min(1, float(1024.0 / length_x))
+
+                factor = 1
+                size = int(factor * length_x), int(factor * width_y)
+                image_resize = self.__surface.resize(size, resample=Image.LANCZOS)
+                image_resize.save(filename, dpi=(1200, 1200), optimize=False)
+
+                # enhancer = ImageEnhance.Sharpness(self.__surface)
+                # im_s_1 = enhancer.enhance(3)
+                # im_s_1.save("sharp.png")
+                # self.__surface.save(filename)
```

### Comparing `processpiper-0.3.1/src/processpiper/pool.py` & `processpiper-0.4.0/src/processpiper/pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,26 +105,35 @@
             text_alignment (str, optional): _lane text alignement. Defaults to "".
             background_fill_colour (str, optional): land background fill colour. Defaults to "".
 
         Returns:
             Lane: Lane object
         """
 
-        if font == "":
-            font = self.painter.lane_font
-        if font_size == 0:
-            font_size = self.painter.lane_font_size
-        if font_colour == "":
-            font_colour = self.painter.lane_font_colour
-        if fill_colour == "":
-            fill_colour = self.painter.lane_fill_colour
-        if text_alignment == "":
-            text_alignment = self.painter.lane_text_alignment
-        if background_fill_colour == "":
-            background_fill_colour = self.painter.lane_background_fill_colour
+        # if font == "":
+        #     font = self.painter.lane_font
+        # if font_size == 0:
+        #     font_size = self.painter.lane_font_size
+        # if font_colour == "":
+        #     font_colour = self.painter.lane_font_colour
+        # if fill_colour == "":
+        #     fill_colour = self.painter.lane_fill_colour
+        # if text_alignment == "":
+        #     text_alignment = self.painter.lane_text_alignment
+        # if background_fill_colour == "":
+        #     background_fill_colour = self.painter.lane_background_fill_colour
+
+        font = font or self.painter.lane_font
+        font_size = font_size or self.painter.lane_font_size
+        font_colour = font_colour or self.painter.lane_font_colour
+        fill_colour = fill_colour or self.painter.lane_fill_colour
+        text_alignment = text_alignment or self.painter.lane_text_alignment
+        background_fill_colour = (
+            background_fill_colour or self.painter.lane_background_fill_colour
+        )
 
         lane = Lane(
             lane_name,
             self.name,
             font,
             font_size,
             font_colour,
```

### Comparing `processpiper-0.3.1/src/processpiper/processmap.py` & `processpiper-0.4.0/src/processpiper/processmap.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from dataclasses import dataclass, field
-from .lane import Lane
+from .event import *
+from .lane import Lane, ElementType, EventType
 from .pool import Pool
 from .painter import Painter
-from .shape import Shape
+from .shape import *
 from .title import Title
 from .footer import Footer
 from .constants import Configs
 from .helper import Helper
 from PIL import Image
 import time
 import logging
@@ -86,22 +87,19 @@
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
         fill_colour: str = "",
         text_alignment: str = "centre",
     ) -> Pool:
         """Add a Pool to the Process Map"""
-        if font == "":
-            font = self.__painter.pool_font
-        if font_size == 0:
-            font_size = self.__painter.pool_font_size
-        if font_colour == "":
-            font_colour = self.__painter.pool_font_colour
-        if fill_colour == "":
-            fill_colour = self.__painter.pool_fill_colour
+
+        font = font or self.__painter.pool_font
+        font_size = font_size or self.__painter.pool_font_size
+        font_colour = font_colour or self.__painter.pool_font_colour
+        fill_colour = fill_colour or self.__painter.pool_fill_colour
 
         pool = Pool(
             pool_name,
             font,
             font_size,
             font_colour,
             fill_colour,
@@ -118,26 +116,35 @@
         font_size: int = 0,
         font_colour: str = "",
         fill_colour: str = "",
         text_alignment: str = "centre",
         background_fill_colour: str = "",
     ) -> Lane:
         """Add a Lane to the Process Map"""
-        if font == "":
-            font = self.__painter.lane_font
-        if font_size == 0:
-            font_size = self.__painter.lane_font_size
-        if font_colour == "":
-            font_colour = self.__painter.lane_font_colour
-        if fill_colour == "":
-            fill_colour = self.__painter.lane_fill_colour
-        if text_alignment == "":
-            text_alignment = self.__painter.lane_text_alignment
-        if background_fill_colour == "":
-            background_fill_colour = self.__painter.lane_background_fill_colour
+        # if font == "":
+        #     font = self.__painter.lane_font
+        # if font_size == 0:
+        #     font_size = self.__painter.lane_font_size
+        # if font_colour == "":
+        #     font_colour = self.__painter.lane_font_colour
+        # if fill_colour == "":
+        #     fill_colour = self.__painter.lane_fill_colour
+        # if text_alignment == "":
+        #     text_alignment = self.__painter.lane_text_alignment
+        # if background_fill_colour == "":
+        #     background_fill_colour = self.__painter.lane_background_fill_colour
+
+        font = font or self.__painter.lane_font
+        font_size = font_size or self.__painter.lane_font_size
+        font_colour = font_colour or self.__painter.lane_font_colour
+        fill_colour = fill_colour or self.__painter.lane_fill_colour
+        text_alignment = text_alignment or self.__painter.lane_text_alignment
+        background_fill_colour = (
+            background_fill_colour or self.__painter.lane_background_fill_colour
+        )
 
         pool = self.add_pool("Default Pool")
         lane = pool.add_lane(
             lane_name,
             font,
             font_size,
             font_colour,
@@ -228,15 +235,14 @@
     ):
         """Set the x position for the shape"""
         current_lane = self.get_lane_by_id(current_shape.lane_id)
         Helper.printc(
             f"set_shape_x_position: {current_lane.name}, {current_shape.name}", "34"
         )
         if index == 0:
-
             if previous_shape is not None:
                 if previous_shape.pool_name == current_shape.pool_name:
                     if previous_shape.lane_id == current_shape.lane_id:
                         current_shape.x = self.get_next_x_position(previous_shape.width)
                         Helper.printc(f"          same pool same lane")
                     else:
                         current_shape.x = self.get_next_x_position(previous_shape.width)
@@ -303,16 +309,20 @@
             )
 
         shape.set_draw_position(self.__painter)
 
         shape.y_pos_traversed = True
 
         # for shape in lane.shapes:
+        Helper.printc(f"         {shape.name} looping..", "32")
         for index, connection in enumerate(shape.connection_to):
             next_shape = connection.target
+            Helper.printc(
+                f"             {next_shape.name}, {next_shape.y_pos_traversed}", "32"
+            )
             if next_shape.y_pos_traversed is True:
                 continue
 
             self.set_shape_y_position(next_shape, index)
 
     def set_draw_position(self, painter: Painter) -> tuple:
         """Set the draw position for the process map"""
@@ -396,19 +406,21 @@
             + Configs.POOL_TEXT_WIDTH
             + self.lane_max_width
             + Configs.SURFACE_LEFT_MARGIN
         )
 
     def reset_traversed_flags(self):
         """Reset the traversed flags for all shapes in the process map"""
+        Helper.printc("*** Resetting traversed flags...", "32")
         for pool in self._pools:
             for lane in pool._lanes:
                 lane.next_shape_y = 0
                 lane.shape_row_count = 0
                 for shape in lane.shapes:
+                    Helper.printc(f"    {shape.name}", "32")
                     shape.y_pos_traversed = False
 
     def get_orphan_elements(self) -> list:
         orphan_elements = []
         for pool in self._pools:
             for lane in pool._lanes:
                 for shape in lane.shapes:
@@ -416,14 +428,20 @@
                         len(shape.connection_to) == 0
                         and len(shape.connection_from) == 0
                     ):
                         orphan_elements.append(shape.name)
 
         return orphan_elements
 
+    def print_connection(self, shape: Shape):
+        Helper.printc(f"*****    {shape.name}", "32")
+        for connection in shape.connection_to:
+            Helper.printc(f"            {connection.target.name}", "32")
+            self.print_connection(connection.target)
+
     def draw(self) -> None:
         """Draw the process map"""
 
         ### Ensure title is defined
         if (len(self.title) == 0) and (self._title == None):
             raise ValueError("The process map must contain a title")
 
@@ -444,14 +462,24 @@
         ### Ensure connections are defined
         orphan_elements = self.get_orphan_elements()
         if len(orphan_elements) > 0:
             raise UnconnectedElementException(
                 f"The following element(s) are defined but not connected to other element(s): \n{orphan_elements}"
             )
 
+        ### Replace the class type of shapes with the correct class type
+        # self.print_connection(self.find_start_shape())
+        for pool in self._pools:
+            for lane in pool._lanes:
+                for index, shape in enumerate(lane.shapes):
+                    self.replace_signal_element(lane, index, shape)
+                    self.replace_conditional_element(lane, index, shape)
+                    self.replace_message_element(lane, index, shape)
+
+        # self.print_connection(self.find_start_shape())
         self.set_draw_position(self.__painter)
 
         self._title.draw()
 
         if self._pools:
             for pool in self._pools:
                 ### Draw the pools first
@@ -473,14 +501,130 @@
 
         if self._footer != None:
             self._footer.draw()
 
         if self.auto_size == True:
             self.__painter.set_surface_size(self.width, self.height)
 
+    def replace_message_element(self, lane, index, shape):
+        if type(shape) == Message:
+            Helper.debug_log(f"  matched with Message")
+            ### Check if the signal is a start signal. i.e it has no connection from
+            if len(shape.connection_to) > 0 and len(shape.connection_from) == 0:
+                Helper.debug_log(f"      start MESSAGE")
+                new_shape = self.replace_element_type(lane, shape, ElementType.MESSAGE)
+
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+            elif (  ### Check if the signal is an intermediate signal. i.e it has both connection from and to
+                len(shape.connection_to) > 0 and len(shape.connection_from) > 0
+            ):
+                Helper.debug_log(f"      MESSAGE_INTERMEDIATE")
+                new_shape = self.replace_element_type(
+                    lane, shape, ElementType.MESSAGE_INTERMEDIATE
+                )
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+            else:  ### Check if the signal is an end signal. i.e it has no connection to
+                Helper.debug_log(f"      MESSAGE_END")
+                new_shape = self.replace_element_type(
+                    lane, shape, ElementType.MESSAGE_END
+                )
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+    def replace_conditional_element(self, lane, index, shape):
+        if type(shape) == Conditional:
+            Helper.debug_log(f"  matched with Conditional")
+            ### Check if the signal is a start signal. i.e it has no connection from
+            if len(shape.connection_to) > 0 and len(shape.connection_from) == 0:
+                Helper.debug_log(f"      start CONDITIONAL")
+                new_shape = self.replace_element_type(
+                    lane, shape, ElementType.CONDITIONAL
+                )
+
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+            elif (  ### Check if the signal is an intermediate signal. i.e it has both connection from and to
+                len(shape.connection_to) > 0 and len(shape.connection_from) > 0
+            ):
+                Helper.debug_log(f"      intermediate CONDITIONAL_INTERMEDIATE")
+                new_shape = self.replace_element_type(
+                    lane, shape, ElementType.CONDITIONAL_INTERMEDIATE
+                )
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+    def replace_signal_element(self, lane, index, shape):
+        if type(shape) == Signal:
+            Helper.debug_log(f"  matched with Signal")
+            ### Check if the signal is a start signal. i.e it has no connection from
+            if len(shape.connection_to) > 0 and len(shape.connection_from) == 0:
+                Helper.debug_log(f"      start signal")
+                new_shape = self.replace_element_type(lane, shape, ElementType.SIGNAL)
+
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+            elif (  ### Check if the signal is an intermediate signal. i.e it has both connection from and to
+                len(shape.connection_to) > 0 and len(shape.connection_from) > 0
+            ):
+                Helper.debug_log(f"      intermediate signal")
+                new_shape = self.replace_element_type(
+                    lane, shape, ElementType.SIGNAL_INTERMEDIATE
+                )
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+            else:  ### Check if the signal is an end signal. i.e it has no connection to
+                Helper.debug_log(f"      end signal")
+                new_shape = self.replace_element_type(
+                    lane, shape, ElementType.SIGNAL_END
+                )
+                lane.shapes[index] = self.replace_connections(shape, new_shape)
+
+    def replace_element_type(self, lane, shape, new_shape_type: ElementType):
+        event_class = globals()[new_shape_type]
+        new_shape = event_class(
+            shape.name,
+            lane.name,
+        )
+
+        return new_shape
+
+    def replace_connections(self, current_shape, new_shape):
+        new_shape.lane_id = current_shape.lane_id
+        new_shape.pool_name = current_shape.pool_name
+        new_shape.font = current_shape.font
+        new_shape.font_size = current_shape.font_size
+        new_shape.font_colour = current_shape.font_colour
+        new_shape.fill_colour = current_shape.fill_colour
+        new_shape.text_alignment = current_shape.text_alignment
+        new_shape.connection_to = current_shape.connection_to
+        for connection_index, connection in enumerate(current_shape.connection_to):
+            new_connection = Connection(
+                new_shape,
+                connection.target,
+                connection.label,
+                connection.connection_type,
+            )
+            Helper.printc(
+                f"      creating new connection: {new_connection.source.name}"
+            )
+            new_shape.connection_to[connection_index] = new_connection
+        self.replace_connection_from(current_shape, new_shape)
+        return new_shape
+
+    def replace_connection_from(self, current_shape, new_shape):
+        for shape_index, shape in enumerate(current_shape.connection_from):
+            for connection_index, connection_to in enumerate(shape.connection_to):
+                new_connection = Connection(
+                    connection_to.source,
+                    new_shape,
+                    connection_to.label,
+                    connection_to.connection_type,
+                )
+                shape.connection_to[shape_index] = new_connection
+
     def __set_colour_theme(self, palette: str) -> None:
         """This method sets the colour palette"""
         self.__painter.set_colour_theme(palette)
 
     def save(self, filename: str) -> None:
         """This method saves the process map to a file"""
         self.__painter.save_surface(filename)
```

### Comparing `processpiper-0.3.1/src/processpiper/shape.py` & `processpiper-0.4.0/src/processpiper/shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
         Args:
             points_source (dict): connection points of source shapes
             points_target (dict): connection points of target shapes
 
         Returns:
             (tuple), (tuple): Nearest connection points between two sets of shapes
         """
-        shortest_distance: int = 9_999_999
+        shortest_distance: int = float("inf")
+
         for source_name, source_points in points_source.items():
             for target_name, target_points in points_target.items():
                 distance = self.get_distance(source_points, target_points)
 
                 if distance < shortest_distance:
                     shortest_distance = distance
                     nearest_points = {
@@ -182,15 +183,15 @@
 
         return target_points
 
     def find_nearest_points_same_pool_diff_lanes(self, points_source, points_target):
         """Find nearest connection points between two sets of shapes
         where source and target shapes are in the same pool but different lanes"""
 
-        shortest_distance: int = 9_999_999
+        shortest_distance: int = float("inf")
         nearest_points = {}
         source_connection_points = self.get_top_bottom_points(points_source)
         target_connection_points = self.get_left_right_points(points_target)
         if len(target_connection_points) == 0:
             target_connection_points = self.get_top_bottom_points(points_target)
 
         for source_name, source_points in source_connection_points.items():
@@ -257,15 +258,14 @@
         """Draw connection between shapes"""
 
         source_points = self.points
         Helper.printc(f"Draw connection for shape: [{self.name}]", 36)
         if self.connection_to:
             connection_style = "solid"
             for connection in self.connection_to:
-
                 target_points = connection.target.points
 
                 if self.is_same_lane(self, connection.target):
                     Helper.printc(
                         f"Same lane: Connection between [{self.name}] and [{connection.target.name}]"
                     )
                     (
@@ -395,14 +395,18 @@
     text_x: int = field(init=False)
     text_y: int = field(init=False)
     text_width: int = field(init=False)
     text_height: int = field(init=False)
 
     def __post_init__(self):
         self.radius = CIRCLE_RADIUS
+        self.text_x: int = 0
+        self.text_y: int = 0
+        self.text_width: int = 0
+        self.text_height: int = 0
 
     def set_draw_position(self, painter: Painter) -> tuple:
         """Set draw position of circle"""
         ### Circle x position starts from the circle centre, so add radius to x.
         ### But we want to cater for cases when circle and box aligned vertically.
         # self.x = int(self.x + CIRCLE_RADIUS + (BOX_WIDTH / 2) - (CIRCLE_RADIUS))
         # self.x = int(self.x + CIRCLE_RADIUS)
```

### Comparing `processpiper-0.3.1/src/processpiper/text2diagram.py` & `processpiper-0.4.0/src/processpiper/text2diagram.py`

 * *Files 24% similar despite different names*

```diff
@@ -191,14 +191,29 @@
         element_type = "EventType.TIMER"
         element_name = element_str[len("(@timer") : element_str.index(")")].strip()
     elif element_str.startswith("(@intermediate"):
         element_type = "EventType.INTERMEDIATE"
         element_name = element_str[
             len("(@intermediate") : element_str.index(")")
         ].strip()
+    elif element_str.startswith("(@message"):
+        element_type = "EventType.MESSAGE"
+        element_name = element_str[len("(@message") : element_str.index(")")].strip()
+    elif element_str.startswith("(@signal"):
+        element_type = "EventType.SIGNAL"
+        element_name = element_str[len("(@signal") : element_str.index(")")].strip()
+    elif element_str.startswith("(@conditional"):
+        element_type = "EventType.CONDITIONAL"
+        element_name = element_str[
+            len("(@conditional") : element_str.index(")")
+        ].strip()
+    elif element_str.startswith("(@link"):
+        element_type = "EventType.LINK"
+        element_name = element_str[len("(@link") : element_str.index(")")].strip()
+
     ### ActivityType
     elif element_str.startswith("[@subprocess"):
         element_type = "ActivityType.SUBPROCESS"
         element_name = element_str[len("[@subprocess") : element_str.index("]")].strip()
     elif element_str.startswith("["):
         element_type = "ActivityType.TASK"
         element_name = element_str[1 : element_str.index("]")].strip()
@@ -211,14 +226,17 @@
         element_name = element_str[len("<@exclusive") : element_str.index(">")].strip()
     elif element_str.startswith("<@exclusive"):
         element_type = "GatewayType.EXCLUSIVE"
         element_name = element_str[len("<@exclusive") : element_str.index(">")].strip()
     elif element_str.startswith("<"):
         element_type = "GatewayType.EXCLUSIVE"
         element_name = element_str[1 : element_str.index(">")].strip()
+    elif element_str.startswith("(@event"):
+        element_type = "GatewayType.EVENT"
+        element_name = element_str[len("(@event") : element_str.index(")")].strip()
 
     else:
         raise ValueError(f"Invalid element string: {element_str}")
 
     element_var = element_str.split(" as ")[1].strip()
 
     return element_type, element_name, element_var
```

### Comparing `processpiper-0.3.1/src/processpiper/title.py` & `processpiper-0.4.0/src/processpiper/title.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 
 @dataclass
 class Title:
     """Title of the process map"""
 
     name: str = field(init=True, default="<Process Map Title>")
-    font: str = field(init=True, default="Arial")
-    font_size: int = field(init=True, default=28)
-    font_colour: str = field(init=True, default="black")
+    font: str = field(init=True, default=None)
+    font_size: int = field(init=True, default=None)
+    font_colour: str = field(init=True, default=None)
 
     x: int = field(init=False, default=0)
     y: int = field(init=False, default=0)
     width: int = field(init=False, default=0)
     height: int = field(init=False, default=0)
     painter: Painter = field(init=False)
```

### Comparing `processpiper-0.3.1/src/processpiper/version.py` & `processpiper-0.4.0/src/processpiper/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Version information for processpiper."""
-__version__ = "v0.3.1"
+__version__ = "v0.4.0"
```

### Comparing `processpiper-0.3.1/src/processpiper.egg-info/PKG-INFO` & `processpiper-0.4.0/src/processpiper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.3.1
+Version: 0.4.0
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,44 +37,56 @@
 * Generate business process diagrams with Python code
 * Alternatively business process diagram can be generated by using plain text
 * Business process diagrams contains
   * Diagram title
   * Pool(s)
   * Lane(s)
   * Elements:
-    * Event: Start, End, Timer, Intermediate
+    * Event: Start, End, Timer, Intermediate, Message, Signal, Conditional and Link
     * Activity: Task, Subprocess
-    * Gateway: Inclusive, Exclusive, Parallel
+    * Gateway: Inclusive, Exclusive, Parallel, Event
 * Support for different colour themes
   * Default
   * GREYWOOF
   * BLUEMOUNTAIN
   * ORANGEPEEL
   * GREENTURTLE
 * Save diagram as PNG file
 
+## Change Logs
+Refer to this [Change Logs](https://github.com/csgoh/processpiper/wiki/Change-Logs) page for the latest updates.
+
+
+
 ## Installation
 ### Install from PyPI
 ```bash
 pip install processpiper
 ```
+<br>
+
+## Frontend Application
+Two frontend applications have been developed to showcase ProcessPiper capability.
+* [Piperoni](https://github.com/csgoh/Piperoni) - A desktop application
+* [Piperita](https://piperita.streamlit.app/) - A Streamlit web application 
+<br>
 
 ### Python version requirements:
 * Python 3.10, 3.11
   
 ### Library Dependencies
-* Pillow 9.4.0
+* Pillow 9.5.0
 
 ### Supported Platforms
 * Windows
 * Ubuntu
 * MacOS
 
 ## Documentation
-Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this RaC library.
+Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this library.
 
 ## Examples
 ### (Method 1) Generate diagram using plain text
 This is a sample code to generate a business process diagram using plain text. 
 ```python
 from processpiper.text2diagram import render
```

### Comparing `processpiper-0.3.1/src/processpiper.egg-info/SOURCES.txt` & `processpiper-0.4.0/src/processpiper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processpiper-0.3.1/src/tests/github_action_test.py` & `processpiper-0.4.0/src/tests/github_action_test.py`

 * *Files identical despite different names*

