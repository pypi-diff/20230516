# Comparing `tmp/joern_lib-0.8.3.tar.gz` & `tmp/joern_lib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.8.3.tar", max compression
+gzip compressed data, was "joern_lib-0.9.1.tar", max compression
```

## Comparing `joern_lib-0.8.3.tar` & `joern_lib-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-05-09 14:14:58.304447 joern_lib-0.8.3/LICENSE
--rw-r--r--   0        0        0     3909 2023-05-09 14:14:58.304447 joern_lib-0.8.3/README.md
--rw-r--r--   0        0        0       86 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/__init__.py
--rw-r--r--   0        0        0    10036 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/client.py
--rw-r--r--   0        0        0       61 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/detectors/c.py
--rw-r--r--   0        0        0     9414 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     2841 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/detectors/java.py
--rw-r--r--   0        0        0     3850 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/detectors/js.py
--rw-r--r--   0        0        0     2101 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/detectors/python.py
--rw-r--r--   0        0        0    18347 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/utils.py
--rw-r--r--   0        0        0     4241 2023-05-09 14:14:58.340447 joern_lib-0.8.3/joern_lib/workspace.py
--rw-r--r--   0        0        0     1261 2023-05-09 14:14:58.340447 joern_lib-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     5259 1970-01-01 00:00:00.000000 joern_lib-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-02 22:16:36.336281 joern_lib-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4469 2023-05-16 12:19:08.582377 joern_lib-0.9.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-04 21:19:10.842784 joern_lib-0.9.1/joern_lib/__init__.py
+-rw-r--r--   0        0        0    10250 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/client.py
+-rw-r--r--   0        0        0       61 2023-05-04 21:19:10.842784 joern_lib-0.9.1/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-04-28 20:22:02.075618 joern_lib-0.9.1/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0    10994 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     3294 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/detectors/java.py
+-rw-r--r--   0        0        0     3850 2023-05-09 10:38:07.751904 joern_lib-0.9.1/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0     2101 2023-05-09 10:38:07.751904 joern_lib-0.9.1/joern_lib/detectors/python.py
+-rw-r--r--   0        0        0     5529 2023-05-12 13:36:08.030864 joern_lib-0.9.1/joern_lib/graph.py
+-rw-r--r--   0        0        0    21494 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/utils.py
+-rw-r--r--   0        0        0     5476 2023-05-16 12:19:08.587376 joern_lib-0.9.1/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1566 2023-05-16 12:21:52.835913 joern_lib-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5947 1970-01-01 00:00:00.000000 joern_lib-0.9.1/PKG-INFO
```

### Comparing `joern_lib-0.8.3/LICENSE` & `joern_lib-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.3/README.md` & `joern_lib-0.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Introduction
 
