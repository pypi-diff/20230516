# Comparing `tmp/gpt3_tokenizer-0.1.3.tar.gz` & `tmp/gpt3_tokenizer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt3_tokenizer-0.1.3.tar", max compression
+gzip compressed data, was "gpt3_tokenizer-0.1.4.tar", max compression
```

## Comparing `gpt3_tokenizer-0.1.3.tar` & `gpt3_tokenizer-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-03-24 21:26:55.598399 gpt3_tokenizer-0.1.3/LICENSE
--rw-r--r--   0        0        0      984 2023-03-24 21:26:55.598399 gpt3_tokenizer-0.1.3/README.rst
--rw-r--r--   0        0        0      125 2023-03-24 21:26:55.598399 gpt3_tokenizer-0.1.3/gpt3_tokenizer/__init__.py
--rw-r--r--   0        0        0     2015 2023-03-24 21:28:44.027028 gpt3_tokenizer-0.1.3/gpt3_tokenizer/_entry.py
--rw-r--r--   0        0        0     3282 2023-03-25 04:58:26.353945 gpt3_tokenizer-0.1.3/gpt3_tokenizer/_functions.py
--rw-r--r--   0        0        0  1042301 2023-03-24 21:26:55.606399 gpt3_tokenizer-0.1.3/gpt3_tokenizer/data/encoder.json
--rw-r--r--   0        0        0   456318 2023-03-24 21:26:55.610399 gpt3_tokenizer-0.1.3/gpt3_tokenizer/data/vocab.bpe
--rw-r--r--   0        0        0     1307 2023-03-25 04:58:50.085207 gpt3_tokenizer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 gpt3_tokenizer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/LICENSE
+-rw-r--r--   0        0        0      984 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/README.rst
+-rw-r--r--   0        0        0      125 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/gpt3_tokenizer/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/gpt3_tokenizer/_entry.py
+-rw-r--r--   0        0        0     3202 2023-05-16 00:41:06.027226 gpt3_tokenizer-0.1.4/gpt3_tokenizer/_functions.py
+-rw-r--r--   0        0        0  1042301 2023-05-16 00:41:06.035225 gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/encoder.json
+-rw-r--r--   0        0        0   456318 2023-05-16 00:41:06.039225 gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/vocab.bpe
+-rw-r--r--   0        0        0     1307 2023-05-16 00:50:16.998990 gpt3_tokenizer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 gpt3_tokenizer-0.1.4/PKG-INFO
```

### Comparing `gpt3_tokenizer-0.1.3/LICENSE` & `gpt3_tokenizer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.3/README.rst` & `gpt3_tokenizer-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.3/gpt3_tokenizer/_entry.py` & `gpt3_tokenizer-0.1.4/gpt3_tokenizer/_entry.py`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.3/gpt3_tokenizer/_functions.py` & `gpt3_tokenizer-0.1.4/gpt3_tokenizer/_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         for merge in bpe_merges:
             final_merges.append([m for m in merge if len(m.strip()) > 0])
         return final_merges
 
 def _dict_zip(x, y):
     result = {}
     for i in y:
-        key = ','.join(x[i])
-        if not isinstance(key, str):
-            key = key.decode(_DEFAULT_ENCODING)
+        key = tuple(x[i])
         result[key] = y[i]
     return result
 
 cache = {}
 
 def _encode_string(token):
     return [str(t) for t in list(bytearray(token.encode(_DEFAULT_ENCODING)))]
@@ -65,23 +63,24 @@
     pairs = _get_pairs(word)
     if not pairs:
         return token
 
     while True:
         min_pairs = {}
         for pair in pairs:
-            pair_key = ','.join(pair)
+            pair_key = tuple(pair)
             rank = bpe_ranks.get(pair_key, float("nan"))
             min_pairs[10e10 if math.isnan(rank) else rank] = pair_key
         bigram = min_pairs[min(map(int, min_pairs.keys()))]
         if not bigram in bpe_ranks:
             break
-        bigram = bigram.split(',', 1)
+        bigram = bigram[0], "".join(bigram[1:])
         first = bigram[0]
         second = bigram[1]
+
         new_word = []
         i = 0
 
         while i < len(word):
             j = -1
             try:
                 j = word.index(first, i)
```

### Comparing `gpt3_tokenizer-0.1.3/gpt3_tokenizer/data/encoder.json` & `gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/encoder.json`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.3/gpt3_tokenizer/data/vocab.bpe` & `gpt3_tokenizer-0.1.4/gpt3_tokenizer/data/vocab.bpe`

 * *Files identical despite different names*

### Comparing `gpt3_tokenizer-0.1.3/pyproject.toml` & `gpt3_tokenizer-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt3_tokenizer"
-version = "0.1.3"
+version = "0.1.4"
 description = "Encoder/Decoder and tokens counter for GPT3"
 authors = ["Alison Ferrenha"]
 readme = "README.rst"
 license = "MIT"
 keywords = ["openai", "gpt", "gpt-3", "gpt3", "gpt4", "gpt-4", "tokenizer"]
 homepage = "https://github.com/alisonjf/gpt3-tokenizer"
 repository = "https://github.com/alisonjf/gpt3-tokenizer"
```

### Comparing `gpt3_tokenizer-0.1.3/PKG-INFO` & `gpt3_tokenizer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt3-tokenizer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Encoder/Decoder and tokens counter for GPT3
 Home-page: https://github.com/alisonjf/gpt3-tokenizer
 License: MIT
 Keywords: openai,gpt,gpt-3,gpt3,gpt4,gpt-4,tokenizer
 Author: Alison Ferrenha
 Requires-Python: >=2.7
 Classifier: License :: OSI Approved :: MIT License
```

