# Comparing `tmp/gradio_client-0.2.4.tar.gz` & `tmp/gradio_client-0.2.5.tar.gz`

## Comparing `gradio_client-0.2.4.tar` & `gradio_client-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.4/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.4/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/__init__.py
--rw-r--r--   0        0        0    46928 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/client.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/media_data.py
--rw-r--r--   0        0        0    19192 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/types.json
--rw-r--r--   0        0        0    16272 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.4/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.2.4/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.5/README.md
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.5/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/__init__.py
+-rw-r--r--   0        0        0    47450 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/client.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/media_data.py
+-rw-r--r--   0        0        0    19194 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/types.json
+-rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.5/gradio_client/version.txt
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 gradio_client-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 gradio_client-0.2.5/PKG-INFO
```

### Comparing `gradio_client-0.2.4/README.md` & `gradio_client-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.4/gradio_client/client.py` & `gradio_client-0.2.5/gradio_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         inferred_fn_index = self._infer_fn_index(api_name, fn_index)
 
         helper = None
         if self.endpoints[inferred_fn_index].use_ws:
             helper = Communicator(
                 Lock(),
                 JobStatus(),
-                self.endpoints[inferred_fn_index].deserialize,
+                self.endpoints[inferred_fn_index].process_predictions,
                 self.reset_url,
             )
         end_to_end_fn = self.endpoints[inferred_fn_index].make_end_to_end_fn(helper)
         future = self.executor.submit(end_to_end_fn, *args)
 
         job = Job(
             future, communicator=helper, verbose=self.verbose, space_id=self.space_id
@@ -435,15 +435,15 @@
             human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}\n"
             for fn_index, endpoint_info in info["unnamed_endpoints"].items():
                 # When loading from json, the fn_indices are read as strings
                 # because json keys can only be strings
                 human_info += self._render_endpoints_info(int(fn_index), endpoint_info)
         else:
             if num_unnamed_endpoints > 0:
-                human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(`all_endpoints=True`)\n"
+                human_info += f"\nUnnamed API endpoints: {num_unnamed_endpoints}, to view, run Client.view_api(all_endpoints=True)\n"
 
         if print_info:
             print(human_info)
         if return_format == "str":
             return human_info
         elif return_format == "dict":
             return info
@@ -612,19 +612,19 @@
     def make_end_to_end_fn(self, helper: Communicator | None = None):
 
         _predict = self.make_predict(helper)
 
         def _inner(*data):
             if not self.is_valid:
                 raise utils.InvalidAPIEndpointError()
+            data = self.insert_state(*data)
             if self.client.serialize:
                 data = self.serialize(*data)
             predictions = _predict(*data)
-            if self.client.serialize:
-                predictions = self.deserialize(*predictions)
+            predictions = self.process_predictions(*predictions)
             # Append final output only if not already present
             # for consistency between generators and not generators
             if helper:
                 with helper.lock:
                     if not helper.job.outputs:
                         helper.job.outputs.append(predictions)
             return predictions
@@ -741,61 +741,78 @@
         """Helper function to modify the input data with the uploaded files."""
         file_counter = 0
         for i, t in enumerate(self.input_component_types):
             if t in ["file", "uploadbutton"]:
                 data[i] = files[file_counter]
                 file_counter += 1
 
-    def serialize(self, *data) -> tuple:
+    def insert_state(self, *data) -> tuple:
         data = list(data)
         for i, input_component_type in enumerate(self.input_component_types):
             if input_component_type == utils.STATE_COMPONENT:
                 data.insert(i, None)
+        return tuple(data)
+
+    def remove_state(self, *data) -> tuple:
+        data = [
+            d
+            for d, oct in zip(data, self.output_component_types)
+            if oct != utils.STATE_COMPONENT
+        ]
+        return tuple(data)
+
+    def reduce_singleton_output(self, *data) -> Any:
+        if (
+            len(
+                [
+                    oct
+                    for oct in self.output_component_types
+                    if oct != utils.STATE_COMPONENT
+                ]
+            )
+            == 1
+        ):
+            return data[0]
+        else:
+            return data
+
+    def serialize(self, *data) -> tuple:
         assert len(data) == len(
             self.serializers
         ), f"Expected {len(self.serializers)} arguments, got {len(data)}"
 
         files = [
             f
             for f, t in zip(data, self.input_component_types)
             if t in ["file", "uploadbutton"]
         ]
         uploaded_files = self._upload(files)
-        self._add_uploaded_files_to_data(uploaded_files, data)
+        self._add_uploaded_files_to_data(uploaded_files, list(data))
 
         o = tuple([s.serialize(d) for s, d in zip(self.serializers, data)])
         return o
 
-    def deserialize(self, *data) -> tuple | Any:
+    def deserialize(self, *data) -> tuple:
         assert len(data) == len(
             self.deserializers
         ), f"Expected {len(self.deserializers)} outputs, got {len(data)}"
         outputs = tuple(
             [
                 s.deserialize(d, hf_token=self.client.hf_token, root_url=self.root_url)
-                for s, d, oct in zip(
-                    self.deserializers, data, self.output_component_types
-                )
-                if oct != utils.STATE_COMPONENT
+                for s, d in zip(self.deserializers, data)
             ]
         )
