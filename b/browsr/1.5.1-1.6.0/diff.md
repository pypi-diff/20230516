# Comparing `tmp/browsr-1.5.1.tar.gz` & `tmp/browsr-1.6.0.tar.gz`

## Comparing `browsr-1.5.1.tar` & `browsr-1.6.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.5.1/.releaserc.js
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 browsr-1.5.1/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.5.1/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/__main__.py
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_base.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_cli.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_config.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/_version.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/browsr.css
--rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 browsr-1.5.1/browsr/browsr.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/contributing.md
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/index.md
--rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/browsr.png
--rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/browsr_no_label.png
--rw-r--r--   0        0        0  1112808 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_datatable.png
--rw-r--r--   0        0        0   838657 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_markdown.png
--rw-r--r--   0        0        0  1550033 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_mona_lisa.png
--rw-r--r--   0        0        0  1031902 2020-02-02 00:00:00.000000 browsr-1.5.1/docs/_static/screenshot_utils.png
--rw-r--r--   0        0        0   124300 2020-02-02 00:00:00.000000 browsr-1.5.1/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.5.1/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.5.1/tests/conftest.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.5.1/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.5.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.5.1/LICENSE
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 browsr-1.5.1/README.md
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 browsr-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 browsr-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.6.0/.releaserc.js
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 browsr-1.6.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.6.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/__main__.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_base.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_cli.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_config.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_tools.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/_version.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/browsr.css
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/browsr.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 browsr-1.6.0/browsr/universal_directory_tree.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/contributing.md
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/index.md
+-rw-r--r--   0        0        0   297863 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/browsr.png
+-rw-r--r--   0        0        0   265046 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/browsr_no_label.png
+-rw-r--r--   0        0        0  2345036 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_datatable.png
+-rw-r--r--   0        0        0  1798671 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_markdown.png
+-rw-r--r--   0        0        0  2487884 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_mona_lisa.png
+-rw-r--r--   0        0        0  2059371 2020-02-02 00:00:00.000000 browsr-1.6.0/docs/_static/screenshot_utils.png
+-rw-r--r--   0        0        0   124300 2020-02-02 00:00:00.000000 browsr-1.6.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82506 2020-02-02 00:00:00.000000 browsr-1.6.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 browsr-1.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 browsr-1.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 browsr-1.6.0/README.md
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 browsr-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 browsr-1.6.0/PKG-INFO
```

### Comparing `browsr-1.5.1/.pre-commit-config.yaml` & `browsr-1.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/.releaserc.js` & `browsr-1.6.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/mkdocs.yaml` & `browsr-1.6.0/mkdocs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -67,7 +67,8 @@
               python:
                   import:
                       - https://docs.python.org/3/objects.inv
                       - https://numpy.org/doc/stable/objects.inv
                       - https://pandas.pydata.org/docs/objects.inv
                   options:
                       docstring_style: numpy
+                      filters: []
```

### Comparing `browsr-1.5.1/.github/semantic_release/package-lock.json` & `browsr-1.6.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/.github/semantic_release/release_notes.hbs` & `browsr-1.6.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/.github/workflows/lint.yaml` & `browsr-1.6.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/.github/workflows/publish.yaml` & `browsr-1.6.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/.github/workflows/release.yaml` & `browsr-1.6.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/.github/workflows/tests.yaml` & `browsr-1.6.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/browsr/_base.py` & `browsr-1.6.0/browsr/_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 
 from __future__ import annotations
 
 import math
 import pathlib
 from dataclasses import dataclass
 from textwrap import dedent
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import numpy as np
 import upath
 from pandas import DataFrame
 from rich import traceback
 from rich.console import RenderableType
 from rich.markdown import Markdown
 from rich.text import Text
 from textual.app import App, ComposeResult
 from textual.containers import Container
 from textual.reactive import reactive, var
 from textual.widget import Widget
-from textual.widgets import Button, DataTable, DirectoryTree, Static
-from textual.widgets._directory_tree import DirEntry
-from textual.widgets._tree import TreeNode
-from upath import UPath
+from textual.widgets import Button, DataTable, Static
 
 from browsr._config import favorite_themes
 from browsr._utils import FileInfo
 
 
 @dataclass
 class TextualAppContext:
@@ -121,58 +118,14 @@
         for index, value_list in enumerate(pandas_dataframe.values.tolist()):
             row = [str(index)] if show_index else []
             row += [str(x) for x in value_list]
             table.add_row(*row)
         return table
 
 
-class UniversalDirectoryTree(DirectoryTree):
-    """
-    A Universal DirectoryTree supporting different filesystems
-    """
-
-    def load_directory(self, node: TreeNode[DirEntry]) -> None:
-        """
-        Load Directory Using Universal Pathlib
-        """
-        assert node.data is not None
-        dir_path = UPath(node.data.path)
-        node.data.loaded = True
-        top_level_buckets = self._handle_top_level_bucket(dir_path=dir_path)
-        if top_level_buckets is None:
-            directory = sorted(
-                dir_path.iterdir(),
-                key=lambda x: (not x.is_dir(), x.name.lower()),
-            )
-        for path in top_level_buckets or directory:
-            if top_level_buckets is None:
-                path_name = path.name
-            else:
-                path_name = str(path).replace("s3://", "").rstrip("/")
-            node.add(
-                path_name,
-                data=DirEntry(str(path), path.is_dir()),
-                allow_expand=path.is_dir(),
-            )
-        node.expand()
-
-    def _handle_top_level_bucket(self, dir_path: UPath) -> Optional[Iterable[UPath]]:
-        """
-        Handle scenarios when someone wants to browse all of s3
-
-        This is because S3FS handles the root directory differently than other filesystems
-        """
-        if str(dir_path) == "s3:/":
-            sub_buckets = sorted(
-                UPath(f"s3://{bucket.name}") for bucket in dir_path.iterdir()
-            )
-            return sub_buckets
-        return None
-
-
 class FileSizeError(Exception):
     """
     File Too Large Error
     """
 
 
 class CurrentFileInfoBar(Widget):
@@ -201,48 +154,38 @@
         if size_bytes == 0:
             return " 0B"
         size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
         index = int(math.floor(math.log(size_bytes, 1024)))
         p = math.pow(1024, index)
         number = round(size_bytes / p, 2)
         unit = size_name[index]
-        return f"{round(number, 0)}{unit}"
+        return f"{number:.0f}{unit}"
 
     def render(self) -> RenderableType:
         """
         Render the Current File Info Bar
         """
         if self.file_info is None or not self.file_info.is_file:
             return Text("")
         modify_time = self.file_info.last_modified.strftime("%b, %-d %Y %I:%M %p")
