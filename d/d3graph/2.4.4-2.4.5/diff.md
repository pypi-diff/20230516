# Comparing `tmp/d3graph-2.4.4.tar.gz` & `tmp/d3graph-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3graph-2.4.4.tar", last modified: Sat Apr 29 17:13:55 2023, max compression
+gzip compressed data, was "dist\d3graph-2.4.5.tar", last modified: Tue May 16 17:53:03 2023, max compression
```

## Comparing `d3graph-2.4.4.tar` & `d3graph-2.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.088237 d3graph-2.4.4/
--rw-rw-rw-   0        0        0     1700 2022-05-20 19:47:24.000000 d3graph-2.4.4/LICENSE
--rw-rw-rw-   0        0        0       82 2022-05-20 19:47:24.000000 d3graph-2.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6248 2023-04-29 17:13:55.089234 d3graph-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     5708 2023-03-10 17:10:19.000000 d3graph-2.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:13:54.950057 d3graph-2.4.4/d3graph/
--rw-rw-rw-   0        0        0     1652 2023-04-29 17:13:42.000000 d3graph-2.4.4/d3graph/__init__.py
--rw-rw-rw-   0        0        0     3510 2022-09-03 19:39:37.000000 d3graph-2.4.4/d3graph/adjmat_vec.py
--rw-rw-rw-   0        0        0    53952 2023-04-29 14:59:55.000000 d3graph-2.4.4/d3graph/d3graph.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.061949 d3graph-2.4.4/d3graph/d3js/
--rw-rw-rw-   0        0        0        0 2022-05-20 19:47:24.000000 d3graph-2.4.4/d3graph/d3js/__init__.py
--rw-rw-rw-   0        0        0   347498 2022-05-20 19:47:24.000000 d3graph-2.4.4/d3graph/d3js/d3.v3.js
--rw-rw-rw-   0        0        0    11062 2023-04-29 14:47:58.000000 d3graph-2.4.4/d3graph/d3js/d3graphscript.js
--rw-rw-rw-   0        0        0     1253 2023-03-19 19:25:32.000000 d3graph-2.4.4/d3graph/d3js/index.html.j2
--rw-rw-rw-   0        0        0      275 2022-05-20 19:47:24.000000 d3graph-2.4.4/d3graph/d3js/style.css
--rw-rw-rw-   0        0        0    16539 2023-04-29 16:20:31.000000 d3graph-2.4.4/d3graph/examples.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.014275 d3graph-2.4.4/d3graph.egg-info/
--rw-rw-rw-   0        0        0     6248 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-04-29 17:13:55.108375 d3graph-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-02-17 16:15:40.000000 d3graph-2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.087241 d3graph-2.4.4/tests/
--rw-rw-rw-   0        0        0        0 2022-09-03 19:39:37.000000 d3graph-2.4.4/tests/__init__.py
--rw-rw-rw-   0        0        0      707 2022-09-03 19:39:37.000000 d3graph-2.4.4/tests/conftest.py
--rw-rw-rw-   0        0        0     1072 2022-11-17 10:04:29.000000 d3graph-2.4.4/tests/test_d3graph.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.120359 d3graph-2.4.5/
+-rw-rw-rw-   0        0        0     1700 2022-05-20 19:47:24.000000 d3graph-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0       82 2022-05-20 19:47:24.000000 d3graph-2.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6289 2023-05-16 17:53:03.120359 d3graph-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5708 2023-03-10 17:10:19.000000 d3graph-2.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.099385 d3graph-2.4.5/d3graph/
+-rw-rw-rw-   0        0        0     1652 2023-05-16 17:51:26.000000 d3graph-2.4.5/d3graph/__init__.py
+-rw-rw-rw-   0        0        0     3510 2022-09-03 19:39:37.000000 d3graph-2.4.5/d3graph/adjmat_vec.py
+-rw-rw-rw-   0        0        0    56679 2023-05-16 17:11:42.000000 d3graph-2.4.5/d3graph/d3graph.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.117340 d3graph-2.4.5/d3graph/d3js/
+-rw-rw-rw-   0        0        0        0 2022-05-20 19:47:24.000000 d3graph-2.4.5/d3graph/d3js/__init__.py
+-rw-rw-rw-   0        0        0   347498 2022-05-20 19:47:24.000000 d3graph-2.4.5/d3graph/d3js/d3.v3.js
+-rw-rw-rw-   0        0        0    11158 2023-05-16 10:08:09.000000 d3graph-2.4.5/d3graph/d3js/d3graphscript.js
+-rw-rw-rw-   0        0        0     1253 2023-05-16 10:07:47.000000 d3graph-2.4.5/d3graph/d3js/index.html.j2
+-rw-rw-rw-   0        0        0      275 2022-05-20 19:47:24.000000 d3graph-2.4.5/d3graph/d3js/style.css
+-rw-rw-rw-   0        0        0    18011 2023-05-16 13:01:27.000000 d3graph-2.4.5/d3graph/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.111354 d3graph-2.4.5/d3graph.egg-info/
+-rw-rw-rw-   0        0        0     6289 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 17:53:02.000000 d3graph-2.4.5/d3graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-05-16 17:53:03.124323 d3graph-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1687 2023-02-17 16:15:40.000000 d3graph-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:53:03.119334 d3graph-2.4.5/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-03 19:39:37.000000 d3graph-2.4.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      707 2022-09-03 19:39:37.000000 d3graph-2.4.5/tests/conftest.py
+-rw-rw-rw-   0        0        0     1072 2022-11-17 10:04:29.000000 d3graph-2.4.5/tests/test_d3graph.py
```

### Comparing `d3graph-2.4.4/LICENSE` & `d3graph-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/PKG-INFO` & `d3graph-2.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: d3graph
-Version: 2.4.4
+Version: 2.4.5
 Summary: Python package to create interactive network based on d3js.
 Home-page: https://erdogant.github.io/d3graph