-This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods are offered to perform code analysis on complex code bases without knowing [CPGQL](https://docs.joern.io/c-syntaxtree).
+This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods including integration with [NetworkX](https://networkx.org/documentation/stable/index.html) are offered to perform code analysis and research on complex code bases in a pythonic manner from cli and from notebooks.
 
 ```
 pip install joern-lib
 ```
 
 The repository includes docker compose configuration to interactively query the joern server with polynote notebooks.
 
@@ -18,14 +18,16 @@
 
 ![polynote interface](docs/sqli.jpg)
 
 ![polynote interface](docs/repl.jpg)
 
 ![polynote interface](docs/call-tree.jpg)
 
+![polynote interface](docs/pdg-dot.jpg)
+
 ## Usage
 
 Run joern server and polynote locally.
 
 ```
 git clone https://github.com/appthreat/joern-lib.git
 # Edit docker-compose.yml to set sources directory
@@ -65,15 +67,15 @@
 ```
 
 ### Workspace
 
 List workspaces
 
 ```
-res = await workspace.list(connection)
+res = await workspace.ls(connection)
 ```
 
 Get workspace path
 
 ```
 res = await workspace.get_path(connection)
 # /workspace (Response would be parsed)
@@ -198,7 +200,19 @@
 
 Adding asyncio.sleep(0) seems to fix such errors.
 
 ```
 # Workaround to fix websockets.exceptions.ConnectionClosedError
 await asyncio.sleep(0)
 ```
+
+### pygraphviz refuses to install
+
+```
+pygraphviz/graphviz_wrap.c:2711:10: fatal error: graphviz/cgraph.h: No such file or directory
+   2711 | #include "graphviz/cgraph.h"
+        |          ^~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command '/usr/bin/gcc' failed with exit code 1
+```
+
+Install `graphviz-devel` or `graphviz-dev` package for your OS. See [here](https://github.com/pygraphviz/pygraphviz/issues/155)
```

### Comparing `joern_lib-0.8.3/joern_lib/client.py` & `joern_lib-0.9.1/joern_lib/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -263,26 +263,36 @@
 
 
 async def reachableByFlows(connection, source, sink, print_result=False):
     """Execute reachableByFlows query"""
     return await df(connection, source, sink, print_result)
 
 
-async def create_cpg(connection, src, out_dir, lang):
+async def create_cpg(
+    connection, src, out_dir=None, lang=None, slice=None, slice_mode="Usages"
+):
     """Create CPG using cpggen server"""
     client = connection.cpggenclient
     if not client:
         return {
             "error": "true",
             "message": "No active connection to cpggen server. Pass the cpggen url to the client.get method.",
         }, 500
     # Suppor for url
     url = ""
-    if src.startswith("http") or src.startswith("git"):
+    if src.startswith("http") or src.startswith("git://") or src.startswith("pkg:"):
         url = src
         src = ""
+    data = {
+        "src": src,
+        "url": url,
+        "out_dir": out_dir,
+        "lang": lang,
+        "slice": "true" if slice else "false",
+        "slice_mode": slice_mode,
+    }
     response = await client.post(
         url="/cpg",
         headers=headers,
-        json={"src": src, "url": url, "out_dir": out_dir, "lang": lang},
+        json=data,
     )
     return response.json()
```

### Comparing `joern_lib-0.8.3/joern_lib/detectors/c.py` & `joern_lib-0.9.1/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.3/joern_lib/detectors/common.py` & `joern_lib-0.9.1/joern_lib/detectors/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from joern_lib import client
-from joern_lib.utils import expand_search_str
+from joern_lib import client, graph
+from joern_lib.utils import colorize_dot_data, expand_search_str
 
 
 async def list_files(connection, search_descriptor=None):
     search_str = expand_search_str(search_descriptor)
     return await client.q(connection, f"cpg.file{search_str}")
 
 
@@ -79,30 +79,61 @@
     return await client.q(connection, "cpg.member")
 
 
 async def list_metadatas(connection):
     return await client.q(connection, "cpg.metaData")
 
 
-async def list_methods(connection, search_descriptor=None, skip_operators=True):
-    search_str = expand_search_str(search_descriptor)
-    filter_str = ""
-    if skip_operators:
-        filter_str = '.whereNot(_.name(".*<operator>.*"))'
+async def nx(connection, method, graph_repr="cpg14"):
+    return await list_methods(
+        connection, search_descriptor=method, as_graph=True, graph_repr=graph_repr
+    )
+
+
+async def get_method(connection, method, as_graph=False, graph_repr="pdg"):
+    return await list_methods(
+        connection, search_descriptor=method, as_graph=as_graph, graph_repr=graph_repr
+    )
+
+
+async def is_similar(connection, M1, M2, upper_bound=500, timeout=5):
+    """Convenient method to check if two methods are similar using graph edit distance"""
+    m1g = await get_method(connection, M1, as_graph=True)
+    m2g = await get_method(connection, M2, as_graph=True)
+    if not m1g or not m2g:
+        return False
+    return graph.is_similar(m1g, m2g, upper_bound=upper_bound, timeout=timeout)
 
-    return await client.q(connection, f"""cpg.method{search_str}{filter_str}""")
+
+async def list_methods(
+    connection,
+    search_descriptor=None,
+    skip_operators=True,
+    as_graph=False,
+    graph_repr="pdg",
+):
+    if as_graph:
+        res = await export(connection, method=search_descriptor, repr=graph_repr)
+        return graph.convert_dot(res)
+    else:
+        search_str = expand_search_str(search_descriptor)
+        filter_str = ""
+        if skip_operators:
+            filter_str = '.whereNot(_.name(".*<(operator|init)>.*"))'
+        return await client.q(connection, f"""cpg.method{search_str}{filter_str}""")
 
 
 async def list_constructors(connection):
     return await client.q(connection, """cpg.method.internal.name("<init>")""")
 
 
 async def list_external_methods(connection):
     return await client.q(
-        connection, """cpg.method.isExternal(true).whereNot(_.name(".*<operator>.*"))"""
+        connection,
+        """cpg.method.isExternal(true).whereNot(_.name(".*<operator|init>.*"))""",
     )
 
 
 async def list_method_refs(connection):
     return await client.q(connection, "cpg.methodRef")
 
 
@@ -317,7 +348,22 @@
         """
         var tree = new ListBuffer[String]()
         printCallTree("%(method_name)s", tree, %(n)d)
         tree.toList.mkString("\\n")
         """
         % dict(method_name=method_name, n=n),
     )
+
+
+async def export(connection, method=None, query=None, repr="pdg", colorize=True):
+    """Method to export graph representations of a method or node"""
+    filter_str = "method"
+    if method:
+        filter_str = f"method{expand_search_str(method)}"
+    elif query:
+        filter_str = query.replace("cpg.", "")
+    res = await client.q(connection, f"""cpg.{filter_str}.dot{repr.capitalize()}""")
+    return (
+        colorize_dot_data(res)
+        if colorize
+        else (res[0] if res and len(res) == 1 else res)
+    )
```

### Comparing `joern_lib-0.8.3/joern_lib/detectors/java.py` & `joern_lib-0.9.1/joern_lib/detectors/java.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,22 +60,36 @@
     res = await client.q(
         connection,
         f"""cpg.typeDecl.where(_.annotation.fullName("{annotations}")).map(m => (m, m.annotation.l))""",
     )
     return expand_annotations(res)
 
 
+async def list_unresolved_external_methods(connection):
+    return await client.q(
+        connection,
+        """cpg.method.isExternal(true).where(_.fullName(".*<unresolved.*")).whereNot(_.name(".*<(operator|init)>.*"))""",
+    )
+
+
 async def list_methods(
-    connection, modifier="public ", include_annotations=True, external=False
+    connection,
+    modifier="public ",
+    include_annotations=True,
+    external=False,
+    unresolved=True,
 ):
     external_bool_str = "true" if external else "false"
+    filter_str = '.whereNot(_.name(".*<(operator|init)>.*"))'
+    if not unresolved:
+        filter_str = f'{filter_str}.whereNot(_.fullName(".*<unresolved.*"))'
     if include_annotations:
         res = await client.q(
             connection,
-            f"""cpg.method.isExternal({external_bool_str}).code("{modifier}.*").map(m => (m, m.annotation.l))""",
+            f"""cpg.method.isExternal({external_bool_str}){filter_str}.code("{modifier}.*").map(m => (m, m.annotation.l))""",
         )
         return expand_annotations(res)
     else:
         return await client.q(
             connection,
-            f"""cpg.method.isExternal({external_bool_str}).code("{modifier}.*")""",
+            f"""cpg.method.isExternal({external_bool_str}){filter_str}.code("{modifier}.*")""",
         )
```

### Comparing `joern_lib-0.8.3/joern_lib/detectors/js.py` & `joern_lib-0.9.1/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.3/joern_lib/detectors/python.py` & `joern_lib-0.9.1/joern_lib/detectors/python.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.8.3/joern_lib/utils.py` & `joern_lib-0.9.1/joern_lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+import base64
+
 import os
 import re
 from hashlib import blake2b
 
+import mimetypes
+
 import orjson
 from rich.console import Console
 from rich.json import JSON
 from rich.panel import Panel
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.tree import Tree
 
+mimetypes.init()
+
 console = Console(
     log_time=False,
     log_path=False,
     color_system="auto",
     width=int(os.getenv("COLUMNS", 180)),
 )
 
@@ -28,14 +34,21 @@
     "convert",
     "authenticate",
     "authorize",
     "encode",
     "encrypt",
 )
 