-        assembled = [
-            "🗄️️️  ",
-            self._convert_size(self.file_info.size),
-            "   📅️  ",
-            modify_time,
-            "  💾  ",
-            self.file_info.file.name,
-            "  📂  ",
-            self.file_info.file.parent.name,
-        ]
+        status_string = (
+            "🗄️️️  "
+            + self._convert_size(self.file_info.size)
+            + "   📅️  "
+            + modify_time
+            + "  💾  "
+            + self.file_info.file.name
+            + "  📂  "
+            + self.file_info.file.parent.name
+        )
         if self.file_info.owner not in ["", None]:
-            assembled += [
-                "  👤  ",
-                self.file_info.owner,
-            ]
+            status_string += "  👤  " + self.file_info.owner
         if self.file_info.group.strip() not in ["", None]:
-            assembled += [
-                "  🏠  ",
-                self.file_info.group,
-            ]
-        assembled += [
-            "  ∙ ",
-        ]
-        dim_text = [Text(item, style="dim") for item in assembled]
-        return Text.assemble(*dim_text)
+            status_string += "  🏠  " + self.file_info.group
+        return Text(status_string, style="dim")
 
 
 class ConfirmationPopUp(Container):
     """
     A Pop Up that asks for confirmation
     """
```

### Comparing `browsr-1.5.1/browsr/_cli.py` & `browsr-1.6.0/browsr/_cli.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/browsr/_config.py` & `browsr-1.6.0/browsr/_config.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/browsr/_utils.py` & `browsr-1.6.0/browsr/_utils.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/browsr/browsr.css` & `browsr-1.6.0/browsr/browsr.css`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     margin-bottom: 1;
     background: $accent-darken-3;
     color: $text;
     height: 1;
 }
 
 CurrentFileInfoBar {
-    width: auto;
+    width: 100%;
 }
 
 #confirmation-container {
     width: 100%;
     height: 100%;
     align: center middle;
 }
```

### Comparing `browsr-1.5.1/browsr/browsr.py` & `browsr-1.6.0/browsr/browsr.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 from rich.syntax import Syntax
 from rich.traceback import Traceback
 from rich_pixels import Pixels
 from textual.binding import Binding
 from textual.containers import Container, Horizontal, VerticalScroll
 from textual.reactive import var
 from textual.widget import Widget
-from textual.widgets import DataTable, DirectoryTree, Footer, Header, Static
+from textual.widgets import DataTable, Footer, Header, Static
 from upath.implementations.cloud import CloudPath
 
 from browsr._base import (
     BrowsrTextualApp,
     ConfirmationPopUp,
     CurrentFileInfoBar,
     FileSizeError,
     TextualAppContext,
-    UniversalDirectoryTree,
 )
 from browsr._config import favorite_themes, image_file_extensions
 from browsr._utils import (
     FileInfo,
     get_file_info,
     handle_duplicate_filenames,
     open_image,
 )
 from browsr._version import __application__
+from browsr.universal_directory_tree import UniversalDirectoryTree
 
 
 class Browsr(BrowsrTextualApp):
     """
     Textual code browser app.
     """
 
@@ -261,16 +261,16 @@
             self.render_code_page(file_path=self.selected_file_path)
         else:
             self.show_tree = True
             self.render_code_page(
                 file_path=pathlib.Path.cwd(), content=__application__.upper()
             )
 