-Download-URL: https://github.com/erdogant/d3graph/archive/2.4.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/d3graph/archive/2.4.5.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -115,7 +117,9 @@
 ### Citation
 Please cite d3graph in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
+
+
```

### Comparing `d3graph-2.4.4/README.md` & `d3graph-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/d3graph/__init__.py` & `d3graph-2.4.5/d3graph/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     json_create,
     adjmat2dict,
     data_checks,
     )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.4.4'
+__version__ = '2.4.5'
 
 
 # module level doc-string
 __doc__ = """
 d3graph
 =======================================================================================
```

### Comparing `d3graph-2.4.4/d3graph/adjmat_vec.py` & `d3graph-2.4.5/d3graph/adjmat_vec.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/d3graph/d3graph.py` & `d3graph-2.4.5/d3graph/d3graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -152,15 +152,16 @@
 
         self.config['figsize'] = figsize
         self.config['network_title'] = title
         self.config['show_slider'] = show_slider
         self.config['showfig'] = showfig
         self.config['notebook'] = notebook
         self.config['click'] = click
-        self.config['filepath'] = self.set_path(filepath)
+        # self.config['filepath'] = self.set_path(filepath)
+        if self.config.get('filepath', None)!='d3graph.html': self.config['filepath'] = self.set_path(filepath)
 
         # Create dataframe from co-occurrence matrix
         self.G = make_graph(self.node_properties, self.edge_properties)
         # Make slider
         self.setup_slider()
         # Create json
         json_data = json_create(self.G)
@@ -190,95 +191,112 @@
             file_location = os.path.abspath(self.config['filepath'])
             if platform == "darwin":  # check if on OSX
                 file_location = "file:///" + file_location
             if os.path.isfile(file_location):
                 webbrowser.open(file_location, new=2)
 
     def set_edge_properties(self,
-                            edge_distance: int = None,
+                            edge_distance=None,
+                            edge_weight=None,
                             scaler: str = 'zscore',
-                            minmax: List[float] = None,
                             directed: bool = False,
                             marker_start=None,
                             marker_end='arrow',
                             marker_color='#808080',
                             label: str = None,
                             label_color = '#808080',
-                            label_fontsize : int = 8) -> dict:
+                            label_fontsize: int = 8,
+                            minmax: List[float] = [0.5, 15],
+                            minmax_distance: List[float] = [50, 100],
+                            ) -> dict:
         """Edge properties.
 
         Parameters
         ----------
