# Comparing `tmp/vision6D-0.0.4.tar.gz` & `tmp/vision6D-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.0.4.tar", last modified: Mon May 15 20:59:12 2023, max compression
+gzip compressed data, was "dist\vision6D-0.0.5.tar", last modified: Mon May 15 22:04:22 2023, max compression
```

## Comparing `vision6D-0.0.4.tar` & `vision6D-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:12.086158 vision6D-0.0.4/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1603 2023-05-15 20:59:12.086158 vision6D-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-15 16:36:59.000000 vision6D-0.0.4/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1918 2023-05-15 20:59:12.089158 vision6D-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-01-03 15:55:08.000000 vision6D-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:11.991158 vision6D-0.0.4/test/
--rw-rw-rw-   0        0        0    21974 2023-05-14 22:36:01.000000 vision6D-0.0.4/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.4/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:12.038157 vision6D-0.0.4/vision6D/
--rw-rw-rw-   0        0        0    45496 2023-05-15 16:26:28.000000 vision6D-0.0.4/vision6D/GUI.py
--rw-rw-rw-   0        0        0      963 2023-05-15 20:58:12.000000 vision6D-0.0.4/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.4/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-14 22:36:01.000000 vision6D-0.0.4/vision6D/config.py
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.4/vision6D/interface.py
--rw-rw-rw-   0        0        0    28492 2023-05-14 22:36:02.000000 vision6D-0.0.4/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.4/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0      509 2023-05-14 22:53:44.000000 vision6D-0.0.4/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.4/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.4/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:59:12.084159 vision6D-0.0.4/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-15 20:59:11.000000 vision6D-0.0.4/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-05-15 20:59:11.000000 vision6D-0.0.4/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:59:11.000000 vision6D-0.0.4/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-05-15 20:59:11.000000 vision6D-0.0.4/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 20:59:11.000000 vision6D-0.0.4/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 22:04:22.479818 vision6D-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1603 2023-05-15 22:04:22.479818 vision6D-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-15 16:36:59.000000 vision6D-0.0.5/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1918 2023-05-15 22:04:22.484818 vision6D-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-01-03 15:55:08.000000 vision6D-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:04:22.302818 vision6D-0.0.5/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-14 22:36:01.000000 vision6D-0.0.5/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.5/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:04:22.410819 vision6D-0.0.5/vision6D/
+-rw-rw-rw-   0        0        0    41698 2023-05-15 21:59:15.000000 vision6D-0.0.5/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-15 21:57:24.000000 vision6D-0.0.5/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.5/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-14 22:36:01.000000 vision6D-0.0.5/vision6D/config.py
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.5/vision6D/interface.py
+-rw-rw-rw-   0        0        0    28470 2023-05-15 21:41:46.000000 vision6D-0.0.5/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.5/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0      583 2023-05-15 21:14:52.000000 vision6D-0.0.5/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.5/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.5/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-15 22:04:22.471819 vision6D-0.0.5/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-15 22:04:21.000000 vision6D-0.0.5/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-05-15 22:04:22.000000 vision6D-0.0.5/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 22:04:22.000000 vision6D-0.0.5/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-05-15 22:04:22.000000 vision6D-0.0.5/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-15 22:04:22.000000 vision6D-0.0.5/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.0.4/LICENSE` & `vision6D-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/PKG-INFO` & `vision6D-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.4
+Version: 0.0.5
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.0.4/README.md` & `vision6D-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/setup.cfg` & `vision6D-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 7572  sion = 0.0.4..ur
+00000020: 7369 6f6e 203d 2030 2e30 2e35 0d0a 7572  sion = 0.0.5..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.0.4/test/test_create_dataset.py` & `vision6D-0.0.5/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/test/test_projection.py` & `vision6D-0.0.5/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/vision6D/GUI.py` & `vision6D-0.0.5/vision6D/GUI.py`

 * *Files 11% similar despite different names*

```diff
@@ -185,21 +185,14 @@
         self.file_dialog = QFileDialog()
         
         self.image_path = None
         self.mask_path = None
         self.mesh_path = None
         self.pose_path = None
         self.meshdict = {}
