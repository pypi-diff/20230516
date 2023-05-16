# Comparing `tmp/callingcardstools-0.1.4.tar.gz` & `tmp/callingcardstools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.1.4.tar", max compression
+gzip compressed data, was "callingcardstools-0.1.5.tar", max compression
```

## Comparing `callingcardstools-0.1.4.tar` & `callingcardstools-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.4/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.4/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/mammals/ReadRecords.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.4/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.4/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.4/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.4/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    16935 2023-05-14 12:37:55.905065 callingcardstools-0.1.4/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.4/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     4084 2023-05-06 12:15:15.710439 callingcardstools-0.1.4/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.4/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     7357 2023-05-06 11:17:03.212706 callingcardstools-0.1.4/callingcardstools/QC/parse_id_to_barcode.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.4/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.4/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.4/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.4/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.4/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.4/callingcardstools/__init__.py
--rw-r--r--   0        0        0     5674 2023-05-14 12:31:35.835834 callingcardstools-0.1.4/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.4/callingcardstools/utils.py
--rw-r--r--   0        0        0     2016 2023-05-14 12:39:49.417968 callingcardstools-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.4/setup.py
--rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/README.md
+-rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.1.5/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0     8592 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/mammals/ReadRecords.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     7744 2023-04-30 11:27:18.725988 callingcardstools-0.1.5/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.1.5/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.1.5/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.1.5/callingcardstools/BarcodeParser/barcode_table_to_json.py
+-rw-r--r--   0        0        0    17091 2023-05-15 16:54:18.678237 callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/combine_qc.py
+-rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.1.5/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.1.5/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.1.5/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.1.5/callingcardstools/Resources/PackageResources.py
+-rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/human/__init__.py
+-rw-r--r--   0        0        0      695 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/human/barcode_details.json
+-rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/human/chr_map.csv
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/mouse/__init__.py
+-rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/mouse/barcode_details.json
+-rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.1.5/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.1.5/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.1.5/callingcardstools/Resources/yeast/yeast.db
+-rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.1.5/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     6020 2023-05-16 01:28:13.619621 callingcardstools-0.1.5/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.1.5/callingcardstools/utils.py
+-rw-r--r--   0        0        0     2016 2023-05-16 01:33:28.098799 callingcardstools-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 callingcardstools-0.1.5/setup.py
+-rw-r--r--   0        0        0     2634 1970-01-01 00:00:00.000000 callingcardstools-0.1.5/PKG-INFO
```

### Comparing `callingcardstools-0.1.4/LICENSE` & `callingcardstools-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/README.md` & `callingcardstools-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-0.1.5/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-0.1.5/callingcardstools/Alignment/SummaryParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Alignment/mammals/ReadRecords.py` & `callingcardstools-0.1.5/callingcardstools/Alignment/mammals/ReadRecords.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-0.1.5/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-0.1.5/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-0.1.5/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-0.1.5/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/BarcodeParser/barcode_table_to_json.py` & `callingcardstools-0.1.5/callingcardstools/BarcodeParser/barcode_table_to_json.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-0.1.5/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,32 +120,32 @@
         # Combine _r1_transposon_seq_dict dictionaries
         for r1_transposon_edit_dist, r1_transposon_seq_set in \
                 other.r1_transposon_dict.items():
             self._r1_transposon_seq_dict[r1_transposon_edit_dist]\
                 .update(r1_transposon_seq_set)
 
     # public methods ----------------------------------------------------------
-
-    @classmethod
-    def load(cls, file_path: str) -> "BarcodeQcCounter":
+    def load(self, file_path: str):
         """Load a BarcodeQcCounter object from a file using Pickle.
 
         Args:
             file_path (str): The file path where the object is stored.
 
         Returns:
-            BarcodeQcCounter: The loaded BarcodeQcCounter object.
+            None
         """
         logger.info("loading BarcodeQcCounter object from %s", file_path)
         with open(file_path, "rb") as file:
             file_data = pickle.load(file)
-            if not isinstance(file_data, cls):
+            if not isinstance(file_data, BarcodeQcCounter):
                 raise TypeError(
                     f"{file_path} is not a BarcodeQcCounter object")
