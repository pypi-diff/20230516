# Comparing `tmp/text2graphapi-0.1.5.tar.gz` & `tmp/text2graphapi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2graphapi-0.1.5.tar", last modified: Thu Apr 27 14:19:56 2023, max compression
+gzip compressed data, was "text2graphapi-0.1.6.tar", last modified: Tue May 16 21:29:31 2023, max compression
```

## Comparing `text2graphapi-0.1.5.tar` & `text2graphapi-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.182045 text2graphapi-0.1.5/
--rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5410 2023-04-27 14:19:56.180033 text2graphapi-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.058283 text2graphapi-0.1.5/docs/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.000754 text2graphapi-0.1.5/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.001651 text2graphapi-0.1.5/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.066281 text2graphapi-0.1.5/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.5/docs/_build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.5/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.5/docs/_build/html/_sources/modules.rst.txt
--rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.5/docs/_build/html/_sources/src.rst.txt
--rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.5/docs/conf.py
--rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.5/notes.txt
--rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 14:19:56.183064 text2graphapi-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-04-27 14:19:45.000000 text2graphapi-0.1.5/setup.py
--rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.5/test_spacy.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.069282 text2graphapi-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.075281 text2graphapi-0.1.5/text2graphapi/
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.011710 text2graphapi-0.1.5/text2graphapi/docs/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.007651 text2graphapi-0.1.5/text2graphapi/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.009653 text2graphapi-0.1.5/text2graphapi/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.122277 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/
--rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
--rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
--rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.125707 text2graphapi-0.1.5/text2graphapi/docs/source/
--rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/docs/source/conf.py
--rw-rw-rw-   0        0        0     8063 2023-04-27 14:12:46.000000 text2graphapi-0.1.5/text2graphapi/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.170010 text2graphapi-0.1.5/text2graphapi/src/
--rw-rw-rw-   0        0        0     7155 2023-04-25 17:20:48.000000 text2graphapi-0.1.5/text2graphapi/src/Cooccurrence.py
--rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/Graph.py
--rw-rw-rw-   0        0        0     1018 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/GraphTransformation.py
--rw-rw-rw-   0        0        0    13651 2023-04-27 14:05:50.000000 text2graphapi-0.1.5/text2graphapi/src/Heterogeneous.py
--rw-rw-rw-   0        0        0     8833 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/src/Preprocessing.py
--rw-rw-rw-   0        0        0     1873 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/src/Utils.py
--rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.5/text2graphapi/src/configs.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.178056 text2graphapi-0.1.5/text2graphapi/src/resources/
--rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_english.txt
--rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_french.txt
--rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_spanish.txt
--rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.5/text2graphapi/testing.py
-drwxrwxrwx   0        0        0        0 2023-04-27 14:19:56.112273 text2graphapi-0.1.5/text2graphapi.egg-info/
--rw-rw-rw-   0        0        0     5410 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-27 14:19:55.000000 text2graphapi-0.1.5/text2graphapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.756653 text2graphapi-0.1.6/
+-rw-rw-rw-   0        0        0       82 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2022-12-02 17:54:23.000000 text2graphapi-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2022-12-02 17:54:23.000000 text2graphapi-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5410 2023-05-16 21:29:31.755625 text2graphapi-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-04-25 17:11:34.000000 text2graphapi-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.639667 text2graphapi-0.1.6/docs/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.595632 text2graphapi-0.1.6/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.597636 text2graphapi-0.1.6/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.658628 text2graphapi-0.1.6/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.6/docs/_build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1663 2023-03-30 14:12:11.000000 text2graphapi-0.1.6/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0       46 2022-12-05 21:50:59.000000 text2graphapi-0.1.6/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0      408 2022-12-05 21:50:59.000000 text2graphapi-0.1.6/docs/_build/html/_sources/src.rst.txt
+-rw-rw-rw-   0        0        0     1783 2022-12-05 21:50:59.000000 text2graphapi-0.1.6/docs/conf.py
+-rw-rw-rw-   0        0        0      590 2023-03-30 04:06:40.000000 text2graphapi-0.1.6/notes.txt
+-rw-rw-rw-   0        0        0      201 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 21:29:31.756653 text2graphapi-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-05-16 21:22:27.000000 text2graphapi-0.1.6/setup.py
+-rw-rw-rw-   0        0        0      379 2023-03-16 18:14:42.000000 text2graphapi-0.1.6/test_spacy.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.661629 text2graphapi-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-12 14:46:40.000000 text2graphapi-0.1.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.669627 text2graphapi-0.1.6/text2graphapi/
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/text2graphapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.608634 text2graphapi-0.1.6/text2graphapi/docs/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.605628 text2graphapi-0.1.6/text2graphapi/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.607635 text2graphapi-0.1.6/text2graphapi/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.690627 text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/
+-rw-rw-rw-   0        0        0     1745 2023-03-30 13:11:13.000000 text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt
+-rw-rw-rw-   0        0        0     1768 2023-03-30 13:07:45.000000 text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt
+-rw-rw-rw-   0        0        0     1702 2023-03-30 11:19:22.000000 text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.692625 text2graphapi-0.1.6/text2graphapi/docs/source/
+-rw-rw-rw-   0        0        0     1352 2023-04-25 17:11:34.000000 text2graphapi-0.1.6/text2graphapi/docs/source/conf.py
+-rw-rw-rw-   0        0        0     8105 2023-04-27 15:47:40.000000 text2graphapi-0.1.6/text2graphapi/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.742832 text2graphapi-0.1.6/text2graphapi/src/
+-rw-rw-rw-   0        0        0     7156 2023-05-16 21:29:13.000000 text2graphapi-0.1.6/text2graphapi/src/Cooccurrence.py
+-rw-rw-rw-   0        0        0     1088 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/text2graphapi/src/Graph.py
+-rw-rw-rw-   0        0        0     1018 2023-05-16 21:29:11.000000 text2graphapi-0.1.6/text2graphapi/src/GraphTransformation.py
+-rw-rw-rw-   0        0        0    13651 2023-05-16 21:29:07.000000 text2graphapi-0.1.6/text2graphapi/src/Heterogeneous.py
+-rw-rw-rw-   0        0        0     8828 2023-04-27 15:49:46.000000 text2graphapi-0.1.6/text2graphapi/src/Preprocessing.py
+-rw-rw-rw-   0        0        0     1873 2023-04-25 17:11:34.000000 text2graphapi-0.1.6/text2graphapi/src/Utils.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/text2graphapi/src/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-25 17:11:34.000000 text2graphapi-0.1.6/text2graphapi/src/configs.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.752628 text2graphapi-0.1.6/text2graphapi/src/resources/
+-rw-rw-rw-   0        0        0     4160 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/text2graphapi/src/resources/stopwords_english.txt
+-rw-rw-rw-   0        0        0     5256 2023-03-08 18:09:28.000000 text2graphapi-0.1.6/text2graphapi/src/resources/stopwords_french.txt
+-rw-rw-rw-   0        0        0     4852 2023-01-17 01:14:45.000000 text2graphapi-0.1.6/text2graphapi/src/resources/stopwords_spanish.txt
+-rw-rw-rw-   0        0        0     2248 2023-03-30 02:11:28.000000 text2graphapi-0.1.6/text2graphapi/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:29:31.683627 text2graphapi-0.1.6/text2graphapi.egg-info/
+-rw-rw-rw-   0        0        0     5410 2023-05-16 21:29:31.000000 text2graphapi-0.1.6/text2graphapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-05-16 21:29:31.000000 text2graphapi-0.1.6/text2graphapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:29:31.000000 text2graphapi-0.1.6/text2graphapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-05-16 21:29:31.000000 text2graphapi-0.1.6/text2graphapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-16 21:29:31.000000 text2graphapi-0.1.6/text2graphapi.egg-info/top_level.txt
```

### Comparing `text2graphapi-0.1.5/LICENSE.txt` & `text2graphapi-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/PKG-INFO` & `text2graphapi-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: UNKNOWN
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.5/README.md` & `text2graphapi-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/docs/_build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.6/docs/_build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/docs/_build/html/_sources/index.rst.txt` & `text2graphapi-0.1.6/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/docs/conf.py` & `text2graphapi-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/notes.txt` & `text2graphapi-0.1.6/notes.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/setup.py` & `text2graphapi-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ROOT = path.abspath(path.dirname(__file__))
 
 with open(path.join(ROOT, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="text2graphapi",
-    version="0.1.5",
+    version="0.1.6",
     description="Use this library to transform raw text into differents graph representations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="PLN-disca-iimas",
     author_email="andric.valdez@gmail.com",
     license="MIT",
```

### Comparing `text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt` & `text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/Cooocurrence.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt` & `text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/Heterogeneous.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/docs/build/html/_sources/index.rst.txt` & `text2graphapi-0.1.6/text2graphapi/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/docs/source/conf.py` & `text2graphapi-0.1.6/text2graphapi/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/main.py` & `text2graphapi-0.1.6/text2graphapi/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # *** Logging configs
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s; - %(levelname)s; - %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 # *** Configs
 ROOT_DIR = os.path.dirname(os.path.dirname(__file__))
-TEST_API_FROM = 'PYPY' #posible values: LOCAL, PYPI
+TEST_API_FROM = 'LOCAL' #posible values: LOCAL, PYPI
 PRINT_NUM_OUTPUT_GRAPHS = 5
 
 
 
 # TEST API PYPI
 if TEST_API_FROM == 'PYPY':
     from text2graphapi.src.Cooccurrence  import Cooccurrence
@@ -109,14 +109,15 @@
 
 def read_pan_dataset(dataset_name, file_name):
     logger.info("*** Using dataset: %s", dataset_name)
     dataset_dir = ROOT_DIR + '/text2graphapi/datasets/' + dataset_name
     files = glob.glob(f"{dataset_dir}/*.jsonl")
     df_files = [pd.read_json(path_or_buf=f, lines=True) for f in files]
     df_reduced = reduce(lambda df1,df2: pd.merge(df1,df2,how='left',on='id'), df_files)
+    print(df_reduced.info())
     return handle_PAN_dataset(df_reduced)
 
 
 def handle_PAN_dataset(corpus_df, num_rows=-1):
     corpus_df.drop_duplicates(subset="pair", keep='first', inplace=True)
     pairs_list = pd.Series([x for _list in pd.Series(corpus_df['pair']) for x in _list])    
     pairs_list = pairs_list.value_counts().index.tolist()
@@ -147,15 +148,15 @@
     hetero_graph = Heterogeneous(
         window_size = 20, 
         graph_type = 'Graph',
         parallel_exec = False,
         apply_preprocessing = True, 
         load_preprocessing = False, 
         steps_preprocessing = {},
-        language = 'en', #es, en,
+        language = 'es', #es, en,
         output_format = 'networkx',
     )
     # apply Heterogeneous transformation
     corpus_hetero_graph = hetero_graph.transform(corpus_docs)
     return corpus_hetero_graph
 
 
@@ -211,8 +212,8 @@
         #print(graph['graph'].edges)
 
 
 if __name__ == '__main__':
     # datasets options  : tass_emotion_detection, spanish_fake_news, 20_newsgroups, pan_14, pan_15, pan_20, pan_22
     # graph_type options: Cooccurrence, Heterogeneous
 
-    main(dataset='pan_23', graph_type='Heterogeneous', cut_dataset=-1)
+    main(dataset='spanish_fake_news', graph_type='Heterogeneous', cut_dataset=-1)
```

### Comparing `text2graphapi-0.1.5/text2graphapi/src/Cooccurrence.py` & `text2graphapi-0.1.6/text2graphapi/src/Cooccurrence.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 TEST_API_FROM = 'PYPI' #posible values: LOCAL, PYPI
 warnings.filterwarnings("ignore")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO, format="%(asctime)s; - %(levelname)s; - %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 logger.debug('Import libraries/modules from :%s', TEST_API_FROM)
-if TEST_API_FROM == 'PYPI':
+if TEST_API_FROM == 'LOCAL':
     from text2graphapi.src.Utils import Utils
     from text2graphapi.src.Preprocessing import Preprocessing
     from text2graphapi.src.GraphTransformation import GraphTransformation
     from text2graphapi.src import Graph
 else:
     from src.Utils import Utils
     from src.Preprocessing import Preprocessing
```

### Comparing `text2graphapi-0.1.5/text2graphapi/src/Graph.py` & `text2graphapi-0.1.6/text2graphapi/src/Graph.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/src/GraphTransformation.py` & `text2graphapi-0.1.6/text2graphapi/src/GraphTransformation.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/src/Heterogeneous.py` & `text2graphapi-0.1.6/text2graphapi/src/Heterogeneous.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/src/Preprocessing.py` & `text2graphapi-0.1.6/text2graphapi/src/Preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             'to_lowercase': self.to_lowercase,
             'handle_blank_spaces': self.handle_blank_spaces
         }
 
         # Load Spacy model: tokenizer, tagger            
         if self.lang == 'es':
             stoword_path = RESOURCES_DIR + '/stopwords_spanish.txt'
-            self.nlp = self.load_spacy_model("es_core_news_sd")
+            self.nlp = self.load_spacy_model("es_core_news_sm")
         elif self.lang == 'fr':
             stoword_path = RESOURCES_DIR + '/stopwords_french.txt'
             self.nlp = self.load_spacy_model("fr_core_news_sm")
         else: #default self.lang == 'en'
             stoword_path = RESOURCES_DIR + '/stopwords_english.txt'
             #self.nlp = spacy.load("en_core_web_sm")
             self.nlp = self.load_spacy_model("en_core_web_sm")
@@ -86,15 +86,15 @@
     def load_spacy_model(self, spacy_model):
         exclude_modules = ["ner", "parser", "lemmatizer", "textcat"]
         try:
             spacy.load(spacy_model, exclude=exclude_modules)
             logger.info('Has already installed spacy model %s', spacy_model)
         except OSError:
             logger.info("Downloading %s model for the spaCy, this will only happen once", spacy_model)
-            download('en_core_web_sm')
+            download(spacy_model)
         finally:
             return spacy.load(spacy_model, exclude=exclude_modules)
 
 
     def prepocessing_pipeline(self, text):
         logger.debug('Aplying Text Preprocessing')
         if len(self.param_prepro) == 0:
```

### Comparing `text2graphapi-0.1.5/text2graphapi/src/Utils.py` & `text2graphapi-0.1.6/text2graphapi/src/Utils.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_english.txt` & `text2graphapi-0.1.6/text2graphapi/src/resources/stopwords_english.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_french.txt` & `text2graphapi-0.1.6/text2graphapi/src/resources/stopwords_french.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/src/resources/stopwords_spanish.txt` & `text2graphapi-0.1.6/text2graphapi/src/resources/stopwords_spanish.txt`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi/testing.py` & `text2graphapi-0.1.6/text2graphapi/testing.py`

 * *Files identical despite different names*

### Comparing `text2graphapi-0.1.5/text2graphapi.egg-info/PKG-INFO` & `text2graphapi-0.1.6/text2graphapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2graphapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: Use this library to transform raw text into differents graph representations.
 Home-page: UNKNOWN
 Author: PLN-disca-iimas
 Author-email: andric.valdez@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `text2graphapi-0.1.5/text2graphapi.egg-info/SOURCES.txt` & `text2graphapi-0.1.6/text2graphapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

