# Comparing `tmp/jsx-lexer-2.0.0.tar.gz` & `tmp/jsx-lexer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsx-lexer-2.0.0.tar", last modified: Wed Jul 13 14:29:53 2022, max compression
+gzip compressed data, was "jsx-lexer-2.0.1.tar", last modified: Tue May 16 15:15:59 2023, max compression
```

## Comparing `jsx-lexer-2.0.0.tar` & `jsx-lexer-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1060 2021-03-10 15:28:09.000000 jsx-lexer-2.0.0/LICENSE
--rw-r--r--   0 flavio.curella   (502) staff       (20)      100 2022-07-13 14:16:04.000000 jsx-lexer-2.0.0/MANIFEST.in
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3298 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)     2870 2022-07-13 14:19:37.000000 jsx-lexer-2.0.0/README.rst
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/jsx/
--rw-r--r--   0 flavio.curella   (502) staff       (20)       60 2022-07-13 14:08:12.000000 jsx-lexer-2.0.0/jsx/__init__.py
--rw-r--r--   0 flavio.curella   (502) staff       (20)     1982 2022-07-13 14:08:12.000000 jsx-lexer-2.0.0/jsx/lexer.py
-drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/
--rw-r--r--   0 flavio.curella   (502) staff       (20)     3298 2022-07-13 14:29:52.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/PKG-INFO
--rw-r--r--   0 flavio.curella   (502) staff       (20)      278 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/SOURCES.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2022-07-13 14:29:52.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/dependency_links.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       37 2022-07-13 14:29:52.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/entry_points.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)       17 2022-07-13 14:29:52.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/requires.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)        4 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/jsx_lexer.egg-info/top_level.txt
--rw-r--r--   0 flavio.curella   (502) staff       (20)      336 2022-07-13 14:29:53.000000 jsx-lexer-2.0.0/setup.cfg
--rw-r--r--   0 flavio.curella   (502) staff       (20)      895 2022-07-13 14:29:19.000000 jsx-lexer-2.0.0/setup.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-16 15:15:59.984631 jsx-lexer-2.0.1/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1060 2021-03-10 15:28:09.000000 jsx-lexer-2.0.1/LICENSE
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      100 2022-07-13 14:16:04.000000 jsx-lexer-2.0.1/MANIFEST.in
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3278 2023-05-16 15:15:59.984925 jsx-lexer-2.0.1/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     2870 2022-07-13 14:19:37.000000 jsx-lexer-2.0.1/README.rst
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-16 15:15:59.977739 jsx-lexer-2.0.1/jsx/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       60 2022-07-13 14:08:12.000000 jsx-lexer-2.0.1/jsx/__init__.py
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     1812 2023-05-16 14:58:52.000000 jsx-lexer-2.0.1/jsx/lexer.py
+drwxr-xr-x   0 flavio.curella   (502) staff       (20)        0 2023-05-16 15:15:59.983460 jsx-lexer-2.0.1/jsx_lexer.egg-info/
+-rw-r--r--   0 flavio.curella   (502) staff       (20)     3278 2023-05-16 15:15:59.000000 jsx-lexer-2.0.1/jsx_lexer.egg-info/PKG-INFO
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      278 2023-05-16 15:15:59.000000 jsx-lexer-2.0.1/jsx_lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        1 2023-05-16 15:15:59.000000 jsx-lexer-2.0.1/jsx_lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       37 2023-05-16 15:15:59.000000 jsx-lexer-2.0.1/jsx_lexer.egg-info/entry_points.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)       17 2023-05-16 15:15:59.000000 jsx-lexer-2.0.1/jsx_lexer.egg-info/requires.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)        4 2023-05-16 15:15:59.000000 jsx-lexer-2.0.1/jsx_lexer.egg-info/top_level.txt
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      336 2023-05-16 15:15:59.986588 jsx-lexer-2.0.1/setup.cfg
+-rw-r--r--   0 flavio.curella   (502) staff       (20)      895 2023-05-16 15:15:02.000000 jsx-lexer-2.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsx-lexer-2.0.0/LICENSE` & `jsx-lexer-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsx-lexer-2.0.0/PKG-INFO` & `jsx-lexer-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: jsx-lexer
-Version: 2.0.0
+Version: 2.0.1
 Summary: A JSX lexer for Pygments
 Home-page: https://github.com/fcurella/jsx-lexer
 Author: Flavio Curella
 Author-email: flavio.curella@gmail.com
 License: MIT License
 Keywords: pygments highlight jsx react
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 jsx-lexer
 =========
@@ -128,9 +127,7 @@
             </div>
             );
           }
         }
     \end{minted}
 
 You can find an example of the lexer in use on Overleaf here: `https://www.overleaf.com/read/xvsytqzkvdjb`
