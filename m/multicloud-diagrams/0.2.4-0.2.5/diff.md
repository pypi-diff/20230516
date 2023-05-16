# Comparing `tmp/multicloud_diagrams-0.2.4.tar.gz` & `tmp/multicloud_diagrams-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.2.4.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.2.5.tar", max compression
```

## Comparing `multicloud_diagrams-0.2.4.tar` & `multicloud_diagrams-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.4/LICENSE
--rw-r--r--   0        0        0     2424 2023-05-14 21:09:48.427093 multicloud_diagrams-0.2.4/README.md
--rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.4/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0      509 2023-05-14 21:10:36.734499 multicloud_diagrams-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2942 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2423 2023-05-16 16:49:37.678198 multicloud_diagrams-0.2.5/README.md
+-rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.5/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0      509 2023-05-16 16:49:37.688685 multicloud_diagrams-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.5/PKG-INFO
```

### Comparing `multicloud_diagrams-0.2.4/LICENSE` & `multicloud_diagrams-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.4/README.md` & `multicloud_diagrams-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -35,20 +35,19 @@
 Generating `drawio` diagrams from the code (Diagrams as a Code) for popular Amazon Web Services:
 
 #### AWS DynamoDB Details
 
 - Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
 
 - Output compiled [drawio diagram](samples/output/output.prod.dynamo.drawio):
-
-![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.dynamo.png?raw=True))
+![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/raw/main/samples/output/png/output.prod.dynamo.png?raw=True)
 
 #### AWS IAM Graph
 
-- Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
+- Source [aws_dynamo.py](samples/samples/aws_iam_roles.py)
 - Output compiled [drawio diagram](samples/output/output.prod.iam-roles.drawio)
 
-![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles.png?raw=True))
+![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles.png?raw=True)
 
 ### FYI:
 
 OpenSource Guide, [How to contribute to opensource](https://opensource.guide/)
```

### Comparing `multicloud_diagrams-0.2.4/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.2.5/multicloud_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.4/PKG-INFO` & `multicloud_diagrams-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicloud-diagrams
-Version: 0.2.4
+Version: 0.2.5
 Summary: Library to generate DRAW.IO compatible diagrams to represent Cloud infrastructure. AWS Cloud supported.
 License: MIT
 Author: Roman Tsypuk
 Author-email: tsypuk.conf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -49,20 +49,19 @@
 Generating `drawio` diagrams from the code (Diagrams as a Code) for popular Amazon Web Services:
 
 #### AWS DynamoDB Details
 
 - Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
 
 - Output compiled [drawio diagram](samples/output/output.prod.dynamo.drawio):
-
-![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.dynamo.png?raw=True))
+![output.prod.dynamo.png](https://github.com/tsypuk/multicloud-diagrams/raw/main/samples/output/png/output.prod.dynamo.png?raw=True)
 
 #### AWS IAM Graph
 
-- Source [aws_dynamo.py](samples/samples/aws_dynamo.py)
+- Source [aws_dynamo.py](samples/samples/aws_iam_roles.py)
 - Output compiled [drawio diagram](samples/output/output.prod.iam-roles.drawio)
 
-![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles.png?raw=True))
+![output.prod.iam-roles.png](https://github.com/tsypuk/multicloud-diagrams/blob/main/samples/output/png/output.prod.iam-roles.png?raw=True)
 
 ### FYI:
 
 OpenSource Guide, [How to contribute to opensource](https://opensource.guide/)
```