+JOERN_DATAFLOW_TRACKED_WIDTH = os.getenv("JOERN_DATAFLOW_TRACKED_WIDTH", 128)
+if (
+    isinstance(JOERN_DATAFLOW_TRACKED_WIDTH, str)
+    and JOERN_DATAFLOW_TRACKED_WIDTH.isdigit()
+):
+    JOERN_DATAFLOW_TRACKED_WIDTH = int(JOERN_DATAFLOW_TRACKED_WIDTH)
+
 
 def t(result, title="", caption="", language="javascript"):
     return print_table(result, title, caption, language)
 
 
 def print_table(result, title="", caption="", language="javascript"):
     table = Table(
@@ -188,17 +201,21 @@
                     (
                         loc.get("node", {})
                         .get("code", "")
                         .encode()
                         .decode("unicode_escape")
                         .strip()
                     )
+                    .replace("    ", " ")
                     .replace("\t", "")
                     .replace("\n", " ")
+                    .replace("    ", "")
                 )
+                if len(code) > JOERN_DATAFLOW_TRACKED_WIDTH:
+                    code = code[:JOERN_DATAFLOW_TRACKED_WIDTH] + " ..."
                 if code == last_code:
                     continue
                 methodFullName = loc.get("methodFullName", "").replace("<init>", "")
                 methodShortName = loc.get("methodShortName", "").replace("<init>", "")
                 class_name = loc.get("className")
                 # If there is no class name but there is a method full name try to recover
                 if not class_name and methodFullName:
