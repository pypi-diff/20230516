# Comparing `tmp/savant_rs-0.1.4.tar.gz` & `tmp/savant_rs-0.1.5.tar.gz`

## Comparing `savant_rs-0.1.4.tar` & `savant_rs-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 savant_rs-0.1.4/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-15 12:21:03.000000 savant_rs-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-15 12:21:03.000000 savant_rs-0.1.4/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-15 12:21:03.000000 savant_rs-0.1.4/LICENSE
--rw-r--r--   0     1001      123      514 2023-05-15 12:21:03.000000 savant_rs-0.1.4/README.md
--rw-r--r--   0     1001      123      769 2023-05-15 12:21:03.000000 savant_rs-0.1.4/benches/batch_snapshot.rs
--rw-r--r--   0     1001      123     1197 2023-05-15 12:21:03.000000 savant_rs-0.1.4/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-15 12:21:03.000000 savant_rs-0.1.4/build.rs
--rw-r--r--   0     1001      123      459 2023-05-15 12:21:03.000000 savant_rs-0.1.4/pyproject.toml
--rw-r--r--   0     1001      123     1790 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/bbox/ops.py
--rw-r--r--   0     1001      123     2533 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/bbox/savant_scale.py
--rw-r--r--   0     1001      123      783 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/buf_copy.py
--rw-r--r--   0     1001      123     3741 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/frame_ops.py
--rw-r--r--   0     1001      123     1108 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/primitives/polygon_match.py
--rw-r--r--   0     1001      123      200 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123      269 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/fps_meter/rust_fps_meter.py
--rw-r--r--   0     1001      123     3515 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/fps_meter/savant_fps_meter.py
--rw-r--r--   0     1001      123     3386 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/symbol_mapper/rust_symbol_mapper.py
--rw-r--r--   0     1001      123     7226 2023-05-15 12:21:03.000000 savant_rs-0.1.4/python/utils/symbol_mapper/savant_symbol_mapper.py
--rw-r--r--   0     1001      123     1018 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/lib.rs
--rw-r--r--   0     1001      123    14160 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/attribute.rs
--rw-r--r--   0     1001      123    15513 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/bbox.rs
--rw-r--r--   0     1001      123     1141 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2141 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1932 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    28830 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    14359 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6710 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/message.rs
--rw-r--r--   0     1001      123      853 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/point.rs
--rw-r--r--   0     1001      123    13870 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     2558 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/segment.rs
--rw-r--r--   0     1001      123       87 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives/to_json_value.rs
--rw-r--r--   0     1001      123     1678 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/primitives.rs
--rw-r--r--   0     1001      123     5863 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/test.rs
--rw-r--r--   0     1001      123     1071 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/test_rkyv_tuple.rs
--rw-r--r--   0     1001      123     2521 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123        1 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils/bounding_box.rs
--rw-r--r--   0     1001      123     5961 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123    21129 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils/symbol_mapper.rs
--rw-r--r--   0     1001      123     2011 2023-05-15 12:21:03.000000 savant_rs-0.1.4/src/utils.rs
--rw-r--r--   0     1001      123    36647 2023-05-15 12:22:28.000000 savant_rs-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 savant_rs-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-16 08:23:57.000000 savant_rs-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-16 08:23:57.000000 savant_rs-0.1.5/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-16 08:23:57.000000 savant_rs-0.1.5/LICENSE
+-rw-r--r--   0     1001      123      514 2023-05-16 08:23:57.000000 savant_rs-0.1.5/README.md
+-rw-r--r--   0     1001      123      769 2023-05-16 08:23:57.000000 savant_rs-0.1.5/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     1197 2023-05-16 08:23:57.000000 savant_rs-0.1.5/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-16 08:23:57.000000 savant_rs-0.1.5/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-16 08:23:57.000000 savant_rs-0.1.5/pyproject.toml
+-rw-r--r--   0     1001      123     2315 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/bbox/ops.py
+-rw-r--r--   0     1001      123     2533 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/bbox/savant_scale.py
+-rw-r--r--   0     1001      123      783 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3741 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1116 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123      269 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123     3386 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/symbol_mapper/rust_symbol_mapper.py
+-rw-r--r--   0     1001      123     7226 2023-05-16 08:23:57.000000 savant_rs-0.1.5/python/utils/symbol_mapper/savant_symbol_mapper.py
+-rw-r--r--   0     1001      123     1018 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      123    14160 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123    16607 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123     1141 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2807 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2141 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1932 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    28830 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123    14359 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6710 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/point.rs
+-rw-r--r--   0     1001      123    14179 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1678 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/primitives.rs
+-rw-r--r--   0     1001      123     5863 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/test.rs
+-rw-r--r--   0     1001      123     1071 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/test_rkyv_tuple.rs
+-rw-r--r--   0     1001      123     2521 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123     5787 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils/bbox.rs
+-rw-r--r--   0     1001      123     5961 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123    21129 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils/symbol_mapper.rs
+-rw-r--r--   0     1001      123     2772 2023-05-16 08:23:57.000000 savant_rs-0.1.5/src/utils.rs
+-rw-r--r--   0     1001      123    37853 2023-05-16 08:25:19.000000 savant_rs-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.5/PKG-INFO
```

### Comparing `savant_rs-0.1.4/Cargo.toml` & `savant_rs-0.1.5/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.4"
+version = "0.1.5"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
@@ -20,15 +20,15 @@
 itertools = "0.10"
 anyhow = "1.0"
 thiserror = "1.0"
 geo = "0.24"
 rayon = "1.7"
 env_logger = "0.10"
 rkyv = { version = "0.7", features = ["validation", "archive_le"] }
