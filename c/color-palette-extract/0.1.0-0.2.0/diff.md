# Comparing `tmp/color_palette_extract-0.1.0.tar.gz` & `tmp/color_palette_extract-0.2.0.tar.gz`

## Comparing `color_palette_extract-0.1.0.tar` & `color_palette_extract-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 color_palette_extract-0.1.0/Cargo.toml
--rwxr-xr-x   0     1001      123      242 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/.github/workflows/build-wheels.sh
--rw-r--r--   0     1001      123     2835 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/.github/workflows/build.yml
--rw-r--r--   0     1001      123      685 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/.gitignore
--rw-r--r--   0     1001      123       24 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/README.md
--rw-r--r--   0     1001      123      329 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      433 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/run.py
--rw-r--r--   0     1001      123      892 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     6155 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/airbnb.png
--rw-r--r--   0     1001      123  1152390 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/instagram.png
--rw-r--r--   0     1001      123     8948 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/instagram.svg
--rw-r--r--   0     1001      123    10752 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/mastercard.webp
--rw-r--r--   0     1001      123    49709 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/test.jpg
--rw-r--r--   0     1001      123     5286 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/test2.png
--rw-r--r--   0     1001      123     2557 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/test/test3.jpeg
--rw-r--r--   0     1001      123    32261 2023-05-16 08:09:58.000000 color_palette_extract-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 color_palette_extract-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 color_palette_extract-0.2.0/Cargo.toml
+-rwxr-xr-x   0     1001      123      242 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/.github/workflows/build-wheels.sh
+-rw-r--r--   0     1001      123     2835 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0     1001      123      685 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/.gitignore
+-rw-r--r--   0     1001      123       24 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/README.md
+-rw-r--r--   0     1001      123      329 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      292 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/run.py
+-rw-r--r--   0     1001      123     1054 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     6155 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/airbnb.png
+-rw-r--r--   0     1001      123  1152390 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/instagram.png
+-rw-r--r--   0     1001      123     8948 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/instagram.svg
+-rw-r--r--   0     1001      123    10752 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/mastercard.webp
+-rw-r--r--   0     1001      123    49709 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/test.jpg
+-rw-r--r--   0     1001      123     5286 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/test2.png
+-rw-r--r--   0     1001      123     2557 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/test/test3.jpeg
+-rw-r--r--   0     1001      123    32261 2023-05-16 08:53:49.000000 color_palette_extract-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 color_palette_extract-0.2.0/PKG-INFO
```

### Comparing `color_palette_extract-0.1.0/.github/workflows/build.yml` & `color_palette_extract-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/.gitignore` & `color_palette_extract-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/src/lib.rs` & `color_palette_extract-0.2.0/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 
 use colors_transform::Rgb;
 use pyo3::wrap_pyfunction;
 
 #[pyfunction]
-fn extract_from_bytes(data: &PyBytes) -> PyResult<Vec<String>> {
-    let mut result: Vec<String> = Vec::new();
+fn extract_from_bytes(data: &PyBytes) -> PyResult<Vec<Vec<f32>>> {
+    let mut result: Vec<Vec<f32>> = Vec::new();
 
     let img = image::load_from_memory(data.as_bytes()).unwrap();
 
     let colors = dominant_color::get_colors(img.to_rgb8().into_raw().as_slice(), false);
 
     let mut group: Vec<f32> = Vec::new();
     for color in colors {
         group.push(color as f32);
         if group.len() == 3 {
-            let rgb = Rgb::from(group[0], group[1], group[2]);
+            result.push(vec![group[0], group[1], group[2]]);
             group.clear();
-            result.push(rgb.to_css_hex_string());
         }
     }
 
     Ok(result)
 }
 
+#[pyfunction]
+fn get_hex_from_rgb(r: f32, g: f32, b: f32) -> PyResult<String> {
+    let rgb = Rgb::from(r, g, b);
+    Ok(rgb.to_css_hex_string())
+}
+
 /// A Python module implemented in Rust.
 #[pymodule]
 fn color_palette_extract(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(extract_from_bytes, m)?)?;
+    m.add_function(wrap_pyfunction!(get_hex_from_rgb, m)?)?;
     Ok(())
 }
```

### Comparing `color_palette_extract-0.1.0/test/airbnb.png` & `color_palette_extract-0.2.0/test/airbnb.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/test/instagram.png` & `color_palette_extract-0.2.0/test/instagram.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/test/instagram.svg` & `color_palette_extract-0.2.0/test/instagram.svg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/test/mastercard.webp` & `color_palette_extract-0.2.0/test/mastercard.webp`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/test/test.jpg` & `color_palette_extract-0.2.0/test/test.jpg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/test/test2.png` & `color_palette_extract-0.2.0/test/test2.png`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/test/test3.jpeg` & `color_palette_extract-0.2.0/test/test3.jpeg`

 * *Files identical despite different names*

### Comparing `color_palette_extract-0.1.0/Cargo.lock` & `color_palette_extract-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "color_palette_extract"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "colors-transform",
  "dominant_color",
  "image",
  "pyo3",
  "pyo3-file",
 ]
```

