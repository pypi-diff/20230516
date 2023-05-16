# Comparing `tmp/ket-lang-0.6.1.dev1.tar.gz` & `tmp/ket-lang-0.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ket-lang-0.6.1.dev1.tar", last modified: Tue May 16 21:15:07 2023, max compression
+gzip compressed data, was "ket-lang-0.6rc2.tar", last modified: Mon May 15 18:50:19 2023, max compression
```

## Comparing `ket-lang-0.6.1.dev1.tar` & `ket-lang-0.6rc2.tar`

### file list

```diff
@@ -1,96 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.094224 ket-lang-0.6.1.dev1/
--rw-rw-rw-   0 root         (0) root         (0)    11455 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7288 2023-05-16 21:15:07.094224 ket-lang-0.6.1.dev1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6527 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-05-16 21:15:07.095224 ket-lang-0.6.1.dev1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.063221 ket-lang-0.6.1.dev1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.069222 ket-lang-0.6.1.dev1/src/ket/
--rw-rw-rw-   0 root         (0) root         (0)     1313 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    29132 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.070222 ket-lang-0.6.1.dev1/src/ket/clib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/clib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3937 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/clib/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     9012 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/clib/libket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.071222 ket-lang-0.6.1.dev1/src/ket/clib/libs/
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.073222 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/README.md
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/kbw.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.077222 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/bitwise.rs
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/c_api.rs
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/convert.rs
--rw-rw-rw-   0 root         (0) root         (0)    20501 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/dense.rs
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     9825 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/quantum_execution.rs
--rw-rw-rw-   0 root         (0) root         (0)    20230 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/sparse.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.077222 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/tests/shor.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.080222 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-16 21:14:55.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.081223 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.082223 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/examples/
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/examples/bell.rs
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/examples/grover.rs
--rw-rw-rw-   0 root         (0) root         (0)     1238 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/examples/grover_process.rs
--rw-rw-rw-   0 root         (0) root         (0)     8457 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/libket.h
--rw-rw-rw-   0 root         (0) root         (0)    10442 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/libket.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.086223 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.087223 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/
--rw-rw-rw-   0 root         (0) root         (0)     1569 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)    14867 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    27318 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     6119 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/code_block.rs
--rw-rw-rw-   0 root         (0) root         (0)     8761 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/decompose.rs
--rw-rw-rw-   0 root         (0) root         (0)     4603 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)    13711 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/gates.rs
--rw-rw-rw-   0 root         (0) root         (0)     4853 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/instruction.rs
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/ir.rs
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/object.rs
--rw-rw-rw-   0 root         (0) root         (0)    36826 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/process.rs
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-16 21:14:56.000000 ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/serialize.rs
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/clib/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.088223 ket-lang-0.6.1.dev1/src/ket/gates/
--rw-rw-rw-   0 root         (0) root         (0)     8530 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/gates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/gates/base_gates.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/gates/quantum_gate.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/import_ket.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.090223 ket-lang-0.6.1.dev1/src/ket/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/preprocessor/statements.py
--rw-rw-rw-   0 root         (0) root         (0)     8995 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/preprocessor/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.091223 ket-lang-0.6.1.dev1/src/ket/standard/
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/standard/adj.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/src/ket/standard/ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.093224 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7288 2023-05-16 21:15:07.000000 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2422 2023-05-16 21:15:07.000000 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 21:15:07.000000 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-16 21:15:07.000000 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 21:15:07.000000 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 21:15:07.000000 ket-lang-0.6.1.dev1/src/ket_lang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 21:15:07.094224 ket-lang-0.6.1.dev1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4698 2023-05-16 21:14:54.000000 ket-lang-0.6.1.dev1/tests/test_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/
+-rw-rw-rw-   0 root         (0) root         (0)    11455 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6527 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-05-15 18:50:19.770542 ket-lang-0.6rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.741540 ket-lang-0.6rc2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.747541 ket-lang-0.6rc2/src/ket/
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29132 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.748541 ket-lang-0.6rc2/src/ket/clib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3937 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     9012 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/libket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.748541 ket-lang-0.6rc2/src/ket/clib/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.751541 ket-lang-0.6rc2/src/ket/clib/libs/kbw/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/kbw.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.754541 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/bitwise.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/c_api.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/convert.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20501 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/dense.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     9825 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/quantum_execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20230 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/sparse.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.754541 ket-lang-0.6rc2/src/ket/clib/libs/kbw/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/tests/shor.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.757541 ket-lang-0.6rc2/src/ket/clib/libs/libket/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.758541 ket-lang-0.6rc2/src/ket/clib/libs/libket/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8457 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.h
+-rw-rw-rw-   0 root         (0) root         (0)    10442 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.762542 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.763542 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)    14867 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    27318 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/code_block.rs
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/decompose.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/gates.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4853 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/instruction.rs
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/ir.rs
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/object.rs
+-rw-rw-rw-   0 root         (0) root         (0)    21092 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/serialize.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.764542 ket-lang-0.6rc2/src/ket/gates/
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/gates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/gates/base_gates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/gates/quantum_gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/import_ket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.765542 ket-lang-0.6rc2/src/ket/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/preprocessor/statements.py
+-rw-rw-rw-   0 root         (0) root         (0)     8995 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/preprocessor/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3751 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.766542 ket-lang-0.6rc2/src/ket/standard/
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/standard/adj.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/standard/ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/src/ket_lang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/tests/test_gates.py
```

### Comparing `ket-lang-0.6.1.dev1/LICENSE` & `ket-lang-0.6rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/PKG-INFO` & `ket-lang-0.6rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.6.1.dev1
+Version: 0.6rc2
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
```

### Comparing `ket-lang-0.6.1.dev1/README.md` & `ket-lang-0.6rc2/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/setup.cfg` & `ket-lang-0.6rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/__init__.py` & `ket-lang-0.6rc2/src/ket/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .process import *
 from .gates import __all__ as all_gate
 from .import_ket import __all__ as all_import
 from .base import __all__ as all_base
 from .standard import __all__ as all_standard
 from .process import __all__ as all_process
 