@@ -423,7 +440,80 @@
 def parse_error(serr):
     """Method to parse joern output and identify friendly error messages"""
     if "No projects loaded" in serr:
         return """ERROR: Import code using import_code api. Usage: await workspace.import_code(connection, directory_name, app_name)"""
     if "No CPG loaded" in serr:
         return """ERROR: Import cpg using import_cpg or create_cpg api."""
     return serr
+
+
+def read_image(file_path):
+    """Method to read image file safely optionally converting binary formats to base64 string. Useful to render images in notebooks"""
+    if os.path.exists(file_path):
+        (mt, encoding) = mimetypes.guess_type(file_path, strict=True)
+        if mt.startswith("image/svg"):
+            with open(file_path, mode="r", encoding=encoding) as fp:
+                return fp.read()
+        if mt.startswith("image/"):
+            with open(file_path, mode="rb") as fp:
+                b = base64.b64encode(fp.read())
+                return b.decode("utf-8")
+    return None
+
+
+def colorize_dot_data(
+    dot_data,
+    scheme="paired9",
+    colors={
+        "method": "1",
+        "literal": "2",
+        "operator": "3",
+        "param": "4",
+        "identifier": "5",
+        "modifier": "6",
+        "unknown": "7",
+        "local": "7",
+        "type_ref": "8",
+        "return": "9",
+    },
+    shapes={
+        "method": "box3d",
+        "literal": "oval",
+        "operator": "box",
+        "param": "tab",
+        "identifier": "note",
+        "modifier": "rect",
+        "type_ref": "component",
+        "return": "cds",
+    },
+    style="filled",
+):
+    """
+    Method to colorize dot data with Brewer color schemes
+
+    This product includes color specifications and designs developed by Cynthia Brewer (http://colorbrewer.org/).
+    """
+    fdot_list = []
+    if dot_data and isinstance(dot_data, list):
+        for d in dot_data:
+            if "digraph" in d:
+                for k, v in colors.items():
+                    if k == "operator":
+                        d = d.replace(
+                            "label = <(&lt;operator&gt;",
+                            f"color = {v}, shape = {shapes.get('operator', 'box')}, style = {style}, label = <(&lt;operator&gt;",
+                        )
+                    else:
+                        d = d.replace(
+                            f"label = <({k.upper()},",
+                            f"color = {v}, shape = {shapes.get(k, 'ellipse')}, style = {style}, label = <({k.upper()},",
+                        )
+                # These two replacements make the string compatible with pygraphviz and pydot
+                # See https://github.com/joernio/joern/issues/2704
+                d = d.replace("label = <", "label=<")
+                afdot = d.split("\n")
+                afdot.insert(1, f"node [colorscheme={scheme}];")
+                fdot_list.append("\n".join(afdot))
+            else:
+                fdot_list.append(d)
+        return fdot_list[0] if fdot_list and len(fdot_list) == 1 else fdot_list
+    return dot_data
```

### Comparing `joern_lib-0.8.3/joern_lib/workspace.py` & `joern_lib-0.9.1/joern_lib/workspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,89 @@
+import json
 import os
 
 from joern_lib import client
 
 
 def extract_dir(res):
     if res.get("response"):
         dir_name = res.get("response").split('String = "')[-1].split('"')[0]
         return dir_name
     return None
 
 
