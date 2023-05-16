# Comparing `tmp/data2latex-1.0.2.tar.gz` & `tmp/data2latex-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2latex-1.0.2.tar", last modified: Sun May 14 14:53:21 2023, max compression
+gzip compressed data, was "data2latex-1.0.4.tar", last modified: Tue May 16 08:23:16 2023, max compression
```

## Comparing `data2latex-1.0.2.tar` & `data2latex-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.630355 data2latex-1.0.2/
--rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4905 2023-05-14 14:53:21.629356 data2latex-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-05-14 12:42:09.000000 data2latex-1.0.2/README.md
--rw-rw-rw-   0        0        0     1824 2023-05-14 14:53:03.000000 data2latex-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 14:53:21.630355 data2latex-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.586357 data2latex-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.606361 data2latex-1.0.2/src/data2latex/
--rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.2/src/data2latex/__init__.py
--rw-rw-rw-   0        0        0     8211 2023-05-11 23:03:20.000000 data2latex-1.0.2/src/data2latex/dm.py
--rw-rw-rw-   0        0        0     7300 2023-05-07 19:42:55.000000 data2latex-1.0.2/src/data2latex/environments.py
--rw-rw-rw-   0        0        0    10015 2023-05-13 22:01:26.000000 data2latex-1.0.2/src/data2latex/features.py
--rw-rw-rw-   0        0        0     7658 2023-05-14 14:44:36.000000 data2latex-1.0.2/src/data2latex/iter_protocols.py
--rw-rw-rw-   0        0        0    30916 2023-05-14 14:44:36.000000 data2latex-1.0.2/src/data2latex/plot.py
--rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.2/src/data2latex/table.py
-drwxrwxrwx   0        0        0        0 2023-05-14 14:53:21.628356 data2latex-1.0.2/src/data2latex.egg-info/
--rw-rw-rw-   0        0        0     4905 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 14:53:21.000000 data2latex-1.0.2/src/data2latex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.401973 data2latex-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-05-14 10:51:18.000000 data2latex-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4923 2023-05-16 08:23:16.400974 data2latex-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2528 2023-05-16 08:12:54.000000 data2latex-1.0.4/README.md
+-rw-rw-rw-   0        0        0     1824 2023-05-16 08:15:25.000000 data2latex-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:23:16.401973 data2latex-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.372974 data2latex-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.387008 data2latex-1.0.4/src/data2latex/
+-rw-rw-rw-   0        0        0      266 2023-05-11 19:09:04.000000 data2latex-1.0.4/src/data2latex/__init__.py
+-rw-rw-rw-   0        0        0     8454 2023-05-14 20:33:59.000000 data2latex-1.0.4/src/data2latex/dm.py
+-rw-rw-rw-   0        0        0     7494 2023-05-14 20:34:47.000000 data2latex-1.0.4/src/data2latex/environments.py
+-rw-rw-rw-   0        0        0    10016 2023-05-14 20:34:10.000000 data2latex-1.0.4/src/data2latex/features.py
+-rw-rw-rw-   0        0        0     7658 2023-05-14 14:44:36.000000 data2latex-1.0.4/src/data2latex/iter_protocols.py
+-rw-rw-rw-   0        0        0    30916 2023-05-14 14:44:36.000000 data2latex-1.0.4/src/data2latex/plot.py
+-rw-rw-rw-   0        0        0    18502 2023-05-13 21:52:50.000000 data2latex-1.0.4/src/data2latex/table.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:23:16.399975 data2latex-1.0.4/src/data2latex.egg-info/
+-rw-rw-rw-   0        0        0     4923 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 08:23:16.000000 data2latex-1.0.4/src/data2latex.egg-info/top_level.txt
```

### Comparing `data2latex-1.0.2/LICENSE` & `data2latex-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.2/PKG-INFO` & `data2latex-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 1.0.2
+Version: 1.0.4
 Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,17 +46,17 @@
 
 # Data2LaTeX
 
 ![Data2LaTeX logo](docs/_static/img/logo.png)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This project is part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
+This project is a part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
 
