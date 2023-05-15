# Comparing `tmp/pywry-0.5.7.tar.gz` & `tmp/pywry-0.5.8.tar.gz`

## Comparing `pywry-0.5.7.tar` & `pywry-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.7/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     4924 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     3565 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     6202 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/events.rs
--rw-r--r--   0     1001      123     3733 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/handlers.rs
--rw-r--r--   0     1001      123     5780 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/headless.rs
--rw-r--r--   0     1001      123     1571 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123      975 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/pipe.rs
--rw-r--r--   0     1001      123     7516 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123     1366 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/utils.rs
--rw-r--r--   0     1001      123     6168 2023-05-15 20:19:25.000000 pywry-0.5.7/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    63815 2023-05-15 20:19:25.000000 pywry-0.5.7/Cargo.lock
--rw-r--r--   0     1001      123     1155 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/py.typed
--rw-r--r--   0     1001      123      180 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/__init__.py
--rw-r--r--   0     1001      123    14417 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/core.py
--rw-r--r--   0     1001      123      217 2023-05-15 20:19:25.000000 pywry-0.5.7/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123      733 2023-05-15 20:19:25.000000 pywry-0.5.7/Cargo.toml
--rw-r--r--   0     1001      123     3565 2023-05-15 20:19:25.000000 pywry-0.5.7/src/constants.rs
--rw-r--r--   0     1001      123     6202 2023-05-15 20:19:25.000000 pywry-0.5.7/src/events.rs
--rw-r--r--   0     1001      123     3733 2023-05-15 20:19:25.000000 pywry-0.5.7/src/handlers.rs
--rw-r--r--   0     1001      123     5780 2023-05-15 20:19:25.000000 pywry-0.5.7/src/headless.rs
--rw-r--r--   0     1001      123     1571 2023-05-15 20:19:25.000000 pywry-0.5.7/src/lib.rs
--rw-r--r--   0     1001      123      975 2023-05-15 20:19:25.000000 pywry-0.5.7/src/pipe.rs
--rw-r--r--   0     1001      123     7516 2023-05-15 20:19:25.000000 pywry-0.5.7/src/structs.rs
--rw-r--r--   0     1001      123     1366 2023-05-15 20:19:25.000000 pywry-0.5.7/src/utils.rs
--rw-r--r--   0     1001      123     6168 2023-05-15 20:19:25.000000 pywry-0.5.7/src/window.rs
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pywry-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.8/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     4924 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     3565 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     6202 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/events.rs
+-rw-r--r--   0     1001      123     3733 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     7516 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/utils.rs
+-rw-r--r--   0     1001      123     6168 2023-05-15 22:14:50.000000 pywry-0.5.8/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    63815 2023-05-15 22:14:50.000000 pywry-0.5.8/Cargo.lock
+-rw-r--r--   0     1001      123     1155 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/py.typed
+-rw-r--r--   0     1001      123      180 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/__init__.py
+-rw-r--r--   0     1001      123    14443 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/core.py
+-rw-r--r--   0     1001      123      217 2023-05-15 22:14:50.000000 pywry-0.5.8/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123      733 2023-05-15 22:14:50.000000 pywry-0.5.8/Cargo.toml
+-rw-r--r--   0     1001      123     3565 2023-05-15 22:14:50.000000 pywry-0.5.8/src/constants.rs
+-rw-r--r--   0     1001      123     6202 2023-05-15 22:14:50.000000 pywry-0.5.8/src/events.rs
+-rw-r--r--   0     1001      123     3733 2023-05-15 22:14:50.000000 pywry-0.5.8/src/handlers.rs
+-rw-r--r--   0     1001      123     5780 2023-05-15 22:14:50.000000 pywry-0.5.8/src/headless.rs
+-rw-r--r--   0     1001      123     1571 2023-05-15 22:14:50.000000 pywry-0.5.8/src/lib.rs
+-rw-r--r--   0     1001      123      975 2023-05-15 22:14:50.000000 pywry-0.5.8/src/pipe.rs
+-rw-r--r--   0     1001      123     7516 2023-05-15 22:14:50.000000 pywry-0.5.8/src/structs.rs
+-rw-r--r--   0     1001      123     1366 2023-05-15 22:14:50.000000 pywry-0.5.8/src/utils.rs
+-rw-r--r--   0     1001      123     6168 2023-05-15 22:14:50.000000 pywry-0.5.8/src/window.rs
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 pywry-0.5.8/PKG-INFO
```

### Comparing `pywry-0.5.7/pyproject.toml` & `pywry-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywry"
-version = "0.5.7"
+version = "0.5.8"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `pywry-0.5.7/rust_src/pywry/Cargo.toml` & `pywry-0.5.8/rust_src/pywry/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.7"
+version = "0.5.8"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.7/rust_src/pywry/LICENSE` & `pywry-0.5.8/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/README.md` & `pywry-0.5.8/rust_src/pywry/README.md`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/constants.rs` & `pywry-0.5.8/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/events.rs` & `pywry-0.5.8/rust_src/pywry/src/events.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/handlers.rs` & `pywry-0.5.8/rust_src/pywry/src/handlers.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/headless.rs` & `pywry-0.5.8/rust_src/pywry/src/headless.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/lib.rs` & `pywry-0.5.8/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/pipe.rs` & `pywry-0.5.8/rust_src/pywry/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/structs.rs` & `pywry-0.5.8/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/utils.rs` & `pywry-0.5.8/rust_src/pywry/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/rust_src/pywry/src/window.rs` & `pywry-0.5.8/rust_src/pywry/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/Cargo.lock` & `pywry-0.5.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1513,15 +1513,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.7"
+version = "0.5.8"
 dependencies = [
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
  "serde_json",
```

### Comparing `pywry-0.5.7/python/pywry/backend.py` & `pywry-0.5.8/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/python/pywry/core.py` & `pywry-0.5.8/python/pywry/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,13 +424,13 @@
 
     async def create_subprocess(self, cmd: Union[str, List[str]], **kwargs):
         if self.shell:
             if isinstance(cmd, list):
                 cmd = " ".join(cmd)
 
             return await asyncio.create_subprocess_shell(
-                cmd, PIPE, PIPE, PIPE, 2**64, **kwargs
+                cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE, limit=2**64, **kwargs
             )
 
         return await asyncio.create_subprocess_exec(
             *cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE, limit=2**64, **kwargs
         )
```

### Comparing `pywry-0.5.7/Cargo.toml` & `pywry-0.5.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.7"
+version = "0.5.8"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.7/src/constants.rs` & `pywry-0.5.8/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/events.rs` & `pywry-0.5.8/src/events.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/handlers.rs` & `pywry-0.5.8/src/handlers.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/headless.rs` & `pywry-0.5.8/src/headless.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/lib.rs` & `pywry-0.5.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/pipe.rs` & `pywry-0.5.8/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/structs.rs` & `pywry-0.5.8/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/utils.rs` & `pywry-0.5.8/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/src/window.rs` & `pywry-0.5.8/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.7/PKG-INFO` & `pywry-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywry
-Version: 0.5.7
+Version: 0.5.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Dist: setproctitle
```

