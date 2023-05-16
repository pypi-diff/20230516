# Comparing `tmp/bingwallpaperpy-0.1.4.tar.gz` & `tmp/bingwallpaperpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingwallpaperpy-0.1.4.tar", max compression
+gzip compressed data, was "bingwallpaperpy-0.1.5.tar", max compression
```

## Comparing `bingwallpaperpy-0.1.4.tar` & `bingwallpaperpy-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-03-29 08:25:14.205910 bingwallpaperpy-0.1.4/LICENSE
--rw-r--r--   0        0        0      750 2023-03-29 09:08:30.122656 bingwallpaperpy-0.1.4/README.md
--rw-r--r--   0        0        0       79 2023-03-29 07:46:42.295840 bingwallpaperpy-0.1.4/bingwallpaperpy/__main__.py
--rw-r--r--   0        0        0      810 2023-03-29 08:37:33.279266 bingwallpaperpy-0.1.4/bingwallpaperpy/bingwallpaper.py
--rw-r--r--   0        0        0      539 2023-03-29 09:12:50.485998 bingwallpaperpy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 bingwallpaperpy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-29 08:25:14.205910 bingwallpaperpy-0.1.5/LICENSE
+-rw-r--r--   0        0        0      750 2023-03-29 09:08:30.122656 bingwallpaperpy-0.1.5/README.md
+-rw-r--r--   0        0        0       79 2023-03-29 07:46:42.295840 bingwallpaperpy-0.1.5/bingwallpaperpy/__main__.py
+-rw-r--r--   0        0        0      844 2023-05-16 07:20:21.946826 bingwallpaperpy-0.1.5/bingwallpaperpy/bingwallpaper.py
+-rw-r--r--   0        0        0      539 2023-05-16 07:21:35.740165 bingwallpaperpy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 bingwallpaperpy-0.1.5/PKG-INFO
```

### Comparing `bingwallpaperpy-0.1.4/LICENSE` & `bingwallpaperpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bingwallpaperpy-0.1.4/README.md` & `bingwallpaperpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bingwallpaperpy-0.1.4/bingwallpaperpy/bingwallpaper.py` & `bingwallpaperpy-0.1.5/bingwallpaperpy/bingwallpaper.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 
 def download():
     '''Download today's Bing wallpaper.'''
     resp = requests.get(URL)
     if resp.ok:
         xml = ET.fromstring(resp.content)
         img_url = xml.find("./image/url").text
+        print(BASE_URL + img_url)
         resp = requests.get(BASE_URL + img_url)
         if resp.ok:
             img = Image.open(BytesIO(resp.content))
             img.save(DEST)
             print(DEST)
```

### Comparing `bingwallpaperpy-0.1.4/pyproject.toml` & `bingwallpaperpy-0.1.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bingwallpaperpy"
-version = "0.1.4"
+version = "0.1.5"
 description = "Download script for Bing daily wallpapers."
 authors = ["Jens Korinth <jkorinth@gmx.net>"]
 repository = "https://github.com/jkorinth/bingwallpaper-py"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `bingwallpaperpy-0.1.4/PKG-INFO` & `bingwallpaperpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingwallpaperpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Download script for Bing daily wallpapers.
 Home-page: https://github.com/jkorinth/bingwallpaper-py
 License: GPL-3.0-or-later
 Author: Jens Korinth
 Author-email: jkorinth@gmx.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

