# Comparing `tmp/transformers-agent-ui-0.4.0.tar.gz` & `tmp/transformers-agent-ui-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers-agent-ui-0.4.0.tar", last modified: Sun May 14 18:59:16 2023, max compression
+gzip compressed data, was "transformers-agent-ui-0.4.1.tar", last modified: Tue May 16 18:03:22 2023, max compression
```

## Comparing `transformers-agent-ui-0.4.0.tar` & `transformers-agent-ui-0.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/
--rw-r--r--   0 jovyan    (1000) users      (100)      119 2023-05-13 18:34:40.000000 transformers-agent-ui-0.4.0/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     7849 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     6220 2023-05-14 18:43:25.000000 transformers-agent-ui-0.4.0/README.md
--rw-r--r--   0 jovyan    (1000) users      (100)     3600 2023-05-14 18:08:48.000000 transformers-agent-ui-0.4.0/pyproject.toml
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/setup.cfg
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.525234 transformers-agent-ui-0.4.0/src/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.529234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/
--rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-05-14 18:58:51.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/__init__.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.533234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/
--rw-r--r--   0 jovyan    (1000) users      (100)      513 2023-05-14 18:38:27.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)   495733 2023-05-14 17:02:40.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/boat-in-water.png
--rw-r--r--   0 jovyan    (1000) users      (100)   445847 2023-05-14 18:35:22.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/capybara.png
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.537234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:44:24.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4993 2023-05-14 16:50:30.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/agent.py
--rw-r--r--   0 jovyan    (1000) users      (100)      813 2023-05-14 03:02:42.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3315 2023-05-14 16:51:53.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/custom_run.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1656 2023-05-14 18:56:46.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/examples.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1919 2023-05-14 17:46:18.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/run.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4431 2023-05-14 07:41:15.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/store.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2166 2023-05-14 02:54:11.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/token.py
--rw-r--r--   0 jovyan    (1000) users      (100)       63 2023-05-13 16:01:28.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/py.typed
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:38:23.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1707 2023-05-14 18:17:54.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/components.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2146 2023-05-14 05:05:11.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1598 2023-05-14 02:39:37.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/token_manager.py
--rw-r--r--   0 jovyan    (1000) users      (100)     8261 2023-05-14 18:15:17.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/transformers_agent_ui.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.529234 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     7849 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     1064 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      147 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/top_level.txt
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.363466 transformers-agent-ui-0.4.1/
+-rw-r--r--   0 jovyan    (1000) users      (100)      119 2023-05-13 18:34:40.000000 transformers-agent-ui-0.4.1/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     7849 2023-05-16 18:03:22.363466 transformers-agent-ui-0.4.1/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     6220 2023-05-16 18:02:33.000000 transformers-agent-ui-0.4.1/README.md
+-rw-r--r--   0 jovyan    (1000) users      (100)     3600 2023-05-14 18:08:48.000000 transformers-agent-ui-0.4.1/pyproject.toml
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-16 18:03:22.363466 transformers-agent-ui-0.4.1/setup.cfg
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.351466 transformers-agent-ui-0.4.1/src/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.351466 transformers-agent-ui-0.4.1/src/transformers_agent_ui/
+-rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-05-16 18:02:50.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/__init__.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.359466 transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/
+-rw-r--r--   0 jovyan    (1000) users      (100)      513 2023-05-14 18:38:27.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)   495733 2023-05-14 17:02:40.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/boat-in-water.png
+-rw-r--r--   0 jovyan    (1000) users      (100)   445847 2023-05-14 18:35:22.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/capybara.png
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.359466 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/
+-rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:44:24.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     4993 2023-05-14 16:50:30.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/agent.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      813 2023-05-14 03:02:42.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/config.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3315 2023-05-14 16:51:53.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/custom_run.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1656 2023-05-14 18:56:46.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/examples.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1919 2023-05-14 17:46:18.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/run.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     4431 2023-05-14 07:41:15.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/store.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     2166 2023-05-14 02:54:11.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/token.py
+-rw-r--r--   0 jovyan    (1000) users      (100)       63 2023-05-13 16:01:28.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/py.typed
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.363466 transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/
+-rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:38:23.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1707 2023-05-14 18:17:54.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/components.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     2159 2023-05-16 16:38:29.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/config.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1598 2023-05-14 02:39:37.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/token_manager.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     8642 2023-05-16 18:00:06.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/transformers_agent_ui.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 18:03:22.355466 transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     7849 2023-05-16 18:03:22.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     1064 2023-05-16 18:03:22.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-16 18:03:22.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      147 2023-05-16 18:03:22.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-05-16 18:03:22.000000 transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/top_level.txt
```

### Comparing `transformers-agent-ui-0.4.0/PKG-INFO` & `transformers-agent-ui-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-agent-ui
-Version: 0.4.0
+Version: 0.4.1
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: awesome-panel
 Project-URL: repository, https://github.com/awesome-panel/transformers-agent-ui
 Keywords: python,huggingface,transformers,deeplearning,ai,agent,holoviz,panel
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `transformers-agent-ui-0.4.0/README.md` & `transformers-agent-ui-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/pyproject.toml` & `transformers-agent-ui-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/__init__.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/boat-in-water.png` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/boat-in-water.png`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/capybara.png` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/assets/capybara.png`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/agent.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/agent.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/config.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/config.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/custom_run.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/custom_run.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/examples.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/examples.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/run.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/run.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/store.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/store.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/token.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/domain/token.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/components.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/components.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/config.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import param
 
 
 class TransformersAgentUIConfig:
     """Configuration settings for the UI"""
 
     title_emoji: str = param.String("🤗")
-    title: str = param.String("Transformers Agent")
+    title: str = param.String("Hugging Face Transformers Agent")
     # pylint: disable=line-too-long
     about: str = param.String(
         f"""The purpose of this app is to provide **an effictive user interface for the
 <a href="https://huggingface.co/docs/transformers/transformers_agents" target="_blank">Hugging Face Transformer Agent</a>.**
 
 <a href="https://panel.holoviz.org" target="_blank"><img src="https://pyviz-dev.github.io/panel/_static/logo_horizontal_light_theme.png" style="height:50px"></img></a>
```

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/token_manager.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/token_manager.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/transformers_agent_ui.py` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui/ui/transformers_agent_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,25 +46,24 @@
 
     def __init__(self, **params):
         if "token_manager" not in params:
             params["token_manager"] = TokenManagerUI(name="Token Manager")
         super().__init__(**params)
 
     def __panel__(self):
-        logo = pn.pane.PNG(
-            object="https://pyviz-dev.github.io/panel/_static/logo_horizontal_light_theme.png",
-            link_url="https://panel.holoviz.org",
-            alt_text="Power by Panel. The powerful data exploration & web app framework for Python",
-            height=50,
-        )
+        # logo = pn.pane.PNG(
+        #     object="https://pyviz-dev.github.io/panel/_static/logo_horizontal_light_theme.png",
+        #     link_url="https://panel.holoviz.org",
+        #     height=50,
+        # )
 
         header = pn.Row(
             f"<h1>{self.config.title_emoji} {self.config.title}</h1>",
             pn.layout.HSpacer(),
-            logo,
+            # logo,
             styles=self.styles.header_styles,
             sizing_mode="stretch_width",
             margin=0,
         )
         editor = self._create_editor()
 
         logs = pn.widgets.Terminal(name="Logs", sizing_mode="stretch_width")
@@ -90,14 +89,41 @@
     def _create_editor(self):
         agent_input = pn.widgets.RadioButtonGroup.from_param(
             self.param.agent, margin=(5, 0), button_style="outline"
         )
         model_input = pn.widgets.RadioButtonGroup.from_param(
             self.param.model, button_style="outline"
         )
+        show_details_input = pn.widgets.Checkbox(
+            value=False,
+            name="Show details",
+            description="If Checked more advanced settings are show",
+        )
+        details = pn.Column(
+            pn.Row(
+                pn.pane.HTML(
+                    "Agent",
+                    styles={
+                        "padding-top": "0.5em",
+                    },
+                ),
+                agent_input,
+                pn.pane.HTML(
+                    "Model",
+                    styles={
+                        "padding-top": "0.5em",
+                        "padding-left": "0.5em",
+                    },
+                ),
+                model_input,
+                align="start",
+            ),
+            pn.Row(self.param.use_cache, self.param.remote, margin=(15, 5)),
+            visible=show_details_input,
+        )
         example_input = get_example_selection_widget(task=self)
         task_input = pn.widgets.TextAreaInput.from_param(
             self.param.task,
             sizing_mode="stretch_width",
             name="Task",
             stylesheets=["textarea { font-size: 2em; }"],
             description="A short text describing the task to run",
@@ -111,33 +137,16 @@
             stylesheets=[self.styles.submit_button_style_sheet],
             name="RUN",
         )
         task_input = pn.Column(task_input, submit_input)
         assets_input = KwargsEditor(kwargs=self.param.kwargs)
 
         inputs = pn.Column(
-            pn.Row(
-                pn.pane.HTML(
-                    "Agent",
-                    styles={
-                        "padding-top": "0.5em",
-                    },
-                ),
-                agent_input,
-                pn.pane.HTML(
-                    "Model",
-                    styles={
-                        "padding-top": "0.5em",
-                        "padding-left": "0.5em",
-                    },
-                ),
-                model_input,
-                align="start",
-            ),
-            pn.Row(self.param.use_cache, self.param.remote, margin=(15, 5)),
+            show_details_input,
+            details,
             pn.Column(
                 example_input,
                 task_input,
                 pn.pane.HTML("Arguments", margin=(0, 10)),
                 pn.pane.Alert(
                     """You can refer to *arguments* in your task by their names. For example \
                         'image'. You can  also refer to the output value on the right via the name \
@@ -166,15 +175,15 @@
             name="Editor",
             margin=(15, 5, 10, 5),
         )
 
     @param.depends("value", "is_running")
     def _value_view(self):
         if not self.is_running and self.value is None:
-            return "Click Submit to generate an output"
+            return "Click RUN to generate an output"
         if self.is_running:
             return f"""Running `{self.agent=}` and `{self.model=}` on \n\n{self.task}"""
 
         return pn.Tabs(
             ("VALUE", self.get_value_pane),
             ("CODE", pn.widgets.Terminal(self.code)),
             ("EXPLANATION", self.explanation),
@@ -186,18 +195,23 @@
     def _get_last_tool(self) -> str:
         """Returns the last tool used in the code"""
         code = self.code
 
         if not code:
             return "NA"
 
-        lines = code.splitlines()
-        if "text_reader" in lines[-1]:
-            return "text_reader"
-        return ""
+        tools = ["text_reader"]
+        last_index = {code.rindex(tool): tool for tool in tools if tool in code}
+        if not last_index:
+            return ""
+
+        max_last_index = max(last_index)
+        last_tool = last_index[max_last_index]
+
+        return last_tool
 
     def get_value_pane(self):
         """Returns a converted value that can be displayed by Panel"""
         # Here we should help the agent return something that can be displayed
         value = self.value
         tool = self._get_last_tool()
```

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/PKG-INFO` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-agent-ui
-Version: 0.4.0
+Version: 0.4.1
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: awesome-panel
 Project-URL: repository, https://github.com/awesome-panel/transformers-agent-ui
 Keywords: python,huggingface,transformers,deeplearning,ai,agent,holoviz,panel
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/SOURCES.txt` & `transformers-agent-ui-0.4.1/src/transformers_agent_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