-The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular `numpy` and `pandas` packages. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using `tblr` environment from `tabularray` package. The plots are created using `tikzpicture` / `axis` environment from `tikz` / `pgfplots` package.
+The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular packages `numpy` and `pandas`. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using the `tblr` environment from the `tabularray` package. The plots are created using the `tikzpicture` / `axis` environment from the `tikz` / `pgfplots` package.
 
 ## Examples
 
 Examples with results can be found in the [documentation](https://trolobezka.github.io/data2latex-docs).
 
 ### Simple features
```

### Comparing `data2latex-1.0.2/README.md` & `data2latex-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Data2LaTeX
 
 ![Data2LaTeX logo](docs/_static/img/logo.png)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This project is part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
+This project is a part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
 
-The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular `numpy` and `pandas` packages. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using `tblr` environment from `tabularray` package. The plots are created using `tikzpicture` / `axis` environment from `tikz` / `pgfplots` package.
+The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular packages `numpy` and `pandas`. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using the `tblr` environment from the `tabularray` package. The plots are created using the `tikzpicture` / `axis` environment from the `tikz` / `pgfplots` package.
 
 ## Examples
 
 Examples with results can be found in the [documentation](https://trolobezka.github.io/data2latex-docs).
 
 ### Simple features
```

### Comparing `data2latex-1.0.2/pyproject.toml` & `data2latex-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "data2latex"
-version = "1.0.2"
+version = "1.0.4"
 authors = [
   { name="Richard Kokštein", email="richard.Kokstein@fs.cvut.cz" },
 ]
 description = "Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document."
 keywords = ["generation", "latex", "table", "plot", "graph", "array", "datatable"]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
```

### Comparing `data2latex-1.0.2/src/data2latex/dm.py` & `data2latex-1.0.4/src/data2latex/dm.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,23 @@
             document_packages.add(Package("indentfirst"))
             document_packages.add(
                 UnsafeCommand(
                     "setlength", r"\parindent", None, extra_arguments=self.par_indent
                 )
             )
 
+        document_packages.add(
+            UnsafeCommand(
+                "newcommand",
+                r"\DataToLaTeX",
+                None,
+                extra_arguments=r"$\Delta$\texttt{ata2}\LaTeX{}",
+            )
+        )
+
         for p in self.packages:
             document_packages.add(p)
 
     @classmethod
     def use_standalone(
         cls,
         horizontal_border: str = "5pt",
```

### Comparing `data2latex-1.0.2/src/data2latex/environments.py` & `data2latex-1.0.4/src/data2latex/environments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Any, Dict, List, Optional, Union
 
-from pylatex import (  # pyright: ignore [reportMissingTypeStubs]
-    Label,
-    Marker,
-    Package,
-)
+from pylatex import Label, Marker, Package  # pyright: ignore [reportMissingTypeStubs]
 from pylatex.base_classes import (  # pyright: ignore [reportMissingTypeStubs]
     Command,
     Container,
     Environment,
     LatexObject,
 )
 from pylatex.base_classes.command import (  # pyright: ignore [reportMissingTypeStubs]
     Parameters,
 )
-from pylatex.utils import NoEscape  # pyright: ignore [reportMissingTypeStubs]
+from pylatex.utils import (  # pyright: ignore [reportMissingTypeStubs]
+    escape_latex,  # pyright: ignore [reportUnknownVariableType]
+    NoEscape,
+)
 
 
 class CommandEnvironment(Container):
     r"""
     Creates an environment with command syntax.
 
     :param command: Name of the command
@@ -219,17 +218,20 @@
 class Text(LatexObject):
     begin_paragraph = True
     end_paragraph = True
     separate_paragraph = True
 
     def __init__(self, content: Union[str, LatexObject], escape: bool = True):
         super().__init__()
-        self.content = content
-        self.escape = escape
+        self.content: Union[str, LatexObject] = content
+        self._escape: bool = escape
 
     def dumps(self) -> str:  # pyright: ignore [reportIncompatibleMethodOverride]
         string: str = ""
         if isinstance(self.content, LatexObject):
             string = self.content.dumps()  # pyright: ignore [reportGeneralTypeIssues]
         else:
-            string = self.content
+            if self._escape:
+                string = escape_latex(self.content)
+            else:
+                string = self.content
         return string
```

### Comparing `data2latex-1.0.2/src/data2latex/features.py` & `data2latex-1.0.4/src/data2latex/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     )
 
 
 def text(content: str, escape: bool = True) -> None:
     """
     Add a paragraph of solid text.
 
-    :param content: Content fo the paragraph.
+    :param content: Content for the paragraph.
     :type content: str
     :param escape: ``True`` for replacing special LaTeX characters, defaults to ``True``.
     :type escape: bool, optional
     """
     if escape:
         content = content.replace("_", r"\_")
     gdm().append(Text(content=content, escape=escape))
```

### Comparing `data2latex-1.0.2/src/data2latex/iter_protocols.py` & `data2latex-1.0.4/src/data2latex/iter_protocols.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.2/src/data2latex/plot.py` & `data2latex-1.0.4/src/data2latex/plot.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.2/src/data2latex/table.py` & `data2latex-1.0.4/src/data2latex/table.py`

 * *Files identical despite different names*

### Comparing `data2latex-1.0.2/src/data2latex.egg-info/PKG-INFO` & `data2latex-1.0.4/src/data2latex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data2latex
-Version: 1.0.2
+Version: 1.0.4
 Summary: Package prototype for simple generation of LaTeX tables and plots from scientific data for use in any document.
 Author-email: Richard Kokštein <richard.Kokstein@fs.cvut.cz>
 License: MIT License
         
         Copyright (c) 2023 Richard Kokstein
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,17 +46,17 @@
 
 # Data2LaTeX
 
 ![Data2LaTeX logo](docs/_static/img/logo.png)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This project is part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
+This project is a part of my bachelor thesis which deals with data representation using **Python** and **LaTeX**. You can find the source code on my [GitHub](https://github.com/Trolobezka/data2latex).
 
-The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular `numpy` and `pandas` packages. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using `tblr` environment from `tabularray` package. The plots are created using `tikzpicture` / `axis` environment from `tikz` / `pgfplots` package.
+The idea behind this package prototype is that generating LaTeX documents containing scientific data from Python should not be difficult and require many steps. Currently the package supports the creation of simple tables and two types of plots: scatter plots and line plots. The package uses the [PyLaTeX](https://github.com/JelteF/PyLaTeX) package to handle the document creation and compilation process. The main data sources are arrays and data tables from the popular packages `numpy` and `pandas`. A major inspiration for the module syntax is the `matplotlib.pyplot` module, which allows plots to be created in a few lines of code. The tables are created using the `tblr` environment from the `tabularray` package. The plots are created using the `tikzpicture` / `axis` environment from the `tikz` / `pgfplots` package.
 
 ## Examples
 
 Examples with results can be found in the [documentation](https://trolobezka.github.io/data2latex-docs).
 
 ### Simple features
```

