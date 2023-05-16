# Comparing `tmp/monkey.crawler-2.0.0.dev3.tar.gz` & `tmp/monkey.crawler-2.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkey.crawler-2.0.0.dev3.tar", last modified: Sat Jan 28 15:56:13 2023, max compression
+gzip compressed data, was "monkey.crawler-2.0.0.dev4.tar", last modified: Sat Jan 28 16:13:22 2023, max compression
```

## Comparing `monkey.crawler-2.0.0.dev3.tar` & `monkey.crawler-2.0.0.dev4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.688335 monkey.crawler-2.0.0.dev3/
--rw-rw-rw-   0        0        0    11556 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/LICENSE.txt
--rw-rw-rw-   0        0        0       60 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/MANIFEST.in
--rw-rw-rw-   0        0        0      855 2023-01-28 15:56:13.687125 monkey.crawler-2.0.0.dev3/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev3/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.574571 monkey.crawler-2.0.0.dev3/monkey/
--rw-rw-rw-   0        0        0       84 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.620737 monkey.crawler-2.0.0.dev3/monkey/crawler/
--rw-rw-rw-   0        0        0       84 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/__init__.py
--rw-rw-rw-   0        0        0     1177 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/crawler.py
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.634618 monkey.crawler-2.0.0.dev3/monkey/crawler/crawlers/
--rw-rw-rw-   0        0        0       84 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/crawlers/__init__.py
--rw-rw-rw-   0        0        0     1191 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/crawlers/csv.py
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.676224 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/
--rw-rw-rw-   0        0        0       82 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/calc.py
--rw-rw-rw-   0        0        0     2025 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/composite.py
--rw-rw-rw-   0        0        0    12818 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/filter.py
--rw-rw-rw-   0        0        0     1962 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/format.py
--rw-rw-rw-   0        0        0     1933 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/project.py
--rw-rw-rw-   0        0        0     8386 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/transform.py
--rw-rw-rw-   0        0        0     1835 2023-01-28 15:54:22.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/op_codes.py
--rw-rw-rw-   0        0        0     6299 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/pipeline.py
--rw-rw-rw-   0        0        0     2885 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/processor.py
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.684369 monkey.crawler-2.0.0.dev3/monkey/crawler/processors/
--rw-rw-rw-   0        0        0       82 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/processors/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/monkey/crawler/processors/dump.py
-drwxrwxrwx   0        0        0        0 2023-01-28 15:56:13.600024 monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/
--rw-rw-rw-   0        0        0      855 2023-01-28 15:56:13.000000 monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-01-28 15:56:13.000000 monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-28 15:56:13.000000 monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-28 15:56:13.000000 monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-28 15:56:13.688335 monkey.crawler-2.0.0.dev3/setup.cfg
--rw-rw-rw-   0        0        0     1302 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.316385 monkey.crawler-2.0.0.dev4/
+-rw-rw-rw-   0        0        0    11556 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/LICENSE.txt
+-rw-rw-rw-   0        0        0       60 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/MANIFEST.in
+-rw-rw-rw-   0        0        0      855 2023-01-28 16:13:22.315384 monkey.crawler-2.0.0.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev4/README.rst
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.217497 monkey.crawler-2.0.0.dev4/monkey/
+-rw-rw-rw-   0        0        0       84 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.264036 monkey.crawler-2.0.0.dev4/monkey/crawler/
+-rw-rw-rw-   0        0        0       84 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/__init__.py
+-rw-rw-rw-   0        0        0     1177 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/crawler.py
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.271008 monkey.crawler-2.0.0.dev4/monkey/crawler/crawlers/
+-rw-rw-rw-   0        0        0       84 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/crawlers/__init__.py
+-rw-rw-rw-   0        0        0     1191 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/crawlers/csv.py
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.301876 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/
+-rw-rw-rw-   0        0        0       82 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/calc.py
+-rw-rw-rw-   0        0        0     2025 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/composite.py
+-rw-rw-rw-   0        0        0    12818 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/filter.py
+-rw-rw-rw-   0        0        0     1962 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/format.py
+-rw-rw-rw-   0        0        0     1933 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/project.py
+-rw-rw-rw-   0        0        0     8386 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/transform.py
+-rw-rw-rw-   0        0        0     1835 2023-01-28 15:54:22.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/op_codes.py
+-rw-rw-rw-   0        0        0     6275 2023-01-28 16:09:51.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/pipeline.py
+-rw-rw-rw-   0        0        0     2885 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/processor.py
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.313390 monkey.crawler-2.0.0.dev4/monkey/crawler/processors/
+-rw-rw-rw-   0        0        0       82 2023-01-28 14:03:37.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/processors/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/monkey/crawler/processors/dump.py
+drwxrwxrwx   0        0        0        0 2023-01-28 16:13:22.243316 monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/
+-rw-rw-rw-   0        0        0      855 2023-01-28 16:13:22.000000 monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2023-01-28 16:13:22.000000 monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-28 16:13:22.000000 monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-01-28 16:13:22.000000 monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-01-28 10:07:36.000000 monkey.crawler-2.0.0.dev4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-01-28 16:13:22.317358 monkey.crawler-2.0.0.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2023-01-28 16:12:22.000000 monkey.crawler-2.0.0.dev4/setup.py
```

### Comparing `monkey.crawler-2.0.0.dev3/LICENSE.txt` & `monkey.crawler-2.0.0.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/PKG-INFO` & `monkey.crawler-2.0.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.crawler
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: Small framework to crawl misc data sources and process records.
 Home-page: https://bitbucket.org/monkeytechnologies/monkey-crawler
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/crawler.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/crawlers/csv.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/crawlers/csv.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/calc.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/calc.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/composite.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/composite.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/filter.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/filter.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/format.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/format.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/project.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/project.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/handlers/transform.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/handlers/transform.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/op_codes.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/op_codes.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/pipeline.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     op_code = OpCode.ERROR
                 except ProcessingError as e:
                     self.logger.error(f'{self.name} - PROCESSING ERROR - {e.message}')
                     op_code = OpCode.ERROR
                 except Exception as e:
                     self.logger.error(f'{self.name} - UNEXPECTED ERROR - {e}')
                     op_code = OpCode.ERROR