-        
-        os.makedirs(vis.config.GITROOT / "output", exist_ok=True)
-        os.makedirs(vis.config.GITROOT / "output" / "image", exist_ok=True)
-        os.makedirs(vis.config.GITROOT / "output" / "mask", exist_ok=True)
-        os.makedirs(vis.config.GITROOT / "output" / "mesh", exist_ok=True)
-        os.makedirs(vis.config.GITROOT / "output" / "segmesh", exist_ok=True)
-        os.makedirs(vis.config.GITROOT / "output" / "gt_poses", exist_ok=True)
             
         # allow to add files
         fileMenu = mainMenu.addMenu('File')
         fileMenu.addAction('Add Workspace', self.add_workspace)
         fileMenu.addAction('Add Image', self.add_image_file)
         fileMenu.addAction('Add Mask', self.add_mask_file)
         fileMenu.addAction('Add Mesh', self.add_mesh_file)
@@ -511,20 +504,20 @@
         self.render.add_actor(image_actor, pickable=False, name="image")
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
-        mirror = np.any((self.mirror_x, self.mirror_y))
-        output_name = pathlib.Path(self.image_path).stem if not mirror else pathlib.Path(self.image_path).stem + "_mirrored"
-        output_path = vis.config.GITROOT / "output" / "image" / (output_name + '.png')
-        rendered_image = PIL.Image.fromarray(image)
-        rendered_image.save(output_path)
-        self.output_text.clear(); self.output_text.append(f"Export image render to:\n {str(output_path)}")
+        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
+        if output_path: 
+            rendered_image = PIL.Image.fromarray(image)
+            rendered_image.save(output_path)
+            self.output_text.clear()
+            self.output_text.append(f"Export image render to:\n {str(output_path)}")
 
     def export_mask_plot(self):
         if self.mask_actor is None:
             QMessageBox.warning(self, 'vision6D', "Need to load a mask first!", QMessageBox.Ok, QMessageBox.Ok)
             return 0
         
         reply = QMessageBox.question(self,"vision6D", "Reset Camera?", QMessageBox.Yes, QMessageBox.No)
@@ -537,22 +530,22 @@
         self.render.add_actor(mask_actor, pickable=False, name="mask")
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
-        mirror = np.any((self.mirror_x, self.mirror_y))
-        output_name = pathlib.Path(self.mask_path).stem if not mirror else pathlib.Path(self.mask_path).stem + "_mirrored"
-        output_path = vis.config.GITROOT / "output" / "mask" / (output_name + '.png')
-        rendered_image = PIL.Image.fromarray(image)
-        rendered_image.save(output_path)
-        self.output_text.clear(); self.output_text.append(f"Export mask render to:\n {str(output_path)}")
+        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
+        if output_path:
+            rendered_image = PIL.Image.fromarray(image)
+            rendered_image.save(output_path)
+            self.output_text.clear()
+            self.output_text.append(f"Export mask render to:\n {str(output_path)}")
 
-    def export_mesh_plot(self, reply_reset_camera=None, reply_render_mesh=None, reply_export_surface=None, msg=True, save_render=True):
+    def export_mesh_plot(self, reply_reset_camera=None, reply_render_mesh=None, reply_export_surface=None, save_render=True):
 
         if self.reference is None:
             QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QMessageBox.Ok, QMessageBox.Ok)
             return 0
 
         if reply_reset_camera is None and reply_render_mesh is None and reply_export_surface is None:
             reply_reset_camera = QMessageBox.question(self,"vision6D", "Reset Camera?", QMessageBox.Yes, QMessageBox.No)
@@ -562,72 +555,46 @@
         if reply_reset_camera == QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
         if reply_render_mesh == QMessageBox.No: render_all_meshes = True
         else: render_all_meshes = False
         if reply_export_surface == QMessageBox.No: point_clouds = True
         else: point_clouds = False
         
+        # Clear out the render
         self.render.clear()
-        reference_name = pathlib.Path(self.meshdict[self.reference]).stem
-
-        mirror = np.any((self.mirror_x, self.mirror_y))
-        if self.image_actor is not None: 
-            id = pathlib.Path(self.image_path).stem.split('_')[-1]
-            output_name = reference_name + f'_render_{id}' if not mirror else reference_name + f'_mirrored_render_{id}'
-        else:
-            output_name = reference_name + '_render' if not mirror else reference_name + '_mirrored_render'
 