-        edge_distance : Int (default: 30)
-            Distance of nodes on the edges.
-            * 0: Weighted approach using edge weights in the adjacency matrix. Weights are normalized between the minmax
-            * 80: Constant edge distance
+        edge_distance : Int (default: 50)
+            Distance between the edges.
+            * None: Distance is based on the weights in the adjacency matrix. Weights are normalized between the minmax
+            * 50: Constant edge distance
+        edge_weight : Int (default: 10)
+            Thickness of the edges.
+            * None: Weighted approach using edge weights in the adjacency matrix. Weights are normalized between the minmax
+            * 10: Constant edge distance
         scaler : str, (default: 'zscore')
             Scale the edge-width using the following scaler:
             'zscore' : Scale values to Z-scores.
             'minmax' : The sklearn scaler will shrink the distribution between minmax.
             None : No scaler is used.
-        minmax : tuple(float, float), (default: [0.5, 15.0])
-            Weights are normalized between minimum and maximum
-            * [0.5, 15]
         directed : Bool, (default: False)
             True: Edges are shown with an marker (e.g. arrow)
             False: Edges do not show markers.
         marker_start : (list of) str, (default: 'arrow')
             The start of the edge can be one of the following markers:
             'arrow','square','circle','stub',None or ''
         marker_end : (list of) str, (default: 'arrow')
             The end of the edge can be one of the following markers:
             'arrow','square','circle','stub',None or ''
         marker_color : str, (default: '#808080')
             The label color in hex.
         label : str, (default: '')
-            The edge label.
+            None : No labels
+            'weight' : This will add the weights on each edge.
+            list : The edge label.
         label_color : str, (default: None)
             The label color in hex.
             None : Inherits the color from marker_color.
         label_fontsize : int, (default: 8)
             The fontsize of the label.
