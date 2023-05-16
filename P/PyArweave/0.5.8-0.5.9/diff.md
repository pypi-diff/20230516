# Comparing `tmp/PyArweave-0.5.8.tar.gz` & `tmp/PyArweave-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyArweave-0.5.8.tar", last modified: Wed Aug 17 11:43:15 2022, max compression
+gzip compressed data, was "PyArweave-0.5.9.tar", last modified: Thu Aug 18 10:55:55 2022, max compression
```

## Comparing `PyArweave-0.5.8.tar` & `PyArweave-0.5.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.392682 PyArweave-0.5.8/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.332683 PyArweave-0.5.8/.github/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.344683 PyArweave-0.5.8/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      573 2022-08-13 09:55:22.000000 PyArweave-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1860 2022-08-13 09:55:22.000000 PyArweave-0.5.8/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1172 2022-08-13 09:55:22.000000 PyArweave-0.5.8/CHANGELOG.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18092 2022-08-13 09:55:22.000000 PyArweave-0.5.8/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1179 2022-08-13 09:55:22.000000 PyArweave-0.5.8/LICENSE_e142b89
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2022-08-17 11:43:15.392682 PyArweave-0.5.8/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.348682 PyArweave-0.5.8/PyArweave.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2022-08-17 11:43:14.000000 PyArweave-0.5.8/PyArweave.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1129 2022-08-17 11:43:15.000000 PyArweave-0.5.8/PyArweave.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-17 11:43:14.000000 PyArweave-0.5.8/PyArweave.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2022-08-17 11:43:14.000000 PyArweave-0.5.8/PyArweave.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-08-17 11:43:14.000000 PyArweave-0.5.8/PyArweave.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4565 2022-08-13 09:55:22.000000 PyArweave-0.5.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.356682 PyArweave-0.5.8/ar/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2022-08-17 11:41:57.000000 PyArweave-0.5.8/ar/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6045 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/ardrive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/arweave_lib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/block.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16838 2022-08-15 21:45:16.000000 PyArweave-0.5.8/ar/bundle.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2748 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/chunk.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1202 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/manifest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17276 2022-08-16 17:51:52.000000 PyArweave-0.5.8/ar/multipeer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    44235 2022-08-17 11:41:07.000000 PyArweave-0.5.8/ar/peer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3205 2022-08-15 20:04:42.000000 PyArweave-0.5.8/ar/stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11714 2022-08-13 11:05:41.000000 PyArweave-0.5.8/ar/transaction.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.360682 PyArweave-0.5.8/ar/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2566 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/ans104_signers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1425 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/deep_hash.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/file_io.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15584 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/merkle.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10950 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/utils/transaction_uploader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2291 2022-08-13 09:55:22.000000 PyArweave-0.5.8/ar/wallet.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.364682 PyArweave-0.5.8/bundlr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2022-08-13 09:55:22.000000 PyArweave-0.5.8/bundlr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2022-08-13 09:55:22.000000 PyArweave-0.5.8/bundlr/loader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3013 2022-08-15 21:54:50.000000 PyArweave-0.5.8/bundlr/node.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2022-08-13 09:55:22.000000 PyArweave-0.5.8/makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-08-17 11:43:15.392682 PyArweave-0.5.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1693 2022-08-17 11:42:38.000000 PyArweave-0.5.8/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.388682 PyArweave-0.5.8/test/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.388682 PyArweave-0.5.8/test/.vscode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/.vscode/launch.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   376522 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/Mining On The Arweave.pdf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   502030 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/data
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17431 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/package-lock.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/package.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1204 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/simple_http_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/simple_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test.pdf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1217 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test_block.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24701 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test_dataitem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test_jwk_file.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7765 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test_transaction.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2068 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/test_wallet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   613800 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/testfile0.bin
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/transactions.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test/transactions.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      645 2022-08-13 09:55:22.000000 PyArweave-0.5.8/test_upload_bundlr.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-17 11:43:15.392682 PyArweave-0.5.8/toys/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      187 2022-08-13 09:55:22.000000 PyArweave-0.5.8/toys/arweave-index.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2650 2022-08-13 09:55:22.000000 PyArweave-0.5.8/toys/bundlewatcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49810 2022-08-13 09:55:22.000000 PyArweave-0.5.8/toys/indexer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5217 2022-08-13 09:55:22.000000 PyArweave-0.5.8/toys/tagswatcher.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.530907 PyArweave-0.5.9/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.462908 PyArweave-0.5.9/.github/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.474908 PyArweave-0.5.9/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      573 2022-08-13 09:55:22.000000 PyArweave-0.5.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1860 2022-08-13 09:55:22.000000 PyArweave-0.5.9/.gitignore
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1172 2022-08-13 09:55:22.000000 PyArweave-0.5.9/CHANGELOG.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18092 2022-08-13 09:55:22.000000 PyArweave-0.5.9/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1179 2022-08-13 09:55:22.000000 PyArweave-0.5.9/LICENSE_e142b89
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2022-08-18 10:55:55.530907 PyArweave-0.5.9/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.478908 PyArweave-0.5.9/PyArweave.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2022-08-18 10:55:54.000000 PyArweave-0.5.9/PyArweave.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1129 2022-08-18 10:55:55.000000 PyArweave-0.5.9/PyArweave.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-18 10:55:54.000000 PyArweave-0.5.9/PyArweave.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2022-08-18 10:55:54.000000 PyArweave-0.5.9/PyArweave.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2022-08-18 10:55:54.000000 PyArweave-0.5.9/PyArweave.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4565 2022-08-13 09:55:22.000000 PyArweave-0.5.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.490908 PyArweave-0.5.9/ar/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2022-08-17 11:41:57.000000 PyArweave-0.5.9/ar/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6045 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/ardrive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/arweave_lib.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/block.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16838 2022-08-15 21:45:16.000000 PyArweave-0.5.9/ar/bundle.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2748 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/chunk.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1202 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/manifest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17276 2022-08-16 17:51:52.000000 PyArweave-0.5.9/ar/multipeer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45017 2022-08-18 09:59:46.000000 PyArweave-0.5.9/ar/peer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3205 2022-08-15 20:04:42.000000 PyArweave-0.5.9/ar/stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11714 2022-08-13 11:05:41.000000 PyArweave-0.5.9/ar/transaction.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.494908 PyArweave-0.5.9/ar/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2566 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/ans104_signers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1425 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/deep_hash.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      907 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/file_io.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15584 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/merkle.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1665 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10950 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/utils/transaction_uploader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2291 2022-08-13 09:55:22.000000 PyArweave-0.5.9/ar/wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.498908 PyArweave-0.5.9/bundlr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2022-08-13 09:55:22.000000 PyArweave-0.5.9/bundlr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4094 2022-08-13 09:55:22.000000 PyArweave-0.5.9/bundlr/loader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3013 2022-08-15 21:54:50.000000 PyArweave-0.5.9/bundlr/node.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      450 2022-08-13 09:55:22.000000 PyArweave-0.5.9/makefile
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-08-18 10:55:55.530907 PyArweave-0.5.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1693 2022-08-18 10:55:05.000000 PyArweave-0.5.9/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.522907 PyArweave-0.5.9/test/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.526907 PyArweave-0.5.9/test/.vscode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      517 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/.vscode/launch.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   376522 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/Mining On The Arweave.pdf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   502030 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/data
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17431 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/package-lock.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/package.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1204 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/simple_http_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1076 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/simple_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test.pdf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1217 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test_block.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24701 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test_dataitem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test_jwk_file.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7765 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test_transaction.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1162 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2068 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/test_wallet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   613800 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/testfile0.bin
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1845 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/transactions.js
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test/transactions.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      645 2022-08-13 09:55:22.000000 PyArweave-0.5.9/test_upload_bundlr.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-18 10:55:55.530907 PyArweave-0.5.9/toys/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      187 2022-08-13 09:55:22.000000 PyArweave-0.5.9/toys/arweave-index.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2650 2022-08-13 09:55:22.000000 PyArweave-0.5.9/toys/bundlewatcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    49810 2022-08-13 09:55:22.000000 PyArweave-0.5.9/toys/indexer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5217 2022-08-13 09:55:22.000000 PyArweave-0.5.9/toys/tagswatcher.py
```

### Comparing `PyArweave-0.5.8/.github/ISSUE_TEMPLATE/bug_report.md` & `PyArweave-0.5.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/.gitignore` & `PyArweave-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/CHANGELOG.md` & `PyArweave-0.5.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/LICENSE` & `PyArweave-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/LICENSE_e142b89` & `PyArweave-0.5.9/LICENSE_e142b89`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/PKG-INFO` & `PyArweave-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyArweave
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tiny Arweave Library
 Home-page: https://github.com/xloem/pyarweave
 License: UNKNOWN
 Description: # PyArweave
         This is a small python client for arweave, based on https://github.com/MikeHibbert/arweave-python-client .
         
         I can struggle to code, so the hope is to keep this small and simple and ask the universe for more developers to take over maintainership.
```

