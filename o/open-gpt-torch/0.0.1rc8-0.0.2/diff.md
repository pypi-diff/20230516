# Comparing `tmp/open_gpt_torch-0.0.1rc8.tar.gz` & `tmp/open_gpt_torch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc8.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.2.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc8.tar` & `open_gpt_torch-0.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10825 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/LICENSE
--rw-r--r--   0        0        0     8750 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/README.md
--rw-r--r--   0        0        0      853 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/__main__.py
--rw-r--r--   0        0        0      474 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/adapter.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1039 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0     1229 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     3706 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/factory.py
--rw-r--r--   0        0        0     2509 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/hub.py
--rw-r--r--   0        0        0      498 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     6038 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     9043 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0        0        0     5644 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     2511 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0     1407 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/llama/modeling.py
--rw-r--r--   0        0        0     4952 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2723 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0      234 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0      239 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0      907 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0        0        0     3372 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/loading.py
--rw-r--r--   0        0        0      771 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0        0        0     2862 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1778 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0     2132 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0        0        0      171 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/utils.py
--rw-r--r--   0        0        0      931 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0        0 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/open_gpt/serve/playground.py
--rw-r--r--   0        0        0     2279 2023-05-11 12:01:40.820915 open_gpt_torch-0.0.1rc8/pyproject.toml
--rw-r--r--   0        0        0    21123 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc8/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6092 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/README.md
+-rw-r--r--   0        0        0      853 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1057 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0      953 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/playground.py
+-rw-r--r--   0        0        0     1229 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     3771 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/factory.py
+-rw-r--r--   0        0        0     2509 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/helper.py
+-rw-r--r--   0        0        0      498 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     6038 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     9043 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5644 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2511 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0     3782 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/generation.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     1407 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     2501 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2101 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0     3549 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0      814 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     2740 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     3372 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0     1534 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     2905 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1778 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0     2132 2023-05-16 05:18:44.862036 open_gpt_torch-0.0.2/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      171 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/executors/utils.py
+-rw-r--r--   0        0        0      931 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0        0 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0        0        0     4689 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0        0        0     7396 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0        0        0     2714 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/open_gpt/serve/playground/gradio_css.py
+-rw-r--r--   0        0        0     3097 2023-05-16 05:18:44.866036 open_gpt_torch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    19264 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.2/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc8/LICENSE` & `open_gpt_torch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/__init__.py` & `open_gpt_torch-0.0.2/open_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/cli/application.py` & `open_gpt_torch-0.0.2/open_gpt/cli/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     return _load
 
 
 COMMANDS = [
     "about",
     "serve",
+    "playground",
 ]
 
 
 class Application(BaseApplication):
     def __init__(self) -> None:
         super().__init__("opengpt", __version__)
```

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.2/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.2/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/factory.py` & `open_gpt_torch-0.0.2/open_gpt/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,17 @@
         return PythiaModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
-    elif model_name.startswith('stabilityai/stablelm'):
+    elif model_name.startswith('stabilityai/stablelm') or model_name.startswith(
+        'CarperAI/stable-vicuna'
+    ):
         from .models.stablelm.modeling import StableLMModel
 
         return StableLMModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
```

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/helper.py` & `open_gpt_torch-0.0.2/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/flamingo_model.py` & `open_gpt_torch-0.0.2/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.2/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.2/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/llama/modeling.py` & `open_gpt_torch-0.0.2/open_gpt/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/pythia/loading.py` & `open_gpt_torch-0.0.2/open_gpt/models/loading.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 from typing import List, Optional, Union
 
 import torch
 from loguru import logger
 
+from open_gpt.helper import auto_dtype_and_device
+
 
 def load_model_and_tokenizer(
     model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     device: Optional[torch.device] = None,
     dtype: Optional[Union[str, torch.dtype]] = None,
     device_map: Optional[Union[str, List[int]]] = None,
-    **kwargs
+    no_split_module_classes: Optional[List[str]] = None,
+    **kwargs,
 ):
     """Load a model and tokenizer from HuggingFace."""
     import os
 
-    import huggingface_hub
-    from accelerate import init_empty_weights, load_checkpoint_and_dispatch
-    from transformers import (
-        AutoConfig,
-        AutoModelForCausalLM,
-        AutoTokenizer,
-        GPTNeoXForCausalLM,
-    )
-
-    from ...helper import auto_dtype_and_device
+    from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 
     dtype, device = auto_dtype_and_device(dtype, device)
-    revision = kwargs.pop('revision', 'step143000')
 
     tokenizer = AutoTokenizer.from_pretrained(
-        tokenizer_name_or_path or model_name_or_path,
-        revision=revision,
+        tokenizer_name_or_path or model_name_or_path, trust_remote_code=True
     )
 
-    tokenizer.padding_side = 'left'
-    tokenizer.pad_token = tokenizer.eos_token
-    tokenizer.pad_token_id = tokenizer.eos_token_id
+    if tokenizer.pad_token is None:
+        # Issue: GPT models don't have a pad token
+        # tokenizer.add_special_tokens({"pad_token": "<PAD>"})
+        tokenizer.pad_token = tokenizer.eos_token
+        tokenizer.pad_token_id = tokenizer.eos_token_id
+
+    # For generation padding tokens should be on the left
+    tokenizer.padding_side = "left"
 
     if device_map:
+        import huggingface_hub
+        from accelerate import init_empty_weights, load_checkpoint_and_dispatch
+
         if not os.path.exists(model_name_or_path):
             model_path = huggingface_hub.snapshot_download(model_name_or_path)
         else:
             model_path = model_name_or_path
 
         config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=True)
-
         with init_empty_weights():
             model = AutoModelForCausalLM.from_config(
                 config, torch_dtype=dtype, trust_remote_code=True
             )
             # make sure token embedding weights are still tied if needed
             model.tie_weights()
 
             model = load_checkpoint_and_dispatch(
                 model,
                 model_path,
                 device_map=device_map,
+                no_split_module_classes=no_split_module_classes,
                 dtype=dtype,
-                no_split_module_classes=["GPTNeoXLayer"],
             )
     else:
-
-        model = GPTNeoXForCausalLM.from_pretrained(
-            model_name_or_path,
-            revision=revision,
-            torch_dtype=dtype,
-            **kwargs,
+        model = AutoModelForCausalLM.from_pretrained(
+            model_name_or_path, torch_dtype=dtype, trust_remote_code=True
         )
         model.to(device)
 
+    if hasattr(model, 'generation_config'):
+        # set pad_token_id to eos_token_id because GPT does not have a PAD token
+        model.generation_config.pad_token_id = model.generation_config.eos_token_id
+
     return model, tokenizer
```

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/models/vicuna/loading.py` & `open_gpt_torch-0.0.2/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/profile.py` & `open_gpt_torch-0.0.2/open_gpt/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 import threading
 import time
 
 import psutil
 import torch
 from accelerate.utils import compute_module_sizes as _compute_module_sizes
 
+KB = 1 << 10
+MB = 1 << 20
+GB = 1 << 30
+T = 1e12
+
 
 def compute_module_sizes(model):
     return _compute_module_sizes(model)
 
 
 class PeakCPUMemory:
     def __init__(self):
@@ -82,24 +87,24 @@
     ) / 2**20
     measures["cpu-peak"] = (cpu_peak_tracker.stop() - start_measures["cpu"]) / 2**20
 
     # GPU mem
     for i in range(torch.cuda.device_count()):
         measures[str(i)] = (
             torch.cuda.memory_allocated(i) - start_measures[str(i)]
-        ) / 2**20
+        ) / GB
         measures[f"{i}-peak"] = (
             torch.cuda.max_memory_allocated(i) - start_measures[str(i)]
-        ) / 2**20
+        ) / GB
 
     return measures
 
 
 def log_measures(measures, description):
     print(f"{description}:")
     print(f"- Time: {measures['time']:.2f}s")
     for i in range(torch.cuda.device_count()):
-        print(f"- GPU {i} allocated: {measures[str(i)]:.2f}MiB")
+        print(f"- GPU {i} allocated: {measures[str(i)]:.3f}GiB")
         peak = measures[f"{i}-peak"]
-        print(f"- GPU {i} peak: {peak:.2f}MiB")
-    print(f"- CPU RAM allocated: {measures['cpu']:.2f}MiB")
-    print(f"- CPU RAM peak: {measures['cpu-peak']:.2f}MiB")
+        print(f"- GPU {i} peak: {peak:.3f}GiB")
+    print(f"- CPU RAM allocated: {measures['cpu']:.3f}GiB")
+    print(f"- CPU RAM peak: {measures['cpu-peak']:.3f}GiB")
```

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.2/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/serve/executors/flamingo.py` & `open_gpt_torch-0.0.2/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.2/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc8/PKG-INFO` & `open_gpt_torch-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,1321 +1,1204 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
 00000020: 2d67 7074 2d74 6f72 6368 0a56 6572 7369  -gpt-torch.Versi
-00000030: 6f6e 3a20 302e 302e 3172 6338 0a53 756d  on: 0.0.1rc8.Sum
-00000040: 6d61 7279 3a20 416e 206f 7065 6e2d 736f  mary: An open-so
-00000050: 7572 6365 2069 6d70 6c65 6d65 6e74 6174  urce implementat
-00000060: 696f 6e20 6f66 206c 6172 6765 2d73 6361  ion of large-sca
-00000070: 6c65 206c 616e 6775 6167 6520 6d6f 6465  le language mode
-00000080: 6c20 284c 4c4d 292e 0a48 6f6d 652d 7061  l (LLM)..Home-pa
-00000090: 6765 3a20 6874 7470 733a 2f2f 6f70 656e  ge: https://open
-000000a0: 2d67 7074 2e6a 696e 612e 6169 0a4c 6963  -gpt.jina.ai.Lic
-000000b0: 656e 7365 3a20 4170 6163 6865 2d32 2e30  ense: Apache-2.0
-000000c0: 0a4b 6579 776f 7264 733a 2050 7974 6f72  .Keywords: Pytor
-000000d0: 6368 2c4c 4c4d 2c47 5054 0a41 7574 686f  ch,LLM,GPT.Autho
-000000e0: 723a 2046 656c 6978 2057 616e 670a 4175  r: Felix Wang.Au
-000000f0: 7468 6f72 2d65 6d61 696c 3a20 6665 6c69  thor-email: feli
-00000100: 782e 7761 6e67 406a 696e 612e 6169 0a52  x.wang@jina.ai.R
-00000110: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00000120: 3e3d 332e 382c 3c34 2e30 0a43 6c61 7373  >=3.8,<4.0.Class
-00000130: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000140: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000150: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
-00000160: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
-00000170: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000180: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000190: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-000001a0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001c0: 7468 6f6e 203a 3a20 332e 380a 436c 6173  thon :: 3.8.Clas
-000001d0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000001e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001f0: 5079 7468 6f6e 203a 3a20 332e 390a 436c  Python :: 3.9.Cl
-00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000250: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000260: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
-00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000290: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-000002a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002c0: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-000002d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000002e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002f0: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
-00000300: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000310: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000320: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
-00000330: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000340: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000350: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
-00000360: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000370: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000380: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
-00000390: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000003a0: 666c 616d 696e 676f 0a52 6571 7569 7265  flamingo.Require
-000003b0: 732d 4469 7374 3a20 6163 6365 6c65 7261  s-Dist: accelera
-000003c0: 7465 2028 3e3d 302e 3138 2e30 2c3c 302e  te (>=0.18.0,<0.
-000003d0: 3139 2e30 290a 5265 7175 6972 6573 2d44  19.0).Requires-D
-000003e0: 6973 743a 2063 6c65 6f20 283e 3d32 2e30  ist: cleo (>=2.0
-000003f0: 2e30 2c3c 332e 302e 3029 0a52 6571 7569  .0,<3.0.0).Requi
-00000400: 7265 732d 4469 7374 3a20 636c 6963 6b20  res-Dist: click 
-00000410: 283e 3d38 2e31 2e33 2c3c 392e 302e 3029  (>=8.1.3,<9.0.0)
-00000420: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000430: 646f 6361 7272 6179 2028 3e3d 302e 3231  docarray (>=0.21
-00000440: 2e30 2c3c 302e 3232 2e30 290a 5265 7175  .0,<0.22.0).Requ
-00000450: 6972 6573 2d44 6973 743a 2065 696e 6f70  ires-Dist: einop
-00000460: 7320 283e 3d30 2e36 2e30 2c3c 302e 372e  s (>=0.6.0,<0.7.
-00000470: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-00000480: 3a20 6a69 6e61 2028 3e3d 332e 3135 2e30  : jina (>=3.15.0
-00000490: 2c3c 342e 302e 3029 0a52 6571 7569 7265  ,<4.0.0).Require
-000004a0: 732d 4469 7374 3a20 6c6f 6775 7275 2028  s-Dist: loguru (
-000004b0: 3e3d 302e 352c 3c30 2e36 290a 5265 7175  >=0.5,<0.6).Requ
-000004c0: 6972 6573 2d44 6973 743a 206e 756d 7079  ires-Dist: numpy
-000004d0: 2028 3e3d 312e 3231 2e32 2c3c 322e 302e   (>=1.21.2,<2.0.
-000004e0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-000004f0: 3a20 6f70 656e 2d66 6c61 6d69 6e67 6f20  : open-flamingo 
-00000500: 283e 3d30 2e30 2c3c 302e 3129 203b 2065  (>=0.0,<0.1) ; e
-00000510: 7874 7261 203d 3d20 2266 6c61 6d69 6e67  xtra == "flaming
-00000520: 6f22 0a52 6571 7569 7265 732d 4469 7374  o".Requires-Dist
-00000530: 3a20 6f70 656e 5f63 6c69 705f 746f 7263  : open_clip_torc
-00000540: 6820 283e 3d32 2e31 362c 3c33 2e30 290a  h (>=2.16,<3.0).
-00000550: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000560: 7164 6d20 283e 3d34 2e36 322e 332c 3c35  qdm (>=4.62.3,<5
-00000570: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
-00000580: 6973 743a 2074 7261 6e73 666f 726d 6572  ist: transformer
-00000590: 7320 283e 3d34 2e32 382e 302c 3c35 2e30  s (>=4.28.0,<5.0
-000005a0: 2e30 290a 5072 6f6a 6563 742d 5552 4c3a  .0).Project-URL:
-000005b0: 2052 6570 6f73 6974 6f72 792c 2068 7474   Repository, htt
-000005c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005d0: 6a69 6e61 2d61 692f 6f70 656e 5f67 7074  jina-ai/open_gpt
-000005e0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000005f0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000600: 6d61 726b 646f 776e 0a0a 2320 4f70 656e  markdown..# Open
-00000610: 4750 540a 0a21 5b5d 2868 7474 7073 3a2f  GPT..![](https:/
-00000620: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000630: 6261 6467 652f 4d61 6465 2532 3077 6974  badge/Made%20wit
-00000640: 682d 4a69 6e61 4149 2d62 6c75 6576 696f  h-JinaAI-bluevio
-00000650: 6c65 743f 7374 796c 653d 666c 6174 290a  let?style=flat).
-00000660: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
-00000670: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000680: 7079 7069 2f76 2f6f 7065 6e5f 6770 745f  pypi/v/open_gpt_
-00000690: 746f 7263 6829 5d28 6874 7470 733a 2f2f  torch)](https://
-000006a0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-000006b0: 2f6f 7065 6e5f 6770 745f 746f 7263 682f  /open_gpt_torch/
-000006c0: 290a 5b21 5b50 7950 4920 2d20 4c69 6365  ).[![PyPI - Lice
-000006d0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
-000006e0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000006f0: 2f6c 2f6f 7065 6e5f 6770 745f 746f 7263  /l/open_gpt_torc
-00000700: 6829 5d28 6874 7470 733a 2f2f 7079 7069  h)](https://pypi
-00000710: 2e6f 7267 2f70 726f 6a65 6374 2f6f 7065  .org/project/ope
-00000720: 6e5f 6770 745f 746f 7263 682f 290a 0a60  n_gpt_torch/)..`
-00000730: 4f70 656e 4750 5460 2069 7320 616e 206f  OpenGPT` is an o
-00000740: 7065 6e2d 736f 7572 6365 205f 636c 6f75  pen-source _clou
-00000750: 642d 6e61 7469 7665 5f20 6c61 7267 6520  d-native_ large 
-00000760: 2a2a 6d75 6c74 692d 6d6f 6461 6c20 6d6f  **multi-modal mo
-00000770: 6465 6c73 2a2a 2028 4c4d 4d73 2920 7365  dels** (LMMs) se
-00000780: 7276 696e 6720 736f 6c75 7469 6f6e 2e20  rving solution. 
-00000790: 0a49 7420 6973 2064 6573 6967 6e65 6420  .It is designed 
-000007a0: 746f 2073 696d 706c 6966 7920 7468 6520  to simplify the 
-000007b0: 6465 706c 6f79 6d65 6e74 2061 6e64 206d  deployment and m
-000007c0: 616e 6167 656d 656e 7420 6f66 206c 6172  anagement of lar
-000007d0: 6765 206c 616e 6775 6167 6520 6d6f 6465  ge language mode
-000007e0: 6c73 2c20 6f6e 2061 2064 6973 7472 6962  ls, on a distrib
-000007f0: 7574 6564 2063 6c75 7374 6572 206f 6620  uted cluster of 
-00000800: 4750 5573 2e0a 0a3e 202a 2a4e 6f74 652a  GPUs...> **Note*
-00000810: 2a0a 3e20 5468 6520 636f 6e74 656e 7420  *.> The content 
-00000820: 6f66 2060 5245 4144 4d45 2e6d 6460 2069  of `README.md` i
-00000830: 7320 6a75 7374 2061 2070 6c61 6365 686f  s just a placeho
-00000840: 6c64 6572 2074 6f20 7265 6d69 6e64 206d  lder to remind m
-00000850: 6520 6f66 2077 6861 7420 4920 7761 6e74  e of what I want
-00000860: 2074 6f20 646f 2e0a 0a23 2320 5461 626c   to do...## Tabl
-00000870: 6520 6f66 2063 6f6e 7465 6e74 730a 0a2d  e of contents..-
-00000880: 205b 4665 6174 7572 6573 5d28 2366 6561   [Features](#fea
-00000890: 7475 7265 7329 0a2d 205b 5375 7070 6f72  tures).- [Suppor
-000008a0: 7465 6420 6d6f 6465 6c73 5d28 2373 7570  ted models](#sup
-000008b0: 706f 7274 6564 2d6d 6f64 656c 7329 0a2d  ported-models).-
-000008c0: 205b 4765 7420 7374 6172 7465 645d 2823   [Get started](#
-000008d0: 6765 742d 7374 6172 7465 6429 0a2d 205b  get-started).- [
-000008e0: 4275 696c 6420 6120 6d6f 6465 6c20 7365  Build a model se
-000008f0: 7276 696e 6720 696e 206f 6e65 206c 696e  rving in one lin
-00000900: 655d 2823 6275 696c 642d 612d 6d6f 6465  e](#build-a-mode
-00000910: 6c2d 7365 7276 696e 672d 696e 2d6f 6e65  l-serving-in-one
-00000920: 2d6c 696e 6529 0a2d 205b 436c 6f75 642d  -line).- [Cloud-
-00000930: 6e61 7469 7665 2064 6570 6c6f 796d 656e  native deploymen
-00000940: 745d 2823 636c 6f75 642d 6e61 7469 7665  t](#cloud-native
-00000950: 2d64 6570 6c6f 796d 656e 7429 0a20 202d  -deployment).  -
-00000960: 205b 4a43 6c6f 7564 5d28 236a 636c 6f75   [JCloud](#jclou
-00000970: 6429 0a20 202d 205b 4b75 6265 726e 6574  d).  - [Kubernet
-00000980: 6573 5d28 236b 7562 6572 6e65 7465 7329  es](#kubernetes)
-00000990: 0a2d 205b 526f 6164 6d61 705d 2823 726f  .- [Roadmap](#ro
-000009a0: 6164 6d61 7029 0a0a 2323 2046 6561 7475  admap)..## Featu
-000009b0: 7265 730a 0a4f 7065 6e47 5054 2070 726f  res..OpenGPT pro
-000009c0: 7669 6465 7320 7468 6520 666f 6c6c 6f77  vides the follow
-000009d0: 696e 6720 6665 6174 7572 6573 2074 6f20  ing features to 
-000009e0: 6d61 6b65 2069 7420 6561 7379 2074 6f20  make it easy to 
-000009f0: 6465 706c 6f79 2061 6e64 2073 6572 7665  deploy and serve
-00000a00: 206c 6172 6765 206d 756c 7469 2d6d 6f64   large multi-mod
-00000a10: 616c 206d 6f64 656c 7320 284c 4d4d 7329  al models (LMMs)
-00000a20: 2069 6e20 7072 6f64 7563 7469 6f6e 3a0a   in production:.
-00000a30: 0a2d 2053 7570 706f 7274 2066 6f72 206d  .- Support for m
-00000a40: 756c 7469 2d6d 6f64 616c 206d 6f64 656c  ulti-modal model
-00000a50: 730a 2d20 5363 616c 6162 6c65 2061 7263  s.- Scalable arc
-00000a60: 6869 7465 6374 7572 6520 666f 7220 6861  hitecture for ha
-00000a70: 6e64 6c69 6e67 2068 6967 6820 7472 6166  ndling high traf
-00000a80: 6669 6320 6c6f 6164 730a 2d20 4f70 7469  fic loads.- Opti
-00000a90: 6d69 7a65 6420 666f 7220 6c6f 772d 6c61  mized for low-la
-00000aa0: 7465 6e63 7920 696e 6665 7265 6e63 650a  tency inference.
-00000ab0: 2d20 4175 746f 6d61 7469 6320 6d6f 6465  - Automatic mode
-00000ac0: 6c20 7061 7274 6974 696f 6e69 6e67 2061  l partitioning a
-00000ad0: 6e64 2064 6973 7472 6962 7574 696f 6e20  nd distribution 
-00000ae0: 6163 726f 7373 206d 756c 7469 706c 6520  across multiple 
-00000af0: 4750 5573 0a2d 2043 656e 7472 616c 697a  GPUs.- Centraliz
-00000b00: 6564 206d 6f64 656c 206d 616e 6167 656d  ed model managem
-00000b10: 656e 7420 616e 6420 6d6f 6e69 746f 7269  ent and monitori
-00000b20: 6e67 0a2d 2052 4553 5420 4150 4920 666f  ng.- REST API fo
-00000b30: 7220 6561 7379 2069 6e74 6567 7261 7469  r easy integrati
-00000b40: 6f6e 2077 6974 6820 6578 6973 7469 6e67  on with existing
-00000b50: 2061 7070 6c69 6361 7469 6f6e 730a 0a23   applications..#
-00000b60: 2320 5570 6461 7465 730a 0a2d 202a 2a32  # Updates..- **2
-00000b70: 3032 332d 3035 2d31 322a 2a3a 20f0 9f8e  023-05-12**: ...
-00000b80: 8920 5765 2068 6176 6520 7265 6c65 6173  . We have releas
-00000b90: 6564 2074 6865 2066 6972 7374 2076 6572  ed the first ver
-00000ba0: 7369 6f6e 2060 7630 2e30 2e31 6020 6f66  sion `v0.0.1` of
-00000bb0: 204f 7065 6e47 5054 2e20 596f 7520 6361   OpenGPT. You ca
-00000bc0: 6e20 696e 7374 616c 6c20 6974 2077 6974  n install it wit
-00000bd0: 6820 6070 6970 2069 6e73 7461 6c6c 206f  h `pip install o
-00000be0: 7065 6e5f 6770 745f 746f 7263 6860 2e0a  pen_gpt_torch`..
-00000bf0: 0a23 2320 5375 7070 6f72 7465 6420 4d6f  .## Supported Mo
-00000c00: 6465 6c73 0a0a 4f70 656e 4750 5420 7375  dels..OpenGPT su
-00000c10: 7070 6f72 7473 2074 6865 2066 6f6c 6c6f  pports the follo
-00000c20: 7769 6e67 206d 6f64 656c 7320 6f75 7420  wing models out 
-00000c30: 6f66 2074 6865 2062 6f78 3a0a 0a2d 204c  of the box:..- L
-00000c40: 4c4d 2028 4c61 7267 6520 4c61 6e67 7561  LM (Large Langua
-00000c50: 6765 204d 6f64 656c 290a 0a20 202d 205b  ge Model)..  - [
-00000c60: 4c6c 616d 615d 2868 7474 7073 3a2f 2f68  Llama](https://h
-00000c70: 7567 6769 6e67 6661 6365 2e63 6f2f 6661  uggingface.co/fa
-00000c80: 6365 626f 6f6b 2f6c 6c61 6d61 2d37 6229  cebook/llama-7b)
-00000c90: 0a20 202d 205b 5079 7468 6961 5d28 6874  .  - [Pythia](ht
-00000ca0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00000cb0: 652e 636f 2f2e 2e2e 290a 2020 2d20 5b53  e.co/...).  - [S
-00000cc0: 7461 626c 654c 4d5d 2868 7474 7073 3a2f  tableLM](https:/
-00000cd0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00000ce0: 2e2e 2e29 0a20 202d 205b 5669 6375 6e61  ...).  - [Vicuna
-00000cf0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00000d00: 6766 6163 652e 636f 2f2e 2e2e 290a 2020  gface.co/...).  
-00000d10: 2d20 5b4d 4f53 535d 2868 7474 7073 3a2f  - [MOSS](https:/
-00000d20: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00000d30: 2e2e 2e29 0a0a 2d20 4c4d 4d20 284c 6172  ...)..- LMM (Lar
-00000d40: 6765 204d 756c 7469 2d6d 6f64 616c 204d  ge Multi-modal M
-00000d50: 6f64 656c 290a 0a20 202d 205b 4f70 656e  odel)..  - [Open
-00000d60: 466c 616d 696e 676f 5d28 6874 7470 733a  Flamingo](https:
-00000d70: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00000d80: 2f2e 2e2e 290a 2020 2d20 5b4d 696e 6947  /...).  - [MiniG
-00000d90: 5054 345d 2868 7474 7073 3a2f 2f68 7567  PT4](https://hug
-00000da0: 6769 6e67 6661 6365 2e63 6f2f 2e2e 2e29  gingface.co/...)
-00000db0: 2028 5749 5029 0a0a 466f 7220 6d6f 7265   (WIP)..For more
-00000dc0: 2064 6574 6169 6c73 2061 626f 7574 2074   details about t
-00000dd0: 6865 2073 7570 706f 7274 6564 206d 6f64  he supported mod
-00000de0: 656c 732c 2070 6c65 6173 6520 7365 6520  els, please see 
-00000df0: 7468 6520 5b4d 6f64 656c 205a 6f6f 5d28  the [Model Zoo](
-00000e00: 2e2f 4d4f 4445 4c5f 5a4f 4f2e 6d64 292e  ./MODEL_ZOO.md).
-00000e10: 0a0a 0a23 2320 526f 6164 6d61 700a 0a59  ...## Roadmap..Y
-00000e20: 6f75 2063 616e 2076 6965 7720 6f75 7220  ou can view our 
-00000e30: 726f 6164 6d61 7020 7769 7468 2066 6561  roadmap with fea
-00000e40: 7475 7265 7320 7468 6174 2061 7265 2070  tures that are p
-00000e50: 6c61 6e6e 6564 2c20 7374 6172 7465 642c  lanned, started,
-00000e60: 2061 6e64 2063 6f6d 706c 6574 6564 206f   and completed o
-00000e70: 6e20 7468 6520 5b52 6f61 646d 6170 2064  n the [Roadmap d
-00000e80: 6973 6375 7373 696f 6e5d 2864 6973 6375  iscussion](discu
-00000e90: 7373 696f 6e73 2f63 6174 6567 6f72 6965  ssions/categorie
-00000ea0: 732f 726f 6164 6d61 7029 2063 6174 6567  s/roadmap) categ
-00000eb0: 6f72 792e 0a0a 2323 2047 6574 2053 7461  ory...## Get Sta
-00000ec0: 7274 6564 0a0a 2323 2320 496e 7374 616c  rted..### Instal
-00000ed0: 6c61 7469 6f6e 0a0a 496e 7374 616c 6c20  lation..Install 
-00000ee0: 7468 6520 7061 636b 6167 6520 7769 7468  the package with
-00000ef0: 2070 6970 3a0a 0a60 6060 6261 7368 0a70   pip:..```bash.p
-00000f00: 6970 2069 6e73 7461 6c6c 206f 7065 6e5f  ip install open_
-00000f10: 6770 745f 746f 7263 680a 6060 600a 0a23  gpt_torch.```..#
-00000f20: 2323 2051 7569 636b 7374 6172 740a 0a60  ## Quickstart..`
-00000f30: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00000f40: 6f70 656e 5f67 7074 0a0a 6d6f 6465 6c20  open_gpt..model 
-00000f50: 3d20 6f70 656e 5f67 7074 2e63 7265 6174  = open_gpt.creat
-00000f60: 655f 6d6f 6465 6c28 2766 6163 6562 6f6f  e_model('faceboo
-00000f70: 6b2f 6c6c 616d 612d 3762 272c 2064 6576  k/llama-7b', dev
-00000f80: 6963 653d 2763 7564 6127 2c20 7072 6563  ice='cuda', prec
-00000f90: 6973 696f 6e3d 2766 7031 3627 290a 0a70  ision='fp16')..p
-00000fa0: 726f 6d70 7420 3d20 2254 6865 2071 7569  rompt = "The qui
-00000fb0: 636b 2062 726f 776e 2066 6f78 206a 756d  ck brown fox jum
-00000fc0: 7073 206f 7665 7220 7468 6520 6c61 7a79  ps over the lazy
-00000fd0: 2064 6f67 2e22 0a0a 6f75 7470 7574 203d   dog."..output =
-00000fe0: 206d 6f64 656c 2e67 656e 6572 6174 6528   model.generate(
-00000ff0: 0a20 2020 2070 726f 6d70 742c 0a20 2020  .    prompt,.   
-00001000: 206d 6178 5f6c 656e 6774 683d 3130 302c   max_length=100,
-00001010: 0a20 2020 2074 656d 7065 7261 7475 7265  .    temperature
-00001020: 3d30 2e39 2c0a 2020 2020 746f 705f 6b3d  =0.9,.    top_k=
-00001030: 3530 2c0a 2020 2020 746f 705f 703d 302e  50,.    top_p=0.
-00001040: 3935 2c0a 2020 2020 7265 7065 7469 7469  95,.    repetiti
-00001050: 6f6e 5f70 656e 616c 7479 3d31 2e32 2c0a  on_penalty=1.2,.
-00001060: 2020 2020 646f 5f73 616d 706c 653d 5472      do_sample=Tr
-00001070: 7565 2c0a 2020 2020 6e75 6d5f 7265 7475  ue,.    num_retu
-00001080: 726e 5f73 6571 7565 6e63 6573 3d31 2c0a  rn_sequences=1,.
-00001090: 290a 6060 600a 0a57 6520 616c 736f 2070  ).```..We also p
-000010a0: 726f 7669 6465 2073 6f6d 6520 6164 7661  rovide some adva
-000010b0: 6e63 6564 2066 6561 7475 7265 7320 746f  nced features to
-000010c0: 2061 6c6c 6f77 2079 6f75 2074 6f20 686f   allow you to ho
-000010d0: 7374 2079 6f75 7220 6d6f 6465 6c73 2063  st your models c
-000010e0: 6f73 742d 6566 6665 6374 6976 656c 793a  ost-effectively:
-000010f0: 0a0a 2d20 2a2a 4f66 666c 6f61 6469 6e67  ..- **Offloading
-00001100: 2a2a 3a20 796f 7520 6361 6e20 6f66 666c  **: you can offl
-00001110: 6f61 6420 7061 7274 7320 6f66 2074 6865  oad parts of the
-00001120: 206d 6f64 656c 2074 6f20 4350 5520 746f   model to CPU to
-00001130: 2072 6564 7563 6520 7468 6520 636f 7374   reduce the cost
-00001140: 206f 6620 696e 6665 7265 6e63 652e 0a0a   of inference...
-00001150: 2d20 2a2a 5175 616e 7469 7a61 7469 6f6e  - **Quantization
-00001160: 2a2a 3a20 796f 7520 6361 6e20 7175 616e  **: you can quan
-00001170: 7469 7a65 2074 6865 206d 6f64 656c 2074  tize the model t
-00001180: 6f20 7265 6475 6365 2074 6865 2063 6f73  o reduce the cos
-00001190: 7420 6f66 2069 6e66 6572 656e 6365 2e0a  t of inference..
-000011a0: 0a46 6f72 206d 6f72 6520 6465 7461 696c  .For more detail
-000011b0: 732c 2070 6c65 6173 6520 7365 6520 7468  s, please see th
-000011c0: 6520 5b64 6f63 756d 656e 7461 7469 6f6e  e [documentation
-000011d0: 5d28 6874 7470 733a 2f2f 6f70 656e 6770  ](https://opengp
-000011e0: 742e 7265 6164 7468 6564 6f63 732e 696f  t.readthedocs.io
-000011f0: 2f65 6e2f 6c61 7465 7374 2f29 2e0a 0a0a  /en/latest/)....
-00001200: 2323 2042 7569 6c64 2061 206d 6f64 656c  ## Build a model
-00001210: 2073 6572 7669 6e67 2069 6e20 6f6e 6520   serving in one 
-00001220: 6c69 6e65 0a0a 596f 7520 6361 6e20 7365  line..You can se
-00001230: 7276 6520 796f 7572 206d 6f64 656c 7320  rve your models 
-00001240: 7769 7468 204f 7065 6e47 5054 2e20 546f  with OpenGPT. To
-00001250: 2064 6f20 736f 2c20 796f 7520 6361 6e20   do so, you can 
-00001260: 7573 6520 7468 6520 6073 6572 7665 6020  use the `serve` 
-00001270: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
-00001280: 680a 6f70 656e 6770 7420 7365 7276 6520  h.opengpt serve 
-00001290: 6661 6365 626f 6f6b 2f6c 6c61 6d61 2d39  facebook/llama-9
-000012a0: 6220 2d2d 6465 7669 6365 2063 7564 6120  b --device cuda 
-000012b0: 2d2d 7072 6563 6973 696f 6e20 6670 3136  --precision fp16
-000012c0: 202d 2d70 6f72 7420 3530 3030 0a60 6060   --port 5000.```
-000012d0: 0a0a 5468 6973 2077 696c 6c20 7374 6172  ..This will star
-000012e0: 7420 6120 7365 7276 6572 206f 6e20 706f  t a server on po
-000012f0: 7274 2035 3030 302e 2059 6f75 2063 616e  rt 5000. You can
-00001300: 2074 6865 6e20 7365 6e64 2072 6571 7565   then send reque
-00001310: 7374 7320 746f 2074 6865 2073 6572 7665  sts to the serve
-00001320: 723a 0a0a 6060 6070 7974 686f 6e0a 696d  r:..```python.im
-00001330: 706f 7274 2072 6571 7565 7374 730a 0a70  port requests..p
-00001340: 726f 6d70 7420 3d20 2254 6865 2071 7569  rompt = "The qui
-00001350: 636b 2062 726f 776e 2066 6f78 206a 756d  ck brown fox jum
-00001360: 7073 206f 7665 7220 7468 6520 6c61 7a79  ps over the lazy
-00001370: 2064 6f67 2e22 0a0a 7265 7370 6f6e 7365   dog."..response
-00001380: 203d 2072 6571 7565 7374 732e 706f 7374   = requests.post
-00001390: 280a 2020 2020 2268 7474 703a 2f2f 6c6f  (.    "http://lo
-000013a0: 6361 6c68 6f73 743a 3530 3030 2f67 656e  calhost:5000/gen
-000013b0: 6572 6174 6522 2c0a 2020 2020 6a73 6f6e  erate",.    json
-000013c0: 3d7b 0a20 2020 2020 2020 2022 7072 6f6d  ={.        "prom
-000013d0: 7074 223a 2070 726f 6d70 742c 0a20 2020  pt": prompt,.   
-000013e0: 2020 2020 2022 6d61 785f 6c65 6e67 7468       "max_length
-000013f0: 223a 2031 3030 2c0a 2020 2020 2020 2020  ": 100,.        
-00001400: 2274 656d 7065 7261 7475 7265 223a 2030  "temperature": 0
-00001410: 2e39 2c0a 2020 2020 2020 2020 2274 6f70  .9,.        "top
-00001420: 5f6b 223a 2035 302c 0a20 2020 2020 2020  _k": 50,.       
-00001430: 2022 746f 705f 7022 3a20 302e 3935 2c0a   "top_p": 0.95,.
-00001440: 2020 2020 2020 2020 2272 6570 6574 6974          "repetit
-00001450: 696f 6e5f 7065 6e61 6c74 7922 3a20 312e  ion_penalty": 1.
-00001460: 322c 0a20 2020 2020 2020 2022 646f 5f73  2,.        "do_s
-00001470: 616d 706c 6522 3a20 5472 7565 2c0a 2020  ample": True,.  
-00001480: 2020 2020 2020 226e 756d 5f72 6574 7572        "num_retur
-00001490: 6e5f 7365 7175 656e 6365 7322 3a20 312c  n_sequences": 1,
-000014a0: 0a20 2020 207d 2c0a 290a 0a0a 2320 5353  .    },.)...# SS
-000014b0: 4520 7375 7070 6f72 740a 6672 6f6d 2061  E support.from a
-000014c0: 696f 6874 7470 5f73 7365 5f63 6c69 656e  iohttp_sse_clien
-000014d0: 7420 696d 706f 7274 2063 6c69 656e 7420  t import client 
-000014e0: 6173 2073 7365 5f63 6c69 656e 740a 0a61  as sse_client..a
-000014f0: 7379 6e63 2077 6974 6820 7373 655f 636c  sync with sse_cl
-00001500: 6965 6e74 2e45 7665 6e74 536f 7572 6365  ient.EventSource
-00001510: 280a 2020 2020 2768 7474 703a 2f2f 6c6f  (.    'http://lo
-00001520: 6361 6c68 6f73 743a 3530 3030 2f73 7472  calhost:5000/str
-00001530: 6561 6d2f 6765 6e65 7261 7465 3f70 726f  eam/generate?pro
-00001540: 6d70 743d 5468 652b 7175 6963 6b2b 6272  mpt=The+quick+br
-00001550: 6f77 6e2b 666f 782b 6a75 6d70 732b 6f76  own+fox+jumps+ov
-00001560: 6572 2b74 6865 2b6c 617a 792b 646f 672e  er+the+lazy+dog.
-00001570: 266d 6178 5f6c 656e 6774 683d 3130 3026  &max_length=100&
-00001580: 7465 6d70 6572 6174 7572 653d 302e 3926  temperature=0.9&
-00001590: 746f 705f 6b3d 3530 2674 6f70 5f70 3d30  top_k=50&top_p=0
-000015a0: 2e39 3526 7265 7065 7469 7469 6f6e 5f70  .95&repetition_p
-000015b0: 656e 616c 7479 3d31 2e32 2664 6f5f 7361  enalty=1.2&do_sa
-000015c0: 6d70 6c65 3d54 7275 6526 6e75 6d5f 7265  mple=True&num_re
-000015d0: 7475 726e 5f73 6571 7565 6e63 6573 3d31  turn_sequences=1
-000015e0: 270a 2920 6173 2065 7665 6e74 5f73 6f75  '.) as event_sou
-000015f0: 7263 653a 0a20 2020 2074 7279 3a0a 2020  rce:.    try:.  
-00001600: 2020 2020 2020 6173 796e 6320 666f 7220        async for 
-00001610: 6576 656e 7420 696e 2065 7665 6e74 5f73  event in event_s
-00001620: 6f75 7263 653a 0a20 2020 2020 2020 2020  ource:.         
-00001630: 2020 2070 7269 6e74 2865 7665 6e74 290a     print(event).
-00001640: 2020 2020 6578 6365 7074 2043 6f6e 6e65      except Conne
-00001650: 6374 696f 6e45 7272 6f72 3a0a 2020 2020  ctionError:.    
-00001660: 2020 2020 7061 7373 0a60 6060 0a0a 4e6f      pass.```..No
-00001670: 7465 2074 6861 7420 7468 6520 7365 7276  te that the serv
-00001680: 6572 2077 696c 6c20 6f6e 6c79 2061 6363  er will only acc
-00001690: 6570 7420 7265 7175 6573 7473 2066 726f  ept requests fro
-000016a0: 6d20 7468 6520 7361 6d65 206d 6163 6869  m the same machi
-000016b0: 6e65 2e20 4966 2079 6f75 2077 616e 7420  ne. If you want 
-000016c0: 746f 2061 6363 6570 7420 7265 7175 6573  to accept reques
-000016d0: 7473 2066 726f 6d20 6f74 6865 7220 6d61  ts from other ma
-000016e0: 6368 696e 6573 2c20 796f 7520 6361 6e20  chines, you can 
-000016f0: 7573 6520 7468 6520 602d 2d68 6f73 7460  use the `--host`
-00001700: 2066 6c61 6720 746f 2073 7065 6369 6679   flag to specify
-00001710: 2074 6865 2068 6f73 7420 746f 2062 696e   the host to bin
-00001720: 6420 746f 2e0a 0a23 2320 436c 6f75 642d  d to...## Cloud-
-00001730: 6e61 7469 7665 2064 6570 6c6f 796d 656e  native deploymen
-00001740: 740a 0a59 6f75 2063 616e 2061 6c73 6f20  t..You can also 
-00001750: 6465 706c 6f79 2074 6865 2073 6572 7665  deploy the serve
-00001760: 7220 746f 2061 2063 6c6f 7564 2070 726f  r to a cloud pro
-00001770: 7669 6465 7220 6c69 6b65 204a 696e 6120  vider like Jina 
-00001780: 436c 6f75 6420 6f72 2041 5753 2e0a 546f  Cloud or AWS..To
-00001790: 2064 6f20 736f 2c20 796f 7520 6361 6e20   do so, you can 
-000017a0: 7573 6520 6064 6570 6c6f 7960 2063 6f6d  use `deploy` com
-000017b0: 6d61 6e64 3a0a 0a2d 204a 696e 6120 436c  mand:..- Jina Cl
-000017c0: 6f75 640a 0a60 6060 6261 7368 0a6f 7065  oud..```bash.ope
-000017d0: 6e67 7074 2064 6570 6c6f 7920 6661 6365  ngpt deploy face
-000017e0: 626f 6f6b 2f6c 6c61 6d61 2d39 6220 2d2d  book/llama-9b --
-000017f0: 6465 7669 6365 2063 7564 6120 2d2d 7072  device cuda --pr
-00001800: 6563 6973 696f 6e20 6670 3136 202d 2d70  ecision fp16 --p
-00001810: 726f 7669 6465 7220 6a69 6e61 202d 2d6e  rovider jina --n
-00001820: 616d 6520 6f70 656e 6770 7420 2d2d 7265  ame opengpt --re
-00001830: 706c 6963 6173 2032 0a60 6060 0a0a 2d20  plicas 2.```..- 
-00001840: 4157 530a 0a54 6f20 6465 706c 6f79 2074  AWS..To deploy t
-00001850: 6f20 4157 532c 2079 6f75 206e 6565 6420  o AWS, you need 
-00001860: 746f 2069 6e73 7461 6c6c 2065 7874 7261  to install extra
-00001870: 2064 6570 656e 6465 6e63 6965 733a 200a   dependencies: .
-00001880: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
-00001890: 7461 6c6c 206f 7065 6770 745b 6177 735d  tall opegpt[aws]
-000018a0: 0a60 6060 0a0a 416e 6420 796f 7520 6e65  .```..And you ne
-000018b0: 6564 2074 6f20 7370 6563 6966 7920 7468  ed to specify th
-000018c0: 6520 7265 6769 6f6e 3a0a 0a60 6060 6261  e region:..```ba
-000018d0: 7368 0a6f 7065 6e67 7074 2064 6570 6c6f  sh.opengpt deplo
-000018e0: 7920 6661 6365 626f 6f6b 2f6c 6c61 6d61  y facebook/llama
-000018f0: 2d39 6220 2d2d 6465 7669 6365 2063 7564  -9b --device cud
-00001900: 6120 2d2d 7072 6563 6973 696f 6e20 6670  a --precision fp
-00001910: 3136 202d 2d70 726f 7669 6465 7220 6177  16 --provider aw
-00001920: 7320 2d2d 7265 6769 6f6e 2075 732d 6561  s --region us-ea
-00001930: 7374 2d31 202d 2d6e 616d 6520 6f70 656e  st-1 --name open
-00001940: 6770 7420 2d2d 7265 706c 6963 6173 2032  gpt --replicas 2
-00001950: 0a60 6060 0a0a 5468 6973 2077 696c 6c20  .```..This will 
-00001960: 6465 706c 6f79 2074 6865 206d 6f64 656c  deploy the model
-00001970: 2074 6f20 7468 6520 636c 6f75 6420 7072   to the cloud pr
-00001980: 6f76 6964 6572 2e20 596f 7520 6361 6e20  ovider. You can 
-00001990: 7468 656e 2073 656e 6420 7265 7175 6573  then send reques
-000019a0: 7473 2074 6f20 7468 6520 7365 7276 6572  ts to the server
-000019b0: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
-000019c0: 6f72 7420 7265 7175 6573 7473 0a0a 7072  ort requests..pr
-000019d0: 6f6d 7074 203d 2022 5468 6520 7175 6963  ompt = "The quic
-000019e0: 6b20 6272 6f77 6e20 666f 7820 6a75 6d70  k brown fox jump
-000019f0: 7320 6f76 6572 2074 6865 206c 617a 7920  s over the lazy 
-00001a00: 646f 672e 220a 0a72 6573 706f 6e73 6520  dog."..response 
-00001a10: 3d20 7265 7175 6573 7473 2e70 6f73 7428  = requests.post(
-00001a20: 0a20 2020 2022 6874 7470 733a 2f2f 6f70  .    "https://op
-00001a30: 656e 6770 742e 6a69 6e61 2e61 692f 6765  engpt.jina.ai/ge
-00001a40: 6e65 7261 7465 222c 0a20 2020 206a 736f  nerate",.    jso
-00001a50: 6e3d 7b0a 2020 2020 2020 2020 2270 726f  n={.        "pro
-00001a60: 6d70 7422 3a20 7072 6f6d 7074 2c0a 2020  mpt": prompt,.  
-00001a70: 2020 2020 2020 226d 6178 5f6c 656e 6774        "max_lengt
-00001a80: 6822 3a20 3130 302c 0a20 2020 2020 2020  h": 100,.       
-00001a90: 2022 7465 6d70 6572 6174 7572 6522 3a20   "temperature": 
-00001aa0: 302e 392c 0a20 2020 2020 2020 2022 746f  0.9,.        "to
-00001ab0: 705f 6b22 3a20 3530 2c0a 2020 2020 2020  p_k": 50,.      
-00001ac0: 2020 2274 6f70 5f70 223a 2030 2e39 352c    "top_p": 0.95,
-00001ad0: 0a20 2020 2020 2020 2022 7265 7065 7469  .        "repeti
-00001ae0: 7469 6f6e 5f70 656e 616c 7479 223a 2031  tion_penalty": 1
-00001af0: 2e32 2c0a 2020 2020 2020 2020 2264 6f5f  .2,.        "do_
-00001b00: 7361 6d70 6c65 223a 2054 7275 652c 0a20  sample": True,. 
-00001b10: 2020 2020 2020 2022 6e75 6d5f 7265 7475         "num_retu
-00001b20: 726e 5f73 6571 7565 6e63 6573 223a 2031  rn_sequences": 1
-00001b30: 2c0a 2020 2020 7d2c 0a29 0a60 6060 0a0a  ,.    },.).```..
-00001b40: 2323 204b 7562 6572 6e65 7465 730a 0a54  ## Kubernetes..T
-00001b50: 6f20 6465 706c 6f79 204f 7065 6e47 5054  o deploy OpenGPT
-00001b60: 206f 6e20 796f 7572 204b 7562 6572 6e65   on your Kuberne
-00001b70: 7465 7320 636c 7573 7465 722c 2066 6f6c  tes cluster, fol
-00001b80: 6c6f 7720 7468 6573 6520 7374 6570 733a  low these steps:
-00001b90: 0a0a 312e 2049 6e73 7461 6c6c 2074 6865  ..1. Install the
-00001ba0: 204f 7065 6e47 5054 206f 7065 7261 746f   OpenGPT operato
-00001bb0: 7220 6f6e 2079 6f75 7220 4b75 6265 726e  r on your Kubern
-00001bc0: 6574 6573 2063 6c75 7374 6572 2075 7369  etes cluster usi
-00001bd0: 6e67 2048 656c 6d3a 0a0a 2020 2020 6060  ng Helm:..    ``
-00001be0: 6062 6173 680a 2020 2020 6865 6c6d 2069  `bash.    helm i
-00001bf0: 6e73 7461 6c6c 206f 7065 6e67 7074 202e  nstall opengpt .
-00001c00: 2f68 656c 6d2f 6f70 656e 6770 7420 2d2d  /helm/opengpt --
-00001c10: 6e61 6d65 7370 6163 6520 6f70 656e 6770  namespace opengp
-00001c20: 740a 2020 2020 6060 600a 0a32 2e20 4372  t.    ```..2. Cr
-00001c30: 6561 7465 2061 2063 7573 746f 6d20 7265  eate a custom re
-00001c40: 736f 7572 6365 2066 6f72 2079 6f75 7220  source for your 
-00001c50: 4750 5420 6d6f 6465 6c3a 0a20 2020 200a  GPT model:.    .
-00001c60: 2020 2020 6060 6059 414d 4c0a 2020 2020      ```YAML.    
-00001c70: 6170 6956 6572 7369 6f6e 3a20 6f70 656e  apiVersion: open
-00001c80: 6770 742e 696f 2f76 3161 6c70 6861 310a  gpt.io/v1alpha1.
-00001c90: 2020 2020 6b69 6e64 3a20 4770 744d 6f64      kind: GptMod
-00001ca0: 656c 0a20 2020 206d 6574 6164 6174 613a  el.    metadata:
-00001cb0: 0a20 2020 2020 206e 616d 653a 206d 792d  .      name: my-
-00001cc0: 6770 742d 6d6f 6465 6c0a 2020 2020 2020  gpt-model.      
-00001cd0: 6e61 6d65 7370 6163 653a 206f 7065 6e67  namespace: openg
-00001ce0: 7074 0a20 2020 2073 7065 633a 0a20 2020  pt.    spec:.   
-00001cf0: 2020 206d 6f64 656c 5061 7468 3a20 7333     modelPath: s3
-00001d00: 3a2f 2f6d 792d 6275 636b 6574 2f6d 792d  ://my-bucket/my-
-00001d10: 6d6f 6465 6c0a 2020 2020 2020 6d6f 6465  model.      mode
-00001d20: 6c4e 616d 653a 206d 792d 6d6f 6465 6c0a  lName: my-model.
-00001d30: 2020 2020 2020 6d61 7842 6174 6368 5369        maxBatchSi
-00001d40: 7a65 3a20 3136 0a20 2020 2020 2069 6e70  ze: 16.      inp
-00001d50: 7574 5368 6170 653a 0a20 2020 2020 2020  utShape:.       
-00001d60: 202d 2031 3032 340a 2020 2020 2020 2020   - 1024.        
-00001d70: 2d20 3130 3234 0a20 2020 2020 2020 202d  - 1024.        -
-00001d80: 2033 0a20 2020 2020 206f 7574 7075 7453   3.      outputS
-00001d90: 6861 7065 3a0a 2020 2020 2020 2020 2d20  hape:.        - 
-00001da0: 3130 3234 0a20 2020 2020 2020 202d 2031  1024.        - 1
-00001db0: 3032 340a 2020 2020 2020 2020 2d20 330a  024.        - 3.
-00001dc0: 0a20 2020 2060 6060 0a20 2020 0a33 2e20  .    ```.   .3. 
-00001dd0: 4170 706c 7920 7468 6520 6375 7374 6f6d  Apply the custom
-00001de0: 2072 6573 6f75 7263 6520 746f 2079 6f75   resource to you
-00001df0: 7220 636c 7573 7465 723a 0a0a 2020 2020  r cluster:..    
-00001e00: 6060 6062 6173 680a 2020 206b 7562 6563  ```bash.   kubec
-00001e10: 746c 2061 7070 6c79 202d 6620 6d79 2d67  tl apply -f my-g
-00001e20: 7074 2d6d 6f64 656c 2e79 616d 6c0a 2020  pt-model.yaml.  
-00001e30: 2020 6060 600a 0a34 2e20 4d6f 6e69 746f    ```..4. Monito
-00001e40: 7220 7468 6520 7374 6174 7573 206f 6620  r the status of 
-00001e50: 796f 7572 2047 5054 206d 6f64 656c 2075  your GPT model u
-00001e60: 7369 6e67 2074 6865 204f 7065 6e47 5054  sing the OpenGPT
-00001e70: 2064 6173 6862 6f61 7264 3a0a 0a20 2020   dashboard:..   
-00001e80: 2060 6060 6261 7368 0a20 2020 6b75 6265   ```bash.   kube
-00001e90: 6374 6c20 706f 7274 2d66 6f72 7761 7264  ctl port-forward
-00001ea0: 202d 6e20 6f70 656e 6770 7420 7376 632f   -n opengpt svc/
-00001eb0: 6f70 656e 6770 742d 6461 7368 626f 6172  opengpt-dashboar
-00001ec0: 6420 3830 3830 3a38 300a 2020 2020 6060  d 8080:80.    ``
-00001ed0: 600a 0a23 2320 4163 6365 7373 696e 6720  `..## Accessing 
-00001ee0: 6d6f 6465 6c73 2076 6961 2041 5049 0a0a  models via API..
-00001ef0: 596f 7520 6361 6e20 616c 736f 2061 6363  You can also acc
-00001f00: 6573 7320 7468 6520 6f6e 6c69 6e65 206d  ess the online m
-00001f10: 6f64 656c 7320 7669 6120 4150 492e 2054  odels via API. T
-00001f20: 6f20 646f 2073 6f2c 2079 6f75 2063 616e  o do so, you can
-00001f30: 2075 7365 2074 6865 2060 696e 6665 7265   use the `infere
-00001f40: 6e63 655f 636c 6965 6e74 6020 7061 636b  nce_client` pack
-00001f50: 6167 653a 0a0a 6060 6070 7974 686f 6e0a  age:..```python.
-00001f60: 6672 6f6d 2069 6e66 6572 656e 6365 5f63  from inference_c
-00001f70: 6c69 656e 7420 696d 706f 7274 2043 6c69  lient import Cli
-00001f80: 656e 740a 0a63 6c69 656e 7420 3d20 436c  ent..client = Cl
-00001f90: 6965 6e74 2874 6f6b 656e 3d27 3c79 6f75  ient(token='<you
-00001fa0: 7220 6163 6365 7373 2074 6f6b 656e 3e27  r access token>'
-00001fb0: 290a 0a6d 6f64 656c 203d 2063 6c69 656e  )..model = clien
-00001fc0: 742e 6765 745f 6d6f 6465 6c28 2766 6163  t.get_model('fac
-00001fd0: 6562 6f6f 6b2f 6c6c 616d 612d 3962 2729  ebook/llama-9b')
-00001fe0: 0a0a 7072 6f6d 7074 203d 2022 5468 6520  ..prompt = "The 
-00001ff0: 7175 6963 6b20 6272 6f77 6e20 666f 7820  quick brown fox 
-00002000: 6a75 6d70 7320 6f76 6572 2074 6865 206c  jumps over the l
-00002010: 617a 7920 646f 672e 220a 0a6f 7574 7075  azy dog."..outpu
-00002020: 7420 3d20 6d6f 6465 6c2e 6765 6e65 7261  t = model.genera
-00002030: 7465 280a 2020 2020 7072 6f6d 7074 2c0a  te(.    prompt,.
-00002040: 2020 2020 6d61 785f 6c65 6e67 7468 3d31      max_length=1
-00002050: 3030 2c0a 2020 2020 7465 6d70 6572 6174  00,.    temperat
-00002060: 7572 653d 302e 392c 0a20 2020 2074 6f70  ure=0.9,.    top
-00002070: 5f6b 3d35 302c 0a20 2020 2074 6f70 5f70  _k=50,.    top_p
-00002080: 3d30 2e39 352c 0a20 2020 2072 6570 6574  =0.95,.    repet
-00002090: 6974 696f 6e5f 7065 6e61 6c74 793d 312e  ition_penalty=1.
-000020a0: 322c 0a20 2020 2064 6f5f 7361 6d70 6c65  2,.    do_sample
-000020b0: 3d54 7275 652c 0a20 2020 206e 756d 5f72  =True,.    num_r
-000020c0: 6574 7572 6e5f 7365 7175 656e 6365 733d  eturn_sequences=
-000020d0: 312c 0a29 0a60 6060 0a0a 4279 2074 6869  1,.).```..By thi
-000020e0: 7320 7761 792c 2079 6f75 2063 616e 2061  s way, you can a
-000020f0: 6363 6573 7320 7468 6520 6d6f 6465 6c73  ccess the models
-00002100: 2077 6974 686f 7574 2064 6570 6c6f 7969   without deployi
-00002110: 6e67 2074 6865 6d20 746f 2079 6f75 7220  ng them to your 
-00002120: 6f77 6e20 6d61 6368 696e 652e 0a0a 2323  own machine...##
-00002130: 2041 6476 616e 6365 6420 5573 6167 650a   Advanced Usage.
-00002140: 0a23 2323 204d 6f64 656c 204f 6666 6c6f  .### Model Offlo
-00002150: 6164 696e 670a 0a59 6f75 2063 616e 2061  ading..You can a
-00002160: 6c73 6f20 6170 706c 7920 7468 6520 6d6f  lso apply the mo
-00002170: 6465 6c20 6f66 666c 6f61 6469 6e67 2074  del offloading t
-00002180: 6563 686e 6971 7565 7320 2862 6173 6564  echniques (based
-00002190: 206f 6e20 5b46 6c65 7854 656e 736f 725d   on [FlexTensor]
-000021a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000021b0: 636f 6d2f 6e75 6d62 3372 332f 666c 6578  com/numb3r3/flex
-000021c0: 2d74 656e 736f 7229 2920 746f 204f 7065  -tensor)) to Ope
-000021d0: 6e47 5054 2e20 546f 2064 6f20 736f 2c20  nGPT. To do so, 
-000021e0: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-000021f0: 602d 2d6f 6666 6c6f 6164 2d70 6572 6365  `--offload-perce
-00002200: 6e74 7360 2066 6c61 673a 0a0a 6060 6062  nts` flag:..```b
-00002210: 6173 680a 6f70 656e 6770 7420 7365 7276  ash.opengpt serv
-00002220: 6520 6661 6365 626f 6f6b 2f6c 6c61 6d61  e facebook/llama
-00002230: 2d39 6220 2d2d 6465 7669 6365 2063 7564  -9b --device cud
-00002240: 6120 2d2d 7072 6563 6973 696f 6e20 6670  a --precision fp
-00002250: 3136 202d 2d70 6f72 7420 3530 3030 202d  16 --port 5000 -
-00002260: 2d6f 6666 6c6f 6164 2d70 6572 6365 6e74  -offload-percent
-00002270: 7320 3130 2c39 302c 3530 2c35 302c 302c  s 10,90,50,50,0,
-00002280: 3130 300a 6060 600a 0a54 6869 7320 7769  100.```..This wi
-00002290: 6c6c 206f 6666 6c6f 6164 2070 6172 7473  ll offload parts
-000022a0: 206f 6620 7468 6520 6d6f 6465 6c20 746f   of the model to
-000022b0: 2074 6865 2043 5055 2e20 596f 7520 6361   the CPU. You ca
-000022c0: 6e20 616c 736f 2075 7365 2074 6865 2060  n also use the `
-000022d0: 2d2d 6f66 666c 6f61 642d 7374 7261 7465  --offload-strate
-000022e0: 6779 6020 666c 6167 2074 6f20 7370 6563  gy` flag to spec
-000022f0: 6966 7920 7468 6520 6f66 666c 6f61 6469  ify the offloadi
-00002300: 6e67 2073 7472 6174 6567 793a 0a0a 6060  ng strategy:..``
-00002310: 6062 6173 680a 6f70 656e 6770 7420 7365  `bash.opengpt se
-00002320: 7276 6520 6661 6365 626f 6f6b 2f6c 6c61  rve facebook/lla
-00002330: 6d61 2d39 6220 2d2d 6465 7669 6365 2063  ma-9b --device c
-00002340: 7564 6120 2d2d 7072 6563 6973 696f 6e20  uda --precision 
-00002350: 6670 3136 202d 2d70 6f72 7420 3530 3030  fp16 --port 5000
-00002360: 202d 2d6f 6666 6c6f 6164 2d73 7472 6174   --offload-strat
-00002370: 6567 7920 2263 7075 2c63 7075 2c63 7075  egy "cpu,cpu,cpu
-00002380: 2c63 7075 2c63 7075 2c63 7075 220a 6060  ,cpu,cpu,cpu".``
-00002390: 600a 0a23 2323 204d 6f64 656c 2051 7561  `..### Model Qua
-000023a0: 6e74 697a 6174 696f 6e0a 0a59 6f75 2063  ntization..You c
-000023b0: 616e 2061 6c73 6f20 6170 706c 7920 7468  an also apply th
-000023c0: 6520 6d6f 6465 6c20 7175 616e 7469 7a61  e model quantiza
-000023d0: 7469 6f6e 2074 6563 686e 6971 7565 732e  tion techniques.
-000023e0: 0a0a 2d20 382d 6269 7420 7175 616e 7469  ..- 8-bit quanti
-000023f0: 7a61 7469 6f6e 0a0a 6060 6062 6173 680a  zation..```bash.
-00002400: 6f70 656e 6770 7420 7365 7276 6520 6661  opengpt serve fa
-00002410: 6365 626f 6f6b 2f6c 6c61 6d61 2d39 6220  cebook/llama-9b 
-00002420: 2d2d 6465 7669 6365 2063 7564 6120 2d2d  --device cuda --
-00002430: 7072 6563 6973 696f 6e20 6670 3136 202d  precision fp16 -
-00002440: 2d70 6f72 7420 3530 3030 202d 2d71 7561  -port 5000 --qua
-00002450: 6e74 697a 6520 3862 6974 0a60 6060 0a0a  ntize 8bit.```..
-00002460: 2323 2046 696e 652d 7475 6e69 6e67 204d  ## Fine-tuning M
-00002470: 6f64 656c 730a 0a57 6520 6375 7272 656e  odels..We curren
-00002480: 746c 7920 7375 7070 6f72 7420 6669 6e65  tly support fine
-00002490: 2d74 756e 696e 6720 6d6f 6465 6c73 2062  -tuning models b
-000024a0: 7920 7573 696e 6720 7468 6520 6066 696e  y using the `fin
-000024b0: 6574 756e 6560 2063 6f6d 6d61 6e64 3a0a  etune` command:.
-000024c0: 0a60 6060 6261 7368 0a6f 7065 6e67 7074  .```bash.opengpt
-000024d0: 2066 696e 6574 756e 6520 6661 6365 626f   finetune facebo
-000024e0: 6f6b 2f6c 6c61 6d61 2d39 6220 2d2d 6461  ok/llama-9b --da
-000024f0: 7461 7365 7420 7769 6b69 7465 7874 2d32  taset wikitext-2
-00002500: 202d 2d64 6576 6963 6520 6375 6461 202d   --device cuda -
-00002510: 2d70 7265 6369 7369 6f6e 2066 7031 3620  -precision fp16 
-00002520: 2d2d 6261 7463 682d 7369 7a65 2033 3220  --batch-size 32 
-00002530: 2d2d 6c65 6172 6e69 6e67 2d72 6174 6520  --learning-rate 
-00002540: 3165 2d34 202d 2d65 706f 6368 7320 3130  1e-4 --epochs 10
-00002550: 0a60 6060 0a0a 5370 6563 6966 6963 616c  .```..Specifical
-00002560: 6c79 2c20 7765 2069 6d70 6c65 6d65 6e74  ly, we implement
-00002570: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-00002580: 696e 652d 7475 6e69 6e67 206d 6574 686f  ine-tuning metho
-00002590: 6473 3a0a 2d20 5b4c 4c61 4d41 2d41 6461  ds:.- [LLaMA-Ada
-000025a0: 7074 6572 3a20 4566 6669 6369 656e 7420  pter: Efficient 
-000025b0: 4669 6e65 2d74 756e 696e 6720 6f66 204c  Fine-tuning of L
-000025c0: 4c61 4d41 5d28 6874 7470 733a 2f2f 6769  LaMA](https://gi
-000025d0: 7468 7562 2e63 6f6d 2f5a 7272 536b 7977  thub.com/ZrrSkyw
-000025e0: 616c 6b65 722f 4c4c 614d 412d 4164 6170  alker/LLaMA-Adap
-000025f0: 7465 7229 3a20 4669 6e65 2d74 756e 696e  ter): Fine-tunin
-00002600: 6720 6d6f 6465 6c20 746f 2066 6f6c 6c6f  g model to follo
-00002610: 7720 696e 7374 7275 6374 696f 6e73 2077  w instructions w
-00002620: 6974 6869 6e20 3120 486f 7572 2061 6e64  ithin 1 Hour and
-00002630: 2031 2e32 4d20 5061 7261 6d65 7465 7273   1.2M Parameters
-00002640: 0a2d 205b 6c6f 772d 7261 6e6b 2061 6461  .- [low-rank ada
-00002650: 7074 6174 696f 6e20 284c 6f52 4129 5d28  ptation (LoRA)](
-00002660: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00002670: 672f 7064 662f 3231 3036 2e30 3936 3835  g/pdf/2106.09685
-00002680: 2e70 6466 293a 204c 6f77 2d52 616e 6b20  .pdf): Low-Rank 
-00002690: 4164 6170 7461 7469 6f6e 2066 6f72 2045  Adaptation for E
-000026a0: 6666 6963 6965 6e74 204c 616e 6775 6167  fficient Languag
-000026b0: 6520 4d6f 6465 6c20 4669 6e65 2d54 756e  e Model Fine-Tun
-000026c0: 696e 670a 0a23 2320 446f 6375 6d65 6e74  ing..## Document
-000026d0: 6174 696f 6e0a 0a46 6f72 206d 6f72 6520  ation..For more 
-000026e0: 696e 666f 726d 6174 696f 6e2c 2063 6865  information, che
-000026f0: 636b 206f 7574 2074 6865 205b 646f 6375  ck out the [docu
-00002700: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00002710: 3a2f 2f6f 7065 6e67 7074 2e72 6561 6474  ://opengpt.readt
-00002720: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00002730: 6573 742f 292e 0a0a 0a23 2320 436f 6e74  est/)....## Cont
-00002740: 7269 6275 7469 6e67 0a0a 5765 2077 656c  ributing..We wel
-00002750: 636f 6d65 2063 6f6e 7472 6962 7574 696f  come contributio
-00002760: 6e73 2066 726f 6d20 7468 6520 636f 6d6d  ns from the comm
-00002770: 756e 6974 7921 2054 6f20 636f 6e74 7269  unity! To contri
-00002780: 6275 7465 2c20 706c 6561 7365 2073 7562  bute, please sub
-00002790: 6d69 7420 6120 7075 6c6c 2072 6571 7565  mit a pull reque
-000027a0: 7374 2066 6f6c 6c6f 7769 6e67 206f 7572  st following our
-000027b0: 2063 6f6e 7472 6962 7574 696e 6720 6775   contributing gu
-000027c0: 6964 656c 696e 6573 2e0a 0a23 2320 4c69  idelines...## Li
-000027d0: 6365 6e73 650a 0a4f 7065 6e47 5054 2069  cense..OpenGPT i
-000027e0: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
-000027f0: 2074 6865 2041 7061 6368 6520 4c69 6365   the Apache Lice
-00002800: 6e73 652c 2056 6572 7369 6f6e 2032 2e30  nse, Version 2.0
-00002810: 2e20 5365 6520 4c49 4345 4e53 4520 666f  . See LICENSE fo
-00002820: 7220 7468 6520 6675 6c6c 206c 6963 656e  r the full licen
-00002830: 7365 2074 6578 742e 0a43 6f70 7972 6967  se text..Copyrig
-00002840: 6874 2032 3032 302d 3230 3232 204a 696e  ht 2020-2022 Jin
-00002850: 6120 4149 204c 696d 6974 6564 2e20 2041  a AI Limited.  A
-00002860: 6c6c 2072 6967 6874 7320 7265 7365 7276  ll rights reserv
-00002870: 6564 2e0a 0a20 2020 2020 2020 2020 2020  ed...           
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 2020 2020 4170 6163 6865 204c 6963        Apache Lic
-000028a0: 656e 7365 0a20 2020 2020 2020 2020 2020  ense.           
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 5665 7273 696f 6e20 322e 302c 204a 616e  Version 2.0, Jan
-000028d0: 7561 7279 2032 3030 340a 2020 2020 2020  uary 2004.      
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2020 6874 7470 3a2f 2f77 7777 2e61 7061    http://www.apa
-00002900: 6368 652e 6f72 672f 6c69 6365 6e73 6573  che.org/licenses
-00002910: 2f0a 0a20 2020 5445 524d 5320 414e 4420  /..   TERMS AND 
-00002920: 434f 4e44 4954 494f 4e53 2046 4f52 2055  CONDITIONS FOR U
-00002930: 5345 2c20 5245 5052 4f44 5543 5449 4f4e  SE, REPRODUCTION
-00002940: 2c20 414e 4420 4449 5354 5249 4255 5449  , AND DISTRIBUTI
-00002950: 4f4e 0a0a 2020 2031 2e20 4465 6669 6e69  ON..   1. Defini
-00002960: 7469 6f6e 732e 0a0a 2020 2020 2020 224c  tions...      "L
-00002970: 6963 656e 7365 2220 7368 616c 6c20 6d65  icense" shall me
-00002980: 616e 2074 6865 2074 6572 6d73 2061 6e64  an the terms and
-00002990: 2063 6f6e 6469 7469 6f6e 7320 666f 7220   conditions for 
-000029a0: 7573 652c 2072 6570 726f 6475 6374 696f  use, reproductio
-000029b0: 6e2c 0a20 2020 2020 2061 6e64 2064 6973  n,.      and dis
-000029c0: 7472 6962 7574 696f 6e20 6173 2064 6566  tribution as def
-000029d0: 696e 6564 2062 7920 5365 6374 696f 6e73  ined by Sections
-000029e0: 2031 2074 6872 6f75 6768 2039 206f 6620   1 through 9 of 
-000029f0: 7468 6973 2064 6f63 756d 656e 742e 0a0a  this document...
-00002a00: 2020 2020 2020 224c 6963 656e 736f 7222        "Licensor"
-00002a10: 2073 6861 6c6c 206d 6561 6e20 7468 6520   shall mean the 
-00002a20: 636f 7079 7269 6768 7420 6f77 6e65 7220  copyright owner 
-00002a30: 6f72 2065 6e74 6974 7920 6175 7468 6f72  or entity author
-00002a40: 697a 6564 2062 790a 2020 2020 2020 7468  ized by.      th
-00002a50: 6520 636f 7079 7269 6768 7420 6f77 6e65  e copyright owne
-00002a60: 7220 7468 6174 2069 7320 6772 616e 7469  r that is granti
-00002a70: 6e67 2074 6865 204c 6963 656e 7365 2e0a  ng the License..
-00002a80: 0a20 2020 2020 2022 4c65 6761 6c20 456e  .      "Legal En
-00002a90: 7469 7479 2220 7368 616c 6c20 6d65 616e  tity" shall mean
-00002aa0: 2074 6865 2075 6e69 6f6e 206f 6620 7468   the union of th
-00002ab0: 6520 6163 7469 6e67 2065 6e74 6974 7920  e acting entity 
-00002ac0: 616e 6420 616c 6c0a 2020 2020 2020 6f74  and all.      ot
-00002ad0: 6865 7220 656e 7469 7469 6573 2074 6861  her entities tha
-00002ae0: 7420 636f 6e74 726f 6c2c 2061 7265 2063  t control, are c
-00002af0: 6f6e 7472 6f6c 6c65 6420 6279 2c20 6f72  ontrolled by, or
-00002b00: 2061 7265 2075 6e64 6572 2063 6f6d 6d6f   are under commo
-00002b10: 6e0a 2020 2020 2020 636f 6e74 726f 6c20  n.      control 
-00002b20: 7769 7468 2074 6861 7420 656e 7469 7479  with that entity
-00002b30: 2e20 466f 7220 7468 6520 7075 7270 6f73  . For the purpos
-00002b40: 6573 206f 6620 7468 6973 2064 6566 696e  es of this defin
-00002b50: 6974 696f 6e2c 0a20 2020 2020 2022 636f  ition,.      "co
-00002b60: 6e74 726f 6c22 206d 6561 6e73 2028 6929  ntrol" means (i)
-00002b70: 2074 6865 2070 6f77 6572 2c20 6469 7265   the power, dire
-00002b80: 6374 206f 7220 696e 6469 7265 6374 2c20  ct or indirect, 
-00002b90: 746f 2063 6175 7365 2074 6865 0a20 2020  to cause the.   
-00002ba0: 2020 2064 6972 6563 7469 6f6e 206f 7220     direction or 
-00002bb0: 6d61 6e61 6765 6d65 6e74 206f 6620 7375  management of su
-00002bc0: 6368 2065 6e74 6974 792c 2077 6865 7468  ch entity, wheth
-00002bd0: 6572 2062 7920 636f 6e74 7261 6374 206f  er by contract o
-00002be0: 720a 2020 2020 2020 6f74 6865 7277 6973  r.      otherwis
-00002bf0: 652c 206f 7220 2869 6929 206f 776e 6572  e, or (ii) owner
-00002c00: 7368 6970 206f 6620 6669 6674 7920 7065  ship of fifty pe
-00002c10: 7263 656e 7420 2835 3025 2920 6f72 206d  rcent (50%) or m
-00002c20: 6f72 6520 6f66 2074 6865 0a20 2020 2020  ore of the.     
-00002c30: 206f 7574 7374 616e 6469 6e67 2073 6861   outstanding sha
-00002c40: 7265 732c 206f 7220 2869 6969 2920 6265  res, or (iii) be
-00002c50: 6e65 6669 6369 616c 206f 776e 6572 7368  neficial ownersh
-00002c60: 6970 206f 6620 7375 6368 2065 6e74 6974  ip of such entit
-00002c70: 792e 0a0a 2020 2020 2020 2259 6f75 2220  y...      "You" 
-00002c80: 286f 7220 2259 6f75 7222 2920 7368 616c  (or "Your") shal
-00002c90: 6c20 6d65 616e 2061 6e20 696e 6469 7669  l mean an indivi
-00002ca0: 6475 616c 206f 7220 4c65 6761 6c20 456e  dual or Legal En
-00002cb0: 7469 7479 0a20 2020 2020 2065 7865 7263  tity.      exerc
-00002cc0: 6973 696e 6720 7065 726d 6973 7369 6f6e  ising permission
-00002cd0: 7320 6772 616e 7465 6420 6279 2074 6869  s granted by thi
-00002ce0: 7320 4c69 6365 6e73 652e 0a0a 2020 2020  s License...    
-00002cf0: 2020 2253 6f75 7263 6522 2066 6f72 6d20    "Source" form 
-00002d00: 7368 616c 6c20 6d65 616e 2074 6865 2070  shall mean the p
-00002d10: 7265 6665 7272 6564 2066 6f72 6d20 666f  referred form fo
-00002d20: 7220 6d61 6b69 6e67 206d 6f64 6966 6963  r making modific
-00002d30: 6174 696f 6e73 2c0a 2020 2020 2020 696e  ations,.      in
-00002d40: 636c 7564 696e 6720 6275 7420 6e6f 7420  cluding but not 
-00002d50: 6c69 6d69 7465 6420 746f 2073 6f66 7477  limited to softw
-00002d60: 6172 6520 736f 7572 6365 2063 6f64 652c  are source code,
-00002d70: 2064 6f63 756d 656e 7461 7469 6f6e 0a20   documentation. 
-00002d80: 2020 2020 2073 6f75 7263 652c 2061 6e64       source, and
-00002d90: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00002da0: 696c 6573 2e0a 0a20 2020 2020 2022 4f62  iles...      "Ob
-00002db0: 6a65 6374 2220 666f 726d 2073 6861 6c6c  ject" form shall
-00002dc0: 206d 6561 6e20 616e 7920 666f 726d 2072   mean any form r
-00002dd0: 6573 756c 7469 6e67 2066 726f 6d20 6d65  esulting from me
-00002de0: 6368 616e 6963 616c 0a20 2020 2020 2074  chanical.      t
-00002df0: 7261 6e73 666f 726d 6174 696f 6e20 6f72  ransformation or
-00002e00: 2074 7261 6e73 6c61 7469 6f6e 206f 6620   translation of 
-00002e10: 6120 536f 7572 6365 2066 6f72 6d2c 2069  a Source form, i
-00002e20: 6e63 6c75 6469 6e67 2062 7574 0a20 2020  ncluding but.   
-00002e30: 2020 206e 6f74 206c 696d 6974 6564 2074     not limited t
-00002e40: 6f20 636f 6d70 696c 6564 206f 626a 6563  o compiled objec
-00002e50: 7420 636f 6465 2c20 6765 6e65 7261 7465  t code, generate
-00002e60: 6420 646f 6375 6d65 6e74 6174 696f 6e2c  d documentation,
-00002e70: 0a20 2020 2020 2061 6e64 2063 6f6e 7665  .      and conve
-00002e80: 7273 696f 6e73 2074 6f20 6f74 6865 7220  rsions to other 
-00002e90: 6d65 6469 6120 7479 7065 732e 0a0a 2020  media types...  
-00002ea0: 2020 2020 2257 6f72 6b22 2073 6861 6c6c      "Work" shall
-00002eb0: 206d 6561 6e20 7468 6520 776f 726b 206f   mean the work o
-00002ec0: 6620 6175 7468 6f72 7368 6970 2c20 7768  f authorship, wh
-00002ed0: 6574 6865 7220 696e 2053 6f75 7263 6520  ether in Source 
-00002ee0: 6f72 0a20 2020 2020 204f 626a 6563 7420  or.      Object 
-00002ef0: 666f 726d 2c20 6d61 6465 2061 7661 696c  form, made avail
-00002f00: 6162 6c65 2075 6e64 6572 2074 6865 204c  able under the L
-00002f10: 6963 656e 7365 2c20 6173 2069 6e64 6963  icense, as indic
-00002f20: 6174 6564 2062 7920 610a 2020 2020 2020  ated by a.      
-00002f30: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
-00002f40: 2074 6861 7420 6973 2069 6e63 6c75 6465   that is include
-00002f50: 6420 696e 206f 7220 6174 7461 6368 6564  d in or attached
-00002f60: 2074 6f20 7468 6520 776f 726b 0a20 2020   to the work.   
-00002f70: 2020 2028 616e 2065 7861 6d70 6c65 2069     (an example i
-00002f80: 7320 7072 6f76 6964 6564 2069 6e20 7468  s provided in th
-00002f90: 6520 4170 7065 6e64 6978 2062 656c 6f77  e Appendix below
-00002fa0: 292e 0a0a 2020 2020 2020 2244 6572 6976  )...      "Deriv
-00002fb0: 6174 6976 6520 576f 726b 7322 2073 6861  ative Works" sha
-00002fc0: 6c6c 206d 6561 6e20 616e 7920 776f 726b  ll mean any work
-00002fd0: 2c20 7768 6574 6865 7220 696e 2053 6f75  , whether in Sou
-00002fe0: 7263 6520 6f72 204f 626a 6563 740a 2020  rce or Object.  
-00002ff0: 2020 2020 666f 726d 2c20 7468 6174 2069      form, that i
-00003000: 7320 6261 7365 6420 6f6e 2028 6f72 2064  s based on (or d
-00003010: 6572 6976 6564 2066 726f 6d29 2074 6865  erived from) the
-00003020: 2057 6f72 6b20 616e 6420 666f 7220 7768   Work and for wh
-00003030: 6963 6820 7468 650a 2020 2020 2020 6564  ich the.      ed
-00003040: 6974 6f72 6961 6c20 7265 7669 7369 6f6e  itorial revision
-00003050: 732c 2061 6e6e 6f74 6174 696f 6e73 2c20  s, annotations, 
-00003060: 656c 6162 6f72 6174 696f 6e73 2c20 6f72  elaborations, or
-00003070: 206f 7468 6572 206d 6f64 6966 6963 6174   other modificat
-00003080: 696f 6e73 0a20 2020 2020 2072 6570 7265  ions.      repre
-00003090: 7365 6e74 2c20 6173 2061 2077 686f 6c65  sent, as a whole
-000030a0: 2c20 616e 206f 7269 6769 6e61 6c20 776f  , an original wo
-000030b0: 726b 206f 6620 6175 7468 6f72 7368 6970  rk of authorship
-000030c0: 2e20 466f 7220 7468 6520 7075 7270 6f73  . For the purpos
-000030d0: 6573 0a20 2020 2020 206f 6620 7468 6973  es.      of this
-000030e0: 204c 6963 656e 7365 2c20 4465 7269 7661   License, Deriva
-000030f0: 7469 7665 2057 6f72 6b73 2073 6861 6c6c  tive Works shall
-00003100: 206e 6f74 2069 6e63 6c75 6465 2077 6f72   not include wor
-00003110: 6b73 2074 6861 7420 7265 6d61 696e 0a20  ks that remain. 
-00003120: 2020 2020 2073 6570 6172 6162 6c65 2066       separable f
-00003130: 726f 6d2c 206f 7220 6d65 7265 6c79 206c  rom, or merely l
-00003140: 696e 6b20 286f 7220 6269 6e64 2062 7920  ink (or bind by 
-00003150: 6e61 6d65 2920 746f 2074 6865 2069 6e74  name) to the int
-00003160: 6572 6661 6365 7320 6f66 2c0a 2020 2020  erfaces of,.    
-00003170: 2020 7468 6520 576f 726b 2061 6e64 2044    the Work and D
-00003180: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
-00003190: 7468 6572 656f 662e 0a0a 2020 2020 2020  thereof...      
-000031a0: 2243 6f6e 7472 6962 7574 696f 6e22 2073  "Contribution" s
-000031b0: 6861 6c6c 206d 6561 6e20 616e 7920 776f  hall mean any wo
-000031c0: 726b 206f 6620 6175 7468 6f72 7368 6970  rk of authorship
-000031d0: 2c20 696e 636c 7564 696e 670a 2020 2020  , including.    
-000031e0: 2020 7468 6520 6f72 6967 696e 616c 2076    the original v
-000031f0: 6572 7369 6f6e 206f 6620 7468 6520 576f  ersion of the Wo
-00003200: 726b 2061 6e64 2061 6e79 206d 6f64 6966  rk and any modif
-00003210: 6963 6174 696f 6e73 206f 7220 6164 6469  ications or addi
-00003220: 7469 6f6e 730a 2020 2020 2020 746f 2074  tions.      to t
-00003230: 6861 7420 576f 726b 206f 7220 4465 7269  hat Work or Deri
-00003240: 7661 7469 7665 2057 6f72 6b73 2074 6865  vative Works the
-00003250: 7265 6f66 2c20 7468 6174 2069 7320 696e  reof, that is in
-00003260: 7465 6e74 696f 6e61 6c6c 790a 2020 2020  tentionally.    
-00003270: 2020 7375 626d 6974 7465 6420 746f 204c    submitted to L
-00003280: 6963 656e 736f 7220 666f 7220 696e 636c  icensor for incl
-00003290: 7573 696f 6e20 696e 2074 6865 2057 6f72  usion in the Wor
-000032a0: 6b20 6279 2074 6865 2063 6f70 7972 6967  k by the copyrig
-000032b0: 6874 206f 776e 6572 0a20 2020 2020 206f  ht owner.      o
-000032c0: 7220 6279 2061 6e20 696e 6469 7669 6475  r by an individu
-000032d0: 616c 206f 7220 4c65 6761 6c20 456e 7469  al or Legal Enti
-000032e0: 7479 2061 7574 686f 7269 7a65 6420 746f  ty authorized to
-000032f0: 2073 7562 6d69 7420 6f6e 2062 6568 616c   submit on behal
-00003300: 6620 6f66 0a20 2020 2020 2074 6865 2063  f of.      the c
-00003310: 6f70 7972 6967 6874 206f 776e 6572 2e20  opyright owner. 
-00003320: 466f 7220 7468 6520 7075 7270 6f73 6573  For the purposes
-00003330: 206f 6620 7468 6973 2064 6566 696e 6974   of this definit
-00003340: 696f 6e2c 2022 7375 626d 6974 7465 6422  ion, "submitted"
-00003350: 0a20 2020 2020 206d 6561 6e73 2061 6e79  .      means any
-00003360: 2066 6f72 6d20 6f66 2065 6c65 6374 726f   form of electro
-00003370: 6e69 632c 2076 6572 6261 6c2c 206f 7220  nic, verbal, or 
-00003380: 7772 6974 7465 6e20 636f 6d6d 756e 6963  written communic
-00003390: 6174 696f 6e20 7365 6e74 0a20 2020 2020  ation sent.     
-000033a0: 2074 6f20 7468 6520 4c69 6365 6e73 6f72   to the Licensor
-000033b0: 206f 7220 6974 7320 7265 7072 6573 656e   or its represen
-000033c0: 7461 7469 7665 732c 2069 6e63 6c75 6469  tatives, includi
-000033d0: 6e67 2062 7574 206e 6f74 206c 696d 6974  ng but not limit
-000033e0: 6564 2074 6f0a 2020 2020 2020 636f 6d6d  ed to.      comm
-000033f0: 756e 6963 6174 696f 6e20 6f6e 2065 6c65  unication on ele
-00003400: 6374 726f 6e69 6320 6d61 696c 696e 6720  ctronic mailing 
-00003410: 6c69 7374 732c 2073 6f75 7263 6520 636f  lists, source co
-00003420: 6465 2063 6f6e 7472 6f6c 2073 7973 7465  de control syste
-00003430: 6d73 2c0a 2020 2020 2020 616e 6420 6973  ms,.      and is
-00003440: 7375 6520 7472 6163 6b69 6e67 2073 7973  sue tracking sys
-00003450: 7465 6d73 2074 6861 7420 6172 6520 6d61  tems that are ma
-00003460: 6e61 6765 6420 6279 2c20 6f72 206f 6e20  naged by, or on 
-00003470: 6265 6861 6c66 206f 662c 2074 6865 0a20  behalf of, the. 
-00003480: 2020 2020 204c 6963 656e 736f 7220 666f       Licensor fo
-00003490: 7220 7468 6520 7075 7270 6f73 6520 6f66  r the purpose of
-000034a0: 2064 6973 6375 7373 696e 6720 616e 6420   discussing and 
-000034b0: 696d 7072 6f76 696e 6720 7468 6520 576f  improving the Wo
-000034c0: 726b 2c20 6275 740a 2020 2020 2020 6578  rk, but.      ex
-000034d0: 636c 7564 696e 6720 636f 6d6d 756e 6963  cluding communic
-000034e0: 6174 696f 6e20 7468 6174 2069 7320 636f  ation that is co
-000034f0: 6e73 7069 6375 6f75 736c 7920 6d61 726b  nspicuously mark
-00003500: 6564 206f 7220 6f74 6865 7277 6973 650a  ed or otherwise.
-00003510: 2020 2020 2020 6465 7369 676e 6174 6564        designated
-00003520: 2069 6e20 7772 6974 696e 6720 6279 2074   in writing by t
-00003530: 6865 2063 6f70 7972 6967 6874 206f 776e  he copyright own
-00003540: 6572 2061 7320 224e 6f74 2061 2043 6f6e  er as "Not a Con
-00003550: 7472 6962 7574 696f 6e2e 220a 0a20 2020  tribution."..   
-00003560: 2020 2022 436f 6e74 7269 6275 746f 7222     "Contributor"
-00003570: 2073 6861 6c6c 206d 6561 6e20 4c69 6365   shall mean Lice
-00003580: 6e73 6f72 2061 6e64 2061 6e79 2069 6e64  nsor and any ind
-00003590: 6976 6964 7561 6c20 6f72 204c 6567 616c  ividual or Legal
-000035a0: 2045 6e74 6974 790a 2020 2020 2020 6f6e   Entity.      on
-000035b0: 2062 6568 616c 6620 6f66 2077 686f 6d20   behalf of whom 
-000035c0: 6120 436f 6e74 7269 6275 7469 6f6e 2068  a Contribution h
-000035d0: 6173 2062 6565 6e20 7265 6365 6976 6564  as been received
-000035e0: 2062 7920 4c69 6365 6e73 6f72 2061 6e64   by Licensor and
-000035f0: 0a20 2020 2020 2073 7562 7365 7175 656e  .      subsequen
-00003600: 746c 7920 696e 636f 7270 6f72 6174 6564  tly incorporated
-00003610: 2077 6974 6869 6e20 7468 6520 576f 726b   within the Work
-00003620: 2e0a 0a20 2020 322e 2047 7261 6e74 206f  ...   2. Grant o
-00003630: 6620 436f 7079 7269 6768 7420 4c69 6365  f Copyright Lice
-00003640: 6e73 652e 2053 7562 6a65 6374 2074 6f20  nse. Subject to 
-00003650: 7468 6520 7465 726d 7320 616e 6420 636f  the terms and co
-00003660: 6e64 6974 696f 6e73 206f 660a 2020 2020  nditions of.    
-00003670: 2020 7468 6973 204c 6963 656e 7365 2c20    this License, 
-00003680: 6561 6368 2043 6f6e 7472 6962 7574 6f72  each Contributor
-00003690: 2068 6572 6562 7920 6772 616e 7473 2074   hereby grants t
-000036a0: 6f20 596f 7520 6120 7065 7270 6574 7561  o You a perpetua
-000036b0: 6c2c 0a20 2020 2020 2077 6f72 6c64 7769  l,.      worldwi
-000036c0: 6465 2c20 6e6f 6e2d 6578 636c 7573 6976  de, non-exclusiv
-000036d0: 652c 206e 6f2d 6368 6172 6765 2c20 726f  e, no-charge, ro
-000036e0: 7961 6c74 792d 6672 6565 2c20 6972 7265  yalty-free, irre
-000036f0: 766f 6361 626c 650a 2020 2020 2020 636f  vocable.      co
-00003700: 7079 7269 6768 7420 6c69 6365 6e73 6520  pyright license 
-00003710: 746f 2072 6570 726f 6475 6365 2c20 7072  to reproduce, pr
-00003720: 6570 6172 6520 4465 7269 7661 7469 7665  epare Derivative
-00003730: 2057 6f72 6b73 206f 662c 0a20 2020 2020   Works of,.     
-00003740: 2070 7562 6c69 636c 7920 6469 7370 6c61   publicly displa
-00003750: 792c 2070 7562 6c69 636c 7920 7065 7266  y, publicly perf
-00003760: 6f72 6d2c 2073 7562 6c69 6365 6e73 652c  orm, sublicense,
-00003770: 2061 6e64 2064 6973 7472 6962 7574 6520   and distribute 
-00003780: 7468 650a 2020 2020 2020 576f 726b 2061  the.      Work a
-00003790: 6e64 2073 7563 6820 4465 7269 7661 7469  nd such Derivati
-000037a0: 7665 2057 6f72 6b73 2069 6e20 536f 7572  ve Works in Sour
-000037b0: 6365 206f 7220 4f62 6a65 6374 2066 6f72  ce or Object for
-000037c0: 6d2e 0a0a 2020 2033 2e20 4772 616e 7420  m...   3. Grant 
-000037d0: 6f66 2050 6174 656e 7420 4c69 6365 6e73  of Patent Licens
-000037e0: 652e 2053 7562 6a65 6374 2074 6f20 7468  e. Subject to th
-000037f0: 6520 7465 726d 7320 616e 6420 636f 6e64  e terms and cond
-00003800: 6974 696f 6e73 206f 660a 2020 2020 2020  itions of.      
-00003810: 7468 6973 204c 6963 656e 7365 2c20 6561  this License, ea
-00003820: 6368 2043 6f6e 7472 6962 7574 6f72 2068  ch Contributor h
-00003830: 6572 6562 7920 6772 616e 7473 2074 6f20  ereby grants to 
-00003840: 596f 7520 6120 7065 7270 6574 7561 6c2c  You a perpetual,
-00003850: 0a20 2020 2020 2077 6f72 6c64 7769 6465  .      worldwide
-00003860: 2c20 6e6f 6e2d 6578 636c 7573 6976 652c  , non-exclusive,
-00003870: 206e 6f2d 6368 6172 6765 2c20 726f 7961   no-charge, roya
-00003880: 6c74 792d 6672 6565 2c20 6972 7265 766f  lty-free, irrevo
-00003890: 6361 626c 650a 2020 2020 2020 2865 7863  cable.      (exc
-000038a0: 6570 7420 6173 2073 7461 7465 6420 696e  ept as stated in
-000038b0: 2074 6869 7320 7365 6374 696f 6e29 2070   this section) p
-000038c0: 6174 656e 7420 6c69 6365 6e73 6520 746f  atent license to
-000038d0: 206d 616b 652c 2068 6176 6520 6d61 6465   make, have made
-000038e0: 2c0a 2020 2020 2020 7573 652c 206f 6666  ,.      use, off
-000038f0: 6572 2074 6f20 7365 6c6c 2c20 7365 6c6c  er to sell, sell
-00003900: 2c20 696d 706f 7274 2c20 616e 6420 6f74  , import, and ot
-00003910: 6865 7277 6973 6520 7472 616e 7366 6572  herwise transfer
-00003920: 2074 6865 2057 6f72 6b2c 0a20 2020 2020   the Work,.     
-00003930: 2077 6865 7265 2073 7563 6820 6c69 6365   where such lice
-00003940: 6e73 6520 6170 706c 6965 7320 6f6e 6c79  nse applies only
-00003950: 2074 6f20 7468 6f73 6520 7061 7465 6e74   to those patent
-00003960: 2063 6c61 696d 7320 6c69 6365 6e73 6162   claims licensab
-00003970: 6c65 0a20 2020 2020 2062 7920 7375 6368  le.      by such
-00003980: 2043 6f6e 7472 6962 7574 6f72 2074 6861   Contributor tha
-00003990: 7420 6172 6520 6e65 6365 7373 6172 696c  t are necessaril
-000039a0: 7920 696e 6672 696e 6765 6420 6279 2074  y infringed by t
-000039b0: 6865 6972 0a20 2020 2020 2043 6f6e 7472  heir.      Contr
-000039c0: 6962 7574 696f 6e28 7329 2061 6c6f 6e65  ibution(s) alone
-000039d0: 206f 7220 6279 2063 6f6d 6269 6e61 7469   or by combinati
-000039e0: 6f6e 206f 6620 7468 6569 7220 436f 6e74  on of their Cont
-000039f0: 7269 6275 7469 6f6e 2873 290a 2020 2020  ribution(s).    
-00003a00: 2020 7769 7468 2074 6865 2057 6f72 6b20    with the Work 
-00003a10: 746f 2077 6869 6368 2073 7563 6820 436f  to which such Co
-00003a20: 6e74 7269 6275 7469 6f6e 2873 2920 7761  ntribution(s) wa
-00003a30: 7320 7375 626d 6974 7465 642e 2049 6620  s submitted. If 
-00003a40: 596f 750a 2020 2020 2020 696e 7374 6974  You.      instit
-00003a50: 7574 6520 7061 7465 6e74 206c 6974 6967  ute patent litig
-00003a60: 6174 696f 6e20 6167 6169 6e73 7420 616e  ation against an
-00003a70: 7920 656e 7469 7479 2028 696e 636c 7564  y entity (includ
-00003a80: 696e 6720 610a 2020 2020 2020 6372 6f73  ing a.      cros
-00003a90: 732d 636c 6169 6d20 6f72 2063 6f75 6e74  s-claim or count
-00003aa0: 6572 636c 6169 6d20 696e 2061 206c 6177  erclaim in a law
-00003ab0: 7375 6974 2920 616c 6c65 6769 6e67 2074  suit) alleging t
-00003ac0: 6861 7420 7468 6520 576f 726b 0a20 2020  hat the Work.   
-00003ad0: 2020 206f 7220 6120 436f 6e74 7269 6275     or a Contribu
-00003ae0: 7469 6f6e 2069 6e63 6f72 706f 7261 7465  tion incorporate
-00003af0: 6420 7769 7468 696e 2074 6865 2057 6f72  d within the Wor
-00003b00: 6b20 636f 6e73 7469 7475 7465 7320 6469  k constitutes di
-00003b10: 7265 6374 0a20 2020 2020 206f 7220 636f  rect.      or co
-00003b20: 6e74 7269 6275 746f 7279 2070 6174 656e  ntributory paten
-00003b30: 7420 696e 6672 696e 6765 6d65 6e74 2c20  t infringement, 
-00003b40: 7468 656e 2061 6e79 2070 6174 656e 7420  then any patent 
-00003b50: 6c69 6365 6e73 6573 0a20 2020 2020 2067  licenses.      g
-00003b60: 7261 6e74 6564 2074 6f20 596f 7520 756e  ranted to You un
-00003b70: 6465 7220 7468 6973 204c 6963 656e 7365  der this License
-00003b80: 2066 6f72 2074 6861 7420 576f 726b 2073   for that Work s
-00003b90: 6861 6c6c 2074 6572 6d69 6e61 7465 0a20  hall terminate. 
-00003ba0: 2020 2020 2061 7320 6f66 2074 6865 2064       as of the d
-00003bb0: 6174 6520 7375 6368 206c 6974 6967 6174  ate such litigat
-00003bc0: 696f 6e20 6973 2066 696c 6564 2e0a 0a20  ion is filed... 
-00003bd0: 2020 342e 2052 6564 6973 7472 6962 7574    4. Redistribut
-00003be0: 696f 6e2e 2059 6f75 206d 6179 2072 6570  ion. You may rep
-00003bf0: 726f 6475 6365 2061 6e64 2064 6973 7472  roduce and distr
-00003c00: 6962 7574 6520 636f 7069 6573 206f 6620  ibute copies of 
-00003c10: 7468 650a 2020 2020 2020 576f 726b 206f  the.      Work o
-00003c20: 7220 4465 7269 7661 7469 7665 2057 6f72  r Derivative Wor
-00003c30: 6b73 2074 6865 7265 6f66 2069 6e20 616e  ks thereof in an
-00003c40: 7920 6d65 6469 756d 2c20 7769 7468 206f  y medium, with o
-00003c50: 7220 7769 7468 6f75 740a 2020 2020 2020  r without.      
-00003c60: 6d6f 6469 6669 6361 7469 6f6e 732c 2061  modifications, a
-00003c70: 6e64 2069 6e20 536f 7572 6365 206f 7220  nd in Source or 
-00003c80: 4f62 6a65 6374 2066 6f72 6d2c 2070 726f  Object form, pro
-00003c90: 7669 6465 6420 7468 6174 2059 6f75 0a20  vided that You. 
-00003ca0: 2020 2020 206d 6565 7420 7468 6520 666f       meet the fo
-00003cb0: 6c6c 6f77 696e 6720 636f 6e64 6974 696f  llowing conditio
-00003cc0: 6e73 3a0a 0a20 2020 2020 2028 6129 2059  ns:..      (a) Y
-00003cd0: 6f75 206d 7573 7420 6769 7665 2061 6e79  ou must give any
-00003ce0: 206f 7468 6572 2072 6563 6970 6965 6e74   other recipient
-00003cf0: 7320 6f66 2074 6865 2057 6f72 6b20 6f72  s of the Work or
-00003d00: 0a20 2020 2020 2020 2020 2044 6572 6976  .          Deriv
-00003d10: 6174 6976 6520 576f 726b 7320 6120 636f  ative Works a co
-00003d20: 7079 206f 6620 7468 6973 204c 6963 656e  py of this Licen
-00003d30: 7365 3b20 616e 640a 0a20 2020 2020 2028  se; and..      (
-00003d40: 6229 2059 6f75 206d 7573 7420 6361 7573  b) You must caus
-00003d50: 6520 616e 7920 6d6f 6469 6669 6564 2066  e any modified f
-00003d60: 696c 6573 2074 6f20 6361 7272 7920 7072  iles to carry pr
-00003d70: 6f6d 696e 656e 7420 6e6f 7469 6365 730a  ominent notices.
-00003d80: 2020 2020 2020 2020 2020 7374 6174 696e            statin
-00003d90: 6720 7468 6174 2059 6f75 2063 6861 6e67  g that You chang
-00003da0: 6564 2074 6865 2066 696c 6573 3b20 616e  ed the files; an
-00003db0: 640a 0a20 2020 2020 2028 6329 2059 6f75  d..      (c) You
-00003dc0: 206d 7573 7420 7265 7461 696e 2c20 696e   must retain, in
-00003dd0: 2074 6865 2053 6f75 7263 6520 666f 726d   the Source form
-00003de0: 206f 6620 616e 7920 4465 7269 7661 7469   of any Derivati
-00003df0: 7665 2057 6f72 6b73 0a20 2020 2020 2020  ve Works.       
-00003e00: 2020 2074 6861 7420 596f 7520 6469 7374     that You dist
-00003e10: 7269 6275 7465 2c20 616c 6c20 636f 7079  ribute, all copy
-00003e20: 7269 6768 742c 2070 6174 656e 742c 2074  right, patent, t
-00003e30: 7261 6465 6d61 726b 2c20 616e 640a 2020  rademark, and.  
-00003e40: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
-00003e50: 696f 6e20 6e6f 7469 6365 7320 6672 6f6d  ion notices from
-00003e60: 2074 6865 2053 6f75 7263 6520 666f 726d   the Source form
-00003e70: 206f 6620 7468 6520 576f 726b 2c0a 2020   of the Work,.  
-00003e80: 2020 2020 2020 2020 6578 636c 7564 696e          excludin
-00003e90: 6720 7468 6f73 6520 6e6f 7469 6365 7320  g those notices 
-00003ea0: 7468 6174 2064 6f20 6e6f 7420 7065 7274  that do not pert
-00003eb0: 6169 6e20 746f 2061 6e79 2070 6172 7420  ain to any part 
-00003ec0: 6f66 0a20 2020 2020 2020 2020 2074 6865  of.          the
-00003ed0: 2044 6572 6976 6174 6976 6520 576f 726b   Derivative Work
-00003ee0: 733b 2061 6e64 0a0a 2020 2020 2020 2864  s; and..      (d
-00003ef0: 2920 4966 2074 6865 2057 6f72 6b20 696e  ) If the Work in
-00003f00: 636c 7564 6573 2061 2022 4e4f 5449 4345  cludes a "NOTICE
-00003f10: 2220 7465 7874 2066 696c 6520 6173 2070  " text file as p
-00003f20: 6172 7420 6f66 2069 7473 0a20 2020 2020  art of its.     
-00003f30: 2020 2020 2064 6973 7472 6962 7574 696f       distributio
-00003f40: 6e2c 2074 6865 6e20 616e 7920 4465 7269  n, then any Deri
-00003f50: 7661 7469 7665 2057 6f72 6b73 2074 6861  vative Works tha
-00003f60: 7420 596f 7520 6469 7374 7269 6275 7465  t You distribute
-00003f70: 206d 7573 740a 2020 2020 2020 2020 2020   must.          
-00003f80: 696e 636c 7564 6520 6120 7265 6164 6162  include a readab
-00003f90: 6c65 2063 6f70 7920 6f66 2074 6865 2061  le copy of the a
-00003fa0: 7474 7269 6275 7469 6f6e 206e 6f74 6963  ttribution notic
-00003fb0: 6573 2063 6f6e 7461 696e 6564 0a20 2020  es contained.   
-00003fc0: 2020 2020 2020 2077 6974 6869 6e20 7375         within su
-00003fd0: 6368 204e 4f54 4943 4520 6669 6c65 2c20  ch NOTICE file, 
-00003fe0: 6578 636c 7564 696e 6720 7468 6f73 6520  excluding those 
-00003ff0: 6e6f 7469 6365 7320 7468 6174 2064 6f20  notices that do 
-00004000: 6e6f 740a 2020 2020 2020 2020 2020 7065  not.          pe
-00004010: 7274 6169 6e20 746f 2061 6e79 2070 6172  rtain to any par
-00004020: 7420 6f66 2074 6865 2044 6572 6976 6174  t of the Derivat
-00004030: 6976 6520 576f 726b 732c 2069 6e20 6174  ive Works, in at
-00004040: 206c 6561 7374 206f 6e65 0a20 2020 2020   least one.     
-00004050: 2020 2020 206f 6620 7468 6520 666f 6c6c       of the foll
-00004060: 6f77 696e 6720 706c 6163 6573 3a20 7769  owing places: wi
-00004070: 7468 696e 2061 204e 4f54 4943 4520 7465  thin a NOTICE te
-00004080: 7874 2066 696c 6520 6469 7374 7269 6275  xt file distribu
-00004090: 7465 640a 2020 2020 2020 2020 2020 6173  ted.          as
-000040a0: 2070 6172 7420 6f66 2074 6865 2044 6572   part of the Der
-000040b0: 6976 6174 6976 6520 576f 726b 733b 2077  ivative Works; w
-000040c0: 6974 6869 6e20 7468 6520 536f 7572 6365  ithin the Source
-000040d0: 2066 6f72 6d20 6f72 0a20 2020 2020 2020   form or.       
-000040e0: 2020 2064 6f63 756d 656e 7461 7469 6f6e     documentation
-000040f0: 2c20 6966 2070 726f 7669 6465 6420 616c  , if provided al
-00004100: 6f6e 6720 7769 7468 2074 6865 2044 6572  ong with the Der
-00004110: 6976 6174 6976 6520 576f 726b 733b 206f  ivative Works; o
-00004120: 722c 0a20 2020 2020 2020 2020 2077 6974  r,.          wit
-00004130: 6869 6e20 6120 6469 7370 6c61 7920 6765  hin a display ge
-00004140: 6e65 7261 7465 6420 6279 2074 6865 2044  nerated by the D
-00004150: 6572 6976 6174 6976 6520 576f 726b 732c  erivative Works,
-00004160: 2069 6620 616e 640a 2020 2020 2020 2020   if and.        
-00004170: 2020 7768 6572 6576 6572 2073 7563 6820    wherever such 
-00004180: 7468 6972 642d 7061 7274 7920 6e6f 7469  third-party noti
-00004190: 6365 7320 6e6f 726d 616c 6c79 2061 7070  ces normally app
-000041a0: 6561 722e 2054 6865 2063 6f6e 7465 6e74  ear. The content
-000041b0: 730a 2020 2020 2020 2020 2020 6f66 2074  s.          of t
-000041c0: 6865 204e 4f54 4943 4520 6669 6c65 2061  he NOTICE file a
-000041d0: 7265 2066 6f72 2069 6e66 6f72 6d61 7469  re for informati
-000041e0: 6f6e 616c 2070 7572 706f 7365 7320 6f6e  onal purposes on
-000041f0: 6c79 2061 6e64 0a20 2020 2020 2020 2020  ly and.         
-00004200: 2064 6f20 6e6f 7420 6d6f 6469 6679 2074   do not modify t
-00004210: 6865 204c 6963 656e 7365 2e20 596f 7520  he License. You 
-00004220: 6d61 7920 6164 6420 596f 7572 206f 776e  may add Your own
-00004230: 2061 7474 7269 6275 7469 6f6e 0a20 2020   attribution.   
-00004240: 2020 2020 2020 206e 6f74 6963 6573 2077         notices w
-00004250: 6974 6869 6e20 4465 7269 7661 7469 7665  ithin Derivative
-00004260: 2057 6f72 6b73 2074 6861 7420 596f 7520   Works that You 
-00004270: 6469 7374 7269 6275 7465 2c20 616c 6f6e  distribute, alon
-00004280: 6773 6964 650a 2020 2020 2020 2020 2020  gside.          
-00004290: 6f72 2061 7320 616e 2061 6464 656e 6475  or as an addendu
-000042a0: 6d20 746f 2074 6865 204e 4f54 4943 4520  m to the NOTICE 
-000042b0: 7465 7874 2066 726f 6d20 7468 6520 576f  text from the Wo
-000042c0: 726b 2c20 7072 6f76 6964 6564 0a20 2020  rk, provided.   
-000042d0: 2020 2020 2020 2074 6861 7420 7375 6368         that such
-000042e0: 2061 6464 6974 696f 6e61 6c20 6174 7472   additional attr
-000042f0: 6962 7574 696f 6e20 6e6f 7469 6365 7320  ibution notices 
-00004300: 6361 6e6e 6f74 2062 6520 636f 6e73 7472  cannot be constr
-00004310: 7565 640a 2020 2020 2020 2020 2020 6173  ued.          as
-00004320: 206d 6f64 6966 7969 6e67 2074 6865 204c   modifying the L
-00004330: 6963 656e 7365 2e0a 0a20 2020 2020 2059  icense...      Y
-00004340: 6f75 206d 6179 2061 6464 2059 6f75 7220  ou may add Your 
-00004350: 6f77 6e20 636f 7079 7269 6768 7420 7374  own copyright st
-00004360: 6174 656d 656e 7420 746f 2059 6f75 7220  atement to Your 
-00004370: 6d6f 6469 6669 6361 7469 6f6e 7320 616e  modifications an
-00004380: 640a 2020 2020 2020 6d61 7920 7072 6f76  d.      may prov
-00004390: 6964 6520 6164 6469 7469 6f6e 616c 206f  ide additional o
-000043a0: 7220 6469 6666 6572 656e 7420 6c69 6365  r different lice
-000043b0: 6e73 6520 7465 726d 7320 616e 6420 636f  nse terms and co
-000043c0: 6e64 6974 696f 6e73 0a20 2020 2020 2066  nditions.      f
-000043d0: 6f72 2075 7365 2c20 7265 7072 6f64 7563  or use, reproduc
-000043e0: 7469 6f6e 2c20 6f72 2064 6973 7472 6962  tion, or distrib
-000043f0: 7574 696f 6e20 6f66 2059 6f75 7220 6d6f  ution of Your mo
-00004400: 6469 6669 6361 7469 6f6e 732c 206f 720a  difications, or.
-00004410: 2020 2020 2020 666f 7220 616e 7920 7375        for any su
-00004420: 6368 2044 6572 6976 6174 6976 6520 576f  ch Derivative Wo
-00004430: 726b 7320 6173 2061 2077 686f 6c65 2c20  rks as a whole, 
-00004440: 7072 6f76 6964 6564 2059 6f75 7220 7573  provided Your us
-00004450: 652c 0a20 2020 2020 2072 6570 726f 6475  e,.      reprodu
-00004460: 6374 696f 6e2c 2061 6e64 2064 6973 7472  ction, and distr
-00004470: 6962 7574 696f 6e20 6f66 2074 6865 2057  ibution of the W
-00004480: 6f72 6b20 6f74 6865 7277 6973 6520 636f  ork otherwise co
-00004490: 6d70 6c69 6573 2077 6974 680a 2020 2020  mplies with.    
-000044a0: 2020 7468 6520 636f 6e64 6974 696f 6e73    the conditions
-000044b0: 2073 7461 7465 6420 696e 2074 6869 7320   stated in this 
-000044c0: 4c69 6365 6e73 652e 0a0a 2020 2035 2e20  License...   5. 
-000044d0: 5375 626d 6973 7369 6f6e 206f 6620 436f  Submission of Co
-000044e0: 6e74 7269 6275 7469 6f6e 732e 2055 6e6c  ntributions. Unl
-000044f0: 6573 7320 596f 7520 6578 706c 6963 6974  ess You explicit
-00004500: 6c79 2073 7461 7465 206f 7468 6572 7769  ly state otherwi
-00004510: 7365 2c0a 2020 2020 2020 616e 7920 436f  se,.      any Co
-00004520: 6e74 7269 6275 7469 6f6e 2069 6e74 656e  ntribution inten
-00004530: 7469 6f6e 616c 6c79 2073 7562 6d69 7474  tionally submitt
-00004540: 6564 2066 6f72 2069 6e63 6c75 7369 6f6e  ed for inclusion
-00004550: 2069 6e20 7468 6520 576f 726b 0a20 2020   in the Work.   
-00004560: 2020 2062 7920 596f 7520 746f 2074 6865     by You to the
-00004570: 204c 6963 656e 736f 7220 7368 616c 6c20   Licensor shall 
-00004580: 6265 2075 6e64 6572 2074 6865 2074 6572  be under the ter
-00004590: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
-000045a0: 7320 6f66 0a20 2020 2020 2074 6869 7320  s of.      this 
-000045b0: 4c69 6365 6e73 652c 2077 6974 686f 7574  License, without
-000045c0: 2061 6e79 2061 6464 6974 696f 6e61 6c20   any additional 
-000045d0: 7465 726d 7320 6f72 2063 6f6e 6469 7469  terms or conditi
-000045e0: 6f6e 732e 0a20 2020 2020 204e 6f74 7769  ons..      Notwi
-000045f0: 7468 7374 616e 6469 6e67 2074 6865 2061  thstanding the a
-00004600: 626f 7665 2c20 6e6f 7468 696e 6720 6865  bove, nothing he
-00004610: 7265 696e 2073 6861 6c6c 2073 7570 6572  rein shall super
-00004620: 7365 6465 206f 7220 6d6f 6469 6679 0a20  sede or modify. 
-00004630: 2020 2020 2074 6865 2074 6572 6d73 206f       the terms o
-00004640: 6620 616e 7920 7365 7061 7261 7465 206c  f any separate l
-00004650: 6963 656e 7365 2061 6772 6565 6d65 6e74  icense agreement
-00004660: 2079 6f75 206d 6179 2068 6176 6520 6578   you may have ex
-00004670: 6563 7574 6564 0a20 2020 2020 2077 6974  ecuted.      wit
-00004680: 6820 4c69 6365 6e73 6f72 2072 6567 6172  h Licensor regar
-00004690: 6469 6e67 2073 7563 6820 436f 6e74 7269  ding such Contri
-000046a0: 6275 7469 6f6e 732e 0a0a 2020 2036 2e20  butions...   6. 
-000046b0: 5472 6164 656d 6172 6b73 2e20 5468 6973  Trademarks. This
-000046c0: 204c 6963 656e 7365 2064 6f65 7320 6e6f   License does no
-000046d0: 7420 6772 616e 7420 7065 726d 6973 7369  t grant permissi
-000046e0: 6f6e 2074 6f20 7573 6520 7468 6520 7472  on to use the tr
-000046f0: 6164 650a 2020 2020 2020 6e61 6d65 732c  ade.      names,
-00004700: 2074 7261 6465 6d61 726b 732c 2073 6572   trademarks, ser
-00004710: 7669 6365 206d 6172 6b73 2c20 6f72 2070  vice marks, or p
-00004720: 726f 6475 6374 206e 616d 6573 206f 6620  roduct names of 
-00004730: 7468 6520 4c69 6365 6e73 6f72 2c0a 2020  the Licensor,.  
-00004740: 2020 2020 6578 6365 7074 2061 7320 7265      except as re
-00004750: 7175 6972 6564 2066 6f72 2072 6561 736f  quired for reaso
-00004760: 6e61 626c 6520 616e 6420 6375 7374 6f6d  nable and custom
-00004770: 6172 7920 7573 6520 696e 2064 6573 6372  ary use in descr
-00004780: 6962 696e 6720 7468 650a 2020 2020 2020  ibing the.      
-00004790: 6f72 6967 696e 206f 6620 7468 6520 576f  origin of the Wo
-000047a0: 726b 2061 6e64 2072 6570 726f 6475 6369  rk and reproduci
-000047b0: 6e67 2074 6865 2063 6f6e 7465 6e74 206f  ng the content o
-000047c0: 6620 7468 6520 4e4f 5449 4345 2066 696c  f the NOTICE fil
-000047d0: 652e 0a0a 2020 2037 2e20 4469 7363 6c61  e...   7. Discla
-000047e0: 696d 6572 206f 6620 5761 7272 616e 7479  imer of Warranty
-000047f0: 2e20 556e 6c65 7373 2072 6571 7569 7265  . Unless require
-00004800: 6420 6279 2061 7070 6c69 6361 626c 6520  d by applicable 
-00004810: 6c61 7720 6f72 0a20 2020 2020 2061 6772  law or.      agr
-00004820: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
-00004830: 672c 204c 6963 656e 736f 7220 7072 6f76  g, Licensor prov
-00004840: 6964 6573 2074 6865 2057 6f72 6b20 2861  ides the Work (a
-00004850: 6e64 2065 6163 680a 2020 2020 2020 436f  nd each.      Co
-00004860: 6e74 7269 6275 746f 7220 7072 6f76 6964  ntributor provid
-00004870: 6573 2069 7473 2043 6f6e 7472 6962 7574  es its Contribut
-00004880: 696f 6e73 2920 6f6e 2061 6e20 2241 5320  ions) on an "AS 
-00004890: 4953 2220 4241 5349 532c 0a20 2020 2020  IS" BASIS,.     
-000048a0: 2057 4954 484f 5554 2057 4152 5241 4e54   WITHOUT WARRANT
-000048b0: 4945 5320 4f52 2043 4f4e 4449 5449 4f4e  IES OR CONDITION
-000048c0: 5320 4f46 2041 4e59 204b 494e 442c 2065  S OF ANY KIND, e
-000048d0: 6974 6865 7220 6578 7072 6573 7320 6f72  ither express or
-000048e0: 0a20 2020 2020 2069 6d70 6c69 6564 2c20  .      implied, 
-000048f0: 696e 636c 7564 696e 672c 2077 6974 686f  including, witho
-00004900: 7574 206c 696d 6974 6174 696f 6e2c 2061  ut limitation, a
-00004910: 6e79 2077 6172 7261 6e74 6965 7320 6f72  ny warranties or
-00004920: 2063 6f6e 6469 7469 6f6e 730a 2020 2020   conditions.    
-00004930: 2020 6f66 2054 4954 4c45 2c20 4e4f 4e2d    of TITLE, NON-
-00004940: 494e 4652 494e 4745 4d45 4e54 2c20 4d45  INFRINGEMENT, ME
-00004950: 5243 4841 4e54 4142 494c 4954 592c 206f  RCHANTABILITY, o
-00004960: 7220 4649 544e 4553 5320 464f 5220 410a  r FITNESS FOR A.
-00004970: 2020 2020 2020 5041 5254 4943 554c 4152        PARTICULAR
-00004980: 2050 5552 504f 5345 2e20 596f 7520 6172   PURPOSE. You ar
-00004990: 6520 736f 6c65 6c79 2072 6573 706f 6e73  e solely respons
-000049a0: 6962 6c65 2066 6f72 2064 6574 6572 6d69  ible for determi
-000049b0: 6e69 6e67 2074 6865 0a20 2020 2020 2061  ning the.      a
-000049c0: 7070 726f 7072 6961 7465 6e65 7373 206f  ppropriateness o
-000049d0: 6620 7573 696e 6720 6f72 2072 6564 6973  f using or redis
-000049e0: 7472 6962 7574 696e 6720 7468 6520 576f  tributing the Wo
-000049f0: 726b 2061 6e64 2061 7373 756d 6520 616e  rk and assume an
-00004a00: 790a 2020 2020 2020 7269 736b 7320 6173  y.      risks as
-00004a10: 736f 6369 6174 6564 2077 6974 6820 596f  sociated with Yo
-00004a20: 7572 2065 7865 7263 6973 6520 6f66 2070  ur exercise of p
-00004a30: 6572 6d69 7373 696f 6e73 2075 6e64 6572  ermissions under
-00004a40: 2074 6869 7320 4c69 6365 6e73 652e 0a0a   this License...
-00004a50: 2020 2038 2e20 4c69 6d69 7461 7469 6f6e     8. Limitation
-00004a60: 206f 6620 4c69 6162 696c 6974 792e 2049   of Liability. I
-00004a70: 6e20 6e6f 2065 7665 6e74 2061 6e64 2075  n no event and u
-00004a80: 6e64 6572 206e 6f20 6c65 6761 6c20 7468  nder no legal th
-00004a90: 656f 7279 2c0a 2020 2020 2020 7768 6574  eory,.      whet
-00004aa0: 6865 7220 696e 2074 6f72 7420 2869 6e63  her in tort (inc
-00004ab0: 6c75 6469 6e67 206e 6567 6c69 6765 6e63  luding negligenc
-00004ac0: 6529 2c20 636f 6e74 7261 6374 2c20 6f72  e), contract, or
-00004ad0: 206f 7468 6572 7769 7365 2c0a 2020 2020   otherwise,.    
-00004ae0: 2020 756e 6c65 7373 2072 6571 7569 7265    unless require
-00004af0: 6420 6279 2061 7070 6c69 6361 626c 6520  d by applicable 
-00004b00: 6c61 7720 2873 7563 6820 6173 2064 656c  law (such as del
-00004b10: 6962 6572 6174 6520 616e 6420 6772 6f73  iberate and gros
-00004b20: 736c 790a 2020 2020 2020 6e65 676c 6967  sly.      neglig
-00004b30: 656e 7420 6163 7473 2920 6f72 2061 6772  ent acts) or agr
-00004b40: 6565 6420 746f 2069 6e20 7772 6974 696e  eed to in writin
-00004b50: 672c 2073 6861 6c6c 2061 6e79 2043 6f6e  g, shall any Con
-00004b60: 7472 6962 7574 6f72 2062 650a 2020 2020  tributor be.    
-00004b70: 2020 6c69 6162 6c65 2074 6f20 596f 7520    liable to You 
-00004b80: 666f 7220 6461 6d61 6765 732c 2069 6e63  for damages, inc
-00004b90: 6c75 6469 6e67 2061 6e79 2064 6972 6563  luding any direc
-00004ba0: 742c 2069 6e64 6972 6563 742c 2073 7065  t, indirect, spe
-00004bb0: 6369 616c 2c0a 2020 2020 2020 696e 6369  cial,.      inci
-00004bc0: 6465 6e74 616c 2c20 6f72 2063 6f6e 7365  dental, or conse
-00004bd0: 7175 656e 7469 616c 2064 616d 6167 6573  quential damages
-00004be0: 206f 6620 616e 7920 6368 6172 6163 7465   of any characte
-00004bf0: 7220 6172 6973 696e 6720 6173 2061 0a20  r arising as a. 
-00004c00: 2020 2020 2072 6573 756c 7420 6f66 2074       result of t
-00004c10: 6869 7320 4c69 6365 6e73 6520 6f72 206f  his License or o
-00004c20: 7574 206f 6620 7468 6520 7573 6520 6f72  ut of the use or
-00004c30: 2069 6e61 6269 6c69 7479 2074 6f20 7573   inability to us
-00004c40: 6520 7468 650a 2020 2020 2020 576f 726b  e the.      Work
-00004c50: 2028 696e 636c 7564 696e 6720 6275 7420   (including but 
-00004c60: 6e6f 7420 6c69 6d69 7465 6420 746f 2064  not limited to d
-00004c70: 616d 6167 6573 2066 6f72 206c 6f73 7320  amages for loss 
-00004c80: 6f66 2067 6f6f 6477 696c 6c2c 0a20 2020  of goodwill,.   
-00004c90: 2020 2077 6f72 6b20 7374 6f70 7061 6765     work stoppage
-00004ca0: 2c20 636f 6d70 7574 6572 2066 6169 6c75  , computer failu
-00004cb0: 7265 206f 7220 6d61 6c66 756e 6374 696f  re or malfunctio
-00004cc0: 6e2c 206f 7220 616e 7920 616e 6420 616c  n, or any and al
-00004cd0: 6c0a 2020 2020 2020 6f74 6865 7220 636f  l.      other co
-00004ce0: 6d6d 6572 6369 616c 2064 616d 6167 6573  mmercial damages
-00004cf0: 206f 7220 6c6f 7373 6573 292c 2065 7665   or losses), eve
-00004d00: 6e20 6966 2073 7563 6820 436f 6e74 7269  n if such Contri
-00004d10: 6275 746f 720a 2020 2020 2020 6861 7320  butor.      has 
-00004d20: 6265 656e 2061 6476 6973 6564 206f 6620  been advised of 
-00004d30: 7468 6520 706f 7373 6962 696c 6974 7920  the possibility 
-00004d40: 6f66 2073 7563 6820 6461 6d61 6765 732e  of such damages.
-00004d50: 0a0a 2020 2039 2e20 4163 6365 7074 696e  ..   9. Acceptin
-00004d60: 6720 5761 7272 616e 7479 206f 7220 4164  g Warranty or Ad
-00004d70: 6469 7469 6f6e 616c 204c 6961 6269 6c69  ditional Liabili
-00004d80: 7479 2e20 5768 696c 6520 7265 6469 7374  ty. While redist
-00004d90: 7269 6275 7469 6e67 0a20 2020 2020 2074  ributing.      t
-00004da0: 6865 2057 6f72 6b20 6f72 2044 6572 6976  he Work or Deriv
-00004db0: 6174 6976 6520 576f 726b 7320 7468 6572  ative Works ther
-00004dc0: 656f 662c 2059 6f75 206d 6179 2063 686f  eof, You may cho
-00004dd0: 6f73 6520 746f 206f 6666 6572 2c0a 2020  ose to offer,.  
-00004de0: 2020 2020 616e 6420 6368 6172 6765 2061      and charge a
-00004df0: 2066 6565 2066 6f72 2c20 6163 6365 7074   fee for, accept
-00004e00: 616e 6365 206f 6620 7375 7070 6f72 742c  ance of support,
-00004e10: 2077 6172 7261 6e74 792c 2069 6e64 656d   warranty, indem
-00004e20: 6e69 7479 2c0a 2020 2020 2020 6f72 206f  nity,.      or o
-00004e30: 7468 6572 206c 6961 6269 6c69 7479 206f  ther liability o
-00004e40: 626c 6967 6174 696f 6e73 2061 6e64 2f6f  bligations and/o
-00004e50: 7220 7269 6768 7473 2063 6f6e 7369 7374  r rights consist
-00004e60: 656e 7420 7769 7468 2074 6869 730a 2020  ent with this.  
-00004e70: 2020 2020 4c69 6365 6e73 652e 2048 6f77      License. How
-00004e80: 6576 6572 2c20 696e 2061 6363 6570 7469  ever, in accepti
-00004e90: 6e67 2073 7563 6820 6f62 6c69 6761 7469  ng such obligati
-00004ea0: 6f6e 732c 2059 6f75 206d 6179 2061 6374  ons, You may act
-00004eb0: 206f 6e6c 790a 2020 2020 2020 6f6e 2059   only.      on Y
-00004ec0: 6f75 7220 6f77 6e20 6265 6861 6c66 2061  our own behalf a
-00004ed0: 6e64 206f 6e20 596f 7572 2073 6f6c 6520  nd on Your sole 
-00004ee0: 7265 7370 6f6e 7369 6269 6c69 7479 2c20  responsibility, 
-00004ef0: 6e6f 7420 6f6e 2062 6568 616c 660a 2020  not on behalf.  
-00004f00: 2020 2020 6f66 2061 6e79 206f 7468 6572      of any other
-00004f10: 2043 6f6e 7472 6962 7574 6f72 2c20 616e   Contributor, an
-00004f20: 6420 6f6e 6c79 2069 6620 596f 7520 6167  d only if You ag
-00004f30: 7265 6520 746f 2069 6e64 656d 6e69 6679  ree to indemnify
-00004f40: 2c0a 2020 2020 2020 6465 6665 6e64 2c20  ,.      defend, 
-00004f50: 616e 6420 686f 6c64 2065 6163 6820 436f  and hold each Co
-00004f60: 6e74 7269 6275 746f 7220 6861 726d 6c65  ntributor harmle
-00004f70: 7373 2066 6f72 2061 6e79 206c 6961 6269  ss for any liabi
-00004f80: 6c69 7479 0a20 2020 2020 2069 6e63 7572  lity.      incur
-00004f90: 7265 6420 6279 2c20 6f72 2063 6c61 696d  red by, or claim
-00004fa0: 7320 6173 7365 7274 6564 2061 6761 696e  s asserted again
-00004fb0: 7374 2c20 7375 6368 2043 6f6e 7472 6962  st, such Contrib
-00004fc0: 7574 6f72 2062 7920 7265 6173 6f6e 0a20  utor by reason. 
-00004fd0: 2020 2020 206f 6620 796f 7572 2061 6363       of your acc
-00004fe0: 6570 7469 6e67 2061 6e79 2073 7563 6820  epting any such 
-00004ff0: 7761 7272 616e 7479 206f 7220 6164 6469  warranty or addi
-00005000: 7469 6f6e 616c 206c 6961 6269 6c69 7479  tional liability
-00005010: 2e0a 0a20 2020 454e 4420 4f46 2054 4552  ...   END OF TER
-00005020: 4d53 2041 4e44 2043 4f4e 4449 5449 4f4e  MS AND CONDITION
-00005030: 530a 0a20 2020 436f 7079 7269 6768 7420  S..   Copyright 
-00005040: 3230 3230 2d32 3032 3220 4a69 6e61 2041  2020-2022 Jina A
-00005050: 4920 4c69 6d69 7465 640a 0a20 2020 4c69  I Limited..   Li
-00005060: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
-00005070: 2041 7061 6368 6520 4c69 6365 6e73 652c   Apache License,
-00005080: 2056 6572 7369 6f6e 2032 2e30 2028 7468   Version 2.0 (th
-00005090: 6520 224c 6963 656e 7365 2229 3b0a 2020  e "License");.  
-000050a0: 2079 6f75 206d 6179 206e 6f74 2075 7365   you may not use
-000050b0: 2074 6869 7320 6669 6c65 2065 7863 6570   this file excep
-000050c0: 7420 696e 2063 6f6d 706c 6961 6e63 6520  t in compliance 
-000050d0: 7769 7468 2074 6865 204c 6963 656e 7365  with the License
-000050e0: 2e0a 2020 2059 6f75 206d 6179 206f 6274  ..   You may obt
-000050f0: 6169 6e20 6120 636f 7079 206f 6620 7468  ain a copy of th
-00005100: 6520 4c69 6365 6e73 6520 6174 0a0a 2020  e License at..  
-00005110: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
-00005120: 6170 6163 6865 2e6f 7267 2f6c 6963 656e  apache.org/licen
-00005130: 7365 732f 4c49 4345 4e53 452d 322e 300a  ses/LICENSE-2.0.
-00005140: 0a20 2020 556e 6c65 7373 2072 6571 7569  .   Unless requi
-00005150: 7265 6420 6279 2061 7070 6c69 6361 626c  red by applicabl
-00005160: 6520 6c61 7720 6f72 2061 6772 6565 6420  e law or agreed 
-00005170: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
-00005180: 6f66 7477 6172 650a 2020 2064 6973 7472  oftware.   distr
-00005190: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
-000051a0: 204c 6963 656e 7365 2069 7320 6469 7374   License is dist
-000051b0: 7269 6275 7465 6420 6f6e 2061 6e20 2241  ributed on an "A
-000051c0: 5320 4953 2220 4241 5349 532c 0a20 2020  S IS" BASIS,.   
-000051d0: 5749 5448 4f55 5420 5741 5252 414e 5449  WITHOUT WARRANTI
-000051e0: 4553 204f 5220 434f 4e44 4954 494f 4e53  ES OR CONDITIONS
-000051f0: 204f 4620 414e 5920 4b49 4e44 2c20 6569   OF ANY KIND, ei
-00005200: 7468 6572 2065 7870 7265 7373 206f 7220  ther express or 
-00005210: 696d 706c 6965 642e 0a20 2020 5365 6520  implied..   See 
-00005220: 7468 6520 4c69 6365 6e73 6520 666f 7220  the License for 
-00005230: 7468 6520 7370 6563 6966 6963 206c 616e  the specific lan
-00005240: 6775 6167 6520 676f 7665 726e 696e 6720  guage governing 
-00005250: 7065 726d 6973 7369 6f6e 7320 616e 640a  permissions and.
-00005260: 2020 206c 696d 6974 6174 696f 6e73 2075     limitations u
-00005270: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
-00005280: 2e0a 0a                                  ...
+00000030: 6f6e 3a20 302e 302e 320a 5375 6d6d 6172  on: 0.0.2.Summar
+00000040: 793a 2041 6e20 6f70 656e 2d73 6f75 7263  y: An open-sourc
+00000050: 6520 636c 6f75 642d 6e61 7469 7665 206f  e cloud-native o
+00000060: 6620 6c61 7267 6520 6d75 6c74 692d 6d6f  f large multi-mo
+00000070: 6461 6c20 6d6f 6465 6c73 2028 4c4d 4d73  dal models (LMMs
+00000080: 2920 7365 7276 696e 6720 6672 616d 6577  ) serving framew
+00000090: 6f72 6b2e 0a48 6f6d 652d 7061 6765 3a20  ork..Home-page: 
+000000a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000b0: 6f6d 2f6a 696e 612d 6169 2f6f 7065 6e67  om/jina-ai/openg
+000000c0: 7074 0a4c 6963 656e 7365 3a20 4170 6163  pt.License: Apac
+000000d0: 6865 2d32 2e30 0a4b 6579 776f 7264 733a  he-2.0.Keywords:
+000000e0: 2050 7974 6f72 6368 2c4c 4d4d 2c47 5054   Pytorch,LMM,GPT
+000000f0: 2c4c 4c4d 2c6d 756c 7469 2d6d 6f64 616c  ,LLM,multi-modal
+00000100: 6974 792c 636c 6f75 642d 6e61 7469 7665  ity,cloud-native
+00000110: 2c6d 6f64 656c 2d73 6572 7669 6e67 2c6d  ,model-serving,m
+00000120: 6f64 656c 2d69 6e66 6572 656e 6365 2c6c  odel-inference,l
+00000130: 6c61 6d61 2c76 6963 756e 612c 7374 6162  lama,vicuna,stab
+00000140: 656c 6c6d 0a41 7574 686f 723a 204a 696e  ellm.Author: Jin
+00000150: 6120 4149 0a41 7574 686f 722d 656d 6169  a AI.Author-emai
+00000160: 6c3a 2068 656c 6c6f 406a 696e 612e 6169  l: hello@jina.ai
+00000170: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+00000180: 3a20 3e3d 332e 382c 3c34 2e30 0a43 6c61  : >=3.8,<4.0.Cla
+00000190: 7373 6966 6965 723a 2044 6576 656c 6f70  ssifier: Develop
+000001a0: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
+000001b0: 202d 2042 6574 610a 436c 6173 7369 6669   - Beta.Classifi
+000001c0: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+000001d0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+000001e0: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
+000001f0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000200: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
+00000210: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
+00000220: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+00000230: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
+00000240: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+00000250: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000260: 204f 7065 7261 7469 6e67 2053 7973 7465   Operating Syste
+00000270: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000280: 656e 740a 436c 6173 7369 6669 6572 3a20  ent.Classifier: 
+00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002b0: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+000002c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002e0: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+000002f0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000310: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000320: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000330: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000340: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000350: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000360: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000370: 7974 686f 6e20 3a3a 2033 2e31 310a 436c  ython :: 3.11.Cl
+00000380: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000390: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000003a0: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+000003b0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000003c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000003d0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+000003e0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000003f0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000400: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000410: 2e31 310a 436c 6173 7369 6669 6572 3a20  .11.Classifier: 
+00000420: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000430: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000440: 3a20 332e 380a 436c 6173 7369 6669 6572  : 3.8.Classifier
+00000450: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000460: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000470: 203a 3a20 332e 390a 436c 6173 7369 6669   :: 3.9.Classifi
+00000480: 6572 3a20 546f 7069 6320 3a3a 2053 6369  er: Topic :: Sci
+00000490: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+000004a0: 696e 670a 436c 6173 7369 6669 6572 3a20  ing.Classifier: 
+000004b0: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
+000004c0: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
+000004d0: 3a3a 2041 7274 6966 6963 6961 6c20 496e  :: Artificial In
+000004e0: 7465 6c6c 6967 656e 6365 0a43 6c61 7373  telligence.Class
+000004f0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
+00000500: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+00000510: 6565 7269 6e67 203a 3a20 4d61 7468 656d  eering :: Mathem
+00000520: 6174 6963 730a 436c 6173 7369 6669 6572  atics.Classifier
+00000530: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
+00000540: 6172 6520 4465 7665 6c6f 706d 656e 740a  are Development.
+00000550: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000560: 6320 3a3a 2053 6f66 7477 6172 6520 4465  c :: Software De
+00000570: 7665 6c6f 706d 656e 7420 3a3a 204c 6962  velopment :: Lib
+00000580: 7261 7269 6573 0a43 6c61 7373 6966 6965  raries.Classifie
+00000590: 723a 2054 6f70 6963 203a 3a20 536f 6674  r: Topic :: Soft
+000005a0: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+000005b0: 203a 3a20 4c69 6272 6172 6965 7320 3a3a   :: Libraries ::
+000005c0: 2050 7974 686f 6e20 4d6f 6475 6c65 730a   Python Modules.
+000005d0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000005e0: 666c 616d 696e 676f 0a50 726f 7669 6465  flamingo.Provide
+000005f0: 732d 4578 7472 613a 2070 6c61 7967 726f  s-Extra: playgro
+00000600: 756e 640a 5265 7175 6972 6573 2d44 6973  und.Requires-Dis
+00000610: 743a 2061 6363 656c 6572 6174 6520 283e  t: accelerate (>
+00000620: 3d30 2e31 382e 302c 3c30 2e31 392e 3029  =0.18.0,<0.19.0)
+00000630: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000640: 636c 656f 2028 3e3d 322e 302e 302c 3c33  cleo (>=2.0.0,<3
+00000650: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+00000660: 6973 743a 2063 6c69 636b 2028 3e3d 382e  ist: click (>=8.
+00000670: 312e 332c 3c39 2e30 2e30 290a 5265 7175  1.3,<9.0.0).Requ
+00000680: 6972 6573 2d44 6973 743a 2064 6f63 6172  ires-Dist: docar
+00000690: 7261 7920 283e 3d30 2e32 312e 302c 3c30  ray (>=0.21.0,<0
+000006a0: 2e32 322e 3029 0a52 6571 7569 7265 732d  .22.0).Requires-
+000006b0: 4469 7374 3a20 6569 6e6f 7073 2028 3e3d  Dist: einops (>=
+000006c0: 302e 362e 302c 3c30 2e37 2e30 290a 5265  0.6.0,<0.7.0).Re
+000006d0: 7175 6972 6573 2d44 6973 743a 2067 7261  quires-Dist: gra
+000006e0: 6469 6f20 283e 3d33 2e33 302e 302c 3c34  dio (>=3.30.0,<4
+000006f0: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
+00000700: 2022 706c 6179 6772 6f75 6e64 220a 5265   "playground".Re
+00000710: 7175 6972 6573 2d44 6973 743a 206a 696e  quires-Dist: jin
+00000720: 6120 283e 3d33 2e31 352e 302c 3c34 2e30  a (>=3.15.0,<4.0
+00000730: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
+00000740: 743a 206c 6f67 7572 7520 283e 3d30 2e35  t: loguru (>=0.5
+00000750: 2c3c 302e 3629 0a52 6571 7569 7265 732d  ,<0.6).Requires-
+00000760: 4469 7374 3a20 6d61 726b 646f 776e 3220  Dist: markdown2 
+00000770: 283e 3d32 2e34 2e30 2c3c 332e 302e 3029  (>=2.4.0,<3.0.0)
+00000780: 203b 2065 7874 7261 203d 3d20 2270 6c61   ; extra == "pla
+00000790: 7967 726f 756e 6422 0a52 6571 7569 7265  yground".Require
+000007a0: 732d 4469 7374 3a20 6d64 7465 7832 6874  s-Dist: mdtex2ht
+000007b0: 6d6c 2028 3e3d 312e 322e 302c 3c32 2e30  ml (>=1.2.0,<2.0
+000007c0: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
+000007d0: 706c 6179 6772 6f75 6e64 220a 5265 7175  playground".Requ
+000007e0: 6972 6573 2d44 6973 743a 206e 756d 7079  ires-Dist: numpy
+000007f0: 2028 3e3d 312e 3231 2e32 2c3c 322e 302e   (>=1.21.2,<2.0.
+00000800: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000810: 3a20 6f70 656e 2d66 6c61 6d69 6e67 6f20  : open-flamingo 
+00000820: 283e 3d30 2e30 2c3c 302e 3129 203b 2065  (>=0.0,<0.1) ; e
+00000830: 7874 7261 203d 3d20 2266 6c61 6d69 6e67  xtra == "flaming
+00000840: 6f22 0a52 6571 7569 7265 732d 4469 7374  o".Requires-Dist
+00000850: 3a20 6f70 656e 5f63 6c69 705f 746f 7263  : open_clip_torc
+00000860: 6820 283e 3d32 2e31 362c 3c33 2e30 290a  h (>=2.16,<3.0).
+00000870: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000880: 7164 6d20 283e 3d34 2e36 322e 332c 3c35  qdm (>=4.62.3,<5
+00000890: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+000008a0: 6973 743a 2074 7261 6e73 666f 726d 6572  ist: transformer
+000008b0: 7320 283e 3d34 2e32 382e 302c 3c35 2e30  s (>=4.28.0,<5.0
+000008c0: 2e30 290a 5072 6f6a 6563 742d 5552 4c3a  .0).Project-URL:
+000008d0: 2052 6570 6f73 6974 6f72 792c 2068 7474   Repository, htt
+000008e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000008f0: 6a69 6e61 2d61 692f 6f70 656e 6770 740a  jina-ai/opengpt.
+00000900: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00000910: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00000920: 6172 6b64 6f77 6e0a 0a23 20e2 9884 efb8  arkdown..# .....
+00000930: 8f20 4f70 656e 4750 540a 0a3c 7020 616c  . OpenGPT..<p al
+00000940: 6967 6e3d 2263 656e 7465 7222 3e0a 3c61  ign="center">.<a
+00000950: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000960: 6974 6875 622e 636f 6d2f 6a69 6e61 2d61  ithub.com/jina-a
+00000970: 692f 6f70 656e 6770 7422 3e3c 696d 6720  i/opengpt"><img 
+00000980: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000990: 6875 622e 636f 6d2f 6a69 6e61 2d61 692f  hub.com/jina-ai/
+000009a0: 6f70 656e 6770 742f 626c 6f62 2f6d 6169  opengpt/blob/mai
+000009b0: 6e2f 2e67 6974 6875 622f 696d 6167 6573  n/.github/images
+000009c0: 2f6c 6f67 6f2e 706e 673f 2220 616c 743d  /logo.png?" alt=
+000009d0: 224f 7065 6e47 5054 3a20 416e 206f 7065  "OpenGPT: An ope
+000009e0: 6e2d 736f 7572 6365 2063 6c6f 7564 2d6e  n-source cloud-n
+000009f0: 6174 6976 6520 6c61 7267 652d 7363 616c  ative large-scal
+00000a00: 6520 6d75 6c74 696d 6f64 616c 206d 6f64  e multimodal mod
+00000a10: 656c 2073 6572 7669 6e67 2066 7261 6d65  el serving frame
+00000a20: 776f 726b 2220 7769 6474 683d 2233 3030  work" width="300
+00000a30: 7078 223e 3c2f 613e 0a3c 6272 3e0a 3c2f  px"></a>.<br>.</
+00000a40: 703e 0a0a 3e20 2241 2070 6c61 7966 756c  p>..> "A playful
+00000a50: 2061 6e64 2077 6869 6d73 6963 616c 2076   and whimsical v
+00000a60: 6563 746f 7220 6172 7420 6f66 2061 2053  ector art of a S
+00000a70: 746f 6368 6173 7469 6320 5469 6767 6572  tochastic Tigger
+00000a80: 2c20 7765 6172 696e 6720 6120 742d 7368  , wearing a t-sh
+00000a90: 6972 7420 7769 7468 2061 2022 4750 5422  irt with a "GPT"
+00000aa0: 2074 6578 7420 7072 696e 7465 6420 6c6f   text printed lo
+00000ab0: 676f 2c20 7375 7272 6f75 6e64 6564 2062  go, surrounded b
+00000ac0: 7920 636f 6c6f 7266 756c 2067 656f 6d65  y colorful geome
+00000ad0: 7472 6963 2073 6861 7065 732e 2020 e280  tric shapes.  ..
+00000ae0: 9361 7220 313a 3120 e280 9375 7062 6574  .ar 1:1 ...upbet
+00000af0: 6122 0a3e 0a3e 20e2 8094 2050 726f 6d70  a".>.> ... Promp
+00000b00: 7473 2061 6e64 206c 6f67 6f20 6172 7420  ts and logo art 
+00000b10: 7761 7320 7072 6f64 7563 6564 2077 6974  was produced wit
+00000b20: 6820 205b 5072 6f6d 7074 5065 7266 6563  h  [PromptPerfec
+00000b30: 745d 2868 7474 7073 3a2f 2f70 726f 6d70  t](https://promp
+00000b40: 7470 6572 6665 6374 2e6a 696e 612e 6169  tperfect.jina.ai
+00000b50: 2f29 2026 205b 5374 6162 6c65 2044 6966  /) & [Stable Dif
+00000b60: 6675 7369 6f6e 2058 5d28 6874 7470 733a  fusion X](https:
+00000b70: 2f2f 636c 6970 6472 6f70 2e63 6f2f 7374  //clipdrop.co/st
+00000b80: 6162 6c65 2d64 6966 6675 7369 6f6e 290a  able-diffusion).
+00000b90: 0a0a 215b 5d28 6874 7470 733a 2f2f 696d  ..![](https://im
+00000ba0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000bb0: 6765 2f4d 6164 6525 3230 7769 7468 2d4a  ge/Made%20with-J
+00000bc0: 696e 6141 492d 626c 7565 7669 6f6c 6574  inaAI-blueviolet
+00000bd0: 3f73 7479 6c65 3d66 6c61 7429 0a5b 215b  ?style=flat).[![
+00000be0: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
+00000bf0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000c00: 692f 762f 6f70 656e 5f67 7074 5f74 6f72  i/v/open_gpt_tor
+00000c10: 6368 295d 2868 7474 7073 3a2f 2f70 7970  ch)](https://pyp
+00000c20: 692e 6f72 672f 7072 6f6a 6563 742f 6f70  i.org/project/op
+00000c30: 656e 5f67 7074 5f74 6f72 6368 2f29 0a5b  en_gpt_torch/).[
+00000c40: 215b 5079 5049 202d 204c 6963 656e 7365  ![PyPI - License
+00000c50: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000c60: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
+00000c70: 6f70 656e 5f67 7074 5f74 6f72 6368 295d  open_gpt_torch)]
+00000c80: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00000c90: 672f 7072 6f6a 6563 742f 6f70 656e 5f67  g/project/open_g
+00000ca0: 7074 5f74 6f72 6368 2f29 0a0a 2a2a 4f70  pt_torch/)..**Op
+00000cb0: 656e 4750 542a 2a20 6973 2061 6e20 6f70  enGPT** is an op
+00000cc0: 656e 2d73 6f75 7263 6520 5f63 6c6f 7564  en-source _cloud
+00000cd0: 2d6e 6174 6976 655f 206c 6172 6765 2d73  -native_ large-s
+00000ce0: 6361 6c65 202a 2a5f 6d75 6c74 696d 6f64  cale **_multimod
+00000cf0: 616c 206d 6f64 656c 735f 2a2a 2028 4c4d  al models_** (LM
+00000d00: 4d73 2920 7365 7276 696e 6720 6672 616d  Ms) serving fram
+00000d10: 6577 6f72 6b2e 200a 4974 2069 7320 6465  ework. .It is de
+00000d20: 7369 676e 6564 2074 6f20 7369 6d70 6c69  signed to simpli
+00000d30: 6679 2074 6865 2064 6570 6c6f 796d 656e  fy the deploymen
+00000d40: 7420 616e 6420 6d61 6e61 6765 6d65 6e74  t and management
+00000d50: 206f 6620 6c61 7267 6520 6c61 6e67 7561   of large langua
+00000d60: 6765 206d 6f64 656c 732c 206f 6e20 6120  ge models, on a 
+00000d70: 6469 7374 7269 6275 7465 6420 636c 7573  distributed clus
+00000d80: 7465 7220 6f66 2047 5055 732e 0a0a 2323  ter of GPUs...##
+00000d90: 2054 6162 6c65 206f 6620 636f 6e74 656e   Table of conten
+00000da0: 7473 0a0a 2d20 5b46 6561 7475 7265 735d  ts..- [Features]
+00000db0: 2823 6665 6174 7572 6573 290a 2d20 5b53  (#features).- [S
+00000dc0: 7570 706f 7274 6564 206d 6f64 656c 735d  upported models]
+00000dd0: 2823 7375 7070 6f72 7465 642d 6d6f 6465  (#supported-mode
+00000de0: 6c73 290a 2d20 5b47 6574 2073 7461 7274  ls).- [Get start
+00000df0: 6564 5d28 2367 6574 2d73 7461 7274 6564  ed](#get-started
+00000e00: 290a 2d20 5b42 7569 6c64 2061 206d 6f64  ).- [Build a mod
+00000e10: 656c 2073 6572 7669 6e67 2069 6e20 6f6e  el serving in on
+00000e20: 6520 6c69 6e65 5d28 2362 7569 6c64 2d61  e line](#build-a
+00000e30: 2d6d 6f64 656c 2d73 6572 7669 6e67 2d69  -model-serving-i
+00000e40: 6e2d 6f6e 652d 6c69 6e65 290a 2d20 5b43  n-one-line).- [C
+00000e50: 6c6f 7564 2d6e 6174 6976 6520 6465 706c  loud-native depl
+00000e60: 6f79 6d65 6e74 5d28 2363 6c6f 7564 2d6e  oyment](#cloud-n
+00000e70: 6174 6976 652d 6465 706c 6f79 6d65 6e74  ative-deployment
+00000e80: 290a 2d20 5b52 6f61 646d 6170 5d28 2372  ).- [Roadmap](#r
+00000e90: 6f61 646d 6170 290a 0a23 2320 4665 6174  oadmap)..## Feat
+00000ea0: 7572 6573 0a0a 4f70 656e 4750 5420 7072  ures..OpenGPT pr
+00000eb0: 6f76 6964 6573 2074 6865 2066 6f6c 6c6f  ovides the follo
+00000ec0: 7769 6e67 2066 6561 7475 7265 7320 746f  wing features to
+00000ed0: 206d 616b 6520 6974 2065 6173 7920 746f   make it easy to
+00000ee0: 2064 6570 6c6f 7920 616e 6420 7365 7276   deploy and serv
+00000ef0: 6520 2a2a 6c61 7267 6520 6d75 6c74 692d  e **large multi-
+00000f00: 6d6f 6461 6c20 6d6f 6465 6c73 2a2a 2028  modal models** (
+00000f10: 4c4d 4d73 2920 6174 2073 6361 6c65 3a0a  LMMs) at scale:.
+00000f20: 0a2d 2053 7570 706f 7274 2066 6f72 206d  .- Support for m
+00000f30: 756c 7469 2d6d 6f64 616c 206d 6f64 656c  ulti-modal model
+00000f40: 7320 6f6e 2074 6f70 206f 6620 6c61 7267  s on top of larg
+00000f50: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
+00000f60: 730a 2d20 5363 616c 6162 6c65 2061 7263  s.- Scalable arc
+00000f70: 6869 7465 6374 7572 6520 666f 7220 6861  hitecture for ha
+00000f80: 6e64 6c69 6e67 2068 6967 6820 7472 6166  ndling high traf
+00000f90: 6669 6320 6c6f 6164 730a 2d20 4f70 7469  fic loads.- Opti
+00000fa0: 6d69 7a65 6420 666f 7220 6c6f 772d 6c61  mized for low-la
+00000fb0: 7465 6e63 7920 696e 6665 7265 6e63 650a  tency inference.
+00000fc0: 2d20 4175 746f 6d61 7469 6320 6d6f 6465  - Automatic mode
+00000fd0: 6c20 7061 7274 6974 696f 6e69 6e67 2061  l partitioning a
+00000fe0: 6e64 2064 6973 7472 6962 7574 696f 6e20  nd distribution 
+00000ff0: 6163 726f 7373 206d 756c 7469 706c 6520  across multiple 
+00001000: 4750 5573 0a2d 2043 656e 7472 616c 697a  GPUs.- Centraliz
+00001010: 6564 206d 6f64 656c 206d 616e 6167 656d  ed model managem
+00001020: 656e 7420 616e 6420 6d6f 6e69 746f 7269  ent and monitori
+00001030: 6e67 0a2d 2052 4553 5420 4150 4920 666f  ng.- REST API fo
+00001040: 7220 6561 7379 2069 6e74 6567 7261 7469  r easy integrati
+00001050: 6f6e 2077 6974 6820 6578 6973 7469 6e67  on with existing
+00001060: 2061 7070 6c69 6361 7469 6f6e 730a 0a23   applications..#
+00001070: 2320 5570 6461 7465 730a 0a2d 202a 2a32  # Updates..- **2
+00001080: 3032 332d 3035 2d31 322a 2a3a 20f0 9f8e  023-05-12**: ...
+00001090: 8957 6520 6861 7665 2072 656c 6561 7365  .We have release
+000010a0: 6420 7468 6520 6669 7273 7420 7665 7273  d the first vers
+000010b0: 696f 6e20 6076 302e 302e 3160 206f 6620  ion `v0.0.1` of 
+000010c0: 4f70 656e 4750 542e 2059 6f75 2063 616e  OpenGPT. You can
+000010d0: 2069 6e73 7461 6c6c 2069 7420 7769 7468   install it with
+000010e0: 2060 7069 7020 696e 7374 616c 6c20 6f70   `pip install op
+000010f0: 656e 5f67 7074 5f74 6f72 6368 602e 0a0a  en_gpt_torch`...
+00001100: 2323 2053 7570 706f 7274 6564 204d 6f64  ## Supported Mod
+00001110: 656c 730a 0a3c 6465 7461 696c 733e 0a0a  els..<details>..
+00001120: 4f70 656e 4750 5420 7375 7070 6f72 7473  OpenGPT supports
+00001130: 2074 6865 2066 6f6c 6c6f 7769 6e67 206d   the following m
+00001140: 6f64 656c 7320 6f75 7420 6f66 2074 6865  odels out of the
+00001150: 2062 6f78 3a0a 0a2d 204c 4c4d 2028 4c61   box:..- LLM (La
+00001160: 7267 6520 4c61 6e67 7561 6765 204d 6f64  rge Language Mod
+00001170: 656c 290a 0a20 202d 205b 4c4c 614d 415d  el)..  - [LLaMA]
+00001180: 2868 7474 7073 3a2f 2f61 692e 6661 6365  (https://ai.face
+00001190: 626f 6f6b 2e63 6f6d 2f62 6c6f 672f 6c61  book.com/blog/la
+000011a0: 7267 652d 6c61 6e67 7561 6765 2d6d 6f64  rge-language-mod
+000011b0: 656c 2d6c 6c61 6d61 2d6d 6574 612d 6169  el-llama-meta-ai
+000011c0: 2f29 3a20 6f70 656e 2061 6e64 2065 6666  /): open and eff
+000011d0: 6963 6965 6e74 2066 6f75 6e64 6174 696f  icient foundatio
+000011e0: 6e20 6c61 6e67 7561 6765 206d 6f64 656c  n language model
+000011f0: 7320 6279 204d 6574 610a 2020 2d20 5b50  s by Meta.  - [P
+00001200: 7974 6869 615d 2868 7474 7073 3a2f 2f67  ythia](https://g
+00001210: 6974 6875 622e 636f 6d2f 456c 6575 7468  ithub.com/Eleuth
+00001220: 6572 4149 2f70 7974 6869 6129 3a20 6120  erAI/pythia): a 
+00001230: 636f 6c6c 6563 7469 6f6e 206f 6620 6d6f  collection of mo
+00001240: 6465 6c73 2064 6576 656c 6f70 6564 2074  dels developed t
+00001250: 6f20 6661 6369 6c69 7461 7465 2069 6e74  o facilitate int
+00001260: 6572 7072 6574 6162 696c 6974 7920 7265  erpretability re
+00001270: 7365 6172 6368 2062 7920 456c 6575 7468  search by Eleuth
+00001280: 6572 4149 0a20 202d 205b 5374 6162 6c65  erAI.  - [Stable
+00001290: 4c4d 5d28 6874 7470 733a 2f2f 6769 7468  LM](https://gith
+000012a0: 7562 2e63 6f6d 2f53 7461 6269 6c69 7479  ub.com/Stability
+000012b0: 2d41 492f 5374 6162 6c65 4c4d 293a 2073  -AI/StableLM): s
+000012c0: 6572 6965 7320 6f66 206c 6172 6765 206c  eries of large l
+000012d0: 616e 6775 6167 6520 6d6f 6465 6c73 2062  anguage models b
+000012e0: 7920 5374 6162 696c 6974 7920 4149 0a20  y Stability AI. 
+000012f0: 202d 205b 5669 6375 6e61 5d28 6874 7470   - [Vicuna](http
+00001300: 733a 2f2f 7669 6375 6e61 2e6c 6d73 7973  s://vicuna.lmsys
+00001310: 2e6f 7267 2f29 3a20 6120 6368 6174 2061  .org/): a chat a
+00001320: 7373 6973 7461 6e74 2066 696e 652d 7475  ssistant fine-tu
+00001330: 6e65 6420 6672 6f6d 204c 4c61 4d41 206f  ned from LLaMA o
+00001340: 6e20 7573 6572 2d73 6861 7265 6420 636f  n user-shared co
+00001350: 6e76 6572 7361 7469 6f6e 7320 6279 204c  nversations by L
+00001360: 4d53 5953 0a20 202d 205b 4d4f 5353 5d28  MSYS.  - [MOSS](
+00001370: 6874 7470 733a 2f2f 7478 7375 6e31 3939  https://txsun199
+00001380: 372e 6769 7468 7562 2e69 6f2f 626c 6f67  7.github.io/blog
+00001390: 732f 6d6f 7373 2e68 746d 6c29 3a20 636f  s/moss.html): co
+000013a0: 6e76 6572 7361 7469 6f6e 616c 206c 616e  nversational lan
+000013b0: 6775 6167 6520 6d6f 6465 6c20 6672 6f6d  guage model from
+000013c0: 2046 7564 616e 2055 6e69 7665 7273 6974   Fudan Universit
+000013d0: 790a 0a2d 204c 4d4d 2028 4c61 7267 6520  y..- LMM (Large 
+000013e0: 4d75 6c74 692d 6d6f 6461 6c20 4d6f 6465  Multi-modal Mode
+000013f0: 6c29 0a0a 2020 2d20 5b4f 7065 6e46 6c61  l)..  - [OpenFla
+00001400: 6d69 6e67 6f5d 2868 7474 7073 3a2f 2f67  mingo](https://g
+00001410: 6974 6875 622e 636f 6d2f 6d6c 666f 756e  ithub.com/mlfoun
+00001420: 6461 7469 6f6e 732f 6f70 656e 5f66 6c61  dations/open_fla
+00001430: 6d69 6e67 6f29 3a20 616e 206f 7065 6e20  mingo): an open 
+00001440: 736f 7572 6365 2076 6572 7369 6f6e 206f  source version o
+00001450: 6620 4465 6570 4d69 6e64 2773 205b 466c  f DeepMind's [Fl
+00001460: 616d 696e 676f 5d28 6874 7470 733a 2f2f  amingo](https://
+00001470: 7777 772e 6465 6570 6d69 6e64 2e63 6f6d  www.deepmind.com
+00001480: 2f62 6c6f 672f 7461 636b 6c69 6e67 2d6d  /blog/tackling-m
+00001490: 756c 7469 706c 652d 7461 736b 732d 7769  ultiple-tasks-wi
+000014a0: 7468 2d61 2d73 696e 676c 652d 7669 7375  th-a-single-visu
+000014b0: 616c 2d6c 616e 6775 6167 652d 6d6f 6465  al-language-mode
+000014c0: 6c29 206d 6f64 656c 0a20 202d 205b 4d69  l) model.  - [Mi
+000014d0: 6e69 4750 542d 345d 2868 7474 7073 3a2f  niGPT-4](https:/
+000014e0: 2f6d 696e 6967 7074 2d34 2e67 6974 6875  /minigpt-4.githu
+000014f0: 622e 696f 2f29 3a20 616c 6967 6e73 2061  b.io/): aligns a
+00001500: 2066 726f 7a65 6e20 7669 7375 616c 2065   frozen visual e
+00001510: 6e63 6f64 6572 2077 6974 6820 6120 6672  ncoder with a fr
+00001520: 6f7a 656e 204c 4c4d 2c20 5669 6375 6e61  ozen LLM, Vicuna
+00001530: 2c20 7573 696e 6720 6a75 7374 206f 6e65  , using just one
+00001540: 2070 726f 6a65 6374 696f 6e20 6c61 7965   projection laye
+00001550: 722e 200a 0a46 6f72 206d 6f72 6520 6465  r. ..For more de
+00001560: 7461 696c 7320 6162 6f75 7420 7468 6520  tails about the 
+00001570: 7375 7070 6f72 7465 6420 6d6f 6465 6c73  supported models
+00001580: 2c20 706c 6561 7365 2073 6565 2074 6865  , please see the
+00001590: 205b 4d6f 6465 6c20 5a6f 6f5d 282e 2f4d   [Model Zoo](./M
+000015a0: 4f44 454c 5f5a 4f4f 2e6d 6429 2e0a 0a3c  ODEL_ZOO.md)...<
+000015b0: 2f64 6574 6169 6c73 3e0a 0a0a 2323 2052  /details>...## R
+000015c0: 6f61 646d 6170 0a0a 596f 7520 6361 6e20  oadmap..You can 
+000015d0: 7669 6577 206f 7572 2072 6f61 646d 6170  view our roadmap
+000015e0: 2077 6974 6820 6665 6174 7572 6573 2074   with features t
+000015f0: 6861 7420 6172 6520 706c 616e 6e65 642c  hat are planned,
+00001600: 2073 7461 7274 6564 2c20 616e 6420 636f   started, and co
+00001610: 6d70 6c65 7465 6420 6f6e 2074 6865 205b  mpleted on the [
+00001620: 526f 6164 6d61 7020 6469 7363 7573 7369  Roadmap discussi
+00001630: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00001640: 7562 2e63 6f6d 2f6a 696e 612d 6169 2f6f  ub.com/jina-ai/o
+00001650: 7065 6e67 7074 2f64 6973 6375 7373 696f  pengpt/discussio
+00001660: 6e73 2f63 6174 6567 6f72 6965 732f 726f  ns/categories/ro
+00001670: 6164 6d61 7029 2063 6174 6567 6f72 792e  admap) category.
+00001680: 0a0a 2323 2047 6574 2053 7461 7274 6564  ..## Get Started
+00001690: 0a0a 2323 2320 496e 7374 616c 6c61 7469  ..### Installati
+000016a0: 6f6e 0a0a 496e 7374 616c 6c20 7468 6520  on..Install the 
+000016b0: 7061 636b 6167 6520 7769 7468 2060 7069  package with `pi
+000016c0: 7060 3a0a 0a60 6060 6261 7368 0a70 6970  p`:..```bash.pip
+000016d0: 2069 6e73 7461 6c6c 206f 7065 6e5f 6770   install open_gp
+000016e0: 745f 746f 7263 680a 6060 600a 0a23 2323  t_torch.```..###
+000016f0: 2051 7569 636b 7374 6172 740a 0a60 6060   Quickstart..```
+00001700: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f70  python.import op
+00001710: 656e 5f67 7074 0a0a 6d6f 6465 6c20 3d20  en_gpt..model = 
+00001720: 6f70 656e 5f67 7074 2e63 7265 6174 655f  open_gpt.create_
+00001730: 6d6f 6465 6c28 2766 6163 6562 6f6f 6b2f  model('facebook/
+00001740: 6c6c 616d 612d 3762 272c 2064 6576 6963  llama-7b', devic
+00001750: 653d 2763 7564 6127 2c20 7072 6563 6973  e='cuda', precis
+00001760: 696f 6e3d 2766 7031 3627 290a 0a70 726f  ion='fp16')..pro
+00001770: 6d70 7420 3d20 2254 6865 2071 7569 636b  mpt = "The quick
+00001780: 2062 726f 776e 2066 6f78 206a 756d 7073   brown fox jumps
+00001790: 206f 7665 7220 7468 6520 6c61 7a79 2064   over the lazy d
+000017a0: 6f67 2e22 0a0a 6f75 7470 7574 203d 206d  og."..output = m
+000017b0: 6f64 656c 2e67 656e 6572 6174 6528 0a20  odel.generate(. 
+000017c0: 2020 2070 726f 6d70 742c 0a20 2020 206d     prompt,.    m
+000017d0: 6178 5f6c 656e 6774 683d 3130 302c 0a20  ax_length=100,. 
+000017e0: 2020 2074 656d 7065 7261 7475 7265 3d30     temperature=0
+000017f0: 2e39 2c0a 2020 2020 746f 705f 6b3d 3530  .9,.    top_k=50
+00001800: 2c0a 2020 2020 746f 705f 703d 302e 3935  ,.    top_p=0.95
+00001810: 2c0a 2020 2020 7265 7065 7469 7469 6f6e  ,.    repetition
+00001820: 5f70 656e 616c 7479 3d31 2e32 2c0a 2020  _penalty=1.2,.  
+00001830: 2020 646f 5f73 616d 706c 653d 5472 7565    do_sample=True
+00001840: 2c0a 2020 2020 6e75 6d5f 7265 7475 726e  ,.    num_return
+00001850: 5f73 6571 7565 6e63 6573 3d31 2c0a 290a  _sequences=1,.).
+00001860: 6060 600a 0a3e 202a 2a57 6172 6e69 6e67  ```..> **Warning
+00001870: 2a2a 0a3e 2049 6e20 7468 6520 6162 6f76  **.> In the abov
+00001880: 6520 6578 616d 706c 652c 2077 6520 7573  e example, we us
+00001890: 6520 6070 7265 6369 7369 6f6e 3d27 6670  e `precision='fp
+000018a0: 3136 2760 2074 6f20 7265 6475 6365 2074  16'` to reduce t
+000018b0: 6865 206d 656d 6f72 7920 7573 6167 6520  he memory usage 
+000018c0: 616e 6420 7370 6565 6420 7570 2074 6865  and speed up the
+000018d0: 2069 6e66 6572 656e 6365 2077 6974 6820   inference with 
+000018e0: 736f 6d65 206c 6f73 7320 696e 2061 6363  some loss in acc
+000018f0: 7572 6163 7920 6f6e 2074 6578 7420 6765  uracy on text ge
+00001900: 6e65 7261 7469 6f6e 2074 6173 6b73 2e20  neration tasks. 
+00001910: 0a3e 2059 6f75 2063 616e 2061 6c73 6f20  .> You can also 
+00001920: 7573 6520 6070 7265 6369 7369 6f6e 3d27  use `precision='
+00001930: 6670 3332 2760 2069 6e73 7465 6164 2061  fp32'` instead a
+00001940: 7320 796f 7520 6c69 6b65 2066 6f72 2062  s you like for b
+00001950: 6574 7465 7220 7065 7266 6f72 6d61 6e63  etter performanc
+00001960: 652e 200a 0a3e 202a 2a4e 6f74 652a 2a0a  e. ..> **Note**.
+00001970: 3e20 4974 2075 7375 616c 6c79 2074 616b  > It usually tak
+00001980: 6573 2061 2077 6869 6c65 2028 7365 7665  es a while (seve
+00001990: 7261 6c20 6d69 6e75 7465 7329 2066 6f72  ral minutes) for
+000019a0: 2074 6865 2066 6972 7374 2074 696d 6520   the first time 
+000019b0: 746f 2064 6f77 6e6c 6f61 6420 616e 6420  to download and 
+000019c0: 6c6f 6164 2074 6865 206d 6f64 656c 2069  load the model i
+000019d0: 6e74 6f20 7468 6520 6d65 6d6f 7279 2e0a  nto the memory..
+000019e0: 0a0a 496e 206d 6f73 7420 6361 7365 7320  ..In most cases 
+000019f0: 6f66 206c 6172 6765 206d 6f64 656c 2073  of large model s
+00001a00: 6572 7669 6e67 2c20 7468 6520 6d6f 6465  erving, the mode
+00001a10: 6c20 6361 6e6e 6f74 2066 6974 2069 6e74  l cannot fit int
+00001a20: 6f20 6120 7369 6e67 6c65 2047 5055 2e20  o a single GPU. 
+00001a30: 546f 2073 6f6c 7665 2074 6869 7320 7072  To solve this pr
+00001a40: 6f62 6c65 6d2c 2077 6520 616c 736f 2070  oblem, we also p
+00001a50: 726f 7669 6465 2061 2060 6465 7669 6365  rovide a `device
+00001a60: 5f6d 6170 6020 6f70 7469 6f6e 2028 7375  _map` option (su
+00001a70: 7070 6f72 7465 6420 6279 2060 6163 6365  pported by `acce
+00001a80: 636c 6561 7465 6020 7061 636b 6167 6529  cleate` package)
+00001a90: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
+00001aa0: 7920 7061 7274 6974 696f 6e20 7468 6520  y partition the 
+00001ab0: 6d6f 6465 6c20 616e 6420 6469 7374 7269  model and distri
+00001ac0: 6275 7465 2069 7420 6163 726f 7373 206d  bute it across m
+00001ad0: 756c 7469 706c 6520 4750 5573 3a0a 0a60  ultiple GPUs:..`
+00001ae0: 6060 7079 7468 6f6e 0a6d 6f64 656c 203d  ``python.model =
+00001af0: 206f 7065 6e5f 6770 742e 6372 6561 7465   open_gpt.create
+00001b00: 5f6d 6f64 656c 280a 2020 2020 2766 6163  _model(.    'fac
+00001b10: 6562 6f6f 6b2f 6c6c 616d 612d 3762 272c  ebook/llama-7b',
+00001b20: 2070 7265 6369 7369 6f6e 3d27 6670 3136   precision='fp16
+00001b30: 272c 2064 6576 6963 655f 6d61 703d 2762  ', device_map='b
+00001b40: 616c 616e 6365 6427 0a29 0a60 6060 0a0a  alanced'.).```..
+00001b50: 5365 6520 5b65 7861 6d70 6c65 7320 6f6e  See [examples on
+00001b60: 2068 6f77 2074 6f20 7573 6520 6f70 656e   how to use open
+00001b70: 6770 7420 7769 7468 2064 6966 6665 7265  gpt with differe
+00001b80: 6e74 206d 6f64 656c 732e 5d28 2e2f 6578  nt models.](./ex
+00001b90: 616d 706c 6573 290a 0a0a 2323 2042 7569  amples)...## Bui
+00001ba0: 6c64 2061 206d 6f64 656c 2073 6572 7669  ld a model servi
+00001bb0: 6e67 2069 6e20 6f6e 6520 6c69 6e65 0a0a  ng in one line..
+00001bc0: 546f 2064 6f20 736f 2c20 796f 7520 6361  To do so, you ca
+00001bd0: 6e20 7573 6520 7468 6520 6073 6572 7665  n use the `serve
+00001be0: 6020 636f 6d6d 616e 643a 0a0a 6060 6062  ` command:..```b
+00001bf0: 6173 680a 6f70 656e 6770 7420 7365 7276  ash.opengpt serv
+00001c00: 6520 6661 6365 626f 6f6b 2f6c 6c61 6d61  e facebook/llama
+00001c10: 2d37 6220 2d2d 7072 6563 6973 696f 6e20  -7b --precision 
+00001c20: 6670 3136 202d 2d70 6f72 7420 3531 3030  fp16 --port 5100
+00001c30: 300a 6060 600a 0a54 6869 7320 7769 6c6c  0.```..This will
+00001c40: 2073 7461 7274 2061 2073 6572 7665 7220   start a server 
+00001c50: 6f6e 2070 6f72 7420 6035 3130 3030 602e  on port `51000`.
+00001c60: 2059 6f75 2063 616e 2074 6865 6e20 7365   You can then se
+00001c70: 6e64 2072 6571 7565 7374 7320 746f 2074  nd requests to t
+00001c80: 6865 2073 6572 7665 723a 0a0a 6060 6070  he server:..```p
+00001c90: 7974 686f 6e0a 696d 706f 7274 2072 6571  ython.import req
+00001ca0: 7565 7374 730a 0a70 726f 6d70 7420 3d20  uests..prompt = 
+00001cb0: 2254 6865 2071 7569 636b 2062 726f 776e  "The quick brown
+00001cc0: 2066 6f78 206a 756d 7073 206f 7665 7220   fox jumps over 
+00001cd0: 7468 6520 6c61 7a79 2064 6f67 2e22 0a0a  the lazy dog."..
+00001ce0: 7265 7370 6f6e 7365 203d 2072 6571 7565  response = reque
+00001cf0: 7374 732e 706f 7374 280a 2020 2020 2268  sts.post(.    "h
+00001d00: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00001d10: 3531 3030 302f 6765 6e65 7261 7465 222c  51000/generate",
+00001d20: 0a20 2020 206a 736f 6e3d 7b0a 2020 2020  .    json={.    
+00001d30: 2020 2020 2270 726f 6d70 7422 3a20 7072      "prompt": pr
+00001d40: 6f6d 7074 2c0a 2020 2020 2020 2020 226d  ompt,.        "m
+00001d50: 6178 5f6c 656e 6774 6822 3a20 3130 302c  ax_length": 100,
+00001d60: 0a20 2020 2020 2020 2022 7465 6d70 6572  .        "temper
+00001d70: 6174 7572 6522 3a20 302e 392c 0a20 2020  ature": 0.9,.   
+00001d80: 2020 2020 2022 746f 705f 6b22 3a20 3530       "top_k": 50
+00001d90: 2c0a 2020 2020 2020 2020 2274 6f70 5f70  ,.        "top_p
+00001da0: 223a 2030 2e39 352c 0a20 2020 2020 2020  ": 0.95,.       
+00001db0: 2022 7265 7065 7469 7469 6f6e 5f70 656e   "repetition_pen
+00001dc0: 616c 7479 223a 2031 2e32 2c0a 2020 2020  alty": 1.2,.    
+00001dd0: 2020 2020 2264 6f5f 7361 6d70 6c65 223a      "do_sample":
+00001de0: 2054 7275 652c 0a20 2020 2020 2020 2022   True,.        "
+00001df0: 6e75 6d5f 7265 7475 726e 5f73 6571 7565  num_return_seque
+00001e00: 6e63 6573 223a 2031 2c0a 2020 2020 7d2c  nces": 1,.    },
+00001e10: 0a29 0a60 6060 0a0a 4e6f 7465 2074 6861  .).```..Note tha
+00001e20: 7420 7468 6520 7365 7276 6572 2077 696c  t the server wil
+00001e30: 6c20 6f6e 6c79 2061 6363 6570 7420 7265  l only accept re
+00001e40: 7175 6573 7473 2066 726f 6d20 7468 6520  quests from the 
+00001e50: 7361 6d65 206d 6163 6869 6e65 2e20 4966  same machine. If
+00001e60: 2079 6f75 2077 616e 7420 746f 2061 6363   you want to acc
+00001e70: 6570 7420 7265 7175 6573 7473 2066 726f  ept requests fro
+00001e80: 6d20 6f74 6865 7220 6d61 6368 696e 6573  m other machines
+00001e90: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
+00001ea0: 6520 602d 2d68 6f73 7460 2066 6c61 6720  e `--host` flag 
+00001eb0: 746f 2073 7065 6369 6679 2074 6865 2068  to specify the h
+00001ec0: 6f73 7420 746f 2062 696e 6420 746f 2e0a  ost to bind to..
+00001ed0: 0a23 2320 436c 6f75 642d 6e61 7469 7665  .## Cloud-native
+00001ee0: 2064 6570 6c6f 796d 656e 740a 0a59 6f75   deployment..You
+00001ef0: 2063 616e 2061 6c73 6f20 6465 706c 6f79   can also deploy
+00001f00: 2074 6865 2073 6572 7665 7220 746f 2061   the server to a
+00001f10: 2063 6c6f 7564 2070 726f 7669 6465 7220   cloud provider 
+00001f20: 6c69 6b65 204a 696e 6120 436c 6f75 6420  like Jina Cloud 
+00001f30: 6f72 2041 5753 2e0a 546f 2064 6f20 736f  or AWS..To do so
+00001f40: 2c20 796f 7520 6361 6e20 7573 6520 6064  , you can use `d
+00001f50: 6570 6c6f 7960 2063 6f6d 6d61 6e64 3a0a  eploy` command:.
+00001f60: 0a2d 204a 696e 6120 436c 6f75 640a 0a60  .- Jina Cloud..`
+00001f70: 6060 6261 7368 0a6f 7065 6e67 7074 2064  ``bash.opengpt d
+00001f80: 6570 6c6f 7920 6661 6365 626f 6f6b 2f6c  eploy facebook/l
+00001f90: 6c61 6d61 2d37 6220 2d2d 6465 7669 6365  lama-7b --device
+00001fa0: 2063 7564 6120 2d2d 7072 6563 6973 696f   cuda --precisio
+00001fb0: 6e20 6670 3136 202d 2d70 726f 7669 6465  n fp16 --provide
+00001fc0: 7220 6a69 6e61 202d 2d6e 616d 6520 6f70  r jina --name op
+00001fd0: 656e 6770 7420 2d2d 7265 706c 6963 6173  engpt --replicas
+00001fe0: 2032 0a60 6060 0a0a 2a2a 5442 4420 2e2e   2.```..**TBD ..
+00001ff0: 2e2a 2a0a 0a0a 2323 2043 6f6e 7472 6962  .**...## Contrib
+00002000: 7574 696e 670a 0a57 6520 7765 6c63 6f6d  uting..We welcom
+00002010: 6520 636f 6e74 7269 6275 7469 6f6e 7320  e contributions 
+00002020: 6672 6f6d 2074 6865 2063 6f6d 6d75 6e69  from the communi
+00002030: 7479 2120 546f 2063 6f6e 7472 6962 7574  ty! To contribut
+00002040: 652c 2070 6c65 6173 6520 7375 626d 6974  e, please submit
+00002050: 2061 2070 756c 6c20 7265 7175 6573 7420   a pull request 
+00002060: 666f 6c6c 6f77 696e 6720 6f75 7220 636f  following our co
+00002070: 6e74 7269 6275 7469 6e67 2067 7569 6465  ntributing guide
+00002080: 6c69 6e65 732e 0a0a 2323 204c 6963 656e  lines...## Licen
+00002090: 7365 0a0a 4f70 656e 4750 5420 6973 206c  se..OpenGPT is l
+000020a0: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+000020b0: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
+000020c0: 2c20 5665 7273 696f 6e20 322e 302e 2053  , Version 2.0. S
+000020d0: 6565 204c 4943 454e 5345 2066 6f72 2074  ee LICENSE for t
+000020e0: 6865 2066 756c 6c20 6c69 6365 6e73 6520  he full license 
+000020f0: 7465 7874 2e0a 436f 7079 7269 6768 7420  text..Copyright 
+00002100: 3230 3230 2d32 3032 3220 4a69 6e61 2041  2020-2022 Jina A
+00002110: 4920 4c69 6d69 7465 642e 2020 416c 6c20  I Limited.  All 
+00002120: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
+00002130: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002150: 2020 2041 7061 6368 6520 4c69 6365 6e73     Apache Licens
+00002160: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00002170: 2020 2020 2020 2020 2020 2020 2056 6572               Ver
+00002180: 7369 6f6e 2032 2e30 2c20 4a61 6e75 6172  sion 2.0, Januar
+00002190: 7920 3230 3034 0a20 2020 2020 2020 2020  y 2004.         
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+000021b0: 7474 703a 2f2f 7777 772e 6170 6163 6865  ttp://www.apache
+000021c0: 2e6f 7267 2f6c 6963 656e 7365 732f 0a0a  .org/licenses/..
+000021d0: 2020 2054 4552 4d53 2041 4e44 2043 4f4e     TERMS AND CON
+000021e0: 4449 5449 4f4e 5320 464f 5220 5553 452c  DITIONS FOR USE,
+000021f0: 2052 4550 524f 4455 4354 494f 4e2c 2041   REPRODUCTION, A
+00002200: 4e44 2044 4953 5452 4942 5554 494f 4e0a  ND DISTRIBUTION.
+00002210: 0a20 2020 312e 2044 6566 696e 6974 696f  .   1. Definitio
+00002220: 6e73 2e0a 0a20 2020 2020 2022 4c69 6365  ns...      "Lice
+00002230: 6e73 6522 2073 6861 6c6c 206d 6561 6e20  nse" shall mean 
+00002240: 7468 6520 7465 726d 7320 616e 6420 636f  the terms and co
+00002250: 6e64 6974 696f 6e73 2066 6f72 2075 7365  nditions for use
+00002260: 2c20 7265 7072 6f64 7563 7469 6f6e 2c0a  , reproduction,.
+00002270: 2020 2020 2020 616e 6420 6469 7374 7269        and distri
+00002280: 6275 7469 6f6e 2061 7320 6465 6669 6e65  bution as define
+00002290: 6420 6279 2053 6563 7469 6f6e 7320 3120  d by Sections 1 
+000022a0: 7468 726f 7567 6820 3920 6f66 2074 6869  through 9 of thi
+000022b0: 7320 646f 6375 6d65 6e74 2e0a 0a20 2020  s document...   
+000022c0: 2020 2022 4c69 6365 6e73 6f72 2220 7368     "Licensor" sh
+000022d0: 616c 6c20 6d65 616e 2074 6865 2063 6f70  all mean the cop
+000022e0: 7972 6967 6874 206f 776e 6572 206f 7220  yright owner or 
+000022f0: 656e 7469 7479 2061 7574 686f 7269 7a65  entity authorize
+00002300: 6420 6279 0a20 2020 2020 2074 6865 2063  d by.      the c
+00002310: 6f70 7972 6967 6874 206f 776e 6572 2074  opyright owner t
+00002320: 6861 7420 6973 2067 7261 6e74 696e 6720  hat is granting 
+00002330: 7468 6520 4c69 6365 6e73 652e 0a0a 2020  the License...  
+00002340: 2020 2020 224c 6567 616c 2045 6e74 6974      "Legal Entit
+00002350: 7922 2073 6861 6c6c 206d 6561 6e20 7468  y" shall mean th
+00002360: 6520 756e 696f 6e20 6f66 2074 6865 2061  e union of the a
+00002370: 6374 696e 6720 656e 7469 7479 2061 6e64  cting entity and
+00002380: 2061 6c6c 0a20 2020 2020 206f 7468 6572   all.      other
+00002390: 2065 6e74 6974 6965 7320 7468 6174 2063   entities that c
+000023a0: 6f6e 7472 6f6c 2c20 6172 6520 636f 6e74  ontrol, are cont
+000023b0: 726f 6c6c 6564 2062 792c 206f 7220 6172  rolled by, or ar
+000023c0: 6520 756e 6465 7220 636f 6d6d 6f6e 0a20  e under common. 
+000023d0: 2020 2020 2063 6f6e 7472 6f6c 2077 6974       control wit
+000023e0: 6820 7468 6174 2065 6e74 6974 792e 2046  h that entity. F
+000023f0: 6f72 2074 6865 2070 7572 706f 7365 7320  or the purposes 
+00002400: 6f66 2074 6869 7320 6465 6669 6e69 7469  of this definiti
+00002410: 6f6e 2c0a 2020 2020 2020 2263 6f6e 7472  on,.      "contr
+00002420: 6f6c 2220 6d65 616e 7320 2869 2920 7468  ol" means (i) th
+00002430: 6520 706f 7765 722c 2064 6972 6563 7420  e power, direct 
+00002440: 6f72 2069 6e64 6972 6563 742c 2074 6f20  or indirect, to 
+00002450: 6361 7573 6520 7468 650a 2020 2020 2020  cause the.      
+00002460: 6469 7265 6374 696f 6e20 6f72 206d 616e  direction or man
+00002470: 6167 656d 656e 7420 6f66 2073 7563 6820  agement of such 
+00002480: 656e 7469 7479 2c20 7768 6574 6865 7220  entity, whether 
+00002490: 6279 2063 6f6e 7472 6163 7420 6f72 0a20  by contract or. 
+000024a0: 2020 2020 206f 7468 6572 7769 7365 2c20       otherwise, 
+000024b0: 6f72 2028 6969 2920 6f77 6e65 7273 6869  or (ii) ownershi
+000024c0: 7020 6f66 2066 6966 7479 2070 6572 6365  p of fifty perce
+000024d0: 6e74 2028 3530 2529 206f 7220 6d6f 7265  nt (50%) or more
+000024e0: 206f 6620 7468 650a 2020 2020 2020 6f75   of the.      ou
+000024f0: 7473 7461 6e64 696e 6720 7368 6172 6573  tstanding shares
+00002500: 2c20 6f72 2028 6969 6929 2062 656e 6566  , or (iii) benef
+00002510: 6963 6961 6c20 6f77 6e65 7273 6869 7020  icial ownership 
+00002520: 6f66 2073 7563 6820 656e 7469 7479 2e0a  of such entity..
+00002530: 0a20 2020 2020 2022 596f 7522 2028 6f72  .      "You" (or
+00002540: 2022 596f 7572 2229 2073 6861 6c6c 206d   "Your") shall m
+00002550: 6561 6e20 616e 2069 6e64 6976 6964 7561  ean an individua
+00002560: 6c20 6f72 204c 6567 616c 2045 6e74 6974  l or Legal Entit
+00002570: 790a 2020 2020 2020 6578 6572 6369 7369  y.      exercisi
+00002580: 6e67 2070 6572 6d69 7373 696f 6e73 2067  ng permissions g
+00002590: 7261 6e74 6564 2062 7920 7468 6973 204c  ranted by this L
+000025a0: 6963 656e 7365 2e0a 0a20 2020 2020 2022  icense...      "
+000025b0: 536f 7572 6365 2220 666f 726d 2073 6861  Source" form sha
+000025c0: 6c6c 206d 6561 6e20 7468 6520 7072 6566  ll mean the pref
+000025d0: 6572 7265 6420 666f 726d 2066 6f72 206d  erred form for m
+000025e0: 616b 696e 6720 6d6f 6469 6669 6361 7469  aking modificati
+000025f0: 6f6e 732c 0a20 2020 2020 2069 6e63 6c75  ons,.      inclu
+00002600: 6469 6e67 2062 7574 206e 6f74 206c 696d  ding but not lim
+00002610: 6974 6564 2074 6f20 736f 6674 7761 7265  ited to software
+00002620: 2073 6f75 7263 6520 636f 6465 2c20 646f   source code, do
+00002630: 6375 6d65 6e74 6174 696f 6e0a 2020 2020  cumentation.    
+00002640: 2020 736f 7572 6365 2c20 616e 6420 636f    source, and co
+00002650: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00002660: 732e 0a0a 2020 2020 2020 224f 626a 6563  s...      "Objec
+00002670: 7422 2066 6f72 6d20 7368 616c 6c20 6d65  t" form shall me
+00002680: 616e 2061 6e79 2066 6f72 6d20 7265 7375  an any form resu
+00002690: 6c74 696e 6720 6672 6f6d 206d 6563 6861  lting from mecha
+000026a0: 6e69 6361 6c0a 2020 2020 2020 7472 616e  nical.      tran
+000026b0: 7366 6f72 6d61 7469 6f6e 206f 7220 7472  sformation or tr
+000026c0: 616e 736c 6174 696f 6e20 6f66 2061 2053  anslation of a S
+000026d0: 6f75 7263 6520 666f 726d 2c20 696e 636c  ource form, incl
+000026e0: 7564 696e 6720 6275 740a 2020 2020 2020  uding but.      
+000026f0: 6e6f 7420 6c69 6d69 7465 6420 746f 2063  not limited to c
+00002700: 6f6d 7069 6c65 6420 6f62 6a65 6374 2063  ompiled object c
+00002710: 6f64 652c 2067 656e 6572 6174 6564 2064  ode, generated d
+00002720: 6f63 756d 656e 7461 7469 6f6e 2c0a 2020  ocumentation,.  
+00002730: 2020 2020 616e 6420 636f 6e76 6572 7369      and conversi
+00002740: 6f6e 7320 746f 206f 7468 6572 206d 6564  ons to other med
+00002750: 6961 2074 7970 6573 2e0a 0a20 2020 2020  ia types...     
+00002760: 2022 576f 726b 2220 7368 616c 6c20 6d65   "Work" shall me
+00002770: 616e 2074 6865 2077 6f72 6b20 6f66 2061  an the work of a
+00002780: 7574 686f 7273 6869 702c 2077 6865 7468  uthorship, wheth
+00002790: 6572 2069 6e20 536f 7572 6365 206f 720a  er in Source or.
+000027a0: 2020 2020 2020 4f62 6a65 6374 2066 6f72        Object for
+000027b0: 6d2c 206d 6164 6520 6176 6169 6c61 626c  m, made availabl
+000027c0: 6520 756e 6465 7220 7468 6520 4c69 6365  e under the Lice
+000027d0: 6e73 652c 2061 7320 696e 6469 6361 7465  nse, as indicate
+000027e0: 6420 6279 2061 0a20 2020 2020 2063 6f70  d by a.      cop
+000027f0: 7972 6967 6874 206e 6f74 6963 6520 7468  yright notice th
+00002800: 6174 2069 7320 696e 636c 7564 6564 2069  at is included i
+00002810: 6e20 6f72 2061 7474 6163 6865 6420 746f  n or attached to
+00002820: 2074 6865 2077 6f72 6b0a 2020 2020 2020   the work.      
+00002830: 2861 6e20 6578 616d 706c 6520 6973 2070  (an example is p
+00002840: 726f 7669 6465 6420 696e 2074 6865 2041  rovided in the A
+00002850: 7070 656e 6469 7820 6265 6c6f 7729 2e0a  ppendix below)..
+00002860: 0a20 2020 2020 2022 4465 7269 7661 7469  .      "Derivati
+00002870: 7665 2057 6f72 6b73 2220 7368 616c 6c20  ve Works" shall 
+00002880: 6d65 616e 2061 6e79 2077 6f72 6b2c 2077  mean any work, w
+00002890: 6865 7468 6572 2069 6e20 536f 7572 6365  hether in Source
+000028a0: 206f 7220 4f62 6a65 6374 0a20 2020 2020   or Object.     
+000028b0: 2066 6f72 6d2c 2074 6861 7420 6973 2062   form, that is b
+000028c0: 6173 6564 206f 6e20 286f 7220 6465 7269  ased on (or deri
+000028d0: 7665 6420 6672 6f6d 2920 7468 6520 576f  ved from) the Wo
+000028e0: 726b 2061 6e64 2066 6f72 2077 6869 6368  rk and for which
+000028f0: 2074 6865 0a20 2020 2020 2065 6469 746f   the.      edito
+00002900: 7269 616c 2072 6576 6973 696f 6e73 2c20  rial revisions, 
+00002910: 616e 6e6f 7461 7469 6f6e 732c 2065 6c61  annotations, ela
+00002920: 626f 7261 7469 6f6e 732c 206f 7220 6f74  borations, or ot
+00002930: 6865 7220 6d6f 6469 6669 6361 7469 6f6e  her modification
+00002940: 730a 2020 2020 2020 7265 7072 6573 656e  s.      represen
+00002950: 742c 2061 7320 6120 7768 6f6c 652c 2061  t, as a whole, a
+00002960: 6e20 6f72 6967 696e 616c 2077 6f72 6b20  n original work 
+00002970: 6f66 2061 7574 686f 7273 6869 702e 2046  of authorship. F
+00002980: 6f72 2074 6865 2070 7572 706f 7365 730a  or the purposes.
+00002990: 2020 2020 2020 6f66 2074 6869 7320 4c69        of this Li
+000029a0: 6365 6e73 652c 2044 6572 6976 6174 6976  cense, Derivativ
+000029b0: 6520 576f 726b 7320 7368 616c 6c20 6e6f  e Works shall no
+000029c0: 7420 696e 636c 7564 6520 776f 726b 7320  t include works 
+000029d0: 7468 6174 2072 656d 6169 6e0a 2020 2020  that remain.    
+000029e0: 2020 7365 7061 7261 626c 6520 6672 6f6d    separable from
+000029f0: 2c20 6f72 206d 6572 656c 7920 6c69 6e6b  , or merely link
+00002a00: 2028 6f72 2062 696e 6420 6279 206e 616d   (or bind by nam
+00002a10: 6529 2074 6f20 7468 6520 696e 7465 7266  e) to the interf
+00002a20: 6163 6573 206f 662c 0a20 2020 2020 2074  aces of,.      t
+00002a30: 6865 2057 6f72 6b20 616e 6420 4465 7269  he Work and Deri
+00002a40: 7661 7469 7665 2057 6f72 6b73 2074 6865  vative Works the
+00002a50: 7265 6f66 2e0a 0a20 2020 2020 2022 436f  reof...      "Co
+00002a60: 6e74 7269 6275 7469 6f6e 2220 7368 616c  ntribution" shal
+00002a70: 6c20 6d65 616e 2061 6e79 2077 6f72 6b20  l mean any work 
+00002a80: 6f66 2061 7574 686f 7273 6869 702c 2069  of authorship, i
+00002a90: 6e63 6c75 6469 6e67 0a20 2020 2020 2074  ncluding.      t
+00002aa0: 6865 206f 7269 6769 6e61 6c20 7665 7273  he original vers
+00002ab0: 696f 6e20 6f66 2074 6865 2057 6f72 6b20  ion of the Work 
+00002ac0: 616e 6420 616e 7920 6d6f 6469 6669 6361  and any modifica
+00002ad0: 7469 6f6e 7320 6f72 2061 6464 6974 696f  tions or additio
+00002ae0: 6e73 0a20 2020 2020 2074 6f20 7468 6174  ns.      to that
+00002af0: 2057 6f72 6b20 6f72 2044 6572 6976 6174   Work or Derivat
+00002b00: 6976 6520 576f 726b 7320 7468 6572 656f  ive Works thereo
+00002b10: 662c 2074 6861 7420 6973 2069 6e74 656e  f, that is inten
+00002b20: 7469 6f6e 616c 6c79 0a20 2020 2020 2073  tionally.      s
+00002b30: 7562 6d69 7474 6564 2074 6f20 4c69 6365  ubmitted to Lice
+00002b40: 6e73 6f72 2066 6f72 2069 6e63 6c75 7369  nsor for inclusi
+00002b50: 6f6e 2069 6e20 7468 6520 576f 726b 2062  on in the Work b
+00002b60: 7920 7468 6520 636f 7079 7269 6768 7420  y the copyright 
+00002b70: 6f77 6e65 720a 2020 2020 2020 6f72 2062  owner.      or b
+00002b80: 7920 616e 2069 6e64 6976 6964 7561 6c20  y an individual 
+00002b90: 6f72 204c 6567 616c 2045 6e74 6974 7920  or Legal Entity 
+00002ba0: 6175 7468 6f72 697a 6564 2074 6f20 7375  authorized to su
+00002bb0: 626d 6974 206f 6e20 6265 6861 6c66 206f  bmit on behalf o
+00002bc0: 660a 2020 2020 2020 7468 6520 636f 7079  f.      the copy
+00002bd0: 7269 6768 7420 6f77 6e65 722e 2046 6f72  right owner. For
+00002be0: 2074 6865 2070 7572 706f 7365 7320 6f66   the purposes of
+00002bf0: 2074 6869 7320 6465 6669 6e69 7469 6f6e   this definition
+00002c00: 2c20 2273 7562 6d69 7474 6564 220a 2020  , "submitted".  
+00002c10: 2020 2020 6d65 616e 7320 616e 7920 666f      means any fo
+00002c20: 726d 206f 6620 656c 6563 7472 6f6e 6963  rm of electronic
+00002c30: 2c20 7665 7262 616c 2c20 6f72 2077 7269  , verbal, or wri
+00002c40: 7474 656e 2063 6f6d 6d75 6e69 6361 7469  tten communicati
+00002c50: 6f6e 2073 656e 740a 2020 2020 2020 746f  on sent.      to
+00002c60: 2074 6865 204c 6963 656e 736f 7220 6f72   the Licensor or
+00002c70: 2069 7473 2072 6570 7265 7365 6e74 6174   its representat
+00002c80: 6976 6573 2c20 696e 636c 7564 696e 6720  ives, including 
+00002c90: 6275 7420 6e6f 7420 6c69 6d69 7465 6420  but not limited 
+00002ca0: 746f 0a20 2020 2020 2063 6f6d 6d75 6e69  to.      communi
+00002cb0: 6361 7469 6f6e 206f 6e20 656c 6563 7472  cation on electr
+00002cc0: 6f6e 6963 206d 6169 6c69 6e67 206c 6973  onic mailing lis
+00002cd0: 7473 2c20 736f 7572 6365 2063 6f64 6520  ts, source code 
+00002ce0: 636f 6e74 726f 6c20 7379 7374 656d 732c  control systems,
+00002cf0: 0a20 2020 2020 2061 6e64 2069 7373 7565  .      and issue
+00002d00: 2074 7261 636b 696e 6720 7379 7374 656d   tracking system
+00002d10: 7320 7468 6174 2061 7265 206d 616e 6167  s that are manag
+00002d20: 6564 2062 792c 206f 7220 6f6e 2062 6568  ed by, or on beh
+00002d30: 616c 6620 6f66 2c20 7468 650a 2020 2020  alf of, the.    
+00002d40: 2020 4c69 6365 6e73 6f72 2066 6f72 2074    Licensor for t
+00002d50: 6865 2070 7572 706f 7365 206f 6620 6469  he purpose of di
+00002d60: 7363 7573 7369 6e67 2061 6e64 2069 6d70  scussing and imp
+00002d70: 726f 7669 6e67 2074 6865 2057 6f72 6b2c  roving the Work,
+00002d80: 2062 7574 0a20 2020 2020 2065 7863 6c75   but.      exclu
+00002d90: 6469 6e67 2063 6f6d 6d75 6e69 6361 7469  ding communicati
+00002da0: 6f6e 2074 6861 7420 6973 2063 6f6e 7370  on that is consp
+00002db0: 6963 756f 7573 6c79 206d 6172 6b65 6420  icuously marked 
+00002dc0: 6f72 206f 7468 6572 7769 7365 0a20 2020  or otherwise.   
+00002dd0: 2020 2064 6573 6967 6e61 7465 6420 696e     designated in
+00002de0: 2077 7269 7469 6e67 2062 7920 7468 6520   writing by the 
+00002df0: 636f 7079 7269 6768 7420 6f77 6e65 7220  copyright owner 
+00002e00: 6173 2022 4e6f 7420 6120 436f 6e74 7269  as "Not a Contri
+00002e10: 6275 7469 6f6e 2e22 0a0a 2020 2020 2020  bution."..      
+00002e20: 2243 6f6e 7472 6962 7574 6f72 2220 7368  "Contributor" sh
+00002e30: 616c 6c20 6d65 616e 204c 6963 656e 736f  all mean Licenso
+00002e40: 7220 616e 6420 616e 7920 696e 6469 7669  r and any indivi
+00002e50: 6475 616c 206f 7220 4c65 6761 6c20 456e  dual or Legal En
+00002e60: 7469 7479 0a20 2020 2020 206f 6e20 6265  tity.      on be
+00002e70: 6861 6c66 206f 6620 7768 6f6d 2061 2043  half of whom a C
+00002e80: 6f6e 7472 6962 7574 696f 6e20 6861 7320  ontribution has 
+00002e90: 6265 656e 2072 6563 6569 7665 6420 6279  been received by
+00002ea0: 204c 6963 656e 736f 7220 616e 640a 2020   Licensor and.  
+00002eb0: 2020 2020 7375 6273 6571 7565 6e74 6c79      subsequently
+00002ec0: 2069 6e63 6f72 706f 7261 7465 6420 7769   incorporated wi
+00002ed0: 7468 696e 2074 6865 2057 6f72 6b2e 0a0a  thin the Work...
+00002ee0: 2020 2032 2e20 4772 616e 7420 6f66 2043     2. Grant of C
+00002ef0: 6f70 7972 6967 6874 204c 6963 656e 7365  opyright License
+00002f00: 2e20 5375 626a 6563 7420 746f 2074 6865  . Subject to the
+00002f10: 2074 6572 6d73 2061 6e64 2063 6f6e 6469   terms and condi
+00002f20: 7469 6f6e 7320 6f66 0a20 2020 2020 2074  tions of.      t
+00002f30: 6869 7320 4c69 6365 6e73 652c 2065 6163  his License, eac
+00002f40: 6820 436f 6e74 7269 6275 746f 7220 6865  h Contributor he
+00002f50: 7265 6279 2067 7261 6e74 7320 746f 2059  reby grants to Y
+00002f60: 6f75 2061 2070 6572 7065 7475 616c 2c0a  ou a perpetual,.
+00002f70: 2020 2020 2020 776f 726c 6477 6964 652c        worldwide,
+00002f80: 206e 6f6e 2d65 7863 6c75 7369 7665 2c20   non-exclusive, 
+00002f90: 6e6f 2d63 6861 7267 652c 2072 6f79 616c  no-charge, royal
+00002fa0: 7479 2d66 7265 652c 2069 7272 6576 6f63  ty-free, irrevoc
+00002fb0: 6162 6c65 0a20 2020 2020 2063 6f70 7972  able.      copyr
+00002fc0: 6967 6874 206c 6963 656e 7365 2074 6f20  ight license to 
+00002fd0: 7265 7072 6f64 7563 652c 2070 7265 7061  reproduce, prepa
+00002fe0: 7265 2044 6572 6976 6174 6976 6520 576f  re Derivative Wo
+00002ff0: 726b 7320 6f66 2c0a 2020 2020 2020 7075  rks of,.      pu
+00003000: 626c 6963 6c79 2064 6973 706c 6179 2c20  blicly display, 
+00003010: 7075 626c 6963 6c79 2070 6572 666f 726d  publicly perform
+00003020: 2c20 7375 626c 6963 656e 7365 2c20 616e  , sublicense, an
+00003030: 6420 6469 7374 7269 6275 7465 2074 6865  d distribute the
+00003040: 0a20 2020 2020 2057 6f72 6b20 616e 6420  .      Work and 
+00003050: 7375 6368 2044 6572 6976 6174 6976 6520  such Derivative 
+00003060: 576f 726b 7320 696e 2053 6f75 7263 6520  Works in Source 
+00003070: 6f72 204f 626a 6563 7420 666f 726d 2e0a  or Object form..
+00003080: 0a20 2020 332e 2047 7261 6e74 206f 6620  .   3. Grant of 
+00003090: 5061 7465 6e74 204c 6963 656e 7365 2e20  Patent License. 
+000030a0: 5375 626a 6563 7420 746f 2074 6865 2074  Subject to the t
+000030b0: 6572 6d73 2061 6e64 2063 6f6e 6469 7469  erms and conditi
+000030c0: 6f6e 7320 6f66 0a20 2020 2020 2074 6869  ons of.      thi
+000030d0: 7320 4c69 6365 6e73 652c 2065 6163 6820  s License, each 
+000030e0: 436f 6e74 7269 6275 746f 7220 6865 7265  Contributor here
+000030f0: 6279 2067 7261 6e74 7320 746f 2059 6f75  by grants to You
+00003100: 2061 2070 6572 7065 7475 616c 2c0a 2020   a perpetual,.  
+00003110: 2020 2020 776f 726c 6477 6964 652c 206e      worldwide, n
+00003120: 6f6e 2d65 7863 6c75 7369 7665 2c20 6e6f  on-exclusive, no
+00003130: 2d63 6861 7267 652c 2072 6f79 616c 7479  -charge, royalty
+00003140: 2d66 7265 652c 2069 7272 6576 6f63 6162  -free, irrevocab
+00003150: 6c65 0a20 2020 2020 2028 6578 6365 7074  le.      (except
+00003160: 2061 7320 7374 6174 6564 2069 6e20 7468   as stated in th
+00003170: 6973 2073 6563 7469 6f6e 2920 7061 7465  is section) pate
+00003180: 6e74 206c 6963 656e 7365 2074 6f20 6d61  nt license to ma
+00003190: 6b65 2c20 6861 7665 206d 6164 652c 0a20  ke, have made,. 
+000031a0: 2020 2020 2075 7365 2c20 6f66 6665 7220       use, offer 
+000031b0: 746f 2073 656c 6c2c 2073 656c 6c2c 2069  to sell, sell, i
+000031c0: 6d70 6f72 742c 2061 6e64 206f 7468 6572  mport, and other
+000031d0: 7769 7365 2074 7261 6e73 6665 7220 7468  wise transfer th
+000031e0: 6520 576f 726b 2c0a 2020 2020 2020 7768  e Work,.      wh
+000031f0: 6572 6520 7375 6368 206c 6963 656e 7365  ere such license
+00003200: 2061 7070 6c69 6573 206f 6e6c 7920 746f   applies only to
+00003210: 2074 686f 7365 2070 6174 656e 7420 636c   those patent cl
+00003220: 6169 6d73 206c 6963 656e 7361 626c 650a  aims licensable.
+00003230: 2020 2020 2020 6279 2073 7563 6820 436f        by such Co
+00003240: 6e74 7269 6275 746f 7220 7468 6174 2061  ntributor that a
+00003250: 7265 206e 6563 6573 7361 7269 6c79 2069  re necessarily i
+00003260: 6e66 7269 6e67 6564 2062 7920 7468 6569  nfringed by thei
+00003270: 720a 2020 2020 2020 436f 6e74 7269 6275  r.      Contribu
+00003280: 7469 6f6e 2873 2920 616c 6f6e 6520 6f72  tion(s) alone or
+00003290: 2062 7920 636f 6d62 696e 6174 696f 6e20   by combination 
+000032a0: 6f66 2074 6865 6972 2043 6f6e 7472 6962  of their Contrib
+000032b0: 7574 696f 6e28 7329 0a20 2020 2020 2077  ution(s).      w
+000032c0: 6974 6820 7468 6520 576f 726b 2074 6f20  ith the Work to 
+000032d0: 7768 6963 6820 7375 6368 2043 6f6e 7472  which such Contr
+000032e0: 6962 7574 696f 6e28 7329 2077 6173 2073  ibution(s) was s
+000032f0: 7562 6d69 7474 6564 2e20 4966 2059 6f75  ubmitted. If You
+00003300: 0a20 2020 2020 2069 6e73 7469 7475 7465  .      institute
+00003310: 2070 6174 656e 7420 6c69 7469 6761 7469   patent litigati
+00003320: 6f6e 2061 6761 696e 7374 2061 6e79 2065  on against any e
+00003330: 6e74 6974 7920 2869 6e63 6c75 6469 6e67  ntity (including
+00003340: 2061 0a20 2020 2020 2063 726f 7373 2d63   a.      cross-c
+00003350: 6c61 696d 206f 7220 636f 756e 7465 7263  laim or counterc
+00003360: 6c61 696d 2069 6e20 6120 6c61 7773 7569  laim in a lawsui
+00003370: 7429 2061 6c6c 6567 696e 6720 7468 6174  t) alleging that
+00003380: 2074 6865 2057 6f72 6b0a 2020 2020 2020   the Work.      
+00003390: 6f72 2061 2043 6f6e 7472 6962 7574 696f  or a Contributio
+000033a0: 6e20 696e 636f 7270 6f72 6174 6564 2077  n incorporated w
+000033b0: 6974 6869 6e20 7468 6520 576f 726b 2063  ithin the Work c
+000033c0: 6f6e 7374 6974 7574 6573 2064 6972 6563  onstitutes direc
+000033d0: 740a 2020 2020 2020 6f72 2063 6f6e 7472  t.      or contr
+000033e0: 6962 7574 6f72 7920 7061 7465 6e74 2069  ibutory patent i
+000033f0: 6e66 7269 6e67 656d 656e 742c 2074 6865  nfringement, the
+00003400: 6e20 616e 7920 7061 7465 6e74 206c 6963  n any patent lic
+00003410: 656e 7365 730a 2020 2020 2020 6772 616e  enses.      gran
+00003420: 7465 6420 746f 2059 6f75 2075 6e64 6572  ted to You under
+00003430: 2074 6869 7320 4c69 6365 6e73 6520 666f   this License fo
+00003440: 7220 7468 6174 2057 6f72 6b20 7368 616c  r that Work shal
+00003450: 6c20 7465 726d 696e 6174 650a 2020 2020  l terminate.    
+00003460: 2020 6173 206f 6620 7468 6520 6461 7465    as of the date
+00003470: 2073 7563 6820 6c69 7469 6761 7469 6f6e   such litigation
+00003480: 2069 7320 6669 6c65 642e 0a0a 2020 2034   is filed...   4
+00003490: 2e20 5265 6469 7374 7269 6275 7469 6f6e  . Redistribution
+000034a0: 2e20 596f 7520 6d61 7920 7265 7072 6f64  . You may reprod
+000034b0: 7563 6520 616e 6420 6469 7374 7269 6275  uce and distribu
+000034c0: 7465 2063 6f70 6965 7320 6f66 2074 6865  te copies of the
+000034d0: 0a20 2020 2020 2057 6f72 6b20 6f72 2044  .      Work or D
+000034e0: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
+000034f0: 7468 6572 656f 6620 696e 2061 6e79 206d  thereof in any m
+00003500: 6564 6975 6d2c 2077 6974 6820 6f72 2077  edium, with or w
+00003510: 6974 686f 7574 0a20 2020 2020 206d 6f64  ithout.      mod
+00003520: 6966 6963 6174 696f 6e73 2c20 616e 6420  ifications, and 
+00003530: 696e 2053 6f75 7263 6520 6f72 204f 626a  in Source or Obj
+00003540: 6563 7420 666f 726d 2c20 7072 6f76 6964  ect form, provid
+00003550: 6564 2074 6861 7420 596f 750a 2020 2020  ed that You.    
+00003560: 2020 6d65 6574 2074 6865 2066 6f6c 6c6f    meet the follo
+00003570: 7769 6e67 2063 6f6e 6469 7469 6f6e 733a  wing conditions:
+00003580: 0a0a 2020 2020 2020 2861 2920 596f 7520  ..      (a) You 
+00003590: 6d75 7374 2067 6976 6520 616e 7920 6f74  must give any ot
+000035a0: 6865 7220 7265 6369 7069 656e 7473 206f  her recipients o
+000035b0: 6620 7468 6520 576f 726b 206f 720a 2020  f the Work or.  
+000035c0: 2020 2020 2020 2020 4465 7269 7661 7469          Derivati
+000035d0: 7665 2057 6f72 6b73 2061 2063 6f70 7920  ve Works a copy 
+000035e0: 6f66 2074 6869 7320 4c69 6365 6e73 653b  of this License;
+000035f0: 2061 6e64 0a0a 2020 2020 2020 2862 2920   and..      (b) 
+00003600: 596f 7520 6d75 7374 2063 6175 7365 2061  You must cause a
+00003610: 6e79 206d 6f64 6966 6965 6420 6669 6c65  ny modified file
+00003620: 7320 746f 2063 6172 7279 2070 726f 6d69  s to carry promi
+00003630: 6e65 6e74 206e 6f74 6963 6573 0a20 2020  nent notices.   
+00003640: 2020 2020 2020 2073 7461 7469 6e67 2074         stating t
+00003650: 6861 7420 596f 7520 6368 616e 6765 6420  hat You changed 
+00003660: 7468 6520 6669 6c65 733b 2061 6e64 0a0a  the files; and..
+00003670: 2020 2020 2020 2863 2920 596f 7520 6d75        (c) You mu
+00003680: 7374 2072 6574 6169 6e2c 2069 6e20 7468  st retain, in th
+00003690: 6520 536f 7572 6365 2066 6f72 6d20 6f66  e Source form of
+000036a0: 2061 6e79 2044 6572 6976 6174 6976 6520   any Derivative 
+000036b0: 576f 726b 730a 2020 2020 2020 2020 2020  Works.          
+000036c0: 7468 6174 2059 6f75 2064 6973 7472 6962  that You distrib
+000036d0: 7574 652c 2061 6c6c 2063 6f70 7972 6967  ute, all copyrig
+000036e0: 6874 2c20 7061 7465 6e74 2c20 7472 6164  ht, patent, trad
+000036f0: 656d 6172 6b2c 2061 6e64 0a20 2020 2020  emark, and.     
+00003700: 2020 2020 2061 7474 7269 6275 7469 6f6e       attribution
+00003710: 206e 6f74 6963 6573 2066 726f 6d20 7468   notices from th
+00003720: 6520 536f 7572 6365 2066 6f72 6d20 6f66  e Source form of
+00003730: 2074 6865 2057 6f72 6b2c 0a20 2020 2020   the Work,.     
+00003740: 2020 2020 2065 7863 6c75 6469 6e67 2074       excluding t
+00003750: 686f 7365 206e 6f74 6963 6573 2074 6861  hose notices tha
+00003760: 7420 646f 206e 6f74 2070 6572 7461 696e  t do not pertain
+00003770: 2074 6f20 616e 7920 7061 7274 206f 660a   to any part of.
+00003780: 2020 2020 2020 2020 2020 7468 6520 4465            the De
+00003790: 7269 7661 7469 7665 2057 6f72 6b73 3b20  rivative Works; 
+000037a0: 616e 640a 0a20 2020 2020 2028 6429 2049  and..      (d) I
+000037b0: 6620 7468 6520 576f 726b 2069 6e63 6c75  f the Work inclu
+000037c0: 6465 7320 6120 224e 4f54 4943 4522 2074  des a "NOTICE" t
+000037d0: 6578 7420 6669 6c65 2061 7320 7061 7274  ext file as part
+000037e0: 206f 6620 6974 730a 2020 2020 2020 2020   of its.        
+000037f0: 2020 6469 7374 7269 6275 7469 6f6e 2c20    distribution, 
+00003800: 7468 656e 2061 6e79 2044 6572 6976 6174  then any Derivat
+00003810: 6976 6520 576f 726b 7320 7468 6174 2059  ive Works that Y
+00003820: 6f75 2064 6973 7472 6962 7574 6520 6d75  ou distribute mu
+00003830: 7374 0a20 2020 2020 2020 2020 2069 6e63  st.          inc
+00003840: 6c75 6465 2061 2072 6561 6461 626c 6520  lude a readable 
+00003850: 636f 7079 206f 6620 7468 6520 6174 7472  copy of the attr
+00003860: 6962 7574 696f 6e20 6e6f 7469 6365 7320  ibution notices 
+00003870: 636f 6e74 6169 6e65 640a 2020 2020 2020  contained.      
+00003880: 2020 2020 7769 7468 696e 2073 7563 6820      within such 
+00003890: 4e4f 5449 4345 2066 696c 652c 2065 7863  NOTICE file, exc
+000038a0: 6c75 6469 6e67 2074 686f 7365 206e 6f74  luding those not
+000038b0: 6963 6573 2074 6861 7420 646f 206e 6f74  ices that do not
+000038c0: 0a20 2020 2020 2020 2020 2070 6572 7461  .          perta
+000038d0: 696e 2074 6f20 616e 7920 7061 7274 206f  in to any part o
+000038e0: 6620 7468 6520 4465 7269 7661 7469 7665  f the Derivative
+000038f0: 2057 6f72 6b73 2c20 696e 2061 7420 6c65   Works, in at le
+00003900: 6173 7420 6f6e 650a 2020 2020 2020 2020  ast one.        
+00003910: 2020 6f66 2074 6865 2066 6f6c 6c6f 7769    of the followi
+00003920: 6e67 2070 6c61 6365 733a 2077 6974 6869  ng places: withi
+00003930: 6e20 6120 4e4f 5449 4345 2074 6578 7420  n a NOTICE text 
+00003940: 6669 6c65 2064 6973 7472 6962 7574 6564  file distributed
+00003950: 0a20 2020 2020 2020 2020 2061 7320 7061  .          as pa
+00003960: 7274 206f 6620 7468 6520 4465 7269 7661  rt of the Deriva
+00003970: 7469 7665 2057 6f72 6b73 3b20 7769 7468  tive Works; with
+00003980: 696e 2074 6865 2053 6f75 7263 6520 666f  in the Source fo
+00003990: 726d 206f 720a 2020 2020 2020 2020 2020  rm or.          
+000039a0: 646f 6375 6d65 6e74 6174 696f 6e2c 2069  documentation, i
+000039b0: 6620 7072 6f76 6964 6564 2061 6c6f 6e67  f provided along
+000039c0: 2077 6974 6820 7468 6520 4465 7269 7661   with the Deriva
+000039d0: 7469 7665 2057 6f72 6b73 3b20 6f72 2c0a  tive Works; or,.
+000039e0: 2020 2020 2020 2020 2020 7769 7468 696e            within
+000039f0: 2061 2064 6973 706c 6179 2067 656e 6572   a display gener
+00003a00: 6174 6564 2062 7920 7468 6520 4465 7269  ated by the Deri
+00003a10: 7661 7469 7665 2057 6f72 6b73 2c20 6966  vative Works, if
+00003a20: 2061 6e64 0a20 2020 2020 2020 2020 2077   and.          w
+00003a30: 6865 7265 7665 7220 7375 6368 2074 6869  herever such thi
+00003a40: 7264 2d70 6172 7479 206e 6f74 6963 6573  rd-party notices
+00003a50: 206e 6f72 6d61 6c6c 7920 6170 7065 6172   normally appear
+00003a60: 2e20 5468 6520 636f 6e74 656e 7473 0a20  . The contents. 
+00003a70: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+00003a80: 4e4f 5449 4345 2066 696c 6520 6172 6520  NOTICE file are 
+00003a90: 666f 7220 696e 666f 726d 6174 696f 6e61  for informationa
+00003aa0: 6c20 7075 7270 6f73 6573 206f 6e6c 7920  l purposes only 
+00003ab0: 616e 640a 2020 2020 2020 2020 2020 646f  and.          do
+00003ac0: 206e 6f74 206d 6f64 6966 7920 7468 6520   not modify the 
+00003ad0: 4c69 6365 6e73 652e 2059 6f75 206d 6179  License. You may
+00003ae0: 2061 6464 2059 6f75 7220 6f77 6e20 6174   add Your own at
+00003af0: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
+00003b00: 2020 2020 6e6f 7469 6365 7320 7769 7468      notices with
+00003b10: 696e 2044 6572 6976 6174 6976 6520 576f  in Derivative Wo
+00003b20: 726b 7320 7468 6174 2059 6f75 2064 6973  rks that You dis
+00003b30: 7472 6962 7574 652c 2061 6c6f 6e67 7369  tribute, alongsi
+00003b40: 6465 0a20 2020 2020 2020 2020 206f 7220  de.          or 
+00003b50: 6173 2061 6e20 6164 6465 6e64 756d 2074  as an addendum t
+00003b60: 6f20 7468 6520 4e4f 5449 4345 2074 6578  o the NOTICE tex
+00003b70: 7420 6672 6f6d 2074 6865 2057 6f72 6b2c  t from the Work,
+00003b80: 2070 726f 7669 6465 640a 2020 2020 2020   provided.      
+00003b90: 2020 2020 7468 6174 2073 7563 6820 6164      that such ad
+00003ba0: 6469 7469 6f6e 616c 2061 7474 7269 6275  ditional attribu
+00003bb0: 7469 6f6e 206e 6f74 6963 6573 2063 616e  tion notices can
+00003bc0: 6e6f 7420 6265 2063 6f6e 7374 7275 6564  not be construed
+00003bd0: 0a20 2020 2020 2020 2020 2061 7320 6d6f  .          as mo
+00003be0: 6469 6679 696e 6720 7468 6520 4c69 6365  difying the Lice
+00003bf0: 6e73 652e 0a0a 2020 2020 2020 596f 7520  nse...      You 
+00003c00: 6d61 7920 6164 6420 596f 7572 206f 776e  may add Your own
+00003c10: 2063 6f70 7972 6967 6874 2073 7461 7465   copyright state
+00003c20: 6d65 6e74 2074 6f20 596f 7572 206d 6f64  ment to Your mod
+00003c30: 6966 6963 6174 696f 6e73 2061 6e64 0a20  ifications and. 
+00003c40: 2020 2020 206d 6179 2070 726f 7669 6465       may provide
+00003c50: 2061 6464 6974 696f 6e61 6c20 6f72 2064   additional or d
+00003c60: 6966 6665 7265 6e74 206c 6963 656e 7365  ifferent license
+00003c70: 2074 6572 6d73 2061 6e64 2063 6f6e 6469   terms and condi
+00003c80: 7469 6f6e 730a 2020 2020 2020 666f 7220  tions.      for 
+00003c90: 7573 652c 2072 6570 726f 6475 6374 696f  use, reproductio
+00003ca0: 6e2c 206f 7220 6469 7374 7269 6275 7469  n, or distributi
+00003cb0: 6f6e 206f 6620 596f 7572 206d 6f64 6966  on of Your modif
+00003cc0: 6963 6174 696f 6e73 2c20 6f72 0a20 2020  ications, or.   
+00003cd0: 2020 2066 6f72 2061 6e79 2073 7563 6820     for any such 
+00003ce0: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
+00003cf0: 2061 7320 6120 7768 6f6c 652c 2070 726f   as a whole, pro
+00003d00: 7669 6465 6420 596f 7572 2075 7365 2c0a  vided Your use,.
+00003d10: 2020 2020 2020 7265 7072 6f64 7563 7469        reproducti
+00003d20: 6f6e 2c20 616e 6420 6469 7374 7269 6275  on, and distribu
+00003d30: 7469 6f6e 206f 6620 7468 6520 576f 726b  tion of the Work
+00003d40: 206f 7468 6572 7769 7365 2063 6f6d 706c   otherwise compl
+00003d50: 6965 7320 7769 7468 0a20 2020 2020 2074  ies with.      t
+00003d60: 6865 2063 6f6e 6469 7469 6f6e 7320 7374  he conditions st
+00003d70: 6174 6564 2069 6e20 7468 6973 204c 6963  ated in this Lic
+00003d80: 656e 7365 2e0a 0a20 2020 352e 2053 7562  ense...   5. Sub
+00003d90: 6d69 7373 696f 6e20 6f66 2043 6f6e 7472  mission of Contr
+00003da0: 6962 7574 696f 6e73 2e20 556e 6c65 7373  ibutions. Unless
+00003db0: 2059 6f75 2065 7870 6c69 6369 746c 7920   You explicitly 
+00003dc0: 7374 6174 6520 6f74 6865 7277 6973 652c  state otherwise,
+00003dd0: 0a20 2020 2020 2061 6e79 2043 6f6e 7472  .      any Contr
+00003de0: 6962 7574 696f 6e20 696e 7465 6e74 696f  ibution intentio
+00003df0: 6e61 6c6c 7920 7375 626d 6974 7465 6420  nally submitted 
+00003e00: 666f 7220 696e 636c 7573 696f 6e20 696e  for inclusion in
+00003e10: 2074 6865 2057 6f72 6b0a 2020 2020 2020   the Work.      
+00003e20: 6279 2059 6f75 2074 6f20 7468 6520 4c69  by You to the Li
+00003e30: 6365 6e73 6f72 2073 6861 6c6c 2062 6520  censor shall be 
+00003e40: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
+00003e50: 616e 6420 636f 6e64 6974 696f 6e73 206f  and conditions o
+00003e60: 660a 2020 2020 2020 7468 6973 204c 6963  f.      this Lic
+00003e70: 656e 7365 2c20 7769 7468 6f75 7420 616e  ense, without an
+00003e80: 7920 6164 6469 7469 6f6e 616c 2074 6572  y additional ter
+00003e90: 6d73 206f 7220 636f 6e64 6974 696f 6e73  ms or conditions
+00003ea0: 2e0a 2020 2020 2020 4e6f 7477 6974 6873  ..      Notwiths
+00003eb0: 7461 6e64 696e 6720 7468 6520 6162 6f76  tanding the abov
+00003ec0: 652c 206e 6f74 6869 6e67 2068 6572 6569  e, nothing herei
+00003ed0: 6e20 7368 616c 6c20 7375 7065 7273 6564  n shall supersed
+00003ee0: 6520 6f72 206d 6f64 6966 790a 2020 2020  e or modify.    
+00003ef0: 2020 7468 6520 7465 726d 7320 6f66 2061    the terms of a
+00003f00: 6e79 2073 6570 6172 6174 6520 6c69 6365  ny separate lice
+00003f10: 6e73 6520 6167 7265 656d 656e 7420 796f  nse agreement yo
+00003f20: 7520 6d61 7920 6861 7665 2065 7865 6375  u may have execu
+00003f30: 7465 640a 2020 2020 2020 7769 7468 204c  ted.      with L
+00003f40: 6963 656e 736f 7220 7265 6761 7264 696e  icensor regardin
+00003f50: 6720 7375 6368 2043 6f6e 7472 6962 7574  g such Contribut
+00003f60: 696f 6e73 2e0a 0a20 2020 362e 2054 7261  ions...   6. Tra
+00003f70: 6465 6d61 726b 732e 2054 6869 7320 4c69  demarks. This Li
+00003f80: 6365 6e73 6520 646f 6573 206e 6f74 2067  cense does not g
+00003f90: 7261 6e74 2070 6572 6d69 7373 696f 6e20  rant permission 
+00003fa0: 746f 2075 7365 2074 6865 2074 7261 6465  to use the trade
+00003fb0: 0a20 2020 2020 206e 616d 6573 2c20 7472  .      names, tr
+00003fc0: 6164 656d 6172 6b73 2c20 7365 7276 6963  ademarks, servic
+00003fd0: 6520 6d61 726b 732c 206f 7220 7072 6f64  e marks, or prod
+00003fe0: 7563 7420 6e61 6d65 7320 6f66 2074 6865  uct names of the
+00003ff0: 204c 6963 656e 736f 722c 0a20 2020 2020   Licensor,.     
+00004000: 2065 7863 6570 7420 6173 2072 6571 7569   except as requi
+00004010: 7265 6420 666f 7220 7265 6173 6f6e 6162  red for reasonab
+00004020: 6c65 2061 6e64 2063 7573 746f 6d61 7279  le and customary
+00004030: 2075 7365 2069 6e20 6465 7363 7269 6269   use in describi
+00004040: 6e67 2074 6865 0a20 2020 2020 206f 7269  ng the.      ori
+00004050: 6769 6e20 6f66 2074 6865 2057 6f72 6b20  gin of the Work 
+00004060: 616e 6420 7265 7072 6f64 7563 696e 6720  and reproducing 
+00004070: 7468 6520 636f 6e74 656e 7420 6f66 2074  the content of t
+00004080: 6865 204e 4f54 4943 4520 6669 6c65 2e0a  he NOTICE file..
+00004090: 0a20 2020 372e 2044 6973 636c 6169 6d65  .   7. Disclaime
+000040a0: 7220 6f66 2057 6172 7261 6e74 792e 2055  r of Warranty. U
+000040b0: 6e6c 6573 7320 7265 7175 6972 6564 2062  nless required b
+000040c0: 7920 6170 706c 6963 6162 6c65 206c 6177  y applicable law
+000040d0: 206f 720a 2020 2020 2020 6167 7265 6564   or.      agreed
+000040e0: 2074 6f20 696e 2077 7269 7469 6e67 2c20   to in writing, 
+000040f0: 4c69 6365 6e73 6f72 2070 726f 7669 6465  Licensor provide
+00004100: 7320 7468 6520 576f 726b 2028 616e 6420  s the Work (and 
+00004110: 6561 6368 0a20 2020 2020 2043 6f6e 7472  each.      Contr
+00004120: 6962 7574 6f72 2070 726f 7669 6465 7320  ibutor provides 
+00004130: 6974 7320 436f 6e74 7269 6275 7469 6f6e  its Contribution
+00004140: 7329 206f 6e20 616e 2022 4153 2049 5322  s) on an "AS IS"
+00004150: 2042 4153 4953 2c0a 2020 2020 2020 5749   BASIS,.      WI
+00004160: 5448 4f55 5420 5741 5252 414e 5449 4553  THOUT WARRANTIES
+00004170: 204f 5220 434f 4e44 4954 494f 4e53 204f   OR CONDITIONS O
+00004180: 4620 414e 5920 4b49 4e44 2c20 6569 7468  F ANY KIND, eith
+00004190: 6572 2065 7870 7265 7373 206f 720a 2020  er express or.  
+000041a0: 2020 2020 696d 706c 6965 642c 2069 6e63      implied, inc
+000041b0: 6c75 6469 6e67 2c20 7769 7468 6f75 7420  luding, without 
+000041c0: 6c69 6d69 7461 7469 6f6e 2c20 616e 7920  limitation, any 
+000041d0: 7761 7272 616e 7469 6573 206f 7220 636f  warranties or co
+000041e0: 6e64 6974 696f 6e73 0a20 2020 2020 206f  nditions.      o
+000041f0: 6620 5449 544c 452c 204e 4f4e 2d49 4e46  f TITLE, NON-INF
+00004200: 5249 4e47 454d 454e 542c 204d 4552 4348  RINGEMENT, MERCH
+00004210: 414e 5441 4249 4c49 5459 2c20 6f72 2046  ANTABILITY, or F
+00004220: 4954 4e45 5353 2046 4f52 2041 0a20 2020  ITNESS FOR A.   
+00004230: 2020 2050 4152 5449 4355 4c41 5220 5055     PARTICULAR PU
+00004240: 5250 4f53 452e 2059 6f75 2061 7265 2073  RPOSE. You are s
+00004250: 6f6c 656c 7920 7265 7370 6f6e 7369 626c  olely responsibl
+00004260: 6520 666f 7220 6465 7465 726d 696e 696e  e for determinin
+00004270: 6720 7468 650a 2020 2020 2020 6170 7072  g the.      appr
+00004280: 6f70 7269 6174 656e 6573 7320 6f66 2075  opriateness of u
+00004290: 7369 6e67 206f 7220 7265 6469 7374 7269  sing or redistri
+000042a0: 6275 7469 6e67 2074 6865 2057 6f72 6b20  buting the Work 
+000042b0: 616e 6420 6173 7375 6d65 2061 6e79 0a20  and assume any. 
+000042c0: 2020 2020 2072 6973 6b73 2061 7373 6f63       risks assoc
+000042d0: 6961 7465 6420 7769 7468 2059 6f75 7220  iated with Your 
+000042e0: 6578 6572 6369 7365 206f 6620 7065 726d  exercise of perm
+000042f0: 6973 7369 6f6e 7320 756e 6465 7220 7468  issions under th
+00004300: 6973 204c 6963 656e 7365 2e0a 0a20 2020  is License...   
+00004310: 382e 204c 696d 6974 6174 696f 6e20 6f66  8. Limitation of
+00004320: 204c 6961 6269 6c69 7479 2e20 496e 206e   Liability. In n
+00004330: 6f20 6576 656e 7420 616e 6420 756e 6465  o event and unde
+00004340: 7220 6e6f 206c 6567 616c 2074 6865 6f72  r no legal theor
+00004350: 792c 0a20 2020 2020 2077 6865 7468 6572  y,.      whether
+00004360: 2069 6e20 746f 7274 2028 696e 636c 7564   in tort (includ
+00004370: 696e 6720 6e65 676c 6967 656e 6365 292c  ing negligence),
+00004380: 2063 6f6e 7472 6163 742c 206f 7220 6f74   contract, or ot
+00004390: 6865 7277 6973 652c 0a20 2020 2020 2075  herwise,.      u
+000043a0: 6e6c 6573 7320 7265 7175 6972 6564 2062  nless required b
+000043b0: 7920 6170 706c 6963 6162 6c65 206c 6177  y applicable law
+000043c0: 2028 7375 6368 2061 7320 6465 6c69 6265   (such as delibe
+000043d0: 7261 7465 2061 6e64 2067 726f 7373 6c79  rate and grossly
+000043e0: 0a20 2020 2020 206e 6567 6c69 6765 6e74  .      negligent
+000043f0: 2061 6374 7329 206f 7220 6167 7265 6564   acts) or agreed
+00004400: 2074 6f20 696e 2077 7269 7469 6e67 2c20   to in writing, 
+00004410: 7368 616c 6c20 616e 7920 436f 6e74 7269  shall any Contri
+00004420: 6275 746f 7220 6265 0a20 2020 2020 206c  butor be.      l
+00004430: 6961 626c 6520 746f 2059 6f75 2066 6f72  iable to You for
+00004440: 2064 616d 6167 6573 2c20 696e 636c 7564   damages, includ
+00004450: 696e 6720 616e 7920 6469 7265 6374 2c20  ing any direct, 
+00004460: 696e 6469 7265 6374 2c20 7370 6563 6961  indirect, specia
+00004470: 6c2c 0a20 2020 2020 2069 6e63 6964 656e  l,.      inciden
+00004480: 7461 6c2c 206f 7220 636f 6e73 6571 7565  tal, or conseque
+00004490: 6e74 6961 6c20 6461 6d61 6765 7320 6f66  ntial damages of
+000044a0: 2061 6e79 2063 6861 7261 6374 6572 2061   any character a
+000044b0: 7269 7369 6e67 2061 7320 610a 2020 2020  rising as a.    
+000044c0: 2020 7265 7375 6c74 206f 6620 7468 6973    result of this
+000044d0: 204c 6963 656e 7365 206f 7220 6f75 7420   License or out 
+000044e0: 6f66 2074 6865 2075 7365 206f 7220 696e  of the use or in
+000044f0: 6162 696c 6974 7920 746f 2075 7365 2074  ability to use t
+00004500: 6865 0a20 2020 2020 2057 6f72 6b20 2869  he.      Work (i
+00004510: 6e63 6c75 6469 6e67 2062 7574 206e 6f74  ncluding but not
+00004520: 206c 696d 6974 6564 2074 6f20 6461 6d61   limited to dama
+00004530: 6765 7320 666f 7220 6c6f 7373 206f 6620  ges for loss of 
+00004540: 676f 6f64 7769 6c6c 2c0a 2020 2020 2020  goodwill,.      
+00004550: 776f 726b 2073 746f 7070 6167 652c 2063  work stoppage, c
+00004560: 6f6d 7075 7465 7220 6661 696c 7572 6520  omputer failure 
+00004570: 6f72 206d 616c 6675 6e63 7469 6f6e 2c20  or malfunction, 
+00004580: 6f72 2061 6e79 2061 6e64 2061 6c6c 0a20  or any and all. 
+00004590: 2020 2020 206f 7468 6572 2063 6f6d 6d65       other comme
+000045a0: 7263 6961 6c20 6461 6d61 6765 7320 6f72  rcial damages or
+000045b0: 206c 6f73 7365 7329 2c20 6576 656e 2069   losses), even i
+000045c0: 6620 7375 6368 2043 6f6e 7472 6962 7574  f such Contribut
+000045d0: 6f72 0a20 2020 2020 2068 6173 2062 6565  or.      has bee
+000045e0: 6e20 6164 7669 7365 6420 6f66 2074 6865  n advised of the
+000045f0: 2070 6f73 7369 6269 6c69 7479 206f 6620   possibility of 
+00004600: 7375 6368 2064 616d 6167 6573 2e0a 0a20  such damages... 
+00004610: 2020 392e 2041 6363 6570 7469 6e67 2057    9. Accepting W
+00004620: 6172 7261 6e74 7920 6f72 2041 6464 6974  arranty or Addit
+00004630: 696f 6e61 6c20 4c69 6162 696c 6974 792e  ional Liability.
+00004640: 2057 6869 6c65 2072 6564 6973 7472 6962   While redistrib
+00004650: 7574 696e 670a 2020 2020 2020 7468 6520  uting.      the 
+00004660: 576f 726b 206f 7220 4465 7269 7661 7469  Work or Derivati
+00004670: 7665 2057 6f72 6b73 2074 6865 7265 6f66  ve Works thereof
+00004680: 2c20 596f 7520 6d61 7920 6368 6f6f 7365  , You may choose
+00004690: 2074 6f20 6f66 6665 722c 0a20 2020 2020   to offer,.     
+000046a0: 2061 6e64 2063 6861 7267 6520 6120 6665   and charge a fe
+000046b0: 6520 666f 722c 2061 6363 6570 7461 6e63  e for, acceptanc
+000046c0: 6520 6f66 2073 7570 706f 7274 2c20 7761  e of support, wa
+000046d0: 7272 616e 7479 2c20 696e 6465 6d6e 6974  rranty, indemnit
+000046e0: 792c 0a20 2020 2020 206f 7220 6f74 6865  y,.      or othe
+000046f0: 7220 6c69 6162 696c 6974 7920 6f62 6c69  r liability obli
+00004700: 6761 7469 6f6e 7320 616e 642f 6f72 2072  gations and/or r
+00004710: 6967 6874 7320 636f 6e73 6973 7465 6e74  ights consistent
+00004720: 2077 6974 6820 7468 6973 0a20 2020 2020   with this.     
+00004730: 204c 6963 656e 7365 2e20 486f 7765 7665   License. Howeve
+00004740: 722c 2069 6e20 6163 6365 7074 696e 6720  r, in accepting 
+00004750: 7375 6368 206f 626c 6967 6174 696f 6e73  such obligations
+00004760: 2c20 596f 7520 6d61 7920 6163 7420 6f6e  , You may act on
+00004770: 6c79 0a20 2020 2020 206f 6e20 596f 7572  ly.      on Your
+00004780: 206f 776e 2062 6568 616c 6620 616e 6420   own behalf and 
+00004790: 6f6e 2059 6f75 7220 736f 6c65 2072 6573  on Your sole res
+000047a0: 706f 6e73 6962 696c 6974 792c 206e 6f74  ponsibility, not
+000047b0: 206f 6e20 6265 6861 6c66 0a20 2020 2020   on behalf.     
+000047c0: 206f 6620 616e 7920 6f74 6865 7220 436f   of any other Co
+000047d0: 6e74 7269 6275 746f 722c 2061 6e64 206f  ntributor, and o
+000047e0: 6e6c 7920 6966 2059 6f75 2061 6772 6565  nly if You agree
+000047f0: 2074 6f20 696e 6465 6d6e 6966 792c 0a20   to indemnify,. 
+00004800: 2020 2020 2064 6566 656e 642c 2061 6e64       defend, and
+00004810: 2068 6f6c 6420 6561 6368 2043 6f6e 7472   hold each Contr
+00004820: 6962 7574 6f72 2068 6172 6d6c 6573 7320  ibutor harmless 
+00004830: 666f 7220 616e 7920 6c69 6162 696c 6974  for any liabilit
+00004840: 790a 2020 2020 2020 696e 6375 7272 6564  y.      incurred
+00004850: 2062 792c 206f 7220 636c 6169 6d73 2061   by, or claims a
+00004860: 7373 6572 7465 6420 6167 6169 6e73 742c  sserted against,
+00004870: 2073 7563 6820 436f 6e74 7269 6275 746f   such Contributo
+00004880: 7220 6279 2072 6561 736f 6e0a 2020 2020  r by reason.    
+00004890: 2020 6f66 2079 6f75 7220 6163 6365 7074    of your accept
+000048a0: 696e 6720 616e 7920 7375 6368 2077 6172  ing any such war
+000048b0: 7261 6e74 7920 6f72 2061 6464 6974 696f  ranty or additio
+000048c0: 6e61 6c20 6c69 6162 696c 6974 792e 0a0a  nal liability...
+000048d0: 2020 2045 4e44 204f 4620 5445 524d 5320     END OF TERMS 
+000048e0: 414e 4420 434f 4e44 4954 494f 4e53 0a0a  AND CONDITIONS..
+000048f0: 2020 2043 6f70 7972 6967 6874 2032 3032     Copyright 202
+00004900: 302d 3230 3232 204a 696e 6120 4149 204c  0-2022 Jina AI L
+00004910: 696d 6974 6564 0a0a 2020 204c 6963 656e  imited..   Licen
+00004920: 7365 6420 756e 6465 7220 7468 6520 4170  sed under the Ap
+00004930: 6163 6865 204c 6963 656e 7365 2c20 5665  ache License, Ve
+00004940: 7273 696f 6e20 322e 3020 2874 6865 2022  rsion 2.0 (the "
+00004950: 4c69 6365 6e73 6522 293b 0a20 2020 796f  License");.   yo
+00004960: 7520 6d61 7920 6e6f 7420 7573 6520 7468  u may not use th
+00004970: 6973 2066 696c 6520 6578 6365 7074 2069  is file except i
+00004980: 6e20 636f 6d70 6c69 616e 6365 2077 6974  n compliance wit
+00004990: 6820 7468 6520 4c69 6365 6e73 652e 0a20  h the License.. 
+000049a0: 2020 596f 7520 6d61 7920 6f62 7461 696e    You may obtain
+000049b0: 2061 2063 6f70 7920 6f66 2074 6865 204c   a copy of the L
+000049c0: 6963 656e 7365 2061 740a 0a20 2020 2020  icense at..     
+000049d0: 2020 6874 7470 3a2f 2f77 7777 2e61 7061    http://www.apa
+000049e0: 6368 652e 6f72 672f 6c69 6365 6e73 6573  che.org/licenses
+000049f0: 2f4c 4943 454e 5345 2d32 2e30 0a0a 2020  /LICENSE-2.0..  
+00004a00: 2055 6e6c 6573 7320 7265 7175 6972 6564   Unless required
+00004a10: 2062 7920 6170 706c 6963 6162 6c65 206c   by applicable l
+00004a20: 6177 206f 7220 6167 7265 6564 2074 6f20  aw or agreed to 
+00004a30: 696e 2077 7269 7469 6e67 2c20 736f 6674  in writing, soft
+00004a40: 7761 7265 0a20 2020 6469 7374 7269 6275  ware.   distribu
+00004a50: 7465 6420 756e 6465 7220 7468 6520 4c69  ted under the Li
+00004a60: 6365 6e73 6520 6973 2064 6973 7472 6962  cense is distrib
+00004a70: 7574 6564 206f 6e20 616e 2022 4153 2049  uted on an "AS I
+00004a80: 5322 2042 4153 4953 2c0a 2020 2057 4954  S" BASIS,.   WIT
+00004a90: 484f 5554 2057 4152 5241 4e54 4945 5320  HOUT WARRANTIES 
+00004aa0: 4f52 2043 4f4e 4449 5449 4f4e 5320 4f46  OR CONDITIONS OF
+00004ab0: 2041 4e59 204b 494e 442c 2065 6974 6865   ANY KIND, eithe
+00004ac0: 7220 6578 7072 6573 7320 6f72 2069 6d70  r express or imp
+00004ad0: 6c69 6564 2e0a 2020 2053 6565 2074 6865  lied..   See the
+00004ae0: 204c 6963 656e 7365 2066 6f72 2074 6865   License for the
+00004af0: 2073 7065 6369 6669 6320 6c61 6e67 7561   specific langua
+00004b00: 6765 2067 6f76 6572 6e69 6e67 2070 6572  ge governing per
+00004b10: 6d69 7373 696f 6e73 2061 6e64 0a20 2020  missions and.   
+00004b20: 6c69 6d69 7461 7469 6f6e 7320 756e 6465  limitations unde
+00004b30: 7220 7468 6520 4c69 6365 6e73 652e 0a0a  r the License...
```

