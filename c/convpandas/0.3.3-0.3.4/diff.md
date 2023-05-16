# Comparing `tmp/convpandas-0.3.3.tar.gz` & `tmp/convpandas-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convpandas-0.3.3.tar", max compression
+gzip compressed data, was "convpandas-0.3.4.tar", max compression
```

## Comparing `convpandas-0.3.3.tar` & `convpandas-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2021-01-18 12:28:00.704854 convpandas-0.3.3/LICENSE
--rw-r--r--   0        0        0     3251 2021-09-08 06:11:23.953856 convpandas-0.3.3/README.md
--rw-r--r--   0        0        0       64 2021-01-18 12:28:00.704854 convpandas-0.3.3/convpandas/__init__.py
--rw-r--r--   0        0        0     1299 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/__main__.py
--rw-r--r--   0        0        0       22 2023-05-08 06:00:18.816410 convpandas-0.3.3/convpandas/__version__.py
--rw-r--r--   0        0        0        0 2021-01-18 12:28:00.704854 convpandas-0.3.3/convpandas/command/__init__.py
--rw-r--r--   0        0        0     4918 2022-01-05 13:44:35.624680 convpandas-0.3.3/convpandas/command/csv2xlsx.py
--rw-r--r--   0        0        0     2644 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/command/xlsx2csv.py
--rw-r--r--   0        0        0       74 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/common/__init__.py
--rw-r--r--   0        0        0      237 2021-09-08 06:11:23.953856 convpandas-0.3.3/convpandas/common/cli.py
--rw-r--r--   0        0        0     1223 2023-05-08 06:00:11.352388 convpandas-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 convpandas-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-16 06:15:38.124622 convpandas-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3408 2023-05-16 06:15:38.124622 convpandas-0.3.4/README.md
+-rw-r--r--   0        0        0       64 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/__main__.py
+-rw-r--r--   0        0        0      131 2023-05-16 06:15:56.200725 convpandas-0.3.4/convpandas/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/command/__init__.py
+-rw-r--r--   0        0        0     4880 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/command/csv2xlsx.py
+-rw-r--r--   0        0        0     2630 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/command/xlsx2csv.py
+-rw-r--r--   0        0        0       74 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/common/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-16 06:15:38.124622 convpandas-0.3.4/convpandas/common/cli.py
+-rw-r--r--   0        0        0     1214 2023-05-16 06:15:56.200725 convpandas-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 convpandas-0.3.4/PKG-INFO
```

### Comparing `convpandas-0.3.3/LICENSE` & `convpandas-0.3.4/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 yuji38kwmt
+Copyright (c) 2020 Kurusugawa Computer Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `convpandas-0.3.3/README.md` & `convpandas-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # convert-fileformat-with-pandas
 Convert file format with [pandas](https://pandas.pydata.org/).
 
-[![Build Status](https://travis-ci.org/yuji38kwmt/convpandas.svg?branch=master)](https://travis-ci.org/yuji38kwmt/convpandas)
+[![Build Status](https://travis-ci.org/kurusugawa-computer/convpandas.svg?branch=main)](https://travis-ci.org/kurusugawa-computer/convpandas)
 [![PyPI version](https://badge.fury.io/py/convpandas.svg)](https://badge.fury.io/py/convpandas)
 [![Python Versions](https://img.shields.io/pypi/pyversions/convpandas.svg)](https://pypi.org/project/convpandas/)
 
 # Requirements
-* Python 3.7+
+* Python 3.8.1+
 
 # Install
 
 ```
 $ pip install convpandas
 ```
 
@@ -121,7 +121,11 @@
 ```
 
 With specifying `--sheet_name`, you can select sheet name that you want to convert.
 
 ```
 $ convpandas csv2xlsx in.xlsx out.csv --sheet_name sheet2
 ```