### Comparing `PyArweave-0.5.8/PyArweave.egg-info/PKG-INFO` & `PyArweave-0.5.9/PyArweave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyArweave
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tiny Arweave Library
 Home-page: https://github.com/xloem/pyarweave
 License: UNKNOWN
 Description: # PyArweave
         This is a small python client for arweave, based on https://github.com/MikeHibbert/arweave-python-client .
         
         I can struggle to code, so the hope is to keep this small and simple and ask the universe for more developers to take over maintainership.
```

### Comparing `PyArweave-0.5.8/PyArweave.egg-info/SOURCES.txt` & `PyArweave-0.5.9/PyArweave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/README.md` & `PyArweave-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/__init__.py` & `PyArweave-0.5.9/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/ardrive.py` & `PyArweave-0.5.9/ar/ardrive.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/arweave_lib.py` & `PyArweave-0.5.9/ar/arweave_lib.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/block.py` & `PyArweave-0.5.9/ar/block.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/bundle.py` & `PyArweave-0.5.9/ar/bundle.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/chunk.py` & `PyArweave-0.5.9/ar/chunk.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/manifest.py` & `PyArweave-0.5.9/ar/manifest.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/multipeer.py` & `PyArweave-0.5.9/ar/multipeer.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/peer.py` & `PyArweave-0.5.9/ar/peer.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,20 @@
                 text = '' if response is None else response.text
                 status_code = 0 if response is None else response.status_code
                 if status_code == 429:
                     # too many requests
                     self._ratelimit_epilogue(False)
                     self.on_too_many_requests()
                     continue
