# Comparing `tmp/google-ads-api-report-fetcher-1.2.1.tar.gz` & `tmp/google-ads-api-report-fetcher-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ads-api-report-fetcher-1.2.1.tar", last modified: Thu Apr  6 10:38:21 2023, max compression
+gzip compressed data, was "google-ads-api-report-fetcher-1.4.0.tar", last modified: Tue May 16 06:26:16 2023, max compression
```

## Comparing `google-ads-api-report-fetcher-1.2.1.tar` & `google-ads-api-report-fetcher-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.803089 google-ads-api-report-fetcher-1.2.1/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-04-06 10:38:21.803089 google-ads-api-report-fetcher-1.2.1/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.2.1/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.799089 google-ads-api-report-fetcher-1.2.1/gaarf/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.2.1/gaarf/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.2.1/gaarf/api_clients.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.2.1/gaarf/base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3525 2023-03-09 07:10:15.000000 google-ads-api-report-fetcher-1.2.1/gaarf/bq_executor.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.799089 google-ads-api-report-fetcher-1.2.1/gaarf/cli/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.2.1/gaarf/cli/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3671 2023-02-20 08:49:55.000000 google-ads-api-report-fetcher-1.2.1/gaarf/cli/bq.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6860 2023-04-06 08:52:28.000000 google-ads-api-report-fetcher-1.2.1/gaarf/cli/gaarf.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3238 2023-01-30 21:09:38.000000 google-ads-api-report-fetcher-1.2.1/gaarf/cli/simulator.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10241 2023-03-09 07:19:16.000000 google-ads-api-report-fetcher-1.2.1/gaarf/cli/utils.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.799089 google-ads-api-report-fetcher-1.2.1/gaarf/io/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.2.1/gaarf/io/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.2.1/gaarf/io/formatter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.2.1/gaarf/io/reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.2.1/gaarf/io/writer.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9666 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.2.1/gaarf/parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.2.1/gaarf/query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10649 2023-03-15 07:18:06.000000 google-ads-api-report-fetcher-1.2.1/gaarf/query_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4944 2023-03-22 21:20:48.000000 google-ads-api-report-fetcher-1.2.1/gaarf/report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.2.1/gaarf/simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1974 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.2.1/gaarf/utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.2.1/gaarf/wip.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.799089 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-04-06 10:38:21.000000 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1033 2023-04-06 10:38:21.000000 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-04-06 10:38:21.000000 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      120 2023-04-06 10:38:21.000000 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      183 2023-04-06 10:38:21.000000 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-04-06 10:38:21.000000 google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-04-06 10:38:21.803089 google-ads-api-report-fetcher-1.2.1/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1577 2023-04-06 10:38:07.000000 google-ads-api-report-fetcher-1.2.1/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.799089 google-ads-api-report-fetcher-1.2.1/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.2.1/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-04-06 10:38:21.799089 google-ads-api-report-fetcher-1.2.1/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1400 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_bq_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10446 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_cli_utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5495 2023-03-22 21:22:55.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3864 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.2.1/tests/unit/test_writer.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.4.0/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.276760 google-ads-api-report-fetcher-1.4.0/gaarf/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.4.0/gaarf/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-04-13 10:50:21.000000 google-ads-api-report-fetcher-1.4.0/gaarf/api_clients.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.4.0/gaarf/base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3744 2023-04-13 14:02:39.000000 google-ads-api-report-fetcher-1.4.0/gaarf/bq_executor.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.276760 google-ads-api-report-fetcher-1.4.0/gaarf/cli/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3671 2023-02-20 08:49:55.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/bq.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7841 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/gaarf.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3238 2023-01-30 21:09:38.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/simulator.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10557 2023-04-07 06:52:45.000000 google-ads-api-report-fetcher-1.4.0/gaarf/cli/utils.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.276760 google-ads-api-report-fetcher-1.4.0/gaarf/io/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/formatter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.4.0/gaarf/io/writer.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9666 2023-05-15 07:22:41.000000 google-ads-api-report-fetcher-1.4.0/gaarf/parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.4.0/gaarf/query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11371 2023-05-04 10:22:26.000000 google-ads-api-report-fetcher-1.4.0/gaarf/query_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5168 2023-05-09 09:54:31.000000 google-ads-api-report-fetcher-1.4.0/gaarf/report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.4.0/gaarf/simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.4.0/gaarf/utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.4.0/gaarf/wip.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1033 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      120 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-05-16 06:26:16.000000 google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1589 2023-05-16 06:17:39.000000 google-ads-api-report-fetcher-1.4.0/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.4.0/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-16 06:26:16.280760 google-ads-api-report-fetcher-1.4.0/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1400 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_bq_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10945 2023-04-07 06:54:54.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_cli_utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5788 2023-05-11 16:09:08.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3864 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.4.0/tests/unit/test_writer.py
```

### Comparing `google-ads-api-report-fetcher-1.2.1/PKG-INFO` & `google-ads-api-report-fetcher-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.2.1
+Version: 1.4.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-ads-api-report-fetcher-1.2.1/README.md` & `google-ads-api-report-fetcher-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/api_clients.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/api_clients.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/base_query.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/bq_executor.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/bq_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,22 @@
             self,
             script_name: str,
             query_text: str,
             params: Optional[Dict[str, Any]] = None) -> Optional[pd.DataFrame]:
         logger.debug("Original query text:\n%s", query_text)
         if params:
             if (templates := params.get("template")):
