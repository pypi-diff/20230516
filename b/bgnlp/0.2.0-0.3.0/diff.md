# Comparing `tmp/bgnlp-0.2.0.tar.gz` & `tmp/bgnlp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgnlp-0.2.0.tar", last modified: Mon May  8 09:18:36 2023, max compression
+gzip compressed data, was "bgnlp-0.3.0.tar", last modified: Tue May 16 15:53:56 2023, max compression
```

## Comparing `bgnlp-0.2.0.tar` & `bgnlp-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 09:18:25.000000 bgnlp-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 09:18:25.000000 bgnlp-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 09:18:36.782844 bgnlp-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-08 09:18:25.000000 bgnlp-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/models/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/serialized/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/serialized/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/serialized/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/serialized/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/serialized/vocabs/
--rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/serialized/vocabs/cb-vocab.pt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    20468 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/taggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-08 09:18:25.000000 bgnlp-0.2.0/bgnlp/tools/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:18:36.782844 bgnlp-0.2.0/bgnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 09:18:36.000000 bgnlp-0.2.0/bgnlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 09:18:25.000000 bgnlp-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:18:36.782844 bgnlp-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-08 09:18:25.000000 bgnlp-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 15:53:44.000000 bgnlp-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 15:53:44.000000 bgnlp-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-16 15:53:56.202476 bgnlp-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-16 15:53:44.000000 bgnlp-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.198475 bgnlp-0.3.0/bgnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/models/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/serialized/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/serialized/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/serialized/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/serialized/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/serialized/vocabs/
+-rw-r--r--   0 runner    (1001) docker     (123)    82097 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/serialized/vocabs/cb-vocab.pt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.202476 bgnlp-0.3.0/bgnlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/taggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-16 15:53:44.000000 bgnlp-0.3.0/bgnlp/tools/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:53:56.198475 bgnlp-0.3.0/bgnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 15:53:56.000000 bgnlp-0.3.0/bgnlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 15:53:44.000000 bgnlp-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:53:56.202476 bgnlp-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-16 15:53:44.000000 bgnlp-0.3.0/setup.py
```

### Comparing `bgnlp-0.2.0/LICENSE` & `bgnlp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/PKG-INFO` & `bgnlp-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
@@ -30,14 +30,23 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)](https://pypi.org/project/bgnlp/)
 
 ```sh
 pip install bgnlp
 ```
 
 ## Package functionalities
+- [Part-of-speech](#pos)
+- [Lemmatization](#lemma)
+- [Named Entity Recognition](#ner)
+- [Keyword Extraction](#keywords)
+
+> Please note - only the first time you run one of these operations a model will be downloaded! Therefore, the first run might take more time.
+
+
+<a id="pos"></a>
 
 ### Part-of-speech (PoS) tagging
 
 ```python
 from bgnlp import pos
 
 
@@ -89,14 +98,16 @@
     "word": ".",
     "tag": "U",
     "bg_desc": "препинателен знак",
     "en_desc": "punctuation"
 }]
 ```
 
+<a id="lemma"></a>
+
 ### Lemmatization
 
 ```python
 from bgnlp import lemmatize
 
 
 text = "Добре дошли!"
@@ -112,14 +123,16 @@
 print(lemmatize(text, as_string=True))
 ```
 
 ```bash
 Добре дойда!
 ```
 
+<a id="ner"></a>
+
 ### Named Entity Recognition (NER) tagging
 
 Currently, the available NER tags are:
 - `PER` - Person
 - `ORG` - Organization
 - `LOC` - Location
 
@@ -135,26 +148,32 @@
 
 ```bash
 Input: Барух Спиноза е роден в Амстердам
 Result: [{'word': 'Барух Спиноза', 'entity_group': 'PER'}, {'word': 'Амстердам', 'entity_group': 'LOC'}]
 ```
 
 
-### Using a Config object
-A tagger Config is used to define the underlying model. 
+<a id="keywords"></a>
 
-You can change the device on which it makes inference:
+### Keyword Extraction
 ```python
-# Make inference using the GPU (by default it is "cpu"):
-config = NerTaggerConfig(device="cuda")
-ner = NerTagger(config=config)
-# ...
-```
+from bgnlp import extract_keywords
 
-You can also change the path to the model weights. For `NerTagger` you can directly pass the HuggingFace's Model Hub path. All other taggers use weights uploaded to Google Drive.
-```python
-# Define the path to the model weights. It can be a single .pt file or a path to HuggingFace's Model Hub (only for NerTagger).
-config = NerTaggerConfig(model_path="path/to/model")
-ner = NerTagger(config=config)
-# ...
+
+# Reading the text from a file, since it may be large, hence it wouldn't be 
+# pleasant to write it directly here.
+# The current input is this Bulgarian news article (only the text, no HTML!):
+# https://novini.bg/sviat/eu/781622
+with open("input_text.txt", "r", encoding="utf-8") as f:
+    text = f.read()
+
+# Extracting keywords with probability of at least 0.5.
+keywords = extract_keywords(text, threshold=0.5)
+print("Keywords:")
+pprint(keywords)
+```
+```bash
+Keywords:
+[{'keyword': 'Еманюел Макрон', 'score': 0.8759163320064545},
+ {'keyword': 'Г-7', 'score': 0.5938143730163574},
+ {'keyword': 'Япония', 'score': 0.607077419757843}]
 ```
-Please, note that the model should be of the same architecture as the one used by the certain Tagger.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.2.0 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.3.0 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -13,45 +13,48 @@
 Python :: 3.10 Classifier: Operating System :: Unix Classifier: Operating
 System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown License-File: LICENSE # **bgnlp**:
 Model-first approach to Bulgarian NLP [Open_In_Colab] [![Downloads](https://
 static.pepy.tech/personalized-badge/
 bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)]
 (https://pypi.org/project/bgnlp/) ```sh pip install bgnlp ``` ## Package
-functionalities ### Part-of-speech (PoS) tagging ```python from bgnlp import
-pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð°
-ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag":
-"PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word":
-"Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" },
-{ "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°",
-"tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word":
-"Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
-Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc":
-"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½",
-"tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
-"adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": ".", "tag":
-"U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation"
-}] ``` ### Lemmatization ```python from bgnlp import lemmatize text =
-"ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word':
-'ÐÐ¾Ð±ÑÐµ', 'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma':
-'Ð´Ð¾Ð¹Ð´Ð°'}, {'word': '!', 'lemma': '!'}] ``` ```python # Generating a string
-of lemmas. print(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
-Ð´Ð¾Ð¹Ð´Ð°! ``` ### Named Entity Recognition (NER) tagging Currently, the
-available NER tags are: - `PER` - Person - `ORG` - Organization - `LOC` -
-Location ```python from bgnlp import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ
-ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner
-(text)) ``` ```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
-ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼ Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°',
-'entity_group': 'PER'}, {'word': 'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}]
-``` ### Using a Config object A tagger Config is used to define the underlying
-model. You can change the device on which it makes inference: ```python # Make
-inference using the GPU (by default it is "cpu"): config = NerTaggerConfig
-(device="cuda") ner = NerTagger(config=config) # ... ``` You can also change
-the path to the model weights. For `NerTagger` you can directly pass the
-HuggingFace's Model Hub path. All other taggers use weights uploaded to Google
-Drive. ```python # Define the path to the model weights. It can be a single .pt
-file or a path to HuggingFace's Model Hub (only for NerTagger). config =
-NerTaggerConfig(model_path="path/to/model") ner = NerTagger(config=config) #
-... ``` Please, note that the model should be of the same architecture as the
-one used by the certain Tagger.
+functionalities - [Part-of-speech](#pos) - [Lemmatization](#lemma) - [Named
+Entity Recognition](#ner) - [Keyword Extraction](#keywords) > Please note -
+only the first time you run one of these operations a model will be downloaded!
+Therefore, the first run might take more time.  ### Part-of-speech (PoS)
+tagging ```python from bgnlp import pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ
+Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð° ÐµÑÑÐµÑÑÐ²ÐµÐ½
+ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag": "PDOsn", "bg_desc":
+"Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word": "Ðµ", "tag":
+"VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" }, { "word":
+"Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
+Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°", "tag": "R", "bg_desc":
+"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°",
+"tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
+"noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc":
+"preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½", "tag": "Asmo", "bg_desc":
+"Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "adjective" }, { "word":
+"ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ",
+"en_desc": "noun" }, { "word": ".", "tag": "U", "bg_desc":
+"Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation" }] ```  ###
+Lemmatization ```python from bgnlp import lemmatize text = "ÐÐ¾Ð±ÑÐµ
+Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word': 'ÐÐ¾Ð±ÑÐµ',
+'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma': 'Ð´Ð¾Ð¹Ð´Ð°'}, {'word':
+'!', 'lemma': '!'}] ``` ```python # Generating a string of lemmas. print
+(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ Ð´Ð¾Ð¹Ð´Ð°! ```  ###
+Named Entity Recognition (NER) tagging Currently, the available NER tags are: -
+`PER` - Person - `ORG` - Organization - `LOC` - Location ```python from bgnlp
+import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
+ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner(text)) ```
+```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼
+Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°', 'entity_group': 'PER'}, {'word':
+'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}] ```  ### Keyword Extraction
+```python from bgnlp import extract_keywords # Reading the text from a file,
+since it may be large, hence it wouldn't be # pleasant to write it directly
+here. # The current input is this Bulgarian news article (only the text, no
+HTML!): # https://novini.bg/sviat/eu/781622 with open("input_text.txt", "r",
+encoding="utf-8") as f: text = f.read() # Extracting keywords with probability
+of at least 0.5. keywords = extract_keywords(text, threshold=0.5) print
+("Keywords:") pprint(keywords) ``` ```bash Keywords: [{'keyword':
+'ÐÐ¼Ð°Ð½ÑÐµÐ» ÐÐ°ÐºÑÐ¾Ð½', 'score': 0.8759163320064545}, {'keyword': 'Ð-
+7', 'score': 0.5938143730163574}, {'keyword': 'Ð¯Ð¿Ð¾Ð½Ð¸Ñ', 'score':
+0.607077419757843}] ```
```

### Comparing `bgnlp-0.2.0/README.md` & `bgnlp-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)](https://pypi.org/project/bgnlp/)
 
 ```sh
 pip install bgnlp
 ```
 
 ## Package functionalities
+- [Part-of-speech](#pos)
+- [Lemmatization](#lemma)
+- [Named Entity Recognition](#ner)
+- [Keyword Extraction](#keywords)
+
+> Please note - only the first time you run one of these operations a model will be downloaded! Therefore, the first run might take more time.
+
+
+<a id="pos"></a>
 
 ### Part-of-speech (PoS) tagging
 
 ```python
 from bgnlp import pos
 
 
@@ -63,14 +72,16 @@
     "word": ".",
     "tag": "U",
     "bg_desc": "препинателен знак",
     "en_desc": "punctuation"
 }]
 ```
 
+<a id="lemma"></a>
+
 ### Lemmatization
 
 ```python
 from bgnlp import lemmatize
 
 
 text = "Добре дошли!"
@@ -86,14 +97,16 @@
 print(lemmatize(text, as_string=True))
 ```
 
 ```bash
 Добре дойда!
 ```
 
+<a id="ner"></a>
+
 ### Named Entity Recognition (NER) tagging
 
 Currently, the available NER tags are:
 - `PER` - Person
 - `ORG` - Organization
 - `LOC` - Location
 
@@ -109,26 +122,32 @@
 
 ```bash
 Input: Барух Спиноза е роден в Амстердам
 Result: [{'word': 'Барух Спиноза', 'entity_group': 'PER'}, {'word': 'Амстердам', 'entity_group': 'LOC'}]
 ```
 
 
-### Using a Config object
-A tagger Config is used to define the underlying model. 
+<a id="keywords"></a>
 
-You can change the device on which it makes inference:
+### Keyword Extraction
 ```python
-# Make inference using the GPU (by default it is "cpu"):
-config = NerTaggerConfig(device="cuda")
-ner = NerTagger(config=config)
-# ...
-```
+from bgnlp import extract_keywords
 
-You can also change the path to the model weights. For `NerTagger` you can directly pass the HuggingFace's Model Hub path. All other taggers use weights uploaded to Google Drive.
-```python
-# Define the path to the model weights. It can be a single .pt file or a path to HuggingFace's Model Hub (only for NerTagger).
-config = NerTaggerConfig(model_path="path/to/model")
-ner = NerTagger(config=config)
-# ...
+
+# Reading the text from a file, since it may be large, hence it wouldn't be 
+# pleasant to write it directly here.
+# The current input is this Bulgarian news article (only the text, no HTML!):
+# https://novini.bg/sviat/eu/781622
+with open("input_text.txt", "r", encoding="utf-8") as f:
+    text = f.read()
+
+# Extracting keywords with probability of at least 0.5.
+keywords = extract_keywords(text, threshold=0.5)
+print("Keywords:")
+pprint(keywords)
+```
+```bash
+Keywords:
+[{'keyword': 'Еманюел Макрон', 'score': 0.8759163320064545},
+ {'keyword': 'Г-7', 'score': 0.5938143730163574},
+ {'keyword': 'Япония', 'score': 0.607077419757843}]
 ```
-Please, note that the model should be of the same architecture as the one used by the certain Tagger.
```

#### html2text {}

```diff
@@ -1,42 +1,45 @@
 # **bgnlp**: Model-first approach to Bulgarian NLP [Open_In_Colab] [!
 [Downloads](https://static.pepy.tech/personalized-badge/
 bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)]
 (https://pypi.org/project/bgnlp/) ```sh pip install bgnlp ``` ## Package
-functionalities ### Part-of-speech (PoS) tagging ```python from bgnlp import
-pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð°
-ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag":
-"PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word":
-"Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" },
-{ "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°",
-"tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word":
-"Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
-Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc":
-"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½",
-"tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
-"adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": ".", "tag":
-"U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation"
-}] ``` ### Lemmatization ```python from bgnlp import lemmatize text =
-"ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word':
-'ÐÐ¾Ð±ÑÐµ', 'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma':
-'Ð´Ð¾Ð¹Ð´Ð°'}, {'word': '!', 'lemma': '!'}] ``` ```python # Generating a string
-of lemmas. print(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
-Ð´Ð¾Ð¹Ð´Ð°! ``` ### Named Entity Recognition (NER) tagging Currently, the
-available NER tags are: - `PER` - Person - `ORG` - Organization - `LOC` -
-Location ```python from bgnlp import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ
-ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner
-(text)) ``` ```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
-ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼ Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°',
-'entity_group': 'PER'}, {'word': 'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}]
-``` ### Using a Config object A tagger Config is used to define the underlying
-model. You can change the device on which it makes inference: ```python # Make
-inference using the GPU (by default it is "cpu"): config = NerTaggerConfig
-(device="cuda") ner = NerTagger(config=config) # ... ``` You can also change
-the path to the model weights. For `NerTagger` you can directly pass the
-HuggingFace's Model Hub path. All other taggers use weights uploaded to Google
-Drive. ```python # Define the path to the model weights. It can be a single .pt
-file or a path to HuggingFace's Model Hub (only for NerTagger). config =
-NerTaggerConfig(model_path="path/to/model") ner = NerTagger(config=config) #
-... ``` Please, note that the model should be of the same architecture as the
-one used by the certain Tagger.
+functionalities - [Part-of-speech](#pos) - [Lemmatization](#lemma) - [Named
+Entity Recognition](#ner) - [Keyword Extraction](#keywords) > Please note -
+only the first time you run one of these operations a model will be downloaded!
+Therefore, the first run might take more time.  ### Part-of-speech (PoS)
+tagging ```python from bgnlp import pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ
+Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð° ÐµÑÑÐµÑÑÐ²ÐµÐ½
+ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag": "PDOsn", "bg_desc":
+"Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word": "Ðµ", "tag":
+"VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" }, { "word":
+"Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
+Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°", "tag": "R", "bg_desc":
+"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°",
+"tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
+"noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc":
+"preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½", "tag": "Asmo", "bg_desc":
+"Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "adjective" }, { "word":
+"ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ",
+"en_desc": "noun" }, { "word": ".", "tag": "U", "bg_desc":
+"Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation" }] ```  ###
+Lemmatization ```python from bgnlp import lemmatize text = "ÐÐ¾Ð±ÑÐµ
+Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word': 'ÐÐ¾Ð±ÑÐµ',
+'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma': 'Ð´Ð¾Ð¹Ð´Ð°'}, {'word':
+'!', 'lemma': '!'}] ``` ```python # Generating a string of lemmas. print
+(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ Ð´Ð¾Ð¹Ð´Ð°! ```  ###
+Named Entity Recognition (NER) tagging Currently, the available NER tags are: -
+`PER` - Person - `ORG` - Organization - `LOC` - Location ```python from bgnlp
+import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
+ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner(text)) ```
+```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼
+Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°', 'entity_group': 'PER'}, {'word':
+'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}] ```  ### Keyword Extraction
+```python from bgnlp import extract_keywords # Reading the text from a file,
+since it may be large, hence it wouldn't be # pleasant to write it directly
+here. # The current input is this Bulgarian news article (only the text, no
+HTML!): # https://novini.bg/sviat/eu/781622 with open("input_text.txt", "r",
+encoding="utf-8") as f: text = f.read() # Extracting keywords with probability
+of at least 0.5. keywords = extract_keywords(text, threshold=0.5) print
+("Keywords:") pprint(keywords) ``` ```bash Keywords: [{'keyword':
+'ÐÐ¼Ð°Ð½ÑÐµÐ» ÐÐ°ÐºÑÐ¾Ð½', 'score': 0.8759163320064545}, {'keyword': 'Ð-
+7', 'score': 0.5938143730163574}, {'keyword': 'Ð¯Ð¿Ð¾Ð½Ð¸Ñ', 'score':
+0.607077419757843}] ```
```

### Comparing `bgnlp-0.2.0/bgnlp/models/bert.py` & `bgnlp-0.3.0/bgnlp/models/bert.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/bgnlp/models/seq2seq.py` & `bgnlp-0.3.0/bgnlp/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/bgnlp/serialized/vocabs/cb-vocab.pt` & `bgnlp-0.3.0/bgnlp/serialized/vocabs/cb-vocab.pt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/bgnlp/tools/configs.py` & `bgnlp-0.3.0/bgnlp/tools/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,7 +43,15 @@
 
 @dataclass
 class NerTaggerConfig(ModelConfig):
     device: str = "cpu"
     # Since I have uploaded this model to Huggingface's Model Hub, it is being 
     # downloaded only using this model ID:
     model_path: str = "auhide/bert-bg-ner"
+
+
+@dataclass
+class KeywordsTaggerConfig(ModelConfig):
+    device: str = "cpu"
+    # Since I have uploaded this model to Huggingface's Model Hub, it is being 
+    # downloaded only using this model ID:
+    model_path: str = "auhide/keybert-bg"
```

### Comparing `bgnlp-0.2.0/bgnlp/tools/mappings.py` & `bgnlp-0.3.0/bgnlp/tools/mappings.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/bgnlp/tools/mixins.py` & `bgnlp-0.3.0/bgnlp/tools/mixins.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/bgnlp/tools/taggers.py` & `bgnlp-0.3.0/bgnlp/tools/taggers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Natural language Taggers for Bulgarian. They are all model-based.
 """
 import os
 import re
-from typing import List, Dict
+from typing import List, Dict, Any
 from abc import ABC, abstractmethod
 
 import torch
 from torch import nn
 import gdown
 from transformers import logging
 from transformers import AutoTokenizer, AutoModelForTokenClassification
 
 from bgnlp.models import LemmaBert
 from bgnlp.tools.mixins import SubwordMixin
 from bgnlp.tools.tokenizers import (
     CharacterBasedPreTokenizer, CharacterBasedTokenizer
 )
-from bgnlp.tools.configs import LemmaTaggerConfig, ModelConfig, PosTaggerConfig
+from bgnlp.tools.configs import ModelConfig, PosTaggerConfig
 
 
 # Logging only error messages from HuggingFace.
 logging.set_verbosity_error()
 
 
 class BaseTagger(ABC):
@@ -123,17 +123,15 @@
             max_len (int, optional): The maximum number of words that you can have in `text`. Defaults to 64.
 
         Returns:
             List[Dict[str, str]]: List of dictionaries for each word and its tags.
 
         Example::
 
-            >>> from bgnlp import PosTagger, PosTaggerConfig
-            >>> config = PosTaggerConfig()
-            >>> pos = PosTagger(config=config)
+            >>> from bgnlp import pos
             >>> pos("Това е библиотека за обработка на естествен език.")
             [{
                 "word": "Това",
                 "tag": "PDOsn",
                 "bg_desc": "местоимение",
                 "en_desc": "pronoun"
             }, {
@@ -432,25 +430,23 @@
             as_string(str): Whether the lemmatization result should be a string or a dictionary.
             additional_info (bool, optional): Whether the output should constist of more data about each word (mainly PoS information). Defaults to False.
 
         Returns:
             List[Dict[str, str]]: List of dictionaries. Each dictionary has a word and a `lemma` key with a value - its lemma. If `additional_info`=True, the dictionary has PoS data.
 
         Example::
-            >>> from bgnlp import LemmaTaggerConfig, LemmaTagger
-            >>> lemma = LemmaTagger(config=LemmaTaggerConfig())
+            >>> from bgnlp import lemmatize
             >>> text = "Добре дошли!"
+            >>> # Return the lemmas as a dictionary.
             >>> print("Input:", text)
-            >>> print("Output:", lemma(text))
+            >>> print("Output:", lemmatize(text))
             [{'word': 'Добре', 'lemma': 'Добре'}, {'word': 'дошли', 'lemma': 'дойда'}, {'word': '!', 'lemma': '!'}]
 
-            >>> lemma = LemmaTagger(config=LemmaTaggerConfig())
-            >>> text = "Добре дошли!"
-            >>> print("Input:", text)
-            >>> print("Output:", lemma(text, as_string=True))
+            >>> # Or return the lemmas as a string.
+            >>> print("Output:", lemmatize(text, as_string=True))
             Input: Добре дошли!
             Output: Добре дойда!
         """
         self.additional_info = additional_info
 
         pos = PosTagger(config=PosTaggerConfig())
         lemma = Lemmatizer(config=self.config)
@@ -546,20 +542,16 @@
         Args:
             text (str): String of Bulgarian words.
 
         Returns:
             List[Dict[str, str]]: List of dictionaries. Each dictionary has a word and its NER tag.
 
         Example::
-            >>> from bgnlp import NerTagger, NerTaggerConfig
-
-
-            >>> ner = NerTagger(config=NerTaggerConfig())
+            >>> from bgnlp import ner
             >>> text = "Барух Спиноза е роден в Амстердам"
-
             >>> print(f"Input: {text}")
             >>> print("Result:", ner(text))
             Input: Барух Спиноза е роден в Амстердам
             Result: [{'word': 'Барух Спиноза', 'entity_group': 'PER'}, {'word': 'Амстердам', 'entity_group': 'LOC'}]
 
         """
         return self.predict(text)
@@ -622,7 +614,184 @@
                         "word": curr_word,
                         "entity_group": entities[i][2:]
                     })
                 
                 curr_word = []
 
         return result
+
+
+class KeywordsTagger(BaseTagger):
+    """Keyword Extraction tagger for Bulgarian texts.
+
+    Args:
+        config (ModelConfig): The model configuration.
+    """
+
+    def __init__(self, config: ModelConfig):
+        self.config = config
+        self.model = self.get_model()
+        self.tokenizer = self.get_tokenizer()
+
+    def __call__(self, text: str, threshold: float = 0.5) -> List[Dict[str, Any]]:
+        """Extract keywords from Bulgarian texts.
+
+        Args:
+            text (str): The source text from which you are going to extract.
+            threshold (float, optional): Threshold based on which some of the keywords with lower probabilties might be excluded. Defaults to 0.5.
+        
+        Returns:
+            List[Dict[str, Any]]: List of dictionaries describing each keyword in `text`.
+
+        Example::
+            >>> from bgnlp import extract_keywords
+            >>> with open("input_text.txt", "r", encoding="utf-8") as f:
+            >>>     text = f.read()
+            >>> # Here threshold is optional, it defaults to 0.5.
+            >>> extract_keywords(text, threshold=0.6)
+            [{'keyword': 'Еманюел Макрон', 'score': 0.8759163320064545},
+            {'keyword': 'Г-7', 'score': 0.5938143730163574},
+            {'keyword': 'Япония', 'score': 0.607077419757843}]
+        """
+        return self.predict(text, threshold)
+
+    def get_tokenizer(self):
+        return AutoTokenizer.from_pretrained(self.config.model_path)
+
+    def get_model(self):
+        return AutoModelForTokenClassification.from_pretrained(self.config.model_path)
+
+    def predict(self, text: str, threshold: float = 0.5) -> List[Dict[str, Any]]:
+        """Extract keywords from Bulgarian texts.
+
+        Args:
+            text (str): The source text from which you are going to extract.
+            threshold (float, optional): Threshold based on which some of the keywords with lower probabilties might be excluded. Defaults to 0.5.
+        
+        Returns:
+            List[Dict[str, Any]]: List of dictionaries describing each keyword in `text`.
+
+        Example::
+            >>> from bgnlp import extract_keywords
+            >>> with open("input_text.txt", "r", encoding="utf-8") as f:
+            >>>     text = f.read()
+            >>> # Here threshold is optional, it defaults to 0.5.
+            >>> extract_keywords(text, threshold=0.6)
+            [{'keyword': 'Еманюел Макрон', 'score': 0.8759163320064545},
+            {'keyword': 'Г-7', 'score': 0.5938143730163574},
+            {'keyword': 'Япония', 'score': 0.607077419757843}]
+        """
+        keywords = self._extract_keywords(text, threshold=threshold)
+
+        return self._format_keywords(keywords)
+    
+    def _format_keywords(self, keywords: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+        """Mainly responsible for the merging of subkeywords into keywords, i.e. when
+        the keyword consists of multiple words - 'Адам Фаузи', the two subkeywords 'Адам' and 'Фаузи'
+        are merged into one. This method also merges the probabilities by calculating
+        their average.
+
+        Args:
+            keywords (List[Dict[str, Any]]): Keywords with their `entity_group` and probability `score`.
+
+        Returns:
+            List[Dict[str, Any]]: Merged keywords (in some cases) with their probability scores.
+        """
+        formatted_keywords = []
+        # This is used for keywords that have multiple words.
+        current_keywords = []
+        scores = []
+
+        for i, kw in enumerate(keywords):
+            if kw["entity_group"] == "B-KWD":
+                if i > 0:
+                    formatted_keywords.append({
+                        "keyword": " ".join(current_keywords),
+                        # Calculating the average score of all keywords in `current_keywords`.
+                        "score": sum(scores) / len(scores)
+                    })
+                current_keywords = []
+                scores = []
+                current_keywords.append(kw["entity"])
+                scores.append(kw["score"])
+
+            if kw["entity_group"] == "I-KWD":
+                current_keywords.append(kw["entity"])
+                scores.append(kw["score"])
+
+            # When the last keyword is of any type - it should be added to 
+            # `formatted_keywords`.
+            if i == len(keywords) - 1:
+                formatted_keywords.append({
+                    "keyword": " ".join(current_keywords),
+                    # Calculating the average score of all keywords in `current_keywords`.
+                    "score": sum(scores) / len(scores)
+                })
+
+        return formatted_keywords
+
+    def _extract_keywords(
+        self,
+        text: str,
+        max_len: int = 300,
+        id2group = {
+            # Indicates that this is not a keyword.
+            0: "O",
+            # Begining of keyword.
+            1: "B-KWD",
+            # Additional keywords (might also indicate the end of a keyword sequence).
+            # You can merge these with the begining keyword `B-KWD`.
+            2: "I-KWD",
+        },
+        threshold: float = 0.5
+    ) -> List[Dict[str, Any]]:
+        """Here the text is preprocessed, tokenized and then sent to the model
+        for inference. There are comments on each step.
+
+        Args:
+            text (str): Raw text.
+            max_len (int, optional): Maximum sequence length passed to the tokenizer. Defaults to 300.
+            id2group (dict, optional): ID to Group mapping for the entity groups. Defaults to { 0: "O", 1: "B-KWD", 2: "I-KWD", }.
+            threshold (float, optional): Threshold based on which some of the keywords with lower probabilties might be excluded. Defaults to 0.5.
+
+        Returns:
+            List[Dict[str, Any]]: Each found entity/keyword with its entity group and probability score.
+        """
+        # Preprocess the text.
+        # Surround punctuation with whitespace and convert multiple whitespaces
+        # into single ones.
+        text = re.sub(r"([,\.?!;:\'\"\(\)\[\]„”])", r" \1 ", text)
+        text = re.sub(r"\s+", r" ", text)
+        words = text.split()
+
+        # Tokenize the processed `text` (this includes padding or truncation).
+        tokens_data = self.tokenizer(
+            text.strip(), 
+            padding="max_length", 
+            max_length=max_len, 
+            truncation=True, 
+            return_tensors="pt"
+        )
+        input_ids = tokens_data.input_ids
+        attention_mask = tokens_data.attention_mask
+
+        # Predict the keywords.
+        out = self.model(input_ids, attention_mask=attention_mask).logits
+        # Softmax the last dimension so that the probabilities add up to 1.0.
+        out = out.softmax(-1)
+        # Based on the probabilities, generate the most probable keywords.
+        out_argmax = out.argmax(-1)
+        prediction = out_argmax.squeeze(0).tolist()
+        probabilities = out.squeeze(0)
+        
+        return [
+            {
+                # Since the list of words does not have a [CLS] token, the index `i`
+                # is one step forward, which means that if we want to access the 
+                # appropriate keyword we should use the index `i - 1`.
+                "entity": words[i - 1],
+                "entity_group": id2group[idx],
+                "score": float(probabilities[i, idx])
+            } 
+            for i, idx in enumerate(prediction) 
+            if (idx == 1 or idx == 2) and float(probabilities[i, idx]) > threshold
+        ]
```

### Comparing `bgnlp-0.2.0/bgnlp/tools/tokenizers.py` & `bgnlp-0.3.0/bgnlp/tools/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/bgnlp.egg-info/PKG-INFO` & `bgnlp-0.3.0/bgnlp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgnlp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package for Bulgarian Natural Language Processing (NLP)
 Author: Adam Fauzi
 Author-email: adamfzh98@gmail.com
 Keywords: pytorch,nlp,bulgaria,machine learning,deep learning,AI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
@@ -30,14 +30,23 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)](https://pypi.org/project/bgnlp/)
 
 ```sh
 pip install bgnlp
 ```
 
 ## Package functionalities
+- [Part-of-speech](#pos)
+- [Lemmatization](#lemma)
+- [Named Entity Recognition](#ner)
+- [Keyword Extraction](#keywords)
+
+> Please note - only the first time you run one of these operations a model will be downloaded! Therefore, the first run might take more time.
+
+
+<a id="pos"></a>
 
 ### Part-of-speech (PoS) tagging
 
 ```python
 from bgnlp import pos
 
 
@@ -89,14 +98,16 @@
     "word": ".",
     "tag": "U",
     "bg_desc": "препинателен знак",
     "en_desc": "punctuation"
 }]
 ```
 
+<a id="lemma"></a>
+
 ### Lemmatization
 
 ```python
 from bgnlp import lemmatize
 
 
 text = "Добре дошли!"
@@ -112,14 +123,16 @@
 print(lemmatize(text, as_string=True))
 ```
 
 ```bash
 Добре дойда!
 ```
 
+<a id="ner"></a>
+
 ### Named Entity Recognition (NER) tagging
 
 Currently, the available NER tags are:
 - `PER` - Person
 - `ORG` - Organization
 - `LOC` - Location
 
@@ -135,26 +148,32 @@
 
 ```bash
 Input: Барух Спиноза е роден в Амстердам
 Result: [{'word': 'Барух Спиноза', 'entity_group': 'PER'}, {'word': 'Амстердам', 'entity_group': 'LOC'}]
 ```
 
 
-### Using a Config object
-A tagger Config is used to define the underlying model. 
+<a id="keywords"></a>
 
-You can change the device on which it makes inference:
+### Keyword Extraction
 ```python
-# Make inference using the GPU (by default it is "cpu"):
-config = NerTaggerConfig(device="cuda")
-ner = NerTagger(config=config)
-# ...
-```
+from bgnlp import extract_keywords
 
-You can also change the path to the model weights. For `NerTagger` you can directly pass the HuggingFace's Model Hub path. All other taggers use weights uploaded to Google Drive.
-```python
-# Define the path to the model weights. It can be a single .pt file or a path to HuggingFace's Model Hub (only for NerTagger).
-config = NerTaggerConfig(model_path="path/to/model")
-ner = NerTagger(config=config)
-# ...
+
+# Reading the text from a file, since it may be large, hence it wouldn't be 
+# pleasant to write it directly here.
+# The current input is this Bulgarian news article (only the text, no HTML!):
+# https://novini.bg/sviat/eu/781622
+with open("input_text.txt", "r", encoding="utf-8") as f:
+    text = f.read()
+
+# Extracting keywords with probability of at least 0.5.
+keywords = extract_keywords(text, threshold=0.5)
+print("Keywords:")
+pprint(keywords)
+```
+```bash
+Keywords:
+[{'keyword': 'Еманюел Макрон', 'score': 0.8759163320064545},
+ {'keyword': 'Г-7', 'score': 0.5938143730163574},
+ {'keyword': 'Япония', 'score': 0.607077419757843}]
 ```
-Please, note that the model should be of the same architecture as the one used by the certain Tagger.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bgnlp Version: 0.2.0 Summary: Package for Bulgarian
+Metadata-Version: 2.1 Name: bgnlp Version: 0.3.0 Summary: Package for Bulgarian
 Natural Language Processing (NLP) Author: Adam Fauzi Author-email:
 adamfzh98@gmail.com Keywords: pytorch,nlp,bulgaria,machine learning,deep
 learning,AI Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries Classifier:
@@ -13,45 +13,48 @@
 Python :: 3.10 Classifier: Operating System :: Unix Classifier: Operating
 System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown License-File: LICENSE # **bgnlp**:
 Model-first approach to Bulgarian NLP [Open_In_Colab] [![Downloads](https://
 static.pepy.tech/personalized-badge/
 bgnlp?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pip%20downloads)]
 (https://pypi.org/project/bgnlp/) ```sh pip install bgnlp ``` ## Package
-functionalities ### Part-of-speech (PoS) tagging ```python from bgnlp import
-pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð°
-ÐµÑÑÐµÑÑÐ²ÐµÐ½ ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag":
-"PDOsn", "bg_desc": "Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word":
-"Ðµ", "tag": "VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" },
-{ "word": "Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°",
-"tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word":
-"Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
-Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc":
-"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½",
-"tag": "Asmo", "bg_desc": "Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
-"adjective" }, { "word": "ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc":
-"ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": ".", "tag":
-"U", "bg_desc": "Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation"
-}] ``` ### Lemmatization ```python from bgnlp import lemmatize text =
-"ÐÐ¾Ð±ÑÐµ Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word':
-'ÐÐ¾Ð±ÑÐµ', 'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma':
-'Ð´Ð¾Ð¹Ð´Ð°'}, {'word': '!', 'lemma': '!'}] ``` ```python # Generating a string
-of lemmas. print(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ
-Ð´Ð¾Ð¹Ð´Ð°! ``` ### Named Entity Recognition (NER) tagging Currently, the
-available NER tags are: - `PER` - Person - `ORG` - Organization - `LOC` -
-Location ```python from bgnlp import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ
-ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner
-(text)) ``` ```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
-ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼ Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°',
-'entity_group': 'PER'}, {'word': 'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}]
-``` ### Using a Config object A tagger Config is used to define the underlying
-model. You can change the device on which it makes inference: ```python # Make
-inference using the GPU (by default it is "cpu"): config = NerTaggerConfig
-(device="cuda") ner = NerTagger(config=config) # ... ``` You can also change
-the path to the model weights. For `NerTagger` you can directly pass the
-HuggingFace's Model Hub path. All other taggers use weights uploaded to Google
-Drive. ```python # Define the path to the model weights. It can be a single .pt
-file or a path to HuggingFace's Model Hub (only for NerTagger). config =
-NerTaggerConfig(model_path="path/to/model") ner = NerTagger(config=config) #
-... ``` Please, note that the model should be of the same architecture as the
-one used by the certain Tagger.
+functionalities - [Part-of-speech](#pos) - [Lemmatization](#lemma) - [Named
+Entity Recognition](#ner) - [Keyword Extraction](#keywords) > Please note -
+only the first time you run one of these operations a model will be downloaded!
+Therefore, the first run might take more time.  ### Part-of-speech (PoS)
+tagging ```python from bgnlp import pos print(pos("Ð¢Ð¾Ð²Ð° Ðµ
+Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ° Ð·Ð° Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ° Ð½Ð° ÐµÑÑÐµÑÑÐ²ÐµÐ½
+ÐµÐ·Ð¸Ðº.")) ``` ```json [{ "word": "Ð¢Ð¾Ð²Ð°", "tag": "PDOsn", "bg_desc":
+"Ð¼ÐµÑÑÐ¾Ð¸Ð¼ÐµÐ½Ð¸Ðµ", "en_desc": "pronoun" }, { "word": "Ðµ", "tag":
+"VLINr3s", "bg_desc": "Ð³Ð»Ð°Ð³Ð¾Ð»", "en_desc": "verb" }, { "word":
+"Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÐ°", "tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾
+Ð¸Ð¼Ðµ", "en_desc": "noun" }, { "word": "Ð·Ð°", "tag": "R", "bg_desc":
+"Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc": "preposition" }, { "word": "Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ°",
+"tag": "NCFsof", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc":
+"noun" }, { "word": "Ð½Ð°", "tag": "R", "bg_desc": "Ð¿ÑÐµÐ´Ð»Ð¾Ð³", "en_desc":
+"preposition" }, { "word": "ÐµÑÑÐµÑÑÐ²ÐµÐ½", "tag": "Asmo", "bg_desc":
+"Ð¿ÑÐ¸Ð»Ð°Ð³Ð°ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ", "en_desc": "adjective" }, { "word":
+"ÐµÐ·Ð¸Ðº", "tag": "NCMsom", "bg_desc": "ÑÑÑÐµÑÑÐ²Ð¸ÑÐµÐ»Ð½Ð¾ Ð¸Ð¼Ðµ",
+"en_desc": "noun" }, { "word": ".", "tag": "U", "bg_desc":
+"Ð¿ÑÐµÐ¿Ð¸Ð½Ð°ÑÐµÐ»ÐµÐ½ Ð·Ð½Ð°Ðº", "en_desc": "punctuation" }] ```  ###
+Lemmatization ```python from bgnlp import lemmatize text = "ÐÐ¾Ð±ÑÐµ
+Ð´Ð¾ÑÐ»Ð¸!" print(lemmatize(text)) ``` ```bash [{'word': 'ÐÐ¾Ð±ÑÐµ',
+'lemma': 'ÐÐ¾Ð±ÑÐµ'}, {'word': 'Ð´Ð¾ÑÐ»Ð¸', 'lemma': 'Ð´Ð¾Ð¹Ð´Ð°'}, {'word':
+'!', 'lemma': '!'}] ``` ```python # Generating a string of lemmas. print
+(lemmatize(text, as_string=True)) ``` ```bash ÐÐ¾Ð±ÑÐµ Ð´Ð¾Ð¹Ð´Ð°! ```  ###
+Named Entity Recognition (NER) tagging Currently, the available NER tags are: -
+`PER` - Person - `ORG` - Organization - `LOC` - Location ```python from bgnlp
+import ner text = "ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð²
+ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼" print(f"Input: {text}") print("Result:", ner(text)) ```
+```bash Input: ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð° Ðµ ÑÐ¾Ð´ÐµÐ½ Ð² ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼
+Result: [{'word': 'ÐÐ°ÑÑÑ Ð¡Ð¿Ð¸Ð½Ð¾Ð·Ð°', 'entity_group': 'PER'}, {'word':
+'ÐÐ¼ÑÑÐµÑÐ´Ð°Ð¼', 'entity_group': 'LOC'}] ```  ### Keyword Extraction
+```python from bgnlp import extract_keywords # Reading the text from a file,
+since it may be large, hence it wouldn't be # pleasant to write it directly
+here. # The current input is this Bulgarian news article (only the text, no
+HTML!): # https://novini.bg/sviat/eu/781622 with open("input_text.txt", "r",
+encoding="utf-8") as f: text = f.read() # Extracting keywords with probability
+of at least 0.5. keywords = extract_keywords(text, threshold=0.5) print
+("Keywords:") pprint(keywords) ``` ```bash Keywords: [{'keyword':
+'ÐÐ¼Ð°Ð½ÑÐµÐ» ÐÐ°ÐºÑÐ¾Ð½', 'score': 0.8759163320064545}, {'keyword': 'Ð-
+7', 'score': 0.5938143730163574}, {'keyword': 'Ð¯Ð¿Ð¾Ð½Ð¸Ñ', 'score':
+0.607077419757843}] ```
```

### Comparing `bgnlp-0.2.0/bgnlp.egg-info/SOURCES.txt` & `bgnlp-0.3.0/bgnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bgnlp-0.2.0/setup.py` & `bgnlp-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ROOT = os.path.abspath(os.path.dirname(__file__))
 README_PATH = os.path.join(ROOT, "README.md")
 REQUIREMENTS_PATH = os.path.join(ROOT, "requirements.txt")
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 DESCRIPTION = 'Package for Bulgarian Natural Language Processing (NLP)'
 
 
 def _get_requirements(path):
     with open(path, "r") as f:
         requirements_str = f.read()
         packages = re.findall(r"(.+=?=?[^\n]+)\n", requirements_str)
```