-                logger.error('{}\n{}\n\n{}'.format(exc, text, request_kwparams))
+                if type(exc) is requests.ReadTimeout:
+                    if status_code == 0:
+                        status_code = 598
+                    logger.info('{}\n{}\n\n{}'.format(exc, text, request_kwparams))
+                else:
+                    logger.error('{}\n{}\n\n{}'.format(exc, text, request_kwparams))
                 if status_code == 520:
                     # cloudfront broke
                     self._ratelimit_epilogue(True)
                     continue
                 elif status_code == 502:
                     # cloudflare broke
                     self._ratelimit_epilogue(True)
@@ -1030,18 +1035,15 @@
 
         return response.content
 
     def stream(self, txid, range = None):
         try:
             return self.peer_stream(txid, range=range)
         except Exception:
-            if reupload(self, txid):
-                return self.gateway_stream(txid, range=range)
-            else:
-                raise
+            return reupload(self, txid, range=range) # now reupload would be changed to stream to a file and return a handle to that file that deletes it when closed. makes faster
 
     def gateway_stream(self, txid, ext ='', range = None):
         if range is not None:
             return GatewayStream.from_txid(self, txid, range[0], range[1] - range[0])
         else:
             return GatewayStream.from_txid(self, txid)
 
@@ -1133,34 +1135,46 @@
 
     def cache_jobs(self):
         response = self._get_json('cache', 'jobs')
         return response
 
 from ar.utils.merkle import compute_root_hash, generate_transaction_chunks
 from ar.utils import b64enc
-def reupload(peer, tx):
-    stream = peer.gateway_stream(tx)
+import tempfile, shutil
+def reupload(peer, tx, range=None):
+    stream = tempfile.SpooledTemporaryFile()
+    with peer.gateway_stream(tx) as network_data:
+        shutil.copyfileobj(network_data, stream)
 
+    stream.seek(0)
     chunks = generate_transaction_chunks(stream)
-    stream = peer.gateway_stream(tx)
     try:
         tx_data_root = peer.tx_data_root(tx)
+        logger.warning(f'uhh trying to reupload {tx}')
     except:
         from ar import Transaction
         tx_data_root = Transaction.frombytes(peer.unconfirmed_tx2(tx)).data_root
