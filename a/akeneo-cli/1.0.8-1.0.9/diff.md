# Comparing `tmp/akeneo-cli-1.0.8.tar.gz` & `tmp/akeneo-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo-cli-1.0.8.tar", last modified: Thu Feb 16 14:18:11 2023, max compression
+gzip compressed data, was "akeneo-cli-1.0.9.tar", last modified: Tue May 16 13:50:55 2023, max compression
```

## Comparing `akeneo-cli-1.0.8.tar` & `akeneo-cli-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-02-16 14:18:11.385095 akeneo-cli-1.0.8/
--rw-r--r--   0 malhgor    (501) staff       (20)     1074 2022-01-26 16:45:21.000000 akeneo-cli-1.0.8/LICENSE
--rw-r--r--   0 malhgor    (501) staff       (20)     1993 2023-02-16 14:18:11.384776 akeneo-cli-1.0.8/PKG-INFO
--rw-r--r--   0 malhgor    (501) staff       (20)     1551 2022-06-03 07:01:58.000000 akeneo-cli-1.0.8/README.md
--rw-r--r--   0 malhgor    (501) staff       (20)       38 2023-02-16 14:18:11.385228 akeneo-cli-1.0.8/setup.cfg
--rw-r--r--   0 malhgor    (501) staff       (20)      844 2023-02-16 14:17:51.000000 akeneo-cli-1.0.8/setup.py
-drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-02-16 14:18:11.380071 akeneo-cli-1.0.8/src/
-drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-02-16 14:18:11.382643 akeneo-cli-1.0.8/src/akeneo_cli/
--rw-r--r--   0 malhgor    (501) staff       (20)        0 2021-11-18 11:41:20.000000 akeneo-cli-1.0.8/src/akeneo_cli/__init__.py
--rw-r--r--   0 malhgor    (501) staff       (20)    11696 2023-02-16 08:58:43.000000 akeneo-cli-1.0.8/src/akeneo_cli/client.py
--rw-r--r--   0 malhgor    (501) staff       (20)      944 2022-01-26 16:46:04.000000 akeneo-cli-1.0.8/src/akeneo_cli/exceptions.py
--rw-r--r--   0 malhgor    (501) staff       (20)     3502 2022-01-26 16:46:04.000000 akeneo-cli-1.0.8/src/akeneo_cli/main.py
-drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-02-16 14:18:11.384410 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/
--rw-r--r--   0 malhgor    (501) staff       (20)     1993 2023-02-16 14:18:11.000000 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/PKG-INFO
--rw-r--r--   0 malhgor    (501) staff       (20)      360 2023-02-16 14:18:11.000000 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/SOURCES.txt
--rw-r--r--   0 malhgor    (501) staff       (20)        1 2023-02-16 14:18:11.000000 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/dependency_links.txt
--rw-r--r--   0 malhgor    (501) staff       (20)       48 2023-02-16 14:18:11.000000 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/entry_points.txt
--rw-r--r--   0 malhgor    (501) staff       (20)       22 2023-02-16 14:18:11.000000 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/requires.txt
--rw-r--r--   0 malhgor    (501) staff       (20)       11 2023-02-16 14:18:11.000000 akeneo-cli-1.0.8/src/akeneo_cli.egg-info/top_level.txt
+drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-05-16 13:50:55.194118 akeneo-cli-1.0.9/
+-rw-r--r--   0 malhgor    (501) staff       (20)     1074 2022-01-26 16:45:21.000000 akeneo-cli-1.0.9/LICENSE
+-rw-r--r--   0 malhgor    (501) staff       (20)     1993 2023-05-16 13:50:55.193864 akeneo-cli-1.0.9/PKG-INFO
+-rw-r--r--   0 malhgor    (501) staff       (20)     1551 2022-06-03 07:01:58.000000 akeneo-cli-1.0.9/README.md
+-rw-r--r--   0 malhgor    (501) staff       (20)       38 2023-05-16 13:50:55.194226 akeneo-cli-1.0.9/setup.cfg
+-rw-r--r--   0 malhgor    (501) staff       (20)      844 2023-05-16 13:50:31.000000 akeneo-cli-1.0.9/setup.py
+drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-05-16 13:50:55.189592 akeneo-cli-1.0.9/src/
+drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-05-16 13:50:55.191998 akeneo-cli-1.0.9/src/akeneo_cli/
+-rw-r--r--   0 malhgor    (501) staff       (20)        0 2021-11-18 11:41:20.000000 akeneo-cli-1.0.9/src/akeneo_cli/__init__.py
+-rw-r--r--   0 malhgor    (501) staff       (20)    11757 2023-05-16 13:49:38.000000 akeneo-cli-1.0.9/src/akeneo_cli/client.py
+-rw-r--r--   0 malhgor    (501) staff       (20)      944 2022-01-26 16:46:04.000000 akeneo-cli-1.0.9/src/akeneo_cli/exceptions.py
+-rw-r--r--   0 malhgor    (501) staff       (20)     3522 2023-05-16 13:49:43.000000 akeneo-cli-1.0.9/src/akeneo_cli/main.py
+drwxr-xr-x   0 malhgor    (501) staff       (20)        0 2023-05-16 13:50:55.193542 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/
+-rw-r--r--   0 malhgor    (501) staff       (20)     1993 2023-05-16 13:50:55.000000 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/PKG-INFO
+-rw-r--r--   0 malhgor    (501) staff       (20)      360 2023-05-16 13:50:55.000000 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 malhgor    (501) staff       (20)        1 2023-05-16 13:50:55.000000 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 malhgor    (501) staff       (20)       48 2023-05-16 13:50:55.000000 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/entry_points.txt
+-rw-r--r--   0 malhgor    (501) staff       (20)       22 2023-05-16 13:50:55.000000 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/requires.txt
+-rw-r--r--   0 malhgor    (501) staff       (20)       11 2023-05-16 13:50:55.000000 akeneo-cli-1.0.9/src/akeneo_cli.egg-info/top_level.txt
```

### Comparing `akeneo-cli-1.0.8/LICENSE` & `akeneo-cli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo-cli-1.0.8/PKG-INFO` & `akeneo-cli-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: CLI for Akeneo API
 Home-page: https://github.com/tms-software/akeneo-cli
 Author: Franck COUTOULY
 Author-email: franck.coutouly@tms-software.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `akeneo-cli-1.0.8/README.md` & `akeneo-cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `akeneo-cli-1.0.8/setup.py` & `akeneo-cli-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="akeneo-cli",
