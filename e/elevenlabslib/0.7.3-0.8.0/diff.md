# Comparing `tmp/elevenlabslib-0.7.3.tar.gz` & `tmp/elevenlabslib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.7.3.tar", last modified: Sun May 14 14:49:10 2023, max compression
+gzip compressed data, was "elevenlabslib-0.8.0.tar", last modified: Tue May 16 12:53:45 2023, max compression
```

## Comparing `elevenlabslib-0.7.3.tar` & `elevenlabslib-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:49:10.944555 elevenlabslib-0.7.3/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-05-14 14:49:10.943554 elevenlabslib-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 14:49:10.927556 elevenlabslib-0.7.3/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    15099 2023-05-14 09:41:13.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    37074 2023-05-14 14:34:49.000000 elevenlabslib-0.7.3/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.7.3/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5924 2023-05-14 14:15:27.000000 elevenlabslib-0.7.3/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:49:10.943554 elevenlabslib-0.7.3/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 14:49:10.000000 elevenlabslib-0.7.3/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-05-14 14:48:50.000000 elevenlabslib-0.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 14:49:10.944555 elevenlabslib-0.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 12:53:45.458269 elevenlabslib-0.8.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-05-16 12:53:45.457269 elevenlabslib-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 12:53:45.437269 elevenlabslib-0.8.0/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    18927 2023-05-16 12:47:18.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    37163 2023-05-16 11:50:49.000000 elevenlabslib-0.8.0/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.8.0/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     6285 2023-05-16 12:08:10.000000 elevenlabslib-0.8.0/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:53:45.456268 elevenlabslib-0.8.0/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-16 12:53:45.000000 elevenlabslib-0.8.0/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-16 12:53:02.000000 elevenlabslib-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:53:45.458269 elevenlabslib-0.8.0/setup.cfg
```

### Comparing `elevenlabslib-0.7.3/LICENSE` & `elevenlabslib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.3/PKG-INFO` & `elevenlabslib-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.3
+Version: 0.8.0
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.3/README.md` & `elevenlabslib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsUser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import io
 import zipfile
 
 from typing import TYPE_CHECKING, BinaryIO, Union
+from warnings import warn
 
 from elevenlabslib.ElevenLabsVoice import ElevenLabsClonedVoice
 from elevenlabslib.ElevenLabsVoice import ElevenLabsDesignedVoice
 
 
 if TYPE_CHECKING:
     from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
@@ -203,52 +204,125 @@
         for voiceData in voicesData["voices"]:
             if voiceData["name"] == voiceName:
                 matchingVoices.append(ElevenLabsVoice.voiceFactory(voiceData, linkedUser=self))
 
         return matchingVoices
 
     def get_history_items(self) -> list[ElevenLabsHistoryItem]:
+        warn("This function is deprecated. Please use get_history_items_paginated() instead, which uses pagination.", DeprecationWarning)
+        return self.get_history_items_paginated(maxNumberOfItems=-1)
+
+
+    def get_history_items_paginated(self, maxNumberOfItems:int=100, startAfterHistoryItem:str|ElevenLabsHistoryItem=None) -> list[ElevenLabsHistoryItem]:
         """
+        This function returns numberOfItems history items, starting from the newest (or the one specified with startAfterHistoryItem) and returning older ones.
+
+        Args:
+            maxNumberOfItems (int): The maximum number of history items to get. A value of 0 or less means all of them.
+            startAfterHistoryItem (str|ElevenLabsHistoryItem): The history item (or its ID) from which to start returning items.
         Returns:
-            list[ElevenLabsHistoryItem]: A list containing all of the user's history items.
+            list[ElevenLabsHistoryItem]: A list containing the requested history items.
         """
+
+        from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
+        params = {}
+
+        if startAfterHistoryItem is not None:
+            if isinstance(startAfterHistoryItem, ElevenLabsHistoryItem):
+                startAfterHistoryItem = startAfterHistoryItem.historyID
+            params["start_after_history_item_id"] = startAfterHistoryItem
+
         outputList = list()
-        response = _api_get("/history", headers=self._headers)
+        singleRequestLimit = 1000
+
+        downloadAll = maxNumberOfItems <= 0
+
+        #While it's over the limit OR the user wants to download all items.
+        while maxNumberOfItems > singleRequestLimit or downloadAll:
+            maxNumberOfItems -= singleRequestLimit
+            #Let's download limit amount of items and append them to the list
+            params["page_size"] = singleRequestLimit
+            response = _api_get("/history", headers=self._headers, params=params)
+            historyData = response.json()
+            for value in historyData["history"]:
+                outputList.append(ElevenLabsHistoryItem(value, self))
+            #We got back at most singleRequestLimit items.
+            params["start_after_history_item_id"] = historyData["last_history_item_id"]
+
+            #In case we're done early.
+            if not historyData["has_more"]:
+                return outputList
+
+        params["page_size"] = maxNumberOfItems
+        response = _api_get("/history", headers=self._headers, params=params)
+
         historyData = response.json()
