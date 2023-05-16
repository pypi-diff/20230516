# Comparing `tmp/iridauploader-0.9.0.tar.gz` & `tmp/iridauploader-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iridauploader-0.9.0.tar", last modified: Mon Mar  6 17:39:54 2023, max compression
+gzip compressed data, was "iridauploader-0.9.2.tar", last modified: Tue May 16 14:34:57 2023, max compression
```

## Comparing `iridauploader-0.9.0.tar` & `iridauploader-0.9.2.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.582199 iridauploader-0.9.0/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11361 2022-11-07 16:16:28.000000 iridauploader-0.9.0/LICENSE
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3848 2023-03-06 17:39:54.582199 iridauploader-0.9.0/PKG-INFO
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3236 2023-03-03 16:58:16.000000 iridauploader-0.9.0/README.md
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.574199 iridauploader-0.9.0/iridauploader/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       25 2023-03-03 17:22:05.000000 iridauploader-0.9.0/iridauploader/__init__.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.574199 iridauploader-0.9.0/iridauploader/api/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      147 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/api/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    46568 2023-03-03 17:22:05.000000 iridauploader-0.9.0/iridauploader/api/api_calls.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.574199 iridauploader-0.9.0/iridauploader/api/exceptions/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      330 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/api/exceptions/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      112 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/api/exceptions/file_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      253 2022-11-25 22:41:38.000000 iridauploader-0.9.0/iridauploader/api/exceptions/irida_connection_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      756 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/api/exceptions/irida_resource_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      258 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/api/exceptions/irida_upload_canceled_exception.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.574199 iridauploader-0.9.0/iridauploader/config/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      133 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/config/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    13224 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/config/config.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/core/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      119 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11821 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/core/api_handler.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    13379 2023-02-09 06:17:19.000000 iridauploader-0.9.0/iridauploader/core/cli.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      834 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/exit_return.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1675 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/file_size_validator.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3065 2023-02-22 20:34:55.000000 iridauploader-0.9.0/iridauploader/core/logger.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3954 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/model_validator.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3163 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/parsing_handler.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1270 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/uniform_file_count_validator.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    14299 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/upload.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9860 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/core/upload_helpers.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/gui/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       53 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/gui/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      199 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/gui/colours.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11620 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/gui/config.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1610 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/gui/gui.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    21755 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/gui/main_dialog.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6217 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/gui/threads.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1287 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/gui/tools.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9934 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/gui/widgets.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/messaging/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/messaging/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1839 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/messaging/pubsub.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/model/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      439 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    10356 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/directory_status.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/model/exceptions/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       87 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/exceptions/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      629 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/exceptions/model_validation_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1299 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/metadata.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2396 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/project.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3559 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/model/sample.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1289 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/model/sequence_file.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2332 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/model/sequencing_run.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      353 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/model/validation_result.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      260 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1204 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/base_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4244 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/common.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/directory/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       58 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/directory/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7385 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/directory/parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9128 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/directory/sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2241 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/directory/validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/exceptions/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      393 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/exceptions/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      505 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/exceptions/directory_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      628 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/exceptions/file_size_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      839 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/exceptions/sample_sheet_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      579 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/exceptions/sequence_file_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      757 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/exceptions/validation_error.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/miniseq/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       56 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miniseq/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8726 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miniseq/parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    12637 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miniseq/sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2768 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miniseq/validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/miseq/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       54 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miseq/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7742 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miseq/parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11622 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miseq/sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2798 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/miseq/validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/nextseq/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       56 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     5345 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq/parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    12326 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq/sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2798 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq/validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       62 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7751 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    10874 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2826 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/validation.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1629 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/parsers/parsers.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/progress/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      258 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/progress/__init__.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/progress/exceptions/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       77 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/progress/exceptions/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      570 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/progress/exceptions/directory_error.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1471 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/progress/upload_signals.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7663 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/progress/upload_status.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/__init__.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/api/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/tests/api/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2314 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/tests/api/test_api_calls.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/config/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/config/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11427 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/tests/config/test_config.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/core/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/core/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    27358 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests/core/test_api_handler.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4476 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/core/test_cli.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3459 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/core/test_file_size_validator.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    10579 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests/core/test_parsing_handler.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9569 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/core/test_uniform_file_count_validator.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    25258 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/core/test_upload.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    26656 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests/core/test_upload_helpers.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/model/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests/model/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4739 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests/model/test_models.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/__init__.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/common/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/common/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4056 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests/parsers/common/test_common.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/directory/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/directory/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9343 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/directory/test_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11035 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/directory/test_sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3648 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/directory/test_validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7664 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/test_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    19824 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/test_sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7480 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/test_validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/miseq/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miseq/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6985 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miseq/test_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    19147 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miseq/test_sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8002 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/miseq/test_validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6342 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/test_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    19743 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/test_sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8004 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/test_validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.578199 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6972 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/test_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    15092 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/test_sample_parser.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7149 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/test_validation.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.582199 iridauploader-0.9.0/iridauploader/tests/progress/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/progress/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8846 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests/progress/test_upload_status.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.582199 iridauploader-0.9.0/iridauploader/tests_integration/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests_integration/__init__.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     5860 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests_integration/integration_data_setup.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1260 2022-11-07 16:16:28.000000 iridauploader-0.9.0/iridauploader/tests_integration/start_integration_tests.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9140 2023-03-03 16:58:16.000000 iridauploader-0.9.0/iridauploader/tests_integration/test_api_integration.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    53799 2023-02-09 06:17:19.000000 iridauploader-0.9.0/iridauploader/tests_integration/test_end_to_end.py
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2898 2023-02-13 03:10:49.000000 iridauploader-0.9.0/iridauploader/tests_integration/tests_integration.py
-drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:39:54.574199 iridauploader-0.9.0/iridauploader.egg-info/
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3848 2023-03-06 17:39:54.000000 iridauploader-0.9.0/iridauploader.egg-info/PKG-INFO
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     5555 2023-03-06 17:39:54.000000 iridauploader-0.9.0/iridauploader.egg-info/SOURCES.txt
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        1 2023-03-06 17:39:54.000000 iridauploader-0.9.0/iridauploader.egg-info/dependency_links.txt
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      205 2023-03-06 17:39:54.000000 iridauploader-0.9.0/iridauploader.egg-info/entry_points.txt
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      153 2023-03-06 17:39:54.000000 iridauploader-0.9.0/iridauploader.egg-info/requires.txt
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       14 2023-03-06 17:39:54.000000 iridauploader-0.9.0/iridauploader.egg-info/top_level.txt
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       38 2023-03-06 17:39:54.582199 iridauploader-0.9.0/setup.cfg
--rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1843 2023-03-03 17:22:05.000000 iridauploader-0.9.0/setup.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.524834 iridauploader-0.9.2/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11361 2022-11-07 16:16:28.000000 iridauploader-0.9.2/LICENSE
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3848 2023-05-16 14:34:57.524834 iridauploader-0.9.2/PKG-INFO
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3236 2023-03-06 17:48:19.000000 iridauploader-0.9.2/README.md
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.516834 iridauploader-0.9.2/iridauploader/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       25 2023-05-15 20:21:33.000000 iridauploader-0.9.2/iridauploader/__init__.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.516834 iridauploader-0.9.2/iridauploader/api/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      147 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/api/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    46432 2023-05-15 20:21:33.000000 iridauploader-0.9.2/iridauploader/api/api_calls.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.516834 iridauploader-0.9.2/iridauploader/api/exceptions/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      330 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/api/exceptions/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      112 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/api/exceptions/file_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      253 2022-11-25 22:41:38.000000 iridauploader-0.9.2/iridauploader/api/exceptions/irida_connection_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      756 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/api/exceptions/irida_resource_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      258 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/api/exceptions/irida_upload_canceled_exception.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.516834 iridauploader-0.9.2/iridauploader/config/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      133 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/config/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    13224 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/config/config.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.516834 iridauploader-0.9.2/iridauploader/core/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      119 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11821 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/core/api_handler.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    13379 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/core/cli.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      834 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/exit_return.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1675 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/file_size_validator.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3065 2023-02-22 20:34:55.000000 iridauploader-0.9.2/iridauploader/core/logger.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3954 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/model_validator.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3163 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/parsing_handler.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1270 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/uniform_file_count_validator.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    14299 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/upload.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9860 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/core/upload_helpers.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/gui/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       53 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/gui/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      199 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/gui/colours.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11620 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/gui/config.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1610 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/gui/gui.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    21755 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/gui/main_dialog.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6217 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/gui/threads.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1287 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/gui/tools.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9934 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/gui/widgets.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/messaging/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/messaging/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1839 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/messaging/pubsub.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/model/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      439 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    10356 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/directory_status.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/model/exceptions/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       87 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/exceptions/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      629 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/exceptions/model_validation_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1299 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/metadata.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2396 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/project.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3559 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/model/sample.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1289 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/model/sequence_file.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2332 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/model/sequencing_run.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      353 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/model/validation_result.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      260 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1204 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/base_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4244 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/common.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/directory/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       58 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/directory/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7385 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/directory/parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9128 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/directory/sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2241 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/directory/validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/exceptions/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      393 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/exceptions/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      505 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/exceptions/directory_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      628 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/exceptions/file_size_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      839 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/exceptions/sample_sheet_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      579 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/exceptions/sequence_file_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      757 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/exceptions/validation_error.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/miniseq/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       56 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miniseq/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8726 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miniseq/parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    12637 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miniseq/sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2768 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miniseq/validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/miseq/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       54 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miseq/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7742 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miseq/parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11622 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miseq/sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2798 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/miseq/validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/nextseq/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       56 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     5345 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq/parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    12326 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq/sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2798 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq/validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       62 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7751 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    10874 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2826 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/validation.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1629 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/parsers/parsers.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/progress/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      258 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/progress/__init__.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/progress/exceptions/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       77 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/progress/exceptions/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      570 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/progress/exceptions/directory_error.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1471 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/progress/upload_signals.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7663 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/progress/upload_status.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/__init__.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/api/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/api/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2314 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/api/test_api_calls.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/config/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/config/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11427 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/config/test_config.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/core/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/core/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    27358 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/core/test_api_handler.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4476 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/core/test_cli.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3459 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/core/test_file_size_validator.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    10579 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/core/test_parsing_handler.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9569 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/core/test_uniform_file_count_validator.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    25258 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/core/test_upload.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    26656 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/core/test_upload_helpers.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/model/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/model/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4739 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/model/test_models.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/parsers/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/__init__.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/parsers/common/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/common/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     4056 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests/parsers/common/test_common.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/parsers/directory/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/directory/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9343 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/directory/test_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    11035 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/directory/test_sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3648 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/directory/test_validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.520834 iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7664 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/test_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    19824 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/test_sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7480 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/test_validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.524834 iridauploader-0.9.2/iridauploader/tests/parsers/miseq/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miseq/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6985 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miseq/test_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    19147 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miseq/test_sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8002 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/miseq/test_validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.524834 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6342 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/test_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    19743 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/test_sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8004 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/test_validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.524834 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     6972 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/test_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    15092 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/test_sample_parser.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     7149 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/test_validation.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.524834 iridauploader-0.9.2/iridauploader/tests/progress/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/progress/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     8846 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests/progress/test_upload_status.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.524834 iridauploader-0.9.2/iridauploader/tests_integration/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        0 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests_integration/__init__.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     5860 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests_integration/integration_data_setup.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1260 2022-11-07 16:16:28.000000 iridauploader-0.9.2/iridauploader/tests_integration/start_integration_tests.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     9140 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests_integration/test_api_integration.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)    53799 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests_integration/test_end_to_end.py
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     2898 2023-03-06 17:48:19.000000 iridauploader-0.9.2/iridauploader/tests_integration/tests_integration.py
+drwxr-xr-x   0 jthiessen (101513) grp_jthiessen (102187)        0 2023-05-16 14:34:57.516834 iridauploader-0.9.2/iridauploader.egg-info/
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     3848 2023-05-16 14:34:57.000000 iridauploader-0.9.2/iridauploader.egg-info/PKG-INFO
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     5555 2023-05-16 14:34:57.000000 iridauploader-0.9.2/iridauploader.egg-info/SOURCES.txt
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)        1 2023-05-16 14:34:57.000000 iridauploader-0.9.2/iridauploader.egg-info/dependency_links.txt
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      205 2023-05-16 14:34:57.000000 iridauploader-0.9.2/iridauploader.egg-info/entry_points.txt
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)      153 2023-05-16 14:34:57.000000 iridauploader-0.9.2/iridauploader.egg-info/requires.txt
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       14 2023-05-16 14:34:57.000000 iridauploader-0.9.2/iridauploader.egg-info/top_level.txt
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)       38 2023-05-16 14:34:57.524834 iridauploader-0.9.2/setup.cfg
+-rw-r--r--   0 jthiessen (101513) grp_jthiessen (102187)     1820 2023-05-16 14:28:46.000000 iridauploader-0.9.2/setup.py
```

### Comparing `iridauploader-0.9.0/LICENSE` & `iridauploader-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/PKG-INFO` & `iridauploader-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: iridauploader
-Version: 0.9.0
+Version: 0.9.2
 Summary: IRIDA uploader: upload NGS data to IRIDA system
 Home-page: https://github.com/phac-nml/irida-uploader
 Author: Jeffrey Thiessen
 Author-email: jeffrey.thiessen@canada.ca
 License: Apache-2.0
 Keywords: IRIDA NGS uploader
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: GUI
 Provides-Extra: TEST
 Provides-Extra: WINDOWS
 License-File: LICENSE
 
 IRIDA Uploader
