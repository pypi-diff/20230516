# Comparing `tmp/aleph-alpha-client-3.1.0.tar.gz` & `tmp/aleph-alpha-client-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-3.1.0.tar", last modified: Wed Apr 12 13:49:55 2023, max compression
+gzip compressed data, was "aleph-alpha-client-3.1.1.tar", last modified: Tue May 16 07:18:49 2023, max compression
```

## Comparing `aleph-alpha-client-3.1.0.tar` & `aleph-alpha-client-3.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.834322 aleph-alpha-client-3.1.0/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18677 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.834322 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.561080 aleph-alpha-client-3.1.1/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.561080 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 07:18:49.000000 aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:18:49.565080 aleph-alpha-client-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-16 07:18:38.000000 aleph-alpha-client-3.1.1/tests/test_tokenize.py
```

### Comparing `aleph-alpha-client-3.1.0/LICENSE` & `aleph-alpha-client-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/PKG-INFO` & `aleph-alpha-client-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.0
+Version: 3.1.1
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.0/README.md` & `aleph-alpha-client-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/__init__.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "ExplanationResponse",
     "Image",
     "ImageControl",
     "ImagePromptItemExplanation",
     "ImageScore",
     "POOLING_OPTIONS",
     "Prompt",
+    "PromptGranularity",
     "QaRequest",
     "QaResponse",
     "QuotaError",
     "SearchRequest",
     "SearchResponse",
     "SearchResult",
     "SemanticEmbeddingRequest",
