# Comparing `tmp/granian-0.4.1.tar.gz` & `tmp/granian-0.4.2.tar.gz`

## Comparing `granian-0.4.1.tar` & `granian-0.4.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.1/Cargo.toml
--rw-r--r--   0     1001      123     1486 2023-05-12 10:32:03.000000 granian-0.4.1/LICENSE
--rw-r--r--   0     1001      123     4024 2023-05-12 10:32:03.000000 granian-0.4.1/README.md
--rw-r--r--   0     1001      123       54 2023-05-12 10:32:03.000000 granian-0.4.1/build.rs
--rw-r--r--   0     1001      123       28 2023-05-12 10:32:03.000000 granian-0.4.1/granian/__init__.py
--rw-r--r--   0     1001      123       22 2023-05-12 10:32:03.000000 granian-0.4.1/granian/__version__.py
--rw-r--r--   0     1001      123     1868 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_granian.pyi
--rw-r--r--   0     1001      123     1677 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_internal.py
--rw-r--r--   0     1001      123     2862 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_loops.py
--rw-r--r--   0     1001      123       93 2023-05-12 10:32:03.000000 granian-0.4.1/granian/_types.py
--rw-r--r--   0     1001      123     4682 2023-05-12 10:32:03.000000 granian-0.4.1/granian/asgi.py
--rw-r--r--   0     1001      123     3590 2023-05-12 10:32:03.000000 granian-0.4.1/granian/cli.py
--rw-r--r--   0     1001      123      357 2023-05-12 10:32:03.000000 granian-0.4.1/granian/constants.py
--rw-r--r--   0     1001      123     1328 2023-05-12 10:32:03.000000 granian-0.4.1/granian/log.py
--rw-r--r--   0     1001      123      153 2023-05-12 10:32:03.000000 granian-0.4.1/granian/net.py
--rw-r--r--   0     1001      123        0 2023-05-12 10:32:03.000000 granian-0.4.1/granian/py.typed
--rw-r--r--   0     1001      123      462 2023-05-12 10:32:03.000000 granian-0.4.1/granian/rsgi.py
--rw-r--r--   0     1001      123    10646 2023-05-12 10:32:03.000000 granian-0.4.1/granian/server.py
--rw-r--r--   0     1001      123     2068 2023-05-12 10:32:03.000000 granian-0.4.1/granian/wsgi.py
--rw-r--r--   0     1001      123     1624 2023-05-12 10:32:03.000000 granian-0.4.1/pyproject.toml
--rw-r--r--   0     1001      123     6824 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/callbacks.rs
--rw-r--r--   0     1001      123     1611 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/errors.rs
--rw-r--r--   0     1001      123     4765 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/http.rs
--rw-r--r--   0     1001      123    15092 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/io.rs
--rw-r--r--   0     1001      123      329 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/mod.rs
--rw-r--r--   0     1001      123     2995 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/serve.rs
--rw-r--r--   0     1001      123     2708 2023-05-12 10:32:03.000000 granian-0.4.1/src/asgi/types.rs
--rw-r--r--   0     1001      123     8784 2023-05-12 10:32:03.000000 granian-0.4.1/src/callbacks.rs
--rw-r--r--   0     1001      123      415 2023-05-12 10:32:03.000000 granian-0.4.1/src/http.rs
--rw-r--r--   0     1001      123      550 2023-05-12 10:32:03.000000 granian-0.4.1/src/lib.rs
--rw-r--r--   0     1001      123     6058 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      123      565 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/errors.rs
--rw-r--r--   0     1001      123     5186 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/http.rs
--rw-r--r--   0     1001      123    10350 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/io.rs
--rw-r--r--   0     1001      123      609 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/mod.rs
--rw-r--r--   0     1001      123     2995 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/serve.rs
--rw-r--r--   0     1001      123     5619 2023-05-12 10:32:03.000000 granian-0.4.1/src/rsgi/types.rs
--rw-r--r--   0     1001      123     8066 2023-05-12 10:32:03.000000 granian-0.4.1/src/runtime.rs
--rw-r--r--   0     1001      123     4301 2023-05-12 10:32:03.000000 granian-0.4.1/src/tcp.rs
--rw-r--r--   0     1001      123     2431 2023-05-12 10:32:03.000000 granian-0.4.1/src/tls.rs
--rw-r--r--   0     1001      123      837 2023-05-12 10:32:03.000000 granian-0.4.1/src/utils.rs
--rw-r--r--   0     1001      123    16456 2023-05-12 10:32:03.000000 granian-0.4.1/src/workers.rs
--rw-r--r--   0     1001      123     3435 2023-05-12 10:32:03.000000 granian-0.4.1/src/ws.rs
--rw-r--r--   0     1001      123     1027 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      123      308 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/errors.rs
--rw-r--r--   0     1001      123     1638 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/http.rs
--rw-r--r--   0     1001      123      312 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/mod.rs
--rw-r--r--   0     1001      123     2206 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/serve.rs
--rw-r--r--   0     1001      123     4151 2023-05-12 10:32:03.000000 granian-0.4.1/src/wsgi/types.rs
--rw-r--r--   0     1001      123     3078 2023-05-12 10:32:03.000000 granian-0.4.1/tests/apps/asgi.py
--rw-r--r--   0     1001      123     2490 2023-05-12 10:32:03.000000 granian-0.4.1/tests/apps/rsgi.py
--rw-r--r--   0     1001      123      861 2023-05-12 10:32:03.000000 granian-0.4.1/tests/apps/wsgi.py
--rw-r--r--   0     1001      123     1759 2023-05-12 10:32:03.000000 granian-0.4.1/tests/conftest.py
--rw-r--r--   0     1001      123     1139 2023-05-12 10:32:03.000000 granian-0.4.1/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      123     1704 2023-05-12 10:32:03.000000 granian-0.4.1/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      123     1830 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_asgi.py
--rw-r--r--   0     1001      123     1851 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_https.py
--rw-r--r--   0     1001      123     1450 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_rsgi.py
--rw-r--r--   0     1001      123     2487 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_ws.py
--rw-r--r--   0     1001      123     1438 2023-05-12 10:32:03.000000 granian-0.4.1/tests/test_wsgi.py
--rw-r--r--   0     1001      123    33385 2023-05-12 10:32:03.000000 granian-0.4.1/Cargo.lock
--rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 granian-0.4.2/Cargo.toml
+-rw-r--r--   0     1001      123     1486 2023-05-16 12:04:16.000000 granian-0.4.2/LICENSE
+-rw-r--r--   0     1001      123     4024 2023-05-16 12:04:16.000000 granian-0.4.2/README.md
+-rw-r--r--   0     1001      123       54 2023-05-16 12:04:16.000000 granian-0.4.2/build.rs
+-rw-r--r--   0     1001      123       28 2023-05-16 12:04:16.000000 granian-0.4.2/granian/__init__.py
+-rw-r--r--   0     1001      123       22 2023-05-16 12:04:16.000000 granian-0.4.2/granian/__version__.py
+-rw-r--r--   0     1001      123     1868 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_granian.pyi
+-rw-r--r--   0     1001      123     1677 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_internal.py
+-rw-r--r--   0     1001      123     2862 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_loops.py
+-rw-r--r--   0     1001      123       93 2023-05-16 12:04:16.000000 granian-0.4.2/granian/_types.py
+-rw-r--r--   0     1001      123     4682 2023-05-16 12:04:16.000000 granian-0.4.2/granian/asgi.py
+-rw-r--r--   0     1001      123     3590 2023-05-16 12:04:16.000000 granian-0.4.2/granian/cli.py
+-rw-r--r--   0     1001      123      357 2023-05-16 12:04:16.000000 granian-0.4.2/granian/constants.py
+-rw-r--r--   0     1001      123     1328 2023-05-16 12:04:16.000000 granian-0.4.2/granian/log.py
+-rw-r--r--   0     1001      123      153 2023-05-16 12:04:16.000000 granian-0.4.2/granian/net.py
+-rw-r--r--   0     1001      123        0 2023-05-16 12:04:16.000000 granian-0.4.2/granian/py.typed
+-rw-r--r--   0     1001      123      462 2023-05-16 12:04:16.000000 granian-0.4.2/granian/rsgi.py
+-rw-r--r--   0     1001      123    10646 2023-05-16 12:04:16.000000 granian-0.4.2/granian/server.py
+-rw-r--r--   0     1001      123     2068 2023-05-16 12:04:16.000000 granian-0.4.2/granian/wsgi.py
+-rw-r--r--   0     1001      123     1624 2023-05-16 12:04:16.000000 granian-0.4.2/pyproject.toml
+-rw-r--r--   0     1001      123     6984 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      123     1611 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/errors.rs
+-rw-r--r--   0     1001      123     4765 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/http.rs
+-rw-r--r--   0     1001      123    15092 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/io.rs
+-rw-r--r--   0     1001      123      329 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/mod.rs
+-rw-r--r--   0     1001      123     2995 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/serve.rs
+-rw-r--r--   0     1001      123     2708 2023-05-16 12:04:16.000000 granian-0.4.2/src/asgi/types.rs
+-rw-r--r--   0     1001      123     9591 2023-05-16 12:04:16.000000 granian-0.4.2/src/callbacks.rs
+-rw-r--r--   0     1001      123      415 2023-05-16 12:04:16.000000 granian-0.4.2/src/http.rs
+-rw-r--r--   0     1001      123      550 2023-05-16 12:04:16.000000 granian-0.4.2/src/lib.rs
+-rw-r--r--   0     1001      123     6256 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      123      565 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/errors.rs
+-rw-r--r--   0     1001      123     5186 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/http.rs
+-rw-r--r--   0     1001      123    10350 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/io.rs
+-rw-r--r--   0     1001      123      609 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/mod.rs
+-rw-r--r--   0     1001      123     2995 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/serve.rs
+-rw-r--r--   0     1001      123     5619 2023-05-16 12:04:16.000000 granian-0.4.2/src/rsgi/types.rs
+-rw-r--r--   0     1001      123     8066 2023-05-16 12:04:16.000000 granian-0.4.2/src/runtime.rs
+-rw-r--r--   0     1001      123     4301 2023-05-16 12:04:16.000000 granian-0.4.2/src/tcp.rs
+-rw-r--r--   0     1001      123     2431 2023-05-16 12:04:16.000000 granian-0.4.2/src/tls.rs
+-rw-r--r--   0     1001      123      837 2023-05-16 12:04:16.000000 granian-0.4.2/src/utils.rs
+-rw-r--r--   0     1001      123    16456 2023-05-16 12:04:16.000000 granian-0.4.2/src/workers.rs
+-rw-r--r--   0     1001      123     3435 2023-05-16 12:04:16.000000 granian-0.4.2/src/ws.rs
+-rw-r--r--   0     1001      123     1027 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      123      308 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/errors.rs
+-rw-r--r--   0     1001      123     1638 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/http.rs
+-rw-r--r--   0     1001      123      312 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/mod.rs
+-rw-r--r--   0     1001      123     2206 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/serve.rs
+-rw-r--r--   0     1001      123     4151 2023-05-16 12:04:16.000000 granian-0.4.2/src/wsgi/types.rs
+-rw-r--r--   0     1001      123     3078 2023-05-16 12:04:16.000000 granian-0.4.2/tests/apps/asgi.py
+-rw-r--r--   0     1001      123     2490 2023-05-16 12:04:16.000000 granian-0.4.2/tests/apps/rsgi.py
+-rw-r--r--   0     1001      123      861 2023-05-16 12:04:16.000000 granian-0.4.2/tests/apps/wsgi.py
+-rw-r--r--   0     1001      123     1759 2023-05-16 12:04:16.000000 granian-0.4.2/tests/conftest.py
+-rw-r--r--   0     1001      123     1139 2023-05-16 12:04:16.000000 granian-0.4.2/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      123     1704 2023-05-16 12:04:16.000000 granian-0.4.2/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      123     1830 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_asgi.py
+-rw-r--r--   0     1001      123     1851 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_https.py
+-rw-r--r--   0     1001      123     1450 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_rsgi.py
+-rw-r--r--   0     1001      123     2487 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_ws.py
+-rw-r--r--   0     1001      123     1438 2023-05-16 12:04:16.000000 granian-0.4.2/tests/test_wsgi.py
+-rw-r--r--   0     1001      123    33385 2023-05-16 12:04:16.000000 granian-0.4.2/Cargo.lock
+-rw-r--r--   0        0        0     5801 1970-01-01 00:00:00.000000 granian-0.4.2/PKG-INFO
```

### Comparing `granian-0.4.1/Cargo.toml` & `granian-0.4.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
```

### Comparing `granian-0.4.1/LICENSE` & `granian-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/README.md` & `granian-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/_granian.pyi` & `granian-0.4.2/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/_internal.py` & `granian-0.4.2/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/_loops.py` & `granian-0.4.2/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/asgi.py` & `granian-0.4.2/granian/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/cli.py` & `granian-0.4.2/granian/cli.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/log.py` & `granian-0.4.2/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/server.py` & `granian-0.4.2/granian/server.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/granian/wsgi.py` & `granian-0.4.2/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/pyproject.toml` & `granian-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/asgi/callbacks.rs` & `granian-0.4.2/src/asgi/callbacks.rs`

 * *Files 3% similar despite different names*

```diff
@@ -53,25 +53,27 @@
     }
 }
 
 #[pyclass]
 pub(crate) struct CallbackTaskHTTP {
     proto: Py<HTTPProtocol>,
     context: TaskLocals,
+    pycontext: PyObject,
     cb: PyObject
 }
 
 impl CallbackTaskHTTP {
     pub fn new(
         py: Python,
         cb: PyObject,
         proto: Py<HTTPProtocol>,
         context: TaskLocals
     ) -> PyResult<Self> {
-        Ok(Self { proto, context: context.copy_context(py)?, cb })
+        let pyctx = context.context(py);
+        Ok(Self { proto, context, pycontext: pyctx.call_method0("copy")?.into(), cb })
     }
 
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
                 let mut res = Response::new("Internal server error".into());
                 *res.status_mut() = hyper::StatusCode::INTERNAL_SERVER_ERROR;
@@ -87,15 +89,15 @@
 
     callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
 impl CallbackTaskHTTP {
-    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<()> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
@@ -132,25 +134,27 @@
     }
 }
 
 #[pyclass]
 pub(crate) struct CallbackTaskWebsocket {
     proto: Py<WebsocketProtocol>,
     context: TaskLocals,
+    pycontext: PyObject,
     cb: PyObject
 }
 
 impl CallbackTaskWebsocket {
     pub fn new(
         py: Python,
         cb: PyObject,
         proto: Py<WebsocketProtocol>,
         context: TaskLocals
     ) -> PyResult<Self> {
-        Ok(Self { proto, context: context.copy_context(py)?, cb })
+        let pyctx = context.context(py);
+        Ok(Self { proto, context, pycontext: pyctx.call_method0("copy")?.into(), cb })
     }
 
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
@@ -164,15 +168,15 @@
 
     callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
 impl CallbackTaskWebsocket {
-    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<()> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
```

### Comparing `granian-0.4.1/src/asgi/errors.rs` & `granian-0.4.2/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/asgi/http.rs` & `granian-0.4.2/src/asgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/asgi/io.rs` & `granian-0.4.2/src/asgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/asgi/serve.rs` & `granian-0.4.2/src/asgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/asgi/types.rs` & `granian-0.4.2/src/asgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/callbacks.rs` & `granian-0.4.2/src/callbacks.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+use once_cell::sync::OnceCell;
 use pyo3::prelude::*;
 use pyo3::pyclass::IterNextOutput;
 
 
+static CONTEXTVARS: OnceCell<PyObject> = OnceCell::new();
+static CONTEXT: OnceCell<PyObject> = OnceCell::new();
+
 #[derive(Clone)]
 pub(crate) struct CallbackWrapper {
     pub callback: PyObject,
     pub context: pyo3_asyncio::TaskLocals
 }
 
 impl CallbackWrapper {
@@ -185,28 +189,49 @@
 #[pymethods]
 impl PyFutureAwaitableResult {
     fn __await__(&mut self, py: Python) -> PyObject {
         self.inner.to_object(py)
     }
 }
 
+fn contextvars(py: Python) -> PyResult<&PyAny> {
+    Ok(CONTEXTVARS
+        .get_or_try_init(|| py.import("contextvars").map(|m| m.into()))?
+        .as_ref(py))
+}
+
+pub fn empty_pycontext(py: Python) -> PyResult<&PyAny> {
+    Ok(CONTEXT
+        .get_or_try_init(|| contextvars(py)?.getattr("Context")?.call0().map(|c| c.into()))?
+        .as_ref(py))
+}
+
 macro_rules! callback_impl_run {
     () => {
         pub fn run<'p>(self, py: Python<'p>) -> PyResult<&'p PyAny> {
             let event_loop = self.context.event_loop(py);
             let target = self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_task"))?;
-            event_loop.call_method1(pyo3::intern!(py, "call_soon_threadsafe"), (target,))
+            let kwctx = pyo3::types::PyDict::new(py);
+            kwctx.set_item(
+                pyo3::intern!(py, "context"),
+                crate::callbacks::empty_pycontext(py)?
+            )?;
+            event_loop.call_method(
+                pyo3::intern!(py, "call_soon_threadsafe"),
+                (target,),
+                Some(kwctx)
+            )
         }
     };
 }
 
 macro_rules! callback_impl_loop_run {
     () => {
         pub fn run<'p>(self, py: Python<'p>) -> PyResult<&'p PyAny> {
-            let context = self.context.context(py);
+            let context = self.pycontext.clone().into_ref(py);
             context.call_method1(
                 pyo3::intern!(py, "run"),
                 (self.into_py(py).getattr(py, pyo3::intern!(py, "_loop_step"))?,)
             )
         }
     };
 }
