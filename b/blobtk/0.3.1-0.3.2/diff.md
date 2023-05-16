# Comparing `tmp/blobtk-0.3.1.tar.gz` & `tmp/blobtk-0.3.2.tar.gz`

## Comparing `blobtk-0.3.1.tar` & `blobtk-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 blobtk-0.3.1/Cargo.toml
--rw-r--r--   0      501       20    59715 2023-05-04 13:21:58.000000 blobtk-0.3.1/Cargo.lock
--rw-r--r--   0      501       20      313 2023-05-04 13:21:58.000000 blobtk-0.3.1/pyproject.toml
--rw-r--r--   0      501       20     9018 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/bam.rs
--rw-r--r--   0      501       20    16853 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/blobdir.rs
--rw-r--r--   0      501       20     7517 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/cli.rs
--rw-r--r--   0      501       20      553 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/depth.rs
--rw-r--r--   0      501       20     1855 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/fasta.rs
--rw-r--r--   0      501       20     6177 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/fastq.rs
--rw-r--r--   0      501       20     1440 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/filter.rs
--rw-r--r--   0      501       20     2738 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/io.rs
--rw-r--r--   0      501       20      788 2023-05-04 13:21:58.000000 blobtk-0.3.1/src/lib.rs
--rw-r--r--   0      501       20      659 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/main.rs
--rw-r--r--   0      501       20     4015 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/axis.rs
--rw-r--r--   0      501       20    16954 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/blob.rs
--rw-r--r--   0      501       20     2888 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/category.rs
--rw-r--r--   0      501       20     4029 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/chart.rs
--rw-r--r--   0      501       20    34843 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/component.rs
--rw-r--r--   0      501       20     2928 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/data.rs
--rw-r--r--   0      501       20    29455 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/snail.rs
--rw-r--r--   0      501       20     1020 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot/style.rs
--rw-r--r--   0      501       20     9156 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/plot.rs
--rw-r--r--   0      501       20     3172 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python/depth.rs
--rw-r--r--   0      501       20     3518 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python/filter.rs
--rw-r--r--   0      501       20     1879 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python/utils.rs
--rw-r--r--   0      501       20      491 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/python.rs
--rw-r--r--   0      501       20     4497 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/taxonomy.rs
--rw-r--r--   0      501       20     7612 2023-05-04 13:21:59.000000 blobtk-0.3.1/src/utils.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 blobtk-0.3.2/Cargo.toml
+-rw-r--r--   0      501       20    59960 2023-05-16 08:39:04.000000 blobtk-0.3.2/Cargo.lock
+-rw-r--r--   0      501       20      313 2023-05-16 08:39:04.000000 blobtk-0.3.2/pyproject.toml
+-rw-r--r--   0      501       20     9018 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/bam.rs
+-rw-r--r--   0      501       20    18205 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/blobdir.rs
+-rw-r--r--   0      501       20     8832 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/cli.rs
+-rw-r--r--   0      501       20      553 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/depth.rs
+-rw-r--r--   0      501       20     1855 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/fasta.rs
+-rw-r--r--   0      501       20     6177 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/fastq.rs
+-rw-r--r--   0      501       20     1440 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/filter.rs
+-rw-r--r--   0      501       20     2738 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/io.rs
+-rw-r--r--   0      501       20      788 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/lib.rs
+-rw-r--r--   0      501       20      659 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/main.rs
+-rw-r--r--   0      501       20     4150 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/axis.rs
+-rw-r--r--   0      501       20    22218 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/blob.rs
+-rw-r--r--   0      501       20     5567 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/category.rs
+-rw-r--r--   0      501       20     5730 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/chart.rs
+-rw-r--r--   0      501       20    38034 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/component.rs
+-rw-r--r--   0      501       20     5835 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/cumulative.rs
+-rw-r--r--   0      501       20     4398 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/data.rs
+-rw-r--r--   0      501       20    29932 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/snail.rs
+-rw-r--r--   0      501       20     1020 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot/style.rs
+-rw-r--r--   0      501       20    11606 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/plot.rs
+-rw-r--r--   0      501       20     3172 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python/depth.rs
+-rw-r--r--   0      501       20     3518 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python/filter.rs
+-rw-r--r--   0      501       20     1879 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python/utils.rs
+-rw-r--r--   0      501       20      491 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/python.rs
+-rw-r--r--   0      501       20     4497 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/taxonomy.rs
+-rw-r--r--   0      501       20     8053 2023-05-16 08:39:04.000000 blobtk-0.3.2/src/utils.rs
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.2/PKG-INFO
```

### Comparing `blobtk-0.3.1/Cargo.toml` & `blobtk-0.3.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "blobtk"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 authors = [
     "Rich Challis <rc28@sanger.ac.uk>",
 ]
 license = "MIT"
 description = "Core utilities for BlobToolKit."
 homepage = "https://github.com/blobtoolkit/blobtk"
@@ -28,21 +28,22 @@
 lto = true
 codegen-units = 1
 panic = "abort"
 
 [dependencies]
 atty = "0.2.14"
 clap = { version = "4.0.29", features = [ "derive" ]}
+clap-num = "1.0.2"
 colorous = "1.0.10"
 coord_transforms = "1.4.0"
 flate2 = "1.0.25"
 glob = "0.3.1"
 indexmap = "1.9.2"
 indicatif = "0.17.2"
-needletail = "0.5.0"
+needletail = "0.5.1"
 num-integer = "0.1.45"
 pyo3 = { version = "0.18.1", features = ["extension-module"] }
 regex = "1.7.0"
 resvg = "0.31.0"
 rust-htslib = "0.40.2"
 rust_decimal = "1.29.1"
 serde = { version = "1.0.152", features= ["derive"] }
```

### Comparing `blobtk-0.3.1/Cargo.lock` & `blobtk-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -104,18 +104,19 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blobtk"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "atty",
  "clap",
+ "clap-num",
  "colorous",
  "coord_transforms",
  "flate2",
  "glob",
  "indexmap",
  "indicatif",
  "needletail",
@@ -179,18 +180,18 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
-name = "buf_redux"
-version = "0.8.4"
+name = "buffer-redux"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b953a6887648bb07a535631f2bc00fbdb2a2216f135552cb3f534ed136b9c07f"
+checksum = "d2886ea01509598caac116942abd33ab5a88fa32acdf7e4abfa0fc489ca520c9"
 dependencies = [
  "memchr",
  "safemem",
 ]
 
 [[package]]
 name = "bumpalo"
@@ -305,14 +306,23 @@
  "is-terminal",
  "once_cell",
  "strsim",
  "termcolor",
 ]
 
 [[package]]
