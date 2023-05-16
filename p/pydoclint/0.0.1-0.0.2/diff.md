# Comparing `tmp/pydoclint-0.0.1.tar.gz` & `tmp/pydoclint-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.1.tar", last modified: Mon May 15 10:14:11 2023, max compression
+gzip compressed data, was "pydoclint-0.0.2.tar", last modified: Tue May 16 08:41:01 2023, max compression
```

## Comparing `pydoclint-0.0.1.tar` & `pydoclint-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:14:11.745226 pydoclint-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 10:13:57.000000 pydoclint-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-15 10:14:11.745226 pydoclint-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-15 10:13:57.000000 pydoclint-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:14:11.741226 pydoclint-0.0.1/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/method_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:14:11.745226 pydoclint-0.0.1/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:14:11.741226 pydoclint-0.0.1/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-15 10:14:11.000000 pydoclint-0.0.1/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-15 10:14:11.000000 pydoclint-0.0.1/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:14:11.000000 pydoclint-0.0.1/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 10:14:11.000000 pydoclint-0.0.1/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 10:14:11.000000 pydoclint-0.0.1/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 10:14:11.000000 pydoclint-0.0.1/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 10:13:57.000000 pydoclint-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-15 10:14:11.745226 pydoclint-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 10:13:57.000000 pydoclint-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:14:11.745226 pydoclint-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-15 10:13:57.000000 pydoclint-0.0.1/tests/test_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-05-15 10:13:57.000000 pydoclint-0.0.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 08:40:48.000000 pydoclint-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-16 08:41:01.770929 pydoclint-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-16 08:40:48.000000 pydoclint-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/method_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 08:41:01.000000 pydoclint-0.0.2/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 08:40:48.000000 pydoclint-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-16 08:41:01.774929 pydoclint-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 08:40:48.000000 pydoclint-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:41:01.770929 pydoclint-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-16 08:40:48.000000 pydoclint-0.0.2/tests/test_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-05-16 08:40:48.000000 pydoclint-0.0.2/tests/test_main.py
```

### Comparing `pydoclint-0.0.1/LICENSE` & `pydoclint-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/PKG-INFO` & `pydoclint-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,74 @@
-Metadata-Version: 2.1
-Name: pydoclint
-Version: 0.0.1
-Summary: A linter to check arguments in Python docstrings
-Home-page: https://github.com/jsh9/pydoclint
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pydoclint
 
-A Python docstring linter to check whether a docstring's sections (arguments, returns, raises, ...) match the function signature or function implementation.
-
-It runs really fast. In fact, it is at least 30,000 times faster than [darglint](https://github.com/terrencepreilly/darglint) (another linter of the same purposes which is no longer maintained).
-
-Here is a comparison of running time on some famous Python projects:
+A Python docstring linter to check whether a docstring's sections (arguments,
+returns, raises, ...) match the function signature or function implementation.
 