+        minmax : tuple(float, float), (default: [0.5, 15.0])
+            Edge thickness is normalized between minimum and maximum
+            * [0.5, 15]
+            * None: Do not change
+        minmax_distance : tuple(float, float), (default: [50, 100])
+            Distances are normalized between minimum and maximum
+            * [50, 100]
+            * None: Do not change
 
         Returns
         -------
         edge_properties: dict
             key: (source, target)
                 'weight': weight of the edge
                 'weight_scaled': scaled weight of the edge
                 'color': color of the edge
 
         """
-        if minmax is None: minmax = [0.5, 15.0]
         self.config['directed'] = directed
-        self.config['edge_distance'] = 30 if edge_distance is None else edge_distance
+        self.config['edge_weight'] = edge_weight
+        self.config['edge_distance'] = edge_distance
         self.config['minmax'] = minmax
+        self.config['minmax_distance'] = minmax_distance
         self.config['edge_scaler'] = scaler
         self.config['marker_start'] = marker_start
         self.config['marker_end'] = marker_end
         self.config['marker_color'] = marker_color
         self.config['label'] = label
         self.config['label_color'] = label_color
         self.config['label_fontsize'] = label_fontsize
 
         if (not directed) and (marker_end is not None) or (marker_start is not None):
             logger.info('Set directed=True to see the markers!')
 
         # Set the edge properties
-        # Set the edge properties
         self.edge_properties = adjmat2dict(self.adjmat,
-                                           min_weight=0,
+                                           filter_weight=0,
                                            minmax=self.config['minmax'],
+                                           minmax_distance=self.config['minmax_distance'],
                                            scaler=self.config['edge_scaler'],
                                            marker_start=self.config['marker_start'],
                                            marker_end=self.config['marker_end'],
                                            marker_color=self.config['marker_color'],
                                            label=self.config['label'],
                                            label_color=self.config['label_color'],
                                            label_fontsize=self.config['label_fontsize'],
+                                           edge_weight=self.config['edge_weight'],
+                                           edge_distance=self.config['edge_distance'],
                                            )
 
         logger.debug('Number of edges: %.0d', len(self.edge_properties.keys()))
 
     def set_node_properties(self,
                             label: List[str] = None,
                             tooltip: List[str] = None,
@@ -643,14 +661,15 @@
             self.config['click'] = {}
         click_properties = {**{'fill': "function(d) {return d.node_color;}", 'stroke': 'black', 'size': 1.3, 'stroke-width': 3}, **self.config['click']}
         if click_properties.get('fill', None) is None:
             click_properties['fill'] = "function(d) {return d.node_color;}"
         # Set quotes surrounding the color name
         if click_properties['fill'] != "function(d) {return d.node_color;}":
             click_properties['fill'] = '"' + click_properties['fill'] + '"'
+        if self.config['edge_distance'] is None: self.config['edge_distance']=50
 
         # Hide slider
         show_slider = ['', ''] if self.config['show_slider'] else ['<!--', '-->']
         # Set width and height to screen resolution if None.
         width = 'window.screen.width' if self.config['figsize'][0] is None else self.config['figsize'][0]
         height = 'window.screen.height' if self.config['figsize'][1] is None else self.config['figsize'][1]
 
@@ -746,15 +765,15 @@
             target = ['node F', 'node B', 'node J', 'node F', 'node F', 'node M', 'node M', 'node A']
             weight = [5.56, 0.5, 0.64, 0.23, 0.9, 3.28, 0.5, 0.45]
             adjmat = vec2adjmat(source, target, weight=weight)
             return adjmat, None
         elif network == 'bigbang':
             source = ['Penny', 'Penny', 'Amy', 'Bernadette', 'Bernadette', 'Sheldon', 'Sheldon', 'Sheldon', 'Rajesh']
             target = ['Leonard', 'Amy', 'Bernadette', 'Rajesh', 'Howard', 'Howard', 'Leonard', 'Amy', 'Penny']
-            weight = [5, 3, 2, 2, 5, 2, 3, 5, 2]
+            weight = [5, 3, 2, 2, 5, 2, 3, 5, 10]
             adjmat = vec2adjmat(source, target, weight=weight)
             return adjmat, None
         elif network == 'karate':
             import scipy
             if version.parse(scipy.__version__) < version.parse('1.8.0'):
                 raise ImportError(
                     '[d3graph] >Error: This release requires scipy version >= 1.8.0. Try: pip install -U scipy>=1.8.0')
@@ -801,30 +820,34 @@
     edges = [*G.edges()]
     source = []
     target = []
     for edge in edges:
         source.append(node_id[edge[0] == node_ui][0])
         target.append(node_id[edge[1] == node_ui][0])
 
+    # Set edge properties
     links = pd.DataFrame([*G.edges.values()]).T.to_dict()
     links_new = []
     for i in range(len(links)):
         links[i]['edge_width'] = links[i].pop('weight_scaled')
+        links[i]['edge_distance'] = links[i].pop('edge_distance')
         links[i]['edge_weight'] = links[i]['weight']
         links[i]['source'] = int(source[i])
         links[i]['target'] = int(target[i])
         links[i]['source_label'] = edges[i][0]
         links[i]['target_label'] = edges[i][1]
         links[i]['marker_start'] = links[i]['marker_start']
         links[i]['marker_end'] = links[i]['marker_end']
         links[i]['marker_color'] = links[i]['marker_color']
         links[i]['label'] = links[i]['label']
         links[i]['label_color'] = links[i]['label_color']
         links[i]['label_fontsize'] = links[i]['label_fontsize']
         links_new.append(links[i])
+
+    # Set node properties
     nodes = pd.DataFrame([*G.nodes.values()]).T.to_dict()
     nodes_new = [None] * len(nodes)
     for i, node in enumerate(nodes):
         nodes[i]['node_name'] = nodes[i].pop('label')
         # nodes[i]['node_label'] = nodes[i].pop('label')
         nodes[i]['node_tooltip'] = nodes[i].pop('tooltip')
         nodes[i]['node_color'] = nodes[i].pop('color')
@@ -837,110 +860,136 @@
         nodes_new[i] = nodes[i]
     data = {'links': links_new, 'nodes': nodes_new}
     return dumps(data, separators=(',', ':'))
 
 
 # %%  Convert adjacency matrix to vector
 def adjmat2dict(adjmat: pd.DataFrame,
-                min_weight: float = 0.0,
+                filter_weight: float = 0.0,
                 scaler: str = 'zscore',
-                minmax=None,
                 marker_start=None,
                 marker_end='arrow',
                 marker_color='#808080',
                 label=None,
                 label_color='#808080',
                 label_fontsize: int = 8,
+                edge_weight: int = 1,
+                edge_distance: int = 50,
+                minmax: list[float] = [0.5, 15],
+                minmax_distance: list[float] = [50, 100],
                 ) -> dict:
     """Convert adjacency matrix into vector with source and target.
 
     Parameters
     ----------
     adjmat : pd.DataFrame()
         Adjacency matrix.