+name = "clap-num"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "488557e97528174edaa2ee268b23a809e0c598213a4bbcb4f34575a46fda147e"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "clap_derive"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "684a277d672e91966334af371f1a7b5833f9aa00b07c84e92fbce95e00208ce8"
 dependencies = [
  "heck",
  "proc-macro-error",
@@ -997,19 +1007,19 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "needletail"
-version = "0.5.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50a9c08c2fd39675e80652857b6d609b5ebe8f6dc72ab62b69faef8838afd3df"
+checksum = "db05a5ab397f64070d8c998fa0fbb84e484b81f95752af317dac183a82d9295d"
 dependencies = [
- "buf_redux",
+ "buffer-redux",
  "bytecount",
  "bzip2",
  "flate2",
  "memchr",
  "xz2",
 ]
```

### Comparing `blobtk-0.3.1/src/bam.rs` & `blobtk-0.3.2/src/bam.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/blobdir.rs` & `blobtk-0.3.2/src/blobdir.rs`

 * *Files 3% similar despite different names*

```diff
@@ -354,27 +354,53 @@
         None => return None,
     };
     let field: Field<String> = serde_json::from_reader(reader).expect("unable to parse json");
     let values = field.values().clone();
     Some(values)
 }
 
-pub fn parse_filters(filters: &Vec<String>) -> HashMap<&str, Filter> {
+pub fn parse_filters(
+    options: &cli::PlotOptions,
+    plot_meta: Option<&HashMap<String, String>>,
+) -> HashMap<String, Filter> {
+    let mut filters = options.filter.clone();
+    if plot_meta.is_some() && options.x_limit.is_some() {
+        if let Some((min_value, max_value)) = options.x_limit.clone().unwrap().split_once(",") {
+            let x_field = plot_meta.unwrap().get("x").unwrap();
+            if !min_value.is_empty() {
+                filters.push(format!("{}--Min={}", x_field, min_value))
+            }
+            if !max_value.is_empty() {
+                filters.push(format!("{}--Max={}", x_field, max_value))
+            }
+        }
+    }
+    if plot_meta.is_some() && options.y_limit.is_some() {
+        if let Some((min_value, max_value)) = options.y_limit.clone().unwrap().split_once(",") {
+            let y_field = plot_meta.unwrap().get("y").unwrap();
+            if !min_value.is_empty() {
+                filters.push(format!("{}--Min={}", y_field, min_value))
+            }
+            if !max_value.is_empty() {
+                filters.push(format!("{}--Max={}", y_field, max_value))
+            }
+        }
+    }
     let mut filter_map = HashMap::new();
-    for filter in filters {
+    for filter in filters.iter() {
         if let Some((id, parameter)) = filter.split_once("--") {
             if !filter_map.contains_key(id) {
                 filter_map.insert(
-                    id,
+                    id.to_string(),
                     Filter {
                         ..Default::default()
                     },
                 );
             };
-            let filter_params = filter_map.get_mut(&id).unwrap();
+            let filter_params = filter_map.get_mut(&id.to_string()).unwrap();
             if parameter == "Inv" {
                 filter_params.invert = true;
                 continue;
             };
             if let Some((param, value)) = parameter.split_once("=") {
                 match param {
                     "Max" => filter_params.max = Some(value.parse().unwrap()),
@@ -451,19 +477,19 @@
         if keep {
             output.push(i);
         }
     }
     output
 }
 
-pub fn set_filters(filters: HashMap<&str, Filter>, meta: &Meta, blobdir: &PathBuf) -> Vec<usize> {
+pub fn set_filters(filters: HashMap<String, Filter>, meta: &Meta, blobdir: &PathBuf) -> Vec<usize> {
     let mut indices = vec![];
     let field_list = meta.field_list.clone().unwrap();
     for (id, filter) in filters {
-        let field_meta_option = field_list.get(id);
+        let field_meta_option = field_list.get(&id);
         match field_meta_option {
             Some(field_meta) => {
                 let field = field_meta.clone();
                 match field.datatype {
                     Some(Datatype::Float) => {
                         let values = parse_field_float(field_meta.id.clone(), blobdir).unwrap();
                         indices = filter_float_values(values, filter, indices);
@@ -516,14 +542,25 @@
     let mut output = vec![];
     for i in indices {
         output.push(values[i.clone()].clone().0)
     }
     output
 }
 
+pub fn apply_filter_cat_tuple(
+    values: &Vec<(String, usize)>,
+    indices: &Vec<usize>,
+) -> Vec<(String, usize)> {
+    let mut output = vec![];
+    for i in indices {
+        output.push(values[i.clone()].clone())
+    }
+    output
+}
+
 pub fn get_plot_values(
     meta: &Meta,
     blobdir: &PathBuf,
     plot_map: &HashMap<String, String>,
 ) -> (HashMap<String, Vec<f64>>, Vec<(String, usize)>) {
     let mut plot_values = HashMap::new();
     let mut cat_values = vec![];
```

### Comparing `blobtk-0.3.1/src/cli.rs` & `blobtk-0.3.2/src/cli.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 use std::collections::HashSet;
 use std::path::PathBuf;
 
 use clap::{ArgGroup, Parser, Subcommand, ValueEnum};
+use clap_num::number_range;
 use pyo3::pyclass;
 
+use crate::plot::axis::Scale;
+use crate::plot::data::Reducer;
+use crate::plot::ShowLegend;
+
 // fn float_range(s: &str, min: f64, max: f64) -> Result<f64, String> {
 //     debug_assert!(min <= max, "minimum of {} exceeds maximum of {}", min, max);
 //     let val = match s.parse::<f64>() {
 //         Ok(v) => v,
 //         Err(e) => panic!("{:?}", e),
 //     };
 //     check_float_range(val, min, max)
@@ -162,20 +167,31 @@
 pub enum View {
     Blob,
     Cumulative,
     Snail,
 }
 
 #[derive(ValueEnum, Clone, Debug)]
+pub enum Origin {
+    O,
+    X,
+    Y,
+}
+
+#[derive(ValueEnum, Clone, Debug)]
 pub enum Palette {
     Default,
     Inverse,
     Viridis,
 }
 
+fn less_than_5(s: &str) -> Result<f64, String> {
+    Ok(number_range(&format!("{}", s.parse::<f64>().unwrap() * 10.0), 2, 50)? as f64 / 10.0)
+}
+
 /// Options to pass to `blobtk plot`
 #[derive(Parser, Debug)]
 #[pyclass]
 pub struct PlotOptions {
     /// Path to BlobDir directory
     #[arg(long, short = 'd')]
     pub blobdir: PathBuf,
@@ -204,26 +220,48 @@
     #[arg(long = "y-field", short = 'y')]
     pub y_field: Option<String>,
     /// Z-axis field for blob plot
     #[arg(long = "z-field", short = 'z')]
     pub z_field: Option<String>,
     /// Category field for blob plot
     #[arg(long = "category", short = 'c')]
-    /// Category field for blob plot
-    #[arg(long = "category", short = 'c')]
     pub cat_field: Option<String>,
     /// Resolution for blob plot
     #[arg(long, default_value_t = 30)]
     pub resolution: usize,
+    /// Maximum histogram height for blob plot
+    #[arg(long = "hist-height")]
+    pub hist_height: Option<usize>,
+    /// Reducer function for blob plot
+    #[arg(long, value_enum, default_value_t = Reducer::Sum)]
+    pub reducer_function: Reducer,
+    /// Scale function for blob plot
+    #[arg(long, value_enum, default_value_t = Scale::SQRT)]
+    pub scale_function: Scale,
+    /// Scale factor for blob plot (0.2 - 5.0)
+    #[arg(long, default_value_t = 1.0, value_parser=less_than_5)]
+    pub scale_factor: f64,
+    /// X-axis limits for blob/cumulative plot (<min>,<max>)
+    #[arg(long = "x-limit")]
+    pub x_limit: Option<String>,
+    /// Y-axis limits for blob/cumulative plot (<min>,<max>)
+    #[arg(long = "y-limit")]
+    pub y_limit: Option<String>,
     /// Maximum number of categories for blob/cumulative plot
     #[arg(long = "cat-count", default_value_t = 10)]
     pub cat_count: usize,
+    /// Maximum number of categories for blob/cumulative plot
+    #[arg(long = "legend", value_enum, default_value_t = ShowLegend::Default)]
+    pub show_legend: ShowLegend,
     /// Category order for blob/cumulative plot (<cat1>,<cat2>,...)
     #[arg(long = "cat-order")]
     pub cat_order: Option<String>,
+    /// Origin for category lines in cumulative plot
+    #[arg(long, value_enum)]
+    pub origin: Option<Origin>,
     /// Colour palette for categories
     #[arg(long, value_enum)]
     pub palette: Option<Palette>,
     /// Individual colours to modify palette (<index>=<hexcode>)
     #[arg(long)]
     pub color: Option<Vec<String>>,
 }
```

### Comparing `blobtk-0.3.1/src/depth.rs` & `blobtk-0.3.2/src/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/fasta.rs` & `blobtk-0.3.2/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/fastq.rs` & `blobtk-0.3.2/src/fastq.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/filter.rs` & `blobtk-0.3.2/src/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/io.rs` & `blobtk-0.3.2/src/io.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/lib.rs` & `blobtk-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/main.rs` & `blobtk-0.3.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/plot/axis.rs` & `blobtk-0.3.2/src/plot/axis.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 use std::str::FromStr;
 
+use clap::ValueEnum;
+
 #[derive(Clone, Debug)]
 pub struct TickOptions {
     pub font_size: f64,
     pub font_color: String,
     pub label_ticks: bool,
     pub weight: f64,
     pub length: f64,
@@ -61,15 +63,15 @@
             "bottom" => Ok(Position::BOTTOM),
             "left" => Ok(Position::LEFT),
             _ => Err(()),
         }
     }
 }
 
-#[derive(Clone, Debug, PartialEq)]
+#[derive(Clone, Debug, PartialEq, ValueEnum)]
 pub enum Scale {
     LINEAR,
     SQRT,
     LOG,
 }
 
 impl FromStr for Scale {
@@ -96,45 +98,49 @@
 #[derive(Clone, Debug)]
 pub struct AxisOptions {
     pub label: String,
     pub label_offset: f64,
     pub position: Position,
     pub padding: [f64; 2],
     pub offset: f64,
+    pub height: f64,
     pub font_size: f64,
     pub weight: f64,
     pub color: String,
     pub scale: Scale,
     pub domain: [f64; 2],
     pub range: [f64; 2],
     pub clamp: Option<f64>,
     pub rotate: bool,
     pub tick_labels: bool,
+    pub gridlines: bool,
     pub tick_count: usize,
     pub major_ticks: Option<TickOptions>,
     pub minor_ticks: Option<TickOptions>,
 }
 
 impl Default for AxisOptions {
     fn default() -> AxisOptions {
         AxisOptions {
             label: "".to_string(),
             label_offset: 70.0,
             position: Position::LEFT,
             padding: [0.0, 0.0],
             offset: 0.0,
+            height: 100.0,
             font_size: 30.0,
             weight: 3.0,
             color: "black".to_string(),
             scale: Scale::LINEAR,
             domain: [0.0, 1.0],
             range: [0.0, 100.0],
             clamp: None,
             rotate: false,
             tick_labels: true,
+            gridlines: true,
             tick_count: 10,
             major_ticks: Some(TickOptions {
                 ..Default::default()
             }),
             minor_ticks: Some(TickOptions {
                 status: TickStatus::Minor,
                 weight: 1.0,
```

### Comparing `blobtk-0.3.1/src/plot/chart.rs` & `blobtk-0.3.2/src/plot/chart.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use svg::node::element::{Circle, Group};
 
 use super::{
     axis::ChartAxes,
     component::chart_axis,
-    data::{HistogramData, ScatterData},
+    data::{HistogramData, LineData, ScatterData},
     style::{path_filled, path_open},
 };
 
 #[derive(Clone, Debug)]
 pub struct Dimensions {
     pub height: f64,
     pub width: f64,
@@ -27,45 +27,74 @@
 }
 
 #[derive(Clone, Debug)]
 pub struct Chart {
     pub axes: ChartAxes,
     pub scatter_data: Option<ScatterData>,
     // pub bar_data: Option<BarData>,
-    // pub line_data: Option<LineData>,
+    pub line_data: Option<LineData>,
     pub histogram_data: Option<Vec<HistogramData>>,
+    pub line_options: Vec<(String, String)>,
     pub scatter_options: Vec<(String, String)>,
     pub histogram_options: Vec<(String, String)>,
     pub dimensions: Dimensions,
 }
 
 impl Default for Chart {
     fn default() -> Chart {
         Chart {
             axes: ChartAxes {
                 x: None,
                 y: None,
                 x2: None,
                 y2: None,
             },
+            line_data: None,
             scatter_data: None,
             histogram_data: None,
+            line_options: vec![],
             scatter_options: vec![],
             histogram_options: vec![],
             dimensions: Dimensions {
                 ..Default::default()
             },
         }
     }
 }
 
 impl Chart {
     pub fn svg(self) -> Group {
         let opacity = 0.6;
         let mut group = Group::new();
+        let mut axis_group = Group::new();
+        let mut gridline_group = Group::new();
+
+        if self.axes.x.is_some() {
+            let (axis, gridlines) = chart_axis(self.axes.x.as_ref().unwrap());
+            axis_group = axis_group.add(axis);
+            gridline_group = gridline_group.add(gridlines);
+        }
+        if self.axes.y.is_some() {
+            let (axis, gridlines) = chart_axis(self.axes.y.as_ref().unwrap());
+            axis_group = axis_group.add(axis);
+            gridline_group = gridline_group.add(gridlines);
+        }
+        if self.axes.x2.is_some() {
+            let (axis, gridlines) = chart_axis(self.axes.x2.as_ref().unwrap());
+            axis_group = axis_group.add(axis);
+            gridline_group = gridline_group.add(gridlines);
+        }
+        if self.axes.y2.is_some() {
+            let (axis, gridlines) = chart_axis(self.axes.y2.as_ref().unwrap());
+            axis_group = axis_group.add(axis);
+            gridline_group = gridline_group.add(gridlines);
+        }
+
+        group = group.add(gridline_group);
+
         if self.scatter_data.is_some() {
             let scatter_data = self.scatter_data.unwrap();
             let mut scatter_group = Group::new();
             for point in scatter_data.points.iter() {
                 scatter_group = scatter_group.add(
                     Circle::new()
                         .set("cx", point.x)
@@ -104,26 +133,36 @@
                 "transform",
                 format!(
                     "translate({}, {})",
                     self.dimensions.padding[3], self.dimensions.padding[2]
                 ),
             ));
         }
-
-        if self.axes.x.is_some() {
-            group = group.add(chart_axis(&self.axes.x.unwrap()));
-        }
-        if self.axes.y.is_some() {
-            group = group.add(chart_axis(&self.axes.y.unwrap()));
-        }
-        if self.axes.x2.is_some() {
-            group = group.add(chart_axis(&self.axes.x2.unwrap()));
-        }
-        if self.axes.y2.is_some() {
-            group = group.add(chart_axis(&self.axes.y2.unwrap()));
+        if self.line_data.is_some() {
+            let mut line_group = Group::new();
+            let line_data = self.line_data.unwrap();
+            for line in line_data.lines.iter() {
+                let color = match line.color.clone() {
+                    Some(col) => col.clone(),
+                    None => "#000000".to_string(),
+                };
+                let path_data = line
+                    .clone()
+                    .to_path_data(self.axes.x.clone().unwrap().position, true);
+                line_group = line_group.add(
+                    path_open(path_data.clone(), Some(&color), Some(line.weight))
+                        .set("stroke-linecap", "round")
+                        .set("stroke-linejoin", "round"),
+                );
+            }
+            group = group.add(line_group.set(
+                "transform",
+                format!(
+                    "translate({}, {})",
+                    self.dimensions.padding[3], self.dimensions.padding[2]
+                ),
+            ));
         }
-        // let x_axis = chart_axis(&scatter_data.x);
-        // let y_axis = chart_axis(&scatter_data.y);
-
+        group = group.add(axis_group);
         group
     }
 }
```

### Comparing `blobtk-0.3.1/src/plot/component.rs` & `blobtk-0.3.2/src/plot/component.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use svg::node::element::path::Data;
 use svg::node::element::{Circle, Group, Line, Path, Rectangle, Text};
 use svg::node::Text as nodeText;
 
 use crate::utils::{format_si, linear_scale, linear_scale_float, scale_float, scale_floats};
 
 use super::axis::{AxisOptions, Position, Scale, TickOptions, TickStatus};
+use super::style::path_open;
 
 #[derive(Clone, Debug)]
 pub struct RadialTick {
     pub index: usize,
     pub offset: f64,
     pub angle: f64,
     pub label: Text,
@@ -24,27 +25,59 @@
 }
 
 #[derive(Clone, Debug)]
 pub struct Tick {
     pub label: Text,
     pub path: Path,
     pub position: f64,
+    pub gridline: Path,
     pub status: TickStatus,
 }
 
+impl Default for Tick {
+    fn default() -> Tick {
+        Tick {
+            label: Text::new(),
+            path: Path::new(),
+            position: 0.0,
+            gridline: Path::new(),
+            status: TickStatus::Major,
+        }
+    }
+}
+
 #[derive(Clone, Debug)]
 pub enum LegendShape {
     Rect,
     Circumference,
     Radius,
+    None,
+}
+
+pub struct LegendEntry {
+    pub title: String,
+    pub subtitle: Option<String>,
+    pub color: String,
+    pub shape: LegendShape,
+}
+
+impl Default for LegendEntry {
+    fn default() -> LegendEntry {
+        LegendEntry {
+            title: "".to_string(),
+            subtitle: None,
+            color: "#000000".to_string(),
+            shape: LegendShape::Rect,
+        }
+    }
 }
 
 pub fn legend(
     title: String,
-    entries: Vec<(String, String, LegendShape)>,
+    entries: Vec<LegendEntry>,
     subtitle: Option<String>,
     columns: u8,
 ) -> Group {
     let title_text = if title.is_empty() {
         Text::new()
     } else {
         Text::new()
@@ -53,63 +86,84 @@
             .set("text-anchor", "start")
             .set("dominant-baseline", "bottom")
             .set("stroke", "none")
             .set("fill", "black")
             .add(nodeText::new(title.clone()))
     };
     let mut group = Group::new().add(title_text);
-    let cell = 18;
+    let cell: i32 = 18;
     let gap = 8;
     let mut offset_y = 0;
     let mut offset_x: i32 = -175;
     let per_column = entries.len() / columns as usize;
     for (i, entry) in entries.iter().enumerate() {
         if i % per_column == 0 {
             offset_x += 175;
             offset_y = if title.is_empty() { 0 } else { gap / 2 };
         }
+        let title_width = cell + gap + entry.title.len() as i32 * cell * 11 / 20;
+        let mut rect_width = title_width;
+        let (anchor, position, rect_x) = match entry.subtitle {
+            Some(_) => {
+                rect_width += gap + entry.subtitle.clone().unwrap().len() as i32 * cell * 11 / 20;
+                ("end", -gap, -gap - title_width)
+            }
+            None => ("start", cell + gap, -gap / 2),
+        };
         let entry_text = Text::new()
             .set("font-family", "Roboto, Open sans, sans-serif")
             .set("font-size", cell)
-            .set("text-anchor", "start")
+            .set("text-anchor", anchor)
             .set("dominant-baseline", "bottom")
             .set("stroke", "none")
             .set("fill", "black")
-            .set("x", cell + gap)
+            .set("x", position)
             .set("y", cell + gap / 2)
-            .add(nodeText::new(&entry.clone().0));
+            .add(nodeText::new(&entry.clone().title));
+        let entry_subtext = if entry.subtitle.is_some() {
+            Text::new()
+                .set("font-family", "Roboto, Open sans, sans-serif")
+                .set("font-size", cell as f64 * 0.9)
+                .set("text-anchor", "start")
+                .set("dominant-baseline", "bottom")
+                .set("stroke", "none")
+                .set("fill", "black")
+                .set("x", cell + gap)
+                .set("y", cell * 9 / 10 + gap / 2)
+                .add(nodeText::new(entry.clone().subtitle.clone().unwrap()))
+        } else {
+            Text::new()
+        };
         let background = Group::new().add(
             Rectangle::new()
                 .set("stroke", "none")
                 .set("fill", "#ffffff")
-                .set("x", -gap / 2)
+                .set("x", rect_x)
                 .set("y", gap / 2)
-                .set("height", cell + gap / 2)
-                .set(
-                    "width",
-                    cell as f64 + gap as f64 + entry.0.len() as f64 * cell as f64 * 0.7,
-                ),
+                .set("height", cell + gap)
+                .set("width", rect_width)
+                .set("opacity", 0.95),
         );
-        let shape = match entry.2 {
+        let shape = match entry.shape {
             LegendShape::Rect => Group::new().add(
                 Rectangle::new()
                     .set("stroke", "black")
                     .set("stroke-width", 2)
-                    .set("fill", entry.clone().1.clone())
+                    .set("fill", entry.color.clone())
                     .set("x", 0)
                     .set("y", 6)
                     .set("height", cell)
                     .set("width", cell),
             ),
             LegendShape::Circumference => Group::new()
                 .add(
                     Circle::new()
                         .set("stroke", "black")
                         .set("stroke-width", 2)
-                        .set("fill", entry.clone().1.clone())
+                        .set("fill", entry.color.clone())
                         .set("cx", cell / 2)
                         .set("cy", 6 + cell / 2)
                         .set("r", cell / 2),
                 )
                 .add(
                     Line::new()
                         .set("fill", "none")
@@ -121,38 +175,40 @@
                         .set("y2", 6),
                 ),
             LegendShape::Radius => Group::new()
                 .add(
                     Circle::new()
                         .set("stroke", "black")
                         .set("stroke-width", 1)
-                        .set("fill", entry.clone().1.clone())
+                        .set("fill", entry.color.clone())
                         .set("cx", cell / 2)
                         .set("cy", 6 + cell / 2)
                         .set("r", cell / 2),
                 )
                 .add(
                     Line::new()
                         .set("fill", "none")
                         .set("stroke", "black")
                         .set("stroke-width", 2)
                         .set("x1", cell / 2)
                         .set("y1", 6 + cell / 2)
                         .set("x2", cell / 2)
                         .set("y2", 6),
                 ),
+            LegendShape::None => Group::new(),
         };
         let entry_group = Group::new()
             .set(
                 "transform",
                 format!("translate({}, {})", offset_x, offset_y),
             )
             .add(background)
             .add(shape)
-            .add(entry_text);
+            .add(entry_text)
+            .add(entry_subtext);
         group = group.add(entry_group);
         offset_y = offset_y + cell + gap;
     }
     match subtitle {
         None => (),
         Some(subtitle_string) => {
             let subtitle_text = Text::new()
@@ -243,14 +299,15 @@
         label: text,
         path,
         position: offset,
         status: match status {
             TickStatus::Major => TickStatus::Major,
             TickStatus::Minor => TickStatus::Minor,
         },
+        ..Default::default()
     }
 }
 
 pub fn create_tick(
     value: f64,
     label: String,
     range: &[f64; 2],
@@ -260,91 +317,111 @@
     let location = scale_floats(
         value,
         &axis_options.domain,
         &range,
         &axis_options.scale,
         None,
     );
+    let axis_height = axis_options.height;
     let rotate = axis_options.rotate;
-    let (x1, y1, x2, y2, x_text, y_text, anchor, baseline, angle) = match axis_options.position {
-        Position::TOP => (
-            location,
-            axis_options.offset,
-            location,
-            axis_options.offset - tick_options.length,
-            location,
-            axis_options.offset - tick_options.length * 1.5,
-            if rotate { "end" } else { "middle" },
-            if rotate { "central" } else { "auto" },
-            if rotate { 90.0 } else { 0.0 },
-        ),
-        Position::RIGHT => (
-            axis_options.offset,
-            location,
-            axis_options.offset + tick_options.length,
-            location,
-            axis_options.offset + tick_options.length * 1.5,
-            location,
-            "middle",
-            "hanging",
-            270.0,
-        ),
-        Position::BOTTOM => (
-            location,
-            axis_options.offset,
-            location,
-            axis_options.offset + tick_options.length,
-            location,
-            axis_options.offset + tick_options.length * 1.5,
-            if rotate { "start" } else { "middle" },
-            if rotate { "central" } else { "hanging" },
-            if rotate { 90.0 } else { 0.0 },
-        ),
-        Position::LEFT => (
-            axis_options.offset,
-            location,
-            axis_options.offset - tick_options.length,
-            location,
-            axis_options.offset - tick_options.length * 1.5,
-            location,
-            if rotate { "end" } else { "middle" },
-            if rotate { "central" } else { "hanging" },
-            if rotate { 0.0 } else { 90.0 },
-        ),
-    };
+    let (x1, y1, x2, y2, x3, y3, x_text, y_text, anchor, baseline, angle) =
+        match axis_options.position {
+            Position::TOP => (
+                location,
+                axis_options.offset,
+                location,
+                axis_options.offset - tick_options.length,
+                location,
+                axis_height,
+                location,
+                axis_options.offset - tick_options.length * 1.5,
+                if rotate { "end" } else { "middle" },
+                if rotate { "central" } else { "auto" },
+                if rotate { 90.0 } else { 0.0 },
+            ),
+            Position::RIGHT => (
+                axis_options.offset,
+                location,
+                axis_options.offset + tick_options.length,
+                location,
+                axis_height,
+                location,
+                axis_options.offset + tick_options.length * 1.5,
+                location,
+                "middle",
+                "hanging",
+                270.0,
+            ),
+            Position::BOTTOM => (
+                location,
+                axis_options.offset,
+                location,
+                axis_options.offset + tick_options.length,
+                location,
+                axis_options.offset - axis_height,
+                location,
+                axis_options.offset + tick_options.length * 1.5,
+                if rotate { "start" } else { "middle" },
+                if rotate { "central" } else { "hanging" },
+                if rotate { 90.0 } else { 0.0 },
+            ),
+            Position::LEFT => (
+                axis_options.offset,
+                location,
+                axis_options.offset - tick_options.length,
+                location,
+                axis_height,
+                location,
+                axis_options.offset - tick_options.length * 1.5,
+                location,
+                if rotate { "end" } else { "middle" },
+                if rotate { "central" } else { "hanging" },
+                if rotate { 0.0 } else { 90.0 },
+            ),
+        };
     let path_data = Data::new().move_to((x1, y1)).line_to((x2, y2));
     let path = match tick_options.status {
         TickStatus::Major => path_axis_major(path_data, Some(&axis_options.color)),
         TickStatus::Minor => path_axis_minor(path_data, Some(&axis_options.color)),
     };
-    let text = if axis_options.tick_labels {
-        match tick_options.status {
-            TickStatus::Major => Text::new()
-                .set("font-family", "Roboto, Open sans, sans-serif")
-                .set("font-size", tick_options.font_size)
-                .set("text-anchor", anchor)
-                .set("dominant-baseline", baseline)
-                .set("stroke", "none")
-                .set("fill", axis_options.color.clone())
-                .set(
-                    "transform",
-                    format!("translate({:?}, {:?}) rotate({:?})", x_text, y_text, angle),
-                )
-                .add(nodeText::new(label)),
-            TickStatus::Minor => Text::new(),
-        }
+    let gridline = match tick_options.status {
+        TickStatus::Major => path_open(
+            Data::new().move_to((x1, y1)).line_to((x3, y3)),
+            Some("#cccccc"),
+            Some(1.0),
+        ),
+        _ => Path::new(),
+    };
+    let text = if axis_options.tick_labels && !label.is_empty() {
+        // match tick_options.status {
+        Text::new()
+            .set("font-family", "Roboto, Open sans, sans-serif")
+            .set("font-size", tick_options.font_size)
+            .set("text-anchor", anchor)
+            .set("dominant-baseline", baseline)
+            .set("stroke", "none")
+            .set("fill", axis_options.color.clone())
+            .set(
+                "transform",
+                format!("translate({:?}, {:?}) rotate({:?})", x_text, y_text, angle),
+            )
+            .add(nodeText::new(label)) //,
+                                       // TickStatus::Minor => Text::new(),
+                                       // }
     } else {
         Text::new()
     };
 
     Tick {
         label: text,
         path,
         position: location,
+        gridline,
         status: tick_options.status.clone(),
+        ..Default::default()
     }
 }
 
 pub fn create_axis_ticks(options: &AxisOptions, status: TickStatus) -> Vec<Tick> {
     let range = [
         options.range[0] + options.padding[0],
         options.range[1] + options.padding[0],
@@ -382,15 +459,15 @@
                     if power < 0 {
                         i = 1.0 / i;
                     }
                     if min_value.clone() < 0.0 {
                         i = -i
                     }
                     while i <= domain[1].clone() {
-                        let label = if i > min_value.clone() {
+                        let label = if i >= min_value.clone() {
                             format_si(&i, 3)
                         } else {
                             String::new()
                         };
                         ticks.push(create_tick(
                             i,
                             label,
@@ -408,18 +485,23 @@
                     }
                     if min_value.clone() < 0.0 {
                         i = -i
                     }
                     while i <= domain[1].clone() {
                         let mut j = i * 2.0;
                         while j < i * 10.0 && j <= domain[1].clone() {
+                            let label = if j >= min_value.clone() {
+                                format_si(&j, 3)
+                            } else {
+                                String::new()
+                            };
                             if j as f64 >= min_value {
                                 ticks.push(create_tick(
                                     j,
-                                    "".to_string(),
+                                    label,
                                     &range,
                                     &options,
                                     &options.minor_ticks.as_ref().unwrap(),
                                 ));
                             }
                             j = j + i;
                         }
@@ -450,15 +532,15 @@
                 multiple *= 10.0;
             }
 
             match status {
                 TickStatus::Major => {
                     let mut i = step * (min_value / step).ceil();
                     while i <= domain[1].clone() {
-                        let label = if i > min_value.clone() {
+                        let label = if i >= min_value.clone() {
                             format_si(&i, 3)
                         } else {
                             String::new()
                         };
                         ticks.push(create_tick(
                             i,
                             label,
@@ -945,28 +1027,36 @@
     }
     if polar_coords.len() > 0 {
         path_data = path_data.close();
     }
     path_data
 }
 
-pub fn chart_axis(plot_axis: &AxisOptions) -> Group {
+pub fn chart_axis(plot_axis: &AxisOptions) -> (Group, Group) {
     let mut major_tick_group = Group::new();
+    let mut major_gridline_group = Group::new();
+    let mut major_tick_count = 0;
     if plot_axis.major_ticks.is_some() {
         let major_ticks = create_axis_ticks(&plot_axis, TickStatus::Major);
+        major_tick_count = major_ticks.len();
         for tick in major_ticks {
             major_tick_group = major_tick_group.add(tick.path).add(tick.label);
+            major_gridline_group = major_gridline_group.add(tick.gridline);
         }
     };
 
     let mut minor_tick_group = Group::new();
     if plot_axis.minor_ticks.is_some() {
         let minor_ticks = create_axis_ticks(&plot_axis, TickStatus::Minor);
         for tick in minor_ticks {
-            minor_tick_group = minor_tick_group.add(tick.path);
+            minor_tick_group = if major_tick_count < 2 {
+                minor_tick_group.add(tick.path).add(tick.label)
+            } else {
+                minor_tick_group.add(tick.path)
+            };
         }
     }
 
     let (x1, y1, x2, y2, label_x, label_y, label_rotate) = match plot_axis.position {
         Position::TOP => (
             plot_axis.range[0],
             plot_axis.offset,
@@ -1027,13 +1117,16 @@
             format!(
                 "translate({:?}, {:?}) rotate({:?})",
                 label_x, label_y, label_rotate
             ),
         )
         .add(nodeText::new(plot_axis.label.clone()));
 
-    Group::new()
-        .add(minor_tick_group)
-        .add(major_tick_group)
-        .add(axis)
-        .add(label)
+    (
+        Group::new()
+            .add(minor_tick_group)
+            .add(major_tick_group)
+            .add(axis)
+            .add(label),
+        Group::new().add(major_gridline_group),
+    )
 }
```

### Comparing `blobtk-0.3.1/src/plot/snail.rs` & `blobtk-0.3.2/src/plot/snail.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 use titlecase::titlecase;
 
 use crate::blobdir::{self, BuscoGene};
 
 use super::axis::{TickOptions, TickStatus};
 use super::component::{
     arc_path, legend, path_axis_major, path_axis_minor, path_gridline_major, path_gridline_minor,
-    polar_to_path, polar_to_path_bounded, set_axis_ticks, set_axis_ticks_circular, LegendShape,
+    polar_to_path, polar_to_path_bounded, set_axis_ticks, set_axis_ticks_circular, LegendEntry,
+    LegendShape,
 };
 use super::style::{path_filled, path_open, path_partial};
 use crate::cli;
 use crate::utils::{
     self, compact_float, format_si, linear_scale, linear_scale_float, log_scale, sqrt_scale,
 };
 
@@ -258,64 +259,64 @@
     let scaffold_length = format_si(&(snail_stats.span() as f64), 3);
     let longest_scaffold = format_si(&(snail_stats.scaffolds()[0] as f64), 3);
     let n50_bin = (options.segments / 2) - 1;
     let n90_bin = (options.segments * 9 / 10) - 1;
     let n50_length = format_si(&(snail_stats.binned_scaffold_lengths()[n50_bin] as f64), 3);
     let n90_length = format_si(&(snail_stats.binned_scaffold_lengths()[n90_bin] as f64), 3);
     let record = snail_stats.record_type();
-    entries.push((
-        format!("Log10 {} count (total {})", record, scaffold_count),
-        "#dddddd".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("{} length (total {})", titlecase(record), scaffold_length),
-        "#999999".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("Longest {} ({})", record, longest_scaffold),
-        "#e31a1c".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("N50 length ({})", n50_length),
-        "#ff7f00".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("N90 length ({})", n90_length),
-        "#fdbf6f".to_string(),
-        LegendShape::Rect,
-    ));
+    entries.push(LegendEntry {
+        title: format!("Log10 {} count (total {})", record, scaffold_count),
+        color: "#dddddd".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("{} length (total {})", titlecase(record), scaffold_length),
+        color: "#999999".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("Longest {} ({})", record, longest_scaffold),
+        color: "#e31a1c".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("N50 length ({})", n50_length),
+        color: "#ff7f00".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("N90 length ({})", n90_length),
+        color: "#fdbf6f".to_string(),
+        ..Default::default()
+    });
 
     let title = format!("{} statistics", titlecase(record));
     legend(title, entries, None, 1)
 }
 
 pub fn composition_stats_legend(snail_stats: &SnailStats, _: &cli::PlotOptions) -> Group {
     let mut entries = vec![];
     let gc_prop = format_si(&(snail_stats.gc_proportion as f64 * 100.0), 3);
     let at_prop = format_si(&(snail_stats.at_proportion as f64 * 100.0), 3);
     let n_prop = format_si(&(snail_stats.n_proportion as f64 * 100.0), 3);
-    entries.push((
-        format!("GC ({}%)", gc_prop),
-        "#1f78b4".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("AT ({}%)", at_prop),
-        "#a6cee3".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("N ({}%)", n_prop),
-        "#ffffff".to_string(),
-        LegendShape::Rect,
-    ));
+    entries.push(LegendEntry {
+        title: format!("GC ({}%)", gc_prop),
+        color: "#1f78b4".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("AT ({}%)", at_prop),
+        color: "#a6cee3".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("N ({}%)", n_prop),
+        color: "#ffffff".to_string(),
+        ..Default::default()
+    });
 
     let title = "Composition".to_string();
     legend(title, entries, None, 1)
 }
 
 pub fn scale_stats_legend(snail_stats: &SnailStats, options: &cli::PlotOptions) -> Group {
     let mut entries = vec![];
@@ -325,24 +326,26 @@
     };
     let max_scaffold = match options.max_scaffold {
         Some(scaffold_length) => scaffold_length,
         None => snail_stats.scaffolds()[0],
     };
     let circ_prop = format_si(&(max_span as f64), 3);
     let rad_prop = format_si(&(max_scaffold as f64), 3);
-    entries.push((
-        format!("{}", circ_prop),
-        "#ffffff".to_string(),
-        LegendShape::Circumference,
-    ));
-    entries.push((
-        format!("{}", rad_prop),
-        "#ffffff".to_string(),
-        LegendShape::Radius,
-    ));
+    entries.push(LegendEntry {
+        title: format!("{}", circ_prop),
+        color: "#ffffff".to_string(),
+        shape: LegendShape::Circumference,
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("{}", rad_prop),
+        color: "#ffffff".to_string(),
+        shape: LegendShape::Radius,
+        ..Default::default()
+    });
 
     let title = "Scale".to_string();
     legend(title, entries, None, 1)
 }
 
 pub fn dataset_name_legend(snail_stats: &SnailStats, _: &cli::PlotOptions) -> Group {
     let entries = vec![];
@@ -372,34 +375,34 @@
         3,
     );
     let subtitle = format!(
         "{} ({})",
         snail_stats.busco_lineage,
         snail_stats.busco_total()
     );
-    entries.push((
-        format!("Comp. ({}%)", comp_prop),
-        "#33a02c".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("Dupl. ({}%)", dup_prop),
-        "#20641b".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("Frag. ({}%)", frag_prop),
-        "#a3e27f".to_string(),
-        LegendShape::Rect,
-    ));
-    entries.push((
-        format!("Missing ({}%)", missing_prop),
-        "#ffffff".to_string(),
-        LegendShape::Rect,
-    ));
+    entries.push(LegendEntry {
+        title: format!("Comp. ({}%)", comp_prop),
+        color: "#33a02c".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("Dupl. ({}%)", dup_prop),
+        color: "#20641b".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("Frag. ({}%)", frag_prop),
+        color: "#a3e27f".to_string(),
+        ..Default::default()
+    });
+    entries.push(LegendEntry {
+        title: format!("Missing ({}%)", missing_prop),
+        color: "#ffffff".to_string(),
+        ..Default::default()
+    });
 
     let title = "BUSCO".to_string();
     legend(title, entries, Some(subtitle), 2)
 }
 
 pub fn svg(snail_stats: &SnailStats, options: &cli::PlotOptions) -> Document {
     let max_span = match options.max_span {
```

### Comparing `blobtk-0.3.1/src/plot/style.rs` & `blobtk-0.3.2/src/plot/style.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/plot.rs` & `blobtk-0.3.2/src/plot.rs`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 use std::collections::HashMap;
 use std::path::PathBuf;
 use std::str::FromStr;
 
 use crate::blobdir;
 use crate::cli;
 use crate::plot::blob::BlobData;
+use crate::plot::cumulative::CumulativeData;
 // use crate::io;
 
+use clap::ValueEnum;
 pub use cli::PlotOptions;
 use colorous;
 use svg::Document;
 use usvg::{fontdb, TreeParsing, TreeTextToPath};
 
-use self::axis::AxisName;
 use self::blob::BlobDimensions;
+use self::chart::Dimensions;
 
 /// Plot axis functions.
 pub mod axis;
 
 /// Blob plot functions.
 pub mod blob;
 
@@ -30,14 +32,17 @@
 
 /// Chart options.
 pub mod chart;
 
 /// Chart components.
 pub mod component;
 
+/// Cumulative plot functions.
+pub mod cumulative;
+
 /// Scatter plot functions.
 pub mod data;
 
 /// Snail plot functions.
 pub mod snail;
 
 /// SVG styling functions.
@@ -81,28 +86,36 @@
             "png" => Ok(Suffix::PNG),
             "svg" => Ok(Suffix::SVG),
             _ => Err(()),
         }
     }
 }
 
+#[derive(ValueEnum, Clone, Debug)]
+pub enum ShowLegend {
+    Default,
+    Full,
+    Compact,
+    None,
+}
+
 pub fn plot_snail(meta: &blobdir::Meta, options: &cli::PlotOptions) {
     // let busco_list = meta.busco_list.clone().unwrap();
     let busco_field = meta.busco_list.clone().unwrap()[0].clone();
     let busco_values = blobdir::parse_field_busco(busco_field.0, &options.blobdir).unwrap();
     let busco_total = busco_field.1;
     let busco_lineage = busco_field.2;
     let gc_values = blobdir::parse_field_float("gc".to_string(), &options.blobdir).unwrap();
     let length_values = blobdir::parse_field_int("length".to_string(), &options.blobdir).unwrap();
     let n_values = blobdir::parse_field_float("n".to_string(), &options.blobdir);
     let ncount_values = blobdir::parse_field_int("ncount".to_string(), &options.blobdir).unwrap();
     let id = meta.id.clone();
     let record_type = meta.record_type.clone();
 
-    let filters = blobdir::parse_filters(&options.filter);
+    let filters = blobdir::parse_filters(&options, None);
     let wanted_indices = blobdir::set_filters(filters, &meta, &options.blobdir);
 
     let gc_filtered = blobdir::apply_filter_float(&gc_values, &wanted_indices);
     let n_filtered = match n_values {
         None => None,
         Some(values) => Some(blobdir::apply_filter_float(&values, &wanted_indices)),
     };
@@ -232,69 +245,128 @@
 
     let (plot_values, cat_values) = blobdir::get_plot_values(&meta, &options.blobdir, &plot_meta);
 
     let palette = set_palette(&options.palette, &options.color, options.cat_count);
 
     let (cat_order, cat_indices) = category::set_cat_order(
         &cat_values,
+        &plot_values["z"],
         &options.cat_order,
         &options.cat_count,
         &palette,
     );
     // let id = meta.id.clone();
     // let record_type = meta.record_type.clone();
 
-    let filters = blobdir::parse_filters(&options.filter);
+    let filters = blobdir::parse_filters(&options, Some(&plot_meta));
     let wanted_indices = blobdir::set_filters(filters, &meta, &options.blobdir);
+    let z = blobdir::apply_filter_float(&plot_values["z"], &wanted_indices);
+    let filtered_cat_values = blobdir::apply_filter_cat_tuple(&cat_values, &wanted_indices);
+    let (cat_order, cat_indices) = if wanted_indices.len() < plot_values["x"].len() {
+        category::set_cat_order(
+            &filtered_cat_values,
+            &z,
+            &Some(cat_order[0].members.join(",")),
+            &options.cat_count,
+            &palette,
+        )
+    } else {
+        (cat_order, cat_indices)
+    };
     let blob_data = BlobData {
         x: blobdir::apply_filter_float(&plot_values["x"], &wanted_indices),
         y: blobdir::apply_filter_float(&plot_values["y"], &wanted_indices),
-        z: blobdir::apply_filter_float(&plot_values["z"], &wanted_indices),
-        cat: blobdir::apply_filter_int(&cat_indices, &wanted_indices),
-        cat_order,
+        z,
+        cat: cat_indices,
+        cat_order: cat_order,
     };
 
-    let scatter_data = blob::blob_points(plot_meta, &blob_data, &meta, &options);
-
     let dimensions = BlobDimensions {
         ..Default::default()
     };
 
-    let (x_bins, x_max) = blob::bin_axis(
-        &scatter_data,
-        &blob_data,
-        AxisName::X,
-        &dimensions,
-        &options,
-    );
-    let (y_bins, y_max) = blob::bin_axis(
-        &scatter_data,
-        &blob_data,
-        AxisName::Y,
-        &dimensions,
-        &options,
-    );
+    let scatter_data = blob::blob_points(plot_meta, &blob_data, &dimensions, &meta, &options);
+
+    let (x_bins, y_bins, max_bin) =
+        blob::bin_axes(&scatter_data, &blob_data, &dimensions, &options);
+
+    // let (x_bins, x_max) = blob::bin_axis(
+    //     &scatter_data,
+    //     &blob_data,
+    //     AxisName::X,
+    //     &dimensions,
+    //     &options,
+    // );
+    // let (y_bins, y_max) = blob::bin_axis(
+    //     &scatter_data,
+    //     &blob_data,
+    //     AxisName::Y,
+    //     &dimensions,
+    //     &options,
+    // );
     // let document: Document = blob::svg(&dimensions, &scatter_data, &x_bins, &y_bins, &options);
 
     let document: Document = blob::plot(
         dimensions,
         scatter_data,
         x_bins,
         y_bins,
-        x_max,
-        y_max,
+        max_bin,
+        max_bin,
         &options,
     );
     save_by_suffix(options, document);
 }
 
+pub fn plot_cumulative(meta: &blobdir::Meta, options: &cli::PlotOptions) {
+    let mut plot_meta: HashMap<String, String> = HashMap::new();
+    plot_meta.insert("z".to_string(), "length".to_string());
+    if options.cat_field.is_some() {
+        plot_meta.insert("cat".to_string(), options.cat_field.clone().unwrap());
+    } else {
+        plot_meta.insert("cat".to_string(), meta.plot.cat.clone().unwrap());
+    }
+    let (plot_values, cat_values) = blobdir::get_plot_values(&meta, &options.blobdir, &plot_meta);
+
+    let palette = set_palette(&options.palette, &options.color, options.cat_count);
+
+    let (cat_order, cat_indices) = category::set_cat_order(
+        &cat_values,
+        &plot_values["z"],
+        &options.cat_order,
+        &options.cat_count,
+        &palette,
+    );
+    // let id = meta.id.clone();
+    // let record_type = meta.record_type.clone();
+
+    let filters = blobdir::parse_filters(&options, None);
+    let wanted_indices = blobdir::set_filters(filters, &meta, &options.blobdir);
+
+    let cumulative_data = CumulativeData {
+        values: blobdir::apply_filter_float(&plot_values["z"], &wanted_indices),
+        cat: blobdir::apply_filter_int(&cat_indices, &wanted_indices),
+        cat_order,
+    };
+
+    let dimensions = Dimensions {
+        ..Default::default()
+    };
+
+    let cumulative_lines = cumulative::cumulative_lines(&cumulative_data, &dimensions, &options);
+
+    let document: Document = cumulative::plot(dimensions, cumulative_lines, &options);
+    save_by_suffix(options, document);
+}
+
 /// Execute the `plot` subcommand from `blobtk`.
 pub fn plot(options: &cli::PlotOptions) -> Result<(), Box<dyn std::error::Error>> {
     let meta = blobdir::parse_blobdir(&options.blobdir);
     let view = &options.view;
     match view {
         Some(cli::View::Blob) => plot_blob(&meta, &options),
+        Some(cli::View::Cumulative) => plot_cumulative(&meta, &options),
         Some(cli::View::Snail) => plot_snail(&meta, &options),
         _ => (),
     }
     Ok(())
 }
```

### Comparing `blobtk-0.3.1/src/python/depth.rs` & `blobtk-0.3.2/src/python/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/python/filter.rs` & `blobtk-0.3.2/src/python/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/python/utils.rs` & `blobtk-0.3.2/src/python/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/taxonomy.rs` & `blobtk-0.3.2/src/taxonomy.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.1/src/utils.rs` & `blobtk-0.3.2/src/utils.rs`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,19 @@
             POSITIVE[thousands as usize]
         } else {
             ""
         };
         suffix.to_string()
     }
 
-    let magnitude = (value.clone()).log10() as i8;
+    let magnitude = if *value == 0.0 {
+        0
+    } else {
+        (value.clone()).log10() as i8
+    };
     let prefix;
     let thousands = magnitude / 3;
     if thousands < 0 {
         prefix = value.clone() * 10u32.pow(3 * (thousands.abs() as u32 + 1)) as f64;
     } else {
         prefix = value.clone() / 10u32.pow(3 * thousands as u32) as f64
     };
@@ -114,14 +118,23 @@
 /// assert_eq!(linear_scale(15, &domain, &range), 50.0);
 /// ```
 pub fn linear_scale(value: usize, domain: &[usize; 2], range: &[f64; 2]) -> f64 {
     let proportion = (value - domain[0]) as f64 / (domain[1] - domain[0]) as f64;
     (range[1] - range[0]) * proportion + range[0]
 }
 
+/// Scale a f64 value from input domain to output range as f64.
+/// # Examples
+///
+/// ```
+/// # use crate::blobtk::utils::linear_scale_float;
+/// let domain = [10.0, 20.0];
+/// let range = [0.0, 100.0];
+/// assert_eq!(linear_scale_float(15.0, &domain, &range), 50.0);
+/// ```
 pub fn linear_scale_float(value: f64, domain: &[f64; 2], range: &[f64; 2]) -> f64 {
     let proportion = (value - domain[0]) / (domain[1] - domain[0]);
     (range[1] - range[0]) * proportion + range[0]
 }
 
 pub fn log_scale(value: usize, domain: &[usize; 2], range: &[f64; 2]) -> f64 {
     let proportion = ((value as f64).log10() - (domain[0] as f64).log10())
@@ -221,7 +234,15 @@
 pub fn max_float<T: PartialOrd>(a: T, b: T) -> T {
     if b > a {
         b
     } else {
         a
     }
 }
+
+pub fn min_float<T: PartialOrd>(a: T, b: T) -> T {
+    if a < b {
+        a
+    } else {
+        b
+    }
+}
```

### Comparing `blobtk-0.3.1/PKG-INFO` & `blobtk-0.3.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtk
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Core utilities for BlobToolKit.
 Keywords: bioinformatics,blobtoolkit,genome,genomics
 Home-Page: https://github.com/blobtoolkit/blobtk
 Author: Rich Challis <rc28@sanger.ac.uk>
```

