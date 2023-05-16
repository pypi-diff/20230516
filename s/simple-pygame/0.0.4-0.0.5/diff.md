# Comparing `tmp/simple_pygame-0.0.4.tar.gz` & `tmp/simple_pygame-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pygame-0.0.4.tar", last modified: Sat Mar  4 13:49:25 2023, max compression
+gzip compressed data, was "simple_pygame-0.0.5.tar", last modified: Tue May 16 16:35:38 2023, max compression
```

## Comparing `simple_pygame-0.0.4.tar` & `simple_pygame-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 13:49:25.178959 simple_pygame-0.0.4/
--rw-rw-rw-   0        0        0     1087 2023-02-13 12:51:16.000000 simple_pygame-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1390 2023-03-04 13:49:25.177956 simple_pygame-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      869 2023-03-04 13:48:17.000000 simple_pygame-0.0.4/README.md
--rw-rw-rw-   0        0        0      604 2023-03-04 13:48:36.000000 simple_pygame-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-04 13:49:25.178959 simple_pygame-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-04 13:49:25.153956 simple_pygame-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-04 13:49:25.161953 simple_pygame-0.0.4/src/simple_pygame/
--rw-rw-rw-   0        0        0      427 2023-03-04 13:39:44.000000 simple_pygame-0.0.4/src/simple_pygame/__init__.py
--rw-rw-rw-   0        0        0      180 2023-02-28 11:50:52.000000 simple_pygame-0.0.4/src/simple_pygame/mixer.py
--rw-rw-rw-   0        0        0    15557 2023-03-04 13:36:23.000000 simple_pygame-0.0.4/src/simple_pygame/music.py
--rw-rw-rw-   0        0        0     6646 2023-03-04 13:36:40.000000 simple_pygame-0.0.4/src/simple_pygame/sound.py
--rw-rw-rw-   0        0        0       21 2023-03-04 13:39:35.000000 simple_pygame-0.0.4/src/simple_pygame/version.py
-drwxrwxrwx   0        0        0        0 2023-03-04 13:49:25.176977 simple_pygame-0.0.4/src/simple_pygame.egg-info/
--rw-rw-rw-   0        0        0     1390 2023-03-04 13:49:25.000000 simple_pygame-0.0.4/src/simple_pygame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-03-04 13:49:25.000000 simple_pygame-0.0.4/src/simple_pygame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 13:49:25.000000 simple_pygame-0.0.4/src/simple_pygame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-04 13:49:25.000000 simple_pygame-0.0.4/src/simple_pygame.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 16:35:38.075778 simple_pygame-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-02-13 12:51:16.000000 simple_pygame-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-05-16 16:35:38.075778 simple_pygame-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2023-05-16 16:09:43.000000 simple_pygame-0.0.5/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-16 16:09:00.000000 simple_pygame-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:35:38.075778 simple_pygame-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 16:35:38.060154 simple_pygame-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 16:35:38.060154 simple_pygame-0.0.5/src/simple_pygame/
+-rw-rw-rw-   0        0        0     1355 2023-05-16 15:52:52.000000 simple_pygame-0.0.5/src/simple_pygame/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-05-16 15:50:51.000000 simple_pygame-0.0.5/src/simple_pygame/constants.py
+-rw-rw-rw-   0        0        0     1172 2023-05-16 15:54:05.000000 simple_pygame-0.0.5/src/simple_pygame/mixer.py
+-rw-rw-rw-   0        0        0    34033 2023-05-16 15:55:07.000000 simple_pygame-0.0.5/src/simple_pygame/music.py
+-rw-rw-rw-   0        0        0     3232 2023-05-16 15:32:02.000000 simple_pygame-0.0.5/src/simple_pygame/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:35:38.075778 simple_pygame-0.0.5/src/simple_pygame.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-05-16 16:35:38.000000 simple_pygame-0.0.5/src/simple_pygame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-16 16:35:38.000000 simple_pygame-0.0.5/src/simple_pygame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:35:38.000000 simple_pygame-0.0.5/src/simple_pygame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 16:35:38.000000 simple_pygame-0.0.5/src/simple_pygame.egg-info/top_level.txt
```

### Comparing `simple_pygame-0.0.4/LICENSE` & `simple_pygame-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_pygame-0.0.4/PKG-INFO` & `simple_pygame-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 Metadata-Version: 2.1
 Name: simple_pygame
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library that provides many features using Pygame and other libraries.
 Author: YoutuberTom
