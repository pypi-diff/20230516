# Comparing `tmp/test_stages-0.1.1.tar.gz` & `tmp/test_stages-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_stages-0.1.1.tar", last modified: Tue Feb  7 07:18:23 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `test_stages-0.1.1.tar` & `test_stages-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,39 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/.config/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/.config/ruff-all/
--rw-r--r--   0 roam      (1000) roam      (1000)       68 2023-02-05 11:39:12.000000 test_stages-0.1.1/.config/ruff-all/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/.config/ruff-base/
--rw-r--r--   0 roam      (1000) roam      (1000)      637 2023-02-05 13:03:05.000000 test_stages-0.1.1/.config/ruff-base/pyproject.toml
--rw-r--r--   0 roam      (1000) roam      (1000)      428 2023-01-23 20:55:33.000000 test_stages-0.1.1/.editorconfig
--rw-r--r--   0 roam      (1000) roam      (1000)      754 2023-02-07 07:14:42.000000 test_stages-0.1.1/CHANGELOG.md
--rw-r--r--   0 roam      (1000) roam      (1000)      201 2023-02-07 07:08:45.000000 test_stages-0.1.1/MANIFEST.in
--rw-r--r--   0 roam      (1000) roam      (1000)     3614 2023-02-07 07:18:23.378913 test_stages-0.1.1/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     2124 2023-02-05 16:29:27.000000 test_stages-0.1.1/README.md
--rw-r--r--   0 roam      (1000) roam      (1000)     3434 2023-02-07 06:35:20.000000 test_stages-0.1.1/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/requirements/
--rw-r--r--   0 roam      (1000) roam      (1000)      211 2023-02-07 00:29:38.000000 test_stages-0.1.1/requirements/install.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       17 2023-02-07 00:28:22.000000 test_stages-0.1.1/requirements/test.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      151 2023-02-07 07:18:23.378913 test_stages-0.1.1/setup.cfg
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/src/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/src/test_stages/
--rw-r--r--   0 roam      (1000) roam      (1000)     1431 2023-02-07 07:08:04.000000 test_stages-0.1.1/src/test_stages/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     7518 2023-02-05 16:04:01.000000 test_stages-0.1.1/src/test_stages/cmd.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2023-01-23 18:35:00.000000 test_stages-0.1.1/src/test_stages/py.typed
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/src/test_stages/tox_stages/
--rw-r--r--   0 roam      (1000) roam      (1000)      184 2023-02-05 11:53:36.000000 test_stages-0.1.1/src/test_stages/tox_stages/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4612 2023-02-07 01:00:55.000000 test_stages-0.1.1/src/test_stages/tox_stages/__main__.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/src/test_stages.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)     3614 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)      822 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       99 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/entry_points.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      178 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/requires.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       25 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-02-07 07:18:23.000000 test_stages-0.1.1/src/test_stages.egg-info/zip-safe
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/src/tox_trivtags/
--rw-r--r--   0 roam      (1000) roam      (1000)     2106 2023-02-07 00:56:46.000000 test_stages-0.1.1/src/tox_trivtags/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4844 2023-02-05 15:38:29.000000 test_stages-0.1.1/src/tox_trivtags/parse.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2022-11-10 07:08:36.000000 test_stages-0.1.1/src/tox_trivtags/py.typed
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/stubs/
--rw-r--r--   0 roam      (1000) roam      (1000)      449 2023-02-05 15:09:55.000000 test_stages-0.1.1/stubs/contextlib_chdir.pyi
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/stubs/tox/
--rw-r--r--   0 roam      (1000) roam      (1000)      236 2023-02-05 13:29:57.000000 test_stages-0.1.1/stubs/tox/__init__.pyi
--rw-r--r--   0 roam      (1000) roam      (1000)      450 2023-02-05 13:29:42.000000 test_stages-0.1.1/stubs/tox/config.pyi
--rw-r--r--   0 roam      (1000) roam      (1000)     3354 2023-02-07 06:30:21.000000 test_stages-0.1.1/tox.ini
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-07 07:18:23.378913 test_stages-0.1.1/unit_tests/
--rw-r--r--   0 roam      (1000) roam      (1000)       79 2023-02-05 11:53:25.000000 test_stages-0.1.1/unit_tests/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4482 2023-02-07 00:48:58.000000 test_stages-0.1.1/unit_tests/test_functional.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 test_stages-0.1.2/.editorconfig
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 test_stages-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 test_stages-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 test_stages-0.1.2/tox.ini
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 test_stages-0.1.2/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 test_stages-0.1.2/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 test_stages-0.1.2/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 test_stages-0.1.2/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 test_stages-0.1.2/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 test_stages-0.1.2/config/ruff-most/pyproject.toml
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 test_stages-0.1.2/docs/changes.md
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 test_stages-0.1.2/docs/index.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 test_stages-0.1.2/docs/cmd/index.md
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 test_stages-0.1.2/docs/cmd/tox-stages.md
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 test_stages-0.1.2/docs/man/tox-stages.1
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 test_stages-0.1.2/requirements/docs.txt
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 test_stages-0.1.2/requirements/install.txt
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 test_stages-0.1.2/requirements/selftest.txt
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 test_stages-0.1.2/requirements/test.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/selftest/__init__.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/selftest/__main__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/test_stages/__init__.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/test_stages/cmd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/test_stages/py.typed
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/test_stages/tox_stages/__init__.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/test_stages/tox_stages/__main__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/tox_trivtags/__init__.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/tox_trivtags/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_stages-0.1.2/src/tox_trivtags/py.typed
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 test_stages-0.1.2/stubs/contextlib_chdir.pyi
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 test_stages-0.1.2/stubs/pyproject_hooks.pyi
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 test_stages-0.1.2/stubs/tox/__init__.pyi
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 test_stages-0.1.2/stubs/tox/config.pyi
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 test_stages-0.1.2/unit_tests/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 test_stages-0.1.2/unit_tests/test_functional.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 test_stages-0.1.2/.gitignore
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 test_stages-0.1.2/README.md
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 test_stages-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 test_stages-0.1.2/PKG-INFO
```

### Comparing `test_stages-0.1.1/PKG-INFO` & `test_stages-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: test_stages
-Version: 0.1.1
+Version: 0.1.2
 Summary: Group Tox, Nox, etc environments into stages, run them in parallel
