# Comparing `tmp/ghostbusterV4-1.0.7.tar.gz` & `tmp/ghostbusterV4-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghostbusterV4-1.0.7.tar", last modified: Wed Mar 22 08:30:28 2023, max compression
+gzip compressed data, was "ghostbusterV4-1.0.8.tar", last modified: Tue May 16 13:33:09 2023, max compression
```

## Comparing `ghostbusterV4-1.0.7.tar` & `ghostbusterV4-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-03-22 08:30:28.118524 ghostbusterV4-1.0.7/
--rw-r--r--   0 pbaid.int (199922920) staff       (20)    34519 2023-03-22 07:00:06.000000 ghostbusterV4-1.0.7/LICENSE
--rw-r--r--   0 pbaid.int (199922920) staff       (20)        1 2023-03-22 07:00:06.000000 ghostbusterV4-1.0.7/MANIFEST.in
--rw-r--r--   0 pbaid.int (199922920) staff       (20)    16153 2023-03-22 08:30:28.118761 ghostbusterV4-1.0.7/PKG-INFO
--rw-r--r--   0 pbaid.int (199922920) staff       (20)    15415 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/README.rst
-drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-03-22 08:30:28.104139 ghostbusterV4-1.0.7/ghostbusterV4/
--rw-r--r--   0 pbaid.int (199922920) staff       (20)      766 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/ghostbusterV4/__init__.py
--rw-r--r--   0 pbaid.int (199922920) staff       (20)     2212 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/ghostbusterV4/cli.py
--rw-r--r--   0 pbaid.int (199922920) staff       (20)    27256 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/ghostbusterV4/scan.py
--rw-r--r--   0 pbaid.int (199922920) staff       (20)      292 2023-03-22 08:29:01.000000 ghostbusterV4-1.0.7/ghostbusterV4/version.py
-drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-03-22 08:30:28.108257 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/
--rw-r--r--   0 pbaid.int (199922920) staff       (20)    16153 2023-03-22 08:30:27.000000 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/PKG-INFO
--rw-r--r--   0 pbaid.int (199922920) staff       (20)      422 2023-03-22 08:30:27.000000 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/SOURCES.txt
--rw-r--r--   0 pbaid.int (199922920) staff       (20)        1 2023-03-22 08:30:27.000000 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/dependency_links.txt
--rw-r--r--   0 pbaid.int (199922920) staff       (20)       56 2023-03-22 08:30:27.000000 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/entry_points.txt
--rw-r--r--   0 pbaid.int (199922920) staff       (20)       57 2023-03-22 08:30:27.000000 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/requires.txt
--rw-r--r--   0 pbaid.int (199922920) staff       (20)       14 2023-03-22 08:30:27.000000 ghostbusterV4-1.0.7/ghostbusterV4.egg-info/top_level.txt
--rw-r--r--   0 pbaid.int (199922920) staff       (20)       84 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/pyproject.toml
--rw-r--r--   0 pbaid.int (199922920) staff       (20)       76 2023-03-22 08:30:28.130264 ghostbusterV4-1.0.7/setup.cfg
--rw-r--r--   0 pbaid.int (199922920) staff       (20)     2980 2023-03-22 07:19:19.000000 ghostbusterV4-1.0.7/setup.py
-drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-03-22 08:30:28.117919 ghostbusterV4-1.0.7/tests/
--rw-r--r--   0 pbaid.int (199922920) staff       (20)     1209 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/tests/test_cli.py
--rw-r--r--   0 pbaid.int (199922920) staff       (20)     1706 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.7/tests/test_example.py
+drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-05-16 13:33:09.398343 ghostbusterV4-1.0.8/
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)    34519 2023-03-22 07:00:06.000000 ghostbusterV4-1.0.8/LICENSE
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)        1 2023-03-22 07:00:06.000000 ghostbusterV4-1.0.8/MANIFEST.in
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)    16153 2023-05-16 13:33:09.398524 ghostbusterV4-1.0.8/PKG-INFO
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)    15415 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/README.rst
+drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-05-16 13:33:09.369383 ghostbusterV4-1.0.8/ghostbusterV4/
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)      766 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/ghostbusterV4/__init__.py
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)     2212 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/ghostbusterV4/cli.py
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)    27256 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/ghostbusterV4/scan.py
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)      292 2023-05-16 12:26:13.000000 ghostbusterV4-1.0.8/ghostbusterV4/version.py
+drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-05-16 13:33:09.381679 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)    16153 2023-05-16 13:33:09.000000 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/PKG-INFO
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)      422 2023-05-16 13:33:09.000000 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/SOURCES.txt
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)        1 2023-05-16 13:33:09.000000 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/dependency_links.txt
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)       56 2023-05-16 13:33:09.000000 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/entry_points.txt
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)       84 2023-05-16 13:33:09.000000 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/requires.txt
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)       14 2023-05-16 13:33:09.000000 ghostbusterV4-1.0.8/ghostbusterV4.egg-info/top_level.txt
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)       84 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/pyproject.toml
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)       76 2023-05-16 13:33:09.417079 ghostbusterV4-1.0.8/setup.cfg
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)     3019 2023-05-16 13:15:09.000000 ghostbusterV4-1.0.8/setup.py
+drwxr-xr-x   0 pbaid.int (199922920) staff       (20)        0 2023-05-16 13:33:09.397768 ghostbusterV4-1.0.8/tests/
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)     1209 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/tests/test_cli.py
+-rw-r--r--   0 pbaid.int (199922920) staff       (20)     1706 2023-03-22 07:18:25.000000 ghostbusterV4-1.0.8/tests/test_example.py
```

### Comparing `ghostbusterV4-1.0.7/LICENSE` & `ghostbusterV4-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ghostbusterV4-1.0.7/PKG-INFO` & `ghostbusterV4-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ghostbusterV4
-Version: 1.0.7
+Version: 1.0.8
 Summary: Eliminate dangling elastic IPs by performing analysis on your resources within all your AWS accounts.
 Home-page: https://gitlab.urbanclap.com/urbanclap/dangling-dns-service