-                query_text = expand_jinja(query_text, **templates)
-                logger.debug("Query text after jinja expansion:\n%s",
-                             query_text)
+                query_templates = {
+                    name: value
+                    for name, value in templates.items() if name in query_text
+                }
+                if query_templates:
+                    query_text = expand_jinja(query_text, **query_templates)
+                    logger.debug("Query text after jinja expansion:\n%s",
+                                 query_text)
             if (macros := params.get("macro")):
                 query_text = query_text.format(**macros)
                 logger.debug("Query text after macro substitution:\n%s",
                              query_text)
         job = self.client.query(query_text)
         try:
             result = job.result()
```

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/cli/bq.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/cli/bq.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/cli/gaarf.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/cli/gaarf.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Dict
 
+from collections.abc import MutableSequence
 from concurrent import futures
 import argparse
 from pathlib import Path
 import logging
 from rich.logging import RichHandler
 from smart_open import open
 import yaml
@@ -24,15 +25,15 @@
 from gaarf import api_clients, utils, query_executor
 from gaarf.io import writer, reader  # type: ignore
 from .utils import GaarfConfigBuilder, ConfigSaver, initialize_runtime_parameters, gaarf_runner
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument("query", nargs="+")
+    parser.add_argument("query", nargs="*")
     parser.add_argument("-c", "--config", dest="gaarf_config", default=None)
     parser.add_argument("--account", dest="customer_id", default=None)
     parser.add_argument("--output", dest="save", default="console")
     parser.add_argument("--input", dest="input", default="file")
     parser.add_argument("--ads-config",
                         dest="config",
                         default=str(Path.home() / "google-ads.yaml"))
@@ -59,29 +60,45 @@
     parser.add_argument("--no-parallel-queries",
                         dest="parallel_queries",
                         action="store_false")
     parser.add_argument("--optimize-performance",
                         dest="optimize_performance",
                         default="NONE")
     parser.add_argument("--dry-run", dest="dry_run", action="store_true")
+    parser.add_argument("--disable-account-expansion",
+                        dest="disable_account_expansion",
+                        action="store_true")
+    parser.add_argument("-v", "--version", dest="version", action="store_true")
     parser.set_defaults(save_config=False)
     parser.set_defaults(parallel_queries=True)
     parser.set_defaults(dry_run=False)
+    parser.set_defaults(disable_account_expansion=False)
     args = parser.parse_known_args()
     main_args = args[0]
 
+    if main_args.version:
+        import pkg_resources
+        version = pkg_resources.require(
+            "google-ads-api-report-fetcher")[0].version
+        print(f"gaarf version {version}")
+        exit()
+
     logging.basicConfig(format="%(message)s",
                         level=main_args.loglevel.upper(),
                         datefmt="%Y-%m-%d %H:%M:%S",
                         handlers=[RichHandler(rich_tracebacks=True)])
     logging.getLogger("google.ads.googleads.client").setLevel(logging.WARNING)
     logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
     logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
     logger = logging.getLogger(__name__)
 
+    if not main_args.query:
+        logger.error("Please provide one or more queries to run")
+        exit()
+
     with open(main_args.config, "r", encoding="utf-8") as f:
         google_ads_config_dict = yaml.safe_load(f)
 
     config = GaarfConfigBuilder(args).build()
     if account := main_args.customer_id:
         config.account = account
     if not config.account:
@@ -94,15 +111,16 @@
     logger.debug("config: %s", config)
 
     if main_args.save_config and not main_args.gaarf_config:
         ConfigSaver(main_args.save_config_dest).save(config)
     if main_args.dry_run:
         exit()
 
-    config = initialize_runtime_parameters(config)
+    if config.params:
+        config = initialize_runtime_parameters(config)
     logger.debug("initialized config: %s", config)
 
     ads_client = api_clients.GoogleAdsApiClient(
         config_dict=google_ads_config_dict, version=f"v{config.api_version}")
     reader_factory = reader.ReaderFactory()
     reader_client = reader_factory.create_reader(main_args.input)
 
@@ -110,16 +128,23 @@
         customer_ids_query = config.customer_ids_query
     elif config.customer_ids_query_file:
         file_reader = reader_factory.create_reader("file")
         customer_ids_query = file_reader.read(config.customer_ids_query_file)
     else:
         customer_ids_query = None
 
-    customer_ids = utils.get_customer_ids(ads_client, config.account,
-                                          customer_ids_query)
+    if main_args.disable_account_expansion:
+        logger.info(
+            "Skipping account expansion because of disable_account_expansion flag"
+        )
+        customer_ids = config.account if isinstance(
+            config.account, MutableSequence) else [config.account]
+    else:
+        customer_ids = utils.get_customer_ids(ads_client, config.account,
+                                              customer_ids_query)
     if customer_ids:
         writer_client = writer.WriterFactory().create_writer(
             config.output, **config.writer_params)
         if config.output == "bq":
             _ = writer_client.create_or_get_dataset()
         ads_query_executor = query_executor.AdsQueryExecutor(ads_client)
```

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/cli/simulator.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/cli/utils.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
-import dataclasses
+from collections.abc import MutableSequence
+from dataclasses import dataclass, field, asdict
 import os
 import datetime
 from smart_open import open
 from dateutil.relativedelta import relativedelta
 import yaml
 from google.ads.googleads.errors import GoogleAdsException  # type: ignore
 import traceback
 
 from gaarf.io.writer import ZeroRowException
 
 
