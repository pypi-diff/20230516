# Comparing `tmp/iotcore_api-1.0.0.tar.gz` & `tmp/iotcore_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.0.0.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.0.tar", max compression
```

## Comparing `iotcore_api-1.0.0.tar` & `iotcore_api-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 12:19:01.890000 iotcore_api-1.0.0/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 17:36:36.620000 iotcore_api-1.0.0/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    52720 2023-03-15 12:23:00.218000 iotcore_api-1.0.0/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0      781 2023-03-15 13:05:05.947000 iotcore_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5294 2023-03-15 16:20:05.832000 iotcore_api-1.0.0/README.md
--rw-r--r--   0        0        0     6018 1970-01-01 00:00:00.000000 iotcore_api-1.0.0/setup.py
--rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 iotcore_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.0/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.0/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    55577 2023-05-16 09:02:50.068030 iotcore_api-1.1.0/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.0/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      782 2023-05-15 16:04:32.304013 iotcore_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    34114 2023-05-16 10:19:21.723415 iotcore_api-1.1.0/README.md
+-rw-r--r--   0        0        0    33711 1970-01-01 00:00:00.000000 iotcore_api-1.1.0/PKG-INFO
```

### Comparing `iotcore_api-1.0.0/iotcoreapi/exceptions.py` & `iotcore_api-1.1.0/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.0.0/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.0/iotcoreapi/iotcoreapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import requests
 import urllib3
 from pandas import json_normalize
 from iotcoreapi.exceptions import IotCoreAPIException
 import warnings
 import re
 
+from iotcoreapi.nan_treatment import nan_treatment
+
 
 class IoTCoreAPI:
     @staticmethod
     def _warnings_and_json_wrapper(func):
         """Decorator including InsecureRequestWarning and then JSON() format"""
 
         def f(*args, **kwargs):
@@ -54,30 +56,33 @@
             else:
                 response = fnc(NX, df_nexus)
             return response
 
         return wrapper
 
     def _convert_response(self, response: dict | list[dict], output_format: str,
-                          time_format: str = None) -> pd.DataFrame | dict | list[dict]:
+                          time_format: str = None, nan_method: str = None) -> pd.DataFrame | dict | list[dict]:
         """
         Auxiliary function to transform response in json format to dataframe if indicated in output_format arg.
         Args:
             response: json
             output_format: 'dataframe' or 'json'
             time_format: 'datetime' or 'unix'
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response: json or dataframe
         """
         if output_format == 'dataframe':
             if response:
                 response = self._json_normalize_check(response)
                 if time_format == 'datetime':
                     response['timeStamp'] = pd.to_datetime(response.timeStamp, unit='s', utc=True)
+                if nan_method is not None:
+                    response = nan_treatment(response, nan_method)
             else:
                 response = pd.DataFrame(columns=['timeStamp', 'uid', 'name', 'value'])
         return response
 
     def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "", version: str | int = "3.0",
                  logger: logging.Logger = None):
         """
@@ -121,26 +126,26 @@
             elif severity == 'warning':
                 self.logger.warning(message)
             else:
                 raise ValueError('Severity not supported')
         else:
             print(message)
 
-    def _json_normalize_check(self, response) -> pd.DataFrame:
+    def _json_normalize_check(self, response: dict | list[dict]) -> pd.DataFrame:
         """
         Intenta convertir a DataFrame la respuesta en json de la API. Si no es posible, es que ha habido un fallo (la respuesta no sigue el formato establecido)
 
         Args:
             response: json con valor de la llamada a NexusAPI
         """
         try:
             return json_normalize(response)
         except Exception as e:
-            self._log_print(f'Error de comunicación en NexusAPI. Motivo: {e}')
-            raise IotCoreAPIException(response)
+            self._log_print(f'IoTCoreAPI communication error. Reason: {e}')
+            raise Exception(f'IoTCoreAPI communication error. Reason: {e}')
 
     @_warnings_and_json_wrapper
     def _getResponse(self, url, params=None):
         """GET method using Request"""
         return requests.get(url, verify=False, params=params, headers=self.header)
 
     @_warnings_and_json_wrapper
@@ -315,180 +320,201 @@
         url_completa = self.url_NX + "/api/Alarms/Groups"
         response = self._getResponse(url_completa)
         return self._convert_response(response, output_format)
 
     # -------- READING OPERATIONS --------
 
     def read_tags_realtime(self, tags_uids: list[str], output_format: str = 'dataframe',
-                           time_format='datetime') -> pd.DataFrame | list[dict]:
+                           time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """Reads real time value of the tags provided in the array tags_uids
 
         Args:
             tags_uids : list with uids of the tags
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         if time_format not in self._time_formats:
             raise ValueError(f'time_format must be in {self._time_formats}')
         body = json.dumps(tags_uids)
         url = self.url_NX + "/api/Tags/realtime"
         response = self._postResponse(url, body)
