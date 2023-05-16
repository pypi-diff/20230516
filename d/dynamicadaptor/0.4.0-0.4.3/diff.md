# Comparing `tmp/dynamicadaptor-0.4.0.tar.gz` & `tmp/dynamicadaptor-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicadaptor-0.4.0.tar", max compression
+gzip compressed data, was "dynamicadaptor-0.4.3.tar", max compression
```

## Comparing `dynamicadaptor-0.4.0.tar` & `dynamicadaptor-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/LICENSE
--rw-r--r--   0        0        0    10010 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/README.md
--rw-r--r--   0        0        0     2136 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/dynamicadaptor/AddonCard.py
--rw-r--r--   0        0        0      926 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/dynamicadaptor/Content.py
--rw-r--r--   0        0        0    20093 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/dynamicadaptor/DynamicConversion.py
--rw-r--r--   0        0        0      575 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Header.py
--rw-r--r--   0        0        0     3402 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Majors.py
--rw-r--r--   0        0        0      410 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Message.py
--rw-r--r--   0        0        0      323 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Repost.py
--rw-r--r--   0        0        0       10 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/__init__.py
--rw-r--r--   0        0        0      504 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/LICENSE
+-rw-r--r--   0        0        0    10010 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/README.md
+-rw-r--r--   0        0        0     2136 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/AddonCard.py
+-rw-r--r--   0        0        0      926 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Content.py
+-rw-r--r--   0        0        0    20217 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/DynamicConversion.py
+-rw-r--r--   0        0        0      575 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Header.py
+-rw-r--r--   0        0        0     3402 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Majors.py
+-rw-r--r--   0        0        0      410 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Message.py
+-rw-r--r--   0        0        0      323 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/Repost.py
+-rw-r--r--   0        0        0       10 2023-05-16 08:27:06.717344 dynamicadaptor-0.4.3/dynamicadaptor/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-16 08:27:06.721344 dynamicadaptor-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.3/PKG-INFO
```

### Comparing `dynamicadaptor-0.4.0/LICENSE` & `dynamicadaptor-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.0/README.md` & `dynamicadaptor-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.0/dynamicadaptor/AddonCard.py` & `dynamicadaptor-0.4.3/dynamicadaptor/AddonCard.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.0/dynamicadaptor/Content.py` & `dynamicadaptor-0.4.3/dynamicadaptor/Content.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.0/dynamicadaptor/DynamicConversion.py` & `dynamicadaptor-0.4.3/dynamicadaptor/DynamicConversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,16 @@
 
     Returns:
         Union[Forward, None]: 符合要求的信息
     """
     dynamic_forward = None
     for i in message["modules"]:
         module_type=i["moduleType"]
-        if module_type == "module_dynamic" and i["moduleDynamic"]["type"]=="mdl_dyn_forward":
+        # try:
+        if module_type == "module_dynamic" and "type" in i["moduleDynamic"] and i["moduleDynamic"]["type"]=="mdl_dyn_forward":
             dynamic_forward = i["moduleDynamic"]["dynForward"]["item"]
             break
         elif module_type == "module_item_null":
             forward_message_type = "DYNAMIC_TYPE_NONE"
             forward_header={"name": "","mid": 0}
             forward_major ={"type": "MAJOR_TYPE_NONE", "none": {"tips":i["moduleItemNull"]["text"]}}
             forward_text =None
@@ -372,14 +373,16 @@
             forward = Forward(
             message_type=forward_message_type,
             header=forward_header,
             text=forward_text,
             major=forward_major,
             additional=forward_additional)
             return forward
+        # except Exception as e:
+        #     print(i["moduleDynamic"])
     if dynamic_forward:
         forward_message_type = dynamic_forward["cardType"]
         forward_header = await get_grpc_forward_header(dynamic_forward)
         forward_major = await get_grpc_major(dynamic_forward)
         forward_text = await get_grpc_text(dynamic_forward)
         forward_additional = await get_grpc_additional(dynamic_forward)
         forward = Forward(
```

### Comparing `dynamicadaptor-0.4.0/dynamicadaptor/Header.py` & `dynamicadaptor-0.4.3/dynamicadaptor/Header.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.0/dynamicadaptor/Majors.py` & `dynamicadaptor-0.4.3/dynamicadaptor/Majors.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.4.0/PKG-INFO` & `dynamicadaptor-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicadaptor
-Version: 0.4.0
+Version: 0.4.3
 Summary: 
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