-            return file_data
+            # copy the data from the loaded object to the current instance
+            self._metrics = file_data._metrics
+            self._r1_transposon_seq_dict = file_data._r1_transposon_seq_dict
 
     @classmethod
     def combine(
             cls, counters: Iterable["BarcodeQcCounter"]) -> "BarcodeQcCounter":
         """Combine multiple BarcodeQcCounter objects into a single object.
 
         Args:
@@ -365,26 +365,27 @@
                 raise ValueError("component_dict values must be lists of "
                                  "the same length")
             # extract summaries from the metrics
             r1_primer_summary, r2_transposon_summary = \
                 self._summarize_by_tf(component_dict)
             
             # write r1_primer_summary to file
+            append_suffix = '_' + suffix if suffix else ''
             r1_primer_basename = \
-                filename + "_r1_primer_summary" + '_' + suffix + ".csv"
+                filename + "_r1_primer_summary" + append_suffix + ".csv"
             r1_primer_summary_path = os.path.join(
                 output_dirpath, r1_primer_basename)
             r1_primer_summary_df = pd.DataFrame(r1_primer_summary)
             logger.info("writing r1_primer_summary "
                         "to %s{r1_primer_summary_path}")
             r1_primer_summary_df.to_csv(r1_primer_summary_path, index=False)
             
             # write r2_transposon summary to file
             r2_transposon_summary_basename = \
-                filename + "_r2_transposon_summary" + '_' + suffix + ".csv"
+                filename + "_r2_transposon_summary" + append_suffix + ".csv"
             r2_transposon_summary_path = os.path.join(
                 output_dirpath, r2_transposon_summary_basename)
             r2_transposon_summary_df = pd.DataFrame(r2_transposon_summary)
             logger.info("writing r2_transposon_summary "
                         "to %s{r2_transposon_summary_path}")
             r2_transposon_summary_df.to_csv(
                 r2_transposon_summary_path, index=False)
```

### Comparing `callingcardstools-0.1.4/callingcardstools/QC/StatusFlags.py` & `callingcardstools-0.1.5/callingcardstools/QC/StatusFlags.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             # if num is 0 and as_str is true, return NO_STATUS. otherwise, the
             # decomposed list will be empty
             if num == 0:
                 if as_str:
                     return ['NO_STATUS']
             # Use list comprehension to find the powers of two that
             # compose the input number
-            powers = [log2(1 << i) for i
+            powers = [int(log2(1 << i)) for i
                       in range(num.bit_length()) if num & (1 << i)]
 
             if as_str:
                 # Convert the powers of two to their string representation
                 powers = [StatusFlags(int(x)).name for x in powers]
 
             return powers
```

### Comparing `callingcardstools-0.1.4/callingcardstools/QC/create_status_coder.py` & `callingcardstools-0.1.5/callingcardstools/QC/create_status_coder.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Reads/ReadParser.py` & `callingcardstools-0.1.5/callingcardstools/Reads/ReadParser.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-0.1.5/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Reads/split_fastq.py` & `callingcardstools-0.1.5/callingcardstools/Reads/split_fastq.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/PackageResources.py` & `callingcardstools-0.1.5/callingcardstools/Resources/PackageResources.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-0.1.5/callingcardstools/Resources/human/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/human/chr_map.csv` & `callingcardstools-0.1.5/callingcardstools/Resources/human/chr_map.csv`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/mouse/barcode_details.json` & `callingcardstools-0.1.5/callingcardstools/Resources/mouse/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/yeast/README.md` & `callingcardstools-0.1.5/callingcardstools/Resources/yeast/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-0.1.5/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/Resources/yeast/yeast.db` & `callingcardstools-0.1.5/callingcardstools/Resources/yeast/yeast.db`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/callingcardstools/__main__.py` & `callingcardstools-0.1.5/callingcardstools/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import argparse
 from typing import Callable
 import logging
 from logging.config import dictConfig
 from importlib.metadata import version
 
 from .BarcodeParser import barcode_table_to_json
+from .BarcodeParser.yeast import combine_qc as yeast_combine_qc
 from .Reads import legacy_split_fastq, split_fastq
 from .Alignment.yeast import legacy_makeccf
 from .Alignment.mammals import process_alignments as process_mammals_bam
 from .Alignment.yeast import process_alignments as process_yeast_bam
 
+
 def parse_args() -> Callable[[list], argparse.Namespace]:
     """Create a cmd line argument parser for callingcardstools
 
     Returns:
             Callable[[list],Namespace]: This function returns the main
              argparser. If the subparser set_defaults method is set, it can
              make the correct decision as to which function to call to execute
@@ -33,14 +35,17 @@
         'legacy_split_fastq': 'yeast cc_tools 3.0 version of parse_fastq',
 
         'legacy_makeccf': 'This function make .ccf files from mapped '
         '.bam files. ccf files have the following columns: '
         '[chr,start,end,reads,strand,barcode] but only the first 4 '
         'columns are required. The genome coordinates are 1-indexed',
 
+        'yeast_combine_qc': 'Combine BarcodeQcCounter objects which may '
+        'result from splitting the fastq files prior to demultiplexing',
+
         'process_yeast_bam': 'Iterate over yeast alignments to produce a '
         'qBed format file of the passing reads, and a qc file which '
         'allows finer exploration of the barcode and alignment metrics',
 
         'process_mammals_bam': 'Iterate over the reads in an alignment file (bam) and '
         'separate reads into passing.bam and failing.bam, a '
         'qBed format file of the passing reads, and a qc file which '
@@ -68,15 +73,15 @@
         "--version",
         action='version',
         version='%(prog)s '+f'{version("callingcardstools")}')
 
     # parse_bam subparser -----------------------------------------------------
     subparsers = parser.add_subparsers(
         help="Available Tools")
-    
+
     subparsers = barcode_table_to_json.parse_args(
         subparsers,
         script_descriptions['barcode_to_json'],
         common_args
     )
 
     subparsers = legacy_split_fastq.parse_args(
@@ -90,14 +95,19 @@
         common_args)
 
     subparsers = split_fastq.parse_args(
         subparsers,
         script_descriptions['split_fastq'],
         common_args)
 
+    subparsers = yeast_combine_qc.parse_args(
+        subparsers,
+        script_descriptions['yeast_combine_qc'],
+        common_args)
+
     subparsers = process_yeast_bam.parse_args(
         subparsers,
         script_descriptions['process_yeast_bam'],
         common_args
     )
 
     subparsers = process_mammals_bam.parse_args(
```

### Comparing `callingcardstools-0.1.4/callingcardstools/utils.py` & `callingcardstools-0.1.5/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.1.4/pyproject.toml` & `callingcardstools-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.1.4"
+version = "0.1.5"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
```

### Comparing `callingcardstools-0.1.4/setup.py` & `callingcardstools-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'scipy>=1.8.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.1.4/PKG-INFO` & `callingcardstools-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