-Project-URL: Homepage, https://github.com/YoutuberTom/Simple_Pygame
+Project-URL: Source, https://github.com/YoutuberTom/Simple_Pygame
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Simple Pygame logo](https://raw.githubusercontent.com/YoutuberTom/Simple_Pygame/main/docs/images/Logo.png)
 
-Simple Pygame is a [Python](https://www.python.org/) library that provides many features using [Pygame](https://www.pygame.org/news) and other libraries. It can help you create multimedia applications much easier and save you a lot of time.
+Simple Pygame is a [Python](https://www.python.org/) library that provides many features using [Pygame](https://www.pygame.org/news) and other libraries. It can help you create multimedia programs much easier and cleaner.
 
 # **Installation:**
 
     pip install simple_pygame
 
 # **Dependencies:**
 
+## Python version:
+
+    Python >= 3.7.0
+
 ## Python libraries:
 
 | Library | Version |
 |:--------|:--------|
 |pygame   |>= 2.0.0 |
-|moviepy  |>= 1.0.0 |
 |pyaudio  |>= 0.2.11|
 
 ## Other requirements:
 
 - ffmpeg.
 
+- ffprobe (optional).
+
 # **Example:**
 
 Go to [examples folder](https://github.com/YoutuberTom/Simple_Pygame/tree/main/examples) for examples.
 
 # **License:**
 
 This library is distributed under [MIT license](https://github.com/YoutuberTom/Simple_Pygame/blob/main/LICENSE).
```

### Comparing `simple_pygame-0.0.4/README.md` & `simple_pygame-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 ![Simple Pygame logo](https://raw.githubusercontent.com/YoutuberTom/Simple_Pygame/main/docs/images/Logo.png)
 
-Simple Pygame is a [Python](https://www.python.org/) library that provides many features using [Pygame](https://www.pygame.org/news) and other libraries. It can help you create multimedia applications much easier and save you a lot of time.
+Simple Pygame is a [Python](https://www.python.org/) library that provides many features using [Pygame](https://www.pygame.org/news) and other libraries. It can help you create multimedia programs much easier and cleaner.
 
 # **Installation:**
 
     pip install simple_pygame
 
 # **Dependencies:**
 
+## Python version:
+
+    Python >= 3.7.0
+
 ## Python libraries:
 
 | Library | Version |
 |:--------|:--------|
 |pygame   |>= 2.0.0 |
-|moviepy  |>= 1.0.0 |
 |pyaudio  |>= 0.2.11|
 
 ## Other requirements:
 
 - ffmpeg.
 
+- ffprobe (optional).
+
 # **Example:**
 
 Go to [examples folder](https://github.com/YoutuberTom/Simple_Pygame/tree/main/examples) for examples.
 
 # **License:**
 
 This library is distributed under [MIT license](https://github.com/YoutuberTom/Simple_Pygame/blob/main/LICENSE).
```

### Comparing `simple_pygame-0.0.4/pyproject.toml` & `simple_pygame-0.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple_pygame"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Python library that provides many features using Pygame and other libraries."
 readme = "README.md"
 requires-python = ">= 3.7"
 authors = [
     {name = "YoutuberTom"}
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Education",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/YoutuberTom/Simple_Pygame"
+"Source" = "https://github.com/YoutuberTom/Simple_Pygame"
```

### Comparing `simple_pygame-0.0.4/src/simple_pygame.egg-info/PKG-INFO` & `simple_pygame-0.0.5/src/simple_pygame.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 Metadata-Version: 2.1
 Name: simple-pygame
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python library that provides many features using Pygame and other libraries.
 Author: YoutuberTom
-Project-URL: Homepage, https://github.com/YoutuberTom/Simple_Pygame
+Project-URL: Source, https://github.com/YoutuberTom/Simple_Pygame
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Simple Pygame logo](https://raw.githubusercontent.com/YoutuberTom/Simple_Pygame/main/docs/images/Logo.png)
 
-Simple Pygame is a [Python](https://www.python.org/) library that provides many features using [Pygame](https://www.pygame.org/news) and other libraries. It can help you create multimedia applications much easier and save you a lot of time.
+Simple Pygame is a [Python](https://www.python.org/) library that provides many features using [Pygame](https://www.pygame.org/news) and other libraries. It can help you create multimedia programs much easier and cleaner.
 
 # **Installation:**
 
     pip install simple_pygame
 
 # **Dependencies:**
 
+## Python version:
+
+    Python >= 3.7.0
+
 ## Python libraries:
 
 | Library | Version |
 |:--------|:--------|
 |pygame   |>= 2.0.0 |
-|moviepy  |>= 1.0.0 |
 |pyaudio  |>= 0.2.11|
 
 ## Other requirements:
 
 - ffmpeg.
 
+- ffprobe (optional).
+
 # **Example:**
 
 Go to [examples folder](https://github.com/YoutuberTom/Simple_Pygame/tree/main/examples) for examples.
 
 # **License:**
 
 This library is distributed under [MIT license](https://github.com/YoutuberTom/Simple_Pygame/blob/main/LICENSE).
```