-async def list(connection):
+async def ls(connection):
     res = await client.q(connection, "workspace")
     if "[io.joern.joerncli.console.JoernProject] = empty" in res.get("response", ""):
         return None
-    return res
+    return res.get("response")
+
+
+async def slice_cpg(
+    connection,
+    src,
+    out_dir=None,
+    languages="autodetect",
+    project_name=None,
+):
+    app_manifests = await create_cpg(
+        connection,
+        src,
+        out_dir=out_dir,
+        languages=languages,
+        project_name=project_name,
+        slice=True,
+        slice_mode="Usages",
+    )
+    if not app_manifests:
+        return None
+    if isinstance(app_manifests, (list, tuple)):
+        app_manifests = app_manifests[0]
+    if app_manifests.get("slice_out") and os.path.exists(
+        app_manifests.get("slice_out")
+    ):
+        try:
+            with open(app_manifests.get("slice_out")) as fp:
+                return json.load(fp)
+        except Exception:
+            return None
+    return None
 
 
 async def create_cpg(
-    connection, src, out_dir=None, languages="autodetect", project_name=None
+    connection,
+    src,
+    out_dir=None,
+    languages="autodetect",
+    project_name=None,
+    slice=None,
+    slice_mode="Usages",
 ):
-    if not out_dir:
-        out_dir = os.path.join(src, "cpg_out")
-    res = await client.create_cpg(connection, src, out_dir, languages)
+    app_manifests = []
+    res = await client.create_cpg(
+        connection,
+        src,
+        out_dir=out_dir,
+        lang=languages,
+        slice=slice,
+        slice_mode=slice_mode,
+    )
     if res:
-        app_manifests = res.get("app_manifests")
+        app_manifests = res.get("app_manifests", [])
         if app_manifests:
             first_app = app_manifests[0]
             if not project_name and first_app.get("app"):
                 project_name = first_app.get("app")
             cpg_path = first_app.get("cpg")
