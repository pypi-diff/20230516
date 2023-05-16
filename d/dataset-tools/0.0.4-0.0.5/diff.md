# Comparing `tmp/dataset-tools-0.0.4.tar.gz` & `tmp/dataset-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-tools-0.0.4.tar", last modified: Tue May 16 13:08:08 2023, max compression
+gzip compressed data, was "dataset-tools-0.0.5.tar", last modified: Tue May 16 17:55:00 2023, max compression
```

## Comparing `dataset-tools-0.0.4.tar` & `dataset-tools-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:08:08.584626 dataset-tools-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 13:08:08.584626 dataset-tools-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:08:08.576626 dataset-tools-0.0.4/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:08:08.580626 dataset-tools-0.0.4/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:08:08.580626 dataset-tools-0.0.4/dataset_tools/image/renders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/renders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/renders/poster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/renders/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/renders/separated_anns_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/renders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:08:08.584626 dataset-tools-0.0.4/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/class_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/class_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/object_and_class_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:08:08.576626 dataset-tools-0.0.4/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 13:08:08.000000 dataset-tools-0.0.4/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 13:08:08.000000 dataset-tools-0.0.4/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:08:08.000000 dataset-tools-0.0.4/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-16 13:08:08.000000 dataset-tools-0.0.4/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 13:08:08.000000 dataset-tools-0.0.4/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:08:08.584626 dataset-tools-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-16 13:05:26.000000 dataset-tools-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.185549 dataset-tools-0.0.5/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.185549 dataset-tools-0.0.5/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/basestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:55:00.185549 dataset-tools-0.0.5/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 17:55:00.000000 dataset-tools-0.0.5/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:55:00.189549 dataset-tools-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-16 17:52:17.000000 dataset-tools-0.0.5/setup.py
```

### Comparing `dataset-tools-0.0.4/LICENSE` & `dataset-tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/PKG-INFO` & `dataset-tools-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.4/dataset_tools/__init__.py` & `dataset-tools-0.0.5/dataset_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/dataset_tools/image/renders/poster.py` & `dataset-tools-0.0.5/dataset_tools/image/renders/poster.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/dataset_tools/image/renders/previews.py` & `dataset-tools-0.0.5/dataset_tools/image/renders/previews.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/dataset_tools/image/renders/separated_anns_grid.py` & `dataset-tools-0.0.5/dataset_tools/image/renders/separated_anns_grid.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/dataset_tools/image/renders/wrapper.py` & `dataset-tools-0.0.5/dataset_tools/image/renders/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/dataset_tools/image/stats/class_cooccurrence.py` & `dataset-tools-0.0.5/dataset_tools/image/stats/class_cooccurrence.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from typing import Dict
 
 import dataframe_image as dfi
 import numpy as np
 import pandas as pd
 import supervisely as sly
 
+from dataset_tools.image.stats.basestats import BaseStats
 from supervisely.app.widgets import ConfusionMatrix
 
 
-class ClassCooccurrence:
+class ClassCooccurrence(BaseStats):
     """
     Classes co-occurrence matrix.
     Column names depends on the number of classes
     """
 
     def __init__(self, project_meta: sly.ProjectMeta) -> None:
         self._meta = project_meta
@@ -70,21 +71,12 @@
             "data": data,
             "referencesRow": self._references,
             "options": options,
             "colomnsOptions": colomns_options,
         }
         return res
 
-    def to_pandas(self) -> pd.DataFrame:
-        json = self.to_json()
-        df = pd.DataFrame(data=json["data"], columns=json["columns"])
-        return df
-
-    def to_image(self, path) -> None:
-        df = self.to_pandas()
-        df.dfi.export(path)
-
     def get_widget(self) -> ConfusionMatrix:
         df = pd.DataFrame(data=self.co_occurrence_matrix.tolist(), columns=self._class_names)
         confusion_matrix = ConfusionMatrix()
         confusion_matrix.read_pandas(df)
         return confusion_matrix
```

### Comparing `dataset-tools-0.0.4/dataset_tools/image/stats/classes_per_image.py` & `dataset-tools-0.0.5/dataset_tools/image/stats/classes_per_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import numpy as np
 import pandas as pd
 
 import supervisely as sly
 