-numpy = "0.18"
+numpy = {version = "0.18", features = ["nalgebra"]}
 pyo3-log = "0.8"
 derive_builder = "0.12"
 num_cpus = "1.15"
 hashbrown = "0.13"
 lazy_static = "1.4"
 
 [dependencies.pyo3]
```

### Comparing `savant_rs-0.1.4/.github/workflows/CI.yml` & `savant_rs-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/LICENSE` & `savant_rs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/README.md` & `savant_rs-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/benches/batch_snapshot.rs` & `savant_rs-0.1.5/benches/batch_snapshot.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/benches/message_save_load.rs` & `savant_rs-0.1.5/benches/message_save_load.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/python/primitives/bbox/ops.py` & `savant_rs-0.1.5/python/primitives/bbox/ops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from savant_rs.primitives import BBox, RBBox
+from savant_rs.utils import *
 
 box = BBox(50, 50, 50, 50)
 print("Original bbox:", box)
 print(box.left, box.top, box.bottom, box.right, box.width, box.height)
 box.width = 120
 box.left = 70
 print(box.xc)
@@ -69,8 +70,22 @@
 box = box.wrapping_box
 print("Wrapping box:", box)
 
 # max_x is limited to 100, max_y is limited to 500
 box = box.as_graphical_wrapping_box(padding=5, border_width=2, max_x=100, max_y=500)
 print("Graphical wrapping box:", box)
 
+print(BBox.ltwh(0, 0, 100, 100))
+print(BBox.ltrb(0, 0, 100, 100))
 
+arr = bboxes_to_ndarray_float([BBox(50.0, 50.0, 30.0, 50.0), BBox(70.0, 70.0, 50.0, 50.0)], BBoxFormat.LeftTopRightBottom)
+print(arr)
+
+boxes = ndarray_float_to_bboxes(arr, BBoxFormat.LeftTopRightBottom)
+print(boxes)
+
+
+arr = bboxes_to_ndarray_int([BBox(50.0, 50.0, 30.0, 50.0), BBox(70.0, 70.0, 50.0, 50.0)], BBoxFormat.LeftTopRightBottom)
+print(arr)
+
+boxes = ndarray_int_to_bboxes(arr, BBoxFormat.LeftTopRightBottom)
+print(boxes)
```

### Comparing `savant_rs-0.1.4/python/primitives/bbox/savant_scale.py` & `savant_rs-0.1.5/python/primitives/bbox/savant_scale.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/python/primitives/buf_copy.py` & `savant_rs-0.1.5/python/primitives/buf_copy.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/python/primitives/frame_ops.py` & `savant_rs-0.1.5/python/primitives/frame_ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/python/primitives/polygon_match.py` & `savant_rs-0.1.5/python/primitives/polygon_match.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 for _ in range(10_000):
     res = area.crossed_by_segments(l)
 
 print("Spent", timer() - t)
 pprint(list(zip(l, res)))
 
 r = res[1]
