# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.14.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.14.tar", last modified: Thu May 11 19:47:28 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.15.tar", last modified: Tue May 16 09:17:35 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.14.tar` & `bytetrade-recommend-model-sdk-0.0.15.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-10 04:37:58.000000 bytetrade-recommend-model-sdk-0.0.14/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-04-24 08:15:48.000000 bytetrade-recommend-model-sdk-0.0.14/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.380156 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      983 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-11 19:47:28.000000 bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.380156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 08:07:33.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 15:19:49.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-04-21 15:20:39.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2518 2023-04-22 09:06:18.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-23 00:13:23.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-04-28 08:19:07.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:16:24.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:17:41.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/faiss_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9462 2023-05-11 19:36:12.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/rank_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-07 06:11:48.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 01:30:23.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      740 2023-04-21 13:49:04.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 12:41:52.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-04-22 22:25:24.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-06 12:19:45.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26424 2023-05-08 01:15:21.000000 bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-11 19:47:28.384156 bytetrade-recommend-model-sdk-0.0.14/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-11 19:46:20.000000 bytetrade-recommend-model-sdk-0.0.14/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.160922 bytetrade-recommend-model-sdk-0.0.15/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-10 04:37:58.000000 bytetrade-recommend-model-sdk-0.0.15/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-16 09:17:35.160922 bytetrade-recommend-model-sdk-0.0.15/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-04-24 08:15:48.000000 bytetrade-recommend-model-sdk-0.0.15/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-16 09:17:35.000000 bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      983 2023-05-16 09:17:35.000000 bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 09:17:35.000000 bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-16 09:17:35.000000 bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-16 09:17:35.000000 bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 08:07:33.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 15:19:49.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-04-21 15:20:39.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-16 08:59:28.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-23 00:13:23.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-04-28 08:19:07.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:16:24.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 03:17:41.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/faiss_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9462 2023-05-11 19:36:12.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/rank_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-07 06:11:48.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-25 01:30:23.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-05-16 09:13:34.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 09:17:35.156922 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-20 12:41:52.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-04-22 22:25:24.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-06 12:19:45.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26860 2023-05-16 09:13:12.000000 bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 09:17:35.160922 bytetrade-recommend-model-sdk-0.0.15/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-16 09:17:21.000000 bytetrade-recommend-model-sdk-0.0.15/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.14/README.md` & `bytetrade-recommend-model-sdk-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.15/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/rank_tool.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/rank_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/rank/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/rank/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/resources/model_management.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'word2vec_google'": "{'v2': OrderedDict([('mongodb_embedding_field', 'word2vec_google_v2'), "*

 * *                      "('pg_embedding_mark_field', 'word2vec_google_v2'), ('s3_bucket', "*

 * *                      "'gpu-model-data'), ('model_related_files', "*

 * *                      "['GoogleNews-vectors-negative300.bin', 'tfidf.model', 'dictionary']), "*

 * *                      "('model_related_files_suffix', "*

 * *                      "OrderedDict([('GoogleNews-vectors-negative300.bin', 'gz'), ('tfidf.model', "*

 * *        […]*

```diff
@@ -16,10 +16,31 @@
                 "GoogleNews-vectors-negative300.bin": "gz",
                 "dictionary": "gz",
                 "tfidf.model": "gz"
             },
             "mongodb_embedding_field": "word2vec_google_v1",
             "pg_embedding_mark_field": "word2vec_google_embedding",
             "s3_bucket": "gpu-model-data"
+        },
+        "v2": {
+            "active": false,
+            "model_related_files": [
+                "GoogleNews-vectors-negative300.bin",
+                "tfidf.model",
+                "dictionary"
+            ],
+            "model_related_files_public": {
+                "GoogleNews-vectors-negative300.bin": true,
+                "dictionary": false,
+                "tfidf.model": false
+            },
+            "model_related_files_suffix": {
+                "GoogleNews-vectors-negative300.bin": "gz",
+                "dictionary": "gz",
+                "tfidf.model": "gz"
+            },
+            "mongodb_embedding_field": "word2vec_google_v2",
+            "pg_embedding_mark_field": "word2vec_google_v2",
+            "s3_bucket": "gpu-model-data"
         }
     }
 }
```

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.14/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.15/recommend_model_sdk/tools/model_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,18 @@
     def valid_model_name_and_version(self,model_name,model_version):
         if isinstance(model_name,str) is False:
             raise ValueError("model name need to be str")
         if isinstance(model_version,str) is False:
             raise ValueError("model_version need to be str")
         
         if model_name not in self.__model_dict:
-            return False
+            raise ValueError(f"model_name {model_name} not exist")
         
         if model_version not in self.__model_dict[model_name]:
-            return False
+            raise ValueError(f'model_version {model_version} not exist')
         
         return self.__model_dict[model_name][model_version]
     
     def word2vec_calculate_embedding(self,model_name,model_version,dict_document):
         self.valid_model_name_and_version(model_name,model_version)
         self.valid_infer_document(dict_document)
         if model_name != "word2vec_google":
@@ -156,16 +156,22 @@
         
         tfidf_path = os.path.join(current_model_dir,"tfidf.model")
         google_word2vec_path = os.path.join(current_common_dir,"GoogleNews-vectors-negative300.bin")
         dictionary_path = os.path.join(current_model_dir,"dictionary")
         
         word2vect_tool = Word2VecEmbedding(tfidf_path,dictionary_path,google_word2vec_path)
         id_to_infer_result = dict()
-        for current_id, current_text in dict_document.items():
-            id_to_infer_result[current_id] = word2vect_tool.calculate_embedding(current_text)
+        if model_version == "v1":
+            for current_id, current_text in dict_document.items():
+                id_to_infer_result[current_id] = word2vect_tool.calculate_embedding(current_text)
+        elif model_version == "v2":
+            for current_id, current_text in dict_document.items():
+                id_to_infer_result[current_id] = word2vect_tool.calculate_embedding_rake_nltk_keyword(current_text)
+        else:
+            raise ValueError(f"not supported version {model_version}")
             
         return id_to_infer_result
         
     def valid_infer_document(self,dict_documents):
         if isinstance(dict_documents,dict) is False:
             raise ValueError("dict_documents is not dict")
         for current_id,current_text in dict_documents.items():
```

### Comparing `bytetrade-recommend-model-sdk-0.0.14/setup.py` & `bytetrade-recommend-model-sdk-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.14",
+    version="0.0.15",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==4.21.8",
         "nltk==3.8.1",
         "boto3"
```

