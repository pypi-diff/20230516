# Comparing `tmp/osnap_client-0.1.1a0.tar.gz` & `tmp/osnap_client-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osnap_client-0.1.1a0.tar", max compression
+gzip compressed data, was "osnap_client-0.1.1a1.tar", max compression
```

## Comparing `osnap_client-0.1.1a0.tar` & `osnap_client-0.1.1a1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-05-08 19:45:21.346835 osnap_client-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     2100 2023-05-08 19:45:21.347228 osnap_client-0.1.1a0/README.md
--rw-r--r--   0        0        0      104 2023-04-30 13:42:55.538518 osnap_client-0.1.1a0/osnap_client/README.md
--rw-r--r--   0        0        0     2487 2023-05-08 19:45:21.354153 osnap_client-0.1.1a0/osnap_client/SwarmAdapters/BaseSwarmAdapter.py
--rw-r--r--   0        0        0     2781 2023-05-08 19:45:21.354324 osnap_client-0.1.1a0/osnap_client/SwarmAdapters/DiscordSwarmAdapter.py
--rw-r--r--   0        0        0      116 2023-05-08 19:45:21.354478 osnap_client-0.1.1a0/osnap_client/SwarmAdapters/__init__.py
--rw-r--r--   0        0        0      185 2023-05-08 19:45:21.354741 osnap_client-0.1.1a0/osnap_client/__init__.py
--rw-r--r--   0        0        0     3680 2023-05-08 19:45:21.354891 osnap_client-0.1.1a0/osnap_client/agents/OutboundAgents Spec.md
--rw-r--r--   0        0        0     3193 2023-05-08 19:45:21.355008 osnap_client-0.1.1a0/osnap_client/agents/PersonalAgent.py
--rw-r--r--   0        0        0     2484 2023-05-08 19:45:21.355126 osnap_client-0.1.1a0/osnap_client/agents/outbound_agent.py
--rw-r--r--   0        0        0     1365 2023-05-08 19:45:21.355231 osnap_client-0.1.1a0/osnap_client/agents/planner.py
--rw-r--r--   0        0        0     1419 2023-05-08 19:45:21.355437 osnap_client-0.1.1a0/osnap_client/core/api.py
--rw-r--r--   0        0        0     1314 2023-05-08 19:45:21.355551 osnap_client-0.1.1a0/osnap_client/core/crypt.py
--rw-r--r--   0        0        0    10280 2023-05-08 19:45:21.355693 osnap_client-0.1.1a0/osnap_client/core/osnap.py
--rw-r--r--   0        0        0     4902 2023-05-08 19:45:21.355822 osnap_client-0.1.1a0/osnap_client/main.py
--rw-r--r--   0        0        0       46 2023-05-04 11:18:07.891203 osnap_client-0.1.1a0/osnap_client/pubsub/__init__.py
--rw-r--r--   0        0        0     2666 2023-05-04 12:56:55.387076 osnap_client-0.1.1a0/osnap_client/pubsub/pubsub.py
--rw-r--r--   0        0        0       98 2023-05-08 19:45:21.355950 osnap_client-0.1.1a0/osnap_client/registry/__init__.py
--rw-r--r--   0        0        0     3149 2023-05-08 19:45:21.356129 osnap_client-0.1.1a0/osnap_client/registry/agent_registry.py
--rw-r--r--   0        0        0        0 2023-05-08 19:47:42.311354 osnap_client-0.1.1a0/osnap_client/registry/registry.py
--rw-r--r--   0        0        0     1813 2023-05-08 19:45:21.356252 osnap_client-0.1.1a0/osnap_client/registry/tool_registry.py
--rw-r--r--   0        0        0        0 2023-05-08 19:45:21.356306 osnap_client-0.1.1a0/osnap_client/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:45:21.356359 osnap_client-0.1.1a0/osnap_client/tools/main.py
--rw-r--r--   0        0        0     2449 2023-05-08 19:45:21.356653 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/EngineBase.py
--rw-r--r--   0        0        0     2846 2023-05-08 19:45:21.356776 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/GPTConversEngine.py
--rw-r--r--   0        0        0     2972 2023-05-08 19:45:21.356913 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
--rw-r--r--   0        0        0      136 2023-05-08 19:45:21.357064 osnap_client-0.1.1a0/osnap_client/utils/ai_engines/__init__.py
--rw-r--r--   0        0        0     1038 2023-05-11 18:23:24.253894 osnap_client-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     3041 1970-01-01 00:00:00.000000 osnap_client-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 13:26:06.322716 osnap_client-0.1.1a1/LICENSE
+-rw-r--r--   0        0        0     2100 2023-05-12 13:26:06.322997 osnap_client-0.1.1a1/README.md
+-rw-r--r--   0        0        0      104 2023-05-15 15:30:42.332818 osnap_client-0.1.1a1/osnap_client/README.md
+-rw-r--r--   0        0        0      214 2023-05-16 10:31:58.826057 osnap_client-0.1.1a1/osnap_client/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-16 10:31:58.826379 osnap_client-0.1.1a1/osnap_client/adapters/AdapterBase.py
+-rw-r--r--   0        0        0     4521 2023-05-16 10:31:58.826577 osnap_client-0.1.1a1/osnap_client/adapters/DiscordAdapter.py
+-rw-r--r--   0        0        0      190 2023-05-16 10:31:58.826785 osnap_client-0.1.1a1/osnap_client/adapters/QueueTaskStruct.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:31:58.826811 osnap_client-0.1.1a1/osnap_client/adapters/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-16 10:31:58.827074 osnap_client-0.1.1a1/osnap_client/agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:31:58.827101 osnap_client-0.1.1a1/osnap_client/agents/base.py
+-rw-r--r--   0        0        0     3744 2023-05-16 10:31:58.827745 osnap_client-0.1.1a1/osnap_client/agents/swarm_agents/swarm_agent.py
+-rw-r--r--   0        0        0      199 2023-05-16 10:31:58.828093 osnap_client-0.1.1a1/osnap_client/core/__init__.py
+-rw-r--r--   0        0        0     5934 2023-05-16 10:31:58.828320 osnap_client-0.1.1a1/osnap_client/core/agent.py
+-rw-r--r--   0        0        0     1419 2023-05-15 15:30:42.335469 osnap_client-0.1.1a1/osnap_client/core/api.py
+-rw-r--r--   0        0        0     1314 2023-05-15 15:30:42.335759 osnap_client-0.1.1a1/osnap_client/core/crypt.py
+-rw-r--r--   0        0        0     6296 2023-05-16 10:31:58.828625 osnap_client-0.1.1a1/osnap_client/core/osnap.py
+-rw-r--r--   0        0        0     5177 2023-05-15 15:30:42.336130 osnap_client-0.1.1a1/osnap_client/main.py
+-rw-r--r--   0        0        0       46 2023-05-15 15:30:42.336488 osnap_client-0.1.1a1/osnap_client/pubsub/__init__.py
+-rw-r--r--   0        0        0     2666 2023-05-15 15:30:42.336780 osnap_client-0.1.1a1/osnap_client/pubsub/pubsub.py
+-rw-r--r--   0        0        0       98 2023-05-15 15:30:42.337005 osnap_client-0.1.1a1/osnap_client/registry/__init__.py
+-rw-r--r--   0        0        0     3149 2023-05-15 15:30:42.337231 osnap_client-0.1.1a1/osnap_client/registry/agent_registry.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:30:42.337257 osnap_client-0.1.1a1/osnap_client/registry/registry.py
+-rw-r--r--   0        0        0     1813 2023-05-15 15:30:42.337386 osnap_client-0.1.1a1/osnap_client/registry/tool_registry.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:30:42.337442 osnap_client-0.1.1a1/osnap_client/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:30:42.337481 osnap_client-0.1.1a1/osnap_client/tools/main.py
+-rw-r--r--   0        0        0     2449 2023-05-15 15:30:42.337767 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/EngineBase.py
+-rw-r--r--   0        0        0     2846 2023-05-15 15:30:42.337959 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/GPTConversEngine.py
+-rw-r--r--   0        0        0     2972 2023-05-15 15:30:42.338318 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/LanchainGoogleEngine.py
+-rw-r--r--   0        0        0      136 2023-05-15 15:30:42.338425 osnap_client-0.1.1a1/osnap_client/utils/ai_engines/__init__.py
+-rw-r--r--   0        0        0     1181 2023-05-16 10:36:06.881324 osnap_client-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     3193 1970-01-01 00:00:00.000000 osnap_client-0.1.1a1/PKG-INFO
```

### Comparing `osnap_client-0.1.1a0/LICENSE` & `osnap_client-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/README.md` & `osnap_client-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/SwarmAdapters/DiscordSwarmAdapter.py` & `osnap_client-0.1.1a1/osnap_client/pubsub/pubsub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,82 @@
-import sys, os
-sys.path.append(os.path.abspath(os.path.join("../..")))
-
-import discord
 import asyncio