-        from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
+
         for value in historyData["history"]:
             outputList.append(ElevenLabsHistoryItem(value, self))
         return outputList
 
+
     def get_history_item(self, historyItemID) -> ElevenLabsHistoryItem:
         """
         Args:
             historyItemID: The HistoryItem ID.
 
         Returns:
             ElevenLabsHistoryItem: The corresponding ElevenLabsHistoryItem
         """
         response = _api_get(f"/history/{historyItemID}", headers=self._headers)
         historyData = response.json()
         from elevenlabslib.ElevenLabsHistoryItem import ElevenLabsHistoryItem
         return ElevenLabsHistoryItem(historyData, self)
 
-    def download_history_items(self, historyItems:list[str|ElevenLabsHistoryItem]) -> dict[str, bytes]:
+    def download_history_items_v2(self, historyItems:list[str|ElevenLabsHistoryItem]) -> dict[ElevenLabsHistoryItem, tuple[bytes, str]]:
         """
-            Download multiple history items and return a dictionary where the key is the history ID
-            and the value is the bytes of the mp3 file.
+        Download multiple history items and return a dictionary where the key is the ElevenLabsHistoryItem and the value is a tuple consisting of the bytes of the audio and its filename.
 
-            Args:
-                historyItems (list[str|ElevenLabsHistoryItem]): List of history items (or their IDs) to download.
+        Args:
+            historyItems (list[str|ElevenLabsHistoryItem]): List of history items (or their IDs) to download.
 
-            Returns:
-                dict[str, bytes]: Dictionary where the key is the history ID and the value is the bytes of the mp3 file.
-            """
+        Returns:
+            dict[ElevenLabsHistoryItem, bytes]: Dictionary where the key is the historyItem and the value is a tuple of the bytes of the mp3 file and its filename.
+        """
 
         historyItemIDs = list()
+        for index, item in enumerate(historyItems):
+            if isinstance(item, str):
+                historyItemIDs.append(item)
+                historyItems[index] = self.get_history_item(item)
+            else:
+                historyItemIDs.append(item.historyID)
+
+        if len(historyItemIDs) == 1:
+            historyItemIDs.append(historyItemIDs[0])
+
+        payload = {"history_item_ids": historyItemIDs}
+        response = _api_json("/history/download", headers=self._headers, jsonData=payload)
+
+        if len(historyItemIDs) == 1:
+            downloadedHistoryItems = {historyItemIDs[0]: response.content}
+        else:
+            downloadedHistoryItems = {}
+            downloadedZip = zipfile.ZipFile(io.BytesIO(response.content))
+            # Extract all files and add them to the dict.
+            for filePath in downloadedZip.namelist():
+                fileName = filePath[filePath.index("/")+1:]
+                historyID = fileName[fileName.rindex("_")+1:fileName.rindex(".")]
+                originalHistoryItem = historyItems[historyItemIDs.index(historyID)]
+                assert originalHistoryItem.historyID == historyID
+                if not originalHistoryItem in downloadedHistoryItems:   #Avoid re-reading duplicates from the zip file.
+                    downloadedHistoryItems[originalHistoryItem] = (downloadedZip.read(filePath), fileName)
+
+        return downloadedHistoryItems
+
+    def download_history_items(self, historyItems:list[str|ElevenLabsHistoryItem]) -> dict[str, bytes]:
+        warn("This function is deprecated, please use download_history_items_v2 instead.", DeprecationWarning)
+        historyItemIDs = list()
         for item in historyItems:
             if isinstance(item, str):
                 historyItemIDs.append(item)
             else:
                 historyItemIDs.append(item.historyID)
 
         payload = {"history_item_ids": historyItemIDs}
@@ -257,17 +331,15 @@
         if len(historyItemIDs) == 1:
             downloadedHistoryItems = {historyItemIDs[0]: response.content}
         else:
             downloadedHistoryItems = {}
             downloadedZip = zipfile.ZipFile(io.BytesIO(response.content))
             #Extract all files and add them to the dict.
             for fileName in downloadedZip.namelist():
-                historyID = fileName[:fileName.rindex(".")]
-                if "/" in historyID:
-                    historyID = historyID[historyID.find("/") + 1:]
+                historyID = fileName[fileName.rindex("_") + 1:fileName.rindex(".")]
                 downloadedHistoryItems[historyID] = downloadedZip.read(fileName)
 
         return downloadedHistoryItems
 
     def design_voice(self, gender:str, accent:str, age:str, accent_strength:float, sampleText:str = "First we thought the PC was a calculator. Then we found out how to turn numbers into letters and we thought it was a typewriter.")\
             -> (str,bytes):
         """