-print(r.kind == IntersectionKind.Cross)
-print(r.edges == [(0, "up"), (2, "down")])
+assert (r.kind == IntersectionKind.Cross)
+assert (r.edges == [(0, "up"), (2, "down")])
 
 r = res[0]
-print(r.kind == IntersectionKind.Cross)
-print(r.edges == [(1, None), (3, None)])
+assert (r.kind == IntersectionKind.Cross)
+assert (r.edges == [(1, None), (3, None)])
```

### Comparing `savant_rs-0.1.4/python/utils/fps_meter/savant_fps_meter.py` & `savant_rs-0.1.5/python/utils/fps_meter/savant_fps_meter.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/python/utils/symbol_mapper/rust_symbol_mapper.py` & `savant_rs-0.1.5/python/utils/symbol_mapper/rust_symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/python/utils/symbol_mapper/savant_symbol_mapper.py` & `savant_rs-0.1.5/python/utils/symbol_mapper/savant_symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/lib.rs` & `savant_rs-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/attribute.rs` & `savant_rs-0.1.5/src/primitives/attribute.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/bbox.rs` & `savant_rs-0.1.5/src/primitives/bbox.rs`

 * *Files 6% similar despite different names*

```diff
@@ -260,14 +260,37 @@
     #[new]
     pub fn new(xc: f64, yc: f64, width: f64, height: f64) -> Self {
         Self {
             rbbox: RBBox::new(xc, yc, width, height, None),
         }
     }
 
+    #[staticmethod]
+    pub fn ltrb(left: f64, top: f64, right: f64, bottom: f64) -> Self {
+        let width = right - left;
+        let height = bottom - top;
+
+        let xc = (left + right) / 2.0;
+        let yc = (top + bottom) / 2.0;
+
+        Self {
+            rbbox: RBBox::new(xc, yc, width, height, None),
+        }
+    }
+
+    #[staticmethod]
+    pub fn ltwh(left: f64, top: f64, width: f64, height: f64) -> Self {
+        let xc = left + width / 2.0;
+        let yc = top + height / 2.0;
+
+        Self {
+            rbbox: RBBox::new(xc, yc, width, height, None),
+        }
+    }
+
     #[getter]
     pub fn get_xc(&self) -> f64 {
         self.rbbox.xc
     }
 
     #[setter]
     pub fn set_xc(&mut self, xc: f64) {
@@ -397,14 +420,30 @@
         let top = self.get_top().floor();
         let left = self.get_left().floor();
         let width = self.get_width().ceil();
         let height = self.get_height().ceil();
         (left as i64, top as i64, width as i64, height as i64)
     }
 
