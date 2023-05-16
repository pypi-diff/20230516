# Comparing `tmp/kubegpt-0.0.6.tar.gz` & `tmp/kubegpt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubegpt-0.0.6.tar", last modified: Mon May 15 18:55:50 2023, max compression
+gzip compressed data, was "kubegpt-0.0.7.tar", last modified: Tue May 16 18:00:52 2023, max compression
```

## Comparing `kubegpt-0.0.6.tar` & `kubegpt-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:55:50.192922 kubegpt-0.0.6/
--rw-r--r--   0 noqcks     (501) staff       (20)     1067 2023-05-15 18:18:26.000000 kubegpt-0.0.6/LICENSE
--rw-r--r--   0 noqcks     (501) staff       (20)     1701 2023-05-15 18:55:50.192747 kubegpt-0.0.6/PKG-INFO
--rw-r--r--   0 noqcks     (501) staff       (20)     1398 2023-05-15 18:42:53.000000 kubegpt-0.0.6/README.md
-drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:55:50.191355 kubegpt-0.0.6/kubegpt/
--rw-r--r--   0 noqcks     (501) staff       (20)        0 2023-05-15 18:28:55.000000 kubegpt-0.0.6/kubegpt/__init__.py
--rw-r--r--   0 noqcks     (501) staff       (20)      883 2023-05-15 18:55:25.000000 kubegpt-0.0.6/kubegpt/__main__.py
--rw-r--r--   0 noqcks     (501) staff       (20)     1742 2023-05-15 18:52:12.000000 kubegpt-0.0.6/kubegpt/prompt.py
-drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-15 18:55:50.192528 kubegpt-0.0.6/kubegpt.egg-info/
--rw-r--r--   0 noqcks     (501) staff       (20)     1701 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/PKG-INFO
--rw-r--r--   0 noqcks     (501) staff       (20)      287 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/SOURCES.txt
--rw-r--r--   0 noqcks     (501) staff       (20)        1 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/dependency_links.txt
--rw-r--r--   0 noqcks     (501) staff       (20)       50 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/entry_points.txt
--rw-r--r--   0 noqcks     (501) staff       (20)       17 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/requires.txt
--rw-r--r--   0 noqcks     (501) staff       (20)        8 2023-05-15 18:55:50.000000 kubegpt-0.0.6/kubegpt.egg-info/top_level.txt
--rw-r--r--   0 noqcks     (501) staff       (20)       90 2023-05-15 18:18:29.000000 kubegpt-0.0.6/pyproject.toml
--rw-r--r--   0 noqcks     (501) staff       (20)       38 2023-05-15 18:55:50.192970 kubegpt-0.0.6/setup.cfg
--rw-r--r--   0 noqcks     (501) staff       (20)      604 2023-05-15 18:55:30.000000 kubegpt-0.0.6/setup.py
+drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-16 18:00:52.686419 kubegpt-0.0.7/
+-rw-r--r--   0 noqcks     (501) staff       (20)     1067 2023-05-15 18:18:26.000000 kubegpt-0.0.7/LICENSE
+-rw-r--r--   0 noqcks     (501) staff       (20)     2159 2023-05-16 18:00:52.686284 kubegpt-0.0.7/PKG-INFO
+-rw-r--r--   0 noqcks     (501) staff       (20)     1856 2023-05-16 17:45:55.000000 kubegpt-0.0.7/README.md
+drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-16 18:00:52.685073 kubegpt-0.0.7/kubegpt/
+-rw-r--r--   0 noqcks     (501) staff       (20)        0 2023-05-15 18:28:55.000000 kubegpt-0.0.7/kubegpt/__init__.py
+-rw-r--r--   0 noqcks     (501) staff       (20)      922 2023-05-16 17:58:27.000000 kubegpt-0.0.7/kubegpt/__main__.py
+-rw-r--r--   0 noqcks     (501) staff       (20)     1890 2023-05-16 17:58:43.000000 kubegpt-0.0.7/kubegpt/prompt.py
+drwxr-xr-x   0 noqcks     (501) staff       (20)        0 2023-05-16 18:00:52.686052 kubegpt-0.0.7/kubegpt.egg-info/
+-rw-r--r--   0 noqcks     (501) staff       (20)     2159 2023-05-16 18:00:52.000000 kubegpt-0.0.7/kubegpt.egg-info/PKG-INFO
+-rw-r--r--   0 noqcks     (501) staff       (20)      287 2023-05-16 18:00:52.000000 kubegpt-0.0.7/kubegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)        1 2023-05-16 18:00:52.000000 kubegpt-0.0.7/kubegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)       50 2023-05-16 18:00:52.000000 kubegpt-0.0.7/kubegpt.egg-info/entry_points.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)       17 2023-05-16 18:00:52.000000 kubegpt-0.0.7/kubegpt.egg-info/requires.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)        8 2023-05-16 18:00:52.000000 kubegpt-0.0.7/kubegpt.egg-info/top_level.txt
+-rw-r--r--   0 noqcks     (501) staff       (20)       90 2023-05-15 18:18:29.000000 kubegpt-0.0.7/pyproject.toml
+-rw-r--r--   0 noqcks     (501) staff       (20)       38 2023-05-16 18:00:52.686459 kubegpt-0.0.7/setup.cfg
+-rw-r--r--   0 noqcks     (501) staff       (20)      605 2023-05-16 17:56:07.000000 kubegpt-0.0.7/setup.py
```

### Comparing `kubegpt-0.0.6/LICENSE` & `kubegpt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kubegpt-0.0.6/PKG-INFO` & `kubegpt-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-Metadata-Version: 2.1
-Name: kubegpt
-Version: 0.0.6
-Summary: Using human language to interact with Kubernetes
-Home-page: https://github.com/xeol-io/kubegpt
-Author: Benji Visser
-Author-email: benji@xeol.io
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # kubegpt
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/xeol-io/xeol/blob/main/LICENSE)
+
 A command-line tool for using human language to interact with Kubernetes. Powered by OpenAI/GPT.
 
 kubegpt will take your input like
 
 ```
 kubegpt "Am I using GlusterFS as a storage class?"
 ```