+
+
+# Usage for Developer
+Refer to https://github.com/kurusugawa-computer/convert-fileformat-with-pandas/blob/main/README_for_developer.md .
```

### Comparing `convpandas-0.3.3/convpandas/__main__.py` & `convpandas-0.3.4/convpandas/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
     """
 
     parser = argparse.ArgumentParser(
         description="Command Line Interface for AnnoFab",
         formatter_class=PrettyHelpFormatter,
     )
-    parser.add_argument(
-        "--version", action="version", version=f"convpandas {convpandas.__version__}"
-    )
+    parser.add_argument("--version", action="version", version=f"convpandas {convpandas.__version__}")
     parser.set_defaults(command_help=parser.print_help)
 
     subparsers = parser.add_subparsers(dest="command_name")
     csv2xlsx_add_parser(subparsers)
     xlsx2csv_add_parser(subparsers)
 
     if arguments is None:
```

### Comparing `convpandas-0.3.3/convpandas/command/csv2xlsx.py` & `convpandas-0.3.4/convpandas/command/csv2xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,15 @@
 
     workbook = openpyxl.Workbook(write_only=True)
     for sheet_name, df in df_dict.items():
         if sheet_name == "-":
             worksheet = workbook.create_sheet()
         else:
             if len(sheet_name) > MAXIMUM_NUMBER_OF_CHARACTERS_OF_SHEET_NAME:
-                warnings.warn(
-                    f"Sheet name '{sheet_name}' is more than 31 characters. So sheet name is truncated."
-                )
+                warnings.warn(f"Sheet name '{sheet_name}' is more than 31 characters. So sheet name is truncated.")
                 sheet_name = sheet_name[0:MAXIMUM_NUMBER_OF_CHARACTERS_OF_SHEET_NAME]
             worksheet = workbook.create_sheet(title=sheet_name)
         values = df.values
         for row_index in range(df.shape[0]):
             row = values[row_index]
             worksheet.append([convert_func(value) for value in row])
     workbook.save(xlsx_file)
```

### Comparing `convpandas-0.3.3/convpandas/command/xlsx2csv.py` & `convpandas-0.3.4/convpandas/command/xlsx2csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,15 @@
 
     parser.add_argument(
         "--sheet_name",
         type=str,
         help="Sheet name when reading xlsx. If not specified, read 1st sheet.",
     )
 
-    parser.add_argument(
-        "--sep", default=",", help="Field delimiter for the output file."
-    )
+    parser.add_argument("--sep", default=",", help="Field delimiter for the output file.")
 
     parser.add_argument(
         "--encoding",
         default="utf-8",
         help="A string representing the encoding to use in the output file.",
     )
     parser.add_argument(
```

### Comparing `convpandas-0.3.3/PKG-INFO` & `convpandas-0.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 Metadata-Version: 2.1
 Name: convpandas
-Version: 0.3.3
+Version: 0.3.4
 Summary: Convert file format with pandas
-Home-page: https://github.com/yuji38kwmt/convert-fileformat-with-pandas.git
+Home-page: https://github.com/kurusugawa-computer/convert-fileformat-with-pandas.git
 License: MIT
 Keywords: pandas,csv,xlsx,excel
-Author: yuji38kwmt
-Maintainer: yuji38kwmt
-Requires-Python: >=3.7.1,<4.0.0
+Author: Kurusugawa Computer Inc.
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: openpyxl
 Requires-Dist: pandas (>=1)
-Project-URL: Repository, https://github.com/yuji38kwmt/convert-fileformat-with-pandas.git
+Project-URL: Repository, https://github.com/kurusugawa-computer/convert-fileformat-with-pandas.git
 Description-Content-Type: text/markdown
 
 # convert-fileformat-with-pandas
 Convert file format with [pandas](https://pandas.pydata.org/).
 
-[![Build Status](https://travis-ci.org/yuji38kwmt/convpandas.svg?branch=master)](https://travis-ci.org/yuji38kwmt/convpandas)
+[![Build Status](https://travis-ci.org/kurusugawa-computer/convpandas.svg?branch=main)](https://travis-ci.org/kurusugawa-computer/convpandas)
 [![PyPI version](https://badge.fury.io/py/convpandas.svg)](https://badge.fury.io/py/convpandas)
 [![Python Versions](https://img.shields.io/pypi/pyversions/convpandas.svg)](https://pypi.org/project/convpandas/)
 
 # Requirements
-* Python 3.7+
+* Python 3.8.1+
 
 # Install
 
 ```
 $ pip install convpandas
 ```
 
@@ -153,7 +146,11 @@
 
 With specifying `--sheet_name`, you can select sheet name that you want to convert.
 
 ```
 $ convpandas csv2xlsx in.xlsx out.csv --sheet_name sheet2
 ```
 
+
+# Usage for Developer
+Refer to https://github.com/kurusugawa-computer/convert-fileformat-with-pandas/blob/main/README_for_developer.md .
+
```