-        # Render all objects 
-        if render_all_meshes:
-            for mesh_name, mesh_actor in self.mesh_actors.items():
-                vertices, faces = vis.utils.get_mesh_actor_vertices_faces(mesh_actor)
-                mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
-
-                colors = vis.utils.get_mesh_actor_scalars(mesh_actor)
-                if colors is not None: 
-                    assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
-                    mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
-                else:
-                    mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
-
-                mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
-
-            self.render.camera = camera
-            self.render.disable(); self.render.show(auto_close=False)
-
-            # obtain the rendered image
-            image = self.render.last_image
-            output_path = vis.config.GITROOT / "output" / "mesh" / (output_name + ".png")
-            rendered_image = PIL.Image.fromarray(image)
-            rendered_image.save(output_path)
-            if msg: self.output_text.clear(); self.output_text.append(f"Export all meshes render to:\n {str(output_path)}")
-        # render the reference mesh only
-        else:
-            mesh_actor = self.mesh_actors[self.reference]
+        for mesh_name, mesh_actor in self.mesh_actors.items():
+            if not render_all_meshes:
+                if mesh_name != self.reference:
+                    continue
             vertices, faces = vis.utils.get_mesh_actor_vertices_faces(mesh_actor)
             mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
             colors = vis.utils.get_mesh_actor_scalars(mesh_actor)
             if colors is not None: 
                 assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
-                mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=self.reference) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=self.reference)
+                mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
             else:
-                mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[self.reference], style='surface', opacity=1, name=self.reference) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[self.reference], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=self.reference)
+                mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
             mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
-            self.render.camera = camera
-            self.render.disable(); self.render.show(auto_close=False)
+      
+        self.render.camera = camera
+        self.render.disable(); self.render.show(auto_close=False)
+
+        # obtain the rendered image
+        image = self.render.last_image
 
-            # obtain the rendered image
-            image = self.render.last_image
-            if save_render:
-                output_path = vis.config.GITROOT / "output" / "mesh" / (output_name + ".png")
+        if save_render:
+            output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
+            if output_path:
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
-            if msg: self.output_text.clear(); self.output_text.append(f"Export reference mesh render to:\n {str(output_path)}")
+                self.output_text.clear()
+                self.output_text.append(f"Export reference mesh render to:\n {str(output_path)}")
 
-            return image
+        return image
 
     def export_segmesh_plot(self):
 
         if self.reference is None:
             QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QMessageBox.Ok, QMessageBox.Ok)
             return 0
         
@@ -650,23 +617,15 @@
         self.render.camera = camera
         self.render.disable()
         self.render.show(auto_close=False)
         segmask = self.render.last_image
         if np.max(segmask) > 1: segmask = segmask / 255
 
         self.render.clear()
-        reference_name = pathlib.Path(self.meshdict[self.reference]).stem
-
-        mirror = np.any((self.mirror_x, self.mirror_y))
-        if self.image_actor is not None: 
-            id = pathlib.Path(self.image_path).stem.split('_')[-1]
-            output_name = reference_name + f'_render_{id}' if not mirror else reference_name + f'_mirrored_render_{id}'
-        else:
-            output_name = reference_name + '_render' if not mirror else reference_name + '_mirrored_render'
-        
+                
         # Render the targeting objects
         vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
         mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
         colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
         if colors is not None: 
             assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
             mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=self.reference) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=self.reference)
@@ -677,39 +636,33 @@
 
         self.render.camera = camera
         self.render.disable(); self.render.show(auto_close=False)
 
         # obtain the rendered image
         image = self.render.last_image
         image = (image * segmask).astype(np.uint8)
-        output_path = vis.config.GITROOT / "output" / "segmesh" / (output_name + ".png")
-        rendered_image = PIL.Image.fromarray(image)
-        rendered_image.save(output_path)
-        self.output_text.clear(); self.output_text.append(f"Export segmask render:\n to {str(output_path)}")
-        
-        return image
+        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
+        if output_path:
+            rendered_image = PIL.Image.fromarray(image)
+            rendered_image.save(output_path)
+            self.output_text.clear()
+            self.output_text.append(f"Export segmask render:\n to {str(output_path)}")
+            
+        # return image
 
     def export_pose(self):
         if self.reference is None: 
             QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QMessageBox.Ok, QMessageBox.Ok)
             return 0