```

### Comparing `elevenlabslib-0.7.3/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.8.0/elevenlabslib/ElevenLabsVoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,16 @@
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
             latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply. See generate_and_stream_audio for more info.
         Returns:
             A tuple consisting of the bytes of the audio file and its historyID.
 
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
-        response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
+        params = {"optimize_streaming_latency":latencyOptimizationLevel}
+        response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload, params=params)
 
         return response.content, response.headers["history-item-id"]
     def generate_audio_bytes(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None, model_id:str="eleven_monolingual_v1") -> bytes:
         warn("This function is deprecated. Please use generate_audio() instead, which returns both the audio data and the historyID.",DeprecationWarning)
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         response = _api_json("/text-to-speech/" + self._voiceID + "/stream", self._linkedUser.headers, jsonData=payload)
```

### Comparing `elevenlabslib-0.7.3/elevenlabslib/__init__.py` & `elevenlabslib-0.8.0/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.7.3/elevenlabslib/helpers.py` & `elevenlabslib-0.8.0/elevenlabslib/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,45 +23,51 @@
     try:
         response.raise_for_status()
         return response
     except requests.exceptions.RequestException as e:
         _pretty_print_POST(response)
         raise e
 
-def _api_get(path, headers, stream=False) -> requests.Response:
+def _api_get(path, headers, stream=False, params=None) -> requests.Response:
     args = {
         "path":path,
         "headers":headers,
         "stream":stream
     }
+    if params is not None:
+        args["params"] = params
     return _api_call_v2(requests.get, args)
 def _api_del(path, headers) -> requests.Response:
     args = {
         "path": path,
         "headers": headers
     }
     return _api_call_v2(requests.delete, args)
-def _api_json(path, headers, jsonData, stream=False) -> requests.Response:
+def _api_json(path, headers, jsonData, stream=False, params=None) -> requests.Response:
     args = {
         "path":path,
         "headers":headers,
         "json":jsonData,
         "stream":stream
     }
+    if params is not None:
+        args["params"] = params
     return _api_call_v2(requests.post, args)
 
-def _api_multipart(path, headers, data, filesData=None, stream=False):
+def _api_multipart(path, headers, data, filesData=None, stream=False, params=None):
     args = {
         "path":path,
         "headers":headers,
         "stream":stream,
         "data":data
     }
     if filesData is not None:
         args["files"] = filesData
+    if params is not None:
+        args["params"] = params
 
     return _api_call_v2(requests.post, args)
 
 def _pretty_print_POST(res:requests.Response):
     req = res.request
     logging.debug(f"RESPONSE DATA: {res.text}")
     logging.debug('REQUEST THAT CAUSED THE ERROR:\n{}\n{}\r\n{}\r\n\r\n{}'.format(
@@ -89,18 +95,20 @@
     Returns:
         None
     """
 
     if portaudioDeviceID is None:
         portaudioDeviceID = sd.default.device[1]
 
-    #Let's make sure the user didn't just forward the tuple from one of the generation functions...
+    #Let's make sure the user didn't just forward a tuple from one of the other functions...
     if isinstance(audioData, tuple):
-        if isinstance(audioData[0], bytes):
-            audioData = audioData[0]
+        for item in audioData:
+            if isinstance(item,bytes):
+                audioData = item
+
 
     playbackWrapper = _SDPlaybackWrapper(audioData, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
     if not playInBackground:
         with playbackWrapper.stream:
             playbackWrapper.endPlaybackEvent.wait()
     else:
@@ -113,17 +121,20 @@
         soundfile is used for the conversion, so it supports any format it does.
 
         Parameters:
             audioData: The audio data.
             saveLocation: The path (or file-like object) where the data will be saved.
             outputFormat: The format in which the audio will be saved
         """
+
+    # Let's make sure the user didn't just forward a tuple from one of the other functions...
     if isinstance(audioData, tuple):
-        if isinstance(audioData[0], bytes):
-            audioData = audioData[0]
+        for item in audioData:
+            if isinstance(item, bytes):
+                audioData = item
 
     tempSoundFile = soundfile.SoundFile(io.BytesIO(audioData))
 
     if isinstance(saveLocation, str):
         with open(saveLocation, "wb") as fp:
             sf.write(fp, tempSoundFile.read(), tempSoundFile.samplerate, format=outputFormat)
     else:
```

### Comparing `elevenlabslib-0.7.3/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.8.0/elevenlabslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.7.3
+Version: 0.8.0
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.7.3/pyproject.toml` & `elevenlabslib-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.7.3"
+version = "0.8.0"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