-@dataclasses.dataclass
+@dataclass
 class GaarfConfig:
     output: str
     api_version: str
     account: str
-    params: Dict[str, Any]
-    writer_params: Dict[str, Any]
-    customer_ids_query: str
-    customer_ids_query_file: str
+    params: Dict[str, Any] = field(default_factory=dict)
+    writer_params: Dict[str, Any] = field(default_factory=dict)
+    customer_ids_query: Optional[str] = None
+    customer_ids_query_file: Optional[str] = None
 
 
-@dataclasses.dataclass
+@dataclass
 class GaarfBqConfig:
     project: str
     dataset_location: Optional[str]
-    params: Dict[str, Any]
+    params: Dict[str, Any] = field(default_factory=dict)
 
 
 class BaseConfigBuilder:
 
     def __init__(self, args):
         self.args = args
         if (gaarf_config_path := self.args[0].gaarf_config):
@@ -218,17 +219,19 @@
                       f,
                       default_flow_style=False,
                       sort_keys=False,
                       encoding="utf-8")
 
     def prepare_config(self, config: Dict[Any, Any],
                        gaarf_config: Union[GaarfConfig, GaarfBqConfig]):
-        gaarf = dataclasses.asdict(gaarf_config)
+        gaarf = asdict(gaarf_config)
         if isinstance(gaarf_config, GaarfConfig):
             gaarf[gaarf_config.output] = gaarf_config.writer_params