-|                                                              | pydoclint | darglint             |
-| ------------------------------------------------------------ | --------- | -------------------- |
-| [numpy](https://github.com/numpy/numpy)                      | 0.08 sec  | > 40 min (> 30,000x) |
-| [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 0.09 sec  | > 40 min (> 30,000x) |
+It runs really fast. In fact, it is at least ~1,475 times faster than
+[darglint](https://github.com/terrencepreilly/darglint) (another linter of the
+same purposes which is no longer maintained).
+
+Here is a comparison of linting time on some famous Python projects:
+
+|                                                              | pydoclint | darglint                          |
+| ------------------------------------------------------------ | --------- | --------------------------------- |
+| [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
+| [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
+
+Currently, _pydoclint_ only works when you write your docstrings in the
+[numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support
+for the
+[Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
+docstrings will be added soon.
 
-Currently, `pydoclint` only works when you write your docstrings in the [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support for the [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html) docstrings will be added soon.
-
-**Note**: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle) serves complementary purposes. It is recommended that you use both together.
+Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
+serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
 pip install pydoclint
 ```
 
-Note that `pydoclint` only supports Python 3.8 and above.
+Note that _pydoclint_ currently only supports Python 3.8 and above. (Python 3.7
+support may be added if there are interests and requests.)
 
 ## 2. Usage
 
-### 2.1. As a standalone command line tool
+### 2.1. As a native command line tool
 
 ```
 pydoclint <FILE_OR_FOLDER>
 ```
 
 Replace `<FILE_OR_FOLDER>` with the file/folder names you want, such as `.`.
 
-### 2.2. As a flake8 plugin
+### 2.2. As a _flake8_ plugin
 
-Once you install `pydoclint` you will have also installed `flake8`. Then you can run:
+Once you install _pydoclint_ you will have also installed _flake8_. Then you
+can run:
 
 ```
 flake8 --select=DOC <FILE_OR_FOLDER>
 ```
 
-If you don't include `--select=DOC` in your command, `flake8` will also run other built-in flake8 linters on your code.
+If you don't include `--select=DOC` in your command, _flake8_ will also run
+other built-in _flake8_ linters on your code.
+
+### 2.3. Native vs _flake8_
+
+Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
+Here's comparison:
+
+|                 | Pros                                       | Cons                                                          |
+| --------------- | ------------------------------------------ | ------------------------------------------------------------- |
+| Native tool     | Slightly faster                            | No per-line or project-wide omission support right now [*]    |
+| _flake8_ plugin | Supports per-line or project-wide omission | Slightly slower because other flake8 plugins are run together |
+
+\*) This feature may be added in the near future
 
 ## 3. Style violation codes
 
 `pydoclint` currently has the following style violation codes:
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
@@ -97,60 +107,97 @@
 | Code     | Explanation                                                                                               |
 | -------- | --------------------------------------------------------------------------------------------------------- |
 | `DOC501` | Function/method has "raise" statements, but the docstring does not have a "Raises" section                |
 | `DOC502` | Function/method has a "Raises" section in the docstring, but there are not "raise" statements in the body |
 
 ## 4. Configuration options
 
-There are several configuration options available. They can be used invidually or together.
+There are several configuration options available. They can be used invidually
+or together.
+
+### 4.1. `--quiet` (shortform: `-q`)
+
+This flag activates the "quite mode", in which no output will be printed to the
+command line if there are no violations.
+
+By default, this flag is _not_ activated, so the files that are scanned are
+printed in the command line.
+
+```
+pydoclint --quiet <FILE_OR_FOLDER>
+```
+
+This option is only available in the "native" command-line mode, rather than in
+flake8. If you use pydoclint in flake8, please use flake8's own verbosity
+configuration instead.
+
+### 4.2. `--exclude`
+
+You can use this option to exclude files within the given folder. It is a regex
+pattern of full file paths.
+
+For example:
+
+```
+pydoclint --exclude='\.git|\.tox|tests/data' <FOLDER_NAME>
+```
+
+This option is only available in the native command-line mode. If you use
+_pydoclint_ within _flake8_, you can use _flake8_'s
+[`--exclude` option](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-exclude).
 
-### 4.1. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.3. `--check-type-hint` (shortform: `-th`, default: `True`)
 
-If `True`, the type hints in the docstring and in the Python code need to exactly match.
+If `True`, the type hints in the docstring and in the Python code need to
+exactly match.
 
 To turn this optoin on/off, do this:
 
 ```
 pydoclint --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
 or
 
 ```
 flake8 --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
-### 4.2. `--check-arg-order` (shortform: `-ao`, default: `True`)
+### 4.4. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
-If `True`, the input argument order in the docstring needs to match that in the function signature.
+If `True`, the input argument order in the docstring needs to match that in the
+function signature.
 
 To turn this optoin on/off, do this:
 
 ```
 pydoclint --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
 or
 
 ```
 flake8 --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
-### 4.3. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
+### 4.5. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
-If `True`, `pydoclint` won't check functions that have only a short description in their docstring.
+If `True`, `pydoclint` won't check functions that have only a short description
+in their docstring.
 
 To turn this optoin on/off, do this:
 
 ```
 pydoclint --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
 or
 
 ```
 flake8 --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
+### 4.6. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
-If `True`, `pydoclint` won't report `DOC501` or `DOC502` if there are `raise` statements in the function/method but there aren't any "raises" sections in the docstring (or vice versa).
+If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
+statements in the function/method but there aren't any "raises" sections in the
+docstring (or vice versa).
```

### Comparing `pydoclint-0.0.1/pydoclint/arg.py` & `pydoclint-0.0.2/pydoclint/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/pydoclint/flake8_entry.py` & `pydoclint-0.0.2/pydoclint/flake8_entry.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/pydoclint/main.py` & `pydoclint-0.0.2/pydoclint/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import re
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 import click
 
 from pydoclint.violation import Violation
 from pydoclint.visitor import Visitor
@@ -17,14 +18,32 @@
 @click.option(
     '-s',
     '--src',
     type=str,
     help='The source code to check',
 )
 @click.option(
+    '-q',
+    '--quiet',
+    is_flag=True,
+    default=False,
+    help='If True, do not print the file names being checked to the terminal.',
+)
+@click.option(
+    '--exclude',
+    type=str,
+    show_default=True,
+    default=r'\.git|\.tox',
+    help=(
+        'Regex pattern to exclude files/folders. Please add quotes (both'
+        ' double and single quotes are fine) around the regex in the'
+        ' command line.'
+    ),
+)
+@click.option(
     '-th',
     '--check-type-hint',
     type=bool,
     show_default=True,
     default=True,
     help='Whether to check type hints in docstrings',
 )
@@ -63,14 +82,16 @@
         allow_dash=True,
     ),
     is_eager=True,
 )
 @click.pass_context
 def main(
         ctx: click.Context,
+        quiet: bool,
+        exclude: str,
         src: Optional[str],
         paths: Tuple[str, ...],
         check_type_hint: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
 ) -> None:
@@ -87,68 +108,90 @@
     if not paths and src is None:
         click.echo(
             main.get_usage(ctx) + "\n\nOne of 'paths' or 'src' is required."
         )
         ctx.exit(1)
 
     violationsInAllFiles: Dict[str, List[Violation]] = _checkPaths(
+        quiet=quiet,
+        exclude=exclude,
         paths=paths,
         checkTypeHint=check_type_hint,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
     )
 
+    violationCounter: int = 0
     if len(violationsInAllFiles) > 0:
         counter = 0
         for filename, violationsInThisFile in violationsInAllFiles.items():
             counter += 1
             if len(violationsInThisFile) > 0:
                 if counter > 1:
                     print('')
 
                 click.echo(click.style(filename, fg='yellow', bold=True))
                 for violation in violationsInThisFile:
+                    violationCounter += 1
                     fourSpaces = '    '
                     click.echo(fourSpaces, nl=False)
                     click.echo(f'{violation.line}: ', nl=False)
                     click.echo(
                         click.style(
                             f'{violation.fullErrorCode}',
                             fg='red',
                             bold=True,
                         ),
                         nl=False,
                     )
                     click.echo(f': {violation.msg}')
 
+    if violationCounter > 0:
         ctx.exit(1)
+    else:
+        if not quiet:
+            click.echo(click.style('🎉 No violations 🎉', fg='green', bold=True))
 
-    ctx.exit(0)
+        ctx.exit(0)
 
 
 def _checkPaths(
         paths: Tuple[str, ...],
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
+        quiet: bool = False,
+        exclude: str = '',
 ) -> Dict[str, List[Violation]]:
     filenames: List[Path] = []
 
+    if not quiet:
+        skipMsg = f'Skipping files that match this pattern: {exclude}'
+        click.echo(click.style(skipMsg, fg='yellow', bold=True))
+
+    excludePattern = re.compile(exclude)
+
     for path_ in paths:
         path = Path(path_)
         if path.is_file():
             filenames.append(path)
         elif path.is_dir():
             filenames.extend(sorted(path.rglob('*.py')))
 
     allViolations: Dict[str, List[Violation]] = {}
 
     for filename in filenames:
+        if excludePattern.search(filename.as_posix()):
+            continue
+
+        if not quiet:
+            click.echo(click.style(filename, fg='cyan', bold=True))
+
         violationsInThisFile: List[Violation] = _checkFile(
             filename,
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydoclint-0.0.1/pydoclint/utils/annotation.py` & `pydoclint-0.0.2/pydoclint/utils/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     if isinstance(node, ast.Index):
         return parseAnnotation(node.value)
 
     if isinstance(node, ast.Tuple):
         return ', '.join(map(parseAnnotation, node.elts))
 
     if isinstance(node, ast.Constant):
+        if isinstance(node, ast.Ellipsis):  # Ellipsis is Constant's subclass
+            return '...'
+
         return str(node.value)
 
     if isinstance(node, ast.BinOp) and isinstance(node.op, ast.BitOr):
         return f'{parseAnnotation(node.left)} | {parseAnnotation(node.right)}'
 
     if isinstance(node, ast.Attribute):
         prefix: str = parseAnnotation(node.value)
```

### Comparing `pydoclint-0.0.1/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.2/pydoclint/utils/return_yield_raise.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/pydoclint/utils/walk.py` & `pydoclint-0.0.2/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/pydoclint/violation.py` & `pydoclint-0.0.2/pydoclint/violation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/pydoclint/visitor.py` & `pydoclint-0.0.2/pydoclint/visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from numpydoc.docscrape import NumpyDocString, Parameter
 
 from pydoclint.arg import Arg, ArgList
 from pydoclint.method_type import MethodType
 from pydoclint.utils.astTypes import FuncOrAsyncFuncDef
 from pydoclint.utils.generic import (
+    collectFuncArgs,
     detectMethodType,
     generateMsgPrefix,
     getDocstring,
     isShortDocstring,
 )
 from pydoclint.utils.return_yield_raise import (
     hasGeneratorAsReturnAnnotation,
@@ -161,15 +162,15 @@
             The parsed docstring structure.
 
         Returns
         -------
         List[Violation]
             A list of argument violations
         """
-        argList: List[ast.arg] = list(node.args.args)
+        argList: List[ast.arg] = collectFuncArgs(node)
 
         isMethod: bool = isinstance(parent_, ast.ClassDef)
         msgPrefix: str = generateMsgPrefix(node, parent_, appendColon=True)
 
         if isMethod:
             mType: MethodType = detectMethodType(node)
             if mType in {MethodType.INSTANCE_METHOD, MethodType.CLASS_METHOD}:
```

### Comparing `pydoclint-0.0.1/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,87 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.1
+Version: 0.0.2
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydoclint
 
-A Python docstring linter to check whether a docstring's sections (arguments, returns, raises, ...) match the function signature or function implementation.
+A Python docstring linter to check whether a docstring's sections (arguments,
+returns, raises, ...) match the function signature or function implementation.
 
-It runs really fast. In fact, it is at least 30,000 times faster than [darglint](https://github.com/terrencepreilly/darglint) (another linter of the same purposes which is no longer maintained).
+It runs really fast. In fact, it is at least ~1,475 times faster than
+[darglint](https://github.com/terrencepreilly/darglint) (another linter of the
+same purposes which is no longer maintained).
+
+Here is a comparison of linting time on some famous Python projects:
+
+|                                                              | pydoclint | darglint                          |
+| ------------------------------------------------------------ | --------- | --------------------------------- |
+| [numpy](https://github.com/numpy/numpy)                      | 2.0 sec   | 49 min 9 sec (1,475x slower)      |
+| [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 2.4 sec   | 3 hr 5 min 33 sec (4,639x slower) |
+
+Currently, _pydoclint_ only works when you write your docstrings in the
+[numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support
+for the
+[Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html)
+docstrings will be added soon.
 
-Here is a comparison of running time on some famous Python projects:
-
-|                                                              | pydoclint | darglint             |
-| ------------------------------------------------------------ | --------- | -------------------- |
-| [numpy](https://github.com/numpy/numpy)                      | 0.08 sec  | > 40 min (> 30,000x) |
-| [scikit-learn](https://github.com/scikit-learn/scikit-learn) | 0.09 sec  | > 40 min (> 30,000x) |
-
-Currently, `pydoclint` only works when you write your docstrings in the [numpy stlyle](https://numpydoc.readthedocs.io/en/latest/format.html). Support for the [Google style](https://www.sphinx-doc.org/en/master/usage/extensions/example_google.html) docstrings will be added soon.
-
-**Note**: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle) serves complementary purposes. It is recommended that you use both together.
+Another note: this linter and [pydocstyle](https://github.com/PyCQA/pydocstyle)
+serves complementary purposes. It is recommended that you use both together.
 
 ## 1. Installation
 
 ```
 pip install pydoclint
 ```
 
-Note that `pydoclint` only supports Python 3.8 and above.
+Note that _pydoclint_ currently only supports Python 3.8 and above. (Python 3.7
+support may be added if there are interests and requests.)
 
 ## 2. Usage
 
-### 2.1. As a standalone command line tool
+### 2.1. As a native command line tool
 
 ```
 pydoclint <FILE_OR_FOLDER>
 ```
 
 Replace `<FILE_OR_FOLDER>` with the file/folder names you want, such as `.`.
 
-### 2.2. As a flake8 plugin
+### 2.2. As a _flake8_ plugin
 
-Once you install `pydoclint` you will have also installed `flake8`. Then you can run:
+Once you install _pydoclint_ you will have also installed _flake8_. Then you
+can run:
 
 ```
 flake8 --select=DOC <FILE_OR_FOLDER>
 ```
 
-If you don't include `--select=DOC` in your command, `flake8` will also run other built-in flake8 linters on your code.
+If you don't include `--select=DOC` in your command, _flake8_ will also run
+other built-in _flake8_ linters on your code.
+
+### 2.3. Native vs _flake8_
+
+Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
+Here's comparison:
+
+|                 | Pros                                       | Cons                                                          |
+| --------------- | ------------------------------------------ | ------------------------------------------------------------- |
+| Native tool     | Slightly faster                            | No per-line or project-wide omission support right now [*]    |
+| _flake8_ plugin | Supports per-line or project-wide omission | Slightly slower because other flake8 plugins are run together |
+
+\*) This feature may be added in the near future
 
 ## 3. Style violation codes
 
 `pydoclint` currently has the following style violation codes:
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
@@ -97,60 +120,97 @@
 | Code     | Explanation                                                                                               |
 | -------- | --------------------------------------------------------------------------------------------------------- |
 | `DOC501` | Function/method has "raise" statements, but the docstring does not have a "Raises" section                |
 | `DOC502` | Function/method has a "Raises" section in the docstring, but there are not "raise" statements in the body |
 
 ## 4. Configuration options
 
-There are several configuration options available. They can be used invidually or together.
+There are several configuration options available. They can be used invidually
+or together.
+
+### 4.1. `--quiet` (shortform: `-q`)
+
+This flag activates the "quite mode", in which no output will be printed to the
+command line if there are no violations.
+
+By default, this flag is _not_ activated, so the files that are scanned are
+printed in the command line.
+
+```
+pydoclint --quiet <FILE_OR_FOLDER>
+```
+
+This option is only available in the "native" command-line mode, rather than in
+flake8. If you use pydoclint in flake8, please use flake8's own verbosity
+configuration instead.
+
+### 4.2. `--exclude`
+
+You can use this option to exclude files within the given folder. It is a regex
+pattern of full file paths.
+
+For example:
+
+```
+pydoclint --exclude='\.git|\.tox|tests/data' <FOLDER_NAME>
+```
+
+This option is only available in the native command-line mode. If you use
+_pydoclint_ within _flake8_, you can use _flake8_'s
+[`--exclude` option](https://flake8.pycqa.org/en/latest/user/options.html#cmdoption-flake8-exclude).
 
-### 4.1. `--check-type-hint` (shortform: `-th`, default: `True`)
+### 4.3. `--check-type-hint` (shortform: `-th`, default: `True`)
 
-If `True`, the type hints in the docstring and in the Python code need to exactly match.
+If `True`, the type hints in the docstring and in the Python code need to
+exactly match.
 
 To turn this optoin on/off, do this:
 
 ```
 pydoclint --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
 or
 
 ```
 flake8 --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
-### 4.2. `--check-arg-order` (shortform: `-ao`, default: `True`)
+### 4.4. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
-If `True`, the input argument order in the docstring needs to match that in the function signature.
+If `True`, the input argument order in the docstring needs to match that in the
+function signature.
 
 To turn this optoin on/off, do this:
 
 ```
 pydoclint --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
 or
 
 ```
 flake8 --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
-### 4.3. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
+### 4.5. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
-If `True`, `pydoclint` won't check functions that have only a short description in their docstring.
+If `True`, `pydoclint` won't check functions that have only a short description
+in their docstring.
 
 To turn this optoin on/off, do this:
 
 ```
 pydoclint --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
 or
 
 ```
 flake8 --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
-### 4.4. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
+### 4.6. `--skip-checking-raises` (shortform: `-scr`, default: `False`)
 
-If `True`, `pydoclint` won't report `DOC501` or `DOC502` if there are `raise` statements in the function/method but there aren't any "raises" sections in the docstring (or vice versa).
+If `True`, _pydoclint_ won't report `DOC501` or `DOC502` if there are `raise`
+statements in the function/method but there aren't any "raises" sections in the
+docstring (or vice versa).
```

### Comparing `pydoclint-0.0.1/pydoclint.egg-info/SOURCES.txt` & `pydoclint-0.0.2/pydoclint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/setup.cfg` & `pydoclint-0.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.1
+version = 0.0.2
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers =
```

### Comparing `pydoclint-0.0.1/tests/test_arg.py` & `pydoclint-0.0.2/tests/test_arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.1/tests/test_main.py` & `pydoclint-0.0.2/tests/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -356,14 +356,46 @@
         'are not "raise" statements in the body ',
     ]
     expected1 = []
     expected = expected1 if skipRaisesCheck else expected0
     assert list(map(str, violations)) == expected
 
 
+def testStarsInArgumentList() -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / 'star_args/cases.py',
+    )
+    expected = [
+        'DOC103: Function `func2`: Docstring arguments are different from function '
+        'arguments. (Or did you miss the space between the argument name and the ":" '
+        'in the docstring?). Arguments in the function signature but not in the '
+        'docstring: [**kwargs: ]. Arguments in the docstring but not in the function '
+        'signature: [kwargs: ].',
+        'DOC103: Function `func4`: Docstring arguments are different from function '
+        'arguments. (Or did you miss the space between the argument name and the ":" '
+        'in the docstring?). Arguments in the function signature but not in the '
+        'docstring: [*args: ]. Arguments in the docstring but not in the function '
+        'signature: [args: ].',
+        'DOC101: Function `func6`: Docstring contains fewer arguments than in '
+        'function signature. ',
+        'DOC103: Function `func6`: Docstring arguments are different from function '
+        'arguments. (Or did you miss the space between the argument name and the ":" '
+        'in the docstring?). Arguments in the function signature but not in the '
+        'docstring: [**kwargs: , *args: ].',
+        'DOC101: Function `func7`: Docstring contains fewer arguments than in '
+        'function signature. ',
+        'DOC103: Function `func7`: Docstring arguments are different from function '
+        'arguments. (Or did you miss the space between the argument name and the ":" '
+        'in the docstring?). Arguments in the function signature but not in the '
+        'docstring: [**kwargs: , *args: , arg1: float, arg2: str]. Arguments in the '
+        'docstring but not in the function signature: [arg1: int, arg2: dict].',
+    ]
+    assert list(map(str, violations)) == expected
+
+
 def testPlayground() -> None:
     """
     This is a placeholder test for testing the `playground.py` file.
 
     When you want to quickly test something, you can add contents into
     tests/data/playground.py and run this test function.
     """
```