-__version__ = '0.6.1dev1'
+__version__ = '0.6rc2'
 __all__ = all_gate + all_import + all_base + all_standard + all_process
 
 from .import_ket import code_ket
 
 from .base import QUANTUM_EXECUTION_TARGET
 if QUANTUM_EXECUTION_TARGET is None:
     from .kbw import use_sparse
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/__main__.py` & `ket-lang-0.6rc2/src/ket/__main__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/base.py` & `ket-lang-0.6rc2/src/ket/base.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/kbw.py` & `ket-lang-0.6rc2/src/ket/clib/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libket.py` & `ket-lang-0.6rc2/src/ket/clib/libket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/__init__.py` & `ket-lang-0.6rc2/src/ket/clib/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/CHANGELOG.md` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/Cargo.toml` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/LICENSE` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/README.md` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/kbw.h` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/kbw.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/bitwise.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/bitwise.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/c_api.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/c_api.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/convert.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/convert.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/dense.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/dense.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/error.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/quantum_execution.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/quantum_execution.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/src/sparse.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/sparse.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/kbw/tests/shor.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/tests/shor.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/Cargo.toml` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "libket"
-version = "0.3.1"
+version = "0.3.0"
 authors = ["Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>"]
 description = "Runtime library for the Ket programming language"
 repository = "https://gitlab.com/quantum-ket/libket"
 documentation = "https://quantumket.org"
 license = "Apache-2.0"
 readme = "README.md"
 edition = "2021"
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/LICENSE` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/README.md` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/libket.h` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/libket.hpp` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.hpp`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/error.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/mod.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-//! # FFI Wrapper
+//! # FFI Wrapper Module
 //!
 //! This module provides a wrapper for Foreign Function Interface (FFI) functions in Rust. 
 //! It includes utility functions for error handling and retrieving error messages, 
 //! as well as functions for interacting with FFI data structures.
 //!
 //! ## Error Handling
 //!
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/objects.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/objects.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/c_api/process.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/process.rs`

 * *Files 1% similar despite different names*

