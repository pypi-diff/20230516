# Comparing `tmp/foxglove-data-platform-0.5.0.tar.gz` & `tmp/foxglove-data-platform-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxglove-data-platform-0.5.0.tar", last modified: Wed Apr 19 23:07:27 2023, max compression
+gzip compressed data, was "foxglove-data-platform-0.6.0.tar", last modified: Tue May 16 21:24:15 2023, max compression
```

## Comparing `foxglove-data-platform-0.5.0.tar` & `foxglove-data-platform-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.116818 foxglove-data-platform-0.5.0/foxglove_data_platform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/foxglove_data_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/foxglove_data_platform/client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/foxglove_data_platform/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.116818 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 23:07:27.000000 foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:07:27.120818 foxglove-data-platform-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/string_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_json_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_protobuf_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_ros1_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-19 23:06:42.000000 foxglove-data-platform-0.5.0/tests/test_ros2_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/foxglove_data_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/foxglove_data_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26827 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/foxglove_data_platform/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/foxglove_data_platform/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:24:15.000000 foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 21:24:15.543779 foxglove-data-platform-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:24:15.539779 foxglove-data-platform-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/string_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_json_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_protobuf_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_ros1_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 21:23:37.000000 foxglove-data-platform-0.6.0/tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.5.0/LICENSE` & `foxglove-data-platform-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/PKG-INFO` & `foxglove-data-platform-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.5.0
+Version: 0.6.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.5.0/README.md` & `foxglove-data-platform-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/foxglove_data_platform/client.py` & `foxglove-data-platform-0.6.0/foxglove_data_platform/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import os
 from enum import Enum
 from io import BytesIO
 import json
 import warnings
 from typing import IO, Any, Dict, List, Optional, Union
+import base64
 
 import arrow
 import requests
 from typing_extensions import Protocol
 
 
 try:
@@ -140,14 +141,29 @@
         response.reason = json.get("error", response.reason)
 
     response.raise_for_status()
 
     return json
 
 
+def _download_stream_with_progress(
+    url: str,
+    headers: Optional[dict] = None,
+    callback: Optional[ProgressCallback] = None,
+):
+    response = requests.get(url, headers=headers, stream=True)
+    response.raise_for_status()
+    data = BytesIO()
+    for chunk in response.iter_content(chunk_size=32 * 1024):
+        data.write(chunk)
+        if callback:
+            callback(progress=data.tell())
+    return data.getvalue()
+
+
 class Client:
     def __init__(self, token: str, host: str = "api.foxglove.dev"):
         self.__token = token
         self.__headers = {
             "Content-type": "application/json",
             "Authorization": "Bearer " + self.__token,
         }
@@ -282,26 +298,58 @@
             else:
                 decoder = decoders[schema.encoding]
             output_messages.append(
                 (channel.topic, message, decoder.decode(schema, message))
             )
         return output_messages
 