+from dataset_tools.image.stats.basestats import BaseStats
+
 UNLABELED_COLOR = [0, 0, 0]
 
 
-class ClassesPerImage:
+class ClassesPerImage(BaseStats):
     """
-    Important fields of modified stats dict:
-        "columns": [],
-        "columnsOptions": [],
-        "data": [],
-        "options": dict
+    Columns:
+        Image
+        dataset
+        height
+        width
+        channels
+        unlabeled
+        class1 objects count
+        class1 covered area (%)
+        class2 objects count
+        class2 covered area (%)
+        etc.
     """
 
     def __init__(self, project_meta: sly.ProjectMeta) -> None:
         self._meta = project_meta
         self._stats = {}
 
         self._class_names = ["unlabeled"]
@@ -63,33 +72,24 @@
             if class_name == "unlabeled":
                 continue
             table_row.append(round(cur_area, 2))
             table_row.append(round(cur_count, 2))
 
         self._stats["data"].append(table_row)
 
-    def to_json(self):
+    def to_json(self) -> dict:
         columns = ["Image", "dataset", "height", "width", "channels", "unlabeled"]
         columns_options = [None] * len(columns)
 
         for obj_class in self._meta.obj_classes:
             columns_options.append({"subtitle": "objects count"})
             columns_options.append({"subtitle": "covered area (%)"})
             columns.extend([obj_class.name] * 2)
 
         options = {"fixColumns": 1}
         res = {
             "columns": columns,
             "columnsOptions": columns_options,
-            "data": self._stats,
+            "data": self._stats["data"],
             "options": options,
         }
         return res
-
-    def to_pandas(self) -> pd.DataFrame:
-        json = self.to_json()
-        table = pd.DataFrame(data=json["data"]["data"], columns=json["columns"])
-        return table
-
-    # def to_image(self, path):
-    #     table = self.to_pandas()
-    #     table.dfi.export(path)
```

### Comparing `dataset-tools-0.0.4/dataset_tools/image/stats/heatmaps_for_classes.py` & `dataset-tools-0.0.5/dataset_tools/image/stats/heatmaps_for_classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import os
 import numpy as np
 from PIL import Image
 import matplotlib.pyplot as plt
 import cv2
 import math
 import supervisely as sly
+from skimage.transform import resize
 
 
 class ClassesHeatmaps:
     def __init__(self, project_meta: sly.ProjectMeta, heatmap_img_size: tuple = None):
         self._meta = project_meta
         self.classname_heatmap = {}
         self._ds_image_sizes = []
         self.heatmap_image_paths = []
 
         if heatmap_img_size:
             self._heatmap_img_size = heatmap_img_size
         else:
-            self._heatmap_img_size = (800, 1200)
+            self._heatmap_img_size = (720, 1280)
 
         for obj_class in self._meta.obj_classes:
             self.classname_heatmap[obj_class.name] = np.zeros(
                 self._heatmap_img_size + (3,), dtype=np.float32
             )
 
     def update(self, image: sly.ImageInfo, ann: sly.Annotation):
@@ -31,39 +33,48 @@
         for label in ann.labels:
             temp_canvas = np.zeros(self._heatmap_img_size + (3,), dtype=np.uint8)
             if label.geometry.geometry_name() in geometry_types_to_heatmap:
                 label.draw(temp_canvas, color=(1, 1, 1))
                 self.classname_heatmap[label.obj_class.name] += temp_canvas
 
     def _create_single_images(self, path):
+        font_height_percent = 5
+        max_text_width = int(self._heatmap_img_size[1] * 0.9)
+        font_height = int(self._heatmap_img_size[0] * font_height_percent / 100)
         for heatmap in self.classname_heatmap:
-            x_pos_center = int(self.classname_heatmap[heatmap].shape[1] * 0.5)
-            y_pos_percent = int(self.classname_heatmap[heatmap].shape[0] * 0.96)
+            resized_image = resize(self.classname_heatmap[heatmap], self._heatmap_img_size)
+            x_pos_center = int(resized_image.shape[1] * 0.5)
+            y_pos_percent = int(resized_image.shape[0] * 0.95)
 
