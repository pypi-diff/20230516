# Comparing `tmp/gptw-0.1.2.tar.gz` & `tmp/gptw-0.2.0.tar.gz`

## Comparing `gptw-0.1.2.tar` & `gptw-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.1.2/gptw/__init__.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 gptw-0.1.2/gptw/config.json
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 gptw-0.1.2/gptw/gptw.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 gptw-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.1.2/LICENSE
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 gptw-0.1.2/README.md
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 gptw-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 gptw-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gptw-0.2.0/gptw/__init__.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 gptw-0.2.0/gptw/gptw.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 gptw-0.2.0/gptw/prompts.json
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 gptw-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gptw-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 gptw-0.2.0/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 gptw-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 gptw-0.2.0/PKG-INFO
```

### Comparing `gptw-0.1.2/gptw/config.json` & `gptw-0.2.0/gptw/prompts.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'cmds'": "{'e': {'prompt': 'Please rephrase the following text into natural-sounding English, "*

 * *           'adhering to native speaker conventions. Limit your response to the translation '*

 * *           "only.'}, 'p': {'prompt': 'Please review the sentence below for grammar, tense, word "*

 * *           'choice, and phrasing issues. Edit the sentence to make it sound natural and align with '*

 * *           "native speaker conventions. Provide a brief explanation for any changes made.'}, 'r': "*

 * *           '{\'prompt\ […]*

```diff
@@ -19,22 +19,22 @@
             "_comment": "Dictionary",
             "example": "ww dic dictionary",
             "prompt": "Please provide the definitions of the following English words, including both English and Chinese explanations, an example sentence in English, and the correct pronunciation. Please also correct any spelling errors in the words. Please refrain from providing any additional output beyond the definitions."
         },
         "e": {
             "_comment": "Translate into English",
             "example": "ww e \u4f60\u597d",
-            "prompt": "Please translate the following text into natural-sounding English, while adhering to native speaker conventions. Do not provide any additional output beyond the translated text."
+            "prompt": "Please rephrase the following text into natural-sounding English, adhering to native speaker conventions. Limit your response to the translation only."
         },
         "p": {
             "_comment": "Polish sentence",
             "example": "ww p hwo are you",
-            "prompt": "Please review the following sentence for any grammatical errors, incorrect tenses, inappropriate word choices or phrasing, and make revisions to ensure it sounds natural and adheres to native speaker conventions. Please provide a brief explanation for any changes made."
+            "prompt": "Please review the sentence below for grammar, tense, word choice, and phrasing issues. Edit the sentence to make it sound natural and align with native speaker conventions. Provide a brief explanation for any changes made."
         },
         "r": {
             "_comment": "Code Review",
             "example": "ww r -f gptw/gptw.py",
-            "prompt": "Please review the code below and provide feedback on any issues or improvements that can be made. Specifically, please check for syntax errors, unclear commit messages, and any potential security risks. Additionally, please suggest ways to improve the code's efficiency, readability, maintainability, and error handling. If you encounter any issues or have any suggestions, please provide detailed descriptions and feasible solutions. If no issues are found, please output 'No issues found'."
+            "prompt": "Please review the provided code snippet for any issues or areas of improvement. Focus on identifying syntax errors, vague commit messages, and potential security risks. Additionally, suggest ways to enhance the code's efficiency, readability, maintainability, and error handling. Provide detailed descriptions and feasible solutions for any identified issues or suggestions. If no issues are found, please respond with 'No issues found'."
         }
     },
     "version": "v1.0.0"
 }
```

### Comparing `gptw-0.1.2/.gitignore` & `gptw-0.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -126,7 +126,8 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # IDE
 .idea/
+.vscode/
```

### Comparing `gptw-0.1.2/LICENSE` & `gptw-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptw-0.1.2/README.md` & `gptw-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,66 @@
-# GPT simplify your daily Workflow (gptW)
+# GPT Simplify Your Daily Workflow (gptW)
 
-It is no longer necessary to manually input prompts and interact with ChatGPT
+No longer is it necessary to manually input prompts and interact with ChatGPT.
 
 With the GPTW tool, prompt operations are fully automated! Simplify your daily workflow.
 
 ## Example
 
 ### Translate
 
-You can simply use the "ww" command without having to first instruct ChatGPT that the following task is a translation
+You can simply use the "ww" command without having to first instruct ChatGPT that the following task is a translation.
 
-Translate to English
+Translate to English:
 
 ```shell
 $ ww e "今天天气怎么样"
-
 How's the weather today?
 ```
 
-Translate to Chinese
+Translate to Chinese:
 
 ```shell
 $ ww c "who are you? "
-
 你是谁？(Nǐ shì shéi?)
 ```
 
-### Polish the document
+### Polish the Document
 
-Polish a document, supporting files as input.
+Polish a document with files as input.
 
 ```shell
 ww d -f README.md
 ```
 
 ### Code Review
 
 ```shell
 $ ww r -f gptw/gptw.py
-
 As an AI language model, I cannot run the code provided, but I can provide some feedback based on the code structure and syntax.
 
-1. The code seems to be well-organized and follows PEP 8 guidelines for Python code.
+1. The code appears to be well-organized and follows the PEP 8 guidelines for Python code.
 
 2. The argparse module is used to parse command-line arguments, which is a good practice for command-line applications.
 
 ...
 
 Overall, the code seems to be well-written and organized, but could benefit from some additional security measures and error handling.
 ```
 
 ### Ask
 
-Ask ChatGPT directly
+Ask ChatGPT directly:
 
 ```shell
 $ ww a "who are you? "
-
 I am an AI language model created by OpenAI.
 ```
 
-### Add your custom prompt
+### Add Your Custom Prompt
 
 Prepare your prompt and modify the gptw/config.json file following the existing format. Then, submit a PR or directly raise an issue to explain the command you want to add.
 
 gtpw/config.json:
 
 ```json
 {
@@ -82,32 +78,50 @@
 }
 ```
 
 Currently, the following workflows are supported. You can run "ww -l" to obtain the available workflows.
 
 ```shell
 $ ww --list
-
 cmd | meaning                        | example
 e   | Translate into English         | ww e 你好
 c   | Translate into Chinese         | ww c how r u
 p   | Polish sentence                | ww p hwo are you
 a   | Just ask ChatGPT directly      | ww a who are you
 d   | Polish document                | ww d -f README.md
 r   | Code Review                    | ww r -f gptw/gptw.py
 dic | Dictionary                     | ww dic dictionary
 ```
 
 ## Installation
 
 ```shell
 pip install --upgrade gptw
-ww --key sk-..... # set your OpenAI API key
 ```
 
+### OpenAI Config
+
+```shell
+ww --config provider=openai
+ww --config openai-model=gpt-3.5-turbo
+ww --config openai-token={YOUR_TOKEN}
+```
+
+### POE Config
+
+```shell
+ww --config provider=poe
+ww --config poe-bot-name=chinchilla
+ww --config poe-token={YOUR_TOKEN}
+```
+
+Bot names:
+
+{'capybara': 'Sage', 'beaver': 'GPT-4', 'a2_2': 'Claude+', 'a2': 'Claude', 'chinchilla': 'ChatGPT', 'nutria': 'Dragonfly'}
+
 ## Uninstall
 
 ```shell
 pip uninstall gptw
 ```
 
 ## Development
```

### Comparing `gptw-0.1.2/pyproject.toml` & `gptw-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 readme.file = "README.md"
 readme.content-type = "text/markdown"
 keywords = ["ChatGPT", "Command Line", "English Translation","English Polishing"]
 license = "Apache-2.0"
 requires-python = ">=3.7.1"
 dependencies = [
   "argparse>=1.4.0",
-  "openai==0.27.0"
+  "openai>=0.27.0",
+  "poe-api>=0.3.1"
 ]
 optional-dependencies.testing = [
   "coverage==5.5",
   "pytest==7.1.3",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `gptw-0.1.2/PKG-INFO` & `gptw-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptw
-Version: 0.1.2
+Version: 0.2.0
 Summary: The ChatGPT command-line wrapper simplifies the execution of predetermined tasks through ChatGPT.
 Author: Xin Yang
 Author-email: xinydev@gmail.com
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: ChatGPT,Command Line,English Polishing,English Translation
 Classifier: Development Status :: 3 - Alpha
@@ -16,83 +16,80 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7.1
 Requires-Dist: argparse>=1.4.0
-Requires-Dist: openai==0.27.0
+Requires-Dist: openai>=0.27.0
+Requires-Dist: poe-api>=0.3.1
 Provides-Extra: testing
 Requires-Dist: coverage==5.5; extra == 'testing'
 Requires-Dist: pytest==7.1.3; extra == 'testing'
 Description-Content-Type: text/markdown
 
-# GPT simplify your daily Workflow (gptW)
+# GPT Simplify Your Daily Workflow (gptW)
 
-It is no longer necessary to manually input prompts and interact with ChatGPT
+No longer is it necessary to manually input prompts and interact with ChatGPT.
 
 With the GPTW tool, prompt operations are fully automated! Simplify your daily workflow.
 
 ## Example
 
 ### Translate
 
-You can simply use the "ww" command without having to first instruct ChatGPT that the following task is a translation
+You can simply use the "ww" command without having to first instruct ChatGPT that the following task is a translation.
 
-Translate to English
+Translate to English:
 
 ```shell
 $ ww e "今天天气怎么样"
-
 How's the weather today?
 ```
 
-Translate to Chinese
+Translate to Chinese:
 
 ```shell
 $ ww c "who are you? "
-
 你是谁？(Nǐ shì shéi?)
 ```
 
-### Polish the document
+### Polish the Document
 
-Polish a document, supporting files as input.
+Polish a document with files as input.
 
 ```shell
 ww d -f README.md
 ```
 
 ### Code Review
 
 ```shell
 $ ww r -f gptw/gptw.py
-
 As an AI language model, I cannot run the code provided, but I can provide some feedback based on the code structure and syntax.
 
-1. The code seems to be well-organized and follows PEP 8 guidelines for Python code.
+1. The code appears to be well-organized and follows the PEP 8 guidelines for Python code.
 
 2. The argparse module is used to parse command-line arguments, which is a good practice for command-line applications.
 
 ...
 
 Overall, the code seems to be well-written and organized, but could benefit from some additional security measures and error handling.
 ```
 
 ### Ask
 
-Ask ChatGPT directly
+Ask ChatGPT directly:
 
 ```shell
 $ ww a "who are you? "
-
 I am an AI language model created by OpenAI.
 ```
 
-### Add your custom prompt
+### Add Your Custom Prompt
 
 Prepare your prompt and modify the gptw/config.json file following the existing format. Then, submit a PR or directly raise an issue to explain the command you want to add.
 
 gtpw/config.json:
 
 ```json
 {
@@ -110,32 +107,50 @@
 }
 ```
 
 Currently, the following workflows are supported. You can run "ww -l" to obtain the available workflows.
 
 ```shell
 $ ww --list
-
 cmd | meaning                        | example
 e   | Translate into English         | ww e 你好
 c   | Translate into Chinese         | ww c how r u
 p   | Polish sentence                | ww p hwo are you
 a   | Just ask ChatGPT directly      | ww a who are you
 d   | Polish document                | ww d -f README.md
 r   | Code Review                    | ww r -f gptw/gptw.py
 dic | Dictionary                     | ww dic dictionary
 ```
 
 ## Installation
 
 ```shell
 pip install --upgrade gptw
-ww --key sk-..... # set your OpenAI API key
 ```
 
+### OpenAI Config
+
+```shell
+ww --config provider=openai
+ww --config openai-model=gpt-3.5-turbo
+ww --config openai-token={YOUR_TOKEN}
+```
+
+### POE Config
+
+```shell
+ww --config provider=poe
+ww --config poe-bot-name=chinchilla
+ww --config poe-token={YOUR_TOKEN}
+```
+
+Bot names:
+
+{'capybara': 'Sage', 'beaver': 'GPT-4', 'a2_2': 'Claude+', 'a2': 'Claude', 'chinchilla': 'ChatGPT', 'nutria': 'Dragonfly'}
+
 ## Uninstall
 
 ```shell
 pip uninstall gptw
 ```
 
 ## Development
```

