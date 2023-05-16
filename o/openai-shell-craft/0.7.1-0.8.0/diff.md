# Comparing `tmp/openai_shell_craft-0.7.1.tar.gz` & `tmp/openai_shell_craft-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_shell_craft-0.7.1.tar", last modified: Sat May 13 16:56:41 2023, max compression
+gzip compressed data, was "openai_shell_craft-0.8.0.tar", last modified: Tue May 16 01:40:00 2023, max compression
```

## Comparing `openai_shell_craft-0.7.1.tar` & `openai_shell_craft-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.806938 openai_shell_craft-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-13 16:56:41.802938 openai_shell_craft-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.798938 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-13 16:56:41.000000 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-13 16:56:41.000000 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 16:56:41.000000 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-13 16:56:41.000000 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-13 16:56:41.000000 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 16:56:41.000000 openai_shell_craft-0.7.1/openai_shell_craft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 16:56:41.806938 openai_shell_craft-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.798938 openai_shell_craft-0.7.1/shell_craft/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.802938 openai_shell_craft-0.7.1/shell_craft/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/cli/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.802938 openai_shell_craft-0.7.1/shell_craft/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/factories/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.802938 openai_shell_craft-0.7.1/shell_craft/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/prompts/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/prompts/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/prompts/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3388 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/shell_craft/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 16:56:41.802938 openai_shell_craft-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-13 16:56:25.000000 openai_shell_craft-0.7.1/tests/test_factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.424236 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 01:40:00.000000 openai_shell_craft-0.8.0/openai_shell_craft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.424236 openai_shell_craft-0.8.0/shell_craft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/shell_craft/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/cli/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/shell_craft/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/factories/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/shell_craft/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/prompts/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3388 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/shell_craft/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:40:00.428236 openai_shell_craft-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-16 01:39:51.000000 openai_shell_craft-0.8.0/tests/test_factories.py
```

### Comparing `openai_shell_craft-0.7.1/LICENSE` & `openai_shell_craft-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/openai_shell_craft.egg-info/SOURCES.txt` & `openai_shell_craft-0.8.0/openai_shell_craft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 openai_shell_craft.egg-info/entry_points.txt
 openai_shell_craft.egg-info/requires.txt
 openai_shell_craft.egg-info/top_level.txt
 shell_craft/__init__.py
 shell_craft/__main__.py
 shell_craft/service.py
 shell_craft/cli/__init__.py
+shell_craft/cli/github.py
 shell_craft/cli/help.py
 shell_craft/cli/key.py
 shell_craft/cli/language.py
 shell_craft/cli/main.py
 shell_craft/cli/models.py
 shell_craft/cli/parser.py
 shell_craft/cli/prompt.py
```

### Comparing `openai_shell_craft-0.7.1/pyproject.toml` & `openai_shell_craft-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai_shell_craft"
-version = "0.7.1"
+version = "0.8.0"
 authors = [
   { name="Johnathan Irvin", email="irvinjohnathan@gmail.com" },
 ]
 description = "Generating shell commands and code using natural language models (OpenAI ChatGPT)."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `openai_shell_craft-0.7.1/shell_craft/__init__.py` & `openai_shell_craft-0.8.0/shell_craft/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/__main__.py` & `openai_shell_craft-0.8.0/shell_craft/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/__init__.py` & `openai_shell_craft-0.8.0/shell_craft/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/help.py` & `openai_shell_craft-0.8.0/shell_craft/cli/help.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     Args:
         parser (ArgumentParser): The parser to add the argument to.
     """    
     parser.add_argument(
         "-h --help",
         action="help",
         help="Show this help message and exit."
-    )
+    )
```

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/key.py` & `openai_shell_craft-0.8.0/shell_craft/cli/key.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/language.py` & `openai_shell_craft-0.8.0/shell_craft/cli/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     Adds 'request' argument to the parser. This argument is used to
     specify the input to prompt the API with. This argument is required,
     however, it can be piped in from another command or from a file.
 
     Args:
         parser (ArgumentParser): The parser to add the argument to.