-            image_path = f"{path}/{heatmap}.png"
-            plt.imsave(image_path, self.classname_heatmap[heatmap][:, :, 0])
+            image_path = os.path.join(path, f"{heatmap}.png")
+            plt.imsave(image_path, resized_image[:, :, 0])
 
             image = cv2.imread(image_path)
             text = f"{heatmap}"
             font = cv2.FONT_HERSHEY_SIMPLEX
-            font_scale = 2
             text_color = (255, 255, 255)
+            font_scale = font_height / 10.0
             thickness = 3
             line_type = cv2.LINE_AA
             (text_width, _), _ = cv2.getTextSize(text, font, font_scale, thickness)
+            font_scale = min(font_scale, max_text_width / text_width)
+            if font_scale < 1:
+                thickness = 1
+            (text_width, _), _ = cv2.getTextSize(text, font, font_scale, thickness)
             text_position = (x_pos_center - int(text_width / 2), y_pos_percent)
             cv2.putText(
                 image, text, text_position, font, font_scale, text_color, thickness, line_type
             )
             cv2.imwrite(image_path, image)
 
-            sly.logger.info(f"Heatmap image for class [{heatmap}] created")
+            sly.logger.info(f"Heatmap image for class [{heatmap}] processed")
             self.heatmap_image_paths.append(image_path)
 
     def to_image(self, path, grid_spacing=20, outer_grid_spacing=20):
+        self._calculate_output_img_size()
         self._create_single_images(path)
         img_height, img_width = cv2.imread(self.heatmap_image_paths[0]).shape[:2]
         num_images = len(self.heatmap_image_paths)
         rows = math.ceil(math.sqrt(num_images))
         cols = math.ceil(num_images / rows)
 
         result_width = cols * (img_width + grid_spacing) - grid_spacing + 2 * outer_grid_spacing
@@ -76,18 +87,22 @@
             row = i // cols
             col = i % cols
             x = outer_grid_spacing + col * (img_width + grid_spacing)
             y = outer_grid_spacing + row * (img_height + grid_spacing)
             result_image.paste(img, (x, y))
             sly.api.file_api.silent_remove(img_path)
 
-        save_path = f"{path}/classes_heatmaps.png"
+        save_path = os.path.join(path, "classes_heatmaps.png")
         result_image.save(save_path)
         sly.logger.info(f"Heatmap image for all classes created at {save_path}")
 
     def _calculate_output_img_size(self):
         sizes = np.array(self._ds_image_sizes)
-        self._heatmap_img_size = (
-            np.max(sizes[:, 0]),
-            np.max(sizes[:, 1]),
-        )
+        if np.all(sizes == sizes[0]):
+            self._heatmap_img_size = sizes[0]
+        else:
+            widths = sizes[:, 1]
+            heights = sizes[:, 0]
+            median_width = np.median(widths)
+            median_height = np.median(heights)
+            self._heatmap_img_size = (median_height, median_width)
         sly.logger.info(f"Max size of {self._heatmap_img_size} for heatmaps calculated")
```

### Comparing `dataset-tools-0.0.4/dataset_tools/image/stats/object_and_class_sizes.py` & `dataset-tools-0.0.5/dataset_tools/image/stats/object_and_class_sizes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import defaultdict
+from dataset_tools.image.stats.basestats import BaseStats
 
 import pandas as pd
 import supervisely as sly
 
 
-class ObjectSizes:
+class ObjectSizes(BaseStats):
     def __init__(self, project_meta: sly.ProjectMeta):
         self.project_meta = project_meta
         self._stats = []
 
     def update(self, image: sly.ImageInfo, ann: sly.Annotation):
         image_height, image_width = ann.img_size
 
@@ -56,21 +57,16 @@
             ],
             "data": self._stats,
             "options": options,
         }
 
         return res
 
-    def to_pandas(self):
-        json = self.to_json()
-        table = pd.DataFrame(json["data"], columns=json["columns"])
-        return table
 
-
-class ClassSizes:
+class ClassSizes(BaseStats):
     def __init__(self, project_meta):
         self.project_meta = project_meta
         self._class_titles = [obj_class.name for obj_class in project_meta.obj_classes]
 
         self._stats = []
 
         self._class_heights_px = defaultdict(list)