+            if not isinstance(gaarf_config.account, MutableSequence):
+                gaarf["account"] = gaarf_config.account.split(",")
             del gaarf["writer_params"]
             if gaarf_config.writer_params:
                 del gaarf["params"][gaarf_config.output]
             gaarf = _remove_empty_values(gaarf)
             config.update({"gaarf": gaarf})
         if isinstance(gaarf_config, GaarfBqConfig):
             gaarf = _remove_empty_values(gaarf)
@@ -248,15 +251,15 @@
     """Remove all empty elements: strings, dictionaries from a dictionary."""
     if isinstance(dict_object, dict):
         return {
             key: value
             for key, value in ((key, _remove_empty_values(value))
                                for key, value in dict_object.items()) if value
         }
-    if isinstance(dict_object, (int, str)):
+    if isinstance(dict_object, (int, str, MutableSequence)):
         return dict_object
 
 
 def gaarf_runner(query: str, callback: Callable, logger) -> None:
     try:
         logger.debug("starting query %s", query)
         callback()
```

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/io/formatter.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/io/formatter.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/io/reader.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/io/reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/io/writer.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/io/writer.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/parsers.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/query_editor.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/query_executor.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/query_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # limitations under the License.
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 from concurrent import futures
 from enum import Enum, auto
 import itertools
 from google.ads.googleads.errors import GoogleAdsException  # type: ignore
 import logging
+from google.api_core import exceptions
+from tenacity import Retrying, RetryError, retry_if_exception_type, stop_after_attempt, wait_exponential
 
 from . import parsers
 from . import api_clients
 from .query_editor import QuerySpecification, QueryElements
 from .report import GaarfReport
 from .io import writer, reader  # type: ignore
 
@@ -39,15 +41,15 @@
 
     Attributes:
         api_client: a client used for connecting to Ads API.
         customer_ids: account_id(s) from which data will be fetches.
     """
 
     def __init__(self, api_client: api_clients.BaseClient,
-                 customer_ids: Union[List[str], str]) -> None:
+                 customer_ids: Union[Sequence[str], str]) -> None:
 
         self.api_client = api_client
         self.customer_ids = [
             customer_ids
         ] if not isinstance(customer_ids, list) else customer_ids
 
     def fetch(self,
@@ -120,17 +122,27 @@
 
         Returns:
             Parsed rows for the whole response.
         """
         total_results: List[List[Tuple[Any]]] = []
         logger.debug("Getting response for query %s for customer_id %s",
                      query_specification.query_title, customer_id)
-        response = self.api_client.get_response(
-            entity_id=str(customer_id),
-            query_text=query_specification.query_text)
+        try:
+            for attempt in Retrying(retry=retry_if_exception_type(
+                    exceptions.InternalServerError),
+                                    stop=stop_after_attempt(3),
+                                    wait=wait_exponential()):
+                with attempt:
+                    response = self.api_client.get_response(
+                        entity_id=str(customer_id),
+                        query_text=query_specification.query_text)
+        except RetryError as retry_failure:
+            logger.error("Cannot fetch data from API for query '%s' %d times",
+                         query_specification.query_title,
+                         retry_failure.last_attempt.attempt_number)
         if optimize_strategy in (OptimizeStrategy.BATCH,
                                  OptimizeStrategy.BATCH_PROTOBUF):
             logger.warning("Running gaarf in an optimized mode")
             logger.warning("Optimize strategy is %s", optimize_strategy.name)
             if optimize_strategy == OptimizeStrategy.BATCH_PROTOBUF:
                 rows = [row._pb for batch in response for row in batch.results]
             else:
```

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/report.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/report.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,25 +79,25 @@
             if key in self.column_names:
                 index = self.column_names.index(key)
                 results = [[row[index]] for row in self.results]
                 return cls(results, [key])
         if self.multi_column_report:
             if isinstance(key, slice):
                 return cls(self.results[key], self.column_names)
-            return cls([self.results[key]], self.column_names)
+            return GaarfRow(self.results[key], self.column_names)
         if isinstance(key, slice):
             return [element[0] for element in self.results[key]]
         index = operator.index(key)
         return self.results[key]
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
         if self.column_names != other.column_names:
-            return false
+            return False
         return self.results == other.results
 
     def __add__(self, other):
         if not isinstance(other, self.__class__):
             raise TypeError("Add operation is supported only for GaarfReport")
         if self.column_names != other.column_names:
             raise ValueError("column_names should be the same in GaarfReport")
@@ -127,10 +127,17 @@
         if isinstance(element, str):
             return self.__getattr__(element)
         raise IndexError(f"cannot find {element} element!")
 
     def get(self, item: str) -> Any:
         return self.__getattr__(item)
 
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        if self.column_names != other.column_names:
+            return False
+        return self.data == other.data
+
     def __repr__(self):
         dict_data = {x[1]: x[0] for x in zip(self.data, self.column_names)}
         return f"GaarfRow(\n{dict_data}\n)"
```

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/simulation.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/gaarf/utils.py` & `google-ads-api-report-fetcher-1.4.0/gaarf/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.import proto
 
-from typing import Sequence
+from typing import Sequence, Union
+from collections.abc import MutableSequence
 
 from .api_clients import GoogleAdsApiClient
 from .query_editor import QuerySpecification
 from .query_executor import AdsReportFetcher
+from .report import GaarfRow
 
 
 def get_customer_ids(ads_client: GoogleAdsApiClient,
-                     customer_id: str,
+                     customer_id: Union[str, MutableSequence[str]],
                      customer_ids_query: str = None) -> Sequence[str]:
     """Gets list of customer_ids from an MCC account.
 
     Args:
         ads_client: GoogleAdsApiClient used for connection.
         customer_id: MCC account_id.
         custom_query: GAQL query used to reduce the number of customer_ids.
@@ -33,18 +35,24 @@
     """
 
     query = """
     SELECT customer_client.id FROM customer_client
     WHERE customer_client.manager = FALSE AND customer_client.status = "ENABLED"
     """
     query_specification = QuerySpecification(query).generate()
+    if not isinstance(customer_id, MutableSequence):
+        customer_id = customer_id.split(",")
     report_fetcher = AdsReportFetcher(ads_client, customer_id)
     customer_ids = report_fetcher.fetch(query_specification).to_list()
     if customer_ids_query:
         report_fetcher = AdsReportFetcher(ads_client, customer_ids)
         query_specification = QuerySpecification(customer_ids_query).generate()
-        customer_ids = report_fetcher.fetch(query_specification).to_list()
-    customer_ids = list(set([
-        customer_id for customer_id in customer_ids if customer_id != 0
-    ]))
+        customer_ids = report_fetcher.fetch(query_specification)
+        customer_ids = [
+            row[0] if isinstance(row, GaarfRow) else row
+            for row in customer_ids
+        ]
+
+    customer_ids = list(
+        set([customer_id for customer_id in customer_ids if customer_id != 0]))
 
     return customer_ids
```

### Comparing `google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/PKG-INFO` & `google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.2.1
+Version: 1.4.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-ads-api-report-fetcher-1.2.1/google_ads_api_report_fetcher.egg-info/SOURCES.txt` & `google-ads-api-report-fetcher-1.4.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/setup.py` & `google-ads-api-report-fetcher-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "sqlalchemy": ["sqlalchemy"],
     "simulator": ["Faker"]
 }
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     name="google-ads-api-report-fetcher",
-    version="1.2.1",
+    version="1.4.0",
     description=
     "Library for fetching reports from Google Ads API and saving them locally / BigQuery.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/google/ads-api-reports-fetcher",
     author="Google Inc. (gTech gPS CSE team)",
     author_email="no-reply@google.com",
