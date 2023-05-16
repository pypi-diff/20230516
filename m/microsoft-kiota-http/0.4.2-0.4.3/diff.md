# Comparing `tmp/microsoft-kiota-http-0.4.2.tar.gz` & `tmp/microsoft_kiota_http-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-http-0.4.2.tar", last modified: Tue May  9 10:48:49 2023, max compression
+gzip compressed data, was "microsoft_kiota_http-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft-kiota-http-0.4.2.tar` & `microsoft_kiota_http-0.4.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      117 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1800 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.gitignore
--rw-r--r--   0        0        0    15946 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.pylintrc
--rw-r--r--   0        0        0     1002 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/LICENSE
--rw-r--r--   0        0        0      447 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/Pipfile
--rw-r--r--   0        0        0    39819 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/Pipfile.lock
--rw-r--r--   0        0        0     2376 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/README.md
--rw-r--r--   0        0        0     2757 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/SUPPORT.md
--rw-r--r--   0        0        0      121 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/kiota_http/__init__.py
--rw-r--r--   0        0        0       23 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/kiota_http/_version.py
--rw-r--r--   0        0        0    14620 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/kiota_http/httpx_request_adapter.py
--rw-r--r--   0        0        0     4823 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/kiota_client_factory.py
--rw-r--r--   0        0        0      276 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/__init__.py
--rw-r--r--   0        0        0      652 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/async_kiota_transport.py
--rw-r--r--   0        0        0     2011 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/middleware.py
--rw-r--r--   0        0        0      321 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/__init__.py
--rw-r--r--   0        0        0     1621 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
--rw-r--r--   0        0        0     2127 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/redirect_handler_option.py
--rw-r--r--   0        0        0      858 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/response_handler_option.py
--rw-r--r--   0        0        0     3067 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/retry_handler_option.py
--rw-r--r--   0        0        0      714 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/telemetry_handler_option.py
--rw-r--r--   0        0        0     2303 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     8479 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/redirect_handler.py
--rw-r--r--   0        0        0     8057 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/retry_handler.py
--rw-r--r--   0        0        0     1286 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1810 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     4636 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0      114 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/helpers/__init__.py
--rw-r--r--   0        0        0     4498 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/helpers/mock_response_object.py
--rw-r--r--   0        0        0      105 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/helpers/office_location.py
--rw-r--r--   0        0        0        0 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/__init__.py
--rw-r--r--   0        0        0      989 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/test_parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     2207 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/test_redirect_handler.py
--rw-r--r--   0        0        0     4324 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/test_retry_handler.py
--rw-r--r--   0        0        0    10291 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/test_httpx_request_adapter.py
--rw-r--r--   0        0        0     3277 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/test_kiota_client_factory.py
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft-kiota-http-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1800 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.gitignore
+-rw-r--r--   0        0        0    15946 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/.pylintrc
+-rw-r--r--   0        0        0     1108 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/LICENSE
+-rw-r--r--   0        0        0      447 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/Pipfile
+-rw-r--r--   0        0        0    39758 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/Pipfile.lock
+-rw-r--r--   0        0        0     2376 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/README.md
+-rw-r--r--   0        0        0     2757 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/SUPPORT.md
+-rw-r--r--   0        0        0      121 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/_version.py
+-rw-r--r--   0        0        0    14637 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/httpx_request_adapter.py
+-rw-r--r--   0        0        0     4823 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/kiota_client_factory.py
+-rw-r--r--   0        0        0      276 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/__init__.py
+-rw-r--r--   0        0        0      652 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/async_kiota_transport.py
+-rw-r--r--   0        0        0     2011 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/middleware.py
+-rw-r--r--   0        0        0      321 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/__init__.py
+-rw-r--r--   0        0        0     1621 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
+-rw-r--r--   0        0        0     2127 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/redirect_handler_option.py
+-rw-r--r--   0        0        0      858 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/response_handler_option.py
+-rw-r--r--   0        0        0     3067 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/retry_handler_option.py
+-rw-r--r--   0        0        0      714 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/options/telemetry_handler_option.py
+-rw-r--r--   0        0        0     2303 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     8588 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/redirect_handler.py
+-rw-r--r--   0        0        0     8057 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/kiota_http/middleware/retry_handler.py
+-rw-r--r--   0        0        0     1286 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1844 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     4882 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0      114 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     4498 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/helpers/mock_response_object.py
+-rw-r--r--   0        0        0      105 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/helpers/office_location.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/__init__.py
+-rw-r--r--   0        0        0      989 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/test_parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     2207 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/test_redirect_handler.py
+-rw-r--r--   0        0        0     4324 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/middleware_tests/test_retry_handler.py
+-rw-r--r--   0        0        0    10952 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/test_httpx_request_adapter.py
+-rw-r--r--   0        0        0     3277 2023-05-16 13:41:11.691110 microsoft_kiota_http-0.4.3/tests/test_kiota_client_factory.py
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft_kiota_http-0.4.3/PKG-INFO
```

### Comparing `microsoft-kiota-http-0.4.2/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_http-0.4.3/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/.github/workflows/build_publish.yml` & `microsoft_kiota_http-0.4.3/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_http-0.4.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_http-0.4.3/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/.gitignore` & `microsoft_kiota_http-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/.pylintrc` & `microsoft_kiota_http-0.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/CHANGELOG.md` & `microsoft_kiota_http-0.4.3/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.3] - 2023-05-16
+
+### Added
+
+### Changed
+
+- Fixes bug in getting content from redirected request.
+
 ## [0.4.2] - 2023-05-02
 
 ### Added
 
 ### Changed
 
 - Includes Response headers in APIException for failed requests.
