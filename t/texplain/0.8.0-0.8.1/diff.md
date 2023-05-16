# Comparing `tmp/texplain-0.8.0.tar.gz` & `tmp/texplain-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texplain-0.8.0.tar", last modified: Wed May  3 15:26:23 2023, max compression
+gzip compressed data, was "texplain-0.8.1.tar", last modified: Tue May 16 13:24:05 2023, max compression
```

## Comparing `texplain-0.8.0.tar` & `texplain-0.8.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.844694 texplain-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-03 15:26:07.000000 texplain-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 15:26:07.000000 texplain-0.8.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 15:26:07.000000 texplain-0.8.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-03 15:26:07.000000 texplain-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-03 15:26:07.000000 texplain-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-03 15:26:07.000000 texplain-0.8.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 15:26:07.000000 texplain-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 15:26:07.000000 texplain-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-03 15:26:23.852695 texplain-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-03 15:26:07.000000 texplain-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/pre-commit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 15:26:07.000000 texplain-0.8.0/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 15:26:07.000000 texplain-0.8.0/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 15:26:07.000000 texplain-0.8.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:26:23.852695 texplain-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-03 15:26:07.000000 texplain-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/tests/input1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/example.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.848694 texplain-0.8.0/tests/input1/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/figures/Diverging.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/figures/Sequential.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/input1/unsrtnat.bst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/tests/output1/
--rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/apalike.bst
--rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/figure_1.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/figure_2.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/goose-article.cls
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/library.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/main.tex
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/output1/unsrtnat.bst
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_find_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_indent_texindent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 15:26:07.000000 texplain-0.8.0/tests/test_texplain_example1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/texplain/
--rw-r--r--   0 runner    (1001) docker     (123)    87026 2023-05-03 15:26:07.000000 texplain-0.8.0/texplain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:26:23.852695 texplain-0.8.0/texplain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 15:26:23.000000 texplain-0.8.0/texplain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.617575 texplain-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.609575 texplain-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.609575 texplain-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-16 13:23:56.000000 texplain-0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 13:23:56.000000 texplain-0.8.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 13:23:56.000000 texplain-0.8.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-16 13:23:56.000000 texplain-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-16 13:23:56.000000 texplain-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-16 13:23:56.000000 texplain-0.8.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 13:23:56.000000 texplain-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 13:23:56.000000 texplain-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-16 13:24:05.617575 texplain-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-16 13:23:56.000000 texplain-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.609575 texplain-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/pre-commit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-16 13:23:56.000000 texplain-0.8.1/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 13:23:56.000000 texplain-0.8.1/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 13:23:56.000000 texplain-0.8.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-16 13:23:56.000000 texplain-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:24:05.617575 texplain-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/input1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/example.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/input1/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/figures/Diverging.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/figures/Sequential.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/input1/unsrtnat.bst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/tests/output1/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/apalike.bst
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/figure_1.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/figure_2.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/goose-article.cls
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/library.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/main.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/output1/unsrtnat.bst
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_find_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167299 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_indent_texindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 13:23:56.000000 texplain-0.8.1/tests/test_texplain_example1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.613575 texplain-0.8.1/texplain/
+-rw-r--r--   0 runner    (1001) docker     (123)    87198 2023-05-16 13:23:56.000000 texplain-0.8.1/texplain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:24:05.617575 texplain-0.8.1/texplain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 13:24:05.000000 texplain-0.8.1/texplain.egg-info/top_level.txt
```

### Comparing `texplain-0.8.0/.github/workflows/ci.yml` & `texplain-0.8.1/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -20,28 +20,33 @@
         shell: bash -l {0}
 
     name: ${{ matrix.runs-on }} • x64 ${{ matrix.args }}
     runs-on: ${{ matrix.runs-on }}
 
     steps:
 
-    - name: Basic GitHub action setup
+    - name: Checkout
       uses: actions/checkout@v3
+      with:
+        fetch-depth: 0
+
+    - name: Checkout latest release tag
+      run: |
+        LATEST_TAG=$(git describe --tags `git rev-list --tags --max-count=1`)
+        echo "SETUPTOOLS_SCM_PRETEND_VERSION=$LATEST_TAG" >> $GITHUB_ENV
 
     - name: Set conda environment
       uses: mamba-org/provision-with-micromamba@main
       with:
         environment-file: environment.yaml
         environment-name: myenv
-
-    - name: Set dummy version
-      run: echo "SETUPTOOLS_SCM_PRETEND_VERSION=0.0" >> $GITHUB_ENV
+        cache-env: true
 
     - name: Install library
-      run: python -m pip install .
+      run: python -m pip install . -v --no-build-isolation --no-deps
 
     - name: Run tests
       run: python -m unittest discover tests -v
 
     - name: Build docs
       working-directory: docs
       run: make html
