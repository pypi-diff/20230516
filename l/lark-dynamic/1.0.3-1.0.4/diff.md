# Comparing `tmp/lark_dynamic-1.0.3.tar.gz` & `tmp/lark_dynamic-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lark_dynamic-1.0.3.tar", last modified: Sun Jun 26 14:36:32 2022, max compression
+gzip compressed data, was "dist\lark_dynamic-1.0.4.tar", last modified: Sun Jun 26 15:47:33 2022, max compression
```

## Comparing `lark_dynamic-1.0.3.tar` & `lark_dynamic-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-06-26 14:36:32.280053 lark_dynamic-1.0.3/
--rw-rw-rw-   0        0        0    14711 2022-06-26 14:36:32.279053 lark_dynamic-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    10941 2022-06-26 14:35:21.000000 lark_dynamic-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-06-26 14:36:32.279053 lark_dynamic-1.0.3/lark_dynamic.egg-info/
--rw-rw-rw-   0        0        0    14711 2022-06-26 14:36:32.000000 lark_dynamic-1.0.3/lark_dynamic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2022-06-26 14:36:32.000000 lark_dynamic-1.0.3/lark_dynamic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-26 14:36:32.000000 lark_dynamic-1.0.3/lark_dynamic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-06-26 14:36:32.000000 lark_dynamic-1.0.3/lark_dynamic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-06-26 14:36:32.000000 lark_dynamic-1.0.3/lark_dynamic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13795 2022-06-26 14:35:18.000000 lark_dynamic-1.0.3/lark_dynamic.py
--rw-rw-rw-   0        0        0       42 2022-06-26 14:36:32.280053 lark_dynamic-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      932 2022-06-26 14:35:39.000000 lark_dynamic-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-26 15:47:33.109653 lark_dynamic-1.0.4/
+-rw-rw-rw-   0        0        0    17545 2022-06-26 15:47:33.109653 lark_dynamic-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12727 2022-06-26 15:46:58.000000 lark_dynamic-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2022-06-26 15:47:33.108652 lark_dynamic-1.0.4/lark_dynamic.egg-info/
+-rw-rw-rw-   0        0        0    17545 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15308 2022-06-26 15:39:47.000000 lark_dynamic-1.0.4/lark_dynamic.py
+-rw-rw-rw-   0        0        0       42 2022-06-26 15:47:33.109653 lark_dynamic-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      932 2022-06-26 15:47:03.000000 lark_dynamic-1.0.4/setup.py
```

### Comparing `lark_dynamic-1.0.3/PKG-INFO` & `lark_dynamic-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lark_dynamic
-Version: 1.0.3
+Version: 1.0.4
 Summary: Dynamic grammar generator for Lark parsing toolkit
 Home-page: https://github.com/courage-py/lark-dynamic
 Author: evtn
 Author-email: courage@evtn.ru
 License: MIT
 Description: Dynamic grammar generator for [Lark parsing toolkit](https://github.com/lark-parser/lark)
         
@@ -420,12 +420,143 @@
         DIGIT: NONZERO | "0"
         NONZERO: "1".."9"
         INTEGER: NONZERO ( DIGIT )*
         FLOAT.2: ( INTEGER "." ( DIGIT )* ) | ( "." ( DIGIT )+ )
         
         number: INTEGER -> integer | FLOAT -> float
         ```
+        
+        
+        # Advanced usage
+        
+        `Grammar` object can be edited after its creation.
+        
+        First, you need to get a grammar wrapper: `wrapper = grammar.use_wrapper()`
+        
+        
+        ## Get a definition
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     "Hello"
+        # )
+        
+        ``` 
+        
+        ## Replace definition contents
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        wrapper.replace("HELLO", "World")
+        
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     "World"
+        # )
+        
+        ``` 
+        
+        ## Edit definition
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        wrapper.edit("HELLO", priority=10)
+        
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     "World"
+        # )
+        
+        ``` 
+        
+        ## Extend definition
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        wrapper.extend("HELLO", "World")
+        
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     Option(
+        #         "Hello"
+        #         "World"
+        #     )
+        # )
+        
+        ``` 
+        
+        ## Getting all definitions / directives
+        
+        You can get dictionaries with rules, terminals, templates, or a list of all directives with a wrapper:
+        
+        ```python
+        
+        g = Grammar()
+        wrapper = g.use_wrapper()
+        
+        wrapper.rules
+        wrapper.terminals
+        wrapper.templates
+        wrapper.directives
+        ```
+        
+        
+        ## Why a wrapper?
+        
+        Because grammar object itself is used to create definitions with arbitrary names. Creating methods with common names would easily create a problem:
+        
+        
+        ```python
+        g = Grammar()
+        
+        g.edit = "EDIT", Some("blah")
+        g.save = "SAVE", Some(Option("lorem", "ipsum", "dolor", "sit", "amet"))
+        
+        g.command = Option(g.edit, g.save) # g.edit used here as a rule, not method
+        
+        ```
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `lark_dynamic-1.0.3/README.md` & `lark_dynamic-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -411,8 +411,138 @@
 ```
 DIGIT: NONZERO | "0"
 NONZERO: "1".."9"
 INTEGER: NONZERO ( DIGIT )*
 FLOAT.2: ( INTEGER "." ( DIGIT )* ) | ( "." ( DIGIT )+ )
 
 number: INTEGER -> integer | FLOAT -> float
-```
+```
+
+
+# Advanced usage
+
+`Grammar` object can be edited after its creation.
+
+First, you need to get a grammar wrapper: `wrapper = grammar.use_wrapper()`
+
+
+## Get a definition
+
+
+```python
+
+g = Grammar()
+
+
+g.HELLO = "Hello"
+
+wrapper = g.use_wrapper()
+
+print(wrapper.get_def("HELLO")) 
+
+# prints
+# RuleDef(
+#     "Hello"
+# )
+
+``` 
+
+## Replace definition contents
+
+
+```python
+
+g = Grammar()
+
+g.HELLO = "Hello"
+
+wrapper = g.use_wrapper()
+wrapper.replace("HELLO", "World")
+
+
+print(wrapper.get_def("HELLO")) 
+
+# prints
+# RuleDef(
+#     "World"
+# )
+
+``` 
+
+## Edit definition
+
+
+```python
+
+g = Grammar()
+
+g.HELLO = "Hello"
+
+wrapper = g.use_wrapper()
+wrapper.edit("HELLO", priority=10)
+
+
+print(wrapper.get_def("HELLO")) 
+
+# prints
+# RuleDef(
+#     "World"
+# )
+
+``` 
+
+## Extend definition
+
+
+```python
+
+g = Grammar()
+
+g.HELLO = "Hello"
+
+wrapper = g.use_wrapper()
+wrapper.extend("HELLO", "World")
+
+
+print(wrapper.get_def("HELLO")) 
+
+# prints
+# RuleDef(
+#     Option(
+#         "Hello"
+#         "World"
+#     )
+# )
+
+``` 
+
+## Getting all definitions / directives
+
+You can get dictionaries with rules, terminals, templates, or a list of all directives with a wrapper:
+
+```python
+
+g = Grammar()
+wrapper = g.use_wrapper()
+
+wrapper.rules
+wrapper.terminals
+wrapper.templates
+wrapper.directives
+```
+
+
+## Why a wrapper?
+
+Because grammar object itself is used to create definitions with arbitrary names. Creating methods with common names would easily create a problem:
+
+
+```python
+g = Grammar()
+
+g.edit = "EDIT", Some("blah")
+g.save = "SAVE", Some(Option("lorem", "ipsum", "dolor", "sit", "amet"))
+
+g.command = Option(g.edit, g.save) # g.edit used here as a rule, not method
+
+```
+
```

### Comparing `lark_dynamic-1.0.3/lark_dynamic.egg-info/PKG-INFO` & `lark_dynamic-1.0.4/lark_dynamic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lark-dynamic
-Version: 1.0.3
+Version: 1.0.4
 Summary: Dynamic grammar generator for Lark parsing toolkit
 Home-page: https://github.com/courage-py/lark-dynamic
 Author: evtn
 Author-email: courage@evtn.ru
 License: MIT
 Description: Dynamic grammar generator for [Lark parsing toolkit](https://github.com/lark-parser/lark)
         
@@ -420,12 +420,143 @@
         DIGIT: NONZERO | "0"
         NONZERO: "1".."9"
         INTEGER: NONZERO ( DIGIT )*
         FLOAT.2: ( INTEGER "." ( DIGIT )* ) | ( "." ( DIGIT )+ )
         
         number: INTEGER -> integer | FLOAT -> float
         ```
+        
+        
+        # Advanced usage
+        
+        `Grammar` object can be edited after its creation.
+        
+        First, you need to get a grammar wrapper: `wrapper = grammar.use_wrapper()`
+        
+        
+        ## Get a definition
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     "Hello"
+        # )
+        
+        ``` 
+        
+        ## Replace definition contents
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        wrapper.replace("HELLO", "World")
+        
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     "World"
+        # )
+        
+        ``` 
+        
+        ## Edit definition
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        wrapper.edit("HELLO", priority=10)
+        
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     "World"
+        # )
+        
+        ``` 
+        
+        ## Extend definition
+        
+        
+        ```python
+        
+        g = Grammar()
+        
+        g.HELLO = "Hello"
+        
+        wrapper = g.use_wrapper()
+        wrapper.extend("HELLO", "World")
+        
+        
+        print(wrapper.get_def("HELLO")) 
+        
+        # prints
+        # RuleDef(
+        #     Option(
+        #         "Hello"
+        #         "World"
+        #     )
+        # )
+        
+        ``` 
+        
+        ## Getting all definitions / directives
+        
+        You can get dictionaries with rules, terminals, templates, or a list of all directives with a wrapper:
+        
+        ```python
+        
+        g = Grammar()
+        wrapper = g.use_wrapper()
+        
+        wrapper.rules
+        wrapper.terminals
+        wrapper.templates
+        wrapper.directives
+        ```
+        
+        
+        ## Why a wrapper?
+        
+        Because grammar object itself is used to create definitions with arbitrary names. Creating methods with common names would easily create a problem:
+        
+        
+        ```python
+        g = Grammar()
+        
+        g.edit = "EDIT", Some("blah")
+        g.save = "SAVE", Some(Option("lorem", "ipsum", "dolor", "sit", "amet"))
+        
+        g.command = Option(g.edit, g.save) # g.edit used here as a rule, not method
+        
+        ```
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `lark_dynamic-1.0.3/lark_dynamic.py` & `lark_dynamic-1.0.4/lark_dynamic.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 
 class Grammar:
     def __init__(self):
         self.__rules = {}
         self.__terminals = {}
         self.__directives = []
         self.__templates = {}
+        self.__wrapper = GrammarWrapper(self)
 
     def generate(self, **context):
-        return "".join(self.iter(context)).strip()
+        return "".join(self.build_grammar(context)).strip()
 
-    def iter(self, context):
+    def build_grammar(self, context):
         for terminal in self.__terminals.values():
             yield from terminal.render(context)
             yield "\n"
         yield "\n"
         for rule in self.__rules.values():
             yield from rule.render(context)
             yield "\n"
@@ -37,25 +38,24 @@
             yield from directive.render(context)
             yield "\n"
         for template in self.__templates.values():
             yield from template.render(context)
             yield "\n"
         yield "\n"
 
-    def make_rule(self, name, tokens, modifier="", priority=1):
+    def make_rule(self, name, tokens, modifier="", priority=1, replace=False):
         if not is_rule(name):
             raise ValueError(
                 f"Invalid rule name: '{name}'. Rule names must only contain chars [a-z0-9_] and cannot start with a digit"
             )
-        if name in self.__rules:
+        if name in self.__rules and not replace:
             raise NameError(f"Rule '{name}' already exists")
         if isinstance(tokens, Modifier):
             tokens, modifier = tokens.tokens, tokens.type
-        if not isinstance(tokens, (tuple, list)):
-            tokens = (tokens,)
+
         ruledef = RuleDef(name, tokens, modifier, priority)
         self.__rules[name] = ruledef
         return ruledef
 
     def make_terminal(self, name, tokens, modifier="", priority=1):
         if not is_term(name):
             raise ValueError(
@@ -63,17 +63,14 @@
             )
         if name in self.__terminals:
             raise NameError(f"Terminal '{name}' already exists")
 
         if isinstance(tokens, Modifier):
             tokens, modifier = tokens.tokens, tokens.type
 
-        if not isinstance(tokens, (tuple, list)):
-            tokens = (tokens,)
-
         termdef = TerminalDef(name, tokens, modifier, priority)
         self.__terminals[name] = termdef
         return termdef
 
     def make_directive(self, name, content):
         directivedef = DirectiveDef(name, content)
         self.__directives.append(directivedef)
@@ -110,14 +107,59 @@
             [
                 *[repr(rule) for rule in self.__rules.values()],
                 *[repr(term) for term in self.__terminals.values()],
                 *[repr(directive) for directive in self.__directives],
             ]
         )
 
+    def use_wrapper(self):
+        return self.__wrapper
+
+
+class GrammarWrapper:
+    def __init__(self, grammar):
+        self.grammar = grammar
+
+    def get_def(self, key):
+        return (
+            self.rules.get(key) 
+            or self.terminals.get(key) 
+            or self.templates.get(key)
+        )
+
+    @property
+    def rules(self):
+        return self.grammar.__rules
+
+    @property
+    def terminals(self):
+        return self.grammar.__terminals
+
+    @property
+    def templates(self):
+        return self.grammar.__terminals
+
+    @property
+    def directives(self):
+        return self.grammar.__directives
+
+    def extend(self, key, *alternatives):
+        definition = self.get_def(key)
+        definition.tokens = (Option(definition.tokens, *alternatives), )
+
+    def replace(self, key, tokens):
+        self.get_def(key).tokens = tokens
+
+    def edit(self, key, modifier=None, priority=None):
+        definition = self.get_def(key)
+        if modifier is not None:
+            definition.modifier = modifier.type
+        if priority is not None:
+            definition.priority = priority
+
 
 class Modifier:
     def __init__(self, type_, *tokens):
         self.type = type_
         self.tokens = tokens
 
     def __call__(self, *tokens):
@@ -165,14 +207,16 @@
     def __ror__(self, other):
         return Option(other, self)
 
 
 class Definition(Token):
     def __init__(self, name, tokens, modifier="", priority=1):
         self.name = name
+        if not isinstance(tokens, tuple):
+            tokens = (tokens, )
         self.tokens = tokens
         self.modifier = modifier
         self.priority = priority
 
     def render(self, context):
         yield self.modifier
         yield self.name
@@ -329,30 +373,42 @@
         yield from Token.render_str(self.token, context)
         yield " "
         yield from Group(self.sep, self.token).render(context)
         yield "*"
         yield ")"
 
     def repr_children(self):
-        return "".join([repr(self.token), " (", '","', repr(self.token), ")*"])
+        return "".join([repr(self.token), " (", repr(self.sep), repr(self.token), ")*"])
 
 
 class Repeat(Token):
     def __init__(self, content, number_or_range):
         self.content = content
         self.number_or_range = number_or_range
 
     def render(self, context):
         yield from Group(self.content).render(context)
         yield " ~ "
+        yield from self.render_range()
+
+    def render_range(self):
+        if not self.number_or_range:
+            raise ValueError("Cannot create a range of 0 occurences")
+
         if isinstance(self.number_or_range, (list, tuple)):
-            yield "..".join(map(str, self.number_or_range))
+            for n in range(len(self.number_or_range) - 1):
+                yield str(n)
+                yield ".."
+            yield str(self.number_or_range[-1])
         else:
             yield str(self.number_or_range)
 
+    def repr_children(self):
+        return "".join([repr(self.content), " ~ ", *self.render_range()])
+
 
 class Literal(Token):
     def __init__(self, string: str, flags=""):
         self.string = string
         self.flags = flags
 
     def render(self, context):
```

### Comparing `lark_dynamic-1.0.3/setup.py` & `lark_dynamic-1.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ]
 
     title = "lark_dynamic"
     description = "Dynamic grammar generator for Lark parsing toolkit"
-    version = "1.0.3"
+    version = "1.0.4"
     author = "evtn"
     author_email = "courage@evtn.ru"
     license = "MIT"
     url = "https://github.com/courage-py/lark-dynamic"
 
 
 with open("README.md") as file:
```

