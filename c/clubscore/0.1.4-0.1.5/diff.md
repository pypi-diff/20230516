# Comparing `tmp/clubscore-0.1.4.tar.gz` & `tmp/clubscore-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clubscore-0.1.4.tar", last modified: Mon May  8 12:13:24 2023, max compression
+gzip compressed data, was "dist/clubscore-0.1.5.tar", last modified: Tue May 16 21:42:34 2023, max compression
```

## Comparing `clubscore-0.1.4.tar` & `clubscore-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 12:13:24.000000 clubscore-0.1.4/
--rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.4/LICENSE
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-08 12:13:24.000000 clubscore-0.1.4/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.4/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore/
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.4/clubscore/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore/objects/
--rw-r--r--   0 dave       (501) staff       (20)     4792 2023-05-06 08:35:20.000000 clubscore-0.1.4/clubscore/objects/CONTAINER.py
--rw-r--r--   0 dave       (501) staff       (20)     2204 2023-05-06 08:35:20.000000 clubscore-0.1.4/clubscore/objects/IMG.py
--rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.4/clubscore/objects/RECTANGLE.py
--rw-r--r--   0 dave       (501) staff       (20)     3936 2023-05-08 12:06:04.000000 clubscore-0.1.4/clubscore/objects/TEXT.py
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.4/clubscore/objects/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     3332 2023-05-06 21:57:49.000000 clubscore-0.1.4/clubscore/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      394 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-08 12:13:24.000000 clubscore-0.1.4/clubscore.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-08 12:13:24.000000 clubscore-0.1.4/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-08 12:13:21.000000 clubscore-0.1.4/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-08 12:13:24.000000 clubscore-0.1.4/tests/
--rw-r--r--   0 dave       (501) staff       (20)     1353 2023-05-07 10:14:30.000000 clubscore-0.1.4/tests/test_utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 21:42:34.000000 clubscore-0.1.5/
+-rw-r--r--   0 dave       (501) staff       (20)     1071 2023-05-05 17:29:41.000000 clubscore-0.1.5/LICENSE
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-16 21:42:34.000000 clubscore-0.1.5/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       23 2023-05-06 09:41:10.000000 clubscore-0.1.5/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore/
+-rw-r--r--   0 dave       (501) staff       (20)      752 2023-05-09 16:58:15.000000 clubscore-0.1.5/clubscore/API.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.5/clubscore/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore/objects/
+-rw-r--r--   0 dave       (501) staff       (20)     5209 2023-05-11 23:15:54.000000 clubscore-0.1.5/clubscore/objects/CONTAINER.py
+-rw-r--r--   0 dave       (501) staff       (20)     2384 2023-05-11 22:57:05.000000 clubscore-0.1.5/clubscore/objects/IMG.py
+-rw-r--r--   0 dave       (501) staff       (20)     1151 2023-02-04 00:33:04.000000 clubscore-0.1.5/clubscore/objects/RECTANGLE.py
+-rw-r--r--   0 dave       (501) staff       (20)     3921 2023-05-15 16:59:08.000000 clubscore-0.1.5/clubscore/objects/TEXT.py
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-06 08:36:10.000000 clubscore-0.1.5/clubscore/objects/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     3743 2023-05-15 17:01:47.000000 clubscore-0.1.5/clubscore/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      909 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      435 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       85 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       10 2023-05-16 21:42:34.000000 clubscore-0.1.5/clubscore.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-16 21:42:34.000000 clubscore-0.1.5/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1220 2023-05-16 21:35:55.000000 clubscore-0.1.5/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-16 21:42:34.000000 clubscore-0.1.5/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     1961 2023-05-11 23:19:07.000000 clubscore-0.1.5/tests/test_templates.py
+-rw-r--r--   0 dave       (501) staff       (20)      881 2023-05-11 23:17:53.000000 clubscore-0.1.5/tests/test_utils.py
```

### Comparing `clubscore-0.1.4/LICENSE` & `clubscore-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.4/PKG-INFO` & `clubscore-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.4/clubscore/objects/CONTAINER.py` & `clubscore-0.1.5/clubscore/objects/CONTAINER.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,18 @@
             current_y += int(u.getTemplateAttribute(template,"paddingY")) if u.getTemplateAttribute(template,"paddingY") else padding_y
 
         return CONTAINER(image, x + int(dict["x"]), y + int(dict["y"]), width, height, multiple_elements)
 
 
     @staticmethod
     def interpretaTemplate(image, template, lines):