```

### Comparing `iridauploader-0.9.0/README.md` & `iridauploader-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/api/api_calls.py` & `iridauploader-0.9.2/iridauploader/api/api_calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                   "Chrome/71.1.2222.33 Safari/537.36",
     "Accept-Encoding": "*",
     "Connection": "keep-alive"
 }
 
 JSON_HEADERS = {"headers": {'Content-Type': 'application/json', **SESSION_HEADERS}}
 
-MINIMUM_IRIDA_VERSION = "20.05"
+MINIMUM_IRIDA_VERSION = "23.01"
 
 
 class ApiCalls(object):
 
     def __init__(self, client_id, client_secret,
                  base_url, username, password, timeout_multiplier=10, max_wait_time=20,
                  http_max_retries=5, http_backoff_factor=0):
@@ -132,15 +132,15 @@
         # backoff = 1 = [0.5, 1, 2, 4, 8, 16, 32, 64, 128, 256, ...]
         # backoff = 2 = [1, 2, 4, 8, 16, 32, 64, 128, 256, 512, ...]
         # backoff = 10 = [5, 10, 20, 40, 80, 160, 320, 640, 1280, 2560, ...]
         retry_strategy = Retry(
             total=self.http_max_retries,
             backoff_factor=self.http_backoff_factor,
             status_forcelist=[429, 500, 502, 503, 504],
-            method_whitelist=["HEAD", "GET", "PUT", "POST"],  # by default POST is excluded
+            allowed_methods=["HEAD", "GET", "PUT", "POST"],  # by default POST is excluded
         )
         # override retries built in max backoff value
         Retry.DEFAULT_BACKOFF_MAX = self.http_backoff_factor
         _sess.mount('https://', HTTPAdapter(max_retries=retry_strategy))
         _sess.mount('http://', HTTPAdapter(max_retries=retry_strategy))
         self._session_instance = _sess
 