-        response = self._convert_response(response, output_format, time_format)
+        response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_realtime(self, uid: str, uids_tags: list[str] = None,
                               output_format: str = 'dataframe',
-                              time_format='datetime') -> pd.DataFrame | list[dict]:
+                              time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """Returns real time value for the uids variables provided in a given tagview
 
         Args:
             uid : uid of the tagview
             uids_tags : list of uids
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         if time_format not in self._time_formats:
             raise ValueError(f'time_format must be in {self._time_formats}')
         if uids_tags is None:
             uids_tags = []
         body = json.dumps(uids_tags)
         url = self.url_NX + "/api/Documents/tagviews/" + uid + "/realtime"
         response = self._postResponse(url, body)
-        response = self._convert_response(response, output_format, time_format)
+        response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_historic(self, uids: list[str], start_ts: int | float, end_ts: int | float,
                            data_source: str | int = 'RAW', resolution: str | int = 'RES_1_HOUR',
                            agg_operation: str | int = "LAST_VALUE", output_format: str = 'dataframe',
-                           time_format='datetime') -> pd.DataFrame | list[dict]:
+                           time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """Obtain historic data of the specified tags
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
-            start_ts: start time in unix time
-            end_ts: end time in unix time
+            start_ts: start time in unix time or datetime
+            end_ts: end time in unix time or datetime
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             agg_operation: MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         if time_format not in self._time_formats:
             raise ValueError(f'time_format must be in {self._time_formats}')
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
         if len(uids) > 100:
             raise AttributeError('Too many tags. Please set the number of tags less or equal than 100')
+        # Convert datetime to TS if needed:
+        if isinstance(start_ts, datetime.datetime):
+            start_ts = start_ts.timestamp()
+        if isinstance(end_ts, datetime.datetime):
+            end_ts = end_ts.timestamp()
         body = json.dumps(
             {"uids": uids, "startTs": start_ts, "endTs": end_ts, "dataSource": data_source, "resolution": resolution,
              "aggOperation": agg_operation})
         url = self.url_NX + "/api/Tags/historic"
         response = self._postResponse(url, body)
-        response = self._convert_response(response, output_format, time_format)
+        response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_rawhistoric(self, uids, start_ts, end_ts, output_format: str = 'dataframe',
-                              time_format='datetime') -> pd.DataFrame | list[dict]:
+                              time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """To obtain raw data with no aggregation or normalization applied
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
-            start_ts: start time in unix time
-            end_ts: end time in unix time
+            start_ts: start time in unix time or datetime
+            end_ts: end time in unix time or datetime
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         if time_format not in self._time_formats:
             raise ValueError(f'time_format must be in {self._time_formats}')
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
+        # Convert datetime to TS if needed:
+        if isinstance(start_ts, datetime.datetime):
+            start_ts = start_ts.timestamp()
+        if isinstance(end_ts, datetime.datetime):
+            end_ts = end_ts.timestamp()
         body = json.dumps({"uids": uids, "startTs": start_ts, "endTs": end_ts})
         url = self.url_NX + "/api/Tags/rawhistoric"
         response = self._postResponse(url, body)
-        response = self._convert_response(response, output_format, time_format)
+        response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_transient(self, uids: list[str], start_ts: int | float, end_ts: int | float,
                             data_source: str | int = None,
                             resolution: str | int = 'RES_1_SEC',
                             output_format: str = 'dataframe',
-                            time_format='datetime') -> pd.DataFrame | list[dict]:
+                            time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """
         This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
         aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
         please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
         for historic.
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained. start_ts:
-            start_ts: time in unix time
-            end_ts: end time in unix time. Timespan must be smaller than 15 mins
+            start_ts: time in unix time or datetime
+            end_ts: end time in unix time or datetime. Timespan must be smaller than 15 mins
             data_source: Can be set to null or empty. Not needed
             resolution: RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         if time_format not in self._time_formats:
             raise ValueError(f'time_format must be in {self._time_formats}')
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
         if len(uids) > 100:
             raise AttributeError('Too many tags. Please set the number of tags less or equal than 100')
