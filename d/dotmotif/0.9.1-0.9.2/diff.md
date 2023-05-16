# Comparing `tmp/dotmotif-0.9.1.tar.gz` & `tmp/dotmotif-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dotmotif-0.9.1.tar", last modified: Thu May  6 18:44:39 2021, max compression
+gzip compressed data, was "dist/dotmotif-0.9.2.tar", last modified: Sat May 29 02:20:16 2021, max compression
```

## Comparing `dotmotif-0.9.1.tar` & `dotmotif-0.9.2.tar`

### file list

```diff
@@ -1,84 +1,82 @@
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/.circleci/
--rw-r--r--   0 mateljk1   (501) staff       (20)     1052 2020-10-14 14:00:36.000000 dotmotif-0.9.1/.circleci/config.yml
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/.github/
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/.github/workflows/
--rw-r--r--   0 mateljk1   (501) staff       (20)     1402 2021-01-08 01:58:09.000000 dotmotif-0.9.1/.github/workflows/python-package.yml
--rw-r--r--   0 mateljk1   (501) staff       (20)     1874 2020-03-23 15:56:31.000000 dotmotif-0.9.1/.gitignore
--rw-r--r--   0 mateljk1   (501) staff       (20)    14810 2020-03-23 15:56:31.000000 dotmotif-0.9.1/.pylintrc
--rw-r--r--   0 mateljk1   (501) staff       (20)     6342 2021-05-06 18:43:52.000000 dotmotif-0.9.1/CHANGELOG.md
--rw-r--r--   0 mateljk1   (501) staff       (20)    10140 2020-09-17 14:36:45.000000 dotmotif-0.9.1/LICENSE
--rw-r--r--   0 mateljk1   (501) staff       (20)       40 2020-10-14 14:00:36.000000 dotmotif-0.9.1/MANIFEST.in
--rw-r--r--   0 mateljk1   (501) staff       (20)     5881 2021-05-06 18:44:39.000000 dotmotif-0.9.1/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)     4663 2021-05-06 18:43:52.000000 dotmotif-0.9.1/README.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/
--rw-r--r--   0 mateljk1   (501) staff       (20)      196 2020-10-14 14:00:36.000000 dotmotif-0.9.1/docs/README.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/examples/
--rw-r--r--   0 mateljk1   (501) staff       (20)      407 2020-10-14 14:22:25.000000 dotmotif-0.9.1/docs/examples/Counting Triangles in MICrONS v185.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/graphics/
--rw-r--r--   0 mateljk1   (501) staff       (20)     2584 2020-03-23 15:56:31.000000 dotmotif-0.9.1/docs/graphics/grant-fig-syntax.html
--rw-r--r--   0 mateljk1   (501) staff       (20)     6545 2020-03-23 15:56:31.000000 dotmotif-0.9.1/docs/graphics/grant-rough-text.tex.frag
--rw-r--r--   0 mateljk1   (501) staff       (20)  2466887 2020-03-23 15:56:31.000000 dotmotif-0.9.1/docs/graphics/takemura-dm-all-participants.svg
--rw-r--r--   0 mateljk1   (501) staff       (20)  2466887 2020-03-23 15:56:31.000000 dotmotif-0.9.1/docs/graphics/takemura-dotmotif.svg
--rw-r--r--   0 mateljk1   (501) staff       (20)     3404 2020-03-23 15:56:31.000000 dotmotif-0.9.1/docs/motif.iro
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/reference/
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/reference/dotmotif/
--rw-r--r--   0 mateljk1   (501) staff       (20)     2256 2021-01-23 15:59:04.000000 dotmotif-0.9.1/docs/reference/dotmotif/dotmotif.md
--rw-r--r--   0 mateljk1   (501) staff       (20)      354 2021-01-23 15:49:23.000000 dotmotif-0.9.1/docs/reference/dotmotif/utils.py.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/reference/executors/
--rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:49:23.000000 dotmotif-0.9.1/docs/reference/executors/Executor.py.md
--rw-r--r--   0 mateljk1   (501) staff       (20)      133 2021-01-23 15:59:04.000000 dotmotif-0.9.1/docs/reference/executors/GrandIsoExecutor.py.md
--rw-r--r--   0 mateljk1   (501) staff       (20)     3025 2021-01-23 15:59:04.000000 dotmotif-0.9.1/docs/reference/executors/Neo4jExecutor.py.md
--rw-r--r--   0 mateljk1   (501) staff       (20)      969 2021-01-23 15:49:23.000000 dotmotif-0.9.1/docs/reference/executors/NetworkXExecutor.py.md
--rw-r--r--   0 mateljk1   (501) staff       (20)     1826 2021-01-23 15:59:04.000000 dotmotif-0.9.1/docs/reference/executors/NeuPrintExecutor.py.md
--rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:49:23.000000 dotmotif-0.9.1/docs/reference/executors/executors.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/reference/ingest/
--rw-r--r--   0 mateljk1   (501) staff       (20)     1938 2021-01-23 15:59:04.000000 dotmotif-0.9.1/docs/reference/ingest/ingest.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/reference/parsers/
--rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:49:23.000000 dotmotif-0.9.1/docs/reference/parsers/parsers.md
--rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:48:45.000000 dotmotif-0.9.1/docs/reference/setup.py.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/docs/reference/validators/
--rw-r--r--   0 mateljk1   (501) staff       (20)      281 2021-01-23 15:49:23.000000 dotmotif-0.9.1/docs/reference/validators/validators.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/
--rw-r--r--   0 mateljk1   (501) staff       (20)     6675 2021-03-23 17:49:46.000000 dotmotif-0.9.1/dotmotif/__init__.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/executors/
--rw-r--r--   0 mateljk1   (501) staff       (20)      177 2020-03-23 15:56:31.000000 dotmotif-0.9.1/dotmotif/executors/Executor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     4619 2021-05-06 18:43:52.000000 dotmotif-0.9.1/dotmotif/executors/GrandIsoExecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    17161 2021-01-23 15:59:04.000000 dotmotif-0.9.1/dotmotif/executors/Neo4jExecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     9741 2021-01-08 03:01:43.000000 dotmotif-0.9.1/dotmotif/executors/NetworkXExecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     3552 2021-01-20 13:15:21.000000 dotmotif-0.9.1/dotmotif/executors/NeuPrintExecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)      772 2020-10-14 14:00:36.000000 dotmotif-0.9.1/dotmotif/executors/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     6293 2020-07-23 16:17:33.000000 dotmotif-0.9.1/dotmotif/executors/test_dm_cypher.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    10128 2020-10-14 14:00:36.000000 dotmotif-0.9.1/dotmotif/executors/test_grandisoexecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)      962 2020-06-30 16:30:54.000000 dotmotif-0.9.1/dotmotif/executors/test_neo4jexecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    17802 2021-01-08 03:01:43.000000 dotmotif-0.9.1/dotmotif/executors/test_networkxexecutor.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     1548 2020-07-23 21:50:31.000000 dotmotif-0.9.1/dotmotif/executors/test_neuprintexecutor.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/ingest/
--rw-r--r--   0 mateljk1   (501) staff       (20)     8759 2021-03-02 15:15:31.000000 dotmotif-0.9.1/dotmotif/ingest/__init__.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/parsers/
--rw-r--r--   0 mateljk1   (501) staff       (20)      152 2020-03-23 15:56:31.000000 dotmotif-0.9.1/dotmotif/parsers/__init__.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/parsers/v1/
--rw-r--r--   0 mateljk1   (501) staff       (20)     2282 2020-07-23 16:17:33.000000 dotmotif-0.9.1/dotmotif/parsers/v1/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     1553 2020-03-23 15:56:31.000000 dotmotif-0.9.1/dotmotif/parsers/v1/test_dm_parse.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/parsers/v2/
--rw-r--r--   0 mateljk1   (501) staff       (20)    11473 2021-01-08 03:01:43.000000 dotmotif-0.9.1/dotmotif/parsers/v2/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     4288 2021-01-08 03:01:43.000000 dotmotif-0.9.1/dotmotif/parsers/v2/grammar.lark
--rw-r--r--   0 mateljk1   (501) staff       (20)    13026 2021-01-08 02:08:40.000000 dotmotif-0.9.1/dotmotif/parsers/v2/test_v2_parser.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/tests/
--rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-03-02 15:39:27.000000 dotmotif-0.9.1/dotmotif/tests/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     2861 2021-03-02 15:39:27.000000 dotmotif-0.9.1/dotmotif/tests/test_dm_flags.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     1300 2021-03-02 15:39:27.000000 dotmotif-0.9.1/dotmotif/tests/test_utils.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     1502 2020-09-17 14:36:45.000000 dotmotif-0.9.1/dotmotif/utils.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif/validators/
--rw-r--r--   0 mateljk1   (501) staff       (20)     1222 2020-03-23 15:56:31.000000 dotmotif-0.9.1/dotmotif/validators/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)      954 2021-03-02 15:39:27.000000 dotmotif-0.9.1/dotmotif/validators/test_dm_illegal_operators.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-06 18:44:39.000000 dotmotif-0.9.1/dotmotif.egg-info/
--rw-r--r--   0 mateljk1   (501) staff       (20)     5881 2021-05-06 18:44:38.000000 dotmotif-0.9.1/dotmotif.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)     1890 2021-05-06 18:44:38.000000 dotmotif-0.9.1/dotmotif.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        1 2021-05-06 18:44:38.000000 dotmotif-0.9.1/dotmotif.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)      112 2021-05-06 18:44:38.000000 dotmotif-0.9.1/dotmotif.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        9 2021-05-06 18:44:38.000000 dotmotif-0.9.1/dotmotif.egg-info/top_level.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)     5749 2020-03-23 15:56:31.000000 dotmotif-0.9.1/logo.png
--rw-r--r--   0 mateljk1   (501) staff       (20)      117 2021-05-06 18:43:52.000000 dotmotif-0.9.1/requirements.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       38 2021-05-06 18:44:39.000000 dotmotif-0.9.1/setup.cfg
--rw-r--r--   0 mateljk1   (501) staff       (20)     1163 2021-05-06 18:43:52.000000 dotmotif-0.9.1/setup.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/.github/
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/.github/workflows/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1402 2021-01-08 01:58:09.000000 dotmotif-0.9.2/.github/workflows/python-package.yml
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1874 2020-03-23 15:56:31.000000 dotmotif-0.9.2/.gitignore
+-rw-r--r--   0 mateljk1   (501) staff       (20)    14810 2020-03-23 15:56:31.000000 dotmotif-0.9.2/.pylintrc
+-rw-r--r--   0 mateljk1   (501) staff       (20)     6563 2021-05-29 02:19:07.000000 dotmotif-0.9.2/CHANGELOG.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10140 2020-09-17 14:36:45.000000 dotmotif-0.9.2/LICENSE
+-rw-r--r--   0 mateljk1   (501) staff       (20)       40 2020-10-14 14:00:36.000000 dotmotif-0.9.2/MANIFEST.in
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5970 2021-05-29 02:20:16.000000 dotmotif-0.9.2/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4752 2021-05-06 18:55:04.000000 dotmotif-0.9.2/README.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      196 2020-10-14 14:00:36.000000 dotmotif-0.9.2/docs/README.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/examples/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      407 2020-10-14 14:22:25.000000 dotmotif-0.9.2/docs/examples/Counting Triangles in MICrONS v185.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/graphics/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2584 2020-03-23 15:56:31.000000 dotmotif-0.9.2/docs/graphics/grant-fig-syntax.html
+-rw-r--r--   0 mateljk1   (501) staff       (20)     6545 2020-03-23 15:56:31.000000 dotmotif-0.9.2/docs/graphics/grant-rough-text.tex.frag
+-rw-r--r--   0 mateljk1   (501) staff       (20)  2466887 2020-03-23 15:56:31.000000 dotmotif-0.9.2/docs/graphics/takemura-dm-all-participants.svg
+-rw-r--r--   0 mateljk1   (501) staff       (20)  2466887 2020-03-23 15:56:31.000000 dotmotif-0.9.2/docs/graphics/takemura-dotmotif.svg
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5749 2021-05-06 18:55:04.000000 dotmotif-0.9.2/docs/logo.png
+-rw-r--r--   0 mateljk1   (501) staff       (20)     3404 2020-03-23 15:56:31.000000 dotmotif-0.9.2/docs/motif.iro
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/reference/
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/reference/dotmotif/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2256 2021-01-23 15:59:04.000000 dotmotif-0.9.2/docs/reference/dotmotif/dotmotif.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)      354 2021-01-23 15:49:23.000000 dotmotif-0.9.2/docs/reference/dotmotif/utils.py.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/reference/executors/
+-rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:49:23.000000 dotmotif-0.9.2/docs/reference/executors/Executor.py.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)      133 2021-01-23 15:59:04.000000 dotmotif-0.9.2/docs/reference/executors/GrandIsoExecutor.py.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)     3025 2021-01-23 15:59:04.000000 dotmotif-0.9.2/docs/reference/executors/Neo4jExecutor.py.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)      969 2021-01-23 15:49:23.000000 dotmotif-0.9.2/docs/reference/executors/NetworkXExecutor.py.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1826 2021-01-23 15:59:04.000000 dotmotif-0.9.2/docs/reference/executors/NeuPrintExecutor.py.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:49:23.000000 dotmotif-0.9.2/docs/reference/executors/executors.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/reference/ingest/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1938 2021-01-23 15:59:04.000000 dotmotif-0.9.2/docs/reference/ingest/ingest.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/reference/parsers/
+-rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:49:23.000000 dotmotif-0.9.2/docs/reference/parsers/parsers.md
+-rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-01-23 15:48:45.000000 dotmotif-0.9.2/docs/reference/setup.py.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/docs/reference/validators/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      281 2021-01-23 15:49:23.000000 dotmotif-0.9.2/docs/reference/validators/validators.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     6675 2021-05-29 02:18:35.000000 dotmotif-0.9.2/dotmotif/__init__.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/executors/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      177 2020-03-23 15:56:31.000000 dotmotif-0.9.2/dotmotif/executors/Executor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     3967 2021-05-29 02:18:08.000000 dotmotif-0.9.2/dotmotif/executors/GrandIsoExecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    17161 2021-01-23 15:59:04.000000 dotmotif-0.9.2/dotmotif/executors/Neo4jExecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10348 2021-05-29 02:18:08.000000 dotmotif-0.9.2/dotmotif/executors/NetworkXExecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     3552 2021-01-20 13:15:21.000000 dotmotif-0.9.2/dotmotif/executors/NeuPrintExecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      772 2020-10-14 14:00:36.000000 dotmotif-0.9.2/dotmotif/executors/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     6293 2020-07-23 16:17:33.000000 dotmotif-0.9.2/dotmotif/executors/test_dm_cypher.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10128 2020-10-14 14:00:36.000000 dotmotif-0.9.2/dotmotif/executors/test_grandisoexecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      962 2020-06-30 16:30:54.000000 dotmotif-0.9.2/dotmotif/executors/test_neo4jexecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    17802 2021-01-08 03:01:43.000000 dotmotif-0.9.2/dotmotif/executors/test_networkxexecutor.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1548 2021-05-28 21:06:40.000000 dotmotif-0.9.2/dotmotif/executors/test_neuprintexecutor.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/ingest/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     8759 2021-03-02 15:15:31.000000 dotmotif-0.9.2/dotmotif/ingest/__init__.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/parsers/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      152 2020-03-23 15:56:31.000000 dotmotif-0.9.2/dotmotif/parsers/__init__.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/parsers/v1/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2282 2020-07-23 16:17:33.000000 dotmotif-0.9.2/dotmotif/parsers/v1/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1553 2020-03-23 15:56:31.000000 dotmotif-0.9.2/dotmotif/parsers/v1/test_dm_parse.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/parsers/v2/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    11473 2021-01-08 03:01:43.000000 dotmotif-0.9.2/dotmotif/parsers/v2/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     4288 2021-01-08 03:01:43.000000 dotmotif-0.9.2/dotmotif/parsers/v2/grammar.lark
+-rw-r--r--   0 mateljk1   (501) staff       (20)    13026 2021-01-08 02:08:40.000000 dotmotif-0.9.2/dotmotif/parsers/v2/test_v2_parser.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/tests/
+-rw-r--r--   0 mateljk1   (501) staff       (20)        0 2021-03-02 15:39:27.000000 dotmotif-0.9.2/dotmotif/tests/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2861 2021-03-02 15:39:27.000000 dotmotif-0.9.2/dotmotif/tests/test_dm_flags.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1300 2021-03-02 15:39:27.000000 dotmotif-0.9.2/dotmotif/tests/test_utils.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1502 2020-09-17 14:36:45.000000 dotmotif-0.9.2/dotmotif/utils.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif/validators/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1222 2020-03-23 15:56:31.000000 dotmotif-0.9.2/dotmotif/validators/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      954 2021-03-02 15:39:27.000000 dotmotif-0.9.2/dotmotif/validators/test_dm_illegal_operators.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif.egg-info/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5970 2021-05-29 02:20:15.000000 dotmotif-0.9.2/dotmotif.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1874 2021-05-29 02:20:16.000000 dotmotif-0.9.2/dotmotif.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        1 2021-05-29 02:20:15.000000 dotmotif-0.9.2/dotmotif.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)      112 2021-05-29 02:20:15.000000 dotmotif-0.9.2/dotmotif.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        9 2021-05-29 02:20:15.000000 dotmotif-0.9.2/dotmotif.egg-info/top_level.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)      117 2021-05-29 02:18:08.000000 dotmotif-0.9.2/requirements.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       38 2021-05-29 02:20:16.000000 dotmotif-0.9.2/setup.cfg
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1163 2021-05-29 02:19:29.000000 dotmotif-0.9.2/setup.py
```

### Comparing `dotmotif-0.9.1/.github/workflows/python-package.yml` & `dotmotif-0.9.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/.gitignore` & `dotmotif-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/.pylintrc` & `dotmotif-0.9.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/CHANGELOG.md` & `dotmotif-0.9.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
--   **0.9.1**
+-   **0.9.2** (May 28 2021)
     -   Features:
-        -   `GrandIsoExecutor`: Adds support for the `grandiso.find_motifs_iter` generator API in grandiso v1.2.0; this reduces the runtime of queries with nonzero `limit` #102
+        -   `GrandIsoExecutor`: Utilizes the node attribute matching flow available in grandiso≥2.0.0 to reduce complexity of attribute-heavy searches (#104)
+-   **0.9.1** (May 6 2021)
+    -   Features:
+        -   `GrandIsoExecutor`: Adds support for the `grandiso.find_motifs_iter` generator API in grandiso v1.2.0; this reduces the runtime of queries with nonzero `limit` (#102)
 -   **0.9.0** (March 23 2021)
     -   Features:
         -   `Neo4jExecutor#create_index`. This function call adds an index to the database on the node attribute specified, in order to improve query performance (#95)
         -   `dotmotif.ingest.EdgelistConverter` now supports importing from a dask or pandas dataframe edgelist in addition to files on disk (#99)
     -   Chores:
         -   Put lingering top-level tests into their own directory (#100)
 -   **0.8.1**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dotmotif-0.9.1/LICENSE` & `dotmotif-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/PKG-INFO` & `dotmotif-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dotmotif
-Version: 0.9.1
+Version: 0.9.2
 Summary: Find graph motifs using simple, intuitive notation
-Home-page: https://github.com/aplbrain/dotmotif/tarball/0.9.1
+Home-page: https://github.com/aplbrain/dotmotif/tarball/0.9.2
 Author: Jordan Matelsky
 Author-email: jordan.matelsky@jhuapl.edu
 License: Apache 2.0
 Description: 
         <p align="center">
-          <img align="center" src="./logo.png" / width="25%">
+          <img align="center" src="https://user-images.githubusercontent.com/693511/117350563-b58b9900-ae7a-11eb-83ce-9f5f9213145e.png" / width="25%">
           <h1 align="center" fontsize="2em">d o t m o t i f</h1>
         </p>
         <p align="center">Find graph motifs using intuitive notation</p>
         
         <p align="center">
         <a href="https://pypi.org/project/dotmotif/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dotmotif?style=for-the-badge"></a>
         <a href="https://bossdb.org/tools/DotMotif"><img src="https://img.shields.io/badge/Pretty Dope-👌-00ddcc.svg?style=for-the-badge" /></a>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: dotmotif Version: 0.9.1 Summary: Find graph motifs
+Metadata-Version: 2.1 Name: dotmotif Version: 0.9.2 Summary: Find graph motifs
 using simple, intuitive notation Home-page: https://github.com/aplbrain/
-dotmotif/tarball/0.9.1 Author: Jordan Matelsky Author-email:
+dotmotif/tarball/0.9.2 Author: Jordan Matelsky Author-email:
 jordan.matelsky@jhuapl.edu License: Apache 2.0 Description:
                                  width="25%">
                          ****** d o t m o t i f ******
                   Find graph motifs using intuitive notation
 [PyPI] [https://img.shields.io/badge/Pretty_Dope-ð-00ddcc.svg?style=for-the-
 badge] [https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=for-the-
                                badge] [Codecov]
```

### Comparing `dotmotif-0.9.1/README.md` & `dotmotif-0.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img align="center" src="./logo.png" / width="25%">
+  <img align="center" src="https://user-images.githubusercontent.com/693511/117350563-b58b9900-ae7a-11eb-83ce-9f5f9213145e.png" / width="25%">
   <h1 align="center" fontsize="2em">d o t m o t i f</h1>
 </p>
 <p align="center">Find graph motifs using intuitive notation</p>
 
 <p align="center">
 <a href="https://pypi.org/project/dotmotif/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dotmotif?style=for-the-badge"></a>
 <a href="https://bossdb.org/tools/DotMotif"><img src="https://img.shields.io/badge/Pretty Dope-👌-00ddcc.svg?style=for-the-badge" /></a>
```

### Comparing `dotmotif-0.9.1/docs/graphics/grant-fig-syntax.html` & `dotmotif-0.9.2/docs/graphics/grant-fig-syntax.html`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/graphics/grant-rough-text.tex.frag` & `dotmotif-0.9.2/docs/graphics/grant-rough-text.tex.frag`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/graphics/takemura-dm-all-participants.svg` & `dotmotif-0.9.2/docs/graphics/takemura-dm-all-participants.svg`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/graphics/takemura-dotmotif.svg` & `dotmotif-0.9.2/docs/graphics/takemura-dotmotif.svg`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/motif.iro` & `dotmotif-0.9.2/docs/motif.iro`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/reference/dotmotif/dotmotif.md` & `dotmotif-0.9.2/docs/reference/dotmotif/dotmotif.md`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/reference/executors/Neo4jExecutor.py.md` & `dotmotif-0.9.2/docs/reference/executors/Neo4jExecutor.py.md`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/reference/executors/NetworkXExecutor.py.md` & `dotmotif-0.9.2/docs/reference/executors/NetworkXExecutor.py.md`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/reference/executors/NeuPrintExecutor.py.md` & `dotmotif-0.9.2/docs/reference/executors/NeuPrintExecutor.py.md`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/docs/reference/ingest/ingest.md` & `dotmotif-0.9.2/docs/reference/ingest/ingest.md`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/__init__.py` & `dotmotif-0.9.2/dotmotif/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Copyright 2020 The Johns Hopkins University Applied Physics Laboratory.
+Copyright 2021 The Johns Hopkins University Applied Physics Laboratory.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -26,15 +26,15 @@
 from .parsers.v2 import ParserV2
 from .validators import DisagreeingEdgesValidator
 
 from .executors.NetworkXExecutor import NetworkXExecutor
 from .executors.GrandIsoExecutor import GrandIsoExecutor
 from .executors.Neo4jExecutor import Neo4jExecutor
 
-__version__ = "0.9.0"
+__version__ = "0.9.2"
 
 DEFAULT_MOTIF_PARSER = ParserV2
 
 
 class MotifError(ValueError):
     pass
```

### Comparing `dotmotif-0.9.1/dotmotif/executors/GrandIsoExecutor.py` & `dotmotif-0.9.2/dotmotif/executors/GrandIsoExecutor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,54 @@
 """
-Copyright 2020 The Johns Hopkins University Applied Physics Laboratory.
+Copyright 2021 The Johns Hopkins University Applied Physics Laboratory.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.`
 """
-
+from functools import lru_cache
 import networkx as nx
 from grandiso import find_motifs_iter
 
-from .NetworkXExecutor import NetworkXExecutor
+from .NetworkXExecutor import NetworkXExecutor, _node_satisfies_constraints
 
 
 class GrandIsoExecutor(NetworkXExecutor):
+    """
+    A DotMotif executor that uses grandiso for subgraph monomorphism.
+
+    This executor is dramatically fast than the NetworkX search, and is still
+    a pure-Python implementation.
+
+    [GrandIso](https://github.com/aplbrain/grandiso-networkx)
+
+    """
+
     def find(self, motif, limit: int = None):
         """
         Find a motif in a larger graph.
 
         Arguments:
-            motif (dotmotif.dotmotif)
+            motif (dotmotif.Motif)
+            limit (int: None)
 
-        """
-        # TODO: Can add constraints on iso node assignment. If we do this a
-        # little smarter, can save a lot of post-processing time-complexity.
+        Returns:
+            List[dict]
 
+        """
         # We need to first remove "negative" nodes from the motif, and then
-        # filter them out later on. Though this reduces the speed of the graph-
-        # matching, NetworkX does not seem to support this out of the box.
-
-        # Two important notes, if you're planning on messing with this method:
-        # The first: The function signature of the `grandiso.find_motifs` call
-        # is the reverse of the NetworkX signature. In other words, in networkx
-        # you call (host, motif). In GrandIso, you call (motif, host). This is
-        # intentional because it enables better partial function calls that
-        # reuse the same motif, which -- if you're using Grand at least --
-        # means that you're avoiding having to serialize the heavy Host graph.
-        # But it is sorta confusing. Not clear if it's going to stay that way,
-        # but for now it's hardly worth the trouble.
-        # The second important note is that GrandIso decides for itself whether
-        # it's going to be able to perform a directed or undirected motif
-        # search; the user doesn't get to decide. (After all, the user
-        # shouldn't have the option to request a poorly defined operation. APIs
-        # should be smart enough to know what you want while avoiding adding
-        # complexity. Anyway, soapbox over.) To that end, this confirmation
-        # that the motif is directed is kinda... Unimportant.
-        graph_matcher = find_motifs_iter
+        # filter them out later on.
 
         if motif.ignore_direction or not self.graph.is_directed:
             graph_constructor = nx.Graph
         else:
             graph_constructor = nx.DiGraph
 
         only_positive_edges_motif = graph_constructor()
@@ -70,25 +62,40 @@
 
         def _doesnt_have_any_of_motifs_negative_edges(mapping):
             for u, v in must_not_exist_edges:
                 if self.graph.has_edge(mapping[u], mapping[v]):
                     return False
             return True
 
-        graph_matches = graph_matcher(only_positive_edges_motif, self.graph)
+        constraints = motif.list_node_constraints()
+
+        @lru_cache()
+        def _node_attr_match_fn(
+            motif_node_id: str, host_node_id: str, motif_nx: nx.Graph, host_nx: nx.Graph
+        ):
+            return _node_satisfies_constraints(
+                host_nx.nodes[host_node_id], constraints.get(motif_node_id, {})
+            )
+            return True
+
+        graph_matches = find_motifs_iter(
+            only_positive_edges_motif,
+            self.graph,
+            is_node_attr_match=_node_attr_match_fn,
+        )
 
         results = []
         for r in graph_matches:
             if _doesnt_have_any_of_motifs_negative_edges(r) and (
                 self._validate_edge_constraints(
                     r, self.graph, motif.list_edge_constraints()
                 )
-                and self._validate_node_constraints(
-                    r, self.graph, motif.list_node_constraints()
-                )
+                # and self._validate_node_constraints(
+                #     r, self.graph, motif.list_node_constraints()
+                # )
                 and self._validate_dynamic_node_constraints(
                     r, self.graph, motif.list_dynamic_node_constraints()
                 )
                 # by default, networkx returns the automorphism that is left-
                 # sorted, so this comparison is _opposite_ the check that we
                 # use in the other executors. In other words, we usually check
                 # that A >= B; here we check A <= B.
```

### Comparing `dotmotif-0.9.1/dotmotif/executors/Neo4jExecutor.py` & `dotmotif-0.9.2/dotmotif/executors/Neo4jExecutor.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/NetworkXExecutor.py` & `dotmotif-0.9.2/dotmotif/executors/NetworkXExecutor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2021 The Johns Hopkins University Applied Physics Laboratory.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.`
+"""
+
 from typing import TYPE_CHECKING
 import networkx as nx
 import pandas as pd
 
 from .Executor import Executor
 
 if TYPE_CHECKING:
```

### Comparing `dotmotif-0.9.1/dotmotif/executors/NeuPrintExecutor.py` & `dotmotif-0.9.2/dotmotif/executors/NeuPrintExecutor.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/__init__.py` & `dotmotif-0.9.2/dotmotif/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/test_dm_cypher.py` & `dotmotif-0.9.2/dotmotif/executors/test_dm_cypher.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/test_grandisoexecutor.py` & `dotmotif-0.9.2/dotmotif/executors/test_grandisoexecutor.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/test_neo4jexecutor.py` & `dotmotif-0.9.2/dotmotif/executors/test_neo4jexecutor.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/test_networkxexecutor.py` & `dotmotif-0.9.2/dotmotif/executors/test_networkxexecutor.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/executors/test_neuprintexecutor.py` & `dotmotif-0.9.2/dotmotif/executors/test_neuprintexecutor.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/ingest/__init__.py` & `dotmotif-0.9.2/dotmotif/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/parsers/v1/__init__.py` & `dotmotif-0.9.2/dotmotif/parsers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/parsers/v1/test_dm_parse.py` & `dotmotif-0.9.2/dotmotif/parsers/v1/test_dm_parse.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/parsers/v2/__init__.py` & `dotmotif-0.9.2/dotmotif/parsers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/parsers/v2/grammar.lark` & `dotmotif-0.9.2/dotmotif/parsers/v2/grammar.lark`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/parsers/v2/test_v2_parser.py` & `dotmotif-0.9.2/dotmotif/parsers/v2/test_v2_parser.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/tests/test_dm_flags.py` & `dotmotif-0.9.2/dotmotif/tests/test_dm_flags.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/tests/test_utils.py` & `dotmotif-0.9.2/dotmotif/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/utils.py` & `dotmotif-0.9.2/dotmotif/utils.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/validators/__init__.py` & `dotmotif-0.9.2/dotmotif/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif/validators/test_dm_illegal_operators.py` & `dotmotif-0.9.2/dotmotif/validators/test_dm_illegal_operators.py`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/dotmotif.egg-info/PKG-INFO` & `dotmotif-0.9.2/dotmotif.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dotmotif
-Version: 0.9.1
+Version: 0.9.2
 Summary: Find graph motifs using simple, intuitive notation
-Home-page: https://github.com/aplbrain/dotmotif/tarball/0.9.1
+Home-page: https://github.com/aplbrain/dotmotif/tarball/0.9.2
 Author: Jordan Matelsky
 Author-email: jordan.matelsky@jhuapl.edu
 License: Apache 2.0
 Description: 
         <p align="center">
-          <img align="center" src="./logo.png" / width="25%">
+          <img align="center" src="https://user-images.githubusercontent.com/693511/117350563-b58b9900-ae7a-11eb-83ce-9f5f9213145e.png" / width="25%">
           <h1 align="center" fontsize="2em">d o t m o t i f</h1>
         </p>
         <p align="center">Find graph motifs using intuitive notation</p>
         
         <p align="center">
         <a href="https://pypi.org/project/dotmotif/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dotmotif?style=for-the-badge"></a>
         <a href="https://bossdb.org/tools/DotMotif"><img src="https://img.shields.io/badge/Pretty Dope-👌-00ddcc.svg?style=for-the-badge" /></a>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: dotmotif Version: 0.9.1 Summary: Find graph motifs
+Metadata-Version: 2.1 Name: dotmotif Version: 0.9.2 Summary: Find graph motifs
 using simple, intuitive notation Home-page: https://github.com/aplbrain/
-dotmotif/tarball/0.9.1 Author: Jordan Matelsky Author-email:
+dotmotif/tarball/0.9.2 Author: Jordan Matelsky Author-email:
 jordan.matelsky@jhuapl.edu License: Apache 2.0 Description:
                                  width="25%">
                          ****** d o t m o t i f ******
                   Find graph motifs using intuitive notation
 [PyPI] [https://img.shields.io/badge/Pretty_Dope-ð-00ddcc.svg?style=for-the-
 badge] [https://img.shields.io/badge/License-Apache_2.0-blue.svg?style=for-the-
                                badge] [Codecov]
```

### Comparing `dotmotif-0.9.1/dotmotif.egg-info/SOURCES.txt` & `dotmotif-0.9.2/dotmotif.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 .gitignore
 .pylintrc
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
-logo.png
 requirements.txt
 setup.py
-.circleci/config.yml
 .github/workflows/python-package.yml
 docs/README.md
+docs/logo.png
 docs/motif.iro
 docs/examples/Counting Triangles in MICrONS v185.py
 docs/graphics/grant-fig-syntax.html
 docs/graphics/grant-rough-text.tex.frag
 docs/graphics/takemura-dm-all-participants.svg
 docs/graphics/takemura-dotmotif.svg
 docs/reference/setup.py.md
```

### Comparing `dotmotif-0.9.1/logo.png` & `dotmotif-0.9.2/docs/logo.png`

 * *Files identical despite different names*

### Comparing `dotmotif-0.9.1/setup.py` & `dotmotif-0.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 git tag {VERSION}
 git push --tags
 python setup.py sdist
 twine upload dist/*
 """
 
-VERSION = "0.9.1"
+VERSION = "0.9.2"
 
 here = os.path.abspath(os.path.dirname(__file__))
 with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 setup(
     name="dotmotif",
@@ -36,11 +36,11 @@
         "lark-parser",
         "docker",
         "pandas",
         "py2neo",
         "dask[dataframe]",
         "tamarind>=0.1.5",
         "neuprint-python",
-        "grandiso>=1.2.0",
+        "grandiso>=2.0.0",
     ],
     include_package_data=True,
 )
```