-                self.logger.log(op_code.get_default_logging_level(), f'{self.name} - {op_code.get_name()} - {record}')
+                self.logger.log(op_code.default_logging_level, f'{self.name} - {op_code.name} - {record}')
 
                 counter.inc(op_code)
                 self.reporter.plot(op_code)
                 self.activity_logger.report(record, op_code)
                 if op_code == OpCode.SKIP or op_code == OpCode.RETRY:
                     self.retry_accumulator.add(record)
 
@@ -124,15 +124,15 @@
 
     def line_head(self, counter: OpCounter):
         if counter.total() % self.max_col == 0:
             self._print(f'\n{self.plot_count:<{self.head_len}}: ')
             self.plot_count += self.max_col
 
     def plot(self, op_code: OpCode):
-        self._print(op_code.get_plot_symbol())
+        self._print(op_code.plot_symbol)
 
     def reset(self):
         self.plot_count = 0
 
 
 class ActivityLogger:
 
@@ -145,8 +145,8 @@
     def report(self, record, op_code: OpCode, message: str = None):
         logger = self.loggers[op_code]
         extra = {
             'op_code': op_code.name,
             'record': record
         }
         msg = f'{op_code.name} - {record}' if message is None else message
-        logger.log(op_code.get_default_logging_level(), msg, extra=extra)
+        logger.log(op_code.default_logging_level, msg, extra=extra)
```

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/processor.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/processor.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey/crawler/processors/dump.py` & `monkey.crawler-2.0.0.dev4/monkey/crawler/processors/dump.py`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/PKG-INFO` & `monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.crawler
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: Small framework to crawl misc data sources and process records.
 Home-page: https://bitbucket.org/monkeytechnologies/monkey-crawler
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `monkey.crawler-2.0.0.dev3/monkey.crawler.egg-info/SOURCES.txt` & `monkey.crawler-2.0.0.dev4/monkey.crawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monkey.crawler-2.0.0.dev3/setup.py` & `monkey.crawler-2.0.0.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 from setuptools import setup, find_packages
 
 __name__ = 'monkey.crawler'
-__version__ = '2.0.0.dev3'
+__version__ = '2.0.0.dev4'
 __author__ = 'Xavier ROY'
 __author_email__ = 'xavier@regbuddy.eu'
 
 project_dir = os.path.dirname(os.path.realpath(__file__))
 requirement_file_path = project_dir + '/requirements.txt'
 requirements = []
 if os.path.isfile(requirement_file_path):
```