```diff
@@ -607,23 +607,23 @@
     data: &mut *const u8,
     size: &mut usize,
     data_type: &mut i32,
 ) -> i32 {
     match process.get_serialized_metrics() {
         Some(metrics) => {
             match metrics {
-                SerializedData::Json(json) => {
+                SerializedData::JSON(json) => {
                     *data = json.as_ptr();
                     *size = json.len();
-                    *data_type = DataType::Json.to_i32().unwrap();
+                    *data_type = DataType::JSON.to_i32().unwrap();
                 }
-                SerializedData::Bin(bin) => {
+                SerializedData::BIN(bin) => {
                     *data = bin.as_ptr();
                     *size = bin.len();
-                    *data_type = DataType::Bin.to_i32().unwrap();
+                    *data_type = DataType::BIN.to_i32().unwrap();
                 }
             }
             KetError::Success.error_code()
         }
         None => KetError::DataNotAvailable.error_code(),
     }
 }
@@ -658,23 +658,23 @@
     data: &mut *const u8,
     size: &mut usize,
     data_type: &mut i32,
 ) -> i32 {
     match process.get_serialized_quantum_code() {
         Some(code) => {
             match code {
-                SerializedData::Json(json) => {
+                SerializedData::JSON(json) => {
                     *data = json.as_ptr();
                     *size = json.len();
-                    *data_type = DataType::Json.to_i32().unwrap();
+                    *data_type = DataType::JSON.to_i32().unwrap();
                 }
-                SerializedData::Bin(bin) => {
+                SerializedData::BIN(bin) => {
                     *data = bin.as_ptr();
                     *size = bin.len();
-                    *data_type = DataType::Bin.to_i32().unwrap();
+                    *data_type = DataType::BIN.to_i32().unwrap();
                 }
             }
             KetError::Success.error_code()
         }
         None => KetError::DataNotAvailable.error_code(),
     }
 }
@@ -720,16 +720,16 @@
         Some(data_type) => data_type,
         None => return KetError::UndefinedDataType.error_code(),
     };
 
     let result = unsafe { std::slice::from_raw_parts(result, result_size) };
 
     let result = match data_type {
-        DataType::Json => SerializedData::Json(String::from(std::str::from_utf8(result).unwrap())),
-        DataType::Bin => SerializedData::Bin(result.to_vec()),
+        DataType::JSON => SerializedData::JSON(String::from(std::str::from_utf8(result).unwrap())),
+        DataType::BIN => SerializedData::BIN(result.to_vec()),
     };
 
     wrapper(process.set_serialized_result(&result))
 }
 
 /// Creates a new `Features` instance with the specified feature flags.
 ///
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/code_block.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/code_block.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/decompose.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/decompose.rs`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,25 @@
                     target: control[lm_pos],
                     control: vec![control[idx]],
                 });
             }
         }
 
         if gray.matches('1').count() % 2 == 0 {
-            instructions.append(&mut decompose_single_control(
-                &gate.inverse(),
-                control[lm_pos],
+            instructions.push(Instruction::Gate {
+                gate: gate.inverse(),
                 target,
-            ));
+                control: vec![control[lm_pos]],
+            });
         } else {
-            instructions.append(&mut decompose_single_control(gate, control[lm_pos], target));
+            instructions.push(Instruction::Gate {
+                gate: gate.clone(),
+                target,
+                control: vec![control[lm_pos]],
+            })
         }
 
         last = gray;
     }
 
     instructions
 }
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/error.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     NoAdj,
     NoCtrl,
     NonGateInstruction,
     NotBIN,
     NotJSON,
     NotUnitary,
     PluginOnCtrl,
-    TargetInControl,
+    TargetOnControl,
     TerminatedBlock,
     UndefinedClassicalOp,
     UndefinedDataType,
     UndefinedGate,
     UnexpectedResultData,
-    PidMismatch,
+    UnmatchedPid,
     DirtyNotAllowed,
     DumpNotAllowed,
     MeasureNotAllowed,
     FreeNotAllowed,
     PluginNotRegistered,
     ControlFlowNotAllowed,
     NotPhaseGate,
@@ -48,23 +48,23 @@
             KetError::NonGateInstruction => {
                 "cannot apply a non-gate instruction within a controlled or inverse scope"
             }
             KetError::NotBIN => "data is not BIN",
             KetError::NotJSON => "data is not JSON",
             KetError::NotUnitary => "the given matrix is not unitary",
             KetError::PluginOnCtrl => "cannot apply plugin within a controlled scope",