+        if os.environ['ENV'] == 'testing':
+            template = "../" + template
+
+
         tree = ET.parse(template)
         root = tree.getroot()
         children = list(root)
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
 
@@ -138,7 +142,17 @@
         main_container = CONTAINER(image, x, y, width, height, elements)
 
         if root.tag == "MAIN_CONTAINER":
             main_container.inserisci()
         else:
             return elements
 
+
+
+    def create_image_from_template(template, l):
+        width = int(u.getTemplateAttribute(template, "width"))
+        height = int(u.getTemplateAttribute(template, "height"))
+
+        image = Image.new('RGB', (width, height), color=(255, 255, 255))
+        CONTAINER.interpretaTemplate(image, template, l)
+
+        return image
```

### Comparing `clubscore-0.1.4/clubscore/objects/IMG.py` & `clubscore-0.1.5/clubscore/objects/IMG.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PIL import Image
 from io import BytesIO
 from clubscore import utils as u
+import os
 
 
 class IMG:
 
     """
     image: immagine di background di riferimento
     foto: nome del file da recuperare (eventuale)
@@ -50,27 +51,36 @@
 
     """
     costruttore a partire da dizionario XML dell'oggetto
     """
     @staticmethod
     def initiate(image, root, dict, lines):
 
+        if "+" in dict["foto"]:
+            dict["foto"] = lines.pop(0).strip()
 
-        print(lines)
-        if "*" in dict["foto"]:
-            testo = lines.pop(0).strip()
+        else:
 
+            if os.environ['ENV'] == 'testing':
+                dict["foto"] = "../" + dict["foto"]
 
-            path = dict["foto"].split("/*")[0]
-            testo = u.matchWord(testo, u.getTeams(path))
+            if "*" in dict["foto"]:
+                testo = lines.pop(0).strip()
+
+
+                path = dict["foto"].split("/*")[0]
+
+
+
+                testo = u.matchWord(testo, u.getTeams(path))
+
+                #dict["foto"] = dict["foto"].replace("*", testo)
+                dict["foto"] = f"{path}/{testo}.png"
 
-            dict["foto"] = dict["foto"].replace("*", testo)
 
-        elif "+" in dict["foto"]:
-            dict["foto"] = lines.pop(0).strip()
 
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
```

### Comparing `clubscore-0.1.4/clubscore/objects/RECTANGLE.py` & `clubscore-0.1.5/clubscore/objects/RECTANGLE.py`

 * *Files identical despite different names*

### Comparing `clubscore-0.1.4/clubscore/objects/TEXT.py` & `clubscore-0.1.5/clubscore/objects/TEXT.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from PIL import Image, ImageDraw, ImageFont
 import clubscore.utils as u
+import os
 
 class TEXT:
 
     """
     image: immagine di background di riferimento
     test: testo da scrivere
     font_path: font di riferimento  da utilizzare (fornire path)
@@ -25,14 +26,17 @@
         self.perimeter_fill = perimeter_fill
 
     """
     inserisce il testo in maniera agnostica, non sa nulla se non le coordinate, e la dimensione del font
     """
 
     def inserisci(self, relative_x = 0, relative_y = 0):
+        if os.environ['ENV'] == 'testing':
+            self.font_path = "../" + self.font_path
+
         font = ImageFont.truetype(self.font_path, self.size)
         draw = ImageDraw.Draw(self.image)
 
         if self.centerX:
             w = int(draw.textlength(self.testo, font)/2)
         else:
             w = 0
@@ -42,15 +46,15 @@
         else:
             h = 0
 
         if self.perimeter_fill == -1:
             draw.text((int(self.x + relative_x-w), int(self.y + relative_y-h)), self.testo, font=font, fill=self.color)
 
         else:
-            print("entroooo")
+
 
             total_text_width, total_text_height = draw.textsize(self.testo, font=font)
             width_difference = self.perimeter_fill - total_text_width
             gap_width = int(width_difference / (len(self.testo) - 1))
             xpos = self.x
             ypos = self.y
             for letter in self.testo:
@@ -65,26 +69,27 @@
     def initiate(image, root, dict, lines):
 
         if "testo" in dict:
             if "*" in dict["testo"]:
 
                 testo = lines.pop(0).strip()
 
-                if "match_word" in dict and "True" in dict["match_word"]:
-                    testo = u.matchWord(testo, u.getTeams("graphics/teams/squadre.txt"))
+                if "match_word" in dict:
+                    print(dict["match_word"])
+                    testo = u.matchWord(testo, u.getTeams(dict["match_word"]))
 
                 if "upper" in dict and "True" in dict["upper"]:
                     testo = testo.upper()
 
                 dict["testo"] = dict["testo"].replace("*", testo)
 
             final_text = dict["testo"]
 
         elif "concatenation" in dict:
-            print("concatenation", lines)
+
             for i in range(len(lines)):
                 repl = "{%s}" % str(i)
                 if repl in dict["concatenation"]:
                     testo = lines[i].strip()
 
                     if "match_word" in dict and "True" in dict["match_word"]:
                         testo = u.matchWord(testo, u.getTeams("graphics/teams/squadre.txt"))
@@ -98,16 +103,16 @@
             final_text = dict["concatenation"]
 
 
 
         x = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["x"])
         y = 0 if root.tag == "MAIN_CONTAINER" else int(root.attrib["y"])
 
-        print(final_text)
+
 
         perimeter_fill = -1 if "perimeter_fill" not in dict else int(dict["perimeter_fill"])
 
-        print(perimeter_fill)
+
         centerX = True if "centerX" not in dict or dict["centerX"] is "True" else False
         centerY = True if "centerY" not in dict or dict["centerY"] is "True" else False
 
         return TEXT(image, final_text, dict["font"], x + int(dict["x"]), y + int(dict["y"]), int(dict["size"]),dict["color"], centerX, centerY,perimeter_fill)
```

### Comparing `clubscore-0.1.4/clubscore/utils.py` & `clubscore-0.1.5/clubscore/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from PIL import Image, ImageDraw, ImageFont
 import xml.etree.ElementTree as ET
 import difflib
 import os
 import requests
 import logging
+import os
 from bs4 import BeautifulSoup
 
 
 # set the logging level (e.g. DEBUG, INFO, WARNING, ERROR)
 logging.basicConfig(level=logging.INFO)
 
 """
@@ -80,14 +81,17 @@
 
 """
 data una parola, viene restituita quella più vicina tra le disponibili in elenco
 """
 
 
 def matchWord(s, arr):
+    print("ee")
+    print(s)
+    print("gg")
     arr = [x.lower() for x in arr]
     s = s.lower()
 
     match = difflib.get_close_matches(s, arr, n=1, cutoff=0.3)
     if match:
         return match[0]
     else:
@@ -101,33 +105,47 @@
 
 
 def getTeams(path):
     if ".txt" in path:
         f = open(path)
         f = f.readlines()
         f = [s.strip() for s in f]
+        print(f)
         return f
     return list(map(lambda elem: elem.replace('.png', ''), os.listdir(path)))
 
 
 
 def getTemplateText(template,s):
+    if os.environ['ENV'] == 'testing':
+        template = "../" + template
+
     tree = ET.parse(template)
-    example = tree.find(s).text.split("\n")
+    example = tree.find(s)
+
+    if example is None:
+        return []
+
+    example = example.text.split("\n")
+
     s = ""
 
     for el in example:
         s += el.strip() + "\n"
 
     return s
 
 def getTemplateGuide(template):
     return getTemplateText(template,"GUIDA")
 
+
 def getTemplateAttribute(template,attribute):
+    if os.environ['ENV'] == 'testing':
+        template = "../" + template
+
     tree = ET.parse(template)
     root = tree.getroot()
     return root.attrib[attribute] if attribute in root.attrib else False
 
 
 
 def getHockeyItalianoClassificaTable(url):
@@ -140,11 +158,15 @@
 def createHockeyItalianoClassificaList(table):
     rows = table.find_all('tr')
     classifica = []
 
     for i in range(2, len(rows)):
         classifica.append(rows[i].find_all('td')[1].text + "," + rows[i].find_all('td')[2].text)
 
-    print(classifica)
     return classifica
 
 
+def getAbsolutePath(relative_path):
+    absolute_path = os.path.abspath(os.path.join(os.getcwd(), relative_path))
+    return absolute_path
+
+
```

### Comparing `clubscore-0.1.4/clubscore.egg-info/PKG-INFO` & `clubscore-0.1.5/clubscore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clubscore
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for creating customizable templates in XML
 Home-page: https://github.com/davegimo/clubscore
 Author: Davide Gimondo
 Author-email: davegimo@gmail.com
 License: MIT
 Keywords: my-package,example,demo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `clubscore-0.1.4/setup.py` & `clubscore-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clubscore',
-    version='0.1.4',
+    version='0.1.5',
     author='Davide Gimondo',
     author_email='davegimo@gmail.com',
     description='A package for creating customizable templates in XML',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clubscore',
     packages=find_packages(),
```