@@ -219,17 +244,17 @@
                     $py,
                     pyo3::intern!($py, "_asyncio_future_blocking")
                 ) {
                     Ok(v) => v.extract($py)?,
                     _ => false
                 };
 
-                let ctx = $pyself.context.context($py);
+                let ctx = $pyself.pycontext.clone();
                 let kwctx = pyo3::types::PyDict::new($py);
-                kwctx.set_item("context", ctx)?;
+                kwctx.set_item(pyo3::intern!($py, "context"), ctx)?;
 
                 match blocking {
                     true => {
                         res.setattr(
                             $py,
                             pyo3::intern!($py, "_asyncio_future_blocking"),
                             false
@@ -240,41 +265,41 @@
                             (
                                 $pyself
                                 .into_py($py)
                                 .getattr($py, pyo3::intern!($py, "_loop_wake"))?,
                             ),
                             Some(kwctx)
                         )?;
-                        Ok($py.None())
+                        Ok(())
                     },
                     false => {
                         let event_loop = $pyself.context.event_loop($py);
                         event_loop.call_method(
                             pyo3::intern!($py, "call_soon"),
                             (
                                 $pyself
                                 .into_py($py)
                                 .getattr($py, pyo3::intern!($py, "_loop_step"))?,
                             ),
                             Some(kwctx)
                         )?;
-                        Ok($py.None())
+                        Ok(())
                     }
                 }
             },
             Err(err) => {
-                match err.is_instance_of::<pyo3::exceptions::PyStopIteration>($py) {
-                    true => {
-                        $pyself.done($py);
-                        Ok($py.None())
-                    },
-                    false => {
-                        $pyself.err($py);
-                        Err(err)
-                    }
+                if (
+                    err.is_instance_of::<pyo3::exceptions::PyStopIteration>($py) ||
+                    err.is_instance_of::<pyo3::exceptions::asyncio::CancelledError>($py)
+                ) {
+                    $pyself.done($py);
+                    Ok(())
+                } else {
+                    $pyself.err($py);
+                    Err(err)
                 }
             }
         }
     };
 }
 
 macro_rules! callback_impl_loop_wake {
```

### Comparing `granian-0.4.1/src/lib.rs` & `granian-0.4.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/rsgi/callbacks.rs` & `granian-0.4.2/src/rsgi/callbacks.rs`

 * *Files 1% similar despite different names*

```diff
@@ -52,25 +52,27 @@
     }
 }
 
 #[pyclass]
 pub(crate) struct CallbackTaskHTTP {
     proto: Py<HTTPProtocol>,
     context: TaskLocals,
+    pycontext: PyObject,
     cb: PyObject
 }
 
 impl CallbackTaskHTTP {
     pub fn new(
         py: Python,
         cb: PyObject,
         proto: Py<HTTPProtocol>,
         context: TaskLocals
     ) -> PyResult<Self> {
-        Ok(Self { proto, context: context.copy_context(py)?, cb })
+        let pyctx = context.context(py);
+        Ok(Self { proto, context, pycontext: pyctx.call_method0(pyo3::intern!(py, "copy"))?.into(), cb })
     }
 
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let Some(tx) = proto.tx() {
                 let _ = tx.send(
                     PyResponse::Bytes(PyResponseBytes::empty(500, Vec::new()))
@@ -86,15 +88,15 @@
 
     callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
 impl CallbackTaskHTTP {
-    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<()> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
@@ -131,25 +133,27 @@
     }
 }
 
 #[pyclass]
 pub(crate) struct CallbackTaskWebsocket {
     proto: Py<WebsocketProtocol>,
     context: TaskLocals,
+    pycontext: PyObject,
     cb: PyObject
 }
 
 impl CallbackTaskWebsocket {
     pub fn new(
         py: Python,
         cb: PyObject,
         proto: Py<WebsocketProtocol>,
         context: TaskLocals
     ) -> PyResult<Self> {
-        Ok(Self { proto, context: context.copy_context(py)?, cb })
+        let pyctx = context.context(py);
+        Ok(Self { proto, context, pycontext: pyctx.call_method0(pyo3::intern!(py, "copy"))?.into(), cb })
     }
 
     fn done(&self, py: Python) {
         if let Ok(mut proto) = self.proto.as_ref(py).try_borrow_mut() {
             if let (Some(tx), res) = proto.tx() {
                 let _ = tx.send(res);
             }
@@ -163,15 +167,15 @@
 
     callback_impl_loop_run!();
     callback_impl_loop_err!();
 }
 
 #[pymethods]
 impl CallbackTaskWebsocket {
-    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<PyObject> {
+    fn _loop_step(pyself: PyRef<'_, Self>, py: Python) -> PyResult<()> {
         callback_impl_loop_step!(pyself, py)
     }
 
     fn _loop_wake(pyself: PyRef<'_, Self>, py: Python, fut: PyObject) -> PyResult<PyObject> {
         callback_impl_loop_wake!(pyself, py, fut)
     }
 }
```

### Comparing `granian-0.4.1/src/rsgi/errors.rs` & `granian-0.4.2/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/rsgi/http.rs` & `granian-0.4.2/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/rsgi/io.rs` & `granian-0.4.2/src/rsgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/rsgi/mod.rs` & `granian-0.4.2/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/rsgi/serve.rs` & `granian-0.4.2/src/rsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/rsgi/types.rs` & `granian-0.4.2/src/rsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/runtime.rs` & `granian-0.4.2/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/tcp.rs` & `granian-0.4.2/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/tls.rs` & `granian-0.4.2/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/utils.rs` & `granian-0.4.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/workers.rs` & `granian-0.4.2/src/workers.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/ws.rs` & `granian-0.4.2/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/wsgi/callbacks.rs` & `granian-0.4.2/src/wsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/wsgi/http.rs` & `granian-0.4.2/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/wsgi/serve.rs` & `granian-0.4.2/src/wsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/src/wsgi/types.rs` & `granian-0.4.2/src/wsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/apps/asgi.py` & `granian-0.4.2/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/apps/rsgi.py` & `granian-0.4.2/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/apps/wsgi.py` & `granian-0.4.2/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/conftest.py` & `granian-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/fixtures/tls/cert.pem` & `granian-0.4.2/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/fixtures/tls/key.pem` & `granian-0.4.2/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/test_asgi.py` & `granian-0.4.2/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/test_https.py` & `granian-0.4.2/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/test_rsgi.py` & `granian-0.4.2/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/test_ws.py` & `granian-0.4.2/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/tests/test_wsgi.py` & `granian-0.4.2/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-0.4.1/Cargo.lock` & `granian-0.4.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "granian"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "bytes",
  "futures",
  "hyper",
  "log",
  "mimalloc",
  "once_cell",
```

### Comparing `granian-0.4.1/PKG-INFO` & `granian-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granian
-Version: 0.4.1
+Version: 0.4.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -30,16 +30,16 @@
 Keywords: web,asyncio
 Home-Page: https://github.com/emmett-framework/granian
 Author: Giovanni Barillari <g@baro.dev>
 Author-email: Giovanni Barillari <g@baro.dev>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/emmett-framework/granian
 Project-URL: Funding, https://github.com/sponsors/gi0baro
+Project-URL: Homepage, https://github.com/emmett-framework/granian
 Project-URL: Source, https://github.com/emmett-framework/granian
 
 # Granian
 
 A Rust HTTP server for Python applications.
 
 ## Rationale
```