+    def download_recording_data(
+        self,
+        *,
+        id: str,
+        output_format: OutputFormat = OutputFormat.mcap0,
+        include_attachments: bool = False,
+        callback: Optional[ProgressCallback] = None,
+    ):
+        """
+        Returns raw data bytes for a recording.
+
+        :param id: the ID of the recording.
+        :param include_attachments: whether to include MCAP attachments in the returned data.
+        :param output_format: The output format of the data, defaulting to .mcap.
+            Note: You can only export a .bag file if you originally uploaded a .bag file.
+        :param callback: an optional callback to report download progress.
+        """
+        params = {
+            "recordingId": id,
+            "includeAttachments": include_attachments,
+            "outputFormat": output_format.value,
+        }
+        link_response = requests.post(
+            self.__url__("/v1/data/stream"),
+            headers=self.__headers,
+            json={k: v for k, v in params.items() if v is not None},
+        )
+
+        json = json_or_raise(link_response)
+
+        return _download_stream_with_progress(json["link"], callback=callback)
+
     def download_data(
         self,
         *,
         device_id: str,
         start: datetime.datetime,
         end: datetime.datetime,
         topics: List[str] = [],
         output_format: OutputFormat = OutputFormat.mcap0,
         callback: Optional[ProgressCallback] = None,
     ) -> bytes:
         """
-        Returns raw data bytes.
+        Returns raw data bytes for a device and time range.
 
         device_id: The id of the device that originated the desired data.
         start: The earliest time from which to retrieve data.
         end: The latest time from which to retrieve data.
         topics: An optional list of topics to retrieve.
             All topics will be retrieved if this is omitted.
         output_format: The output format of the data, either .bag or .mcap, defaulting to .mcap.
@@ -317,22 +365,15 @@
             self.__url__("/v1/data/stream"),
             headers=self.__headers,
             json={k: v for k, v in params.items() if v is not None},
         )
 
         json = json_or_raise(link_response)
 
-        link = json["link"]
-        response = requests.get(link, stream=True)
-        data = BytesIO()
-        for chunk in response.iter_content(chunk_size=32 * 1024):
-            data.write(chunk)
-            if callback:
-                callback(progress=data.tell())
-        return data.getvalue()
+        return _download_stream_with_progress(json["link"], callback=callback)
 
     def get_coverage(
         self,
         *,
         start: datetime.datetime,
         end: datetime.datetime,
         device_id: Optional[str] = None,
@@ -523,44 +564,196 @@
                 "filename": i["filename"],
                 "input_size": i["inputSize"],
                 "total_output_size": i["totalOutputSize"],
             }
             for i in json
         ]
 
+    def get_recordings(
+        self,
+        *,
+        device_id: Optional[str] = None,
+        start: Optional[datetime.datetime] = None,
+        end: Optional[datetime.datetime] = None,
+        path: Optional[str] = None,
+        site_id: Optional[str] = None,
+        edge_site_id: Optional[str] = None,
+        import_status: Optional[str] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        sort_by: Optional[str] = None,
+        sort_order: Optional[str] = None,
+    ):
+        """Fetches recordings.
+
+        :param device_id: Optionally filter responses by this device ID.
+        :param start: Optionally specify the start of an inclusive time range.
+            Only recordings with messages within this time range will be returned.
+        :param end: Optionally specify the end of an inclusive time range.
+            Only recordings with messages within this time range will be returned.
+        :param path: Optionally filter responses to recordings with a matching path.
+        :param site_id: Optionally filter responses to recordings stored at this primary site.
+        :param edge_site_id: Optionally filter responses to recordings stored at this edge site.
+        :param import_status: Optionally filter responses to recordings with this import status.
+        :param sort_by: Optionally sort returned recordings by a field in the response type.
+            Specifying duration sorts by the duration between the recording start and end fields.
+        :param sort_order: Optionally specify the sort order, either "asc" or "desc".
+        :param limit: Optionally limit the number of records returned.
+        :param offset: Optionally offset the results by this many records.
+        """
+        all_params = {
+            "device.id": device_id,
+            "start": start.astimezone().isoformat() if start else None,
+            "end": end.astimezone().isoformat() if end else None,
+            "site.id": site_id,
+            "edgeSite.id": edge_site_id,
+            "importStatus": import_status,
+            "path": path,
+            "sortBy": camelize(sort_by),
+            "sortOrder": sort_order,
+            "limit": limit,
+            "offset": offset,
+        }
+        response = requests.get(
+            self.__url__("/v1/recordings"),
+            params={k: v for k, v in all_params.items() if v is not None},
+            headers=self.__headers,
+        )
+        json = json_or_raise(response)
+
+        out = []
+        for i in json:
+            imported_at = i.get("importedAt")
+            if imported_at is not None:
+                imported_at = arrow.get(imported_at).datetime
+            out.append(
+                {
+                    "id": i["id"],
+                    "path": i["path"],
+                    "size": i["size"],
+                    "message_count": i.get("messageCount"),
+                    "created_at": arrow.get(i["createdAt"]).datetime,
+                    "imported_at": imported_at,
+                    "start": arrow.get(i["start"]).datetime,
+                    "end": arrow.get(i["end"]).datetime,
+                    "import_status": i["importStatus"],
+                    "site": i.get("site"),
+                    "edge_site": i.get("edgeSite"),
+                    "device": i.get("device"),
+                    "metadata": i.get("metadata"),
+                }
+            )
+
+        return out
+
+    def get_attachments(
+        self,
+        *,
+        device_id: Optional[str] = None,
+        recording_id: Optional[str] = None,
+        site_id: Optional[str] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        sort_by: Optional[str] = None,
+        sort_order: Optional[str] = None,
+    ):
+        """List recording attachments.
+
+        :param device_id: Optionally filter responses by this device ID.
+        :param recording_id: Optionally filter responses by this recording ID.
+        :param site_id: Optionally filter responses by this site ID.
+        :param sort_by: Optionally sort responses by this field name.
+            currently only "log_time" is supported.
+        :param sort_order: Optionally specify the sort order, either "asc" or "desc".
+        :param limit: Optionally limit the number of records returned.
+        :param offset: Optionally offset the results by this many records.
+        """
+        all_params = {
+            "deviceId": device_id,
+            "siteId": site_id,
+            "recordingId": recording_id,
+            "sortBy": camelize(sort_by),
+            "sortOrder": sort_order,
+            "limit": limit,
+            "offset": offset,
+        }
+        response = requests.get(
+            self.__url__("/v1/recording-attachments"),
+            params={k: v for k, v in all_params.items() if v is not None},
+            headers=self.__headers,
+        )
+        json = json_or_raise(response)
+        return [
+            {
+                "id": i["id"],
+                "recording_id": i["recordingId"],
+                "site_id": i["siteId"],
+                "name": i["name"],
+                "media_type": i["mediaType"],
+                "size": i["size"],
+                "crc": i["crc"],
+                "fingerprint": i["fingerprint"],
+                "log_time": arrow.get(i["logTime"]).datetime,
+                "create_time": arrow.get(i["createTime"]).datetime,
+            }
+            for i in json
+        ]
+
+    def download_attachment(
+        self,
+        *,
+        id: str,
+        callback: Optional[ProgressCallback] = None,
+    ):
+        """Download an attachment by ID.
+
+        :param attachment_id: the attachment ID.
+        :param callback: a callback to track download progress
+        :returns: The downloaded attachment bytes.
+        """
+        return _download_stream_with_progress(
+            self.__url__(f"/v1/recording-attachments/{id}/download"),
+            headers=self.__headers,
+            callback=callback,
+        )
+
     def get_topics(
         self,
         *,
         device_id: str,
         start: datetime.datetime,
         end: datetime.datetime,
+        include_schemas: bool = False,
     ):
         response = requests.get(
             self.__url__("/v1/data/topics"),
             headers=self.__headers,
             params={
                 "deviceId": device_id,
                 "start": start.astimezone().isoformat(),
                 "end": end.astimezone().isoformat(),
-                "includeSchemas": "false",
+                "includeSchemas": "true" if include_schemas else "false",
             },
         )
 
         json = json_or_raise(response)
 
-        return [
-            {
+        results = []
+        for t in json:
+            result = {
                 "topic": t["topic"],
                 "version": t["version"],
                 "encoding": t["encoding"],
                 "schema_encoding": t["schemaEncoding"],
                 "schema_name": t["schemaName"],
             }
-            for t in json
-        ]
+            if include_schemas:
+                result["schema"] = base64.b64decode(t["schema"])
+            results.append(result)
+        return results
 
     def upload_data(
         self,
         *,
         device_id: str,
         filename: str,
         data: Union[bytes, IO[Any]],
```

### Comparing `foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/PKG-INFO` & `foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxglove-data-platform
-Version: 0.5.0
+Version: 0.6.0
 Summary: Client library for Foxglove Data Platform.
 Home-page: https://github.com/foxglove/py-data-platform
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `foxglove-data-platform-0.5.0/foxglove_data_platform.egg-info/SOURCES.txt` & `foxglove-data-platform-0.6.0/foxglove_data_platform.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 foxglove_data_platform.egg-info/dependency_links.txt
 foxglove_data_platform.egg-info/requires.txt
 foxglove_data_platform.egg-info/top_level.txt
 tests/__init__.py
 tests/api_url.py
 tests/generate.py
 tests/string_message_pb2.py
+tests/test_attachments.py
 tests/test_client.py
 tests/test_coverage.py
 tests/test_data.py
 tests/test_devices.py
 tests/test_events.py
 tests/test_imports.py
 tests/test_json_messages.py
 tests/test_protobuf_messages.py
+tests/test_recordings.py
 tests/test_ros1_messages.py
 tests/test_ros2_messages.py
```

### Comparing `foxglove-data-platform-0.5.0/setup.cfg` & `foxglove-data-platform-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foxglove-data-platform
-version = 0.5.0
+version = 0.6.0
 description = Client library for Foxglove Data Platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxglove/py-data-platform
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `foxglove-data-platform-0.5.0/tests/generate.py` & `foxglove-data-platform-0.6.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_client.py` & `foxglove-data-platform-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_coverage.py` & `foxglove-data-platform-0.6.0/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_data.py` & `foxglove-data-platform-0.6.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_devices.py` & `foxglove-data-platform-0.6.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_events.py` & `foxglove-data-platform-0.6.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_imports.py` & `foxglove-data-platform-0.6.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_protobuf_messages.py` & `foxglove-data-platform-0.6.0/tests/test_protobuf_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_ros1_messages.py` & `foxglove-data-platform-0.6.0/tests/test_ros1_messages.py`

 * *Files identical despite different names*

### Comparing `foxglove-data-platform-0.5.0/tests/test_ros2_messages.py` & `foxglove-data-platform-0.6.0/tests/test_ros2_messages.py`

 * *Files identical despite different names*

