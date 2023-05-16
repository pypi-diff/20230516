# Comparing `tmp/mathtranslate-2.2.1.tar.gz` & `tmp/mathtranslate-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.2.1.tar", last modified: Mon May 15 07:47:38 2023, max compression
+gzip compressed data, was "mathtranslate-2.2.2.tar", last modified: Tue May 16 03:56:35 2023, max compression
```

## Comparing `mathtranslate-2.2.1.tar` & `mathtranslate-2.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.187955 mathtranslate-2.2.1/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.187955 mathtranslate-2.2.1/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:47:38.187955 mathtranslate-2.2.1/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-15 07:47:38.000000 mathtranslate-2.2.1/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-15 07:47:38.000000 mathtranslate-2.2.1/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:47:38.000000 mathtranslate-2.2.1/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 07:47:38.000000 mathtranslate-2.2.1/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 07:47:38.000000 mathtranslate-2.2.1/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 07:47:38.000000 mathtranslate-2.2.1/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:47:38.191955 mathtranslate-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-15 07:47:17.000000 mathtranslate-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.843904 mathtranslate-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-16 03:56:35.843904 mathtranslate-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.839904 mathtranslate-2.2.2/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.839904 mathtranslate-2.2.2/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.839904 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.839904 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.839904 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.843904 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.843904 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.843904 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:56:35.839904 mathtranslate-2.2.2/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-16 03:56:35.000000 mathtranslate-2.2.2/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-16 03:56:35.000000 mathtranslate-2.2.2/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:56:35.000000 mathtranslate-2.2.2/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-16 03:56:35.000000 mathtranslate-2.2.2/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 03:56:35.000000 mathtranslate-2.2.2/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 03:56:35.000000 mathtranslate-2.2.2/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 03:56:35.843904 mathtranslate-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-16 03:56:16.000000 mathtranslate-2.2.2/setup.py
```

### Comparing `mathtranslate-2.2.1/LICENSE` & `mathtranslate-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/PKG-INFO` & `mathtranslate-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.2.1
+Version: 2.2.2
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -83,7 +83,13 @@
 2. There is a small probability to get something like "XMATHX_1_2" or wrong formula during translation. The accuracy rate of Tencent translation is slightly lower than that of Google translation.
 
 ## Further developments
 1. Fix bugs in the latex translations.
 2. A more user-friendly interface.
 
 If you have any questions or have interests in making contributions, please contact me by susyustc@gmail.com or joining QQ group 288646946.
+
+## Donation
+If you think this project is helping you a lot, you can support us by the Wechat QR code below
+<p align="center">
+  <img width=30% src="https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-82ad-bbcbdad1c19d">
+</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.1 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.2 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
@@ -63,8 +63,11 @@
 Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
 will not be translated correctly. 2. There is a small probability to get
 something like "XMATHX_1_2" or wrong formula during translation. The accuracy
 rate of Tencent translation is slightly lower than that of Google translation.
 ## Further developments 1. Fix bugs in the latex translations. 2. A more user-
 friendly interface. If you have any questions or have interests in making
 contributions, please contact me by susyustc@gmail.com or joining QQ group
-288646946.
+288646946. ## Donation If you think this project is helping you a lot, you can
+support us by the Wechat QR code below
+[https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-
+                              82ad-bbcbdad1c19d]
```

### Comparing `mathtranslate-2.2.1/README.md` & `mathtranslate-2.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,7 +71,13 @@
 2. There is a small probability to get something like "XMATHX_1_2" or wrong formula during translation. The accuracy rate of Tencent translation is slightly lower than that of Google translation.
 
 ## Further developments
 1. Fix bugs in the latex translations.
 2. A more user-friendly interface.
 
 If you have any questions or have interests in making contributions, please contact me by susyustc@gmail.com or joining QQ group 288646946.
+
+## Donation
+If you think this project is helping you a lot, you can support us by the Wechat QR code below
+<p align="center">
+  <img width=30% src="https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-82ad-bbcbdad1c19d">
+</p>
```

#### html2text {}

```diff
@@ -58,8 +58,11 @@
 Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
 will not be translated correctly. 2. There is a small probability to get
 something like "XMATHX_1_2" or wrong formula during translation. The accuracy
 rate of Tencent translation is slightly lower than that of Google translation.
 ## Further developments 1. Fix bugs in the latex translations. 2. A more user-
 friendly interface. If you have any questions or have interests in making
 contributions, please contact me by susyustc@gmail.com or joining QQ group