+        logger.info(f'{tx} not confirmed yet, got the data from gateway and am ensuring another node has it')
     if chunks['data_root'] != tx_data_root:
         logger.error(f'{peer.api_url}: Data for {tx} mismatches generated root.')
         return False
-    logger.warning(f'uhh trying to reupload {tx}')
     offset = 0
+    stream.seek(0)
     for proof, chunk in zip(chunks['proofs'], chunks['chunks']):
         chunk_size = chunk.data_size
         chunk = {
             'data_root': chunks['data_root'],
             'data_size': str(chunks['chunks'][-1].max_byte_range),
             'data_path': b64enc(proof.proof),
             'offset': str(proof.offset),
             'chunk': b64enc(stream.read(chunk_size))
         }
         peer.send_chunk(chunk)
         offset+=chunk_size
-    return True
+    stream.seek(0)
+    if range is not None:
+        ranged_stream = tempfile.SpooledTemporaryFile()
+        stream.seek(range[0])
+        ranged_stream.write(stream.read(range[1]-range[0]))
+        return ranged_stream
+    else:
+        return stream
```

### Comparing `PyArweave-0.5.8/ar/stream.py` & `PyArweave-0.5.9/ar/stream.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/transaction.py` & `PyArweave-0.5.9/ar/transaction.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/__init__.py` & `PyArweave-0.5.9/ar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/ans104_signers.py` & `PyArweave-0.5.9/ar/utils/ans104_signers.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/deep_hash.py` & `PyArweave-0.5.9/ar/utils/deep_hash.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/file_io.py` & `PyArweave-0.5.9/ar/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/merkle.py` & `PyArweave-0.5.9/ar/utils/merkle.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/serialization.py` & `PyArweave-0.5.9/ar/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/utils/transaction_uploader.py` & `PyArweave-0.5.9/ar/utils/transaction_uploader.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/ar/wallet.py` & `PyArweave-0.5.9/ar/wallet.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/bundlr/loader.py` & `PyArweave-0.5.9/bundlr/loader.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/bundlr/node.py` & `PyArweave-0.5.9/bundlr/node.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/setup.py` & `PyArweave-0.5.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # You should have received a copy of the GNU General Public License along with
 # PyArweave. If not, see <https://www.gnu.org/licenses/>.
 
 from setuptools import setup, find_packages
 
 setup(
   name='PyArweave',
-  version='0.5.8',
+  version='0.5.9',
   description='Tiny Arweave Library',
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/xloem/pyarweave',
   keywords=['arweave', 'crypto'],
   classifiers=[
     'Programming Language :: Python :: 3',
```

### Comparing `PyArweave-0.5.8/test/.vscode/launch.json` & `PyArweave-0.5.9/test/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/Mining On The Arweave.pdf` & `PyArweave-0.5.9/test/Mining On The Arweave.pdf`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/data` & `PyArweave-0.5.9/test/data`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/package-lock.json` & `PyArweave-0.5.9/test/package-lock.json`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/simple_http_server.py` & `PyArweave-0.5.9/test/simple_http_server.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/simple_server.py` & `PyArweave-0.5.9/test/simple_server.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/test_block.py` & `PyArweave-0.5.9/test/test_block.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/test_dataitem.py` & `PyArweave-0.5.9/test/test_dataitem.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/test_jwk_file.json` & `PyArweave-0.5.9/test/test_jwk_file.json`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/test_transaction.py` & `PyArweave-0.5.9/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/test_utils.py` & `PyArweave-0.5.9/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/test_wallet.py` & `PyArweave-0.5.9/test/test_wallet.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/testfile0.bin` & `PyArweave-0.5.9/test/testfile0.bin`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/transactions.js` & `PyArweave-0.5.9/test/transactions.js`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test/transactions.py` & `PyArweave-0.5.9/test/transactions.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/test_upload_bundlr.py` & `PyArweave-0.5.9/test_upload_bundlr.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/toys/bundlewatcher.py` & `PyArweave-0.5.9/toys/bundlewatcher.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/toys/indexer.py` & `PyArweave-0.5.9/toys/indexer.py`

 * *Files identical despite different names*

### Comparing `PyArweave-0.5.8/toys/tagswatcher.py` & `PyArweave-0.5.9/toys/tagswatcher.py`

 * *Files identical despite different names*