-        
         self.update_gt_pose()
-
-        mesh_path_name = pathlib.Path(self.mesh_path).stem.split('_')
-        
-        mirror = np.any((self.mirror_x, self.mirror_y))
-        if self.image_actor is not None: 
-            id = pathlib.Path(self.image_path).stem.split('_')[-1]
-            output_name = "_".join(mesh_path_name[:2]) + f'_gt_pose_{id}' if not mirror else "_".join(mesh_path_name[:2]) + f'_mirrored_gt_pose_{id}'
-        else: output_name = "_".join(mesh_path_name[:2]) + '_gt_pose' if not mirror else "_".join(mesh_path_name[:2]) + f'_mirrored_gt_pose'
-
-        output_path = vis.config.GITROOT / "output" / "gt_poses" / (output_name + ".npy")
-        np.save(output_path, self.transformation_matrix)
-        self.output_text.clear(); self.output_text.append(f"\nSaved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
+        output_path, _ = QFileDialog.getSaveFileName(self, "Save File", "", "Pose Files (*.npy)")
+        if output_path:
+            np.save(output_path, self.transformation_matrix)
+            self.output_text.clear()
+            self.output_text.append(f"\nSaved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
 
     # ^Panel
     def set_panel_bar(self):
         # Create a left panel layout
         self.panel_widget = QtWidgets.QWidget()
         self.panel_layout = QtWidgets.QVBoxLayout(self.panel_widget)
```

### Comparing `vision6D-0.0.4/vision6D/__init__.py` & `vision6D-0.0.5/vision6D/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 # Setup the logging configuration
 logging.config.dictConfig(LOGGING_CONFIG)
 
 from .app import App
 from .interface import Interface
 from .interface_gui import Interface_GUI
 from . import utils
-# from . import config
 from .run_gui import exe
```

### Comparing `vision6D-0.0.4/vision6D/app.py` & `vision6D-0.0.5/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/vision6D/config.py` & `vision6D-0.0.5/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/vision6D/interface.py` & `vision6D-0.0.5/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/vision6D/interface_gui.py` & `vision6D-0.0.5/vision6D/interface_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
     def epnp_mesh(self):
         if self.reference is not None:
             colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
             if colors is None or (np.all(colors == colors[0])):
                 QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QMessageBox.Ok, QMessageBox.Ok)
                 return 0
-            color_mask = self.export_mesh_plot(QMessageBox.Yes, QMessageBox.Yes, QMessageBox.Yes, msg=False, save_render=False)
+            color_mask = self.export_mesh_plot(QMessageBox.Yes, QMessageBox.Yes, QMessageBox.Yes, save_render=False)
             gt_pose = self.mesh_actors[self.reference].user_matrix
             if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
             if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
 
             if np.sum(color_mask) == 0:
                 QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QMessageBox.Ok, QMessageBox.Ok)
                 return 0
@@ -461,15 +461,15 @@
             # binary mask
             if np.all(np.logical_or(mask_data == 0, mask_data == 1)):
                 if self.reference is not None:
                     colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
                     if colors is None or (np.all(colors == colors[0])):
                         QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QMessageBox.Ok, QMessageBox.Ok)
                         return 0
-                    color_mask = self.export_mesh_plot(QMessageBox.Yes, QMessageBox.Yes, QMessageBox.Yes, msg=False, save_render=False)
+                    color_mask = self.export_mesh_plot(QMessageBox.Yes, QMessageBox.Yes, QMessageBox.Yes, save_render=False)
                     # nocs_color = False if np.sum(color_mask[..., 2]) == 0 else True
                     nocs_color = (self.mesh_colors[self.reference] == 'nocs')
                     gt_pose = self.mesh_actors[self.reference].user_matrix
                     if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
                     if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
                     vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
                     mesh = trimesh.Trimesh(vertices, faces, process=False)
```

### Comparing `vision6D-0.0.4/vision6D/mainwindow.py` & `vision6D-0.0.5/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/vision6D/utils.py` & `vision6D-0.0.5/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.4/vision6D.egg-info/PKG-INFO` & `vision6D-0.0.5/vision6D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.4
+Version: 0.0.5
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