-288646946.
+288646946. ## Donation If you think this project is helping you a lot, you can
+support us by the Wechat QR code below
+[https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-
+                              82ad-bbcbdad1c19d]
```

### Comparing `mathtranslate-2.2.1/mathtranslate/config.py` & `mathtranslate-2.2.2/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/encoding.py` & `mathtranslate-2.2.2/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/process_file.py` & `mathtranslate-2.2.2/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/process_latex.py` & `mathtranslate-2.2.2/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/process_text.py` & `mathtranslate-2.2.2/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencent.py` & `mathtranslate-2.2.2/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.2.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/translate.py` & `mathtranslate-2.2.2/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/translate_arxiv.py` & `mathtranslate-2.2.2/mathtranslate/translate_arxiv.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import gzip
 import zipfile
 import tarfile
 import tempfile
 import urllib.request
 
 
-def download_source(number):
+def download_source(number, path):
     url = f'https://arxiv.org/e-print/{number}'
-    urllib.request.urlretrieve(url, number)
+    print('trying to download from', url)
+    urllib.request.urlretrieve(url, path)
 
 
 def is_pdf(filename):
     return open(filename, 'rb').readline()[0:4] == b'%PDF'
 
 
 def loop_files(dir):
@@ -101,50 +102,48 @@
     utils.process_options(options)
 
     if options.number is None:
         parser.print_help()
         sys.exit()
 
     number = options.number
+    print('arxiv number:', number)
+    print()
+    download_path = number.replace('/', '-')
     if options.o is None:
-        output_path = f'{number}.zip'
+        output_path = f'{download_path}.zip'
     else:
         output_path = options.o
-    print('arxiv number:', number)
-    print()
 
     success = True
     cwd = os.getcwd()
     with tempfile.TemporaryDirectory() as temp_dir:
         print('temporary directory', temp_dir)
         os.chdir(temp_dir)
         try:
-            download_source(number)
-        except urllib.error.HTTPError:
-            print(f'Specified arxiv {number} not found')
-            return False
+            download_source(number, download_path)
         except BaseException:
-            print('Cannot download source, maybe network issue')
+            print('Cannot download source, maybe network issue or wrong link')
             return False
-        if is_pdf(number):
+        if is_pdf(download_path):
             # case 1
             success = False
         else:
-            content = gzip.decompress(open(number, "rb").read())
-            with open(number, "wb") as f:
+            content = gzip.decompress(open(download_path, "rb").read())
+            with open(download_path, "wb") as f:
                 f.write(content)
             try:
                 # case 4
-                with tarfile.open(number, mode='r') as f:
+                with tarfile.open(download_path, mode='r') as f:
                     f.extractall()
-                os.remove(number)
+                os.remove(download_path)
             except tarfile.ReadError:
                 # case 2 or 3
                 print('This is a pure text file')
-                shutil.move(number, 'main.tex')
+                shutil.move(download_path, 'main.tex')
             success = translate_dir('.', options)
             if success:
                 # case 3
                 os.chdir(cwd)
                 zipdir(temp_dir, output_path)
 
     if success:
```

### Comparing `mathtranslate-2.2.1/mathtranslate/translate_tex.py` & `mathtranslate-2.2.2/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/upload_overleaf.py` & `mathtranslate-2.2.2/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate/utils.py` & `mathtranslate-2.2.2/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.2.2/mathtranslate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.2.1
+Version: 2.2.2
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -83,7 +83,13 @@
 2. There is a small probability to get something like "XMATHX_1_2" or wrong formula during translation. The accuracy rate of Tencent translation is slightly lower than that of Google translation.
 
 ## Further developments
 1. Fix bugs in the latex translations.
 2. A more user-friendly interface.
 
 If you have any questions or have interests in making contributions, please contact me by susyustc@gmail.com or joining QQ group 288646946.
+
+## Donation
+If you think this project is helping you a lot, you can support us by the Wechat QR code below
+<p align="center">
+  <img width=30% src="https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-82ad-bbcbdad1c19d">
+</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.1 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.2.2 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
@@ -63,8 +63,11 @@
 Issues 1. If `\begin{env} \end{env}` is reset with `\newcommand` in latex, it
 will not be translated correctly. 2. There is a small probability to get
 something like "XMATHX_1_2" or wrong formula during translation. The accuracy
 rate of Tencent translation is slightly lower than that of Google translation.
 ## Further developments 1. Fix bugs in the latex translations. 2. A more user-
 friendly interface. If you have any questions or have interests in making
 contributions, please contact me by susyustc@gmail.com or joining QQ group
-288646946.
+288646946. ## Donation If you think this project is helping you a lot, you can
+support us by the Wechat QR code below
+[https://github.com/SUSYUSTC/MathTranslate/assets/30529122/16f82637-e102-4330-
+                              82ad-bbcbdad1c19d]
```

### Comparing `mathtranslate-2.2.1/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.2.2/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.2.1/setup.py` & `mathtranslate-2.2.2/setup.py`

 * *Files identical despite different names*