-import json
-import time
-from jsonschema import validate
-
-from osnap.SwarmAdapters.BaseSwarmAdapter import BaseSwarmAdapter
-
-class DiscordSwarmAdapter(BaseSwarmAdapter):
-    """And implementation of the Swarm Adapter for Discord.
-
-    Args:
-        - config (dict): The configuration of the adapter.
-    """
-    def __init__(self, config:dict):
-        super().__init__(config)
-        self.configure(config)
-
-    def configure(self, config:dict):
-        """Configure the adapter.
-
-        Args:
-            - config (dict): The configuration of the adapter.
-            {
-                "bot_token": "your_token",
-                "server": "your_prefix",
-                "entry_channel": "your_entry_channel"
-                "intents": []
-            }
-        """
-        config_schema = {
-            "type": "object",
-            "properties": {
-                "bot_token": {"type": "string"},
-                "server": {"type": "string"},
-                "entry_channel": {"type": "string"},
-                "intents": {"type": "array"}
-            },
-            "required": ["bot_token", "server", "entry_channel"]
-        }
-        validate(instance=config, schema=config_schema)
-
-        self.config = config
-        self.bot_token = config["bot_token"]
-
-        # intents: https://discordpy.readthedocs.io/en/stable/intents.html
-        self.intents = discord.Intents.default()
-        for intent in config["intents"]:
-            # check if the intent is a vaild attribute of discord.Intents
-            if hasattr(self.intents, intent):
-                setattr(self.intents, intent, True)
-            else:
-                raise ValueError(f"Invalid intent: {intent}")
-            
-        self.client = discord.Client(intents=self.intents)
-        
-        # events and commands: https://dev.to/mikeywastaken/events-in-discord-py-mk0
-        self.client.event(self.on_ready)
-        self.client.event(self.on_message)
-
-    def run(self):
-        # TODO: can add logger directly here as a kwarg
-        self.client.run(self.bot_token)
-
-    async def on_ready(self):
-        print(f'{self.client.user} is connected to Discord!')
-
-    async def on_message(self, message):
-        if message.author == self.client.user:
-            return
-
-        if message.content.startswith('!discover'):
-            response = f"Hi, I'm test_bot1"
-            await message.channel.send(response)
-
-        if message.content.startswith('!produce_icecream'):
-            icecreams = self.handle_who_can(message)
-            await message.channel.send(response)
-
-    def handle_who_can(self, message):
-        time.sleep(1)
-        return [{'body': 'icecream'} for _ in range(1)]
+import os
+import redis.asyncio as redis
+from fastapi import WebSocket
+
+REDIS_HOST = os.getenv("REDIS_HOST")
+REDIS_PORT = os.getenv("REDIS_PORT")
+REDIS_USERNAME = os.getenv("REDIS_USERNAME")
+REDIS_PASSWORD = os.getenv("REDIS_PASSWORD")
+
+STOPWORD = "STOP"
+
+
+class ConnectionManager:
+    def __init__(self):
+        self.active_connections: list[WebSocket] = []
+
+    async def connect(self, websocket: WebSocket):
+        await websocket.accept()
+        self.active_connections.append(websocket)
+
+    def disconnect(self, websocket: WebSocket):
+        self.active_connections.remove(websocket)
+
+    async def send_personal_message(self, message: str, websocket: WebSocket):
+        await websocket.send_text(message)
+
+    async def broadcast(self, message: str):
+        print(f"Broadcasting: {message}")
+        for connection in self.active_connections:
+            await connection.send_text(message)
+
+
+class PubSub:
+    def __init__(self, redis_url: str = None, channel_name: str = "osnap"):
+        self.redis_url = redis_url
+        self.channel_name = channel_name
+        self.redis = None
+        self.pubsub = None
+        self.manager = ConnectionManager()
+
+    async def connect(self):
+        self.redis = redis.Redis(
+            host=REDIS_HOST,
+            port=REDIS_PORT,
+            username=REDIS_USERNAME,
+            password=REDIS_PASSWORD,
+            db=0,
+        )
+        self.pubsub = self.redis.pubsub()
+
+    async def close(self):
+        if self.redis:
+            self.redis.close()
+            await self.redis.wait_closed()
+
+    async def subscribe(self):
+        self.sub = await self.pubsub.subscribe(self.channel_name)
+        future = asyncio.create_task(self.reader(self.pubsub))
+        return future
+
+    async def reader(self, channel: redis.client.PubSub):
+        while True:
+            message = await channel.get_message(ignore_subscribe_messages=True)
+            if message is not None:
+                decoded_message = message["data"].decode()
+                print(f"(Reader) Message Received: {message}")
+                # BUG: not seeing this broadcasted to the client
+                await self.manager.broadcast(decoded_message)
+                if message["data"].decode() == STOPWORD:
+                    print("(Reader) STOP")
+                    break
+
+    async def publish(self, message: str):
+        await self.redis.publish(self.channel_name, message)
+        await self.manager.broadcast(message)
 
