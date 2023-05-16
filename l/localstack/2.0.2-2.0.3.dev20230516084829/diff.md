# Comparing `tmp/localstack-2.0.2.tar.gz` & `tmp/localstack-2.0.3.dev20230516084829.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-2.0.2.tar", last modified: Mon Apr 17 14:30:13 2023, max compression
+gzip compressed data, was "localstack-2.0.3.dev20230516084829.tar", last modified: Tue May 16 08:52:00 2023, max compression
```

## Comparing `localstack-2.0.2.tar` & `localstack-2.0.3.dev20230516084829.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-17 14:30:13.878814 localstack-2.0.2/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11400 2023-04-17 14:30:13.878814 localstack-2.0.2/PKG-INFO
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-17 14:30:13.878814 localstack-2.0.2/localstack.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)    11400 2023-04-17 14:30:13.000000 localstack-2.0.2/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-04-17 14:30:13.000000 localstack-2.0.2/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-17 14:30:13.000000 localstack-2.0.2/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      169 2023-04-17 14:30:13.000000 localstack-2.0.2/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-04-17 14:30:13.000000 localstack-2.0.2/localstack.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-17 14:30:13.878814 localstack-2.0.2/localstack_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)       50 2023-04-17 14:30:13.000000 localstack-2.0.2/localstack_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-17 14:30:13.878814 localstack-2.0.2/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-04-17 14:26:37.000000 localstack-2.0.2/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-16 08:52:00.126552 localstack-2.0.3.dev20230516084829/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11418 2023-05-16 08:52:00.126552 localstack-2.0.3.dev20230516084829/PKG-INFO
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-16 08:52:00.126552 localstack-2.0.3.dev20230516084829/localstack.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    11418 2023-05-16 08:52:00.000000 localstack-2.0.3.dev20230516084829/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-05-16 08:52:00.000000 localstack-2.0.3.dev20230516084829/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-05-16 08:52:00.000000 localstack-2.0.3.dev20230516084829/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-05-16 08:52:00.000000 localstack-2.0.3.dev20230516084829/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-05-16 08:52:00.000000 localstack-2.0.3.dev20230516084829/localstack.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-16 08:52:00.126552 localstack-2.0.3.dev20230516084829/localstack_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-05-16 08:51:59.000000 localstack-2.0.3.dev20230516084829/localstack_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-05-16 08:52:00.126552 localstack-2.0.3.dev20230516084829/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-05-16 08:48:17.000000 localstack-2.0.3.dev20230516084829/setup.py
```

### Comparing `localstack-2.0.2/PKG-INFO` & `localstack-2.0.3.dev20230516084829/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.0.2
+Version: 2.0.3.dev20230516084829
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.0.2 Summary: LocalStack - A
-fully functional local Cloud stack Home-page: https://github.com/localstack/
-localstack Author: LocalStack Contributors Author-email: info@localstack.cloud
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Emulators Description-Content-Type: text/
-markdown Provides-Extra: runtime Provides-Extra: full
+Metadata-Version: 2.1 Name: localstack Version: 2.0.3.dev20230516084829
+Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
+github.com/localstack/localstack Author: LocalStack Contributors Author-email:
+info@localstack.cloud License: Apache License 2.0 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Testing Classifier: Topic :: System :: Emulators Description-
+Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
   :zap: We are thrilled to announce LocalStack_2.0 which brings new features,
                         enhancements and bugfixes :zap:
               [LocalStack - A fully functional local cloud stack]
  [CircleCI] [Coverage_Status] [PyPI_Version] [Docker_Pulls] [PyPi_downloads]
 [Backers_on_Open_Collective] [Sponsors_on_Open_Collective] [PyPI_License] [Code
                             style:_black] [Twitter]
 LocalStack provides an easy-to-use test/mocking framework for developing cloud
```

### Comparing `localstack-2.0.2/localstack.egg-info/PKG-INFO` & `localstack-2.0.3.dev20230516084829/localstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.0.2
+Version: 2.0.3.dev20230516084829
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.0.2 Summary: LocalStack - A
-fully functional local Cloud stack Home-page: https://github.com/localstack/
-localstack Author: LocalStack Contributors Author-email: info@localstack.cloud
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Emulators Description-Content-Type: text/
-markdown Provides-Extra: runtime Provides-Extra: full
+Metadata-Version: 2.1 Name: localstack Version: 2.0.3.dev20230516084829
+Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
+github.com/localstack/localstack Author: LocalStack Contributors Author-email:
+info@localstack.cloud License: Apache License 2.0 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Testing Classifier: Topic :: System :: Emulators Description-
+Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
   :zap: We are thrilled to announce LocalStack_2.0 which brings new features,
                         enhancements and bugfixes :zap:
               [LocalStack - A fully functional local cloud stack]
  [CircleCI] [Coverage_Status] [PyPI_Version] [Docker_Pulls] [PyPi_downloads]
 [Backers_on_Open_Collective] [Sponsors_on_Open_Collective] [PyPI_License] [Code
                             style:_black] [Twitter]
 LocalStack provides an easy-to-use test/mocking framework for developing cloud
```

### Comparing `localstack-2.0.2/setup.py` & `localstack-2.0.3.dev20230516084829/setup.py`

 * *Files identical despite different names*