-Author-email: Peter Pentchev <roam@ringlet.net>
-Project-URL: Homepage, https://gitlab.com/ppentchev/test-stages
-Project-URL: Changes, https://gitlab.com/ppentchev/test-stages/-/blob/main/CHANGELOG.md
+Project-URL: Homepage, https://devel.ringlet.net/devel/test-stages
+Project-URL: Changes, https://devel.ringlet.net/devel/test-stages/changes/
 Project-URL: Issue Tracker, https://gitlab.com/ppentchev/test-stages/-/issues
 Project-URL: Source Code, https://gitlab.com/ppentchev/test-stages
+Author-email: Peter Pentchev <roam@ringlet.net>
+License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: License :: Freely Distributable
 Classifier: License :: OSI Approved
@@ -24,17 +25,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Requires-Dist: click<9,>=8
+Requires-Dist: distlib<0.4,>=0.3.6
+Requires-Dist: parse-stages<0.2,>=0.1.4
+Requires-Dist: pyparsing<4,>=3
+Requires-Dist: tomli<3,>=2; python_version < '3.11'
+Requires-Dist: utf8-locale<2,>=1
 Provides-Extra: tox
+Requires-Dist: tox<4,>=3; extra == 'tox'
+Description-Content-Type: text/markdown
+
+<!--
+SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+SPDX-License-Identifier: BSD-2-Clause
+-->
 
 # Run Tox tests in groups, stopping on errors
 
 The `test-stages` library provides command-line tools that wrap
 Python test environment runners such as [Tox][tox] or [Nox][nox],
 invoking them so as the various tests are run in parallel, in groups,
 as specified on the command line. This allows the fastest tests to be run
@@ -61,21 +75,19 @@
 If the `tox-stages run` command is invoked without any stage specifications,
 the tool looks for the `stages` list of strings in the `[tool.test-stages]`
 section of the `pyproject.toml` file:
 
     [tool.test-stages]
     stages = ["ruff and not @manual", "@check", "@tests"]
 
-Note that the `tox-stages` tool only supports Tox version 3 for the present.
-
 ## Author
 
 The `test-stages` library is developed by [Peter Pentchev][roam] in
 [a GitLab repository][gitlab].
 
 [flake8]: https://github.com/pycqa/flake8 "The flake8 Python syntax and style checker"
 [gitlab]: https://gitlab.com/ppentchev/test-stages "The test-stages GitLab repository"
 [nox]: https://nox.thea.codes/ "The Nox test runner"
-[parse-stages]: https://gitlab.com/ppentchev/parse-stages "Parse a mini-language for selecting objects by tag or name"
+[parse-stages]: https://devel.ringlet.net/devel/parse-stages "Parse a mini-language for selecting objects by tag or name"
 [roam]: mailto:roam@ringlet.net "Peter Pentchev"
 [ruff]: https://github.com/charliermarsh/ruff "Ruff, the extremely fast Python linter"
 [tox]: https://tox.wiki/ "The Tox automation project"
