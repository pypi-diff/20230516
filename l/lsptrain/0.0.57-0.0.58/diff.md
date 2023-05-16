# Comparing `tmp/lsptrain-0.0.57.tar.gz` & `tmp/lsptrain-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.57.tar", last modified: Thu Apr 27 08:11:48 2023, max compression
+gzip compressed data, was "lsptrain-0.0.58.tar", last modified: Tue May 16 02:25:54 2023, max compression
```

## Comparing `lsptrain-0.0.57.tar` & `lsptrain-0.0.58.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.020914 lsptrain-0.0.57/
--rw-rw-rw-   0        0        0      510 2023-04-27 08:11:48.020914 lsptrain-0.0.57/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.57/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.002915 lsptrain-0.0.57/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.57/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.011914 lsptrain-0.0.57/lsptrain/nlp_classification/
--rw-rw-rw-   0        0        0       32 2023-04-23 08:32:50.000000 lsptrain-0.0.57/lsptrain/nlp_classification/__init__.py
--rw-rw-rw-   0        0        0     9714 2023-04-23 09:11:48.000000 lsptrain-0.0.57/lsptrain/nlp_classification/model.py
--rw-rw-rw-   0        0        0     2161 2023-04-23 08:02:20.000000 lsptrain-0.0.57/lsptrain/nlp_classification/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.014914 lsptrain-0.0.57/lsptrain/nlp_classification_predictor/
--rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.57/lsptrain/nlp_classification_predictor/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.57/lsptrain/nlp_classification_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.016914 lsptrain-0.0.57/lsptrain/nlp_similarity_predictor/
--rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.57/lsptrain/nlp_similarity_predictor/__init__.py
--rw-rw-rw-   0        0        0     2060 2023-04-27 07:49:33.000000 lsptrain-0.0.57/lsptrain/nlp_similarity_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.019915 lsptrain-0.0.57/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.57/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.57/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.57/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-27 08:11:48.008916 lsptrain-0.0.57/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      510 2023-04-27 08:11:47.000000 lsptrain-0.0.57/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-04-27 08:11:47.000000 lsptrain-0.0.57/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 08:11:47.000000 lsptrain-0.0.57/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-27 08:11:47.000000 lsptrain-0.0.57/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 08:11:47.000000 lsptrain-0.0.57/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 08:11:48.020914 lsptrain-0.0.57/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-04-27 08:11:46.000000 lsptrain-0.0.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.222131 lsptrain-0.0.58/
+-rw-rw-rw-   0        0        0      510 2023-05-16 02:25:54.221134 lsptrain-0.0.58/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.58/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.198130 lsptrain-0.0.58/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.58/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.209131 lsptrain-0.0.58/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.58/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     9773 2023-05-16 02:13:43.000000 lsptrain-0.0.58/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     5321 2023-05-16 02:22:37.000000 lsptrain-0.0.58/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.211130 lsptrain-0.0.58/lsptrain/nlp_classification_predictor/
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.58/lsptrain/nlp_classification_predictor/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.58/lsptrain/nlp_classification_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.214131 lsptrain-0.0.58/lsptrain/nlp_similarity_predictor/
+-rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.58/lsptrain/nlp_similarity_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.58/lsptrain/nlp_similarity_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.219130 lsptrain-0.0.58/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.58/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.58/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.58/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:25:54.205130 lsptrain-0.0.58/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-05-16 02:25:54.000000 lsptrain-0.0.58/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-05-16 02:25:54.000000 lsptrain-0.0.58/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 02:25:54.000000 lsptrain-0.0.58/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-16 02:25:54.000000 lsptrain-0.0.58/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 02:25:54.000000 lsptrain-0.0.58/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 02:25:54.222131 lsptrain-0.0.58/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-16 02:24:51.000000 lsptrain-0.0.58/setup.py
```

### Comparing `lsptrain-0.0.57/lsptrain/nlp_classification/model.py` & `lsptrain-0.0.58/lsptrain/nlp_classification/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 
 def get_train_test_data(datas, split_data="__", max_length=args.max_length, test_size=args.test_size):
     """
     :param datas: ["样本数据__标签",]
     :param max_length: 样本最大长度，超过会自动截断
     :param test_size: 测试集比率
-    :return: X_train, X_test, y_train, y_test
+    :return: X_train, X_test, y_train, y_test, info_labels
     """
     texts = []
     labels = []
 
     for one in tqdm(datas):
         result = one.split(split_data)
         if len(result) != 2:
@@ -114,19 +114,19 @@
             texts.append(text)
             labels.append(lebal_index)
         except Exception as e:
             print(e)
             continue
     X_train, X_test, y_train, y_test = train_test_split(texts, labels, test_size=test_size, random_state=0,
                                                         shuffle=True)
-    return (X_train, y_train), (X_test, y_test)
+    return (X_train, y_train), (X_test, y_test), info_labels
 
 
 print("开始转换数据")
-(X_train, y_train), (X_test, y_test) = get_train_test_data(datas=datas, test_size=0.1)
+(X_train, y_train), (X_test, y_test), info_labels = get_train_test_data(datas=datas, test_size=0.1)
 print("完成转换数据")
 
 label_path = os.path.join(args.save_dir, args.label_file_name)
 
 with open(label_path, "w", encoding=args.encoding) as f:
     for label in info_labels:
         f.write(f"{label}\n")
@@ -177,14 +177,15 @@
         raise Exception(f"device error: {device}")
     if device and device.startswith("cuda"):
         _device = torch.device(args.device) if torch.cuda.is_available() else 'cpu'
     elif device == "cpu":
         _device = torch.device("cpu")
     else:
         _device = torch.device(args.device)
+    return _device
 
 
 model = Model(bert_model, config, len(info_labels))
 if args.device and args.device.startswith("cuda"):
     device = torch.device(args.device) if torch.cuda.is_available() else 'cpu'
 elif args.device == "cpu":
     device = torch.device("cpu")
```

### Comparing `lsptrain-0.0.57/lsptrain/nlp_classification_predictor/predictor.py` & `lsptrain-0.0.58/lsptrain/nlp_classification_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.57/lsptrain/nlp_similarity_predictor/predictor.py` & `lsptrain-0.0.58/lsptrain/nlp_similarity_predictor/predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 class TextSimilarityPredictor(object):
 
     def __init__(self, pretrained_tokenizer: str = "hfl/chinese-roberta-wwm-ext"):
         """
         :param pretrained_model: 预训练模型，默认使用 'hfl/chinese-roberta-wwm-ext'
         """
+        if not pretrained_tokenizer:
+            raise ValueError("pretrained_tokenizer input error")
         self.tokenizer = BertTokenizer.from_pretrained(pretrained_tokenizer)
 
     def compute(self, list1, list2):
         """
         计算余弦相似度，基础方法
         输入值为转换后的 tokenizer
         """
```

### Comparing `lsptrain-0.0.57/lsptrain.egg-info/SOURCES.txt` & `lsptrain-0.0.58/lsptrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.57/setup.py` & `lsptrain-0.0.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.57',
+      version='0.0.58',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch',
                         'transformers',
```