```

### Comparing `texplain-0.8.0/.gitignore` & `texplain-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/LICENSE` & `texplain-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/PKG-INFO` & `texplain-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.0
-Summary: Create directory with TeX-file and only dependencies.
-Home-page: https://github.com/tdegeus/texplain
-Author: Tom de Geus
-Author-email: tom@geus.me
-License: MIT
-Keywords: LaTeX
+Version: 0.8.1
+Summary: TeX file formatting
+Author-email: Tom de Geus <tom@geus.me>
+Project-URL: Source, https://github.com/tdegeus/texplain
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![ci](https://github.com/tdegeus/texplain/workflows/CI/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![Documentation Status](https://readthedocs.org/projects/texplain/badge/?version=latest)](https://texplain.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit](https://github.com/tdegeus/texplain/workflows/pre-commit/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

### Comparing `texplain-0.8.0/README.md` & `texplain-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/docs/Makefile` & `texplain-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/docs/make.bat` & `texplain-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/docs/module.rst` & `texplain-0.8.1/docs/module.rst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/apalike.bst` & `texplain-0.8.1/tests/input1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/example.tex` & `texplain-0.8.1/tests/input1/example.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/figures/Diverging.pdf` & `texplain-0.8.1/tests/input1/figures/Diverging.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/figures/Sequential.pdf` & `texplain-0.8.1/tests/input1/figures/Sequential.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/goose-article.cls` & `texplain-0.8.1/tests/input1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/refs.bib` & `texplain-0.8.1/tests/input1/refs.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/input1/unsrtnat.bst` & `texplain-0.8.1/tests/input1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/apalike.bst` & `texplain-0.8.1/tests/output1/apalike.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/figure_1.pdf` & `texplain-0.8.1/tests/output1/figure_1.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/figure_2.pdf` & `texplain-0.8.1/tests/output1/figure_2.pdf`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/goose-article.cls` & `texplain-0.8.1/tests/output1/goose-article.cls`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/library.bib` & `texplain-0.8.1/tests/output1/library.bib`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/main.tex` & `texplain-0.8.1/tests/output1/main.tex`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/output1/unsrtnat.bst` & `texplain-0.8.1/tests/output1/unsrtnat.bst`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_align.py` & `texplain-0.8.1/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_classify.py` & `texplain-0.8.1/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_find_command.py` & `texplain-0.8.1/tests/test_find_command.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_indent.py` & `texplain-0.8.1/tests/test_indent_simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -389,14 +389,95 @@
 }
         """
 
         ret = texplain.indent(text)
         self.assertEqual(ret.strip(), formatted.strip())
 
 
+class TestIndentItem(unittest.TestCase):
+    def test_simple(self):
+        text = r"""
+\begin{itemize} \item a \item b
+\item c \item d
+\item e \end{itemize}
+        """
+
+        formatted = r"""
+\begin{itemize}
+    \item a
+    \item b
+    \item c
+    \item d
+    \item e
+\end{itemize}
+        """
+
+        ret = texplain.indent(text)
+        self.assertEqual(ret.strip(), formatted.strip())
+
+    def test_multiline(self):
+        text = r"""
+\begin{itemize} \item a \item b has a long
+text that spans multiple lines. But also multiple
+sentences.
+
+With even
+a new paragraph.
+\item c \item d
+\item e \end{itemize}
+        """
+
+        formatted = r"""
+\begin{itemize}
+    \item a
+    \item b has a long text that spans multiple lines.
+    But also multiple sentences.
+
+    With even a new paragraph.
+    \item c
+    \item d
+    \item e
+\end{itemize}
+        """
+
+        ret = texplain.indent(text)
+        self.assertEqual(ret.strip(), formatted.strip())
+
+    def test_nested(self):
+        text = r"""
+\begin{itemize} \item a \item b
+\item c \item d \begin{itemize} \item suba \item subb with
+some text.
+And another
+sentence.
+\item subc \item subd \end{itemize}
+\item e \end{itemize}
+        """
+
+        formatted = r"""
+\begin{itemize}
+    \item a
+    \item b
+    \item c
+    \item d
+    \begin{itemize}
+        \item suba
+        \item subb with some text.
+        And another sentence.
+        \item subc
+        \item subd
+    \end{itemize}
+    \item e
+\end{itemize}
+        """
+
+        ret = texplain.indent(text)
+        self.assertEqual(ret.strip(), formatted.strip())
+
+
 class TestIndentCommand(unittest.TestCase):
     def test_command_punctuation(self):
         text = r"""
 A start\footnote{
     This is a footnote
 }.
 A new sentence.
