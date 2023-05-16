# Comparing `tmp/dynamicadaptor-0.3.9.tar.gz` & `tmp/dynamicadaptor-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicadaptor-0.3.9.tar", max compression
+gzip compressed data, was "dynamicadaptor-0.4.0.tar", max compression
```

## Comparing `dynamicadaptor-0.3.9.tar` & `dynamicadaptor-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    18431 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/LICENSE
--rw-r--r--   0        0        0    10010 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/README.md
--rw-r--r--   0        0        0     2136 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/AddonCard.py
--rw-r--r--   0        0        0      926 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/Content.py
--rw-r--r--   0        0        0    19821 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/DynamicConversion.py
--rw-r--r--   0        0        0      575 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/Header.py
--rw-r--r--   0        0        0     3402 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/Majors.py
--rw-r--r--   0        0        0      410 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/Message.py
--rw-r--r--   0        0        0      323 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/Repost.py
--rw-r--r--   0        0        0       10 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/dynamicadaptor/__init__.py
--rw-r--r--   0        0        0      504 2023-04-01 12:25:10.809739 dynamicadaptor-0.3.9/pyproject.toml
--rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    18431 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10010 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/README.md
+-rw-r--r--   0        0        0     2136 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/dynamicadaptor/AddonCard.py
+-rw-r--r--   0        0        0      926 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/dynamicadaptor/Content.py
+-rw-r--r--   0        0        0    20093 2023-05-16 02:22:41.620221 dynamicadaptor-0.4.0/dynamicadaptor/DynamicConversion.py
+-rw-r--r--   0        0        0      575 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Header.py
+-rw-r--r--   0        0        0     3402 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Majors.py
+-rw-r--r--   0        0        0      410 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Message.py
+-rw-r--r--   0        0        0      323 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/Repost.py
+-rw-r--r--   0        0        0       10 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/dynamicadaptor/__init__.py
+-rw-r--r--   0        0        0      504 2023-05-16 02:22:41.624222 dynamicadaptor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 dynamicadaptor-0.4.0/PKG-INFO
```

### Comparing `dynamicadaptor-0.3.9/LICENSE` & `dynamicadaptor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.3.9/README.md` & `dynamicadaptor-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.3.9/dynamicadaptor/AddonCard.py` & `dynamicadaptor-0.4.0/dynamicadaptor/AddonCard.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.3.9/dynamicadaptor/Content.py` & `dynamicadaptor-0.4.0/dynamicadaptor/Content.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.3.9/dynamicadaptor/DynamicConversion.py` & `dynamicadaptor-0.4.0/dynamicadaptor/DynamicConversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     """
     message_type = message["cardType"]
     message_id = message["extend"]["dynIdStr"]
     header = await get_grpc_header(message["modules"][0]["moduleAuthor"])
     
     text = await get_grpc_text(message)
+    # print(text)
     major = await get_grpc_major(message)
     additional = await get_grpc_additional(message)
     # print(additional)
     forward = await get_grpc_forward(message)
     render_message = RenderMessage(
         message_type=message_type,
         message_id=message_id,
@@ -149,15 +150,20 @@
         try:
             if i["moduleType"] == "module_desc":
                 plain_text = i["moduleDesc"]["text"]
                 rich_text_nodes = []
                 for j in i["moduleDesc"]["desc"]:
                     temp = {"type": rich_type_dict[j["type"]], "text": j["text"], "orig_text": j["origText"]}
                     try:
-                        temp["emoji"] = {"icon_url": j["uri"], "type": j["emojiType"], "text": j["text"]}
+                        # print(j)
+                        if "emojiType" in j:
+                            
+                            temp["emoji"] = {"icon_url": j["uri"], "type": j["emojiType"], "text": j["text"]}
+                        else:
+                            temp["emoji"] = {"icon_url": j["uri"], "type": j["type"], "text": j["text"]}
                     except Exception as e:
                         pass
                     rich_text_nodes.append(temp)
                 text["text"] = plain_text
                 text["rich_text_nodes"] = rich_text_nodes
         except Exception:
             logger.exception("error")
```

### Comparing `dynamicadaptor-0.3.9/dynamicadaptor/Header.py` & `dynamicadaptor-0.4.0/dynamicadaptor/Header.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.3.9/dynamicadaptor/Majors.py` & `dynamicadaptor-0.4.0/dynamicadaptor/Majors.py`

 * *Files identical despite different names*

### Comparing `dynamicadaptor-0.3.9/PKG-INFO` & `dynamicadaptor-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicadaptor
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Author: DMC
 Author-email: lzxder@outlook.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

