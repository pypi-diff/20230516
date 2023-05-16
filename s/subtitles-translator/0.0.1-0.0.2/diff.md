# Comparing `tmp/subtitles_translator-0.0.1.tar.gz` & `tmp/subtitles_translator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtitles_translator-0.0.1.tar", max compression
+gzip compressed data, was "subtitles_translator-0.0.2.tar", max compression
```

## Comparing `subtitles_translator-0.0.1.tar` & `subtitles_translator-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-05-15 10:52:05.340510 subtitles_translator-0.0.1/LICENSE
--rw-r--r--   0        0        0     2768 2023-05-15 10:52:05.340510 subtitles_translator-0.0.1/README.md
--rw-r--r--   0        0        0     2127 2023-05-15 10:53:14.041038 subtitles_translator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 10:52:05.344510 subtitles_translator-0.0.1/subtitles_translator/__init__.py
--rw-r--r--   0        0        0      547 2023-05-15 10:52:05.344510 subtitles_translator-0.0.1/subtitles_translator/available_languages.py
--rw-r--r--   0        0        0     3411 2023-05-15 10:52:05.344510 subtitles_translator-0.0.1/subtitles_translator/cli.py
--rw-r--r--   0        0        0     1507 2023-05-15 10:52:05.344510 subtitles_translator-0.0.1/subtitles_translator/ffmpeg_utils.py
--rw-r--r--   0        0        0     3111 2023-05-15 10:52:05.344510 subtitles_translator-0.0.1/subtitles_translator/subtitles.py
--rw-r--r--   0        0        0     5179 2023-05-15 10:52:05.344510 subtitles_translator-0.0.1/subtitles_translator/translator.py
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 subtitles_translator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 10:15:09.626561 subtitles_translator-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2906 2023-05-16 10:15:09.626561 subtitles_translator-0.0.2/README.md
+-rw-r--r--   0        0        0     2127 2023-05-16 10:16:04.375248 subtitles_translator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 10:15:09.630561 subtitles_translator-0.0.2/subtitles_translator/__init__.py
+-rw-r--r--   0        0        0      547 2023-05-16 10:15:09.630561 subtitles_translator-0.0.2/subtitles_translator/available_languages.py
+-rw-r--r--   0        0        0     3411 2023-05-16 10:15:09.630561 subtitles_translator-0.0.2/subtitles_translator/cli.py
+-rw-r--r--   0        0        0     1481 2023-05-16 10:15:09.630561 subtitles_translator-0.0.2/subtitles_translator/ffmpeg_utils.py
+-rw-r--r--   0        0        0     3111 2023-05-16 10:15:09.630561 subtitles_translator-0.0.2/subtitles_translator/subtitles.py
+-rw-r--r--   0        0        0     5179 2023-05-16 10:15:09.630561 subtitles_translator-0.0.2/subtitles_translator/translator.py
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 subtitles_translator-0.0.2/PKG-INFO
```

### Comparing `subtitles_translator-0.0.1/LICENSE` & `subtitles_translator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subtitles_translator-0.0.1/README.md` & `subtitles_translator-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Neural Subtitles Translator
 
 [![Release](https://img.shields.io/github/v/release/tdhm/subtitles-translator)](https://img.shields.io/github/v/release/tdhm/subtitles-translator)
 [![Build status](https://img.shields.io/github/actions/workflow/status/tdhm/subtitles-translator/main.yml?branch=main)](https://github.com/tdhm/subtitles-translator/actions/workflows/main.yml?query=branch%3Amain)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/subtitles-translator.svg)](https://pypi.python.org/pypi/subtitles-translator/)
 [![codecov](https://codecov.io/gh/tdhm/subtitles-translator/branch/main/graph/badge.svg)](https://codecov.io/gh/tdhm/subtitles-translator)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/tdhm/subtitles-translator)](https://img.shields.io/github/commit-activity/m/tdhm/subtitles-translator)
 [![License](https://img.shields.io/github/license/tdhm/subtitles-translator)](https://img.shields.io/github/license/tdhm/subtitles-translator)
 
 Automatic subtitles translation with a local neural machine translation model. No third-party service required: the translation is done locally with small but efficient neural network models.
 
 > **Github repository**: <https://github.com/tdhm/subtitles-translator/>
 
-> **Documentation** <https://tdhm.github.io/subtitles-translator/>
+> **Documentation** <https://tdhm.github.io/Subtitles-Translator/>
 
 Original movie in French            |  Output of automatic translation
 :-------------------------:|:-------------------------:
 ![](./docs/img/bon_voyage_fr.png)  |  ![](./docs/img/bon_voyage_en.png)
 
 > **Note**
 > Screenshots are taken from *Bon voyage*, a short French language propaganda film made by Alfred Hitchcock for the British Ministry of Information.
```

### Comparing `subtitles_translator-0.0.1/pyproject.toml` & `subtitles_translator-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subtitles_translator"
-version = "v0.0.1"
+version = "v0.0.2"
 description = "Automatic subtitles translation with a local neural machine translation model. No third-party service required: the translation is done locally with small but efficient neural network models."
 authors = ["TDHM <tdhm-git@outlook.com>"]
 repository = "https://github.com/tdhm/subtitles-translator"
 documentation = "https://tdhm.github.io/subtitles-translator/"
 readme = "README.md"
 packages = [
   {include = "subtitles_translator"}
```

### Comparing `subtitles_translator-0.0.1/subtitles_translator/available_languages.py` & `subtitles_translator-0.0.2/subtitles_translator/available_languages.py`

 * *Files identical despite different names*

### Comparing `subtitles_translator-0.0.1/subtitles_translator/cli.py` & `subtitles_translator-0.0.2/subtitles_translator/cli.py`

 * *Files identical despite different names*

### Comparing `subtitles_translator-0.0.1/subtitles_translator/ffmpeg_utils.py` & `subtitles_translator-0.0.2/subtitles_translator/ffmpeg_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,17 +17,16 @@
     Returns:
         str: Full subtitles in srt format
 
     """
 
     # Use subprocess to call FFmpeg CLI
     out = sp.run(["ffmpeg", "-i", video_path, "-map", "s:0", "-f", "srt", "-"], capture_output=True, text=True)
-    subtitles = out.stdout
 
-    return subtitles
+    return out.stdout
 
 
 def insert_srt(video_path: str, output_path: str, srt_path: str) -> None:
     """Use FFmpeg to insert a new subtitles track.
 
     Args:
         video_path (str): Path to the source movie file
```

### Comparing `subtitles_translator-0.0.1/subtitles_translator/subtitles.py` & `subtitles_translator-0.0.2/subtitles_translator/subtitles.py`

 * *Files identical despite different names*

### Comparing `subtitles_translator-0.0.1/subtitles_translator/translator.py` & `subtitles_translator-0.0.2/subtitles_translator/translator.py`

 * *Files identical despite different names*

### Comparing `subtitles_translator-0.0.1/PKG-INFO` & `subtitles_translator-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subtitles-translator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automatic subtitles translation with a local neural machine translation model. No third-party service required: the translation is done locally with small but efficient neural network models.
 Home-page: https://github.com/tdhm/subtitles-translator
 Author: TDHM
 Author-email: tdhm-git@outlook.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,23 +17,24 @@
 Project-URL: Repository, https://github.com/tdhm/subtitles-translator
 Description-Content-Type: text/markdown
 
 # Neural Subtitles Translator
 
 [![Release](https://img.shields.io/github/v/release/tdhm/subtitles-translator)](https://img.shields.io/github/v/release/tdhm/subtitles-translator)
 [![Build status](https://img.shields.io/github/actions/workflow/status/tdhm/subtitles-translator/main.yml?branch=main)](https://github.com/tdhm/subtitles-translator/actions/workflows/main.yml?query=branch%3Amain)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/subtitles-translator.svg)](https://pypi.python.org/pypi/subtitles-translator/)
 [![codecov](https://codecov.io/gh/tdhm/subtitles-translator/branch/main/graph/badge.svg)](https://codecov.io/gh/tdhm/subtitles-translator)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/tdhm/subtitles-translator)](https://img.shields.io/github/commit-activity/m/tdhm/subtitles-translator)
 [![License](https://img.shields.io/github/license/tdhm/subtitles-translator)](https://img.shields.io/github/license/tdhm/subtitles-translator)
 
 Automatic subtitles translation with a local neural machine translation model. No third-party service required: the translation is done locally with small but efficient neural network models.
 
 > **Github repository**: <https://github.com/tdhm/subtitles-translator/>
 
-> **Documentation** <https://tdhm.github.io/subtitles-translator/>
+> **Documentation** <https://tdhm.github.io/Subtitles-Translator/>
 
 Original movie in French            |  Output of automatic translation
 :-------------------------:|:-------------------------:
 ![](./docs/img/bon_voyage_fr.png)  |  ![](./docs/img/bon_voyage_en.png)
 
 > **Note**
 > Screenshots are taken from *Bon voyage*, a short French language propaganda film made by Alfred Hitchcock for the British Ministry of Information.
```