+    def on_message(self, message):
+        print(f"Received message: {message}")
 
+    async def add_conn_manager(self, websocket: WebSocket):
+        await self.manager.connect(websocket)
```

### Comparing `osnap_client-0.1.1a0/osnap_client/core/api.py` & `osnap_client-0.1.1a1/osnap_client/core/api.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/core/crypt.py` & `osnap_client-0.1.1a1/osnap_client/core/crypt.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/main.py` & `osnap_client-0.1.1a1/osnap_client/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-import os
-import math
-from redis.exceptions import ResponseError
-from langchain import LLMChain, PromptTemplate
-from langchain.agents import ZeroShotAgent, Tool, AgentExecutor
-from registry.agent_registry import AgentRegistry
-from langchain.agents.agent_toolkits import FileManagementToolkit
-from langchain.chains import RetrievalQA
-from langchain.chat_models import ChatOpenAI
-from langchain.embeddings import OpenAIEmbeddings
-from langchain.experimental import BabyAGI
-from langchain.retrievers import TimeWeightedVectorStoreRetriever
-from langchain.tools import ShellTool
-from langchain.vectorstores.redis import Redis
-
-from langchain.agents.agent_toolkits import (
-    create_vectorstore_agent,
-    VectorStoreToolkit,
-    VectorStoreInfo,
-)
-from tempfile import TemporaryDirectory
-
-from langchain.llms import OpenAI
-from langchain.agents import initialize_agent
-from langchain.agents.agent_toolkits import ZapierToolkit
-from langchain.agents import AgentType
-from langchain.utilities.zapier import ZapierNLAWrapper
-
-# Change to your liking
-verbose = True
-
-REDIS_HOST = os.getenv("REDIS_HOST")
-REDIS_PORT = os.getenv("REDIS_PORT")
-REDIS_USERNAME = os.getenv("REDIS_USERNAME")
-REDIS_PASSWORD = os.getenv("REDIS_PASSWORD")
-
-ZAPIER_API_KEY = os.environ["ZAPIER_NLA_API_KEY"] = os.getenv("ZAPIER_API_KEY")
-
-agent_registry = AgentRegistry(REDIS_HOST, REDIS_PORT, REDIS_USERNAME, REDIS_PASSWORD)
-
-embeddings_model = OpenAIEmbeddings(model="text-embedding-ada-002")
-
-def relevance_score_fn(score: float) -> float:
-    return 1.0 - score / math.sqrt(2)
-
-vectorstore = Redis(
-    embedding_function=embeddings_model.embed_query,
-    redis_url=f"redis://{REDIS_USERNAME}:{REDIS_PASSWORD}@{REDIS_HOST}:{REDIS_PORT}",
-    index_name='link',
-    relevance_score_fn=relevance_score_fn,
-)
-
-try:
-    vectorstore._create_index()
-except ResponseError:
-    print('no')
-
-llm = ChatOpenAI(
-    model="gpt-3.5-turbo",
-    temperature=0,
-    #max_tokens=1500,
-    #streaming=True
-    verbose=verbose,
- )
-
-memory_chain = RetrievalQA.from_chain_type(
-    llm=llm,
-    chain_type="stuff",
-    retriever=TimeWeightedVectorStoreRetriever(
-        vectorstore=vectorstore,
-        other_score_keys=["importance"],
-        k=15,
-        decay_rate=0.01,
-        verbose=verbose,
-    ),
-    verbose=verbose,
-)
-
-# Option 1: Complete vectorstore
-tools = VectorStoreToolkit(
-    vectorstore_info=VectorStoreInfo(
-        name="Memory",
-        description="Useful for when you need to quickly access memory of events and people and things that happened recently or longer ago. Always do this first whenever you need external information.",
-        vectorstore=vectorstore,
-        verbose=verbose,
-    ),
-    verbose=verbose,
-).get_tools()
-# Option 2: Time weigh
-#tools.append(
-#    Tool(
-#        name="Memory",
-#        func=memory_chain,
-#        description="Always do this first. Useful for when you need to access memory of events or people or things that happened recently or longer ago.",
-#    )
-#)
-
-tools += FileManagementToolkit().get_tools()
-
-tools += ZapierToolkit.from_zapier_nla_wrapper(ZapierNLAWrapper()).get_tools()
-
-shellTool = ShellTool()
-#shellTool.description = shellTool.description + f"args {shellTool.args}".replace("{", "{{").replace("}", "}}")
-tools.append(shellTool)
-
-tools.append(
-    Tool(
-        name="TODO",
-        func=LLMChain(
-            llm=llm,
-            prompt=PromptTemplate.from_template(
-                "You are a planner who is an expert at coming up with a todo list for a given objective. Come up with a todo list for this objective: {objective}"
-            ),
-            verbose=verbose,
-        ),
-        description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for. Output: a todo list for that objective. Please be very clear what the objective is!",
-        verbose=verbose,
-    ),
-)
-
-prefix = """You are an AI who performs one task based on the following objective: {objective}."""
-suffix = """Question: {objective}
-{agent_scratchpad}"""
-prompt = ZeroShotAgent.create_prompt(
-    tools=tools,
-    prefix=prefix,
-    suffix=suffix,
-    input_variables=["objective", "agent_scratchpad"],
-)
-
-agent_executor = AgentExecutor.from_agent_and_tools(
-    agent=ZeroShotAgent(
-        llm_chain=LLMChain(
-            llm=llm,
-            prompt=prompt,
-            verbose=verbose,
-        ),
-        allowed_tools=[tool.name for tool in tools],
-        verbose=verbose,
-    ),
-    tools=tools,
-    verbose=verbose,
-    #return_intermediate_steps=True,
-    max_iterations=3,
-    max_execution_time=60,
-    early_stopping_method="generate"
-)
-
-OBJECTIVE = "Plan a meeting for today at 4pm"
-
-agent_executor({"objective": OBJECTIVE})
-
-#baby_agi = BabyAGI.from_llm(
-#    llm=llm, 
-#    vectorstore=vectorstore, 
-#    task_execution_chain=agent_executor,
-#    max_iterations=3,
-#    verbose=verbose,
-#)
+# import os
+# import math
+# from redis.exceptions import ResponseError
+# from langchain import LLMChain, PromptTemplate
+# from langchain.agents import ZeroShotAgent, Tool, AgentExecutor
+# from registry.agent_registry import AgentRegistry
+# from langchain.agents.agent_toolkits import FileManagementToolkit
+# from langchain.chains import RetrievalQA
+# from langchain.chat_models import ChatOpenAI
+# from langchain.embeddings import OpenAIEmbeddings
+# from langchain.experimental import BabyAGI
+# from langchain.retrievers import TimeWeightedVectorStoreRetriever
+# from langchain.tools import ShellTool
+# from langchain.vectorstores.redis import Redis
+
+# from langchain.agents.agent_toolkits import (
+#     create_vectorstore_agent,
+#     VectorStoreToolkit,
+#     VectorStoreInfo,
+# )
+# from tempfile import TemporaryDirectory
+
+# from langchain.llms import OpenAI
+# from langchain.agents import initialize_agent
+# from langchain.agents.agent_toolkits import ZapierToolkit
+# from langchain.agents import AgentType
+# from langchain.utilities.zapier import ZapierNLAWrapper
+
+# # Change to your liking
+# verbose = True
+
+# REDIS_HOST = os.getenv("REDIS_HOST")
+# REDIS_PORT = os.getenv("REDIS_PORT")
+# REDIS_USERNAME = os.getenv("REDIS_USERNAME")
+# REDIS_PASSWORD = os.getenv("REDIS_PASSWORD")
+
+# ZAPIER_API_KEY = os.environ["ZAPIER_NLA_API_KEY"] = os.getenv("ZAPIER_API_KEY")
+
+# agent_registry = AgentRegistry(REDIS_HOST, REDIS_PORT, REDIS_USERNAME, REDIS_PASSWORD)
+
+# embeddings_model = OpenAIEmbeddings(model="text-embedding-ada-002")
+
+# def relevance_score_fn(score: float) -> float:
+#     return 1.0 - score / math.sqrt(2)
+
+# vectorstore = Redis(
+#     embedding_function=embeddings_model.embed_query,
+#     redis_url=f"redis://{REDIS_USERNAME}:{REDIS_PASSWORD}@{REDIS_HOST}:{REDIS_PORT}",
+#     index_name='link',
+#     relevance_score_fn=relevance_score_fn,
+# )
+
+# try:
+#     vectorstore._create_index()
+# except ResponseError:
+#     print('no')
+
+# llm = ChatOpenAI(
+#     model="gpt-3.5-turbo",
+#     temperature=0,
+#     #max_tokens=1500,
+#     #streaming=True
+#     verbose=verbose,
+#  )
+
+# memory_chain = RetrievalQA.from_chain_type(
+#     llm=llm,
+#     chain_type="stuff",
+#     retriever=TimeWeightedVectorStoreRetriever(
+#         vectorstore=vectorstore,
+#         other_score_keys=["importance"],
+#         k=15,
+#         decay_rate=0.01,
+#         verbose=verbose,
+#     ),
+#     verbose=verbose,
+# )
+
+# # Option 1: Complete vectorstore
+# tools = VectorStoreToolkit(
+#     vectorstore_info=VectorStoreInfo(
+#         name="Memory",
+#         description="Useful for when you need to quickly access memory of events and people and things that happened recently or longer ago. Always do this first whenever you need external information.",
+#         vectorstore=vectorstore,
+#         verbose=verbose,
+#     ),
+#     verbose=verbose,
+# ).get_tools()
+# # Option 2: Time weigh
+# #tools.append(
+# #    Tool(
+# #        name="Memory",
+# #        func=memory_chain,
+# #        description="Always do this first. Useful for when you need to access memory of events or people or things that happened recently or longer ago.",
+# #    )
+# #)
+
+# tools += FileManagementToolkit().get_tools()
+
+# tools += ZapierToolkit.from_zapier_nla_wrapper(ZapierNLAWrapper()).get_tools()
+
+# shellTool = ShellTool()
+# #shellTool.description = shellTool.description + f"args {shellTool.args}".replace("{", "{{").replace("}", "}}")
+# tools.append(shellTool)
+
+# tools.append(
+#     Tool(
+#         name="TODO",
+#         func=LLMChain(
+#             llm=llm,
+#             prompt=PromptTemplate.from_template(
+#                 "You are a planner who is an expert at coming up with a todo list for a given objective. Come up with a todo list for this objective: {objective}"
+#             ),
+#             verbose=verbose,
+#         ),
+#         description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for. Output: a todo list for that objective. Please be very clear what the objective is!",
+#         verbose=verbose,
+#     ),
+# )
+
+# prefix = """You are an AI who performs one task based on the following objective: {objective}."""
+# suffix = """Question: {objective}
+# {agent_scratchpad}"""
+# prompt = ZeroShotAgent.create_prompt(
+#     tools=tools,
+#     prefix=prefix,
+#     suffix=suffix,
+#     input_variables=["objective", "agent_scratchpad"],
+# )
+
+# agent_executor = AgentExecutor.from_agent_and_tools(
+#     agent=ZeroShotAgent(
+#         llm_chain=LLMChain(
+#             llm=llm,
+#             prompt=prompt,
+#             verbose=verbose,
+#         ),
+#         allowed_tools=[tool.name for tool in tools],
+#         verbose=verbose,
+#     ),
+#     tools=tools,
+#     verbose=verbose,
+#     #return_intermediate_steps=True,
+#     max_iterations=3,
+#     max_execution_time=60,
+#     early_stopping_method="generate"
+# )
+
+# OBJECTIVE = "Plan a meeting for today at 4pm"
+
+# agent_executor({"objective": OBJECTIVE})
+
+# #baby_agi = BabyAGI.from_llm(
+# #    llm=llm,
+# #    vectorstore=vectorstore,
+# #    task_execution_chain=agent_executor,
+# #    max_iterations=3,
+# #    verbose=verbose,
+# #)
 