-            KetError::TargetInControl => {
+            KetError::TargetOnControl => {
                 "a qubit cannot be targeted and controlled at the same time"
             }
             KetError::TerminatedBlock => "cannot append statements to a terminated block",
             KetError::UndefinedClassicalOp => "undefined classical operation",
             KetError::UndefinedDataType => "undefined data type",
             KetError::UndefinedGate => "undefined quantum gate",
             KetError::UnexpectedResultData => "result do not have the expected number of values",
-            KetError::PidMismatch => "unmatched pid",
+            KetError::UnmatchedPid => "unmatched pid",
             KetError::UndefinedError => "undefined error",
             KetError::DataNotAvailable => "data not available",
             KetError::DirtyNotAllowed => "cannot allocate or free dirty qubits (feature disabled)",
             KetError::FreeNotAllowed => "cannot free qubit (feature disabled)",
             KetError::PluginNotRegistered => "plugin not registered",
             KetError::ControlFlowNotAllowed => {
                 "classical control flow not allowed (feature disabled)"
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/instruction.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/ir.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/ir.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/libs/libket/src/serialize.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/serialize.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 use num_derive::{FromPrimitive, ToPrimitive};
 
 #[derive(FromPrimitive, ToPrimitive, Debug)]
 pub enum DataType {
-    Json,
-    Bin,
+    JSON,
+    BIN,
 }
 
 #[derive(Debug)]
 pub enum SerializedData {
-    Json(String),
-    Bin(Vec<u8>),
+    JSON(String),
+    BIN(Vec<u8>),
 }
 
 #[cfg(test)]
 mod tests {
     use super::DataType;
     use num::FromPrimitive;
```

### Comparing `ket-lang-0.6.1.dev1/src/ket/clib/wrapper.py` & `ket-lang-0.6rc2/src/ket/clib/wrapper.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/gates/__init__.py` & `ket-lang-0.6rc2/src/ket/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/gates/base_gates.py` & `ket-lang-0.6rc2/src/ket/gates/base_gates.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/gates/quantum_gate.py` & `ket-lang-0.6rc2/src/ket/gates/quantum_gate.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/import_ket.py` & `ket-lang-0.6rc2/src/ket/import_ket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/kbw.py` & `ket-lang-0.6rc2/src/ket/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/lib.py` & `ket-lang-0.6rc2/src/ket/lib.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/plugins.py` & `ket-lang-0.6rc2/src/ket/plugins.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/preprocessor/statements.py` & `ket-lang-0.6rc2/src/ket/preprocessor/statements.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/preprocessor/transformer.py` & `ket-lang-0.6rc2/src/ket/preprocessor/transformer.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/process.py` & `ket-lang-0.6rc2/src/ket/process.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/standard/__init__.py` & `ket-lang-0.6rc2/src/ket/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/standard/adj.py` & `ket-lang-0.6rc2/src/ket/standard/adj.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket/standard/ctrl.py` & `ket-lang-0.6rc2/src/ket/standard/ctrl.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.1.dev1/src/ket_lang.egg-info/PKG-INFO` & `ket-lang-0.6rc2/src/ket_lang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.6.1.dev1
+Version: 0.6rc2
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
```

### Comparing `ket-lang-0.6.1.dev1/src/ket_lang.egg-info/SOURCES.txt` & `ket-lang-0.6rc2/src/ket_lang.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,14 @@
 src/ket/clib/libs/libket/CHANGELOG.md
 src/ket/clib/libs/libket/Cargo.toml
 src/ket/clib/libs/libket/LICENSE
 src/ket/clib/libs/libket/README.md
 src/ket/clib/libs/libket/libket.h
 src/ket/clib/libs/libket/libket.hpp
 src/ket/clib/libs/libket/.vscode/settings.json
-src/ket/clib/libs/libket/examples/bell.rs
-src/ket/clib/libs/libket/examples/grover.rs
-src/ket/clib/libs/libket/examples/grover_process.rs
 src/ket/clib/libs/libket/src/code_block.rs
 src/ket/clib/libs/libket/src/decompose.rs
 src/ket/clib/libs/libket/src/error.rs
 src/ket/clib/libs/libket/src/gates.rs
 src/ket/clib/libs/libket/src/instruction.rs
 src/ket/clib/libs/libket/src/ir.rs
 src/ket/clib/libs/libket/src/lib.rs
```

### Comparing `ket-lang-0.6.1.dev1/tests/test_gates.py` & `ket-lang-0.6rc2/tests/test_gates.py`

 * *Files identical despite different names*