-    def on_directory_tree_file_selected(
-        self, event: DirectoryTree.FileSelected
+    def on_universal_directory_tree_file_selected(
+        self, event: UniversalDirectoryTree.FileSelected
     ) -> None:
         """
         Called when the user click a file in the directory tree.
         """
         self.selected_file_path = upath.UPath(event.path)
         file_info = get_file_info(file_path=self.selected_file_path)
         self.render_code_page(file_path=upath.UPath(event.path))
@@ -350,7 +350,13 @@
                 """
             )
             self.confirmation.download_message.update(Markdown(prompt_message))
             self.confirmation.refresh()
             self.hidden_table_view = self.table_view.display
             self.table_view.display = False
             self.confirmation_window.display = True
+
+
+app = Browsr(config_object=TextualAppContext(file_path=None, debug=True))
+
+if __name__ == "__main__":
+    app.run()
```

### Comparing `browsr-1.5.1/docs/contributing.md` & `browsr-1.6.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/docs/gen_ref_pages.py` & `browsr-1.6.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/docs/index.md` & `browsr-1.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,38 @@
 # browsr
 
-<div align="center">
-    <picture>
-        <img src=https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/browsr.png
-             width="400" alt="browsr">
-    </picture>
+<div align="center" href="https://github.com/juftin/browsr">
+    <a href="https://github.com/juftin/browsr">
+      <img src=https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/browsr.png
+        width="400" alt="browsr">
+    </a>
 </div>
 
 [![browsr Version](https://img.shields.io/pypi/v/browsr?color=blue&label=browsr)](https://github.com/juftin/browsr)
 [![PyPI](https://img.shields.io/pypi/pyversions/browsr)](https://pypi.python.org/pypi/browsr/)
 [![Testing Status](https://github.com/juftin/browsr/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/workflows/tests.yaml?query=branch%3Amain)
 [![GitHub License](https://img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://github.com/juftin/browsr/blob/main/LICENSE)
 
 **`browsr`** is a TUI (text-based user interface) file browser for your terminal.
 It's a simple way to browse your files and take a peek at their contents. Plus it
 works on local and remote file systems.
 
-<style>
-  .grid-item {
-    transition: all 0.5s ease;
-  }
-
-  .grid-item:hover {
-    transform: scale(1.2);
-  }
-
-  .expanded {
-    position: fixed;
-    top: 0;
-    left: 0;
-    width: 100%;
-    height: 100%;
-    background-color: rgba(0, 0, 0, 0.9);
-    display: flex;
-    align-items: center;
-    justify-content: center;
-    z-index: 9999;
-  }
-
-  .expanded img {
-    max-width: 80%;
-    max-height: 80%;
-    object-fit: contain;
-  }
-</style>
+<details open></summary></summary>
 
 <body>
-  <div class="grid" style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
-    <div class="grid-item">
-      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png" alt="Image 1">
-    </div>
-    <div class="grid-item">
-      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_datatable.png" alt="Image 2">
-    </div>
-    <div class="grid-item">
-      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_mona_lisa.png" alt="Image 3">
-    </div>
-    <div class="grid-item">
-      <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_markdown.png" alt="Image 4">
-    </div>
-  </div>
-
-  <div class="expanded" style="display: none;">
-    <img src="">
-  </div>
-
-  <script>
-    var expanded = document.querySelector('.expanded');
-    expanded.onclick = function() {
-      this.style.display = 'none';
-    };
-  </script>
+<div style="display: grid; grid-template-columns: repeat(2, 1fr); grid-gap: 10px;">
+    <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_utils.png" alt="Image 1">
+    <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_datatable.png" alt="Image 2">
+    <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_mona_lisa.png" alt="Image 3">
+    <img src="https://raw.githubusercontent.com/juftin/browsr/main/docs/_static/screenshot_markdown.png" alt="Image 4">
+</div>
 </body>
 
+</details>
+
 ## Installation
 
 The below command recommends [pipx](https://pypa.github.io/pipx/) instead of pip. `pipx` installs the package in
 an isolated environment and makes it easy to uninstall. If you'd like to use `pip` instead, just replace `pipx`
 with `pip` in the below command.
 
 ```shell
@@ -101,7 +57,13 @@
 
 Simply give **`browsr`** a path to a file/directory and it will open a browser window
 with a file browser. You can also give it a URL to a remote file system, like AWS S3.
 
 ```shell
 browsr s3://my-bucket/my-file.parquet
 ```
+
+### [Check out the Documentation](https://juftin.com/browsr/) for more
+
+## License
+
+**`browsr`** is distributed under the terms of the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -7,24 +7,22 @@
 tests.yaml/badge.svg?branch=main)](https://github.com/juftin/browsr/actions/
 workflows/tests.yaml?query=branch%3Amain) [![GitHub License](https://
 img.shields.io/github/license/juftin/browsr?color=blue&label=License)](https://
 github.com/juftin/browsr/blob/main/LICENSE) **`browsr`** is a TUI (text-based
 user interface) file browser for your terminal. It's a simple way to browse
 your files and take a peek at their contents. Plus it works on local and remote
 file systems.
-[Image 1]
-[Image 2]
-[Image 3]
-[Image 4]
-[Image]
-## Installation The below command recommends [pipx](https://pypa.github.io/
+[Image 1] [Image 2] [Image 3] [Image 4]
+ ## Installation The below command recommends [pipx](https://pypa.github.io/
 pipx/) instead of pip. `pipx` installs the package in an isolated environment
 and makes it easy to uninstall. If you'd like to use `pip` instead, just
 replace `pipx` with `pip` in the below command. ```shell pipx install browsr
 ``` ## Extra Installation If you're looking to use **`browsr`** on remote file
 systems, like AWS S3, you'll need to install the `remote` extra. If you'd like
 to browse parquet files, you'll need to install the `parquet` extra. Or, even
 simpler, you can install the `all` extra to get all the extras. ```shell pipx
 install "browsr[all]" ``` ## Usage ```shell browsr ~/Downloads/ ``` Simply give
 **`browsr`** a path to a file/directory and it will open a browser window with
 a file browser. You can also give it a URL to a remote file system, like AWS
-S3. ```shell browsr s3://my-bucket/my-file.parquet ```
+S3. ```shell browsr s3://my-bucket/my-file.parquet ``` ### [Check out the
+Documentation](https://juftin.com/browsr/) for more ## License **`browsr`** is
+distributed under the terms of the [MIT license](LICENSE).
```

### Comparing `browsr-1.5.1/docs/_static/browsr.png` & `browsr-1.6.0/docs/_static/browsr.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/docs/_static/browsr_no_label.png` & `browsr-1.6.0/docs/_static/browsr_no_label.png`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/requirements/requirements-dev.txt` & `browsr-1.6.0/requirements/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1511,17 +1511,17 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual[dev]==0.22.3 \
-    --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
-    --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
+textual[dev]==0.24.1 \
+    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
+    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
     # via -r requirements.in
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   black
     #   build
```

### Comparing `browsr-1.5.1/requirements/requirements-prod.txt` & `browsr-1.6.0/requirements/requirements-prod.txt`

 * *Files 0% similar despite different names*

```diff
@@ -961,17 +961,17 @@
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   azure-core
     #   azure-identity
     #   google-auth
     #   isodate
     #   python-dateutil
-textual==0.22.3 \
-    --hash=sha256:1ef6457b9d8b727a67d2344bf2d0b530dce1afab55e1bf4e964e430929301baa \
-    --hash=sha256:a68172f7797e9f269270491e039f1e48096530dff64dbfe893e8477f2d4e200c
+textual==0.24.1 \
+    --hash=sha256:4c7e1f4ed12b9615c63fa3eb7cb9df68d29e0ae5b2352997958cd7ee5533f926 \
+    --hash=sha256:a7deb7ac5a1502424c754fe165ae13cb3890e47ddc514d3f089cb2984c336d1d
     # via -r requirements.in
 typing-extensions==4.5.0 \
     --hash=sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb \
     --hash=sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4
     # via
     #   azure-core
     #   azure-storage-blob
```

### Comparing `browsr-1.5.1/.gitignore` & `browsr-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/LICENSE` & `browsr-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `browsr-1.5.1/pyproject.toml` & `browsr-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "art~=5.7",
   "click~=8.1.3",
   "fsspec~=2023.1.0",
   "pandas~=1.5.2",
   "rich~=13.3.5",
   "rich-click~=1.5.2",
   "rich-pixels~=2.1.1",
-  "textual~=0.22.3",
+  "textual~=0.24.1",
   "universal-pathlib~=0.0.21",
   "Pillow>=9.1.0",
   "PyMuPDF~=1.22.3"
 ]
 description = "TUI File Browser App"
 dynamic = ["version"]
 keywords = []
@@ -83,15 +83,15 @@
   "mkdocs-literate-nav~=0.6.0",
   "mkdocs-section-index~=0.3.5",
   "black~=23.3.0",
   "ruff~=0.0.261",
   "mypy~=1.2.0",
   "pandas-stubs~=2.0.0.230412",
   "pip-tools~=6.13.0",
-  "textual[dev]~=0.22.3"
+  "textual[dev]~=0.24.1"
 ]
 features = ["all"]
 pre-install-commands = ["pip install -U --no-deps -r requirements/requirements-dev.txt"]
 python = "3.10"
 
 [tool.hatch.envs.default.scripts]
 _pip_compile = "pip-compile --resolver=backtracking --generate-hashes requirements.in"
```

### Comparing `browsr-1.5.1/PKG-INFO` & `browsr-1.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6272 6f77  : 2.1.Name: brow
-00000020: 7372 0a56 6572 7369 6f6e 3a20 312e 352e  sr.Version: 1.5.
-00000030: 310a 5375 6d6d 6172 793a 2054 5549 2046  1.Summary: TUI F
+00000020: 7372 0a56 6572 7369 6f6e 3a20 312e 362e  sr.Version: 1.6.
+00000030: 300a 5375 6d6d 6172 793a 2054 5549 2046  0.Summary: TUI F
 00000040: 696c 6520 4272 6f77 7365 7220 4170 700a  ile Browser App.
 00000050: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
 00000060: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
 00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
 00000080: 7566 7469 6e2f 6272 6f77 7372 2372 6561  uftin/browsr#rea
 00000090: 646d 650a 5072 6f6a 6563 742d 5552 4c3a  dme.Project-URL:
 000000a0: 2049 7373 7565 732c 2068 7474 7073 3a2f   Issues, https:/
@@ -55,15 +55,15 @@
 00000360: 732d 4469 7374 3a20 7269 6368 2d63 6c69  s-Dist: rich-cli
 00000370: 636b 7e3d 312e 352e 320a 5265 7175 6972  ck~=1.5.2.Requir
 00000380: 6573 2d44 6973 743a 2072 6963 682d 7069  es-Dist: rich-pi
 00000390: 7865 6c73 7e3d 322e 312e 310a 5265 7175  xels~=2.1.1.Requ
 000003a0: 6972 6573 2d44 6973 743a 2072 6963 687e  ires-Dist: rich~
 000003b0: 3d31 332e 332e 350a 5265 7175 6972 6573  =13.3.5.Requires
 000003c0: 2d44 6973 743a 2074 6578 7475 616c 7e3d  -Dist: textual~=
-000003d0: 302e 3232 2e33 0a52 6571 7569 7265 732d  0.22.3.Requires-
+000003d0: 302e 3234 2e31 0a52 6571 7569 7265 732d  0.24.1.Requires-
 000003e0: 4469 7374 3a20 756e 6976 6572 7361 6c2d  Dist: universal-
 000003f0: 7061 7468 6c69 627e 3d30 2e30 2e32 310a  pathlib~=0.0.21.
 00000400: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
 00000410: 616c 6c0a 5265 7175 6972 6573 2d44 6973  all.Requires-Dis
 00000420: 743a 2061 646c 6673 7e3d 3230 3233 2e31  t: adlfs~=2023.1
 00000430: 2e30 3b20 6578 7472 6120 3d3d 2027 616c  .0; extra == 'al
 00000440: 6c27 0a52 6571 7569 7265 732d 4469 7374  l'.Requires-Dist
@@ -102,181 +102,177 @@
 00000650: 656d 6f74 6527 0a52 6571 7569 7265 732d  emote'.Requires-
 00000660: 4469 7374 3a20 7333 6673 7e3d 3230 3233  Dist: s3fs~=2023
 00000670: 2e31 2e30 3b20 6578 7472 6120 3d3d 2027  .1.0; extra == '
 00000680: 7265 6d6f 7465 270a 4465 7363 7269 7074  remote'.Descript
 00000690: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 000006a0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 000006b0: 0a23 2062 726f 7773 720a 0a3c 6469 7620  .# browsr..<div 
-000006c0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-000006d0: 2020 2020 3c70 6963 7475 7265 3e0a 2020      <picture>.  
-000006e0: 2020 2020 2020 3c69 6d67 2073 7263 3d68        <img src=h
-000006f0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000700: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000710: 2f6a 7566 7469 6e2f 6272 6f77 7372 2f6d  /juftin/browsr/m
-00000720: 6169 6e2f 646f 6373 2f5f 7374 6174 6963  ain/docs/_static
-00000730: 2f62 726f 7773 722e 706e 670a 2020 2020  /browsr.png.    
-00000740: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
-00000750: 3430 3022 2061 6c74 3d22 6272 6f77 7372  400" alt="browsr
-00000760: 223e 0a20 2020 203c 2f70 6963 7475 7265  ">.    </picture
-00000770: 3e0a 3c2f 6469 763e 0a0a 5b21 5b62 726f  >.</div>..[![bro
-00000780: 7773 7220 5665 7273 696f 6e5d 2868 7474  wsr Version](htt
-00000790: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000007a0: 2e69 6f2f 7079 7069 2f76 2f62 726f 7773  .io/pypi/v/brows
-000007b0: 723f 636f 6c6f 723d 626c 7565 266c 6162  r?color=blue&lab
-000007c0: 656c 3d62 726f 7773 7229 5d28 6874 7470  el=browsr)](http
-000007d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000007e0: 7566 7469 6e2f 6272 6f77 7372 290a 5b21  uftin/browsr).[!
-000007f0: 5b50 7950 495d 2868 7474 7073 3a2f 2f69  [PyPI](https://i
-00000800: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000810: 7069 2f70 7976 6572 7369 6f6e 732f 6272  pi/pyversions/br
-00000820: 6f77 7372 295d 2868 7474 7073 3a2f 2f70  owsr)](https://p
-00000830: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-00000840: 7970 692f 6272 6f77 7372 2f29 0a5b 215b  ypi/browsr/).[![
-00000850: 5465 7374 696e 6720 5374 6174 7573 5d28  Testing Status](
-00000860: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000870: 6f6d 2f6a 7566 7469 6e2f 6272 6f77 7372  om/juftin/browsr
-00000880: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000890: 7773 2f74 6573 7473 2e79 616d 6c2f 6261  ws/tests.yaml/ba
-000008a0: 6467 652e 7376 673f 6272 616e 6368 3d6d  dge.svg?branch=m
-000008b0: 6169 6e29 5d28 6874 7470 733a 2f2f 6769  ain)](https://gi
-000008c0: 7468 7562 2e63 6f6d 2f6a 7566 7469 6e2f  thub.com/juftin/
-000008d0: 6272 6f77 7372 2f61 6374 696f 6e73 2f77  browsr/actions/w
-000008e0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
-000008f0: 616d 6c3f 7175 6572 793d 6272 616e 6368  aml?query=branch
-00000900: 2533 416d 6169 6e29 0a5b 215b 4769 7448  %3Amain).[![GitH
-00000910: 7562 204c 6963 656e 7365 5d28 6874 7470  ub License](http
-00000920: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000930: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
-00000940: 652f 6a75 6674 696e 2f62 726f 7773 723f  e/juftin/browsr?
-00000950: 636f 6c6f 723d 626c 7565 266c 6162 656c  color=blue&label
-00000960: 3d4c 6963 656e 7365 295d 2868 7474 7073  =License)](https
-00000970: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a75  ://github.com/ju
-00000980: 6674 696e 2f62 726f 7773 722f 626c 6f62  ftin/browsr/blob
-00000990: 2f6d 6169 6e2f 4c49 4345 4e53 4529 0a0a  /main/LICENSE)..
-000009a0: 2a2a 6062 726f 7773 7260 2a2a 2069 7320  **`browsr`** is 
-000009b0: 6120 5455 4920 2874 6578 742d 6261 7365  a TUI (text-base
-000009c0: 6420 7573 6572 2069 6e74 6572 6661 6365  d user interface
-000009d0: 2920 6669 6c65 2062 726f 7773 6572 2066  ) file browser f
-000009e0: 6f72 2079 6f75 7220 7465 726d 696e 616c  or your terminal
-000009f0: 2e0a 4974 2773 2061 2073 696d 706c 6520  ..It's a simple 
-00000a00: 7761 7920 746f 2062 726f 7773 6520 796f  way to browse yo
-00000a10: 7572 2066 696c 6573 2061 6e64 2074 616b  ur files and tak
-00000a20: 6520 6120 7065 656b 2061 7420 7468 6569  e a peek at thei
-00000a30: 7220 636f 6e74 656e 7473 2e20 506c 7573  r contents. Plus
-00000a40: 2069 740a 776f 726b 7320 6f6e 206c 6f63   it.works on loc
-00000a50: 616c 2061 6e64 2072 656d 6f74 6520 6669  al and remote fi
-00000a60: 6c65 2073 7973 7465 6d73 2e0a 0a3c 6465  le systems...<de
-00000a70: 7461 696c 7320 6f70 656e 3e3c 2f73 756d  tails open></sum
-00000a80: 6d61 7279 3e3c 2f73 756d 6d61 7279 3e0a  mary></summary>.
-00000a90: 0a3c 626f 6479 3e0a 3c64 6976 2073 7479  .<body>.<div sty
-00000aa0: 6c65 3d22 6469 7370 6c61 793a 2067 7269  le="display: gri
-00000ab0: 643b 2067 7269 642d 7465 6d70 6c61 7465  d; grid-template
-00000ac0: 2d63 6f6c 756d 6e73 3a20 7265 7065 6174  -columns: repeat
-00000ad0: 2832 2c20 3166 7229 3b20 6772 6964 2d67  (2, 1fr); grid-g
-00000ae0: 6170 3a20 3130 7078 3b22 3e0a 2020 2020  ap: 10px;">.    
-00000af0: 3c70 6963 7475 7265 3e0a 2020 2020 2020  <picture>.      
-00000b00: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000b10: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00000b20: 6572 636f 6e74 656e 742e 636f 6d2f 6a75  ercontent.com/ju
-00000b30: 6674 696e 2f62 726f 7773 722f 6d61 696e  ftin/browsr/main
-00000b40: 2f64 6f63 732f 5f73 7461 7469 632f 7363  /docs/_static/sc
-00000b50: 7265 656e 7368 6f74 5f75 7469 6c73 2e70  reenshot_utils.p
-00000b60: 6e67 2220 616c 743d 2249 6d61 6765 2031  ng" alt="Image 1
-00000b70: 223e 0a20 2020 203c 2f70 6963 7475 7265  ">.    </picture
-00000b80: 3e0a 2020 2020 3c70 6963 7475 7265 3e0a  >.    <picture>.
-00000b90: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00000ba0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00000bb0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000bc0: 636f 6d2f 6a75 6674 696e 2f62 726f 7773  com/juftin/brows
-00000bd0: 722f 6d61 696e 2f64 6f63 732f 5f73 7461  r/main/docs/_sta
-00000be0: 7469 632f 7363 7265 656e 7368 6f74 5f64  tic/screenshot_d
-00000bf0: 6174 6174 6162 6c65 2e70 6e67 2220 616c  atatable.png" al
-00000c00: 743d 2249 6d61 6765 2032 223e 0a20 2020  t="Image 2">.   
-00000c10: 203c 2f70 6963 7475 7265 3e0a 2020 2020   </picture>.    
-00000c20: 3c70 6963 7475 7265 3e0a 2020 2020 2020  <picture>.      
-00000c30: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000c40: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00000c50: 6572 636f 6e74 656e 742e 636f 6d2f 6a75  ercontent.com/ju
-00000c60: 6674 696e 2f62 726f 7773 722f 6d61 696e  ftin/browsr/main
-00000c70: 2f64 6f63 732f 5f73 7461 7469 632f 7363  /docs/_static/sc
-00000c80: 7265 656e 7368 6f74 5f6d 6f6e 615f 6c69  reenshot_mona_li
-00000c90: 7361 2e70 6e67 2220 616c 743d 2249 6d61  sa.png" alt="Ima
-00000ca0: 6765 2033 223e 0a20 2020 203c 2f70 6963  ge 3">.    </pic
-00000cb0: 7475 7265 3e0a 2020 2020 3c70 6963 7475  ture>.    <pictu
-00000cc0: 7265 3e0a 2020 2020 2020 2020 3c69 6d67  re>.        <img
-00000cd0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000ce0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000cf0: 656e 742e 636f 6d2f 6a75 6674 696e 2f62  ent.com/juftin/b
-00000d00: 726f 7773 722f 6d61 696e 2f64 6f63 732f  rowsr/main/docs/
-00000d10: 5f73 7461 7469 632f 7363 7265 656e 7368  _static/screensh
-00000d20: 6f74 5f6d 6172 6b64 6f77 6e2e 706e 6722  ot_markdown.png"
-00000d30: 2061 6c74 3d22 496d 6167 6520 3422 3e0a   alt="Image 4">.
-00000d40: 2020 2020 3c2f 7069 6374 7572 653e 0a3c      </picture>.<
-00000d50: 2f64 6976 3e0a 3c2f 626f 6479 3e0a 0a3c  /div>.</body>..<
-00000d60: 2f64 6574 6169 6c73 3e0a 0a23 2320 496e  /details>..## In
-00000d70: 7374 616c 6c61 7469 6f6e 0a0a 5468 6520  stallation..The 
-00000d80: 6265 6c6f 7720 636f 6d6d 616e 6420 7265  below command re
-00000d90: 636f 6d6d 656e 6473 205b 7069 7078 5d28  commends [pipx](
-00000da0: 6874 7470 733a 2f2f 7079 7061 2e67 6974  https://pypa.git
-00000db0: 6875 622e 696f 2f70 6970 782f 2920 696e  hub.io/pipx/) in
-00000dc0: 7374 6561 6420 6f66 2070 6970 2e20 6070  stead of pip. `p
-00000dd0: 6970 7860 2069 6e73 7461 6c6c 7320 7468  ipx` installs th
-00000de0: 6520 7061 636b 6167 6520 696e 0a61 6e20  e package in.an 
-00000df0: 6973 6f6c 6174 6564 2065 6e76 6972 6f6e  isolated environ
-00000e00: 6d65 6e74 2061 6e64 206d 616b 6573 2069  ment and makes i
-00000e10: 7420 6561 7379 2074 6f20 756e 696e 7374  t easy to uninst
-00000e20: 616c 6c2e 2049 6620 796f 7527 6420 6c69  all. If you'd li
-00000e30: 6b65 2074 6f20 7573 6520 6070 6970 6020  ke to use `pip` 
-00000e40: 696e 7374 6561 642c 206a 7573 7420 7265  instead, just re
-00000e50: 706c 6163 6520 6070 6970 7860 0a77 6974  place `pipx`.wit
-00000e60: 6820 6070 6970 6020 696e 2074 6865 2062  h `pip` in the b
-00000e70: 656c 6f77 2063 6f6d 6d61 6e64 2e0a 0a60  elow command...`
-00000e80: 6060 7368 656c 6c0a 7069 7078 2069 6e73  ``shell.pipx ins
-00000e90: 7461 6c6c 2062 726f 7773 720a 6060 600a  tall browsr.```.
-00000ea0: 0a23 2320 4578 7472 6120 496e 7374 616c  .## Extra Instal
-00000eb0: 6c61 7469 6f6e 0a0a 4966 2079 6f75 2772  lation..If you'r
-00000ec0: 6520 6c6f 6f6b 696e 6720 746f 2075 7365  e looking to use
-00000ed0: 202a 2a60 6272 6f77 7372 602a 2a20 6f6e   **`browsr`** on
-00000ee0: 2072 656d 6f74 6520 6669 6c65 2073 7973   remote file sys
-00000ef0: 7465 6d73 2c20 6c69 6b65 2041 5753 2053  tems, like AWS S
-00000f00: 332c 2079 6f75 276c 6c20 6e65 6564 2074  3, you'll need t
-00000f10: 6f20 696e 7374 616c 6c20 7468 6520 6072  o install the `r
-00000f20: 656d 6f74 6560 2065 7874 7261 2e0a 4966  emote` extra..If
-00000f30: 2079 6f75 2764 206c 696b 6520 746f 2062   you'd like to b
-00000f40: 726f 7773 6520 7061 7271 7565 7420 6669  rowse parquet fi
-00000f50: 6c65 732c 2079 6f75 276c 6c20 6e65 6564  les, you'll need
-00000f60: 2074 6f20 696e 7374 616c 6c20 7468 6520   to install the 
-00000f70: 6070 6172 7175 6574 6020 6578 7472 612e  `parquet` extra.
-00000f80: 204f 722c 2065 7665 6e20 7369 6d70 6c65   Or, even simple
-00000f90: 722c 0a79 6f75 2063 616e 2069 6e73 7461  r,.you can insta
-00000fa0: 6c6c 2074 6865 2060 616c 6c60 2065 7874  ll the `all` ext
-00000fb0: 7261 2074 6f20 6765 7420 616c 6c20 7468  ra to get all th
-00000fc0: 6520 6578 7472 6173 2e0a 0a60 6060 7368  e extras...```sh
-00000fd0: 656c 6c0a 7069 7078 2069 6e73 7461 6c6c  ell.pipx install
-00000fe0: 2022 6272 6f77 7372 5b61 6c6c 5d22 0a60   "browsr[all]".`
-00000ff0: 6060 0a0a 2323 2055 7361 6765 0a0a 6060  ``..## Usage..``
-00001000: 6073 6865 6c6c 0a62 726f 7773 7220 7e2f  `shell.browsr ~/
-00001010: 446f 776e 6c6f 6164 732f 0a60 6060 0a0a  Downloads/.```..
-00001020: 5369 6d70 6c79 2067 6976 6520 2a2a 6062  Simply give **`b
-00001030: 726f 7773 7260 2a2a 2061 2070 6174 6820  rowsr`** a path 
-00001040: 746f 2061 2066 696c 652f 6469 7265 6374  to a file/direct
-00001050: 6f72 7920 616e 6420 6974 2077 696c 6c20  ory and it will 
-00001060: 6f70 656e 2061 2062 726f 7773 6572 2077  open a browser w
-00001070: 696e 646f 770a 7769 7468 2061 2066 696c  indow.with a fil
-00001080: 6520 6272 6f77 7365 722e 2059 6f75 2063  e browser. You c
-00001090: 616e 2061 6c73 6f20 6769 7665 2069 7420  an also give it 
-000010a0: 6120 5552 4c20 746f 2061 2072 656d 6f74  a URL to a remot
-000010b0: 6520 6669 6c65 2073 7973 7465 6d2c 206c  e file system, l
-000010c0: 696b 6520 4157 5320 5333 2e0a 0a60 6060  ike AWS S3...```
-000010d0: 7368 656c 6c0a 6272 6f77 7372 2073 333a  shell.browsr s3:
-000010e0: 2f2f 6d79 2d62 7563 6b65 742f 6d79 2d66  //my-bucket/my-f
-000010f0: 696c 652e 7061 7271 7565 740a 6060 600a  ile.parquet.```.
-00001100: 0a23 2323 205b 4368 6563 6b20 6f75 7420  .### [Check out 
-00001110: 7468 6520 446f 6375 6d65 6e74 6174 696f  the Documentatio
-00001120: 6e5d 2868 7474 7073 3a2f 2f6a 7566 7469  n](https://jufti
-00001130: 6e2e 636f 6d2f 6272 6f77 7372 2f29 2066  n.com/browsr/) f
-00001140: 6f72 206d 6f72 650a 0a23 2320 4c69 6365  or more..## Lice
-00001150: 6e73 650a 0a2a 2a60 6272 6f77 7372 602a  nse..**`browsr`*
-00001160: 2a20 6973 2064 6973 7472 6962 7574 6564  * is distributed
-00001170: 2075 6e64 6572 2074 6865 2074 6572 6d73   under the terms
-00001180: 206f 6620 7468 6520 5b4d 4954 206c 6963   of the [MIT lic
-00001190: 656e 7365 5d28 4c49 4345 4e53 4529 2e0a  ense](LICENSE)..
+000006c0: 616c 6967 6e3d 2263 656e 7465 7222 2068  align="center" h
+000006d0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000006e0: 6875 622e 636f 6d2f 6a75 6674 696e 2f62  hub.com/juftin/b
+000006f0: 726f 7773 7222 3e0a 2020 2020 3c61 2068  rowsr">.    <a h
+00000700: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000710: 6875 622e 636f 6d2f 6a75 6674 696e 2f62  hub.com/juftin/b
+00000720: 726f 7773 7222 3e0a 2020 2020 2020 3c69  rowsr">.      <i
+00000730: 6d67 2073 7263 3d68 7474 7073 3a2f 2f72  mg src=https://r
+00000740: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000750: 7465 6e74 2e63 6f6d 2f6a 7566 7469 6e2f  tent.com/juftin/
+00000760: 6272 6f77 7372 2f6d 6169 6e2f 646f 6373  browsr/main/docs
+00000770: 2f5f 7374 6174 6963 2f62 726f 7773 722e  /_static/browsr.
+00000780: 706e 670a 2020 2020 2020 2020 7769 6474  png.        widt
+00000790: 683d 2234 3030 2220 616c 743d 2262 726f  h="400" alt="bro
+000007a0: 7773 7222 3e0a 2020 2020 3c2f 613e 0a3c  wsr">.    </a>.<
+000007b0: 2f64 6976 3e0a 0a5b 215b 6272 6f77 7372  /div>..[![browsr
+000007c0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+000007d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007e0: 2f70 7970 692f 762f 6272 6f77 7372 3f63  /pypi/v/browsr?c
+000007f0: 6f6c 6f72 3d62 6c75 6526 6c61 6265 6c3d  olor=blue&label=
+00000800: 6272 6f77 7372 295d 2868 7474 7073 3a2f  browsr)](https:/
+00000810: 2f67 6974 6875 622e 636f 6d2f 6a75 6674  /github.com/juft
+00000820: 696e 2f62 726f 7773 7229 0a5b 215b 5079  in/browsr).[![Py
+00000830: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
+00000840: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000850: 7079 7665 7273 696f 6e73 2f62 726f 7773  pyversions/brows
+00000860: 7229 5d28 6874 7470 733a 2f2f 7079 7069  r)](https://pypi
+00000870: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000880: 2f62 726f 7773 722f 290a 5b21 5b54 6573  /browsr/).[![Tes
+00000890: 7469 6e67 2053 7461 7475 735d 2868 7474  ting Status](htt
+000008a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000008b0: 6a75 6674 696e 2f62 726f 7773 722f 6163  juftin/browsr/ac
+000008c0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000008d0: 7465 7374 732e 7961 6d6c 2f62 6164 6765  tests.yaml/badge
+000008e0: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+000008f0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000900: 622e 636f 6d2f 6a75 6674 696e 2f62 726f  b.com/juftin/bro
+00000910: 7773 722f 6163 7469 6f6e 732f 776f 726b  wsr/actions/work
+00000920: 666c 6f77 732f 7465 7374 732e 7961 6d6c  flows/tests.yaml
+00000930: 3f71 7565 7279 3d62 7261 6e63 6825 3341  ?query=branch%3A
+00000940: 6d61 696e 290a 5b21 5b47 6974 4875 6220  main).[![GitHub 
+00000950: 4c69 6365 6e73 655d 2868 7474 7073 3a2f  License](https:/
+00000960: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000970: 6769 7468 7562 2f6c 6963 656e 7365 2f6a  github/license/j
+00000980: 7566 7469 6e2f 6272 6f77 7372 3f63 6f6c  uftin/browsr?col
+00000990: 6f72 3d62 6c75 6526 6c61 6265 6c3d 4c69  or=blue&label=Li
+000009a0: 6365 6e73 6529 5d28 6874 7470 733a 2f2f  cense)](https://
+000009b0: 6769 7468 7562 2e63 6f6d 2f6a 7566 7469  github.com/jufti
+000009c0: 6e2f 6272 6f77 7372 2f62 6c6f 622f 6d61  n/browsr/blob/ma
+000009d0: 696e 2f4c 4943 454e 5345 290a 0a2a 2a60  in/LICENSE)..**`
+000009e0: 6272 6f77 7372 602a 2a20 6973 2061 2054  browsr`** is a T
+000009f0: 5549 2028 7465 7874 2d62 6173 6564 2075  UI (text-based u
+00000a00: 7365 7220 696e 7465 7266 6163 6529 2066  ser interface) f
+00000a10: 696c 6520 6272 6f77 7365 7220 666f 7220  ile browser for 
+00000a20: 796f 7572 2074 6572 6d69 6e61 6c2e 0a49  your terminal..I
+00000a30: 7427 7320 6120 7369 6d70 6c65 2077 6179  t's a simple way
+00000a40: 2074 6f20 6272 6f77 7365 2079 6f75 7220   to browse your 
+00000a50: 6669 6c65 7320 616e 6420 7461 6b65 2061  files and take a
+00000a60: 2070 6565 6b20 6174 2074 6865 6972 2063   peek at their c
+00000a70: 6f6e 7465 6e74 732e 2050 6c75 7320 6974  ontents. Plus it
+00000a80: 0a77 6f72 6b73 206f 6e20 6c6f 6361 6c20  .works on local 
+00000a90: 616e 6420 7265 6d6f 7465 2066 696c 6520  and remote file 
+00000aa0: 7379 7374 656d 732e 0a0a 3c64 6574 6169  systems...<detai
+00000ab0: 6c73 206f 7065 6e3e 3c2f 7375 6d6d 6172  ls open></summar
+00000ac0: 793e 3c2f 7375 6d6d 6172 793e 0a0a 3c62  y></summary>..<b
+00000ad0: 6f64 793e 0a3c 6469 7620 7374 796c 653d  ody>.<div style=
+00000ae0: 2264 6973 706c 6179 3a20 6772 6964 3b20  "display: grid; 
+00000af0: 6772 6964 2d74 656d 706c 6174 652d 636f  grid-template-co
+00000b00: 6c75 6d6e 733a 2072 6570 6561 7428 322c  lumns: repeat(2,
+00000b10: 2031 6672 293b 2067 7269 642d 6761 703a   1fr); grid-gap:
+00000b20: 2031 3070 783b 223e 0a20 2020 203c 696d   10px;">.    <im
+00000b30: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000b40: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000b50: 7465 6e74 2e63 6f6d 2f6a 7566 7469 6e2f  tent.com/juftin/
+00000b60: 6272 6f77 7372 2f6d 6169 6e2f 646f 6373  browsr/main/docs
+00000b70: 2f5f 7374 6174 6963 2f73 6372 6565 6e73  /_static/screens
+00000b80: 686f 745f 7574 696c 732e 706e 6722 2061  hot_utils.png" a
+00000b90: 6c74 3d22 496d 6167 6520 3122 3e0a 2020  lt="Image 1">.  
+00000ba0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000bb0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000bc0: 6572 636f 6e74 656e 742e 636f 6d2f 6a75  ercontent.com/ju
+00000bd0: 6674 696e 2f62 726f 7773 722f 6d61 696e  ftin/browsr/main
+00000be0: 2f64 6f63 732f 5f73 7461 7469 632f 7363  /docs/_static/sc
+00000bf0: 7265 656e 7368 6f74 5f64 6174 6174 6162  reenshot_datatab
+00000c00: 6c65 2e70 6e67 2220 616c 743d 2249 6d61  le.png" alt="Ima
+00000c10: 6765 2032 223e 0a20 2020 203c 696d 6720  ge 2">.    <img 
+00000c20: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00000c30: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000c40: 6e74 2e63 6f6d 2f6a 7566 7469 6e2f 6272  nt.com/juftin/br
+00000c50: 6f77 7372 2f6d 6169 6e2f 646f 6373 2f5f  owsr/main/docs/_
+00000c60: 7374 6174 6963 2f73 6372 6565 6e73 686f  static/screensho
+00000c70: 745f 6d6f 6e61 5f6c 6973 612e 706e 6722  t_mona_lisa.png"
+00000c80: 2061 6c74 3d22 496d 6167 6520 3322 3e0a   alt="Image 3">.
+00000c90: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000ca0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000cb0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000cc0: 6a75 6674 696e 2f62 726f 7773 722f 6d61  juftin/browsr/ma
+00000cd0: 696e 2f64 6f63 732f 5f73 7461 7469 632f  in/docs/_static/
+00000ce0: 7363 7265 656e 7368 6f74 5f6d 6172 6b64  screenshot_markd
+00000cf0: 6f77 6e2e 706e 6722 2061 6c74 3d22 496d  own.png" alt="Im
+00000d00: 6167 6520 3422 3e0a 3c2f 6469 763e 0a3c  age 4">.</div>.<
+00000d10: 2f62 6f64 793e 0a0a 3c2f 6465 7461 696c  /body>..</detail
+00000d20: 733e 0a0a 2323 2049 6e73 7461 6c6c 6174  s>..## Installat
+00000d30: 696f 6e0a 0a54 6865 2062 656c 6f77 2063  ion..The below c
+00000d40: 6f6d 6d61 6e64 2072 6563 6f6d 6d65 6e64  ommand recommend
+00000d50: 7320 5b70 6970 785d 2868 7474 7073 3a2f  s [pipx](https:/
+00000d60: 2f70 7970 612e 6769 7468 7562 2e69 6f2f  /pypa.github.io/
+00000d70: 7069 7078 2f29 2069 6e73 7465 6164 206f  pipx/) instead o
+00000d80: 6620 7069 702e 2060 7069 7078 6020 696e  f pip. `pipx` in
+00000d90: 7374 616c 6c73 2074 6865 2070 6163 6b61  stalls the packa
+00000da0: 6765 2069 6e0a 616e 2069 736f 6c61 7465  ge in.an isolate
+00000db0: 6420 656e 7669 726f 6e6d 656e 7420 616e  d environment an
+00000dc0: 6420 6d61 6b65 7320 6974 2065 6173 7920  d makes it easy 
+00000dd0: 746f 2075 6e69 6e73 7461 6c6c 2e20 4966  to uninstall. If
+00000de0: 2079 6f75 2764 206c 696b 6520 746f 2075   you'd like to u
+00000df0: 7365 2060 7069 7060 2069 6e73 7465 6164  se `pip` instead
+00000e00: 2c20 6a75 7374 2072 6570 6c61 6365 2060  , just replace `
+00000e10: 7069 7078 600a 7769 7468 2060 7069 7060  pipx`.with `pip`
+00000e20: 2069 6e20 7468 6520 6265 6c6f 7720 636f   in the below co
+00000e30: 6d6d 616e 642e 0a0a 6060 6073 6865 6c6c  mmand...```shell
+00000e40: 0a70 6970 7820 696e 7374 616c 6c20 6272  .pipx install br
+00000e50: 6f77 7372 0a60 6060 0a0a 2323 2045 7874  owsr.```..## Ext
+00000e60: 7261 2049 6e73 7461 6c6c 6174 696f 6e0a  ra Installation.
+00000e70: 0a49 6620 796f 7527 7265 206c 6f6f 6b69  .If you're looki
+00000e80: 6e67 2074 6f20 7573 6520 2a2a 6062 726f  ng to use **`bro
+00000e90: 7773 7260 2a2a 206f 6e20 7265 6d6f 7465  wsr`** on remote
+00000ea0: 2066 696c 6520 7379 7374 656d 732c 206c   file systems, l
+00000eb0: 696b 6520 4157 5320 5333 2c20 796f 7527  ike AWS S3, you'
+00000ec0: 6c6c 206e 6565 6420 746f 2069 6e73 7461  ll need to insta
+00000ed0: 6c6c 2074 6865 2060 7265 6d6f 7465 6020  ll the `remote` 
+00000ee0: 6578 7472 612e 0a49 6620 796f 7527 6420  extra..If you'd 
+00000ef0: 6c69 6b65 2074 6f20 6272 6f77 7365 2070  like to browse p
+00000f00: 6172 7175 6574 2066 696c 6573 2c20 796f  arquet files, yo
+00000f10: 7527 6c6c 206e 6565 6420 746f 2069 6e73  u'll need to ins
+00000f20: 7461 6c6c 2074 6865 2060 7061 7271 7565  tall the `parque
+00000f30: 7460 2065 7874 7261 2e20 4f72 2c20 6576  t` extra. Or, ev
+00000f40: 656e 2073 696d 706c 6572 2c0a 796f 7520  en simpler,.you 
+00000f50: 6361 6e20 696e 7374 616c 6c20 7468 6520  can install the 
+00000f60: 6061 6c6c 6020 6578 7472 6120 746f 2067  `all` extra to g
+00000f70: 6574 2061 6c6c 2074 6865 2065 7874 7261  et all the extra
+00000f80: 732e 0a0a 6060 6073 6865 6c6c 0a70 6970  s...```shell.pip
+00000f90: 7820 696e 7374 616c 6c20 2262 726f 7773  x install "brows
+00000fa0: 725b 616c 6c5d 220a 6060 600a 0a23 2320  r[all]".```..## 
+00000fb0: 5573 6167 650a 0a60 6060 7368 656c 6c0a  Usage..```shell.
+00000fc0: 6272 6f77 7372 207e 2f44 6f77 6e6c 6f61  browsr ~/Downloa
+00000fd0: 6473 2f0a 6060 600a 0a53 696d 706c 7920  ds/.```..Simply 
+00000fe0: 6769 7665 202a 2a60 6272 6f77 7372 602a  give **`browsr`*
+00000ff0: 2a20 6120 7061 7468 2074 6f20 6120 6669  * a path to a fi
+00001000: 6c65 2f64 6972 6563 746f 7279 2061 6e64  le/directory and
+00001010: 2069 7420 7769 6c6c 206f 7065 6e20 6120   it will open a 
+00001020: 6272 6f77 7365 7220 7769 6e64 6f77 0a77  browser window.w
+00001030: 6974 6820 6120 6669 6c65 2062 726f 7773  ith a file brows
+00001040: 6572 2e20 596f 7520 6361 6e20 616c 736f  er. You can also
+00001050: 2067 6976 6520 6974 2061 2055 524c 2074   give it a URL t
+00001060: 6f20 6120 7265 6d6f 7465 2066 696c 6520  o a remote file 
+00001070: 7379 7374 656d 2c20 6c69 6b65 2041 5753  system, like AWS
+00001080: 2053 332e 0a0a 6060 6073 6865 6c6c 0a62   S3...```shell.b
+00001090: 726f 7773 7220 7333 3a2f 2f6d 792d 6275  rowsr s3://my-bu
+000010a0: 636b 6574 2f6d 792d 6669 6c65 2e70 6172  cket/my-file.par
+000010b0: 7175 6574 0a60 6060 0a0a 2323 2320 5b43  quet.```..### [C
+000010c0: 6865 636b 206f 7574 2074 6865 2044 6f63  heck out the Doc
+000010d0: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+000010e0: 733a 2f2f 6a75 6674 696e 2e63 6f6d 2f62  s://juftin.com/b
+000010f0: 726f 7773 722f 2920 666f 7220 6d6f 7265  rowsr/) for more
+00001100: 0a0a 2323 204c 6963 656e 7365 0a0a 2a2a  ..## License..**
+00001110: 6062 726f 7773 7260 2a2a 2069 7320 6469  `browsr`** is di
+00001120: 7374 7269 6275 7465 6420 756e 6465 7220  stributed under 
+00001130: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
+00001140: 205b 4d49 5420 6c69 6365 6e73 655d 284c   [MIT license](L
+00001150: 4943 454e 5345 292e 0a                   ICENSE)..
```