-    version="1.0.8",
+    version="1.0.9",
     url="https://github.com/tms-software/akeneo-cli",
     author="Franck COUTOULY",
     author_email="franck.coutouly@tms-software.ch",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `akeneo-cli-1.0.8/src/akeneo_cli/client.py` & `akeneo-cli-1.0.9/src/akeneo_cli/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,16 +41,18 @@
         self.__refresh_token = 0
         self.__expiration_date = datetime.now()
 
     def __call(self, url, method="GET", data=None, additional_headers={}):
         files = None
         headers = {**self.__headers, **additional_headers}
         if headers["Content-Type"] == "application/json":
+            if data is not None:
+                data = json.dumps(data)
             response = getattr(requests, method.lower())(
-                url, verify=False, headers=headers, data=json.dumps(data)
+                url, verify=False, headers=headers, data=data
             )
 
         elif headers["Content-Type"] == "multipart/form-data":
             del headers["Content-Type"]
             files = data
             files["file"] = (
                 data["file"],
```

### Comparing `akeneo-cli-1.0.8/src/akeneo_cli/exceptions.py` & `akeneo-cli-1.0.9/src/akeneo_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `akeneo-cli-1.0.8/src/akeneo_cli/main.py` & `akeneo-cli-1.0.9/src/akeneo_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if args.object == "product":
             if args.mode == "get":
                 result = client.get(
                     "products",
                     args.code,
                     filters=dict(page=args.page, limit=args.per_page),
                 )
-    print(json.dumps(result, indent=4))
+                print(json.dumps(result["json"], indent=4))
 
 
 def getArgParser():
     objects = prepareObjectsParserDefinitions()
     optional = prepareOptionalArgsDefinitions()
     main = argparse.ArgumentParser(
         prog="akeneo",
```

### Comparing `akeneo-cli-1.0.8/src/akeneo_cli.egg-info/PKG-INFO` & `akeneo-cli-1.0.9/src/akeneo_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: CLI for Akeneo API
 Home-page: https://github.com/tms-software/akeneo-cli
 Author: Franck COUTOULY
 Author-email: franck.coutouly@tms-software.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

