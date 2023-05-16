# Comparing `tmp/crossroads-schematization-0.0.7.tar.gz` & `tmp/crossroads-schematization-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.0.7.tar", last modified: Thu Dec  8 11:48:13 2022, max compression
+gzip compressed data, was "crossroads-schematization-0.0.8.tar", last modified: Tue May 16 13:36:38 2023, max compression
```

## Comparing `crossroads-schematization-0.0.7.tar` & `crossroads-schematization-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-12-08 11:48:13.214794 crossroads-schematization-0.0.7/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.0.7/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2022-12-08 11:48:13.214794 crossroads-schematization-0.0.7/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.0.7/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-12-08 11:48:13.210794 crossroads-schematization-0.0.7/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2022-12-08 11:48:13.000000 crossroads-schematization-0.0.7/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      608 2022-12-08 11:48:13.000000 crossroads-schematization-0.0.7/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2022-12-08 11:48:13.000000 crossroads-schematization-0.0.7/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2022-12-08 11:48:13.000000 crossroads-schematization-0.0.7/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2022-12-08 11:48:13.000000 crossroads-schematization-0.0.7/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-12-08 11:48:13.210794 crossroads-schematization-0.0.7/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2022-12-08 11:47:55.000000 crossroads-schematization-0.0.7/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5853 2022-12-02 09:57:06.000000 crossroads-schematization-0.0.7/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    33385 2022-11-28 14:15:09.000000 crossroads-schematization-0.0.7/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    20421 2022-12-08 11:47:35.000000 crossroads-schematization-0.0.7/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2022-10-26 07:55:25.000000 crossroads-schematization-0.0.7/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2022-12-08 11:48:13.214794 crossroads-schematization-0.0.7/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.0.7/crschem/resources/crossing.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    21635 2022-11-28 14:43:32.000000 crossroads-schematization-0.0.7/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    23386 2022-11-30 16:22:46.000000 crossroads-schematization-0.0.7/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29547 2022-11-28 15:02:19.000000 crossroads-schematization-0.0.7/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.0.7/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     6342 2022-10-14 13:54:53.000000 crossroads-schematization-0.0.7/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       15 2022-11-30 15:55:39.000000 crossroads-schematization-0.0.7/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2022-12-08 11:48:13.214794 crossroads-schematization-0.0.7/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.0.7/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.0.8/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.0.8/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.427705 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-05-16 13:34:46.000000 crossroads-schematization-0.0.8/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5853 2022-12-02 09:57:06.000000 crossroads-schematization-0.0.8/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    37904 2023-05-16 13:20:22.000000 crossroads-schematization-0.0.8/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    21458 2023-05-16 13:06:22.000000 crossroads-schematization-0.0.8/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.0.8/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.0.8/crschem/resources/crossing.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29217 2023-01-16 14:33:05.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-01-16 15:35:19.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22752 2023-02-06 15:36:47.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35242 2023-01-16 09:30:00.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.0.8/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7350 2023-05-16 08:27:12.000000 crossroads-schematization-0.0.8/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.0.8/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.0.8/setup.py
```

### Comparing `crossroads-schematization-0.0.7/PKG-INFO` & `crossroads-schematization-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.0.7
+Version: 0.0.8
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.0.7/README.md` & `crossroads-schematization-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.7/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.0.8/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.0.7
+Version: 0.0.8
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.0.7/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.0.8/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,10 +11,14 @@
 crschem/cmd.py
 crschem/crossroad.py
 crschem/crossroad_schematization.py
 crschem/processing.py
 crschem/utils.py
 crschem/resources/crossing.svg
 crschem/resources/rendering-areas.qml
+crschem/resources/rendering-nodes-crossings.qml
+crschem/resources/rendering-nodes-islands.qml
+crschem/resources/rendering-nodes-space.qml
 crschem/resources/rendering-nodes.qml
+crschem/resources/rendering-polylines-space.qml
 crschem/resources/rendering-polylines.qml
 crschem/resources/tactile-a5.qpt
```

### Comparing `crossroads-schematization-0.0.7/crschem/cmd.py` & `crossroads-schematization-0.0.8/crschem/cmd.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.7/crschem/crossroad.py` & `crossroads-schematization-0.0.8/crschem/crossroad.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,27 +25,33 @@
         self.n2 = n2
         self.same_osm_orientation = same_osm_orientation
         self.edge_tags = edge_tags
         self.is_crossing_interior_node = is_crossing_interior_node
 
 
     def has_sidewalk(self):
-        return self.edge_tags["left_sidewalk"] != "" or self.edge_tags["right_sidewalk"] != ""
+        return SimpleWay.is_number(self.edge_tags["left_sidewalk"]) or SimpleWay.is_number(self.edge_tags["right_sidewalk"])
 
 
+    def is_number(value):
+        if isinstance(value, str):
+            return value != ""
+        else:
+            return not math.isnan(value)
+
     def get_sidewalk_id(self):
-        if self.edge_tags["left_sidewalk"] != "":
+        if SimpleWay.is_number(self.edge_tags["left_sidewalk"]):
             return self.edge_tags["left_sidewalk"]
-        elif self.edge_tags["right_sidewalk"] != "":
+        elif SimpleWay.is_number(self.edge_tags["right_sidewalk"]):
             return self.edge_tags["right_sidewalk"]
         else:
             return ""
 
     def has_sidewalks_both_sides(self):
-        return self.edge_tags["left_sidewalk"] != "" and self.edge_tags["right_sidewalk"] != ""
+        return SimpleWay.is_number(self.edge_tags["left_sidewalk"]) and SimpleWay.is_number(self.edge_tags["right_sidewalk"])
 
 
     def is_crossing_inner_node(self):
         return self.is_crossing_interior_node
 
 
     def get_initial_edge_id(self):
@@ -195,19 +201,21 @@
         l2 = sw.extends()
 
         # compute intersection between them
         return l1.intersection(l2)
 
 
     def getOSMIds(self):
-        return self.description["id"]
+        return ";".join(self.description["osm_node_ids"])
 
 
 class TurningSidewalk:
 
+    # TODO: add a supplementary point of pedestrian crossings in the turn (./example-pdf.sh 10)
+
     def __init__(self, str_sidewalks, osm_input, distance_kerb_footway):
         self.distance_kerb_footway = distance_kerb_footway
 
         self.str_sidewalks = str_sidewalks
         
         self.osm_input = osm_input
 
@@ -240,16 +248,16 @@
             
             elements = buffered_osm.boundary.intersection(edge)
             if not elements.is_empty:
                 nearest = shapely.ops.nearest_points(middle_bevel, elements)
                 self.build_beveled_turn(nearest[1])
 
 
-    def branch_names(self):
-        return [x.description["name"] for x in self.str_sidewalks]
+    def branch_ids(self):
+        return [x.description["id"] for x in self.str_sidewalks]
     
 
     def sidewalk_id(self):
         return self.str_sidewalks[0].sidewalk_id()
 
 
     def get_intersection(self):
@@ -388,15 +396,14 @@
         ys = [c["y"] for c in l]
         self.center = (sum(xs) / len(xs), sum(ys) / len(ys))
         ds = [osmnx.distance.euclidean_dist_vec(c["x"], c["y"], self.center[0], self.center[1]) for c in l]
         self.radius = sum(ds) / len(ds)
 
 
     def get_border_sections(self, crossings):
-
         c_in_poly = [i for i, x in enumerate(self.polygon) if x in crossings.keys()]
         if len(c_in_poly) == 0:
             print("Error: cannot have an island without crossing at this stage")
             return None
         polyshift = self.polygon[c_in_poly[0]:] + self.polygon[:c_in_poly[0]]
         # make it as a loop
         polyshift.append(polyshift[0])
@@ -460,15 +467,14 @@
         oedges = [orient_edge(e, self.center) for e in edges]
 
         # normalize vectors
         return [u.Utils.normalized_vector(e[0], e[1]) for e in oedges]
 
 
     def get_straight_island_direction(self, polylines):
-        
         # linearize the two polylines
         lz = p.Linearization(length=50, initial_step=0.5, exponential_coef=1.2)
         ll1 = lz.process(LineString(polylines[0]))
         ll2 = lz.process(LineString(polylines[1]))
 
         # use their directions to get a global direction for the island
         n1 = u.Utils.normalized_vector(ll1.coords[0], ll1.coords[1])
@@ -483,14 +489,16 @@
 
     def build_polylines_from_section(self, section):
 
         edges = [e for e in zip(section, section[1:]) if e[0] != e[1]]
         outside = list(locate(edges, lambda e: not u.Utils.edge_in_osm(e[0], e[1], self.osm_input)))
 
         if len(outside) != 0:
+            print(outside)
+            print(section)
             side1 = section[0:outside[0] + 1]
             side2 = section[outside[-1] + 1:]
             side2.reverse()
             return u.Utils.pathid_to_pathcoords(side1, self.osm_input), u.Utils.pathid_to_pathcoords(side2, self.osm_input)
         else:
             # use length to split
             path = LineString(u.Utils.pathid_to_pathcoords(section, self.osm_input))
@@ -576,34 +584,38 @@
         
 
     def compute_generalization(self, crossings, inner_region):
 
         # compute crossing's center
         self.compute_center_and_radius(crossings)
 
+        # TODO: if it's a a large region, build a polygon (./example-pdf.sh 13)
+
         if self.is_reachable:
             #compute supplementary edges if some of points of the polygons are far from the center
             self.compute_edges(crossings, inner_region)
         else:
             self.extremities = []
 
 
     def getGeometry(self):
+        # TODO: alternative geometry in case of a polygon (cf compute_generalization)
         if len(self.extremities) == 0:
             return [Point(self.center)]
         else:
             return [LineString([self.center, e]) for e in self.extremities]
 
 
     def toGDFTrafficIslands(traffic_islands, only_reachable = True):
         d = {'type': [], 'osm_id': [], 'geometry': []}
 
         for t in traffic_islands:
             if t.is_reachable or not only_reachable:
                 geom = t.getGeometry()
+                # TODO: add supplementary attribute to distinguish between a polygon and a more generalized island (cf compute_generalization)
                 for g in geom:
                     d["type"].append("traffic_island")
                     d["osm_id"].append(";".join(map(str, t.polygon)))
                     d["geometry"].append(g)
 
         return geopandas.GeoDataFrame(d, crs=2154)
 
@@ -611,17 +623,33 @@
 class Crossing:
 
     def __init__(self, node_id, osm_input):
 
         self.node_id = node_id
         self.osm_input = osm_input
 
+        self.island_width = 0.50 # cm
+
         self.compute_location()
         self.compute_orientation()
 
+        self.compute_crossing_profile()
+
+    def compute_crossing_profile(self):
+        self.has_island = "crossing:island" in self.osm_input.nodes[self.node_id] and self.osm_input.nodes[self.node_id]["crossing:island"] == "yes"
+        car_way = u.Utils.get_adjacent_road_edge(self.node_id, self.osm_input)
+        if car_way != None:
+            nb_backward, nb_forward, width = u.Utils.evaluate_way_composition(car_way)
+            self.nb_lanes_backward = nb_backward
+            self.nb_lanes_forward = nb_forward
+            self.lane_width = width
+        else:
+            self.nb_lanes_backward = 0
+            self.nb_lanes_forward = 0
+            self.lane_width = 0
 
     def compute_location(self):
         self.x = self.osm_input.nodes[self.node_id]["x"]
         self.y = self.osm_input.nodes[self.node_id]["y"]
 
 
     def compute_orientation(self):
@@ -704,33 +732,103 @@
         shifty = math.sin(self.bearing) * length
         return [(x - shiftx, y - shifty), (x, y), (x + shiftx, y + shifty)]
 
 
     def getGeometry(self):
         return Point(self.osm_input.nodes[self.node_id]["x"], self.osm_input.nodes[self.node_id]["y"])
 
-    def toGDFCrossings(crossings):
-        d = {'type': [], 'orientation': [], 'osm_id': [], 'geometry': [], 'orientation_confidence': []}
+    def getCrossingElements(self):
+        nb = self.nb_lanes_backward + self.nb_lanes_forward
+        start_shift = (nb - 1) * self.lane_width / 2
+        total_width = nb * self.lane_width
+        if self.has_island:
+            lane_width_effective = (total_width - self.island_width) / nb
+        else: 
+            lane_width_effective = self.lane_width
+
+        elements = []
+        x = self.osm_input.nodes[self.node_id]["x"]
+        y = self.osm_input.nodes[self.node_id]["y"]
+
+        # crossings
+        for i in range(nb):
+            shift = -start_shift + i * lane_width_effective + (self.island_width if self.has_island and i >= self.nb_lanes_forward else 0)
+            shiftx = math.cos(self.bearing) * shift
+            shifty = math.sin(self.bearing) * shift
+            elements.append({ "type": "crossing",
+                              "geometry": Point(x + shiftx, y + shifty),
+                              "lane_orientation": "forward" if i < self.nb_lanes_forward else "backward",
+                              "lane_width": lane_width_effective })
+
+        # separators
+        start_shift -= self.lane_width / 2
+        for i in range(nb - 1):
+            shift = -start_shift + i * lane_width_effective
+            if self.has_island:
+                if i + 1== self.nb_lanes_forward:
+                    shift += self.island_width / 2
+                elif i + 1 > self.nb_lanes_forward:
+                    shift += self.island_width
+            shiftx = math.cos(self.bearing) * shift
+            shifty = math.sin(self.bearing) * shift
+            island = self.has_island and i + 1 == self.nb_lanes_backward
+            elements.append({ "type": "traffic_island" if island else "lane_separator",
+                              "geometry": Point(x + shiftx, y + shifty),
+                              "lane_orientation": None,
+                              "lane_width": self.island_width if island else 0 })
+
+        return elements
+
+
+    def toGDFCrossings(crossings, details = True):
+        d = {'type': [], 
+             'osm_id': [],
+             'geometry': [],
+             'orientation': [],
+             'orientation_confidence': [],
+             'lane_width': [] }
+
+        if details:
+            d['lane_orientation'] = []
+        else:
+            d['has_island'] = []
+            d['nb_lanes_backward'] = []
+            d['nb_lanes_forward'] = []
 
         for cid in crossings:
             c = crossings[cid]
-            d["type"].append("crossing")
-            d["orientation"].append(c.bearing)
-            d["orientation_confidence"].append(c.bearing_confidence)
-            d["osm_id"].append(c.node_id)
-            d["geometry"].append(c.getGeometry())
+            if details:
+                for e in c.getCrossingElements():
+                    d["type"].append(e["type"])
+                    d["osm_id"].append(c.node_id)
+                    d["geometry"].append(e["geometry"])
+                    d["orientation"].append(c.bearing)
+                    d['lane_orientation'].append(e["lane_orientation"])
+                    d["orientation_confidence"].append(c.bearing_confidence)
+                    d["lane_width"].append(e["lane_width"])
+            else:
+                d["type"].append("crossing")
+                d["orientation"].append(c.bearing)
+                d["orientation_confidence"].append(c.bearing_confidence)
+                d["osm_id"].append(c.node_id)
+                d["geometry"].append(c.getGeometry())
+                d["has_island"].append(c.has_island)
+                d["nb_lanes_backward"].append(c.nb_lanes_backward)
+                d["nb_lanes_forward"].append(c.nb_lanes_forward)
+                d["lane_width"].append(c.lane_width)
 
         return geopandas.GeoDataFrame(d, crs=2154)
 
 
 class Branch:
 
-    def __init__(self, name, osm_input, cr_input, distance_kerb_footway):
+    def __init__(self, name, id, osm_input, cr_input, distance_kerb_footway):
         self.ways = []
         self.name = name
+        self.id = id
         self.osm_input = osm_input
         self.cr_input = cr_input
         self.distance_kerb_footway = distance_kerb_footway
 
     
     def add_way(self, way):
         self.ways.append(way)
@@ -742,15 +840,15 @@
 
     # return all the edges contained in the initial intersection
     # that are not part of this branch
     def get_other_edges(self):
         result = []
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"] and elem["name"] != self.name:
-                ids = list(map(int, elem["id"].split(";")))
+                ids = list(map(int, elem["osm_node_ids"]))
                 result.append(ids)
         return result
 
 
     def build_two_sidewalks(self):
         # the shift corresponds to half the width of the street
         shift = self.width / 2
@@ -762,20 +860,20 @@
                                    "left",
                                    self.sides[0].is_crossing_inner_node()),
                    StraightSidewalk(self.middle_line.parallel_offset(shift, "right"),
                                    self.sides[1].edge_tags,
                                    self.sides[1].same_osm_orientation,
                                    "right",
                                    self.sides[1].is_crossing_inner_node())]
-
         buf = u.Utils.get_edges_buffered_by_osm(self.get_other_edges(), self.osm_input, self.distance_kerb_footway).boundary
         for i, s in enumerate(result):
-            intersections = s.edge.intersection(buf)
-            if not intersections.is_empty and isinstance(intersections, Point):
-                result[i].update_first_node(intersections)
+            if s.edge.intersects(buf):
+                intersections = s.edge.intersection(buf)
+                if not intersections.is_empty and isinstance(intersections, Point):
+                    result[i].update_first_node(intersections)
 
         return result
 
 
 
     # maximum distance between two extremity points of the ways
     def get_initial_branche_width(self):
```

### Comparing `crossroads-schematization-0.0.7/crschem/crossroad_schematization.py` & `crossroads-schematization-0.0.8/crschem/crossroad_schematization.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         # label edges of the graph from cr_input
         print("Label OSM network")
         networkx.set_edge_attributes(self.osm_input, values="unknown", name="type")
         networkx.set_edge_attributes(self.osm_input, values="created", name="type_origin")
         networkx.set_node_attributes(self.osm_input, values="unknown", name="type")
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"]:
-                ids = list(map(int, elem["id"].split(";")))
+                ids = list(map(int, elem["osm_node_ids"]))
                 self.osm_input[ids[0]][ids[1]][0]["type"] = elem["type"]
                 self.osm_input[ids[0]][ids[1]][0]["type_origin"] = "input"
                 self.osm_input.nodes[ids[0]]["type"] = "input"
                 self.osm_input.nodes[ids[1]]["type"] = "input"
 
 
     def is_boundary_node(self, node):
@@ -211,25 +211,26 @@
     def build_branches(self):
         print("Grouping ways by branch")
         self.branches = {}
 
         bid = 0
         for index, elem in self.cr_input.iterrows():
             if elem["type"] == "branch":
-                ids = list(map(int, elem["id"].split(";")))
+                ids = list(map(int, elem["osm_node_ids"]))
                 osm_n1 = ids[0] # first id in the OSM direction
                 osm_n2 = ids[1] # last id in the OSM direction
                 n1 = osm_n1 if self.is_boundary_node(osm_n1) else osm_n2
                 n2 = osm_n2 if n1 == osm_n1 else osm_n1
                 e = u.Utils.get_initial_edge_tags(self.cr_input, osm_n1, osm_n2)
                 if e is not None:
-                    bname = e["name"].split("|")[0]
-                    if not bname in self.branches:
-                        self.branches[bname] = c.Branch(bname, self.osm_input, self.cr_input, self.distance_kerb_footway)
-                    self.branches[bname].add_way(c.SimpleWay(n1, n2, e, osm_n1 == n1,
+                    id = e["id"]
+                    bname = e["name"]
+                    if not id in self.branches:
+                        self.branches[id] = c.Branch(bname, id, self.osm_input, self.cr_input, self.distance_kerb_footway)
+                    self.branches[id].add_way(c.SimpleWay(n1, n2, e, osm_n1 == n1,
                                                         c.Crossing.is_crossing(n1, self.cr_input)))
 
 
     def build_sidewalks(self):
         print("Building sidewalks")
         self.sidewalks = {}
         
@@ -244,21 +245,19 @@
                 for sw in self.sidewalks[bid]:
                     result.add(sw.sidewalk_id())
         return list(result)
 
 
     def get_sidewalks_by_id(self, sid):
         result = []
-
         for bid in self.sidewalks:
             if self.sidewalks[bid]:
                 for sw in self.sidewalks[bid]:
                     if sw.sidewalk_id() == sid:
                         result.append(sw)
-        
         return result
 
     def assemble_sidewalks(self):
         print("Assembling sidewalks")
         self.cr_input.replace('', np.nan, inplace=True)
         original_sidewalks_ids = self.get_sidewalk_ids()
         self.merged_sidewalks = []
@@ -270,22 +269,22 @@
     def build_inner_region(self):
         print("Building inner region")
         open_sides = copy.copy(self.merged_sidewalks)
 
         # order sidewalks
         final_shape = [(open_sides.pop(), True)]
         while len(open_sides) != 0:
-            cid = final_shape[-1][0].branch_names()[1 if final_shape[-1][1] else 0]
+            cid = final_shape[-1][0].branch_ids()[1 if final_shape[-1][1] else 0]
             found = False
             for i, o in enumerate(open_sides):
-                if o.branch_names()[0] == cid:
+                if o.branch_ids()[0] == cid:
                     final_shape.append((open_sides.pop(i), True))
                     found = True
                     break
-                elif o.branch_names()[1] == cid:
+                elif o.branch_ids()[1] == cid:
                     final_shape.append((open_sides.pop(i), False))
                     found = True
                     break
             if not found:
                 print("Error: cannot found next sidewalk")
                 return
         
@@ -305,24 +304,24 @@
         for index, elem in self.cr_input.iterrows():
             if elem["type"] in ["branch", "way"]:
                 for side in ["left", "right"]:
                     id = u.Utils.get_number_from_label(elem[side + "_island"])
                     if not id is None:
                         if not id in traffic_islands_edges:
                             traffic_islands_edges[id] = []
-                        traffic_islands_edges[id].append(elem["id"])
+                        traffic_islands_edges[id].append(";".join(elem["osm_node_ids"]))
         
         # then build traffic islands
         self.traffic_islands = []
         for eid in traffic_islands_edges:
             self.traffic_islands.append(c.TrafficIsland(traffic_islands_edges[eid], self.osm_input, self.cr_input))
 
 
-    def to_printable_internal(self, filename, log_files, dpi = -1, crs = 3857):
-        from qgis.core import QgsApplication, QgsProject, QgsPrintLayout, QgsLayout, QgsVectorLayer, QgsLayoutExporter, QgsLayoutItemPage, QgsReadWriteContext, QgsRectangle, QgsCoordinateReferenceSystem, QgsCoordinateTransform
+    def to_printable_internal(self, filename, log_files, dpi = -1, crs = 2154):
+        from qgis.core import QgsApplication, QgsProject, QgsPrintLayout, QgsLayout, QgsVectorLayer, QgsLayoutExporter, QgsLayoutItemPage, QgsReadWriteContext, QgsRectangle, QgsCoordinateReferenceSystem, QgsCoordinateTransform, QgsFeatureRequest, QgsExpression
         from qgis.PyQt.QtXml import QDomDocument
         import tempfile
         import os
 
         tmp = tempfile.NamedTemporaryFile(mode='w', delete=False) 
         self.toGeojson(tmp.name, True)
         qgs = QgsApplication([], False)
@@ -331,27 +330,33 @@
         # get project
         project = QgsProject.instance()
         composition = QgsPrintLayout(project)
         project.setCrs(QgsCoordinateReferenceSystem(crs))
         
         # load layers
         geojson = tmp.name
-        points_layer = QgsVectorLayer(geojson + '|geometrytype=Point', "points", "ogr")
+        points_crossings_layer = QgsVectorLayer(geojson + '|geometrytype=Point', "points", "ogr")
+        points_islands_layer = QgsVectorLayer(geojson + '|geometrytype=Point', "points", "ogr")
+        points_space_layer = QgsVectorLayer(geojson + '|geometrytype=Point', "points", "ogr")
         lines_layer = QgsVectorLayer(geojson + '|geometrytype=LineString', "lines", "ogr")
+        lines_space_layer = QgsVectorLayer(geojson + '|geometrytype=LineString', "lines", "ogr")
         polygons_layer = QgsVectorLayer(geojson + '|geometrytype=Polygon', "polygons", "ogr") # 4326
         # project them on map
         project.addMapLayer(polygons_layer)
+        project.addMapLayer(lines_space_layer)
+        project.addMapLayer(points_space_layer)
+        project.addMapLayer(points_crossings_layer)
+        project.addMapLayer(points_islands_layer)
         project.addMapLayer(lines_layer)
-        project.addMapLayer(points_layer)
 
         # compute region of interest
         polygons_layer.selectAll() # the polygon corresponding to the car ways
         pg_box = polygons_layer.boundingBoxOfSelected()
-        points_layer.selectByRect(pg_box) # only keep points inside (crossings, islands)
-        pt_box = points_layer.boundingBoxOfSelected()
+        points_space_layer.selectByRect(pg_box) # only keep points inside (crossings, islands)
+        pt_box = points_space_layer.boundingBoxOfSelected()
         # then combine both rectangles to zoom on the points within the main region
         pp = 2
         pb = 1
         sourceCrs = QgsCoordinateReferenceSystem(polygons_layer.crs())
         destCrs = QgsCoordinateReferenceSystem(project.crs())
         tr = QgsCoordinateTransform(sourceCrs, destCrs, project)
 
@@ -380,20 +385,26 @@
                     i.setScale(400)
         # to solve the SVG relative path in qml files, use a trick [BEGIN]
         filename = os.path.abspath(filename)
         cwd = os.getcwd()
         os.chdir(os.path.dirname(__file__))
 
         # load layer styles and assign them to the layers
-        points_style = os.path.dirname(__file__) + "/resources/rendering-nodes.qml" # TODO: integrate them for pipe
+        points_islands_style = os.path.dirname(__file__) + "/resources/rendering-nodes-islands.qml" # TODO: integrate them for pipe
+        points_crossings_style = os.path.dirname(__file__) + "/resources/rendering-nodes-crossings.qml"
+        points_space_style = os.path.dirname(__file__) + "/resources/rendering-nodes-space.qml"
         lines_style = os.path.dirname(__file__) + "/resources/rendering-polylines.qml"
         polygons_style = os.path.dirname(__file__) + "/resources/rendering-areas.qml" # sld
+        lines_space_style = os.path.dirname(__file__) + "/resources/rendering-polylines-space.qml"
         
-        points_layer.loadNamedStyle(points_style)
         lines_layer.loadNamedStyle(lines_style)
+        points_space_layer.loadNamedStyle(points_space_style)
+        points_crossings_layer.loadNamedStyle(points_crossings_style)
+        points_islands_layer.loadNamedStyle(points_islands_style)
+        lines_space_layer.loadNamedStyle(lines_space_style)
         polygons_layer.loadNamedStyle(polygons_style)
         
         exporter = QgsLayoutExporter(layout)
         settings = exporter.PdfExportSettings()
         settings.rasterizeWholeImage = False
         if filename.endswith(".pdf"):
             exporter.exportToPdf(filename, settings)
```

### Comparing `crossroads-schematization-0.0.7/crschem/processing.py` & `crossroads-schematization-0.0.8/crschem/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     # return true if the point p2 (middle point of pts=[p1, p2, p3])
     # is a splitting node, or an node with a strong angle
     def is_split_in_straight_part(G, pts):
         p1, p2, p3 = pts
         if len(G[p2]) > 2:
             return True
-        angle = u.Utils.turn_angle(G, p1, p2, p3)
+        angle = u.Utils.turn_angle(G, p2, p1, p3)
         if angle > 180:
             angle = 360 - angle 
         if abs(angle) > 30:
             return True
         
         return False
 
@@ -107,16 +107,16 @@
             return polyline
 
 
     def convert_to_linestring(G, polyline):
         return LineString([Point(G.nodes[x]["x"], G.nodes[x]["y"]) for x in polyline])
 
 
-    def is_turn(G, c1, m, c2):
-        ta = u.Utils.turn_angle(G, c1, m, c2)
+    def is_turn(G, m, c1, c2):
+        ta = u.Utils.turn_angle(G, m, c1, c2)
         return ta < 90 or ta > 90 * 3
 
 
     def is_similar_edge(G, e1, e2):
         tags_e1 = G[e1[0]][e1[1]][0]
         tags_e2 = G[e2[0]][e2[1]][0]
 
@@ -142,15 +142,15 @@
         other = [n for n in G[n2] if n != n1 and G[n2][n][0]["type"] == "unknown" and
                  Expander.is_similar_edge(G, [n1, n2], [n2, n])]
         if len(other) == 0:
             return None
         elif len(other) == 1:
             return other[0]
         else:
-            sorted_other = sorted(other, key=lambda n: u.Utils.turn_angle(G, n1, n2, n), reverse=not left_first)
+            sorted_other = sorted(other, key=lambda n: u.Utils.turn_angle(G, n2, n1, n), reverse=not left_first)
             return sorted_other[0]
 
 
     def extend_branch(G, n1, n2, left_first):
         # find next edge in the same street
         next = Expander.find_next_edge(G, n1, n2, left_first)
         # if not found, we reach the end of the path
```

### Comparing `crossroads-schematization-0.0.7/crschem/resources/crossing.svg` & `crossroads-schematization-0.0.8/crschem/resources/crossing.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.7/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-space.qml`

 * *Files 7% similar despite different names*

```diff
@@ -1,1353 +1,1422 @@
 00000000: 3c21 444f 4354 5950 4520 7167 6973 2050  <!DOCTYPE qgis P
 00000010: 5542 4c49 4320 2768 7474 703a 2f2f 6d72  UBLIC 'http://mr
 00000020: 6363 2e63 6f6d 2f71 6769 732e 6474 6427  cc.com/qgis.dtd'
 00000030: 2027 5359 5354 454d 273e 0a3c 7167 6973   'SYSTEM'>.<qgis
-00000040: 206d 6178 5363 616c 653d 2230 2220 7665   maxScale="0" ve
-00000050: 7273 696f 6e3d 2233 2e32 382e 312d 4669  rsion="3.28.1-Fi
-00000060: 7265 6e7a 6522 2073 696d 706c 6966 7944  renze" simplifyD
-00000070: 7261 7769 6e67 4869 6e74 733d 2231 2220  rawingHints="1" 
-00000080: 7369 6d70 6c69 6679 416c 676f 7269 7468  simplifyAlgorith
-00000090: 6d3d 2230 2220 7369 6d70 6c69 6679 4d61  m="0" simplifyMa
-000000a0: 7853 6361 6c65 3d22 3122 2073 696d 706c  xScale="1" simpl
-000000b0: 6966 794c 6f63 616c 3d22 3122 2068 6173  ifyLocal="1" has
-000000c0: 5363 616c 6542 6173 6564 5669 7369 6269  ScaleBasedVisibi
-000000d0: 6c69 7479 466c 6167 3d22 3022 2072 6561  lityFlag="0" rea
-000000e0: 644f 6e6c 793d 2230 2220 7374 796c 6543  dOnly="0" styleC
-000000f0: 6174 6567 6f72 6965 733d 2241 6c6c 5374  ategories="AllSt
-00000100: 796c 6543 6174 6567 6f72 6965 7322 206c  yleCategories" l
-00000110: 6162 656c 7345 6e61 626c 6564 3d22 3022  abelsEnabled="0"
-00000120: 2073 696d 706c 6966 7944 7261 7769 6e67   simplifyDrawing
-00000130: 546f 6c3d 2231 2220 7379 6d62 6f6c 6f67  Tol="1" symbolog
-00000140: 7952 6566 6572 656e 6365 5363 616c 653d  yReferenceScale=
-00000150: 222d 3122 206d 696e 5363 616c 653d 2231  "-1" minScale="1
-00000160: 3030 3030 3030 3030 223e 0a20 203c 666c  00000000">.  <fl
+00000040: 206c 6162 656c 7345 6e61 626c 6564 3d22   labelsEnabled="
+00000050: 3022 2073 796d 626f 6c6f 6779 5265 6665  0" symbologyRefe
+00000060: 7265 6e63 6553 6361 6c65 3d22 2d31 2220  renceScale="-1" 
+00000070: 6d69 6e53 6361 6c65 3d22 3130 3030 3030  minScale="100000
+00000080: 3030 3022 2073 696d 706c 6966 7944 7261  000" simplifyDra
+00000090: 7769 6e67 546f 6c3d 2231 2220 7369 6d70  wingTol="1" simp
+000000a0: 6c69 6679 416c 676f 7269 7468 6d3d 2230  lifyAlgorithm="0
+000000b0: 2220 7369 6d70 6c69 6679 4472 6177 696e  " simplifyDrawin
+000000c0: 6748 696e 7473 3d22 3022 2073 7479 6c65  gHints="0" style
+000000d0: 4361 7465 676f 7269 6573 3d22 416c 6c53  Categories="AllS
+000000e0: 7479 6c65 4361 7465 676f 7269 6573 2220  tyleCategories" 
+000000f0: 6d61 7853 6361 6c65 3d22 3022 2073 696d  maxScale="0" sim
+00000100: 706c 6966 794c 6f63 616c 3d22 3122 2076  plifyLocal="1" v
+00000110: 6572 7369 6f6e 3d22 332e 3238 2e33 2d46  ersion="3.28.3-F
+00000120: 6972 656e 7a65 2220 7265 6164 4f6e 6c79  irenze" readOnly
+00000130: 3d22 3022 2073 696d 706c 6966 794d 6178  ="0" simplifyMax
+00000140: 5363 616c 653d 2231 2220 6861 7353 6361  Scale="1" hasSca
+00000150: 6c65 4261 7365 6456 6973 6962 696c 6974  leBasedVisibilit
+00000160: 7946 6c61 673d 2230 223e 0a20 203c 666c  yFlag="0">.  <fl
 00000170: 6167 733e 0a20 2020 203c 4964 656e 7469  ags>.    <Identi
 00000180: 6669 6162 6c65 3e31 3c2f 4964 656e 7469  fiable>1</Identi
 00000190: 6669 6162 6c65 3e0a 2020 2020 3c52 656d  fiable>.    <Rem
 000001a0: 6f76 6162 6c65 3e31 3c2f 5265 6d6f 7661  ovable>1</Remova
 000001b0: 626c 653e 0a20 2020 203c 5365 6172 6368  ble>.    <Search
 000001c0: 6162 6c65 3e31 3c2f 5365 6172 6368 6162  able>1</Searchab
 000001d0: 6c65 3e0a 2020 2020 3c50 7269 7661 7465  le>.    <Private
 000001e0: 3e30 3c2f 5072 6976 6174 653e 0a20 203c  >0</Private>.  <
 000001f0: 2f66 6c61 6773 3e0a 2020 3c74 656d 706f  /flags>.  <tempo
-00000200: 7261 6c20 656e 6162 6c65 643d 2230 2220  ral enabled="0" 
-00000210: 6c69 6d69 744d 6f64 653d 2230 2220 656e  limitMode="0" en
-00000220: 6446 6965 6c64 3d22 2220 656e 6445 7870  dField="" endExp
-00000230: 7265 7373 696f 6e3d 2222 2064 7572 6174  ression="" durat
-00000240: 696f 6e55 6e69 743d 226d 696e 2220 7374  ionUnit="min" st
-00000250: 6172 7446 6965 6c64 3d22 2220 7374 6172  artField="" star
-00000260: 7445 7870 7265 7373 696f 6e3d 2222 206d  tExpression="" m
-00000270: 6f64 653d 2230 2220 6475 7261 7469 6f6e  ode="0" duration
-00000280: 4669 656c 643d 2222 2066 6978 6564 4475  Field="" fixedDu
-00000290: 7261 7469 6f6e 3d22 3022 2061 6363 756d  ration="0" accum
-000002a0: 756c 6174 653d 2230 223e 0a20 2020 203c  ulate="0">.    <
+00000200: 7261 6c20 6c69 6d69 744d 6f64 653d 2230  ral limitMode="0
+00000210: 2220 7374 6172 7446 6965 6c64 3d22 2220  " startField="" 
+00000220: 6669 7865 6444 7572 6174 696f 6e3d 2230  fixedDuration="0
+00000230: 2220 6163 6375 6d75 6c61 7465 3d22 3022  " accumulate="0"
+00000240: 2065 6e64 4669 656c 643d 2222 2073 7461   endField="" sta
+00000250: 7274 4578 7072 6573 7369 6f6e 3d22 2220  rtExpression="" 
+00000260: 6475 7261 7469 6f6e 556e 6974 3d22 6d69  durationUnit="mi
+00000270: 6e22 206d 6f64 653d 2230 2220 656e 6445  n" mode="0" endE
+00000280: 7870 7265 7373 696f 6e3d 2222 2065 6e61  xpression="" ena
+00000290: 626c 6564 3d22 3022 2064 7572 6174 696f  bled="0" duratio
+000002a0: 6e46 6965 6c64 3d22 223e 0a20 2020 203c  nField="">.    <
 000002b0: 6669 7865 6452 616e 6765 3e0a 2020 2020  fixedRange>.    
 000002c0: 2020 3c73 7461 7274 3e3c 2f73 7461 7274    <start></start
 000002d0: 3e0a 2020 2020 2020 3c65 6e64 3e3c 2f65  >.      <end></e
 000002e0: 6e64 3e0a 2020 2020 3c2f 6669 7865 6452  nd>.    </fixedR
 000002f0: 616e 6765 3e0a 2020 3c2f 7465 6d70 6f72  ange>.  </tempor
 00000300: 616c 3e0a 2020 3c65 6c65 7661 7469 6f6e  al>.  <elevation
-00000310: 207a 6f66 6673 6574 3d22 3022 2065 7874   zoffset="0" ext
-00000320: 7275 7369 6f6e 456e 6162 6c65 643d 2230  rusionEnabled="0
-00000330: 2220 7368 6f77 4d61 726b 6572 5379 6d62  " showMarkerSymb
-00000340: 6f6c 496e 5375 7266 6163 6550 6c6f 7473  olInSurfacePlots
-00000350: 3d22 3022 2065 7874 7275 7369 6f6e 3d22  ="0" extrusion="
-00000360: 3022 2062 696e 6469 6e67 3d22 4365 6e74  0" binding="Cent
-00000370: 726f 6964 2220 7265 7370 6563 744c 6179  roid" respectLay
-00000380: 6572 5379 6d62 6f6c 3d22 3122 2063 6c61  erSymbol="1" cla
-00000390: 6d70 696e 673d 2254 6572 7261 696e 2220  mping="Terrain" 
-000003a0: 7479 7065 3d22 496e 6469 7669 6475 616c  type="Individual
-000003b0: 4665 6174 7572 6573 2220 7a73 6361 6c65  Features" zscale
-000003c0: 3d22 3122 2073 796d 626f 6c6f 6779 3d22  ="1" symbology="
-000003d0: 4c69 6e65 223e 0a20 2020 203c 6461 7461  Line">.    <data
+00000310: 2073 796d 626f 6c6f 6779 3d22 4c69 6e65   symbology="Line
+00000320: 2220 7265 7370 6563 744c 6179 6572 5379  " respectLayerSy
+00000330: 6d62 6f6c 3d22 3122 207a 7363 616c 653d  mbol="1" zscale=
+00000340: 2231 2220 636c 616d 7069 6e67 3d22 5465  "1" clamping="Te
+00000350: 7272 6169 6e22 2073 686f 774d 6172 6b65  rrain" showMarke
+00000360: 7253 796d 626f 6c49 6e53 7572 6661 6365  rSymbolInSurface
+00000370: 506c 6f74 733d 2230 2220 7a6f 6666 7365  Plots="0" zoffse
+00000380: 743d 2230 2220 6578 7472 7573 696f 6e3d  t="0" extrusion=
+00000390: 2230 2220 6269 6e64 696e 673d 2243 656e  "0" binding="Cen
+000003a0: 7472 6f69 6422 2065 7874 7275 7369 6f6e  troid" extrusion
+000003b0: 456e 6162 6c65 643d 2230 2220 7479 7065  Enabled="0" type
+000003c0: 3d22 496e 6469 7669 6475 616c 4665 6174  ="IndividualFeat
+000003d0: 7572 6573 223e 0a20 2020 203c 6461 7461  ures">.    <data
 000003e0: 2d64 6566 696e 6564 2d70 726f 7065 7274  -defined-propert
 000003f0: 6965 733e 0a20 2020 2020 203c 4f70 7469  ies>.      <Opti
 00000400: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
 00000410: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00000420: 616c 7565 3d22 2220 7479 7065 3d22 5153  alue="" type="QS
-00000430: 7472 696e 6722 206e 616d 653d 226e 616d  tring" name="nam
-00000440: 6522 2f3e 0a20 2020 2020 2020 203c 4f70  e"/>.        <Op
+00000420: 616c 7565 3d22 2220 6e61 6d65 3d22 6e61  alue="" name="na
+00000430: 6d65 2220 7479 7065 3d22 5153 7472 696e  me" type="QStrin
+00000440: 6722 2f3e 0a20 2020 2020 2020 203c 4f70  g"/>.        <Op
 00000450: 7469 6f6e 206e 616d 653d 2270 726f 7065  tion name="prope
 00000460: 7274 6965 7322 2f3e 0a20 2020 2020 2020  rties"/>.       
 00000470: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00000480: 636f 6c6c 6563 7469 6f6e 2220 7479 7065  collection" type
-00000490: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-000004a0: 2274 7970 6522 2f3e 0a20 2020 2020 203c  "type"/>.      <
+00000480: 636f 6c6c 6563 7469 6f6e 2220 6e61 6d65  collection" name
+00000490: 3d22 7479 7065 2220 7479 7065 3d22 5153  ="type" type="QS
+000004a0: 7472 696e 6722 2f3e 0a20 2020 2020 203c  tring"/>.      <
 000004b0: 2f4f 7074 696f 6e3e 0a20 2020 203c 2f64  /Option>.    </d
 000004c0: 6174 612d 6465 6669 6e65 642d 7072 6f70  ata-defined-prop
 000004d0: 6572 7469 6573 3e0a 2020 2020 3c70 726f  erties>.    <pro
 000004e0: 6669 6c65 4c69 6e65 5379 6d62 6f6c 3e0a  fileLineSymbol>.
-000004f0: 2020 2020 2020 3c73 796d 626f 6c20 636c        <symbol cl
-00000500: 6970 5f74 6f5f 6578 7465 6e74 3d22 3122  ip_to_extent="1"
-00000510: 2069 735f 616e 696d 6174 6564 3d22 3022   is_animated="0"
-00000520: 2074 7970 653d 226c 696e 6522 2066 6f72   type="line" for
-00000530: 6365 5f72 6872 3d22 3022 206e 616d 653d  ce_rhr="0" name=
-00000540: 2222 2061 6c70 6861 3d22 3122 2066 7261  "" alpha="1" fra
-00000550: 6d65 5f72 6174 653d 2231 3022 3e0a 2020  me_rate="10">.  
+000004f0: 2020 2020 2020 3c73 796d 626f 6c20 6672        <symbol fr
+00000500: 616d 655f 7261 7465 3d22 3130 2220 6e61  ame_rate="10" na
+00000510: 6d65 3d22 2220 616c 7068 613d 2231 2220  me="" alpha="1" 
+00000520: 6973 5f61 6e69 6d61 7465 643d 2230 2220  is_animated="0" 
+00000530: 636c 6970 5f74 6f5f 6578 7465 6e74 3d22  clip_to_extent="
+00000540: 3122 2074 7970 653d 226c 696e 6522 2066  1" type="line" f
+00000550: 6f72 6365 5f72 6872 3d22 3022 3e0a 2020  orce_rhr="0">.  
 00000560: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
 00000570: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
 00000580: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
 00000590: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
 000005a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000005b0: 6e20 7661 6c75 653d 2222 2074 7970 653d  n value="" type=
-000005c0: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-000005d0: 6e61 6d65 222f 3e0a 2020 2020 2020 2020  name"/>.        
+000005b0: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
+000005c0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
+000005d0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
 000005e0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
 000005f0: 3d22 7072 6f70 6572 7469 6573 222f 3e0a  ="properties"/>.
 00000600: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
 00000610: 696f 6e20 7661 6c75 653d 2263 6f6c 6c65  ion value="colle
-00000620: 6374 696f 6e22 2074 7970 653d 2251 5374  ction" type="QSt
-00000630: 7269 6e67 2220 6e61 6d65 3d22 7479 7065  ring" name="type
+00000620: 6374 696f 6e22 206e 616d 653d 2274 7970  ction" name="typ
+00000630: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
 00000640: 222f 3e0a 2020 2020 2020 2020 2020 3c2f  "/>.          </
 00000650: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
 00000660: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
 00000670: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00000680: 2020 203c 6c61 7965 7220 656e 6162 6c65     <layer enable
-00000690: 643d 2231 2220 636c 6173 733d 2253 696d  d="1" class="Sim
-000006a0: 706c 654c 696e 6522 2070 6173 733d 2230  pleLine" pass="0
+00000680: 2020 203c 6c61 7965 7220 636c 6173 733d     <layer class=
+00000690: 2253 696d 706c 654c 696e 6522 2070 6173  "SimpleLine" pas
+000006a0: 733d 2230 2220 656e 6162 6c65 643d 2231  s="0" enabled="1
 000006b0: 2220 6c6f 636b 6564 3d22 3022 3e0a 2020  " locked="0">.  
 000006c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
 000006d0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
 000006e0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000006f0: 7661 6c75 653d 2230 2220 7479 7065 3d22  value="0" type="
-00000700: 5153 7472 696e 6722 206e 616d 653d 2261  QString" name="a
-00000710: 6c69 676e 5f64 6173 685f 7061 7474 6572  lign_dash_patter
-00000720: 6e22 2f3e 0a20 2020 2020 2020 2020 2020  n"/>.           
+000006f0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
+00000700: 616c 6967 6e5f 6461 7368 5f70 6174 7465  align_dash_patte
+00000710: 726e 2220 7479 7065 3d22 5153 7472 696e  rn" type="QStrin
+00000720: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
 00000730: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00000740: 7371 7561 7265 2220 7479 7065 3d22 5153  square" type="QS
-00000750: 7472 696e 6722 206e 616d 653d 2263 6170  tring" name="cap
-00000760: 7374 796c 6522 2f3e 0a20 2020 2020 2020  style"/>.       
+00000740: 7371 7561 7265 2220 6e61 6d65 3d22 6361  square" name="ca
+00000750: 7073 7479 6c65 2220 7479 7065 3d22 5153  pstyle" type="QS
+00000760: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
 00000770: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00000780: 7565 3d22 353b 3222 2074 7970 653d 2251  ue="5;2" type="Q
-00000790: 5374 7269 6e67 2220 6e61 6d65 3d22 6375  String" name="cu
-000007a0: 7374 6f6d 6461 7368 222f 3e0a 2020 2020  stomdash"/>.    
+00000780: 7565 3d22 353b 3222 206e 616d 653d 2263  ue="5;2" name="c
+00000790: 7573 746f 6d64 6173 6822 2074 7970 653d  ustomdash" type=
+000007a0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
 000007b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
 000007c0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
-000007d0: 302c 302c 3022 2074 7970 653d 2251 5374  0,0,0" type="QSt
-000007e0: 7269 6e67 2220 6e61 6d65 3d22 6375 7374  ring" name="cust
-000007f0: 6f6d 6461 7368 5f6d 6170 5f75 6e69 745f  omdash_map_unit_
-00000800: 7363 616c 6522 2f3e 0a20 2020 2020 2020  scale"/>.       
+000007d0: 302c 302c 3022 206e 616d 653d 2263 7573  0,0,0" name="cus
+000007e0: 746f 6d64 6173 685f 6d61 705f 756e 6974  tomdash_map_unit
+000007f0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
+00000800: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
 00000810: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00000820: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
-00000830: 7472 696e 6722 206e 616d 653d 2263 7573  tring" name="cus
-00000840: 746f 6d64 6173 685f 756e 6974 222f 3e0a  tomdash_unit"/>.
+00000820: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6375  ue="MM" name="cu
+00000830: 7374 6f6d 6461 7368 5f75 6e69 7422 2074  stomdash_unit" t
+00000840: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
 00000850: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00000860: 696f 6e20 7661 6c75 653d 2230 2220 7479  ion value="0" ty
-00000870: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00000880: 653d 2264 6173 685f 7061 7474 6572 6e5f  e="dash_pattern_
-00000890: 6f66 6673 6574 222f 3e0a 2020 2020 2020  offset"/>.      
+00000860: 696f 6e20 7661 6c75 653d 2230 2220 6e61  ion value="0" na
+00000870: 6d65 3d22 6461 7368 5f70 6174 7465 726e  me="dash_pattern
+00000880: 5f6f 6666 7365 7422 2074 7970 653d 2251  _offset" type="Q
+00000890: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
 000008a0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
 000008b0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-000008c0: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-000008d0: 6e67 2220 6e61 6d65 3d22 6461 7368 5f70  ng" name="dash_p
-000008e0: 6174 7465 726e 5f6f 6666 7365 745f 6d61  attern_offset_ma
-000008f0: 705f 756e 6974 5f73 6361 6c65 222f 3e0a  p_unit_scale"/>.
+000008c0: 302c 3022 206e 616d 653d 2264 6173 685f  0,0" name="dash_
+000008d0: 7061 7474 6572 6e5f 6f66 6673 6574 5f6d  pattern_offset_m
+000008e0: 6170 5f75 6e69 745f 7363 616c 6522 2074  ap_unit_scale" t
+000008f0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
 00000900: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00000910: 696f 6e20 7661 6c75 653d 224d 4d22 2074  ion value="MM" t
-00000920: 7970 653d 2251 5374 7269 6e67 2220 6e61  ype="QString" na
-00000930: 6d65 3d22 6461 7368 5f70 6174 7465 726e  me="dash_pattern
-00000940: 5f6f 6666 7365 745f 756e 6974 222f 3e0a  _offset_unit"/>.
+00000910: 696f 6e20 7661 6c75 653d 224d 4d22 206e  ion value="MM" n
+00000920: 616d 653d 2264 6173 685f 7061 7474 6572  ame="dash_patter
+00000930: 6e5f 6f66 6673 6574 5f75 6e69 7422 2074  n_offset_unit" t
+00000940: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
 00000950: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00000960: 696f 6e20 7661 6c75 653d 2230 2220 7479  ion value="0" ty
-00000970: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00000980: 653d 2264 7261 775f 696e 7369 6465 5f70  e="draw_inside_p
-00000990: 6f6c 7967 6f6e 222f 3e0a 2020 2020 2020  olygon"/>.      
+00000960: 696f 6e20 7661 6c75 653d 2230 2220 6e61  ion value="0" na
+00000970: 6d65 3d22 6472 6177 5f69 6e73 6964 655f  me="draw_inside_
+00000980: 706f 6c79 676f 6e22 2074 7970 653d 2251  polygon" type="Q
+00000990: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
 000009a0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000009b0: 6c75 653d 2262 6576 656c 2220 7479 7065  lue="bevel" type
-000009c0: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-000009d0: 226a 6f69 6e73 7479 6c65 222f 3e0a 2020  "joinstyle"/>.  
+000009b0: 6c75 653d 2262 6576 656c 2220 6e61 6d65  lue="bevel" name
+000009c0: 3d22 6a6f 696e 7374 796c 6522 2074 7970  ="joinstyle" typ
+000009d0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
 000009e0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000009f0: 6e20 7661 6c75 653d 2231 3930 2c32 3037  n value="190,207
-00000a00: 2c38 302c 3235 3522 2074 7970 653d 2251  ,80,255" type="Q
-00000a10: 5374 7269 6e67 2220 6e61 6d65 3d22 6c69  String" name="li
-00000a20: 6e65 5f63 6f6c 6f72 222f 3e0a 2020 2020  ne_color"/>.    
-00000a30: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00000a40: 7661 6c75 653d 2273 6f6c 6964 2220 7479  value="solid" ty
-00000a50: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00000a60: 653d 226c 696e 655f 7374 796c 6522 2f3e  e="line_style"/>
-00000a70: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00000a80: 7469 6f6e 2076 616c 7565 3d22 302e 3622  tion value="0.6"
-00000a90: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-00000aa0: 6e61 6d65 3d22 6c69 6e65 5f77 6964 7468  name="line_width
-00000ab0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00000ac0: 3c4f 7074 696f 6e20 7661 6c75 653d 224d  <Option value="M
-00000ad0: 4d22 2074 7970 653d 2251 5374 7269 6e67  M" type="QString
-00000ae0: 2220 6e61 6d65 3d22 6c69 6e65 5f77 6964  " name="line_wid
-00000af0: 7468 5f75 6e69 7422 2f3e 0a20 2020 2020  th_unit"/>.     
-00000b00: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00000b10: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
-00000b20: 5374 7269 6e67 2220 6e61 6d65 3d22 6f66  String" name="of
-00000b30: 6673 6574 222f 3e0a 2020 2020 2020 2020  fset"/>.        
-00000b40: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00000b50: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00000b60: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00000b70: 2220 6e61 6d65 3d22 6f66 6673 6574 5f6d  " name="offset_m
-00000b80: 6170 5f75 6e69 745f 7363 616c 6522 2f3e  ap_unit_scale"/>
-00000b90: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00000ba0: 7469 6f6e 2076 616c 7565 3d22 4d4d 2220  tion value="MM" 
-00000bb0: 7479 7065 3d22 5153 7472 696e 6722 206e  type="QString" n
-00000bc0: 616d 653d 226f 6666 7365 745f 756e 6974  ame="offset_unit
-00000bd0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00000be0: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
-00000bf0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00000c00: 206e 616d 653d 2272 696e 675f 6669 6c74   name="ring_filt
-00000c10: 6572 222f 3e0a 2020 2020 2020 2020 2020  er"/>.          
-00000c20: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00000c30: 2230 2220 7479 7065 3d22 5153 7472 696e  "0" type="QStrin
-00000c40: 6722 206e 616d 653d 2274 7269 6d5f 6469  g" name="trim_di
-00000c50: 7374 616e 6365 5f65 6e64 222f 3e0a 2020  stance_end"/>.  
-00000c60: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00000c70: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-00000c80: 302c 302c 302c 3022 2074 7970 653d 2251  0,0,0,0" type="Q
-00000c90: 5374 7269 6e67 2220 6e61 6d65 3d22 7472  String" name="tr
-00000ca0: 696d 5f64 6973 7461 6e63 655f 656e 645f  im_distance_end_
-00000cb0: 6d61 705f 756e 6974 5f73 6361 6c65 222f  map_unit_scale"/
-00000cc0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00000cd0: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
-00000ce0: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-00000cf0: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00000d00: 6e63 655f 656e 645f 756e 6974 222f 3e0a  nce_end_unit"/>.
-00000d10: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00000d20: 696f 6e20 7661 6c75 653d 2230 2220 7479  ion value="0" ty
-00000d30: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00000d40: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
-00000d50: 5f73 7461 7274 222f 3e0a 2020 2020 2020  _start"/>.      
-00000d60: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00000d70: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00000d80: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-00000d90: 6e67 2220 6e61 6d65 3d22 7472 696d 5f64  ng" name="trim_d
-00000da0: 6973 7461 6e63 655f 7374 6172 745f 6d61  istance_start_ma
-00000db0: 705f 756e 6974 5f73 6361 6c65 222f 3e0a  p_unit_scale"/>.
-00000dc0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00000dd0: 696f 6e20 7661 6c75 653d 224d 4d22 2074  ion value="MM" t
-00000de0: 7970 653d 2251 5374 7269 6e67 2220 6e61  ype="QString" na
-00000df0: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
-00000e00: 655f 7374 6172 745f 756e 6974 222f 3e0a  e_start_unit"/>.
-00000e10: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00000e20: 696f 6e20 7661 6c75 653d 2230 2220 7479  ion value="0" ty
-00000e30: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00000e40: 653d 2274 7765 616b 5f64 6173 685f 7061  e="tweak_dash_pa
-00000e50: 7474 6572 6e5f 6f6e 5f63 6f72 6e65 7273  ttern_on_corners
-00000e60: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00000e70: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
-00000e80: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00000e90: 206e 616d 653d 2275 7365 5f63 7573 746f   name="use_custo
-00000ea0: 6d5f 6461 7368 222f 3e0a 2020 2020 2020  m_dash"/>.      
-00000eb0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00000ec0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00000ed0: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-00000ee0: 6e67 2220 6e61 6d65 3d22 7769 6474 685f  ng" name="width_
-00000ef0: 6d61 705f 756e 6974 5f73 6361 6c65 222f  map_unit_scale"/
-00000f00: 3e0a 2020 2020 2020 2020 2020 3c2f 4f70  >.          </Op
-00000f10: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00000f20: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-00000f30: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00000f40: 2020 2020 2020 3c4f 7074 696f 6e20 7479        <Option ty
-00000f50: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
-00000f60: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00000f70: 7661 6c75 653d 2222 2074 7970 653d 2251  value="" type="Q
-00000f80: 5374 7269 6e67 2220 6e61 6d65 3d22 6e61  String" name="na
-00000f90: 6d65 222f 3e0a 2020 2020 2020 2020 2020  me"/>.          
-00000fa0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00000fb0: 3d22 7072 6f70 6572 7469 6573 222f 3e0a  ="properties"/>.
-00000fc0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00000fd0: 7074 696f 6e20 7661 6c75 653d 2263 6f6c  ption value="col
-00000fe0: 6c65 6374 696f 6e22 2074 7970 653d 2251  lection" type="Q
-00000ff0: 5374 7269 6e67 2220 6e61 6d65 3d22 7479  String" name="ty
-00001000: 7065 222f 3e0a 2020 2020 2020 2020 2020  pe"/>.          
-00001010: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-00001020: 2020 2020 2020 3c2f 6461 7461 5f64 6566        </data_def
-00001030: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
-00001040: 0a20 2020 2020 2020 203c 2f6c 6179 6572  .        </layer
-00001050: 3e0a 2020 2020 2020 3c2f 7379 6d62 6f6c  >.      </symbol
-00001060: 3e0a 2020 2020 3c2f 7072 6f66 696c 654c  >.    </profileL
-00001070: 696e 6553 796d 626f 6c3e 0a20 2020 203c  ineSymbol>.    <
-00001080: 7072 6f66 696c 6546 696c 6c53 796d 626f  profileFillSymbo
-00001090: 6c3e 0a20 2020 2020 203c 7379 6d62 6f6c  l>.      <symbol
-000010a0: 2063 6c69 705f 746f 5f65 7874 656e 743d   clip_to_extent=
-000010b0: 2231 2220 6973 5f61 6e69 6d61 7465 643d  "1" is_animated=
-000010c0: 2230 2220 7479 7065 3d22 6669 6c6c 2220  "0" type="fill" 
-000010d0: 666f 7263 655f 7268 723d 2230 2220 6e61  force_rhr="0" na
-000010e0: 6d65 3d22 2220 616c 7068 613d 2231 2220  me="" alpha="1" 
-000010f0: 6672 616d 655f 7261 7465 3d22 3130 223e  frame_rate="10">
-00001100: 0a20 2020 2020 2020 203c 6461 7461 5f64  .        <data_d
-00001110: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
-00001120: 733e 0a20 2020 2020 2020 2020 203c 4f70  s>.          <Op
-00001130: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
-00001140: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00001150: 7469 6f6e 2076 616c 7565 3d22 2220 7479  tion value="" ty
-00001160: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00001170: 653d 226e 616d 6522 2f3e 0a20 2020 2020  e="name"/>.     
-00001180: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00001190: 616d 653d 2270 726f 7065 7274 6965 7322  ame="properties"
-000011a0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000011b0: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
-000011c0: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
-000011d0: 5153 7472 696e 6722 206e 616d 653d 2274  QString" name="t
-000011e0: 7970 6522 2f3e 0a20 2020 2020 2020 2020  ype"/>.         
-000011f0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
-00001200: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
-00001210: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00001220: 2020 2020 2020 3c6c 6179 6572 2065 6e61        <layer ena
-00001230: 626c 6564 3d22 3122 2063 6c61 7373 3d22  bled="1" class="
-00001240: 5369 6d70 6c65 4669 6c6c 2220 7061 7373  SimpleFill" pass
-00001250: 3d22 3022 206c 6f63 6b65 643d 2230 223e  ="0" locked="0">
-00001260: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-00001270: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
-00001280: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00001290: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
-000012a0: 2c30 2c30 2c30 2c30 2220 7479 7065 3d22  ,0,0,0,0" type="
-000012b0: 5153 7472 696e 6722 206e 616d 653d 2262  QString" name="b
-000012c0: 6f72 6465 725f 7769 6474 685f 6d61 705f  order_width_map_
-000012d0: 756e 6974 5f73 6361 6c65 222f 3e0a 2020  unit_scale"/>.  
-000012e0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000012f0: 6e20 7661 6c75 653d 2231 3930 2c32 3037  n value="190,207
-00001300: 2c38 302c 3235 3522 2074 7970 653d 2251  ,80,255" type="Q
-00001310: 5374 7269 6e67 2220 6e61 6d65 3d22 636f  String" name="co
-00001320: 6c6f 7222 2f3e 0a20 2020 2020 2020 2020  lor"/>.         
-00001330: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00001340: 3d22 6265 7665 6c22 2074 7970 653d 2251  ="bevel" type="Q
-00001350: 5374 7269 6e67 2220 6e61 6d65 3d22 6a6f  String" name="jo
-00001360: 696e 7374 796c 6522 2f3e 0a20 2020 2020  instyle"/>.     
-00001370: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00001380: 616c 7565 3d22 302c 3022 2074 7970 653d  alue="0,0" type=
-00001390: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-000013a0: 6f66 6673 6574 222f 3e0a 2020 2020 2020  offset"/>.      
-000013b0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000013c0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-000013d0: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-000013e0: 6e67 2220 6e61 6d65 3d22 6f66 6673 6574  ng" name="offset
-000013f0: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
-00001400: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001410: 4f70 7469 6f6e 2076 616c 7565 3d22 4d4d  Option value="MM
-00001420: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00001430: 206e 616d 653d 226f 6666 7365 745f 756e   name="offset_un
-00001440: 6974 222f 3e0a 2020 2020 2020 2020 2020  it"/>.          
-00001450: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00001460: 2231 3336 2c31 3438 2c35 372c 3235 3522  "136,148,57,255"
-00001470: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-00001480: 6e61 6d65 3d22 6f75 746c 696e 655f 636f  name="outline_co
-00001490: 6c6f 7222 2f3e 0a20 2020 2020 2020 2020  lor"/>.         
-000014a0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000014b0: 3d22 736f 6c69 6422 2074 7970 653d 2251  ="solid" type="Q
-000014c0: 5374 7269 6e67 2220 6e61 6d65 3d22 6f75  String" name="ou
-000014d0: 746c 696e 655f 7374 796c 6522 2f3e 0a20  tline_style"/>. 
-000014e0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000014f0: 6f6e 2076 616c 7565 3d22 302e 3222 2074  on value="0.2" t
-00001500: 7970 653d 2251 5374 7269 6e67 2220 6e61  ype="QString" na
-00001510: 6d65 3d22 6f75 746c 696e 655f 7769 6474  me="outline_widt
-00001520: 6822 2f3e 0a20 2020 2020 2020 2020 2020  h"/>.           
-00001530: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00001540: 4d4d 2220 7479 7065 3d22 5153 7472 696e  MM" type="QStrin
-00001550: 6722 206e 616d 653d 226f 7574 6c69 6e65  g" name="outline
-00001560: 5f77 6964 7468 5f75 6e69 7422 2f3e 0a20  _width_unit"/>. 
-00001570: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00001580: 6f6e 2076 616c 7565 3d22 736f 6c69 6422  on value="solid"
-00001590: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-000015a0: 6e61 6d65 3d22 7374 796c 6522 2f3e 0a20  name="style"/>. 
-000015b0: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-000015c0: 6e3e 0a20 2020 2020 2020 2020 203c 6461  n>.          <da
-000015d0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-000015e0: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
-000015f0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00001600: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00001610: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00001620: 7565 3d22 2220 7479 7065 3d22 5153 7472  ue="" type="QStr
-00001630: 696e 6722 206e 616d 653d 226e 616d 6522  ing" name="name"
-00001640: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00001650: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
-00001660: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
-00001670: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00001680: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
-00001690: 7469 6f6e 2220 7479 7065 3d22 5153 7472  tion" type="QStr
-000016a0: 696e 6722 206e 616d 653d 2274 7970 6522  ing" name="type"
-000016b0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000016c0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-000016d0: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
-000016e0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-000016f0: 2020 2020 2020 3c2f 6c61 7965 723e 0a20        </layer>. 
-00001700: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
-00001710: 2020 203c 2f70 726f 6669 6c65 4669 6c6c     </profileFill
-00001720: 5379 6d62 6f6c 3e0a 2020 2020 3c70 726f  Symbol>.    <pro
-00001730: 6669 6c65 4d61 726b 6572 5379 6d62 6f6c  fileMarkerSymbol
-00001740: 3e0a 2020 2020 2020 3c73 796d 626f 6c20  >.      <symbol 
-00001750: 636c 6970 5f74 6f5f 6578 7465 6e74 3d22  clip_to_extent="
-00001760: 3122 2069 735f 616e 696d 6174 6564 3d22  1" is_animated="
-00001770: 3022 2074 7970 653d 226d 6172 6b65 7222  0" type="marker"
-00001780: 2066 6f72 6365 5f72 6872 3d22 3022 206e   force_rhr="0" n
-00001790: 616d 653d 2222 2061 6c70 6861 3d22 3122  ame="" alpha="1"
-000017a0: 2066 7261 6d65 5f72 6174 653d 2231 3022   frame_rate="10"
-000017b0: 3e0a 2020 2020 2020 2020 3c64 6174 615f  >.        <data_
-000017c0: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
-000017d0: 6573 3e0a 2020 2020 2020 2020 2020 3c4f  es>.          <O
-000017e0: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
-000017f0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00001800: 7074 696f 6e20 7661 6c75 653d 2222 2074  ption value="" t
-00001810: 7970 653d 2251 5374 7269 6e67 2220 6e61  ype="QString" na
-00001820: 6d65 3d22 6e61 6d65 222f 3e0a 2020 2020  me="name"/>.    
-00001830: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00001840: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
-00001850: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00001860: 3c4f 7074 696f 6e20 7661 6c75 653d 2263  <Option value="c
-00001870: 6f6c 6c65 6374 696f 6e22 2074 7970 653d  ollection" type=
-00001880: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00001890: 7479 7065 222f 3e0a 2020 2020 2020 2020  type"/>.        
-000018a0: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-000018b0: 2020 2020 3c2f 6461 7461 5f64 6566 696e      </data_defin
-000018c0: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
-000018d0: 2020 2020 2020 203c 6c61 7965 7220 656e         <layer en
-000018e0: 6162 6c65 643d 2231 2220 636c 6173 733d  abled="1" class=
-000018f0: 2253 696d 706c 654d 6172 6b65 7222 2070  "SimpleMarker" p
-00001900: 6173 733d 2230 2220 6c6f 636b 6564 3d22  ass="0" locked="
-00001910: 3022 3e0a 2020 2020 2020 2020 2020 3c4f  0">.          <O
-00001920: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
-00001930: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00001940: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-00001950: 7479 7065 3d22 5153 7472 696e 6722 206e  type="QString" n
-00001960: 616d 653d 2261 6e67 6c65 222f 3e0a 2020  ame="angle"/>.  
-00001970: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00001980: 6e20 7661 6c75 653d 2273 7175 6172 6522  n value="square"
-00001990: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-000019a0: 6e61 6d65 3d22 6361 705f 7374 796c 6522  name="cap_style"
-000019b0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000019c0: 4f70 7469 6f6e 2076 616c 7565 3d22 3139  Option value="19
-000019d0: 302c 3230 372c 3830 2c32 3535 2220 7479  0,207,80,255" ty
-000019e0: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-000019f0: 653d 2263 6f6c 6f72 222f 3e0a 2020 2020  e="color"/>.    
-00001a00: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00001a10: 7661 6c75 653d 2231 2220 7479 7065 3d22  value="1" type="
-00001a20: 5153 7472 696e 6722 206e 616d 653d 2268  QString" name="h
-00001a30: 6f72 697a 6f6e 7461 6c5f 616e 6368 6f72  orizontal_anchor
-00001a40: 5f70 6f69 6e74 222f 3e0a 2020 2020 2020  _point"/>.      
-00001a50: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00001a60: 6c75 653d 2262 6576 656c 2220 7479 7065  lue="bevel" type
-00001a70: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-00001a80: 226a 6f69 6e73 7479 6c65 222f 3e0a 2020  "joinstyle"/>.  
-00001a90: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00001aa0: 6e20 7661 6c75 653d 2264 6961 6d6f 6e64  n value="diamond
-00001ab0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00001ac0: 206e 616d 653d 226e 616d 6522 2f3e 0a20   name="name"/>. 
-00001ad0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00001ae0: 6f6e 2076 616c 7565 3d22 302c 3022 2074  on value="0,0" t
-00001af0: 7970 653d 2251 5374 7269 6e67 2220 6e61  ype="QString" na
-00001b00: 6d65 3d22 6f66 6673 6574 222f 3e0a 2020  me="offset"/>.  
-00001b10: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00001b20: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-00001b30: 302c 302c 302c 3022 2074 7970 653d 2251  0,0,0,0" type="Q
-00001b40: 5374 7269 6e67 2220 6e61 6d65 3d22 6f66  String" name="of
-00001b50: 6673 6574 5f6d 6170 5f75 6e69 745f 7363  fset_map_unit_sc
-00001b60: 616c 6522 2f3e 0a20 2020 2020 2020 2020  ale"/>.         
-00001b70: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00001b80: 3d22 4d4d 2220 7479 7065 3d22 5153 7472  ="MM" type="QStr
-00001b90: 696e 6722 206e 616d 653d 226f 6666 7365  ing" name="offse
-00001ba0: 745f 756e 6974 222f 3e0a 2020 2020 2020  t_unit"/>.      
-00001bb0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00001bc0: 6c75 653d 2231 3336 2c31 3438 2c35 372c  lue="136,148,57,
-00001bd0: 3235 3522 2074 7970 653d 2251 5374 7269  255" type="QStri
-00001be0: 6e67 2220 6e61 6d65 3d22 6f75 746c 696e  ng" name="outlin
-00001bf0: 655f 636f 6c6f 7222 2f3e 0a20 2020 2020  e_color"/>.     
-00001c00: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00001c10: 616c 7565 3d22 736f 6c69 6422 2074 7970  alue="solid" typ
-00001c20: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-00001c30: 3d22 6f75 746c 696e 655f 7374 796c 6522  ="outline_style"
-00001c40: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001c50: 4f70 7469 6f6e 2076 616c 7565 3d22 302e  Option value="0.
-00001c60: 3222 2074 7970 653d 2251 5374 7269 6e67  2" type="QString
-00001c70: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
-00001c80: 7769 6474 6822 2f3e 0a20 2020 2020 2020  width"/>.       
-00001c90: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00001ca0: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
-00001cb0: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
-00001cc0: 6722 206e 616d 653d 226f 7574 6c69 6e65  g" name="outline
-00001cd0: 5f77 6964 7468 5f6d 6170 5f75 6e69 745f  _width_map_unit_
-00001ce0: 7363 616c 6522 2f3e 0a20 2020 2020 2020  scale"/>.       
-00001cf0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00001d00: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
-00001d10: 7472 696e 6722 206e 616d 653d 226f 7574  tring" name="out
-00001d20: 6c69 6e65 5f77 6964 7468 5f75 6e69 7422  line_width_unit"
-00001d30: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00001d40: 4f70 7469 6f6e 2076 616c 7565 3d22 6469  Option value="di
-00001d50: 616d 6574 6572 2220 7479 7065 3d22 5153  ameter" type="QS
-00001d60: 7472 696e 6722 206e 616d 653d 2273 6361  tring" name="sca
-00001d70: 6c65 5f6d 6574 686f 6422 2f3e 0a20 2020  le_method"/>.   
-00001d80: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00001d90: 2076 616c 7565 3d22 3322 2074 7970 653d   value="3" type=
-00001da0: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00001db0: 7369 7a65 222f 3e0a 2020 2020 2020 2020  size"/>.        
-00001dc0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00001dd0: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00001de0: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00001df0: 2220 6e61 6d65 3d22 7369 7a65 5f6d 6170  " name="size_map
-00001e00: 5f75 6e69 745f 7363 616c 6522 2f3e 0a20  _unit_scale"/>. 
-00001e10: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00001e20: 6f6e 2076 616c 7565 3d22 4d4d 2220 7479  on value="MM" ty
-00001e30: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00001e40: 653d 2273 697a 655f 756e 6974 222f 3e0a  e="size_unit"/>.
-00001e50: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00001e60: 696f 6e20 7661 6c75 653d 2231 2220 7479  ion value="1" ty
-00001e70: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00001e80: 653d 2276 6572 7469 6361 6c5f 616e 6368  e="vertical_anch
-00001e90: 6f72 5f70 6f69 6e74 222f 3e0a 2020 2020  or_point"/>.    
-00001ea0: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
-00001eb0: 2020 2020 2020 2020 2020 3c64 6174 615f            <data_
-00001ec0: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
-00001ed0: 6573 3e0a 2020 2020 2020 2020 2020 2020  es>.            
-00001ee0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
-00001ef0: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
-00001f00: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00001f10: 2222 2074 7970 653d 2251 5374 7269 6e67  "" type="QString
-00001f20: 2220 6e61 6d65 3d22 6e61 6d65 222f 3e0a  " name="name"/>.
-00001f30: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-00001f40: 7074 696f 6e20 6e61 6d65 3d22 7072 6f70  ption name="prop
-00001f50: 6572 7469 6573 222f 3e0a 2020 2020 2020  erties"/>.      
-00001f60: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00001f70: 7661 6c75 653d 2263 6f6c 6c65 6374 696f  value="collectio
-00001f80: 6e22 2074 7970 653d 2251 5374 7269 6e67  n" type="QString
-00001f90: 2220 6e61 6d65 3d22 7479 7065 222f 3e0a  " name="type"/>.
-00001fa0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-00001fb0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00001fc0: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
-00001fd0: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00001fe0: 2020 203c 2f6c 6179 6572 3e0a 2020 2020     </layer>.    
-00001ff0: 2020 3c2f 7379 6d62 6f6c 3e0a 2020 2020    </symbol>.    
-00002000: 3c2f 7072 6f66 696c 654d 6172 6b65 7253  </profileMarkerS
-00002010: 796d 626f 6c3e 0a20 203c 2f65 6c65 7661  ymbol>.  </eleva
-00002020: 7469 6f6e 3e0a 2020 3c72 656e 6465 7265  tion>.  <rendere
-00002030: 722d 7632 2066 6f72 6365 7261 7374 6572  r-v2 forceraster
-00002040: 3d22 3022 2065 6e61 626c 656f 7264 6572  ="0" enableorder
-00002050: 6279 3d22 3022 2074 7970 653d 2273 696e  by="0" type="sin
-00002060: 676c 6553 796d 626f 6c22 2072 6566 6572  gleSymbol" refer
-00002070: 656e 6365 7363 616c 653d 222d 3122 2073  encescale="-1" s
-00002080: 796d 626f 6c6c 6576 656c 733d 2230 223e  ymbollevels="0">
-00002090: 0a20 2020 203c 7379 6d62 6f6c 733e 0a20  .    <symbols>. 
-000020a0: 2020 2020 203c 7379 6d62 6f6c 2063 6c69       <symbol cli
-000020b0: 705f 746f 5f65 7874 656e 743d 2231 2220  p_to_extent="1" 
-000020c0: 6973 5f61 6e69 6d61 7465 643d 2230 2220  is_animated="0" 
-000020d0: 7479 7065 3d22 6669 6c6c 2220 666f 7263  type="fill" forc
-000020e0: 655f 7268 723d 2230 2220 6e61 6d65 3d22  e_rhr="0" name="
-000020f0: 3022 2061 6c70 6861 3d22 3122 2066 7261  0" alpha="1" fra
-00002100: 6d65 5f72 6174 653d 2231 3022 3e0a 2020  me_rate="10">.  
-00002110: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
-00002120: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
-00002130: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002140: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
-00002150: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002160: 6e20 7661 6c75 653d 2222 2074 7970 653d  n value="" type=
-00002170: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00002180: 6e61 6d65 222f 3e0a 2020 2020 2020 2020  name"/>.        
-00002190: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000021a0: 3d22 7072 6f70 6572 7469 6573 222f 3e0a  ="properties"/>.
-000021b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000021c0: 696f 6e20 7661 6c75 653d 2263 6f6c 6c65  ion value="colle
-000021d0: 6374 696f 6e22 2074 7970 653d 2251 5374  ction" type="QSt
-000021e0: 7269 6e67 2220 6e61 6d65 3d22 7479 7065  ring" name="type
-000021f0: 222f 3e0a 2020 2020 2020 2020 2020 3c2f  "/>.          </
-00002200: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
-00002210: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
-00002220: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00002230: 2020 203c 6c61 7965 7220 656e 6162 6c65     <layer enable
-00002240: 643d 2231 2220 636c 6173 733d 2253 696d  d="1" class="Sim
-00002250: 706c 6546 696c 6c22 2070 6173 733d 2230  pleFill" pass="0
-00002260: 2220 6c6f 636b 6564 3d22 3022 3e0a 2020  " locked="0">.  
-00002270: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002280: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-00002290: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000022a0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
-000022b0: 302c 302c 3022 2074 7970 653d 2251 5374  0,0,0" type="QSt
-000022c0: 7269 6e67 2220 6e61 6d65 3d22 626f 7264  ring" name="bord
-000022d0: 6572 5f77 6964 7468 5f6d 6170 5f75 6e69  er_width_map_uni
-000022e0: 745f 7363 616c 6522 2f3e 0a20 2020 2020  t_scale"/>.     
-000022f0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00002300: 616c 7565 3d22 3235 352c 3235 352c 3235  alue="255,255,25
-00002310: 352c 3235 3522 2074 7970 653d 2251 5374  5,255" type="QSt
-00002320: 7269 6e67 2220 6e61 6d65 3d22 636f 6c6f  ring" name="colo
-00002330: 7222 2f3e 0a20 2020 2020 2020 2020 2020  r"/>.           
-00002340: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00002350: 6265 7665 6c22 2074 7970 653d 2251 5374  bevel" type="QSt
-00002360: 7269 6e67 2220 6e61 6d65 3d22 6a6f 696e  ring" name="join
-00002370: 7374 796c 6522 2f3e 0a20 2020 2020 2020  style"/>.       
-00002380: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002390: 7565 3d22 302c 3022 2074 7970 653d 2251  ue="0,0" type="Q
-000023a0: 5374 7269 6e67 2220 6e61 6d65 3d22 6f66  String" name="of
-000023b0: 6673 6574 222f 3e0a 2020 2020 2020 2020  fset"/>.        
-000023c0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000023d0: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-000023e0: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-000023f0: 2220 6e61 6d65 3d22 6f66 6673 6574 5f6d  " name="offset_m
-00002400: 6170 5f75 6e69 745f 7363 616c 6522 2f3e  ap_unit_scale"/>
-00002410: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00002420: 7469 6f6e 2076 616c 7565 3d22 4d4d 2220  tion value="MM" 
-00002430: 7479 7065 3d22 5153 7472 696e 6722 206e  type="QString" n
-00002440: 616d 653d 226f 6666 7365 745f 756e 6974  ame="offset_unit
-00002450: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002460: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
-00002470: 352c 3335 2c33 352c 3235 3522 2074 7970  5,35,35,255" typ
-00002480: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-00002490: 3d22 6f75 746c 696e 655f 636f 6c6f 7222  ="outline_color"
-000024a0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000024b0: 4f70 7469 6f6e 2076 616c 7565 3d22 6e6f  Option value="no
-000024c0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000024d0: 206e 616d 653d 226f 7574 6c69 6e65 5f73   name="outline_s
-000024e0: 7479 6c65 222f 3e0a 2020 2020 2020 2020  tyle"/>.        
-000024f0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002500: 653d 2230 2220 7479 7065 3d22 5153 7472  e="0" type="QStr
-00002510: 696e 6722 206e 616d 653d 226f 7574 6c69  ing" name="outli
-00002520: 6e65 5f77 6964 7468 222f 3e0a 2020 2020  ne_width"/>.    
-00002530: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002540: 7661 6c75 653d 224d 4d22 2074 7970 653d  value="MM" type=
-00002550: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00002560: 6f75 746c 696e 655f 7769 6474 685f 756e  outline_width_un
-00002570: 6974 222f 3e0a 2020 2020 2020 2020 2020  it"/>.          
-00002580: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00002590: 2273 6f6c 6964 2220 7479 7065 3d22 5153  "solid" type="QS
-000025a0: 7472 696e 6722 206e 616d 653d 2273 7479  tring" name="sty
-000025b0: 6c65 222f 3e0a 2020 2020 2020 2020 2020  le"/>.          
-000025c0: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
-000025d0: 2020 2020 3c64 6174 615f 6465 6669 6e65      <data_define
-000025e0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-000025f0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002600: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
-00002610: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00002620: 696f 6e20 7661 6c75 653d 2222 2074 7970  ion value="" typ
-00002630: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-00002640: 3d22 6e61 6d65 222f 3e0a 2020 2020 2020  ="name"/>.      
-00002650: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002660: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
-00002670: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002680: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00002690: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-000026a0: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-000026b0: 3d22 7479 7065 222f 3e0a 2020 2020 2020  ="type"/>.      
-000026c0: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
-000026d0: 2020 2020 2020 2020 2020 3c2f 6461 7461            </data
-000026e0: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
-000026f0: 6965 733e 0a20 2020 2020 2020 203c 2f6c  ies>.        </l
-00002700: 6179 6572 3e0a 2020 2020 2020 2020 3c6c  ayer>.        <l
-00002710: 6179 6572 2065 6e61 626c 6564 3d22 3122  ayer enabled="1"
-00002720: 2063 6c61 7373 3d22 5356 4746 696c 6c22   class="SVGFill"
-00002730: 2070 6173 733d 2230 2220 6c6f 636b 6564   pass="0" locked
-00002740: 3d22 3022 3e0a 2020 2020 2020 2020 2020  ="0">.          
-00002750: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
-00002760: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
-00002770: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
-00002780: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00002790: 206e 616d 653d 2261 6e67 6c65 222f 3e0a   name="angle"/>.
-000027a0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000027b0: 696f 6e20 7661 6c75 653d 2239 372c 3937  ion value="97,97
-000027c0: 2c39 372c 3235 3522 2074 7970 653d 2251  ,97,255" type="Q
-000027d0: 5374 7269 6e67 2220 6e61 6d65 3d22 636f  String" name="co
-000027e0: 6c6f 7222 2f3e 0a20 2020 2020 2020 2020  lor"/>.         
-000027f0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00002800: 3d22 3235 352c 3235 352c 3235 352c 3235  ="255,255,255,25
-00002810: 3522 2074 7970 653d 2251 5374 7269 6e67  5" type="QString
-00002820: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
-00002830: 636f 6c6f 7222 2f3e 0a20 2020 2020 2020  color"/>.       
-00002840: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002850: 7565 3d22 3022 2074 7970 653d 2251 5374  ue="0" type="QSt
-00002860: 7269 6e67 2220 6e61 6d65 3d22 6f75 746c  ring" name="outl
-00002870: 696e 655f 7769 6474 6822 2f3e 0a20 2020  ine_width"/>.   
-00002880: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00002890: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
-000028a0: 2c30 2c30 2c30 2220 7479 7065 3d22 5153  ,0,0,0" type="QS
-000028b0: 7472 696e 6722 206e 616d 653d 226f 7574  tring" name="out
-000028c0: 6c69 6e65 5f77 6964 7468 5f6d 6170 5f75  line_width_map_u
-000028d0: 6e69 745f 7363 616c 6522 2f3e 0a20 2020  nit_scale"/>.   
-000028e0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000028f0: 2076 616c 7565 3d22 4d4d 2220 7479 7065   value="MM" type
-00002900: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-00002910: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
-00002920: 6e69 7422 2f3e 0a20 2020 2020 2020 2020  nit"/>.         
-00002930: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00002940: 2270 6172 616d 6574 6572 7322 2f3e 0a20  "parameters"/>. 
-00002950: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00002960: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
-00002970: 2c30 2c30 2c30 2c30 2220 7479 7065 3d22  ,0,0,0,0" type="
-00002980: 5153 7472 696e 6722 206e 616d 653d 2270  QString" name="p
-00002990: 6174 7465 726e 5f77 6964 7468 5f6d 6170  attern_width_map
-000029a0: 5f75 6e69 745f 7363 616c 6522 2f3e 0a20  _unit_scale"/>. 
-000029b0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000029c0: 6f6e 2076 616c 7565 3d22 4d4d 2220 7479  on value="MM" ty
-000029d0: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-000029e0: 653d 2270 6174 7465 726e 5f77 6964 7468  e="pattern_width
-000029f0: 5f75 6e69 7422 2f3e 0a20 2020 2020 2020  _unit"/>.       
-00002a00: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002a10: 7565 3d22 6770 7369 636f 6e73 2f70 6f69  ue="gpsicons/poi
-00002a20: 6e74 2e73 7667 2220 7479 7065 3d22 5153  nt.svg" type="QS
-00002a30: 7472 696e 6722 206e 616d 653d 2273 7667  tring" name="svg
-00002a40: 4669 6c65 222f 3e0a 2020 2020 2020 2020  File"/>.        
-00002a50: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002a60: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00002a70: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00002a80: 2220 6e61 6d65 3d22 7376 675f 6f75 746c  " name="svg_outl
-00002a90: 696e 655f 7769 6474 685f 6d61 705f 756e  ine_width_map_un
-00002aa0: 6974 5f73 6361 6c65 222f 3e0a 2020 2020  it_scale"/>.    
-00002ab0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002ac0: 7661 6c75 653d 224d 4d22 2074 7970 653d  value="MM" type=
-00002ad0: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00002ae0: 7376 675f 6f75 746c 696e 655f 7769 6474  svg_outline_widt
-00002af0: 685f 756e 6974 222f 3e0a 2020 2020 2020  h_unit"/>.      
-00002b00: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00002b10: 6c75 653d 2235 2220 7479 7065 3d22 5153  lue="5" type="QS
-00002b20: 7472 696e 6722 206e 616d 653d 2277 6964  tring" name="wid
-00002b30: 7468 222f 3e0a 2020 2020 2020 2020 2020  th"/>.          
-00002b40: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
-00002b50: 2020 2020 3c64 6174 615f 6465 6669 6e65      <data_define
-00002b60: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00002b70: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002b80: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
-00002b90: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00002ba0: 696f 6e20 7661 6c75 653d 2222 2074 7970  ion value="" typ
-00002bb0: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-00002bc0: 3d22 6e61 6d65 222f 3e0a 2020 2020 2020  ="name"/>.      
-00002bd0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002be0: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
-00002bf0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002c00: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00002c10: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-00002c20: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-00002c30: 3d22 7479 7065 222f 3e0a 2020 2020 2020  ="type"/>.      
-00002c40: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
-00002c50: 2020 2020 2020 2020 2020 3c2f 6461 7461            </data
-00002c60: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
-00002c70: 6965 733e 0a20 2020 2020 2020 203c 2f6c  ies>.        </l
-00002c80: 6179 6572 3e0a 2020 2020 2020 3c2f 7379  ayer>.      </sy
-00002c90: 6d62 6f6c 3e0a 2020 2020 3c2f 7379 6d62  mbol>.    </symb
-00002ca0: 6f6c 733e 0a20 2020 203c 726f 7461 7469  ols>.    <rotati
-00002cb0: 6f6e 2f3e 0a20 2020 203c 7369 7a65 7363  on/>.    <sizesc
-00002cc0: 616c 652f 3e0a 2020 3c2f 7265 6e64 6572  ale/>.  </render
-00002cd0: 6572 2d76 323e 0a20 203c 6375 7374 6f6d  er-v2>.  <custom
-00002ce0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-00002cf0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
-00002d00: 7022 3e0a 2020 2020 2020 3c4f 7074 696f  p">.      <Optio
-00002d10: 6e20 7661 6c75 653d 2230 2220 7479 7065  n value="0" type
-00002d20: 3d22 696e 7422 206e 616d 653d 2265 6d62  ="int" name="emb
-00002d30: 6564 6465 6457 6964 6765 7473 2f63 6f75  eddedWidgets/cou
-00002d40: 6e74 222f 3e0a 2020 2020 2020 3c4f 7074  nt"/>.      <Opt
-00002d50: 696f 6e20 6e61 6d65 3d22 7661 7269 6162  ion name="variab
-00002d60: 6c65 4e61 6d65 7322 2f3e 0a20 2020 2020  leNames"/>.     
-00002d70: 203c 4f70 7469 6f6e 206e 616d 653d 2276   <Option name="v
-00002d80: 6172 6961 626c 6556 616c 7565 7322 2f3e  ariableValues"/>
-00002d90: 0a20 2020 203c 2f4f 7074 696f 6e3e 0a20  .    </Option>. 
-00002da0: 203c 2f63 7573 746f 6d70 726f 7065 7274   </custompropert
-00002db0: 6965 733e 0a20 203c 626c 656e 644d 6f64  ies>.  <blendMod
-00002dc0: 653e 303c 2f62 6c65 6e64 4d6f 6465 3e0a  e>0</blendMode>.
-00002dd0: 2020 3c66 6561 7475 7265 426c 656e 644d    <featureBlendM
-00002de0: 6f64 653e 303c 2f66 6561 7475 7265 426c  ode>0</featureBl
-00002df0: 656e 644d 6f64 653e 0a20 203c 6c61 7965  endMode>.  <laye
-00002e00: 724f 7061 6369 7479 3e31 3c2f 6c61 7965  rOpacity>1</laye
-00002e10: 724f 7061 6369 7479 3e0a 2020 3c53 696e  rOpacity>.  <Sin
-00002e20: 676c 6543 6174 6567 6f72 7944 6961 6772  gleCategoryDiagr
-00002e30: 616d 5265 6e64 6572 6572 2064 6961 6772  amRenderer diagr
-00002e40: 616d 5479 7065 3d22 4869 7374 6f67 7261  amType="Histogra
-00002e50: 6d22 2061 7474 7269 6275 7465 4c65 6765  m" attributeLege
-00002e60: 6e64 3d22 3122 3e0a 2020 2020 3c44 6961  nd="1">.    <Dia
-00002e70: 6772 616d 4361 7465 676f 7279 2062 6163  gramCategory bac
-00002e80: 6b67 726f 756e 6443 6f6c 6f72 3d22 2366  kgroundColor="#f
-00002e90: 6666 6666 6622 2073 7061 6369 6e67 556e  fffff" spacingUn
-00002ea0: 6974 3d22 4d4d 2220 7363 616c 6542 6173  it="MM" scaleBas
-00002eb0: 6564 5669 7369 6269 6c69 7479 3d22 3022  edVisibility="0"
-00002ec0: 2073 7061 6369 6e67 3d22 3522 206c 696e   spacing="5" lin
-00002ed0: 6553 697a 6553 6361 6c65 3d22 3378 3a30  eSizeScale="3x:0
-00002ee0: 2c30 2c30 2c30 2c30 2c30 2220 6469 7265  ,0,0,0,0,0" dire
-00002ef0: 6374 696f 6e3d 2230 2220 6d61 7853 6361  ction="0" maxSca
-00002f00: 6c65 4465 6e6f 6d69 6e61 746f 723d 2231  leDenominator="1
-00002f10: 652b 3038 2220 6d69 6e53 6361 6c65 4465  e+08" minScaleDe
-00002f20: 6e6f 6d69 6e61 746f 723d 2230 2220 6261  nominator="0" ba
-00002f30: 7257 6964 7468 3d22 3522 2072 6f74 6174  rWidth="5" rotat
-00002f40: 696f 6e4f 6666 7365 743d 2232 3730 2220  ionOffset="270" 
-00002f50: 6261 636b 6772 6f75 6e64 416c 7068 613d  backgroundAlpha=
-00002f60: 2232 3535 2220 6f70 6163 6974 793d 2231  "255" opacity="1
-00002f70: 2220 6c69 6e65 5369 7a65 5479 7065 3d22  " lineSizeType="
-00002f80: 4d4d 2220 7363 616c 6544 6570 656e 6465  MM" scaleDepende
-00002f90: 6e63 793d 2241 7265 6122 2073 686f 7741  ncy="Area" showA
-00002fa0: 7869 733d 2231 2220 7769 6474 683d 2231  xis="1" width="1
-00002fb0: 3522 2073 7061 6369 6e67 556e 6974 5363  5" spacingUnitSc
-00002fc0: 616c 653d 2233 783a 302c 302c 302c 302c  ale="3x:0,0,0,0,
-00002fd0: 302c 3022 2070 656e 436f 6c6f 723d 2223  0,0" penColor="#
-00002fe0: 3030 3030 3030 2220 7065 6e57 6964 7468  000000" penWidth
-00002ff0: 3d22 3022 206c 6162 656c 506c 6163 656d  ="0" labelPlacem
-00003000: 656e 744d 6574 686f 643d 2258 4865 6967  entMethod="XHeig
-00003010: 6874 2220 7065 6e41 6c70 6861 3d22 3235  ht" penAlpha="25
-00003020: 3522 2073 697a 6553 6361 6c65 3d22 3378  5" sizeScale="3x
-00003030: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6d69  :0,0,0,0,0,0" mi
-00003040: 6e69 6d75 6d53 697a 653d 2230 2220 656e  nimumSize="0" en
-00003050: 6162 6c65 643d 2230 2220 6865 6967 6874  abled="0" height
-00003060: 3d22 3135 2220 7369 7a65 5479 7065 3d22  ="15" sizeType="
-00003070: 4d4d 2220 6469 6167 7261 6d4f 7269 656e  MM" diagramOrien
-00003080: 7461 7469 6f6e 3d22 5570 223e 0a20 2020  tation="Up">.   
-00003090: 2020 203c 666f 6e74 5072 6f70 6572 7469     <fontProperti
-000030a0: 6573 2069 7461 6c69 633d 2230 2220 756e  es italic="0" un
-000030b0: 6465 726c 696e 653d 2230 2220 6465 7363  derline="0" desc
-000030c0: 7269 7074 696f 6e3d 224e 6f74 6f20 5361  ription="Noto Sa
-000030d0: 6e73 2c31 302c 2d31 2c30 2c35 302c 302c  ns,10,-1,0,50,0,
-000030e0: 302c 302c 302c 3022 2073 7472 696b 6574  0,0,0,0" striket
-000030f0: 6872 6f75 6768 3d22 3022 2073 7479 6c65  hrough="0" style
-00003100: 3d22 2220 626f 6c64 3d22 3022 2f3e 0a20  ="" bold="0"/>. 
-00003110: 2020 2020 203c 6174 7472 6962 7574 6520       <attribute 
-00003120: 6669 656c 643d 2222 2063 6f6c 6f72 3d22  field="" color="
-00003130: 2330 3030 3030 3022 206c 6162 656c 3d22  #000000" label="
-00003140: 2220 636f 6c6f 724f 7061 6369 7479 3d22  " colorOpacity="
-00003150: 3122 2f3e 0a20 2020 2020 203c 6178 6973  1"/>.      <axis
-00003160: 5379 6d62 6f6c 3e0a 2020 2020 2020 2020  Symbol>.        
-00003170: 3c73 796d 626f 6c20 636c 6970 5f74 6f5f  <symbol clip_to_
-00003180: 6578 7465 6e74 3d22 3122 2069 735f 616e  extent="1" is_an
-00003190: 696d 6174 6564 3d22 3022 2074 7970 653d  imated="0" type=
-000031a0: 226c 696e 6522 2066 6f72 6365 5f72 6872  "line" force_rhr
-000031b0: 3d22 3022 206e 616d 653d 2222 2061 6c70  ="0" name="" alp
-000031c0: 6861 3d22 3122 2066 7261 6d65 5f72 6174  ha="1" frame_rat
-000031d0: 653d 2231 3022 3e0a 2020 2020 2020 2020  e="10">.        
-000031e0: 2020 3c64 6174 615f 6465 6669 6e65 645f    <data_defined_
-000031f0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-00003200: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003210: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-00003220: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003230: 6e20 7661 6c75 653d 2222 2074 7970 653d  n value="" type=
-00003240: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00003250: 6e61 6d65 222f 3e0a 2020 2020 2020 2020  name"/>.        
-00003260: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00003270: 6d65 3d22 7072 6f70 6572 7469 6573 222f  me="properties"/
-00003280: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003290: 3c4f 7074 696f 6e20 7661 6c75 653d 2263  <Option value="c
-000032a0: 6f6c 6c65 6374 696f 6e22 2074 7970 653d  ollection" type=
-000032b0: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-000032c0: 7479 7065 222f 3e0a 2020 2020 2020 2020  type"/>.        
-000032d0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-000032e0: 2020 2020 2020 2020 3c2f 6461 7461 5f64          </data_d
-000032f0: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
-00003300: 733e 0a20 2020 2020 2020 2020 203c 6c61  s>.          <la
-00003310: 7965 7220 656e 6162 6c65 643d 2231 2220  yer enabled="1" 
-00003320: 636c 6173 733d 2253 696d 706c 654c 696e  class="SimpleLin
-00003330: 6522 2070 6173 733d 2230 2220 6c6f 636b  e" pass="0" lock
-00003340: 6564 3d22 3022 3e0a 2020 2020 2020 2020  ed="0">.        
-00003350: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
-00003360: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-00003370: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003380: 6c75 653d 2230 2220 7479 7065 3d22 5153  lue="0" type="QS
-00003390: 7472 696e 6722 206e 616d 653d 2261 6c69  tring" name="ali
-000033a0: 676e 5f64 6173 685f 7061 7474 6572 6e22  gn_dash_pattern"
-000033b0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-000033c0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000033d0: 7371 7561 7265 2220 7479 7065 3d22 5153  square" type="QS
-000033e0: 7472 696e 6722 206e 616d 653d 2263 6170  tring" name="cap
-000033f0: 7374 796c 6522 2f3e 0a20 2020 2020 2020  style"/>.       
-00003400: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003410: 616c 7565 3d22 353b 3222 2074 7970 653d  alue="5;2" type=
-00003420: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00003430: 6375 7374 6f6d 6461 7368 222f 3e0a 2020  customdash"/>.  
-00003440: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00003450: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
-00003460: 302c 302c 302c 302c 3022 2074 7970 653d  0,0,0,0,0" type=
-00003470: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00003480: 6375 7374 6f6d 6461 7368 5f6d 6170 5f75  customdash_map_u
-00003490: 6e69 745f 7363 616c 6522 2f3e 0a20 2020  nit_scale"/>.   
-000034a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000034b0: 6f6e 2076 616c 7565 3d22 4d4d 2220 7479  on value="MM" ty
-000034c0: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-000034d0: 653d 2263 7573 746f 6d64 6173 685f 756e  e="customdash_un
-000034e0: 6974 222f 3e0a 2020 2020 2020 2020 2020  it"/>.          
-000034f0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003500: 653d 2230 2220 7479 7065 3d22 5153 7472  e="0" type="QStr
-00003510: 696e 6722 206e 616d 653d 2264 6173 685f  ing" name="dash_
-00003520: 7061 7474 6572 6e5f 6f66 6673 6574 222f  pattern_offset"/
-00003530: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003540: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
-00003550: 783a 302c 302c 302c 302c 302c 3022 2074  x:0,0,0,0,0,0" t
-00003560: 7970 653d 2251 5374 7269 6e67 2220 6e61  ype="QString" na
-00003570: 6d65 3d22 6461 7368 5f70 6174 7465 726e  me="dash_pattern
-00003580: 5f6f 6666 7365 745f 6d61 705f 756e 6974  _offset_map_unit
-00003590: 5f73 6361 6c65 222f 3e0a 2020 2020 2020  _scale"/>.      
-000035a0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000035b0: 7661 6c75 653d 224d 4d22 2074 7970 653d  value="MM" type=
-000035c0: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-000035d0: 6461 7368 5f70 6174 7465 726e 5f6f 6666  dash_pattern_off
-000035e0: 7365 745f 756e 6974 222f 3e0a 2020 2020  set_unit"/>.    
-000035f0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003600: 6e20 7661 6c75 653d 2230 2220 7479 7065  n value="0" type
-00003610: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-00003620: 2264 7261 775f 696e 7369 6465 5f70 6f6c  "draw_inside_pol
-00003630: 7967 6f6e 222f 3e0a 2020 2020 2020 2020  ygon"/>.        
-00003640: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003650: 6c75 653d 2262 6576 656c 2220 7479 7065  lue="bevel" type
-00003660: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-00003670: 226a 6f69 6e73 7479 6c65 222f 3e0a 2020  "joinstyle"/>.  
-00003680: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00003690: 696f 6e20 7661 6c75 653d 2233 352c 3335  ion value="35,35
-000036a0: 2c33 352c 3235 3522 2074 7970 653d 2251  ,35,255" type="Q
-000036b0: 5374 7269 6e67 2220 6e61 6d65 3d22 6c69  String" name="li
-000036c0: 6e65 5f63 6f6c 6f72 222f 3e0a 2020 2020  ne_color"/>.    
+000009f0: 6e20 7661 6c75 653d 2232 3332 2c31 3133  n value="232,113
+00000a00: 2c31 3431 2c32 3535 2220 6e61 6d65 3d22  ,141,255" name="
+00000a10: 6c69 6e65 5f63 6f6c 6f72 2220 7479 7065  line_color" type
+00000a20: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00000a30: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00000a40: 2076 616c 7565 3d22 736f 6c69 6422 206e   value="solid" n
+00000a50: 616d 653d 226c 696e 655f 7374 796c 6522  ame="line_style"
+00000a60: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00000a70: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00000a80: 7074 696f 6e20 7661 6c75 653d 2230 2e36  ption value="0.6
+00000a90: 2220 6e61 6d65 3d22 6c69 6e65 5f77 6964  " name="line_wid
+00000aa0: 7468 2220 7479 7065 3d22 5153 7472 696e  th" type="QStrin
+00000ab0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00000ac0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00000ad0: 4d4d 2220 6e61 6d65 3d22 6c69 6e65 5f77  MM" name="line_w
+00000ae0: 6964 7468 5f75 6e69 7422 2074 7970 653d  idth_unit" type=
+00000af0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00000b00: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00000b10: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
+00000b20: 6f66 6673 6574 2220 7479 7065 3d22 5153  offset" type="QS
+00000b30: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00000b40: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00000b50: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+00000b60: 2c30 2220 6e61 6d65 3d22 6f66 6673 6574  ,0" name="offset
+00000b70: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
+00000b80: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00000b90: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00000ba0: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
+00000bb0: 206e 616d 653d 226f 6666 7365 745f 756e   name="offset_un
+00000bc0: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00000bd0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00000be0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00000bf0: 3022 206e 616d 653d 2272 696e 675f 6669  0" name="ring_fi
+00000c00: 6c74 6572 2220 7479 7065 3d22 5153 7472  lter" type="QStr
+00000c10: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00000c20: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00000c30: 3d22 3022 206e 616d 653d 2274 7269 6d5f  ="0" name="trim_
+00000c40: 6469 7374 616e 6365 5f65 6e64 2220 7479  distance_end" ty
+00000c50: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00000c60: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00000c70: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
+00000c80: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
+00000c90: 7472 696d 5f64 6973 7461 6e63 655f 656e  trim_distance_en
+00000ca0: 645f 6d61 705f 756e 6974 5f73 6361 6c65  d_map_unit_scale
+00000cb0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00000cc0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00000cd0: 4f70 7469 6f6e 2076 616c 7565 3d22 4d4d  Option value="MM
+00000ce0: 2220 6e61 6d65 3d22 7472 696d 5f64 6973  " name="trim_dis
+00000cf0: 7461 6e63 655f 656e 645f 756e 6974 2220  tance_end_unit" 
+00000d00: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00000d10: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00000d20: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00000d30: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
+00000d40: 6365 5f73 7461 7274 2220 7479 7065 3d22  ce_start" type="
+00000d50: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00000d60: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00000d70: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00000d80: 2c30 2c30 2220 6e61 6d65 3d22 7472 696d  ,0,0" name="trim
+00000d90: 5f64 6973 7461 6e63 655f 7374 6172 745f  _distance_start_
+00000da0: 6d61 705f 756e 6974 5f73 6361 6c65 2220  map_unit_scale" 
+00000db0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00000dc0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00000dd0: 7469 6f6e 2076 616c 7565 3d22 4d4d 2220  tion value="MM" 
+00000de0: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
+00000df0: 6e63 655f 7374 6172 745f 756e 6974 2220  nce_start_unit" 
+00000e00: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00000e10: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00000e20: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00000e30: 616d 653d 2274 7765 616b 5f64 6173 685f  ame="tweak_dash_
+00000e40: 7061 7474 6572 6e5f 6f6e 5f63 6f72 6e65  pattern_on_corne
+00000e50: 7273 2220 7479 7065 3d22 5153 7472 696e  rs" type="QStrin
+00000e60: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00000e70: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00000e80: 3022 206e 616d 653d 2275 7365 5f63 7573  0" name="use_cus
+00000e90: 746f 6d5f 6461 7368 2220 7479 7065 3d22  tom_dash" type="
+00000ea0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00000eb0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00000ec0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00000ed0: 2c30 2c30 2220 6e61 6d65 3d22 7769 6474  ,0,0" name="widt
+00000ee0: 685f 6d61 705f 756e 6974 5f73 6361 6c65  h_map_unit_scale
+00000ef0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00000f00: 2f3e 0a20 2020 2020 2020 2020 203c 2f4f  />.          </O
+00000f10: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+00000f20: 203c 6461 7461 5f64 6566 696e 6564 5f70   <data_defined_p
+00000f30: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+00000f40: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00000f50: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00000f60: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00000f70: 2076 616c 7565 3d22 2220 6e61 6d65 3d22   value="" name="
+00000f80: 6e61 6d65 2220 7479 7065 3d22 5153 7472  name" type="QStr
+00000f90: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00000fa0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00000fb0: 653d 2270 726f 7065 7274 6965 7322 2f3e  e="properties"/>
+00000fc0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00000fd0: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
+00000fe0: 6c6c 6563 7469 6f6e 2220 6e61 6d65 3d22  llection" name="
+00000ff0: 7479 7065 2220 7479 7065 3d22 5153 7472  type" type="QStr
+00001000: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00001010: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+00001020: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
+00001030: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
+00001040: 3e0a 2020 2020 2020 2020 3c2f 6c61 7965  >.        </laye
+00001050: 723e 0a20 2020 2020 203c 2f73 796d 626f  r>.      </symbo
+00001060: 6c3e 0a20 2020 203c 2f70 726f 6669 6c65  l>.    </profile
+00001070: 4c69 6e65 5379 6d62 6f6c 3e0a 2020 2020  LineSymbol>.    
+00001080: 3c70 726f 6669 6c65 4669 6c6c 5379 6d62  <profileFillSymb
+00001090: 6f6c 3e0a 2020 2020 2020 3c73 796d 626f  ol>.      <symbo
+000010a0: 6c20 6672 616d 655f 7261 7465 3d22 3130  l frame_rate="10
+000010b0: 2220 6e61 6d65 3d22 2220 616c 7068 613d  " name="" alpha=
+000010c0: 2231 2220 6973 5f61 6e69 6d61 7465 643d  "1" is_animated=
+000010d0: 2230 2220 636c 6970 5f74 6f5f 6578 7465  "0" clip_to_exte
+000010e0: 6e74 3d22 3122 2074 7970 653d 2266 696c  nt="1" type="fil
+000010f0: 6c22 2066 6f72 6365 5f72 6872 3d22 3022  l" force_rhr="0"
+00001100: 3e0a 2020 2020 2020 2020 3c64 6174 615f  >.        <data_
+00001110: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
+00001120: 6573 3e0a 2020 2020 2020 2020 2020 3c4f  es>.          <O
+00001130: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
+00001140: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00001150: 7074 696f 6e20 7661 6c75 653d 2222 206e  ption value="" n
+00001160: 616d 653d 226e 616d 6522 2074 7970 653d  ame="name" type=
+00001170: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00001180: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00001190: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
+000011a0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000011b0: 3c4f 7074 696f 6e20 7661 6c75 653d 2263  <Option value="c
+000011c0: 6f6c 6c65 6374 696f 6e22 206e 616d 653d  ollection" name=
+000011d0: 2274 7970 6522 2074 7970 653d 2251 5374  "type" type="QSt
+000011e0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000011f0: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
+00001200: 2020 2020 3c2f 6461 7461 5f64 6566 696e      </data_defin
+00001210: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
+00001220: 2020 2020 2020 203c 6c61 7965 7220 636c         <layer cl
+00001230: 6173 733d 2253 696d 706c 6546 696c 6c22  ass="SimpleFill"
+00001240: 2070 6173 733d 2230 2220 656e 6162 6c65   pass="0" enable
+00001250: 643d 2231 2220 6c6f 636b 6564 3d22 3022  d="1" locked="0"
+00001260: 3e0a 2020 2020 2020 2020 2020 3c4f 7074  >.          <Opt
+00001270: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
+00001280: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00001290: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
+000012a0: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
+000012b0: 2262 6f72 6465 725f 7769 6474 685f 6d61  "border_width_ma
+000012c0: 705f 756e 6974 5f73 6361 6c65 2220 7479  p_unit_scale" ty
+000012d0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000012e0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000012f0: 6f6e 2076 616c 7565 3d22 3233 322c 3131  on value="232,11
+00001300: 332c 3134 312c 3235 3522 206e 616d 653d  3,141,255" name=
+00001310: 2263 6f6c 6f72 2220 7479 7065 3d22 5153  "color" type="QS
+00001320: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00001330: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00001340: 7565 3d22 6265 7665 6c22 206e 616d 653d  ue="bevel" name=
+00001350: 226a 6f69 6e73 7479 6c65 2220 7479 7065  "joinstyle" type
+00001360: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00001370: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00001380: 2076 616c 7565 3d22 302c 3022 206e 616d   value="0,0" nam
+00001390: 653d 226f 6666 7365 7422 2074 7970 653d  e="offset" type=
+000013a0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000013b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000013c0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+000013d0: 302c 302c 3022 206e 616d 653d 226f 6666  0,0,0" name="off
+000013e0: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
+000013f0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00001400: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00001410: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00001420: 4d4d 2220 6e61 6d65 3d22 6f66 6673 6574  MM" name="offset
+00001430: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
+00001440: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00001450: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00001460: 653d 2231 3636 2c38 312c 3130 312c 3235  e="166,81,101,25
+00001470: 3522 206e 616d 653d 226f 7574 6c69 6e65  5" name="outline
+00001480: 5f63 6f6c 6f72 2220 7479 7065 3d22 5153  _color" type="QS
+00001490: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000014a0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000014b0: 7565 3d22 736f 6c69 6422 206e 616d 653d  ue="solid" name=
+000014c0: 226f 7574 6c69 6e65 5f73 7479 6c65 2220  "outline_style" 
+000014d0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000014e0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+000014f0: 7469 6f6e 2076 616c 7565 3d22 302e 3222  tion value="0.2"
+00001500: 206e 616d 653d 226f 7574 6c69 6e65 5f77   name="outline_w
+00001510: 6964 7468 2220 7479 7065 3d22 5153 7472  idth" type="QStr
+00001520: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00001530: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00001540: 3d22 4d4d 2220 6e61 6d65 3d22 6f75 746c  ="MM" name="outl
+00001550: 696e 655f 7769 6474 685f 756e 6974 2220  ine_width_unit" 
+00001560: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00001570: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00001580: 7469 6f6e 2076 616c 7565 3d22 736f 6c69  tion value="soli
+00001590: 6422 206e 616d 653d 2273 7479 6c65 2220  d" name="style" 
+000015a0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000015b0: 0a20 2020 2020 2020 2020 203c 2f4f 7074  .          </Opt
+000015c0: 696f 6e3e 0a20 2020 2020 2020 2020 203c  ion>.          <
+000015d0: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+000015e0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+000015f0: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
+00001600: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00001610: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00001620: 616c 7565 3d22 2220 6e61 6d65 3d22 6e61  alue="" name="na
+00001630: 6d65 2220 7479 7065 3d22 5153 7472 696e  me" type="QStrin
+00001640: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00001650: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00001660: 2270 726f 7065 7274 6965 7322 2f3e 0a20  "properties"/>. 
+00001670: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00001680: 7469 6f6e 2076 616c 7565 3d22 636f 6c6c  tion value="coll
+00001690: 6563 7469 6f6e 2220 6e61 6d65 3d22 7479  ection" name="ty
+000016a0: 7065 2220 7479 7065 3d22 5153 7472 696e  pe" type="QStrin
+000016b0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+000016c0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
+000016d0: 2020 2020 203c 2f64 6174 615f 6465 6669       </data_defi
+000016e0: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
+000016f0: 2020 2020 2020 2020 3c2f 6c61 7965 723e          </layer>
+00001700: 0a20 2020 2020 203c 2f73 796d 626f 6c3e  .      </symbol>
+00001710: 0a20 2020 203c 2f70 726f 6669 6c65 4669  .    </profileFi
+00001720: 6c6c 5379 6d62 6f6c 3e0a 2020 2020 3c70  llSymbol>.    <p
+00001730: 726f 6669 6c65 4d61 726b 6572 5379 6d62  rofileMarkerSymb
+00001740: 6f6c 3e0a 2020 2020 2020 3c73 796d 626f  ol>.      <symbo
+00001750: 6c20 6672 616d 655f 7261 7465 3d22 3130  l frame_rate="10
+00001760: 2220 6e61 6d65 3d22 2220 616c 7068 613d  " name="" alpha=
+00001770: 2231 2220 6973 5f61 6e69 6d61 7465 643d  "1" is_animated=
+00001780: 2230 2220 636c 6970 5f74 6f5f 6578 7465  "0" clip_to_exte
+00001790: 6e74 3d22 3122 2074 7970 653d 226d 6172  nt="1" type="mar
+000017a0: 6b65 7222 2066 6f72 6365 5f72 6872 3d22  ker" force_rhr="
+000017b0: 3022 3e0a 2020 2020 2020 2020 3c64 6174  0">.        <dat
+000017c0: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+000017d0: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
+000017e0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+000017f0: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00001800: 3c4f 7074 696f 6e20 7661 6c75 653d 2222  <Option value=""
+00001810: 206e 616d 653d 226e 616d 6522 2074 7970   name="name" typ
+00001820: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00001830: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00001840: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
+00001850: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
+00001860: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00001870: 2263 6f6c 6c65 6374 696f 6e22 206e 616d  "collection" nam
+00001880: 653d 2274 7970 6522 2074 7970 653d 2251  e="type" type="Q
+00001890: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000018a0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+000018b0: 2020 2020 2020 3c2f 6461 7461 5f64 6566        </data_def
+000018c0: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
+000018d0: 0a20 2020 2020 2020 203c 6c61 7965 7220  .        <layer 
+000018e0: 636c 6173 733d 2253 696d 706c 654d 6172  class="SimpleMar
+000018f0: 6b65 7222 2070 6173 733d 2230 2220 656e  ker" pass="0" en
+00001900: 6162 6c65 643d 2231 2220 6c6f 636b 6564  abled="1" locked
+00001910: 3d22 3022 3e0a 2020 2020 2020 2020 2020  ="0">.          
+00001920: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00001930: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00001940: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00001950: 2220 6e61 6d65 3d22 616e 676c 6522 2074  " name="angle" t
+00001960: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00001970: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00001980: 696f 6e20 7661 6c75 653d 2273 7175 6172  ion value="squar
+00001990: 6522 206e 616d 653d 2263 6170 5f73 7479  e" name="cap_sty
+000019a0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+000019b0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+000019c0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000019d0: 3233 322c 3131 332c 3134 312c 3235 3522  232,113,141,255"
+000019e0: 206e 616d 653d 2263 6f6c 6f72 2220 7479   name="color" ty
+000019f0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00001a00: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00001a10: 6f6e 2076 616c 7565 3d22 3122 206e 616d  on value="1" nam
+00001a20: 653d 2268 6f72 697a 6f6e 7461 6c5f 616e  e="horizontal_an
+00001a30: 6368 6f72 5f70 6f69 6e74 2220 7479 7065  chor_point" type
+00001a40: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00001a50: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00001a60: 2076 616c 7565 3d22 6265 7665 6c22 206e   value="bevel" n
+00001a70: 616d 653d 226a 6f69 6e73 7479 6c65 2220  ame="joinstyle" 
+00001a80: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00001a90: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00001aa0: 7469 6f6e 2076 616c 7565 3d22 6469 616d  tion value="diam
+00001ab0: 6f6e 6422 206e 616d 653d 226e 616d 6522  ond" name="name"
+00001ac0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00001ad0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00001ae0: 7074 696f 6e20 7661 6c75 653d 2230 2c30  ption value="0,0
+00001af0: 2220 6e61 6d65 3d22 6f66 6673 6574 2220  " name="offset" 
+00001b00: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00001b10: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00001b20: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
+00001b30: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
+00001b40: 3d22 6f66 6673 6574 5f6d 6170 5f75 6e69  ="offset_map_uni
+00001b50: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
+00001b60: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00001b70: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00001b80: 6c75 653d 224d 4d22 206e 616d 653d 226f  lue="MM" name="o
+00001b90: 6666 7365 745f 756e 6974 2220 7479 7065  ffset_unit" type
+00001ba0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00001bb0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00001bc0: 2076 616c 7565 3d22 3136 362c 3831 2c31   value="166,81,1
+00001bd0: 3031 2c32 3535 2220 6e61 6d65 3d22 6f75  01,255" name="ou
+00001be0: 746c 696e 655f 636f 6c6f 7222 2074 7970  tline_color" typ
+00001bf0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00001c00: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00001c10: 6e20 7661 6c75 653d 2273 6f6c 6964 2220  n value="solid" 
+00001c20: 6e61 6d65 3d22 6f75 746c 696e 655f 7374  name="outline_st
+00001c30: 796c 6522 2074 7970 653d 2251 5374 7269  yle" type="QStri
+00001c40: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00001c50: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00001c60: 2230 2e32 2220 6e61 6d65 3d22 6f75 746c  "0.2" name="outl
+00001c70: 696e 655f 7769 6474 6822 2074 7970 653d  ine_width" type=
+00001c80: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00001c90: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00001ca0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+00001cb0: 302c 302c 3022 206e 616d 653d 226f 7574  0,0,0" name="out
+00001cc0: 6c69 6e65 5f77 6964 7468 5f6d 6170 5f75  line_width_map_u
+00001cd0: 6e69 745f 7363 616c 6522 2074 7970 653d  nit_scale" type=
+00001ce0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00001cf0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00001d00: 7661 6c75 653d 224d 4d22 206e 616d 653d  value="MM" name=
+00001d10: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
+00001d20: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00001d30: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00001d40: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00001d50: 2264 6961 6d65 7465 7222 206e 616d 653d  "diameter" name=
+00001d60: 2273 6361 6c65 5f6d 6574 686f 6422 2074  "scale_method" t
+00001d70: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00001d80: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00001d90: 696f 6e20 7661 6c75 653d 2233 2220 6e61  ion value="3" na
+00001da0: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
+00001db0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00001dc0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00001dd0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00001de0: 2c30 2c30 2220 6e61 6d65 3d22 7369 7a65  ,0,0" name="size
+00001df0: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
+00001e00: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00001e10: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00001e20: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
+00001e30: 206e 616d 653d 2273 697a 655f 756e 6974   name="size_unit
+00001e40: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00001e50: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00001e60: 4f70 7469 6f6e 2076 616c 7565 3d22 3122  Option value="1"
+00001e70: 206e 616d 653d 2276 6572 7469 6361 6c5f   name="vertical_
+00001e80: 616e 6368 6f72 5f70 6f69 6e74 2220 7479  anchor_point" ty
+00001e90: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00001ea0: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00001eb0: 6e3e 0a20 2020 2020 2020 2020 203c 6461  n>.          <da
+00001ec0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+00001ed0: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+00001ee0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+00001ef0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00001f00: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00001f10: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
+00001f20: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00001f30: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00001f40: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00001f50: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
+00001f60: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00001f70: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
+00001f80: 7469 6f6e 2220 6e61 6d65 3d22 7479 7065  tion" name="type
+00001f90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00001fa0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00001fb0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00001fc0: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
+00001fd0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
+00001fe0: 2020 2020 2020 3c2f 6c61 7965 723e 0a20        </layer>. 
+00001ff0: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
+00002000: 2020 203c 2f70 726f 6669 6c65 4d61 726b     </profileMark
+00002010: 6572 5379 6d62 6f6c 3e0a 2020 3c2f 656c  erSymbol>.  </el
+00002020: 6576 6174 696f 6e3e 0a20 203c 7265 6e64  evation>.  <rend
+00002030: 6572 6572 2d76 3220 7265 6665 7265 6e63  erer-v2 referenc
+00002040: 6573 6361 6c65 3d22 2d31 2220 656e 6162  escale="-1" enab
+00002050: 6c65 6f72 6465 7262 793d 2230 2220 7379  leorderby="0" sy
+00002060: 6d62 6f6c 6c65 7665 6c73 3d22 3022 2066  mbollevels="0" f
+00002070: 6f72 6365 7261 7374 6572 3d22 3022 2074  orceraster="0" t
+00002080: 7970 653d 2252 756c 6552 656e 6465 7265  ype="RuleRendere
+00002090: 7222 3e0a 2020 2020 3c72 756c 6573 206b  r">.    <rules k
+000020a0: 6579 3d22 7b31 6163 6338 3136 392d 3632  ey="{1acc8169-62
+000020b0: 3230 2d34 6161 352d 6264 3661 2d38 3831  20-4aa5-bd6a-881
+000020c0: 3739 6264 6466 6666 637d 223e 0a20 2020  79bddfffc}">.   
+000020d0: 2020 203c 7275 6c65 206b 6579 3d22 7b64     <rule key="{d
+000020e0: 6363 6433 6162 312d 6335 6363 2d34 6665  ccd3ab1-c5cc-4fe
+000020f0: 372d 6136 3735 2d37 3638 3937 3931 6631  7-a675-7689791f1
+00002100: 6135 347d 2220 7379 6d62 6f6c 3d22 3022  a54}" symbol="0"
+00002110: 2f3e 0a20 2020 203c 2f72 756c 6573 3e0a  />.    </rules>.
+00002120: 2020 2020 3c73 796d 626f 6c73 3e0a 2020      <symbols>.  
+00002130: 2020 2020 3c73 796d 626f 6c20 6672 616d      <symbol fram
+00002140: 655f 7261 7465 3d22 3130 2220 6e61 6d65  e_rate="10" name
+00002150: 3d22 3022 2061 6c70 6861 3d22 3122 2069  ="0" alpha="1" i
+00002160: 735f 616e 696d 6174 6564 3d22 3022 2063  s_animated="0" c
+00002170: 6c69 705f 746f 5f65 7874 656e 743d 2231  lip_to_extent="1
+00002180: 2220 7479 7065 3d22 6d61 726b 6572 2220  " type="marker" 
+00002190: 666f 7263 655f 7268 723d 2230 223e 0a20  force_rhr="0">. 
+000021a0: 2020 2020 2020 203c 6461 7461 5f64 6566         <data_def
+000021b0: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
+000021c0: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
+000021d0: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
+000021e0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000021f0: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
+00002200: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
+00002210: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002220: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00002230: 653d 2270 726f 7065 7274 6965 7322 2f3e  e="properties"/>
+00002240: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00002250: 7469 6f6e 2076 616c 7565 3d22 636f 6c6c  tion value="coll
+00002260: 6563 7469 6f6e 2220 6e61 6d65 3d22 7479  ection" name="ty
+00002270: 7065 2220 7479 7065 3d22 5153 7472 696e  pe" type="QStrin
+00002280: 6722 2f3e 0a20 2020 2020 2020 2020 203c  g"/>.          <
+00002290: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+000022a0: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
+000022b0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
+000022c0: 2020 2020 3c6c 6179 6572 2063 6c61 7373      <layer class
+000022d0: 3d22 5369 6d70 6c65 4d61 726b 6572 2220  ="SimpleMarker" 
+000022e0: 7061 7373 3d22 3022 2065 6e61 626c 6564  pass="0" enabled
+000022f0: 3d22 3122 206c 6f63 6b65 643d 2230 223e  ="1" locked="0">
+00002300: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
+00002310: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
+00002320: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002330: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
+00002340: 653d 2261 6e67 6c65 2220 7479 7065 3d22  e="angle" type="
+00002350: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00002360: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00002370: 616c 7565 3d22 666c 6174 2220 6e61 6d65  alue="flat" name
+00002380: 3d22 6361 705f 7374 796c 6522 2074 7970  ="cap_style" typ
+00002390: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000023a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000023b0: 6e20 7661 6c75 653d 2231 3435 2c38 322c  n value="145,82,
+000023c0: 3435 2c32 3535 2220 6e61 6d65 3d22 636f  45,255" name="co
+000023d0: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
+000023e0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000023f0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00002400: 2231 2220 6e61 6d65 3d22 686f 7269 7a6f  "1" name="horizo
+00002410: 6e74 616c 5f61 6e63 686f 725f 706f 696e  ntal_anchor_poin
+00002420: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00002430: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00002440: 3c4f 7074 696f 6e20 7661 6c75 653d 226d  <Option value="m
+00002450: 6974 6572 2220 6e61 6d65 3d22 6a6f 696e  iter" name="join
+00002460: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
+00002470: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00002480: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00002490: 653d 226c 696e 6522 206e 616d 653d 226e  e="line" name="n
+000024a0: 616d 6522 2074 7970 653d 2251 5374 7269  ame" type="QStri
+000024b0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000024c0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000024d0: 2230 2c30 2220 6e61 6d65 3d22 6f66 6673  "0,0" name="offs
+000024e0: 6574 2220 7479 7065 3d22 5153 7472 696e  et" type="QStrin
+000024f0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00002500: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00002510: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
+00002520: 6e61 6d65 3d22 6f66 6673 6574 5f6d 6170  name="offset_map
+00002530: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
+00002540: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002550: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002560: 6e20 7661 6c75 653d 224d 4d22 206e 616d  n value="MM" nam
+00002570: 653d 226f 6666 7365 745f 756e 6974 2220  e="offset_unit" 
+00002580: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00002590: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+000025a0: 7469 6f6e 2076 616c 7565 3d22 3235 352c  tion value="255,
+000025b0: 3235 352c 3235 352c 3235 3522 206e 616d  255,255,255" nam
+000025c0: 653d 226f 7574 6c69 6e65 5f63 6f6c 6f72  e="outline_color
+000025d0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000025e0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+000025f0: 4f70 7469 6f6e 2076 616c 7565 3d22 736f  Option value="so
+00002600: 6c69 6422 206e 616d 653d 226f 7574 6c69  lid" name="outli
+00002610: 6e65 5f73 7479 6c65 2220 7479 7065 3d22  ne_style" type="
+00002620: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00002630: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00002640: 616c 7565 3d22 3222 206e 616d 653d 226f  alue="2" name="o
+00002650: 7574 6c69 6e65 5f77 6964 7468 2220 7479  utline_width" ty
+00002660: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00002670: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002680: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
+00002690: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
+000026a0: 6f75 746c 696e 655f 7769 6474 685f 6d61  outline_width_ma
+000026b0: 705f 756e 6974 5f73 6361 6c65 2220 7479  p_unit_scale" ty
+000026c0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000026d0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000026e0: 6f6e 2076 616c 7565 3d22 5265 6e64 6572  on value="Render
+000026f0: 4d65 7465 7273 496e 4d61 7055 6e69 7473  MetersInMapUnits
+00002700: 2220 6e61 6d65 3d22 6f75 746c 696e 655f  " name="outline_
+00002710: 7769 6474 685f 756e 6974 2220 7479 7065  width_unit" type
+00002720: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002730: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002740: 2076 616c 7565 3d22 6469 616d 6574 6572   value="diameter
+00002750: 2220 6e61 6d65 3d22 7363 616c 655f 6d65  " name="scale_me
+00002760: 7468 6f64 2220 7479 7065 3d22 5153 7472  thod" type="QStr
+00002770: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00002780: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00002790: 3d22 3322 206e 616d 653d 2273 697a 6522  ="3" name="size"
+000027a0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000027b0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000027c0: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
+000027d0: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
+000027e0: 653d 2273 697a 655f 6d61 705f 756e 6974  e="size_map_unit
+000027f0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
+00002800: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002810: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00002820: 7565 3d22 5265 6e64 6572 4d65 7465 7273  ue="RenderMeters
+00002830: 496e 4d61 7055 6e69 7473 2220 6e61 6d65  InMapUnits" name
+00002840: 3d22 7369 7a65 5f75 6e69 7422 2074 7970  ="size_unit" typ
+00002850: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002860: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002870: 6e20 7661 6c75 653d 2231 2220 6e61 6d65  n value="1" name
+00002880: 3d22 7665 7274 6963 616c 5f61 6e63 686f  ="vertical_ancho
+00002890: 725f 706f 696e 7422 2074 7970 653d 2251  r_point" type="Q
+000028a0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000028b0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+000028c0: 2020 2020 2020 2020 3c64 6174 615f 6465          <data_de
+000028d0: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
+000028e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000028f0: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
+00002900: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002910: 3c4f 7074 696f 6e20 7661 6c75 653d 2222  <Option value=""
+00002920: 206e 616d 653d 226e 616d 6522 2074 7970   name="name" typ
+00002930: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002940: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00002950: 696f 6e20 6e61 6d65 3d22 7072 6f70 6572  ion name="proper
+00002960: 7469 6573 2220 7479 7065 3d22 4d61 7022  ties" type="Map"
+00002970: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002980: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00002990: 616e 676c 6522 2074 7970 653d 224d 6170  angle" type="Map
+000029a0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000029b0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000029c0: 7565 3d22 7472 7565 2220 6e61 6d65 3d22  ue="true" name="
+000029d0: 6163 7469 7665 2220 7479 7065 3d22 626f  active" type="bo
+000029e0: 6f6c 222f 3e0a 2020 2020 2020 2020 2020  ol"/>.          
+000029f0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00002a00: 7661 6c75 653d 2231 3830 202b 2028 2d26  value="180 + (-&
+00002a10: 7175 6f74 3b6f 7269 656e 7461 7469 6f6e  quot;orientation
+00002a20: 2671 756f 743b 202f 2070 6928 2929 202a  &quot; / pi()) *
+00002a30: 2031 3830 2220 6e61 6d65 3d22 6578 7072   180" name="expr
+00002a40: 6573 7369 6f6e 2220 7479 7065 3d22 5153  ession" type="QS
+00002a50: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002a60: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002a70: 6f6e 2076 616c 7565 3d22 3322 206e 616d  on value="3" nam
+00002a80: 653d 2274 7970 6522 2074 7970 653d 2269  e="type" type="i
+00002a90: 6e74 222f 3e0a 2020 2020 2020 2020 2020  nt"/>.          
+00002aa0: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ac0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
+00002ad0: 746c 696e 6557 6964 7468 2220 7479 7065  tlineWidth" type
+00002ae0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00002af0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002b00: 6e20 7661 6c75 653d 2274 7275 6522 206e  n value="true" n
+00002b10: 616d 653d 2261 6374 6976 6522 2074 7970  ame="active" typ
+00002b20: 653d 2262 6f6f 6c22 2f3e 0a20 2020 2020  e="bool"/>.     
+00002b30: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00002b40: 7469 6f6e 2076 616c 7565 3d22 2671 756f  tion value="&quo
+00002b50: 743b 6c61 6e65 5f77 6964 7468 2671 756f  t;lane_width&quo
+00002b60: 743b 202a 2031 2e33 2220 6e61 6d65 3d22  t; * 1.3" name="
+00002b70: 6578 7072 6573 7369 6f6e 2220 7479 7065  expression" type
+00002b80: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002b90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00002ba0: 4f70 7469 6f6e 2076 616c 7565 3d22 3322  Option value="3"
+00002bb0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
+00002bc0: 653d 2269 6e74 222f 3e0a 2020 2020 2020  e="int"/>.      
+00002bd0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00002be0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+00002bf0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00002c00: 3d22 7369 7a65 2220 7479 7065 3d22 4d61  ="size" type="Ma
+00002c10: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00002c20: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00002c30: 6c75 653d 2274 7275 6522 206e 616d 653d  lue="true" name=
+00002c40: 2261 6374 6976 6522 2074 7970 653d 2262  "active" type="b
+00002c50: 6f6f 6c22 2f3e 0a20 2020 2020 2020 2020  ool"/>.         
+00002c60: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002c70: 2076 616c 7565 3d22 3320 2b20 3220 2a20   value="3 + 2 * 
+00002c80: 302e 3030 3220 2a20 2040 6d61 705f 7363  0.002 *  @map_sc
+00002c90: 616c 6522 206e 616d 653d 2265 7870 7265  ale" name="expre
+00002ca0: 7373 696f 6e22 2074 7970 653d 2251 5374  ssion" type="QSt
+00002cb0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00002cc0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002cd0: 6e20 7661 6c75 653d 2233 2220 6e61 6d65  n value="3" name
+00002ce0: 3d22 7479 7065 2220 7479 7065 3d22 696e  ="type" type="in
+00002cf0: 7422 2f3e 0a20 2020 2020 2020 2020 2020  t"/>.           
+00002d00: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00002d10: 2020 2020 2020 2020 2020 2020 203c 2f4f               </O
+00002d20: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+00002d30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00002d40: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
+00002d50: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
+00002d60: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002d70: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00002d80: 6e3e 0a20 2020 2020 2020 2020 203c 2f64  n>.          </d
+00002d90: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+00002da0: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+00002db0: 3c2f 6c61 7965 723e 0a20 2020 2020 203c  </layer>.      <
+00002dc0: 2f73 796d 626f 6c3e 0a20 2020 203c 2f73  /symbol>.    </s
+00002dd0: 796d 626f 6c73 3e0a 2020 3c2f 7265 6e64  ymbols>.  </rend
+00002de0: 6572 6572 2d76 323e 0a20 203c 6375 7374  erer-v2>.  <cust
+00002df0: 6f6d 7072 6f70 6572 7469 6573 3e0a 2020  omproperties>.  
+00002e00: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
+00002e10: 4d61 7022 3e0a 2020 2020 2020 3c4f 7074  Map">.      <Opt
+00002e20: 696f 6e20 6e61 6d65 3d22 6475 616c 7669  ion name="dualvi
+00002e30: 6577 2f70 7265 7669 6577 4578 7072 6573  ew/previewExpres
+00002e40: 7369 6f6e 7322 2074 7970 653d 224c 6973  sions" type="Lis
+00002e50: 7422 3e0a 2020 2020 2020 2020 3c4f 7074  t">.        <Opt
+00002e60: 696f 6e20 7661 6c75 653d 2226 7175 6f74  ion value="&quot
+00002e70: 3b74 7970 6526 7175 6f74 3b22 2074 7970  ;type&quot;" typ
+00002e80: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002e90: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00002ea0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00002eb0: 653d 2230 2220 6e61 6d65 3d22 656d 6265  e="0" name="embe
+00002ec0: 6464 6564 5769 6467 6574 732f 636f 756e  ddedWidgets/coun
+00002ed0: 7422 2074 7970 653d 2269 6e74 222f 3e0a  t" type="int"/>.
+00002ee0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00002ef0: 6d65 3d22 7661 7269 6162 6c65 4e61 6d65  me="variableName
+00002f00: 7322 2f3e 0a20 2020 2020 203c 4f70 7469  s"/>.      <Opti
+00002f10: 6f6e 206e 616d 653d 2276 6172 6961 626c  on name="variabl
+00002f20: 6556 616c 7565 7322 2f3e 0a20 2020 203c  eValues"/>.    <
+00002f30: 2f4f 7074 696f 6e3e 0a20 203c 2f63 7573  /Option>.  </cus
+00002f40: 746f 6d70 726f 7065 7274 6965 733e 0a20  tomproperties>. 
+00002f50: 203c 626c 656e 644d 6f64 653e 303c 2f62   <blendMode>0</b
+00002f60: 6c65 6e64 4d6f 6465 3e0a 2020 3c66 6561  lendMode>.  <fea
+00002f70: 7475 7265 426c 656e 644d 6f64 653e 303c  tureBlendMode>0<
+00002f80: 2f66 6561 7475 7265 426c 656e 644d 6f64  /featureBlendMod
+00002f90: 653e 0a20 203c 6c61 7965 724f 7061 6369  e>.  <layerOpaci
+00002fa0: 7479 3e31 3c2f 6c61 7965 724f 7061 6369  ty>1</layerOpaci
+00002fb0: 7479 3e0a 2020 3c53 696e 676c 6543 6174  ty>.  <SingleCat
+00002fc0: 6567 6f72 7944 6961 6772 616d 5265 6e64  egoryDiagramRend
+00002fd0: 6572 6572 2064 6961 6772 616d 5479 7065  erer diagramType
+00002fe0: 3d22 4869 7374 6f67 7261 6d22 2061 7474  ="Histogram" att
+00002ff0: 7269 6275 7465 4c65 6765 6e64 3d22 3122  ributeLegend="1"
+00003000: 3e0a 2020 2020 3c44 6961 6772 616d 4361  >.    <DiagramCa
+00003010: 7465 676f 7279 2070 656e 436f 6c6f 723d  tegory penColor=
+00003020: 2223 3030 3030 3030 2220 7065 6e57 6964  "#000000" penWid
+00003030: 7468 3d22 3022 2077 6964 7468 3d22 3135  th="0" width="15
+00003040: 2220 7369 7a65 5479 7065 3d22 4d4d 2220  " sizeType="MM" 
+00003050: 6469 7265 6374 696f 6e3d 2230 2220 6c61  direction="0" la
+00003060: 6265 6c50 6c61 6365 6d65 6e74 4d65 7468  belPlacementMeth
+00003070: 6f64 3d22 5848 6569 6768 7422 2065 6e61  od="XHeight" ena
+00003080: 626c 6564 3d22 3022 2062 6172 5769 6474  bled="0" barWidt
+00003090: 683d 2235 2220 6d61 7853 6361 6c65 4465  h="5" maxScaleDe
+000030a0: 6e6f 6d69 6e61 746f 723d 2231 652b 3038  nominator="1e+08
+000030b0: 2220 7370 6163 696e 6755 6e69 7453 6361  " spacingUnitSca
+000030c0: 6c65 3d22 3378 3a30 2c30 2c30 2c30 2c30  le="3x:0,0,0,0,0
+000030d0: 2c30 2220 6f70 6163 6974 793d 2231 2220  ,0" opacity="1" 
+000030e0: 7363 616c 6544 6570 656e 6465 6e63 793d  scaleDependency=
+000030f0: 2241 7265 6122 2062 6163 6b67 726f 756e  "Area" backgroun
+00003100: 6441 6c70 6861 3d22 3235 3522 206d 696e  dAlpha="255" min
+00003110: 5363 616c 6544 656e 6f6d 696e 6174 6f72  ScaleDenominator
+00003120: 3d22 3022 2073 7061 6369 6e67 556e 6974  ="0" spacingUnit
+00003130: 3d22 4d4d 2220 6d69 6e69 6d75 6d53 697a  ="MM" minimumSiz
+00003140: 653d 2230 2220 6261 636b 6772 6f75 6e64  e="0" background
+00003150: 436f 6c6f 723d 2223 6666 6666 6666 2220  Color="#ffffff" 
+00003160: 6c69 6e65 5369 7a65 5479 7065 3d22 4d4d  lineSizeType="MM
+00003170: 2220 6c69 6e65 5369 7a65 5363 616c 653d  " lineSizeScale=
+00003180: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
+00003190: 2073 697a 6553 6361 6c65 3d22 3378 3a30   sizeScale="3x:0
+000031a0: 2c30 2c30 2c30 2c30 2c30 2220 7363 616c  ,0,0,0,0,0" scal
+000031b0: 6542 6173 6564 5669 7369 6269 6c69 7479  eBasedVisibility
+000031c0: 3d22 3022 2073 7061 6369 6e67 3d22 3522  ="0" spacing="5"
+000031d0: 2072 6f74 6174 696f 6e4f 6666 7365 743d   rotationOffset=
+000031e0: 2232 3730 2220 6865 6967 6874 3d22 3135  "270" height="15
+000031f0: 2220 7368 6f77 4178 6973 3d22 3122 2064  " showAxis="1" d
+00003200: 6961 6772 616d 4f72 6965 6e74 6174 696f  iagramOrientatio
+00003210: 6e3d 2255 7022 2070 656e 416c 7068 613d  n="Up" penAlpha=
+00003220: 2232 3535 223e 0a20 2020 2020 203c 666f  "255">.      <fo
+00003230: 6e74 5072 6f70 6572 7469 6573 2062 6f6c  ntProperties bol
+00003240: 643d 2230 2220 7374 7269 6b65 7468 726f  d="0" strikethro
+00003250: 7567 683d 2230 2220 7374 796c 653d 2222  ugh="0" style=""
+00003260: 2075 6e64 6572 6c69 6e65 3d22 3022 2064   underline="0" d
+00003270: 6573 6372 6970 7469 6f6e 3d22 4e6f 746f  escription="Noto
+00003280: 2053 616e 732c 3130 2c2d 312c 302c 3530   Sans,10,-1,0,50
+00003290: 2c30 2c30 2c30 2c30 2c30 2220 6974 616c  ,0,0,0,0,0" ital
+000032a0: 6963 3d22 3022 2f3e 0a20 2020 2020 203c  ic="0"/>.      <
+000032b0: 6174 7472 6962 7574 6520 636f 6c6f 724f  attribute colorO
+000032c0: 7061 6369 7479 3d22 3122 2063 6f6c 6f72  pacity="1" color
+000032d0: 3d22 2330 3030 3030 3022 2066 6965 6c64  ="#000000" field
+000032e0: 3d22 2220 6c61 6265 6c3d 2222 2f3e 0a20  ="" label=""/>. 
+000032f0: 2020 2020 203c 6178 6973 5379 6d62 6f6c       <axisSymbol
+00003300: 3e0a 2020 2020 2020 2020 3c73 796d 626f  >.        <symbo
+00003310: 6c20 6672 616d 655f 7261 7465 3d22 3130  l frame_rate="10
+00003320: 2220 6e61 6d65 3d22 2220 616c 7068 613d  " name="" alpha=
+00003330: 2231 2220 6973 5f61 6e69 6d61 7465 643d  "1" is_animated=
+00003340: 2230 2220 636c 6970 5f74 6f5f 6578 7465  "0" clip_to_exte
+00003350: 6e74 3d22 3122 2074 7970 653d 226c 696e  nt="1" type="lin
+00003360: 6522 2066 6f72 6365 5f72 6872 3d22 3022  e" force_rhr="0"
+00003370: 3e0a 2020 2020 2020 2020 2020 3c64 6174  >.          <dat
+00003380: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+00003390: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
+000033a0: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
+000033b0: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+000033c0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+000033d0: 653d 2222 206e 616d 653d 226e 616d 6522  e="" name="name"
+000033e0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000033f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003400: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7072  <Option name="pr
+00003410: 6f70 6572 7469 6573 222f 3e0a 2020 2020  operties"/>.    
+00003420: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003430: 6e20 7661 6c75 653d 2263 6f6c 6c65 6374  n value="collect
+00003440: 696f 6e22 206e 616d 653d 2274 7970 6522  ion" name="type"
+00003450: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003460: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00003470: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00003480: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
+00003490: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
+000034a0: 2020 2020 2020 203c 6c61 7965 7220 636c         <layer cl
+000034b0: 6173 733d 2253 696d 706c 654c 696e 6522  ass="SimpleLine"
+000034c0: 2070 6173 733d 2230 2220 656e 6162 6c65   pass="0" enable
+000034d0: 643d 2231 2220 6c6f 636b 6564 3d22 3022  d="1" locked="0"
+000034e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000034f0: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
+00003500: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00003510: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00003520: 2220 6e61 6d65 3d22 616c 6967 6e5f 6461  " name="align_da
+00003530: 7368 5f70 6174 7465 726e 2220 7479 7065  sh_pattern" type
+00003540: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003550: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003560: 6f6e 2076 616c 7565 3d22 7371 7561 7265  on value="square
+00003570: 2220 6e61 6d65 3d22 6361 7073 7479 6c65  " name="capstyle
+00003580: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003590: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000035a0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000035b0: 353b 3222 206e 616d 653d 2263 7573 746f  5;2" name="custo
+000035c0: 6d64 6173 6822 2074 7970 653d 2251 5374  mdash" type="QSt
+000035d0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000035e0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000035f0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
+00003600: 302c 3022 206e 616d 653d 2263 7573 746f  0,0" name="custo
+00003610: 6d64 6173 685f 6d61 705f 756e 6974 5f73  mdash_map_unit_s
+00003620: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
+00003630: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003640: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00003650: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6375  ue="MM" name="cu
+00003660: 7374 6f6d 6461 7368 5f75 6e69 7422 2074  stomdash_unit" t
+00003670: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003680: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003690: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
+000036a0: 6e61 6d65 3d22 6461 7368 5f70 6174 7465  name="dash_patte
+000036b0: 726e 5f6f 6666 7365 7422 2074 7970 653d  rn_offset" type=
+000036c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
 000036d0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000036e0: 6e20 7661 6c75 653d 2273 6f6c 6964 2220  n value="solid" 
-000036f0: 7479 7065 3d22 5153 7472 696e 6722 206e  type="QString" n
-00003700: 616d 653d 226c 696e 655f 7374 796c 6522  ame="line_style"
-00003710: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003720: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003730: 302e 3236 2220 7479 7065 3d22 5153 7472  0.26" type="QStr
-00003740: 696e 6722 206e 616d 653d 226c 696e 655f  ing" name="line_
-00003750: 7769 6474 6822 2f3e 0a20 2020 2020 2020  width"/>.       
-00003760: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003770: 616c 7565 3d22 4d4d 2220 7479 7065 3d22  alue="MM" type="
-00003780: 5153 7472 696e 6722 206e 616d 653d 226c  QString" name="l
-00003790: 696e 655f 7769 6474 685f 756e 6974 222f  ine_width_unit"/
-000037a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000037b0: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
-000037c0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000037d0: 206e 616d 653d 226f 6666 7365 7422 2f3e   name="offset"/>
-000037e0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-000037f0: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-00003800: 3a30 2c30 2c30 2c30 2c30 2c30 2220 7479  :0,0,0,0,0,0" ty
-00003810: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00003820: 653d 226f 6666 7365 745f 6d61 705f 756e  e="offset_map_un
-00003830: 6974 5f73 6361 6c65 222f 3e0a 2020 2020  it_scale"/>.    
-00003840: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003850: 6e20 7661 6c75 653d 224d 4d22 2074 7970  n value="MM" typ
-00003860: 653d 2251 5374 7269 6e67 2220 6e61 6d65  e="QString" name
-00003870: 3d22 6f66 6673 6574 5f75 6e69 7422 2f3e  ="offset_unit"/>
-00003880: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003890: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
-000038a0: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-000038b0: 6e61 6d65 3d22 7269 6e67 5f66 696c 7465  name="ring_filte
-000038c0: 7222 2f3e 0a20 2020 2020 2020 2020 2020  r"/>.           
-000038d0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000038e0: 3d22 3022 2074 7970 653d 2251 5374 7269  ="0" type="QStri
-000038f0: 6e67 2220 6e61 6d65 3d22 7472 696d 5f64  ng" name="trim_d
-00003900: 6973 7461 6e63 655f 656e 6422 2f3e 0a20  istance_end"/>. 
-00003910: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00003920: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
-00003930: 2c30 2c30 2c30 2c30 2c30 2220 7479 7065  ,0,0,0,0,0" type
-00003940: 3d22 5153 7472 696e 6722 206e 616d 653d  ="QString" name=
-00003950: 2274 7269 6d5f 6469 7374 616e 6365 5f65  "trim_distance_e
-00003960: 6e64 5f6d 6170 5f75 6e69 745f 7363 616c  nd_map_unit_scal
-00003970: 6522 2f3e 0a20 2020 2020 2020 2020 2020  e"/>.           
-00003980: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00003990: 3d22 4d4d 2220 7479 7065 3d22 5153 7472  ="MM" type="QStr
-000039a0: 696e 6722 206e 616d 653d 2274 7269 6d5f  ing" name="trim_
-000039b0: 6469 7374 616e 6365 5f65 6e64 5f75 6e69  distance_end_uni
-000039c0: 7422 2f3e 0a20 2020 2020 2020 2020 2020  t"/>.           
-000039d0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000039e0: 3d22 3022 2074 7970 653d 2251 5374 7269  ="0" type="QStri
-000039f0: 6e67 2220 6e61 6d65 3d22 7472 696d 5f64  ng" name="trim_d
-00003a00: 6973 7461 6e63 655f 7374 6172 7422 2f3e  istance_start"/>
-00003a10: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003a20: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-00003a30: 3a30 2c30 2c30 2c30 2c30 2c30 2220 7479  :0,0,0,0,0,0" ty
-00003a40: 7065 3d22 5153 7472 696e 6722 206e 616d  pe="QString" nam
-00003a50: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
-00003a60: 5f73 7461 7274 5f6d 6170 5f75 6e69 745f  _start_map_unit_
-00003a70: 7363 616c 6522 2f3e 0a20 2020 2020 2020  scale"/>.       
-00003a80: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003a90: 616c 7565 3d22 4d4d 2220 7479 7065 3d22  alue="MM" type="
-00003aa0: 5153 7472 696e 6722 206e 616d 653d 2274  QString" name="t
-00003ab0: 7269 6d5f 6469 7374 616e 6365 5f73 7461  rim_distance_sta
-00003ac0: 7274 5f75 6e69 7422 2f3e 0a20 2020 2020  rt_unit"/>.     
-00003ad0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003ae0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
-00003af0: 2251 5374 7269 6e67 2220 6e61 6d65 3d22  "QString" name="
-00003b00: 7477 6561 6b5f 6461 7368 5f70 6174 7465  tweak_dash_patte
-00003b10: 726e 5f6f 6e5f 636f 726e 6572 7322 2f3e  rn_on_corners"/>
-00003b20: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003b30: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
-00003b40: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-00003b50: 6e61 6d65 3d22 7573 655f 6375 7374 6f6d  name="use_custom
-00003b60: 5f64 6173 6822 2f3e 0a20 2020 2020 2020  _dash"/>.       
-00003b70: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003b80: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-00003b90: 2c30 2c30 2220 7479 7065 3d22 5153 7472  ,0,0" type="QStr
-00003ba0: 696e 6722 206e 616d 653d 2277 6964 7468  ing" name="width
-00003bb0: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
-00003bc0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003bd0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00003be0: 2020 2020 203c 6461 7461 5f64 6566 696e       <data_defin
-00003bf0: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
-00003c00: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00003c10: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
-00003c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c30: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003c40: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003c50: 206e 616d 653d 226e 616d 6522 2f3e 0a20   name="name"/>. 
-00003c60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00003c70: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
-00003c80: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
-00003c90: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003ca0: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
-00003cb0: 7469 6f6e 2220 7479 7065 3d22 5153 7472  tion" type="QStr
-00003cc0: 696e 6722 206e 616d 653d 2274 7970 6522  ing" name="type"
-00003cd0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003ce0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
-00003cf0: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
-00003d00: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
-00003d10: 3e0a 2020 2020 2020 2020 2020 3c2f 6c61  >.          </la
-00003d20: 7965 723e 0a20 2020 2020 2020 203c 2f73  yer>.        </s
-00003d30: 796d 626f 6c3e 0a20 2020 2020 203c 2f61  ymbol>.      </a
-00003d40: 7869 7353 796d 626f 6c3e 0a20 2020 203c  xisSymbol>.    <
-00003d50: 2f44 6961 6772 616d 4361 7465 676f 7279  /DiagramCategory
-00003d60: 3e0a 2020 3c2f 5369 6e67 6c65 4361 7465  >.  </SingleCate
-00003d70: 676f 7279 4469 6167 7261 6d52 656e 6465  goryDiagramRende
-00003d80: 7265 723e 0a20 203c 4469 6167 7261 6d4c  rer>.  <DiagramL
-00003d90: 6179 6572 5365 7474 696e 6773 2064 6973  ayerSettings dis
-00003da0: 743d 2230 2220 7368 6f77 416c 6c3d 2231  t="0" showAll="1
-00003db0: 2220 706c 6163 656d 656e 743d 2231 2220  " placement="1" 
-00003dc0: 7072 696f 7269 7479 3d22 3022 206f 6273  priority="0" obs
-00003dd0: 7461 636c 653d 2230 2220 7a49 6e64 6578  tacle="0" zIndex
-00003de0: 3d22 3022 206c 696e 6550 6c61 6365 6d65  ="0" linePlaceme
-00003df0: 6e74 466c 6167 733d 2231 3822 3e0a 2020  ntFlags="18">.  
-00003e00: 2020 3c70 726f 7065 7274 6965 733e 0a20    <properties>. 
-00003e10: 2020 2020 203c 4f70 7469 6f6e 2074 7970       <Option typ
-00003e20: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
-00003e30: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003e40: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003e50: 206e 616d 653d 226e 616d 6522 2f3e 0a20   name="name"/>. 
-00003e60: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00003e70: 616d 653d 2270 726f 7065 7274 6965 7322  ame="properties"
-00003e80: 2f3e 0a20 2020 2020 2020 203c 4f70 7469  />.        <Opti
-00003e90: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
-00003ea0: 7469 6f6e 2220 7479 7065 3d22 5153 7472  tion" type="QStr
-00003eb0: 696e 6722 206e 616d 653d 2274 7970 6522  ing" name="type"
-00003ec0: 2f3e 0a20 2020 2020 203c 2f4f 7074 696f  />.      </Optio
-00003ed0: 6e3e 0a20 2020 203c 2f70 726f 7065 7274  n>.    </propert
-00003ee0: 6965 733e 0a20 203c 2f44 6961 6772 616d  ies>.  </Diagram
-00003ef0: 4c61 7965 7253 6574 7469 6e67 733e 0a20  LayerSettings>. 
-00003f00: 203c 6765 6f6d 6574 7279 4f70 7469 6f6e   <geometryOption
-00003f10: 7320 7265 6d6f 7665 4475 706c 6963 6174  s removeDuplicat
-00003f20: 654e 6f64 6573 3d22 3022 2067 656f 6d65  eNodes="0" geome
-00003f30: 7472 7950 7265 6369 7369 6f6e 3d22 3022  tryPrecision="0"
-00003f40: 3e0a 2020 2020 3c61 6374 6976 6543 6865  >.    <activeChe
-00003f50: 636b 732f 3e0a 2020 2020 3c63 6865 636b  cks/>.    <check
-00003f60: 436f 6e66 6967 7572 6174 696f 6e20 7479  Configuration ty
-00003f70: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
-00003f80: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
-00003f90: 7022 206e 616d 653d 2251 6773 4765 6f6d  p" name="QgsGeom
-00003fa0: 6574 7279 4761 7043 6865 636b 223e 0a20  etryGapCheck">. 
-00003fb0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003fc0: 616c 7565 3d22 3022 2074 7970 653d 2264  alue="0" type="d
-00003fd0: 6f75 626c 6522 206e 616d 653d 2261 6c6c  ouble" name="all
-00003fe0: 6f77 6564 4761 7073 4275 6666 6572 222f  owedGapsBuffer"/
-00003ff0: 3e0a 2020 2020 2020 2020 3c4f 7074 696f  >.        <Optio
-00004000: 6e20 7661 6c75 653d 2266 616c 7365 2220  n value="false" 
-00004010: 7479 7065 3d22 626f 6f6c 2220 6e61 6d65  type="bool" name
-00004020: 3d22 616c 6c6f 7765 6447 6170 7345 6e61  ="allowedGapsEna
-00004030: 626c 6564 222f 3e0a 2020 2020 2020 2020  bled"/>.        
-00004040: 3c4f 7074 696f 6e20 7661 6c75 653d 2222  <Option value=""
-00004050: 2074 7970 653d 2251 5374 7269 6e67 2220   type="QString" 
-00004060: 6e61 6d65 3d22 616c 6c6f 7765 6447 6170  name="allowedGap
-00004070: 734c 6179 6572 222f 3e0a 2020 2020 2020  sLayer"/>.      
-00004080: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 3c2f  </Option>.    </
-00004090: 6368 6563 6b43 6f6e 6669 6775 7261 7469  checkConfigurati
-000040a0: 6f6e 3e0a 2020 3c2f 6765 6f6d 6574 7279  on>.  </geometry
-000040b0: 4f70 7469 6f6e 733e 0a20 203c 6c65 6765  Options>.  <lege
-000040c0: 6e64 2073 686f 774c 6162 656c 4c65 6765  nd showLabelLege
-000040d0: 6e64 3d22 3022 2074 7970 653d 2264 6566  nd="0" type="def
-000040e0: 6175 6c74 2d76 6563 746f 7222 2f3e 0a20  ault-vector"/>. 
-000040f0: 203c 7265 6665 7265 6e63 6564 4c61 7965   <referencedLaye
-00004100: 7273 2f3e 0a20 203c 6669 656c 6443 6f6e  rs/>.  <fieldCon
-00004110: 6669 6775 7261 7469 6f6e 3e0a 2020 2020  figuration>.    
-00004120: 3c66 6965 6c64 2063 6f6e 6669 6775 7261  <field configura
-00004130: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
-00004140: 206e 616d 653d 2274 7970 6522 3e0a 2020   name="type">.  
-00004150: 2020 2020 3c65 6469 7457 6964 6765 7420      <editWidget 
-00004160: 7479 7065 3d22 5465 7874 4564 6974 223e  type="TextEdit">
-00004170: 0a20 2020 2020 2020 203c 636f 6e66 6967  .        <config
-00004180: 3e0a 2020 2020 2020 2020 2020 3c4f 7074  >.          <Opt
-00004190: 696f 6e2f 3e0a 2020 2020 2020 2020 3c2f  ion/>.        </
-000041a0: 636f 6e66 6967 3e0a 2020 2020 2020 3c2f  config>.      </
-000041b0: 6564 6974 5769 6467 6574 3e0a 2020 2020  editWidget>.    
-000041c0: 3c2f 6669 656c 643e 0a20 2020 203c 6669  </field>.    <fi
-000041d0: 656c 6420 636f 6e66 6967 7572 6174 696f  eld configuratio
-000041e0: 6e46 6c61 6773 3d22 4e6f 6e65 2220 6e61  nFlags="None" na
-000041f0: 6d65 3d22 6f73 6d5f 6964 223e 0a20 2020  me="osm_id">.   
-00004200: 2020 203c 6564 6974 5769 6467 6574 2074     <editWidget t
-00004210: 7970 653d 2254 6578 7445 6469 7422 3e0a  ype="TextEdit">.
-00004220: 2020 2020 2020 2020 3c63 6f6e 6669 673e          <config>
-00004230: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
-00004240: 6f6e 2f3e 0a20 2020 2020 2020 203c 2f63  on/>.        </c
-00004250: 6f6e 6669 673e 0a20 2020 2020 203c 2f65  onfig>.      </e
-00004260: 6469 7457 6964 6765 743e 0a20 2020 203c  ditWidget>.    <
-00004270: 2f66 6965 6c64 3e0a 2020 2020 3c66 6965  /field>.    <fie
-00004280: 6c64 2063 6f6e 6669 6775 7261 7469 6f6e  ld configuration
-00004290: 466c 6167 733d 224e 6f6e 6522 206e 616d  Flags="None" nam
-000042a0: 653d 226f 7269 656e 7461 7469 6f6e 223e  e="orientation">
-000042b0: 0a20 2020 2020 203c 6564 6974 5769 6467  .      <editWidg
-000042c0: 6574 2074 7970 653d 2254 6578 7445 6469  et type="TextEdi
-000042d0: 7422 3e0a 2020 2020 2020 2020 3c63 6f6e  t">.        <con
-000042e0: 6669 673e 0a20 2020 2020 2020 2020 203c  fig>.          <
-000042f0: 4f70 7469 6f6e 2f3e 0a20 2020 2020 2020  Option/>.       
-00004300: 203c 2f63 6f6e 6669 673e 0a20 2020 2020   </config>.     
-00004310: 203c 2f65 6469 7457 6964 6765 743e 0a20   </editWidget>. 
-00004320: 2020 203c 2f66 6965 6c64 3e0a 2020 2020     </field>.    
-00004330: 3c66 6965 6c64 2063 6f6e 6669 6775 7261  <field configura
-00004340: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
-00004350: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
-00004360: 6f6e 5f63 6f6e 6669 6465 6e63 6522 3e0a  on_confidence">.
-00004370: 2020 2020 2020 3c65 6469 7457 6964 6765        <editWidge
-00004380: 7420 7479 7065 3d22 5465 7874 4564 6974  t type="TextEdit
-00004390: 223e 0a20 2020 2020 2020 203c 636f 6e66  ">.        <conf
-000043a0: 6967 3e0a 2020 2020 2020 2020 2020 3c4f  ig>.          <O
-000043b0: 7074 696f 6e2f 3e0a 2020 2020 2020 2020  ption/>.        
-000043c0: 3c2f 636f 6e66 6967 3e0a 2020 2020 2020  </config>.      
-000043d0: 3c2f 6564 6974 5769 6467 6574 3e0a 2020  </editWidget>.  
-000043e0: 2020 3c2f 6669 656c 643e 0a20 2020 203c    </field>.    <
-000043f0: 6669 656c 6420 636f 6e66 6967 7572 6174  field configurat
-00004400: 696f 6e46 6c61 6773 3d22 4e6f 6e65 2220  ionFlags="None" 
-00004410: 6e61 6d65 3d22 616e 676c 6522 3e0a 2020  name="angle">.  
-00004420: 2020 2020 3c65 6469 7457 6964 6765 7420      <editWidget 
-00004430: 7479 7065 3d22 5261 6e67 6522 3e0a 2020  type="Range">.  
-00004440: 2020 2020 2020 3c63 6f6e 6669 673e 0a20        <config>. 
-00004450: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00004460: 2f3e 0a20 2020 2020 2020 203c 2f63 6f6e  />.        </con
-00004470: 6669 673e 0a20 2020 2020 203c 2f65 6469  fig>.      </edi
-00004480: 7457 6964 6765 743e 0a20 2020 203c 2f66  tWidget>.    </f
-00004490: 6965 6c64 3e0a 2020 3c2f 6669 656c 6443  ield>.  </fieldC
-000044a0: 6f6e 6669 6775 7261 7469 6f6e 3e0a 2020  onfiguration>.  
-000044b0: 3c61 6c69 6173 6573 3e0a 2020 2020 3c61  <aliases>.    <a
-000044c0: 6c69 6173 2066 6965 6c64 3d22 7479 7065  lias field="type
-000044d0: 2220 696e 6465 783d 2230 2220 6e61 6d65  " index="0" name
-000044e0: 3d22 222f 3e0a 2020 2020 3c61 6c69 6173  =""/>.    <alias
-000044f0: 2066 6965 6c64 3d22 6f73 6d5f 6964 2220   field="osm_id" 
-00004500: 696e 6465 783d 2231 2220 6e61 6d65 3d22  index="1" name="
-00004510: 222f 3e0a 2020 2020 3c61 6c69 6173 2066  "/>.    <alias f
-00004520: 6965 6c64 3d22 6f72 6965 6e74 6174 696f  ield="orientatio
-00004530: 6e22 2069 6e64 6578 3d22 3222 206e 616d  n" index="2" nam
-00004540: 653d 2222 2f3e 0a20 2020 203c 616c 6961  e=""/>.    <alia
-00004550: 7320 6669 656c 643d 226f 7269 656e 7461  s field="orienta
-00004560: 7469 6f6e 5f63 6f6e 6669 6465 6e63 6522  tion_confidence"
-00004570: 2069 6e64 6578 3d22 3322 206e 616d 653d   index="3" name=
-00004580: 2222 2f3e 0a20 2020 203c 616c 6961 7320  ""/>.    <alias 
-00004590: 6669 656c 643d 2261 6e67 6c65 2220 696e  field="angle" in
-000045a0: 6465 783d 2234 2220 6e61 6d65 3d22 222f  dex="4" name=""/
-000045b0: 3e0a 2020 3c2f 616c 6961 7365 733e 0a20  >.  </aliases>. 
-000045c0: 203c 6465 6661 756c 7473 3e0a 2020 2020   <defaults>.    
-000045d0: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
-000045e0: 7479 7065 2220 6170 706c 794f 6e55 7064  type" applyOnUpd
-000045f0: 6174 653d 2230 2220 6578 7072 6573 7369  ate="0" expressi
-00004600: 6f6e 3d22 222f 3e0a 2020 2020 3c64 6566  on=""/>.    <def
-00004610: 6175 6c74 2066 6965 6c64 3d22 6f73 6d5f  ault field="osm_
-00004620: 6964 2220 6170 706c 794f 6e55 7064 6174  id" applyOnUpdat
-00004630: 653d 2230 2220 6578 7072 6573 7369 6f6e  e="0" expression
-00004640: 3d22 222f 3e0a 2020 2020 3c64 6566 6175  =""/>.    <defau
-00004650: 6c74 2066 6965 6c64 3d22 6f72 6965 6e74  lt field="orient
-00004660: 6174 696f 6e22 2061 7070 6c79 4f6e 5570  ation" applyOnUp
-00004670: 6461 7465 3d22 3022 2065 7870 7265 7373  date="0" express
-00004680: 696f 6e3d 2222 2f3e 0a20 2020 203c 6465  ion=""/>.    <de
-00004690: 6661 756c 7420 6669 656c 643d 226f 7269  fault field="ori
-000046a0: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
-000046b0: 6e63 6522 2061 7070 6c79 4f6e 5570 6461  nce" applyOnUpda
-000046c0: 7465 3d22 3022 2065 7870 7265 7373 696f  te="0" expressio
-000046d0: 6e3d 2222 2f3e 0a20 2020 203c 6465 6661  n=""/>.    <defa
-000046e0: 756c 7420 6669 656c 643d 2261 6e67 6c65  ult field="angle
-000046f0: 2220 6170 706c 794f 6e55 7064 6174 653d  " applyOnUpdate=
-00004700: 2230 2220 6578 7072 6573 7369 6f6e 3d22  "0" expression="
-00004710: 222f 3e0a 2020 3c2f 6465 6661 756c 7473  "/>.  </defaults
-00004720: 3e0a 2020 3c63 6f6e 7374 7261 696e 7473  >.  <constraints
-00004730: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
-00004740: 7420 756e 6971 7565 5f73 7472 656e 6774  t unique_strengt
-00004750: 683d 2230 2220 6669 656c 643d 2274 7970  h="0" field="typ
-00004760: 6522 206e 6f74 6e75 6c6c 5f73 7472 656e  e" notnull_stren
-00004770: 6774 683d 2230 2220 6578 705f 7374 7265  gth="0" exp_stre
-00004780: 6e67 7468 3d22 3022 2063 6f6e 7374 7261  ngth="0" constra
-00004790: 696e 7473 3d22 3022 2f3e 0a20 2020 203c  ints="0"/>.    <
-000047a0: 636f 6e73 7472 6169 6e74 2075 6e69 7175  constraint uniqu
-000047b0: 655f 7374 7265 6e67 7468 3d22 3022 2066  e_strength="0" f
-000047c0: 6965 6c64 3d22 6f73 6d5f 6964 2220 6e6f  ield="osm_id" no
-000047d0: 746e 756c 6c5f 7374 7265 6e67 7468 3d22  tnull_strength="
-000047e0: 3022 2065 7870 5f73 7472 656e 6774 683d  0" exp_strength=
-000047f0: 2230 2220 636f 6e73 7472 6169 6e74 733d  "0" constraints=
-00004800: 2230 222f 3e0a 2020 2020 3c63 6f6e 7374  "0"/>.    <const
-00004810: 7261 696e 7420 756e 6971 7565 5f73 7472  raint unique_str
-00004820: 656e 6774 683d 2230 2220 6669 656c 643d  ength="0" field=
-00004830: 226f 7269 656e 7461 7469 6f6e 2220 6e6f  "orientation" no
-00004840: 746e 756c 6c5f 7374 7265 6e67 7468 3d22  tnull_strength="
-00004850: 3022 2065 7870 5f73 7472 656e 6774 683d  0" exp_strength=
-00004860: 2230 2220 636f 6e73 7472 6169 6e74 733d  "0" constraints=
-00004870: 2230 222f 3e0a 2020 2020 3c63 6f6e 7374  "0"/>.    <const
-00004880: 7261 696e 7420 756e 6971 7565 5f73 7472  raint unique_str
-00004890: 656e 6774 683d 2230 2220 6669 656c 643d  ength="0" field=
-000048a0: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
-000048b0: 6669 6465 6e63 6522 206e 6f74 6e75 6c6c  fidence" notnull
-000048c0: 5f73 7472 656e 6774 683d 2230 2220 6578  _strength="0" ex
-000048d0: 705f 7374 7265 6e67 7468 3d22 3022 2063  p_strength="0" c
-000048e0: 6f6e 7374 7261 696e 7473 3d22 3022 2f3e  onstraints="0"/>
-000048f0: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
-00004900: 2075 6e69 7175 655f 7374 7265 6e67 7468   unique_strength
-00004910: 3d22 3022 2066 6965 6c64 3d22 616e 676c  ="0" field="angl
-00004920: 6522 206e 6f74 6e75 6c6c 5f73 7472 656e  e" notnull_stren
-00004930: 6774 683d 2230 2220 6578 705f 7374 7265  gth="0" exp_stre
-00004940: 6e67 7468 3d22 3022 2063 6f6e 7374 7261  ngth="0" constra
-00004950: 696e 7473 3d22 3022 2f3e 0a20 203c 2f63  ints="0"/>.  </c
-00004960: 6f6e 7374 7261 696e 7473 3e0a 2020 3c63  onstraints>.  <c
-00004970: 6f6e 7374 7261 696e 7445 7870 7265 7373  onstraintExpress
-00004980: 696f 6e73 3e0a 2020 2020 3c63 6f6e 7374  ions>.    <const
-00004990: 7261 696e 7420 6465 7363 3d22 2220 6578  raint desc="" ex
-000049a0: 703d 2222 2066 6965 6c64 3d22 7479 7065  p="" field="type
-000049b0: 222f 3e0a 2020 2020 3c63 6f6e 7374 7261  "/>.    <constra
-000049c0: 696e 7420 6465 7363 3d22 2220 6578 703d  int desc="" exp=
-000049d0: 2222 2066 6965 6c64 3d22 6f73 6d5f 6964  "" field="osm_id
-000049e0: 222f 3e0a 2020 2020 3c63 6f6e 7374 7261  "/>.    <constra
-000049f0: 696e 7420 6465 7363 3d22 2220 6578 703d  int desc="" exp=
-00004a00: 2222 2066 6965 6c64 3d22 6f72 6965 6e74  "" field="orient
-00004a10: 6174 696f 6e22 2f3e 0a20 2020 203c 636f  ation"/>.    <co
-00004a20: 6e73 7472 6169 6e74 2064 6573 633d 2222  nstraint desc=""
-00004a30: 2065 7870 3d22 2220 6669 656c 643d 226f   exp="" field="o
-00004a40: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
-00004a50: 6465 6e63 6522 2f3e 0a20 2020 203c 636f  dence"/>.    <co
-00004a60: 6e73 7472 6169 6e74 2064 6573 633d 2222  nstraint desc=""
-00004a70: 2065 7870 3d22 2220 6669 656c 643d 2261   exp="" field="a
-00004a80: 6e67 6c65 222f 3e0a 2020 3c2f 636f 6e73  ngle"/>.  </cons
-00004a90: 7472 6169 6e74 4578 7072 6573 7369 6f6e  traintExpression
-00004aa0: 733e 0a20 203c 6578 7072 6573 7369 6f6e  s>.  <expression
-00004ab0: 6669 656c 6473 2f3e 0a20 203c 6174 7472  fields/>.  <attr
-00004ac0: 6962 7574 6561 6374 696f 6e73 3e0a 2020  ibuteactions>.  
-00004ad0: 2020 3c64 6566 6175 6c74 4163 7469 6f6e    <defaultAction
-00004ae0: 2076 616c 7565 3d22 7b30 3030 3030 3030   value="{0000000
-00004af0: 302d 3030 3030 2d30 3030 302d 3030 3030  0-0000-0000-0000
-00004b00: 2d30 3030 3030 3030 3030 3030 307d 2220  -000000000000}" 
-00004b10: 6b65 793d 2243 616e 7661 7322 2f3e 0a20  key="Canvas"/>. 
-00004b20: 203c 2f61 7474 7269 6275 7465 6163 7469   </attributeacti
-00004b30: 6f6e 733e 0a20 203c 6174 7472 6962 7574  ons>.  <attribut
-00004b40: 6574 6162 6c65 636f 6e66 6967 2061 6374  etableconfig act
-00004b50: 696f 6e57 6964 6765 7453 7479 6c65 3d22  ionWidgetStyle="
-00004b60: 6472 6f70 446f 776e 2220 736f 7274 4578  dropDown" sortEx
-00004b70: 7072 6573 7369 6f6e 3d22 2220 736f 7274  pression="" sort
-00004b80: 4f72 6465 723d 2230 223e 0a20 2020 203c  Order="0">.    <
-00004b90: 636f 6c75 6d6e 733e 0a20 2020 2020 203c  columns>.      <
-00004ba0: 636f 6c75 6d6e 2077 6964 7468 3d22 2d31  column width="-1
-00004bb0: 2220 7479 7065 3d22 6669 656c 6422 2068  " type="field" h
-00004bc0: 6964 6465 6e3d 2230 2220 6e61 6d65 3d22  idden="0" name="
-00004bd0: 7479 7065 222f 3e0a 2020 2020 2020 3c63  type"/>.      <c
-00004be0: 6f6c 756d 6e20 7769 6474 683d 222d 3122  olumn width="-1"
-00004bf0: 2074 7970 653d 2266 6965 6c64 2220 6869   type="field" hi
-00004c00: 6464 656e 3d22 3022 206e 616d 653d 226f  dden="0" name="o
-00004c10: 736d 5f69 6422 2f3e 0a20 2020 2020 203c  sm_id"/>.      <
-00004c20: 636f 6c75 6d6e 2077 6964 7468 3d22 2d31  column width="-1
-00004c30: 2220 7479 7065 3d22 6669 656c 6422 2068  " type="field" h
-00004c40: 6964 6465 6e3d 2230 2220 6e61 6d65 3d22  idden="0" name="
-00004c50: 6f72 6965 6e74 6174 696f 6e22 2f3e 0a20  orientation"/>. 
-00004c60: 2020 2020 203c 636f 6c75 6d6e 2077 6964       <column wid
-00004c70: 7468 3d22 2d31 2220 7479 7065 3d22 6669  th="-1" type="fi
-00004c80: 656c 6422 2068 6964 6465 6e3d 2230 2220  eld" hidden="0" 
-00004c90: 6e61 6d65 3d22 6f72 6965 6e74 6174 696f  name="orientatio
-00004ca0: 6e5f 636f 6e66 6964 656e 6365 222f 3e0a  n_confidence"/>.
-00004cb0: 2020 2020 2020 3c63 6f6c 756d 6e20 7769        <column wi
-00004cc0: 6474 683d 222d 3122 2074 7970 653d 2266  dth="-1" type="f
-00004cd0: 6965 6c64 2220 6869 6464 656e 3d22 3022  ield" hidden="0"
-00004ce0: 206e 616d 653d 2261 6e67 6c65 222f 3e0a   name="angle"/>.
-00004cf0: 2020 2020 2020 3c63 6f6c 756d 6e20 7769        <column wi
-00004d00: 6474 683d 222d 3122 2074 7970 653d 2261  dth="-1" type="a
-00004d10: 6374 696f 6e73 2220 6869 6464 656e 3d22  ctions" hidden="
-00004d20: 3122 2f3e 0a20 2020 203c 2f63 6f6c 756d  1"/>.    </colum
-00004d30: 6e73 3e0a 2020 3c2f 6174 7472 6962 7574  ns>.  </attribut
-00004d40: 6574 6162 6c65 636f 6e66 6967 3e0a 2020  etableconfig>.  
-00004d50: 3c63 6f6e 6469 7469 6f6e 616c 7374 796c  <conditionalstyl
-00004d60: 6573 3e0a 2020 2020 3c72 6f77 7374 796c  es>.    <rowstyl
-00004d70: 6573 2f3e 0a20 2020 203c 6669 656c 6473  es/>.    <fields
-00004d80: 7479 6c65 732f 3e0a 2020 3c2f 636f 6e64  tyles/>.  </cond
-00004d90: 6974 696f 6e61 6c73 7479 6c65 733e 0a20  itionalstyles>. 
-00004da0: 203c 7374 6f72 6564 6578 7072 6573 7369   <storedexpressi
-00004db0: 6f6e 732f 3e0a 2020 3c65 6469 7466 6f72  ons/>.  <editfor
-00004dc0: 6d20 746f 6c65 7261 6e74 3d22 3122 3e3c  m tolerant="1"><
-00004dd0: 2f65 6469 7466 6f72 6d3e 0a20 203c 6564  /editform>.  <ed
-00004de0: 6974 666f 726d 696e 6974 2f3e 0a20 203c  itforminit/>.  <
-00004df0: 6564 6974 666f 726d 696e 6974 636f 6465  editforminitcode
-00004e00: 736f 7572 6365 3e30 3c2f 6564 6974 666f  source>0</editfo
-00004e10: 726d 696e 6974 636f 6465 736f 7572 6365  rminitcodesource
-00004e20: 3e0a 2020 3c65 6469 7466 6f72 6d69 6e69  >.  <editformini
-00004e30: 7466 696c 6570 6174 683e 3c2f 6564 6974  tfilepath></edit
-00004e40: 666f 726d 696e 6974 6669 6c65 7061 7468  forminitfilepath
-00004e50: 3e0a 2020 3c65 6469 7466 6f72 6d69 6e69  >.  <editformini
-00004e60: 7463 6f64 653e 3c21 5b43 4441 5441 5b23  tcode><![CDATA[#
-00004e70: 202d 2a2d 2063 6f64 696e 673a 2075 7466   -*- coding: utf
-00004e80: 2d38 202d 2a2d 0a22 2222 0a4c 6573 2066  -8 -*-.""".Les f
-00004e90: 6f72 6d75 6c61 6972 6573 2051 4749 5320  ormulaires QGIS 
-00004ea0: 7065 7576 656e 7420 6176 6f69 7220 756e  peuvent avoir un
-00004eb0: 6520 666f 6e63 7469 6f6e 2050 7974 686f  e fonction Pytho
-00004ec0: 6e20 7175 6920 6573 7420 6170 7065 6cc3  n qui est appel.
-00004ed0: a965 206c 6f72 7371 7565 206c 6520 666f  .e lorsque le fo
-00004ee0: 726d 756c 6169 7265 2065 7374 0a6f 7576  rmulaire est.ouv
-00004ef0: 6572 742e 0a0a 5574 696c 6973 657a 2063  ert...Utilisez c
-00004f00: 6574 7465 2066 6f6e 6374 696f 6e20 706f  ette fonction po
-00004f10: 7572 2061 6a6f 7574 6572 2075 6e65 206c  ur ajouter une l
-00004f20: 6f67 6971 7565 2073 7570 706c c3a9 6d65  ogique suppl..me
-00004f30: 6e74 6169 7265 20c3 a020 766f 7320 666f  ntaire .. vos fo
-00004f40: 726d 756c 6169 7265 732e 0a0a 456e 7472  rmulaires...Entr
-00004f50: 657a 206c 6520 6e6f 6d20 6465 206c 6120  ez le nom de la 
-00004f60: 666f 6e63 7469 6f6e 2064 616e 7320 6c65  fonction dans le
-00004f70: 2063 6861 6d70 200a 2246 6f6e 6374 696f   champ ."Fonctio
-00004f80: 6e20 6427 696e 6974 6961 6c69 7361 7469  n d'initialisati
-00004f90: 6f6e 2050 7974 686f 6e22 2e0a 566f 6963  on Python"..Voic
-00004fa0: 6920 756e 2065 7865 6d70 6c65 3a0a 2222  i un exemple:.""
-00004fb0: 220a 6672 6f6d 2071 6769 732e 5079 5174  ".from qgis.PyQt
-00004fc0: 2e51 7457 6964 6765 7473 2069 6d70 6f72  .QtWidgets impor
-00004fd0: 7420 5157 6964 6765 740a 0a64 6566 206d  t QWidget..def m
-00004fe0: 795f 666f 726d 5f6f 7065 6e28 6469 616c  y_form_open(dial
-00004ff0: 6f67 2c20 6c61 7965 722c 2066 6561 7475  og, layer, featu
-00005000: 7265 293a 0a20 2020 2067 656f 6d20 3d20  re):.    geom = 
-00005010: 6665 6174 7572 652e 6765 6f6d 6574 7279  feature.geometry
-00005020: 2829 0a20 2020 2063 6f6e 7472 6f6c 203d  ().    control =
-00005030: 2064 6961 6c6f 672e 6669 6e64 4368 696c   dialog.findChil
-00005040: 6428 5157 6964 6765 742c 2022 4d79 4c69  d(QWidget, "MyLi
-00005050: 6e65 4564 6974 2229 0a5d 5d3e 3c2f 6564  neEdit").]]></ed
-00005060: 6974 666f 726d 696e 6974 636f 6465 3e0a  itforminitcode>.
-00005070: 2020 3c66 6561 7466 6f72 6d73 7570 7072    <featformsuppr
-00005080: 6573 733e 303c 2f66 6561 7466 6f72 6d73  ess>0</featforms
-00005090: 7570 7072 6573 733e 0a20 203c 6564 6974  uppress>.  <edit
-000050a0: 6f72 6c61 796f 7574 3e67 656e 6572 6174  orlayout>generat
-000050b0: 6564 6c61 796f 7574 3c2f 6564 6974 6f72  edlayout</editor
-000050c0: 6c61 796f 7574 3e0a 2020 3c65 6469 7461  layout>.  <edita
-000050d0: 626c 653e 0a20 2020 203c 6669 656c 6420  ble>.    <field 
-000050e0: 6e61 6d65 3d22 616e 676c 6522 2065 6469  name="angle" edi
-000050f0: 7461 626c 653d 2231 222f 3e0a 2020 2020  table="1"/>.    
-00005100: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
-00005110: 656e 7461 7469 6f6e 2220 6564 6974 6162  entation" editab
-00005120: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
-00005130: 656c 6420 6e61 6d65 3d22 6f72 6965 6e74  eld name="orient
-00005140: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
-00005150: 2220 6564 6974 6162 6c65 3d22 3122 2f3e  " editable="1"/>
-00005160: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-00005170: 3d22 6f73 6d5f 6964 2220 6564 6974 6162  ="osm_id" editab
-00005180: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
-00005190: 656c 6420 6e61 6d65 3d22 7479 7065 2220  eld name="type" 
-000051a0: 6564 6974 6162 6c65 3d22 3122 2f3e 0a20  editable="1"/>. 
-000051b0: 203c 2f65 6469 7461 626c 653e 0a20 203c   </editable>.  <
-000051c0: 6c61 6265 6c4f 6e54 6f70 3e0a 2020 2020  labelOnTop>.    
-000051d0: 3c66 6965 6c64 206c 6162 656c 4f6e 546f  <field labelOnTo
-000051e0: 703d 2230 2220 6e61 6d65 3d22 616e 676c  p="0" name="angl
-000051f0: 6522 2f3e 0a20 2020 203c 6669 656c 6420  e"/>.    <field 
-00005200: 6c61 6265 6c4f 6e54 6f70 3d22 3022 206e  labelOnTop="0" n
-00005210: 616d 653d 226f 7269 656e 7461 7469 6f6e  ame="orientation
-00005220: 222f 3e0a 2020 2020 3c66 6965 6c64 206c  "/>.    <field l
-00005230: 6162 656c 4f6e 546f 703d 2230 2220 6e61  abelOnTop="0" na
-00005240: 6d65 3d22 6f72 6965 6e74 6174 696f 6e5f  me="orientation_
-00005250: 636f 6e66 6964 656e 6365 222f 3e0a 2020  confidence"/>.  
-00005260: 2020 3c66 6965 6c64 206c 6162 656c 4f6e    <field labelOn
-00005270: 546f 703d 2230 2220 6e61 6d65 3d22 6f73  Top="0" name="os
-00005280: 6d5f 6964 222f 3e0a 2020 2020 3c66 6965  m_id"/>.    <fie
-00005290: 6c64 206c 6162 656c 4f6e 546f 703d 2230  ld labelOnTop="0
-000052a0: 2220 6e61 6d65 3d22 7479 7065 222f 3e0a  " name="type"/>.
-000052b0: 2020 3c2f 6c61 6265 6c4f 6e54 6f70 3e0a    </labelOnTop>.
-000052c0: 2020 3c72 6575 7365 4c61 7374 5661 6c75    <reuseLastValu
-000052d0: 653e 0a20 2020 203c 6669 656c 6420 7265  e>.    <field re
-000052e0: 7573 654c 6173 7456 616c 7565 3d22 3022  useLastValue="0"
-000052f0: 206e 616d 653d 2261 6e67 6c65 222f 3e0a   name="angle"/>.
-00005300: 2020 2020 3c66 6965 6c64 2072 6575 7365      <field reuse
-00005310: 4c61 7374 5661 6c75 653d 2230 2220 6e61  LastValue="0" na
-00005320: 6d65 3d22 6f72 6965 6e74 6174 696f 6e22  me="orientation"
-00005330: 2f3e 0a20 2020 203c 6669 656c 6420 7265  />.    <field re
-00005340: 7573 654c 6173 7456 616c 7565 3d22 3022  useLastValue="0"
-00005350: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
-00005360: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2f3e  on_confidence"/>
-00005370: 0a20 2020 203c 6669 656c 6420 7265 7573  .    <field reus
-00005380: 654c 6173 7456 616c 7565 3d22 3022 206e  eLastValue="0" n
-00005390: 616d 653d 226f 736d 5f69 6422 2f3e 0a20  ame="osm_id"/>. 
-000053a0: 2020 203c 6669 656c 6420 7265 7573 654c     <field reuseL
-000053b0: 6173 7456 616c 7565 3d22 3022 206e 616d  astValue="0" nam
-000053c0: 653d 2274 7970 6522 2f3e 0a20 203c 2f72  e="type"/>.  </r
-000053d0: 6575 7365 4c61 7374 5661 6c75 653e 0a20  euseLastValue>. 
-000053e0: 203c 6461 7461 4465 6669 6e65 6446 6965   <dataDefinedFie
-000053f0: 6c64 5072 6f70 6572 7469 6573 2f3e 0a20  ldProperties/>. 
-00005400: 203c 7769 6467 6574 732f 3e0a 2020 3c70   <widgets/>.  <p
-00005410: 7265 7669 6577 4578 7072 6573 7369 6f6e  reviewExpression
-00005420: 3e22 7479 7065 223c 2f70 7265 7669 6577  >"type"</preview
-00005430: 4578 7072 6573 7369 6f6e 3e0a 2020 3c6d  Expression>.  <m
-00005440: 6170 5469 703e 3c2f 6d61 7054 6970 3e0a  apTip></mapTip>.
-00005450: 2020 3c6c 6179 6572 4765 6f6d 6574 7279    <layerGeometry
-00005460: 5479 7065 3e32 3c2f 6c61 7965 7247 656f  Type>2</layerGeo
-00005470: 6d65 7472 7954 7970 653e 0a3c 2f71 6769  metryType>.</qgi
-00005480: 733e 0a                                  s>.
+000036e0: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+000036f0: 302c 302c 302c 3022 206e 616d 653d 2264  0,0,0,0" name="d
+00003700: 6173 685f 7061 7474 6572 6e5f 6f66 6673  ash_pattern_offs
+00003710: 6574 5f6d 6170 5f75 6e69 745f 7363 616c  et_map_unit_scal
+00003720: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00003730: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003740: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003750: 224d 4d22 206e 616d 653d 2264 6173 685f  "MM" name="dash_
+00003760: 7061 7474 6572 6e5f 6f66 6673 6574 5f75  pattern_offset_u
+00003770: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00003780: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003790: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+000037a0: 653d 2230 2220 6e61 6d65 3d22 6472 6177  e="0" name="draw
+000037b0: 5f69 6e73 6964 655f 706f 6c79 676f 6e22  _inside_polygon"
+000037c0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000037d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000037e0: 3c4f 7074 696f 6e20 7661 6c75 653d 2262  <Option value="b
+000037f0: 6576 656c 2220 6e61 6d65 3d22 6a6f 696e  evel" name="join
+00003800: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
+00003810: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003820: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00003830: 6c75 653d 2233 352c 3335 2c33 352c 3235  lue="35,35,35,25
+00003840: 3522 206e 616d 653d 226c 696e 655f 636f  5" name="line_co
+00003850: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
+00003860: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003870: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003880: 653d 2273 6f6c 6964 2220 6e61 6d65 3d22  e="solid" name="
+00003890: 6c69 6e65 5f73 7479 6c65 2220 7479 7065  line_style" type
+000038a0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000038b0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000038c0: 6f6e 2076 616c 7565 3d22 302e 3236 2220  on value="0.26" 
+000038d0: 6e61 6d65 3d22 6c69 6e65 5f77 6964 7468  name="line_width
+000038e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000038f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00003900: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003910: 4d4d 2220 6e61 6d65 3d22 6c69 6e65 5f77  MM" name="line_w
+00003920: 6964 7468 5f75 6e69 7422 2074 7970 653d  idth_unit" type=
+00003930: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003940: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003950: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+00003960: 3d22 6f66 6673 6574 2220 7479 7065 3d22  ="offset" type="
+00003970: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003980: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003990: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
+000039a0: 2c30 2c30 2c30 2220 6e61 6d65 3d22 6f66  ,0,0,0" name="of
+000039b0: 6673 6574 5f6d 6170 5f75 6e69 745f 7363  fset_map_unit_sc
+000039c0: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+000039d0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000039e0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+000039f0: 653d 224d 4d22 206e 616d 653d 226f 6666  e="MM" name="off
+00003a00: 7365 745f 756e 6974 2220 7479 7065 3d22  set_unit" type="
+00003a10: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003a20: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003a30: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
+00003a40: 2272 696e 675f 6669 6c74 6572 2220 7479  "ring_filter" ty
+00003a50: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003a60: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00003a70: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00003a80: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
+00003a90: 6365 5f65 6e64 2220 7479 7065 3d22 5153  ce_end" type="QS
+00003aa0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00003ab0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00003ac0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00003ad0: 2c30 2c30 2220 6e61 6d65 3d22 7472 696d  ,0,0" name="trim
+00003ae0: 5f64 6973 7461 6e63 655f 656e 645f 6d61  _distance_end_ma
+00003af0: 705f 756e 6974 5f73 6361 6c65 2220 7479  p_unit_scale" ty
+00003b00: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003b10: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00003b20: 7469 6f6e 2076 616c 7565 3d22 4d4d 2220  tion value="MM" 
+00003b30: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
+00003b40: 6e63 655f 656e 645f 756e 6974 2220 7479  nce_end_unit" ty
+00003b50: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003b60: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00003b70: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00003b80: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
+00003b90: 6365 5f73 7461 7274 2220 7479 7065 3d22  ce_start" type="
+00003ba0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003bb0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003bc0: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
+00003bd0: 2c30 2c30 2c30 2220 6e61 6d65 3d22 7472  ,0,0,0" name="tr
+00003be0: 696d 5f64 6973 7461 6e63 655f 7374 6172  im_distance_star
+00003bf0: 745f 6d61 705f 756e 6974 5f73 6361 6c65  t_map_unit_scale
+00003c00: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003c10: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00003c20: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003c30: 4d4d 2220 6e61 6d65 3d22 7472 696d 5f64  MM" name="trim_d
+00003c40: 6973 7461 6e63 655f 7374 6172 745f 756e  istance_start_un
+00003c50: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00003c60: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003c70: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003c80: 3d22 3022 206e 616d 653d 2274 7765 616b  ="0" name="tweak
+00003c90: 5f64 6173 685f 7061 7474 6572 6e5f 6f6e  _dash_pattern_on
+00003ca0: 5f63 6f72 6e65 7273 2220 7479 7065 3d22  _corners" type="
+00003cb0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003cc0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003cd0: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
+00003ce0: 2275 7365 5f63 7573 746f 6d5f 6461 7368  "use_custom_dash
+00003cf0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003d00: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00003d10: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003d20: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
+00003d30: 6e61 6d65 3d22 7769 6474 685f 6d61 705f  name="width_map_
+00003d40: 756e 6974 5f73 6361 6c65 2220 7479 7065  unit_scale" type
+00003d50: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003d60: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00003d70: 6e3e 0a20 2020 2020 2020 2020 2020 203c  n>.            <
+00003d80: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+00003d90: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+00003da0: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00003db0: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00003dc0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003dd0: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
+00003de0: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
+00003df0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00003e00: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003e10: 206e 616d 653d 2270 726f 7065 7274 6965   name="propertie
+00003e20: 7322 2f3e 0a20 2020 2020 2020 2020 2020  s"/>.           
+00003e30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00003e40: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
+00003e50: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
+00003e60: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003e70: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+00003e80: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00003e90: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
+00003ea0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
+00003eb0: 2020 2020 2020 3c2f 6c61 7965 723e 0a20        </layer>. 
+00003ec0: 2020 2020 2020 203c 2f73 796d 626f 6c3e         </symbol>
+00003ed0: 0a20 2020 2020 203c 2f61 7869 7353 796d  .      </axisSym
+00003ee0: 626f 6c3e 0a20 2020 203c 2f44 6961 6772  bol>.    </Diagr
+00003ef0: 616d 4361 7465 676f 7279 3e0a 2020 3c2f  amCategory>.  </
+00003f00: 5369 6e67 6c65 4361 7465 676f 7279 4469  SingleCategoryDi
+00003f10: 6167 7261 6d52 656e 6465 7265 723e 0a20  agramRenderer>. 
+00003f20: 203c 4469 6167 7261 6d4c 6179 6572 5365   <DiagramLayerSe
+00003f30: 7474 696e 6773 207a 496e 6465 783d 2230  ttings zIndex="0
+00003f40: 2220 7368 6f77 416c 6c3d 2231 2220 706c  " showAll="1" pl
+00003f50: 6163 656d 656e 743d 2230 2220 6c69 6e65  acement="0" line
+00003f60: 506c 6163 656d 656e 7446 6c61 6773 3d22  PlacementFlags="
+00003f70: 3138 2220 6f62 7374 6163 6c65 3d22 3022  18" obstacle="0"
+00003f80: 2064 6973 743d 2230 2220 7072 696f 7269   dist="0" priori
+00003f90: 7479 3d22 3022 3e0a 2020 2020 3c70 726f  ty="0">.    <pro
+00003fa0: 7065 7274 6965 733e 0a20 2020 2020 203c  perties>.      <
+00003fb0: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
+00003fc0: 223e 0a20 2020 2020 2020 203c 4f70 7469  ">.        <Opti
+00003fd0: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
+00003fe0: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
+00003ff0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00004000: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00004010: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
+00004020: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00004030: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
+00004040: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
+00004050: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00004060: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+00004070: 203c 2f70 726f 7065 7274 6965 733e 0a20   </properties>. 
+00004080: 203c 2f44 6961 6772 616d 4c61 7965 7253   </DiagramLayerS
+00004090: 6574 7469 6e67 733e 0a20 203c 6765 6f6d  ettings>.  <geom
+000040a0: 6574 7279 4f70 7469 6f6e 7320 7265 6d6f  etryOptions remo
+000040b0: 7665 4475 706c 6963 6174 654e 6f64 6573  veDuplicateNodes
+000040c0: 3d22 3022 2067 656f 6d65 7472 7950 7265  ="0" geometryPre
+000040d0: 6369 7369 6f6e 3d22 3022 3e0a 2020 2020  cision="0">.    
+000040e0: 3c61 6374 6976 6543 6865 636b 732f 3e0a  <activeChecks/>.
+000040f0: 2020 2020 3c63 6865 636b 436f 6e66 6967      <checkConfig
+00004100: 7572 6174 696f 6e2f 3e0a 2020 3c2f 6765  uration/>.  </ge
+00004110: 6f6d 6574 7279 4f70 7469 6f6e 733e 0a20  ometryOptions>. 
+00004120: 203c 6c65 6765 6e64 2073 686f 774c 6162   <legend showLab
+00004130: 656c 4c65 6765 6e64 3d22 3022 2074 7970  elLegend="0" typ
+00004140: 653d 2264 6566 6175 6c74 2d76 6563 746f  e="default-vecto
+00004150: 7222 2f3e 0a20 203c 7265 6665 7265 6e63  r"/>.  <referenc
+00004160: 6564 4c61 7965 7273 2f3e 0a20 203c 6669  edLayers/>.  <fi
+00004170: 656c 6443 6f6e 6669 6775 7261 7469 6f6e  eldConfiguration
+00004180: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00004190: 653d 2274 7970 6522 2063 6f6e 6669 6775  e="type" configu
+000041a0: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
+000041b0: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
+000041c0: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
+000041d0: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
+000041e0: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
+000041f0: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
+00004200: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
+00004210: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
+00004220: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
+00004230: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00004240: 6f73 6d5f 6964 2220 636f 6e66 6967 7572  osm_id" configur
+00004250: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
+00004260: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
+00004270: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
+00004280: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
+00004290: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
+000042a0: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
+000042b0: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
+000042c0: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
+000042d0: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
+000042e0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+000042f0: 7269 656e 7461 7469 6f6e 2220 636f 6e66  rientation" conf
+00004300: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
+00004310: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
+00004320: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
+00004330: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
+00004340: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
+00004350: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
+00004360: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
+00004370: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
+00004380: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
+00004390: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+000043a0: 653d 226f 7269 656e 7461 7469 6f6e 5f63  e="orientation_c
+000043b0: 6f6e 6669 6465 6e63 6522 2063 6f6e 6669  onfidence" confi
+000043c0: 6775 7261 7469 6f6e 466c 6167 733d 224e  gurationFlags="N
+000043d0: 6f6e 6522 3e0a 2020 2020 2020 3c65 6469  one">.      <edi
+000043e0: 7457 6964 6765 7420 7479 7065 3d22 5465  tWidget type="Te
+000043f0: 7874 4564 6974 223e 0a20 2020 2020 2020  xtEdit">.       
+00004400: 203c 636f 6e66 6967 3e0a 2020 2020 2020   <config>.      
+00004410: 2020 2020 3c4f 7074 696f 6e2f 3e0a 2020      <Option/>.  
+00004420: 2020 2020 2020 3c2f 636f 6e66 6967 3e0a        </config>.
+00004430: 2020 2020 2020 3c2f 6564 6974 5769 6467        </editWidg
+00004440: 6574 3e0a 2020 2020 3c2f 6669 656c 643e  et>.    </field>
+00004450: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00004460: 3d22 6c61 6e65 5f77 6964 7468 2220 636f  ="lane_width" co
+00004470: 6e66 6967 7572 6174 696f 6e46 6c61 6773  nfigurationFlags
+00004480: 3d22 4e6f 6e65 223e 0a20 2020 2020 203c  ="None">.      <
+00004490: 6564 6974 5769 6467 6574 2074 7970 653d  editWidget type=
+000044a0: 2254 6578 7445 6469 7422 3e0a 2020 2020  "TextEdit">.    
+000044b0: 2020 2020 3c63 6f6e 6669 673e 0a20 2020      <config>.   
+000044c0: 2020 2020 2020 203c 4f70 7469 6f6e 2f3e         <Option/>
+000044d0: 0a20 2020 2020 2020 203c 2f63 6f6e 6669  .        </confi
+000044e0: 673e 0a20 2020 2020 203c 2f65 6469 7457  g>.      </editW
+000044f0: 6964 6765 743e 0a20 2020 203c 2f66 6965  idget>.    </fie
+00004500: 6c64 3e0a 2020 2020 3c66 6965 6c64 206e  ld>.    <field n
+00004510: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
+00004520: 6174 696f 6e22 2063 6f6e 6669 6775 7261  ation" configura
+00004530: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
+00004540: 3e0a 2020 2020 2020 3c65 6469 7457 6964  >.      <editWid
+00004550: 6765 7420 7479 7065 3d22 5465 7874 4564  get type="TextEd
+00004560: 6974 223e 0a20 2020 2020 2020 203c 636f  it">.        <co
+00004570: 6e66 6967 3e0a 2020 2020 2020 2020 2020  nfig>.          
+00004580: 3c4f 7074 696f 6e2f 3e0a 2020 2020 2020  <Option/>.      
+00004590: 2020 3c2f 636f 6e66 6967 3e0a 2020 2020    </config>.    
+000045a0: 2020 3c2f 6564 6974 5769 6467 6574 3e0a    </editWidget>.
+000045b0: 2020 2020 3c2f 6669 656c 643e 0a20 203c      </field>.  <
+000045c0: 2f66 6965 6c64 436f 6e66 6967 7572 6174  /fieldConfigurat
+000045d0: 696f 6e3e 0a20 203c 616c 6961 7365 733e  ion>.  <aliases>
+000045e0: 0a20 2020 203c 616c 6961 7320 6e61 6d65  .    <alias name
+000045f0: 3d22 2220 696e 6465 783d 2230 2220 6669  ="" index="0" fi
+00004600: 656c 643d 2274 7970 6522 2f3e 0a20 2020  eld="type"/>.   
+00004610: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
+00004620: 696e 6465 783d 2231 2220 6669 656c 643d  index="1" field=
+00004630: 226f 736d 5f69 6422 2f3e 0a20 2020 203c  "osm_id"/>.    <
+00004640: 616c 6961 7320 6e61 6d65 3d22 2220 696e  alias name="" in
+00004650: 6465 783d 2232 2220 6669 656c 643d 226f  dex="2" field="o
+00004660: 7269 656e 7461 7469 6f6e 222f 3e0a 2020  rientation"/>.  
+00004670: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
+00004680: 2069 6e64 6578 3d22 3322 2066 6965 6c64   index="3" field
+00004690: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+000046a0: 6e66 6964 656e 6365 222f 3e0a 2020 2020  nfidence"/>.    
+000046b0: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
+000046c0: 6e64 6578 3d22 3422 2066 6965 6c64 3d22  ndex="4" field="
+000046d0: 6c61 6e65 5f77 6964 7468 222f 3e0a 2020  lane_width"/>.  
+000046e0: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
+000046f0: 2069 6e64 6578 3d22 3522 2066 6965 6c64   index="5" field
+00004700: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+00004710: 6f6e 222f 3e0a 2020 3c2f 616c 6961 7365  on"/>.  </aliase
+00004720: 733e 0a20 203c 6465 6661 756c 7473 3e0a  s>.  <defaults>.
+00004730: 2020 2020 3c64 6566 6175 6c74 2066 6965      <default fie
+00004740: 6c64 3d22 7479 7065 2220 6578 7072 6573  ld="type" expres
+00004750: 7369 6f6e 3d22 2220 6170 706c 794f 6e55  sion="" applyOnU
+00004760: 7064 6174 653d 2230 222f 3e0a 2020 2020  pdate="0"/>.    
+00004770: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
+00004780: 6f73 6d5f 6964 2220 6578 7072 6573 7369  osm_id" expressi
+00004790: 6f6e 3d22 2220 6170 706c 794f 6e55 7064  on="" applyOnUpd
+000047a0: 6174 653d 2230 222f 3e0a 2020 2020 3c64  ate="0"/>.    <d
+000047b0: 6566 6175 6c74 2066 6965 6c64 3d22 6f72  efault field="or
+000047c0: 6965 6e74 6174 696f 6e22 2065 7870 7265  ientation" expre
+000047d0: 7373 696f 6e3d 2222 2061 7070 6c79 4f6e  ssion="" applyOn
+000047e0: 5570 6461 7465 3d22 3022 2f3e 0a20 2020  Update="0"/>.   
+000047f0: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
+00004800: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
+00004810: 6669 6465 6e63 6522 2065 7870 7265 7373  fidence" express
+00004820: 696f 6e3d 2222 2061 7070 6c79 4f6e 5570  ion="" applyOnUp
+00004830: 6461 7465 3d22 3022 2f3e 0a20 2020 203c  date="0"/>.    <
+00004840: 6465 6661 756c 7420 6669 656c 643d 226c  default field="l
+00004850: 616e 655f 7769 6474 6822 2065 7870 7265  ane_width" expre
+00004860: 7373 696f 6e3d 2222 2061 7070 6c79 4f6e  ssion="" applyOn
+00004870: 5570 6461 7465 3d22 3022 2f3e 0a20 2020  Update="0"/>.   
+00004880: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
+00004890: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+000048a0: 6e22 2065 7870 7265 7373 696f 6e3d 2222  n" expression=""
+000048b0: 2061 7070 6c79 4f6e 5570 6461 7465 3d22   applyOnUpdate="
+000048c0: 3022 2f3e 0a20 203c 2f64 6566 6175 6c74  0"/>.  </default
+000048d0: 733e 0a20 203c 636f 6e73 7472 6169 6e74  s>.  <constraint
+000048e0: 733e 0a20 2020 203c 636f 6e73 7472 6169  s>.    <constrai
+000048f0: 6e74 2075 6e69 7175 655f 7374 7265 6e67  nt unique_streng
+00004900: 7468 3d22 3022 206e 6f74 6e75 6c6c 5f73  th="0" notnull_s
+00004910: 7472 656e 6774 683d 2230 2220 6578 705f  trength="0" exp_
+00004920: 7374 7265 6e67 7468 3d22 3022 2066 6965  strength="0" fie
+00004930: 6c64 3d22 7479 7065 2220 636f 6e73 7472  ld="type" constr
+00004940: 6169 6e74 733d 2230 222f 3e0a 2020 2020  aints="0"/>.    
+00004950: 3c63 6f6e 7374 7261 696e 7420 756e 6971  <constraint uniq
+00004960: 7565 5f73 7472 656e 6774 683d 2230 2220  ue_strength="0" 
+00004970: 6e6f 746e 756c 6c5f 7374 7265 6e67 7468  notnull_strength
+00004980: 3d22 3022 2065 7870 5f73 7472 656e 6774  ="0" exp_strengt
+00004990: 683d 2230 2220 6669 656c 643d 226f 736d  h="0" field="osm
+000049a0: 5f69 6422 2063 6f6e 7374 7261 696e 7473  _id" constraints
+000049b0: 3d22 3022 2f3e 0a20 2020 203c 636f 6e73  ="0"/>.    <cons
+000049c0: 7472 6169 6e74 2075 6e69 7175 655f 7374  traint unique_st
+000049d0: 7265 6e67 7468 3d22 3022 206e 6f74 6e75  rength="0" notnu
+000049e0: 6c6c 5f73 7472 656e 6774 683d 2230 2220  ll_strength="0" 
+000049f0: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
+00004a00: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
+00004a10: 696f 6e22 2063 6f6e 7374 7261 696e 7473  ion" constraints
+00004a20: 3d22 3022 2f3e 0a20 2020 203c 636f 6e73  ="0"/>.    <cons
+00004a30: 7472 6169 6e74 2075 6e69 7175 655f 7374  traint unique_st
+00004a40: 7265 6e67 7468 3d22 3022 206e 6f74 6e75  rength="0" notnu
+00004a50: 6c6c 5f73 7472 656e 6774 683d 2230 2220  ll_strength="0" 
+00004a60: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
+00004a70: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
+00004a80: 696f 6e5f 636f 6e66 6964 656e 6365 2220  ion_confidence" 
+00004a90: 636f 6e73 7472 6169 6e74 733d 2230 222f  constraints="0"/
+00004aa0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00004ab0: 7420 756e 6971 7565 5f73 7472 656e 6774  t unique_strengt
+00004ac0: 683d 2230 2220 6e6f 746e 756c 6c5f 7374  h="0" notnull_st
+00004ad0: 7265 6e67 7468 3d22 3022 2065 7870 5f73  rength="0" exp_s
+00004ae0: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
+00004af0: 643d 226c 616e 655f 7769 6474 6822 2063  d="lane_width" c
+00004b00: 6f6e 7374 7261 696e 7473 3d22 3022 2f3e  onstraints="0"/>
+00004b10: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
+00004b20: 2075 6e69 7175 655f 7374 7265 6e67 7468   unique_strength
+00004b30: 3d22 3022 206e 6f74 6e75 6c6c 5f73 7472  ="0" notnull_str
+00004b40: 656e 6774 683d 2230 2220 6578 705f 7374  ength="0" exp_st
+00004b50: 7265 6e67 7468 3d22 3022 2066 6965 6c64  rength="0" field
+00004b60: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+00004b70: 6f6e 2220 636f 6e73 7472 6169 6e74 733d  on" constraints=
+00004b80: 2230 222f 3e0a 2020 3c2f 636f 6e73 7472  "0"/>.  </constr
+00004b90: 6169 6e74 733e 0a20 203c 636f 6e73 7472  aints>.  <constr
+00004ba0: 6169 6e74 4578 7072 6573 7369 6f6e 733e  aintExpressions>
+00004bb0: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
+00004bc0: 2064 6573 633d 2222 2065 7870 3d22 2220   desc="" exp="" 
+00004bd0: 6669 656c 643d 2274 7970 6522 2f3e 0a20  field="type"/>. 
+00004be0: 2020 203c 636f 6e73 7472 6169 6e74 2064     <constraint d
+00004bf0: 6573 633d 2222 2065 7870 3d22 2220 6669  esc="" exp="" fi
+00004c00: 656c 643d 226f 736d 5f69 6422 2f3e 0a20  eld="osm_id"/>. 
+00004c10: 2020 203c 636f 6e73 7472 6169 6e74 2064     <constraint d
+00004c20: 6573 633d 2222 2065 7870 3d22 2220 6669  esc="" exp="" fi
+00004c30: 656c 643d 226f 7269 656e 7461 7469 6f6e  eld="orientation
+00004c40: 222f 3e0a 2020 2020 3c63 6f6e 7374 7261  "/>.    <constra
+00004c50: 696e 7420 6465 7363 3d22 2220 6578 703d  int desc="" exp=
+00004c60: 2222 2066 6965 6c64 3d22 6f72 6965 6e74  "" field="orient
+00004c70: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
+00004c80: 222f 3e0a 2020 2020 3c63 6f6e 7374 7261  "/>.    <constra
+00004c90: 696e 7420 6465 7363 3d22 2220 6578 703d  int desc="" exp=
+00004ca0: 2222 2066 6965 6c64 3d22 6c61 6e65 5f77  "" field="lane_w
+00004cb0: 6964 7468 222f 3e0a 2020 2020 3c63 6f6e  idth"/>.    <con
+00004cc0: 7374 7261 696e 7420 6465 7363 3d22 2220  straint desc="" 
+00004cd0: 6578 703d 2222 2066 6965 6c64 3d22 6c61  exp="" field="la
+00004ce0: 6e65 5f6f 7269 656e 7461 7469 6f6e 222f  ne_orientation"/
+00004cf0: 3e0a 2020 3c2f 636f 6e73 7472 6169 6e74  >.  </constraint
+00004d00: 4578 7072 6573 7369 6f6e 733e 0a20 203c  Expressions>.  <
+00004d10: 6578 7072 6573 7369 6f6e 6669 656c 6473  expressionfields
+00004d20: 2f3e 0a20 203c 6174 7472 6962 7574 6561  />.  <attributea
+00004d30: 6374 696f 6e73 3e0a 2020 2020 3c64 6566  ctions>.    <def
+00004d40: 6175 6c74 4163 7469 6f6e 2076 616c 7565  aultAction value
+00004d50: 3d22 7b30 3030 3030 3030 302d 3030 3030  ="{00000000-0000
+00004d60: 2d30 3030 302d 3030 3030 2d30 3030 3030  -0000-0000-00000
+00004d70: 3030 3030 3030 307d 2220 6b65 793d 2243  0000000}" key="C
+00004d80: 616e 7661 7322 2f3e 0a20 203c 2f61 7474  anvas"/>.  </att
+00004d90: 7269 6275 7465 6163 7469 6f6e 733e 0a20  ributeactions>. 
+00004da0: 203c 6174 7472 6962 7574 6574 6162 6c65   <attributetable
+00004db0: 636f 6e66 6967 2061 6374 696f 6e57 6964  config actionWid
+00004dc0: 6765 7453 7479 6c65 3d22 6472 6f70 446f  getStyle="dropDo
+00004dd0: 776e 2220 736f 7274 4f72 6465 723d 2230  wn" sortOrder="0
+00004de0: 2220 736f 7274 4578 7072 6573 7369 6f6e  " sortExpression
+00004df0: 3d22 223e 0a20 2020 203c 636f 6c75 6d6e  ="">.    <column
+00004e00: 733e 0a20 2020 2020 203c 636f 6c75 6d6e  s>.      <column
+00004e10: 206e 616d 653d 2274 7970 6522 2077 6964   name="type" wid
+00004e20: 7468 3d22 2d31 2220 6869 6464 656e 3d22  th="-1" hidden="
+00004e30: 3022 2074 7970 653d 2266 6965 6c64 222f  0" type="field"/
+00004e40: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+00004e50: 6e61 6d65 3d22 6f73 6d5f 6964 2220 7769  name="osm_id" wi
+00004e60: 6474 683d 2231 3731 2220 6869 6464 656e  dth="171" hidden
+00004e70: 3d22 3022 2074 7970 653d 2266 6965 6c64  ="0" type="field
+00004e80: 222f 3e0a 2020 2020 2020 3c63 6f6c 756d  "/>.      <colum
+00004e90: 6e20 6e61 6d65 3d22 6f72 6965 6e74 6174  n name="orientat
+00004ea0: 696f 6e22 2077 6964 7468 3d22 3239 3222  ion" width="292"
+00004eb0: 2068 6964 6465 6e3d 2230 2220 7479 7065   hidden="0" type
+00004ec0: 3d22 6669 656c 6422 2f3e 0a20 2020 2020  ="field"/>.     
+00004ed0: 203c 636f 6c75 6d6e 206e 616d 653d 226f   <column name="o
+00004ee0: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
+00004ef0: 6465 6e63 6522 2077 6964 7468 3d22 2d31  dence" width="-1
+00004f00: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
+00004f10: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
+00004f20: 2020 3c63 6f6c 756d 6e20 6e61 6d65 3d22    <column name="
+00004f30: 6c61 6e65 5f6f 7269 656e 7461 7469 6f6e  lane_orientation
+00004f40: 2220 7769 6474 683d 222d 3122 2068 6964  " width="-1" hid
+00004f50: 6465 6e3d 2230 2220 7479 7065 3d22 6669  den="0" type="fi
+00004f60: 656c 6422 2f3e 0a20 2020 2020 203c 636f  eld"/>.      <co
+00004f70: 6c75 6d6e 206e 616d 653d 226c 616e 655f  lumn name="lane_
+00004f80: 7769 6474 6822 2077 6964 7468 3d22 2d31  width" width="-1
+00004f90: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
+00004fa0: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
+00004fb0: 2020 3c63 6f6c 756d 6e20 7769 6474 683d    <column width=
+00004fc0: 222d 3122 2068 6964 6465 6e3d 2231 2220  "-1" hidden="1" 
+00004fd0: 7479 7065 3d22 6163 7469 6f6e 7322 2f3e  type="actions"/>
+00004fe0: 0a20 2020 203c 2f63 6f6c 756d 6e73 3e0a  .    </columns>.
+00004ff0: 2020 3c2f 6174 7472 6962 7574 6574 6162    </attributetab
+00005000: 6c65 636f 6e66 6967 3e0a 2020 3c63 6f6e  leconfig>.  <con
+00005010: 6469 7469 6f6e 616c 7374 796c 6573 3e0a  ditionalstyles>.
+00005020: 2020 2020 3c72 6f77 7374 796c 6573 2f3e      <rowstyles/>
+00005030: 0a20 2020 203c 6669 656c 6473 7479 6c65  .    <fieldstyle
+00005040: 732f 3e0a 2020 3c2f 636f 6e64 6974 696f  s/>.  </conditio
+00005050: 6e61 6c73 7479 6c65 733e 0a20 203c 7374  nalstyles>.  <st
+00005060: 6f72 6564 6578 7072 6573 7369 6f6e 732f  oredexpressions/
+00005070: 3e0a 2020 3c65 6469 7466 6f72 6d20 746f  >.  <editform to
+00005080: 6c65 7261 6e74 3d22 3122 3e3c 2f65 6469  lerant="1"></edi
+00005090: 7466 6f72 6d3e 0a20 203c 6564 6974 666f  tform>.  <editfo
+000050a0: 726d 696e 6974 2f3e 0a20 203c 6564 6974  rminit/>.  <edit
+000050b0: 666f 726d 696e 6974 636f 6465 736f 7572  forminitcodesour
+000050c0: 6365 3e30 3c2f 6564 6974 666f 726d 696e  ce>0</editformin
+000050d0: 6974 636f 6465 736f 7572 6365 3e0a 2020  itcodesource>.  
+000050e0: 3c65 6469 7466 6f72 6d69 6e69 7466 696c  <editforminitfil
+000050f0: 6570 6174 683e 3c2f 6564 6974 666f 726d  epath></editform
+00005100: 696e 6974 6669 6c65 7061 7468 3e0a 2020  initfilepath>.  
+00005110: 3c65 6469 7466 6f72 6d69 6e69 7463 6f64  <editforminitcod
+00005120: 653e 3c21 5b43 4441 5441 5b23 202d 2a2d  e><![CDATA[# -*-
+00005130: 2063 6f64 696e 673a 2075 7466 2d38 202d   coding: utf-8 -
+00005140: 2a2d 0a22 2222 0a4c 6573 2066 6f72 6d75  *-.""".Les formu
+00005150: 6c61 6972 6573 2051 4749 5320 7065 7576  laires QGIS peuv
+00005160: 656e 7420 6176 6f69 7220 756e 6520 666f  ent avoir une fo
+00005170: 6e63 7469 6f6e 2050 7974 686f 6e20 7175  nction Python qu
+00005180: 6920 6573 7420 6170 7065 6cc3 a965 206c  i est appel..e l
+00005190: 6f72 7371 7565 206c 6520 666f 726d 756c  orsque le formul
+000051a0: 6169 7265 2065 7374 0a6f 7576 6572 742e  aire est.ouvert.
+000051b0: 0a0a 5574 696c 6973 657a 2063 6574 7465  ..Utilisez cette
+000051c0: 2066 6f6e 6374 696f 6e20 706f 7572 2061   fonction pour a
+000051d0: 6a6f 7574 6572 2075 6e65 206c 6f67 6971  jouter une logiq
+000051e0: 7565 2073 7570 706c c3a9 6d65 6e74 6169  ue suppl..mentai
+000051f0: 7265 20c3 a020 766f 7320 666f 726d 756c  re .. vos formul
+00005200: 6169 7265 732e 0a0a 456e 7472 657a 206c  aires...Entrez l
+00005210: 6520 6e6f 6d20 6465 206c 6120 666f 6e63  e nom de la fonc
+00005220: 7469 6f6e 2064 616e 7320 6c65 2063 6861  tion dans le cha
+00005230: 6d70 200a 2246 6f6e 6374 696f 6e20 6427  mp ."Fonction d'
+00005240: 696e 6974 6961 6c69 7361 7469 6f6e 2050  initialisation P
+00005250: 7974 686f 6e22 2e0a 566f 6963 6920 756e  ython"..Voici un
+00005260: 2065 7865 6d70 6c65 3a0a 2222 220a 6672   exemple:.""".fr
+00005270: 6f6d 2071 6769 732e 5079 5174 2e51 7457  om qgis.PyQt.QtW
+00005280: 6964 6765 7473 2069 6d70 6f72 7420 5157  idgets import QW
+00005290: 6964 6765 740a 0a64 6566 206d 795f 666f  idget..def my_fo
+000052a0: 726d 5f6f 7065 6e28 6469 616c 6f67 2c20  rm_open(dialog, 
+000052b0: 6c61 7965 722c 2066 6561 7475 7265 293a  layer, feature):
+000052c0: 0a20 2020 2067 656f 6d20 3d20 6665 6174  .    geom = feat
+000052d0: 7572 652e 6765 6f6d 6574 7279 2829 0a20  ure.geometry(). 
+000052e0: 2020 2063 6f6e 7472 6f6c 203d 2064 6961     control = dia
+000052f0: 6c6f 672e 6669 6e64 4368 696c 6428 5157  log.findChild(QW
+00005300: 6964 6765 742c 2022 4d79 4c69 6e65 4564  idget, "MyLineEd
+00005310: 6974 2229 0a5d 5d3e 3c2f 6564 6974 666f  it").]]></editfo
+00005320: 726d 696e 6974 636f 6465 3e0a 2020 3c66  rminitcode>.  <f
+00005330: 6561 7466 6f72 6d73 7570 7072 6573 733e  eatformsuppress>
+00005340: 303c 2f66 6561 7466 6f72 6d73 7570 7072  0</featformsuppr
+00005350: 6573 733e 0a20 203c 6564 6974 6f72 6c61  ess>.  <editorla
+00005360: 796f 7574 3e67 656e 6572 6174 6564 6c61  yout>generatedla
+00005370: 796f 7574 3c2f 6564 6974 6f72 6c61 796f  yout</editorlayo
+00005380: 7574 3e0a 2020 3c65 6469 7461 626c 653e  ut>.  <editable>
+00005390: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+000053a0: 3d22 616e 676c 6522 2065 6469 7461 626c  ="angle" editabl
+000053b0: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
+000053c0: 6c64 206e 616d 653d 2266 6964 2220 6564  ld name="fid" ed
+000053d0: 6974 6162 6c65 3d22 3122 2f3e 0a20 2020  itable="1"/>.   
+000053e0: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
+000053f0: 6e65 5f6f 7269 656e 7461 7469 6f6e 2220  ne_orientation" 
+00005400: 6564 6974 6162 6c65 3d22 3122 2f3e 0a20  editable="1"/>. 
+00005410: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00005420: 6c61 6e65 5f77 6964 7468 2220 6564 6974  lane_width" edit
+00005430: 6162 6c65 3d22 3122 2f3e 0a20 2020 203c  able="1"/>.    <
+00005440: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
+00005450: 6e74 6174 696f 6e22 2065 6469 7461 626c  ntation" editabl
+00005460: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
+00005470: 6c64 206e 616d 653d 226f 7269 656e 7461  ld name="orienta
+00005480: 7469 6f6e 5f63 6f6e 6669 6465 6e63 6522  tion_confidence"
+00005490: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
+000054a0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+000054b0: 226f 736d 5f69 6422 2065 6469 7461 626c  "osm_id" editabl
+000054c0: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
+000054d0: 6c64 206e 616d 653d 2274 7970 6522 2065  ld name="type" e
+000054e0: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+000054f0: 3c2f 6564 6974 6162 6c65 3e0a 2020 3c6c  </editable>.  <l
+00005500: 6162 656c 4f6e 546f 703e 0a20 2020 203c  abelOnTop>.    <
+00005510: 6669 656c 6420 6e61 6d65 3d22 616e 676c  field name="angl
+00005520: 6522 206c 6162 656c 4f6e 546f 703d 2230  e" labelOnTop="0
+00005530: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
+00005540: 616d 653d 2266 6964 2220 6c61 6265 6c4f  ame="fid" labelO
+00005550: 6e54 6f70 3d22 3022 2f3e 0a20 2020 203c  nTop="0"/>.    <
+00005560: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
+00005570: 5f6f 7269 656e 7461 7469 6f6e 2220 6c61  _orientation" la
+00005580: 6265 6c4f 6e54 6f70 3d22 3022 2f3e 0a20  belOnTop="0"/>. 
+00005590: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+000055a0: 6c61 6e65 5f77 6964 7468 2220 6c61 6265  lane_width" labe
+000055b0: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
+000055c0: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
+000055d0: 6965 6e74 6174 696f 6e22 206c 6162 656c  ientation" label
+000055e0: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
+000055f0: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
+00005600: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
+00005610: 6e63 6522 206c 6162 656c 4f6e 546f 703d  nce" labelOnTop=
+00005620: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
+00005630: 206e 616d 653d 226f 736d 5f69 6422 206c   name="osm_id" l
+00005640: 6162 656c 4f6e 546f 703d 2230 222f 3e0a  abelOnTop="0"/>.
+00005650: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00005660: 2274 7970 6522 206c 6162 656c 4f6e 546f  "type" labelOnTo
+00005670: 703d 2230 222f 3e0a 2020 3c2f 6c61 6265  p="0"/>.  </labe
+00005680: 6c4f 6e54 6f70 3e0a 2020 3c72 6575 7365  lOnTop>.  <reuse
+00005690: 4c61 7374 5661 6c75 653e 0a20 2020 203c  LastValue>.    <
+000056a0: 6669 656c 6420 6e61 6d65 3d22 616e 676c  field name="angl
+000056b0: 6522 2072 6575 7365 4c61 7374 5661 6c75  e" reuseLastValu
+000056c0: 653d 2230 222f 3e0a 2020 2020 3c66 6965  e="0"/>.    <fie
+000056d0: 6c64 206e 616d 653d 2266 6964 2220 7265  ld name="fid" re
+000056e0: 7573 654c 6173 7456 616c 7565 3d22 3022  useLastValue="0"
+000056f0: 2f3e 0a20 2020 203c 6669 656c 6420 6e61  />.    <field na
+00005700: 6d65 3d22 6c61 6e65 5f6f 7269 656e 7461  me="lane_orienta
+00005710: 7469 6f6e 2220 7265 7573 654c 6173 7456  tion" reuseLastV
+00005720: 616c 7565 3d22 3022 2f3e 0a20 2020 203c  alue="0"/>.    <
+00005730: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
+00005740: 5f77 6964 7468 2220 7265 7573 654c 6173  _width" reuseLas
+00005750: 7456 616c 7565 3d22 3022 2f3e 0a20 2020  tValue="0"/>.   
+00005760: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
+00005770: 6965 6e74 6174 696f 6e22 2072 6575 7365  ientation" reuse
+00005780: 4c61 7374 5661 6c75 653d 2230 222f 3e0a  LastValue="0"/>.
+00005790: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+000057a0: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
+000057b0: 6669 6465 6e63 6522 2072 6575 7365 4c61  fidence" reuseLa
+000057c0: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+000057d0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+000057e0: 736d 5f69 6422 2072 6575 7365 4c61 7374  sm_id" reuseLast
+000057f0: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
+00005800: 3c66 6965 6c64 206e 616d 653d 2274 7970  <field name="typ
+00005810: 6522 2072 6575 7365 4c61 7374 5661 6c75  e" reuseLastValu
+00005820: 653d 2230 222f 3e0a 2020 3c2f 7265 7573  e="0"/>.  </reus
+00005830: 654c 6173 7456 616c 7565 3e0a 2020 3c64  eLastValue>.  <d
+00005840: 6174 6144 6566 696e 6564 4669 656c 6450  ataDefinedFieldP
+00005850: 726f 7065 7274 6965 732f 3e0a 2020 3c77  roperties/>.  <w
+00005860: 6964 6765 7473 2f3e 0a20 203c 7072 6576  idgets/>.  <prev
+00005870: 6965 7745 7870 7265 7373 696f 6e3e 2274  iewExpression>"t
+00005880: 7970 6522 3c2f 7072 6576 6965 7745 7870  ype"</previewExp
+00005890: 7265 7373 696f 6e3e 0a20 203c 6d61 7054  ression>.  <mapT
+000058a0: 6970 3e3c 2f6d 6170 5469 703e 0a20 203c  ip></mapTip>.  <
+000058b0: 6c61 7965 7247 656f 6d65 7472 7954 7970  layerGeometryTyp
+000058c0: 653e 303c 2f6c 6179 6572 4765 6f6d 6574  e>0</layerGeomet
+000058d0: 7279 5479 7065 3e0a 3c2f 7167 6973 3e0a  ryType>.</qgis>.
```

### Comparing `crossroads-schematization-0.0.7/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-crossings.qml`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 00000000: 3c21 444f 4354 5950 4520 7167 6973 2050  <!DOCTYPE qgis P
 00000010: 5542 4c49 4320 2768 7474 703a 2f2f 6d72  UBLIC 'http://mr
 00000020: 6363 2e63 6f6d 2f71 6769 732e 6474 6427  cc.com/qgis.dtd'
 00000030: 2027 5359 5354 454d 273e 0a3c 7167 6973   'SYSTEM'>.<qgis
-00000040: 206c 6162 656c 7345 6e61 626c 6564 3d22   labelsEnabled="
-00000050: 3022 2073 696d 706c 6966 7941 6c67 6f72  0" simplifyAlgor
-00000060: 6974 686d 3d22 3022 2073 696d 706c 6966  ithm="0" simplif
-00000070: 794d 6178 5363 616c 653d 2231 2220 7369  yMaxScale="1" si
-00000080: 6d70 6c69 6679 4c6f 6361 6c3d 2231 2220  mplifyLocal="1" 
-00000090: 6d61 7853 6361 6c65 3d22 3022 2068 6173  maxScale="0" has
-000000a0: 5363 616c 6542 6173 6564 5669 7369 6269  ScaleBasedVisibi
-000000b0: 6c69 7479 466c 6167 3d22 3022 206d 696e  lityFlag="0" min
-000000c0: 5363 616c 653d 2231 3030 3030 3030 3030  Scale="100000000
-000000d0: 2220 7369 6d70 6c69 6679 4472 6177 696e  " simplifyDrawin
-000000e0: 6748 696e 7473 3d22 3022 2073 796d 626f  gHints="0" symbo
-000000f0: 6c6f 6779 5265 6665 7265 6e63 6553 6361  logyReferenceSca
-00000100: 6c65 3d22 2d31 2220 7265 6164 4f6e 6c79  le="-1" readOnly
-00000110: 3d22 3022 2073 696d 706c 6966 7944 7261  ="0" simplifyDra
-00000120: 7769 6e67 546f 6c3d 2231 2220 7665 7273  wingTol="1" vers
-00000130: 696f 6e3d 2233 2e32 382e 302d 4669 7265  ion="3.28.0-Fire
-00000140: 6e7a 6522 2073 7479 6c65 4361 7465 676f  nze" styleCatego
-00000150: 7269 6573 3d22 416c 6c53 7479 6c65 4361  ries="AllStyleCa
-00000160: 7465 676f 7269 6573 223e 0a20 203c 666c  tegories">.  <fl
+00000040: 206d 696e 5363 616c 653d 2231 3030 3030   minScale="10000
+00000050: 3030 3030 2220 7369 6d70 6c69 6679 4c6f  0000" simplifyLo
+00000060: 6361 6c3d 2231 2220 7369 6d70 6c69 6679  cal="1" simplify
+00000070: 416c 676f 7269 7468 6d3d 2230 2220 7379  Algorithm="0" sy
+00000080: 6d62 6f6c 6f67 7952 6566 6572 656e 6365  mbologyReference
+00000090: 5363 616c 653d 222d 3122 2068 6173 5363  Scale="-1" hasSc
+000000a0: 616c 6542 6173 6564 5669 7369 6269 6c69  aleBasedVisibili
+000000b0: 7479 466c 6167 3d22 3022 2073 696d 706c  tyFlag="0" simpl
+000000c0: 6966 794d 6178 5363 616c 653d 2231 2220  ifyMaxScale="1" 
+000000d0: 7265 6164 4f6e 6c79 3d22 3022 2076 6572  readOnly="0" ver
+000000e0: 7369 6f6e 3d22 332e 3238 2e32 2d46 6972  sion="3.28.2-Fir
+000000f0: 656e 7a65 2220 7369 6d70 6c69 6679 4472  enze" simplifyDr
+00000100: 6177 696e 6754 6f6c 3d22 3122 206c 6162  awingTol="1" lab
+00000110: 656c 7345 6e61 626c 6564 3d22 3022 206d  elsEnabled="0" m
+00000120: 6178 5363 616c 653d 2230 2220 7374 796c  axScale="0" styl
+00000130: 6543 6174 6567 6f72 6965 733d 2241 6c6c  eCategories="All
+00000140: 5374 796c 6543 6174 6567 6f72 6965 7322  StyleCategories"
+00000150: 2073 696d 706c 6966 7944 7261 7769 6e67   simplifyDrawing
+00000160: 4869 6e74 733d 2230 223e 0a20 203c 666c  Hints="0">.  <fl
 00000170: 6167 733e 0a20 2020 203c 4964 656e 7469  ags>.    <Identi
 00000180: 6669 6162 6c65 3e31 3c2f 4964 656e 7469  fiable>1</Identi
 00000190: 6669 6162 6c65 3e0a 2020 2020 3c52 656d  fiable>.    <Rem
 000001a0: 6f76 6162 6c65 3e31 3c2f 5265 6d6f 7661  ovable>1</Remova
 000001b0: 626c 653e 0a20 2020 203c 5365 6172 6368  ble>.    <Search
 000001c0: 6162 6c65 3e31 3c2f 5365 6172 6368 6162  able>1</Searchab
 000001d0: 6c65 3e0a 2020 2020 3c50 7269 7661 7465  le>.    <Private
 000001e0: 3e30 3c2f 5072 6976 6174 653e 0a20 203c  >0</Private>.  <
 000001f0: 2f66 6c61 6773 3e0a 2020 3c74 656d 706f  /flags>.  <tempo
 00000200: 7261 6c20 6669 7865 6444 7572 6174 696f  ral fixedDuratio
-00000210: 6e3d 2230 2220 6c69 6d69 744d 6f64 653d  n="0" limitMode=
-00000220: 2230 2220 6475 7261 7469 6f6e 556e 6974  "0" durationUnit
-00000230: 3d22 6d69 6e22 2065 6e64 4669 656c 643d  ="min" endField=
-00000240: 2222 2065 6e61 626c 6564 3d22 3022 2065  "" enabled="0" e
-00000250: 6e64 4578 7072 6573 7369 6f6e 3d22 2220  ndExpression="" 
-00000260: 6475 7261 7469 6f6e 4669 656c 643d 2222  durationField=""
-00000270: 2061 6363 756d 756c 6174 653d 2230 2220   accumulate="0" 
-00000280: 7374 6172 7446 6965 6c64 3d22 2220 7374  startField="" st
-00000290: 6172 7445 7870 7265 7373 696f 6e3d 2222  artExpression=""
-000002a0: 206d 6f64 653d 2230 223e 0a20 2020 203c   mode="0">.    <
+00000210: 6e3d 2230 2220 6d6f 6465 3d22 3022 2065  n="0" mode="0" e
+00000220: 6e64 4578 7072 6573 7369 6f6e 3d22 2220  ndExpression="" 
+00000230: 6c69 6d69 744d 6f64 653d 2230 2220 7374  limitMode="0" st
+00000240: 6172 7446 6965 6c64 3d22 2220 656e 6446  artField="" endF
+00000250: 6965 6c64 3d22 2220 6475 7261 7469 6f6e  ield="" duration
+00000260: 556e 6974 3d22 6d69 6e22 2061 6363 756d  Unit="min" accum
+00000270: 756c 6174 653d 2230 2220 7374 6172 7445  ulate="0" startE
+00000280: 7870 7265 7373 696f 6e3d 2222 2064 7572  xpression="" dur
+00000290: 6174 696f 6e46 6965 6c64 3d22 2220 656e  ationField="" en
+000002a0: 6162 6c65 643d 2230 223e 0a20 2020 203c  abled="0">.    <
 000002b0: 6669 7865 6452 616e 6765 3e0a 2020 2020  fixedRange>.    
 000002c0: 2020 3c73 7461 7274 3e3c 2f73 7461 7274    <start></start
 000002d0: 3e0a 2020 2020 2020 3c65 6e64 3e3c 2f65  >.      <end></e
 000002e0: 6e64 3e0a 2020 2020 3c2f 6669 7865 6452  nd>.    </fixedR
 000002f0: 616e 6765 3e0a 2020 3c2f 7465 6d70 6f72  ange>.  </tempor
 00000300: 616c 3e0a 2020 3c65 6c65 7661 7469 6f6e  al>.  <elevation
-00000310: 2065 7874 7275 7369 6f6e 3d22 3022 2072   extrusion="0" r
-00000320: 6573 7065 6374 4c61 7965 7253 796d 626f  espectLayerSymbo
-00000330: 6c3d 2231 2220 7379 6d62 6f6c 6f67 793d  l="1" symbology=
-00000340: 224c 696e 6522 2063 6c61 6d70 696e 673d  "Line" clamping=
-00000350: 2254 6572 7261 696e 2220 7a6f 6666 7365  "Terrain" zoffse
-00000360: 743d 2230 2220 7a73 6361 6c65 3d22 3122  t="0" zscale="1"
-00000370: 2062 696e 6469 6e67 3d22 4365 6e74 726f   binding="Centro
-00000380: 6964 2220 7479 7065 3d22 496e 6469 7669  id" type="Indivi
-00000390: 6475 616c 4665 6174 7572 6573 2220 6578  dualFeatures" ex
-000003a0: 7472 7573 696f 6e45 6e61 626c 6564 3d22  trusionEnabled="
-000003b0: 3022 2073 686f 774d 6172 6b65 7253 796d  0" showMarkerSym
-000003c0: 626f 6c49 6e53 7572 6661 6365 506c 6f74  bolInSurfacePlot
-000003d0: 733d 2230 223e 0a20 2020 203c 6461 7461  s="0">.    <data
+00000310: 207a 7363 616c 653d 2231 2220 6578 7472   zscale="1" extr
+00000320: 7573 696f 6e45 6e61 626c 6564 3d22 3022  usionEnabled="0"
+00000330: 2062 696e 6469 6e67 3d22 4365 6e74 726f   binding="Centro
+00000340: 6964 2220 7265 7370 6563 744c 6179 6572  id" respectLayer
+00000350: 5379 6d62 6f6c 3d22 3122 2073 686f 774d  Symbol="1" showM
+00000360: 6172 6b65 7253 796d 626f 6c49 6e53 7572  arkerSymbolInSur
+00000370: 6661 6365 506c 6f74 733d 2230 2220 636c  facePlots="0" cl
+00000380: 616d 7069 6e67 3d22 5465 7272 6169 6e22  amping="Terrain"
+00000390: 2065 7874 7275 7369 6f6e 3d22 3022 207a   extrusion="0" z
+000003a0: 6f66 6673 6574 3d22 3022 2073 796d 626f  offset="0" symbo
+000003b0: 6c6f 6779 3d22 4c69 6e65 2220 7479 7065  logy="Line" type
+000003c0: 3d22 496e 6469 7669 6475 616c 4665 6174  ="IndividualFeat
+000003d0: 7572 6573 223e 0a20 2020 203c 6461 7461  ures">.    <data
 000003e0: 2d64 6566 696e 6564 2d70 726f 7065 7274  -defined-propert
 000003f0: 6965 733e 0a20 2020 2020 203c 4f70 7469  ies>.      <Opti
 00000400: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
 00000410: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
 00000420: 616d 653d 226e 616d 6522 2076 616c 7565  ame="name" value
 00000430: 3d22 2220 7479 7065 3d22 5153 7472 696e  ="" type="QStrin
 00000440: 6722 2f3e 0a20 2020 2020 2020 203c 4f70  g"/>.        <Op
@@ -74,20 +74,20 @@
 00000490: 6563 7469 6f6e 2220 7479 7065 3d22 5153  ection" type="QS
 000004a0: 7472 696e 6722 2f3e 0a20 2020 2020 203c  tring"/>.      <
 000004b0: 2f4f 7074 696f 6e3e 0a20 2020 203c 2f64  /Option>.    </d
 000004c0: 6174 612d 6465 6669 6e65 642d 7072 6f70  ata-defined-prop
 000004d0: 6572 7469 6573 3e0a 2020 2020 3c70 726f  erties>.    <pro
 000004e0: 6669 6c65 4c69 6e65 5379 6d62 6f6c 3e0a  fileLineSymbol>.
 000004f0: 2020 2020 2020 3c73 796d 626f 6c20 6e61        <symbol na
-00000500: 6d65 3d22 2220 636c 6970 5f74 6f5f 6578  me="" clip_to_ex
-00000510: 7465 6e74 3d22 3122 2066 6f72 6365 5f72  tent="1" force_r
-00000520: 6872 3d22 3022 2069 735f 616e 696d 6174  hr="0" is_animat
-00000530: 6564 3d22 3022 2074 7970 653d 226c 696e  ed="0" type="lin
-00000540: 6522 2061 6c70 6861 3d22 3122 2066 7261  e" alpha="1" fra
-00000550: 6d65 5f72 6174 653d 2231 3022 3e0a 2020  me_rate="10">.  
+00000500: 6d65 3d22 2220 666f 7263 655f 7268 723d  me="" force_rhr=
+00000510: 2230 2220 6672 616d 655f 7261 7465 3d22  "0" frame_rate="
+00000520: 3130 2220 616c 7068 613d 2231 2220 636c  10" alpha="1" cl
+00000530: 6970 5f74 6f5f 6578 7465 6e74 3d22 3122  ip_to_extent="1"
+00000540: 2069 735f 616e 696d 6174 6564 3d22 3022   is_animated="0"
+00000550: 2074 7970 653d 226c 696e 6522 3e0a 2020   type="line">.  
 00000560: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
 00000570: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
 00000580: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
 00000590: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
 000005a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
 000005b0: 6e20 6e61 6d65 3d22 6e61 6d65 2220 7661  n name="name" va
 000005c0: 6c75 653d 2222 2074 7970 653d 2251 5374  lue="" type="QSt
@@ -98,18 +98,18 @@
 00000610: 696f 6e20 6e61 6d65 3d22 7479 7065 2220  ion name="type" 
 00000620: 7661 6c75 653d 2263 6f6c 6c65 6374 696f  value="collectio
 00000630: 6e22 2074 7970 653d 2251 5374 7269 6e67  n" type="QString
 00000640: 222f 3e0a 2020 2020 2020 2020 2020 3c2f  "/>.          </
 00000650: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
 00000660: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
 00000670: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00000680: 2020 203c 6c61 7965 7220 636c 6173 733d     <layer class=
-00000690: 2253 696d 706c 654c 696e 6522 2065 6e61  "SimpleLine" ena
-000006a0: 626c 6564 3d22 3122 206c 6f63 6b65 643d  bled="1" locked=
-000006b0: 2230 2220 7061 7373 3d22 3022 3e0a 2020  "0" pass="0">.  
+00000680: 2020 203c 6c61 7965 7220 7061 7373 3d22     <layer pass="
+00000690: 3022 206c 6f63 6b65 643d 2230 2220 656e  0" locked="0" en
+000006a0: 6162 6c65 643d 2231 2220 636c 6173 733d  abled="1" class=
+000006b0: 2253 696d 706c 654c 696e 6522 3e0a 2020  "SimpleLine">.  
 000006c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
 000006d0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
 000006e0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
 000006f0: 6e61 6d65 3d22 616c 6967 6e5f 6461 7368  name="align_dash
 00000700: 5f70 6174 7465 726e 2220 7661 6c75 653d  _pattern" value=
 00000710: 2230 2220 7479 7065 3d22 5153 7472 696e  "0" type="QStrin
 00000720: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
@@ -260,20 +260,20 @@
 00001030: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
 00001040: 3e0a 2020 2020 2020 2020 3c2f 6c61 7965  >.        </laye
 00001050: 723e 0a20 2020 2020 203c 2f73 796d 626f  r>.      </symbo
 00001060: 6c3e 0a20 2020 203c 2f70 726f 6669 6c65  l>.    </profile
 00001070: 4c69 6e65 5379 6d62 6f6c 3e0a 2020 2020  LineSymbol>.    
 00001080: 3c70 726f 6669 6c65 4669 6c6c 5379 6d62  <profileFillSymb
 00001090: 6f6c 3e0a 2020 2020 2020 3c73 796d 626f  ol>.      <symbo
-000010a0: 6c20 6e61 6d65 3d22 2220 636c 6970 5f74  l name="" clip_t
-000010b0: 6f5f 6578 7465 6e74 3d22 3122 2066 6f72  o_extent="1" for
-000010c0: 6365 5f72 6872 3d22 3022 2069 735f 616e  ce_rhr="0" is_an
-000010d0: 696d 6174 6564 3d22 3022 2074 7970 653d  imated="0" type=
-000010e0: 2266 696c 6c22 2061 6c70 6861 3d22 3122  "fill" alpha="1"
-000010f0: 2066 7261 6d65 5f72 6174 653d 2231 3022   frame_rate="10"
+000010a0: 6c20 6e61 6d65 3d22 2220 666f 7263 655f  l name="" force_
+000010b0: 7268 723d 2230 2220 6672 616d 655f 7261  rhr="0" frame_ra
+000010c0: 7465 3d22 3130 2220 616c 7068 613d 2231  te="10" alpha="1
+000010d0: 2220 636c 6970 5f74 6f5f 6578 7465 6e74  " clip_to_extent
+000010e0: 3d22 3122 2069 735f 616e 696d 6174 6564  ="1" is_animated
+000010f0: 3d22 3022 2074 7970 653d 2266 696c 6c22  ="0" type="fill"
 00001100: 3e0a 2020 2020 2020 2020 3c64 6174 615f  >.        <data_
 00001110: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
 00001120: 6573 3e0a 2020 2020 2020 2020 2020 3c4f  es>.          <O
 00001130: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
 00001140: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
 00001150: 7074 696f 6e20 6e61 6d65 3d22 6e61 6d65  ption name="name
 00001160: 2220 7661 6c75 653d 2222 2074 7970 653d  " value="" type=
@@ -284,18 +284,18 @@
 000011b0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
 000011c0: 7065 2220 7661 6c75 653d 2263 6f6c 6c65  pe" value="colle
 000011d0: 6374 696f 6e22 2074 7970 653d 2251 5374  ction" type="QSt
 000011e0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
 000011f0: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
 00001200: 2020 2020 3c2f 6461 7461 5f64 6566 696e      </data_defin
 00001210: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
-00001220: 2020 2020 2020 203c 6c61 7965 7220 636c         <layer cl
-00001230: 6173 733d 2253 696d 706c 6546 696c 6c22  ass="SimpleFill"
-00001240: 2065 6e61 626c 6564 3d22 3122 206c 6f63   enabled="1" loc
-00001250: 6b65 643d 2230 2220 7061 7373 3d22 3022  ked="0" pass="0"
+00001220: 2020 2020 2020 203c 6c61 7965 7220 7061         <layer pa
+00001230: 7373 3d22 3022 206c 6f63 6b65 643d 2230  ss="0" locked="0
+00001240: 2220 656e 6162 6c65 643d 2231 2220 636c  " enabled="1" cl
+00001250: 6173 733d 2253 696d 706c 6546 696c 6c22  ass="SimpleFill"
 00001260: 3e0a 2020 2020 2020 2020 2020 3c4f 7074  >.          <Opt
 00001270: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
 00001280: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
 00001290: 696f 6e20 6e61 6d65 3d22 626f 7264 6572  ion name="border
 000012a0: 5f77 6964 7468 5f6d 6170 5f75 6e69 745f  _width_map_unit_
 000012b0: 7363 616c 6522 2076 616c 7565 3d22 3378  scale" value="3x
 000012c0: 3a30 2c30 2c30 2c30 2c30 2c30 2220 7479  :0,0,0,0,0,0" ty
@@ -367,21 +367,21 @@
 000016e0: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
 000016f0: 2020 2020 2020 2020 3c2f 6c61 7965 723e          </layer>
 00001700: 0a20 2020 2020 203c 2f73 796d 626f 6c3e  .      </symbol>
 00001710: 0a20 2020 203c 2f70 726f 6669 6c65 4669  .    </profileFi
 00001720: 6c6c 5379 6d62 6f6c 3e0a 2020 2020 3c70  llSymbol>.    <p
 00001730: 726f 6669 6c65 4d61 726b 6572 5379 6d62  rofileMarkerSymb
 00001740: 6f6c 3e0a 2020 2020 2020 3c73 796d 626f  ol>.      <symbo
-00001750: 6c20 6e61 6d65 3d22 2220 636c 6970 5f74  l name="" clip_t
-00001760: 6f5f 6578 7465 6e74 3d22 3122 2066 6f72  o_extent="1" for
-00001770: 6365 5f72 6872 3d22 3022 2069 735f 616e  ce_rhr="0" is_an
-00001780: 696d 6174 6564 3d22 3022 2074 7970 653d  imated="0" type=
-00001790: 226d 6172 6b65 7222 2061 6c70 6861 3d22  "marker" alpha="
-000017a0: 3122 2066 7261 6d65 5f72 6174 653d 2231  1" frame_rate="1
-000017b0: 3022 3e0a 2020 2020 2020 2020 3c64 6174  0">.        <dat
+00001750: 6c20 6e61 6d65 3d22 2220 666f 7263 655f  l name="" force_
+00001760: 7268 723d 2230 2220 6672 616d 655f 7261  rhr="0" frame_ra
+00001770: 7465 3d22 3130 2220 616c 7068 613d 2231  te="10" alpha="1
+00001780: 2220 636c 6970 5f74 6f5f 6578 7465 6e74  " clip_to_extent
+00001790: 3d22 3122 2069 735f 616e 696d 6174 6564  ="1" is_animated
+000017a0: 3d22 3022 2074 7970 653d 226d 6172 6b65  ="0" type="marke
+000017b0: 7222 3e0a 2020 2020 2020 2020 3c64 6174  r">.        <dat
 000017c0: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
 000017d0: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
 000017e0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
 000017f0: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
 00001800: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6e61  <Option name="na
 00001810: 6d65 2220 7661 6c75 653d 2222 2074 7970  me" value="" typ
 00001820: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
@@ -392,18 +392,18 @@
 00001870: 7479 7065 2220 7661 6c75 653d 2263 6f6c  type" value="col
 00001880: 6c65 6374 696f 6e22 2074 7970 653d 2251  lection" type="Q
 00001890: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
 000018a0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
 000018b0: 2020 2020 2020 3c2f 6461 7461 5f64 6566        </data_def
 000018c0: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
 000018d0: 0a20 2020 2020 2020 203c 6c61 7965 7220  .        <layer 
-000018e0: 636c 6173 733d 2253 696d 706c 654d 6172  class="SimpleMar
-000018f0: 6b65 7222 2065 6e61 626c 6564 3d22 3122  ker" enabled="1"
-00001900: 206c 6f63 6b65 643d 2230 2220 7061 7373   locked="0" pass
-00001910: 3d22 3022 3e0a 2020 2020 2020 2020 2020  ="0">.          
+000018e0: 7061 7373 3d22 3022 206c 6f63 6b65 643d  pass="0" locked=
+000018f0: 2230 2220 656e 6162 6c65 643d 2231 2220  "0" enabled="1" 
+00001900: 636c 6173 733d 2253 696d 706c 654d 6172  class="SimpleMar
+00001910: 6b65 7222 3e0a 2020 2020 2020 2020 2020  ker">.          
 00001920: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
 00001930: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
 00001940: 3c4f 7074 696f 6e20 6e61 6d65 3d22 616e  <Option name="an
 00001950: 676c 6522 2076 616c 7565 3d22 3022 2074  gle" value="0" t
 00001960: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
 00001970: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
 00001980: 696f 6e20 6e61 6d65 3d22 6361 705f 7374  ion name="cap_st
@@ -509,954 +509,1319 @@
 00001fc0: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
 00001fd0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
 00001fe0: 2020 2020 2020 3c2f 6c61 7965 723e 0a20        </layer>. 
 00001ff0: 2020 2020 203c 2f73 796d 626f 6c3e 0a20       </symbol>. 
 00002000: 2020 203c 2f70 726f 6669 6c65 4d61 726b     </profileMark
 00002010: 6572 5379 6d62 6f6c 3e0a 2020 3c2f 656c  erSymbol>.  </el
 00002020: 6576 6174 696f 6e3e 0a20 203c 7265 6e64  evation>.  <rend
-00002030: 6572 6572 2d76 3220 7379 6d62 6f6c 6c65  erer-v2 symbolle
-00002040: 7665 6c73 3d22 3022 2072 6566 6572 656e  vels="0" referen
-00002050: 6365 7363 616c 653d 222d 3122 2066 6f72  cescale="-1" for
-00002060: 6365 7261 7374 6572 3d22 3022 2065 6e61  ceraster="0" ena
-00002070: 626c 656f 7264 6572 6279 3d22 3022 2074  bleorderby="0" t
-00002080: 7970 653d 2252 756c 6552 656e 6465 7265  ype="RuleRendere
-00002090: 7222 3e0a 2020 2020 3c72 756c 6573 206b  r">.    <rules k
+00002030: 6572 6572 2d76 3220 666f 7263 6572 6173  erer-v2 forceras
+00002040: 7465 723d 2230 2220 7379 6d62 6f6c 6c65  ter="0" symbolle
+00002050: 7665 6c73 3d22 3022 2072 6566 6572 656e  vels="0" referen
+00002060: 6365 7363 616c 653d 222d 3122 2074 7970  cescale="-1" typ
+00002070: 653d 2252 756c 6552 656e 6465 7265 7222  e="RuleRenderer"
+00002080: 2065 6e61 626c 656f 7264 6572 6279 3d22   enableorderby="
+00002090: 3022 3e0a 2020 2020 3c72 756c 6573 206b  0">.    <rules k
 000020a0: 6579 3d22 7b31 6163 6338 3136 392d 3632  ey="{1acc8169-62
 000020b0: 3230 2d34 6161 352d 6264 3661 2d38 3831  20-4aa5-bd6a-881
 000020c0: 3739 6264 6466 6666 637d 223e 0a20 2020  79bddfffc}">.   
 000020d0: 2020 203c 7275 6c65 2073 796d 626f 6c3d     <rule symbol=
-000020e0: 2230 2220 6b65 793d 227b 3536 3333 3937  "0" key="{563397
-000020f0: 3363 2d64 6336 332d 3432 3264 2d39 6135  3c-dc63-422d-9a5
-00002100: 312d 3933 3964 6532 3662 3831 3365 7d22  1-939de26b813e}"
+000020e0: 2230 2220 6b65 793d 227b 6635 3939 3765  "0" key="{f5997e
+000020f0: 6665 2d64 6635 312d 3435 3339 2d38 6130  fe-df51-4539-8a0
+00002100: 312d 3331 3666 6238 3532 6339 3136 7d22  1-316fb852c916}"
 00002110: 2066 696c 7465 723d 2226 7175 6f74 3b74   filter="&quot;t
-00002120: 7970 6526 7175 6f74 3b20 3d20 2774 7261  ype&quot; = 'tra
-00002130: 6666 6963 5f69 736c 616e 6427 222f 3e0a  ffic_island'"/>.
-00002140: 2020 2020 2020 3c72 756c 6520 7379 6d62        <rule symb
-00002150: 6f6c 3d22 3122 206b 6579 3d22 7b62 6239  ol="1" key="{bb9
-00002160: 3934 3933 652d 3435 3734 2d34 3134 332d  9493e-4574-4143-
-00002170: 6162 3335 2d63 3036 3162 6139 6666 6534  ab35-c061ba9ffe4
-00002180: 667d 2220 6669 6c74 6572 3d22 2671 756f  f}" filter="&quo
-00002190: 743b 7479 7065 2671 756f 743b 3d27 6372  t;type&quot;='cr
-000021a0: 6f73 7369 6e67 2722 2f3e 0a20 2020 203c  ossing'"/>.    <
-000021b0: 2f72 756c 6573 3e0a 2020 2020 3c73 796d  /rules>.    <sym
-000021c0: 626f 6c73 3e0a 2020 2020 2020 3c73 796d  bols>.      <sym
-000021d0: 626f 6c20 6e61 6d65 3d22 3022 2063 6c69  bol name="0" cli
-000021e0: 705f 746f 5f65 7874 656e 743d 2231 2220  p_to_extent="1" 
-000021f0: 666f 7263 655f 7268 723d 2230 2220 6973  force_rhr="0" is
-00002200: 5f61 6e69 6d61 7465 643d 2230 2220 7479  _animated="0" ty
-00002210: 7065 3d22 6d61 726b 6572 2220 616c 7068  pe="marker" alph
-00002220: 613d 2231 2220 6672 616d 655f 7261 7465  a="1" frame_rate
-00002230: 3d22 3130 223e 0a20 2020 2020 2020 203c  ="10">.        <
-00002240: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-00002250: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-00002260: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00002270: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00002280: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00002290: 226e 616d 6522 2076 616c 7565 3d22 2220  "name" value="" 
-000022a0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-000022b0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-000022c0: 7469 6f6e 206e 616d 653d 2270 726f 7065  tion name="prope
-000022d0: 7274 6965 7322 2f3e 0a20 2020 2020 2020  rties"/>.       
-000022e0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-000022f0: 653d 2274 7970 6522 2076 616c 7565 3d22  e="type" value="
-00002300: 636f 6c6c 6563 7469 6f6e 2220 7479 7065  collection" type
-00002310: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002320: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
-00002330: 0a20 2020 2020 2020 203c 2f64 6174 615f  .        </data_
-00002340: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
-00002350: 6573 3e0a 2020 2020 2020 2020 3c6c 6179  es>.        <lay
-00002360: 6572 2063 6c61 7373 3d22 5369 6d70 6c65  er class="Simple
-00002370: 4d61 726b 6572 2220 656e 6162 6c65 643d  Marker" enabled=
-00002380: 2231 2220 6c6f 636b 6564 3d22 3022 2070  "1" locked="0" p
-00002390: 6173 733d 2230 223e 0a20 2020 2020 2020  ass="0">.       
-000023a0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-000023b0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-000023c0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-000023d0: 2261 6e67 6c65 2220 7661 6c75 653d 2230  "angle" value="0
-000023e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000023f0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00002400: 4f70 7469 6f6e 206e 616d 653d 2263 6170  Option name="cap
-00002410: 5f73 7479 6c65 2220 7661 6c75 653d 2273  _style" value="s
-00002420: 7175 6172 6522 2074 7970 653d 2251 5374  quare" type="QSt
-00002430: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002440: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00002450: 3d22 636f 6c6f 7222 2076 616c 7565 3d22  ="color" value="
-00002460: 302c 302c 302c 3235 3522 2074 7970 653d  0,0,0,255" type=
-00002470: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00002480: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002490: 6e61 6d65 3d22 686f 7269 7a6f 6e74 616c  name="horizontal
-000024a0: 5f61 6e63 686f 725f 706f 696e 7422 2076  _anchor_point" v
-000024b0: 616c 7565 3d22 3122 2074 7970 653d 2251  alue="1" type="Q
-000024c0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-000024d0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-000024e0: 6d65 3d22 6a6f 696e 7374 796c 6522 2076  me="joinstyle" v
-000024f0: 616c 7565 3d22 6265 7665 6c22 2074 7970  alue="bevel" typ
-00002500: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002510: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002520: 6e20 6e61 6d65 3d22 6e61 6d65 2220 7661  n name="name" va
-00002530: 6c75 653d 2263 6972 636c 6522 2074 7970  lue="circle" typ
-00002540: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002550: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002560: 6e20 6e61 6d65 3d22 6f66 6673 6574 2220  n name="offset" 
-00002570: 7661 6c75 653d 2230 2c30 2220 7479 7065  value="0,0" type
-00002580: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002590: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000025a0: 206e 616d 653d 226f 6666 7365 745f 6d61   name="offset_ma
-000025b0: 705f 756e 6974 5f73 6361 6c65 2220 7661  p_unit_scale" va
-000025c0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-000025d0: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-000025e0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-000025f0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00002600: 6f66 6673 6574 5f75 6e69 7422 2076 616c  offset_unit" val
-00002610: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
-00002620: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002630: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00002640: 653d 226f 7574 6c69 6e65 5f63 6f6c 6f72  e="outline_color
-00002650: 2220 7661 6c75 653d 2233 352c 3335 2c33  " value="35,35,3
-00002660: 352c 3235 3522 2074 7970 653d 2251 5374  5,255" type="QSt
-00002670: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002680: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00002690: 3d22 6f75 746c 696e 655f 7374 796c 6522  ="outline_style"
-000026a0: 2076 616c 7565 3d22 736f 6c69 6422 2074   value="solid" t
-000026b0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000026c0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000026d0: 696f 6e20 6e61 6d65 3d22 6f75 746c 696e  ion name="outlin
-000026e0: 655f 7769 6474 6822 2076 616c 7565 3d22  e_width" value="
-000026f0: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00002700: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002710: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
-00002720: 746c 696e 655f 7769 6474 685f 6d61 705f  tline_width_map_
-00002730: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
-00002740: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00002750: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
-00002760: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002770: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
-00002780: 746c 696e 655f 7769 6474 685f 756e 6974  tline_width_unit
-00002790: 2220 7661 6c75 653d 224d 4d22 2074 7970  " value="MM" typ
-000027a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000027b0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000027c0: 6e20 6e61 6d65 3d22 7363 616c 655f 6d65  n name="scale_me
-000027d0: 7468 6f64 2220 7661 6c75 653d 2264 6961  thod" value="dia
-000027e0: 6d65 7465 7222 2074 7970 653d 2251 5374  meter" type="QSt
-000027f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002800: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00002810: 3d22 7369 7a65 2220 7661 6c75 653d 2236  ="size" value="6
-00002820: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00002830: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00002840: 4f70 7469 6f6e 206e 616d 653d 2273 697a  Option name="siz
-00002850: 655f 6d61 705f 756e 6974 5f73 6361 6c65  e_map_unit_scale
-00002860: 2220 7661 6c75 653d 2233 783a 302c 302c  " value="3x:0,0,
-00002870: 302c 302c 302c 3022 2074 7970 653d 2251  0,0,0,0" type="Q
-00002880: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00002890: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-000028a0: 6d65 3d22 7369 7a65 5f75 6e69 7422 2076  me="size_unit" v
-000028b0: 616c 7565 3d22 4d4d 2220 7479 7065 3d22  alue="MM" type="
-000028c0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-000028d0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-000028e0: 616d 653d 2276 6572 7469 6361 6c5f 616e  ame="vertical_an
-000028f0: 6368 6f72 5f70 6f69 6e74 2220 7661 6c75  chor_point" valu
-00002900: 653d 2231 2220 7479 7065 3d22 5153 7472  e="1" type="QStr
-00002910: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00002920: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
-00002930: 2020 2020 203c 6461 7461 5f64 6566 696e       <data_defin
-00002940: 6564 5f70 726f 7065 7274 6965 733e 0a20  ed_properties>. 
+00002120: 7970 6526 7175 6f74 3b3d 2763 726f 7373  ype&quot;='cross
+00002130: 696e 6727 222f 3e0a 2020 2020 2020 3c72  ing'"/>.      <r
+00002140: 756c 6520 7379 6d62 6f6c 3d22 3122 206b  ule symbol="1" k
+00002150: 6579 3d22 7b34 3532 3262 3735 322d 3564  ey="{4522b752-5d
+00002160: 6231 2d34 3136 332d 6266 3561 2d32 6464  b1-4163-bf5a-2dd
+00002170: 6433 6434 3539 6334 327d 2220 6669 6c74  d3d459c42}" filt
+00002180: 6572 3d22 2671 756f 743b 7479 7065 2671  er="&quot;type&q
+00002190: 756f 743b 3d27 6372 6f73 7369 6e67 2722  uot;='crossing'"
+000021a0: 2073 6361 6c65 6d61 7864 656e 6f6d 3d22   scalemaxdenom="
+000021b0: 3130 3030 3030 2220 7363 616c 656d 696e  100000" scalemin
+000021c0: 6465 6e6f 6d3d 2233 3030 222f 3e0a 2020  denom="300"/>.  
+000021d0: 2020 2020 3c72 756c 6520 7379 6d62 6f6c      <rule symbol
+000021e0: 3d22 3222 206b 6579 3d22 7b35 3164 3964  ="2" key="{51d9d
+000021f0: 3730 372d 3161 6365 2d34 6262 392d 3837  707-1ace-4bb9-87
+00002200: 6365 2d31 6562 6366 6265 3463 6163 347d  ce-1ebcfbe4cac4}
+00002210: 2220 6669 6c74 6572 3d22 2671 756f 743b  " filter="&quot;
+00002220: 7479 7065 2671 756f 743b 3d27 6372 6f73  type&quot;='cros
+00002230: 7369 6e67 2722 2073 6361 6c65 6d61 7864  sing'" scalemaxd
+00002240: 656e 6f6d 3d22 3330 3022 2073 6361 6c65  enom="300" scale
+00002250: 6d69 6e64 656e 6f6d 3d22 3122 2f3e 0a20  mindenom="1"/>. 
+00002260: 2020 203c 2f72 756c 6573 3e0a 2020 2020     </rules>.    
+00002270: 3c73 796d 626f 6c73 3e0a 2020 2020 2020  <symbols>.      
+00002280: 3c73 796d 626f 6c20 6e61 6d65 3d22 3022  <symbol name="0"
+00002290: 2066 6f72 6365 5f72 6872 3d22 3022 2066   force_rhr="0" f
+000022a0: 7261 6d65 5f72 6174 653d 2231 3022 2061  rame_rate="10" a
+000022b0: 6c70 6861 3d22 3122 2063 6c69 705f 746f  lpha="1" clip_to
+000022c0: 5f65 7874 656e 743d 2231 2220 6973 5f61  _extent="1" is_a
+000022d0: 6e69 6d61 7465 643d 2230 2220 7479 7065  nimated="0" type
+000022e0: 3d22 6d61 726b 6572 223e 0a20 2020 2020  ="marker">.     
+000022f0: 2020 203c 6461 7461 5f64 6566 696e 6564     <data_defined
+00002300: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
+00002310: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00002320: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00002330: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00002340: 616d 653d 226e 616d 6522 2076 616c 7565  ame="name" value
+00002350: 3d22 2220 7479 7065 3d22 5153 7472 696e  ="" type="QStrin
+00002360: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00002370: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00002380: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
+00002390: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000023a0: 206e 616d 653d 2274 7970 6522 2076 616c   name="type" val
+000023b0: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
+000023c0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000023d0: 0a20 2020 2020 2020 2020 203c 2f4f 7074  .          </Opt
+000023e0: 696f 6e3e 0a20 2020 2020 2020 203c 2f64  ion>.        </d
+000023f0: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+00002400: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+00002410: 3c6c 6179 6572 2070 6173 733d 2230 2220  <layer pass="0" 
+00002420: 6c6f 636b 6564 3d22 3022 2065 6e61 626c  locked="0" enabl
+00002430: 6564 3d22 3122 2063 6c61 7373 3d22 5369  ed="1" class="Si
+00002440: 6d70 6c65 4d61 726b 6572 223e 0a20 2020  mpleMarker">.   
+00002450: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
+00002460: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+00002470: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00002480: 616d 653d 2261 6e67 6c65 2220 7661 6c75  ame="angle" valu
+00002490: 653d 2230 2220 7479 7065 3d22 5153 7472  e="0" type="QStr
+000024a0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000024b0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+000024c0: 2263 6170 5f73 7479 6c65 2220 7661 6c75  "cap_style" valu
+000024d0: 653d 2266 6c61 7422 2074 7970 653d 2251  e="flat" type="Q
+000024e0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000024f0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00002500: 6d65 3d22 636f 6c6f 7222 2076 616c 7565  me="color" value
+00002510: 3d22 3134 352c 3832 2c34 352c 3235 3522  ="145,82,45,255"
+00002520: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00002530: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00002540: 7074 696f 6e20 6e61 6d65 3d22 686f 7269  ption name="hori
+00002550: 7a6f 6e74 616c 5f61 6e63 686f 725f 706f  zontal_anchor_po
+00002560: 696e 7422 2076 616c 7565 3d22 3122 2074  int" value="1" t
+00002570: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00002580: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00002590: 696f 6e20 6e61 6d65 3d22 6a6f 696e 7374  ion name="joinst
+000025a0: 796c 6522 2076 616c 7565 3d22 6d69 7465  yle" value="mite
+000025b0: 7222 2074 7970 653d 2251 5374 7269 6e67  r" type="QString
+000025c0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000025d0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6e61  <Option name="na
+000025e0: 6d65 2220 7661 6c75 653d 226c 696e 6522  me" value="line"
+000025f0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00002600: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00002610: 7074 696f 6e20 6e61 6d65 3d22 6f66 6673  ption name="offs
+00002620: 6574 2220 7661 6c75 653d 2230 2c30 2220  et" value="0,0" 
+00002630: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00002640: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00002650: 7469 6f6e 206e 616d 653d 226f 6666 7365  tion name="offse
+00002660: 745f 6d61 705f 756e 6974 5f73 6361 6c65  t_map_unit_scale
+00002670: 2220 7661 6c75 653d 2233 783a 302c 302c  " value="3x:0,0,
+00002680: 302c 302c 302c 3022 2074 7970 653d 2251  0,0,0,0" type="Q
+00002690: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000026a0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+000026b0: 6d65 3d22 6f66 6673 6574 5f75 6e69 7422  me="offset_unit"
+000026c0: 2076 616c 7565 3d22 4d4d 2220 7479 7065   value="MM" type
+000026d0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000026e0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000026f0: 206e 616d 653d 226f 7574 6c69 6e65 5f63   name="outline_c
+00002700: 6f6c 6f72 2220 7661 6c75 653d 2230 2c30  olor" value="0,0
+00002710: 2c30 2c32 3535 2220 7479 7065 3d22 5153  ,0,255" type="QS
+00002720: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002730: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00002740: 653d 226f 7574 6c69 6e65 5f73 7479 6c65  e="outline_style
+00002750: 2220 7661 6c75 653d 2273 6f6c 6964 2220  " value="solid" 
+00002760: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00002770: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00002780: 7469 6f6e 206e 616d 653d 226f 7574 6c69  tion name="outli
+00002790: 6e65 5f77 6964 7468 2220 7661 6c75 653d  ne_width" value=
+000027a0: 2232 2220 7479 7065 3d22 5153 7472 696e  "2" type="QStrin
+000027b0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+000027c0: 203c 4f70 7469 6f6e 206e 616d 653d 226f   <Option name="o
+000027d0: 7574 6c69 6e65 5f77 6964 7468 5f6d 6170  utline_width_map
+000027e0: 5f75 6e69 745f 7363 616c 6522 2076 616c  _unit_scale" val
+000027f0: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+00002800: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
+00002810: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00002820: 203c 4f70 7469 6f6e 206e 616d 653d 226f   <Option name="o
+00002830: 7574 6c69 6e65 5f77 6964 7468 5f75 6e69  utline_width_uni
+00002840: 7422 2076 616c 7565 3d22 5265 6e64 6572  t" value="Render
+00002850: 4d65 7465 7273 496e 4d61 7055 6e69 7473  MetersInMapUnits
+00002860: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00002870: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00002880: 4f70 7469 6f6e 206e 616d 653d 2273 6361  Option name="sca
+00002890: 6c65 5f6d 6574 686f 6422 2076 616c 7565  le_method" value
+000028a0: 3d22 6469 616d 6574 6572 2220 7479 7065  ="diameter" type
+000028b0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000028c0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000028d0: 206e 616d 653d 2273 697a 6522 2076 616c   name="size" val
+000028e0: 7565 3d22 3322 2074 7970 653d 2251 5374  ue="3" type="QSt
+000028f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00002900: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00002910: 3d22 7369 7a65 5f6d 6170 5f75 6e69 745f  ="size_map_unit_
+00002920: 7363 616c 6522 2076 616c 7565 3d22 3378  scale" value="3x
+00002930: 3a30 2c30 2c30 2c30 2c30 2c30 2220 7479  :0,0,0,0,0,0" ty
+00002940: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
 00002950: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00002960: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
-00002970: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00002980: 7469 6f6e 206e 616d 653d 226e 616d 6522  tion name="name"
-00002990: 2076 616c 7565 3d22 2220 7479 7065 3d22   value="" type="
-000029a0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-000029b0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000029c0: 206e 616d 653d 2270 726f 7065 7274 6965   name="propertie
-000029d0: 7322 2f3e 0a20 2020 2020 2020 2020 2020  s"/>.           
-000029e0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-000029f0: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
-00002a00: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
-00002a10: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00002a20: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
-00002a30: 0a20 2020 2020 2020 2020 203c 2f64 6174  .          </dat
-00002a40: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
-00002a50: 7469 6573 3e0a 2020 2020 2020 2020 3c2f  ties>.        </
-00002a60: 6c61 7965 723e 0a20 2020 2020 203c 2f73  layer>.      </s
-00002a70: 796d 626f 6c3e 0a20 2020 2020 203c 7379  ymbol>.      <sy
-00002a80: 6d62 6f6c 206e 616d 653d 2231 2220 636c  mbol name="1" cl
-00002a90: 6970 5f74 6f5f 6578 7465 6e74 3d22 3122  ip_to_extent="1"
-00002aa0: 2066 6f72 6365 5f72 6872 3d22 3022 2069   force_rhr="0" i
-00002ab0: 735f 616e 696d 6174 6564 3d22 3022 2074  s_animated="0" t
-00002ac0: 7970 653d 226d 6172 6b65 7222 2061 6c70  ype="marker" alp
-00002ad0: 6861 3d22 3122 2066 7261 6d65 5f72 6174  ha="1" frame_rat
-00002ae0: 653d 2231 3022 3e0a 2020 2020 2020 2020  e="10">.        
-00002af0: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-00002b00: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00002b10: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
-00002b20: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-00002b30: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00002b40: 3d22 6e61 6d65 2220 7661 6c75 653d 2222  ="name" value=""
-00002b50: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00002b60: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00002b70: 7074 696f 6e20 6e61 6d65 3d22 7072 6f70  ption name="prop
-00002b80: 6572 7469 6573 222f 3e0a 2020 2020 2020  erties"/>.      
-00002b90: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00002ba0: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
-00002bb0: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
-00002bc0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002bd0: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-00002be0: 3e0a 2020 2020 2020 2020 3c2f 6461 7461  >.        </data
-00002bf0: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
-00002c00: 6965 733e 0a20 2020 2020 2020 203c 6c61  ies>.        <la
-00002c10: 7965 7220 636c 6173 733d 2253 7667 4d61  yer class="SvgMa
-00002c20: 726b 6572 2220 656e 6162 6c65 643d 2231  rker" enabled="1
-00002c30: 2220 6c6f 636b 6564 3d22 3022 2070 6173  " locked="0" pas
-00002c40: 733d 2230 223e 0a20 2020 2020 2020 2020  s="0">.         
-00002c50: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-00002c60: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
-00002c70: 203c 4f70 7469 6f6e 206e 616d 653d 2261   <Option name="a
-00002c80: 6e67 6c65 2220 7661 6c75 653d 2230 2220  ngle" value="0" 
-00002c90: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00002ca0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00002cb0: 7469 6f6e 206e 616d 653d 2263 6f6c 6f72  tion name="color
-00002cc0: 2220 7661 6c75 653d 2231 3435 2c38 322c  " value="145,82,
-00002cd0: 3435 2c32 3535 2220 7479 7065 3d22 5153  45,255" type="QS
-00002ce0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002cf0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00002d00: 653d 2266 6978 6564 4173 7065 6374 5261  e="fixedAspectRa
-00002d10: 7469 6f22 2076 616c 7565 3d22 3022 2074  tio" value="0" t
-00002d20: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00002d30: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00002d40: 696f 6e20 6e61 6d65 3d22 686f 7269 7a6f  ion name="horizo
-00002d50: 6e74 616c 5f61 6e63 686f 725f 706f 696e  ntal_anchor_poin
-00002d60: 7422 2076 616c 7565 3d22 3122 2074 7970  t" value="1" typ
-00002d70: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002d80: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002d90: 6e20 6e61 6d65 3d22 6e61 6d65 2220 7661  n name="name" va
-00002da0: 6c75 653d 2272 6573 6f75 7263 6573 2f63  lue="resources/c
-00002db0: 726f 7373 696e 672e 7376 6722 2074 7970  rossing.svg" typ
-00002dc0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002dd0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002de0: 6e20 6e61 6d65 3d22 6f66 6673 6574 2220  n name="offset" 
-00002df0: 7661 6c75 653d 2230 2c30 2220 7479 7065  value="0,0" type
-00002e00: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002e10: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00002e20: 206e 616d 653d 226f 6666 7365 745f 6d61   name="offset_ma
-00002e30: 705f 756e 6974 5f73 6361 6c65 2220 7661  p_unit_scale" va
-00002e40: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00002e50: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-00002e60: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00002e70: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00002e80: 6f66 6673 6574 5f75 6e69 7422 2076 616c  offset_unit" val
-00002e90: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
-00002ea0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002eb0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00002ec0: 653d 226f 7574 6c69 6e65 5f63 6f6c 6f72  e="outline_color
-00002ed0: 2220 7661 6c75 653d 2233 352c 3335 2c33  " value="35,35,3
-00002ee0: 352c 3235 3522 2074 7970 653d 2251 5374  5,255" type="QSt
-00002ef0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002f00: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00002f10: 3d22 6f75 746c 696e 655f 7769 6474 6822  ="outline_width"
-00002f20: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
-00002f30: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00002f40: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002f50: 6e61 6d65 3d22 6f75 746c 696e 655f 7769  name="outline_wi
-00002f60: 6474 685f 6d61 705f 756e 6974 5f73 6361  dth_map_unit_sca
-00002f70: 6c65 2220 7661 6c75 653d 2233 783a 302c  le" value="3x:0,
-00002f80: 302c 302c 302c 302c 3022 2074 7970 653d  0,0,0,0,0" type=
-00002f90: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00002fa0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002fb0: 6e61 6d65 3d22 6f75 746c 696e 655f 7769  name="outline_wi
-00002fc0: 6474 685f 756e 6974 2220 7661 6c75 653d  dth_unit" value=
-00002fd0: 224d 4d22 2074 7970 653d 2251 5374 7269  "MM" type="QStri
-00002fe0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00002ff0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00003000: 7061 7261 6d65 7465 7273 222f 3e0a 2020  parameters"/>.  
-00003010: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003020: 6e20 6e61 6d65 3d22 7363 616c 655f 6d65  n name="scale_me
-00003030: 7468 6f64 2220 7661 6c75 653d 2264 6961  thod" value="dia
-00003040: 6d65 7465 7222 2074 7970 653d 2251 5374  meter" type="QSt
-00003050: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003060: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00003070: 3d22 7369 7a65 2220 7661 6c75 653d 2231  ="size" value="1
-00003080: 3222 2074 7970 653d 2251 5374 7269 6e67  2" type="QString
-00003090: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-000030a0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7369  <Option name="si
-000030b0: 7a65 5f6d 6170 5f75 6e69 745f 7363 616c  ze_map_unit_scal
-000030c0: 6522 2076 616c 7565 3d22 3378 3a30 2c30  e" value="3x:0,0
-000030d0: 2c30 2c30 2c30 2c30 2220 7479 7065 3d22  ,0,0,0,0" type="
-000030e0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-000030f0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
-00003100: 616d 653d 2273 697a 655f 756e 6974 2220  ame="size_unit" 
-00003110: 7661 6c75 653d 224d 4d22 2074 7970 653d  value="MM" type=
-00003120: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003130: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00003140: 6e61 6d65 3d22 7665 7274 6963 616c 5f61  name="vertical_a
-00003150: 6e63 686f 725f 706f 696e 7422 2076 616c  nchor_point" val
-00003160: 7565 3d22 3122 2074 7970 653d 2251 5374  ue="1" type="QSt
-00003170: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003180: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-00003190: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
-000031a0: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
-000031b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000031c0: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
-000031d0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000031e0: 7074 696f 6e20 6e61 6d65 3d22 6e61 6d65  ption name="name
-000031f0: 2220 7661 6c75 653d 2222 2074 7970 653d  " value="" type=
-00003200: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003210: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003220: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
-00003230: 6573 2220 7479 7065 3d22 4d61 7022 3e0a  es" type="Map">.
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 3c4f 7074 696f 6e20 6e61 6d65 3d22 616e  <Option name="an
-00003260: 676c 6522 2074 7970 653d 224d 6170 223e  gle" type="Map">
-00003270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003280: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003290: 2261 6374 6976 6522 2076 616c 7565 3d22  "active" value="
-000032a0: 7472 7565 2220 7479 7065 3d22 626f 6f6c  true" type="bool
-000032b0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-000032c0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-000032d0: 6d65 3d22 6578 7072 6573 7369 6f6e 2220  me="expression" 
-000032e0: 7661 6c75 653d 2231 3830 202b 2028 2d26  value="180 + (-&
-000032f0: 7175 6f74 3b6f 7269 656e 7461 7469 6f6e  quot;orientation
-00003300: 2671 756f 743b 202f 2070 6928 2929 202a  &quot; / pi()) *
-00003310: 2031 3830 2220 7479 7065 3d22 5153 7472   180" type="QStr
-00003320: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003330: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003340: 206e 616d 653d 2274 7970 6522 2076 616c   name="type" val
-00003350: 7565 3d22 3322 2074 7970 653d 2269 6e74  ue="3" type="int
-00003360: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003370: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00003380: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-00003390: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-000033a0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000033b0: 3d22 7479 7065 2220 7661 6c75 653d 2263  ="type" value="c
-000033c0: 6f6c 6c65 6374 696f 6e22 2074 7970 653d  ollection" type=
-000033d0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000033e0: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-000033f0: 3e0a 2020 2020 2020 2020 2020 3c2f 6461  >.          </da
-00003400: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00003410: 7274 6965 733e 0a20 2020 2020 2020 203c  rties>.        <
-00003420: 2f6c 6179 6572 3e0a 2020 2020 2020 3c2f  /layer>.      </
-00003430: 7379 6d62 6f6c 3e0a 2020 2020 3c2f 7379  symbol>.    </sy
-00003440: 6d62 6f6c 733e 0a20 203c 2f72 656e 6465  mbols>.  </rende
-00003450: 7265 722d 7632 3e0a 2020 3c63 7573 746f  rer-v2>.  <custo
-00003460: 6d70 726f 7065 7274 6965 733e 0a20 2020  mproperties>.   
-00003470: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-00003480: 6170 223e 0a20 2020 2020 203c 4f70 7469  ap">.      <Opti
-00003490: 6f6e 206e 616d 653d 2264 7561 6c76 6965  on name="dualvie
-000034a0: 772f 7072 6576 6965 7745 7870 7265 7373  w/previewExpress
-000034b0: 696f 6e73 2220 7479 7065 3d22 4c69 7374  ions" type="List
-000034c0: 223e 0a20 2020 2020 2020 203c 4f70 7469  ">.        <Opti
-000034d0: 6f6e 2076 616c 7565 3d22 2671 756f 743b  on value="&quot;
-000034e0: 7479 7065 2671 756f 743b 2220 7479 7065  type&quot;" type
-000034f0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003500: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
-00003510: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003520: 2265 6d62 6564 6465 6457 6964 6765 7473  "embeddedWidgets
-00003530: 2f63 6f75 6e74 2220 7661 6c75 653d 2230  /count" value="0
-00003540: 2220 7479 7065 3d22 696e 7422 2f3e 0a20  " type="int"/>. 
-00003550: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00003560: 653d 2276 6172 6961 626c 654e 616d 6573  e="variableNames
-00003570: 222f 3e0a 2020 2020 2020 3c4f 7074 696f  "/>.      <Optio
-00003580: 6e20 6e61 6d65 3d22 7661 7269 6162 6c65  n name="variable
-00003590: 5661 6c75 6573 222f 3e0a 2020 2020 3c2f  Values"/>.    </
-000035a0: 4f70 7469 6f6e 3e0a 2020 3c2f 6375 7374  Option>.  </cust
-000035b0: 6f6d 7072 6f70 6572 7469 6573 3e0a 2020  omproperties>.  
-000035c0: 3c62 6c65 6e64 4d6f 6465 3e30 3c2f 626c  <blendMode>0</bl
-000035d0: 656e 644d 6f64 653e 0a20 203c 6665 6174  endMode>.  <feat
-000035e0: 7572 6542 6c65 6e64 4d6f 6465 3e30 3c2f  ureBlendMode>0</
-000035f0: 6665 6174 7572 6542 6c65 6e64 4d6f 6465  featureBlendMode
-00003600: 3e0a 2020 3c6c 6179 6572 4f70 6163 6974  >.  <layerOpacit
-00003610: 793e 313c 2f6c 6179 6572 4f70 6163 6974  y>1</layerOpacit
-00003620: 793e 0a20 203c 5369 6e67 6c65 4361 7465  y>.  <SingleCate
-00003630: 676f 7279 4469 6167 7261 6d52 656e 6465  goryDiagramRende
-00003640: 7265 7220 6174 7472 6962 7574 654c 6567  rer attributeLeg
-00003650: 656e 643d 2231 2220 6469 6167 7261 6d54  end="1" diagramT
-00003660: 7970 653d 2248 6973 746f 6772 616d 223e  ype="Histogram">
-00003670: 0a20 2020 203c 4469 6167 7261 6d43 6174  .    <DiagramCat
-00003680: 6567 6f72 7920 7065 6e41 6c70 6861 3d22  egory penAlpha="
-00003690: 3235 3522 2073 697a 6553 6361 6c65 3d22  255" sizeScale="
-000036a0: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-000036b0: 6c69 6e65 5369 7a65 5363 616c 653d 2233  lineSizeScale="3
-000036c0: 783a 302c 302c 302c 302c 302c 3022 2077  x:0,0,0,0,0,0" w
-000036d0: 6964 7468 3d22 3135 2220 7065 6e43 6f6c  idth="15" penCol
-000036e0: 6f72 3d22 2330 3030 3030 3022 206d 696e  or="#000000" min
-000036f0: 5363 616c 6544 656e 6f6d 696e 6174 6f72  ScaleDenominator
-00003700: 3d22 3022 2073 697a 6554 7970 653d 224d  ="0" sizeType="M
-00003710: 4d22 2073 6361 6c65 4465 7065 6e64 656e  M" scaleDependen
-00003720: 6379 3d22 4172 6561 2220 6469 6167 7261  cy="Area" diagra
-00003730: 6d4f 7269 656e 7461 7469 6f6e 3d22 5570  mOrientation="Up
-00003740: 2220 726f 7461 7469 6f6e 4f66 6673 6574  " rotationOffset
-00003750: 3d22 3237 3022 206d 6178 5363 616c 6544  ="270" maxScaleD
-00003760: 656e 6f6d 696e 6174 6f72 3d22 3165 2b30  enominator="1e+0
-00003770: 3822 2073 7061 6369 6e67 3d22 3522 2068  8" spacing="5" h
-00003780: 6569 6768 743d 2231 3522 2064 6972 6563  eight="15" direc
-00003790: 7469 6f6e 3d22 3022 206f 7061 6369 7479  tion="0" opacity
-000037a0: 3d22 3122 206c 696e 6553 697a 6554 7970  ="1" lineSizeTyp
-000037b0: 653d 224d 4d22 2062 6172 5769 6474 683d  e="MM" barWidth=
-000037c0: 2235 2220 7370 6163 696e 6755 6e69 743d  "5" spacingUnit=
-000037d0: 224d 4d22 2062 6163 6b67 726f 756e 6443  "MM" backgroundC
-000037e0: 6f6c 6f72 3d22 2366 6666 6666 6622 2070  olor="#ffffff" p
-000037f0: 656e 5769 6474 683d 2230 2220 6c61 6265  enWidth="0" labe
-00003800: 6c50 6c61 6365 6d65 6e74 4d65 7468 6f64  lPlacementMethod
-00003810: 3d22 5848 6569 6768 7422 206d 696e 696d  ="XHeight" minim
-00003820: 756d 5369 7a65 3d22 3022 2073 6361 6c65  umSize="0" scale
-00003830: 4261 7365 6456 6973 6962 696c 6974 793d  BasedVisibility=
-00003840: 2230 2220 6261 636b 6772 6f75 6e64 416c  "0" backgroundAl
-00003850: 7068 613d 2232 3535 2220 7368 6f77 4178  pha="255" showAx
-00003860: 6973 3d22 3122 2065 6e61 626c 6564 3d22  is="1" enabled="
-00003870: 3022 2073 7061 6369 6e67 556e 6974 5363  0" spacingUnitSc
-00003880: 616c 653d 2233 783a 302c 302c 302c 302c  ale="3x:0,0,0,0,
-00003890: 302c 3022 3e0a 2020 2020 2020 3c66 6f6e  0,0">.      <fon
-000038a0: 7450 726f 7065 7274 6965 7320 626f 6c64  tProperties bold
-000038b0: 3d22 3022 2073 7479 6c65 3d22 2220 6974  ="0" style="" it
-000038c0: 616c 6963 3d22 3022 2075 6e64 6572 6c69  alic="0" underli
-000038d0: 6e65 3d22 3022 2073 7472 696b 6574 6872  ne="0" strikethr
-000038e0: 6f75 6768 3d22 3022 2064 6573 6372 6970  ough="0" descrip
-000038f0: 7469 6f6e 3d22 4e6f 746f 2053 616e 732c  tion="Noto Sans,
-00003900: 3130 2c2d 312c 302c 3530 2c30 2c30 2c30  10,-1,0,50,0,0,0
-00003910: 2c30 2c30 222f 3e0a 2020 2020 2020 3c61  ,0,0"/>.      <a
-00003920: 7474 7269 6275 7465 2066 6965 6c64 3d22  ttribute field="
-00003930: 2220 636f 6c6f 723d 2223 3030 3030 3030  " color="#000000
-00003940: 2220 6c61 6265 6c3d 2222 2063 6f6c 6f72  " label="" color
-00003950: 4f70 6163 6974 793d 2231 222f 3e0a 2020  Opacity="1"/>.  
-00003960: 2020 2020 3c61 7869 7353 796d 626f 6c3e      <axisSymbol>
-00003970: 0a20 2020 2020 2020 203c 7379 6d62 6f6c  .        <symbol
-00003980: 206e 616d 653d 2222 2063 6c69 705f 746f   name="" clip_to
-00003990: 5f65 7874 656e 743d 2231 2220 666f 7263  _extent="1" forc
-000039a0: 655f 7268 723d 2230 2220 6973 5f61 6e69  e_rhr="0" is_ani
-000039b0: 6d61 7465 643d 2230 2220 7479 7065 3d22  mated="0" type="
-000039c0: 6c69 6e65 2220 616c 7068 613d 2231 2220  line" alpha="1" 
-000039d0: 6672 616d 655f 7261 7465 3d22 3130 223e  frame_rate="10">
-000039e0: 0a20 2020 2020 2020 2020 203c 6461 7461  .          <data
-000039f0: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
-00003a00: 6965 733e 0a20 2020 2020 2020 2020 2020  ies>.           
-00003a10: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-00003a20: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
-00003a30: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003a40: 226e 616d 6522 2076 616c 7565 3d22 2220  "name" value="" 
-00003a50: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003a60: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003a70: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
-00003a80: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
-00003a90: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003aa0: 206e 616d 653d 2274 7970 6522 2076 616c   name="type" val
-00003ab0: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
-00003ac0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003ad0: 0a20 2020 2020 2020 2020 2020 203c 2f4f  .            </O
-00003ae0: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
-00003af0: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
-00003b00: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
-00003b10: 2020 2020 2020 3c6c 6179 6572 2063 6c61        <layer cla
-00003b20: 7373 3d22 5369 6d70 6c65 4c69 6e65 2220  ss="SimpleLine" 
-00003b30: 656e 6162 6c65 643d 2231 2220 6c6f 636b  enabled="1" lock
-00003b40: 6564 3d22 3022 2070 6173 733d 2230 223e  ed="0" pass="0">
-00003b50: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003b60: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
-00003b70: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003b80: 4f70 7469 6f6e 206e 616d 653d 2261 6c69  Option name="ali
-00003b90: 676e 5f64 6173 685f 7061 7474 6572 6e22  gn_dash_pattern"
-00003ba0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
-00003bb0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003bc0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003bd0: 6e20 6e61 6d65 3d22 6361 7073 7479 6c65  n name="capstyle
-00003be0: 2220 7661 6c75 653d 2273 7175 6172 6522  " value="square"
-00003bf0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00003c00: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003c10: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6375  <Option name="cu
-00003c20: 7374 6f6d 6461 7368 2220 7661 6c75 653d  stomdash" value=
-00003c30: 2235 3b32 2220 7479 7065 3d22 5153 7472  "5;2" type="QStr
-00003c40: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003c50: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00003c60: 653d 2263 7573 746f 6d64 6173 685f 6d61  e="customdash_ma
-00003c70: 705f 756e 6974 5f73 6361 6c65 2220 7661  p_unit_scale" va
-00003c80: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00003c90: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
-00003ca0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003cb0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-00003cc0: 3d22 6375 7374 6f6d 6461 7368 5f75 6e69  ="customdash_uni
-00003cd0: 7422 2076 616c 7565 3d22 4d4d 2220 7479  t" value="MM" ty
-00003ce0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003cf0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-00003d00: 7469 6f6e 206e 616d 653d 2264 6173 685f  tion name="dash_
-00003d10: 7061 7474 6572 6e5f 6f66 6673 6574 2220  pattern_offset" 
-00003d20: 7661 6c75 653d 2230 2220 7479 7065 3d22  value="0" type="
-00003d30: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003d40: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003d50: 206e 616d 653d 2264 6173 685f 7061 7474   name="dash_patt
-00003d60: 6572 6e5f 6f66 6673 6574 5f6d 6170 5f75  ern_offset_map_u
-00003d70: 6e69 745f 7363 616c 6522 2076 616c 7565  nit_scale" value
-00003d80: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
-00003d90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003da0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00003db0: 203c 4f70 7469 6f6e 206e 616d 653d 2264   <Option name="d
-00003dc0: 6173 685f 7061 7474 6572 6e5f 6f66 6673  ash_pattern_offs
-00003dd0: 6574 5f75 6e69 7422 2076 616c 7565 3d22  et_unit" value="
-00003de0: 4d4d 2220 7479 7065 3d22 5153 7472 696e  MM" type="QStrin
-00003df0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00003e00: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003e10: 2264 7261 775f 696e 7369 6465 5f70 6f6c  "draw_inside_pol
-00003e20: 7967 6f6e 2220 7661 6c75 653d 2230 2220  ygon" value="0" 
-00003e30: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003e40: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003e50: 4f70 7469 6f6e 206e 616d 653d 226a 6f69  Option name="joi
-00003e60: 6e73 7479 6c65 2220 7661 6c75 653d 2262  nstyle" value="b
-00003e70: 6576 656c 2220 7479 7065 3d22 5153 7472  evel" type="QStr
-00003e80: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003e90: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
-00003ea0: 653d 226c 696e 655f 636f 6c6f 7222 2076  e="line_color" v
-00003eb0: 616c 7565 3d22 3335 2c33 352c 3335 2c32  alue="35,35,35,2
-00003ec0: 3535 2220 7479 7065 3d22 5153 7472 696e  55" type="QStrin
-00003ed0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00003ee0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00003ef0: 226c 696e 655f 7374 796c 6522 2076 616c  "line_style" val
-00003f00: 7565 3d22 736f 6c69 6422 2074 7970 653d  ue="solid" type=
-00003f10: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003f20: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003f30: 6e20 6e61 6d65 3d22 6c69 6e65 5f77 6964  n name="line_wid
-00003f40: 7468 2220 7661 6c75 653d 2230 2e32 3622  th" value="0.26"
-00003f50: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00003f60: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00003f70: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6c69  <Option name="li
-00003f80: 6e65 5f77 6964 7468 5f75 6e69 7422 2076  ne_width_unit" v
-00003f90: 616c 7565 3d22 4d4d 2220 7479 7065 3d22  alue="MM" type="
-00003fa0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003fb0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003fc0: 206e 616d 653d 226f 6666 7365 7422 2076   name="offset" v
-00003fd0: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
-00003fe0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00003ff0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004000: 6e61 6d65 3d22 6f66 6673 6574 5f6d 6170  name="offset_map
-00004010: 5f75 6e69 745f 7363 616c 6522 2076 616c  _unit_scale" val
-00004020: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
-00004030: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
-00004040: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00004050: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
-00004060: 226f 6666 7365 745f 756e 6974 2220 7661  "offset_unit" va
-00004070: 6c75 653d 224d 4d22 2074 7970 653d 2251  lue="MM" type="Q
-00004080: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004090: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000040a0: 6e61 6d65 3d22 7269 6e67 5f66 696c 7465  name="ring_filte
-000040b0: 7222 2076 616c 7565 3d22 3022 2074 7970  r" value="0" typ
-000040c0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000040d0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000040e0: 696f 6e20 6e61 6d65 3d22 7472 696d 5f64  ion name="trim_d
-000040f0: 6973 7461 6e63 655f 656e 6422 2076 616c  istance_end" val
-00004100: 7565 3d22 3022 2074 7970 653d 2251 5374  ue="0" type="QSt
-00004110: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004120: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
-00004130: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
-00004140: 655f 656e 645f 6d61 705f 756e 6974 5f73  e_end_map_unit_s
-00004150: 6361 6c65 2220 7661 6c75 653d 2233 783a  cale" value="3x:
-00004160: 302c 302c 302c 302c 302c 3022 2074 7970  0,0,0,0,0,0" typ
-00004170: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00004180: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004190: 696f 6e20 6e61 6d65 3d22 7472 696d 5f64  ion name="trim_d
-000041a0: 6973 7461 6e63 655f 656e 645f 756e 6974  istance_end_unit
-000041b0: 2220 7661 6c75 653d 224d 4d22 2074 7970  " value="MM" typ
-000041c0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000041d0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000041e0: 696f 6e20 6e61 6d65 3d22 7472 696d 5f64  ion name="trim_d
-000041f0: 6973 7461 6e63 655f 7374 6172 7422 2076  istance_start" v
-00004200: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
-00004210: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004220: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004230: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00004240: 6e63 655f 7374 6172 745f 6d61 705f 756e  nce_start_map_un
-00004250: 6974 5f73 6361 6c65 2220 7661 6c75 653d  it_scale" value=
-00004260: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
-00004270: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004280: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004290: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7472  <Option name="tr
-000042a0: 696d 5f64 6973 7461 6e63 655f 7374 6172  im_distance_star
-000042b0: 745f 756e 6974 2220 7661 6c75 653d 224d  t_unit" value="M
-000042c0: 4d22 2074 7970 653d 2251 5374 7269 6e67  M" type="QString
-000042d0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-000042e0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-000042f0: 7477 6561 6b5f 6461 7368 5f70 6174 7465  tweak_dash_patte
-00004300: 726e 5f6f 6e5f 636f 726e 6572 7322 2076  rn_on_corners" v
-00004310: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
-00004320: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004330: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004340: 6e61 6d65 3d22 7573 655f 6375 7374 6f6d  name="use_custom
-00004350: 5f64 6173 6822 2076 616c 7565 3d22 3022  _dash" value="0"
-00004360: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004370: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004380: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7769  <Option name="wi
-00004390: 6474 685f 6d61 705f 756e 6974 5f73 6361  dth_map_unit_sca
-000043a0: 6c65 2220 7661 6c75 653d 2233 783a 302c  le" value="3x:0,
-000043b0: 302c 302c 302c 302c 3022 2074 7970 653d  0,0,0,0,0" type=
-000043c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000043d0: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-000043e0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
-000043f0: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
-00004400: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
-00004410: 2020 2020 2020 3c4f 7074 696f 6e20 7479        <Option ty
-00004420: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
-00004430: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00004440: 6e20 6e61 6d65 3d22 6e61 6d65 2220 7661  n name="name" va
-00004450: 6c75 653d 2222 2074 7970 653d 2251 5374  lue="" type="QSt
-00004460: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004470: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004480: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
-00004490: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-000044a0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000044b0: 3d22 7479 7065 2220 7661 6c75 653d 2263  ="type" value="c
-000044c0: 6f6c 6c65 6374 696f 6e22 2074 7970 653d  ollection" type=
-000044d0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000044e0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-000044f0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00004500: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
-00004510: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00004520: 2020 2020 203c 2f6c 6179 6572 3e0a 2020       </layer>.  
-00004530: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
-00004540: 2020 2020 2020 3c2f 6178 6973 5379 6d62        </axisSymb
-00004550: 6f6c 3e0a 2020 2020 3c2f 4469 6167 7261  ol>.    </Diagra
-00004560: 6d43 6174 6567 6f72 793e 0a20 203c 2f53  mCategory>.  </S
-00004570: 696e 676c 6543 6174 6567 6f72 7944 6961  ingleCategoryDia
-00004580: 6772 616d 5265 6e64 6572 6572 3e0a 2020  gramRenderer>.  
-00004590: 3c44 6961 6772 616d 4c61 7965 7253 6574  <DiagramLayerSet
-000045a0: 7469 6e67 7320 7072 696f 7269 7479 3d22  tings priority="
-000045b0: 3022 206c 696e 6550 6c61 6365 6d65 6e74  0" linePlacement
-000045c0: 466c 6167 733d 2231 3822 2064 6973 743d  Flags="18" dist=
-000045d0: 2230 2220 7a49 6e64 6578 3d22 3022 206f  "0" zIndex="0" o
-000045e0: 6273 7461 636c 653d 2230 2220 706c 6163  bstacle="0" plac
-000045f0: 656d 656e 743d 2230 2220 7368 6f77 416c  ement="0" showAl
-00004600: 6c3d 2231 223e 0a20 2020 203c 7072 6f70  l="1">.    <prop
-00004610: 6572 7469 6573 3e0a 2020 2020 2020 3c4f  erties>.      <O
-00004620: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
-00004630: 3e0a 2020 2020 2020 2020 3c4f 7074 696f  >.        <Optio
-00004640: 6e20 6e61 6d65 3d22 6e61 6d65 2220 7661  n name="name" va
-00004650: 6c75 653d 2222 2074 7970 653d 2251 5374  lue="" type="QSt
-00004660: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004670: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7072  <Option name="pr
-00004680: 6f70 6572 7469 6573 222f 3e0a 2020 2020  operties"/>.    
-00004690: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
-000046a0: 3d22 7479 7065 2220 7661 6c75 653d 2263  ="type" value="c
-000046b0: 6f6c 6c65 6374 696f 6e22 2074 7970 653d  ollection" type=
-000046c0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000046d0: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
-000046e0: 3c2f 7072 6f70 6572 7469 6573 3e0a 2020  </properties>.  
-000046f0: 3c2f 4469 6167 7261 6d4c 6179 6572 5365  </DiagramLayerSe
-00004700: 7474 696e 6773 3e0a 2020 3c67 656f 6d65  ttings>.  <geome
-00004710: 7472 794f 7074 696f 6e73 2067 656f 6d65  tryOptions geome
-00004720: 7472 7950 7265 6369 7369 6f6e 3d22 3022  tryPrecision="0"
-00004730: 2072 656d 6f76 6544 7570 6c69 6361 7465   removeDuplicate
-00004740: 4e6f 6465 733d 2230 223e 0a20 2020 203c  Nodes="0">.    <
-00004750: 6163 7469 7665 4368 6563 6b73 2f3e 0a20  activeChecks/>. 
-00004760: 2020 203c 6368 6563 6b43 6f6e 6669 6775     <checkConfigu
-00004770: 7261 7469 6f6e 2f3e 0a20 203c 2f67 656f  ration/>.  </geo
-00004780: 6d65 7472 794f 7074 696f 6e73 3e0a 2020  metryOptions>.  
-00004790: 3c6c 6567 656e 6420 7479 7065 3d22 6465  <legend type="de
-000047a0: 6661 756c 742d 7665 6374 6f72 2220 7368  fault-vector" sh
-000047b0: 6f77 4c61 6265 6c4c 6567 656e 643d 2230  owLabelLegend="0
-000047c0: 222f 3e0a 2020 3c72 6566 6572 656e 6365  "/>.  <reference
-000047d0: 644c 6179 6572 732f 3e0a 2020 3c66 6965  dLayers/>.  <fie
-000047e0: 6c64 436f 6e66 6967 7572 6174 696f 6e3e  ldConfiguration>
-000047f0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-00004800: 3d22 7479 7065 2220 636f 6e66 6967 7572  ="type" configur
-00004810: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
-00004820: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
-00004830: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
-00004840: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
-00004850: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
-00004860: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
-00004870: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
-00004880: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
-00004890: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
-000048a0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
-000048b0: 736d 5f69 6422 2063 6f6e 6669 6775 7261  sm_id" configura
-000048c0: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
-000048d0: 3e0a 2020 2020 2020 3c65 6469 7457 6964  >.      <editWid
-000048e0: 6765 7420 7479 7065 3d22 5465 7874 4564  get type="TextEd
-000048f0: 6974 223e 0a20 2020 2020 2020 203c 636f  it">.        <co
-00004900: 6e66 6967 3e0a 2020 2020 2020 2020 2020  nfig>.          
-00004910: 3c4f 7074 696f 6e2f 3e0a 2020 2020 2020  <Option/>.      
-00004920: 2020 3c2f 636f 6e66 6967 3e0a 2020 2020    </config>.    
-00004930: 2020 3c2f 6564 6974 5769 6467 6574 3e0a    </editWidget>.
-00004940: 2020 2020 3c2f 6669 656c 643e 0a20 2020      </field>.   
-00004950: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
-00004960: 6965 6e74 6174 696f 6e22 2063 6f6e 6669  ientation" confi
-00004970: 6775 7261 7469 6f6e 466c 6167 733d 224e  gurationFlags="N
-00004980: 6f6e 6522 3e0a 2020 2020 2020 3c65 6469  one">.      <edi
-00004990: 7457 6964 6765 7420 7479 7065 3d22 5465  tWidget type="Te
-000049a0: 7874 4564 6974 223e 0a20 2020 2020 2020  xtEdit">.       
-000049b0: 203c 636f 6e66 6967 3e0a 2020 2020 2020   <config>.      
-000049c0: 2020 2020 3c4f 7074 696f 6e2f 3e0a 2020      <Option/>.  
-000049d0: 2020 2020 2020 3c2f 636f 6e66 6967 3e0a        </config>.
-000049e0: 2020 2020 2020 3c2f 6564 6974 5769 6467        </editWidg
-000049f0: 6574 3e0a 2020 2020 3c2f 6669 656c 643e  et>.    </field>
-00004a00: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
-00004a10: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-00004a20: 6e66 6964 656e 6365 2220 636f 6e66 6967  nfidence" config
-00004a30: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
-00004a40: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
-00004a50: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
-00004a60: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
-00004a70: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
-00004a80: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
-00004a90: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
-00004aa0: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
-00004ab0: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
-00004ac0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00004ad0: 2261 6e67 6c65 2220 636f 6e66 6967 7572  "angle" configur
-00004ae0: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
-00004af0: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
-00004b00: 6467 6574 2074 7970 653d 2252 616e 6765  dget type="Range
-00004b10: 223e 0a20 2020 2020 2020 203c 636f 6e66  ">.        <conf
-00004b20: 6967 3e0a 2020 2020 2020 2020 2020 3c4f  ig>.          <O
-00004b30: 7074 696f 6e2f 3e0a 2020 2020 2020 2020  ption/>.        
-00004b40: 3c2f 636f 6e66 6967 3e0a 2020 2020 2020  </config>.      
-00004b50: 3c2f 6564 6974 5769 6467 6574 3e0a 2020  </editWidget>.  
-00004b60: 2020 3c2f 6669 656c 643e 0a20 203c 2f66    </field>.  </f
-00004b70: 6965 6c64 436f 6e66 6967 7572 6174 696f  ieldConfiguratio
-00004b80: 6e3e 0a20 203c 616c 6961 7365 733e 0a20  n>.  <aliases>. 
-00004b90: 2020 203c 616c 6961 7320 6669 656c 643d     <alias field=
-00004ba0: 2274 7970 6522 206e 616d 653d 2222 2069  "type" name="" i
-00004bb0: 6e64 6578 3d22 3022 2f3e 0a20 2020 203c  ndex="0"/>.    <
-00004bc0: 616c 6961 7320 6669 656c 643d 226f 736d  alias field="osm
-00004bd0: 5f69 6422 206e 616d 653d 2222 2069 6e64  _id" name="" ind
-00004be0: 6578 3d22 3122 2f3e 0a20 2020 203c 616c  ex="1"/>.    <al
-00004bf0: 6961 7320 6669 656c 643d 226f 7269 656e  ias field="orien
-00004c00: 7461 7469 6f6e 2220 6e61 6d65 3d22 2220  tation" name="" 
-00004c10: 696e 6465 783d 2232 222f 3e0a 2020 2020  index="2"/>.    
-00004c20: 3c61 6c69 6173 2066 6965 6c64 3d22 6f72  <alias field="or
-00004c30: 6965 6e74 6174 696f 6e5f 636f 6e66 6964  ientation_confid
-00004c40: 656e 6365 2220 6e61 6d65 3d22 2220 696e  ence" name="" in
-00004c50: 6465 783d 2233 222f 3e0a 2020 2020 3c61  dex="3"/>.    <a
-00004c60: 6c69 6173 2066 6965 6c64 3d22 616e 676c  lias field="angl
-00004c70: 6522 206e 616d 653d 2222 2069 6e64 6578  e" name="" index
-00004c80: 3d22 3422 2f3e 0a20 203c 2f61 6c69 6173  ="4"/>.  </alias
-00004c90: 6573 3e0a 2020 3c64 6566 6175 6c74 733e  es>.  <defaults>
-00004ca0: 0a20 2020 203c 6465 6661 756c 7420 6669  .    <default fi
-00004cb0: 656c 643d 2274 7970 6522 2061 7070 6c79  eld="type" apply
-00004cc0: 4f6e 5570 6461 7465 3d22 3022 2065 7870  OnUpdate="0" exp
-00004cd0: 7265 7373 696f 6e3d 2222 2f3e 0a20 2020  ression=""/>.   
-00004ce0: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
-00004cf0: 226f 736d 5f69 6422 2061 7070 6c79 4f6e  "osm_id" applyOn
-00004d00: 5570 6461 7465 3d22 3022 2065 7870 7265  Update="0" expre
-00004d10: 7373 696f 6e3d 2222 2f3e 0a20 2020 203c  ssion=""/>.    <
-00004d20: 6465 6661 756c 7420 6669 656c 643d 226f  default field="o
-00004d30: 7269 656e 7461 7469 6f6e 2220 6170 706c  rientation" appl
-00004d40: 794f 6e55 7064 6174 653d 2230 2220 6578  yOnUpdate="0" ex
-00004d50: 7072 6573 7369 6f6e 3d22 222f 3e0a 2020  pression=""/>.  
-00004d60: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
-00004d70: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-00004d80: 6e66 6964 656e 6365 2220 6170 706c 794f  nfidence" applyO
-00004d90: 6e55 7064 6174 653d 2230 2220 6578 7072  nUpdate="0" expr
-00004da0: 6573 7369 6f6e 3d22 222f 3e0a 2020 2020  ession=""/>.    
-00004db0: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
-00004dc0: 616e 676c 6522 2061 7070 6c79 4f6e 5570  angle" applyOnUp
-00004dd0: 6461 7465 3d22 3022 2065 7870 7265 7373  date="0" express
-00004de0: 696f 6e3d 2222 2f3e 0a20 203c 2f64 6566  ion=""/>.  </def
-00004df0: 6175 6c74 733e 0a20 203c 636f 6e73 7472  aults>.  <constr
-00004e00: 6169 6e74 733e 0a20 2020 203c 636f 6e73  aints>.    <cons
-00004e10: 7472 6169 6e74 2063 6f6e 7374 7261 696e  traint constrain
-00004e20: 7473 3d22 3022 2066 6965 6c64 3d22 7479  ts="0" field="ty
-00004e30: 7065 2220 756e 6971 7565 5f73 7472 656e  pe" unique_stren
-00004e40: 6774 683d 2230 2220 6e6f 746e 756c 6c5f  gth="0" notnull_
-00004e50: 7374 7265 6e67 7468 3d22 3022 2065 7870  strength="0" exp
-00004e60: 5f73 7472 656e 6774 683d 2230 222f 3e0a  _strength="0"/>.
-00004e70: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
-00004e80: 636f 6e73 7472 6169 6e74 733d 2230 2220  constraints="0" 
-00004e90: 6669 656c 643d 226f 736d 5f69 6422 2075  field="osm_id" u
-00004ea0: 6e69 7175 655f 7374 7265 6e67 7468 3d22  nique_strength="
-00004eb0: 3022 206e 6f74 6e75 6c6c 5f73 7472 656e  0" notnull_stren
-00004ec0: 6774 683d 2230 2220 6578 705f 7374 7265  gth="0" exp_stre
-00004ed0: 6e67 7468 3d22 3022 2f3e 0a20 2020 203c  ngth="0"/>.    <
-00004ee0: 636f 6e73 7472 6169 6e74 2063 6f6e 7374  constraint const
-00004ef0: 7261 696e 7473 3d22 3022 2066 6965 6c64  raints="0" field
-00004f00: 3d22 6f72 6965 6e74 6174 696f 6e22 2075  ="orientation" u
-00004f10: 6e69 7175 655f 7374 7265 6e67 7468 3d22  nique_strength="
-00004f20: 3022 206e 6f74 6e75 6c6c 5f73 7472 656e  0" notnull_stren
-00004f30: 6774 683d 2230 2220 6578 705f 7374 7265  gth="0" exp_stre
-00004f40: 6e67 7468 3d22 3022 2f3e 0a20 2020 203c  ngth="0"/>.    <
-00004f50: 636f 6e73 7472 6169 6e74 2063 6f6e 7374  constraint const
-00004f60: 7261 696e 7473 3d22 3022 2066 6965 6c64  raints="0" field
-00004f70: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-00004f80: 6e66 6964 656e 6365 2220 756e 6971 7565  nfidence" unique
-00004f90: 5f73 7472 656e 6774 683d 2230 2220 6e6f  _strength="0" no
-00004fa0: 746e 756c 6c5f 7374 7265 6e67 7468 3d22  tnull_strength="
-00004fb0: 3022 2065 7870 5f73 7472 656e 6774 683d  0" exp_strength=
-00004fc0: 2230 222f 3e0a 2020 2020 3c63 6f6e 7374  "0"/>.    <const
-00004fd0: 7261 696e 7420 636f 6e73 7472 6169 6e74  raint constraint
-00004fe0: 733d 2230 2220 6669 656c 643d 2261 6e67  s="0" field="ang
-00004ff0: 6c65 2220 756e 6971 7565 5f73 7472 656e  le" unique_stren
-00005000: 6774 683d 2230 2220 6e6f 746e 756c 6c5f  gth="0" notnull_
-00005010: 7374 7265 6e67 7468 3d22 3022 2065 7870  strength="0" exp
-00005020: 5f73 7472 656e 6774 683d 2230 222f 3e0a  _strength="0"/>.
-00005030: 2020 3c2f 636f 6e73 7472 6169 6e74 733e    </constraints>
-00005040: 0a20 203c 636f 6e73 7472 6169 6e74 4578  .  <constraintEx
-00005050: 7072 6573 7369 6f6e 733e 0a20 2020 203c  pressions>.    <
-00005060: 636f 6e73 7472 6169 6e74 2064 6573 633d  constraint desc=
-00005070: 2222 2066 6965 6c64 3d22 7479 7065 2220  "" field="type" 
-00005080: 6578 703d 2222 2f3e 0a20 2020 203c 636f  exp=""/>.    <co
-00005090: 6e73 7472 6169 6e74 2064 6573 633d 2222  nstraint desc=""
-000050a0: 2066 6965 6c64 3d22 6f73 6d5f 6964 2220   field="osm_id" 
-000050b0: 6578 703d 2222 2f3e 0a20 2020 203c 636f  exp=""/>.    <co
-000050c0: 6e73 7472 6169 6e74 2064 6573 633d 2222  nstraint desc=""
-000050d0: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
-000050e0: 696f 6e22 2065 7870 3d22 222f 3e0a 2020  ion" exp=""/>.  
-000050f0: 2020 3c63 6f6e 7374 7261 696e 7420 6465    <constraint de
-00005100: 7363 3d22 2220 6669 656c 643d 226f 7269  sc="" field="ori
-00005110: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
-00005120: 6e63 6522 2065 7870 3d22 222f 3e0a 2020  nce" exp=""/>.  
-00005130: 2020 3c63 6f6e 7374 7261 696e 7420 6465    <constraint de
-00005140: 7363 3d22 2220 6669 656c 643d 2261 6e67  sc="" field="ang
-00005150: 6c65 2220 6578 703d 2222 2f3e 0a20 203c  le" exp=""/>.  <
-00005160: 2f63 6f6e 7374 7261 696e 7445 7870 7265  /constraintExpre
-00005170: 7373 696f 6e73 3e0a 2020 3c65 7870 7265  ssions>.  <expre
-00005180: 7373 696f 6e66 6965 6c64 732f 3e0a 2020  ssionfields/>.  
-00005190: 3c61 7474 7269 6275 7465 6163 7469 6f6e  <attributeaction
-000051a0: 733e 0a20 2020 203c 6465 6661 756c 7441  s>.    <defaultA
-000051b0: 6374 696f 6e20 6b65 793d 2243 616e 7661  ction key="Canva
-000051c0: 7322 2076 616c 7565 3d22 7b30 3030 3030  s" value="{00000
-000051d0: 3030 302d 3030 3030 2d30 3030 302d 3030  000-0000-0000-00
-000051e0: 3030 2d30 3030 3030 3030 3030 3030 307d  00-000000000000}
-000051f0: 222f 3e0a 2020 3c2f 6174 7472 6962 7574  "/>.  </attribut
-00005200: 6561 6374 696f 6e73 3e0a 2020 3c61 7474  eactions>.  <att
-00005210: 7269 6275 7465 7461 626c 6563 6f6e 6669  ributetableconfi
-00005220: 6720 736f 7274 4578 7072 6573 7369 6f6e  g sortExpression
-00005230: 3d22 2220 736f 7274 4f72 6465 723d 2230  ="" sortOrder="0
-00005240: 2220 6163 7469 6f6e 5769 6467 6574 5374  " actionWidgetSt
-00005250: 796c 653d 2264 726f 7044 6f77 6e22 3e0a  yle="dropDown">.
-00005260: 2020 2020 3c63 6f6c 756d 6e73 3e0a 2020      <columns>.  
-00005270: 2020 2020 3c63 6f6c 756d 6e20 6e61 6d65      <column name
-00005280: 3d22 7479 7065 2220 6869 6464 656e 3d22  ="type" hidden="
-00005290: 3022 2074 7970 653d 2266 6965 6c64 2220  0" type="field" 
-000052a0: 7769 6474 683d 222d 3122 2f3e 0a20 2020  width="-1"/>.   
-000052b0: 2020 203c 636f 6c75 6d6e 206e 616d 653d     <column name=
-000052c0: 226f 736d 5f69 6422 2068 6964 6465 6e3d  "osm_id" hidden=
-000052d0: 2230 2220 7479 7065 3d22 6669 656c 6422  "0" type="field"
-000052e0: 2077 6964 7468 3d22 3137 3122 2f3e 0a20   width="171"/>. 
-000052f0: 2020 2020 203c 636f 6c75 6d6e 206e 616d       <column nam
-00005300: 653d 226f 7269 656e 7461 7469 6f6e 2220  e="orientation" 
-00005310: 6869 6464 656e 3d22 3022 2074 7970 653d  hidden="0" type=
-00005320: 2266 6965 6c64 2220 7769 6474 683d 2232  "field" width="2
-00005330: 3932 222f 3e0a 2020 2020 2020 3c63 6f6c  92"/>.      <col
-00005340: 756d 6e20 6e61 6d65 3d22 6f72 6965 6e74  umn name="orient
-00005350: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
-00005360: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
-00005370: 653d 2266 6965 6c64 2220 7769 6474 683d  e="field" width=
-00005380: 222d 3122 2f3e 0a20 2020 2020 203c 636f  "-1"/>.      <co
-00005390: 6c75 6d6e 206e 616d 653d 2261 6e67 6c65  lumn name="angle
-000053a0: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
-000053b0: 653d 2266 6965 6c64 2220 7769 6474 683d  e="field" width=
-000053c0: 222d 3122 2f3e 0a20 2020 2020 203c 636f  "-1"/>.      <co
-000053d0: 6c75 6d6e 2068 6964 6465 6e3d 2231 2220  lumn hidden="1" 
-000053e0: 7479 7065 3d22 6163 7469 6f6e 7322 2077  type="actions" w
-000053f0: 6964 7468 3d22 2d31 222f 3e0a 2020 2020  idth="-1"/>.    
-00005400: 3c2f 636f 6c75 6d6e 733e 0a20 203c 2f61  </columns>.  </a
-00005410: 7474 7269 6275 7465 7461 626c 6563 6f6e  ttributetablecon
-00005420: 6669 673e 0a20 203c 636f 6e64 6974 696f  fig>.  <conditio
-00005430: 6e61 6c73 7479 6c65 733e 0a20 2020 203c  nalstyles>.    <
-00005440: 726f 7773 7479 6c65 732f 3e0a 2020 2020  rowstyles/>.    
-00005450: 3c66 6965 6c64 7374 796c 6573 2f3e 0a20  <fieldstyles/>. 
-00005460: 203c 2f63 6f6e 6469 7469 6f6e 616c 7374   </conditionalst
-00005470: 796c 6573 3e0a 2020 3c73 746f 7265 6465  yles>.  <storede
-00005480: 7870 7265 7373 696f 6e73 2f3e 0a20 203c  xpressions/>.  <
-00005490: 6564 6974 666f 726d 2074 6f6c 6572 616e  editform toleran
-000054a0: 743d 2231 223e 3c2f 6564 6974 666f 726d  t="1"></editform
-000054b0: 3e0a 2020 3c65 6469 7466 6f72 6d69 6e69  >.  <editformini
-000054c0: 742f 3e0a 2020 3c65 6469 7466 6f72 6d69  t/>.  <editformi
-000054d0: 6e69 7463 6f64 6573 6f75 7263 653e 303c  nitcodesource>0<
-000054e0: 2f65 6469 7466 6f72 6d69 6e69 7463 6f64  /editforminitcod
-000054f0: 6573 6f75 7263 653e 0a20 203c 6564 6974  esource>.  <edit
-00005500: 666f 726d 696e 6974 6669 6c65 7061 7468  forminitfilepath
-00005510: 3e3c 2f65 6469 7466 6f72 6d69 6e69 7466  ></editforminitf
-00005520: 696c 6570 6174 683e 0a20 203c 6564 6974  ilepath>.  <edit
-00005530: 666f 726d 696e 6974 636f 6465 3e3c 215b  forminitcode><![
-00005540: 4344 4154 415b 2320 2d2a 2d20 636f 6469  CDATA[# -*- codi
-00005550: 6e67 3a20 7574 662d 3820 2d2a 2d0a 2222  ng: utf-8 -*-.""
-00005560: 220a 4c65 7320 666f 726d 756c 6169 7265  ".Les formulaire
-00005570: 7320 5147 4953 2070 6575 7665 6e74 2061  s QGIS peuvent a
-00005580: 766f 6972 2075 6e65 2066 6f6e 6374 696f  voir une fonctio
-00005590: 6e20 5079 7468 6f6e 2071 7569 2065 7374  n Python qui est
-000055a0: 2061 7070 656c c3a9 6520 6c6f 7273 7175   appel..e lorsqu
-000055b0: 6520 6c65 2066 6f72 6d75 6c61 6972 6520  e le formulaire 
-000055c0: 6573 740a 6f75 7665 7274 2e0a 0a55 7469  est.ouvert...Uti
-000055d0: 6c69 7365 7a20 6365 7474 6520 666f 6e63  lisez cette fonc
-000055e0: 7469 6f6e 2070 6f75 7220 616a 6f75 7465  tion pour ajoute
-000055f0: 7220 756e 6520 6c6f 6769 7175 6520 7375  r une logique su
-00005600: 7070 6cc3 a96d 656e 7461 6972 6520 c3a0  ppl..mentaire ..
-00005610: 2076 6f73 2066 6f72 6d75 6c61 6972 6573   vos formulaires
-00005620: 2e0a 0a45 6e74 7265 7a20 6c65 206e 6f6d  ...Entrez le nom
-00005630: 2064 6520 6c61 2066 6f6e 6374 696f 6e20   de la fonction 
-00005640: 6461 6e73 206c 6520 6368 616d 7020 0a22  dans le champ ."
-00005650: 466f 6e63 7469 6f6e 2064 2769 6e69 7469  Fonction d'initi
-00005660: 616c 6973 6174 696f 6e20 5079 7468 6f6e  alisation Python
-00005670: 222e 0a56 6f69 6369 2075 6e20 6578 656d  "..Voici un exem
-00005680: 706c 653a 0a22 2222 0a66 726f 6d20 7167  ple:.""".from qg
-00005690: 6973 2e50 7951 742e 5174 5769 6467 6574  is.PyQt.QtWidget
-000056a0: 7320 696d 706f 7274 2051 5769 6467 6574  s import QWidget
-000056b0: 0a0a 6465 6620 6d79 5f66 6f72 6d5f 6f70  ..def my_form_op
-000056c0: 656e 2864 6961 6c6f 672c 206c 6179 6572  en(dialog, layer
-000056d0: 2c20 6665 6174 7572 6529 3a0a 2020 2020  , feature):.    
-000056e0: 6765 6f6d 203d 2066 6561 7475 7265 2e67  geom = feature.g
-000056f0: 656f 6d65 7472 7928 290a 2020 2020 636f  eometry().    co
-00005700: 6e74 726f 6c20 3d20 6469 616c 6f67 2e66  ntrol = dialog.f
-00005710: 696e 6443 6869 6c64 2851 5769 6467 6574  indChild(QWidget
-00005720: 2c20 224d 794c 696e 6545 6469 7422 290a  , "MyLineEdit").
-00005730: 5d5d 3e3c 2f65 6469 7466 6f72 6d69 6e69  ]]></editformini
-00005740: 7463 6f64 653e 0a20 203c 6665 6174 666f  tcode>.  <featfo
-00005750: 726d 7375 7070 7265 7373 3e30 3c2f 6665  rmsuppress>0</fe
-00005760: 6174 666f 726d 7375 7070 7265 7373 3e0a  atformsuppress>.
-00005770: 2020 3c65 6469 746f 726c 6179 6f75 743e    <editorlayout>
-00005780: 6765 6e65 7261 7465 646c 6179 6f75 743c  generatedlayout<
-00005790: 2f65 6469 746f 726c 6179 6f75 743e 0a20  /editorlayout>. 
-000057a0: 203c 6564 6974 6162 6c65 3e0a 2020 2020   <editable>.    
-000057b0: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
-000057c0: 6c65 2220 6564 6974 6162 6c65 3d22 3122  le" editable="1"
-000057d0: 2f3e 0a20 2020 203c 6669 656c 6420 6e61  />.    <field na
-000057e0: 6d65 3d22 6f72 6965 6e74 6174 696f 6e22  me="orientation"
-000057f0: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
-00005800: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00005810: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
-00005820: 6669 6465 6e63 6522 2065 6469 7461 626c  fidence" editabl
-00005830: 653d 2231 222f 3e0a 2020 2020 3c66 6965  e="1"/>.    <fie
-00005840: 6c64 206e 616d 653d 226f 736d 5f69 6422  ld name="osm_id"
-00005850: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
-00005860: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00005870: 2274 7970 6522 2065 6469 7461 626c 653d  "type" editable=
-00005880: 2231 222f 3e0a 2020 3c2f 6564 6974 6162  "1"/>.  </editab
-00005890: 6c65 3e0a 2020 3c6c 6162 656c 4f6e 546f  le>.  <labelOnTo
-000058a0: 703e 0a20 2020 203c 6669 656c 6420 6e61  p>.    <field na
-000058b0: 6d65 3d22 616e 676c 6522 206c 6162 656c  me="angle" label
-000058c0: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
-000058d0: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
-000058e0: 656e 7461 7469 6f6e 2220 6c61 6265 6c4f  entation" labelO
-000058f0: 6e54 6f70 3d22 3022 2f3e 0a20 2020 203c  nTop="0"/>.    <
-00005900: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
-00005910: 6e74 6174 696f 6e5f 636f 6e66 6964 656e  ntation_confiden
-00005920: 6365 2220 6c61 6265 6c4f 6e54 6f70 3d22  ce" labelOnTop="
-00005930: 3022 2f3e 0a20 2020 203c 6669 656c 6420  0"/>.    <field 
-00005940: 6e61 6d65 3d22 6f73 6d5f 6964 2220 6c61  name="osm_id" la
-00005950: 6265 6c4f 6e54 6f70 3d22 3022 2f3e 0a20  belOnTop="0"/>. 
-00005960: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-00005970: 7479 7065 2220 6c61 6265 6c4f 6e54 6f70  type" labelOnTop
-00005980: 3d22 3022 2f3e 0a20 203c 2f6c 6162 656c  ="0"/>.  </label
-00005990: 4f6e 546f 703e 0a20 203c 7265 7573 654c  OnTop>.  <reuseL
-000059a0: 6173 7456 616c 7565 3e0a 2020 2020 3c66  astValue>.    <f
-000059b0: 6965 6c64 206e 616d 653d 2261 6e67 6c65  ield name="angle
-000059c0: 2220 7265 7573 654c 6173 7456 616c 7565  " reuseLastValue
-000059d0: 3d22 3022 2f3e 0a20 2020 203c 6669 656c  ="0"/>.    <fiel
-000059e0: 6420 6e61 6d65 3d22 6f72 6965 6e74 6174  d name="orientat
-000059f0: 696f 6e22 2072 6575 7365 4c61 7374 5661  ion" reuseLastVa
-00005a00: 6c75 653d 2230 222f 3e0a 2020 2020 3c66  lue="0"/>.    <f
-00005a10: 6965 6c64 206e 616d 653d 226f 7269 656e  ield name="orien
-00005a20: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
-00005a30: 6522 2072 6575 7365 4c61 7374 5661 6c75  e" reuseLastValu
-00005a40: 653d 2230 222f 3e0a 2020 2020 3c66 6965  e="0"/>.    <fie
-00005a50: 6c64 206e 616d 653d 226f 736d 5f69 6422  ld name="osm_id"
-00005a60: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
-00005a70: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
-00005a80: 206e 616d 653d 2274 7970 6522 2072 6575   name="type" reu
-00005a90: 7365 4c61 7374 5661 6c75 653d 2230 222f  seLastValue="0"/
-00005aa0: 3e0a 2020 3c2f 7265 7573 654c 6173 7456  >.  </reuseLastV
-00005ab0: 616c 7565 3e0a 2020 3c64 6174 6144 6566  alue>.  <dataDef
-00005ac0: 696e 6564 4669 656c 6450 726f 7065 7274  inedFieldPropert
-00005ad0: 6965 732f 3e0a 2020 3c77 6964 6765 7473  ies/>.  <widgets
-00005ae0: 2f3e 0a20 203c 7072 6576 6965 7745 7870  />.  <previewExp
-00005af0: 7265 7373 696f 6e3e 2274 7970 6522 3c2f  ression>"type"</
-00005b00: 7072 6576 6965 7745 7870 7265 7373 696f  previewExpressio
-00005b10: 6e3e 0a20 203c 6d61 7054 6970 3e3c 2f6d  n>.  <mapTip></m
-00005b20: 6170 5469 703e 0a20 203c 6c61 7965 7247  apTip>.  <layerG
-00005b30: 656f 6d65 7472 7954 7970 653e 303c 2f6c  eometryType>0</l
-00005b40: 6179 6572 4765 6f6d 6574 7279 5479 7065  ayerGeometryType
-00005b50: 3e0a 3c2f 7167 6973 3e0a                 >.</qgis>.
+00002960: 6f6e 206e 616d 653d 2273 697a 655f 756e  on name="size_un
+00002970: 6974 2220 7661 6c75 653d 2252 656e 6465  it" value="Rende
+00002980: 724d 6574 6572 7349 6e4d 6170 556e 6974  rMetersInMapUnit
+00002990: 7322 2074 7970 653d 2251 5374 7269 6e67  s" type="QString
+000029a0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000029b0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7665  <Option name="ve
+000029c0: 7274 6963 616c 5f61 6e63 686f 725f 706f  rtical_anchor_po
+000029d0: 696e 7422 2076 616c 7565 3d22 3122 2074  int" value="1" t
+000029e0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+000029f0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00002a00: 6f6e 3e0a 2020 2020 2020 2020 2020 3c64  on>.          <d
+00002a10: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+00002a20: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+00002a30: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
+00002a40: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00002a50: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00002a60: 6d65 3d22 6e61 6d65 2220 7661 6c75 653d  me="name" value=
+00002a70: 2222 2074 7970 653d 2251 5374 7269 6e67  "" type="QString
+00002a80: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00002a90: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00002aa0: 7072 6f70 6572 7469 6573 2220 7479 7065  properties" type
+00002ab0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00002ac0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00002ad0: 6e61 6d65 3d22 616e 676c 6522 2074 7970  name="angle" typ
+00002ae0: 653d 224d 6170 223e 0a20 2020 2020 2020  e="Map">.       
+00002af0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002b00: 6f6e 206e 616d 653d 2261 6374 6976 6522  on name="active"
+00002b10: 2076 616c 7565 3d22 7472 7565 2220 7479   value="true" ty
+00002b20: 7065 3d22 626f 6f6c 222f 3e0a 2020 2020  pe="bool"/>.    
+00002b30: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00002b40: 7074 696f 6e20 6e61 6d65 3d22 6578 7072  ption name="expr
+00002b50: 6573 7369 6f6e 2220 7661 6c75 653d 2231  ession" value="1
+00002b60: 3830 202b 2028 2d26 7175 6f74 3b6f 7269  80 + (-&quot;ori
+00002b70: 656e 7461 7469 6f6e 2671 756f 743b 202f  entation&quot; /
+00002b80: 2070 6928 2929 202a 2031 3830 2220 7479   pi()) * 180" ty
+00002b90: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 203c 4f70 7469 6f6e 206e 616d 653d 2274   <Option name="t
+00002bc0: 7970 6522 2076 616c 7565 3d22 3322 2074  ype" value="3" t
+00002bd0: 7970 653d 2269 6e74 222f 3e0a 2020 2020  ype="int"/>.    
+00002be0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+00002bf0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00002c00: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00002c10: 6d65 3d22 6f75 746c 696e 6557 6964 7468  me="outlineWidth
+00002c20: 2220 7479 7065 3d22 4d61 7022 3e0a 2020  " type="Map">.  
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6163  <Option name="ac
+00002c50: 7469 7665 2220 7661 6c75 653d 2274 7275  tive" value="tru
+00002c60: 6522 2074 7970 653d 2262 6f6f 6c22 2f3e  e" type="bool"/>
+00002c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c80: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00002c90: 2265 7870 7265 7373 696f 6e22 2076 616c  "expression" val
+00002ca0: 7565 3d22 2671 756f 743b 6c61 6e65 5f77  ue="&quot;lane_w
+00002cb0: 6964 7468 2671 756f 743b 202a 2030 2e37  idth&quot; * 0.7
+00002cc0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00002cd0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00002ce0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00002cf0: 653d 2274 7970 6522 2076 616c 7565 3d22  e="type" value="
+00002d00: 3322 2074 7970 653d 2269 6e74 222f 3e0a  3" type="int"/>.
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
+00002d30: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
+00002d40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002d50: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
+00002d60: 7065 2220 7661 6c75 653d 2263 6f6c 6c65  pe" value="colle
+00002d70: 6374 696f 6e22 2074 7970 653d 2251 5374  ction" type="QSt
+00002d80: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00002d90: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00002da0: 2020 2020 2020 2020 3c2f 6461 7461 5f64          </data_d
+00002db0: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
+00002dc0: 733e 0a20 2020 2020 2020 203c 2f6c 6179  s>.        </lay
+00002dd0: 6572 3e0a 2020 2020 2020 3c2f 7379 6d62  er>.      </symb
+00002de0: 6f6c 3e0a 2020 2020 2020 3c73 796d 626f  ol>.      <symbo
+00002df0: 6c20 6e61 6d65 3d22 3122 2066 6f72 6365  l name="1" force
+00002e00: 5f72 6872 3d22 3022 2066 7261 6d65 5f72  _rhr="0" frame_r
+00002e10: 6174 653d 2231 3022 2061 6c70 6861 3d22  ate="10" alpha="
+00002e20: 3122 2063 6c69 705f 746f 5f65 7874 656e  1" clip_to_exten
+00002e30: 743d 2231 2220 6973 5f61 6e69 6d61 7465  t="1" is_animate
+00002e40: 643d 2230 2220 7479 7065 3d22 6d61 726b  d="0" type="mark
+00002e50: 6572 223e 0a20 2020 2020 2020 203c 6461  er">.        <da
+00002e60: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+00002e70: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+00002e80: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
+00002e90: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
+00002ea0: 203c 4f70 7469 6f6e 206e 616d 653d 226e   <Option name="n
+00002eb0: 616d 6522 2076 616c 7565 3d22 2220 7479  ame" value="" ty
+00002ec0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00002ed0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002ee0: 6f6e 206e 616d 653d 2270 726f 7065 7274  on name="propert
+00002ef0: 6965 7322 2f3e 0a20 2020 2020 2020 2020  ies"/>.         
+00002f00: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00002f10: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
+00002f20: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
+00002f30: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00002f40: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00002f50: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
+00002f60: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
+00002f70: 3e0a 2020 2020 2020 2020 3c6c 6179 6572  >.        <layer
+00002f80: 2070 6173 733d 2230 2220 6c6f 636b 6564   pass="0" locked
+00002f90: 3d22 3022 2065 6e61 626c 6564 3d22 3122  ="0" enabled="1"
+00002fa0: 2063 6c61 7373 3d22 5369 6d70 6c65 4d61   class="SimpleMa
+00002fb0: 726b 6572 223e 0a20 2020 2020 2020 2020  rker">.         
+00002fc0: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
+00002fd0: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
+00002fe0: 203c 4f70 7469 6f6e 206e 616d 653d 2261   <Option name="a
+00002ff0: 6e67 6c65 2220 7661 6c75 653d 2230 2220  ngle" value="0" 
+00003000: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00003010: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00003020: 7469 6f6e 206e 616d 653d 2263 6170 5f73  tion name="cap_s
+00003030: 7479 6c65 2220 7661 6c75 653d 2266 6c61  tyle" value="fla
+00003040: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00003050: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003060: 3c4f 7074 696f 6e20 6e61 6d65 3d22 636f  <Option name="co
+00003070: 6c6f 7222 2076 616c 7565 3d22 3233 322c  lor" value="232,
+00003080: 3835 2c30 2c32 3535 2220 7479 7065 3d22  85,0,255" type="
+00003090: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000030a0: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+000030b0: 616d 653d 2268 6f72 697a 6f6e 7461 6c5f  ame="horizontal_
+000030c0: 616e 6368 6f72 5f70 6f69 6e74 2220 7661  anchor_point" va
+000030d0: 6c75 653d 2231 2220 7479 7065 3d22 5153  lue="1" type="QS
+000030e0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000030f0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00003100: 653d 226a 6f69 6e73 7479 6c65 2220 7661  e="joinstyle" va
+00003110: 6c75 653d 2262 6576 656c 2220 7479 7065  lue="bevel" type
+00003120: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003130: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003140: 206e 616d 653d 226e 616d 6522 2076 616c   name="name" val
+00003150: 7565 3d22 6c69 6e65 2220 7479 7065 3d22  ue="line" type="
+00003160: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003170: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00003180: 616d 653d 226f 6666 7365 7422 2076 616c  ame="offset" val
+00003190: 7565 3d22 302c 3022 2074 7970 653d 2251  ue="0,0" type="Q
+000031a0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000031b0: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+000031c0: 6d65 3d22 6f66 6673 6574 5f6d 6170 5f75  me="offset_map_u
+000031d0: 6e69 745f 7363 616c 6522 2076 616c 7565  nit_scale" value
+000031e0: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
+000031f0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003200: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003210: 4f70 7469 6f6e 206e 616d 653d 226f 6666  Option name="off
+00003220: 7365 745f 756e 6974 2220 7661 6c75 653d  set_unit" value=
+00003230: 224d 4d22 2074 7970 653d 2251 5374 7269  "MM" type="QStri
+00003240: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003250: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00003260: 6f75 746c 696e 655f 636f 6c6f 7222 2076  outline_color" v
+00003270: 616c 7565 3d22 3235 352c 3235 352c 3235  alue="255,255,25
+00003280: 352c 3235 3522 2074 7970 653d 2251 5374  5,255" type="QSt
+00003290: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000032a0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+000032b0: 3d22 6f75 746c 696e 655f 7374 796c 6522  ="outline_style"
+000032c0: 2076 616c 7565 3d22 736f 6c69 6422 2074   value="solid" t
+000032d0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+000032e0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000032f0: 696f 6e20 6e61 6d65 3d22 6f75 746c 696e  ion name="outlin
+00003300: 655f 7769 6474 6822 2076 616c 7565 3d22  e_width" value="
+00003310: 3222 2074 7970 653d 2251 5374 7269 6e67  2" type="QString
+00003320: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003330: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
+00003340: 746c 696e 655f 7769 6474 685f 6d61 705f  tline_width_map_
+00003350: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
+00003360: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+00003370: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
+00003380: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003390: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6f75  <Option name="ou
+000033a0: 746c 696e 655f 7769 6474 685f 756e 6974  tline_width_unit
+000033b0: 2220 7661 6c75 653d 2252 656e 6465 724d  " value="RenderM
+000033c0: 6574 6572 7349 6e4d 6170 556e 6974 7322  etersInMapUnits"
+000033d0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000033e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+000033f0: 7074 696f 6e20 6e61 6d65 3d22 7363 616c  ption name="scal
+00003400: 655f 6d65 7468 6f64 2220 7661 6c75 653d  e_method" value=
+00003410: 2264 6961 6d65 7465 7222 2074 7970 653d  "diameter" type=
+00003420: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003430: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003440: 6e61 6d65 3d22 7369 7a65 2220 7661 6c75  name="size" valu
+00003450: 653d 2233 2220 7479 7065 3d22 5153 7472  e="3" type="QStr
+00003460: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003470: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00003480: 2273 697a 655f 6d61 705f 756e 6974 5f73  "size_map_unit_s
+00003490: 6361 6c65 2220 7661 6c75 653d 2233 783a  cale" value="3x:
+000034a0: 302c 302c 302c 302c 302c 3022 2074 7970  0,0,0,0,0,0" typ
+000034b0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000034c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000034d0: 6e20 6e61 6d65 3d22 7369 7a65 5f75 6e69  n name="size_uni
+000034e0: 7422 2076 616c 7565 3d22 5265 6e64 6572  t" value="Render
+000034f0: 4d65 7465 7273 496e 4d61 7055 6e69 7473  MetersInMapUnits
+00003500: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003510: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003520: 4f70 7469 6f6e 206e 616d 653d 2276 6572  Option name="ver
+00003530: 7469 6361 6c5f 616e 6368 6f72 5f70 6f69  tical_anchor_poi
+00003540: 6e74 2220 7661 6c75 653d 2231 2220 7479  nt" value="1" ty
+00003550: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003560: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00003570: 6e3e 0a20 2020 2020 2020 2020 203c 6461  n>.          <da
+00003580: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+00003590: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+000035a0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+000035b0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+000035c0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000035d0: 653d 226e 616d 6522 2076 616c 7565 3d22  e="name" value="
+000035e0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000035f0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00003600: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00003610: 726f 7065 7274 6965 7322 2074 7970 653d  roperties" type=
+00003620: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00003630: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00003640: 616d 653d 2261 6e67 6c65 2220 7479 7065  ame="angle" type
+00003650: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00003660: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003670: 6e20 6e61 6d65 3d22 6163 7469 7665 2220  n name="active" 
+00003680: 7661 6c75 653d 2274 7275 6522 2074 7970  value="true" typ
+00003690: 653d 2262 6f6f 6c22 2f3e 0a20 2020 2020  e="bool"/>.     
+000036a0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+000036b0: 7469 6f6e 206e 616d 653d 2265 7870 7265  tion name="expre
+000036c0: 7373 696f 6e22 2076 616c 7565 3d22 3138  ssion" value="18
+000036d0: 3020 2b20 282d 2671 756f 743b 6f72 6965  0 + (-&quot;orie
+000036e0: 6e74 6174 696f 6e26 7175 6f74 3b20 2f20  ntation&quot; / 
+000036f0: 7069 2829 2920 2a20 3138 3022 2074 7970  pi()) * 180" typ
+00003700: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7479  <Option name="ty
+00003730: 7065 2220 7661 6c75 653d 2233 2220 7479  pe" value="3" ty
+00003740: 7065 3d22 696e 7422 2f3e 0a20 2020 2020  pe="int"/>.     
+00003750: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+00003760: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00003770: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00003780: 653d 226f 7574 6c69 6e65 5769 6474 6822  e="outlineWidth"
+00003790: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
+000037a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000037b0: 4f70 7469 6f6e 206e 616d 653d 2261 6374  Option name="act
+000037c0: 6976 6522 2076 616c 7565 3d22 7472 7565  ive" value="true
+000037d0: 2220 7479 7065 3d22 626f 6f6c 222f 3e0a  " type="bool"/>.
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00003800: 6578 7072 6573 7369 6f6e 2220 7661 6c75  expression" valu
+00003810: 653d 2226 7175 6f74 3b6c 616e 655f 7769  e="&quot;lane_wi
+00003820: 6474 6826 7175 6f74 3b22 2074 7970 653d  dth&quot;" type=
+00003830: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003840: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00003850: 7074 696f 6e20 6e61 6d65 3d22 7479 7065  ption name="type
+00003860: 2220 7661 6c75 653d 2233 2220 7479 7065  " value="3" type
+00003870: 3d22 696e 7422 2f3e 0a20 2020 2020 2020  ="int"/>.       
+00003880: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
+00003890: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+000038a0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+000038b0: 2273 697a 6522 2074 7970 653d 224d 6170  "size" type="Map
+000038c0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000038d0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000038e0: 653d 2261 6374 6976 6522 2076 616c 7565  e="active" value
+000038f0: 3d22 7472 7565 2220 7479 7065 3d22 626f  ="true" type="bo
+00003900: 6f6c 222f 3e0a 2020 2020 2020 2020 2020  ol"/>.          
+00003910: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003920: 6e61 6d65 3d22 6578 7072 6573 7369 6f6e  name="expression
+00003930: 2220 7661 6c75 653d 2233 202d 2032 202a  " value="3 - 2 *
+00003940: 2030 2e30 3031 202a 2040 6d61 705f 7363   0.001 * @map_sc
+00003950: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+00003960: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003970: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003980: 6e61 6d65 3d22 7479 7065 2220 7661 6c75  name="type" valu
+00003990: 653d 2233 2220 7479 7065 3d22 696e 7422  e="3" type="int"
+000039a0: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+000039b0: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+000039c0: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
+000039d0: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+000039e0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+000039f0: 2274 7970 6522 2076 616c 7565 3d22 636f  "type" value="co
+00003a00: 6c6c 6563 7469 6f6e 2220 7479 7065 3d22  llection" type="
+00003a10: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003a20: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
+00003a30: 0a20 2020 2020 2020 2020 203c 2f64 6174  .          </dat
+00003a40: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+00003a50: 7469 6573 3e0a 2020 2020 2020 2020 3c2f  ties>.        </
+00003a60: 6c61 7965 723e 0a20 2020 2020 203c 2f73  layer>.      </s
+00003a70: 796d 626f 6c3e 0a20 2020 2020 203c 7379  ymbol>.      <sy
+00003a80: 6d62 6f6c 206e 616d 653d 2232 2220 666f  mbol name="2" fo
+00003a90: 7263 655f 7268 723d 2230 2220 6672 616d  rce_rhr="0" fram
+00003aa0: 655f 7261 7465 3d22 3130 2220 616c 7068  e_rate="10" alph
+00003ab0: 613d 2231 2220 636c 6970 5f74 6f5f 6578  a="1" clip_to_ex
+00003ac0: 7465 6e74 3d22 3122 2069 735f 616e 696d  tent="1" is_anim
+00003ad0: 6174 6564 3d22 3022 2074 7970 653d 226d  ated="0" type="m
+00003ae0: 6172 6b65 7222 3e0a 2020 2020 2020 2020  arker">.        
+00003af0: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
+00003b00: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+00003b10: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
+00003b20: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00003b30: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00003b40: 3d22 6e61 6d65 2220 7661 6c75 653d 2222  ="name" value=""
+00003b50: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003b60: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003b70: 7074 696f 6e20 6e61 6d65 3d22 7072 6f70  ption name="prop
+00003b80: 6572 7469 6573 222f 3e0a 2020 2020 2020  erties"/>.      
+00003b90: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00003ba0: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
+00003bb0: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
+00003bc0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003bd0: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
+00003be0: 3e0a 2020 2020 2020 2020 3c2f 6461 7461  >.        </data
+00003bf0: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
+00003c00: 6965 733e 0a20 2020 2020 2020 203c 6c61  ies>.        <la
+00003c10: 7965 7220 7061 7373 3d22 3022 206c 6f63  yer pass="0" loc
+00003c20: 6b65 643d 2230 2220 656e 6162 6c65 643d  ked="0" enabled=
+00003c30: 2231 2220 636c 6173 733d 2253 696d 706c  "1" class="Simpl
+00003c40: 654d 6172 6b65 7222 3e0a 2020 2020 2020  eMarker">.      
+00003c50: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
+00003c60: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
+00003c70: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+00003c80: 3d22 616e 676c 6522 2076 616c 7565 3d22  ="angle" value="
+00003c90: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
+00003ca0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003cb0: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6361  <Option name="ca
+00003cc0: 705f 7374 796c 6522 2076 616c 7565 3d22  p_style" value="
+00003cd0: 666c 6174 2220 7479 7065 3d22 5153 7472  flat" type="QStr
+00003ce0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003cf0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00003d00: 2263 6f6c 6f72 2220 7661 6c75 653d 2232  "color" value="2
+00003d10: 3332 2c38 352c 302c 3235 3522 2074 7970  32,85,0,255" typ
+00003d20: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003d30: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003d40: 6e20 6e61 6d65 3d22 686f 7269 7a6f 6e74  n name="horizont
+00003d50: 616c 5f61 6e63 686f 725f 706f 696e 7422  al_anchor_point"
+00003d60: 2076 616c 7565 3d22 3122 2074 7970 653d   value="1" type=
+00003d70: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003d80: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003d90: 6e61 6d65 3d22 6a6f 696e 7374 796c 6522  name="joinstyle"
+00003da0: 2076 616c 7565 3d22 6265 7665 6c22 2074   value="bevel" t
+00003db0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003dc0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003dd0: 696f 6e20 6e61 6d65 3d22 6e61 6d65 2220  ion name="name" 
+00003de0: 7661 6c75 653d 226c 696e 6522 2074 7970  value="line" typ
+00003df0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003e00: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003e10: 6e20 6e61 6d65 3d22 6f66 6673 6574 2220  n name="offset" 
+00003e20: 7661 6c75 653d 2230 2c30 2220 7479 7065  value="0,0" type
+00003e30: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00003e40: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00003e50: 206e 616d 653d 226f 6666 7365 745f 6d61   name="offset_ma
+00003e60: 705f 756e 6974 5f73 6361 6c65 2220 7661  p_unit_scale" va
+00003e70: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
+00003e80: 302c 3022 2074 7970 653d 2251 5374 7269  0,0" type="QStri
+00003e90: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003ea0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00003eb0: 6f66 6673 6574 5f75 6e69 7422 2076 616c  offset_unit" val
+00003ec0: 7565 3d22 4d4d 2220 7479 7065 3d22 5153  ue="MM" type="QS
+00003ed0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00003ee0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00003ef0: 653d 226f 7574 6c69 6e65 5f63 6f6c 6f72  e="outline_color
+00003f00: 2220 7661 6c75 653d 2232 3535 2c32 3535  " value="255,255
+00003f10: 2c32 3535 2c32 3535 2220 7479 7065 3d22  ,255,255" type="
+00003f20: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003f30: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00003f40: 616d 653d 226f 7574 6c69 6e65 5f73 7479  ame="outline_sty
+00003f50: 6c65 2220 7661 6c75 653d 2273 6f6c 6964  le" value="solid
+00003f60: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003f70: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003f80: 4f70 7469 6f6e 206e 616d 653d 226f 7574  Option name="out
+00003f90: 6c69 6e65 5f77 6964 7468 2220 7661 6c75  line_width" valu
+00003fa0: 653d 2232 2220 7479 7065 3d22 5153 7472  e="2" type="QStr
+00003fb0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003fc0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00003fd0: 226f 7574 6c69 6e65 5f77 6964 7468 5f6d  "outline_width_m
+00003fe0: 6170 5f75 6e69 745f 7363 616c 6522 2076  ap_unit_scale" v
+00003ff0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00004000: 2c30 2c30 2220 7479 7065 3d22 5153 7472  ,0,0" type="QStr
+00004010: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004020: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00004030: 226f 7574 6c69 6e65 5f77 6964 7468 5f75  "outline_width_u
+00004040: 6e69 7422 2076 616c 7565 3d22 5265 6e64  nit" value="Rend
+00004050: 6572 4d65 7465 7273 496e 4d61 7055 6e69  erMetersInMapUni
+00004060: 7473 2220 7479 7065 3d22 5153 7472 696e  ts" type="QStrin
+00004070: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004080: 203c 4f70 7469 6f6e 206e 616d 653d 2273   <Option name="s
+00004090: 6361 6c65 5f6d 6574 686f 6422 2076 616c  cale_method" val
+000040a0: 7565 3d22 6469 616d 6574 6572 2220 7479  ue="diameter" ty
+000040b0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000040c0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000040d0: 6f6e 206e 616d 653d 2273 697a 6522 2076  on name="size" v
+000040e0: 616c 7565 3d22 3322 2074 7970 653d 2251  alue="3" type="Q
+000040f0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00004100: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00004110: 6d65 3d22 7369 7a65 5f6d 6170 5f75 6e69  me="size_map_uni
+00004120: 745f 7363 616c 6522 2076 616c 7565 3d22  t_scale" value="
+00004130: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
+00004140: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004150: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00004160: 7469 6f6e 206e 616d 653d 2273 697a 655f  tion name="size_
+00004170: 756e 6974 2220 7661 6c75 653d 2252 656e  unit" value="Ren
+00004180: 6465 724d 6574 6572 7349 6e4d 6170 556e  derMetersInMapUn
+00004190: 6974 7322 2074 7970 653d 2251 5374 7269  its" type="QStri
+000041a0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000041b0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+000041c0: 7665 7274 6963 616c 5f61 6e63 686f 725f  vertical_anchor_
+000041d0: 706f 696e 7422 2076 616c 7565 3d22 3122  point" value="1"
+000041e0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+000041f0: 3e0a 2020 2020 2020 2020 2020 3c2f 4f70  >.          </Op
+00004200: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00004210: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
+00004220: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+00004230: 2020 2020 2020 3c4f 7074 696f 6e20 7479        <Option ty
+00004240: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
+00004250: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00004260: 6e61 6d65 3d22 6e61 6d65 2220 7661 6c75  name="name" valu
+00004270: 653d 2222 2074 7970 653d 2251 5374 7269  e="" type="QStri
+00004280: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004290: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+000042a0: 3d22 7072 6f70 6572 7469 6573 2220 7479  ="properties" ty
+000042b0: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
+000042c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000042d0: 6e20 6e61 6d65 3d22 616e 676c 6522 2074  n name="angle" t
+000042e0: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
+000042f0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00004300: 7469 6f6e 206e 616d 653d 2261 6374 6976  tion name="activ
+00004310: 6522 2076 616c 7565 3d22 7472 7565 2220  e" value="true" 
+00004320: 7479 7065 3d22 626f 6f6c 222f 3e0a 2020  type="bool"/>.  
+00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004340: 3c4f 7074 696f 6e20 6e61 6d65 3d22 6578  <Option name="ex
+00004350: 7072 6573 7369 6f6e 2220 7661 6c75 653d  pression" value=
+00004360: 2231 3830 202b 2028 2d26 7175 6f74 3b6f  "180 + (-&quot;o
+00004370: 7269 656e 7461 7469 6f6e 2671 756f 743b  rientation&quot;
+00004380: 202f 2070 6928 2929 202a 2031 3830 2220   / pi()) * 180" 
+00004390: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000043a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000043b0: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+000043c0: 2274 7970 6522 2076 616c 7565 3d22 3322  "type" value="3"
+000043d0: 2074 7970 653d 2269 6e74 222f 3e0a 2020   type="int"/>.  
+000043e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000043f0: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00004400: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00004410: 6e61 6d65 3d22 6f75 746c 696e 6557 6964  name="outlineWid
+00004420: 7468 2220 7479 7065 3d22 4d61 7022 3e0a  th" type="Map">.
+00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004440: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00004450: 6163 7469 7665 2220 7661 6c75 653d 2274  active" value="t
+00004460: 7275 6522 2074 7970 653d 2262 6f6f 6c22  rue" type="bool"
+00004470: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00004480: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00004490: 653d 2265 7870 7265 7373 696f 6e22 2076  e="expression" v
+000044a0: 616c 7565 3d22 2671 756f 743b 6c61 6e65  alue="&quot;lane
+000044b0: 5f77 6964 7468 2671 756f 743b 2220 7479  _width&quot;" ty
+000044c0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044e0: 203c 4f70 7469 6f6e 206e 616d 653d 2274   <Option name="t
+000044f0: 7970 6522 2076 616c 7565 3d22 3322 2074  ype" value="3" t
+00004500: 7970 653d 2269 6e74 222f 3e0a 2020 2020  ype="int"/>.    
+00004510: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+00004520: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+00004530: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00004540: 6d65 3d22 7369 7a65 2220 7479 7065 3d22  me="size" type="
+00004550: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
+00004560: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00004570: 6e61 6d65 3d22 6163 7469 7665 2220 7661  name="active" va
+00004580: 6c75 653d 2274 7275 6522 2074 7970 653d  lue="true" type=
+00004590: 2262 6f6f 6c22 2f3e 0a20 2020 2020 2020  "bool"/>.       
+000045a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000045b0: 6f6e 206e 616d 653d 2265 7870 7265 7373  on name="express
+000045c0: 696f 6e22 2076 616c 7565 3d22 3320 2d20  ion" value="3 - 
+000045d0: 3220 2a20 302e 3030 3220 2a20 406d 6170  2 * 0.002 * @map
+000045e0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
+000045f0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00004600: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00004610: 6f6e 206e 616d 653d 2274 7970 6522 2076  on name="type" v
+00004620: 616c 7565 3d22 3322 2074 7970 653d 2269  alue="3" type="i
+00004630: 6e74 222f 3e0a 2020 2020 2020 2020 2020  nt"/>.          
+00004640: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+00004650: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00004660: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
+00004670: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00004680: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
+00004690: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
+000046a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000046b0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+000046c0: 6f6e 3e0a 2020 2020 2020 2020 2020 3c2f  on>.          </
+000046d0: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
+000046e0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
+000046f0: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
+00004700: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 3c2f  </symbol>.    </
+00004710: 7379 6d62 6f6c 733e 0a20 203c 2f72 656e  symbols>.  </ren
+00004720: 6465 7265 722d 7632 3e0a 2020 3c63 7573  derer-v2>.  <cus
+00004730: 746f 6d70 726f 7065 7274 6965 733e 0a20  tomproperties>. 
+00004740: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+00004750: 224d 6170 223e 0a20 2020 2020 203c 4f70  "Map">.      <Op
+00004760: 7469 6f6e 206e 616d 653d 2264 7561 6c76  tion name="dualv
+00004770: 6965 772f 7072 6576 6965 7745 7870 7265  iew/previewExpre
+00004780: 7373 696f 6e73 2220 7479 7065 3d22 4c69  ssions" type="Li
+00004790: 7374 223e 0a20 2020 2020 2020 203c 4f70  st">.        <Op
+000047a0: 7469 6f6e 2076 616c 7565 3d22 2671 756f  tion value="&quo
+000047b0: 743b 7479 7065 2671 756f 743b 2220 7479  t;type&quot;" ty
+000047c0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000047d0: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+000047e0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000047f0: 653d 2265 6d62 6564 6465 6457 6964 6765  e="embeddedWidge
+00004800: 7473 2f63 6f75 6e74 2220 7661 6c75 653d  ts/count" value=
+00004810: 2230 2220 7479 7065 3d22 696e 7422 2f3e  "0" type="int"/>
+00004820: 0a20 2020 2020 203c 4f70 7469 6f6e 206e  .      <Option n
+00004830: 616d 653d 2276 6172 6961 626c 654e 616d  ame="variableNam
+00004840: 6573 222f 3e0a 2020 2020 2020 3c4f 7074  es"/>.      <Opt
+00004850: 696f 6e20 6e61 6d65 3d22 7661 7269 6162  ion name="variab
+00004860: 6c65 5661 6c75 6573 222f 3e0a 2020 2020  leValues"/>.    
+00004870: 3c2f 4f70 7469 6f6e 3e0a 2020 3c2f 6375  </Option>.  </cu
+00004880: 7374 6f6d 7072 6f70 6572 7469 6573 3e0a  stomproperties>.
+00004890: 2020 3c62 6c65 6e64 4d6f 6465 3e30 3c2f    <blendMode>0</
+000048a0: 626c 656e 644d 6f64 653e 0a20 203c 6665  blendMode>.  <fe
+000048b0: 6174 7572 6542 6c65 6e64 4d6f 6465 3e30  atureBlendMode>0
+000048c0: 3c2f 6665 6174 7572 6542 6c65 6e64 4d6f  </featureBlendMo
+000048d0: 6465 3e0a 2020 3c6c 6179 6572 4f70 6163  de>.  <layerOpac
+000048e0: 6974 793e 313c 2f6c 6179 6572 4f70 6163  ity>1</layerOpac
+000048f0: 6974 793e 0a20 203c 5369 6e67 6c65 4361  ity>.  <SingleCa
+00004900: 7465 676f 7279 4469 6167 7261 6d52 656e  tegoryDiagramRen
+00004910: 6465 7265 7220 6174 7472 6962 7574 654c  derer attributeL
+00004920: 6567 656e 643d 2231 2220 6469 6167 7261  egend="1" diagra
+00004930: 6d54 7970 653d 2248 6973 746f 6772 616d  mType="Histogram
+00004940: 223e 0a20 2020 203c 4469 6167 7261 6d43  ">.    <DiagramC
+00004950: 6174 6567 6f72 7920 7065 6e41 6c70 6861  ategory penAlpha
+00004960: 3d22 3235 3522 2068 6569 6768 743d 2231  ="255" height="1
+00004970: 3522 2073 7061 6369 6e67 556e 6974 5363  5" spacingUnitSc
+00004980: 616c 653d 2233 783a 302c 302c 302c 302c  ale="3x:0,0,0,0,
+00004990: 302c 3022 206f 7061 6369 7479 3d22 3122  0,0" opacity="1"
+000049a0: 206d 6178 5363 616c 6544 656e 6f6d 696e   maxScaleDenomin
+000049b0: 6174 6f72 3d22 3165 2b30 3822 206c 6162  ator="1e+08" lab
+000049c0: 656c 506c 6163 656d 656e 744d 6574 686f  elPlacementMetho
+000049d0: 643d 2258 4865 6967 6874 2220 6469 7265  d="XHeight" dire
+000049e0: 6374 696f 6e3d 2230 2220 6c69 6e65 5369  ction="0" lineSi
+000049f0: 7a65 5363 616c 653d 2233 783a 302c 302c  zeScale="3x:0,0,
+00004a00: 302c 302c 302c 3022 2064 6961 6772 616d  0,0,0,0" diagram
+00004a10: 4f72 6965 6e74 6174 696f 6e3d 2255 7022  Orientation="Up"
+00004a20: 2073 7061 6369 6e67 556e 6974 3d22 4d4d   spacingUnit="MM
+00004a30: 2220 7369 7a65 5363 616c 653d 2233 783a  " sizeScale="3x:
+00004a40: 302c 302c 302c 302c 302c 3022 2073 6361  0,0,0,0,0,0" sca
+00004a50: 6c65 4465 7065 6e64 656e 6379 3d22 4172  leDependency="Ar
+00004a60: 6561 2220 6d69 6e69 6d75 6d53 697a 653d  ea" minimumSize=
+00004a70: 2230 2220 656e 6162 6c65 643d 2230 2220  "0" enabled="0" 
+00004a80: 7369 7a65 5479 7065 3d22 4d4d 2220 6d69  sizeType="MM" mi
+00004a90: 6e53 6361 6c65 4465 6e6f 6d69 6e61 746f  nScaleDenominato
+00004aa0: 723d 2230 2220 726f 7461 7469 6f6e 4f66  r="0" rotationOf
+00004ab0: 6673 6574 3d22 3237 3022 2070 656e 436f  fset="270" penCo
+00004ac0: 6c6f 723d 2223 3030 3030 3030 2220 6261  lor="#000000" ba
+00004ad0: 636b 6772 6f75 6e64 416c 7068 613d 2232  ckgroundAlpha="2
+00004ae0: 3535 2220 6261 7257 6964 7468 3d22 3522  55" barWidth="5"
+00004af0: 2062 6163 6b67 726f 756e 6443 6f6c 6f72   backgroundColor
+00004b00: 3d22 2366 6666 6666 6622 206c 696e 6553  ="#ffffff" lineS
+00004b10: 697a 6554 7970 653d 224d 4d22 2073 6361  izeType="MM" sca
+00004b20: 6c65 4261 7365 6456 6973 6962 696c 6974  leBasedVisibilit
+00004b30: 793d 2230 2220 7368 6f77 4178 6973 3d22  y="0" showAxis="
+00004b40: 3122 2073 7061 6369 6e67 3d22 3522 2070  1" spacing="5" p
+00004b50: 656e 5769 6474 683d 2230 2220 7769 6474  enWidth="0" widt
+00004b60: 683d 2231 3522 3e0a 2020 2020 2020 3c66  h="15">.      <f
+00004b70: 6f6e 7450 726f 7065 7274 6965 7320 7374  ontProperties st
+00004b80: 7269 6b65 7468 726f 7567 683d 2230 2220  rikethrough="0" 
+00004b90: 6465 7363 7269 7074 696f 6e3d 224e 6f74  description="Not
+00004ba0: 6f20 5361 6e73 2c31 302c 2d31 2c30 2c35  o Sans,10,-1,0,5
+00004bb0: 302c 302c 302c 302c 302c 3022 2069 7461  0,0,0,0,0,0" ita
+00004bc0: 6c69 633d 2230 2220 756e 6465 726c 696e  lic="0" underlin
+00004bd0: 653d 2230 2220 7374 796c 653d 2222 2062  e="0" style="" b
+00004be0: 6f6c 643d 2230 222f 3e0a 2020 2020 2020  old="0"/>.      
+00004bf0: 3c61 7474 7269 6275 7465 2063 6f6c 6f72  <attribute color
+00004c00: 3d22 2330 3030 3030 3022 2066 6965 6c64  ="#000000" field
+00004c10: 3d22 2220 636f 6c6f 724f 7061 6369 7479  ="" colorOpacity
+00004c20: 3d22 3122 206c 6162 656c 3d22 222f 3e0a  ="1" label=""/>.
+00004c30: 2020 2020 2020 3c61 7869 7353 796d 626f        <axisSymbo
+00004c40: 6c3e 0a20 2020 2020 2020 203c 7379 6d62  l>.        <symb
+00004c50: 6f6c 206e 616d 653d 2222 2066 6f72 6365  ol name="" force
+00004c60: 5f72 6872 3d22 3022 2066 7261 6d65 5f72  _rhr="0" frame_r
+00004c70: 6174 653d 2231 3022 2061 6c70 6861 3d22  ate="10" alpha="
+00004c80: 3122 2063 6c69 705f 746f 5f65 7874 656e  1" clip_to_exten
+00004c90: 743d 2231 2220 6973 5f61 6e69 6d61 7465  t="1" is_animate
+00004ca0: 643d 2230 2220 7479 7065 3d22 6c69 6e65  d="0" type="line
+00004cb0: 223e 0a20 2020 2020 2020 2020 203c 6461  ">.          <da
+00004cc0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+00004cd0: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+00004ce0: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
+00004cf0: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
+00004d00: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00004d10: 653d 226e 616d 6522 2076 616c 7565 3d22  e="name" value="
+00004d20: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00004d30: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00004d40: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
+00004d50: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
+00004d60: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00004d70: 6f6e 206e 616d 653d 2274 7970 6522 2076  on name="type" v
+00004d80: 616c 7565 3d22 636f 6c6c 6563 7469 6f6e  alue="collection
+00004d90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00004da0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00004db0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00004dc0: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
+00004dd0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
+00004de0: 2020 2020 2020 2020 3c6c 6179 6572 2070          <layer p
+00004df0: 6173 733d 2230 2220 6c6f 636b 6564 3d22  ass="0" locked="
+00004e00: 3022 2065 6e61 626c 6564 3d22 3122 2063  0" enabled="1" c
+00004e10: 6c61 7373 3d22 5369 6d70 6c65 4c69 6e65  lass="SimpleLine
+00004e20: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00004e30: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
+00004e40: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00004e50: 203c 4f70 7469 6f6e 206e 616d 653d 2261   <Option name="a
+00004e60: 6c69 676e 5f64 6173 685f 7061 7474 6572  lign_dash_patter
+00004e70: 6e22 2076 616c 7565 3d22 3022 2074 7970  n" value="0" typ
+00004e80: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00004e90: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00004ea0: 696f 6e20 6e61 6d65 3d22 6361 7073 7479  ion name="capsty
+00004eb0: 6c65 2220 7661 6c75 653d 2273 7175 6172  le" value="squar
+00004ec0: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00004ed0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00004ee0: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00004ef0: 6375 7374 6f6d 6461 7368 2220 7661 6c75  customdash" valu
+00004f00: 653d 2235 3b32 2220 7479 7065 3d22 5153  e="5;2" type="QS
+00004f10: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00004f20: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00004f30: 616d 653d 2263 7573 746f 6d64 6173 685f  ame="customdash_
+00004f40: 6d61 705f 756e 6974 5f73 6361 6c65 2220  map_unit_scale" 
+00004f50: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+00004f60: 302c 302c 3022 2074 7970 653d 2251 5374  0,0,0" type="QSt
+00004f70: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004f80: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00004f90: 6d65 3d22 6375 7374 6f6d 6461 7368 5f75  me="customdash_u
+00004fa0: 6e69 7422 2076 616c 7565 3d22 4d4d 2220  nit" value="MM" 
+00004fb0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004fc0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00004fd0: 4f70 7469 6f6e 206e 616d 653d 2264 6173  Option name="das
+00004fe0: 685f 7061 7474 6572 6e5f 6f66 6673 6574  h_pattern_offset
+00004ff0: 2220 7661 6c75 653d 2230 2220 7479 7065  " value="0" type
+00005000: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00005010: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005020: 6f6e 206e 616d 653d 2264 6173 685f 7061  on name="dash_pa
+00005030: 7474 6572 6e5f 6f66 6673 6574 5f6d 6170  ttern_offset_map
+00005040: 5f75 6e69 745f 7363 616c 6522 2076 616c  _unit_scale" val
+00005050: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+00005060: 2c30 2220 7479 7065 3d22 5153 7472 696e  ,0" type="QStrin
+00005070: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00005080: 2020 203c 4f70 7469 6f6e 206e 616d 653d     <Option name=
+00005090: 2264 6173 685f 7061 7474 6572 6e5f 6f66  "dash_pattern_of
+000050a0: 6673 6574 5f75 6e69 7422 2076 616c 7565  fset_unit" value
+000050b0: 3d22 4d4d 2220 7479 7065 3d22 5153 7472  ="MM" type="QStr
+000050c0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000050d0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000050e0: 653d 2264 7261 775f 696e 7369 6465 5f70  e="draw_inside_p
+000050f0: 6f6c 7967 6f6e 2220 7661 6c75 653d 2230  olygon" value="0
+00005100: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00005110: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00005120: 203c 4f70 7469 6f6e 206e 616d 653d 226a   <Option name="j
+00005130: 6f69 6e73 7479 6c65 2220 7661 6c75 653d  oinstyle" value=
+00005140: 2262 6576 656c 2220 7479 7065 3d22 5153  "bevel" type="QS
+00005150: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00005160: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00005170: 616d 653d 226c 696e 655f 636f 6c6f 7222  ame="line_color"
+00005180: 2076 616c 7565 3d22 3335 2c33 352c 3335   value="35,35,35
+00005190: 2c32 3535 2220 7479 7065 3d22 5153 7472  ,255" type="QStr
+000051a0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+000051b0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+000051c0: 653d 226c 696e 655f 7374 796c 6522 2076  e="line_style" v
+000051d0: 616c 7565 3d22 736f 6c69 6422 2074 7970  alue="solid" typ
+000051e0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000051f0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005200: 696f 6e20 6e61 6d65 3d22 6c69 6e65 5f77  ion name="line_w
+00005210: 6964 7468 2220 7661 6c75 653d 2230 2e32  idth" value="0.2
+00005220: 3622 2074 7970 653d 2251 5374 7269 6e67  6" type="QString
+00005230: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005240: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00005250: 6c69 6e65 5f77 6964 7468 5f75 6e69 7422  line_width_unit"
+00005260: 2076 616c 7565 3d22 4d4d 2220 7479 7065   value="MM" type
+00005270: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00005280: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00005290: 6f6e 206e 616d 653d 226f 6666 7365 7422  on name="offset"
+000052a0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
+000052b0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000052c0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000052d0: 6e20 6e61 6d65 3d22 6f66 6673 6574 5f6d  n name="offset_m
+000052e0: 6170 5f75 6e69 745f 7363 616c 6522 2076  ap_unit_scale" v
+000052f0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+00005300: 2c30 2c30 2220 7479 7065 3d22 5153 7472  ,0,0" type="QStr
+00005310: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00005320: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00005330: 653d 226f 6666 7365 745f 756e 6974 2220  e="offset_unit" 
+00005340: 7661 6c75 653d 224d 4d22 2074 7970 653d  value="MM" type=
+00005350: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00005360: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00005370: 6e20 6e61 6d65 3d22 7269 6e67 5f66 696c  n name="ring_fil
+00005380: 7465 7222 2076 616c 7565 3d22 3022 2074  ter" value="0" t
+00005390: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+000053a0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+000053b0: 7074 696f 6e20 6e61 6d65 3d22 7472 696d  ption name="trim
+000053c0: 5f64 6973 7461 6e63 655f 656e 6422 2076  _distance_end" v
+000053d0: 616c 7565 3d22 3022 2074 7970 653d 2251  alue="0" type="Q
+000053e0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000053f0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005400: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
+00005410: 6e63 655f 656e 645f 6d61 705f 756e 6974  nce_end_map_unit
+00005420: 5f73 6361 6c65 2220 7661 6c75 653d 2233  _scale" value="3
+00005430: 783a 302c 302c 302c 302c 302c 3022 2074  x:0,0,0,0,0,0" t
+00005440: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00005450: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+00005460: 7074 696f 6e20 6e61 6d65 3d22 7472 696d  ption name="trim
+00005470: 5f64 6973 7461 6e63 655f 656e 645f 756e  _distance_end_un
+00005480: 6974 2220 7661 6c75 653d 224d 4d22 2074  it" value="MM" t
+00005490: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+000054a0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+000054b0: 7074 696f 6e20 6e61 6d65 3d22 7472 696d  ption name="trim
+000054c0: 5f64 6973 7461 6e63 655f 7374 6172 7422  _distance_start"
+000054d0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
+000054e0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+000054f0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00005500: 6e20 6e61 6d65 3d22 7472 696d 5f64 6973  n name="trim_dis
+00005510: 7461 6e63 655f 7374 6172 745f 6d61 705f  tance_start_map_
+00005520: 756e 6974 5f73 6361 6c65 2220 7661 6c75  unit_scale" valu
+00005530: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+00005540: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
+00005550: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005560: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00005570: 7472 696d 5f64 6973 7461 6e63 655f 7374  trim_distance_st
+00005580: 6172 745f 756e 6974 2220 7661 6c75 653d  art_unit" value=
+00005590: 224d 4d22 2074 7970 653d 2251 5374 7269  "MM" type="QStri
+000055a0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000055b0: 2020 2020 3c4f 7074 696f 6e20 6e61 6d65      <Option name
+000055c0: 3d22 7477 6561 6b5f 6461 7368 5f70 6174  ="tweak_dash_pat
+000055d0: 7465 726e 5f6f 6e5f 636f 726e 6572 7322  tern_on_corners"
+000055e0: 2076 616c 7565 3d22 3022 2074 7970 653d   value="0" type=
+000055f0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00005600: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00005610: 6e20 6e61 6d65 3d22 7573 655f 6375 7374  n name="use_cust
+00005620: 6f6d 5f64 6173 6822 2076 616c 7565 3d22  om_dash" value="
+00005630: 3022 2074 7970 653d 2251 5374 7269 6e67  0" type="QString
+00005640: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005650: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00005660: 7769 6474 685f 6d61 705f 756e 6974 5f73  width_map_unit_s
+00005670: 6361 6c65 2220 7661 6c75 653d 2233 783a  cale" value="3x:
+00005680: 302c 302c 302c 302c 302c 3022 2074 7970  0,0,0,0,0,0" typ
+00005690: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000056a0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+000056b0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+000056c0: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
+000056d0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+000056e0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000056f0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
+00005700: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005710: 696f 6e20 6e61 6d65 3d22 6e61 6d65 2220  ion name="name" 
+00005720: 7661 6c75 653d 2222 2074 7970 653d 2251  value="" type="Q
+00005730: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005740: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00005750: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
+00005760: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
+00005770: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00005780: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
+00005790: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
+000057a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000057b0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
+000057c0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
+000057d0: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
+000057e0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
+000057f0: 2020 2020 2020 203c 2f6c 6179 6572 3e0a         </layer>.
+00005800: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
+00005810: 3e0a 2020 2020 2020 3c2f 6178 6973 5379  >.      </axisSy
+00005820: 6d62 6f6c 3e0a 2020 2020 3c2f 4469 6167  mbol>.    </Diag
+00005830: 7261 6d43 6174 6567 6f72 793e 0a20 203c  ramCategory>.  <
+00005840: 2f53 696e 676c 6543 6174 6567 6f72 7944  /SingleCategoryD
+00005850: 6961 6772 616d 5265 6e64 6572 6572 3e0a  iagramRenderer>.
+00005860: 2020 3c44 6961 6772 616d 4c61 7965 7253    <DiagramLayerS
+00005870: 6574 7469 6e67 7320 6469 7374 3d22 3022  ettings dist="0"
+00005880: 2073 686f 7741 6c6c 3d22 3122 206f 6273   showAll="1" obs
+00005890: 7461 636c 653d 2230 2220 706c 6163 656d  tacle="0" placem
+000058a0: 656e 743d 2230 2220 7a49 6e64 6578 3d22  ent="0" zIndex="
+000058b0: 3022 2070 7269 6f72 6974 793d 2230 2220  0" priority="0" 
+000058c0: 6c69 6e65 506c 6163 656d 656e 7446 6c61  linePlacementFla
+000058d0: 6773 3d22 3138 223e 0a20 2020 203c 7072  gs="18">.    <pr
+000058e0: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
+000058f0: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00005900: 7022 3e0a 2020 2020 2020 2020 3c4f 7074  p">.        <Opt
+00005910: 696f 6e20 6e61 6d65 3d22 6e61 6d65 2220  ion name="name" 
+00005920: 7661 6c75 653d 2222 2074 7970 653d 2251  value="" type="Q
+00005930: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005940: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
+00005950: 7072 6f70 6572 7469 6573 222f 3e0a 2020  properties"/>.  
+00005960: 2020 2020 2020 3c4f 7074 696f 6e20 6e61        <Option na
+00005970: 6d65 3d22 7479 7065 2220 7661 6c75 653d  me="type" value=
+00005980: 2263 6f6c 6c65 6374 696f 6e22 2074 7970  "collection" typ
+00005990: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000059a0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+000059b0: 2020 3c2f 7072 6f70 6572 7469 6573 3e0a    </properties>.
+000059c0: 2020 3c2f 4469 6167 7261 6d4c 6179 6572    </DiagramLayer
+000059d0: 5365 7474 696e 6773 3e0a 2020 3c67 656f  Settings>.  <geo
+000059e0: 6d65 7472 794f 7074 696f 6e73 2072 656d  metryOptions rem
+000059f0: 6f76 6544 7570 6c69 6361 7465 4e6f 6465  oveDuplicateNode
+00005a00: 733d 2230 2220 6765 6f6d 6574 7279 5072  s="0" geometryPr
+00005a10: 6563 6973 696f 6e3d 2230 223e 0a20 2020  ecision="0">.   
+00005a20: 203c 6163 7469 7665 4368 6563 6b73 2f3e   <activeChecks/>
+00005a30: 0a20 2020 203c 6368 6563 6b43 6f6e 6669  .    <checkConfi
+00005a40: 6775 7261 7469 6f6e 2f3e 0a20 203c 2f67  guration/>.  </g
+00005a50: 656f 6d65 7472 794f 7074 696f 6e73 3e0a  eometryOptions>.
+00005a60: 2020 3c6c 6567 656e 6420 7368 6f77 4c61    <legend showLa
+00005a70: 6265 6c4c 6567 656e 643d 2230 2220 7479  belLegend="0" ty
+00005a80: 7065 3d22 6465 6661 756c 742d 7665 6374  pe="default-vect
+00005a90: 6f72 222f 3e0a 2020 3c72 6566 6572 656e  or"/>.  <referen
+00005aa0: 6365 644c 6179 6572 732f 3e0a 2020 3c66  cedLayers/>.  <f
+00005ab0: 6965 6c64 436f 6e66 6967 7572 6174 696f  ieldConfiguratio
+00005ac0: 6e3e 0a20 2020 203c 6669 656c 6420 6e61  n>.    <field na
+00005ad0: 6d65 3d22 7479 7065 2220 636f 6e66 6967  me="type" config
+00005ae0: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
+00005af0: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
+00005b00: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
+00005b10: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
+00005b20: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
+00005b30: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
+00005b40: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
+00005b50: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
+00005b60: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
+00005b70: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00005b80: 226f 736d 5f69 6422 2063 6f6e 6669 6775  "osm_id" configu
+00005b90: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
+00005ba0: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
+00005bb0: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
+00005bc0: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
+00005bd0: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
+00005be0: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
+00005bf0: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
+00005c00: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
+00005c10: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
+00005c20: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00005c30: 6f72 6965 6e74 6174 696f 6e22 2063 6f6e  orientation" con
+00005c40: 6669 6775 7261 7469 6f6e 466c 6167 733d  figurationFlags=
+00005c50: 224e 6f6e 6522 3e0a 2020 2020 2020 3c65  "None">.      <e
+00005c60: 6469 7457 6964 6765 7420 7479 7065 3d22  ditWidget type="
+00005c70: 5465 7874 4564 6974 223e 0a20 2020 2020  TextEdit">.     
+00005c80: 2020 203c 636f 6e66 6967 3e0a 2020 2020     <config>.    
+00005c90: 2020 2020 2020 3c4f 7074 696f 6e2f 3e0a        <Option/>.
+00005ca0: 2020 2020 2020 2020 3c2f 636f 6e66 6967          </config
+00005cb0: 3e0a 2020 2020 2020 3c2f 6564 6974 5769  >.      </editWi
+00005cc0: 6467 6574 3e0a 2020 2020 3c2f 6669 656c  dget>.    </fiel
+00005cd0: 643e 0a20 2020 203c 6669 656c 6420 6e61  d>.    <field na
+00005ce0: 6d65 3d22 6f72 6965 6e74 6174 696f 6e5f  me="orientation_
+00005cf0: 636f 6e66 6964 656e 6365 2220 636f 6e66  confidence" conf
+00005d00: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
+00005d10: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
+00005d20: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
+00005d30: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
+00005d40: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
+00005d50: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
+00005d60: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
+00005d70: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
+00005d80: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
+00005d90: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00005da0: 653d 226c 616e 655f 7769 6474 6822 2063  e="lane_width" c
+00005db0: 6f6e 6669 6775 7261 7469 6f6e 466c 6167  onfigurationFlag
+00005dc0: 733d 224e 6f6e 6522 3e0a 2020 2020 2020  s="None">.      
+00005dd0: 3c65 6469 7457 6964 6765 7420 7479 7065  <editWidget type
+00005de0: 3d22 5465 7874 4564 6974 223e 0a20 2020  ="TextEdit">.   
+00005df0: 2020 2020 203c 636f 6e66 6967 3e0a 2020       <config>.  
+00005e00: 2020 2020 2020 2020 3c4f 7074 696f 6e2f          <Option/
+00005e10: 3e0a 2020 2020 2020 2020 3c2f 636f 6e66  >.        </conf
+00005e20: 6967 3e0a 2020 2020 2020 3c2f 6564 6974  ig>.      </edit
+00005e30: 5769 6467 6574 3e0a 2020 2020 3c2f 6669  Widget>.    </fi
+00005e40: 656c 643e 0a20 2020 203c 6669 656c 6420  eld>.    <field 
+00005e50: 6e61 6d65 3d22 6c61 6e65 5f6f 7269 656e  name="lane_orien
+00005e60: 7461 7469 6f6e 2220 636f 6e66 6967 7572  tation" configur
+00005e70: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
+00005e80: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
+00005e90: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
+00005ea0: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
+00005eb0: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
+00005ec0: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
+00005ed0: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
+00005ee0: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
+00005ef0: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
+00005f00: 3c2f 6669 656c 6443 6f6e 6669 6775 7261  </fieldConfigura
+00005f10: 7469 6f6e 3e0a 2020 3c61 6c69 6173 6573  tion>.  <aliases
+00005f20: 3e0a 2020 2020 3c61 6c69 6173 206e 616d  >.    <alias nam
+00005f30: 653d 2222 2069 6e64 6578 3d22 3022 2066  e="" index="0" f
+00005f40: 6965 6c64 3d22 7479 7065 222f 3e0a 2020  ield="type"/>.  
+00005f50: 2020 3c61 6c69 6173 206e 616d 653d 2222    <alias name=""
+00005f60: 2069 6e64 6578 3d22 3122 2066 6965 6c64   index="1" field
+00005f70: 3d22 6f73 6d5f 6964 222f 3e0a 2020 2020  ="osm_id"/>.    
+00005f80: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
+00005f90: 6e64 6578 3d22 3222 2066 6965 6c64 3d22  ndex="2" field="
+00005fa0: 6f72 6965 6e74 6174 696f 6e22 2f3e 0a20  orientation"/>. 
+00005fb0: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
+00005fc0: 2220 696e 6465 783d 2233 2220 6669 656c  " index="3" fiel
+00005fd0: 643d 226f 7269 656e 7461 7469 6f6e 5f63  d="orientation_c
+00005fe0: 6f6e 6669 6465 6e63 6522 2f3e 0a20 2020  onfidence"/>.   
+00005ff0: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
+00006000: 696e 6465 783d 2234 2220 6669 656c 643d  index="4" field=
+00006010: 226c 616e 655f 7769 6474 6822 2f3e 0a20  "lane_width"/>. 
+00006020: 2020 203c 616c 6961 7320 6e61 6d65 3d22     <alias name="
+00006030: 2220 696e 6465 783d 2235 2220 6669 656c  " index="5" fiel
+00006040: 643d 226c 616e 655f 6f72 6965 6e74 6174  d="lane_orientat
+00006050: 696f 6e22 2f3e 0a20 203c 2f61 6c69 6173  ion"/>.  </alias
+00006060: 6573 3e0a 2020 3c64 6566 6175 6c74 733e  es>.  <defaults>
+00006070: 0a20 2020 203c 6465 6661 756c 7420 6669  .    <default fi
+00006080: 656c 643d 2274 7970 6522 2061 7070 6c79  eld="type" apply
+00006090: 4f6e 5570 6461 7465 3d22 3022 2065 7870  OnUpdate="0" exp
+000060a0: 7265 7373 696f 6e3d 2222 2f3e 0a20 2020  ression=""/>.   
+000060b0: 203c 6465 6661 756c 7420 6669 656c 643d   <default field=
+000060c0: 226f 736d 5f69 6422 2061 7070 6c79 4f6e  "osm_id" applyOn
+000060d0: 5570 6461 7465 3d22 3022 2065 7870 7265  Update="0" expre
+000060e0: 7373 696f 6e3d 2222 2f3e 0a20 2020 203c  ssion=""/>.    <
+000060f0: 6465 6661 756c 7420 6669 656c 643d 226f  default field="o
+00006100: 7269 656e 7461 7469 6f6e 2220 6170 706c  rientation" appl
+00006110: 794f 6e55 7064 6174 653d 2230 2220 6578  yOnUpdate="0" ex
+00006120: 7072 6573 7369 6f6e 3d22 222f 3e0a 2020  pression=""/>.  
+00006130: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
+00006140: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+00006150: 6e66 6964 656e 6365 2220 6170 706c 794f  nfidence" applyO
+00006160: 6e55 7064 6174 653d 2230 2220 6578 7072  nUpdate="0" expr
+00006170: 6573 7369 6f6e 3d22 222f 3e0a 2020 2020  ession=""/>.    
+00006180: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
+00006190: 6c61 6e65 5f77 6964 7468 2220 6170 706c  lane_width" appl
+000061a0: 794f 6e55 7064 6174 653d 2230 2220 6578  yOnUpdate="0" ex
+000061b0: 7072 6573 7369 6f6e 3d22 222f 3e0a 2020  pression=""/>.  
+000061c0: 2020 3c64 6566 6175 6c74 2066 6965 6c64    <default field
+000061d0: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+000061e0: 6f6e 2220 6170 706c 794f 6e55 7064 6174  on" applyOnUpdat
+000061f0: 653d 2230 2220 6578 7072 6573 7369 6f6e  e="0" expression
+00006200: 3d22 222f 3e0a 2020 3c2f 6465 6661 756c  =""/>.  </defaul
+00006210: 7473 3e0a 2020 3c63 6f6e 7374 7261 696e  ts>.  <constrain
+00006220: 7473 3e0a 2020 2020 3c63 6f6e 7374 7261  ts>.    <constra
+00006230: 696e 7420 6e6f 746e 756c 6c5f 7374 7265  int notnull_stre
+00006240: 6e67 7468 3d22 3022 2063 6f6e 7374 7261  ngth="0" constra
+00006250: 696e 7473 3d22 3022 2075 6e69 7175 655f  ints="0" unique_
+00006260: 7374 7265 6e67 7468 3d22 3022 2066 6965  strength="0" fie
+00006270: 6c64 3d22 7479 7065 2220 6578 705f 7374  ld="type" exp_st
+00006280: 7265 6e67 7468 3d22 3022 2f3e 0a20 2020  rength="0"/>.   
+00006290: 203c 636f 6e73 7472 6169 6e74 206e 6f74   <constraint not
+000062a0: 6e75 6c6c 5f73 7472 656e 6774 683d 2230  null_strength="0
+000062b0: 2220 636f 6e73 7472 6169 6e74 733d 2230  " constraints="0
+000062c0: 2220 756e 6971 7565 5f73 7472 656e 6774  " unique_strengt
+000062d0: 683d 2230 2220 6669 656c 643d 226f 736d  h="0" field="osm
+000062e0: 5f69 6422 2065 7870 5f73 7472 656e 6774  _id" exp_strengt
+000062f0: 683d 2230 222f 3e0a 2020 2020 3c63 6f6e  h="0"/>.    <con
+00006300: 7374 7261 696e 7420 6e6f 746e 756c 6c5f  straint notnull_
+00006310: 7374 7265 6e67 7468 3d22 3022 2063 6f6e  strength="0" con
+00006320: 7374 7261 696e 7473 3d22 3022 2075 6e69  straints="0" uni
+00006330: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
+00006340: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
+00006350: 696f 6e22 2065 7870 5f73 7472 656e 6774  ion" exp_strengt
+00006360: 683d 2230 222f 3e0a 2020 2020 3c63 6f6e  h="0"/>.    <con
+00006370: 7374 7261 696e 7420 6e6f 746e 756c 6c5f  straint notnull_
+00006380: 7374 7265 6e67 7468 3d22 3022 2063 6f6e  strength="0" con
+00006390: 7374 7261 696e 7473 3d22 3022 2075 6e69  straints="0" uni
+000063a0: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
+000063b0: 2066 6965 6c64 3d22 6f72 6965 6e74 6174   field="orientat
+000063c0: 696f 6e5f 636f 6e66 6964 656e 6365 2220  ion_confidence" 
+000063d0: 6578 705f 7374 7265 6e67 7468 3d22 3022  exp_strength="0"
+000063e0: 2f3e 0a20 2020 203c 636f 6e73 7472 6169  />.    <constrai
+000063f0: 6e74 206e 6f74 6e75 6c6c 5f73 7472 656e  nt notnull_stren
+00006400: 6774 683d 2230 2220 636f 6e73 7472 6169  gth="0" constrai
+00006410: 6e74 733d 2230 2220 756e 6971 7565 5f73  nts="0" unique_s
+00006420: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
+00006430: 643d 226c 616e 655f 7769 6474 6822 2065  d="lane_width" e
+00006440: 7870 5f73 7472 656e 6774 683d 2230 222f  xp_strength="0"/
+00006450: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00006460: 7420 6e6f 746e 756c 6c5f 7374 7265 6e67  t notnull_streng
+00006470: 7468 3d22 3022 2063 6f6e 7374 7261 696e  th="0" constrain
+00006480: 7473 3d22 3022 2075 6e69 7175 655f 7374  ts="0" unique_st
+00006490: 7265 6e67 7468 3d22 3022 2066 6965 6c64  rength="0" field
+000064a0: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+000064b0: 6f6e 2220 6578 705f 7374 7265 6e67 7468  on" exp_strength
+000064c0: 3d22 3022 2f3e 0a20 203c 2f63 6f6e 7374  ="0"/>.  </const
+000064d0: 7261 696e 7473 3e0a 2020 3c63 6f6e 7374  raints>.  <const
+000064e0: 7261 696e 7445 7870 7265 7373 696f 6e73  raintExpressions
+000064f0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00006500: 7420 6578 703d 2222 2064 6573 633d 2222  t exp="" desc=""
+00006510: 2066 6965 6c64 3d22 7479 7065 222f 3e0a   field="type"/>.
+00006520: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+00006530: 6578 703d 2222 2064 6573 633d 2222 2066  exp="" desc="" f
+00006540: 6965 6c64 3d22 6f73 6d5f 6964 222f 3e0a  ield="osm_id"/>.
+00006550: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+00006560: 6578 703d 2222 2064 6573 633d 2222 2066  exp="" desc="" f
+00006570: 6965 6c64 3d22 6f72 6965 6e74 6174 696f  ield="orientatio
+00006580: 6e22 2f3e 0a20 2020 203c 636f 6e73 7472  n"/>.    <constr
+00006590: 6169 6e74 2065 7870 3d22 2220 6465 7363  aint exp="" desc
+000065a0: 3d22 2220 6669 656c 643d 226f 7269 656e  ="" field="orien
+000065b0: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
+000065c0: 6522 2f3e 0a20 2020 203c 636f 6e73 7472  e"/>.    <constr
+000065d0: 6169 6e74 2065 7870 3d22 2220 6465 7363  aint exp="" desc
+000065e0: 3d22 2220 6669 656c 643d 226c 616e 655f  ="" field="lane_
+000065f0: 7769 6474 6822 2f3e 0a20 2020 203c 636f  width"/>.    <co
+00006600: 6e73 7472 6169 6e74 2065 7870 3d22 2220  nstraint exp="" 
+00006610: 6465 7363 3d22 2220 6669 656c 643d 226c  desc="" field="l
+00006620: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
+00006630: 2f3e 0a20 203c 2f63 6f6e 7374 7261 696e  />.  </constrain
+00006640: 7445 7870 7265 7373 696f 6e73 3e0a 2020  tExpressions>.  
+00006650: 3c65 7870 7265 7373 696f 6e66 6965 6c64  <expressionfield
+00006660: 732f 3e0a 2020 3c61 7474 7269 6275 7465  s/>.  <attribute
+00006670: 6163 7469 6f6e 733e 0a20 2020 203c 6465  actions>.    <de
+00006680: 6661 756c 7441 6374 696f 6e20 6b65 793d  faultAction key=
+00006690: 2243 616e 7661 7322 2076 616c 7565 3d22  "Canvas" value="
+000066a0: 7b30 3030 3030 3030 302d 3030 3030 2d30  {00000000-0000-0
+000066b0: 3030 302d 3030 3030 2d30 3030 3030 3030  000-0000-0000000
+000066c0: 3030 3030 307d 222f 3e0a 2020 3c2f 6174  00000}"/>.  </at
+000066d0: 7472 6962 7574 6561 6374 696f 6e73 3e0a  tributeactions>.
+000066e0: 2020 3c61 7474 7269 6275 7465 7461 626c    <attributetabl
+000066f0: 6563 6f6e 6669 6720 736f 7274 4578 7072  econfig sortExpr
+00006700: 6573 7369 6f6e 3d22 2220 736f 7274 4f72  ession="" sortOr
+00006710: 6465 723d 2230 2220 6163 7469 6f6e 5769  der="0" actionWi
+00006720: 6467 6574 5374 796c 653d 2264 726f 7044  dgetStyle="dropD
+00006730: 6f77 6e22 3e0a 2020 2020 3c63 6f6c 756d  own">.    <colum
+00006740: 6e73 3e0a 2020 2020 2020 3c63 6f6c 756d  ns>.      <colum
+00006750: 6e20 6e61 6d65 3d22 7479 7065 2220 7769  n name="type" wi
+00006760: 6474 683d 222d 3122 2068 6964 6465 6e3d  dth="-1" hidden=
+00006770: 2230 2220 7479 7065 3d22 6669 656c 6422  "0" type="field"
+00006780: 2f3e 0a20 2020 2020 203c 636f 6c75 6d6e  />.      <column
+00006790: 206e 616d 653d 226f 736d 5f69 6422 2077   name="osm_id" w
+000067a0: 6964 7468 3d22 3137 3122 2068 6964 6465  idth="171" hidde
+000067b0: 6e3d 2230 2220 7479 7065 3d22 6669 656c  n="0" type="fiel
+000067c0: 6422 2f3e 0a20 2020 2020 203c 636f 6c75  d"/>.      <colu
+000067d0: 6d6e 206e 616d 653d 226f 7269 656e 7461  mn name="orienta
+000067e0: 7469 6f6e 2220 7769 6474 683d 2232 3932  tion" width="292
+000067f0: 2220 6869 6464 656e 3d22 3022 2074 7970  " hidden="0" typ
+00006800: 653d 2266 6965 6c64 222f 3e0a 2020 2020  e="field"/>.    
+00006810: 2020 3c63 6f6c 756d 6e20 6e61 6d65 3d22    <column name="
+00006820: 6f72 6965 6e74 6174 696f 6e5f 636f 6e66  orientation_conf
+00006830: 6964 656e 6365 2220 7769 6474 683d 222d  idence" width="-
+00006840: 3122 2068 6964 6465 6e3d 2230 2220 7479  1" hidden="0" ty
+00006850: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
+00006860: 2020 203c 636f 6c75 6d6e 206e 616d 653d     <column name=
+00006870: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+00006880: 6e22 2077 6964 7468 3d22 2d31 2220 6869  n" width="-1" hi
+00006890: 6464 656e 3d22 3022 2074 7970 653d 2266  dden="0" type="f
+000068a0: 6965 6c64 222f 3e0a 2020 2020 2020 3c63  ield"/>.      <c
+000068b0: 6f6c 756d 6e20 6e61 6d65 3d22 6c61 6e65  olumn name="lane
+000068c0: 5f77 6964 7468 2220 7769 6474 683d 222d  _width" width="-
+000068d0: 3122 2068 6964 6465 6e3d 2230 2220 7479  1" hidden="0" ty
+000068e0: 7065 3d22 6669 656c 6422 2f3e 0a20 2020  pe="field"/>.   
+000068f0: 2020 203c 636f 6c75 6d6e 2077 6964 7468     <column width
+00006900: 3d22 2d31 2220 6869 6464 656e 3d22 3122  ="-1" hidden="1"
+00006910: 2074 7970 653d 2261 6374 696f 6e73 222f   type="actions"/
+00006920: 3e0a 2020 2020 3c2f 636f 6c75 6d6e 733e  >.    </columns>
+00006930: 0a20 203c 2f61 7474 7269 6275 7465 7461  .  </attributeta
+00006940: 626c 6563 6f6e 6669 673e 0a20 203c 636f  bleconfig>.  <co
+00006950: 6e64 6974 696f 6e61 6c73 7479 6c65 733e  nditionalstyles>
+00006960: 0a20 2020 203c 726f 7773 7479 6c65 732f  .    <rowstyles/
+00006970: 3e0a 2020 2020 3c66 6965 6c64 7374 796c  >.    <fieldstyl
+00006980: 6573 2f3e 0a20 203c 2f63 6f6e 6469 7469  es/>.  </conditi
+00006990: 6f6e 616c 7374 796c 6573 3e0a 2020 3c73  onalstyles>.  <s
+000069a0: 746f 7265 6465 7870 7265 7373 696f 6e73  toredexpressions
+000069b0: 2f3e 0a20 203c 6564 6974 666f 726d 2074  />.  <editform t
+000069c0: 6f6c 6572 616e 743d 2231 223e 3c2f 6564  olerant="1"></ed
+000069d0: 6974 666f 726d 3e0a 2020 3c65 6469 7466  itform>.  <editf
+000069e0: 6f72 6d69 6e69 742f 3e0a 2020 3c65 6469  orminit/>.  <edi
+000069f0: 7466 6f72 6d69 6e69 7463 6f64 6573 6f75  tforminitcodesou
+00006a00: 7263 653e 303c 2f65 6469 7466 6f72 6d69  rce>0</editformi
+00006a10: 6e69 7463 6f64 6573 6f75 7263 653e 0a20  nitcodesource>. 
+00006a20: 203c 6564 6974 666f 726d 696e 6974 6669   <editforminitfi
+00006a30: 6c65 7061 7468 3e3c 2f65 6469 7466 6f72  lepath></editfor
+00006a40: 6d69 6e69 7466 696c 6570 6174 683e 0a20  minitfilepath>. 
+00006a50: 203c 6564 6974 666f 726d 696e 6974 636f   <editforminitco
+00006a60: 6465 3e3c 215b 4344 4154 415b 2320 2d2a  de><![CDATA[# -*
+00006a70: 2d20 636f 6469 6e67 3a20 7574 662d 3820  - coding: utf-8 
+00006a80: 2d2a 2d0a 2222 220a 4c65 7320 666f 726d  -*-.""".Les form
+00006a90: 756c 6169 7265 7320 5147 4953 2070 6575  ulaires QGIS peu
+00006aa0: 7665 6e74 2061 766f 6972 2075 6e65 2066  vent avoir une f
+00006ab0: 6f6e 6374 696f 6e20 5079 7468 6f6e 2071  onction Python q
+00006ac0: 7569 2065 7374 2061 7070 656c c3a9 6520  ui est appel..e 
+00006ad0: 6c6f 7273 7175 6520 6c65 2066 6f72 6d75  lorsque le formu
+00006ae0: 6c61 6972 6520 6573 740a 6f75 7665 7274  laire est.ouvert
+00006af0: 2e0a 0a55 7469 6c69 7365 7a20 6365 7474  ...Utilisez cett
+00006b00: 6520 666f 6e63 7469 6f6e 2070 6f75 7220  e fonction pour 
+00006b10: 616a 6f75 7465 7220 756e 6520 6c6f 6769  ajouter une logi
+00006b20: 7175 6520 7375 7070 6cc3 a96d 656e 7461  que suppl..menta
+00006b30: 6972 6520 c3a0 2076 6f73 2066 6f72 6d75  ire .. vos formu
+00006b40: 6c61 6972 6573 2e0a 0a45 6e74 7265 7a20  laires...Entrez 
+00006b50: 6c65 206e 6f6d 2064 6520 6c61 2066 6f6e  le nom de la fon
+00006b60: 6374 696f 6e20 6461 6e73 206c 6520 6368  ction dans le ch
+00006b70: 616d 7020 0a22 466f 6e63 7469 6f6e 2064  amp ."Fonction d
+00006b80: 2769 6e69 7469 616c 6973 6174 696f 6e20  'initialisation 
+00006b90: 5079 7468 6f6e 222e 0a56 6f69 6369 2075  Python"..Voici u
+00006ba0: 6e20 6578 656d 706c 653a 0a22 2222 0a66  n exemple:.""".f
+00006bb0: 726f 6d20 7167 6973 2e50 7951 742e 5174  rom qgis.PyQt.Qt
+00006bc0: 5769 6467 6574 7320 696d 706f 7274 2051  Widgets import Q
+00006bd0: 5769 6467 6574 0a0a 6465 6620 6d79 5f66  Widget..def my_f
+00006be0: 6f72 6d5f 6f70 656e 2864 6961 6c6f 672c  orm_open(dialog,
+00006bf0: 206c 6179 6572 2c20 6665 6174 7572 6529   layer, feature)
+00006c00: 3a0a 2020 2020 6765 6f6d 203d 2066 6561  :.    geom = fea
+00006c10: 7475 7265 2e67 656f 6d65 7472 7928 290a  ture.geometry().
+00006c20: 2020 2020 636f 6e74 726f 6c20 3d20 6469      control = di
+00006c30: 616c 6f67 2e66 696e 6443 6869 6c64 2851  alog.findChild(Q
+00006c40: 5769 6467 6574 2c20 224d 794c 696e 6545  Widget, "MyLineE
+00006c50: 6469 7422 290a 5d5d 3e3c 2f65 6469 7466  dit").]]></editf
+00006c60: 6f72 6d69 6e69 7463 6f64 653e 0a20 203c  orminitcode>.  <
+00006c70: 6665 6174 666f 726d 7375 7070 7265 7373  featformsuppress
+00006c80: 3e30 3c2f 6665 6174 666f 726d 7375 7070  >0</featformsupp
+00006c90: 7265 7373 3e0a 2020 3c65 6469 746f 726c  ress>.  <editorl
+00006ca0: 6179 6f75 743e 6765 6e65 7261 7465 646c  ayout>generatedl
+00006cb0: 6179 6f75 743c 2f65 6469 746f 726c 6179  ayout</editorlay
+00006cc0: 6f75 743e 0a20 203c 6564 6974 6162 6c65  out>.  <editable
+00006cd0: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00006ce0: 653d 2261 6e67 6c65 2220 6564 6974 6162  e="angle" editab
+00006cf0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+00006d00: 656c 6420 6e61 6d65 3d22 6669 6422 2065  eld name="fid" e
+00006d10: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+00006d20: 2020 3c66 6965 6c64 206e 616d 653d 226c    <field name="l
+00006d30: 616e 655f 6f72 6965 6e74 6174 696f 6e22  ane_orientation"
+00006d40: 2065 6469 7461 626c 653d 2231 222f 3e0a   editable="1"/>.
+00006d50: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00006d60: 226c 616e 655f 7769 6474 6822 2065 6469  "lane_width" edi
+00006d70: 7461 626c 653d 2231 222f 3e0a 2020 2020  table="1"/>.    
+00006d80: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
+00006d90: 656e 7461 7469 6f6e 2220 6564 6974 6162  entation" editab
+00006da0: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+00006db0: 656c 6420 6e61 6d65 3d22 6f72 6965 6e74  eld name="orient
+00006dc0: 6174 696f 6e5f 636f 6e66 6964 656e 6365  ation_confidence
+00006dd0: 2220 6564 6974 6162 6c65 3d22 3122 2f3e  " editable="1"/>
+00006de0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00006df0: 3d22 6f73 6d5f 6964 2220 6564 6974 6162  ="osm_id" editab
+00006e00: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+00006e10: 656c 6420 6e61 6d65 3d22 7479 7065 2220  eld name="type" 
+00006e20: 6564 6974 6162 6c65 3d22 3122 2f3e 0a20  editable="1"/>. 
+00006e30: 203c 2f65 6469 7461 626c 653e 0a20 203c   </editable>.  <
+00006e40: 6c61 6265 6c4f 6e54 6f70 3e0a 2020 2020  labelOnTop>.    
+00006e50: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
+00006e60: 6c65 2220 6c61 6265 6c4f 6e54 6f70 3d22  le" labelOnTop="
+00006e70: 3022 2f3e 0a20 2020 203c 6669 656c 6420  0"/>.    <field 
+00006e80: 6e61 6d65 3d22 6669 6422 206c 6162 656c  name="fid" label
+00006e90: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
+00006ea0: 3c66 6965 6c64 206e 616d 653d 226c 616e  <field name="lan
+00006eb0: 655f 6f72 6965 6e74 6174 696f 6e22 206c  e_orientation" l
+00006ec0: 6162 656c 4f6e 546f 703d 2230 222f 3e0a  abelOnTop="0"/>.
+00006ed0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00006ee0: 226c 616e 655f 7769 6474 6822 206c 6162  "lane_width" lab
+00006ef0: 656c 4f6e 546f 703d 2230 222f 3e0a 2020  elOnTop="0"/>.  
+00006f00: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00006f10: 7269 656e 7461 7469 6f6e 2220 6c61 6265  rientation" labe
+00006f20: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
+00006f30: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
+00006f40: 6965 6e74 6174 696f 6e5f 636f 6e66 6964  ientation_confid
+00006f50: 656e 6365 2220 6c61 6265 6c4f 6e54 6f70  ence" labelOnTop
+00006f60: 3d22 3022 2f3e 0a20 2020 203c 6669 656c  ="0"/>.    <fiel
+00006f70: 6420 6e61 6d65 3d22 6f73 6d5f 6964 2220  d name="osm_id" 
+00006f80: 6c61 6265 6c4f 6e54 6f70 3d22 3022 2f3e  labelOnTop="0"/>
+00006f90: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00006fa0: 3d22 7479 7065 2220 6c61 6265 6c4f 6e54  ="type" labelOnT
+00006fb0: 6f70 3d22 3022 2f3e 0a20 203c 2f6c 6162  op="0"/>.  </lab
+00006fc0: 656c 4f6e 546f 703e 0a20 203c 7265 7573  elOnTop>.  <reus
+00006fd0: 654c 6173 7456 616c 7565 3e0a 2020 2020  eLastValue>.    
+00006fe0: 3c66 6965 6c64 206e 616d 653d 2261 6e67  <field name="ang
+00006ff0: 6c65 2220 7265 7573 654c 6173 7456 616c  le" reuseLastVal
+00007000: 7565 3d22 3022 2f3e 0a20 2020 203c 6669  ue="0"/>.    <fi
+00007010: 656c 6420 6e61 6d65 3d22 6669 6422 2072  eld name="fid" r
+00007020: 6575 7365 4c61 7374 5661 6c75 653d 2230  euseLastValue="0
+00007030: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
+00007040: 616d 653d 226c 616e 655f 6f72 6965 6e74  ame="lane_orient
+00007050: 6174 696f 6e22 2072 6575 7365 4c61 7374  ation" reuseLast
+00007060: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
+00007070: 3c66 6965 6c64 206e 616d 653d 226c 616e  <field name="lan
+00007080: 655f 7769 6474 6822 2072 6575 7365 4c61  e_width" reuseLa
+00007090: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+000070a0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+000070b0: 7269 656e 7461 7469 6f6e 2220 7265 7573  rientation" reus
+000070c0: 654c 6173 7456 616c 7565 3d22 3022 2f3e  eLastValue="0"/>
+000070d0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+000070e0: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+000070f0: 6e66 6964 656e 6365 2220 7265 7573 654c  nfidence" reuseL
+00007100: 6173 7456 616c 7565 3d22 3022 2f3e 0a20  astValue="0"/>. 
+00007110: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00007120: 6f73 6d5f 6964 2220 7265 7573 654c 6173  osm_id" reuseLas
+00007130: 7456 616c 7565 3d22 3022 2f3e 0a20 2020  tValue="0"/>.   
+00007140: 203c 6669 656c 6420 6e61 6d65 3d22 7479   <field name="ty
+00007150: 7065 2220 7265 7573 654c 6173 7456 616c  pe" reuseLastVal
+00007160: 7565 3d22 3022 2f3e 0a20 203c 2f72 6575  ue="0"/>.  </reu
+00007170: 7365 4c61 7374 5661 6c75 653e 0a20 203c  seLastValue>.  <
+00007180: 6461 7461 4465 6669 6e65 6446 6965 6c64  dataDefinedField
+00007190: 5072 6f70 6572 7469 6573 2f3e 0a20 203c  Properties/>.  <
+000071a0: 7769 6467 6574 732f 3e0a 2020 3c70 7265  widgets/>.  <pre
+000071b0: 7669 6577 4578 7072 6573 7369 6f6e 3e22  viewExpression>"
+000071c0: 7479 7065 223c 2f70 7265 7669 6577 4578  type"</previewEx
+000071d0: 7072 6573 7369 6f6e 3e0a 2020 3c6d 6170  pression>.  <map
+000071e0: 5469 703e 3c2f 6d61 7054 6970 3e0a 2020  Tip></mapTip>.  
+000071f0: 3c6c 6179 6572 4765 6f6d 6574 7279 5479  <layerGeometryTy
+00007200: 7065 3e30 3c2f 6c61 7965 7247 656f 6d65  pe>0</layerGeome
+00007210: 7472 7954 7970 653e 0a3c 2f71 6769 733e  tryType>.</qgis>
+00007220: 0a                                       .
```

### Comparing `crossroads-schematization-0.0.7/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.0.8/crschem/resources/rendering-polylines-space.qml`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 00000000: 3c21 444f 4354 5950 4520 7167 6973 2050  <!DOCTYPE qgis P
 00000010: 5542 4c49 4320 2768 7474 703a 2f2f 6d72  UBLIC 'http://mr
 00000020: 6363 2e63 6f6d 2f71 6769 732e 6474 6427  cc.com/qgis.dtd'
 00000030: 2027 5359 5354 454d 273e 0a3c 7167 6973   'SYSTEM'>.<qgis
 00000040: 206c 6162 656c 7345 6e61 626c 6564 3d22   labelsEnabled="
-00000050: 3022 2073 696d 706c 6966 7944 7261 7769  0" simplifyDrawi
-00000060: 6e67 4869 6e74 733d 2231 2220 7369 6d70  ngHints="1" simp
-00000070: 6c69 6679 4d61 7853 6361 6c65 3d22 3122  lifyMaxScale="1"
-00000080: 2073 696d 706c 6966 794c 6f63 616c 3d22   simplifyLocal="
-00000090: 3122 2076 6572 7369 6f6e 3d22 332e 3238  1" version="3.28
-000000a0: 2e31 2d46 6972 656e 7a65 2220 6861 7353  .1-Firenze" hasS
-000000b0: 6361 6c65 4261 7365 6456 6973 6962 696c  caleBasedVisibil
-000000c0: 6974 7946 6c61 673d 2230 2220 7379 6d62  ityFlag="0" symb
-000000d0: 6f6c 6f67 7952 6566 6572 656e 6365 5363  ologyReferenceSc
-000000e0: 616c 653d 222d 3122 2072 6561 644f 6e6c  ale="-1" readOnl
-000000f0: 793d 2230 2220 7369 6d70 6c69 6679 416c  y="0" simplifyAl
-00000100: 676f 7269 7468 6d3d 2230 2220 7369 6d70  gorithm="0" simp
-00000110: 6c69 6679 4472 6177 696e 6754 6f6c 3d22  lifyDrawingTol="
-00000120: 3122 2073 7479 6c65 4361 7465 676f 7269  1" styleCategori
-00000130: 6573 3d22 416c 6c53 7479 6c65 4361 7465  es="AllStyleCate
-00000140: 676f 7269 6573 2220 6d61 7853 6361 6c65  gories" maxScale
-00000150: 3d22 3022 206d 696e 5363 616c 653d 2231  ="0" minScale="1
-00000160: 3030 3030 3030 3030 223e 0a20 203c 666c  00000000">.  <fl
+00000050: 3022 2073 796d 626f 6c6f 6779 5265 6665  0" symbologyRefe
+00000060: 7265 6e63 6553 6361 6c65 3d22 2d31 2220  renceScale="-1" 
+00000070: 6d69 6e53 6361 6c65 3d22 3130 3030 3030  minScale="100000
+00000080: 3030 3022 2073 696d 706c 6966 7944 7261  000" simplifyDra
+00000090: 7769 6e67 546f 6c3d 2231 2220 7369 6d70  wingTol="1" simp
+000000a0: 6c69 6679 416c 676f 7269 7468 6d3d 2230  lifyAlgorithm="0
+000000b0: 2220 7369 6d70 6c69 6679 4472 6177 696e  " simplifyDrawin
+000000c0: 6748 696e 7473 3d22 3122 2073 7479 6c65  gHints="1" style
+000000d0: 4361 7465 676f 7269 6573 3d22 416c 6c53  Categories="AllS
+000000e0: 7479 6c65 4361 7465 676f 7269 6573 2220  tyleCategories" 
+000000f0: 6d61 7853 6361 6c65 3d22 3022 2073 696d  maxScale="0" sim
+00000100: 706c 6966 794c 6f63 616c 3d22 3122 2076  plifyLocal="1" v
+00000110: 6572 7369 6f6e 3d22 332e 3238 2e33 2d46  ersion="3.28.3-F
+00000120: 6972 656e 7a65 2220 7265 6164 4f6e 6c79  irenze" readOnly
+00000130: 3d22 3022 2073 696d 706c 6966 794d 6178  ="0" simplifyMax
+00000140: 5363 616c 653d 2231 2220 6861 7353 6361  Scale="1" hasSca
+00000150: 6c65 4261 7365 6456 6973 6962 696c 6974  leBasedVisibilit
+00000160: 7946 6c61 673d 2230 223e 0a20 203c 666c  yFlag="0">.  <fl
 00000170: 6167 733e 0a20 2020 203c 4964 656e 7469  ags>.    <Identi
 00000180: 6669 6162 6c65 3e31 3c2f 4964 656e 7469  fiable>1</Identi
 00000190: 6669 6162 6c65 3e0a 2020 2020 3c52 656d  fiable>.    <Rem
 000001a0: 6f76 6162 6c65 3e31 3c2f 5265 6d6f 7661  ovable>1</Remova
 000001b0: 626c 653e 0a20 2020 203c 5365 6172 6368  ble>.    <Search
 000001c0: 6162 6c65 3e31 3c2f 5365 6172 6368 6162  able>1</Searchab
 000001d0: 6c65 3e0a 2020 2020 3c50 7269 7661 7465  le>.    <Private
 000001e0: 3e30 3c2f 5072 6976 6174 653e 0a20 203c  >0</Private>.  <
 000001f0: 2f66 6c61 6773 3e0a 2020 3c74 656d 706f  /flags>.  <tempo
-00000200: 7261 6c20 6163 6375 6d75 6c61 7465 3d22  ral accumulate="
-00000210: 3022 206d 6f64 653d 2230 2220 656e 6446  0" mode="0" endF
-00000220: 6965 6c64 3d22 2220 6475 7261 7469 6f6e  ield="" duration
-00000230: 4669 656c 643d 2222 2064 7572 6174 696f  Field="" duratio
-00000240: 6e55 6e69 743d 226d 696e 2220 6669 7865  nUnit="min" fixe
-00000250: 6444 7572 6174 696f 6e3d 2230 2220 7374  dDuration="0" st
-00000260: 6172 7445 7870 7265 7373 696f 6e3d 2222  artExpression=""
-00000270: 206c 696d 6974 4d6f 6465 3d22 3022 2073   limitMode="0" s
-00000280: 7461 7274 4669 656c 643d 2222 2065 6e64  tartField="" end
-00000290: 4578 7072 6573 7369 6f6e 3d22 2220 656e  Expression="" en
-000002a0: 6162 6c65 643d 2230 223e 0a20 2020 203c  abled="0">.    <
+00000200: 7261 6c20 6c69 6d69 744d 6f64 653d 2230  ral limitMode="0
+00000210: 2220 7374 6172 7446 6965 6c64 3d22 2220  " startField="" 
+00000220: 6669 7865 6444 7572 6174 696f 6e3d 2230  fixedDuration="0
+00000230: 2220 6163 6375 6d75 6c61 7465 3d22 3022  " accumulate="0"
+00000240: 2065 6e64 4669 656c 643d 2222 2073 7461   endField="" sta
+00000250: 7274 4578 7072 6573 7369 6f6e 3d22 2220  rtExpression="" 
+00000260: 6475 7261 7469 6f6e 556e 6974 3d22 6d69  durationUnit="mi
+00000270: 6e22 206d 6f64 653d 2230 2220 656e 6445  n" mode="0" endE
+00000280: 7870 7265 7373 696f 6e3d 2222 2065 6e61  xpression="" ena
+00000290: 626c 6564 3d22 3022 2064 7572 6174 696f  bled="0" duratio
+000002a0: 6e46 6965 6c64 3d22 223e 0a20 2020 203c  nField="">.    <
 000002b0: 6669 7865 6452 616e 6765 3e0a 2020 2020  fixedRange>.    
 000002c0: 2020 3c73 7461 7274 3e3c 2f73 7461 7274    <start></start
 000002d0: 3e0a 2020 2020 2020 3c65 6e64 3e3c 2f65  >.      <end></e
 000002e0: 6e64 3e0a 2020 2020 3c2f 6669 7865 6452  nd>.    </fixedR
 000002f0: 616e 6765 3e0a 2020 3c2f 7465 6d70 6f72  ange>.  </tempor
 00000300: 616c 3e0a 2020 3c65 6c65 7661 7469 6f6e  al>.  <elevation
 00000310: 2073 796d 626f 6c6f 6779 3d22 4c69 6e65   symbology="Line
-00000320: 2220 7a73 6361 6c65 3d22 3122 2073 686f  " zscale="1" sho
-00000330: 774d 6172 6b65 7253 796d 626f 6c49 6e53  wMarkerSymbolInS
-00000340: 7572 6661 6365 506c 6f74 733d 2230 2220  urfacePlots="0" 
-00000350: 6578 7472 7573 696f 6e3d 2230 2220 6269  extrusion="0" bi
-00000360: 6e64 696e 673d 2243 656e 7472 6f69 6422  nding="Centroid"
-00000370: 2065 7874 7275 7369 6f6e 456e 6162 6c65   extrusionEnable
-00000380: 643d 2230 2220 7479 7065 3d22 496e 6469  d="0" type="Indi
-00000390: 7669 6475 616c 4665 6174 7572 6573 2220  vidualFeatures" 
-000003a0: 7a6f 6666 7365 743d 2230 2220 636c 616d  zoffset="0" clam
-000003b0: 7069 6e67 3d22 5465 7272 6169 6e22 2072  ping="Terrain" r
-000003c0: 6573 7065 6374 4c61 7965 7253 796d 626f  espectLayerSymbo
-000003d0: 6c3d 2231 223e 0a20 2020 203c 6461 7461  l="1">.    <data
+00000320: 2220 7265 7370 6563 744c 6179 6572 5379  " respectLayerSy
+00000330: 6d62 6f6c 3d22 3122 207a 7363 616c 653d  mbol="1" zscale=
+00000340: 2231 2220 636c 616d 7069 6e67 3d22 5465  "1" clamping="Te
+00000350: 7272 6169 6e22 2073 686f 774d 6172 6b65  rrain" showMarke
+00000360: 7253 796d 626f 6c49 6e53 7572 6661 6365  rSymbolInSurface
+00000370: 506c 6f74 733d 2230 2220 7a6f 6666 7365  Plots="0" zoffse
+00000380: 743d 2230 2220 6578 7472 7573 696f 6e3d  t="0" extrusion=
+00000390: 2230 2220 6269 6e64 696e 673d 2243 656e  "0" binding="Cen
+000003a0: 7472 6f69 6422 2065 7874 7275 7369 6f6e  troid" extrusion
+000003b0: 456e 6162 6c65 643d 2230 2220 7479 7065  Enabled="0" type
+000003c0: 3d22 496e 6469 7669 6475 616c 4665 6174  ="IndividualFeat
+000003d0: 7572 6573 223e 0a20 2020 203c 6461 7461  ures">.    <data
 000003e0: 2d64 6566 696e 6564 2d70 726f 7065 7274  -defined-propert
 000003f0: 6965 733e 0a20 2020 2020 203c 4f70 7469  ies>.      <Opti
 00000400: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
 00000410: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
 00000420: 616c 7565 3d22 2220 6e61 6d65 3d22 6e61  alue="" name="na
 00000430: 6d65 2220 7479 7065 3d22 5153 7472 696e  me" type="QStrin
 00000440: 6722 2f3e 0a20 2020 2020 2020 203c 4f70  g"/>.        <Op
@@ -73,21 +73,21 @@
 00000480: 636f 6c6c 6563 7469 6f6e 2220 6e61 6d65  collection" name
 00000490: 3d22 7479 7065 2220 7479 7065 3d22 5153  ="type" type="QS
 000004a0: 7472 696e 6722 2f3e 0a20 2020 2020 203c  tring"/>.      <
 000004b0: 2f4f 7074 696f 6e3e 0a20 2020 203c 2f64  /Option>.    </d
 000004c0: 6174 612d 6465 6669 6e65 642d 7072 6f70  ata-defined-prop
 000004d0: 6572 7469 6573 3e0a 2020 2020 3c70 726f  erties>.    <pro
 000004e0: 6669 6c65 4c69 6e65 5379 6d62 6f6c 3e0a  fileLineSymbol>.
-000004f0: 2020 2020 2020 3c73 796d 626f 6c20 6973        <symbol is
-00000500: 5f61 6e69 6d61 7465 643d 2230 2220 6e61  _animated="0" na
-00000510: 6d65 3d22 2220 7479 7065 3d22 6c69 6e65  me="" type="line
-00000520: 2220 616c 7068 613d 2231 2220 636c 6970  " alpha="1" clip
-00000530: 5f74 6f5f 6578 7465 6e74 3d22 3122 2066  _to_extent="1" f
-00000540: 6f72 6365 5f72 6872 3d22 3022 2066 7261  orce_rhr="0" fra
-00000550: 6d65 5f72 6174 653d 2231 3022 3e0a 2020  me_rate="10">.  
+000004f0: 2020 2020 2020 3c73 796d 626f 6c20 6672        <symbol fr
+00000500: 616d 655f 7261 7465 3d22 3130 2220 6e61  ame_rate="10" na
+00000510: 6d65 3d22 2220 616c 7068 613d 2231 2220  me="" alpha="1" 
+00000520: 6973 5f61 6e69 6d61 7465 643d 2230 2220  is_animated="0" 
+00000530: 636c 6970 5f74 6f5f 6578 7465 6e74 3d22  clip_to_extent="
+00000540: 3122 2074 7970 653d 226c 696e 6522 2066  1" type="line" f
+00000550: 6f72 6365 5f72 6872 3d22 3022 3e0a 2020  orce_rhr="0">.  
 00000560: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
 00000570: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
 00000580: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
 00000590: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
 000005a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
 000005b0: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
 000005c0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
@@ -98,18 +98,18 @@
 00000610: 696f 6e20 7661 6c75 653d 2263 6f6c 6c65  ion value="colle
 00000620: 6374 696f 6e22 206e 616d 653d 2274 7970  ction" name="typ
 00000630: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
 00000640: 222f 3e0a 2020 2020 2020 2020 2020 3c2f  "/>.          </
 00000650: 4f70 7469 6f6e 3e0a 2020 2020 2020 2020  Option>.        
 00000660: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
 00000670: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
-00000680: 2020 203c 6c61 7965 7220 6c6f 636b 6564     <layer locked
-00000690: 3d22 3022 2063 6c61 7373 3d22 5369 6d70  ="0" class="Simp
-000006a0: 6c65 4c69 6e65 2220 7061 7373 3d22 3022  leLine" pass="0"
-000006b0: 2065 6e61 626c 6564 3d22 3122 3e0a 2020   enabled="1">.  
+00000680: 2020 203c 6c61 7965 7220 636c 6173 733d     <layer class=
+00000690: 2253 696d 706c 654c 696e 6522 2070 6173  "SimpleLine" pas
+000006a0: 733d 2230 2220 656e 6162 6c65 643d 2231  s="0" enabled="1
+000006b0: 2220 6c6f 636b 6564 3d22 3022 3e0a 2020  " locked="0">.  
 000006c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
 000006d0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
 000006e0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
 000006f0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
 00000700: 616c 6967 6e5f 6461 7368 5f70 6174 7465  align_dash_patte
 00000710: 726e 2220 7479 7065 3d22 5153 7472 696e  rn" type="QStrin
 00000720: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
@@ -260,20 +260,20 @@
 00001030: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
 00001040: 0a20 2020 2020 2020 203c 2f6c 6179 6572  .        </layer
 00001050: 3e0a 2020 2020 2020 3c2f 7379 6d62 6f6c  >.      </symbol
 00001060: 3e0a 2020 2020 3c2f 7072 6f66 696c 654c  >.    </profileL
 00001070: 696e 6553 796d 626f 6c3e 0a20 2020 203c  ineSymbol>.    <
 00001080: 7072 6f66 696c 6546 696c 6c53 796d 626f  profileFillSymbo
 00001090: 6c3e 0a20 2020 2020 203c 7379 6d62 6f6c  l>.      <symbol
-000010a0: 2069 735f 616e 696d 6174 6564 3d22 3022   is_animated="0"
-000010b0: 206e 616d 653d 2222 2074 7970 653d 2266   name="" type="f
-000010c0: 696c 6c22 2061 6c70 6861 3d22 3122 2063  ill" alpha="1" c
-000010d0: 6c69 705f 746f 5f65 7874 656e 743d 2231  lip_to_extent="1
-000010e0: 2220 666f 7263 655f 7268 723d 2230 2220  " force_rhr="0" 
-000010f0: 6672 616d 655f 7261 7465 3d22 3130 223e  frame_rate="10">
+000010a0: 2066 7261 6d65 5f72 6174 653d 2231 3022   frame_rate="10"
+000010b0: 206e 616d 653d 2222 2061 6c70 6861 3d22   name="" alpha="
+000010c0: 3122 2069 735f 616e 696d 6174 6564 3d22  1" is_animated="
+000010d0: 3022 2063 6c69 705f 746f 5f65 7874 656e  0" clip_to_exten
+000010e0: 743d 2231 2220 7479 7065 3d22 6669 6c6c  t="1" type="fill
+000010f0: 2220 666f 7263 655f 7268 723d 2230 223e  " force_rhr="0">
 00001100: 0a20 2020 2020 2020 203c 6461 7461 5f64  .        <data_d
 00001110: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
 00001120: 733e 0a20 2020 2020 2020 2020 203c 4f70  s>.          <Op
 00001130: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
 00001140: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
 00001150: 7469 6f6e 2076 616c 7565 3d22 2220 6e61  tion value="" na
 00001160: 6d65 3d22 6e61 6d65 2220 7479 7065 3d22  me="name" type="
@@ -284,18 +284,18 @@
 000011b0: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
 000011c0: 6c6c 6563 7469 6f6e 2220 6e61 6d65 3d22  llection" name="
 000011d0: 7479 7065 2220 7479 7065 3d22 5153 7472  type" type="QStr
 000011e0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
 000011f0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
 00001200: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
 00001210: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00001220: 2020 2020 2020 3c6c 6179 6572 206c 6f63        <layer loc
-00001230: 6b65 643d 2230 2220 636c 6173 733d 2253  ked="0" class="S
-00001240: 696d 706c 6546 696c 6c22 2070 6173 733d  impleFill" pass=
-00001250: 2230 2220 656e 6162 6c65 643d 2231 223e  "0" enabled="1">
+00001220: 2020 2020 2020 3c6c 6179 6572 2063 6c61        <layer cla
+00001230: 7373 3d22 5369 6d70 6c65 4669 6c6c 2220  ss="SimpleFill" 
+00001240: 7061 7373 3d22 3022 2065 6e61 626c 6564  pass="0" enabled
+00001250: 3d22 3122 206c 6f63 6b65 643d 2230 223e  ="1" locked="0">
 00001260: 0a20 2020 2020 2020 2020 203c 4f70 7469  .          <Opti
 00001270: 6f6e 2074 7970 653d 224d 6170 223e 0a20  on type="Map">. 
 00001280: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
 00001290: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
 000012a0: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
 000012b0: 626f 7264 6572 5f77 6964 7468 5f6d 6170  border_width_map
 000012c0: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
@@ -366,21 +366,21 @@
 000016d0: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
 000016e0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
 000016f0: 2020 2020 203c 2f6c 6179 6572 3e0a 2020       </layer>.  
 00001700: 2020 2020 3c2f 7379 6d62 6f6c 3e0a 2020      </symbol>.  
 00001710: 2020 3c2f 7072 6f66 696c 6546 696c 6c53    </profileFillS
 00001720: 796d 626f 6c3e 0a20 2020 203c 7072 6f66  ymbol>.    <prof
 00001730: 696c 654d 6172 6b65 7253 796d 626f 6c3e  ileMarkerSymbol>
-00001740: 0a20 2020 2020 203c 7379 6d62 6f6c 2069  .      <symbol i
-00001750: 735f 616e 696d 6174 6564 3d22 3022 206e  s_animated="0" n
-00001760: 616d 653d 2222 2074 7970 653d 226d 6172  ame="" type="mar
-00001770: 6b65 7222 2061 6c70 6861 3d22 3122 2063  ker" alpha="1" c
-00001780: 6c69 705f 746f 5f65 7874 656e 743d 2231  lip_to_extent="1
-00001790: 2220 666f 7263 655f 7268 723d 2230 2220  " force_rhr="0" 
-000017a0: 6672 616d 655f 7261 7465 3d22 3130 223e  frame_rate="10">
+00001740: 0a20 2020 2020 203c 7379 6d62 6f6c 2066  .      <symbol f
+00001750: 7261 6d65 5f72 6174 653d 2231 3022 206e  rame_rate="10" n
+00001760: 616d 653d 2222 2061 6c70 6861 3d22 3122  ame="" alpha="1"
+00001770: 2069 735f 616e 696d 6174 6564 3d22 3022   is_animated="0"
+00001780: 2063 6c69 705f 746f 5f65 7874 656e 743d   clip_to_extent=
+00001790: 2231 2220 7479 7065 3d22 6d61 726b 6572  "1" type="marker
+000017a0: 2220 666f 7263 655f 7268 723d 2230 223e  " force_rhr="0">
 000017b0: 0a20 2020 2020 2020 203c 6461 7461 5f64  .        <data_d
 000017c0: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
 000017d0: 733e 0a20 2020 2020 2020 2020 203c 4f70  s>.          <Op
 000017e0: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
 000017f0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
 00001800: 7469 6f6e 2076 616c 7565 3d22 2220 6e61  tion value="" na
 00001810: 6d65 3d22 6e61 6d65 2220 7479 7065 3d22  me="name" type="
@@ -391,18 +391,18 @@
 00001860: 4f70 7469 6f6e 2076 616c 7565 3d22 636f  Option value="co
 00001870: 6c6c 6563 7469 6f6e 2220 6e61 6d65 3d22  llection" name="
 00001880: 7479 7065 2220 7479 7065 3d22 5153 7472  type" type="QStr
 00001890: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
 000018a0: 203c 2f4f 7074 696f 6e3e 0a20 2020 2020   </Option>.     
 000018b0: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
 000018c0: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-000018d0: 2020 2020 2020 3c6c 6179 6572 206c 6f63        <layer loc
-000018e0: 6b65 643d 2230 2220 636c 6173 733d 2253  ked="0" class="S
-000018f0: 696d 706c 654d 6172 6b65 7222 2070 6173  impleMarker" pas
-00001900: 733d 2230 2220 656e 6162 6c65 643d 2231  s="0" enabled="1
+000018d0: 2020 2020 2020 3c6c 6179 6572 2063 6c61        <layer cla
+000018e0: 7373 3d22 5369 6d70 6c65 4d61 726b 6572  ss="SimpleMarker
+000018f0: 2220 7061 7373 3d22 3022 2065 6e61 626c  " pass="0" enabl
+00001900: 6564 3d22 3122 206c 6f63 6b65 643d 2230  ed="1" locked="0
 00001910: 223e 0a20 2020 2020 2020 2020 203c 4f70  ">.          <Op
 00001920: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
 00001930: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
 00001940: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
 00001950: 616d 653d 2261 6e67 6c65 2220 7479 7065  ame="angle" type
 00001960: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
 00001970: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
@@ -509,1339 +509,1283 @@
 00001fc0: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
 00001fd0: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
 00001fe0: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
 00001ff0: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 3c2f  </symbol>.    </
 00002000: 7072 6f66 696c 654d 6172 6b65 7253 796d  profileMarkerSym
 00002010: 626f 6c3e 0a20 203c 2f65 6c65 7661 7469  bol>.  </elevati
 00002020: 6f6e 3e0a 2020 3c72 656e 6465 7265 722d  on>.  <renderer-
-00002030: 7632 2073 796d 626f 6c6c 6576 656c 733d  v2 symbollevels=
-00002040: 2230 2220 7265 6665 7265 6e63 6573 6361  "0" referencesca
-00002050: 6c65 3d22 2d31 2220 656e 6162 6c65 6f72  le="-1" enableor
-00002060: 6465 7262 793d 2230 2220 7479 7065 3d22  derby="0" type="
-00002070: 5275 6c65 5265 6e64 6572 6572 2220 666f  RuleRenderer" fo
-00002080: 7263 6572 6173 7465 723d 2230 223e 0a20  rceraster="0">. 
+00002030: 7632 2072 6566 6572 656e 6365 7363 616c  v2 referencescal
+00002040: 653d 222d 3122 2065 6e61 626c 656f 7264  e="-1" enableord
+00002050: 6572 6279 3d22 3022 2073 796d 626f 6c6c  erby="0" symboll
+00002060: 6576 656c 733d 2230 2220 666f 7263 6572  evels="0" forcer
+00002070: 6173 7465 723d 2230 2220 7479 7065 3d22  aster="0" type="
+00002080: 5275 6c65 5265 6e64 6572 6572 223e 0a20  RuleRenderer">. 
 00002090: 2020 203c 7275 6c65 7320 6b65 793d 227b     <rules key="{
 000020a0: 3130 6330 3465 3336 2d31 6633 632d 3437  10c04e36-1f3c-47
 000020b0: 6365 2d61 3230 632d 3831 3430 3533 6161  ce-a20c-814053aa
 000020c0: 3332 3865 7d22 3e0a 2020 2020 2020 3c72  328e}">.      <r
-000020d0: 756c 6520 6b65 793d 227b 3338 3939 3865  ule key="{38998e
-000020e0: 6366 2d37 3533 302d 3439 3362 2d38 3263  cf-7530-493b-82c
-000020f0: 362d 3236 3661 6130 3034 3339 3330 7d22  6-266aa0043930}"
-00002100: 2073 796d 626f 6c3d 2230 2220 6669 6c74   symbol="0" filt
-00002110: 6572 3d22 2671 756f 743b 7479 7065 2671  er="&quot;type&q
-00002120: 756f 743b 203d 2027 7369 6465 7761 6c6b  uot; = 'sidewalk
-00002130: 2726 2378 613b 222f 3e0a 2020 2020 2020  '&#xa;"/>.      
-00002140: 3c72 756c 6520 6b65 793d 227b 3535 6136  <rule key="{55a6
-00002150: 6233 3433 2d32 6431 612d 3464 3461 2d38  b343-2d1a-4d4a-8
-00002160: 3237 622d 3230 3333 3532 6131 3965 3132  27b-203352a19e12
-00002170: 7d22 2073 796d 626f 6c3d 2231 2220 6669  }" symbol="1" fi
-00002180: 6c74 6572 3d22 2671 756f 743b 7479 7065  lter="&quot;type
-00002190: 2671 756f 743b 203d 2027 7472 6166 6669  &quot; = 'traffi
-000021a0: 635f 6973 6c61 6e64 2722 2f3e 0a20 2020  c_island'"/>.   
-000021b0: 203c 2f72 756c 6573 3e0a 2020 2020 3c73   </rules>.    <s
-000021c0: 796d 626f 6c73 3e0a 2020 2020 2020 3c73  ymbols>.      <s
-000021d0: 796d 626f 6c20 6973 5f61 6e69 6d61 7465  ymbol is_animate
-000021e0: 643d 2230 2220 6e61 6d65 3d22 3022 2074  d="0" name="0" t
-000021f0: 7970 653d 226c 696e 6522 2061 6c70 6861  ype="line" alpha
-00002200: 3d22 3122 2063 6c69 705f 746f 5f65 7874  ="1" clip_to_ext
-00002210: 656e 743d 2231 2220 666f 7263 655f 7268  ent="1" force_rh
-00002220: 723d 2230 2220 6672 616d 655f 7261 7465  r="0" frame_rate
-00002230: 3d22 3130 223e 0a20 2020 2020 2020 203c  ="10">.        <
-00002240: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-00002250: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-00002260: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00002270: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00002280: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00002290: 3d22 2220 6e61 6d65 3d22 6e61 6d65 2220  ="" name="name" 
-000022a0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-000022b0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-000022c0: 7469 6f6e 206e 616d 653d 2270 726f 7065  tion name="prope
-000022d0: 7274 6965 7322 2f3e 0a20 2020 2020 2020  rties"/>.       
-000022e0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-000022f0: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
-00002300: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
-00002310: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00002320: 2020 2020 2020 203c 2f4f 7074 696f 6e3e         </Option>
-00002330: 0a20 2020 2020 2020 203c 2f64 6174 615f  .        </data_
-00002340: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
-00002350: 6573 3e0a 2020 2020 2020 2020 3c6c 6179  es>.        <lay
-00002360: 6572 206c 6f63 6b65 643d 2230 2220 636c  er locked="0" cl
-00002370: 6173 733d 2253 696d 706c 654c 696e 6522  ass="SimpleLine"
-00002380: 2070 6173 733d 2230 2220 656e 6162 6c65   pass="0" enable
-00002390: 643d 2231 223e 0a20 2020 2020 2020 2020  d="1">.         
-000023a0: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
-000023b0: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
-000023c0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000023d0: 3022 206e 616d 653d 2261 6c69 676e 5f64  0" name="align_d
-000023e0: 6173 685f 7061 7474 6572 6e22 2074 7970  ash_pattern" typ
-000023f0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002400: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002410: 6e20 7661 6c75 653d 2273 7175 6172 6522  n value="square"
-00002420: 206e 616d 653d 2263 6170 7374 796c 6522   name="capstyle"
-00002430: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00002440: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00002450: 7074 696f 6e20 7661 6c75 653d 2235 3b32  ption value="5;2
-00002460: 2220 6e61 6d65 3d22 6375 7374 6f6d 6461  " name="customda
-00002470: 7368 2220 7479 7065 3d22 5153 7472 696e  sh" type="QStrin
-00002480: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00002490: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000024a0: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-000024b0: 6e61 6d65 3d22 6375 7374 6f6d 6461 7368  name="customdash
-000024c0: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
-000024d0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000024e0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-000024f0: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
-00002500: 206e 616d 653d 2263 7573 746f 6d64 6173   name="customdas
-00002510: 685f 756e 6974 2220 7479 7065 3d22 5153  h_unit" type="QS
-00002520: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002530: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002540: 7565 3d22 3022 206e 616d 653d 2264 6173  ue="0" name="das
-00002550: 685f 7061 7474 6572 6e5f 6f66 6673 6574  h_pattern_offset
-00002560: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00002570: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00002580: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-00002590: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
-000025a0: 6d65 3d22 6461 7368 5f70 6174 7465 726e  me="dash_pattern
-000025b0: 5f6f 6666 7365 745f 6d61 705f 756e 6974  _offset_map_unit
-000025c0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-000025d0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-000025e0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-000025f0: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6461  ue="MM" name="da
-00002600: 7368 5f70 6174 7465 726e 5f6f 6666 7365  sh_pattern_offse
-00002610: 745f 756e 6974 2220 7479 7065 3d22 5153  t_unit" type="QS
-00002620: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002630: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002640: 7565 3d22 3022 206e 616d 653d 2264 7261  ue="0" name="dra
-00002650: 775f 696e 7369 6465 5f70 6f6c 7967 6f6e  w_inside_polygon
-00002660: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00002670: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00002680: 4f70 7469 6f6e 2076 616c 7565 3d22 6265  Option value="be
-00002690: 7665 6c22 206e 616d 653d 226a 6f69 6e73  vel" name="joins
-000026a0: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
-000026b0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000026c0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000026d0: 3d22 3235 352c 3235 352c 3235 352c 3235  ="255,255,255,25
-000026e0: 3522 206e 616d 653d 226c 696e 655f 636f  5" name="line_co
-000026f0: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
-00002700: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00002710: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00002720: 2273 6f6c 6964 2220 6e61 6d65 3d22 6c69  "solid" name="li
-00002730: 6e65 5f73 7479 6c65 2220 7479 7065 3d22  ne_style" type="
-00002740: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00002750: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00002760: 616c 7565 3d22 3822 206e 616d 653d 226c  alue="8" name="l
-00002770: 696e 655f 7769 6474 6822 2074 7970 653d  ine_width" type=
-00002780: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00002790: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000027a0: 7661 6c75 653d 224d 4d22 206e 616d 653d  value="MM" name=
-000027b0: 226c 696e 655f 7769 6474 685f 756e 6974  "line_width_unit
-000027c0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000027d0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000027e0: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
-000027f0: 206e 616d 653d 226f 6666 7365 7422 2074   name="offset" t
-00002800: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00002810: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00002820: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
-00002830: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
-00002840: 226f 6666 7365 745f 6d61 705f 756e 6974  "offset_map_unit
-00002850: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00002860: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00002870: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00002880: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6f66  ue="MM" name="of
-00002890: 6673 6574 5f75 6e69 7422 2074 7970 653d  fset_unit" type=
-000028a0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000028b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000028c0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-000028d0: 7269 6e67 5f66 696c 7465 7222 2074 7970  ring_filter" typ
-000028e0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000028f0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002900: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-00002910: 3d22 7472 696d 5f64 6973 7461 6e63 655f  ="trim_distance_
-00002920: 656e 6422 2074 7970 653d 2251 5374 7269  end" type="QStri
-00002930: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00002940: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00002950: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
-00002960: 206e 616d 653d 2274 7269 6d5f 6469 7374   name="trim_dist
-00002970: 616e 6365 5f65 6e64 5f6d 6170 5f75 6e69  ance_end_map_uni
-00002980: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-00002990: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-000029a0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000029b0: 6c75 653d 224d 4d22 206e 616d 653d 2274  lue="MM" name="t
-000029c0: 7269 6d5f 6469 7374 616e 6365 5f65 6e64  rim_distance_end
-000029d0: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
-000029e0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000029f0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002a00: 653d 2230 2220 6e61 6d65 3d22 7472 696d  e="0" name="trim
-00002a10: 5f64 6973 7461 6e63 655f 7374 6172 7422  _distance_start"
-00002a20: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00002a30: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00002a40: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
-00002a50: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
-00002a60: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
-00002a70: 5f73 7461 7274 5f6d 6170 5f75 6e69 745f  _start_map_unit_
-00002a80: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
-00002a90: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002aa0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002ab0: 653d 224d 4d22 206e 616d 653d 2274 7269  e="MM" name="tri
-00002ac0: 6d5f 6469 7374 616e 6365 5f73 7461 7274  m_distance_start
-00002ad0: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
-00002ae0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002af0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002b00: 653d 2230 2220 6e61 6d65 3d22 7477 6561  e="0" name="twea
-00002b10: 6b5f 6461 7368 5f70 6174 7465 726e 5f6f  k_dash_pattern_o
-00002b20: 6e5f 636f 726e 6572 7322 2074 7970 653d  n_corners" type=
-00002b30: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00002b40: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00002b50: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-00002b60: 7573 655f 6375 7374 6f6d 5f64 6173 6822  use_custom_dash"
-00002b70: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00002b80: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00002b90: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
-00002ba0: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
-00002bb0: 653d 2277 6964 7468 5f6d 6170 5f75 6e69  e="width_map_uni
-00002bc0: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-00002bd0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00002be0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00002bf0: 2020 2020 2020 2020 3c64 6174 615f 6465          <data_de
-00002c00: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
-00002c10: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00002c20: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
-00002c30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002c40: 3c4f 7074 696f 6e20 7661 6c75 653d 2222  <Option value=""
-00002c50: 206e 616d 653d 226e 616d 6522 2074 7970   name="name" typ
-00002c60: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002c70: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00002c80: 696f 6e20 6e61 6d65 3d22 7072 6f70 6572  ion name="proper
-00002c90: 7469 6573 222f 3e0a 2020 2020 2020 2020  ties"/>.        
-00002ca0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00002cb0: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
-00002cc0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00002cd0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002ce0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-00002cf0: 6f6e 3e0a 2020 2020 2020 2020 2020 3c2f  on>.          </
-00002d00: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-00002d10: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-00002d20: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
-00002d30: 2020 3c6c 6179 6572 206c 6f63 6b65 643d    <layer locked=
-00002d40: 2230 2220 636c 6173 733d 2253 696d 706c  "0" class="Simpl
-00002d50: 654c 696e 6522 2070 6173 733d 2230 2220  eLine" pass="0" 
-00002d60: 656e 6162 6c65 643d 2231 223e 0a20 2020  enabled="1">.   
-00002d70: 2020 2020 2020 203c 4f70 7469 6f6e 2074         <Option t
-00002d80: 7970 653d 224d 6170 223e 0a20 2020 2020  ype="Map">.     
-00002d90: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00002da0: 616c 7565 3d22 3022 206e 616d 653d 2261  alue="0" name="a
-00002db0: 6c69 676e 5f64 6173 685f 7061 7474 6572  lign_dash_patter
-00002dc0: 6e22 2074 7970 653d 2251 5374 7269 6e67  n" type="QString
-00002dd0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00002de0: 3c4f 7074 696f 6e20 7661 6c75 653d 2272  <Option value="r
-00002df0: 6f75 6e64 2220 6e61 6d65 3d22 6361 7073  ound" name="caps
-00002e00: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
-00002e10: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00002e20: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00002e30: 3d22 353b 3222 206e 616d 653d 2263 7573  ="5;2" name="cus
-00002e40: 746f 6d64 6173 6822 2074 7970 653d 2251  tomdash" type="Q
-00002e50: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00002e60: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00002e70: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
-00002e80: 302c 3022 206e 616d 653d 2263 7573 746f  0,0" name="custo
-00002e90: 6d64 6173 685f 6d61 705f 756e 6974 5f73  mdash_map_unit_s
-00002ea0: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
-00002eb0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00002ec0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00002ed0: 3d22 4d4d 2220 6e61 6d65 3d22 6375 7374  ="MM" name="cust
-00002ee0: 6f6d 6461 7368 5f75 6e69 7422 2074 7970  omdash_unit" typ
-00002ef0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002f00: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002f10: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-00002f20: 3d22 6461 7368 5f70 6174 7465 726e 5f6f  ="dash_pattern_o
-00002f30: 6666 7365 7422 2074 7970 653d 2251 5374  ffset" type="QSt
-00002f40: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00002f50: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00002f60: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
-00002f70: 3022 206e 616d 653d 2264 6173 685f 7061  0" name="dash_pa
-00002f80: 7474 6572 6e5f 6f66 6673 6574 5f6d 6170  ttern_offset_map
-00002f90: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
-00002fa0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00002fb0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00002fc0: 6e20 7661 6c75 653d 224d 4d22 206e 616d  n value="MM" nam
-00002fd0: 653d 2264 6173 685f 7061 7474 6572 6e5f  e="dash_pattern_
-00002fe0: 6f66 6673 6574 5f75 6e69 7422 2074 7970  offset_unit" typ
-00002ff0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003000: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00003010: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-00003020: 3d22 6472 6177 5f69 6e73 6964 655f 706f  ="draw_inside_po
-00003030: 6c79 676f 6e22 2074 7970 653d 2251 5374  lygon" type="QSt
-00003040: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003050: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003060: 653d 2272 6f75 6e64 2220 6e61 6d65 3d22  e="round" name="
-00003070: 6a6f 696e 7374 796c 6522 2074 7970 653d  joinstyle" type=
-00003080: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00003090: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000030a0: 7661 6c75 653d 2230 2c30 2c30 2c32 3535  value="0,0,0,255
-000030b0: 2220 6e61 6d65 3d22 6c69 6e65 5f63 6f6c  " name="line_col
-000030c0: 6f72 2220 7479 7065 3d22 5153 7472 696e  or" type="QStrin
-000030d0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-000030e0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000030f0: 736f 6c69 6422 206e 616d 653d 226c 696e  solid" name="lin
-00003100: 655f 7374 796c 6522 2074 7970 653d 2251  e_style" type="Q
-00003110: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00003120: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003130: 6c75 653d 2232 2220 6e61 6d65 3d22 6c69  lue="2" name="li
-00003140: 6e65 5f77 6964 7468 2220 7479 7065 3d22  ne_width" type="
-00003150: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003160: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003170: 616c 7565 3d22 4d4d 2220 6e61 6d65 3d22  alue="MM" name="
-00003180: 6c69 6e65 5f77 6964 7468 5f75 6e69 7422  line_width_unit"
-00003190: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000031a0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-000031b0: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-000031c0: 6e61 6d65 3d22 6f66 6673 6574 2220 7479  name="offset" ty
-000031d0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-000031e0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000031f0: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
-00003200: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
-00003210: 6f66 6673 6574 5f6d 6170 5f75 6e69 745f  offset_map_unit_
-00003220: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
-00003230: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00003240: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00003250: 653d 224d 4d22 206e 616d 653d 226f 6666  e="MM" name="off
-00003260: 7365 745f 756e 6974 2220 7479 7065 3d22  set_unit" type="
-00003270: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003280: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003290: 616c 7565 3d22 3022 206e 616d 653d 2272  alue="0" name="r
-000032a0: 696e 675f 6669 6c74 6572 2220 7479 7065  ing_filter" type
-000032b0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-000032c0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000032d0: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
-000032e0: 2274 7269 6d5f 6469 7374 616e 6365 5f65  "trim_distance_e
-000032f0: 6e64 2220 7479 7065 3d22 5153 7472 696e  nd" type="QStrin
-00003300: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00003310: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00003320: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-00003330: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00003340: 6e63 655f 656e 645f 6d61 705f 756e 6974  nce_end_map_unit
-00003350: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00003360: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003370: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003380: 7565 3d22 4d4d 2220 6e61 6d65 3d22 7472  ue="MM" name="tr
-00003390: 696d 5f64 6973 7461 6e63 655f 656e 645f  im_distance_end_
-000033a0: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
-000033b0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000033c0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000033d0: 3d22 3022 206e 616d 653d 2274 7269 6d5f  ="0" name="trim_
-000033e0: 6469 7374 616e 6365 5f73 7461 7274 2220  distance_start" 
-000033f0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003400: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003410: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
-00003420: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
-00003430: 3d22 7472 696d 5f64 6973 7461 6e63 655f  ="trim_distance_
-00003440: 7374 6172 745f 6d61 705f 756e 6974 5f73  start_map_unit_s
-00003450: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
-00003460: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003470: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00003480: 3d22 4d4d 2220 6e61 6d65 3d22 7472 696d  ="MM" name="trim
-00003490: 5f64 6973 7461 6e63 655f 7374 6172 745f  _distance_start_
-000034a0: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
-000034b0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000034c0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000034d0: 3d22 3022 206e 616d 653d 2274 7765 616b  ="0" name="tweak
-000034e0: 5f64 6173 685f 7061 7474 6572 6e5f 6f6e  _dash_pattern_on
-000034f0: 5f63 6f72 6e65 7273 2220 7479 7065 3d22  _corners" type="
-00003500: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003510: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003520: 616c 7565 3d22 3022 206e 616d 653d 2275  alue="0" name="u
-00003530: 7365 5f63 7573 746f 6d5f 6461 7368 2220  se_custom_dash" 
-00003540: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003550: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003560: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
-00003570: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
-00003580: 3d22 7769 6474 685f 6d61 705f 756e 6974  ="width_map_unit
-00003590: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-000035a0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-000035b0: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
-000035c0: 2020 2020 2020 203c 6461 7461 5f64 6566         <data_def
-000035d0: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
-000035e0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-000035f0: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
-00003600: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00003610: 4f70 7469 6f6e 2076 616c 7565 3d22 2220  Option value="" 
-00003620: 6e61 6d65 3d22 6e61 6d65 2220 7479 7065  name="name" type
-00003630: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003640: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003650: 6f6e 206e 616d 653d 2270 726f 7065 7274  on name="propert
-00003660: 6965 7322 2f3e 0a20 2020 2020 2020 2020  ies"/>.         
-00003670: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003680: 7565 3d22 636f 6c6c 6563 7469 6f6e 2220  ue="collection" 
-00003690: 6e61 6d65 3d22 7479 7065 2220 7479 7065  name="type" type
-000036a0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-000036b0: 2020 2020 2020 2020 203c 2f4f 7074 696f           </Optio
-000036c0: 6e3e 0a20 2020 2020 2020 2020 203c 2f64  n>.          </d
-000036d0: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
-000036e0: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
-000036f0: 3c2f 6c61 7965 723e 0a20 2020 2020 203c  </layer>.      <
-00003700: 2f73 796d 626f 6c3e 0a20 2020 2020 203c  /symbol>.      <
-00003710: 7379 6d62 6f6c 2069 735f 616e 696d 6174  symbol is_animat
-00003720: 6564 3d22 3022 206e 616d 653d 2231 2220  ed="0" name="1" 
-00003730: 7479 7065 3d22 6c69 6e65 2220 616c 7068  type="line" alph
-00003740: 613d 2231 2220 636c 6970 5f74 6f5f 6578  a="1" clip_to_ex
-00003750: 7465 6e74 3d22 3122 2066 6f72 6365 5f72  tent="1" force_r
-00003760: 6872 3d22 3022 2066 7261 6d65 5f72 6174  hr="0" frame_rat
-00003770: 653d 2231 3022 3e0a 2020 2020 2020 2020  e="10">.        
-00003780: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-00003790: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-000037a0: 2020 2020 3c4f 7074 696f 6e20 7479 7065      <Option type
-000037b0: 3d22 4d61 7022 3e0a 2020 2020 2020 2020  ="Map">.        
-000037c0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000037d0: 653d 2222 206e 616d 653d 226e 616d 6522  e="" name="name"
-000037e0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-000037f0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00003800: 7074 696f 6e20 6e61 6d65 3d22 7072 6f70  ption name="prop
-00003810: 6572 7469 6573 222f 3e0a 2020 2020 2020  erties"/>.      
-00003820: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003830: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
-00003840: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00003850: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00003860: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
-00003870: 3e0a 2020 2020 2020 2020 3c2f 6461 7461  >.        </data
-00003880: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
-00003890: 6965 733e 0a20 2020 2020 2020 203c 6c61  ies>.        <la
-000038a0: 7965 7220 6c6f 636b 6564 3d22 3022 2063  yer locked="0" c
-000038b0: 6c61 7373 3d22 5369 6d70 6c65 4c69 6e65  lass="SimpleLine
-000038c0: 2220 7061 7373 3d22 3022 2065 6e61 626c  " pass="0" enabl
-000038d0: 6564 3d22 3122 3e0a 2020 2020 2020 2020  ed="1">.        
-000038e0: 2020 3c4f 7074 696f 6e20 7479 7065 3d22    <Option type="
-000038f0: 4d61 7022 3e0a 2020 2020 2020 2020 2020  Map">.          
-00003900: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00003910: 2230 2220 6e61 6d65 3d22 616c 6967 6e5f  "0" name="align_
-00003920: 6461 7368 5f70 6174 7465 726e 2220 7479  dash_pattern" ty
-00003930: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003940: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003950: 6f6e 2076 616c 7565 3d22 726f 756e 6422  on value="round"
-00003960: 206e 616d 653d 2263 6170 7374 796c 6522   name="capstyle"
-00003970: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00003980: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00003990: 7074 696f 6e20 7661 6c75 653d 2235 3b32  ption value="5;2
-000039a0: 2220 6e61 6d65 3d22 6375 7374 6f6d 6461  " name="customda
-000039b0: 7368 2220 7479 7065 3d22 5153 7472 696e  sh" type="QStrin
-000039c0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-000039d0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000039e0: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
-000039f0: 6e61 6d65 3d22 6375 7374 6f6d 6461 7368  name="customdash
-00003a00: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
-00003a10: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00003a20: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00003a30: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
-00003a40: 206e 616d 653d 2263 7573 746f 6d64 6173   name="customdas
-00003a50: 685f 756e 6974 2220 7479 7065 3d22 5153  h_unit" type="QS
-00003a60: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003a70: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003a80: 7565 3d22 3022 206e 616d 653d 2264 6173  ue="0" name="das
-00003a90: 685f 7061 7474 6572 6e5f 6f66 6673 6574  h_pattern_offset
-00003aa0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003ab0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003ac0: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-00003ad0: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
-00003ae0: 6d65 3d22 6461 7368 5f70 6174 7465 726e  me="dash_pattern
-00003af0: 5f6f 6666 7365 745f 6d61 705f 756e 6974  _offset_map_unit
-00003b00: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00003b10: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003b20: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003b30: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6461  ue="MM" name="da
-00003b40: 7368 5f70 6174 7465 726e 5f6f 6666 7365  sh_pattern_offse
-00003b50: 745f 756e 6974 2220 7479 7065 3d22 5153  t_unit" type="QS
-00003b60: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003b70: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003b80: 7565 3d22 3022 206e 616d 653d 2264 7261  ue="0" name="dra
-00003b90: 775f 696e 7369 6465 5f70 6f6c 7967 6f6e  w_inside_polygon
-00003ba0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003bb0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003bc0: 4f70 7469 6f6e 2076 616c 7565 3d22 726f  Option value="ro
-00003bd0: 756e 6422 206e 616d 653d 226a 6f69 6e73  und" name="joins
-00003be0: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
-00003bf0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003c00: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00003c10: 3d22 3235 352c 3235 352c 3235 352c 3235  ="255,255,255,25
-00003c20: 3522 206e 616d 653d 226c 696e 655f 636f  5" name="line_co
-00003c30: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
-00003c40: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00003c50: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00003c60: 2273 6f6c 6964 2220 6e61 6d65 3d22 6c69  "solid" name="li
-00003c70: 6e65 5f73 7479 6c65 2220 7479 7065 3d22  ne_style" type="
-00003c80: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003c90: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003ca0: 616c 7565 3d22 3130 2220 6e61 6d65 3d22  alue="10" name="
-00003cb0: 6c69 6e65 5f77 6964 7468 2220 7479 7065  line_width" type
-00003cc0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003cd0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003ce0: 2076 616c 7565 3d22 4d4d 2220 6e61 6d65   value="MM" name
-00003cf0: 3d22 6c69 6e65 5f77 6964 7468 5f75 6e69  ="line_width_uni
-00003d00: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
-00003d10: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00003d20: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
-00003d30: 2220 6e61 6d65 3d22 6f66 6673 6574 2220  " name="offset" 
-00003d40: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00003d50: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
-00003d60: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
-00003d70: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
-00003d80: 3d22 6f66 6673 6574 5f6d 6170 5f75 6e69  ="offset_map_uni
-00003d90: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-00003da0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00003db0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00003dc0: 6c75 653d 224d 4d22 206e 616d 653d 226f  lue="MM" name="o
-00003dd0: 6666 7365 745f 756e 6974 2220 7479 7065  ffset_unit" type
-00003de0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00003df0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00003e00: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
-00003e10: 2272 696e 675f 6669 6c74 6572 2220 7479  "ring_filter" ty
-00003e20: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00003e30: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00003e40: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
-00003e50: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
-00003e60: 5f65 6e64 2220 7479 7065 3d22 5153 7472  _end" type="QStr
-00003e70: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00003e80: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-00003e90: 3d22 3378 3a30 2c30 2c30 2c30 2c30 2c30  ="3x:0,0,0,0,0,0
-00003ea0: 2220 6e61 6d65 3d22 7472 696d 5f64 6973  " name="trim_dis
-00003eb0: 7461 6e63 655f 656e 645f 6d61 705f 756e  tance_end_map_un
-00003ec0: 6974 5f73 6361 6c65 2220 7479 7065 3d22  it_scale" type="
-00003ed0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00003ee0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00003ef0: 616c 7565 3d22 4d4d 2220 6e61 6d65 3d22  alue="MM" name="
-00003f00: 7472 696d 5f64 6973 7461 6e63 655f 656e  trim_distance_en
-00003f10: 645f 756e 6974 2220 7479 7065 3d22 5153  d_unit" type="QS
-00003f20: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003f30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003f40: 7565 3d22 3022 206e 616d 653d 2274 7269  ue="0" name="tri
-00003f50: 6d5f 6469 7374 616e 6365 5f73 7461 7274  m_distance_start
-00003f60: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00003f70: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-00003f80: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-00003f90: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
-00003fa0: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
-00003fb0: 655f 7374 6172 745f 6d61 705f 756e 6974  e_start_map_unit
-00003fc0: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00003fd0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00003fe0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00003ff0: 7565 3d22 4d4d 2220 6e61 6d65 3d22 7472  ue="MM" name="tr
-00004000: 696d 5f64 6973 7461 6e63 655f 7374 6172  im_distance_star
-00004010: 745f 756e 6974 2220 7479 7065 3d22 5153  t_unit" type="QS
-00004020: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004030: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00004040: 7565 3d22 3022 206e 616d 653d 2274 7765  ue="0" name="twe
-00004050: 616b 5f64 6173 685f 7061 7474 6572 6e5f  ak_dash_pattern_
-00004060: 6f6e 5f63 6f72 6e65 7273 2220 7479 7065  on_corners" type
-00004070: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00004080: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-00004090: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
-000040a0: 2275 7365 5f63 7573 746f 6d5f 6461 7368  "use_custom_dash
-000040b0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000040c0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000040d0: 4f70 7469 6f6e 2076 616c 7565 3d22 3378  Option value="3x
-000040e0: 3a30 2c30 2c30 2c30 2c30 2c30 2220 6e61  :0,0,0,0,0,0" na
-000040f0: 6d65 3d22 7769 6474 685f 6d61 705f 756e  me="width_map_un
-00004100: 6974 5f73 6361 6c65 2220 7479 7065 3d22  it_scale" type="
-00004110: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00004120: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-00004130: 2020 2020 2020 2020 203c 6461 7461 5f64           <data_d
-00004140: 6566 696e 6564 5f70 726f 7065 7274 6965  efined_propertie
-00004150: 733e 0a20 2020 2020 2020 2020 2020 203c  s>.            <
-00004160: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
-00004170: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00004180: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00004190: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
-000041a0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-000041b0: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
-000041c0: 7469 6f6e 206e 616d 653d 2270 726f 7065  tion name="prope
-000041d0: 7274 6965 7322 2f3e 0a20 2020 2020 2020  rties"/>.       
-000041e0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-000041f0: 616c 7565 3d22 636f 6c6c 6563 7469 6f6e  alue="collection
-00004200: 2220 6e61 6d65 3d22 7479 7065 2220 7479  " name="type" ty
-00004210: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00004220: 2020 2020 2020 2020 2020 203c 2f4f 7074             </Opt
-00004230: 696f 6e3e 0a20 2020 2020 2020 2020 203c  ion>.          <
-00004240: 2f64 6174 615f 6465 6669 6e65 645f 7072  /data_defined_pr
-00004250: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00004260: 2020 3c2f 6c61 7965 723e 0a20 2020 2020    </layer>.     
-00004270: 2020 203c 6c61 7965 7220 6c6f 636b 6564     <layer locked
-00004280: 3d22 3022 2063 6c61 7373 3d22 5369 6d70  ="0" class="Simp
-00004290: 6c65 4c69 6e65 2220 7061 7373 3d22 3022  leLine" pass="0"
-000042a0: 2065 6e61 626c 6564 3d22 3122 3e0a 2020   enabled="1">.  
-000042b0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000042c0: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-000042d0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000042e0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-000042f0: 616c 6967 6e5f 6461 7368 5f70 6174 7465  align_dash_patte
-00004300: 726e 2220 7479 7065 3d22 5153 7472 696e  rn" type="QStrin
-00004310: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-00004320: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00004330: 726f 756e 6422 206e 616d 653d 2263 6170  round" name="cap
-00004340: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
-00004350: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004360: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004370: 653d 2235 3b32 2220 6e61 6d65 3d22 6375  e="5;2" name="cu
-00004380: 7374 6f6d 6461 7368 2220 7479 7065 3d22  stomdash" type="
-00004390: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-000043a0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-000043b0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-000043c0: 2c30 2c30 2220 6e61 6d65 3d22 6375 7374  ,0,0" name="cust
-000043d0: 6f6d 6461 7368 5f6d 6170 5f75 6e69 745f  omdash_map_unit_
-000043e0: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
-000043f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004400: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004410: 653d 224d 4d22 206e 616d 653d 2263 7573  e="MM" name="cus
-00004420: 746f 6d64 6173 685f 756e 6974 2220 7479  tomdash_unit" ty
-00004430: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00004440: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004450: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
-00004460: 653d 2264 6173 685f 7061 7474 6572 6e5f  e="dash_pattern_
-00004470: 6f66 6673 6574 2220 7479 7065 3d22 5153  offset" type="QS
-00004480: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004490: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-000044a0: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
-000044b0: 2c30 2220 6e61 6d65 3d22 6461 7368 5f70  ,0" name="dash_p
-000044c0: 6174 7465 726e 5f6f 6666 7365 745f 6d61  attern_offset_ma
-000044d0: 705f 756e 6974 5f73 6361 6c65 2220 7479  p_unit_scale" ty
-000044e0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-000044f0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004500: 6f6e 2076 616c 7565 3d22 4d4d 2220 6e61  on value="MM" na
-00004510: 6d65 3d22 6461 7368 5f70 6174 7465 726e  me="dash_pattern
-00004520: 5f6f 6666 7365 745f 756e 6974 2220 7479  _offset_unit" ty
-00004530: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00004540: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00004550: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
-00004560: 653d 2264 7261 775f 696e 7369 6465 5f70  e="draw_inside_p
-00004570: 6f6c 7967 6f6e 2220 7479 7065 3d22 5153  olygon" type="QS
-00004580: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004590: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-000045a0: 7565 3d22 726f 756e 6422 206e 616d 653d  ue="round" name=
-000045b0: 226a 6f69 6e73 7479 6c65 2220 7479 7065  "joinstyle" type
-000045c0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-000045d0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
-000045e0: 2076 616c 7565 3d22 302c 302c 302c 3235   value="0,0,0,25
-000045f0: 3522 206e 616d 653d 226c 696e 655f 636f  5" name="line_co
-00004600: 6c6f 7222 2074 7970 653d 2251 5374 7269  lor" type="QStri
-00004610: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00004620: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00004630: 2273 6f6c 6964 2220 6e61 6d65 3d22 6c69  "solid" name="li
-00004640: 6e65 5f73 7479 6c65 2220 7479 7065 3d22  ne_style" type="
-00004650: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
-00004660: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00004670: 616c 7565 3d22 3622 206e 616d 653d 226c  alue="6" name="l
-00004680: 696e 655f 7769 6474 6822 2074 7970 653d  ine_width" type=
-00004690: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000046a0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000046b0: 7661 6c75 653d 224d 4d22 206e 616d 653d  value="MM" name=
-000046c0: 226c 696e 655f 7769 6474 685f 756e 6974  "line_width_unit
-000046d0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000046e0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000046f0: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
-00004700: 206e 616d 653d 226f 6666 7365 7422 2074   name="offset" t
-00004710: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00004720: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004730: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
-00004740: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
-00004750: 226f 6666 7365 745f 6d61 705f 756e 6974  "offset_map_unit
-00004760: 5f73 6361 6c65 2220 7479 7065 3d22 5153  _scale" type="QS
-00004770: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00004780: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00004790: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6f66  ue="MM" name="of
-000047a0: 6673 6574 5f75 6e69 7422 2074 7970 653d  fset_unit" type=
-000047b0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000047c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-000047d0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-000047e0: 7269 6e67 5f66 696c 7465 7222 2074 7970  ring_filter" typ
-000047f0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00004800: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00004810: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-00004820: 3d22 7472 696d 5f64 6973 7461 6e63 655f  ="trim_distance_
-00004830: 656e 6422 2074 7970 653d 2251 5374 7269  end" type="QStri
-00004840: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00004850: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00004860: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
-00004870: 206e 616d 653d 2274 7269 6d5f 6469 7374   name="trim_dist
-00004880: 616e 6365 5f65 6e64 5f6d 6170 5f75 6e69  ance_end_map_uni
-00004890: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-000048a0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-000048b0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000048c0: 6c75 653d 224d 4d22 206e 616d 653d 2274  lue="MM" name="t
-000048d0: 7269 6d5f 6469 7374 616e 6365 5f65 6e64  rim_distance_end
-000048e0: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
-000048f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004900: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004910: 653d 2230 2220 6e61 6d65 3d22 7472 696d  e="0" name="trim
-00004920: 5f64 6973 7461 6e63 655f 7374 6172 7422  _distance_start"
-00004930: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004940: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00004950: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
-00004960: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
-00004970: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
-00004980: 5f73 7461 7274 5f6d 6170 5f75 6e69 745f  _start_map_unit_
-00004990: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
-000049a0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000049b0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-000049c0: 653d 224d 4d22 206e 616d 653d 2274 7269  e="MM" name="tri
-000049d0: 6d5f 6469 7374 616e 6365 5f73 7461 7274  m_distance_start
-000049e0: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
-000049f0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-00004a00: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00004a10: 653d 2230 2220 6e61 6d65 3d22 7477 6561  e="0" name="twea
-00004a20: 6b5f 6461 7368 5f70 6174 7465 726e 5f6f  k_dash_pattern_o
-00004a30: 6e5f 636f 726e 6572 7322 2074 7970 653d  n_corners" type=
-00004a40: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00004a50: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00004a60: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
-00004a70: 7573 655f 6375 7374 6f6d 5f64 6173 6822  use_custom_dash"
-00004a80: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
-00004a90: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00004aa0: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
-00004ab0: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
-00004ac0: 653d 2277 6964 7468 5f6d 6170 5f75 6e69  e="width_map_uni
-00004ad0: 745f 7363 616c 6522 2074 7970 653d 2251  t_scale" type="Q
-00004ae0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00004af0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00004b00: 2020 2020 2020 2020 3c64 6174 615f 6465          <data_de
-00004b10: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
-00004b20: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
-00004b30: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
-00004b40: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00004b50: 3c4f 7074 696f 6e20 7661 6c75 653d 2222  <Option value=""
-00004b60: 206e 616d 653d 226e 616d 6522 2074 7970   name="name" typ
-00004b70: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00004b80: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00004b90: 696f 6e20 6e61 6d65 3d22 7072 6f70 6572  ion name="proper
-00004ba0: 7469 6573 222f 3e0a 2020 2020 2020 2020  ties"/>.        
-00004bb0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00004bc0: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
-00004bd0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00004be0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00004bf0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-00004c00: 6f6e 3e0a 2020 2020 2020 2020 2020 3c2f  on>.          </
-00004c10: 6461 7461 5f64 6566 696e 6564 5f70 726f  data_defined_pro
-00004c20: 7065 7274 6965 733e 0a20 2020 2020 2020  perties>.       
-00004c30: 203c 2f6c 6179 6572 3e0a 2020 2020 2020   </layer>.      
-00004c40: 3c2f 7379 6d62 6f6c 3e0a 2020 2020 3c2f  </symbol>.    </
-00004c50: 7379 6d62 6f6c 733e 0a20 203c 2f72 656e  symbols>.  </ren
-00004c60: 6465 7265 722d 7632 3e0a 2020 3c63 7573  derer-v2>.  <cus
-00004c70: 746f 6d70 726f 7065 7274 6965 733e 0a20  tomproperties>. 
-00004c80: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00004c90: 224d 6170 223e 0a20 2020 2020 203c 4f70  "Map">.      <Op
-00004ca0: 7469 6f6e 206e 616d 653d 2264 7561 6c76  tion name="dualv
-00004cb0: 6965 772f 7072 6576 6965 7745 7870 7265  iew/previewExpre
-00004cc0: 7373 696f 6e73 2220 7479 7065 3d22 4c69  ssions" type="Li
-00004cd0: 7374 223e 0a20 2020 2020 2020 203c 4f70  st">.        <Op
-00004ce0: 7469 6f6e 2076 616c 7565 3d22 2671 756f  tion value="&quo
-00004cf0: 743b 7479 7065 2671 756f 743b 2220 7479  t;type&quot;" ty
-00004d00: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
-00004d10: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
-00004d20: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00004d30: 7565 3d22 3022 206e 616d 653d 2265 6d62  ue="0" name="emb
-00004d40: 6564 6465 6457 6964 6765 7473 2f63 6f75  eddedWidgets/cou
-00004d50: 6e74 2220 7479 7065 3d22 696e 7422 2f3e  nt" type="int"/>
-00004d60: 0a20 2020 2020 203c 4f70 7469 6f6e 206e  .      <Option n
-00004d70: 616d 653d 2276 6172 6961 626c 654e 616d  ame="variableNam
-00004d80: 6573 222f 3e0a 2020 2020 2020 3c4f 7074  es"/>.      <Opt
-00004d90: 696f 6e20 6e61 6d65 3d22 7661 7269 6162  ion name="variab
-00004da0: 6c65 5661 6c75 6573 222f 3e0a 2020 2020  leValues"/>.    
-00004db0: 3c2f 4f70 7469 6f6e 3e0a 2020 3c2f 6375  </Option>.  </cu
-00004dc0: 7374 6f6d 7072 6f70 6572 7469 6573 3e0a  stomproperties>.
-00004dd0: 2020 3c62 6c65 6e64 4d6f 6465 3e30 3c2f    <blendMode>0</
-00004de0: 626c 656e 644d 6f64 653e 0a20 203c 6665  blendMode>.  <fe
-00004df0: 6174 7572 6542 6c65 6e64 4d6f 6465 3e30  atureBlendMode>0
-00004e00: 3c2f 6665 6174 7572 6542 6c65 6e64 4d6f  </featureBlendMo
-00004e10: 6465 3e0a 2020 3c6c 6179 6572 4f70 6163  de>.  <layerOpac
-00004e20: 6974 793e 313c 2f6c 6179 6572 4f70 6163  ity>1</layerOpac
-00004e30: 6974 793e 0a20 203c 5369 6e67 6c65 4361  ity>.  <SingleCa
-00004e40: 7465 676f 7279 4469 6167 7261 6d52 656e  tegoryDiagramRen
-00004e50: 6465 7265 7220 6174 7472 6962 7574 654c  derer attributeL
-00004e60: 6567 656e 643d 2231 2220 6469 6167 7261  egend="1" diagra
-00004e70: 6d54 7970 653d 2248 6973 746f 6772 616d  mType="Histogram
-00004e80: 223e 0a20 2020 203c 4469 6167 7261 6d43  ">.    <DiagramC
-00004e90: 6174 6567 6f72 7920 6f70 6163 6974 793d  ategory opacity=
-00004ea0: 2231 2220 6261 636b 6772 6f75 6e64 436f  "1" backgroundCo
-00004eb0: 6c6f 723d 2223 6666 6666 6666 2220 6261  lor="#ffffff" ba
-00004ec0: 7257 6964 7468 3d22 3522 2073 7061 6369  rWidth="5" spaci
-00004ed0: 6e67 556e 6974 5363 616c 653d 2233 783a  ngUnitScale="3x:
-00004ee0: 302c 302c 302c 302c 302c 3022 2073 697a  0,0,0,0,0,0" siz
-00004ef0: 6553 6361 6c65 3d22 3378 3a30 2c30 2c30  eScale="3x:0,0,0
-00004f00: 2c30 2c30 2c30 2220 7065 6e57 6964 7468  ,0,0,0" penWidth
-00004f10: 3d22 3022 2073 697a 6554 7970 653d 224d  ="0" sizeType="M
-00004f20: 4d22 2073 7061 6369 6e67 556e 6974 3d22  M" spacingUnit="
-00004f30: 4d4d 2220 6c69 6e65 5369 7a65 5479 7065  MM" lineSizeType
-00004f40: 3d22 4d4d 2220 7370 6163 696e 673d 2235  ="MM" spacing="5
-00004f50: 2220 6469 7265 6374 696f 6e3d 2230 2220  " direction="0" 
-00004f60: 6d61 7853 6361 6c65 4465 6e6f 6d69 6e61  maxScaleDenomina
-00004f70: 746f 723d 2231 652b 3038 2220 7065 6e41  tor="1e+08" penA
-00004f80: 6c70 6861 3d22 3235 3522 2072 6f74 6174  lpha="255" rotat
-00004f90: 696f 6e4f 6666 7365 743d 2232 3730 2220  ionOffset="270" 
-00004fa0: 656e 6162 6c65 643d 2230 2220 6261 636b  enabled="0" back
-00004fb0: 6772 6f75 6e64 416c 7068 613d 2232 3535  groundAlpha="255
-00004fc0: 2220 6c61 6265 6c50 6c61 6365 6d65 6e74  " labelPlacement
-00004fd0: 4d65 7468 6f64 3d22 5848 6569 6768 7422  Method="XHeight"
-00004fe0: 2064 6961 6772 616d 4f72 6965 6e74 6174   diagramOrientat
-00004ff0: 696f 6e3d 2255 7022 206d 696e 696d 756d  ion="Up" minimum
-00005000: 5369 7a65 3d22 3022 206d 696e 5363 616c  Size="0" minScal
-00005010: 6544 656e 6f6d 696e 6174 6f72 3d22 3022  eDenominator="0"
-00005020: 2073 686f 7741 7869 733d 2231 2220 7363   showAxis="1" sc
-00005030: 616c 6542 6173 6564 5669 7369 6269 6c69  aleBasedVisibili
-00005040: 7479 3d22 3022 2077 6964 7468 3d22 3135  ty="0" width="15
-00005050: 2220 7363 616c 6544 6570 656e 6465 6e63  " scaleDependenc
-00005060: 793d 2241 7265 6122 2068 6569 6768 743d  y="Area" height=
-00005070: 2231 3522 2070 656e 436f 6c6f 723d 2223  "15" penColor="#
-00005080: 3030 3030 3030 2220 6c69 6e65 5369 7a65  000000" lineSize
-00005090: 5363 616c 653d 2233 783a 302c 302c 302c  Scale="3x:0,0,0,
-000050a0: 302c 302c 3022 3e0a 2020 2020 2020 3c66  0,0,0">.      <f
-000050b0: 6f6e 7450 726f 7065 7274 6965 7320 626f  ontProperties bo
-000050c0: 6c64 3d22 3022 2073 7479 6c65 3d22 2220  ld="0" style="" 
-000050d0: 6465 7363 7269 7074 696f 6e3d 224e 6f74  description="Not
-000050e0: 6f20 5361 6e73 2c31 302c 2d31 2c30 2c35  o Sans,10,-1,0,5
-000050f0: 302c 302c 302c 302c 302c 3022 2069 7461  0,0,0,0,0,0" ita
-00005100: 6c69 633d 2230 2220 756e 6465 726c 696e  lic="0" underlin
-00005110: 653d 2230 2220 7374 7269 6b65 7468 726f  e="0" strikethro
-00005120: 7567 683d 2230 222f 3e0a 2020 2020 2020  ugh="0"/>.      
-00005130: 3c61 7474 7269 6275 7465 2063 6f6c 6f72  <attribute color
-00005140: 4f70 6163 6974 793d 2231 2220 6c61 6265  Opacity="1" labe
-00005150: 6c3d 2222 2066 6965 6c64 3d22 2220 636f  l="" field="" co
-00005160: 6c6f 723d 2223 3030 3030 3030 222f 3e0a  lor="#000000"/>.
-00005170: 2020 2020 2020 3c61 7869 7353 796d 626f        <axisSymbo
-00005180: 6c3e 0a20 2020 2020 2020 203c 7379 6d62  l>.        <symb
-00005190: 6f6c 2069 735f 616e 696d 6174 6564 3d22  ol is_animated="
-000051a0: 3022 206e 616d 653d 2222 2074 7970 653d  0" name="" type=
-000051b0: 226c 696e 6522 2061 6c70 6861 3d22 3122  "line" alpha="1"
-000051c0: 2063 6c69 705f 746f 5f65 7874 656e 743d   clip_to_extent=
-000051d0: 2231 2220 666f 7263 655f 7268 723d 2230  "1" force_rhr="0
-000051e0: 2220 6672 616d 655f 7261 7465 3d22 3130  " frame_rate="10
-000051f0: 223e 0a20 2020 2020 2020 2020 203c 6461  ">.          <da
-00005200: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
-00005210: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
-00005220: 2020 203c 4f70 7469 6f6e 2074 7970 653d     <Option type=
-00005230: 224d 6170 223e 0a20 2020 2020 2020 2020  "Map">.         
-00005240: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00005250: 7565 3d22 2220 6e61 6d65 3d22 6e61 6d65  ue="" name="name
-00005260: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00005270: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00005280: 203c 4f70 7469 6f6e 206e 616d 653d 2270   <Option name="p
-00005290: 726f 7065 7274 6965 7322 2f3e 0a20 2020  roperties"/>.   
-000052a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000052b0: 6f6e 2076 616c 7565 3d22 636f 6c6c 6563  on value="collec
-000052c0: 7469 6f6e 2220 6e61 6d65 3d22 7479 7065  tion" name="type
-000052d0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-000052e0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
-000052f0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
-00005300: 2020 203c 2f64 6174 615f 6465 6669 6e65     </data_define
-00005310: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
-00005320: 2020 2020 2020 2020 3c6c 6179 6572 206c          <layer l
-00005330: 6f63 6b65 643d 2230 2220 636c 6173 733d  ocked="0" class=
-00005340: 2253 696d 706c 654c 696e 6522 2070 6173  "SimpleLine" pas
-00005350: 733d 2230 2220 656e 6162 6c65 643d 2231  s="0" enabled="1
-00005360: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-00005370: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
-00005380: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00005390: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-000053a0: 3022 206e 616d 653d 2261 6c69 676e 5f64  0" name="align_d
-000053b0: 6173 685f 7061 7474 6572 6e22 2074 7970  ash_pattern" typ
-000053c0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-000053d0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-000053e0: 696f 6e20 7661 6c75 653d 2273 7175 6172  ion value="squar
-000053f0: 6522 206e 616d 653d 2263 6170 7374 796c  e" name="capstyl
-00005400: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
-00005410: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005420: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00005430: 2235 3b32 2220 6e61 6d65 3d22 6375 7374  "5;2" name="cust
-00005440: 6f6d 6461 7368 2220 7479 7065 3d22 5153  omdash" type="QS
-00005450: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-00005460: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-00005470: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
-00005480: 2c30 2c30 2220 6e61 6d65 3d22 6375 7374  ,0,0" name="cust
-00005490: 6f6d 6461 7368 5f6d 6170 5f75 6e69 745f  omdash_map_unit_
-000054a0: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
-000054b0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
-000054c0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-000054d0: 6c75 653d 224d 4d22 206e 616d 653d 2263  lue="MM" name="c
-000054e0: 7573 746f 6d64 6173 685f 756e 6974 2220  ustomdash_unit" 
-000054f0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
-00005500: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00005510: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
-00005520: 206e 616d 653d 2264 6173 685f 7061 7474   name="dash_patt
-00005530: 6572 6e5f 6f66 6673 6574 2220 7479 7065  ern_offset" type
-00005540: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-00005550: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-00005560: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
-00005570: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
-00005580: 6461 7368 5f70 6174 7465 726e 5f6f 6666  dash_pattern_off
-00005590: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
-000055a0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
-000055b0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
-000055c0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
-000055d0: 3d22 4d4d 2220 6e61 6d65 3d22 6461 7368  ="MM" name="dash
-000055e0: 5f70 6174 7465 726e 5f6f 6666 7365 745f  _pattern_offset_
-000055f0: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
-00005600: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00005610: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00005620: 7565 3d22 3022 206e 616d 653d 2264 7261  ue="0" name="dra
-00005630: 775f 696e 7369 6465 5f70 6f6c 7967 6f6e  w_inside_polygon
-00005640: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
-00005650: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
-00005660: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
-00005670: 6265 7665 6c22 206e 616d 653d 226a 6f69  bevel" name="joi
-00005680: 6e73 7479 6c65 2220 7479 7065 3d22 5153  nstyle" type="QS
-00005690: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
-000056a0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
-000056b0: 616c 7565 3d22 3335 2c33 352c 3335 2c32  alue="35,35,35,2
-000056c0: 3535 2220 6e61 6d65 3d22 6c69 6e65 5f63  55" name="line_c
-000056d0: 6f6c 6f72 2220 7479 7065 3d22 5153 7472  olor" type="QStr
-000056e0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-000056f0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00005700: 7565 3d22 736f 6c69 6422 206e 616d 653d  ue="solid" name=
-00005710: 226c 696e 655f 7374 796c 6522 2074 7970  "line_style" typ
-00005720: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00005730: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00005740: 696f 6e20 7661 6c75 653d 2230 2e32 3622  ion value="0.26"
-00005750: 206e 616d 653d 226c 696e 655f 7769 6474   name="line_widt
-00005760: 6822 2074 7970 653d 2251 5374 7269 6e67  h" type="QString
-00005770: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005780: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00005790: 224d 4d22 206e 616d 653d 226c 696e 655f  "MM" name="line_
-000057a0: 7769 6474 685f 756e 6974 2220 7479 7065  width_unit" type
-000057b0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
-000057c0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
-000057d0: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
-000057e0: 653d 226f 6666 7365 7422 2074 7970 653d  e="offset" type=
-000057f0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00005800: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005810: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-00005820: 302c 302c 302c 3022 206e 616d 653d 226f  0,0,0,0" name="o
-00005830: 6666 7365 745f 6d61 705f 756e 6974 5f73  ffset_map_unit_s
-00005840: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
-00005850: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
-00005860: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
-00005870: 7565 3d22 4d4d 2220 6e61 6d65 3d22 6f66  ue="MM" name="of
-00005880: 6673 6574 5f75 6e69 7422 2074 7970 653d  fset_unit" type=
-00005890: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-000058a0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-000058b0: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-000058c0: 3d22 7269 6e67 5f66 696c 7465 7222 2074  ="ring_filter" t
-000058d0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000058e0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000058f0: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-00005900: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00005910: 6e63 655f 656e 6422 2074 7970 653d 2251  nce_end" type="Q
-00005920: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00005930: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00005940: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
-00005950: 302c 302c 3022 206e 616d 653d 2274 7269  0,0,0" name="tri
-00005960: 6d5f 6469 7374 616e 6365 5f65 6e64 5f6d  m_distance_end_m
-00005970: 6170 5f75 6e69 745f 7363 616c 6522 2074  ap_unit_scale" t
-00005980: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-00005990: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000059a0: 7074 696f 6e20 7661 6c75 653d 224d 4d22  ption value="MM"
-000059b0: 206e 616d 653d 2274 7269 6d5f 6469 7374   name="trim_dist
-000059c0: 616e 6365 5f65 6e64 5f75 6e69 7422 2074  ance_end_unit" t
-000059d0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
-000059e0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
-000059f0: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
-00005a00: 6e61 6d65 3d22 7472 696d 5f64 6973 7461  name="trim_dista
-00005a10: 6e63 655f 7374 6172 7422 2074 7970 653d  nce_start" type=
-00005a20: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00005a30: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005a40: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
-00005a50: 302c 302c 302c 3022 206e 616d 653d 2274  0,0,0,0" name="t
-00005a60: 7269 6d5f 6469 7374 616e 6365 5f73 7461  rim_distance_sta
-00005a70: 7274 5f6d 6170 5f75 6e69 745f 7363 616c  rt_map_unit_scal
-00005a80: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
-00005a90: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005aa0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00005ab0: 224d 4d22 206e 616d 653d 2274 7269 6d5f  "MM" name="trim_
-00005ac0: 6469 7374 616e 6365 5f73 7461 7274 5f75  distance_start_u
-00005ad0: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
-00005ae0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
-00005af0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
-00005b00: 653d 2230 2220 6e61 6d65 3d22 7477 6561  e="0" name="twea
-00005b10: 6b5f 6461 7368 5f70 6174 7465 726e 5f6f  k_dash_pattern_o
-00005b20: 6e5f 636f 726e 6572 7322 2074 7970 653d  n_corners" type=
-00005b30: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
-00005b40: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005b50: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
-00005b60: 3d22 7573 655f 6375 7374 6f6d 5f64 6173  ="use_custom_das
-00005b70: 6822 2074 7970 653d 2251 5374 7269 6e67  h" type="QString
-00005b80: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
-00005b90: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
-00005ba0: 2233 783a 302c 302c 302c 302c 302c 3022  "3x:0,0,0,0,0,0"
-00005bb0: 206e 616d 653d 2277 6964 7468 5f6d 6170   name="width_map
-00005bc0: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
-00005bd0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00005be0: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
-00005bf0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-00005c00: 3c64 6174 615f 6465 6669 6e65 645f 7072  <data_defined_pr
-00005c10: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00005c20: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
-00005c30: 7479 7065 3d22 4d61 7022 3e0a 2020 2020  type="Map">.    
-00005c40: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
-00005c50: 696f 6e20 7661 6c75 653d 2222 206e 616d  ion value="" nam
-00005c60: 653d 226e 616d 6522 2074 7970 653d 2251  e="name" type="Q
-00005c70: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00005c80: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
-00005c90: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
-00005ca0: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
-00005cb0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00005cc0: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
-00005cd0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00005ce0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00005cf0: 2020 2020 2020 2020 2020 2020 3c2f 4f70              </Op
-00005d00: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00005d10: 2020 3c2f 6461 7461 5f64 6566 696e 6564    </data_defined
-00005d20: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
-00005d30: 2020 2020 2020 203c 2f6c 6179 6572 3e0a         </layer>.
-00005d40: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-00005d50: 3e0a 2020 2020 2020 3c2f 6178 6973 5379  >.      </axisSy
-00005d60: 6d62 6f6c 3e0a 2020 2020 3c2f 4469 6167  mbol>.    </Diag
-00005d70: 7261 6d43 6174 6567 6f72 793e 0a20 203c  ramCategory>.  <
-00005d80: 2f53 696e 676c 6543 6174 6567 6f72 7944  /SingleCategoryD
-00005d90: 6961 6772 616d 5265 6e64 6572 6572 3e0a  iagramRenderer>.
-00005da0: 2020 3c44 6961 6772 616d 4c61 7965 7253    <DiagramLayerS
-00005db0: 6574 7469 6e67 7320 706c 6163 656d 656e  ettings placemen
-00005dc0: 743d 2232 2220 6c69 6e65 506c 6163 656d  t="2" linePlacem
-00005dd0: 656e 7446 6c61 6773 3d22 3138 2220 6f62  entFlags="18" ob
-00005de0: 7374 6163 6c65 3d22 3022 2070 7269 6f72  stacle="0" prior
-00005df0: 6974 793d 2230 2220 7a49 6e64 6578 3d22  ity="0" zIndex="
-00005e00: 3022 2073 686f 7741 6c6c 3d22 3122 2064  0" showAll="1" d
-00005e10: 6973 743d 2230 223e 0a20 2020 203c 7072  ist="0">.    <pr
-00005e20: 6f70 6572 7469 6573 3e0a 2020 2020 2020  operties>.      
-00005e30: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
-00005e40: 7022 3e0a 2020 2020 2020 2020 3c4f 7074  p">.        <Opt
-00005e50: 696f 6e20 7661 6c75 653d 2222 206e 616d  ion value="" nam
-00005e60: 653d 226e 616d 6522 2074 7970 653d 2251  e="name" type="Q
-00005e70: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
-00005e80: 2020 3c4f 7074 696f 6e20 6e61 6d65 3d22    <Option name="
-00005e90: 7072 6f70 6572 7469 6573 222f 3e0a 2020  properties"/>.  
-00005ea0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
-00005eb0: 6c75 653d 2263 6f6c 6c65 6374 696f 6e22  lue="collection"
-00005ec0: 206e 616d 653d 2274 7970 6522 2074 7970   name="type" typ
-00005ed0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
-00005ee0: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
-00005ef0: 2020 3c2f 7072 6f70 6572 7469 6573 3e0a    </properties>.
-00005f00: 2020 3c2f 4469 6167 7261 6d4c 6179 6572    </DiagramLayer
-00005f10: 5365 7474 696e 6773 3e0a 2020 3c67 656f  Settings>.  <geo
-00005f20: 6d65 7472 794f 7074 696f 6e73 2067 656f  metryOptions geo
-00005f30: 6d65 7472 7950 7265 6369 7369 6f6e 3d22  metryPrecision="
-00005f40: 3022 2072 656d 6f76 6544 7570 6c69 6361  0" removeDuplica
-00005f50: 7465 4e6f 6465 733d 2230 223e 0a20 2020  teNodes="0">.   
-00005f60: 203c 6163 7469 7665 4368 6563 6b73 2f3e   <activeChecks/>
-00005f70: 0a20 2020 203c 6368 6563 6b43 6f6e 6669  .    <checkConfi
-00005f80: 6775 7261 7469 6f6e 2f3e 0a20 203c 2f67  guration/>.  </g
-00005f90: 656f 6d65 7472 794f 7074 696f 6e73 3e0a  eometryOptions>.
-00005fa0: 2020 3c6c 6567 656e 6420 7479 7065 3d22    <legend type="
-00005fb0: 6465 6661 756c 742d 7665 6374 6f72 2220  default-vector" 
-00005fc0: 7368 6f77 4c61 6265 6c4c 6567 656e 643d  showLabelLegend=
-00005fd0: 2230 222f 3e0a 2020 3c72 6566 6572 656e  "0"/>.  <referen
-00005fe0: 6365 644c 6179 6572 732f 3e0a 2020 3c66  cedLayers/>.  <f
-00005ff0: 6965 6c64 436f 6e66 6967 7572 6174 696f  ieldConfiguratio
-00006000: 6e3e 0a20 2020 203c 6669 656c 6420 6e61  n>.    <field na
-00006010: 6d65 3d22 7479 7065 2220 636f 6e66 6967  me="type" config
-00006020: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
-00006030: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
-00006040: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
-00006050: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
-00006060: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
-00006070: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
-00006080: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
-00006090: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
-000060a0: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
-000060b0: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-000060c0: 226f 736d 5f69 6422 2063 6f6e 6669 6775  "osm_id" configu
-000060d0: 7261 7469 6f6e 466c 6167 733d 224e 6f6e  rationFlags="Non
-000060e0: 6522 3e0a 2020 2020 2020 3c65 6469 7457  e">.      <editW
-000060f0: 6964 6765 7420 7479 7065 3d22 5465 7874  idget type="Text
-00006100: 4564 6974 223e 0a20 2020 2020 2020 203c  Edit">.        <
-00006110: 636f 6e66 6967 3e0a 2020 2020 2020 2020  config>.        
-00006120: 2020 3c4f 7074 696f 6e2f 3e0a 2020 2020    <Option/>.    
-00006130: 2020 2020 3c2f 636f 6e66 6967 3e0a 2020      </config>.  
-00006140: 2020 2020 3c2f 6564 6974 5769 6467 6574      </editWidget
-00006150: 3e0a 2020 2020 3c2f 6669 656c 643e 0a20  >.    </field>. 
-00006160: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
-00006170: 6f72 6965 6e74 6174 696f 6e22 2063 6f6e  orientation" con
-00006180: 6669 6775 7261 7469 6f6e 466c 6167 733d  figurationFlags=
-00006190: 224e 6f6e 6522 3e0a 2020 2020 2020 3c65  "None">.      <e
-000061a0: 6469 7457 6964 6765 7420 7479 7065 3d22  ditWidget type="
-000061b0: 5465 7874 4564 6974 223e 0a20 2020 2020  TextEdit">.     
-000061c0: 2020 203c 636f 6e66 6967 3e0a 2020 2020     <config>.    
-000061d0: 2020 2020 2020 3c4f 7074 696f 6e2f 3e0a        <Option/>.
-000061e0: 2020 2020 2020 2020 3c2f 636f 6e66 6967          </config
-000061f0: 3e0a 2020 2020 2020 3c2f 6564 6974 5769  >.      </editWi
-00006200: 6467 6574 3e0a 2020 2020 3c2f 6669 656c  dget>.    </fiel
-00006210: 643e 0a20 2020 203c 6669 656c 6420 6e61  d>.    <field na
-00006220: 6d65 3d22 6f72 6965 6e74 6174 696f 6e5f  me="orientation_
-00006230: 636f 6e66 6964 656e 6365 2220 636f 6e66  confidence" conf
-00006240: 6967 7572 6174 696f 6e46 6c61 6773 3d22  igurationFlags="
-00006250: 4e6f 6e65 223e 0a20 2020 2020 203c 6564  None">.      <ed
-00006260: 6974 5769 6467 6574 2074 7970 653d 2254  itWidget type="T
-00006270: 6578 7445 6469 7422 3e0a 2020 2020 2020  extEdit">.      
-00006280: 2020 3c63 6f6e 6669 673e 0a20 2020 2020    <config>.     
-00006290: 2020 2020 203c 4f70 7469 6f6e 2f3e 0a20       <Option/>. 
-000062a0: 2020 2020 2020 203c 2f63 6f6e 6669 673e         </config>
-000062b0: 0a20 2020 2020 203c 2f65 6469 7457 6964  .      </editWid
-000062c0: 6765 743e 0a20 2020 203c 2f66 6965 6c64  get>.    </field
-000062d0: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
-000062e0: 653d 2261 6e67 6c65 2220 636f 6e66 6967  e="angle" config
-000062f0: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
-00006300: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
-00006310: 5769 6467 6574 2074 7970 653d 2252 616e  Widget type="Ran
-00006320: 6765 223e 0a20 2020 2020 2020 203c 636f  ge">.        <co
-00006330: 6e66 6967 3e0a 2020 2020 2020 2020 2020  nfig>.          
-00006340: 3c4f 7074 696f 6e2f 3e0a 2020 2020 2020  <Option/>.      
-00006350: 2020 3c2f 636f 6e66 6967 3e0a 2020 2020    </config>.    
-00006360: 2020 3c2f 6564 6974 5769 6467 6574 3e0a    </editWidget>.
-00006370: 2020 2020 3c2f 6669 656c 643e 0a20 203c      </field>.  <
-00006380: 2f66 6965 6c64 436f 6e66 6967 7572 6174  /fieldConfigurat
-00006390: 696f 6e3e 0a20 203c 616c 6961 7365 733e  ion>.  <aliases>
-000063a0: 0a20 2020 203c 616c 6961 7320 696e 6465  .    <alias inde
-000063b0: 783d 2230 2220 6e61 6d65 3d22 2220 6669  x="0" name="" fi
-000063c0: 656c 643d 2274 7970 6522 2f3e 0a20 2020  eld="type"/>.   
-000063d0: 203c 616c 6961 7320 696e 6465 783d 2231   <alias index="1
-000063e0: 2220 6e61 6d65 3d22 2220 6669 656c 643d  " name="" field=
-000063f0: 226f 736d 5f69 6422 2f3e 0a20 2020 203c  "osm_id"/>.    <
-00006400: 616c 6961 7320 696e 6465 783d 2232 2220  alias index="2" 
-00006410: 6e61 6d65 3d22 2220 6669 656c 643d 226f  name="" field="o
-00006420: 7269 656e 7461 7469 6f6e 222f 3e0a 2020  rientation"/>.  
-00006430: 2020 3c61 6c69 6173 2069 6e64 6578 3d22    <alias index="
-00006440: 3322 206e 616d 653d 2222 2066 6965 6c64  3" name="" field
-00006450: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
-00006460: 6e66 6964 656e 6365 222f 3e0a 2020 2020  nfidence"/>.    
-00006470: 3c61 6c69 6173 2069 6e64 6578 3d22 3422  <alias index="4"
-00006480: 206e 616d 653d 2222 2066 6965 6c64 3d22   name="" field="
-00006490: 616e 676c 6522 2f3e 0a20 203c 2f61 6c69  angle"/>.  </ali
-000064a0: 6173 6573 3e0a 2020 3c64 6566 6175 6c74  ases>.  <default
-000064b0: 733e 0a20 2020 203c 6465 6661 756c 7420  s>.    <default 
-000064c0: 6578 7072 6573 7369 6f6e 3d22 2220 6170  expression="" ap
-000064d0: 706c 794f 6e55 7064 6174 653d 2230 2220  plyOnUpdate="0" 
-000064e0: 6669 656c 643d 2274 7970 6522 2f3e 0a20  field="type"/>. 
-000064f0: 2020 203c 6465 6661 756c 7420 6578 7072     <default expr
-00006500: 6573 7369 6f6e 3d22 2220 6170 706c 794f  ession="" applyO
-00006510: 6e55 7064 6174 653d 2230 2220 6669 656c  nUpdate="0" fiel
-00006520: 643d 226f 736d 5f69 6422 2f3e 0a20 2020  d="osm_id"/>.   
-00006530: 203c 6465 6661 756c 7420 6578 7072 6573   <default expres
-00006540: 7369 6f6e 3d22 2220 6170 706c 794f 6e55  sion="" applyOnU
-00006550: 7064 6174 653d 2230 2220 6669 656c 643d  pdate="0" field=
-00006560: 226f 7269 656e 7461 7469 6f6e 222f 3e0a  "orientation"/>.
-00006570: 2020 2020 3c64 6566 6175 6c74 2065 7870      <default exp
-00006580: 7265 7373 696f 6e3d 2222 2061 7070 6c79  ression="" apply
-00006590: 4f6e 5570 6461 7465 3d22 3022 2066 6965  OnUpdate="0" fie
-000065a0: 6c64 3d22 6f72 6965 6e74 6174 696f 6e5f  ld="orientation_
-000065b0: 636f 6e66 6964 656e 6365 222f 3e0a 2020  confidence"/>.  
-000065c0: 2020 3c64 6566 6175 6c74 2065 7870 7265    <default expre
-000065d0: 7373 696f 6e3d 2222 2061 7070 6c79 4f6e  ssion="" applyOn
-000065e0: 5570 6461 7465 3d22 3022 2066 6965 6c64  Update="0" field
-000065f0: 3d22 616e 676c 6522 2f3e 0a20 203c 2f64  ="angle"/>.  </d
-00006600: 6566 6175 6c74 733e 0a20 203c 636f 6e73  efaults>.  <cons
-00006610: 7472 6169 6e74 733e 0a20 2020 203c 636f  traints>.    <co
-00006620: 6e73 7472 6169 6e74 2063 6f6e 7374 7261  nstraint constra
-00006630: 696e 7473 3d22 3022 2075 6e69 7175 655f  ints="0" unique_
-00006640: 7374 7265 6e67 7468 3d22 3022 2065 7870  strength="0" exp
-00006650: 5f73 7472 656e 6774 683d 2230 2220 6e6f  _strength="0" no
-00006660: 746e 756c 6c5f 7374 7265 6e67 7468 3d22  tnull_strength="
-00006670: 3022 2066 6965 6c64 3d22 7479 7065 222f  0" field="type"/
-00006680: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
-00006690: 7420 636f 6e73 7472 6169 6e74 733d 2230  t constraints="0
-000066a0: 2220 756e 6971 7565 5f73 7472 656e 6774  " unique_strengt
-000066b0: 683d 2230 2220 6578 705f 7374 7265 6e67  h="0" exp_streng
-000066c0: 7468 3d22 3022 206e 6f74 6e75 6c6c 5f73  th="0" notnull_s
-000066d0: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
-000066e0: 643d 226f 736d 5f69 6422 2f3e 0a20 2020  d="osm_id"/>.   
-000066f0: 203c 636f 6e73 7472 6169 6e74 2063 6f6e   <constraint con
-00006700: 7374 7261 696e 7473 3d22 3022 2075 6e69  straints="0" uni
-00006710: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
-00006720: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
-00006730: 2220 6e6f 746e 756c 6c5f 7374 7265 6e67  " notnull_streng
-00006740: 7468 3d22 3022 2066 6965 6c64 3d22 6f72  th="0" field="or
-00006750: 6965 6e74 6174 696f 6e22 2f3e 0a20 2020  ientation"/>.   
-00006760: 203c 636f 6e73 7472 6169 6e74 2063 6f6e   <constraint con
-00006770: 7374 7261 696e 7473 3d22 3022 2075 6e69  straints="0" uni
-00006780: 7175 655f 7374 7265 6e67 7468 3d22 3022  que_strength="0"
-00006790: 2065 7870 5f73 7472 656e 6774 683d 2230   exp_strength="0
-000067a0: 2220 6e6f 746e 756c 6c5f 7374 7265 6e67  " notnull_streng
-000067b0: 7468 3d22 3022 2066 6965 6c64 3d22 6f72  th="0" field="or
-000067c0: 6965 6e74 6174 696f 6e5f 636f 6e66 6964  ientation_confid
-000067d0: 656e 6365 222f 3e0a 2020 2020 3c63 6f6e  ence"/>.    <con
-000067e0: 7374 7261 696e 7420 636f 6e73 7472 6169  straint constrai
-000067f0: 6e74 733d 2230 2220 756e 6971 7565 5f73  nts="0" unique_s
-00006800: 7472 656e 6774 683d 2230 2220 6578 705f  trength="0" exp_
-00006810: 7374 7265 6e67 7468 3d22 3022 206e 6f74  strength="0" not
-00006820: 6e75 6c6c 5f73 7472 656e 6774 683d 2230  null_strength="0
-00006830: 2220 6669 656c 643d 2261 6e67 6c65 222f  " field="angle"/
-00006840: 3e0a 2020 3c2f 636f 6e73 7472 6169 6e74  >.  </constraint
-00006850: 733e 0a20 203c 636f 6e73 7472 6169 6e74  s>.  <constraint
-00006860: 4578 7072 6573 7369 6f6e 733e 0a20 2020  Expressions>.   
-00006870: 203c 636f 6e73 7472 6169 6e74 2066 6965   <constraint fie
-00006880: 6c64 3d22 7479 7065 2220 6578 703d 2222  ld="type" exp=""
-00006890: 2064 6573 633d 2222 2f3e 0a20 2020 203c   desc=""/>.    <
-000068a0: 636f 6e73 7472 6169 6e74 2066 6965 6c64  constraint field
-000068b0: 3d22 6f73 6d5f 6964 2220 6578 703d 2222  ="osm_id" exp=""
-000068c0: 2064 6573 633d 2222 2f3e 0a20 2020 203c   desc=""/>.    <
-000068d0: 636f 6e73 7472 6169 6e74 2066 6965 6c64  constraint field
-000068e0: 3d22 6f72 6965 6e74 6174 696f 6e22 2065  ="orientation" e
-000068f0: 7870 3d22 2220 6465 7363 3d22 222f 3e0a  xp="" desc=""/>.
-00006900: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
-00006910: 6669 656c 643d 226f 7269 656e 7461 7469  field="orientati
-00006920: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2065  on_confidence" e
-00006930: 7870 3d22 2220 6465 7363 3d22 222f 3e0a  xp="" desc=""/>.
-00006940: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
-00006950: 6669 656c 643d 2261 6e67 6c65 2220 6578  field="angle" ex
-00006960: 703d 2222 2064 6573 633d 2222 2f3e 0a20  p="" desc=""/>. 
-00006970: 203c 2f63 6f6e 7374 7261 696e 7445 7870   </constraintExp
-00006980: 7265 7373 696f 6e73 3e0a 2020 3c65 7870  ressions>.  <exp
-00006990: 7265 7373 696f 6e66 6965 6c64 732f 3e0a  ressionfields/>.
-000069a0: 2020 3c61 7474 7269 6275 7465 6163 7469    <attributeacti
-000069b0: 6f6e 733e 0a20 2020 203c 6465 6661 756c  ons>.    <defaul
-000069c0: 7441 6374 696f 6e20 6b65 793d 2243 616e  tAction key="Can
-000069d0: 7661 7322 2076 616c 7565 3d22 7b30 3030  vas" value="{000
-000069e0: 3030 3030 302d 3030 3030 2d30 3030 302d  00000-0000-0000-
-000069f0: 3030 3030 2d30 3030 3030 3030 3030 3030  0000-00000000000
-00006a00: 307d 222f 3e0a 2020 3c2f 6174 7472 6962  0}"/>.  </attrib
-00006a10: 7574 6561 6374 696f 6e73 3e0a 2020 3c61  uteactions>.  <a
-00006a20: 7474 7269 6275 7465 7461 626c 6563 6f6e  ttributetablecon
-00006a30: 6669 6720 6163 7469 6f6e 5769 6467 6574  fig actionWidget
-00006a40: 5374 796c 653d 2264 726f 7044 6f77 6e22  Style="dropDown"
-00006a50: 2073 6f72 744f 7264 6572 3d22 3022 2073   sortOrder="0" s
-00006a60: 6f72 7445 7870 7265 7373 696f 6e3d 2222  ortExpression=""
-00006a70: 3e0a 2020 2020 3c63 6f6c 756d 6e73 3e0a  >.    <columns>.
-00006a80: 2020 2020 2020 3c63 6f6c 756d 6e20 6e61        <column na
-00006a90: 6d65 3d22 7479 7065 2220 7479 7065 3d22  me="type" type="
-00006aa0: 6669 656c 6422 2068 6964 6465 6e3d 2230  field" hidden="0
-00006ab0: 2220 7769 6474 683d 2233 3737 222f 3e0a  " width="377"/>.
-00006ac0: 2020 2020 2020 3c63 6f6c 756d 6e20 6e61        <column na
-00006ad0: 6d65 3d22 6f73 6d5f 6964 2220 7479 7065  me="osm_id" type
-00006ae0: 3d22 6669 656c 6422 2068 6964 6465 6e3d  ="field" hidden=
-00006af0: 2230 2220 7769 6474 683d 222d 3122 2f3e  "0" width="-1"/>
-00006b00: 0a20 2020 2020 203c 636f 6c75 6d6e 206e  .      <column n
-00006b10: 616d 653d 226f 7269 656e 7461 7469 6f6e  ame="orientation
-00006b20: 2220 7479 7065 3d22 6669 656c 6422 2068  " type="field" h
-00006b30: 6964 6465 6e3d 2230 2220 7769 6474 683d  idden="0" width=
-00006b40: 222d 3122 2f3e 0a20 2020 2020 203c 636f  "-1"/>.      <co
-00006b50: 6c75 6d6e 206e 616d 653d 226f 7269 656e  lumn name="orien
-00006b60: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
-00006b70: 6522 2074 7970 653d 2266 6965 6c64 2220  e" type="field" 
-00006b80: 6869 6464 656e 3d22 3022 2077 6964 7468  hidden="0" width
-00006b90: 3d22 2d31 222f 3e0a 2020 2020 2020 3c63  ="-1"/>.      <c
-00006ba0: 6f6c 756d 6e20 6e61 6d65 3d22 616e 676c  olumn name="angl
-00006bb0: 6522 2074 7970 653d 2266 6965 6c64 2220  e" type="field" 
-00006bc0: 6869 6464 656e 3d22 3022 2077 6964 7468  hidden="0" width
-00006bd0: 3d22 2d31 222f 3e0a 2020 2020 2020 3c63  ="-1"/>.      <c
-00006be0: 6f6c 756d 6e20 7479 7065 3d22 6163 7469  olumn type="acti
-00006bf0: 6f6e 7322 2068 6964 6465 6e3d 2231 2220  ons" hidden="1" 
-00006c00: 7769 6474 683d 222d 3122 2f3e 0a20 2020  width="-1"/>.   
-00006c10: 203c 2f63 6f6c 756d 6e73 3e0a 2020 3c2f   </columns>.  </
-00006c20: 6174 7472 6962 7574 6574 6162 6c65 636f  attributetableco
-00006c30: 6e66 6967 3e0a 2020 3c63 6f6e 6469 7469  nfig>.  <conditi
-00006c40: 6f6e 616c 7374 796c 6573 3e0a 2020 2020  onalstyles>.    
-00006c50: 3c72 6f77 7374 796c 6573 2f3e 0a20 2020  <rowstyles/>.   
-00006c60: 203c 6669 656c 6473 7479 6c65 732f 3e0a   <fieldstyles/>.
-00006c70: 2020 3c2f 636f 6e64 6974 696f 6e61 6c73    </conditionals
-00006c80: 7479 6c65 733e 0a20 203c 7374 6f72 6564  tyles>.  <stored
-00006c90: 6578 7072 6573 7369 6f6e 732f 3e0a 2020  expressions/>.  
-00006ca0: 3c65 6469 7466 6f72 6d20 746f 6c65 7261  <editform tolera
-00006cb0: 6e74 3d22 3122 3e3c 2f65 6469 7466 6f72  nt="1"></editfor
-00006cc0: 6d3e 0a20 203c 6564 6974 666f 726d 696e  m>.  <editformin
-00006cd0: 6974 2f3e 0a20 203c 6564 6974 666f 726d  it/>.  <editform
-00006ce0: 696e 6974 636f 6465 736f 7572 6365 3e30  initcodesource>0
-00006cf0: 3c2f 6564 6974 666f 726d 696e 6974 636f  </editforminitco
-00006d00: 6465 736f 7572 6365 3e0a 2020 3c65 6469  desource>.  <edi
-00006d10: 7466 6f72 6d69 6e69 7466 696c 6570 6174  tforminitfilepat
-00006d20: 683e 3c2f 6564 6974 666f 726d 696e 6974  h></editforminit
-00006d30: 6669 6c65 7061 7468 3e0a 2020 3c65 6469  filepath>.  <edi
-00006d40: 7466 6f72 6d69 6e69 7463 6f64 653e 3c21  tforminitcode><!
-00006d50: 5b43 4441 5441 5b23 202d 2a2d 2063 6f64  [CDATA[# -*- cod
-00006d60: 696e 673a 2075 7466 2d38 202d 2a2d 0a22  ing: utf-8 -*-."
-00006d70: 2222 0a4c 6573 2066 6f72 6d75 6c61 6972  "".Les formulair
-00006d80: 6573 2051 4749 5320 7065 7576 656e 7420  es QGIS peuvent 
-00006d90: 6176 6f69 7220 756e 6520 666f 6e63 7469  avoir une foncti
-00006da0: 6f6e 2050 7974 686f 6e20 7175 6920 6573  on Python qui es
-00006db0: 7420 6170 7065 6cc3 a965 206c 6f72 7371  t appel..e lorsq
-00006dc0: 7565 206c 6520 666f 726d 756c 6169 7265  ue le formulaire
-00006dd0: 2065 7374 0a6f 7576 6572 742e 0a0a 5574   est.ouvert...Ut
-00006de0: 696c 6973 657a 2063 6574 7465 2066 6f6e  ilisez cette fon
-00006df0: 6374 696f 6e20 706f 7572 2061 6a6f 7574  ction pour ajout
-00006e00: 6572 2075 6e65 206c 6f67 6971 7565 2073  er une logique s
-00006e10: 7570 706c c3a9 6d65 6e74 6169 7265 20c3  uppl..mentaire .
-00006e20: a020 766f 7320 666f 726d 756c 6169 7265  . vos formulaire
-00006e30: 732e 0a0a 456e 7472 657a 206c 6520 6e6f  s...Entrez le no
-00006e40: 6d20 6465 206c 6120 666f 6e63 7469 6f6e  m de la fonction
-00006e50: 2064 616e 7320 6c65 2063 6861 6d70 200a   dans le champ .
-00006e60: 2246 6f6e 6374 696f 6e20 6427 696e 6974  "Fonction d'init
-00006e70: 6961 6c69 7361 7469 6f6e 2050 7974 686f  ialisation Pytho
-00006e80: 6e22 2e0a 566f 6963 6920 756e 2065 7865  n"..Voici un exe
-00006e90: 6d70 6c65 3a0a 2222 220a 6672 6f6d 2071  mple:.""".from q
-00006ea0: 6769 732e 5079 5174 2e51 7457 6964 6765  gis.PyQt.QtWidge
-00006eb0: 7473 2069 6d70 6f72 7420 5157 6964 6765  ts import QWidge
-00006ec0: 740a 0a64 6566 206d 795f 666f 726d 5f6f  t..def my_form_o
-00006ed0: 7065 6e28 6469 616c 6f67 2c20 6c61 7965  pen(dialog, laye
-00006ee0: 722c 2066 6561 7475 7265 293a 0a20 2020  r, feature):.   
-00006ef0: 2067 656f 6d20 3d20 6665 6174 7572 652e   geom = feature.
-00006f00: 6765 6f6d 6574 7279 2829 0a20 2020 2063  geometry().    c
-00006f10: 6f6e 7472 6f6c 203d 2064 6961 6c6f 672e  ontrol = dialog.
-00006f20: 6669 6e64 4368 696c 6428 5157 6964 6765  findChild(QWidge
-00006f30: 742c 2022 4d79 4c69 6e65 4564 6974 2229  t, "MyLineEdit")
-00006f40: 0a5d 5d3e 3c2f 6564 6974 666f 726d 696e  .]]></editformin
-00006f50: 6974 636f 6465 3e0a 2020 3c66 6561 7466  itcode>.  <featf
-00006f60: 6f72 6d73 7570 7072 6573 733e 303c 2f66  ormsuppress>0</f
-00006f70: 6561 7466 6f72 6d73 7570 7072 6573 733e  eatformsuppress>
-00006f80: 0a20 203c 6564 6974 6f72 6c61 796f 7574  .  <editorlayout
-00006f90: 3e67 656e 6572 6174 6564 6c61 796f 7574  >generatedlayout
-00006fa0: 3c2f 6564 6974 6f72 6c61 796f 7574 3e0a  </editorlayout>.
-00006fb0: 2020 3c65 6469 7461 626c 653e 0a20 2020    <editable>.   
-00006fc0: 203c 6669 656c 6420 6564 6974 6162 6c65   <field editable
-00006fd0: 3d22 3122 206e 616d 653d 2261 6e67 6c65  ="1" name="angle
-00006fe0: 222f 3e0a 2020 2020 3c66 6965 6c64 2065  "/>.    <field e
-00006ff0: 6469 7461 626c 653d 2231 2220 6e61 6d65  ditable="1" name
-00007000: 3d22 6f72 6965 6e74 6174 696f 6e22 2f3e  ="orientation"/>
-00007010: 0a20 2020 203c 6669 656c 6420 6564 6974  .    <field edit
-00007020: 6162 6c65 3d22 3122 206e 616d 653d 226f  able="1" name="o
-00007030: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
-00007040: 6465 6e63 6522 2f3e 0a20 2020 203c 6669  dence"/>.    <fi
-00007050: 656c 6420 6564 6974 6162 6c65 3d22 3122  eld editable="1"
-00007060: 206e 616d 653d 226f 736d 5f69 6422 2f3e   name="osm_id"/>
-00007070: 0a20 2020 203c 6669 656c 6420 6564 6974  .    <field edit
-00007080: 6162 6c65 3d22 3122 206e 616d 653d 2274  able="1" name="t
-00007090: 7970 6522 2f3e 0a20 203c 2f65 6469 7461  ype"/>.  </edita
-000070a0: 626c 653e 0a20 203c 6c61 6265 6c4f 6e54  ble>.  <labelOnT
-000070b0: 6f70 3e0a 2020 2020 3c66 6965 6c64 206e  op>.    <field n
-000070c0: 616d 653d 2261 6e67 6c65 2220 6c61 6265  ame="angle" labe
-000070d0: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
-000070e0: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
-000070f0: 6965 6e74 6174 696f 6e22 206c 6162 656c  ientation" label
-00007100: 4f6e 546f 703d 2230 222f 3e0a 2020 2020  OnTop="0"/>.    
-00007110: 3c66 6965 6c64 206e 616d 653d 226f 7269  <field name="ori
-00007120: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
-00007130: 6e63 6522 206c 6162 656c 4f6e 546f 703d  nce" labelOnTop=
-00007140: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
-00007150: 206e 616d 653d 226f 736d 5f69 6422 206c   name="osm_id" l
-00007160: 6162 656c 4f6e 546f 703d 2230 222f 3e0a  abelOnTop="0"/>.
-00007170: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
-00007180: 2274 7970 6522 206c 6162 656c 4f6e 546f  "type" labelOnTo
-00007190: 703d 2230 222f 3e0a 2020 3c2f 6c61 6265  p="0"/>.  </labe
-000071a0: 6c4f 6e54 6f70 3e0a 2020 3c72 6575 7365  lOnTop>.  <reuse
-000071b0: 4c61 7374 5661 6c75 653e 0a20 2020 203c  LastValue>.    <
-000071c0: 6669 656c 6420 7265 7573 654c 6173 7456  field reuseLastV
-000071d0: 616c 7565 3d22 3022 206e 616d 653d 2261  alue="0" name="a
-000071e0: 6e67 6c65 222f 3e0a 2020 2020 3c66 6965  ngle"/>.    <fie
-000071f0: 6c64 2072 6575 7365 4c61 7374 5661 6c75  ld reuseLastValu
-00007200: 653d 2230 2220 6e61 6d65 3d22 6f72 6965  e="0" name="orie
-00007210: 6e74 6174 696f 6e22 2f3e 0a20 2020 203c  ntation"/>.    <
-00007220: 6669 656c 6420 7265 7573 654c 6173 7456  field reuseLastV
-00007230: 616c 7565 3d22 3022 206e 616d 653d 226f  alue="0" name="o
-00007240: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
-00007250: 6465 6e63 6522 2f3e 0a20 2020 203c 6669  dence"/>.    <fi
-00007260: 656c 6420 7265 7573 654c 6173 7456 616c  eld reuseLastVal
-00007270: 7565 3d22 3022 206e 616d 653d 226f 736d  ue="0" name="osm
-00007280: 5f69 6422 2f3e 0a20 2020 203c 6669 656c  _id"/>.    <fiel
-00007290: 6420 7265 7573 654c 6173 7456 616c 7565  d reuseLastValue
-000072a0: 3d22 3022 206e 616d 653d 2274 7970 6522  ="0" name="type"
-000072b0: 2f3e 0a20 203c 2f72 6575 7365 4c61 7374  />.  </reuseLast
-000072c0: 5661 6c75 653e 0a20 203c 6461 7461 4465  Value>.  <dataDe
-000072d0: 6669 6e65 6446 6965 6c64 5072 6f70 6572  finedFieldProper
-000072e0: 7469 6573 2f3e 0a20 203c 7769 6467 6574  ties/>.  <widget
-000072f0: 732f 3e0a 2020 3c70 7265 7669 6577 4578  s/>.  <previewEx
-00007300: 7072 6573 7369 6f6e 3e22 7479 7065 223c  pression>"type"<
-00007310: 2f70 7265 7669 6577 4578 7072 6573 7369  /previewExpressi
-00007320: 6f6e 3e0a 2020 3c6d 6170 5469 703e 3c2f  on>.  <mapTip></
-00007330: 6d61 7054 6970 3e0a 2020 3c6c 6179 6572  mapTip>.  <layer
-00007340: 4765 6f6d 6574 7279 5479 7065 3e31 3c2f  GeometryType>1</
-00007350: 6c61 7965 7247 656f 6d65 7472 7954 7970  layerGeometryTyp
-00007360: 653e 0a3c 2f71 6769 733e 0a              e>.</qgis>.
+000020d0: 756c 6520 6669 6c74 6572 3d22 2671 756f  ule filter="&quo
+000020e0: 743b 7479 7065 2671 756f 743b 203d 2027  t;type&quot; = '
+000020f0: 7369 6465 7761 6c6b 2726 2378 613b 2220  sidewalk'&#xa;" 
+00002100: 7363 616c 656d 6178 6465 6e6f 6d3d 2233  scalemaxdenom="3
+00002110: 3030 2220 6b65 793d 227b 3338 3939 3865  00" key="{38998e
+00002120: 6366 2d37 3533 302d 3439 3362 2d38 3263  cf-7530-493b-82c
+00002130: 362d 3236 3661 6130 3034 3339 3330 7d22  6-266aa0043930}"
+00002140: 2073 796d 626f 6c3d 2230 2220 7363 616c   symbol="0" scal
+00002150: 656d 696e 6465 6e6f 6d3d 2231 222f 3e0a  emindenom="1"/>.
+00002160: 2020 2020 2020 3c72 756c 6520 6669 6c74        <rule filt
+00002170: 6572 3d22 2671 756f 743b 7479 7065 2671  er="&quot;type&q
+00002180: 756f 743b 3d27 7369 6465 7761 6c6b 2722  uot;='sidewalk'"
+00002190: 2073 6361 6c65 6d61 7864 656e 6f6d 3d22   scalemaxdenom="
+000021a0: 3130 3030 3030 2220 6b65 793d 227b 3063  100000" key="{0c
+000021b0: 3065 3536 3863 2d34 6336 652d 3464 6164  0e568c-4c6e-4dad
+000021c0: 2d39 3830 362d 3533 6138 6339 3230 6634  -9806-53a8c920f4
+000021d0: 6136 7d22 2073 796d 626f 6c3d 2231 2220  a6}" symbol="1" 
+000021e0: 7363 616c 656d 696e 6465 6e6f 6d3d 2233  scalemindenom="3
+000021f0: 3030 222f 3e0a 2020 2020 2020 3c72 756c  00"/>.      <rul
+00002200: 6520 6669 6c74 6572 3d22 2671 756f 743b  e filter="&quot;
+00002210: 7479 7065 2671 756f 743b 203d 2027 7472  type&quot; = 'tr
+00002220: 6166 6669 635f 6973 6c61 6e64 2722 206b  affic_island'" k
+00002230: 6579 3d22 7b35 3561 3662 3334 332d 3264  ey="{55a6b343-2d
+00002240: 3161 2d34 6434 612d 3832 3762 2d32 3033  1a-4d4a-827b-203
+00002250: 3335 3261 3139 6531 327d 2220 7379 6d62  352a19e12}" symb
+00002260: 6f6c 3d22 3222 2f3e 0a20 2020 203c 2f72  ol="2"/>.    </r
+00002270: 756c 6573 3e0a 2020 2020 3c73 796d 626f  ules>.    <symbo
+00002280: 6c73 3e0a 2020 2020 2020 3c73 796d 626f  ls>.      <symbo
+00002290: 6c20 6672 616d 655f 7261 7465 3d22 3130  l frame_rate="10
+000022a0: 2220 6e61 6d65 3d22 3022 2061 6c70 6861  " name="0" alpha
+000022b0: 3d22 3122 2069 735f 616e 696d 6174 6564  ="1" is_animated
+000022c0: 3d22 3022 2063 6c69 705f 746f 5f65 7874  ="0" clip_to_ext
+000022d0: 656e 743d 2231 2220 7479 7065 3d22 6c69  ent="1" type="li
+000022e0: 6e65 2220 666f 7263 655f 7268 723d 2230  ne" force_rhr="0
+000022f0: 223e 0a20 2020 2020 2020 203c 6461 7461  ">.        <data
+00002300: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
+00002310: 6965 733e 0a20 2020 2020 2020 2020 203c  ies>.          <
+00002320: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
+00002330: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00002340: 4f70 7469 6f6e 2076 616c 7565 3d22 2220  Option value="" 
+00002350: 6e61 6d65 3d22 6e61 6d65 2220 7479 7065  name="name" type
+00002360: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002370: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002380: 206e 616d 653d 2270 726f 7065 7274 6965   name="propertie
+00002390: 7322 2f3e 0a20 2020 2020 2020 2020 2020  s"/>.           
+000023a0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000023b0: 636f 6c6c 6563 7469 6f6e 2220 6e61 6d65  collection" name
+000023c0: 3d22 7479 7065 2220 7479 7065 3d22 5153  ="type" type="QS
+000023d0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000023e0: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+000023f0: 2020 2020 203c 2f64 6174 615f 6465 6669       </data_defi
+00002400: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
+00002410: 2020 2020 2020 2020 3c6c 6179 6572 2063          <layer c
+00002420: 6c61 7373 3d22 5369 6d70 6c65 4c69 6e65  lass="SimpleLine
+00002430: 2220 7061 7373 3d22 3022 2065 6e61 626c  " pass="0" enabl
+00002440: 6564 3d22 3122 206c 6f63 6b65 643d 2230  ed="1" locked="0
+00002450: 223e 0a20 2020 2020 2020 2020 203c 4f70  ">.          <Op
+00002460: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
+00002470: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00002480: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00002490: 616d 653d 2261 6c69 676e 5f64 6173 685f  ame="align_dash_
+000024a0: 7061 7474 6572 6e22 2074 7970 653d 2251  pattern" type="Q
+000024b0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000024c0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000024d0: 6c75 653d 2272 6f75 6e64 2220 6e61 6d65  lue="round" name
+000024e0: 3d22 6361 7073 7479 6c65 2220 7479 7065  ="capstyle" type
+000024f0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002500: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002510: 2076 616c 7565 3d22 353b 3222 206e 616d   value="5;2" nam
+00002520: 653d 2263 7573 746f 6d64 6173 6822 2074  e="customdash" t
+00002530: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00002540: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00002550: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
+00002560: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
+00002570: 2263 7573 746f 6d64 6173 685f 6d61 705f  "customdash_map_
+00002580: 756e 6974 5f73 6361 6c65 2220 7479 7065  unit_scale" type
+00002590: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000025a0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+000025b0: 2076 616c 7565 3d22 4d4d 2220 6e61 6d65   value="MM" name
+000025c0: 3d22 6375 7374 6f6d 6461 7368 5f75 6e69  ="customdash_uni
+000025d0: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+000025e0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000025f0: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00002600: 2220 6e61 6d65 3d22 6461 7368 5f70 6174  " name="dash_pat
+00002610: 7465 726e 5f6f 6666 7365 7422 2074 7970  tern_offset" typ
+00002620: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002630: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002640: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+00002650: 302c 302c 302c 3022 206e 616d 653d 2264  0,0,0,0" name="d
+00002660: 6173 685f 7061 7474 6572 6e5f 6f66 6673  ash_pattern_offs
+00002670: 6574 5f6d 6170 5f75 6e69 745f 7363 616c  et_map_unit_scal
+00002680: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00002690: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000026a0: 3c4f 7074 696f 6e20 7661 6c75 653d 224d  <Option value="M
+000026b0: 4d22 206e 616d 653d 2264 6173 685f 7061  M" name="dash_pa
+000026c0: 7474 6572 6e5f 6f66 6673 6574 5f75 6e69  ttern_offset_uni
+000026d0: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+000026e0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000026f0: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00002700: 2220 6e61 6d65 3d22 6472 6177 5f69 6e73  " name="draw_ins
+00002710: 6964 655f 706f 6c79 676f 6e22 2074 7970  ide_polygon" typ
+00002720: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002730: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002740: 6e20 7661 6c75 653d 2272 6f75 6e64 2220  n value="round" 
+00002750: 6e61 6d65 3d22 6a6f 696e 7374 796c 6522  name="joinstyle"
+00002760: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00002770: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00002780: 7074 696f 6e20 7661 6c75 653d 2232 3535  ption value="255
+00002790: 2c32 3535 2c32 3535 2c32 3535 2220 6e61  ,255,255,255" na
+000027a0: 6d65 3d22 6c69 6e65 5f63 6f6c 6f72 2220  me="line_color" 
+000027b0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000027c0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+000027d0: 7469 6f6e 2076 616c 7565 3d22 736f 6c69  tion value="soli
+000027e0: 6422 206e 616d 653d 226c 696e 655f 7374  d" name="line_st
+000027f0: 796c 6522 2074 7970 653d 2251 5374 7269  yle" type="QStri
+00002800: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00002810: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00002820: 2236 2220 6e61 6d65 3d22 6c69 6e65 5f77  "6" name="line_w
+00002830: 6964 7468 2220 7479 7065 3d22 5153 7472  idth" type="QStr
+00002840: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00002850: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00002860: 3d22 4d4d 2220 6e61 6d65 3d22 6c69 6e65  ="MM" name="line
+00002870: 5f77 6964 7468 5f75 6e69 7422 2074 7970  _width_unit" typ
+00002880: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002890: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000028a0: 6e20 7661 6c75 653d 2230 2220 6e61 6d65  n value="0" name
+000028b0: 3d22 6f66 6673 6574 2220 7479 7065 3d22  ="offset" type="
+000028c0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+000028d0: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+000028e0: 616c 7565 3d22 3378 3a30 2c30 2c30 2c30  alue="3x:0,0,0,0
+000028f0: 2c30 2c30 2220 6e61 6d65 3d22 6f66 6673  ,0,0" name="offs
+00002900: 6574 5f6d 6170 5f75 6e69 745f 7363 616c  et_map_unit_scal
+00002910: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00002920: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00002930: 3c4f 7074 696f 6e20 7661 6c75 653d 224d  <Option value="M
+00002940: 4d22 206e 616d 653d 226f 6666 7365 745f  M" name="offset_
+00002950: 756e 6974 2220 7479 7065 3d22 5153 7472  unit" type="QStr
+00002960: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00002970: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00002980: 3d22 3022 206e 616d 653d 2272 696e 675f  ="0" name="ring_
+00002990: 6669 6c74 6572 2220 7479 7065 3d22 5153  filter" type="QS
+000029a0: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+000029b0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+000029c0: 7565 3d22 3022 206e 616d 653d 2274 7269  ue="0" name="tri
+000029d0: 6d5f 6469 7374 616e 6365 5f65 6e64 2220  m_distance_end" 
+000029e0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000029f0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00002a00: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
+00002a10: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
+00002a20: 3d22 7472 696d 5f64 6973 7461 6e63 655f  ="trim_distance_
+00002a30: 656e 645f 6d61 705f 756e 6974 5f73 6361  end_map_unit_sca
+00002a40: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00002a50: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00002a60: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00002a70: 4d4d 2220 6e61 6d65 3d22 7472 696d 5f64  MM" name="trim_d
+00002a80: 6973 7461 6e63 655f 656e 645f 756e 6974  istance_end_unit
+00002a90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00002aa0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00002ab0: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+00002ac0: 206e 616d 653d 2274 7269 6d5f 6469 7374   name="trim_dist
+00002ad0: 616e 6365 5f73 7461 7274 2220 7479 7065  ance_start" type
+00002ae0: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002af0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002b00: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
+00002b10: 2c30 2c30 2c30 2220 6e61 6d65 3d22 7472  ,0,0,0" name="tr
+00002b20: 696d 5f64 6973 7461 6e63 655f 7374 6172  im_distance_star
+00002b30: 745f 6d61 705f 756e 6974 5f73 6361 6c65  t_map_unit_scale
+00002b40: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00002b50: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00002b60: 4f70 7469 6f6e 2076 616c 7565 3d22 4d4d  Option value="MM
+00002b70: 2220 6e61 6d65 3d22 7472 696d 5f64 6973  " name="trim_dis
+00002b80: 7461 6e63 655f 7374 6172 745f 756e 6974  tance_start_unit
+00002b90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00002ba0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00002bb0: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+00002bc0: 206e 616d 653d 2274 7765 616b 5f64 6173   name="tweak_das
+00002bd0: 685f 7061 7474 6572 6e5f 6f6e 5f63 6f72  h_pattern_on_cor
+00002be0: 6e65 7273 2220 7479 7065 3d22 5153 7472  ners" type="QStr
+00002bf0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00002c00: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00002c10: 3d22 3022 206e 616d 653d 2275 7365 5f63  ="0" name="use_c
+00002c20: 7573 746f 6d5f 6461 7368 2220 7479 7065  ustom_dash" type
+00002c30: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+00002c40: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002c50: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
+00002c60: 2c30 2c30 2c30 2220 6e61 6d65 3d22 7769  ,0,0,0" name="wi
+00002c70: 6474 685f 6d61 705f 756e 6974 5f73 6361  dth_map_unit_sca
+00002c80: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00002c90: 6722 2f3e 0a20 2020 2020 2020 2020 203c  g"/>.          <
+00002ca0: 2f4f 7074 696f 6e3e 0a20 2020 2020 2020  /Option>.       
+00002cb0: 2020 203c 6461 7461 5f64 6566 696e 6564     <data_defined
+00002cc0: 5f70 726f 7065 7274 6965 733e 0a20 2020  _properties>.   
+00002cd0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00002ce0: 2074 7970 653d 224d 6170 223e 0a20 2020   type="Map">.   
+00002cf0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00002d00: 6f6e 2076 616c 7565 3d22 2220 6e61 6d65  on value="" name
+00002d10: 3d22 6e61 6d65 2220 7479 7065 3d22 5153  ="name" type="QS
+00002d20: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002d30: 2020 2020 2020 203c 4f70 7469 6f6e 206e         <Option n
+00002d40: 616d 653d 2270 726f 7065 7274 6965 7322  ame="properties"
+00002d50: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00002d60: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00002d70: 636f 6c6c 6563 7469 6f6e 2220 6e61 6d65  collection" name
+00002d80: 3d22 7479 7065 2220 7479 7065 3d22 5153  ="type" type="QS
+00002d90: 7472 696e 6722 2f3e 0a20 2020 2020 2020  tring"/>.       
+00002da0: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00002db0: 2020 2020 2020 2020 203c 2f64 6174 615f           </data_
+00002dc0: 6465 6669 6e65 645f 7072 6f70 6572 7469  defined_properti
+00002dd0: 6573 3e0a 2020 2020 2020 2020 3c2f 6c61  es>.        </la
+00002de0: 7965 723e 0a20 2020 2020 203c 2f73 796d  yer>.      </sym
+00002df0: 626f 6c3e 0a20 2020 2020 203c 7379 6d62  bol>.      <symb
+00002e00: 6f6c 2066 7261 6d65 5f72 6174 653d 2231  ol frame_rate="1
+00002e10: 3022 206e 616d 653d 2231 2220 616c 7068  0" name="1" alph
+00002e20: 613d 2231 2220 6973 5f61 6e69 6d61 7465  a="1" is_animate
+00002e30: 643d 2230 2220 636c 6970 5f74 6f5f 6578  d="0" clip_to_ex
+00002e40: 7465 6e74 3d22 3122 2074 7970 653d 226c  tent="1" type="l
+00002e50: 696e 6522 2066 6f72 6365 5f72 6872 3d22  ine" force_rhr="
+00002e60: 3022 3e0a 2020 2020 2020 2020 3c64 6174  0">.        <dat
+00002e70: 615f 6465 6669 6e65 645f 7072 6f70 6572  a_defined_proper
+00002e80: 7469 6573 3e0a 2020 2020 2020 2020 2020  ties>.          
+00002e90: 3c4f 7074 696f 6e20 7479 7065 3d22 4d61  <Option type="Ma
+00002ea0: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
+00002eb0: 3c4f 7074 696f 6e20 7661 6c75 653d 2222  <Option value=""
+00002ec0: 206e 616d 653d 226e 616d 6522 2074 7970   name="name" typ
+00002ed0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00002ee0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00002ef0: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
+00002f00: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
+00002f10: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00002f20: 2263 6f6c 6c65 6374 696f 6e22 206e 616d  "collection" nam
+00002f30: 653d 2274 7970 6522 2074 7970 653d 2251  e="type" type="Q
+00002f40: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00002f50: 2020 2020 3c2f 4f70 7469 6f6e 3e0a 2020      </Option>.  
+00002f60: 2020 2020 2020 3c2f 6461 7461 5f64 6566        </data_def
+00002f70: 696e 6564 5f70 726f 7065 7274 6965 733e  ined_properties>
+00002f80: 0a20 2020 2020 2020 203c 6c61 7965 7220  .        <layer 
+00002f90: 636c 6173 733d 2253 696d 706c 654c 696e  class="SimpleLin
+00002fa0: 6522 2070 6173 733d 2230 2220 656e 6162  e" pass="0" enab
+00002fb0: 6c65 643d 2231 2220 6c6f 636b 6564 3d22  led="1" locked="
+00002fc0: 3022 3e0a 2020 2020 2020 2020 2020 3c4f  0">.          <O
+00002fd0: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
+00002fe0: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00002ff0: 7074 696f 6e20 7661 6c75 653d 2230 2220  ption value="0" 
+00003000: 6e61 6d65 3d22 616c 6967 6e5f 6461 7368  name="align_dash
+00003010: 5f70 6174 7465 726e 2220 7479 7065 3d22  _pattern" type="
+00003020: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003030: 2020 2020 2020 203c 4f70 7469 6f6e 2076         <Option v
+00003040: 616c 7565 3d22 726f 756e 6422 206e 616d  alue="round" nam
+00003050: 653d 2263 6170 7374 796c 6522 2074 7970  e="capstyle" typ
+00003060: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003070: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003080: 6e20 7661 6c75 653d 2235 3b32 2220 6e61  n value="5;2" na
+00003090: 6d65 3d22 6375 7374 6f6d 6461 7368 2220  me="customdash" 
+000030a0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+000030b0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+000030c0: 7469 6f6e 2076 616c 7565 3d22 3378 3a30  tion value="3x:0
+000030d0: 2c30 2c30 2c30 2c30 2c30 2220 6e61 6d65  ,0,0,0,0,0" name
+000030e0: 3d22 6375 7374 6f6d 6461 7368 5f6d 6170  ="customdash_map
+000030f0: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
+00003100: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003110: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003120: 6e20 7661 6c75 653d 224d 4d22 206e 616d  n value="MM" nam
+00003130: 653d 2263 7573 746f 6d64 6173 685f 756e  e="customdash_un
+00003140: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00003150: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003160: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003170: 3022 206e 616d 653d 2264 6173 685f 7061  0" name="dash_pa
+00003180: 7474 6572 6e5f 6f66 6673 6574 2220 7479  ttern_offset" ty
+00003190: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000031a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000031b0: 6f6e 2076 616c 7565 3d22 3378 3a30 2c30  on value="3x:0,0
+000031c0: 2c30 2c30 2c30 2c30 2220 6e61 6d65 3d22  ,0,0,0,0" name="
+000031d0: 6461 7368 5f70 6174 7465 726e 5f6f 6666  dash_pattern_off
+000031e0: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
+000031f0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00003200: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003210: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003220: 4d4d 2220 6e61 6d65 3d22 6461 7368 5f70  MM" name="dash_p
+00003230: 6174 7465 726e 5f6f 6666 7365 745f 756e  attern_offset_un
+00003240: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00003250: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00003260: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003270: 3022 206e 616d 653d 2264 7261 775f 696e  0" name="draw_in
+00003280: 7369 6465 5f70 6f6c 7967 6f6e 2220 7479  side_polygon" ty
+00003290: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+000032a0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+000032b0: 6f6e 2076 616c 7565 3d22 726f 756e 6422  on value="round"
+000032c0: 206e 616d 653d 226a 6f69 6e73 7479 6c65   name="joinstyle
+000032d0: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+000032e0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+000032f0: 4f70 7469 6f6e 2076 616c 7565 3d22 3235  Option value="25
+00003300: 352c 3235 352c 3235 352c 3235 3522 206e  5,255,255,255" n
+00003310: 616d 653d 226c 696e 655f 636f 6c6f 7222  ame="line_color"
+00003320: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003330: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003340: 7074 696f 6e20 7661 6c75 653d 2273 6f6c  ption value="sol
+00003350: 6964 2220 6e61 6d65 3d22 6c69 6e65 5f73  id" name="line_s
+00003360: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
+00003370: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00003380: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003390: 3d22 3522 206e 616d 653d 226c 696e 655f  ="5" name="line_
+000033a0: 7769 6474 6822 2074 7970 653d 2251 5374  width" type="QSt
+000033b0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000033c0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+000033d0: 653d 224d 4d22 206e 616d 653d 226c 696e  e="MM" name="lin
+000033e0: 655f 7769 6474 685f 756e 6974 2220 7479  e_width_unit" ty
+000033f0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003400: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003410: 6f6e 2076 616c 7565 3d22 3022 206e 616d  on value="0" nam
+00003420: 653d 226f 6666 7365 7422 2074 7970 653d  e="offset" type=
+00003430: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003440: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003450: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+00003460: 302c 302c 3022 206e 616d 653d 226f 6666  0,0,0" name="off
+00003470: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
+00003480: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+00003490: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+000034a0: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+000034b0: 4d4d 2220 6e61 6d65 3d22 6f66 6673 6574  MM" name="offset
+000034c0: 5f75 6e69 7422 2074 7970 653d 2251 5374  _unit" type="QSt
+000034d0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000034e0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+000034f0: 653d 2230 2220 6e61 6d65 3d22 7269 6e67  e="0" name="ring
+00003500: 5f66 696c 7465 7222 2074 7970 653d 2251  _filter" type="Q
+00003510: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003520: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00003530: 6c75 653d 2230 2220 6e61 6d65 3d22 7472  lue="0" name="tr
+00003540: 696d 5f64 6973 7461 6e63 655f 656e 6422  im_distance_end"
+00003550: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003560: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003570: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
+00003580: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
+00003590: 653d 2274 7269 6d5f 6469 7374 616e 6365  e="trim_distance
+000035a0: 5f65 6e64 5f6d 6170 5f75 6e69 745f 7363  _end_map_unit_sc
+000035b0: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+000035c0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+000035d0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000035e0: 224d 4d22 206e 616d 653d 2274 7269 6d5f  "MM" name="trim_
+000035f0: 6469 7374 616e 6365 5f65 6e64 5f75 6e69  distance_end_uni
+00003600: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00003610: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003620: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00003630: 2220 6e61 6d65 3d22 7472 696d 5f64 6973  " name="trim_dis
+00003640: 7461 6e63 655f 7374 6172 7422 2074 7970  tance_start" typ
+00003650: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003660: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003670: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+00003680: 302c 302c 302c 3022 206e 616d 653d 2274  0,0,0,0" name="t
+00003690: 7269 6d5f 6469 7374 616e 6365 5f73 7461  rim_distance_sta
+000036a0: 7274 5f6d 6170 5f75 6e69 745f 7363 616c  rt_map_unit_scal
+000036b0: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+000036c0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000036d0: 3c4f 7074 696f 6e20 7661 6c75 653d 224d  <Option value="M
+000036e0: 4d22 206e 616d 653d 2274 7269 6d5f 6469  M" name="trim_di
+000036f0: 7374 616e 6365 5f73 7461 7274 5f75 6e69  stance_start_uni
+00003700: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00003710: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003720: 3c4f 7074 696f 6e20 7661 6c75 653d 2230  <Option value="0
+00003730: 2220 6e61 6d65 3d22 7477 6561 6b5f 6461  " name="tweak_da
+00003740: 7368 5f70 6174 7465 726e 5f6f 6e5f 636f  sh_pattern_on_co
+00003750: 726e 6572 7322 2074 7970 653d 2251 5374  rners" type="QSt
+00003760: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003770: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003780: 653d 2230 2220 6e61 6d65 3d22 7573 655f  e="0" name="use_
+00003790: 6375 7374 6f6d 5f64 6173 6822 2074 7970  custom_dash" typ
+000037a0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+000037b0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000037c0: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+000037d0: 302c 302c 302c 3022 206e 616d 653d 2277  0,0,0,0" name="w
+000037e0: 6964 7468 5f6d 6170 5f75 6e69 745f 7363  idth_map_unit_sc
+000037f0: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+00003800: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003810: 3c2f 4f70 7469 6f6e 3e0a 2020 2020 2020  </Option>.      
+00003820: 2020 2020 3c64 6174 615f 6465 6669 6e65      <data_define
+00003830: 645f 7072 6f70 6572 7469 6573 3e0a 2020  d_properties>.  
+00003840: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003850: 6e20 7479 7065 3d22 4d61 7022 3e0a 2020  n type="Map">.  
+00003860: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003870: 696f 6e20 7661 6c75 653d 2222 206e 616d  ion value="" nam
+00003880: 653d 226e 616d 6522 2074 7970 653d 2251  e="name" type="Q
+00003890: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000038a0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000038b0: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
+000038c0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000038d0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000038e0: 2263 6f6c 6c65 6374 696f 6e22 206e 616d  "collection" nam
+000038f0: 653d 2274 7970 6522 2074 7970 653d 2251  e="type" type="Q
+00003900: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003910: 2020 2020 2020 3c2f 4f70 7469 6f6e 3e0a        </Option>.
+00003920: 2020 2020 2020 2020 2020 3c2f 6461 7461            </data
+00003930: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
+00003940: 6965 733e 0a20 2020 2020 2020 203c 2f6c  ies>.        </l
+00003950: 6179 6572 3e0a 2020 2020 2020 3c2f 7379  ayer>.      </sy
+00003960: 6d62 6f6c 3e0a 2020 2020 2020 3c73 796d  mbol>.      <sym
+00003970: 626f 6c20 6672 616d 655f 7261 7465 3d22  bol frame_rate="
+00003980: 3130 2220 6e61 6d65 3d22 3222 2061 6c70  10" name="2" alp
+00003990: 6861 3d22 3122 2069 735f 616e 696d 6174  ha="1" is_animat
+000039a0: 6564 3d22 3022 2063 6c69 705f 746f 5f65  ed="0" clip_to_e
+000039b0: 7874 656e 743d 2231 2220 7479 7065 3d22  xtent="1" type="
+000039c0: 6c69 6e65 2220 666f 7263 655f 7268 723d  line" force_rhr=
+000039d0: 2230 223e 0a20 2020 2020 2020 203c 6461  "0">.        <da
+000039e0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+000039f0: 7274 6965 733e 0a20 2020 2020 2020 2020  rties>.         
+00003a00: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
+00003a10: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
+00003a20: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00003a30: 2220 6e61 6d65 3d22 6e61 6d65 2220 7479  " name="name" ty
+00003a40: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003a50: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003a60: 6f6e 206e 616d 653d 2270 726f 7065 7274  on name="propert
+00003a70: 6965 7322 2f3e 0a20 2020 2020 2020 2020  ies"/>.         
+00003a80: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00003a90: 3d22 636f 6c6c 6563 7469 6f6e 2220 6e61  ="collection" na
+00003aa0: 6d65 3d22 7479 7065 2220 7479 7065 3d22  me="type" type="
+00003ab0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00003ac0: 2020 2020 203c 2f4f 7074 696f 6e3e 0a20       </Option>. 
+00003ad0: 2020 2020 2020 203c 2f64 6174 615f 6465         </data_de
+00003ae0: 6669 6e65 645f 7072 6f70 6572 7469 6573  fined_properties
+00003af0: 3e0a 2020 2020 2020 2020 3c6c 6179 6572  >.        <layer
+00003b00: 2063 6c61 7373 3d22 5369 6d70 6c65 4c69   class="SimpleLi
+00003b10: 6e65 2220 7061 7373 3d22 3022 2065 6e61  ne" pass="0" ena
+00003b20: 626c 6564 3d22 3122 206c 6f63 6b65 643d  bled="1" locked=
+00003b30: 2230 223e 0a20 2020 2020 2020 2020 203c  "0">.          <
+00003b40: 4f70 7469 6f6e 2074 7970 653d 224d 6170  Option type="Map
+00003b50: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00003b60: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+00003b70: 206e 616d 653d 2261 6c69 676e 5f64 6173   name="align_das
+00003b80: 685f 7061 7474 6572 6e22 2074 7970 653d  h_pattern" type=
+00003b90: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00003ba0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00003bb0: 7661 6c75 653d 2272 6f75 6e64 2220 6e61  value="round" na
+00003bc0: 6d65 3d22 6361 7073 7479 6c65 2220 7479  me="capstyle" ty
+00003bd0: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003be0: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003bf0: 6f6e 2076 616c 7565 3d22 353b 3222 206e  on value="5;2" n
+00003c00: 616d 653d 2263 7573 746f 6d64 6173 6822  ame="customdash"
+00003c10: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00003c20: 3e0a 2020 2020 2020 2020 2020 2020 3c4f  >.            <O
+00003c30: 7074 696f 6e20 7661 6c75 653d 2233 783a  ption value="3x:
+00003c40: 302c 302c 302c 302c 302c 3022 206e 616d  0,0,0,0,0,0" nam
+00003c50: 653d 2263 7573 746f 6d64 6173 685f 6d61  e="customdash_ma
+00003c60: 705f 756e 6974 5f73 6361 6c65 2220 7479  p_unit_scale" ty
+00003c70: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00003c80: 2020 2020 2020 2020 2020 203c 4f70 7469             <Opti
+00003c90: 6f6e 2076 616c 7565 3d22 4d4d 2220 6e61  on value="MM" na
+00003ca0: 6d65 3d22 6375 7374 6f6d 6461 7368 5f75  me="customdash_u
+00003cb0: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00003cc0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003cd0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003ce0: 2230 2220 6e61 6d65 3d22 6461 7368 5f70  "0" name="dash_p
+00003cf0: 6174 7465 726e 5f6f 6666 7365 7422 2074  attern_offset" t
+00003d00: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003d10: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003d20: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
+00003d30: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
+00003d40: 2264 6173 685f 7061 7474 6572 6e5f 6f66  "dash_pattern_of
+00003d50: 6673 6574 5f6d 6170 5f75 6e69 745f 7363  fset_map_unit_sc
+00003d60: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+00003d70: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003d80: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003d90: 224d 4d22 206e 616d 653d 2264 6173 685f  "MM" name="dash_
+00003da0: 7061 7474 6572 6e5f 6f66 6673 6574 5f75  pattern_offset_u
+00003db0: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00003dc0: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00003dd0: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00003de0: 2230 2220 6e61 6d65 3d22 6472 6177 5f69  "0" name="draw_i
+00003df0: 6e73 6964 655f 706f 6c79 676f 6e22 2074  nside_polygon" t
+00003e00: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00003e10: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00003e20: 696f 6e20 7661 6c75 653d 2272 6f75 6e64  ion value="round
+00003e30: 2220 6e61 6d65 3d22 6a6f 696e 7374 796c  " name="joinstyl
+00003e40: 6522 2074 7970 653d 2251 5374 7269 6e67  e" type="QString
+00003e50: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00003e60: 3c4f 7074 696f 6e20 7661 6c75 653d 2232  <Option value="2
+00003e70: 3535 2c32 3535 2c32 3535 2c32 3535 2220  55,255,255,255" 
+00003e80: 6e61 6d65 3d22 6c69 6e65 5f63 6f6c 6f72  name="line_color
+00003e90: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00003ea0: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00003eb0: 4f70 7469 6f6e 2076 616c 7565 3d22 736f  Option value="so
+00003ec0: 6c69 6422 206e 616d 653d 226c 696e 655f  lid" name="line_
+00003ed0: 7374 796c 6522 2074 7970 653d 2251 5374  style" type="QSt
+00003ee0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00003ef0: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00003f00: 653d 2231 3222 206e 616d 653d 226c 696e  e="12" name="lin
+00003f10: 655f 7769 6474 6822 2074 7970 653d 2251  e_width" type="Q
+00003f20: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00003f30: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00003f40: 6c75 653d 224d 4d22 206e 616d 653d 226c  lue="MM" name="l
+00003f50: 696e 655f 7769 6474 685f 756e 6974 2220  ine_width_unit" 
+00003f60: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00003f70: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00003f80: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00003f90: 616d 653d 226f 6666 7365 7422 2074 7970  ame="offset" typ
+00003fa0: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00003fb0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00003fc0: 6e20 7661 6c75 653d 2233 783a 302c 302c  n value="3x:0,0,
+00003fd0: 302c 302c 302c 3022 206e 616d 653d 226f  0,0,0,0" name="o
+00003fe0: 6666 7365 745f 6d61 705f 756e 6974 5f73  ffset_map_unit_s
+00003ff0: 6361 6c65 2220 7479 7065 3d22 5153 7472  cale" type="QStr
+00004000: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004010: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004020: 3d22 4d4d 2220 6e61 6d65 3d22 6f66 6673  ="MM" name="offs
+00004030: 6574 5f75 6e69 7422 2074 7970 653d 2251  et_unit" type="Q
+00004040: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00004050: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+00004060: 6c75 653d 2230 2220 6e61 6d65 3d22 7269  lue="0" name="ri
+00004070: 6e67 5f66 696c 7465 7222 2074 7970 653d  ng_filter" type=
+00004080: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004090: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000040a0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
+000040b0: 7472 696d 5f64 6973 7461 6e63 655f 656e  trim_distance_en
+000040c0: 6422 2074 7970 653d 2251 5374 7269 6e67  d" type="QString
+000040d0: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+000040e0: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
+000040f0: 783a 302c 302c 302c 302c 302c 3022 206e  x:0,0,0,0,0,0" n
+00004100: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
+00004110: 6365 5f65 6e64 5f6d 6170 5f75 6e69 745f  ce_end_map_unit_
+00004120: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
+00004130: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004140: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004150: 653d 224d 4d22 206e 616d 653d 2274 7269  e="MM" name="tri
+00004160: 6d5f 6469 7374 616e 6365 5f65 6e64 5f75  m_distance_end_u
+00004170: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00004180: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004190: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000041a0: 2230 2220 6e61 6d65 3d22 7472 696d 5f64  "0" name="trim_d
+000041b0: 6973 7461 6e63 655f 7374 6172 7422 2074  istance_start" t
+000041c0: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+000041d0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000041e0: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
+000041f0: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
+00004200: 2274 7269 6d5f 6469 7374 616e 6365 5f73  "trim_distance_s
+00004210: 7461 7274 5f6d 6170 5f75 6e69 745f 7363  tart_map_unit_sc
+00004220: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+00004230: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004240: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00004250: 224d 4d22 206e 616d 653d 2274 7269 6d5f  "MM" name="trim_
+00004260: 6469 7374 616e 6365 5f73 7461 7274 5f75  distance_start_u
+00004270: 6e69 7422 2074 7970 653d 2251 5374 7269  nit" type="QStri
+00004280: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004290: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+000042a0: 2230 2220 6e61 6d65 3d22 7477 6561 6b5f  "0" name="tweak_
+000042b0: 6461 7368 5f70 6174 7465 726e 5f6f 6e5f  dash_pattern_on_
+000042c0: 636f 726e 6572 7322 2074 7970 653d 2251  corners" type="Q
+000042d0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000042e0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000042f0: 6c75 653d 2230 2220 6e61 6d65 3d22 7573  lue="0" name="us
+00004300: 655f 6375 7374 6f6d 5f64 6173 6822 2074  e_custom_dash" t
+00004310: 7970 653d 2251 5374 7269 6e67 222f 3e0a  ype="QString"/>.
+00004320: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00004330: 696f 6e20 7661 6c75 653d 2233 783a 302c  ion value="3x:0,
+00004340: 302c 302c 302c 302c 3022 206e 616d 653d  0,0,0,0,0" name=
+00004350: 2277 6964 7468 5f6d 6170 5f75 6e69 745f  "width_map_unit_
+00004360: 7363 616c 6522 2074 7970 653d 2251 5374  scale" type="QSt
+00004370: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00004380: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
+00004390: 2020 2020 2020 3c64 6174 615f 6465 6669        <data_defi
+000043a0: 6e65 645f 7072 6f70 6572 7469 6573 3e0a  ned_properties>.
+000043b0: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+000043c0: 696f 6e20 7479 7065 3d22 4d61 7022 3e0a  ion type="Map">.
+000043d0: 2020 2020 2020 2020 2020 2020 2020 3c4f                <O
+000043e0: 7074 696f 6e20 7661 6c75 653d 2222 206e  ption value="" n
+000043f0: 616d 653d 226e 616d 6522 2074 7970 653d  ame="name" type=
+00004400: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004410: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00004420: 6e20 6e61 6d65 3d22 7072 6f70 6572 7469  n name="properti
+00004430: 6573 222f 3e0a 2020 2020 2020 2020 2020  es"/>.          
+00004440: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004450: 653d 2263 6f6c 6c65 6374 696f 6e22 206e  e="collection" n
+00004460: 616d 653d 2274 7970 6522 2074 7970 653d  ame="type" type=
+00004470: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004480: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
+00004490: 3e0a 2020 2020 2020 2020 2020 3c2f 6461  >.          </da
+000044a0: 7461 5f64 6566 696e 6564 5f70 726f 7065  ta_defined_prope
+000044b0: 7274 6965 733e 0a20 2020 2020 2020 203c  rties>.        <
+000044c0: 2f6c 6179 6572 3e0a 2020 2020 2020 3c2f  /layer>.      </
+000044d0: 7379 6d62 6f6c 3e0a 2020 2020 3c2f 7379  symbol>.    </sy
+000044e0: 6d62 6f6c 733e 0a20 203c 2f72 656e 6465  mbols>.  </rende
+000044f0: 7265 722d 7632 3e0a 2020 3c63 7573 746f  rer-v2>.  <custo
+00004500: 6d70 726f 7065 7274 6965 733e 0a20 2020  mproperties>.   
+00004510: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
+00004520: 6170 223e 0a20 2020 2020 203c 4f70 7469  ap">.      <Opti
+00004530: 6f6e 206e 616d 653d 2264 7561 6c76 6965  on name="dualvie
+00004540: 772f 7072 6576 6965 7745 7870 7265 7373  w/previewExpress
+00004550: 696f 6e73 2220 7479 7065 3d22 4c69 7374  ions" type="List
+00004560: 223e 0a20 2020 2020 2020 203c 4f70 7469  ">.        <Opti
+00004570: 6f6e 2076 616c 7565 3d22 2671 756f 743b  on value="&quot;
+00004580: 7479 7065 2671 756f 743b 2220 7479 7065  type&quot;" type
+00004590: 3d22 5153 7472 696e 6722 2f3e 0a20 2020  ="QString"/>.   
+000045a0: 2020 203c 2f4f 7074 696f 6e3e 0a20 2020     </Option>.   
+000045b0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+000045c0: 3d22 3022 206e 616d 653d 2265 6d62 6564  ="0" name="embed
+000045d0: 6465 6457 6964 6765 7473 2f63 6f75 6e74  dedWidgets/count
+000045e0: 2220 7479 7065 3d22 696e 7422 2f3e 0a20  " type="int"/>. 
+000045f0: 2020 2020 203c 4f70 7469 6f6e 206e 616d       <Option nam
+00004600: 653d 2276 6172 6961 626c 654e 616d 6573  e="variableNames
+00004610: 222f 3e0a 2020 2020 2020 3c4f 7074 696f  "/>.      <Optio
+00004620: 6e20 6e61 6d65 3d22 7661 7269 6162 6c65  n name="variable
+00004630: 5661 6c75 6573 222f 3e0a 2020 2020 3c2f  Values"/>.    </
+00004640: 4f70 7469 6f6e 3e0a 2020 3c2f 6375 7374  Option>.  </cust
+00004650: 6f6d 7072 6f70 6572 7469 6573 3e0a 2020  omproperties>.  
+00004660: 3c62 6c65 6e64 4d6f 6465 3e30 3c2f 626c  <blendMode>0</bl
+00004670: 656e 644d 6f64 653e 0a20 203c 6665 6174  endMode>.  <feat
+00004680: 7572 6542 6c65 6e64 4d6f 6465 3e30 3c2f  ureBlendMode>0</
+00004690: 6665 6174 7572 6542 6c65 6e64 4d6f 6465  featureBlendMode
+000046a0: 3e0a 2020 3c6c 6179 6572 4f70 6163 6974  >.  <layerOpacit
+000046b0: 793e 313c 2f6c 6179 6572 4f70 6163 6974  y>1</layerOpacit
+000046c0: 793e 0a20 203c 5369 6e67 6c65 4361 7465  y>.  <SingleCate
+000046d0: 676f 7279 4469 6167 7261 6d52 656e 6465  goryDiagramRende
+000046e0: 7265 7220 6469 6167 7261 6d54 7970 653d  rer diagramType=
+000046f0: 2248 6973 746f 6772 616d 2220 6174 7472  "Histogram" attr
+00004700: 6962 7574 654c 6567 656e 643d 2231 223e  ibuteLegend="1">
+00004710: 0a20 2020 203c 4469 6167 7261 6d43 6174  .    <DiagramCat
+00004720: 6567 6f72 7920 7065 6e43 6f6c 6f72 3d22  egory penColor="
+00004730: 2330 3030 3030 3022 2070 656e 5769 6474  #000000" penWidt
+00004740: 683d 2230 2220 7769 6474 683d 2231 3522  h="0" width="15"
+00004750: 2073 697a 6554 7970 653d 224d 4d22 2064   sizeType="MM" d
+00004760: 6972 6563 7469 6f6e 3d22 3022 206c 6162  irection="0" lab
+00004770: 656c 506c 6163 656d 656e 744d 6574 686f  elPlacementMetho
+00004780: 643d 2258 4865 6967 6874 2220 656e 6162  d="XHeight" enab
+00004790: 6c65 643d 2230 2220 6261 7257 6964 7468  led="0" barWidth
+000047a0: 3d22 3522 206d 6178 5363 616c 6544 656e  ="5" maxScaleDen
+000047b0: 6f6d 696e 6174 6f72 3d22 3165 2b30 3822  ominator="1e+08"
+000047c0: 2073 7061 6369 6e67 556e 6974 5363 616c   spacingUnitScal
+000047d0: 653d 2233 783a 302c 302c 302c 302c 302c  e="3x:0,0,0,0,0,
+000047e0: 3022 206f 7061 6369 7479 3d22 3122 2073  0" opacity="1" s
+000047f0: 6361 6c65 4465 7065 6e64 656e 6379 3d22  caleDependency="
+00004800: 4172 6561 2220 6261 636b 6772 6f75 6e64  Area" background
+00004810: 416c 7068 613d 2232 3535 2220 6d69 6e53  Alpha="255" minS
+00004820: 6361 6c65 4465 6e6f 6d69 6e61 746f 723d  caleDenominator=
+00004830: 2230 2220 7370 6163 696e 6755 6e69 743d  "0" spacingUnit=
+00004840: 224d 4d22 206d 696e 696d 756d 5369 7a65  "MM" minimumSize
+00004850: 3d22 3022 2062 6163 6b67 726f 756e 6443  ="0" backgroundC
+00004860: 6f6c 6f72 3d22 2366 6666 6666 6622 206c  olor="#ffffff" l
+00004870: 696e 6553 697a 6554 7970 653d 224d 4d22  ineSizeType="MM"
+00004880: 206c 696e 6553 697a 6553 6361 6c65 3d22   lineSizeScale="
+00004890: 3378 3a30 2c30 2c30 2c30 2c30 2c30 2220  3x:0,0,0,0,0,0" 
+000048a0: 7369 7a65 5363 616c 653d 2233 783a 302c  sizeScale="3x:0,
+000048b0: 302c 302c 302c 302c 3022 2073 6361 6c65  0,0,0,0,0" scale
+000048c0: 4261 7365 6456 6973 6962 696c 6974 793d  BasedVisibility=
+000048d0: 2230 2220 7370 6163 696e 673d 2235 2220  "0" spacing="5" 
+000048e0: 726f 7461 7469 6f6e 4f66 6673 6574 3d22  rotationOffset="
+000048f0: 3237 3022 2068 6569 6768 743d 2231 3522  270" height="15"
+00004900: 2073 686f 7741 7869 733d 2231 2220 6469   showAxis="1" di
+00004910: 6167 7261 6d4f 7269 656e 7461 7469 6f6e  agramOrientation
+00004920: 3d22 5570 2220 7065 6e41 6c70 6861 3d22  ="Up" penAlpha="
+00004930: 3235 3522 3e0a 2020 2020 2020 3c66 6f6e  255">.      <fon
+00004940: 7450 726f 7065 7274 6965 7320 626f 6c64  tProperties bold
+00004950: 3d22 3022 2073 7472 696b 6574 6872 6f75  ="0" strikethrou
+00004960: 6768 3d22 3022 2073 7479 6c65 3d22 2220  gh="0" style="" 
+00004970: 756e 6465 726c 696e 653d 2230 2220 6465  underline="0" de
+00004980: 7363 7269 7074 696f 6e3d 224e 6f74 6f20  scription="Noto 
+00004990: 5361 6e73 2c31 302c 2d31 2c30 2c35 302c  Sans,10,-1,0,50,
+000049a0: 302c 302c 302c 302c 3022 2069 7461 6c69  0,0,0,0,0" itali
+000049b0: 633d 2230 222f 3e0a 2020 2020 2020 3c61  c="0"/>.      <a
+000049c0: 7474 7269 6275 7465 2063 6f6c 6f72 4f70  ttribute colorOp
+000049d0: 6163 6974 793d 2231 2220 636f 6c6f 723d  acity="1" color=
+000049e0: 2223 3030 3030 3030 2220 6669 656c 643d  "#000000" field=
+000049f0: 2222 206c 6162 656c 3d22 222f 3e0a 2020  "" label=""/>.  
+00004a00: 2020 2020 3c61 7869 7353 796d 626f 6c3e      <axisSymbol>
+00004a10: 0a20 2020 2020 2020 203c 7379 6d62 6f6c  .        <symbol
+00004a20: 2066 7261 6d65 5f72 6174 653d 2231 3022   frame_rate="10"
+00004a30: 206e 616d 653d 2222 2061 6c70 6861 3d22   name="" alpha="
+00004a40: 3122 2069 735f 616e 696d 6174 6564 3d22  1" is_animated="
+00004a50: 3022 2063 6c69 705f 746f 5f65 7874 656e  0" clip_to_exten
+00004a60: 743d 2231 2220 7479 7065 3d22 6c69 6e65  t="1" type="line
+00004a70: 2220 666f 7263 655f 7268 723d 2230 223e  " force_rhr="0">
+00004a80: 0a20 2020 2020 2020 2020 203c 6461 7461  .          <data
+00004a90: 5f64 6566 696e 6564 5f70 726f 7065 7274  _defined_propert
+00004aa0: 6965 733e 0a20 2020 2020 2020 2020 2020  ies>.           
+00004ab0: 203c 4f70 7469 6f6e 2074 7970 653d 224d   <Option type="M
+00004ac0: 6170 223e 0a20 2020 2020 2020 2020 2020  ap">.           
+00004ad0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004ae0: 3d22 2220 6e61 6d65 3d22 6e61 6d65 2220  ="" name="name" 
+00004af0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004b00: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00004b10: 4f70 7469 6f6e 206e 616d 653d 2270 726f  Option name="pro
+00004b20: 7065 7274 6965 7322 2f3e 0a20 2020 2020  perties"/>.     
+00004b30: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004b40: 2076 616c 7565 3d22 636f 6c6c 6563 7469   value="collecti
+00004b50: 6f6e 2220 6e61 6d65 3d22 7479 7065 2220  on" name="type" 
+00004b60: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004b70: 0a20 2020 2020 2020 2020 2020 203c 2f4f  .            </O
+00004b80: 7074 696f 6e3e 0a20 2020 2020 2020 2020  ption>.         
+00004b90: 203c 2f64 6174 615f 6465 6669 6e65 645f   </data_defined_
+00004ba0: 7072 6f70 6572 7469 6573 3e0a 2020 2020  properties>.    
+00004bb0: 2020 2020 2020 3c6c 6179 6572 2063 6c61        <layer cla
+00004bc0: 7373 3d22 5369 6d70 6c65 4c69 6e65 2220  ss="SimpleLine" 
+00004bd0: 7061 7373 3d22 3022 2065 6e61 626c 6564  pass="0" enabled
+00004be0: 3d22 3122 206c 6f63 6b65 643d 2230 223e  ="1" locked="0">
+00004bf0: 0a20 2020 2020 2020 2020 2020 203c 4f70  .            <Op
+00004c00: 7469 6f6e 2074 7970 653d 224d 6170 223e  tion type="Map">
+00004c10: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00004c20: 4f70 7469 6f6e 2076 616c 7565 3d22 3022  Option value="0"
+00004c30: 206e 616d 653d 2261 6c69 676e 5f64 6173   name="align_das
+00004c40: 685f 7061 7474 6572 6e22 2074 7970 653d  h_pattern" type=
+00004c50: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004c60: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00004c70: 6e20 7661 6c75 653d 2273 7175 6172 6522  n value="square"
+00004c80: 206e 616d 653d 2263 6170 7374 796c 6522   name="capstyle"
+00004c90: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00004ca0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00004cb0: 3c4f 7074 696f 6e20 7661 6c75 653d 2235  <Option value="5
+00004cc0: 3b32 2220 6e61 6d65 3d22 6375 7374 6f6d  ;2" name="custom
+00004cd0: 6461 7368 2220 7479 7065 3d22 5153 7472  dash" type="QStr
+00004ce0: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004cf0: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00004d00: 7565 3d22 3378 3a30 2c30 2c30 2c30 2c30  ue="3x:0,0,0,0,0
+00004d10: 2c30 2220 6e61 6d65 3d22 6375 7374 6f6d  ,0" name="custom
+00004d20: 6461 7368 5f6d 6170 5f75 6e69 745f 7363  dash_map_unit_sc
+00004d30: 616c 6522 2074 7970 653d 2251 5374 7269  ale" type="QStri
+00004d40: 6e67 222f 3e0a 2020 2020 2020 2020 2020  ng"/>.          
+00004d50: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00004d60: 653d 224d 4d22 206e 616d 653d 2263 7573  e="MM" name="cus
+00004d70: 746f 6d64 6173 685f 756e 6974 2220 7479  tomdash_unit" ty
+00004d80: 7065 3d22 5153 7472 696e 6722 2f3e 0a20  pe="QString"/>. 
+00004d90: 2020 2020 2020 2020 2020 2020 203c 4f70               <Op
+00004da0: 7469 6f6e 2076 616c 7565 3d22 3022 206e  tion value="0" n
+00004db0: 616d 653d 2264 6173 685f 7061 7474 6572  ame="dash_patter
+00004dc0: 6e5f 6f66 6673 6574 2220 7479 7065 3d22  n_offset" type="
+00004dd0: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00004de0: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00004df0: 2076 616c 7565 3d22 3378 3a30 2c30 2c30   value="3x:0,0,0
+00004e00: 2c30 2c30 2c30 2220 6e61 6d65 3d22 6461  ,0,0,0" name="da
+00004e10: 7368 5f70 6174 7465 726e 5f6f 6666 7365  sh_pattern_offse
+00004e20: 745f 6d61 705f 756e 6974 5f73 6361 6c65  t_map_unit_scale
+00004e30: 2220 7479 7065 3d22 5153 7472 696e 6722  " type="QString"
+00004e40: 2f3e 0a20 2020 2020 2020 2020 2020 2020  />.             
+00004e50: 203c 4f70 7469 6f6e 2076 616c 7565 3d22   <Option value="
+00004e60: 4d4d 2220 6e61 6d65 3d22 6461 7368 5f70  MM" name="dash_p
+00004e70: 6174 7465 726e 5f6f 6666 7365 745f 756e  attern_offset_un
+00004e80: 6974 2220 7479 7065 3d22 5153 7472 696e  it" type="QStrin
+00004e90: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004ea0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004eb0: 3d22 3022 206e 616d 653d 2264 7261 775f  ="0" name="draw_
+00004ec0: 696e 7369 6465 5f70 6f6c 7967 6f6e 2220  inside_polygon" 
+00004ed0: 7479 7065 3d22 5153 7472 696e 6722 2f3e  type="QString"/>
+00004ee0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00004ef0: 4f70 7469 6f6e 2076 616c 7565 3d22 6265  Option value="be
+00004f00: 7665 6c22 206e 616d 653d 226a 6f69 6e73  vel" name="joins
+00004f10: 7479 6c65 2220 7479 7065 3d22 5153 7472  tyle" type="QStr
+00004f20: 696e 6722 2f3e 0a20 2020 2020 2020 2020  ing"/>.         
+00004f30: 2020 2020 203c 4f70 7469 6f6e 2076 616c       <Option val
+00004f40: 7565 3d22 3335 2c33 352c 3335 2c32 3535  ue="35,35,35,255
+00004f50: 2220 6e61 6d65 3d22 6c69 6e65 5f63 6f6c  " name="line_col
+00004f60: 6f72 2220 7479 7065 3d22 5153 7472 696e  or" type="QStrin
+00004f70: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+00004f80: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00004f90: 3d22 736f 6c69 6422 206e 616d 653d 226c  ="solid" name="l
+00004fa0: 696e 655f 7374 796c 6522 2074 7970 653d  ine_style" type=
+00004fb0: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00004fc0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+00004fd0: 6e20 7661 6c75 653d 2230 2e32 3622 206e  n value="0.26" n
+00004fe0: 616d 653d 226c 696e 655f 7769 6474 6822  ame="line_width"
+00004ff0: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00005000: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005010: 3c4f 7074 696f 6e20 7661 6c75 653d 224d  <Option value="M
+00005020: 4d22 206e 616d 653d 226c 696e 655f 7769  M" name="line_wi
+00005030: 6474 685f 756e 6974 2220 7479 7065 3d22  dth_unit" type="
+00005040: 5153 7472 696e 6722 2f3e 0a20 2020 2020  QString"/>.     
+00005050: 2020 2020 2020 2020 203c 4f70 7469 6f6e           <Option
+00005060: 2076 616c 7565 3d22 3022 206e 616d 653d   value="0" name=
+00005070: 226f 6666 7365 7422 2074 7970 653d 2251  "offset" type="Q
+00005080: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005090: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000050a0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+000050b0: 302c 302c 3022 206e 616d 653d 226f 6666  0,0,0" name="off
+000050c0: 7365 745f 6d61 705f 756e 6974 5f73 6361  set_map_unit_sca
+000050d0: 6c65 2220 7479 7065 3d22 5153 7472 696e  le" type="QStrin
+000050e0: 6722 2f3e 0a20 2020 2020 2020 2020 2020  g"/>.           
+000050f0: 2020 203c 4f70 7469 6f6e 2076 616c 7565     <Option value
+00005100: 3d22 4d4d 2220 6e61 6d65 3d22 6f66 6673  ="MM" name="offs
+00005110: 6574 5f75 6e69 7422 2074 7970 653d 2251  et_unit" type="Q
+00005120: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+00005130: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005140: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
+00005150: 7269 6e67 5f66 696c 7465 7222 2074 7970  ring_filter" typ
+00005160: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00005170: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005180: 696f 6e20 7661 6c75 653d 2230 2220 6e61  ion value="0" na
+00005190: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
+000051a0: 655f 656e 6422 2074 7970 653d 2251 5374  e_end" type="QSt
+000051b0: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+000051c0: 2020 2020 2020 3c4f 7074 696f 6e20 7661        <Option va
+000051d0: 6c75 653d 2233 783a 302c 302c 302c 302c  lue="3x:0,0,0,0,
+000051e0: 302c 3022 206e 616d 653d 2274 7269 6d5f  0,0" name="trim_
+000051f0: 6469 7374 616e 6365 5f65 6e64 5f6d 6170  distance_end_map
+00005200: 5f75 6e69 745f 7363 616c 6522 2074 7970  _unit_scale" typ
+00005210: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00005220: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005230: 696f 6e20 7661 6c75 653d 224d 4d22 206e  ion value="MM" n
+00005240: 616d 653d 2274 7269 6d5f 6469 7374 616e  ame="trim_distan
+00005250: 6365 5f65 6e64 5f75 6e69 7422 2074 7970  ce_end_unit" typ
+00005260: 653d 2251 5374 7269 6e67 222f 3e0a 2020  e="QString"/>.  
+00005270: 2020 2020 2020 2020 2020 2020 3c4f 7074              <Opt
+00005280: 696f 6e20 7661 6c75 653d 2230 2220 6e61  ion value="0" na
+00005290: 6d65 3d22 7472 696d 5f64 6973 7461 6e63  me="trim_distanc
+000052a0: 655f 7374 6172 7422 2074 7970 653d 2251  e_start" type="Q
+000052b0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000052c0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000052d0: 7661 6c75 653d 2233 783a 302c 302c 302c  value="3x:0,0,0,
+000052e0: 302c 302c 3022 206e 616d 653d 2274 7269  0,0,0" name="tri
+000052f0: 6d5f 6469 7374 616e 6365 5f73 7461 7274  m_distance_start
+00005300: 5f6d 6170 5f75 6e69 745f 7363 616c 6522  _map_unit_scale"
+00005310: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00005320: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005330: 3c4f 7074 696f 6e20 7661 6c75 653d 224d  <Option value="M
+00005340: 4d22 206e 616d 653d 2274 7269 6d5f 6469  M" name="trim_di
+00005350: 7374 616e 6365 5f73 7461 7274 5f75 6e69  stance_start_uni
+00005360: 7422 2074 7970 653d 2251 5374 7269 6e67  t" type="QString
+00005370: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005380: 2020 3c4f 7074 696f 6e20 7661 6c75 653d    <Option value=
+00005390: 2230 2220 6e61 6d65 3d22 7477 6561 6b5f  "0" name="tweak_
+000053a0: 6461 7368 5f70 6174 7465 726e 5f6f 6e5f  dash_pattern_on_
+000053b0: 636f 726e 6572 7322 2074 7970 653d 2251  corners" type="Q
+000053c0: 5374 7269 6e67 222f 3e0a 2020 2020 2020  String"/>.      
+000053d0: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+000053e0: 7661 6c75 653d 2230 2220 6e61 6d65 3d22  value="0" name="
+000053f0: 7573 655f 6375 7374 6f6d 5f64 6173 6822  use_custom_dash"
+00005400: 2074 7970 653d 2251 5374 7269 6e67 222f   type="QString"/
+00005410: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00005420: 3c4f 7074 696f 6e20 7661 6c75 653d 2233  <Option value="3
+00005430: 783a 302c 302c 302c 302c 302c 3022 206e  x:0,0,0,0,0,0" n
+00005440: 616d 653d 2277 6964 7468 5f6d 6170 5f75  ame="width_map_u
+00005450: 6e69 745f 7363 616c 6522 2074 7970 653d  nit_scale" type=
+00005460: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00005470: 2020 2020 2020 2020 3c2f 4f70 7469 6f6e          </Option
+00005480: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+00005490: 6174 615f 6465 6669 6e65 645f 7072 6f70  ata_defined_prop
+000054a0: 6572 7469 6573 3e0a 2020 2020 2020 2020  erties>.        
+000054b0: 2020 2020 2020 3c4f 7074 696f 6e20 7479        <Option ty
+000054c0: 7065 3d22 4d61 7022 3e0a 2020 2020 2020  pe="Map">.      
+000054d0: 2020 2020 2020 2020 2020 3c4f 7074 696f            <Optio
+000054e0: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
+000054f0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
+00005500: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00005510: 2020 2020 2020 2020 3c4f 7074 696f 6e20          <Option 
+00005520: 6e61 6d65 3d22 7072 6f70 6572 7469 6573  name="properties
+00005530: 222f 3e0a 2020 2020 2020 2020 2020 2020  "/>.            
+00005540: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00005550: 653d 2263 6f6c 6c65 6374 696f 6e22 206e  e="collection" n
+00005560: 616d 653d 2274 7970 6522 2074 7970 653d  ame="type" type=
+00005570: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00005580: 2020 2020 2020 2020 2020 3c2f 4f70 7469            </Opti
+00005590: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+000055a0: 3c2f 6461 7461 5f64 6566 696e 6564 5f70  </data_defined_p
+000055b0: 726f 7065 7274 6965 733e 0a20 2020 2020  roperties>.     
+000055c0: 2020 2020 203c 2f6c 6179 6572 3e0a 2020       </layer>.  
+000055d0: 2020 2020 2020 3c2f 7379 6d62 6f6c 3e0a        </symbol>.
+000055e0: 2020 2020 2020 3c2f 6178 6973 5379 6d62        </axisSymb
+000055f0: 6f6c 3e0a 2020 2020 3c2f 4469 6167 7261  ol>.    </Diagra
+00005600: 6d43 6174 6567 6f72 793e 0a20 203c 2f53  mCategory>.  </S
+00005610: 696e 676c 6543 6174 6567 6f72 7944 6961  ingleCategoryDia
+00005620: 6772 616d 5265 6e64 6572 6572 3e0a 2020  gramRenderer>.  
+00005630: 3c44 6961 6772 616d 4c61 7965 7253 6574  <DiagramLayerSet
+00005640: 7469 6e67 7320 7a49 6e64 6578 3d22 3022  tings zIndex="0"
+00005650: 2073 686f 7741 6c6c 3d22 3122 2070 6c61   showAll="1" pla
+00005660: 6365 6d65 6e74 3d22 3222 206c 696e 6550  cement="2" lineP
+00005670: 6c61 6365 6d65 6e74 466c 6167 733d 2231  lacementFlags="1
+00005680: 3822 206f 6273 7461 636c 653d 2230 2220  8" obstacle="0" 
+00005690: 6469 7374 3d22 3022 2070 7269 6f72 6974  dist="0" priorit
+000056a0: 793d 2230 223e 0a20 2020 203c 7072 6f70  y="0">.    <prop
+000056b0: 6572 7469 6573 3e0a 2020 2020 2020 3c4f  erties>.      <O
+000056c0: 7074 696f 6e20 7479 7065 3d22 4d61 7022  ption type="Map"
+000056d0: 3e0a 2020 2020 2020 2020 3c4f 7074 696f  >.        <Optio
+000056e0: 6e20 7661 6c75 653d 2222 206e 616d 653d  n value="" name=
+000056f0: 226e 616d 6522 2074 7970 653d 2251 5374  "name" type="QSt
+00005700: 7269 6e67 222f 3e0a 2020 2020 2020 2020  ring"/>.        
+00005710: 3c4f 7074 696f 6e20 6e61 6d65 3d22 7072  <Option name="pr
+00005720: 6f70 6572 7469 6573 222f 3e0a 2020 2020  operties"/>.    
+00005730: 2020 2020 3c4f 7074 696f 6e20 7661 6c75      <Option valu
+00005740: 653d 2263 6f6c 6c65 6374 696f 6e22 206e  e="collection" n
+00005750: 616d 653d 2274 7970 6522 2074 7970 653d  ame="type" type=
+00005760: 2251 5374 7269 6e67 222f 3e0a 2020 2020  "QString"/>.    
+00005770: 2020 3c2f 4f70 7469 6f6e 3e0a 2020 2020    </Option>.    
+00005780: 3c2f 7072 6f70 6572 7469 6573 3e0a 2020  </properties>.  
+00005790: 3c2f 4469 6167 7261 6d4c 6179 6572 5365  </DiagramLayerSe
+000057a0: 7474 696e 6773 3e0a 2020 3c67 656f 6d65  ttings>.  <geome
+000057b0: 7472 794f 7074 696f 6e73 2072 656d 6f76  tryOptions remov
+000057c0: 6544 7570 6c69 6361 7465 4e6f 6465 733d  eDuplicateNodes=
+000057d0: 2230 2220 6765 6f6d 6574 7279 5072 6563  "0" geometryPrec
+000057e0: 6973 696f 6e3d 2230 223e 0a20 2020 203c  ision="0">.    <
+000057f0: 6163 7469 7665 4368 6563 6b73 2f3e 0a20  activeChecks/>. 
+00005800: 2020 203c 6368 6563 6b43 6f6e 6669 6775     <checkConfigu
+00005810: 7261 7469 6f6e 2f3e 0a20 203c 2f67 656f  ration/>.  </geo
+00005820: 6d65 7472 794f 7074 696f 6e73 3e0a 2020  metryOptions>.  
+00005830: 3c6c 6567 656e 6420 7368 6f77 4c61 6265  <legend showLabe
+00005840: 6c4c 6567 656e 643d 2230 2220 7479 7065  lLegend="0" type
+00005850: 3d22 6465 6661 756c 742d 7665 6374 6f72  ="default-vector
+00005860: 222f 3e0a 2020 3c72 6566 6572 656e 6365  "/>.  <reference
+00005870: 644c 6179 6572 732f 3e0a 2020 3c66 6965  dLayers/>.  <fie
+00005880: 6c64 436f 6e66 6967 7572 6174 696f 6e3e  ldConfiguration>
+00005890: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+000058a0: 3d22 7479 7065 2220 636f 6e66 6967 7572  ="type" configur
+000058b0: 6174 696f 6e46 6c61 6773 3d22 4e6f 6e65  ationFlags="None
+000058c0: 223e 0a20 2020 2020 203c 6564 6974 5769  ">.      <editWi
+000058d0: 6467 6574 2074 7970 653d 2254 6578 7445  dget type="TextE
+000058e0: 6469 7422 3e0a 2020 2020 2020 2020 3c63  dit">.        <c
+000058f0: 6f6e 6669 673e 0a20 2020 2020 2020 2020  onfig>.         
+00005900: 203c 4f70 7469 6f6e 2f3e 0a20 2020 2020   <Option/>.     
+00005910: 2020 203c 2f63 6f6e 6669 673e 0a20 2020     </config>.   
+00005920: 2020 203c 2f65 6469 7457 6964 6765 743e     </editWidget>
+00005930: 0a20 2020 203c 2f66 6965 6c64 3e0a 2020  .    </field>.  
+00005940: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00005950: 736d 5f69 6422 2063 6f6e 6669 6775 7261  sm_id" configura
+00005960: 7469 6f6e 466c 6167 733d 224e 6f6e 6522  tionFlags="None"
+00005970: 3e0a 2020 2020 2020 3c65 6469 7457 6964  >.      <editWid
+00005980: 6765 7420 7479 7065 3d22 5465 7874 4564  get type="TextEd
+00005990: 6974 223e 0a20 2020 2020 2020 203c 636f  it">.        <co
+000059a0: 6e66 6967 3e0a 2020 2020 2020 2020 2020  nfig>.          
+000059b0: 3c4f 7074 696f 6e2f 3e0a 2020 2020 2020  <Option/>.      
+000059c0: 2020 3c2f 636f 6e66 6967 3e0a 2020 2020    </config>.    
+000059d0: 2020 3c2f 6564 6974 5769 6467 6574 3e0a    </editWidget>.
+000059e0: 2020 2020 3c2f 6669 656c 643e 0a20 2020      </field>.   
+000059f0: 203c 6669 656c 6420 6e61 6d65 3d22 6f72   <field name="or
+00005a00: 6965 6e74 6174 696f 6e22 2063 6f6e 6669  ientation" confi
+00005a10: 6775 7261 7469 6f6e 466c 6167 733d 224e  gurationFlags="N
+00005a20: 6f6e 6522 3e0a 2020 2020 2020 3c65 6469  one">.      <edi
+00005a30: 7457 6964 6765 7420 7479 7065 3d22 5465  tWidget type="Te
+00005a40: 7874 4564 6974 223e 0a20 2020 2020 2020  xtEdit">.       
+00005a50: 203c 636f 6e66 6967 3e0a 2020 2020 2020   <config>.      
+00005a60: 2020 2020 3c4f 7074 696f 6e2f 3e0a 2020      <Option/>.  
+00005a70: 2020 2020 2020 3c2f 636f 6e66 6967 3e0a        </config>.
+00005a80: 2020 2020 2020 3c2f 6564 6974 5769 6467        </editWidg
+00005a90: 6574 3e0a 2020 2020 3c2f 6669 656c 643e  et>.    </field>
+00005aa0: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00005ab0: 3d22 6f72 6965 6e74 6174 696f 6e5f 636f  ="orientation_co
+00005ac0: 6e66 6964 656e 6365 2220 636f 6e66 6967  nfidence" config
+00005ad0: 7572 6174 696f 6e46 6c61 6773 3d22 4e6f  urationFlags="No
+00005ae0: 6e65 223e 0a20 2020 2020 203c 6564 6974  ne">.      <edit
+00005af0: 5769 6467 6574 2074 7970 653d 2254 6578  Widget type="Tex
+00005b00: 7445 6469 7422 3e0a 2020 2020 2020 2020  tEdit">.        
+00005b10: 3c63 6f6e 6669 673e 0a20 2020 2020 2020  <config>.       
+00005b20: 2020 203c 4f70 7469 6f6e 2f3e 0a20 2020     <Option/>.   
+00005b30: 2020 2020 203c 2f63 6f6e 6669 673e 0a20       </config>. 
+00005b40: 2020 2020 203c 2f65 6469 7457 6964 6765       </editWidge
+00005b50: 743e 0a20 2020 203c 2f66 6965 6c64 3e0a  t>.    </field>.
+00005b60: 2020 2020 3c66 6965 6c64 206e 616d 653d      <field name=
+00005b70: 226c 616e 655f 7769 6474 6822 2063 6f6e  "lane_width" con
+00005b80: 6669 6775 7261 7469 6f6e 466c 6167 733d  figurationFlags=
+00005b90: 224e 6f6e 6522 3e0a 2020 2020 2020 3c65  "None">.      <e
+00005ba0: 6469 7457 6964 6765 7420 7479 7065 3d22  ditWidget type="
+00005bb0: 5465 7874 4564 6974 223e 0a20 2020 2020  TextEdit">.     
+00005bc0: 2020 203c 636f 6e66 6967 3e0a 2020 2020     <config>.    
+00005bd0: 2020 2020 2020 3c4f 7074 696f 6e2f 3e0a        <Option/>.
+00005be0: 2020 2020 2020 2020 3c2f 636f 6e66 6967          </config
+00005bf0: 3e0a 2020 2020 2020 3c2f 6564 6974 5769  >.      </editWi
+00005c00: 6467 6574 3e0a 2020 2020 3c2f 6669 656c  dget>.    </fiel
+00005c10: 643e 0a20 2020 203c 6669 656c 6420 6e61  d>.    <field na
+00005c20: 6d65 3d22 6c61 6e65 5f6f 7269 656e 7461  me="lane_orienta
+00005c30: 7469 6f6e 2220 636f 6e66 6967 7572 6174  tion" configurat
+00005c40: 696f 6e46 6c61 6773 3d22 4e6f 6e65 223e  ionFlags="None">
+00005c50: 0a20 2020 2020 203c 6564 6974 5769 6467  .      <editWidg
+00005c60: 6574 2074 7970 653d 2254 6578 7445 6469  et type="TextEdi
+00005c70: 7422 3e0a 2020 2020 2020 2020 3c63 6f6e  t">.        <con
+00005c80: 6669 673e 0a20 2020 2020 2020 2020 203c  fig>.          <
+00005c90: 4f70 7469 6f6e 2f3e 0a20 2020 2020 2020  Option/>.       
+00005ca0: 203c 2f63 6f6e 6669 673e 0a20 2020 2020   </config>.     
+00005cb0: 203c 2f65 6469 7457 6964 6765 743e 0a20   </editWidget>. 
+00005cc0: 2020 203c 2f66 6965 6c64 3e0a 2020 3c2f     </field>.  </
+00005cd0: 6669 656c 6443 6f6e 6669 6775 7261 7469  fieldConfigurati
+00005ce0: 6f6e 3e0a 2020 3c61 6c69 6173 6573 3e0a  on>.  <aliases>.
+00005cf0: 2020 2020 3c61 6c69 6173 206e 616d 653d      <alias name=
+00005d00: 2222 2069 6e64 6578 3d22 3022 2066 6965  "" index="0" fie
+00005d10: 6c64 3d22 7479 7065 222f 3e0a 2020 2020  ld="type"/>.    
+00005d20: 3c61 6c69 6173 206e 616d 653d 2222 2069  <alias name="" i
+00005d30: 6e64 6578 3d22 3122 2066 6965 6c64 3d22  ndex="1" field="
+00005d40: 6f73 6d5f 6964 222f 3e0a 2020 2020 3c61  osm_id"/>.    <a
+00005d50: 6c69 6173 206e 616d 653d 2222 2069 6e64  lias name="" ind
+00005d60: 6578 3d22 3222 2066 6965 6c64 3d22 6f72  ex="2" field="or
+00005d70: 6965 6e74 6174 696f 6e22 2f3e 0a20 2020  ientation"/>.   
+00005d80: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
+00005d90: 696e 6465 783d 2233 2220 6669 656c 643d  index="3" field=
+00005da0: 226f 7269 656e 7461 7469 6f6e 5f63 6f6e  "orientation_con
+00005db0: 6669 6465 6e63 6522 2f3e 0a20 2020 203c  fidence"/>.    <
+00005dc0: 616c 6961 7320 6e61 6d65 3d22 2220 696e  alias name="" in
+00005dd0: 6465 783d 2234 2220 6669 656c 643d 226c  dex="4" field="l
+00005de0: 616e 655f 7769 6474 6822 2f3e 0a20 2020  ane_width"/>.   
+00005df0: 203c 616c 6961 7320 6e61 6d65 3d22 2220   <alias name="" 
+00005e00: 696e 6465 783d 2235 2220 6669 656c 643d  index="5" field=
+00005e10: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+00005e20: 6e22 2f3e 0a20 203c 2f61 6c69 6173 6573  n"/>.  </aliases
+00005e30: 3e0a 2020 3c64 6566 6175 6c74 733e 0a20  >.  <defaults>. 
+00005e40: 2020 203c 6465 6661 756c 7420 6669 656c     <default fiel
+00005e50: 643d 2274 7970 6522 2065 7870 7265 7373  d="type" express
+00005e60: 696f 6e3d 2222 2061 7070 6c79 4f6e 5570  ion="" applyOnUp
+00005e70: 6461 7465 3d22 3022 2f3e 0a20 2020 203c  date="0"/>.    <
+00005e80: 6465 6661 756c 7420 6669 656c 643d 226f  default field="o
+00005e90: 736d 5f69 6422 2065 7870 7265 7373 696f  sm_id" expressio
+00005ea0: 6e3d 2222 2061 7070 6c79 4f6e 5570 6461  n="" applyOnUpda
+00005eb0: 7465 3d22 3022 2f3e 0a20 2020 203c 6465  te="0"/>.    <de
+00005ec0: 6661 756c 7420 6669 656c 643d 226f 7269  fault field="ori
+00005ed0: 656e 7461 7469 6f6e 2220 6578 7072 6573  entation" expres
+00005ee0: 7369 6f6e 3d22 2220 6170 706c 794f 6e55  sion="" applyOnU
+00005ef0: 7064 6174 653d 2230 222f 3e0a 2020 2020  pdate="0"/>.    
+00005f00: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
+00005f10: 6f72 6965 6e74 6174 696f 6e5f 636f 6e66  orientation_conf
+00005f20: 6964 656e 6365 2220 6578 7072 6573 7369  idence" expressi
+00005f30: 6f6e 3d22 2220 6170 706c 794f 6e55 7064  on="" applyOnUpd
+00005f40: 6174 653d 2230 222f 3e0a 2020 2020 3c64  ate="0"/>.    <d
+00005f50: 6566 6175 6c74 2066 6965 6c64 3d22 6c61  efault field="la
+00005f60: 6e65 5f77 6964 7468 2220 6578 7072 6573  ne_width" expres
+00005f70: 7369 6f6e 3d22 2220 6170 706c 794f 6e55  sion="" applyOnU
+00005f80: 7064 6174 653d 2230 222f 3e0a 2020 2020  pdate="0"/>.    
+00005f90: 3c64 6566 6175 6c74 2066 6965 6c64 3d22  <default field="
+00005fa0: 6c61 6e65 5f6f 7269 656e 7461 7469 6f6e  lane_orientation
+00005fb0: 2220 6578 7072 6573 7369 6f6e 3d22 2220  " expression="" 
+00005fc0: 6170 706c 794f 6e55 7064 6174 653d 2230  applyOnUpdate="0
+00005fd0: 222f 3e0a 2020 3c2f 6465 6661 756c 7473  "/>.  </defaults
+00005fe0: 3e0a 2020 3c63 6f6e 7374 7261 696e 7473  >.  <constraints
+00005ff0: 3e0a 2020 2020 3c63 6f6e 7374 7261 696e  >.    <constrain
+00006000: 7420 756e 6971 7565 5f73 7472 656e 6774  t unique_strengt
+00006010: 683d 2230 2220 6e6f 746e 756c 6c5f 7374  h="0" notnull_st
+00006020: 7265 6e67 7468 3d22 3022 2065 7870 5f73  rength="0" exp_s
+00006030: 7472 656e 6774 683d 2230 2220 6669 656c  trength="0" fiel
+00006040: 643d 2274 7970 6522 2063 6f6e 7374 7261  d="type" constra
+00006050: 696e 7473 3d22 3022 2f3e 0a20 2020 203c  ints="0"/>.    <
+00006060: 636f 6e73 7472 6169 6e74 2075 6e69 7175  constraint uniqu
+00006070: 655f 7374 7265 6e67 7468 3d22 3022 206e  e_strength="0" n
+00006080: 6f74 6e75 6c6c 5f73 7472 656e 6774 683d  otnull_strength=
+00006090: 2230 2220 6578 705f 7374 7265 6e67 7468  "0" exp_strength
+000060a0: 3d22 3022 2066 6965 6c64 3d22 6f73 6d5f  ="0" field="osm_
+000060b0: 6964 2220 636f 6e73 7472 6169 6e74 733d  id" constraints=
+000060c0: 2230 222f 3e0a 2020 2020 3c63 6f6e 7374  "0"/>.    <const
+000060d0: 7261 696e 7420 756e 6971 7565 5f73 7472  raint unique_str
+000060e0: 656e 6774 683d 2230 2220 6e6f 746e 756c  ength="0" notnul
+000060f0: 6c5f 7374 7265 6e67 7468 3d22 3022 2065  l_strength="0" e
+00006100: 7870 5f73 7472 656e 6774 683d 2230 2220  xp_strength="0" 
+00006110: 6669 656c 643d 226f 7269 656e 7461 7469  field="orientati
+00006120: 6f6e 2220 636f 6e73 7472 6169 6e74 733d  on" constraints=
+00006130: 2230 222f 3e0a 2020 2020 3c63 6f6e 7374  "0"/>.    <const
+00006140: 7261 696e 7420 756e 6971 7565 5f73 7472  raint unique_str
+00006150: 656e 6774 683d 2230 2220 6e6f 746e 756c  ength="0" notnul
+00006160: 6c5f 7374 7265 6e67 7468 3d22 3022 2065  l_strength="0" e
+00006170: 7870 5f73 7472 656e 6774 683d 2230 2220  xp_strength="0" 
+00006180: 6669 656c 643d 226f 7269 656e 7461 7469  field="orientati
+00006190: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2063  on_confidence" c
+000061a0: 6f6e 7374 7261 696e 7473 3d22 3022 2f3e  onstraints="0"/>
+000061b0: 0a20 2020 203c 636f 6e73 7472 6169 6e74  .    <constraint
+000061c0: 2075 6e69 7175 655f 7374 7265 6e67 7468   unique_strength
+000061d0: 3d22 3022 206e 6f74 6e75 6c6c 5f73 7472  ="0" notnull_str
+000061e0: 656e 6774 683d 2230 2220 6578 705f 7374  ength="0" exp_st
+000061f0: 7265 6e67 7468 3d22 3022 2066 6965 6c64  rength="0" field
+00006200: 3d22 6c61 6e65 5f77 6964 7468 2220 636f  ="lane_width" co
+00006210: 6e73 7472 6169 6e74 733d 2230 222f 3e0a  nstraints="0"/>.
+00006220: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+00006230: 756e 6971 7565 5f73 7472 656e 6774 683d  unique_strength=
+00006240: 2230 2220 6e6f 746e 756c 6c5f 7374 7265  "0" notnull_stre
+00006250: 6e67 7468 3d22 3022 2065 7870 5f73 7472  ngth="0" exp_str
+00006260: 656e 6774 683d 2230 2220 6669 656c 643d  ength="0" field=
+00006270: 226c 616e 655f 6f72 6965 6e74 6174 696f  "lane_orientatio
+00006280: 6e22 2063 6f6e 7374 7261 696e 7473 3d22  n" constraints="
+00006290: 3022 2f3e 0a20 203c 2f63 6f6e 7374 7261  0"/>.  </constra
+000062a0: 696e 7473 3e0a 2020 3c63 6f6e 7374 7261  ints>.  <constra
+000062b0: 696e 7445 7870 7265 7373 696f 6e73 3e0a  intExpressions>.
+000062c0: 2020 2020 3c63 6f6e 7374 7261 696e 7420      <constraint 
+000062d0: 6465 7363 3d22 2220 6578 703d 2222 2066  desc="" exp="" f
+000062e0: 6965 6c64 3d22 7479 7065 222f 3e0a 2020  ield="type"/>.  
+000062f0: 2020 3c63 6f6e 7374 7261 696e 7420 6465    <constraint de
+00006300: 7363 3d22 2220 6578 703d 2222 2066 6965  sc="" exp="" fie
+00006310: 6c64 3d22 6f73 6d5f 6964 222f 3e0a 2020  ld="osm_id"/>.  
+00006320: 2020 3c63 6f6e 7374 7261 696e 7420 6465    <constraint de
+00006330: 7363 3d22 2220 6578 703d 2222 2066 6965  sc="" exp="" fie
+00006340: 6c64 3d22 6f72 6965 6e74 6174 696f 6e22  ld="orientation"
+00006350: 2f3e 0a20 2020 203c 636f 6e73 7472 6169  />.    <constrai
+00006360: 6e74 2064 6573 633d 2222 2065 7870 3d22  nt desc="" exp="
+00006370: 2220 6669 656c 643d 226f 7269 656e 7461  " field="orienta
+00006380: 7469 6f6e 5f63 6f6e 6669 6465 6e63 6522  tion_confidence"
+00006390: 2f3e 0a20 2020 203c 636f 6e73 7472 6169  />.    <constrai
+000063a0: 6e74 2064 6573 633d 2222 2065 7870 3d22  nt desc="" exp="
+000063b0: 2220 6669 656c 643d 226c 616e 655f 7769  " field="lane_wi
+000063c0: 6474 6822 2f3e 0a20 2020 203c 636f 6e73  dth"/>.    <cons
+000063d0: 7472 6169 6e74 2064 6573 633d 2222 2065  traint desc="" e
+000063e0: 7870 3d22 2220 6669 656c 643d 226c 616e  xp="" field="lan
+000063f0: 655f 6f72 6965 6e74 6174 696f 6e22 2f3e  e_orientation"/>
+00006400: 0a20 203c 2f63 6f6e 7374 7261 696e 7445  .  </constraintE
+00006410: 7870 7265 7373 696f 6e73 3e0a 2020 3c65  xpressions>.  <e
+00006420: 7870 7265 7373 696f 6e66 6965 6c64 732f  xpressionfields/
+00006430: 3e0a 2020 3c61 7474 7269 6275 7465 6163  >.  <attributeac
+00006440: 7469 6f6e 733e 0a20 2020 203c 6465 6661  tions>.    <defa
+00006450: 756c 7441 6374 696f 6e20 7661 6c75 653d  ultAction value=
+00006460: 227b 3030 3030 3030 3030 2d30 3030 302d  "{00000000-0000-
+00006470: 3030 3030 2d30 3030 302d 3030 3030 3030  0000-0000-000000
+00006480: 3030 3030 3030 7d22 206b 6579 3d22 4361  000000}" key="Ca
+00006490: 6e76 6173 222f 3e0a 2020 3c2f 6174 7472  nvas"/>.  </attr
+000064a0: 6962 7574 6561 6374 696f 6e73 3e0a 2020  ibuteactions>.  
+000064b0: 3c61 7474 7269 6275 7465 7461 626c 6563  <attributetablec
+000064c0: 6f6e 6669 6720 6163 7469 6f6e 5769 6467  onfig actionWidg
+000064d0: 6574 5374 796c 653d 2264 726f 7044 6f77  etStyle="dropDow
+000064e0: 6e22 2073 6f72 744f 7264 6572 3d22 3022  n" sortOrder="0"
+000064f0: 2073 6f72 7445 7870 7265 7373 696f 6e3d   sortExpression=
+00006500: 2222 3e0a 2020 2020 3c63 6f6c 756d 6e73  "">.    <columns
+00006510: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+00006520: 6e61 6d65 3d22 7479 7065 2220 7769 6474  name="type" widt
+00006530: 683d 2233 3737 2220 6869 6464 656e 3d22  h="377" hidden="
+00006540: 3022 2074 7970 653d 2266 6965 6c64 222f  0" type="field"/
+00006550: 3e0a 2020 2020 2020 3c63 6f6c 756d 6e20  >.      <column 
+00006560: 6e61 6d65 3d22 6f73 6d5f 6964 2220 7769  name="osm_id" wi
+00006570: 6474 683d 222d 3122 2068 6964 6465 6e3d  dth="-1" hidden=
+00006580: 2230 2220 7479 7065 3d22 6669 656c 6422  "0" type="field"
+00006590: 2f3e 0a20 2020 2020 203c 636f 6c75 6d6e  />.      <column
+000065a0: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
+000065b0: 6f6e 2220 7769 6474 683d 222d 3122 2068  on" width="-1" h
+000065c0: 6964 6465 6e3d 2230 2220 7479 7065 3d22  idden="0" type="
+000065d0: 6669 656c 6422 2f3e 0a20 2020 2020 203c  field"/>.      <
+000065e0: 636f 6c75 6d6e 206e 616d 653d 226f 7269  column name="ori
+000065f0: 656e 7461 7469 6f6e 5f63 6f6e 6669 6465  entation_confide
+00006600: 6e63 6522 2077 6964 7468 3d22 2d31 2220  nce" width="-1" 
+00006610: 6869 6464 656e 3d22 3022 2074 7970 653d  hidden="0" type=
+00006620: 2266 6965 6c64 222f 3e0a 2020 2020 2020  "field"/>.      
+00006630: 3c63 6f6c 756d 6e20 6e61 6d65 3d22 6c61  <column name="la
+00006640: 6e65 5f6f 7269 656e 7461 7469 6f6e 2220  ne_orientation" 
+00006650: 7769 6474 683d 222d 3122 2068 6964 6465  width="-1" hidde
+00006660: 6e3d 2230 2220 7479 7065 3d22 6669 656c  n="0" type="fiel
+00006670: 6422 2f3e 0a20 2020 2020 203c 636f 6c75  d"/>.      <colu
+00006680: 6d6e 206e 616d 653d 226c 616e 655f 7769  mn name="lane_wi
+00006690: 6474 6822 2077 6964 7468 3d22 2d31 2220  dth" width="-1" 
+000066a0: 6869 6464 656e 3d22 3022 2074 7970 653d  hidden="0" type=
+000066b0: 2266 6965 6c64 222f 3e0a 2020 2020 2020  "field"/>.      
+000066c0: 3c63 6f6c 756d 6e20 7769 6474 683d 222d  <column width="-
+000066d0: 3122 2068 6964 6465 6e3d 2231 2220 7479  1" hidden="1" ty
+000066e0: 7065 3d22 6163 7469 6f6e 7322 2f3e 0a20  pe="actions"/>. 
+000066f0: 2020 203c 2f63 6f6c 756d 6e73 3e0a 2020     </columns>.  
+00006700: 3c2f 6174 7472 6962 7574 6574 6162 6c65  </attributetable
+00006710: 636f 6e66 6967 3e0a 2020 3c63 6f6e 6469  config>.  <condi
+00006720: 7469 6f6e 616c 7374 796c 6573 3e0a 2020  tionalstyles>.  
+00006730: 2020 3c72 6f77 7374 796c 6573 2f3e 0a20    <rowstyles/>. 
+00006740: 2020 203c 6669 656c 6473 7479 6c65 732f     <fieldstyles/
+00006750: 3e0a 2020 3c2f 636f 6e64 6974 696f 6e61  >.  </conditiona
+00006760: 6c73 7479 6c65 733e 0a20 203c 7374 6f72  lstyles>.  <stor
+00006770: 6564 6578 7072 6573 7369 6f6e 732f 3e0a  edexpressions/>.
+00006780: 2020 3c65 6469 7466 6f72 6d20 746f 6c65    <editform tole
+00006790: 7261 6e74 3d22 3122 3e3c 2f65 6469 7466  rant="1"></editf
+000067a0: 6f72 6d3e 0a20 203c 6564 6974 666f 726d  orm>.  <editform
+000067b0: 696e 6974 2f3e 0a20 203c 6564 6974 666f  init/>.  <editfo
+000067c0: 726d 696e 6974 636f 6465 736f 7572 6365  rminitcodesource
+000067d0: 3e30 3c2f 6564 6974 666f 726d 696e 6974  >0</editforminit
+000067e0: 636f 6465 736f 7572 6365 3e0a 2020 3c65  codesource>.  <e
+000067f0: 6469 7466 6f72 6d69 6e69 7466 696c 6570  ditforminitfilep
+00006800: 6174 683e 3c2f 6564 6974 666f 726d 696e  ath></editformin
+00006810: 6974 6669 6c65 7061 7468 3e0a 2020 3c65  itfilepath>.  <e
+00006820: 6469 7466 6f72 6d69 6e69 7463 6f64 653e  ditforminitcode>
+00006830: 3c21 5b43 4441 5441 5b23 202d 2a2d 2063  <![CDATA[# -*- c
+00006840: 6f64 696e 673a 2075 7466 2d38 202d 2a2d  oding: utf-8 -*-
+00006850: 0a22 2222 0a4c 6573 2066 6f72 6d75 6c61  .""".Les formula
+00006860: 6972 6573 2051 4749 5320 7065 7576 656e  ires QGIS peuven
+00006870: 7420 6176 6f69 7220 756e 6520 666f 6e63  t avoir une fonc
+00006880: 7469 6f6e 2050 7974 686f 6e20 7175 6920  tion Python qui 
+00006890: 6573 7420 6170 7065 6cc3 a965 206c 6f72  est appel..e lor
+000068a0: 7371 7565 206c 6520 666f 726d 756c 6169  sque le formulai
+000068b0: 7265 2065 7374 0a6f 7576 6572 742e 0a0a  re est.ouvert...
+000068c0: 5574 696c 6973 657a 2063 6574 7465 2066  Utilisez cette f
+000068d0: 6f6e 6374 696f 6e20 706f 7572 2061 6a6f  onction pour ajo
+000068e0: 7574 6572 2075 6e65 206c 6f67 6971 7565  uter une logique
+000068f0: 2073 7570 706c c3a9 6d65 6e74 6169 7265   suppl..mentaire
+00006900: 20c3 a020 766f 7320 666f 726d 756c 6169   .. vos formulai
+00006910: 7265 732e 0a0a 456e 7472 657a 206c 6520  res...Entrez le 
+00006920: 6e6f 6d20 6465 206c 6120 666f 6e63 7469  nom de la foncti
+00006930: 6f6e 2064 616e 7320 6c65 2063 6861 6d70  on dans le champ
+00006940: 200a 2246 6f6e 6374 696f 6e20 6427 696e   ."Fonction d'in
+00006950: 6974 6961 6c69 7361 7469 6f6e 2050 7974  itialisation Pyt
+00006960: 686f 6e22 2e0a 566f 6963 6920 756e 2065  hon"..Voici un e
+00006970: 7865 6d70 6c65 3a0a 2222 220a 6672 6f6d  xemple:.""".from
+00006980: 2071 6769 732e 5079 5174 2e51 7457 6964   qgis.PyQt.QtWid
+00006990: 6765 7473 2069 6d70 6f72 7420 5157 6964  gets import QWid
+000069a0: 6765 740a 0a64 6566 206d 795f 666f 726d  get..def my_form
+000069b0: 5f6f 7065 6e28 6469 616c 6f67 2c20 6c61  _open(dialog, la
+000069c0: 7965 722c 2066 6561 7475 7265 293a 0a20  yer, feature):. 
+000069d0: 2020 2067 656f 6d20 3d20 6665 6174 7572     geom = featur
+000069e0: 652e 6765 6f6d 6574 7279 2829 0a20 2020  e.geometry().   
+000069f0: 2063 6f6e 7472 6f6c 203d 2064 6961 6c6f   control = dialo
+00006a00: 672e 6669 6e64 4368 696c 6428 5157 6964  g.findChild(QWid
+00006a10: 6765 742c 2022 4d79 4c69 6e65 4564 6974  get, "MyLineEdit
+00006a20: 2229 0a5d 5d3e 3c2f 6564 6974 666f 726d  ").]]></editform
+00006a30: 696e 6974 636f 6465 3e0a 2020 3c66 6561  initcode>.  <fea
+00006a40: 7466 6f72 6d73 7570 7072 6573 733e 303c  tformsuppress>0<
+00006a50: 2f66 6561 7466 6f72 6d73 7570 7072 6573  /featformsuppres
+00006a60: 733e 0a20 203c 6564 6974 6f72 6c61 796f  s>.  <editorlayo
+00006a70: 7574 3e67 656e 6572 6174 6564 6c61 796f  ut>generatedlayo
+00006a80: 7574 3c2f 6564 6974 6f72 6c61 796f 7574  ut</editorlayout
+00006a90: 3e0a 2020 3c65 6469 7461 626c 653e 0a20  >.  <editable>. 
+00006aa0: 2020 203c 6669 656c 6420 6e61 6d65 3d22     <field name="
+00006ab0: 616e 676c 6522 2065 6469 7461 626c 653d  angle" editable=
+00006ac0: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00006ad0: 206e 616d 653d 2266 6964 2220 6564 6974   name="fid" edit
+00006ae0: 6162 6c65 3d22 3122 2f3e 0a20 2020 203c  able="1"/>.    <
+00006af0: 6669 656c 6420 6e61 6d65 3d22 6c61 6e65  field name="lane
+00006b00: 5f6f 7269 656e 7461 7469 6f6e 2220 6564  _orientation" ed
+00006b10: 6974 6162 6c65 3d22 3122 2f3e 0a20 2020  itable="1"/>.   
+00006b20: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
+00006b30: 6e65 5f77 6964 7468 2220 6564 6974 6162  ne_width" editab
+00006b40: 6c65 3d22 3122 2f3e 0a20 2020 203c 6669  le="1"/>.    <fi
+00006b50: 656c 6420 6e61 6d65 3d22 6f72 6965 6e74  eld name="orient
+00006b60: 6174 696f 6e22 2065 6469 7461 626c 653d  ation" editable=
+00006b70: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00006b80: 206e 616d 653d 226f 7269 656e 7461 7469   name="orientati
+00006b90: 6f6e 5f63 6f6e 6669 6465 6e63 6522 2065  on_confidence" e
+00006ba0: 6469 7461 626c 653d 2231 222f 3e0a 2020  ditable="1"/>.  
+00006bb0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00006bc0: 736d 5f69 6422 2065 6469 7461 626c 653d  sm_id" editable=
+00006bd0: 2231 222f 3e0a 2020 2020 3c66 6965 6c64  "1"/>.    <field
+00006be0: 206e 616d 653d 2274 7970 6522 2065 6469   name="type" edi
+00006bf0: 7461 626c 653d 2231 222f 3e0a 2020 3c2f  table="1"/>.  </
+00006c00: 6564 6974 6162 6c65 3e0a 2020 3c6c 6162  editable>.  <lab
+00006c10: 656c 4f6e 546f 703e 0a20 2020 203c 6669  elOnTop>.    <fi
+00006c20: 656c 6420 6e61 6d65 3d22 616e 676c 6522  eld name="angle"
+00006c30: 206c 6162 656c 4f6e 546f 703d 2230 222f   labelOnTop="0"/
+00006c40: 3e0a 2020 2020 3c66 6965 6c64 206e 616d  >.    <field nam
+00006c50: 653d 2266 6964 2220 6c61 6265 6c4f 6e54  e="fid" labelOnT
+00006c60: 6f70 3d22 3022 2f3e 0a20 2020 203c 6669  op="0"/>.    <fi
+00006c70: 656c 6420 6e61 6d65 3d22 6c61 6e65 5f6f  eld name="lane_o
+00006c80: 7269 656e 7461 7469 6f6e 2220 6c61 6265  rientation" labe
+00006c90: 6c4f 6e54 6f70 3d22 3022 2f3e 0a20 2020  lOnTop="0"/>.   
+00006ca0: 203c 6669 656c 6420 6e61 6d65 3d22 6c61   <field name="la
+00006cb0: 6e65 5f77 6964 7468 2220 6c61 6265 6c4f  ne_width" labelO
+00006cc0: 6e54 6f70 3d22 3022 2f3e 0a20 2020 203c  nTop="0"/>.    <
+00006cd0: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
+00006ce0: 6e74 6174 696f 6e22 206c 6162 656c 4f6e  ntation" labelOn
+00006cf0: 546f 703d 2230 222f 3e0a 2020 2020 3c66  Top="0"/>.    <f
+00006d00: 6965 6c64 206e 616d 653d 226f 7269 656e  ield name="orien
+00006d10: 7461 7469 6f6e 5f63 6f6e 6669 6465 6e63  tation_confidenc
+00006d20: 6522 206c 6162 656c 4f6e 546f 703d 2230  e" labelOnTop="0
+00006d30: 222f 3e0a 2020 2020 3c66 6965 6c64 206e  "/>.    <field n
+00006d40: 616d 653d 226f 736d 5f69 6422 206c 6162  ame="osm_id" lab
+00006d50: 656c 4f6e 546f 703d 2230 222f 3e0a 2020  elOnTop="0"/>.  
+00006d60: 2020 3c66 6965 6c64 206e 616d 653d 2274    <field name="t
+00006d70: 7970 6522 206c 6162 656c 4f6e 546f 703d  ype" labelOnTop=
+00006d80: 2230 222f 3e0a 2020 3c2f 6c61 6265 6c4f  "0"/>.  </labelO
+00006d90: 6e54 6f70 3e0a 2020 3c72 6575 7365 4c61  nTop>.  <reuseLa
+00006da0: 7374 5661 6c75 653e 0a20 2020 203c 6669  stValue>.    <fi
+00006db0: 656c 6420 6e61 6d65 3d22 616e 676c 6522  eld name="angle"
+00006dc0: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
+00006dd0: 2230 222f 3e0a 2020 2020 3c66 6965 6c64  "0"/>.    <field
+00006de0: 206e 616d 653d 2266 6964 2220 7265 7573   name="fid" reus
+00006df0: 654c 6173 7456 616c 7565 3d22 3022 2f3e  eLastValue="0"/>
+00006e00: 0a20 2020 203c 6669 656c 6420 6e61 6d65  .    <field name
+00006e10: 3d22 6c61 6e65 5f6f 7269 656e 7461 7469  ="lane_orientati
+00006e20: 6f6e 2220 7265 7573 654c 6173 7456 616c  on" reuseLastVal
+00006e30: 7565 3d22 3022 2f3e 0a20 2020 203c 6669  ue="0"/>.    <fi
+00006e40: 656c 6420 6e61 6d65 3d22 6c61 6e65 5f77  eld name="lane_w
+00006e50: 6964 7468 2220 7265 7573 654c 6173 7456  idth" reuseLastV
+00006e60: 616c 7565 3d22 3022 2f3e 0a20 2020 203c  alue="0"/>.    <
+00006e70: 6669 656c 6420 6e61 6d65 3d22 6f72 6965  field name="orie
+00006e80: 6e74 6174 696f 6e22 2072 6575 7365 4c61  ntation" reuseLa
+00006e90: 7374 5661 6c75 653d 2230 222f 3e0a 2020  stValue="0"/>.  
+00006ea0: 2020 3c66 6965 6c64 206e 616d 653d 226f    <field name="o
+00006eb0: 7269 656e 7461 7469 6f6e 5f63 6f6e 6669  rientation_confi
+00006ec0: 6465 6e63 6522 2072 6575 7365 4c61 7374  dence" reuseLast
+00006ed0: 5661 6c75 653d 2230 222f 3e0a 2020 2020  Value="0"/>.    
+00006ee0: 3c66 6965 6c64 206e 616d 653d 226f 736d  <field name="osm
+00006ef0: 5f69 6422 2072 6575 7365 4c61 7374 5661  _id" reuseLastVa
+00006f00: 6c75 653d 2230 222f 3e0a 2020 2020 3c66  lue="0"/>.    <f
+00006f10: 6965 6c64 206e 616d 653d 2274 7970 6522  ield name="type"
+00006f20: 2072 6575 7365 4c61 7374 5661 6c75 653d   reuseLastValue=
+00006f30: 2230 222f 3e0a 2020 3c2f 7265 7573 654c  "0"/>.  </reuseL
+00006f40: 6173 7456 616c 7565 3e0a 2020 3c64 6174  astValue>.  <dat
+00006f50: 6144 6566 696e 6564 4669 656c 6450 726f  aDefinedFieldPro
+00006f60: 7065 7274 6965 732f 3e0a 2020 3c77 6964  perties/>.  <wid
+00006f70: 6765 7473 2f3e 0a20 203c 7072 6576 6965  gets/>.  <previe
+00006f80: 7745 7870 7265 7373 696f 6e3e 2274 7970  wExpression>"typ
+00006f90: 6522 3c2f 7072 6576 6965 7745 7870 7265  e"</previewExpre
+00006fa0: 7373 696f 6e3e 0a20 203c 6d61 7054 6970  ssion>.  <mapTip
+00006fb0: 3e3c 2f6d 6170 5469 703e 0a20 203c 6c61  ></mapTip>.  <la
+00006fc0: 7965 7247 656f 6d65 7472 7954 7970 653e  yerGeometryType>
+00006fd0: 313c 2f6c 6179 6572 4765 6f6d 6574 7279  1</layerGeometry
+00006fe0: 5479 7065 3e0a 3c2f 7167 6973 3e0a       Type>.</qgis>.
```

### Comparing `crossroads-schematization-0.0.7/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.0.8/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.7/crschem/utils.py` & `crossroads-schematization-0.0.8/crschem/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         m1 = (a1 + a2) / 2
         if m1 > math.pi:
             return m1 - math.pi
         else:
             return m1
 
     
-    def turn_angle(G, n1, n2, n3):
-        c1 = (G.nodes[n1]["x"], G.nodes[n1]["y"])
+    def turn_angle(G, middle, n2, n3):
+        c1 = (G.nodes[middle]["x"], G.nodes[middle]["y"])
         c2 = (G.nodes[n2]["x"], G.nodes[n2]["y"])
         c3 = (G.nodes[n3]["x"], G.nodes[n3]["y"])
         b1 = ox.bearing.calculate_bearing(c2[1], c2[0], c1[1], c1[0])
         b2 = ox.bearing.calculate_bearing(c3[1], c3[0], c1[1], c1[0])
         a = b2 - b1
         if a < 0:
             a += 360
@@ -137,72 +137,99 @@
         return shapely.ops.unary_union(regions)
 
 
     def get_buffered_by_osm(polyline, osm, supplementary_width = 0):
         return Utils.get_edges_buffered_by_osm(zip(polyline, polyline[1:]), osm, supplementary_width)
 
 
-    def evaluate_width_way(gEdge):
-        if "width" in gEdge and not re.match(r'^-?\d+(?:\.\d+)$', gEdge["width"]) is None:
-            return float(gEdge["width"])
-        elif "lanes" in gEdge:
+    def get_adjacent_road_edge(node, osm):
+        for n2 in osm[node]:
+            edge = osm[node][n2][0]
+            if Utils.is_roadway_edge(edge):
+                return edge
+        return None
+
+    def evaluate_way_composition(gEdge):
+        nb_forward = -1
+        nb_backward = -1
+        if "lanes:forward" in gEdge:
+            nb_forward = int(gEdge["lanes:forward"])
+        if "lanes:backward" in gEdge:
+            nb_backward = int(gEdge["lanes:backward"])
+
+        if "lanes" in gEdge:
             nb = int(gEdge["lanes"])
         else:
             if "oneway" in gEdge and gEdge["oneway"]:
                 nb = 1
             else:
                 nb = 2
-        
+
+        if nb_forward == -1:
+            if nb_backward == -1:
+                nb_backward = int(nb/2)
+            nb_forward = nb - nb_backward
+        elif nb_backward == -1:
+                nb_backward = nb - nb_backward
+        else:
+            if nb_backward + nb_forward != nb:
+                print("WARNING: number of lanes not coherent (", nb_backward, "+", nb_forward, "!=", nb)
+
+        # compute width
         if "highway" in gEdge:
             if gEdge["highway"] in ["motorway", "trunk"]:
                 width = 3.5
             elif gEdge["highway"] in ["primary"]:
                 width = 3
             elif gEdge["highway"] in ["secondary"]:
                 width = 3
             elif gEdge["highway"] in ["service"]:
                 width = 2.25
             else:
                 width = 2.75
         else:
             width = 3
-        
-        result = 0
+
         if ("cycleway" in gEdge and gEdge["cycleway"] == "track") or \
             ("cycleway:left" in gEdge and gEdge["cycleway:left"] == "track") or \
             ("cycleway:right" in gEdge and gEdge["cycleway:right"] == "track"):
             nb += 1 # ~ COVID tracks
+
+        return nb_backward, nb_forward, width
+
+    def evaluate_width_way(gEdge):
+        if "width" in gEdge and not re.match(r'^-?\d+(?:\.\d+)$', gEdge["width"]) is None:
+            return float(gEdge["width"])
+
+        nb_lanes_backward, nb_lanes_forward, lane_width = Utils.evaluate_way_composition(gEdge)
+        
+        result = (nb_lanes_backward + nb_lanes_forward) * lane_width
         if ("cycleway:right" in gEdge and gEdge["cycleway:right"] == "lane") or \
            ("cycleway:left" in gEdge and gEdge["cycleway:left"] == "lane"):
             result += 1 # one meter per cycle lane
 
-        result += nb * width
-
         return result
 
-
     def get_initial_node_tags(cr_input, osm_n1):
-        is_n = cr_input["id"] == str(osm_n1)
+        is_n = cr_input["osm_node_id"] == str(osm_n1)
         filtered = cr_input[is_n]
         if len(filtered) > 0:
             return filtered.iloc[0, :].to_dict()
         else:
             return None
 
 
     def get_initial_edge_tags(cr_input, osm_n1, osm_n2, inverse = False):
-        is_w = cr_input["id"] == str(osm_n1) + ";" + str(osm_n2)
-        filtered = cr_input[is_w]
-        if len(filtered) > 0:
-            return filtered.iloc[0, :].to_dict()
+        for index, row in cr_input.iterrows():
+            if row["osm_node_ids"] == [str(osm_n1), str(osm_n2)]:
+                return row.to_dict()
+        if inverse:
+            return Utils.get_initial_edge_tags(cr_input, osm_n1, osm_n2, False)
         else:
-            if inverse:
-                return Utils.get_initial_edge_tags(cr_input, osm_n1, osm_n2, False)
-            else:
-                return None
+            return None
 
 
     def pathid_to_pathcoords(path, osm):
         return [(osm.nodes[n]["x"], osm.nodes[n]["y"]) for n in path]
     
     def edge_in_osm(n1, n2, osm):
         return n1 in osm and n2 in osm[n1]
```

### Comparing `crossroads-schematization-0.0.7/setup.py` & `crossroads-schematization-0.0.8/setup.py`

 * *Files identical despite different names*

