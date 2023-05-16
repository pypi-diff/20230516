# Comparing `tmp/lambdaprompt-0.5.2.tar.gz` & `tmp/lambdaprompt-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-z5zihc3q/lambdaprompt-0.5.2.tar", last modified: Fri May 12 11:21:58 2023, max compression
+gzip compressed data, was "/home/runner/work/lambdaprompt/lambdaprompt/dist/.tmp-s7mnpc4l/lambdaprompt-0.5.3.tar", last modified: Tue May 16 06:57:26 2023, max compression
```

## Comparing `lambdaprompt-0.5.2.tar` & `lambdaprompt-0.5.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/examples/one.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/examples/two.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/examples/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/server/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/lambdaprompt/server/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/lambdaprompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:21:58.000000 lambdaprompt-0.5.2/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/library/serverexamples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/test_gpt3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-12 11:21:45.000000 lambdaprompt-0.5.2/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/examples/one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/examples/two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/examples/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/server/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/lambdaprompt/server/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/lambdaprompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:57:26.000000 lambdaprompt-0.5.3/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/library/serverexamples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/test_gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-16 06:57:17.000000 lambdaprompt-0.5.3/tests/test_server.py
```

### Comparing `lambdaprompt-0.5.2/.github/workflows/publish-to-pypi.yml` & `lambdaprompt-0.5.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/.gitignore` & `lambdaprompt-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/LICENSE` & `lambdaprompt-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/PKG-INFO` & `lambdaprompt-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.2
+Version: 0.5.3
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.2/README.md` & `lambdaprompt-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/lambdaprompt/__init__.py` & `lambdaprompt-0.5.3/lambdaprompt/__init__.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/lambdaprompt/backends.py` & `lambdaprompt-0.5.3/lambdaprompt/backends.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 
 def set_backend(backend_name):
     if backend_name == 'MPT':
         backends['completion'] = MPT7BInstructCompletion()
     elif backend_name == 'StarCoder':
         backends['completion'] = StarCoderCompletion()
+    elif backend_name == 'StarCoderGGML':
+        backends['completion'] = StarCoderGGMLQuantizedCompletion()
+    elif backend_name == 'SantaCoderGGML':
+        backends['completion'] = SantaCoderGGMLQuantizedCompletion()
     elif backend_name == 'GPT3' or backend_name == 'OpenAI':
         backends['completion'] = OpenAICompletion()
         backends['chat'] = OpenAIChat()
     else:
         raise ValueError(f"Unknown backend {backend_name}")
 
 
@@ -138,14 +142,76 @@
             if "Rate limit" in answer.get("error", {}).get("message", ""):
                 raise RateLimitError()
             else:
                 raise Exception(f"Not sure what happened: {answer}")
         return answer["choices"][0]["message"]['content']
 
 
+class CTransformersBackend(Backend):
+    # https://github.com/marella/ctransformers
+
+    class Parameters(Backend.Parameters):
+        max_new_tokens: int = 200
+        temperature: float = 0.01
+        top_p: float = 0.92
+        top_k: int = 0
+        repetition_penalty: float = 1.1
+        stop: Optional[Union[str, List[str]]]
+    
+    def __init__(self, model_name, model_type, **param_override):
+        try:
+            from ctransformers import AutoModelForCausalLM
+        except ImportError:
+            raise ImportError("You must install ctransformers to use this backend (`pip install ctransformers`)")
+        self.model = AutoModelForCausalLM.from_pretrained(
+            model_name,
+            model_type=model_type)
+        super().__init__(**param_override)
+    
+    def preprocess(self, prompt):
+        return prompt
+    
+    async def __call__(self, prompt, **kwargs):
+        prompt = self.preprocess(prompt)
+        genkwargs = self.parse_param(**kwargs)
+        max_new_tokens = genkwargs.pop("max_new_tokens")
+
+        tokens = self.model.tokenize(prompt)
+        stop = genkwargs.pop("stop", None) or []
+        if isinstance(stop, str):
+            stop = [stop]
+        end_ids = [self.model.tokenize(x) for x in stop]
+
+        def should_stop(response_tokens):
+            for end in end_ids:
+                if all(x == y for x, y in zip(response_tokens[-len(end):], end)):
+                    return True
+            if len(response_tokens) >= max_new_tokens:
+                return True
+            return False
+
+        response = []
+        for token in self.model.generate(tokens, **genkwargs):
+            response.append(token)
+            if should_stop(response):
+                break
+
+        return self.model.detokenize(response)
+
+
+class StarCoderGGMLQuantizedCompletion(CTransformersBackend):
+    def __init__(self, **kwargs):
+        super().__init__("nouamanetazi/starcoder-ggml", model_type='starcoder', **kwargs)
+
+
+class SantaCoderGGMLQuantizedCompletion(CTransformersBackend):
+    def __init__(self, **kwargs):
+        super().__init__("danforbes/santacoder-ggml-q4_1", model_type='starcoder', **kwargs)
+
+
 class HuggingFaceBackend(Backend):
     class Parameters(Backend.Parameters):
         temperature: float = 0.01
         max_new_tokens: int = 500
         use_cache: bool = True
         do_sample: bool = True
         top_p: float = 0.92
```

### Comparing `lambdaprompt-0.5.2/lambdaprompt/gpt3.py` & `lambdaprompt-0.5.3/lambdaprompt/gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/lambdaprompt/prompt.py` & `lambdaprompt-0.5.3/lambdaprompt/prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/lambdaprompt/server/data.py` & `lambdaprompt-0.5.3/lambdaprompt/server/data.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/lambdaprompt/server/main.py` & `lambdaprompt-0.5.3/lambdaprompt/server/main.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/lambdaprompt.egg-info/PKG-INFO` & `lambdaprompt-0.5.3/lambdaprompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambdaprompt
-Version: 0.5.2
+Version: 0.5.3
 Summary: A functional programming interface for building AI systems
 License: MIT
 Project-URL: homepage, https://github.com/approximatelabs/lambdaprompt
 Keywords: nlp,ai,functional,composition,prompt,apply,chain,machine
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lambdaprompt-0.5.2/lambdaprompt.egg-info/SOURCES.txt` & `lambdaprompt-0.5.3/lambdaprompt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/pyproject.toml` & `lambdaprompt-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/tests/test_gpt3.py` & `lambdaprompt-0.5.3/tests/test_gpt3.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/tests/test_prompt.py` & `lambdaprompt-0.5.3/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `lambdaprompt-0.5.2/tests/test_server.py` & `lambdaprompt-0.5.3/tests/test_server.py`

 * *Files identical despite different names*