@@ -203,19 +199,14 @@
             ],
             "data": self._stats,
             "options": options,
         }
 
         return res
 
-    def to_pandas(self):
-        json = self.to_json()
-        table = pd.DataFrame(json["data"], columns=json["columns"])
-        return table
-
 
 def calculate_obj_sizes(label, image_height, image_width):
     image_area = image_height * image_width
 
     rect_geometry = label.geometry.to_bbox()
 
     height_px = rect_geometry.height
```

### Comparing `dataset-tools-0.0.4/dataset_tools/image/stats/objects_distribution.py` & `dataset-tools-0.0.5/dataset_tools/image/stats/objects_distribution.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from collections import defaultdict
+from dataset_tools.image.stats.basestats import BaseStats
 
 import pandas as pd
 import supervisely as sly
 
 
-class ObjectsDistribution:
+class ObjectsDistribution(BaseStats):
     def __init__(self, project_meta: sly.ProjectMeta):
         self.project_meta = project_meta
-        self._stats = defaultdict(lambda: defaultdict(lambda: {"count": 0, "image_ids": []}))
         self._counters = defaultdict(lambda: {"count": 0, "image_ids": []})
         self._class_titles = [obj_class.name for obj_class in project_meta.obj_classes]
+        self._data = []
 
     def update(self, image: sly.ImageInfo, ann: sly.Annotation):
-        for label in ann.labels:
-            class_title = label.obj_class.name
-            self._counters[class_title]["count"] += 1
-            self._counters[class_title]["image_ids"].append(image.id)
-
-        for class_title in self._class_titles:
-            count = self._counters[class_title]["count"]
-            image_ids = self._counters[class_title]["image_ids"]
-            self._stats[class_title][count]["image_ids"].extend(list(set(image_ids)))
-            self._stats[class_title][count]["count"] += 1
+        self._data.append((image, ann))
 
     def to_json(self):
+        self._stats = defaultdict(lambda: defaultdict(lambda: {"count": 0, "image_ids": []}))
+        counters = defaultdict(lambda: {"count": 0, "image_ids": []})
+
+        for image, ann in self._data:
+            image_id = image.id
+            counters = defaultdict(lambda: {"count": 0, "image_ids": []})
+
+            for label in ann.labels:
+                class_title = label.obj_class.name
+                counters[class_title]["count"] += 1
+                counters[class_title]["image_ids"].append(image_id)
+
+            for class_title in self._class_titles:
+                count = counters[class_title]["count"]
+                image_ids = counters[class_title]["image_ids"]
+                self._stats[class_title][count]["image_ids"].extend(list(set(image_ids)))
+                self._stats[class_title][count]["count"] += 1
+
         columns = set()
         for class_title, class_data in self._stats.items():
             columns.update(class_data.keys())
 
         columns = sorted(list(columns))
 
         data = list()
```

### Comparing `dataset-tools-0.0.4/dataset_tools/image/stats/wrapper.py` & `dataset-tools-0.0.5/dataset_tools/image/stats/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/dataset_tools.egg-info/PKG-INFO` & `dataset-tools-0.0.5/dataset_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.4/dataset_tools.egg-info/SOURCES.txt` & `dataset-tools-0.0.5/dataset_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 dataset_tools/image/__init__.py
 dataset_tools/image/renders/__init__.py
 dataset_tools/image/renders/poster.py
 dataset_tools/image/renders/previews.py
 dataset_tools/image/renders/separated_anns_grid.py
 dataset_tools/image/renders/wrapper.py
 dataset_tools/image/stats/__init__.py
+dataset_tools/image/stats/basestats.py
 dataset_tools/image/stats/class_balance.py
 dataset_tools/image/stats/class_cooccurrence.py
 dataset_tools/image/stats/classes_per_image.py
 dataset_tools/image/stats/heatmaps_for_classes.py
 dataset_tools/image/stats/object_and_class_sizes.py
 dataset_tools/image/stats/objects_distribution.py
 dataset_tools/image/stats/wrapper.py
```

### Comparing `dataset-tools-0.0.4/dataset_tools.egg-info/requires.txt` & `dataset-tools-0.0.5/dataset_tools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.4/setup.py` & `dataset-tools-0.0.5/setup.py`

 * *Files identical despite different names*