```

### Comparing `test_stages-0.1.1/README.md` & `test_stages-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<!--
+SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+SPDX-License-Identifier: BSD-2-Clause
+-->
+
 # Run Tox tests in groups, stopping on errors
 
 The `test-stages` library provides command-line tools that wrap
 Python test environment runners such as [Tox][tox] or [Nox][nox],
 invoking them so as the various tests are run in parallel, in groups,
 as specified on the command line. This allows the fastest tests to be run
 first, and the slower ones to only be started if it makes sense (e.g. if
@@ -27,21 +32,19 @@
 If the `tox-stages run` command is invoked without any stage specifications,
 the tool looks for the `stages` list of strings in the `[tool.test-stages]`
 section of the `pyproject.toml` file:
 
     [tool.test-stages]
     stages = ["ruff and not @manual", "@check", "@tests"]
 
-Note that the `tox-stages` tool only supports Tox version 3 for the present.
-
 ## Author
 
 The `test-stages` library is developed by [Peter Pentchev][roam] in
 [a GitLab repository][gitlab].
 
 [flake8]: https://github.com/pycqa/flake8 "The flake8 Python syntax and style checker"
 [gitlab]: https://gitlab.com/ppentchev/test-stages "The test-stages GitLab repository"
 [nox]: https://nox.thea.codes/ "The Nox test runner"
-[parse-stages]: https://gitlab.com/ppentchev/parse-stages "Parse a mini-language for selecting objects by tag or name"
+[parse-stages]: https://devel.ringlet.net/devel/parse-stages "Parse a mini-language for selecting objects by tag or name"
 [roam]: mailto:roam@ringlet.net "Peter Pentchev"
 [ruff]: https://github.com/charliermarsh/ruff "Ruff, the extremely fast Python linter"
 [tox]: https://tox.wiki/ "The Tox automation project"
```

### Comparing `test_stages-0.1.1/pyproject.toml` & `test_stages-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
+
 [build-system]
-requires = ["setuptools >= 61", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = [
+  "hatchling >= 1.8, < 2",
+  "hatch-requirements-txt >= 0.3, < 0.5",
+]
+build-backend = "hatchling.build"
 
 [project]
 name = "test_stages"
 description = "Group Tox, Nox, etc environments into stages, run them in parallel"
 readme = "README.md"
+license = {text = "BSD-2-Clause"}
 requires-python = ">= 3.8"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Environment :: Console",
   "Framework :: tox",
   "Intended Audience :: Developers",
   "License :: DFSG approved",
@@ -25,14 +32,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development",
   "Topic :: Software Development :: Testing",
   "Topic :: Software Development :: Testing :: Unit",
   "Topic :: Utilities",
+  "Typing :: Typed",
 ]
 dynamic = ["dependencies", "version"]
 
 [[project.authors]]
 name = "Peter Pentchev"
 email = "roam@ringlet.net"
 
@@ -42,56 +50,54 @@
 [project.optional-dependencies]
 tox = ["tox >= 3, < 4"]
 
 [project.scripts]
 tox-stages = "test_stages.tox_stages.__main__:main"
 
 [project.urls]
-Homepage = "https://gitlab.com/ppentchev/test-stages"
-Changes = "https://gitlab.com/ppentchev/test-stages/-/blob/main/CHANGELOG.md"
+Homepage = "https://devel.ringlet.net/devel/test-stages"
+Changes = "https://devel.ringlet.net/devel/test-stages/changes/"
 "Issue Tracker" = "https://gitlab.com/ppentchev/test-stages/-/issues"
 "Source Code" = "https://gitlab.com/ppentchev/test-stages"
 
-[tool.setuptools]
-zip-safe = true
-package-dir = {"" = "src"}
-packages = ["test_stages", "test_stages.tox_stages", "tox_trivtags"]
-
-[tool.setuptools.package-data]
-test_stages = ["py.typed"]
-tox_trivtags = ["py.typed"]
-
-[tool.setuptools.dynamic]
-dependencies = {file = "requirements/install.txt"}
-version = {attr = "test_stages.VERSION"}
+[tool.hatch.build.targets.wheel]
+packages = ["src/test_stages", "src/tox_trivtags"]
+
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements/install.txt"]
+
+[tool.hatch.version]
+path = "src/test_stages/__init__.py"
 
 [tool.black]
+target-version = ["py38", "py39", "py310", "py311"]
 line-length = 100
 
 [tool.mypy]
 strict = true
 python_version = "3.8"
 
 # This is the list of the Pylint 2.16.1 default plugins.
 [tool.pylint]
+py-version = "3.8"
 load-plugins = [
   "pylint.extensions.bad_builtin",
   "pylint.extensions.broad_try_clause",
   "pylint.extensions.check_elif",
   "pylint.extensions.code_style",
   # "pylint.extensions.comparetozero",  # clarity
   "pylint.extensions.comparison_placement",
   "pylint.extensions.confusing_elif",
   "pylint.extensions.consider_refactoring_into_while_condition",
   "pylint.extensions.consider_ternary_expression",
   "pylint.extensions.dict_init_mutate",
   "pylint.extensions.docparams",
   "pylint.extensions.docstyle",
   "pylint.extensions.dunder",
-  # "pylint.extensions.empty_comment",  # the copyright notices trigger that one
+  "pylint.extensions.empty_comment",
   "pylint.extensions.emptystring",
   "pylint.extensions.eq_without_hash",
   "pylint.extensions.for_any_all",
   "pylint.extensions.magic_value",
   "pylint.extensions.mccabe",
   "pylint.extensions.no_self_use",
   "pylint.extensions.overlapping_exceptions",
@@ -104,13 +110,9 @@
 ]
 
 [tool.pylint.main]
 disable = [
   "consider-using-assignment-expr",
 ]
 
-[tool.ruff]
-extend = ".config/ruff-base/pyproject.toml"
-select = ["E", "F"]
-
 [tool.test-stages]
-stages = ["ruff", "@check", "@tests"]
+stages = ["ruff and not @manual", "@check and not @manual", "@tests and not @manual"]
```

### Comparing `test_stages-0.1.1/src/test_stages/__init__.py` & `test_stages-0.1.2/LICENSES/BSD-2-Clause.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,9 @@
-# Copyright (c) Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
-#
-"""Run `tox` on several groups of environments, stopping on errors."""
+Copyright (c) <year> <owner> 
 
-VERSION = "0.1.1"
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `test_stages-0.1.1/src/test_stages/cmd.py` & `test_stages-0.1.2/src/test_stages/cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,69 @@
-# Copyright (c) Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
-#
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
 """Command-line tool helpers for the various test-stages implementations."""
 
 from __future__ import annotations
 
 import dataclasses
 import functools
 import pathlib
 import sys
-
-from collections.abc import Callable
-from typing import Any, Final, NamedTuple, TypeVar
+from typing import TYPE_CHECKING, NamedTuple
 
 import click
 import parse_stages as parse
 import utf8_locale
 
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
+    from typing import Any, Final, TypeVar
+
+    # pylint: disable-next=invalid-name
+    _T = TypeVar("_T")
+
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 
 TestEnv = parse.TaggedFrozen
 
 
 class Stage(NamedTuple):
     """A stage specification and its boolean expression."""
 
     spec: str
     expr: parse.BoolExpr
+    parallel: bool
+
+
+class TestStage(NamedTuple):
+    """A final representation of a test stage: the environments to run and some attributes."""
+
+    envlist: list[TestEnv]
+    """The list of environments to run at this stage."""
+
+    parallel: bool
+    """Run the environments in parallel."""
+
+
+class StagesList:
+    """Parse the `--parallel` command-line option argument into a set."""
+
+    # pylint: disable=too-few-public-methods
+
+    stages: set[int]
+    """The selected stages, 1-based."""
+
+    def __init__(self, value: str) -> None:
+        """Record the selected set of stages."""
+        self.stages = set(parse.parse_stage_ids(value))
 
 
 @dataclasses.dataclass(frozen=True)
 class Config:
     """Runtime configuration for the test runner tool."""
 
     filename: pathlib.Path
@@ -69,46 +77,42 @@
 @dataclasses.dataclass
 class ConfigHolder:
     """Hold a Config object."""
 
     cfg: Config | None = None
 
 
-# pylint: disable-next=invalid-name
-_T = TypeVar("_T")
-
-
 def _split_by(current: list[_T], func: Callable[[_T], bool]) -> tuple[list[_T], list[_T]]:
     """Split an ordered list of items in two by the given predicate."""
     res: Final[tuple[list[_T], list[_T]]] = ([], [])
     for stage in current:
         if func(stage):
             res[1].append(stage)
         else:
             res[0].append(stage)
     return res
 
 
-def select_stages(cfg: Config, all_stages: list[TestEnv]) -> list[list[TestEnv]]:
+def select_stages(cfg: Config, all_stages: list[TestEnv]) -> list[TestStage]:
     """Group the stages as specified."""
 
     def process_stage(
-        acc: tuple[list[list[TestEnv]], list[TestEnv]], stage: Stage
-    ) -> tuple[list[list[TestEnv]], list[TestEnv]]:
+        acc: tuple[list[TestStage], list[TestEnv]], stage: Stage
+    ) -> tuple[list[TestStage], list[TestEnv]]:
         """Stash the environments matched by a stage specification."""
         res, current = acc
         if not current:
             sys.exit(f"No test environments left for {stage.spec}")
         left, matched = _split_by(current, stage.expr.evaluate)
         if not matched:
             sys.exit(f"No test environments matched by {stage.spec}")
-        res.append(matched)
+        res.append(TestStage(envlist=matched, parallel=stage.parallel))
         return res, left
 
-    res_init: Final[list[list[TestEnv]]] = []
+    res_init: Final[list[TestStage]] = []
     return functools.reduce(process_stage, cfg.stages, (res_init, list(all_stages)))[0]
 
 
 def extract_cfg(ctx: click.Context) -> Config:
     """Extract the Config object from the ConfigHolder."""
     cfg_hold: Final = ctx.find_object(ConfigHolder)
     # mypy needs these assertions
@@ -152,39 +156,61 @@
             sys.exit(0 if handler(extract_cfg(ctx)) else 1)
 
         return real_available
 
     return inner
 
 
-def click_run() -> Callable[[Callable[[Config, list[list[TestEnv]]], None]], click.Command]:
+def click_run() -> Callable[[Callable[[Config, list[TestStage], list[str]], None]], click.Command]:
     """Wrap a run() function, preparing the configuration."""
 
-    def inner(handler: Callable[[Config, list[list[TestEnv]]], None]) -> click.Command:
+    def inner(handler: Callable[[Config, list[TestStage], list[str]], None]) -> click.Command:
         """Wrap the run function."""
 
         @click.command(name="run")
+        @click.option(
+            "-A",
+            "--arg",
+            type=str,
+            multiple=True,
+            help=(
+                "an additional argument to pass to the test runner; "
+                "may be specified multiple times"
+            ),
+        )
+        @click.option(
+            "-p",
+            "--parallel",
+            type=StagesList,
+            help="specify which stages to run in parallel (e.g. '1,4-6')",
+        )
         @click.argument("stages_spec", nargs=-1, required=False, type=str)
         @click.pass_context
-        def real_run(ctx: click.Context, stages_spec: list[str]) -> None:
+        def real_run(
+            ctx: click.Context, arg: list[str], parallel: StagesList | None, stages_spec: list[str]
+        ) -> None:
             """Run the test environments in stages."""
             cfg_base: Final = extract_cfg(ctx)
             if not stages_spec:
                 pyproj: Final = _find_and_load_pyproject(cfg_base.filename.parent)
                 stages_spec = pyproj.get("tool", {}).get("test-stages", {}).get("stages", [])
                 if not stages_spec:
                     sys.exit("No stages specified either on the command line or in pyproject.toml")
 
+            pstages: Final = set(range(len(stages_spec))) if parallel is None else parallel.stages
             cfg: Final = dataclasses.replace(
                 cfg_base,
-                stages=[Stage(spec, parse.parse_spec(spec)) for spec in stages_spec],
+                stages=[
+                    Stage(spec, parse.parse_spec(spec), idx in pstages)
+                    for idx, spec in enumerate(stages_spec)
+                ],
             )
             ctx.obj.cfg = cfg
 
-            handler(cfg, select_stages(cfg, cfg.get_all_envs(cfg)))
+            handler(cfg, select_stages(cfg, cfg.get_all_envs(cfg)), arg)
 
         return real_run
 
     return inner
 
 
 def click_main(
```

### Comparing `test_stages-0.1.1/src/test_stages/tox_stages/__main__.py` & `test_stages-0.1.2/src/test_stages/tox_stages/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,85 @@
-# Copyright (c) Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
-#
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
 """The main tox-stages command-line executable."""
 
-# This is a command-line tool, output is part of its job.
-# flake8: noqa: T201
-
 from __future__ import annotations
 
 import dataclasses
-import pathlib
 import subprocess
 import sys
-
-from typing import Final
+from typing import TYPE_CHECKING
 
 import tox_trivtags
+from test_stages import cmd
 
-from .. import cmd
 
-if tox_trivtags.HAVE_MOD_TOX_3:
+if tox_trivtags.HAVE_MOD_TOX_3 or tox_trivtags.HAVE_MOD_TOX_4:
     from tox_trivtags import parse as ttt_parse
 
+if TYPE_CHECKING:
+    import pathlib
+    from typing import Final
+
 
 @dataclasses.dataclass(frozen=True)
 class Config(cmd.Config):
     """Also store the path to the Tox executable if found."""
 
     tox_program: list[str | pathlib.Path] | None = None
 
 
 @cmd.click_available()
 def _cmd_available(cfg: cmd.Config) -> bool:
     """Check whether we can parse the Tox configuration in any of the supported ways.
 
     Currently the only supported way is `tox --showconfig`.
     """
-    assert isinstance(cfg, Config)
+    assert isinstance(cfg, Config)  # noqa: S101  # mypy needs this
     return cfg.tox_program is not None
 
 
 @cmd.click_run()
-def _cmd_run(cfg: cmd.Config, stages: list[list[cmd.TestEnv]]) -> None:
+def _cmd_run(cfg: cmd.Config, stages: list[cmd.TestStage], extra_args: list[str]) -> None:
     """Run the Tox environments in groups."""
     toxdir = cfg.filename.parent
 
-    def run_group(group: list[cmd.TestEnv]) -> None:
+    def run_group(group: list[cmd.TestEnv], *, parallel: bool) -> None:
         """Run the stages in a single group."""
         if not isinstance(cfg, Config) or cfg.tox_program is None:
             #  _tox_get_envs() really should have taken care of that
             sys.exit(f"Internal error: tox-stages run_group: Config? {cfg!r}")
 
         names: Final = ",".join(env.name for env in group)
-        print(f"\n=== Running Tox environments: {names}\n")
+        print(f"\n=== Running Tox environments: {names}\n")  # noqa: T201
+        run_parallel = (
+            (["-p", "all"] if parallel else [])
+            if tox_trivtags.HAVE_MOD_TOX_3
+            else (["run-parallel"] if parallel else ["run"])
+        )
+        tox_cmd: Final = [*cfg.tox_program, *run_parallel, "-e", names, *extra_args]
         res: Final = subprocess.run(
-            cfg.tox_program + ["-p", "all", "-e", names],
+            tox_cmd,
             check=False,
             cwd=toxdir,
             env=cfg.utf8_env,
-            shell=False,
+            shell=False,  # noqa: S603
         )
         if res.returncode != 0:
             sys.exit(f"Tox failed for the {names} environments")
 
-    for group in stages:
-        run_group(group)
+    for desc in stages:
+        run_group(desc.envlist, parallel=desc.parallel)
 
-    print("\n=== All Tox environment groups passed!")
+    print("\n=== All Tox environment groups passed!")  # noqa: T201
 
 
 def _tox_get_envs(cfg: cmd.Config) -> list[cmd.TestEnv]:
     """Get all the Tox environments from the config file."""
-    assert isinstance(cfg, Config)
+    assert isinstance(cfg, Config)  # noqa: S101  # mypy needs this
     if cfg.tox_program is None:
         sys.exit("No tox program found or specified")
     tcfg: Final = ttt_parse.parse_showconfig(
         filename=cfg.filename, env=cfg.utf8_env, tox_invoke=cfg.tox_program
     )
     return [cmd.TestEnv(name, env.tags) for name, env in tcfg.items()]
 
@@ -106,15 +89,15 @@
 
     For the present, only a Tox installation in the current Python interpreter's
     package directories is supported, since we need to be sure that we can rely on
     the `tox-trivtags` package being installed.
 
     Also, we only support Tox 3.x for the present.
     """
-    if not tox_trivtags.HAVE_MOD_TOX_3:
+    if not tox_trivtags.HAVE_MOD_TOX_3 and not tox_trivtags.HAVE_MOD_TOX_4:
         return None
 
     return [sys.executable, "-m", "tox"]
 
 
 @cmd.click_main(
     prog="tox-stages",
@@ -126,7 +109,12 @@
 def main(cfg: cmd.Config) -> cmd.Config:
     """Return our `Config` object with the path to Tox if found."""
     return Config(**dataclasses.asdict(cfg), tox_program=_find_tox_program())
 
 
 main.add_command(_cmd_available)
 main.add_command(_cmd_run)
+
+
+if __name__ == "__main__":
+    # pylint: disable-next=no-value-for-parameter
+    main()
```

### Comparing `test_stages-0.1.1/tox.ini` & `test_stages-0.1.2/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,120 +1,105 @@
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
+
 [tox]
+minversion = 4.1
 envlist =
   ruff
-  black
-  pep8
+  ruff-all
+  format
   mypy
   pylint
-  unit_tests-no-tox
-  unit_tests-tox-3
-  unit_tests-tox-4
+  unit-tests-no-tox
+  unit-tests-tox-3
+  unit-tests-tox-4
+  selftest
 isolated_build = True
 
 [defs]
+pyfiles_mypy =
+  src/selftest \
+  src/test_stages \
+  unit_tests
+
 pyfiles =
-  src/test_stages
+  {[defs]pyfiles_mypy} \
   src/tox_trivtags
-  unit_tests
 
 [testenv:ruff]
 skip_install = True
 tags =
   check
 deps =
-  ruff >= 0.0.243, < 0.1
+  ruff >= 0.0.265, < 0.1
 commands =
-  ruff -- {[defs]pyfiles}
+  ruff check --config config/ruff-most/pyproject.toml -- {[defs]pyfiles}
 
 [testenv:ruff-all]
 skip_install = True
 tags =
   check
 deps =
-  ruff == 0.0.243
+  ruff == 0.0.265
 commands =
-  ruff --config .config/ruff-all/pyproject.toml -- {[defs]pyfiles}
+  ruff check --config config/ruff-all/pyproject.toml -- {[defs]pyfiles}
 
-[testenv:black]
+[testenv:format]
 skip_install = True
 tags =
   check
 deps =
   black >= 23, < 24
+  ruff >= 0.0.265, < 0.1
 commands =
+  ruff check --config config/ruff-base/pyproject.toml --select=I --diff -- {[defs]pyfiles}
   black --check {[defs]pyfiles}
 
-[testenv:black-reformat]
+[testenv:reformat]
 skip_install = True
 tags =
   format
+  manual
 deps =
   black >= 23, < 24
+  ruff >= 0.0.265, < 0.1
 commands =
+  ruff check --config config/ruff-base/pyproject.toml --select=I --fix -- {[defs]pyfiles}
   black {[defs]pyfiles}
 
-[testenv:pep8]
-skip_install = True
-tags =
-  check
-deps =
-  flake8 >= 6, < 7
-  flake8-2020 >= 1, < 2
-  flake8-annotations >= 3, < 4
-  flake8-blind-except >= 0.2, < 0.3
-  flake8-bugbear >= 23, < 24
-  flake8-builtins >= 2, < 3
-  flake8-commas >= 2, < 3
-  flake8-comprehensions >= 3, < 4
-  flake8-datetimez >= 20, < 21
-  flake8-debugger >= 4, < 5
-  flake8-executable >= 2, < 3
-  flake8-implicit-str-concat >= 0.3, < 0.4
-  flake8-no-pep420 >= 2, < 3
-  flake8-pie >= 0.16, < 0.17
-  flake8-print >= 5, < 6
-  flake8-pytest-style >= 1, < 2
-  flake8-quotes >= 3, < 4
-  flake8-return >= 1, < 2
-  flake8-simplify >= 0.19, < 0.20
-  flake8-use-pathlib >= 0.3, < 0.4
-  mccabe >= 0.7, < 0.8
-  pep8-naming >= 0.13, < 0.14
-  pycodestyle >= 2.10, < 3
-commands =
-  flake8 {[defs]pyfiles}
-  pycodestyle {[defs]pyfiles}
-
 [testenv:mypy]
 skip_install = True
 tags =
   check
 deps =
   -r requirements/install.txt
+  -r requirements/selftest.txt
   -r requirements/test.txt
-  mypy >= 0.942
+  mypy >= 1, < 2
   tomli >= 2, < 3
-  tox >= 3, < 4
+
+  # pytest still needs this one...
   types-setuptools >= 20
 setenv =
   MYPYPATH = {toxinidir}/stubs
 commands =
-  mypy {[defs]pyfiles}
+  mypy --follow-imports silent --exclude tox_trivtags {[defs]pyfiles_mypy}
 
 [testenv:pylint]
 skip_install = True
 tags =
   check
 deps =
   -r requirements/install.txt
+  -r requirements/selftest.txt
   -r requirements/test.txt
-  pylint >= 2.16, < 2.17
-  tox >= 3, < 4
+  pylint >= 2.17, < 2.18
+  tox >= 3, < 5
 commands =
-  pylint {[defs]pyfiles}
+  pylint --ignore tox_trivtags {[defs]pyfiles_mypy}
 
 [testenv:unit-tests-no-tox]
 tags =
   tests
 deps =
   -r requirements/install.txt
   -r requirements/test.txt
@@ -143,28 +128,63 @@
   -r requirements/install.txt
   -r requirements/test.txt
   tox >= 4, < 5
 allowlist_externals =
   sh
 commands =
   tox-stages --help
-  sh -c 'if tox-stages available; then echo Waat; exit 1; else echo Not available; fi'
+  tox-stages available
+  pytest {posargs} unit_tests
+
+[testenv:selftest]
+tags =
+  tests
+deps =
+  -r requirements/install.txt
+  -r requirements/selftest.txt
+  hatchling >= 1.14.1, < 2
+  hatch-requirements-txt >= 0.4, < 0.5
+setenv =
+  PYTHONPATH = {toxinidir}/src
+commands =
+  python3 -m selftest
 
 # The pyupgrade tool does not seem to have a "check only" mode
 [testenv:pyupgrade]
 skip_install = True
 tags =
-  check-later
+  check
+  manual
 deps =
   pyupgrade >= 3, < 4
 allowlist_externals =
   sh
 commands =
   sh -c 'pyupgrade --py38-plus src/test_stages/*.py src/test_stages/tox_stages/*.py src/tox_trivtags/*.py unit_tests/*.py'
 
+[testenv:reuse]
+skip_install = True
+tags =
+  check
+  manual
+deps =
+  reuse >= 1, < 2
+commands =
+  reuse lint
+
+[testenv:docs]
+skip_install = True
+tags =
+  docs
+  manual
+deps =
+  -r requirements/docs.txt
+commands =
+  mkdocs build
+
 [testenv:t-single]
 tags =
   something
 commands =
   python3 -c 'raise NotImplementedError()'
 
 [testenv:t-several]
@@ -180,7 +200,13 @@
   So,
   how many
   $tags
   is "too many",
   'eh"?
 commands =
   python3 -c 'raise NotImplementedError()'
+
+[testenv:t-selftest-marker]
+tags =
+  selftest
+commands =
+  python3 -c 'import pathlib; pathlib.Path("selftest-marker.txt").write_text("", encoding="UTF-8")'
```

### Comparing `test_stages-0.1.1/unit_tests/test_functional.py` & `test_stages-0.1.2/unit_tests/test_functional.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,86 @@
-# Copyright (c) Peter Pentchev <roam@ringlet.net>
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without
-# modification, are permitted provided that the following conditions
-# are met:
-# 1. Redistributions of source code must retain the above copyright
-#    notice, this list of conditions and the following disclaimer.
-# 2. Redistributions in binary form must reproduce the above copyright
-#    notice, this list of conditions and the following disclaimer in the
-#    documentation and/or other materials provided with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS ``AS IS'' AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-# ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
-# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
-# OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
-# OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-# SUCH DAMAGE.
+# SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
+# SPDX-License-Identifier: BSD-2-Clause
 """Load the Tox configuration, look for our tags thing."""
 
-# This is a test suite.
-# flake8: noqa: T201
-
 from __future__ import annotations
 
 import contextlib
 import pathlib
+import shutil
+import subprocess
 import sys
 import tempfile
-
-from collections.abc import Callable, Iterator
-from contextlib import AbstractContextManager
-from typing import Final
+from typing import TYPE_CHECKING
 
 import pytest
 import utf8_locale
 
+import tox_trivtags
 import tox_trivtags.parse as ttt_parse
 
+
 if sys.version_info >= (3, 11):
     import contextlib as contextlib_chdir  # pylint: disable=reimported
 else:
     import contextlib_chdir
 
+if TYPE_CHECKING:
+    from collections.abc import Callable, Iterator
+    from contextlib import AbstractContextManager
+    from typing import Final
+
+
 _EXPECTED: Final[dict[str, list[str]]] = {
-    "black": ["check"],
-    "black-reformat": ["format"],
+    "format": ["check"],
+    "reformat": ["format", "manual"],
     "unit-tests-no-tox": ["tests"],
     "unit-tests-tox-3": ["tests"],
     "unit-tests-tox-4": ["tests"],
-    ".package": [],
+    (".package" if tox_trivtags.HAVE_MOD_TOX_3 else ".pkg"): [],
     "t-single": ["something"],
     "t-several": ["all", "the", "things"],
     "t-special": ["So,", "how many", "$tags", 'is "too many",', "'eh\"?"],
 }
 
 
+def copy_and_adapt(srcdir: pathlib.Path, dstdir: pathlib.Path) -> None:
+    """Copy some files over, adapt the tox.ini file."""
+    src_tox = srcdir / "tox.ini"
+    dst_tox = dstdir / "tox.ini"
+    lines: Final = src_tox.read_text(encoding="UTF-8").splitlines()
+    adapted: Final = [
+        line.replace(" \\", "") for line in lines if not line.startswith("minversion")
+    ]
+    dst_tox.write_text("".join(line + "\n" for line in adapted), encoding="UTF-8")
+    res: Final = subprocess.run(["diff", "-u", "--", src_tox, dst_tox], check=False)
+    assert res.returncode != 0
+
+    shutil.copytree(srcdir / "config", dstdir / "config")
+    shutil.copytree(srcdir / "requirements", dstdir / "requirements")
+    shutil.copy2(srcdir / "pyproject.toml", dstdir / "pyproject.toml")
+
+
+@contextlib.contextmanager
+def adapt_tox_cwd() -> Iterator[pathlib.Path]:
+    """If using Tox 3.x, copy the files over and adapt them."""
+    cwd: Final = pathlib.Path("").absolute()
+    if not tox_trivtags.HAVE_MOD_TOX_3:
+        print("Not using Tox 3.x, no need to copy or adapt any files")
+        yield cwd
+        return
+
+    with tempfile.TemporaryDirectory() as toxd_name:
+        toxd = pathlib.Path(toxd_name).absolute()
+        print(f"Adapting files for Tox 3.x from {cwd} to {toxd}")
+        copy_and_adapt(cwd, toxd)
+        with contextlib_chdir.chdir(toxd):
+            yield toxd
+
+
 @contextlib.contextmanager
 def _cfg_filename_cwd() -> Iterator[pathlib.Path]:
     """No arguments, parse the tox.ini file in the current directory."""
     yield pathlib.Path("tox.ini")
 
 
 @contextlib.contextmanager
@@ -88,26 +105,9 @@
         assert envs[envname].tags == expected
 
 
 @pytest.mark.parametrize("cfg_filename", [_cfg_filename_cwd, _cfg_filename_tempdir])
 def test_run_showconfig(cfg_filename: Callable[[], AbstractContextManager[pathlib.Path]]) -> None:
     """Run `tox --showconfig` expecting tox.ini to be in the specified directory."""
     print()
-    with cfg_filename() as filename:
+    with adapt_tox_cwd(), cfg_filename() as filename:
         _do_test_run_showconfig(filename)
-
-
-def _do_test_call_tox_config(filename: pathlib.Path) -> None:
-    """Invoke tox.config.Config() to parse the Tox configuration."""
-    envs: Final = ttt_parse.parse_config(filename)
-    print(f"Got some Tox environments: {' '.join(sorted(envs))}")
-    for envname, expected in _EXPECTED.items():
-        print(f"- envname {envname!r} expected {expected!r}")
-        assert envs[envname].tags == expected
-
-
-@pytest.mark.parametrize("cfg_filename", [_cfg_filename_cwd, _cfg_filename_tempdir])
-def test_call_tox_config(cfg_filename: Callable[[], AbstractContextManager[pathlib.Path]]) -> None:
-    """Parse the tox.ini file in the specified directory."""
-    print()
-    with cfg_filename() as filename:
-        _do_test_call_tox_config(filename)
```