-#baby_agi({"objective": OBJECTIVE})
+# #baby_agi({"objective": OBJECTIVE})
```

### Comparing `osnap_client-0.1.1a0/osnap_client/registry/agent_registry.py` & `osnap_client-0.1.1a1/osnap_client/registry/agent_registry.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/registry/tool_registry.py` & `osnap_client-0.1.1a1/osnap_client/registry/tool_registry.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/utils/ai_engines/EngineBase.py` & `osnap_client-0.1.1a1/osnap_client/utils/ai_engines/EngineBase.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/utils/ai_engines/GPTConversEngine.py` & `osnap_client-0.1.1a1/osnap_client/utils/ai_engines/GPTConversEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/osnap_client/utils/ai_engines/LanchainGoogleEngine.py` & `osnap_client-0.1.1a1/osnap_client/utils/ai_engines/LanchainGoogleEngine.py`

 * *Files identical despite different names*

### Comparing `osnap_client-0.1.1a0/PKG-INFO` & `osnap_client-0.1.1a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: osnap-client
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: 
 Author: Forrest Murray
 Author-email: FMurray@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: cryptography (>=40.0.2,<40.1.0)
+Requires-Dist: discord (>=2.2.3,<3.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
-Requires-Dist: langchain (>=0.0.154,<0.0.155)
+Requires-Dist: ipykernel (>=6.23.0,<7.0.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Requires-Dist: langchain (>=0.0.153,<0.1.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: redis (>=4.5.4,<5.0.0)
+Requires-Dist: pydantic (>=1.10.7,<1.11.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: redis (>=4.5.4,<4.6.0)
 Requires-Dist: rsa (>=4.9,<5.0)
-Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0)
-Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Description-Content-Type: text/markdown
 
 # OSNAP
```