-    """    
+    """
     group = parser.add_mutually_exclusive_group(required=False)
     group.add_argument(
         '--refactor',
         action='store_true',
         help='Refactor the code.'
     )
     group.add_argument(
```

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/main.py` & `openai_shell_craft-0.8.0/shell_craft/factories/prompt.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,55 +14,38 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from argparse import ArgumentParser
+from shell_craft.prompts import Prompt
 
-from shell_craft import Service
-from shell_craft.factories import PromptFactory
 
-from .parser import get_arguments, initialize_parser
+class PromptFactory:
+    @staticmethod
+    def get_prompt(prompt: str) -> Prompt:
+        """
+        Generates a new prompt object based on the prompt type.
 
+        Args:
+            prompt (str): A string representing the prompt type.
 
-def main():
-    """
-    Main function that processes the command-line arguments and queries the
-    OpenAI API using shell_craft.
-    """
-    args = get_arguments(
-        initialize_parser(
-            ArgumentParser(
-                prog="shell-craft",
-                description="Generating shell commands and code using natural language models (OpenAI ChatGPT).",
-                add_help=False
-            )
-        )
-    )
-    prompt = PromptFactory.get_prompt(args.prompt)
-
-    if getattr(args, "refactor", False):
-        prompt = prompt.refactoring
-    elif getattr(args, "document", False):
-        prompt = prompt.documentation
-    elif getattr(args, "test", False):
-        prompt = prompt.testing
-
-    result = (
-        Service(
-            api_key=args.api_key,
-            prompt=prompt,
-            model=args.model
-        ).query(
-            message=' '.join(args.request),
-            count=args.count,
-            temperature=args.temperature
-        )
-    )
-
-    if isinstance(result, list):
-        for _, r in enumerate(result):
-            print(r)
-    else:
-        print(result)
+        Raises:
+            ValueError: If the prompt type is not supported.
+
+        Returns:
+            Prompt: A new prompt object.
+        """        
+        import shell_craft.prompts as prompts
+
+        available_prompts = [
+            prompt.removesuffix('_PROMPT').casefold()
+            for prompt in dir(prompts)
+            if prompt.endswith("_PROMPT")
+        ]
+
+        if prompt.casefold() in available_prompts:
+            return getattr(prompts, f"{prompt.upper()}_PROMPT")
+
+
+        raise ValueError(f"Unknown prompt type: {prompt}")
```

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/models.py` & `openai_shell_craft-0.8.0/shell_craft/cli/models.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/parser.py` & `openai_shell_craft-0.8.0/shell_craft/cli/parser.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/prompt.py` & `openai_shell_craft-0.8.0/shell_craft/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/request.py` & `openai_shell_craft-0.8.0/shell_craft/cli/request.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/cli/results.py` & `openai_shell_craft-0.8.0/shell_craft/cli/results.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/factories/__init__.py` & `openai_shell_craft-0.8.0/shell_craft/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/factories/prompt.py` & `openai_shell_craft-0.8.0/tests/test_factories.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,38 +14,28 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-from shell_craft.prompts import Prompt
+import pytest
 
+import shell_craft.prompts as prompts
+from shell_craft.factories import PromptFactory
 
-class PromptFactory:
-    @staticmethod
-    def get_prompt(prompt: str) -> Prompt:
-        """
-        Generates a new prompt object based on the prompt type.
-
-        Args:
-            prompt (str): A string representing the prompt type.
-
-        Raises:
-            ValueError: If the prompt type is not supported.
-
-        Returns:
-            Prompt: A new prompt object.
-        """        
-        import shell_craft.prompts as prompts
-
-        available_prompts = [
-            prompt.removesuffix('_PROMPT').casefold()
-            for prompt in dir(prompts)
-            if prompt.endswith("_PROMPT")
-        ]
-
-        if prompt.casefold() in available_prompts:
-            return getattr(prompts, f"{prompt.upper()}_PROMPT")
-
-
-        raise ValueError(f"Unknown prompt type: {prompt}")
+PROMPTS = [
+    prompt
+    for prompt in dir(prompts)
+    if prompt.endswith("_PROMPT")
+    and not prompt.startswith("_")
+]
+
+@pytest.mark.parametrize("prompt", PROMPTS)
+def test_prompt_factory(prompt: str):
+    """
+    Test that the prompt factory returns the correct prompt.
+
+    Args:
+        prompt (str): The prompt to test.
+    """    
+    assert PromptFactory.get_prompt(prompt.removesuffix("_PROMPT")) == getattr(prompts, prompt)
```

### Comparing `openai_shell_craft-0.7.1/shell_craft/prompts/__init__.py` & `openai_shell_craft-0.8.0/shell_craft/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/prompts/languages.py` & `openai_shell_craft-0.8.0/shell_craft/prompts/languages.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/prompts/prompt.py` & `openai_shell_craft-0.8.0/shell_craft/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/prompts/templates.py` & `openai_shell_craft-0.8.0/shell_craft/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/shell_craft/service.py` & `openai_shell_craft-0.8.0/shell_craft/service.py`

 * *Files identical despite different names*

### Comparing `openai_shell_craft-0.7.1/tests/test_cli.py` & `openai_shell_craft-0.8.0/tests/test_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,24 +15,72 @@
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 # LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 # WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from argparse import ArgumentParser
+from typing import Union
 
-from shell_craft.cli.models import add_arguments as add_model_arguments
 from pytest import mark
 
+from shell_craft.cli.github import GitHubArguments
+from shell_craft.cli.github import add_arguments as add_github_arguments
+from shell_craft.cli.models import add_arguments as add_model_arguments
+
+
 @mark.parametrize('model', [
     'gpt-4',
     'gpt-4-0314',
     'gpt-4-32k',
     'gpt-4-32k-0314',
     'gpt-3.5-turbo',
     'gpt-3.5-turbo-0301',
 ])
 def test_ai_model_arguments(model: str):
     parser = ArgumentParser()
     add_model_arguments(parser)
     args = parser.parse_args(['--model', model])
     assert args.model == model
+
+def test_github_arguments():
+    parser = ArgumentParser()
+    add_github_arguments(parser)
+    args = parser.parse_args(['--github', 'https://github.com/JohnnyIrvin/shell-craft/'])
+    assert args.github == 'https://github.com/JohnnyIrvin/shell-craft/'
+
+@mark.parametrize('field, value', [
+    ('title', 'test'),
+    ('labels', ['one', 'two', 'three']),
+    ('body', 'about me\n\nbody'),
+])
+def test_github_arguments_from_prompt(field: str, value: Union[list[str], str]):
+    args = GitHubArguments.from_prompt("""
+---
+name: test
+about: about me
+labels: one,two,three
+---
+body
+    """)
+    assert getattr(args, field) == value
+
+def test_github_arguments_as_url():
+    from urllib.parse import urlencode
+
+    args = GitHubArguments.from_prompt("""
+---
+name: test
+about: about me
+labels: one,two,three
+---
+body
+    """)
+
+    assert args.as_url('https://github.com/JohnnyIrvin/shell-craft/') == (
+        'https://github.com/JohnnyIrvin/shell-craft/issues/new?'
+        + urlencode({
+            'title': 'test',
+            'labels': 'one,two,three',
+            'body': 'about me\n\nbody'
+        })
+    )
```