-    min_weight : float
+    filter_weight : float
         edges are returned with a minimum weight.
     scaler : str, (default: 'zscore')
         Scale the edge-width using the following scaler:
         'zscore' : Scale values to Z-scores.
         'minmax' : The sklearn scaler will shrink the distribution between minmax.
         None : No scaler is used.
-    minmax : tuple(int,int), (default: [0.5, 15])
-        Weights are normalized between minimum and maximum
-        * [0.5, 15]
     marker_start : (list of) str, (default: 'arrow')
         The start of the edge can be one of the following markers:
         'arrow','square','circle','stub',None or ''
     marker_end : (list of) str, (default: 'arrow')
         The end of the edge can be one of the following markers:
         'arrow','square','circle','stub',None or ''
     marker_color : str, (default: '#808080')
         The label color in hex.
     label : str, (default: None)
-        The edge label.
+        None : No label
+        'weight' : Weight of the edge
+        list : The edge label.
     label_color : str, (default: None)
         The label color in hex.
         None : Inherits the color from marker_color.
     label_fontsize : int, (default: 8)
         The fontsize of the label.
+    minmax : tuple(int,int), (default: [0.5, 15])
+        Thickness of the edges are normalized between minimum and maximum
+        * [0.5, 15]
+        * None: Do not change
+    minmax_distance : tuple(int,int), (default: [50, 100])
+        Distances between the edges are normalized between minimum and maximum
+        * [50, 100]
+        * None: Do not change
 
     Returns
     -------
     edge_properties: dict
         key: (source, target)
             'weight': weight of the edge.
