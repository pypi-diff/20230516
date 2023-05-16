# Comparing `tmp/dataset-tools-0.0.2.tar.gz` & `tmp/dataset-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-tools-0.0.2.tar", last modified: Sat May 13 11:26:24 2023, max compression
+gzip compressed data, was "dataset-tools-0.0.3.tar", last modified: Tue May 16 12:23:19 2023, max compression
```

## Comparing `dataset-tools-0.0.2.tar` & `dataset-tools-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/object_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-13 11:26:24.000000 dataset-tools-0.0.2/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-13 11:26:24.000000 dataset-tools-0.0.2/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:26:24.000000 dataset-tools-0.0.2/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-13 11:26:24.000000 dataset-tools-0.0.2/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-13 11:26:24.000000 dataset-tools-0.0.2/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 11:26:24.695060 dataset-tools-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-13 11:26:09.000000 dataset-tools-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.570404 dataset-tools-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 12:23:19.570404 dataset-tools-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:23:19.570404 dataset-tools-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/setup.py
```

### Comparing `dataset-tools-0.0.2/LICENSE` & `dataset-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.2/PKG-INFO` & `dataset-tools-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.2/dataset_tools/image/stats/wrapper.py` & `dataset-tools-0.0.3/dataset_tools/image/stats/wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,79 @@
-import random
 import os
+import random
+from typing import Union, List
 
-from collections import defaultdict
+from tqdm import tqdm
 
 import supervisely as sly
 
 
-def sample_images(api, datasets, sample_rate):
-    all_images = []
+def sample_images(
+    api: sly.Api,
+    project: Union[int, str],
+    datasets: List[Union[sly.DatasetInfo, sly.Project.DatasetDict]],
+    sample_rate: float,
+):
+    total = 0
+    samples = []
     for dataset in datasets:
-        images = api.image.get_list(dataset.id)
-        all_images.extend(images)
-
-    cnt_images = len(all_images)
-    if sample_rate != 1:
-        cnt_images = int(max(1, sample_rate * len(all_images)))
-        random.shuffle(all_images)
-        all_images = all_images[:cnt_images]
-
-    ds_images = defaultdict(list)
-    for image_info in all_images:
-        ds_images[image_info.dataset_id].append(image_info)
-    return ds_images, cnt_images
-
-
-def get_sample(images, sample_rate):
-    cnt = int(max(1, sample_rate * len(images)))
-    random.shuffle(images)
-    images = images[:cnt]
-    return images
-
-
-def calculate(api, cfg=None, project_id=None, project_dir=None, sample_rate=0.1):
-    result = {}
-
-    if project_id is not None:
-        meta_json = api.project.get_meta(project_id)
-        meta = sly.ProjectMeta.from_json(meta_json)
-
-        for statsType, Statistics in cfg.items():
-            stats = {}
-            datasets = api.dataset.get_list(project_id)
-            ds_images, sample_count = sample_images(api, datasets, sample_rate)
-
-            Statistics.prepare_data(stats, meta)
-
-            for dataset_id, images in ds_images.items():
-                dataset = api.dataset.get_info_by_id(dataset_id)
-
-                for img_batch in sly.batched(images):
-                    image_ids = [image_info.id for image_info in img_batch]
-                    ann_batch = api.annotation.download_batch(dataset.id, image_ids)
-
-                    for image_info, ann_info in zip(img_batch, ann_batch):
-                        #  maybe *args **kwargs?
-                        Statistics.update(stats, image_info, ann_info, meta, dataset)
-
-            Statistics.aggregate_calculations(stats)
-
-            result[statsType] = stats
-
-    elif project_dir is not None:
-        project_fs = sly.read_single_project(project_dir)
-        meta = project_fs.meta
-
-        for statsType, Statistics in cfg.items():
-            stats = {}
-            datasets = project_fs.datasets
-
-            for dataset in datasets:
-                images = [
-                    dataset.get_image_info(sly.fs.get_file_name(img))
-                    for img in os.listdir(dataset.ann_dir)
-                ]
-                images = get_sample(images, sample_rate) if sample_rate is not None else images
-
-                Statistics.prepare_data(stats, meta)
-
-                for img_batch in sly.batched(images):
-                    image_ids = [image_info.id for image_info in img_batch]
-
-                    ann_batch = api.annotation.download_batch(img_batch[0].dataset_id, image_ids)
-
-                    for image_info, ann_info in zip(img_batch, ann_batch):
-                        #  maybe *args **kwargs?
-                        Statistics.update(stats, image_info, ann_info, meta, dataset)
-
-            Statistics.aggregate_calculations(stats)
-
-            result[statsType] = stats
-
-    return result
+        k = int(
+            max(
+                1,
+                sample_rate
+                * (
+                    dataset.items_count
+                    if isinstance(project, int)
+                    else len(os.listdir(dataset.ann_dir))
+                ),
+            )
+        )
+
+        ds_images = (
+            api.image.get_list(dataset.id)
+            if isinstance(project, int)
+            else [
+                dataset.get_image_info(sly.fs.get_file_name(img))
+                for img in os.listdir(dataset.ann_dir)
+            ]
+        )
+
+        s = random.sample(ds_images, k)
+        samples.append((dataset, s))
+        total += k
+    return samples, total
+
+
+def count_stats(
+    project: Union[int, str], stats: list, sample_rate: float = 1, api: sly.Api = None
+) -> None:
+    if sample_rate <= 0 or sample_rate > 1:
+        raise ValueError("Sample rate has to be in range (0, 1]")
+    if api is None:
+        api = sly.Api.from_env()
+
+    if isinstance(project, int):
+        project_meta = sly.ProjectMeta.from_json(api.project.get_meta(project))
+        datasets = api.dataset.get_list(project)
+    elif isinstance(project, str):
+        project_fs = sly.Project(project, sly.OpenMode.READ)
+        project_meta = project_fs.meta
+        datasets = project_fs.datasets
+    else:
+        raise ValueError("Project should be either an integer project ID or a string project path.")
+
+    samples, total = sample_images(api, project, datasets, sample_rate)
+    desc = "Calculating stats" + (f" [sample={sample_rate}]" if sample_rate != 1 else "")
+    with tqdm(desc=desc, total=total) as pbar:
+        for dataset, images in samples:
+            for batch in sly.batched(images):
+                image_ids = [image.id for image in batch]
+
+                janns = api.annotation.download_json_batch(
+                    (dataset.id if isinstance(project, int) else batch[0].dataset_id), image_ids
+                )
+
+                for img, jann in zip(batch, janns):
+                    ann = sly.Annotation.from_json(jann, project_meta)
+                    for stat in stats:
+                        stat.update(img, ann)
+                    pbar.update(1)
```

### Comparing `dataset-tools-0.0.2/dataset_tools.egg-info/PKG-INFO` & `dataset-tools-0.0.3/dataset_tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.2/setup.py` & `dataset-tools-0.0.3/setup.py`

 * *Files identical despite different names*