@@ -656,21 +656,19 @@
         :param project_id:
         :param sample_name:
         :return: Sample obj or None
         """
 
         logging.info("Getting Sample object for project id '{}' and sample name '{}'".format(project_id, sample_name))
 
-        # This is using a deprecated end point. In a future release it will be replaced with
-        # /projects/{project_id}/samples/bySampleName
-        # and use params instead
-        url = f"{self.base_url}projects/{project_id}/samples/bySequencerId/{sample_name}"
+        url = f"{self.base_url}projects/{project_id}/samples/bySampleName"
+        params = {'sampleName': sample_name}
 
         try:
-            response = self._session.get(url)
+            response = self._session.get(url, params=params)
         except Exception as e:
             raise ApiCalls._handle_rest_exception(url, e)
         if response.status_code == HTTPStatus.OK:  # 200, return sample object
             logging.debug("sample found")
             sample_dict = response.json()["resource"]
             return ApiCalls._build_sample_obj_from_resource(sample_dict)
         elif response.status_code == HTTPStatus.NOT_FOUND:  # 404, return None
```

### Comparing `iridauploader-0.9.0/iridauploader/api/exceptions/irida_resource_error.py` & `iridauploader-0.9.2/iridauploader/api/exceptions/irida_resource_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/config/config.py` & `iridauploader-0.9.2/iridauploader/config/config.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/api_handler.py` & `iridauploader-0.9.2/iridauploader/core/api_handler.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/cli.py` & `iridauploader-0.9.2/iridauploader/core/cli.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/exit_return.py` & `iridauploader-0.9.2/iridauploader/core/exit_return.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/file_size_validator.py` & `iridauploader-0.9.2/iridauploader/core/file_size_validator.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/logger.py` & `iridauploader-0.9.2/iridauploader/core/logger.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/model_validator.py` & `iridauploader-0.9.2/iridauploader/core/model_validator.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/parsing_handler.py` & `iridauploader-0.9.2/iridauploader/core/parsing_handler.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/uniform_file_count_validator.py` & `iridauploader-0.9.2/iridauploader/core/uniform_file_count_validator.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/upload.py` & `iridauploader-0.9.2/iridauploader/core/upload.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/core/upload_helpers.py` & `iridauploader-0.9.2/iridauploader/core/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/gui/config.py` & `iridauploader-0.9.2/iridauploader/gui/config.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/gui/gui.py` & `iridauploader-0.9.2/iridauploader/gui/gui.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/gui/main_dialog.py` & `iridauploader-0.9.2/iridauploader/gui/main_dialog.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/gui/threads.py` & `iridauploader-0.9.2/iridauploader/gui/threads.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/gui/tools.py` & `iridauploader-0.9.2/iridauploader/gui/tools.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/gui/widgets.py` & `iridauploader-0.9.2/iridauploader/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/messaging/pubsub.py` & `iridauploader-0.9.2/iridauploader/messaging/pubsub.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/directory_status.py` & `iridauploader-0.9.2/iridauploader/model/directory_status.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/exceptions/model_validation_error.py` & `iridauploader-0.9.2/iridauploader/model/exceptions/model_validation_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/metadata.py` & `iridauploader-0.9.2/iridauploader/model/metadata.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/project.py` & `iridauploader-0.9.2/iridauploader/model/project.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/sample.py` & `iridauploader-0.9.2/iridauploader/model/sample.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/sequence_file.py` & `iridauploader-0.9.2/iridauploader/model/sequence_file.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/model/sequencing_run.py` & `iridauploader-0.9.2/iridauploader/model/sequencing_run.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/base_parser.py` & `iridauploader-0.9.2/iridauploader/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/common.py` & `iridauploader-0.9.2/iridauploader/parsers/common.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/directory/parser.py` & `iridauploader-0.9.2/iridauploader/parsers/directory/parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/directory/sample_parser.py` & `iridauploader-0.9.2/iridauploader/parsers/directory/sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/directory/validation.py` & `iridauploader-0.9.2/iridauploader/parsers/directory/validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/exceptions/file_size_error.py` & `iridauploader-0.9.2/iridauploader/parsers/exceptions/file_size_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/exceptions/sample_sheet_error.py` & `iridauploader-0.9.2/iridauploader/parsers/exceptions/sample_sheet_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/exceptions/sequence_file_error.py` & `iridauploader-0.9.2/iridauploader/parsers/exceptions/sequence_file_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/exceptions/validation_error.py` & `iridauploader-0.9.2/iridauploader/parsers/exceptions/validation_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/miniseq/parser.py` & `iridauploader-0.9.2/iridauploader/parsers/miniseq/parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/miniseq/sample_parser.py` & `iridauploader-0.9.2/iridauploader/parsers/miniseq/sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/miniseq/validation.py` & `iridauploader-0.9.2/iridauploader/parsers/miniseq/validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/miseq/parser.py` & `iridauploader-0.9.2/iridauploader/parsers/miseq/parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/miseq/sample_parser.py` & `iridauploader-0.9.2/iridauploader/parsers/miseq/sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/miseq/validation.py` & `iridauploader-0.9.2/iridauploader/parsers/miseq/validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/nextseq/parser.py` & `iridauploader-0.9.2/iridauploader/parsers/nextseq/parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/nextseq/sample_parser.py` & `iridauploader-0.9.2/iridauploader/parsers/nextseq/sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/nextseq/validation.py` & `iridauploader-0.9.2/iridauploader/parsers/nextseq/validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/parser.py` & `iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/sample_parser.py` & `iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/nextseq2k_nml/validation.py` & `iridauploader-0.9.2/iridauploader/parsers/nextseq2k_nml/validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/parsers/parsers.py` & `iridauploader-0.9.2/iridauploader/parsers/parsers.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/progress/exceptions/directory_error.py` & `iridauploader-0.9.2/iridauploader/progress/exceptions/directory_error.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/progress/upload_signals.py` & `iridauploader-0.9.2/iridauploader/progress/upload_signals.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/progress/upload_status.py` & `iridauploader-0.9.2/iridauploader/progress/upload_status.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/api/test_api_calls.py` & `iridauploader-0.9.2/iridauploader/tests/api/test_api_calls.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/config/test_config.py` & `iridauploader-0.9.2/iridauploader/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_api_handler.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_api_handler.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_cli.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_cli.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_file_size_validator.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_file_size_validator.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_parsing_handler.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_parsing_handler.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_uniform_file_count_validator.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_uniform_file_count_validator.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_upload.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_upload.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/core/test_upload_helpers.py` & `iridauploader-0.9.2/iridauploader/tests/core/test_upload_helpers.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/model/test_models.py` & `iridauploader-0.9.2/iridauploader/tests/model/test_models.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/common/test_common.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/common/test_common.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/directory/test_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/directory/test_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/directory/test_sample_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/directory/test_sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/directory/test_validation.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/directory/test_validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/test_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/test_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/test_sample_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/test_sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/miniseq/test_validation.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/miniseq/test_validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/miseq/test_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/miseq/test_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/miseq/test_sample_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/miseq/test_sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/miseq/test_validation.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/miseq/test_validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/test_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/test_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/test_sample_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/test_sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/nextseq/test_validation.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/nextseq/test_validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/test_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/test_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/test_sample_parser.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/test_sample_parser.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/parsers/nextseq2k_nml/test_validation.py` & `iridauploader-0.9.2/iridauploader/tests/parsers/nextseq2k_nml/test_validation.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests/progress/test_upload_status.py` & `iridauploader-0.9.2/iridauploader/tests/progress/test_upload_status.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests_integration/integration_data_setup.py` & `iridauploader-0.9.2/iridauploader/tests_integration/integration_data_setup.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests_integration/start_integration_tests.py` & `iridauploader-0.9.2/iridauploader/tests_integration/start_integration_tests.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests_integration/test_api_integration.py` & `iridauploader-0.9.2/iridauploader/tests_integration/test_api_integration.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests_integration/test_end_to_end.py` & `iridauploader-0.9.2/iridauploader/tests_integration/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader/tests_integration/tests_integration.py` & `iridauploader-0.9.2/iridauploader/tests_integration/tests_integration.py`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/iridauploader.egg-info/PKG-INFO` & `iridauploader-0.9.2/iridauploader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: iridauploader
-Version: 0.9.0
+Version: 0.9.2
 Summary: IRIDA uploader: upload NGS data to IRIDA system
 Home-page: https://github.com/phac-nml/irida-uploader
 Author: Jeffrey Thiessen
 Author-email: jeffrey.thiessen@canada.ca
 License: Apache-2.0
 Keywords: IRIDA NGS uploader
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: GUI
 Provides-Extra: TEST
 Provides-Extra: WINDOWS
 License-File: LICENSE
 
 IRIDA Uploader
```

### Comparing `iridauploader-0.9.0/iridauploader.egg-info/SOURCES.txt` & `iridauploader-0.9.2/iridauploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iridauploader-0.9.0/setup.py` & `iridauploader-0.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Use the readme file as the long description on PyPi
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iridauploader',
-    version='0.9.0',
+    version='0.9.2',
     description='IRIDA uploader: upload NGS data to IRIDA system',
     url='https://github.com/phac-nml/irida-uploader',
     author='Jeffrey Thiessen',
     author_email='jeffrey.thiessen@canada.ca',
     long_description=long_description,
     long_description_content_type="text/markdown",
     # license specified on github
@@ -42,11 +42,11 @@
     # https://pypi.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
-    # Test cases makes make it incompatible with pre 3.6
-    python_requires='>=3.6',
+    # urllib3 v2.0 requires >=3.7
+    python_requires='>=3.7',
 
 )
```

