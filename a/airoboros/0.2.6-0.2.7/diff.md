# Comparing `tmp/airoboros-0.2.6.tar.gz` & `tmp/airoboros-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airoboros-0.2.6.tar", last modified: Sat May 13 23:18:16 2023, max compression
+gzip compressed data, was "airoboros-0.2.7.tar", last modified: Tue May 16 16:35:04 2023, max compression
```

## Comparing `airoboros-0.2.6.tar` & `airoboros-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:18:16.709378 airoboros-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-13 23:18:02.000000 airoboros-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-13 23:18:16.709378 airoboros-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-13 23:18:02.000000 airoboros-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:18:16.705378 airoboros-0.2.6/airoboros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 23:18:02.000000 airoboros-0.2.6/airoboros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-13 23:18:02.000000 airoboros-0.2.6/airoboros/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-13 23:18:02.000000 airoboros-0.2.6/airoboros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-05-13 23:18:02.000000 airoboros-0.2.6/airoboros/self_instruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:18:16.709378 airoboros-0.2.6/airoboros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-13 23:18:16.000000 airoboros-0.2.6/airoboros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-13 23:18:16.000000 airoboros-0.2.6/airoboros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:18:16.000000 airoboros-0.2.6/airoboros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-13 23:18:16.000000 airoboros-0.2.6/airoboros.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-13 23:18:16.000000 airoboros-0.2.6/airoboros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-13 23:18:16.000000 airoboros-0.2.6/airoboros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 23:18:16.709378 airoboros-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-13 23:18:02.000000 airoboros-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:35:04.189690 airoboros-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 16:34:50.000000 airoboros-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-16 16:35:04.189690 airoboros-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-16 16:34:50.000000 airoboros-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:35:04.185690 airoboros-0.2.7/airoboros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:34:50.000000 airoboros-0.2.7/airoboros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-16 16:34:50.000000 airoboros-0.2.7/airoboros/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-16 16:34:50.000000 airoboros-0.2.7/airoboros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-05-16 16:34:50.000000 airoboros-0.2.7/airoboros/self_instruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:35:04.189690 airoboros-0.2.7/airoboros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-16 16:35:04.000000 airoboros-0.2.7/airoboros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 16:35:04.000000 airoboros-0.2.7/airoboros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:35:04.000000 airoboros-0.2.7/airoboros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 16:35:04.000000 airoboros-0.2.7/airoboros.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 16:35:04.000000 airoboros-0.2.7/airoboros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 16:35:04.000000 airoboros-0.2.7/airoboros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:35:04.189690 airoboros-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 16:34:50.000000 airoboros-0.2.7/setup.py
```

### Comparing `airoboros-0.2.6/LICENSE` & `airoboros-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airoboros-0.2.6/PKG-INFO` & `airoboros-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.2.6
+Version: 0.2.7
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-0.2.6/README.md` & `airoboros-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `airoboros-0.2.6/airoboros/self_instruct.py` & `airoboros-0.2.7/airoboros/self_instruct.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import string
 import sys
 import threading
 import concurrent.futures
 from functools import partial
 from loguru import logger
 from queue import Queue, Empty
+from time import sleep
 from typing import List, Dict, Any
 from uuid import uuid4
 from .exceptions import (
     RateLimitError,
     TooManyRequestsError,
     TokensExhaustedError,
     ServerOverloadedError,
@@ -63,14 +64,15 @@
 
 Requirements:
 {topics}
 
 Numbered list of {batch_size} instructions:
 """
 CONTEXT_TASK_INJECTION = """After generating your response, add a line with "=:=:=", then generate a unique and interesting instruction or question that could be answered using only the generated text.  Examples include summarization, questions about specific details found within the text, or information extraction."""
+FORMAT_INJECTION = """If appropriate, the instruction or question should ask for a specific response format, e.g. JSON, YAML, SQL, markdown table, XML, CSV, etc."""
 DEFAULT_PROMPT = """Create a set of {batch_size} diverse instructions.
 
 Requirements for the instructions:
  * Do not repeat the verb for each instruction to maximize diversity.
  * The list of instructions should include a variety of types of prompts, such as open-ended text generation, creative writing, brainstorming, classification, editing, logical reasoning, riddles, mathematics, etc.
  * Any task related to logical reasoning or mathematics should also include asking for step-by-step reasoning.
  * Each instruction must be something a large language model can complete with a text-only response without any access to the internet.  For example do not create a task asking to create or use visual/audio output, setting an alarm, scheduling something on the calendar, read content from a website, etc. because the language model cannot perform those tasks.
@@ -165,14 +167,19 @@
             "help": "prompt prefix to use for generating non-contextual instructions",
         },
         "--contextual-prompt": {
             "type": str,
             "default": CONTEXTUAL_PROMPT,
             "help": "prompt to use for generating contextual prompts",
         },
+        "--uncensored-prompt": {
+            "type": str,
+            "default": UNCENSORED_PROMPT,
+            "help": "prompt to use when attempting to avoid OpenAI censorship",
+        },
         "--topic-generation-prompt": {
             "type": str,
             "default": TOPIC_GENERATION_PROMPT,
             "help": "prompt to use in generating random topics",
         },
         "--topic-request-count": {
             "type": int,
@@ -292,15 +299,16 @@
         self.presence_penalty = presence_penalty
         self.max_usage_tokens = max_usage_tokens
         self.validate_model()
         self.used_tokens = 0
         self.stop_producing = False
         self.concurrency = concurrency
         self.min_docsearch_score = min_docsearch_score
-        self.initialize_docstores()
+        self.topic_index = 0
+        self.topic_lock = threading.Lock()
 
     def initialize_docstores(self):
         """Initialize the in-memory vector databases used to check prompt uniqueness."""
         self.machine_task_count = 0
         docs = []
         if os.path.exists(self.output_path):
             if self.overwrite:
@@ -322,14 +330,16 @@
             "Initializing in-memory document store for similarity comparison..."
         )
         if not docs:
             docs = ["__initialize__"]
         self.embeddings = HuggingFaceEmbeddings()
         self.docstores = [Chroma.from_texts(docs, self.embeddings)]
         self.docstore_rotated_at = 0
+        self.topic_index = self.machine_task_count % len(self.topics)
+        self.topic_index = 0
         if self.machine_task_count >= MAX_DOCSTORE_SIZE:
             logger.info("Initializing fresh docstore due to doc count...")
             self.docstore_rotated_at = self.machine_task_count
             self.docstores.append(
                 Chroma.from_texts(["__initialize__"], self.embeddings)
             )
 
@@ -353,31 +363,34 @@
                 f"Invalid openai API key [{result.status_code}: {result.text}]"
             )
         available = {item["id"] for item in result.json()["data"]}
         if self.model not in available:
             raise ValueError(f"Model is not available to your API key: {self.model}")
         logger.success(f"Successfully validated model: {self.model}")
 
-    def initialize_topics(self) -> None:
-        """Read existing cached topics, or generate a new list."""
-        if self.topics_path:
+    def initialize_topics(self, save: bool = True) -> None:
+        """Read existing cached topics, or generate a new list.
+
+        :param save: Flag dictating whether or not to save results to disk.
+        :type save: bool
+        """
+        if save and self.topics_path:
             if not os.path.exists(self.topics_path):
-                raise ValueError(f"Topics file: {self.topics_path} does not exis!")
-        if not self.topics_path:
+                raise ValueError(f"Topics file: {self.topics_path} does not exist!")
+        if save and not self.topics_path:
             self.topics_path = f"topics-{hashlib.md5((self.topic_generation_prompt + str(self.topic_request_count)).encode()).hexdigest()}.txt"
-        if os.path.exists(self.topics_path):
+        if save and os.path.exists(self.topics_path):
             with open(self.topics_path, "r") as infile:
-                self.topics = {
-                    line.strip() for line in infile.readlines() if line.strip()
-                }
+                self.topics = list(
+                    {line.strip() for line in infile.readlines() if line.strip()}
+                )
                 logger.info(
                     f"Using {len(self.topics)} topics from {self.topics_path}..."
                 )
                 return
-        self.topics = set([])
         logger.info("Generating random topics to use in prompts...")
         prompt_payload = {
             "model": "gpt-3.5-turbo",
             "messages": [
                 {
                     "role": "user",
                     "content": self.topic_generation_prompt,
@@ -399,50 +412,63 @@
             ]
         topic_prompts = [prompt_payload for _ in range(self.topic_request_count)]
         with concurrent.futures.ThreadPoolExecutor(self.concurrency) as pool:
             responses = pool.map(
                 partial(self._post_no_exc, "/v1/chat/completions"), topic_prompts
             )
         seen = set([])
-        with open(self.topics_path, "w") as outfile:
+        self.topics = []
+        try:
+            if save:
+                outfile = open(self.topics_path, "w")
             for response in responses:
                 if not response:
                     continue
                 for choice in response["choices"]:
                     for line in choice["message"]["content"].splitlines():
                         if self.uncensored:
                             if line.startswith("REMINDER:") or self.bot_name in line:
                                 continue
                         if " list of " in line:
                             continue
                         topic = re.sub(r"(\s*\d+\s*\.\s+)+", "", line).strip()
                         if not topic or topic.lower() in seen:
                             continue
                         seen.add(topic.lower())
-                        self.topics.add(topic)
-                        outfile.write(topic + "\n")
+                        self.topics.append(topic)
+                        if save:
+                            outfile.write(topic + "\n")
+        finally:
+            if save:
+                outfile.close()
         logger.success(
             f"Successfully generated {len(self.topics)} topics, stored in {self.topics_path}..."
         )
 
     def generate_prompt(self, template: str):
         """Generate a single prompt, inserting random topics.
 
         :param template: The prompt template to use.
         :type template: str
 
         :return: The prompt, including a list of random topics.
         :rtype: str
         """
+        self.topic_lock.acquire()
+        topics = []
+        for _ in range(self.batch_size):
+            topics.append(self.topics[self.topic_index])
+            self.topic_index += 1
+            if self.topic_index >= len(self.topics):
+                self.topic_index = 0
+        self.topic_lock.release()
         topics = "\n".join(
             [
                 f" * instruction {idx + 1} must be related to topic: {json.dumps(topic)}"
-                for idx, topic in enumerate(
-                    random.sample(list(self.topics), self.batch_size)
-                )
+                for idx, topic in enumerate(topics)
             ]
         )
         return template.format(topics=topics, batch_size=self.batch_size)
 
     def extract_instructions_from_response(self, text: str) -> List[str]:
         """Extract the list of instructions from the OpenAI response.
 
@@ -504,17 +530,19 @@
             f"{OPENAI_API_BASE_URL}{path}",
             headers=headers,
             json=payload,
             timeout=600.0,
         )
         if result.status_code != 200:
             text = result.text
+            logger.error(f"OpenAI request error: {text}")
             if "too many requests" in text.lower():
                 raise TooManyRequestsError(text)
             if "rate limit reached" in text.lower():
+                sleep(30)
                 raise RateLimitError(text)
             elif "context_length_exceeded" in text.lower():
                 raise ContextLengthExceededError(text)
             elif "server_error" in text and "overloaded" in text.lower():
                 raise ServerOverloadedError(text)
             elif "bad gateway" in text.lower() or "server_error" in text.lower():
                 raise ServerError(text)
@@ -566,15 +594,14 @@
                 instruction = (
                     self.uncensored_prompt.format(bot_name=self.bot_name)
                     + f"\nInstruction: {instruction}"
                 )
             payload["prompt"] = instruction
             payload["max_tokens"] = 2000
         else:
-            payload["max_tokens"] = 2000
             if self.uncensored:
                 payload["messages"] = [
                     {
                         "role": "user",
                         "content": self.uncensored_prompt.format(
                             bot_name=self.bot_name
                         ),
@@ -607,15 +634,15 @@
                 f"(^|[\\r\\n\\s]+){re.escape(self.bot_name)}(\\s+\\w+\\s*)?:[\\s\\r\\n]*",
                 r"\1",
                 text,
             ).strip()
             if "OpenAI" in text:
                 logger.warning(f"Attempt to bypass restrictions failed: {text}")
                 return None
-            if "As an AI" in text:
+            if "as an ai " in text.lower() or "as an ai," in text.lower():
                 logger.warning(
                     f"{self.bot_name} appears to have left character:\nInstruction: {instruction}\nResponse: {text}"
                 )
                 if recurse:
                     return self.generate_response(
                         f"Rewriting the following output to remove any reference that it was generated by an AI:\n{text}",
                         recurse=False,
@@ -637,23 +664,28 @@
         for new_instruction in self.extract_instructions_from_response(
             self.generate_response(
                 prompt, temperature=self.prompt_generation_temperature
             )
         ):
             prompt = new_instruction
             if contextual:
-                prompt = self.generate_response(
-                    "  ".join([new_instruction, CONTEXT_TASK_INJECTION])
-                )
+                injected = new_instruction + CONTEXT_TASK_INJECTION
+                if random.random() <= 0.2:
+                    injected += " " + FORMAT_INJECTION
+                prompt = self.generate_response(injected)
                 if not prompt or "=:=:=" not in prompt:
                     logger.error(
                         f"Error generating contextual prompt: {new_instruction}"
                     )
                     continue
-                parts = [part.strip() for part in prompt.split("=:=:=") if part.strip()]
+                parts = [
+                    part.strip().lstrip(":").strip()
+                    for part in prompt.split("=:=:=")
+                    if part.strip()
+                ]
                 if len(parts) != 2:
                     logger.warning(
                         f"Contextual prompt returned incorrect part count: {prompt}"
                     )
                     continue
                 flip = random.random()
                 if flip <= 0.7:
@@ -705,15 +737,15 @@
                         instruction["instruction"], k=1
                     )
                     for _, score in similar:
                         if score < min_score:
                             min_score = score
                 if min_score <= self.min_docsearch_score:
                     logger.warning(
-                        f"Skipping instruction, too similar [{score}]: {instruction['instruction']}"
+                        f"Skipping instruction, too similar [{min_score}]: {instruction['instruction']}"
                     )
                     continue
                 outfile.write(json.dumps(instruction) + "\n")
                 outfile.flush()
                 self.machine_task_count += 1
                 if self.machine_task_count >= self.instruction_count:
                     self.stop_producing = True
@@ -742,15 +774,14 @@
         result = self.generate_response(instruction["instruction"])
         if result:
             return {"instruction": instruction["instruction"], "response": result}
         return None
 
     def run_prompt_generation_phase(self):
         """Run the self-instruct, instruction generation (without responses)."""
-        self.initialize_topics()
         if self.machine_task_count >= self.instruction_count:
             logger.warning(
                 f"Already have {self.machine_task_count} machine-generated tasks, skipping generation..."
             )
             return
         queue = Queue(maxsize=self.concurrency * BATCH_SIZE)
         producers = [
@@ -858,27 +889,104 @@
         for producer in producers:
             producer.join()
         consumer.join()
         os.rename(tmp_path, self.output_path)
 
     def run(self):
         """Run prompt generation and answer to completion."""
+        self.initialize_topics()
+        self.initialize_docstores()
         self.run_prompt_generation_phase()
         logger.success(
             f"Finished generating instructions [asked for {self.instruction_count}, created {self.machine_task_count}], generating responses..."
         )
         self.run_response_generation_phase()
         logger.success(
             f"Finished self-instruct task, total instructions: {self.machine_task_count}"
         )
 
 
-def main(args):
+def generate_instructions(args):
     random.seed(secrets.randbelow(1000000000))
     parser = argparse.ArgumentParser()
     for arg, kwargs in SelfInstructor.CLI_ARGS.items():
         parser.add_argument(arg, **kwargs)
     SelfInstructor(**vars(parser.parse_args(args))).run()
 
 
+def generate_topic_batch(worker: SelfInstructor) -> List[str]:
+    """Generate a list of topics (used by generate_topics)."""
+    worker.initialize_topics()
+    return worker.topics
+
+
+def generate_topics(args):
+    random.seed(secrets.randbelow(1000000000))
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "--prompts-path",
+        type=str,
+        help="path to a newline seperated list of prompts to use in generating topics",
+    )
+    parser.add_argument(
+        "--prompts",
+        type=str,
+        nargs="+",
+        help="prompt(s) to use in generating topics",
+    )
+    parser.add_argument("--concurrency", **SelfInstructor.CLI_ARGS["--concurrency"])
+    parser.add_argument(
+        "--output-path",
+        type=str,
+        required=True,
+        help="path to save generated topics to",
+    )
+    parser.add_argument(
+        "--request-count", **SelfInstructor.CLI_ARGS["--topic-request-count"]
+    )
+    parser.add_argument("--uncensored", **SelfInstructor.CLI_ARGS["--uncensored"])
+    parser.add_argument(
+        "--uncensored-prompt", **SelfInstructor.CLI_ARGS["--uncensored-prompt"]
+    )
+    args = vars(parser.parse_args(args))
+    output_path = args.pop("output_path")
+    if os.path.exists(output_path):
+        raise ValueError(f"{output_path} exists, please specify new file path")
+    args["topic_request_count"] = args.pop("request_count")
+    prompts = args.pop("prompts", None)
+    path = args.pop("prompts_path", None)
+    if not prompts:
+        if path:
+            with open(path, "r") as infile:
+                prompts = [line.strip() for line in infile.readlines() if line.strip()]
+        else:
+            prompts = [TOPIC_GENERATION_PROMPT]
+    worker_concurrency = (
+        len(prompts) if len(prompts) <= args["concurrency"] else args["concurrency"]
+    )
+    request_concurrency = 1
+    if worker_concurrency < args["concurrency"] and args["topic_request_count"] > 1:
+        request_concurrency = min(
+            int(args["concurrency"] / worker_concurrency) or 1, args["concurrency"]
+        )
+    args["concurrency"] = request_concurrency
+    instructors = [
+        SelfInstructor(topic_generation_prompt=prompt, **args) for prompt in prompts
+    ]
+    seen = set([])
+    logger.info(f"Generating topics with {len(prompts)} prompt(s)...")
+    with open(output_path, "w") as outfile:
+        with concurrent.futures.ThreadPoolExecutor(worker_concurrency) as pool:
+            for topics in pool.map(generate_topic_batch, instructors):
+                for topic in topics:
+                    key = topic.lower().strip()
+                    if key in seen:
+                        continue
+                    seen.add(key)
+                    outfile.write(topic + "\n")
+    logger.success(
+        f"Successfully generated {len(seen)} unique topics with {len(prompts)} prompt(s)."
+    )
+
+
 if __name__ == "__main__":
-    main(sys.argv[1:])
+    generate_instructions(sys.argv[1:])
```

### Comparing `airoboros-0.2.6/airoboros.egg-info/PKG-INFO` & `airoboros-0.2.7/airoboros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.2.6
+Version: 0.2.7
 Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `airoboros-0.2.6/setup.py` & `airoboros-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md")) as infile:
     long_description = infile.read()
 
 setup(
     name="airoboros",
-    version="0.2.6",
+    version="0.2.7",
     description="Updated and improved implementation of the self-instruct system.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jondurbin/airoboros",
     author="Jon Durbin",
     license="Apache 2.0",
     packages=["airoboros"],
```