```

### Comparing `texplain-0.8.0/tests/test_indent_long.py` & `texplain-0.8.1/tests/test_indent_long.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_indent_options.py` & `texplain-0.8.1/tests/test_indent_options.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_indent_texindent.py` & `texplain-0.8.1/tests/test_indent_texindent.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_placeholders.py` & `texplain-0.8.1/tests/test_placeholders.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_simple.py` & `texplain-0.8.1/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/tests/test_texplain_example1.py` & `texplain-0.8.1/tests/test_texplain_example1.py`

 * *Files identical despite different names*

### Comparing `texplain-0.8.0/texplain/__init__.py` & `texplain-0.8.1/texplain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,15 +584,15 @@
             last = indices[i, 1]
 
     return indices[keep]
 
 
 def _apply_placeholders(
     text: str,
-    indices: NDArray[np.int_] | list[tuple[int, int]],
+    indices: ArrayLike,
     base: str,
     name: str,
     ptype: PlaceholderType,
     filter_nested: bool = True,
 ) -> tuple[str, list[Placeholder]]:
     """
     Replace text with placeholders.
@@ -1329,14 +1329,15 @@
     squashlines: bool = True,
     squashspaces: bool = True,
     symbols: bool = True,
     environment: bool = True,
     argument: bool = True,
     inlinemath: bool = True,
     linebreak: bool = True,
+    itemize: bool = True,
     sentence: bool = True,
     alignment: bool = True,
     texindent: bool = True,
     noindent: bool = True,
 ) -> str:
     r"""
     Indent text.
@@ -1381,14 +1382,15 @@
             xxx {
                 This is a very long argument
                 that is more than one line long.
             } yyy
 
     :param inlinemath: Inline math is placed on one line.
     :param linebreak: ``\\`` is followed by a newline.
+    :param itemize: Each ``\item`` is placed on a separate line.
 
     :param sentence:
         One sentence per line.
         Every sentence should start on a new line,
         and it should be (as much as possible) on a single line.
         The following rules of thumb are followed:
 
@@ -1519,14 +1521,18 @@
         text = _begin_end_one_separate_line(text, placeholders_comments)
         text = text_from_placeholders(text, placeholders_let)
 
     # \\ ends on line
     if linebreak:
         text = re.sub(r"(?<!\\)(\\\\)(\ *\n?)", r"\1\n", text)
 
+    # \item starts on a new line
+    if itemize:
+        text = re.sub(r"(\s*)(?<!\\)(\\item)", r"\n\2", text)
+
     # format tables: align if possible
     if alignment:
         text, placeholders_table = text_to_placeholders(text, [PlaceholderType.tabular])
         for placeholder in placeholders_table:
             placeholder.content = _align(placeholder.content)
         text = text_from_placeholders(text, placeholders_table)
```

### Comparing `texplain-0.8.0/texplain.egg-info/PKG-INFO` & `texplain-0.8.1/texplain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: texplain
-Version: 0.8.0
-Summary: Create directory with TeX-file and only dependencies.
-Home-page: https://github.com/tdegeus/texplain
-Author: Tom de Geus
-Author-email: tom@geus.me
-License: MIT
-Keywords: LaTeX
+Version: 0.8.1
+Summary: TeX file formatting
+Author-email: Tom de Geus <tom@geus.me>
+Project-URL: Source, https://github.com/tdegeus/texplain
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![ci](https://github.com/tdegeus/texplain/workflows/CI/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![Documentation Status](https://readthedocs.org/projects/texplain/badge/?version=latest)](https://texplain.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit](https://github.com/tdegeus/texplain/workflows/pre-commit/badge.svg)](https://github.com/tdegeus/texplain/actions)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

### Comparing `texplain-0.8.0/texplain.egg-info/SOURCES.txt` & `texplain-0.8.1/texplain.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .pre-commit-config.yaml
 .pre-commit-hooks.yaml
 .readthedocs.yml
 LICENSE
 README.md
 environment.yaml
 environment.yml
-setup.py
+pyproject.toml
 .github/workflows/ci.yml
 .github/workflows/pre-commit.yml
 .github/workflows/pythonpublish.yml
 docs/.gitignore
 docs/Makefile
 docs/conf.py
 docs/index.rst
@@ -18,17 +18,17 @@
 docs/module.rst
 docs/pre-commit.rst
 docs/tools.rst
 tests/__init__.py
 tests/test_align.py
 tests/test_classify.py
 tests/test_find_command.py
-tests/test_indent.py
 tests/test_indent_long.py
 tests/test_indent_options.py
+tests/test_indent_simple.py
 tests/test_indent_texindent.py
 tests/test_placeholders.py
 tests/test_simple.py
 tests/test_texplain_example1.py
 tests/input1/apalike.bst
 tests/input1/example.tex
 tests/input1/goose-article.cls
```

