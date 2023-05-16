# Comparing `tmp/streamlit-deckgl-0.2.1.tar.gz` & `tmp/streamlit-deckgl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deckgl-0.2.1.tar", last modified: Mon May  8 19:48:16 2023, max compression
+gzip compressed data, was "streamlit-deckgl-0.3.0.tar", last modified: Tue May 16 00:07:39 2023, max compression
```

## Comparing `streamlit-deckgl-0.2.1.tar` & `streamlit-deckgl-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.2.1/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-08 19:48:11.000000 streamlit-deckgl-0.2.1/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.130981 streamlit-deckgl-0.2.1/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.130981 streamlit-deckgl-0.2.1/src/streamlit_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2188 2023-05-08 19:23:55.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     2004 2023-05-05 05:17:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.130981 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-08 19:48:16.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.3.0/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-16 00:03:31.000000 streamlit-deckgl-0.3.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.338717 streamlit-deckgl-0.3.0/src/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.338717 streamlit-deckgl-0.3.0/src/streamlit_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-05-15 20:40:20.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      816 2023-05-15 23:58:43.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3348 2023-05-16 00:01:14.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/main.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/style.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-16 00:07:39.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/top_level.txt
```

### Comparing `streamlit-deckgl-0.2.1/LICENSE` & `streamlit-deckgl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.2.1/PKG-INFO` & `streamlit-deckgl-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.2.1
+Version: 0.3.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-deckgl-0.2.1/README.md` & `streamlit-deckgl-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.2.1/setup.py` & `streamlit-deckgl-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-deckgl",
-    version="0.2.1",
+    version="0.3.0",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for deck.gl visualisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_deckgl"],
     package_dir={"": "src"},
```

### Comparing `streamlit-deckgl-0.2.1/src/streamlit_deckgl/__init__.py` & `streamlit-deckgl-0.3.0/src/streamlit_deckgl/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 def st_deckgl(
     deck: pdk.Deck,
     key: Optional[str] = "deck_gl",
     height: int = 500,
     events: Optional[list] = None,
     description: Optional[dict] = None,
     configuration: Optional[dict] = None,
+    overlay: Optional[pdk.Layer] = None,
 ):
     """Create a deck.gl map in Streamlit.
 
     Parameters
     ==========
     deck : pydeck.Deck instance
         The pydeck map to render.
@@ -38,32 +39,41 @@
         - 'hover'
         - 'drag'
     description : dict, default None
         A dictionary with additional description components to overlay on the map
         The keys are the position which can be one of 'top-right','top-left','bottom-right','bottom-left'
         The values are the html elements to place in each position
         Example {'top-right':<div>This is a nice map</div>}
+    overlay:pydeck.Layer instance, default None
+        A second pydeck layer to overlay on the map - useful for land masks etc.
     configuration : dict, default None
         A dictionary of configuration options for the map.
 
     Returns
     =======
     component_value : dict
         A dictionary containing the info dictionary of the event.
 
     """
     json = deck.to_json()
+    overlay_json = overlay.to_json() if overlay else None
     customLibraries = pdk.settings.custom_libraries
     configuration = pdk.settings.configuration
 
+    mapbox_key = deck.mapbox_key or (overlay and overlay.mapbox_key)
+    google_maps_key = deck.google_maps_key or (overlay and overlay.google_maps_key)
+
     component_value = _component_func(
         key=key,
         height=height,
         spec=json,
         tooltip=deck._tooltip,
         customLibraries=customLibraries,
         configuration=configuration,
         events=events,
         description=description,
+        overlay=overlay_json,
+        mapbox_key=mapbox_key,
+        google_maps_key=google_maps_key,
     )
 
     return component_value
```

### Comparing `streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/index.html` & `streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -10,10 +10,11 @@
     <script src="https://unpkg.com/@deck.gl/json@8.8.9/dist.min.js"></script>
     <script src="https://unpkg.com/@deck.gl/carto@8.8.9/dist.min.js"></script>
     <script src="https://unpkg.com/@deck.gl/jupyter-widget@8.8.9/dist/index.js"></script>
     <script src="./main.js"></script>
     <link rel="stylesheet" href="./style.css" />
   </head>
   <body>
-    <div id="root"></div>
+    <div id="deckgl-primary"></div>
+    <div id="deckgl-overlay"></div>
   </body>
 </html>
```

### Comparing `streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js` & `streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/PKG-INFO` & `streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.2.1
+Version: 0.3.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