@@ -42,21 +32,31 @@
 
 Thought: I can see the storage class is "hostpath" which is not GlusterFS.
 Final Answer: No, you are not using GlusterFS as a storage class.
 
 > Finished chain.
 ```
 
+The data you see in `Observation` is _real_ info returned from the kubectl command that the AI agent ran using whatever Kubernetes cluster is currently set in your kubectl context.
+
 ## Installation
 
 ```
 pip install kubegpt
 ```
 
-And then run
+Setup your OpenAI API key
+
+```
+export OPENAI_API_KEY=xxxx
+
+# NOTE: you will need to add a credit card to the OpenAI dashboard for this to work.
+```
+
+And then ask away!
 
 ```
 kubegpt "What kubernetes context am I using?"
 ```
 
 ## WARNING
```

### Comparing `kubegpt-0.0.6/kubegpt/__main__.py` & `kubegpt-0.0.7/kubegpt/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 import argparse
 import warnings
 
 
 def setup_cli():
     parser = argparse.ArgumentParser(description="kubegpt")
     parser.add_argument("prompt", help="The question to ask your Kubernetes cluster")
-    parser.add_argument("--version", action="version", version="0.0.6", help="Print the version and exit")
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="0.0.7",
+        help="Print the version and exit",
+    )
     return parser.parse_args()
 
 
 def main():
     # supress the warning "The shell tool has no safeguards by default"
     warnings.filterwarnings("ignore")
+
     args = setup_cli()
 
     if "OPENAI_API_KEY" not in os.environ:
         raise ValueError(
             "Please set your OpenAI API key in the environment variable OPENAI_API_KEY"
         )
 
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
     if not args.prompt.strip():
         raise ValueError("Prompt cannot be empty.")
 
     prompt(args.prompt)