```

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/aleph_alpha_client.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/aleph_alpha_client.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/completion.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/detokenization.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/document.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/embedding.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/embedding.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/evaluation.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/explanation.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/explanation.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,26 +48,29 @@
 
     delimiter: str
 
     def to_json(self) -> Mapping[str, Any]:
         return {"type": "custom", "delimiter": self.delimiter}
 
 
-PromptGranularity = Union[
-    Literal["token"],
-    Literal["word"],
-    Literal["sentence"],
-    Literal["paragraph"],
-    CustomGranularity,
-]
+class PromptGranularity(Enum):
+    Token = "token"
+    Word = "word"
+    Sentence = "sentence"
+    Paragraph = "paragraph"
+
+    def to_json(self):
+        return {"type": self.value}
 
 
 def prompt_granularity_to_json(
-    prompt_granularity: PromptGranularity,
+    prompt_granularity: Union[PromptGranularity, str, CustomGranularity],
 ) -> Mapping[str, Any]:
+    # we allow str for backwards compatibility
+    # This was previously possible because PromptGranularity was not an Enum
     if isinstance(prompt_granularity, str):
         return {"type": prompt_granularity}
 
     return prompt_granularity.to_json()
 
 
 class TargetGranularity(Enum):
@@ -116,27 +119,33 @@
             4 token characters, would be adjusted to 1.5.
             If set to "complete", the full factor will be applied as long as the control
             overlaps with the token at all.
         control_log_additive (bool, default None)
             True: apply control by adding the log(control_factor) to attention scores.
             False: apply control by (attention_scores - - attention_scores.min(-1)) * control_factor
             If None, the API will default to True
-        prompt_granularity (PromptGranularity, default None)
+        prompt_granularity (Union[PromptGranularity, str, CustomGranularity], default None)
             At which granularity should the target be explained in terms of the prompt.
             If you choose, for example, "sentence" then we report the importance score of each
             sentence in the prompt towards generating the target output.
 
             If you do not choose a granularity then we will try to find the granularity that
             brings you closest to around 30 explanations. For large documents, this would likely
             be sentences. For short prompts this might be individual words or even tokens.
 
             If you choose a custom granularity then you must provide a custom delimiter. We then
             split your prompt by that delimiter. This might be helpful if you are using few-shot
             prompts that contain stop sequences.
 
+            We currently support providing the prompt_granularity as PromptGranularity (recommended)
+            or CustomGranularity (if needed) or str (deprecated). Note that supplying plain strings
+            only makes sense if you choose one of the values defined in the PromptGranularity enum.
+            All other strings will be rejected by the API. In future versions we might cut support
+            for plain str values.
+
             For image prompt items, the granularities determine into how many tiles we divide
             the image for the explanation.
             "token" -> 12x12
             "word" -> 6x6
             "sentence" -> 3x3
             "paragraph" -> 1
         target_granularity (TargetGranularity, default None)
@@ -157,15 +166,15 @@
 
     prompt: Prompt
     target: str
     contextual_control_threshold: Optional[float] = None
     control_factor: Optional[float] = None
     control_token_overlap: Optional[ControlTokenOverlap] = None
     control_log_additive: Optional[bool] = None
-    prompt_granularity: Optional[PromptGranularity] = None
+    prompt_granularity: Optional[Union[PromptGranularity, str, CustomGranularity]] = None
     target_granularity: Optional[TargetGranularity] = None
     postprocessing: Optional[ExplanationPostprocessing] = None
     normalize: Optional[bool] = None
 
     def to_json(self) -> Dict[str, Any]:
         payload: Dict[str, Any] = {
             "prompt": self.prompt.to_json(),
```

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/prompt.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/qa.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/search.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/summarization.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client/tokenization.py` & `aleph-alpha-client-3.1.1/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/PKG-INFO` & `aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.1.0
+Version: 3.1.1
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph-alpha-client-3.1.1/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/setup.py` & `aleph-alpha-client-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_clients.py` & `aleph-alpha-client-3.1.1/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_complete.py` & `aleph-alpha-client-3.1.1/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_detokenize.py` & `aleph-alpha-client-3.1.1/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_embed.py` & `aleph-alpha-client-3.1.1/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_error_handling.py` & `aleph-alpha-client-3.1.1/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_evaluate.py` & `aleph-alpha-client-3.1.1/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_explanation.py` & `aleph-alpha-client-3.1.1/tests/test_explanation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from pathlib import Path
-from aleph_alpha_client.explanation import TargetScoreWithRaw, TextScoreWithRaw
+from aleph_alpha_client.explanation import (
+    TargetScoreWithRaw,
+    TextScoreWithRaw,
+)
 from aleph_alpha_client.prompt import Tokens
 import pytest
 from aleph_alpha_client import (
     ControlTokenOverlap,
     ExplanationRequest,
     AsyncClient,
     Client,
@@ -50,15 +53,15 @@
     assert len(explanation.explanations) == 3
     assert all([len(exp.items) == 3 for exp in explanation.explanations])
     assert len(explanation.explanations[0].items[0].scores) == 4
 
 
 # Client
 
-
+@pytest.mark.system_test
 def test_explanation(sync_client: Client, model_name: str):
     image_source_path = Path(__file__).parent / "dog-and-cat-cover.jpg"
     img = Image.from_image_source(image_source=str(image_source_path))
 
     request = ExplanationRequest(
         prompt=Prompt(
             [
@@ -139,22 +142,19 @@
         [
             isinstance(image_score, ImageScore) and isinstance(image_score.left, int)
             for image_score in explanation.explanations[0].items[0].scores
         ]
     )
 
 
-def test_explanation_of_text_in_prompt_relativ_indeces(
-    sync_client: Client, model_name: str
-):
+def test_explanation_with_text_from_request(sync_client: Client, model_name: str):
     request = ExplanationRequest(
         prompt=Prompt(
             [
                 Text.from_text("I am a programmer and French. My favourite food is"),
-                # " My favorite food is"
                 Tokens.from_token_ids([4014, 36316, 5681, 387]),
             ]
         ),
         target=" pizza with cheese",
         prompt_granularity=None,
         target_granularity=TargetGranularity.Token,
     )
```

### Comparing `aleph-alpha-client-3.1.0/tests/test_image.py` & `aleph-alpha-client-3.1.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_prompt.py` & `aleph-alpha-client-3.1.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_qa.py` & `aleph-alpha-client-3.1.1/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_search.py` & `aleph-alpha-client-3.1.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_summarize.py` & `aleph-alpha-client-3.1.1/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.1.0/tests/test_tokenize.py` & `aleph-alpha-client-3.1.1/tests/test_tokenize.py`

 * *Files identical despite different names*