-            'weight_scaled': scaled weight of the edge.
+            'weight_scaled': scaled weight (thickness) of the edge.
+            'edge_distance': scaled distance of the edge.
             'color': color of the edge.
             'marker_start': '', 'circle', 'square', 'arrow', 'stub'
             'marker_end': '', 'circle', 'square', 'arrow', 'stub'
             'marker_color': hex color of the marker.
             'label': Text label for the edge.
             'label_color': color of the label.
             'label_fontsize': fontsize of the label.
 
     """
     # Convert adjacency matrix into vector
-    if minmax is None: minmax = [0.5, 15]
     df = adjmat.stack().reset_index()
     # Set columns
     df.columns = ['source', 'target', 'weight']
     # Remove self loops and no-connected edges
     Iloc = df['source'] != df['target']
     # Keep only edges with a minimum edge strength
-    if min_weight is not None:
-        logger.info("Keep only edges with weight>%g" % min_weight)
-        Iloc2 = df['weight'] > min_weight
+    if filter_weight is not None:
+        logger.info("Keep only edges with weight>%g" % filter_weight)
+        Iloc2 = df['weight'] > filter_weight
         Iloc = Iloc & Iloc2
     df = df.loc[Iloc, :]
     df.reset_index(drop=True, inplace=True)
 
     # Scale the weights for visualization purposes
-    if len(np.unique(df['weight'].values.reshape(-1, 1))) > 2:
+    if minmax_distance is not None:
+        df['edge_distance'] = _normalize_size(df['weight'].values.reshape(-1, 1), minmax_distance[0], minmax_distance[1], scaler='minmax')
+    elif edge_distance is not None:
+        df['edge_distance'] = edge_distance
+        logger.info('Setting constant edge distance of %g' %(edge_distance))
+    else:
+        df['edge_distance'] = df['weight']
+
+    if (len(np.unique(df['weight'].values.reshape(-1, 1))) > 2 or (minmax is not None)) and (scaler is not None):
         df['weight_scaled'] = _normalize_size(df['weight'].values.reshape(-1, 1), minmax[0], minmax[1], scaler=scaler)
+    elif edge_weight is not None:
+        df['weight_scaled'] = edge_weight
+        logger.info('Setting constant edge thickness of %g' %(edge_weight))
     else:
-        df['weight_scaled'] = np.ones(df.shape[0]) * 1
+        df['edge_distance'] = df['weight']
 
     # Set marker start-end
     if marker_start is None: marker_start=''
     if marker_end is None: marker_end=''
-    if label is None: label=''
+    if label is None:
+        label=''
+    elif label == 'weight':
+        # Remove trailing zeros
+        label = list(map(lambda x: '(' + ('%f' % x).rstrip('0').rstrip('.') + ')', df['weight'].values))
 
     # Store in dataframe
     df['marker_start']=marker_start
     df['marker_end']=marker_end
     df['marker_color']=marker_color
     df['label']=label
     df['label_color']=label_color
     df['label_fontsize']=label_fontsize
 
     # Creation dictionary
     source_target = list(zip(df['source'], df['target']))
     # Return
     return {edge: {'weight': df['weight'].iloc[i],
                    'weight_scaled': df['weight_scaled'].iloc[i],
+                   'edge_distance': df['edge_distance'].iloc[i],
                    'color': '#808080', 'marker_start': df['marker_start'].iloc[i],
                    'marker_end': df['marker_end'].iloc[i],
                    'marker_color': df['marker_color'].iloc[i],
                    'label': df['label'].iloc[i],
                    'label_color': df['label_color'].iloc[i],
                    'label_fontsize': df['label_fontsize'].iloc[i],
                    } for
@@ -970,14 +1019,15 @@
     for edge in edges:
         G.add_edge(edge[0],
                    edge[1],
                    marker_color=edge_properties[edge]['marker_color'],
                    marker_start=edge_properties[edge]['marker_start'],
                    marker_end=edge_properties[edge]['marker_end'],
                    weight_scaled=np.abs(edge_properties[edge]['weight_scaled']),
+                   edge_distance=np.abs(edge_properties[edge]['edge_distance']),
                    weight=np.abs(edge_properties[edge]['weight']),
                    color=edge_properties[edge]['color'],
                    label=edge_properties[edge]['label'],
                    label_color=edge_properties[edge]['label_color'],
                    label_fontsize=edge_properties[edge]['label_fontsize'],
                    )
     return G
```

### Comparing `d3graph-2.4.4/d3graph/d3js/d3.v3.js` & `d3graph-2.4.5/d3graph/d3js/d3.v3.js`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/d3graph/d3js/d3graphscript.js` & `d3graph-2.4.5/d3graph/d3js/d3graphscript.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,16 @@
     var height = config.height;
 
     //Set up the colour scale
     var color = d3.scale.category20();
 
     var force = d3.layout.force()
         .charge(config.charge)
-        .linkDistance((d) => config.distance > 0 ? config.distance : d.edge_weight)
+        .linkDistance((d) => d.edge_distance || config.distance)
+        //.linkDistance((d) => config.distance > 0 ? config.distance : d.edge_weight)
         .size([width, height]);
 
     // DRAGGING START
     function dragstarted(d) {
         d3.event.sourceEvent.stopPropagation();
         d3.select(this).classed("dragging", true);
     }
@@ -124,14 +125,15 @@
     node.append("circle")
         .attr("r", function(d) {
             return d.node_size;
         }) // NODE SIZE
         .style("fill", function(d) {
             return d.node_color;
         }) // NODE-COLOR
+        .style("opacity", 0.95)
         .style("stroke-width", function(d) {
             return d.node_size_edge;
         }) // NODE-EDGE-SIZE
         .style("stroke", function(d) {
             return d.node_color_edge;
         }) // NODE-COLOR-EDGE
     //  .style("stroke", '#000')										// NODE-EDGE-COLOR (all black)
@@ -245,16 +247,16 @@
         //.attr("transform", "rotate(180)")                    // Marker-start mirrored
         .attr('d', function(d) {
             return d.path
         }) // Marker type
         //.style("fill", function(d) {return d.marker_color;}) // Marker color
         .style("fill", '#808080') // Marker color
         .style("stroke", '#808080') // Marker edge-color
-        .style("opacity", "1") // Marker opacity
-        .style("stroke-width", '1'); // Marker edge thickness
+        .style("opacity", 0.95) // Marker opacity
+        .style("stroke-width", 1); // Marker edge thickness
 
     // --------- END MARKER -----------
 
 
     // collision detection
 
     var padding = 1, // separation between circles
@@ -356,15 +358,15 @@
             link.style("opacity", function(o) {
                 return d.index == o.source.index | d.index == o.target.index ? 1 : 0.1;
             });
             //Reduce the op
             toggle = 1;
         } else {
             //Put them back to opacity=1
-            node.style("opacity", 1);
+            node.style("opacity", 0.95);
             link.style("opacity", 1);
 
             toggle = 0;
         }
     }
     //*************************************************************
```

### Comparing `d3graph-2.4.4/d3graph/d3js/index.html.j2` & `d3graph-2.4.5/d3graph/d3js/index.html.j2`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/d3graph/examples.py` & `d3graph-2.4.5/d3graph/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,51 @@
 # %% Libraries
 import networkx as nx
 import pandas as pd
 import numpy as np
 from d3graph import d3graph, adjmat2vec
 
+# %% Edge distance
+
+# Import
+from d3graph import d3graph
+# intialize to load example dataset
+d3 = d3graph()
+adjmat, _ = d3.import_example('bigbang')
+
+# Initialize with clustering colors
+d3.graph(adjmat, color='cluster')
+
+# Set all edge labels to "test"
+d3.set_edge_properties(directed=True, minmax_distance=None)
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_1.html')
+d3.set_edge_properties(directed=True)
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_3.html')
+d3.set_edge_properties(directed=True, minmax_distance=[20, 200])
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_3.html')
+d3.set_edge_properties
+
+d3.set_edge_properties(directed=True, label=None)
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_2.html')
+
+# Set edge labels 
+d3.edge_properties
+
+# We will first set all label properties to None and then we will adjust two of them
+d3.set_edge_properties(directed=True, marker_color='#000FFF', label=None)
+d3.edge_properties['Amy', 'Bernadette']['weight_scaled']=10
+d3.edge_properties['Amy', 'Bernadette']['label']='amy-bern'
+d3.edge_properties['Amy', 'Bernadette']['label_color']='#000FFF'
+d3.edge_properties['Amy', 'Bernadette']['label_fontsize']=8
+d3.edge_properties['Bernadette', 'Howard']['label']='bern-how'
+d3.edge_properties['Bernadette', 'Howard']['label_fontsize']=20
+d3.edge_properties['Bernadette', 'Howard']['label_color']='#000000'
+
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_2.html')
+
 # %% Edge link
 d3 = d3graph()
 adjmat, df = d3.import_example('karate')
 d3.graph(adjmat, color='cluster')
 d3.show(filepath=r'c:\temp\\d3graph\d3graph1.html')
 
 # %% Edge link
@@ -37,15 +75,15 @@
 d3.edge_properties['Bernadette', 'Howard']['label']='bern-how'
 d3.edge_properties['Bernadette', 'Howard']['label_fontsize']=20
 d3.edge_properties['Bernadette', 'Howard']['label_color']='#000000'
 
 d3.show(filepath=r'c:\temp\\d3graph\edge_labels_2.html')
 
 # %% Change color of text
-
+import numpy as np
 # Import library
 from d3graph import d3graph
 
 # Initialize with defaults
 d3 = d3graph()
 
 # Load example
```

### Comparing `d3graph-2.4.4/d3graph.egg-info/PKG-INFO` & `d3graph-2.4.5/d3graph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: d3graph
-Version: 2.4.4
+Version: 2.4.5
 Summary: Python package to create interactive network based on d3js.
 Home-page: https://erdogant.github.io/d3graph
-Download-URL: https://github.com/erdogant/d3graph/archive/2.4.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/erdogant/d3graph/archive/2.4.5.tar.gz
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -115,7 +117,9 @@
 ### Citation
 Please cite d3graph in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
+
+
```

### Comparing `d3graph-2.4.4/setup.py` & `d3graph-2.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/tests/conftest.py` & `d3graph-2.4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.4/tests/test_d3graph.py` & `d3graph-2.4.5/tests/test_d3graph.py`

 * *Files identical despite different names*