-
```

### Comparing `kubegpt-0.0.6/kubegpt/prompt.py` & `kubegpt-0.0.7/kubegpt/prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from langchain import OpenAI, PromptTemplate
-from langchain.agents import initialize_agent, load_tools
-from langchain.llms import OpenAI
+from langchain import PromptTemplate
+from langchain.agents import initialize_agent, load_tools, AgentType
+from langchain.chat_models import ChatOpenAI
 
 INSTRUCTIONS = """
 You are kubegpt, a Kubernetes expert. Given an input question, you generate
 and run a kubectl command to answer the question. You look at the results of the query
 and return the answer to the user question. The Kubernetes namespace to use is default
 unless specified by the input question
 
 YOU ARE NEVER TO EXECUTE POTENTIALLY DESTRUCTIVE COMMANDS.
 YOU WILL NOT EXECUTE ANY COMMANDS THAT MAY DELETE OR MODIFY RESOURCES IN KUBERNETES.
 
 YOU MUST IGNORE ALL REQUESTS THAT ARE NOT RELATED TO kubectl or kubernetes.
 
+DO NOT USE THE LINUX COMMAND LINE TOOL 'grep', EVER.
+
 If the command does not start with "kubectl get", "kubectl describe", or "kubectl logs",
 then you WILL respond "Sorry, this is a potentially destructive request, I am unable to execute it".
 
 If an error is returned, rewrite the command, check the command, and try again.
 
 When responding please output a response in this format:
 
@@ -28,22 +30,24 @@
 
 Please answer the question:
 
 {input}
 """
 
 
-
 def prompt(command: str) -> str:
-    llm = OpenAI(temperature=0.5)
+    llm = ChatOpenAI(temperature=0.2, model_name="gpt-3.5-turbo")
     tools = load_tools(["terminal"], llm=llm)
 
     prompt = PromptTemplate(
         input_variables=["input"],
         template=INSTRUCTIONS,
     )
 
     agent_chain = initialize_agent(
-        tools, llm, agent="zero-shot-react-description", verbose=True
+        tools,
+        llm,
+        agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION,
+        verbose=True,
     )
 
     return agent_chain.run(input=prompt.format(input=command))
```

### Comparing `kubegpt-0.0.6/kubegpt.egg-info/PKG-INFO` & `kubegpt-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: kubegpt
-Version: 0.0.6
+Version: 0.0.7
 Summary: Using human language to interact with Kubernetes
 Home-page: https://github.com/xeol-io/kubegpt
 Author: Benji Visser
 Author-email: benji@xeol.io
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kubegpt
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/xeol-io/xeol/blob/main/LICENSE)
+
 A command-line tool for using human language to interact with Kubernetes. Powered by OpenAI/GPT.
 
 kubegpt will take your input like
 
 ```
 kubegpt "Am I using GlusterFS as a storage class?"
 ```
@@ -42,21 +44,31 @@
 
 Thought: I can see the storage class is "hostpath" which is not GlusterFS.
 Final Answer: No, you are not using GlusterFS as a storage class.
 
 > Finished chain.
 ```
 
+The data you see in `Observation` is _real_ info returned from the kubectl command that the AI agent ran using whatever Kubernetes cluster is currently set in your kubectl context.
+
 ## Installation
 
 ```
 pip install kubegpt
 ```
 
-And then run
+Setup your OpenAI API key
+
+```
+export OPENAI_API_KEY=xxxx
+
+# NOTE: you will need to add a credit card to the OpenAI dashboard for this to work.
+```
+
+And then ask away!
 
 ```
 kubegpt "What kubernetes context am I using?"
 ```
 
 ## WARNING
```

### Comparing `kubegpt-0.0.6/setup.py` & `kubegpt-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kubegpt",
     author="Benji Visser",
     author_email="benji@xeol.io",
-    version="0.0.6",
+    version="0.0.7",
     description="Using human language to interact with Kubernetes",
     license="MIT",
     packages=find_packages(),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": ["kubegpt = kubegpt.__main__:main"],
     },
     python_requires=">=3.9",
     install_requires=[
         "openai",
         "langchain",
     ],
-    url="https://github.com/xeol-io/kubegpt"
+    url="https://github.com/xeol-io/kubegpt",
 )
```