```

### Comparing `microsoft-kiota-http-0.4.2/LICENSE` & `microsoft_kiota_http-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/Pipfile.lock` & `microsoft_kiota_http-0.4.3/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9786348848848849%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'6d136825ef6a93a33d54d28e58d6ea6fa46b6321fe7578dba9b2a87efb19def4'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}}",*

 * * "'develop'": "{'astroid': {'hashes': "*

 * *              "['sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "9168d36e511d3e76f3df5bdd3f2f496a5d8ce2a88baa0ce9206514aacae0538d"
+            "sha256": "6d136825ef6a93a33d54d28e58d6ea6fa46b6321fe7578dba9b2a87efb19def4"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -20,19 +20,19 @@
                 "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"
             ],
             "markers": "python_full_version >= '3.6.2'",
             "version": "==3.6.2"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "h11": {
             "hashes": [
                 "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d",
                 "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"
             ],
             "markers": "python_version >= '3.7'",
@@ -112,35 +112,35 @@
             "markers": "python_version >= '3.6'",
             "version": "==4.1.1"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
-                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.4"
+            "version": "==2.15.5"
         },
         "asyncmock": {
             "hashes": [
                 "sha256:c251889d542e98fe5f7ece2b5b8643b7d62b50a5657d34a4cbce8a1d5170d750",
                 "sha256:fd8bc4e7813251a8959d1140924ccba3adbbc7af885dba7047c67f73c0b664b1"
             ],
             "index": "pypi",
             "version": "==0.4.2"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
@@ -293,43 +293,43 @@
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
+                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "flit": {
             "hashes": [
-                "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
-                "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
+                "sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca",
+                "sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7"
             ],
             "index": "pypi",
-            "version": "==3.8.0"
+            "version": "==3.9.0"
         },
         "flit-core": {
             "hashes": [
-                "sha256:64a29ec845164a6abe1136bf4bc5ae012bdfe758ed42fc7571a9059a7c80bd83",
-                "sha256:b305b30c99526df5e63d6022dd2310a0a941a187bd3884f4c8ef0418df6c39f3"
+                "sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba",
+                "sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==3.8.0"
+            "version": "==3.9.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -407,43 +407,43 @@
                 "sha256:0e0bc5ba78b8db3667ad636d964eb963dc97a59f04c6f6214c5f0e4a8f726c56"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==5.0.2"
         },
         "mypy": {
             "hashes": [
-                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
-                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
-                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
-                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
-                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
-                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
-                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
-                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
-                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
-                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
-                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
-                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
-                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
-                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
-                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
-                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
-                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
-                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
-                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
-                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
-                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
-                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
-                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
-                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
-                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
-                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
+                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
+                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
+                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
+                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
+                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
+                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
+                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
+                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
+                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
+                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
+                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
+                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
+                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
+                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
+                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
+                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
+                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
+                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
+                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
+                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
+                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
+                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
+                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
+                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
+                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
+                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.3.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -455,35 +455,35 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:761907349e699f8afdcd56c4fe02f3021ab5b3a0fc26d19a9bfdc66c7d0d5cd5",
-                "sha256:a6cbb4c6e96eab4a3c7de7c6383c512478f58f88d95764507d84c899d656a89a"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "index": "pypi",
-            "version": "==2.17.3"
+            "version": "==2.17.4"
         },
         "pytest": {
             "hashes": [
                 "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
                 "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
@@ -511,19 +511,19 @@
                 "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
             ],
             "index": "pypi",
             "version": "==3.10.0"
         },
         "requests": {
             "hashes": [
-                "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b",
-                "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.29.0"
+            "version": "==2.30.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
@@ -551,35 +551,35 @@
                 "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.8"
         },
         "types-python-dateutil": {
             "hashes": [
-                "sha256:355b2cb82b31e556fd18e7b074de7c350c680ab80608f0cc55ba6770d986d67d",
-                "sha256:fe5b545e678ec13e3ddc83a0eee1545c1b5e2fba4cfc39b276ab6f4e7604a923"
+                "sha256:09a0275f95ee31ce68196710ed2c3d1b9dc42e0b61cc43acc369a42cb939134f",
+                "sha256:0b0e7c68e7043b0354b26a1e0225cb1baea7abb1b324d02b50e2d08f1221043f"
             ],
             "index": "pypi",
-            "version": "==2.8.19.12"
+            "version": "==2.8.19.13"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
```

### Comparing `microsoft-kiota-http-0.4.2/README.md` & `microsoft_kiota_http-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/SECURITY.md` & `microsoft_kiota_http-0.4.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/SUPPORT.md` & `microsoft_kiota_http-0.4.3/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/httpx_request_adapter.py` & `microsoft_kiota_http-0.4.3/kiota_http/httpx_request_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional, TypeVar
+from typing import Any, Dict, List, Optional, TypeVar, Union
 
 import httpx
 from kiota_abstractions.api_client_builder import (
     enable_backing_store_for_parse_node_factory,
     enable_backing_store_for_serialization_writer_factory,
 )
 from kiota_abstractions.api_error import APIError
@@ -20,15 +20,15 @@
     SerializationWriterFactoryRegistry,
 )
 from kiota_abstractions.store import BackingStoreFactory, BackingStoreFactorySingleton
 
 from .kiota_client_factory import KiotaClientFactory
 from .middleware.options import ResponseHandlerOption
 
-ResponseType = TypeVar("ResponseType", str, int, float, bool, datetime, bytes)
+ResponseType = Union[str, int, float, bool, datetime, bytes]
 ModelType = TypeVar("ModelType", bound=Parsable)
 
 
 class HttpxRequestAdapter(RequestAdapter):
 
     def __init__(
         self,
@@ -95,15 +95,16 @@
         self, request_info: RequestInformation, model_type: ParsableFactory,
         error_map: Dict[str, ParsableFactory]
     ) -> Optional[ModelType]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model.
         Args:
             request_info (RequestInformation): the request info to execute.
-            type (ParsableFactory): the class of the response model to deserialize the response into
+            model_type (ParsableFactory): the class of the response model 
+            to deserialize the response into.
             error_map (Dict[str, ParsableFactory]): the error dict to use in
             case of a failed request.
 
         Returns:
             ModelType: the deserialized response model.
         """
         if not request_info:
@@ -126,15 +127,16 @@
         self, request_info: RequestInformation, model_type: ParsableFactory,
         error_map: Dict[str, ParsableFactory]
     ) -> Optional[List[ModelType]]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model collection.
         Args:
             request_info (RequestInformation): the request info to execute.
-            type (ParsableFactory): the class of the response model to deserialize the response into
+            model_type (ParsableFactory): the class of the response model
+            to deserialize the response into.
             error_map (Dict[str, ParsableFactory]): the error dict to use in
             case of a failed request.
 
         Returns:
             ModelType: the deserialized response model collection.
         """
         if not request_info:
@@ -156,16 +158,16 @@
         self, request_info: RequestInformation, response_type: ResponseType,
         error_map: Dict[str, ParsableFactory]
     ) -> Optional[List[ResponseType]]:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized response model collection.
         Args:
             request_info (RequestInformation): the request info to execute.
-            response_type (ResponseType): the class of the response model to deserialize the
-            response into.
+            response_type (ResponseType): the class of the response model
+            to deserialize the response into.
             error_map (Dict[str, ParsableFactory]): the error dict to use in
             case of a failed request.
 
         Returns:
             Optional[List[ModelType]]: he deserialized response model collection.
         """
         if not request_info:
@@ -207,27 +209,27 @@
         response_handler = self.get_response_handler(request_info)
         if response_handler:
             return await response_handler.handle_response_async(response, error_map)
 
         await self.throw_failed_responses(response, error_map)
         if self._should_return_none(response):
             return None
+        if response_type == "bytes":
+            return response.content
         root_node = await self.get_root_parse_node(response)
         if response_type == "str":
             return root_node.get_str_value()
         if response_type == "int":
             return root_node.get_int_value()
         if response_type == "float":
             return root_node.get_float_value()
         if response_type == "bool":
             return root_node.get_bool_value()
         if response_type == "datetime":
             return root_node.get_datetime_value()
-        if response_type == "bytes":
-            return root_node.get_bytes_value()
         raise Exception("Found unexpected type to deserialize")
 
     async def send_no_response_content_async(
         self, request_info: RequestInformation, error_map: Dict[str, ParsableFactory]
     ) -> None:
         """Excutes the HTTP request specified by the given RequestInformation and returns the
         deserialized primitive response model.
```

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/kiota_client_factory.py` & `microsoft_kiota_http-0.4.3/kiota_http/kiota_client_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/async_kiota_transport.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/async_kiota_transport.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/middleware.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/parameters_name_decoding_handler_option.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/parameters_name_decoding_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/redirect_handler_option.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/redirect_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/response_handler_option.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/response_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/retry_handler_option.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/retry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/telemetry_handler_option.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/options/telemetry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/parameters_name_decoding_handler.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/redirect_handler.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/redirect_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,16 @@
         new_request = httpx.Request(
             method=method,
             url=url,
             headers=headers,
             stream=stream,
             extensions=request.extensions,
         )
+        new_request.context = request.context  #type: ignore
+        new_request.options = {}  #type: ignore
         return new_request
 
     def _redirect_method(self, request: httpx.Request, response: httpx.Response) -> str:
         """
         When being redirected we may want to change the method of the request
         based on certain specs or browser behavior.
         """
```

### Comparing `microsoft-kiota-http-0.4.2/kiota_http/middleware/retry_handler.py` & `microsoft_kiota_http-0.4.3/kiota_http/middleware/retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/pyproject.toml` & `microsoft_kiota_http-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/requirements-dev.txt` & `microsoft_kiota_http-0.4.3/requirements-dev.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 -i https://pypi.org/simple
 
-astroid==2.15.4 ; python_full_version >= '3.7.2'
+astroid==2.15.5 ; python_full_version >= '3.7.2'
 
 asyncmock==0.4.2
 
-certifi==2022.12.7 ; python_version >= '3.6'
+certifi==2023.5.7 ; python_version >= '3.6'
 
 charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
 
 colorama==0.4.6 ; sys_platform == 'win32'
 
 coverage[toml]==7.2.5 ; python_version >= '3.7'
 
 dill==0.3.6 ; python_version < '3.11'
 
-docutils==0.19 ; python_version >= '3.7'
+docutils==0.20 ; python_version >= '3.7'
 
 exceptiongroup==1.1.1 ; python_version < '3.11'
 
 flit==3.8.0
 
-flit-core==3.8.0 ; python_version >= '3.6'
+flit-core==3.9.0 ; python_version >= '3.6'
 
 idna==3.4 ; python_version >= '3.5'
 
 iniconfig==2.0.0 ; python_version >= '3.7'
 
 isort==5.12.0
 
 lazy-object-proxy==1.9.0 ; python_version >= '3.7'
 
 mccabe==0.7.0 ; python_version >= '3.6'
 
 mock==5.0.2 ; python_version >= '3.6'
 
-mypy==1.2.0
+mypy==1.3.0
 
 mypy-extensions==1.0.0 ; python_version >= '3.5'
 
 packaging==23.1 ; python_version >= '3.7'
 
-platformdirs==3.5.0 ; python_version >= '3.7'
+platformdirs==3.5.1 ; python_version >= '3.7'
 
 pluggy==1.0.0 ; python_version >= '3.6'
 
-pylint==2.17.3
+pylint==2.17.4
 
 pytest==7.3.1
 
 pytest-asyncio==0.21.0
 
 pytest-cov==4.0.0
 
 pytest-mock==3.10.0
 
-requests==2.29.0 ; python_version >= '3.7'
+requests==2.30.0 ; python_version >= '3.7'
 
 toml==0.10.2
 
 tomli==2.0.1 ; python_version < '3.11'
 
 tomli-w==1.0.0 ; python_version >= '3.7'
 
 tomlkit==0.11.8 ; python_version >= '3.7'
 
-types-python-dateutil==2.8.19.12
+types-python-dateutil==2.8.19.13
 
 typing-extensions==4.5.0 ; python_version >= '3.7'
 
-urllib3==1.26.15 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+urllib3==2.0.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 
 wrapt==1.15.0 ; python_version < '3.11'
 
 yapf==0.33.0
 
 anyio==3.6.2 ; python_full_version >= '3.6.2'
 
@@ -84,13 +84,15 @@
 
 httpcore==0.17.0 ; python_version >= '3.7'
 
 httpx[http2]==0.24.0
 
 hyperframe==6.0.1 ; python_full_version >= '3.6.1'
 
+idna==3.4 ; python_version >= '3.5'
+
 microsoft-kiota-abstractions==0.5.1
 
 sniffio==1.3.0 ; python_version >= '3.7'
 
 uritemplate==4.1.1 ; python_version >= '3.6'
```

### Comparing `microsoft-kiota-http-0.4.2/tests/conftest.py` & `microsoft_kiota_http-0.4.3/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,11 +163,19 @@
     return resp
 
 
 @pytest.fixture
 def mock_primitive_response(mocker):
     return httpx.Response(200, json=22.3, headers={"Content-Type": "application/json"})
 
+@pytest.fixture
+def mock_primitive_response_bytes(mocker):
+    return httpx.Response(
+        200,
+        content=b'Hello World',
+        headers={"Content-Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document"}
+    )
+
 
 @pytest.fixture
 def mock_no_content_response(mocker):
     return httpx.Response(204, json="Radom JSON", headers={"Content-Type": "application/json"})
```

### Comparing `microsoft-kiota-http-0.4.2/tests/helpers/mock_response_object.py` & `microsoft_kiota_http-0.4.3/tests/helpers/mock_response_object.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/tests/middleware_tests/test_parameters_name_decoding_handler.py` & `microsoft_kiota_http-0.4.3/tests/middleware_tests/test_parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/tests/middleware_tests/test_redirect_handler.py` & `microsoft_kiota_http-0.4.3/tests/middleware_tests/test_redirect_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/tests/middleware_tests/test_retry_handler.py` & `microsoft_kiota_http-0.4.3/tests/middleware_tests/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/tests/test_httpx_request_adapter.py` & `microsoft_kiota_http-0.4.3/tests/test_httpx_request_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,25 @@
 ):
     request_adapter.get_http_response_message = AsyncMock(return_value=mock_primitive_response)
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_primitive)
     resp = await request_adapter.get_http_response_message(request_info)
     assert resp.headers.get("content-type") == 'application/json'
     final_result = await request_adapter.send_primitive_async(request_info, "float", {})
     assert final_result == 22.3
+    
+@pytest.mark.asyncio
+async def test_send_primitive_async_bytes(
+    request_adapter, request_info, mock_primitive_response_bytes, mock_primitive
+):
+    request_adapter.get_http_response_message = AsyncMock(return_value=mock_primitive_response_bytes)
+    request_adapter.get_root_parse_node = AsyncMock(return_value=mock_primitive)
+    resp = await request_adapter.get_http_response_message(request_info)
+    assert resp.headers.get("content-type") == 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'
+    final_result = await request_adapter.send_primitive_async(request_info, "bytes", {})
+    assert final_result == b'Hello World'
 
 
 @pytest.mark.asyncio
 async def test_send_primitive_async_no_content(
     request_adapter, request_info, mock_no_content_response
 ):
     request_adapter.get_http_response_message = AsyncMock(return_value=mock_no_content_response)
```

### Comparing `microsoft-kiota-http-0.4.2/tests/test_kiota_client_factory.py` & `microsoft_kiota_http-0.4.3/tests/test_kiota_client_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.2/PKG-INFO` & `microsoft_kiota_http-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-http
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kiota http request adapter implementation for httpx library
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