-            return await import_cpg(connection, cpg_path, project_name)
-    return False
+            res = await import_cpg(connection, cpg_path, project_name)
+            if not res:
+                return None
+    return (
+        app_manifests[0] if app_manifests and len(app_manifests) == 1 else app_manifests
+    )
 
 
 async def import_cpg(connection, cpg_path, project_name=None):
     if cpg_path:
         res = await dir_exists(connection, cpg_path)
         if not res:
             raise ValueError(
@@ -80,15 +128,15 @@
 
 async def from_string(connection, code_snippet, language="jssrc"):
     res = await client.q(
         connection, f'importCode.{language}.fromString("""{code_snippet}""")'
     )
     if isinstance(res, str):
         return False
-    if "Code successfully imported" in res.get("response", ""):
+    if res and "Code successfully imported" in res.get("response", ""):
         return True
     return False
 
 
 async def reset(connection):
     await client.q(connection, "workspace.reset")
     return True
@@ -100,36 +148,41 @@
 
 
 async def get_active_project(connection):
     return await client.q(connection, "workspace.getActiveProject")
 
 
 async def set_active_project(connection, project_name):
-    return await client.q(
+    res = await client.q(
         connection, f"""workspace.setActiveProject("{project_name}")"""
     )
+    if isinstance(res, str):
+        return False
+    if res and "projectFile = ProjectFile(inputPath =" in res.get("response", ""):
+        return True
+    return False
 
 
 async def delete_project(connection, project_name):
     return await client.q(connection, f"""workspace.deleteProject("{project_name}")""")
 
 
 async def cpg_exists(connection, project_name):
     if project_name:
         res = await client.q(connection, f"""workspace.cpgExists("{project_name}")""")
-        if "Boolean = true" in res.get("response", ""):
+        if res and "Boolean = true" in res.get("response", ""):
             return True
     return False
 
 
 async def get_overlay_dir(connection, project_name):
     res = await client.q(
         connection, f"""workspace.overlayDirByProjectName("{project_name}")"""
     )
     return extract_dir(res)
 
 
 async def dir_exists(connection, dir_name):
     res = await client.q(connection, f"""os.exists(os.Path("{dir_name}"))""")
-    if "Boolean = true" in res.get("response", ""):
+    if res and "Boolean = true" in res.get("response", ""):
         return True
     return False
```

### Comparing `joern_lib-0.8.3/pyproject.toml` & `joern_lib-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.8.3"
+version = "0.9.1"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
@@ -26,19 +26,30 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 httpx = "^0.24.0"
 websockets = "^11.0.2"
 uvloop = "^0.17.0"
 orjson = "^3.8.11"
 rich = "^13.3.5"
+networkx = {extras = ["default"], version = "^3.1"}
+pydotplus = "^2.0.2"
+pygraphviz = "^1.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
 pyinstaller = "^5.10.1"
 pdoc3 = "^0.10.0"
 
+[tool.poetry.group.science]
+optional = true
+
+[tool.poetry.group.science.dependencies]
+graphviz = {version = "^0.20.1"}
+gensim = {version = "^4.3.1"}
+networkx = {extras = ["default", "extra"], version = "^3.1"}
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `joern_lib-0.8.3/PKG-INFO` & `joern_lib-0.9.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.8.3
+Version: 0.9.1
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8.1,<3.12
@@ -20,24 +20,27 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: networkx[default] (>=3.1,<4.0)
 Requires-Dist: orjson (>=3.8.11,<4.0.0)
+Requires-Dist: pydotplus (>=2.0.2,<3.0.0)
+Requires-Dist: pygraphviz (>=1.10,<2.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: websockets (>=11.0.2,<12.0.0)
 Project-URL: Repository, https://github.com/AppThreat/joern-lib
 Description-Content-Type: text/markdown
 
 # Introduction
 
-This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods are offered to perform code analysis on complex code bases without knowing [CPGQL](https://docs.joern.io/c-syntaxtree).
+This project offers a high level python library to interact with a Joern [server](https://docs.joern.io/server). Several API methods including integration with [NetworkX](https://networkx.org/documentation/stable/index.html) are offered to perform code analysis and research on complex code bases in a pythonic manner from cli and from notebooks.
 
 ```
 pip install joern-lib
 ```
 
 The repository includes docker compose configuration to interactively query the joern server with polynote notebooks.
 
@@ -51,14 +54,16 @@
 
 ![polynote interface](docs/sqli.jpg)
 
 ![polynote interface](docs/repl.jpg)
 
 ![polynote interface](docs/call-tree.jpg)
 
+![polynote interface](docs/pdg-dot.jpg)
+
 ## Usage
 
 Run joern server and polynote locally.
 
 ```
 git clone https://github.com/appthreat/joern-lib.git
 # Edit docker-compose.yml to set sources directory
@@ -98,15 +103,15 @@
 ```
 
 ### Workspace
 
 List workspaces
 
 ```
-res = await workspace.list(connection)
+res = await workspace.ls(connection)
 ```
 
 Get workspace path
 
 ```
 res = await workspace.get_path(connection)
 # /workspace (Response would be parsed)
@@ -232,7 +237,19 @@
 Adding asyncio.sleep(0) seems to fix such errors.
 
 ```
 # Workaround to fix websockets.exceptions.ConnectionClosedError
 await asyncio.sleep(0)
 ```
 
+### pygraphviz refuses to install
+
+```
+pygraphviz/graphviz_wrap.c:2711:10: fatal error: graphviz/cgraph.h: No such file or directory
+   2711 | #include "graphviz/cgraph.h"
+        |          ^~~~~~~~~~~~~~~~~~~
+  compilation terminated.
+  error: command '/usr/bin/gcc' failed with exit code 1
+```
+
+Install `graphviz-devel` or `graphviz-dev` package for your OS. See [here](https://github.com/pygraphviz/pygraphviz/issues/155)
+
```

