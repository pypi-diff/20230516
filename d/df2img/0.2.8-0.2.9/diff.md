# Comparing `tmp/df2img-0.2.8.tar.gz` & `tmp/df2img-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df2img-0.2.8.tar", max compression
+gzip compressed data, was "df2img-0.2.9.tar", max compression
```

## Comparing `df2img-0.2.8.tar` & `df2img-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     5703 2022-10-31 23:53:09.925344 df2img-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0     3125 2022-10-31 22:11:14.596243 df2img-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    14678 2022-10-31 22:11:14.596243 df2img-0.2.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1071 2022-10-21 19:37:10.073181 df2img-0.2.8/LICENSE
--rw-r--r--   0        0        0     5219 2022-11-01 00:24:41.381724 df2img-0.2.8/README.md
--rw-r--r--   0        0        0     2638 2022-11-01 00:25:37.855886 df2img-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      193 2022-10-21 19:37:10.083181 df2img-0.2.8/src/df2img/__init__.py
--rw-r--r--   0        0        0     7034 2022-10-28 20:57:23.493389 df2img-0.2.8/src/df2img/df2img.py
--rw-r--r--   0        0        0        0 2022-10-21 19:37:10.083181 df2img-0.2.8/src/df2img/py.typed
--rw-r--r--   0        0        0     6137 1970-01-01 00:00:00.000000 df2img-0.2.8/setup.py
--rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 df2img-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     5836 2023-01-03 07:51:33.389094 df2img-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     3125 2022-10-31 22:11:14.596243 df2img-0.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    14658 2023-01-03 07:51:33.389094 df2img-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1071 2022-10-21 19:37:10.073181 df2img-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5219 2022-11-01 00:24:41.381724 df2img-0.2.9/README.md
+-rw-r--r--   0        0        0     2638 2023-01-03 07:51:33.389094 df2img-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      193 2023-01-03 07:51:33.389094 df2img-0.2.9/src/df2img/__init__.py
+-rw-r--r--   0        0        0     7034 2022-10-28 20:57:23.493389 df2img-0.2.9/src/df2img/df2img.py
+-rw-r--r--   0        0        0        0 2022-10-21 19:37:10.083181 df2img-0.2.9/src/df2img/py.typed
+-rw-r--r--   0        0        0     6137 1970-01-01 00:00:00.000000 df2img-0.2.9/setup.py
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 df2img-0.2.9/PKG-INFO
```

### Comparing `df2img-0.2.8/CHANGELOG.md` & `df2img-0.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is loosely based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.9] - 2023-01-03
+### Security
+- Updated dependencies
+
 ## [0.2.8] - 2022-11-01
 ### Improved
 - Introduce **Contributing** section and **Code of conduct** to documentation.
 - Using [nox](https://nox.thea.codes/) for testing:
     - Unit testing using pytest
     - Added pytest coverage report.
     - Linting using [flake8](https://flake8.pycqa.org/en/latest/).
@@ -111,15 +115,16 @@
 - Possibility to add title to the image.
 - Possibility to define the number of header rows and header columns.
 - Possibility to change colors for header rows.
 - Possibility to alternate row colors for better readability.
 - Possibility to change column width and row height.
 - Possibility to change font size.
 
-[Unreleased]: https://github.com/andreas-vester/df2img/compare/0.2.8...HEAD
+[Unreleased]: https://github.com/andreas-vester/df2img/compare/0.2.9...main
+[0.2.9]: https://github.com/andreas-vester/df2img/compare/0.2.8...0.2.9
 [0.2.8]: https://github.com/andreas-vester/df2img/compare/v0.2.7...v0.2.8
 [0.2.7]: https://github.com/andreas-vester/df2img/compare/v0.2.6...v0.2.7
 [0.2.6]: https://github.com/andreas-vester/df2img/compare/v0.2.5...v0.2.6
 [0.2.5]: https://github.com/andreas-vester/df2img/compare/v0.2.4...v0.2.5
 [0.2.4]: https://github.com/andreas-vester/df2img/compare/v0.2.3...v0.2.4
 [0.2.3]: https://github.com/andreas-vester/df2img/compare/v0.2.2...v0.2.3
 [0.2.2]: https://github.com/andreas-vester/df2img/compare/v0.2.1...v0.2.2
```

### Comparing `df2img-0.2.8/CODE_OF_CONDUCT.md` & `df2img-0.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `df2img-0.2.8/CONTRIBUTING.md` & `df2img-0.2.9/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-!-- omit in toc -->
 # Contributing to df2img
 
 First off, thanks for taking the time to contribute! ❤️
 
 All types of contributions are encouraged and valued. See the
 [Table of Contents](#table-of-contents) for different ways to help and details about
 how this project handles them. Please make sure to read the relevant section before
```

### Comparing `df2img-0.2.8/LICENSE` & `df2img-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `df2img-0.2.8/README.md` & `df2img-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `df2img-0.2.8/pyproject.toml` & `df2img-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "df2img"
-version = "0.2.8"
+version = "0.2.9"
 description = "Save a Pandas DataFrame as image"
 license = "MIT"
 authors = ["Andreas Vester <info@df2img.dev>"]
 readme = "README.md"
 homepage = "https://df2img.dev"
 repository = "https://github.com/andreas-vester/df2img"
 documentation = "https://df2img.dev"
```

### Comparing `df2img-0.2.8/src/df2img/df2img.py` & `df2img-0.2.9/src/df2img/df2img.py`

 * *Files identical despite different names*

### Comparing `df2img-0.2.8/setup.py` & `df2img-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['kaleido==0.2.1', 'pandas>=1.0.0,<2.0.0', 'plotly>=5.3.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'df2img',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Save a Pandas DataFrame as image',
     'long_description': '# df2img: Save a Pandas DataFrame as image\n\n![img](https://img.shields.io/pypi/v/df2img)\n![img](https://img.shields.io/pypi/pyversions/df2img)\n![img](https://img.shields.io/github/license/andreas-vester/df2img)\n![img](https://img.shields.io/github/issues/andreas-vester/df2img)\n![img](https://img.shields.io/github/stars/andreas-vester/df2img)\n\n## What is it all about?\n\nHave you ever tried to save a ``pd.DataFrame`` into an image file? This is not a straightforward process at all. Unfortunately, ``pandas`` itself doesn\'t provide this functionality out of the box.\n\n**df2img** tries to fill the gap. It is a Python library that greatly simplifies the process of saving a ``pd.DataFrame`` into an image file (e.g. ``png`` or ``jpg``).\n\nIt is a wrapper/convenience function in order to create a ``plotly`` Table. That is, one can use ``plotly``\'s styling function to format the table.\n\n\n## Dependencies\n\n**df2img** has a limited number of dependencies, namely\n\n- ``pandas``\n- ``plotly``\n- ``kaleido``\n\n\n## Documentation\n\nAn extensive documentation is available at https://df2img.dev.\n\n\n## Quickstart\n\nYou can install the package via ``pip``.\n\n```bash\npip install df2img\n```\n\nUsing ``poetry``?\n\n```bash\npoetry add df2img\n```\n\nLet\'s create a simple ``pd.DataFrame`` with some dummy data:\n\n```python\nimport pandas as pd\n\nimport df2img\n\ndf = pd.DataFrame(\n    data=dict(\n        float_col=[1.4, float("NaN"), 250, 24.65],\n        str_col=("string1", "string2", float("NaN"), "string4"),\n    ),\n    index=["row1", "row2", "row3", "row4"],\n)\n```\n```python\n      float_col  str_col\nrow1       1.40  string1\nrow2        NaN  string2\nrow3     250.00      NaN\nrow4      24.65  string4\n```\n\n### Basics\n\nSaving ``df`` into a png-file now takes just two lines of code including some styling out of the box.\n\n* First, we create a ``plotly`` figure.\n* Second, we save the figure to disk.\n\n```python\nfig = df2img.plot_dataframe(df, fig_size=(500, 140))\n\ndf2img.save_dataframe(fig=fig, filename="plot1.png")\n```\n\n![img](https://github.com/andreas-vester/df2img/blob/main/docs/img/plot1.png?raw=true)\n\n\n### Formatting\n\nYou can control the settings for the header row via the ``tbl_header`` input argument. This accepts a regular ``dict``. This ``dict`` can comprise various key/value pairs that are also accepted by ``plotly``. All available key/value pairs can be seen at ``plotly``\'s website at https://plotly.com/python/reference/table/#table-header.\n\nLet\'s set the header row in a different color and size. Also, let\'s set the alignment to "left".\n\n```python\nfig = df2img.plot_dataframe(\n    df,\n    tbl_header=dict(\n        align="left",\n        fill_color="blue",\n        font_color="white",\n        font_size=14,\n    ),\n    fig_size=(500, 140),\n)\n```\n![img](https://github.com/andreas-vester/df2img/blob/main/docs/img/plot2.png?raw=true)\n\n\nControlling the table body (cells) is basically the same. Just use the ``tbl_cells`` input argument, which happens to be a ``dict``, too.\nSee https://plotly.com/python/reference/table/#table-cells for all the possible key/value pairs.\n\nLet\'s print the table cell values in yellow on a green background and align them "right".\n\n```python\nfig = df2img.plot_dataframe(\n    df,\n    tbl_cells=dict(\n        align="right",\n        fill_color="green",\n        font_color="yellow",\n    ),\n    fig_size=(500, 140),\n)\n```\n\n![img](https://github.com/andreas-vester/df2img/blob/main/docs/img/plot3.png?raw=true)\n\n\nYou can alternate row colors for better readability by using the ``row_fill_color`` input argument. Using HEX colors is also possible:\n\n```python\nfig = df2img.plot_dataframe(\n    df,\n    row_fill_color=("#ffffff", "#d7d8d6"),\n    fig_size=(500, 140),\n)\n```\n\n![img](https://github.com/andreas-vester/df2img/blob/main/docs/img/plot4.png?raw=true)\n\n\nSetting the title will be controlled via the ``title`` input argument. You can find the relevant key/value pairs here: https://plotly.com/python/reference/layout/#layout-title.\n\nLet\'s put the title in a different font and size. In addition, we can control the alignment via the ``x`` key/value pair. It sets the x (horizontal) position in normalized coordinates from "0" (left) to "1" (right).\n\n```python\n  fig = df2img.plot_dataframe(\n      df,\n      title=dict(\n          font_color="darkred",\n          font_family="Times New Roman",\n          font_size=24,\n          text="This is a title starting at the x-value x=0.1",\n          x=0.1,\n          xanchor="left",\n      ),\n      fig_size=(500, 140),\n  )\n  ```\n\n![img](https://github.com/andreas-vester/df2img/blob/main/docs/img/plot5.png?raw=true)\n\n\nYou can also control relative column width via the ``col_width`` argument. Let\'s set the first column\'s width triple the width of the third column and the second column\'s width double the width of the third column.\n\n```python\nfig = df2img.plot_dataframe(\n    df,\n    col_width=[3, 2, 1],\n    fig_size=(500, 140),\n)\n```\n\n![img](https://github.com/andreas-vester/df2img/blob/main/docs/img/plot6.png?raw=true)\n\n## Contributing to df2img\n\nIf you consider to contribute to **df2img**, please read the [Contributing to df2img](./CONTRIBUTING.md) section in the documentation. This document is supposed to guide you through the whole process.\n',
     'author': 'Andreas Vester',
     'author_email': 'info@df2img.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://df2img.dev',
```

### Comparing `df2img-0.2.8/PKG-INFO` & `df2img-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df2img
-Version: 0.2.8
+Version: 0.2.9
 Summary: Save a Pandas DataFrame as image
 Home-page: https://df2img.dev
 License: MIT
 Keywords: pandas,dataframe,image
 Author: Andreas Vester
 Author-email: info@df2img.dev
 Requires-Python: >=3.8,<4.0
```

