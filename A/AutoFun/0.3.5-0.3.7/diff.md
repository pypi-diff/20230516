# Comparing `tmp/AutoFun-0.3.5.tar.gz` & `tmp/AutoFun-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFun-0.3.5.tar", last modified: Fri May 12 09:29:04 2023, max compression
+gzip compressed data, was "AutoFun-0.3.7.tar", last modified: Tue May 16 03:36:29 2023, max compression
```

## Comparing `AutoFun-0.3.5.tar` & `AutoFun-0.3.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.753850 AutoFun-0.3.5/
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.667967 AutoFun-0.3.5/AutoFun/
--rw-rw-rw-   0        0        0    97792 2023-05-12 09:28:28.000000 AutoFun-0.3.5/AutoFun/AutoFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.678963 AutoFun-0.3.5/AutoFun/CutPdf/
--rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.5/AutoFun/CutPdf/CutPdf.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.681964 AutoFun-0.3.5/AutoFun/CutPdf/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/CutPdf/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.5/AutoFun/CutPdf/Function/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.685963 AutoFun-0.3.5/AutoFun/CutPdf/Ui/
--rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.5/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/CutPdf/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/CutPdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.690966 AutoFun-0.3.5/AutoFun/OcrFinish/
--rw-rw-rw-   0        0        0   177664 2023-05-05 03:14:26.000000 AutoFun-0.3.5/AutoFun/OcrFinish/OcrFinish.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.693963 AutoFun-0.3.5/AutoFun/OcrFinish/Ui/
--rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.5/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/OcrFinish/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/OcrFinish/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.697968 AutoFun-0.3.5/AutoFun/OcrPicFun/
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.704964 AutoFun-0.3.5/AutoFun/OcrPicFun/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/Function/__init__.py
--rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/Function/dict_to_json.pyd
--rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/Function/get_json.pyd
--rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/Function/splitJpg.pyd
--rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/OcrPicFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.708963 AutoFun-0.3.5/AutoFun/OcrPicFun/Ui/
--rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/OcrPicFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.711963 AutoFun-0.3.5/AutoFun/OcrTableFun/
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.724992 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/
--rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/optionDb.pyd
--rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/saveLoad.py
--rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Function/txt_OCR.db
--rw-rw-rw-   0        0        0   194048 2023-05-05 06:43:24.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/OcrTableFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.729017 AutoFun-0.3.5/AutoFun/OcrTableFun/Ui/
--rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.5/AutoFun/OcrTableFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.734018 AutoFun-0.3.5/AutoFun/SplitPdfFun/
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.747885 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/
--rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/optionDb.pyd
--rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
--rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
--rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
--rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
--rw-rw-rw-   0        0        0   167936 2023-05-12 08:06:13.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/SplitPdfFun.pyd
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.752967 AutoFun-0.3.5/AutoFun/SplitPdfFun/Ui/
--rw-rw-rw-   0        0        0    72192 2023-05-12 08:06:23.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.5/AutoFun/SplitPdfFun/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.5/AutoFun/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 09:29:04.675963 AutoFun-0.3.5/AutoFun.egg-info/
--rw-rw-rw-   0        0        0      396 2023-05-12 09:29:04.000000 AutoFun-0.3.5/AutoFun.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1695 2023-05-12 09:29:04.000000 AutoFun-0.3.5/AutoFun.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 09:29:04.000000 AutoFun-0.3.5/AutoFun.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 09:29:04.000000 AutoFun-0.3.5/AutoFun.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      396 2023-05-12 09:29:04.753850 AutoFun-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.5/README.md
--rw-rw-rw-   0        0        0      136 2023-05-12 09:29:04.754849 AutoFun-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      967 2023-05-12 09:28:52.000000 AutoFun-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.668067 AutoFun-0.3.7/
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.536191 AutoFun-0.3.7/AutoFun/
+-rw-rw-rw-   0        0        0    97792 2023-05-16 01:18:21.000000 AutoFun-0.3.7/AutoFun/AutoFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.549075 AutoFun-0.3.7/AutoFun/CutPdf/
+-rw-rw-rw-   0        0        0   245760 2023-05-05 08:57:48.000000 AutoFun-0.3.7/AutoFun/CutPdf/CutPdf.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.554075 AutoFun-0.3.7/AutoFun/CutPdf/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/CutPdf/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-05-05 03:08:24.000000 AutoFun-0.3.7/AutoFun/CutPdf/Function/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.562072 AutoFun-0.3.7/AutoFun/CutPdf/Ui/
+-rw-rw-rw-   0        0        0    98816 2023-05-05 03:08:08.000000 AutoFun-0.3.7/AutoFun/CutPdf/Ui/CutPdfPicUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/CutPdf/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/CutPdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.566072 AutoFun-0.3.7/AutoFun/OcrFinish/
+-rw-rw-rw-   0        0        0   177664 2023-05-16 01:18:58.000000 AutoFun-0.3.7/AutoFun/OcrFinish/OcrFinish.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.573073 AutoFun-0.3.7/AutoFun/OcrFinish/Ui/
+-rw-rw-rw-   0        0        0    56832 2023-05-05 03:14:46.000000 AutoFun-0.3.7/AutoFun/OcrFinish/Ui/OcrfinishUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrFinish/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrFinish/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.579083 AutoFun-0.3.7/AutoFun/OcrPicFun/
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.591072 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    35328 2023-05-05 03:22:58.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/dict_to_json.pyd
+-rw-rw-rw-   0        0        0    60416 2023-05-05 03:24:04.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/get_json.pyd
+-rw-rw-rw-   0        0        0    42496 2023-05-05 03:25:20.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Function/splitJpg.pyd
+-rw-rw-rw-   0        0        0   303616 2023-05-06 06:48:22.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/OcrPicFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.596100 AutoFun-0.3.7/AutoFun/OcrPicFun/Ui/
+-rw-rw-rw-   0        0        0    96256 2023-05-05 03:24:34.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Ui/OcrparameterUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/OcrPicFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.601086 AutoFun-0.3.7/AutoFun/OcrTableFun/
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.620067 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:46:44.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:52.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:47:22.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    18608 2023-05-05 09:10:40.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/saveLoad.py
+-rw-rw-rw-   0        0        0   175104 2023-04-28 05:48:00.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:48.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Function/txt_OCR.db
+-rw-rw-rw-   0        0        0   195584 2023-05-16 01:19:44.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/OcrTableFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.626067 AutoFun-0.3.7/AutoFun/OcrTableFun/Ui/
+-rw-rw-rw-   0        0        0    80384 2023-05-05 03:30:36.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Ui/OcrTableUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:50.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:54.000000 AutoFun-0.3.7/AutoFun/OcrTableFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.632068 AutoFun-0.3.7/AutoFun/SplitPdfFun/
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.657067 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/
+-rw-rw-rw-   0        0        0    47616 2023-04-28 05:51:40.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/DB_in_sqlite.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-04-28 05:51:48.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/optionDb.pyd
+-rw-rw-rw-   0        0        0    70656 2023-04-28 05:51:56.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/pdf_utils.pyd
+-rw-rw-rw-   0        0        0   146944 2023-04-28 05:52:08.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/splite_pdf.pyd
+-rw-rw-rw-   0        0        0   122368 2023-04-28 05:52:20.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/splite_pdf_no_Table.pyd
+-rw-rw-rw-   0        0        0   169472 2023-04-28 05:52:32.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Function/sqlite_to_excel.pyd
+-rw-rw-rw-   0        0        0   167936 2023-05-12 08:06:13.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/SplitPdfFun.pyd
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.665077 AutoFun-0.3.7/AutoFun/SplitPdfFun/Ui/
+-rw-rw-rw-   0        0        0    72192 2023-05-12 08:06:23.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Ui/SplitPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-04-27 12:00:00.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-27 11:59:58.000000 AutoFun-0.3.7/AutoFun/SplitPdfFun/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 09:51:16.000000 AutoFun-0.3.7/AutoFun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:29.543191 AutoFun-0.3.7/AutoFun.egg-info/
+-rw-rw-rw-   0        0        0      396 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1695 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 03:36:29.000000 AutoFun-0.3.7/AutoFun.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 AutoFun-0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AutoFun-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      396 2023-05-16 03:36:29.668067 AutoFun-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 AutoFun-0.3.7/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-16 03:36:29.669077 AutoFun-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-05-16 03:36:17.000000 AutoFun-0.3.7/setup.py
```

### Comparing `AutoFun-0.3.5/AutoFun/OcrTableFun/Function/saveLoad.py` & `AutoFun-0.3.7/AutoFun/OcrTableFun/Function/saveLoad.py`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.5/AutoFun.egg-info/SOURCES.txt` & `AutoFun-0.3.7/AutoFun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.5/LICENSE.txt` & `AutoFun-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AutoFun-0.3.5/setup.py` & `AutoFun-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 5
+PATCH = 7
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AutoFun",
```