+    pub fn as_xcycwh(&self) -> (f64, f64, f64, f64) {
+        let xc = self.get_xc();
+        let yc = self.get_yc();
+        let width = self.get_width();
+        let height = self.get_height();
+        (xc, yc, width, height)
+    }
+
+    pub fn as_xcycwh_int(&self) -> (i64, i64, i64, i64) {
+        let xc = self.get_xc();
+        let yc = self.get_yc();
+        let width = self.get_width();
+        let height = self.get_height();
+        (xc as i64, yc as i64, width as i64, height as i64)
+    }
+
     pub fn as_rbbox(&self) -> RBBox {
         self.rbbox.clone()
     }
 
     pub fn scale(&mut self, scale_x: f64, scale_y: f64) {
         Python::with_gil(|py| {
             py.allow_threads(|| {
```

### Comparing `savant_rs-0.1.4/src/primitives/message/eos.rs` & `savant_rs-0.1.5/src/primitives/message/eos.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/message/loader.rs` & `savant_rs-0.1.5/src/primitives/message/loader.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/message/saver.rs` & `savant_rs-0.1.5/src/primitives/message/saver.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/message/video/batch.rs` & `savant_rs-0.1.5/src/primitives/message/video/batch.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/message/video/frame.rs` & `savant_rs-0.1.5/src/primitives/message/video/frame.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/message/video/object.rs` & `savant_rs-0.1.5/src/primitives/message/video/object.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/message.rs` & `savant_rs-0.1.5/src/primitives/message.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/point.rs` & `savant_rs-0.1.5/src/primitives/point.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives/polygonal_area.rs` & `savant_rs-0.1.5/src/primitives/polygonal_area.rs`

 * *Files 4% similar despite different names*

```diff
@@ -69,50 +69,60 @@
                 } else {
                     Ok(tags.get(edge).unwrap().clone())
                 }
             }
         }
     }
 
-    pub fn crossed_by_segment(&mut self, seg: &Segment) -> Intersection {
-        self.build_polygon();
-        self.crossed_by_segment_int(seg)
+    #[pyo3(name = "crossed_by_segment")]
+    pub fn crossed_by_segment_py(&mut self, seg: &Segment) -> Intersection {
+        Python::with_gil(|py| {
+            py.allow_threads(|| {
+                self.build_polygon();
+                self.crossed_by_segment(seg)
+            })
+        })
     }
 
     pub fn crossed_by_segments(&mut self, segs: Vec<Segment>) -> Vec<Intersection> {
         Python::with_gil(|py| {
-            self.build_polygon();
             py.allow_threads(|| {
-                segs.iter()
-                    .map(|s| self.crossed_by_segment_int(s))
-                    .collect()
+                self.build_polygon();
+                segs.iter().map(|s| self.crossed_by_segment(s)).collect()
             })
         })
     }
 
-    pub fn contains(&mut self, p: &Point) -> bool {
-        self.build_polygon();
-        self.contains_int(p)
+    #[pyo3(name = "contains")]
+    pub fn contains_py(&mut self, p: &Point) -> bool {
+        Python::with_gil(|py| {
+            py.allow_threads(|| {
+                self.build_polygon();
+                self.contains(p)
+            })
+        })
     }
 
     pub fn contains_many_points(&mut self, points: Vec<Point>) -> Vec<bool> {
         Python::with_gil(|py| {
-            self.build_polygon();
-            py.allow_threads(|| points.iter().map(|p| self.contains_int(p)).collect())
+            py.allow_threads(|| {
+                self.build_polygon();
+                points.iter().map(|p| self.contains(p)).collect()
+            })
         })
     }
 
     #[staticmethod]
     pub fn points_positions(polys: Vec<Self>, points: Vec<Point>) -> Vec<Vec<bool>> {
         let pts = &points;
         polys
             .into_par_iter()
             .map(|mut p| {
                 p.build_polygon();
-                pts.iter().map(|pt| p.contains_int(pt)).collect()
+                pts.iter().map(|pt| p.contains(pt)).collect()
             })
             .collect()
     }
 
     #[staticmethod]
     pub fn segments_intersections(
         polys: Vec<Self>,
@@ -121,23 +131,23 @@
         let segments = &segments;
         polys
             .into_par_iter()
             .map(|mut p| {
                 p.build_polygon();
                 segments
                     .iter()
-                    .map(|seg| p.crossed_by_segment(seg))
+                    .map(|seg| p.crossed_by_segment_py(seg))
                     .collect()
             })
             .collect()
     }
 }
 
 impl PolygonalArea {
-    pub fn crossed_by_segment_int(&mut self, seg: &Segment) -> Intersection {
+    pub fn crossed_by_segment(&mut self, seg: &Segment) -> Intersection {
         let seg = Line::from([(seg.begin.x, seg.begin.y), (seg.end.x, seg.end.y)]);
         let poly = self.polygon.as_ref().unwrap();
 
         let intersections = poly
             .exterior()
             .lines()
             .enumerate()
@@ -158,15 +168,15 @@
             intersections
                 .iter()
                 .map(|i| (*i, self.get_tag(*i).unwrap()))
                 .collect(),
         )
     }
 
-    pub fn contains_int(&self, p: &Point) -> bool {
+    pub fn contains(&self, p: &Point) -> bool {
         self.polygon
             .as_ref()
             .unwrap()
             .contains(&geo::Point::from((p.x, p.y)))
     }
 
     fn gen_polygon(vertices: &[Point]) -> geo::Polygon {
@@ -219,17 +229,17 @@
         let p1 = Point::new(0.0, 0.0);
         let p2 = Point::new(0.99, 0.0);
         let p3 = Point::new(1.0, 0.0);
 
         let mut area1 = PolygonalArea::new(get_square_area(0.0, 0.0, 2.0), None);
         let area2 = PolygonalArea::new(get_square_area(-1.0, 0.0, 2.0), None);
 
-        assert!(area1.contains(&p1));
-        assert!(area1.contains(&p2));
-        assert!(!area1.contains(&p3));
+        assert!(area1.contains_py(&p1));
+        assert!(area1.contains_py(&p2));
+        assert!(!area1.contains_py(&p3));
 
         assert_eq!(
             area1.contains_many_points(vec![p1.clone(), p2.clone(), p3.clone()]),
             vec![true, true, false]
         );
 
         assert_eq!(
@@ -265,15 +275,15 @@
         pyo3::prepare_freethreaded_python();
 
         let area = PolygonalArea::new(get_square_area(0.0, 0.0, 2.0), None);
 
         let bytes = rkyv::to_bytes::<_, 256>(&area).unwrap();
         let area = rkyv::from_bytes::<PolygonalArea>(&bytes[..]).unwrap();
         let p1 = Point::new(0.0, 0.0);
-        assert!(area.clone().contains(&p1));
+        assert!(area.clone().contains_py(&p1));
 
         assert_eq!(
             area.clone().contains_many_points(vec![p1.clone()]),
             vec![true]
         );
 
         assert_eq!(
@@ -288,89 +298,89 @@
 
         let mut area = PolygonalArea::new(
             get_square_area(0.0, 0.0, 2.0),
             Some(vec![Some(UPPER.into()), None, Some(LOWER.into()), None]),
         );
 
         let seg1 = Segment::new(Point::new(0.0, 2.0), Point::new(0.0, 0.0));
-        let res = area.crossed_by_segment(&seg1);
+        let res = area.crossed_by_segment_py(&seg1);
         assert_eq!(
             res,
             Intersection::new(IntersectionKind::Enter, vec![(0, Some(UPPER.into()))])
         );
 
         let seg2 = Segment::new(Point::new(0.0, 0.0), Point::new(0.0, -2.0));
-        let res = area.crossed_by_segment(&seg2);
+        let res = area.crossed_by_segment_py(&seg2);
         assert_eq!(
             res,
             Intersection::new(IntersectionKind::Leave, vec![(2, Some(LOWER.into()))])
         );
 
         let seg3 = Segment::new(Point::new(0.0, 0.0), Point::new(0.0, -0.5));
-        let res = area.crossed_by_segment(&seg3);
+        let res = area.crossed_by_segment_py(&seg3);
         assert_eq!(res, Intersection::new(IntersectionKind::Inside, vec![]));
 
         let seg4 = Segment::new(Point::new(-1.0, 2.0), Point::new(1.0, 2.0));
-        let res = area.crossed_by_segment(&seg4);
+        let res = area.crossed_by_segment_py(&seg4);
         assert_eq!(res, Intersection::new(IntersectionKind::Outside, vec![]));
 
         let seg5 = Segment::new(Point::new(-2.0, 0.0), Point::new(2.0, 0.0));
-        let res = area.crossed_by_segment(&seg5);
+        let res = area.crossed_by_segment_py(&seg5);
         assert_eq!(
             res,
             Intersection::new(IntersectionKind::Cross, vec![(1, None), (3, None)])
         );
 
         let seg6 = Segment::new(Point::new(0.0, 2.0), Point::new(0.0, -2.0));
-        let res = area.crossed_by_segment(&seg6);
+        let res = area.crossed_by_segment_py(&seg6);
         assert_eq!(
             res,
             Intersection::new(
                 IntersectionKind::Cross,
                 vec![(0, Some(UPPER.into())), (2, Some(LOWER.into()))]
             )
         );
 
         let seg7 = Segment::new(Point::new(0.0, 0.0), Point::new(1.0, 1.0));
-        let res = area.crossed_by_segment(&seg7);
+        let res = area.crossed_by_segment_py(&seg7);
         assert_eq!(
             res,
             Intersection::new(
                 IntersectionKind::Inside,
                 vec![(0, Some(UPPER.into())), (1, None)]
             )
         );
 
         let seg8 = Segment::new(Point::new(2.0, 2.0), Point::new(1.0, 1.0));
-        let res = area.crossed_by_segment(&seg8);
+        let res = area.crossed_by_segment_py(&seg8);
         assert_eq!(
             res,
             Intersection::new(
                 IntersectionKind::Enter,
                 vec![(0, Some(UPPER.into())), (1, None)]
             )
         );
 
         let seg9 = Segment::new(Point::new(-1.0, -1.0), Point::new(1.0, 1.0));
-        let res = area.crossed_by_segment(&seg9);
+        let res = area.crossed_by_segment_py(&seg9);
         assert_eq!(
             res,
             Intersection::new(
                 IntersectionKind::Inside,
                 vec![
                     (0, Some(UPPER.into())),
                     (1, None),
                     (2, Some(LOWER.into())),
                     (3, None)
                 ]
             )
         );
 
         let seg9 = Segment::new(Point::new(0.0, 1.0), Point::new(1.0, 0.0));
-        let res = area.crossed_by_segment(&seg9);
+        let res = area.crossed_by_segment_py(&seg9);
         assert_eq!(
             res,
             Intersection::new(
                 IntersectionKind::Inside,
                 vec![(0, Some(UPPER.into())), (1, None),]
             )
         );
```

### Comparing `savant_rs-0.1.4/src/primitives/segment.rs` & `savant_rs-0.1.5/src/primitives/segment.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/primitives.rs` & `savant_rs-0.1.5/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/test.rs` & `savant_rs-0.1.5/src/test.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/test_rkyv_tuple.rs` & `savant_rs-0.1.5/src/test_rkyv_tuple.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/tests_pyo3_access.rs` & `savant_rs-0.1.5/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/utils/fps_meter.rs` & `savant_rs-0.1.5/src/utils/fps_meter.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/src/utils/symbol_mapper.rs` & `savant_rs-0.1.5/src/utils/symbol_mapper.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.4/Cargo.lock` & `savant_rs-0.1.5/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -558,17 +558,17 @@
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
@@ -613,14 +613,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "nalgebra"
+version = "0.32.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d68d47bba83f9e2006d117a9a33af1524e655516b8919caac694427a6fb1e511"
+dependencies = [
+ "approx",
+ "num-complex",
+ "num-rational",
+ "num-traits",
+ "simba",
+ "typenum",
+]
+
+[[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
@@ -645,14 +659,25 @@
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
  "libm",
@@ -671,14 +696,15 @@
 [[package]]
 name = "numpy"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
 dependencies = [
  "libc",
+ "nalgebra",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
@@ -709,14 +735,20 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "paste"
+version = "1.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "pin-utils"
@@ -980,15 +1012,15 @@
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "savant_rs"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
  "hashbrown 0.13.2",
  "itertools",
@@ -1076,14 +1108,26 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.16",
 ]
 
 [[package]]
+name = "simba"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
+dependencies = [
+ "approx",
+ "num-complex",
+ "num-traits",
+ "paste",
+]
+
+[[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "slab"
@@ -1196,14 +1240,20 @@
 [[package]]
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
+name = "typenum"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
```

### Comparing `savant_rs-0.1.4/PKG-INFO` & `savant_rs-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savant_rs
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Savant rust optimization library
 Keywords: computer-vision,video-processing
 Home-Page: https://github.com/insight-platform/savant-rs
```