-Download-URL: https://github.com/assetnote/ghostbusterV4/archive/1.0.7.tar.gz
+Download-URL: https://github.com/assetnote/ghostbusterV4/archive/1.0.8.tar.gz
 Author: yashbharadwaj
 Author-email: yashbharadwaj@urbancompany.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ghostbusterV4-1.0.7/README.rst` & `ghostbusterV4-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `ghostbusterV4-1.0.7/ghostbusterV4/__init__.py` & `ghostbusterV4-1.0.8/ghostbusterV4/__init__.py`

 * *Files identical despite different names*

### Comparing `ghostbusterV4-1.0.7/ghostbusterV4/cli.py` & `ghostbusterV4-1.0.8/ghostbusterV4/cli.py`

 * *Files identical despite different names*

### Comparing `ghostbusterV4-1.0.7/ghostbusterV4/scan.py` & `ghostbusterV4-1.0.8/ghostbusterV4/scan.py`

 * *Files identical despite different names*

### Comparing `ghostbusterV4-1.0.7/ghostbusterV4.egg-info/PKG-INFO` & `ghostbusterV4-1.0.8/ghostbusterV4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ghostbusterV4
-Version: 1.0.7
+Version: 1.0.8
 Summary: Eliminate dangling elastic IPs by performing analysis on your resources within all your AWS accounts.
 Home-page: https://gitlab.urbanclap.com/urbanclap/dangling-dns-service
-Download-URL: https://github.com/assetnote/ghostbusterV4/archive/1.0.7.tar.gz
+Download-URL: https://github.com/assetnote/ghostbusterV4/archive/1.0.8.tar.gz
 Author: yashbharadwaj
 Author-email: yashbharadwaj@urbancompany.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ghostbusterV4-1.0.7/setup.py` & `ghostbusterV4-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,19 @@
     description="Eliminate dangling elastic IPs by performing analysis on your resources within all your AWS accounts.",
     long_description=long_description,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     version=version,
     install_requires=[
         # Include dependencies here
         "click<9.0,>=8.0.3",
-        "boto3",
+        "boto3==1.23.10",
         "cloudflare",
         "awsipranges",
-        "slack_sdk"
+        "slack_sdk",
+        "botocore<1.26.102",
     ],
     entry_points="""
     [console_scripts]
     ghostbusterV4=ghostbusterV4.cli:cli
     """,
     python_requires=">=0.0.1",
     license="Apache Software License 2.0",  # noqa
```

### Comparing `ghostbusterV4-1.0.7/tests/test_cli.py` & `ghostbusterV4-1.0.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ghostbusterV4-1.0.7/tests/test_example.py` & `ghostbusterV4-1.0.8/tests/test_example.py`

 * *Files identical despite different names*