+        # Convert datetime to TS if needed:
+        if isinstance(start_ts, datetime.datetime):
+            start_ts = start_ts.timestamp()
+        if isinstance(end_ts, datetime.datetime):
+            end_ts = end_ts.timestamp()
         body = json.dumps(
             {"uids": uids, "startTs": start_ts, "endTs": end_ts, "resolution": resolution})
         url = self.url_NX + "/api/Tags/transient"
         response = self._postResponse(url, body)
-        response = self._convert_response(response, output_format, time_format)
+        response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_historic(self, uid: str, start_ts: datetime.datetime | float | int,
                               end_ts: datetime.datetime | float | int, tags_uids: list[str] = None, data_source='RAW',
                               resolution='RES_1_HOUR', output_format: str = 'dataframe',
-                              time_format='datetime') -> pd.DataFrame | list[dict]:
+                              time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
         Args:
             uid: uid of the tagview
-            start_ts: start time in unix
-            end_ts: end time in unix
+            start_ts: start time in unix or datetime
+            end_ts: end time in unix or datetime
             tags_uids (optional): list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
             """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -502,34 +528,35 @@
         if tags_uids is None:
             tags_uids = []
         body = json.dumps(
             {"uids": tags_uids, "startTs": start_ts, "endTs": end_ts, "dataSource": data_source,
              "resolution": resolution})
         url = self.url_NX + "/api/Documents/tagviews/" + uid + "/historic"
         response = self._postResponse(url, body)
-        response = self._convert_response(response, output_format, time_format)
+        response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_historic_text_filters(self, uid_tagview: str, start_ts: datetime.datetime | float | int,
                                            end_ts: datetime.datetime | float | int,
                                            filter_txt: str | list[str] = None, data_source: str = 'RAW',
                                            resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe',
-                                           time_format: str = 'datetime') -> pd.DataFrame | list[dict]:
+                                           time_format: str = 'datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """
         Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt): text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             filtered_hist (dataframe):
                 columns:
                     name: name of tag
                     value: value of tag
                     timeStamp: timeStamp in datatetime or unix time
@@ -552,35 +579,37 @@
                 tags_uids.extend(uids_loop)
         else:
             if filter_txt:
                 tags_uids = list(tagview_info[tagview_info['name'].str.contains(filter_txt, case=False)].uid)
         # Remove duplicate UIDS
         tags_uids = list(set(tags_uids))
         filtered_hist = self.read_tagview_historic(uid_tagview, start_ts, end_ts, tags_uids, data_source, resolution,
-                                                   output_format, time_format)
+                                                   output_format, time_format, nan_method)
         diccio = dict([(i, j) for i, j in zip(tagview_info.uid, tagview_info.name)])
         if isinstance(filtered_hist, pd.DataFrame):
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
     def read_tagview_realtime_text_filters(self, uid_tagview: str,
                                            filter_txt: str | list[str] = None,
                                            output_format: str = 'dataframe',
-                                           time_format: str = 'datetime') -> pd.DataFrame | list[dict]:
+                                           time_format: str = 'datetime',
+                                           nan_method: str = None) -> pd.DataFrame | list[dict]:
         """
         Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             filtered_hist (dataframe):
                 columns:
                     name: name of tag
                     value: value of tag
                     timeStamp: timeStamp in datatetime or unix time
@@ -597,41 +626,42 @@
                 uids_loop = list(tagview_info[tagview_info['name'].str.contains(filter, case=False)].uid)
                 tags_uids.extend(uids_loop)
         else:
             if filter_txt:
                 tags_uids = list(tagview_info[tagview_info['name'].str.contains(filter_txt, case=False)].uid)
         # Remove duplicate UIDS
         tags_uids = list(set(tags_uids))
-        filtered_hist = self.read_tagview_realtime(uid_tagview, tags_uids, output_format, time_format)
+        filtered_hist = self.read_tagview_realtime(uid_tagview, tags_uids, output_format, time_format, nan_method)
         diccio = dict([(i, j) for i, j in zip(tagview_info.uid, tagview_info.name)])
         if isinstance(filtered_hist, pd.DataFrame):
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
     def read_tags_historic_text_filters(self, uids: list[str], start_ts: datetime.datetime | int | float,
                                         end_ts: datetime.datetime | int | float,
                                         filter_txt: str | list[str] = None, data_source: str | int = 'RAW',
                                         resolution: str | int = 'RES_1_HOUR',
                                         agg_operation: str | int = "LAST_VALUE", output_format: str = 'dataframe',
-                                        time_format: str = 'datetime') -> pd.DataFrame | list[dict]:
+                                        time_format: str = 'datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
         """Obtain historic data of the specified tags by name
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             agg_operation: MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -652,34 +682,36 @@
                 tags_uids.extend(uids_loop)
         else:
             if filter_txt:
                 tags_uids = list(tag_info[tag_info['name'].str.contains(filter_txt, case=False)].uid)
         # Remove duplicate UIDS
         tags_uids = list(set(tags_uids))
         filtered_hist = self.read_tags_historic(tags_uids, start_ts, end_ts, data_source, resolution, agg_operation,
-                                                output_format, time_format)
+                                                output_format, time_format, nan_method)
         diccio = dict([(i, j) for i, j in zip(tag_info.uid, tag_info.name)])
         if isinstance(filtered_hist, pd.DataFrame):
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
     def read_tags_realtime_text_filters(self,
                                         filter_txt: str | list[str] = None,
                                         output_format: str = 'dataframe',
-                                        time_format: str = 'datetime') -> pd.DataFrame | list[dict]:
+                                        time_format: str = 'datetime',
+                                        nan_method: str = None) -> pd.DataFrame | list[dict]:
         """
         Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             dataframe or json:
                 columns:
                     name: name of tag
                     value: value of tag
                     timeStamp: timeStamp in datatetime or unix time
@@ -696,15 +728,15 @@
                 uids_loop = list(tag_info[tag_info['name'].str.contains(filter, case=False)].uid)
                 tags_uids.extend(uids_loop)
         else:
             if filter_txt:
                 tags_uids = list(tag_info[tag_info['name'].str.contains(filter_txt, case=False)].uid)
         # Remove duplicate UIDS
         tags_uids = list(set(tags_uids))
-        filtered_hist = self.read_tags_realtime(tags_uids, output_format, time_format)
+        filtered_hist = self.read_tags_realtime(tags_uids, output_format, time_format, nan_method)
         diccio = dict([(i, j) for i, j in zip(tag_info.uid, tag_info.name)])
         if isinstance(filtered_hist, pd.DataFrame):
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
@@ -773,49 +805,36 @@
         if isinstance(tags, str):
             tags = [tags]
         body = json.dumps(tags)
         self._log_print(f'Tags to be created: {body}')
         url_post = self.url_NX + "/api/Tags/Insert"
         return self._postResponse(url_post, body)
 
-    def write_tag_insert_or_update(self, tagname, nameofattribute1="", valueofattribute1="", nameofattribute2="",
-                                   valueofattribute2="", nameofattribute3="", valueofattribute3="") -> list[dict]:
+    def write_tag_insert_or_update(self, tagname, **attributes) -> list[dict]:
         """This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
         Args:
             tagname: name of the new tag