-        if (
-            len(
-                [
-                    oct
-                    for oct in self.output_component_types
-                    if oct != utils.STATE_COMPONENT
-                ]
-            )
-            == 1
-        ):
-            output = outputs[0]
-        else:
-            output = outputs
-        return output
+        return outputs
+
+    def process_predictions(self, *predictions):
+        if self.client.serialize:
+            predictions = self.deserialize(*predictions)
+        predictions = self.remove_state(*predictions)
+        predictions = self.reduce_singleton_output(*predictions)
+        return predictions
 
     def _setup_serializers(self) -> tuple[list[Serializable], list[Serializable]]:
         inputs = self.dependency["inputs"]
         serializers = []
 
         for i in inputs:
             for component in self.client.config["components"]:
```

### Comparing `gradio_client-0.2.4/gradio_client/documentation.py` & `gradio_client-0.2.5/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.4/gradio_client/media_data.py` & `gradio_client-0.2.5/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.4/gradio_client/serializing.py` & `gradio_client-0.2.5/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
     def serialize(
         self,
         x: str | None,
         load_dir: str | Path = "",
     ) -> str | None:
         """
-        Convert from human-friendly version of a file (string filepath) to a seralized
+        Convert from human-friendly version of a file (string filepath) to a serialized
         representation (base64).
         Parameters:
             x: String path to file to serialize
             load_dir: Path to directory containing x
         """
         if x is None or x == "":
             return None
@@ -304,15 +304,15 @@
     def serialize(
         self,
         x: str | FileData | None | list[str | FileData | None],
         load_dir: str | Path = "",
     ) -> FileData | None | list[FileData | None]:
         """
         Convert from human-friendly version of a file (string filepath) to a
-        seralized representation (base64)
+        serialized representation (base64)
         Parameters:
             x: String path to file to serialize
             load_dir: Path to directory containing x
         """
         if x is None or x == "":
             return None
         if isinstance(x, list):
```

### Comparing `gradio_client-0.2.4/gradio_client/types.json` & `gradio_client-0.2.5/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.4/gradio_client/utils.py` & `gradio_client-0.2.5/gradio_client/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,28 +165,28 @@
     )
 
 
 @dataclass
 class JobStatus:
     """The job status.
 
-    Keeps strack of the latest status update and intermediate outputs (not yet implements).
+    Keeps track of the latest status update and intermediate outputs (not yet implements).
     """
 
     latest_status: StatusUpdate = field(default_factory=create_initial_status_update)
     outputs: list[Any] = field(default_factory=list)
 
 
 @dataclass
 class Communicator:
     """Helper class to help communicate between the worker thread and main thread."""
 
     lock: Lock
     job: JobStatus
-    deserialize: Callable[..., tuple]
+    prediction_processor: Callable[..., tuple]
     reset_url: str
     should_cancel: bool = False
 
 
 ########################
 # Network utils
 ########################
@@ -247,15 +247,15 @@
                     progress_data=ProgressUnit.from_ws_msg(resp["progress_data"])
                     if has_progress
                     else None,
                 )
                 output = resp.get("output", {}).get("data", [])
                 if output and status_update.code != Status.FINISHED:
                     try:
-                        result = helper.deserialize(*output)
+                        result = helper.prediction_processor(*output)
                     except Exception as e:
                         result = [e]
                     helper.job.outputs.append(result)
                 helper.job.latest_status = status_update
         if resp["msg"] == "queue_full":
             raise QueueError("Queue is full! Please try again.")
         if resp["msg"] == "send_hash":
@@ -376,18 +376,18 @@
             if len(filename) == 0:
                 break
             filename = filename[:-1]
             filename_len = len(filename.encode())
     return filename
 
 
-def sanitize_parameter_names(original_param_name: str) -> str:
-    """Strips invalid characters from a parameter name and replaces spaces with underscores."""
+def sanitize_parameter_names(original_name: str) -> str:
+    """Cleans up a Python parameter name to make the API info more readable."""
     return (
-        "".join([char for char in original_param_name if char.isalnum() or char in " "])
+        "".join([char for char in original_name if char.isalnum() or char in " _"])
         .replace(" ", "_")
         .lower()
     )
 
 
 def decode_base64_to_file(
     encoding: str,
```

### Comparing `gradio_client-0.2.4/.gitignore` & `gradio_client-0.2.5/.gitignore`

 * *Files 15% similar despite different names*

```diff
@@ -54,8 +54,9 @@
 
 # FRP
 gradio/frpc_*
 
 # js
 node_modules
 public/build/
-test-results
+test-results
+client/js/test.js
```

### Comparing `gradio_client-0.2.4/pyproject.toml` & `gradio_client-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.4/PKG-INFO` & `gradio_client-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Requires-Python: >=3.7
 Requires-Dist: fsspec
```