@@ -28,17 +28,17 @@
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License"
     ],
     packages=find_packages(),
     install_requires=[
-        "google-ads>=16.0.0", "google-cloud-bigquery", "pandas>=1.3.4",
+        "google-ads>=21.0.0", "google-cloud-bigquery", "pandas>=1.3.4",
         "pyarrow>=6.0.1", "smart_open[all]", "jinja2", "python-dateutil",
-        "rich"
+        "rich", "tenacity"
     ],
     extras_require=EXTRAS_REQUIRE,
     setup_requires=["pytest-runner"],
     tests_requires=["pytest"],
     entry_points={
         "console_scripts": [
             "gaarf=gaarf.cli.gaarf:main",
```

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_base_query.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_bq_executor.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_bq_executor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_cli_utils.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,27 +116,43 @@
 
 
 @pytest.fixture
 def config_saver(config_args):
     return utils.ConfigSaver("/tmp/config.yaml")
 
 
+def test_gaarf_config_saver_gaarf_transforms_comma_separated_account_into_list(
+        config_saver):
+    gaarf_config = utils.GaarfConfig(output="console",
+                                     api_version="10",
+                                     account="1,2,3")
+
+    config = config_saver.prepare_config({}, gaarf_config)
+    assert config == {
+        "gaarf": {
+            "account": ["1", "2", "3"],
+            "output": "console",
+            "api_version": "10",
+        }
+    }
+
+
 def test_gaarf_config_saver_gaarf_dont_save_empty_values(config_saver):
     gaarf_config = utils.GaarfConfig(output="console",
                                      api_version="10",
                                      account="1",
                                      params={},
                                      writer_params={},
                                      customer_ids_query="",
                                      customer_ids_query_file="")
 
     config = config_saver.prepare_config({}, gaarf_config)
     assert config == {
         "gaarf": {
-            "account": "1",
+            "account": ["1"],
             "output": "console",
             "api_version": "10",
         }
     }
 
 
 def test_gaarf_config_saver_gaarf_dont_save_inner_empty_values(config_saver):
@@ -149,15 +165,15 @@
                                      writer_params={},
                                      customer_ids_query="",
                                      customer_ids_query_file="")
 
     config = config_saver.prepare_config({}, gaarf_config)
     assert config == {
         "gaarf": {
-            "account": "1",
+            "account": ["1"],
             "output": "console",
             "api_version": "10",
             "params": {
                 "macro": {
                     "start_date": ":YYYYMMDD"
                 }
             }
@@ -173,15 +189,15 @@
                                      writer_params={},
                                      customer_ids_query="SELECT",
                                      customer_ids_query_file="path/to/file.sql")
 
     config = config_saver.prepare_config({}, gaarf_config)
     assert config == {
         "gaarf": {
-            "account": "1",
+            "account": ["1"],
             "output": "console",
             "api_version": "10",
             "customer_ids_query": "SELECT",
             "customer_ids_query_file": "path/to/file.sql"
         }
     }
```

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_parsers.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_query_editor.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_reader.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_report.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,19 +126,26 @@
 def test_slicing_multi_column_gaarf_report_returns_gaarf_report(
         multi_column_report):
     new_report = multi_column_report[0:2]
     assert new_report == GaarfReport(
         results=[[1, 2], [2, 3]], column_names=["campaign_id", "ad_group_id"])
 
 
-def test_indexing_multi_column_gaarf_report_by_index_returns_gaarf_report(
+def test_indexing_multi_column_gaarf_report_by_single_index_returns_gaarf_row(
         multi_column_report):
     new_report = multi_column_report[0]
+    assert new_report == GaarfRow(data=[1, 2],
+                                  column_names=["campaign_id", "ad_group_id"])
+
+
+def test_indexing_multi_column_gaarf_report_by_multi_index_returns_gaarf_report(
+        multi_column_report):
+    new_report = multi_column_report[0:2]
     assert new_report == GaarfReport(
-        results=[[1, 2]], column_names=["campaign_id", "ad_group_id"])
+        results=[[1, 2], [2, 3]], column_names=["campaign_id", "ad_group_id"])
 
 
 def test_indexing_multi_column_gaarf_report_by_one_column_returns_gaarf_report(
         multi_column_report):
     new_report = multi_column_report["campaign_id"]
     assert new_report == GaarfReport(results=[[1], [2], [3]],
                                      column_names=["campaign_id"])
```

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_simulation.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.2.1/tests/unit/test_writer.py` & `google-ads-api-report-fetcher-1.4.0/tests/unit/test_writer.py`

 * *Files identical despite different names*