-            nameofattribute1
-            valueofattribute1
-            nameofattribute2
-            valueofattribute2
-            nameofattribute3
-            valueofattribute3
+            **attributes: dictionary of attributes and their values
 
         Returns:
             response in json format
+
+        Examples:
+            Call the function with a tag name and any number of attributes
+            response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
         """
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
-        body = json.dumps([{"Name": tagname, "Attributes": [
-            {"attributeName": nameofattribute1,
-             "value": valueofattribute1
-             },
-            {"attributeName": nameofattribute2,
-             "value": valueofattribute2
-             },
-            {"attributeName": nameofattribute3,
-             "value": valueofattribute3
-             }
-        ]
-                            }
-                           ])
+        attribute_list = [{"attributeName": name, "value": value} for name, value in attributes.items()]
+        body = json.dumps([{"Name": tagname, "Attributes": attribute_list}])
         url = self.url_NX + "/api/Tags/InsertOrUpdate"
         return self._postResponse(url, body)
 
-    def write_tags_insert_or_update_mult(self, tags_and_attributes: list[dict]):
+    def write_tags_insert_or_update_by_json(self, tags_and_attributes: list[dict]):
         """This method creates the tags with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
         Args:
             tags_and_attributes: json list containing info for each tag:
                 [
                     {
                     "Name": "name of the new tag",
```

### Comparing `iotcore_api-1.0.0/pyproject.toml` & `iotcore_api-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "iotcore-api"
-version = "1.0.0"
+version = "1.1.0"
 authors = ["Nexus Integra"]
 description ="IoT core connection methods and utilities"
 readme = "README.md"
 homepage = "https://nexusintegra.io"
 repository = 'https://github.com/NexusIntegra/iotcoreAPI'
 packages = [
     {include = 'iotcoreapi/*.py'}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pandas = "1.5.3"
-requests = "^2.28.2"
+pandas = "^2.0.1"
+requests = "^2.30.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 pytest = "^7.2.2"
 mkdocs = "^1.4.2"
 mkdocstrings = "^0.20.0"
```