-
-
```

### Comparing `jsx-lexer-2.0.0/README.rst` & `jsx-lexer-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `jsx-lexer-2.0.0/jsx/lexer.py` & `jsx-lexer-2.0.1/jsx/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 import re
 
-from pygments.lexer import bygroups, default, include
+from pygments.lexer import bygroups, default, include, inherit
 from pygments.lexers.javascript import JavascriptLexer
 from pygments.token import Name, Operator, Punctuation, String, Text
 
 # Use same tokens as `JavascriptLexer`, but with tags and attributes support
-TOKENS = JavascriptLexer.tokens
-TOKENS.update(
-    {
-        "jsx": [
-            (
-                r"(<)(/?)(>)",
-                bygroups(Punctuation, Punctuation, Punctuation),
-            ),  # JSXFragment <>|</>
-            (r"(<)([\w]+)(\.?)", bygroups(Punctuation, Name.Tag, Punctuation), "tag"),
-            (
-                r"(<)(/)([\w]+)(>)",
-                bygroups(Punctuation, Punctuation, Name.Tag, Punctuation),
-            ),
-            (
-                r"(<)(/)([\w]+)",
-                bygroups(Punctuation, Punctuation, Name.Tag),
-                "fragment",
-            ),  # Same for React.Context
-        ],
-        "tag": [
-            (r"\s+", Text),
-            (r"([\w-]+\s*)(=)(\s*)", bygroups(Name.Attribute, Operator, Text), "attr"),
-            (r"[{}]+", Punctuation),
-            (r"[\w\.]+", Name.Attribute),
-            (r"(/?)(\s*)(>)", bygroups(Punctuation, Text, Punctuation), "#pop"),
-        ],
-        "fragment": [
-            (r"(.)([\w]+)", bygroups(Punctuation, Name.Attribute)),
-            (r"(>)", bygroups(Punctuation), "#pop"),
-        ],
-        "attr": [
-            ("{", Punctuation, "expression"),
-            ('".*?"', String, "#pop"),
-            ("'.*?'", String, "#pop"),
-            default("#pop"),
-        ],
-        "expression": [
-            ("{", Punctuation, "#push"),
-            ("}", Punctuation, "#pop"),
-            include("root"),
-        ],
-    }
-)
-TOKENS["root"].insert(0, include("jsx"))
+TOKENS = {
+    "root": [
+        include("jsx"),
+        inherit,
+    ],
+    "jsx": [
+        (
+            r"(<)(/?)(>)",
+            bygroups(Punctuation, Punctuation, Punctuation),
+        ),  # JSXFragment <>|</>
+        (r"(<)([\w]+)(\.?)", bygroups(Punctuation, Name.Tag, Punctuation), "tag"),
+        (
+            r"(<)(/)([\w]+)(>)",
+            bygroups(Punctuation, Punctuation, Name.Tag, Punctuation),
+        ),
+        (
+            r"(<)(/)([\w]+)",
+            bygroups(Punctuation, Punctuation, Name.Tag),
+            "fragment",
+        ),  # Same for React.Context
+    ],
+    "tag": [
+        (r"\s+", Text),
+        (r"([\w-]+\s*)(=)(\s*)", bygroups(Name.Attribute, Operator, Text), "attr"),
+        (r"[{}]+", Punctuation),
+        (r"[\w\.]+", Name.Attribute),
+        (r"(/?)(\s*)(>)", bygroups(Punctuation, Text, Punctuation), "#pop"),
+    ],
+    "fragment": [
+        (r"(.)([\w]+)", bygroups(Punctuation, Name.Attribute)),
+        (r"(>)", bygroups(Punctuation), "#pop"),
+    ],
+    "attr": [
+        ("{", Punctuation, "expression"),
+        ('".*?"', String, "#pop"),
+        ("'.*?'", String, "#pop"),
+        default("#pop"),
+    ],
+    "expression": [
+        ("{", Punctuation, "#push"),
+        ("}", Punctuation, "#pop"),
+        include("root"),
+    ],
+}
 
 
 class JsxLexer(JavascriptLexer):
     name = "react"
     aliases = ["jsx", "react"]
     filenames = ["*.jsx", "*.react"]
     mimetypes = ["text/jsx", "text/typescript-jsx"]
```

### Comparing `jsx-lexer-2.0.0/jsx_lexer.egg-info/PKG-INFO` & `jsx-lexer-2.0.1/jsx_lexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: jsx-lexer
-Version: 2.0.0
+Version: 2.0.1
 Summary: A JSX lexer for Pygments
 Home-page: https://github.com/fcurella/jsx-lexer
 Author: Flavio Curella
 Author-email: flavio.curella@gmail.com
 License: MIT License
 Keywords: pygments highlight jsx react
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 jsx-lexer
 =========
@@ -128,9 +127,7 @@
             </div>
             );
           }
         }
     \end{minted}
 
 You can find an example of the lexer in use on Overleaf here: `https://www.overleaf.com/read/xvsytqzkvdjb`
-
-
```

### Comparing `jsx-lexer-2.0.0/setup.py` & `jsx-lexer-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import os
 
 from setuptools import find_packages, setup
 
-VERSION = "2.0.0"
+VERSION = "2.0.1"
 here = os.path.abspath(os.path.dirname(__file__))
 README = io.open(os.path.join(here, "README.rst"), encoding="utf8").read()
 
 setup(
     name="jsx-lexer",
     description="A JSX lexer for Pygments",
     long_description=README,
```

