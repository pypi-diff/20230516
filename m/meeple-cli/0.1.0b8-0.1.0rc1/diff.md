# Comparing `tmp/meeple-cli-0.1.0b8.tar.gz` & `tmp/meeple_cli-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeple-cli-0.1.0b8.tar", last modified: Thu May 11 02:20:26 2023, max compression
+gzip compressed data, was "meeple_cli-0.1.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meeple-cli-0.1.0b8.tar` & `meeple_cli-0.1.0rc1.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0       66 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/.flake8
--rw-r--r--   0        0        0     1090 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1279 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      289 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/.gitignore
--rw-r--r--   0        0        0      168 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/.markdownlint.yaml
--rw-r--r--   0        0        0     1347 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/LICENSE
--rw-r--r--   0        0        0     4265 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/README.md
--rw-r--r--   0        0        0      249 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/codecov.yml
--rw-r--r--   0        0        0     7118 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/docs/changelog.md
--rw-r--r--   0        0        0      838 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/justfile
--rw-r--r--   0        0        0     1014 2023-05-11 02:20:19.879829 meeple-cli-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/__init__.py
--rw-r--r--   0        0        0      639 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/__init__.py
--rw-r--r--   0        0        0     2118 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/add.py
--rw-r--r--   0        0        0     2676 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/collections.py
--rw-r--r--   0        0        0      955 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/completions.py
--rw-r--r--   0        0        0     1502 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/delete.py
--rw-r--r--   0        0        0     2138 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/drop.py
--rw-r--r--   0        0        0     5843 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/find.py
--rw-r--r--   0        0        0      670 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/hot.py
--rw-r--r--   0        0        0     1528 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/info.py
--rw-r--r--   0        0        0     3973 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/list.py
--rw-r--r--   0        0        0     3257 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/move.py
--rw-r--r--   0        0        0      765 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/new.py
--rw-r--r--   0        0        0     1271 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/open.py
--rw-r--r--   0        0        0     1361 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/rename.py
--rw-r--r--   0        0        0     1250 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/search.py
--rw-r--r--   0        0        0     4026 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/stats.py
--rw-r--r--   0        0        0     3893 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/command/update.py
--rw-r--r--   0        0        0     1153 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/root.py
--rw-r--r--   0        0        0        0 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/type/__init__.py
--rw-r--r--   0        0        0      278 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/type/collection.py
--rw-r--r--   0        0        0     4385 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/type/item.py
--rw-r--r--   0        0        0        0 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/__init__.py
--rw-r--r--   0        0        0     1450 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/api_util.py
--rw-r--r--   0        0        0      697 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/cmd_util.py
--rw-r--r--   0        0        0     3229 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/collection_util.py
--rw-r--r--   0        0        0      235 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/completion_util.py
--rw-r--r--   0        0        0     2486 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/data_util.py
--rw-r--r--   0        0        0      927 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/filter_util.py
--rw-r--r--   0        0        0      617 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/fs_util.py
--rw-r--r--   0        0        0      320 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/input_util.py
--rw-r--r--   0        0        0     4025 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/output_util.py
--rw-r--r--   0        0        0     2616 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/src/meeple/util/sort_util.py
--rw-r--r--   0        0        0        0 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/__init__.py
--rw-r--r--   0        0        0      313 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/test_root.py
--rw-r--r--   0        0        0        0 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/util/__init__.py
--rw-r--r--   0        0        0     1879 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/util/test_filter_util.py
--rw-r--r--   0        0        0     2188 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/util/test_fs_util.py
--rw-r--r--   0        0        0     2274 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/util/test_output_util.py
--rw-r--r--   0        0        0     2525 2023-05-11 02:20:19.883828 meeple-cli-0.1.0b8/tests/util/test_sort_util.py
--rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.flake8
+-rw-r--r--   0        0        0     1090 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1279 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      289 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.gitignore
+-rw-r--r--   0        0        0      168 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.markdownlint.yaml
+-rw-r--r--   0        0        0     1358 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     4915 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/README.md
+-rw-r--r--   0        0        0      249 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/codecov.yml
+-rw-r--r--   0        0        0     7919 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/docs/changelog.md
+-rw-r--r--   0        0        0      837 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/justfile
+-rw-r--r--   0        0        0     1014 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/__init__.py
+-rw-r--r--   0        0        0     1915 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/add.py
+-rw-r--r--   0        0        0     2584 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/collections.py
+-rw-r--r--   0        0        0      948 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/completions.py
+-rw-r--r--   0        0        0     1434 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/delete.py
+-rw-r--r--   0        0        0     1903 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/drop.py
+-rw-r--r--   0        0        0     5726 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/find.py
+-rw-r--r--   0        0        0      701 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/hot.py
+-rw-r--r--   0        0        0     1604 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/info.py
+-rw-r--r--   0        0        0     4072 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/list.py
+-rw-r--r--   0        0        0     3464 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/move.py
+-rw-r--r--   0        0        0      684 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/new.py
+-rw-r--r--   0        0        0     1186 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/open.py
+-rw-r--r--   0        0        0     1238 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/rename.py
+-rw-r--r--   0        0        0     1233 2023-05-16 03:35:54.998165 meeple_cli-0.1.0rc1/src/meeple/command/search.py
+-rw-r--r--   0        0        0     3917 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/command/stats.py
+-rw-r--r--   0        0        0     3652 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/command/update.py
+-rw-r--r--   0        0        0     1153 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/root.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/type/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/type/collection.py
+-rw-r--r--   0        0        0     4385 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/type/item.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/__init__.py
+-rw-r--r--   0        0        0     1460 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/api_util.py
+-rw-r--r--   0        0        0      702 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/cmd_util.py
+-rw-r--r--   0        0        0     3255 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/collection_util.py
+-rw-r--r--   0        0        0      235 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/completion_util.py
+-rw-r--r--   0        0        0     2877 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/data_util.py
+-rw-r--r--   0        0        0      927 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/filter_util.py
+-rw-r--r--   0        0        0     2298 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/fmt_util.py
+-rw-r--r--   0        0        0      617 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/fs_util.py
+-rw-r--r--   0        0        0      357 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/input_util.py
+-rw-r--r--   0        0        0      945 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/message_util.py
+-rw-r--r--   0        0        0     2614 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/sort_util.py
+-rw-r--r--   0        0        0     1323 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/src/meeple/util/table_util.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/test_root.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/__init__.py
+-rw-r--r--   0        0        0     1879 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_filter_util.py
+-rw-r--r--   0        0        0     2296 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_fmt_util.py
+-rw-r--r--   0        0        0     2188 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_fs_util.py
+-rw-r--r--   0        0        0     2525 2023-05-16 03:35:55.002165 meeple_cli-0.1.0rc1/tests/util/test_sort_util.py
+-rw-r--r--   0        0        0     5915 1970-01-01 00:00:00.000000 meeple_cli-0.1.0rc1/PKG-INFO
```

### Comparing `meeple-cli-0.1.0b8/.github/workflows/python-publish.yml` & `meeple_cli-0.1.0rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/.github/workflows/python-test.yml` & `meeple_cli-0.1.0rc1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/.pre-commit-config.yaml` & `meeple_cli-0.1.0rc1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-toml
       - id: check-added-large-files
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.267
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
@@ -23,27 +23,27 @@
     hooks:
       - id: flake8
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.22.0
+    rev: 0.23.0
     hooks:
       - id: check-github-workflows
   - repo: https://github.com/gitleaks/gitleaks
-    rev: v8.16.2
+    rev: v8.16.3
     hooks:
       - id: gitleaks
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
   - repo: https://github.com/returntocorp/semgrep
-    rev: v1.17.1
+    rev: v1.21.0
     hooks:
       - id: semgrep
         args: ["--config", "auto", "--error", "--skip-unknown-extensions"]
   - repo: https://github.com/dosisod/refurb
-    rev: v1.15.0
+    rev: v1.16.0
     hooks:
       - id: refurb
```

### Comparing `meeple-cli-0.1.0b8/LICENSE` & `meeple_cli-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/README.md` & `meeple_cli-0.1.0rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -132,14 +132,26 @@
 [BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
 provides limited _read-only_ data about user collections/GeekLists.
 
 While it is _technically_ feasible to interface with GeekLists via
 webscrapers/spiders, this kind of practice would be both complex and also
 violate [BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
 
+### Why do some items show a weight of `NA` when boardgamegeek.com has a value?
+
+This is a known and occasionally recurring bug in the BoardGameGeek database. It
+usually resolves itself within a day. For more info or additional support, read
+this [thread](https://boardgamegeek.com/thread/3049286/some-games-show-weight-000).
+
+Luckily for us, game weights do not often change drastically. In most cases, we
+can assume that the weight from yesterday is _close enough_.
+[In the future](https://github.com/boldandbrad/meeple-cli/issues/61),
+`meeple-cli` will account for this automatically and display the last known
+value by default, if there is one.
+
 ### Where does `meeple-cli` store data?
 
 `meeple-cli` stores collection data in `~/.meeple` and only makes network
 connections to retrieve data from the BoardGameGeek API.
 
 ## License
```

### Comparing `meeple-cli-0.1.0b8/docs/changelog.md` & `meeple_cli-0.1.0rc1/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,37 @@
 The format is based on
 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/ "Keep a Changelog"),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html "Semantic Versioning").
 
 ## [Unreleased]
 
+## [v0.1.0rc1] - 2023-05-15
+
+### Added
+
+- `meeple list` - Show warning message when the collection has pending changes.
+- `meeple move`
+  - Gracefully handle the re-removal of items slated to be added to the source collection.
+  - Gracefully handle the re-addition of items slated to be dropped from the destination collection.
+
+### Changed
+
+- `meeple add`/`meeple drop`/`meeple move`/`meeple update` - Update output message wording.
+- `meeple update` - Skipped collection output is now dimmed.
+- `GENERAL` - Reduce duplicate code.
+
+### Fixed
+
+- `meeple add`
+  - Remove rogue `'` character in output.
+  - Properly colorize collection name in output.
+- `meeple search` - Properly show error message when no results found matching query.
+- `meeple collections` - Properly dim NA _Last Updated_ value.
+
 ## [v0.1.0b8] - 2023-05-10
 
 ### Fixed
 
 - `meeple stats`: `-b/-e` - Fix output format issue.
 
 ## [v0.1.0b7] - 2023-05-10
@@ -55,15 +78,15 @@
   result is a process termination.
 
 ## [v0.1.0b6] - 2023-04-16
 
 ### Added
 
 - `GENERAL` - Sortedby column indicator in sorted output.
-- `meeple list` - _Type_ column included if output contains both boardgames and expansions.
+- `meeple list` - _Type_ column included if output contains both board games and expansions.
 - `TESTS` - Increase test coverage.
 - `CI` - Report test coverage to [Codecov](https://codecov.io).
 - `CI` - Speed up test github action with `pre-commit` caching.
 
 ## [v0.1.0b5] - 2023-04-10
 
 ### Added
```

### Comparing `meeple-cli-0.1.0b8/justfile` & `meeple_cli-0.1.0rc1/justfile`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # activate venv
 venv:
     . .venv/bin/activate
 
 # install meeple-cli from local
 install:
     pip install -q ."[test]"
```

### Comparing `meeple-cli-0.1.0b8/pyproject.toml` & `meeple_cli-0.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/__init__.py` & `meeple_cli-0.1.0rc1/src/meeple/command/__init__.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/add.py` & `meeple_cli-0.1.0rc1/src/meeple/command/drop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,59 @@
-import sys
-
 import click
 
 from meeple.util.api_util import get_bgg_item
 from meeple.util.collection_util import (
     is_collection,
     read_collection,
     update_collection,
 )
 from meeple.util.completion_util import complete_collections
-from meeple.util.output_util import print_error, print_info
+from meeple.util.message_util import (
+    error_msg,
+    info_msg,
+    invalid_collection_error,
+    invalid_id_error,
+)
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.argument("id", type=int)
 @click.help_option("-h", "--help")
-def add(collection: str, id: int) -> None:
-    """Add an item to a collection.
+def drop(collection: str, id: int) -> None:
+    """Remove an item from a collection.
 
-    - COLLECTION is the name of the intended destination collection.
+    - COLLECTION is the name of the collection to be modified.
 
-    - ID is the BoardGameGeek ID of the board game/expansion to be added.
+    - ID is the BoardGameGeek ID of the board game/expansion to be removed.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(
-            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
-        )
+        invalid_id_error(bgg_id)
 
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(
-            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
-        )
+        invalid_collection_error(collection)
 
+    # get collection item ids
     item_ids, to_add_ids, to_drop_ids = read_collection(collection)
 
-    # check if the given id already exists in the given collection
-    if (item_ids and bgg_id in item_ids) or (to_add_ids and bgg_id in to_add_ids):
-        sys.exit(
-            print_error(
-                f"[i blue]{bgg_item.name}[/i blue] already exists in collection [u magenta]{collection}[/u magenta]."
-            )
-        )
-
-    if to_drop_ids and bgg_id in to_drop_ids:
-        # if the given id is slated to be dropped, simply undo that
-        to_drop_ids.remove(bgg_id)
-        item_ids.append(bgg_id)
-        item_ids.sort()
+    # if the given id is slated to be added, simply undo that
+    if to_add_ids and bgg_id in to_add_ids:
+        to_add_ids.remove(bgg_id)
+    # if the given id exists in the collection, drop the id
+    elif item_ids and bgg_id in item_ids:
+        item_ids.remove(bgg_id)
+        to_drop_ids.append(bgg_id)
+        to_drop_ids.sort()
     else:
-        # otherwise, add the id to the collection as normal
-        to_add_ids.append(bgg_id)
-        to_add_ids.sort()
+        error_msg(
+            f"[i blue]{bgg_item.name}[/i blue] already doesn't exist in collection [u magenta]{collection}[/u magenta]."
+        )
 
     # persist changes
     update_collection(collection, item_ids, to_add_ids, to_drop_ids)
-    print_info(
-        f"Added [i blue]{bgg_item.name}[/i blue]' to [u]{collection}[/u]. To update, run: [green]meeple update[/green]"
+    info_msg(
+        f"Dropped [i blue]{bgg_item.name}[/i blue] from collection [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update[/green]"
     )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/collections.py` & `meeple_cli-0.1.0rc1/src/meeple/command/collections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-import sys
-
 import click
 
 from meeple.type.collection import Collection
 from meeple.util.collection_util import get_collections, is_pending_updates
 from meeple.util.data_util import get_collection_data, last_updated
-from meeple.util.output_util import (
-    CollectionHeader,
-    fmt_collection_name,
-    fmt_headers,
-    print_error,
-    print_table,
-    print_warning,
-)
+from meeple.util.fmt_util import fmt_collection_name, fmt_headers
+from meeple.util.message_util import no_collections_exist_error, warn_msg
 from meeple.util.sort_util import COLLECTION_SORT_KEYS, sort_collections
+from meeple.util.table_util import CollectionHeader, print_table
 
 
 @click.command()
 @click.option(
     "--sort",
     type=click.Choice(COLLECTION_SORT_KEYS, case_sensitive=False),
     default="updated",
@@ -29,26 +22,22 @@
 def collections(sort: str, verbose: bool) -> None:
     """List all collections."""
     # attempt to retrieve collections
     collections = get_collections()
 
     # check that local collections exist
     if not collections:
-        sys.exit(
-            print_error(
-                "No local collections yet exist. To create one, run: [green]meeple new[/green]"
-            )
-        )
+        no_collections_exist_error()
 
     collection_list = []
     pending_changes = False
     for collection in collections:
-        boardgames, expansions = get_collection_data(collection)
+        board_games, expansions = get_collection_data(collection)
         collection_list.append(
-            Collection(collection, boardgames, expansions, last_updated(collection))
+            Collection(collection, board_games, expansions, last_updated(collection))
         )
         if is_pending_updates(collection):
             pending_changes = True
 
     # sort output
     collection_list, sort_direction = sort_collections(collection_list, sort)
 
@@ -69,22 +58,22 @@
     rows = []
     for collection in collection_list:
         cols = [fmt_collection_name(collection.name)]
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
-                    str(len(collection.boardgames)),
+                    str(len(collection.board_games)),
                     str(len(collection.expansions)),
                     collection.last_updated,
                 ]
             )
 
         rows.append(cols)
 
     # print warning if some collections need to be updated
     if pending_changes:
-        print_warning(
+        warn_msg(
             "Some collections ([red]*[/red]) are pending changes. To apply, run [green]meeple update[/green]"
         )
 
     print_table(rows, headers)
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/completions.py` & `meeple_cli-0.1.0rc1/src/meeple/command/completions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import click
 
-from meeple.util.output_util import print_info
+from meeple.util.message_util import info_msg
 
 SHELLS = ["bash", "zsh", "fish"]
 
 
 @click.command()
 @click.argument("shell", type=click.Choice(SHELLS, case_sensitive=False))
 @click.help_option("-h", "--help")
 def completions(shell: str) -> None:
     """Setup meeple shell completions.
 
     - SHELL is the shell for which to setup completions.
     """
     match shell.lower():
         case "bash":
-            print_info(
+            info_msg(
                 'To install completions, add this to ~/.bashrc: [green]eval "$(_MEEPLE_COMPLETE=bash_source meeple)"[/green]'
             )
         case "zsh":
-            print_info(
+            info_msg(
                 'To install completions, add this to ~/.zshrc: [green]eval "$(_MEEPLE_COMPLETE=zsh_source meeple)"[/green]'
             )
         case "fish":
-            print_info(
+            info_msg(
                 "To install completions, run: [green]_MEEPLE_COMPLETE=fish_source meeple > ~/.config/fish/completions/meeple.fish[/green]"
             )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/delete.py` & `meeple_cli-0.1.0rc1/src/meeple/command/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-import sys
-
 import click
 
 from meeple.util.collection_util import delete_collection, is_collection
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import delete_collection_data, get_collection_data
 from meeple.util.input_util import bool_input
-from meeple.util.output_util import print_error, print_info
+from meeple.util.message_util import info_msg, invalid_collection_error
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.option("-y", "--yes", is_flag=True, help="Dangerous - Bypass confirmation.")
 @click.help_option("-h", "--help")
 def delete(collection: str, yes: bool) -> None:
     """Delete a collection.
 
     - COLLECTION is the name of the collection to be deleted.
     """
     # check that the given collection exists
     if not is_collection(collection):
-        sys.exit(
-            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
-        )
+        invalid_collection_error(collection)
 
     # ask for confirmation or not depending on presence of flag
     if not yes:
         confirmation = bool_input(
             f"Are you sure you want to delete collection [u magenta]{collection}[/u magenta]?"
         )
     else:
         confirmation = True
 
     # delete collection and its data if confirmation succeeded
     if confirmation:
         delete_collection(collection)
-        boardgames, expansions = get_collection_data(collection)
-        if boardgames or expansions:
+        board_games, expansions = get_collection_data(collection)
+        if board_games or expansions:
             delete_collection_data(collection)
-        print_info(f"Deleted collection [u magenta]{collection}[/u magenta].")
+        info_msg(f"Deleted collection [u magenta]{collection}[/u magenta].")
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/drop.py` & `meeple_cli-0.1.0rc1/src/meeple/command/add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,60 @@
-import sys
-
 import click
 
 from meeple.util.api_util import get_bgg_item
 from meeple.util.collection_util import (
     is_collection,
     read_collection,
     update_collection,
 )
 from meeple.util.completion_util import complete_collections
-from meeple.util.output_util import print_error, print_info
+from meeple.util.message_util import (
+    error_msg,
+    info_msg,
+    invalid_collection_error,
+    invalid_id_error,
+)
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.argument("id", type=int)
 @click.help_option("-h", "--help")
-def drop(collection: str, id: int) -> None:
-    """Remove an item from a collection.
+def add(collection: str, id: int) -> None:
+    """Add an item to a collection.
 
-    - COLLECTION is the name of the collection to be modified.
+    - COLLECTION is the name of the intended destination collection.
 
-    - ID is the BoardGameGeek ID of the board game/expansion to be removed.
+    - ID is the BoardGameGeek ID of the board game/expansion to be added.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(
-            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
-        )
+        invalid_id_error(bgg_id)
 
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(
-            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
-        )
+        invalid_collection_error(collection)
 
+    # get collection item ids
     item_ids, to_add_ids, to_drop_ids = read_collection(collection)
 
-    # check if the given id already does not exist in the given collection
-    if (not item_ids or bgg_id not in item_ids) and (
-        not to_add_ids and bgg_id not in to_add_ids
-    ):
-        sys.exit(
-            print_error(
-                f"[i blue]{bgg_item.name}[/i blue] already doesn't exist in [u magenta]{collection}[/u magenta]."
-            )
-        )
-
-    if to_add_ids and bgg_id in to_add_ids:
-        # if the given id is slated to be added, simply undo that
-        to_add_ids.remove(bgg_id)
+    # if the given id is slated to be dropped, simply undo that
+    if to_drop_ids and bgg_id in to_drop_ids:
+        to_drop_ids.remove(bgg_id)
+        item_ids.append(bgg_id)
+        item_ids.sort()
+    # if the given id does not exist in the collection, add the id
+    elif bgg_id not in item_ids:
+        to_add_ids.append(bgg_id)
+        to_add_ids.sort()
     else:
-        # drop the id from the collection as normal
-        item_ids.remove(bgg_id)
-        to_drop_ids.append(bgg_id)
-        to_drop_ids.sort()
+        error_msg(
+            f"[i blue]{bgg_item.name}[/i blue] already exists in collection [u magenta]{collection}[/u magenta]."
+        )
 
     # persist changes
     update_collection(collection, item_ids, to_add_ids, to_drop_ids)
-    print_info(
-        f"Dropped [i blue]{bgg_item.name}[/i blue] from [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update[/green]"
+    info_msg(
+        f"Added [i blue]{bgg_item.name}[/i blue] to collection [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update[/green]"
     )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/find.py` & `meeple_cli-0.1.0rc1/src/meeple/command/find.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import sys
-
 import click
 
 from meeple.type.collection import Collection
 from meeple.util.collection_util import are_collections, get_collections
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
 from meeple.util.filter_util import filterby_players, filterby_playtime, filterby_weight
-from meeple.util.output_util import (
-    ItemHeader,
+from meeple.util.fmt_util import (
     fmt_headers,
+    fmt_item_type,
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
-    fmt_type,
     fmt_weight,
     fmt_year,
-    print_error,
-    print_table,
-    print_warning,
 )
+from meeple.util.message_util import error_msg, no_collections_exist_error
 from meeple.util.sort_util import ITEM_SORT_KEYS, sort_items
+from meeple.util.table_util import ItemHeader, print_table
 
 
 @click.command()
 @click.argument("collections", nargs=-1, shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
@@ -77,60 +73,54 @@
 ) -> None:
     """Search collections for items.
 
     - COLLECTIONS are the names of a collections to query. [default: all]
     """
     # check if provided collections exist
     if not are_collections(collections):
-        sys.exit(print_error("Not all provided collections are valid collections."))
+        error_msg("Not all provided collections are valid collections.")
 
     # if no collections provided, default to all local collections
     if not collections:
         collections = get_collections()
 
     # check that local collections exist
     if not collections:
-        sys.exit(
-            print_error(
-                "No local collections yet exist. To create one, run: [green]meeple new[/green]"
-            )
-        )
+        no_collections_exist_error()
 
     # get collection items
     result_items = []
     collection_list = []
     for collection in collections:
-        boardgames, expansions = get_collection_data(collection)
-        collection_list.append(Collection(collection, boardgames, expansions, None))
+        board_games, expansions = get_collection_data(collection)
+        collection_list.append(Collection(collection, board_games, expansions, None))
 
         # determine what to include in results depending on given flags
         if item_type == "bg":
-            result_items.extend(boardgames)
+            result_items.extend(board_games)
         elif item_type == "ex":
             result_items.extend(expansions)
         else:
-            result_items.extend(boardgames + expansions)
+            result_items.extend(board_games + expansions)
 
     # remove duplicates
     result_items = list(set(result_items))
 
     # apply provided filters
     if players:
         result_items = filterby_players(result_items, players)
     if max_time:
         result_items = filterby_playtime(result_items, max_time)
     if weight:
         result_items = filterby_weight(result_items, weight)
 
     # check that data exists after applied filters
     if not result_items:
-        sys.exit(
-            print_warning(
-                f"No items found matching provided filters for collection(s) [u magenta]{collections}[/u magenta]."
-            )
+        error_msg(
+            f"No items found matching provided filters for collection(s) [u magenta]{collections}[/u magenta]."
         )
 
     # sort output
     result_items, sort_direction = sort_items(result_items, sort)
 
     # prepare table headers
     headers = [ItemHeader.ID, ItemHeader.NAME]
@@ -158,23 +148,23 @@
 
     # prepare table data
     rows = []
     for item in result_items:
         cols = [str(item.id), item.name]
         # include type data if neither type is ommitted
         if item_type not in ("bg", "ex"):
-            cols.append(fmt_type(item.type))
+            cols.append(fmt_item_type(item.type))
         # include collections data if more than one collection was included
         if len(collections) > 1:
             # determine which collections the item exists in
             containing_collections = set(
                 [
                     collection.name
                     for collection in collection_list
-                    if item in collection.boardgames or item in collection.expansions
+                    if item in collection.board_games or item in collection.expansions
                 ]
             )
             cols.append(", ".join(containing_collections))
         # include additional data if verbose flag present
         if verbose:
             cols.extend(
                 [
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/hot.py` & `meeple_cli-0.1.0rc1/src/meeple/command/hot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 
 from meeple.util.api_util import get_bgg_hot
-from meeple.util.output_util import ItemHeader, fmt_headers, print_table
+from meeple.util.fmt_util import fmt_headers
+from meeple.util.table_util import ItemHeader, print_table
 
 
 @click.command()
 @click.help_option("-h", "--help")
 def hot() -> None:
     """List current BoardGameGeek trending items."""
     # retrieve hotness data from BoardGameGeek
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/info.py` & `meeple_cli-0.1.0rc1/src/meeple/command/info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import sys
-
 import click
 
 from meeple.util.api_util import get_bgg_item
-from meeple.util.output_util import (
+from meeple.util.fmt_util import (
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
     fmt_weight,
     fmt_year,
-    print_error,
-    print_table,
 )
+from meeple.util.message_util import invalid_id_error
+from meeple.util.table_util import print_table
 
 
 @click.command()
 @click.argument("id", type=int)
 @click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
 def info(id: int, verbose: bool) -> None:
@@ -24,32 +22,39 @@
 
     - ID is the BoardGameGeek ID of the board game/expansion to be detailed.
     """
     # check that the given id is a valid one
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(
-            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
-        )
+        invalid_id_error(bgg_id)
 
     info_rows = [
         [
             f"Rating: {fmt_rating(bgg_item.rating)}",
             f"Players: {fmt_players(bgg_item.minplayers, bgg_item.maxplayers)}",
             f"Min Age: {bgg_item.minage}",
         ],
         [
             f"Rank: {fmt_rank(bgg_item.rank)}",
             f"Play Time: {fmt_playtime(bgg_item.playtime)}",
             f"Weight: {fmt_weight(bgg_item.weight)}",
         ],
     ]
-    print_table([[f"{bgg_item.id}", f"{bgg_item.name} ({fmt_year(bgg_item.year)})"]])
-    print_table(info_rows, lines=True)
+
+    print_table(
+        [
+            [
+                f"{bgg_item.id}",
+                f"[i blue]{bgg_item.name}[/i blue] ({fmt_year(bgg_item.year)})",
+            ]
+        ]
+    )
+    print_table(info_rows, row_lines=True)
+
     # include additional data if verbose flag present
     if verbose:
         print_table(
             [
                 ["Description", bgg_item.description],
             ]
         )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/list.py` & `meeple_cli-0.1.0rc1/src/meeple/command/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-import sys
-
 import click
 
-from meeple.util.collection_util import is_collection
+from meeple.util.collection_util import is_collection, is_pending_updates
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
-from meeple.util.output_util import (
-    ItemHeader,
+from meeple.util.fmt_util import (
     fmt_headers,
+    fmt_item_type,
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
-    fmt_type,
     fmt_weight,
     fmt_year,
-    print_error,
-    print_table,
-    print_warning,
 )
+from meeple.util.message_util import error_msg, invalid_collection_error, warn_msg
 from meeple.util.sort_util import ITEM_SORT_KEYS, sort_items
+from meeple.util.table_util import ItemHeader, print_table
 
 
 @click.command(name="list")
 @click.argument("collection", shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
@@ -53,43 +49,42 @@
 def list_collection(collection: str, item_type: str, sort: str, verbose: bool) -> None:
     """List contents of a collection.
 
     - COLLECTION is the name of the collection to be listed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(
-            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
-        )
+        invalid_collection_error(collection)
 
-    boardgames, expansions = get_collection_data(collection)
+    board_games, expansions = get_collection_data(collection)
 
     # check that local data exists for the given collection
-    # TODO: add better error handling for when a collection has no data files and/or is empty?
-    if not boardgames and not expansions:
-        sys.exit(
-            print_error(
-                f"Local data not found for [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update {collection}[/green]"
-            )
+    if not board_games and not expansions:
+        error_msg(
+            f"Local data not found for [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update {collection}[/green]"
         )
 
     # determine what to include in results depending on given flags
     if item_type == "bg":
-        out_list = boardgames
+        out_list = board_games
     elif item_type == "ex":
         out_list = expansions
     else:
-        out_list = boardgames + expansions
+        out_list = board_games + expansions
 
     # check that data exists after applied filters
     if not out_list:
-        sys.exit(
-            print_warning(
-                f"No items found matching provided filters for collection [u magenta]{collection}[/u magenta]."
-            )
+        error_msg(
+            f"No items found matching provided filters for collection [u magenta]{collection}[/u magenta]."
+        )
+
+    # check if the collection is pending updates
+    if is_pending_updates(collection):
+        warn_msg(
+            f"Collection [u magenta]{collection}[/u magenta] has pending changes. To apply, run [green]meeple update {collection}[/green]"
         )
 
     # sort output
     out_list, sort_direction = sort_items(out_list, sort)
 
     # prepare table data
     headers = [ItemHeader.ID, ItemHeader.NAME]
@@ -112,15 +107,15 @@
     headers = fmt_headers(headers, sort, sort_direction)
 
     rows = []
     for item in out_list:
         cols = [str(item.id), item.name]
         # include type data if neither type is ommitted
         if item_type not in ("bg", "ex"):
-            cols.append(fmt_type(item.type))
+            cols.append(fmt_item_type(item.type))
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
                     fmt_year(item.year),
                     fmt_rank(str(item.rank)),
                     fmt_rating(item.rating),
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/move.py` & `meeple_cli-0.1.0rc1/src/meeple/command/move.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-import sys
-
 import click
 
 from meeple.util.api_util import get_bgg_item
 from meeple.util.collection_util import (
     is_collection,
     read_collection,
     update_collection,
 )
 from meeple.util.completion_util import complete_collections
-from meeple.util.output_util import print_error, print_info
+from meeple.util.message_util import (
+    error_msg,
+    info_msg,
+    invalid_collection_error,
+    invalid_id_error,
+)
 
 
 @click.command()
 @click.argument("from_collection", shell_complete=complete_collections)
 @click.argument("to_collection", shell_complete=complete_collections)
 @click.argument("id", type=int)
 @click.help_option("-h", "--help")
@@ -26,64 +29,61 @@
 
     - ID is the BoardGameGeek ID of the board game/expansion to be moved.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
     if not bgg_item:
-        sys.exit(
-            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
-        )
+        invalid_id_error(bgg_id)
 
-    # check that the given collection is a valid collection
+    # check that the given from collection is a valid collection
     if not is_collection(from_collection):
-        sys.exit(
-            print_error(
-                f"[yellow]{from_collection}[/yellow] is not a valid collection."
-            )
-        )
+        invalid_collection_error(from_collection)
 
+    # get from collection item ids
     from_item_ids, from_to_add_ids, from_to_drop_ids = read_collection(from_collection)
 
-    # check that the given collection is a valid collection
+    # check that the given to collection is a valid collection
     if not is_collection(to_collection):
-        # TODO: offer to create the new collection
-        sys.exit(
-            print_error(f"[yellow]{to_collection}[/yellow] is not a valid collection.")
-        )
+        # TODO: prompt to create the dest collection
+        invalid_collection_error(to_collection)
 
+    # get destination collection item ids
     dest_item_ids, dest_to_add_ids, dest_to_drop_ids = read_collection(to_collection)
 
-    # check that the id exists in from collection
-    # TODO: check the from collection to_add list and to_drop list
-    if bgg_id not in from_item_ids:
-        # TODO: ask if they want to add it to the destination collection anyway
-        sys.exit(
-            print_error(
-                f"[i blue]{bgg_item.name}[/i blue] already doesn't exist in [u magenta]{from_collection}[/u magenta]."
-            )
-        )
-
-    # check that the id doesn't exist in dest collection
-    # TODO: check the dest collection to_add list and to_drop list
-    if dest_item_ids and bgg_id in dest_item_ids:
-        sys.exit(
-            print_error(
-                f"[i blue]{bgg_item.name}[/i blue] already exists in collection [u magenta]{to_collection}[/u magenta]."
-            )
-        )
-
     # drop the id from the from collection
-    from_item_ids.remove(bgg_id)
-    from_to_drop_ids.append(bgg_id)
-    from_to_drop_ids.sort()
+    # if the given id is slated to be added, simply undo that
+    if from_to_add_ids and bgg_id in from_to_add_ids:
+        from_to_add_ids.remove(bgg_id)
+    # if the given id exists in the collection, drop the id
+    elif from_item_ids and bgg_id in from_item_ids:
+        from_item_ids.remove(bgg_id)
+        from_to_drop_ids.append(bgg_id)
+        from_to_drop_ids.sort()
+    else:
+        # TODO: prompt to just add to the destination collection anyway
+        error_msg(
+            f"[i blue]{bgg_item.name}[/i blue] already doesn't exist in collection [u magenta]{from_collection}[/u magenta]."
+        )
 
     # add the id to the destination collection
-    dest_to_add_ids.append(bgg_id)
-    dest_to_add_ids.sort()
+    # if the given id is slated to be dropped, simply undo that
+    if dest_to_drop_ids and bgg_id in dest_to_drop_ids:
+        dest_to_drop_ids.remove(bgg_id)
+        dest_item_ids.append(bgg_id)
+        dest_item_ids.sort()
+    # if the given id does not exist in the collection, add the id
+    elif bgg_id not in dest_item_ids:
+        dest_to_add_ids.append(bgg_id)
+        dest_to_add_ids.sort()
+    else:
+        # TODO: prompt to just remove from the from collection anyway
+        error_msg(
+            f"[i blue]{bgg_item.name}[/i blue] already exists in collection [u magenta]{to_collection}[/u magenta]."
+        )
 
     # persist changes
     update_collection(from_collection, from_item_ids, from_to_add_ids, from_to_drop_ids)
     update_collection(to_collection, dest_item_ids, dest_to_add_ids, dest_to_drop_ids)
-    print_info(
-        f"Moved [i blue]{bgg_item.name}[/i blue] from [u magenta]{from_collection}[/u magenta] to [u magenta]{to_collection}[/u magenta]. To update, run: [green]meeple update[/green]"
+    info_msg(
+        f"Moved [i blue]{bgg_item.name}[/i blue] from collection [u magenta]{from_collection}[/u magenta] to collection [u magenta]{to_collection}[/u magenta]. To update, run: [green]meeple update[/green]"
     )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/new.py` & `meeple_cli-0.1.0rc1/src/meeple/command/new.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-import sys
-
 import click
 
 from meeple.util.collection_util import create_collection, is_collection
-from meeple.util.output_util import print_error, print_info
+from meeple.util.message_util import error_msg, info_msg
 
 
 @click.command()
 @click.argument("collection")
 @click.help_option("-h", "--help")
 def new(collection: str) -> None:
     """Create a new collection.
 
     - COLLECTION is the name of the collection to be created.
     """
     # check that the given collection doesn't already exist
     if is_collection(collection):
-        sys.exit(
-            print_error(
-                f"Collection [u magenta]{collection}[/u magenta] already exists."
-            )
-        )
+        error_msg(f"Collection [u magenta]{collection}[/u magenta] already exists.")
 
     # create new collection
     create_collection(collection)
-    print_info(f"Created new collection [u magenta]{collection}[/u magenta].")
+    info_msg(f"Created new collection [u magenta]{collection}[/u magenta].")
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/open.py` & `meeple_cli-0.1.0rc1/src/meeple/command/open.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import sys
 import webbrowser
 
 import click
 
 from meeple.util.api_util import BGG_DOMAIN, get_bgg_items
 from meeple.util.input_util import bool_input
-from meeple.util.output_util import print_error, print_info, printf
+from meeple.util.message_util import info_msg, invalid_id_error, print_msg
 
 
 @click.command(name="open")
 @click.argument("id", type=int)
 @click.option("-y", "--yes", is_flag=True, help="Bypass confirmation.")
 @click.help_option("-h", "--help")
 def open_on_bgg(id: int, yes: bool) -> None:
@@ -17,20 +16,18 @@
 
     - ID is the BoardGameGeek ID of the board game/expansion to be opened on boardgamegeek.com.
     """
     # check that the given id is a valid BoardGameGeek ID
     bgg_id = id
     api_result = get_bgg_items([bgg_id])
     if not api_result:
-        sys.exit(
-            print_error(f"[yellow]{bgg_id}[/yellow] is not a valid BoardGameGeek ID.")
-        )
+        invalid_id_error(bgg_id)
 
     # confirm the user wants to open the board game/expansion on BoardGameGeek website
     item = api_result[0]
     url = f"https://{BGG_DOMAIN}/{item.type}/{bgg_id}"
     name = item.name
     if yes or bool_input(f"Open [i blue]{name}[/i blue] on {BGG_DOMAIN}?"):
-        printf(f" ╰╴ Opening [i blue]{name}[/i blue] on {BGG_DOMAIN} ...")
+        print_msg(f" ╰╴ Opening [i blue]{name}[/i blue] on {BGG_DOMAIN} ...")
         webbrowser.open(url)
     else:
-        print_info(f"View [i blue]{name}[/i blue] at {url}")
+        info_msg(f"View [i blue]{name}[/i blue] at {url}")
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/rename.py` & `meeple_cli-0.1.0rc1/src/meeple/command/rename.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-import sys
-
 import click
 
 from meeple.util.collection_util import is_collection, rename_collection
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import rename_collection_data_dir
-from meeple.util.output_util import print_error, print_info
+from meeple.util.message_util import error_msg, info_msg, invalid_collection_error
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.argument("new_name")
 @click.help_option("-h", "--help")
 def rename(collection: str, new_name: str) -> None:
     """Rename a local collection.
 
     - COLLECTION is the name of the collection to be renamed.
     - NEW_NAME is the new name to assign to the collection.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(
-            print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
-        )
+        invalid_collection_error(collection)
 
     # check that the given collection new name doesn't already exist
     if is_collection(new_name):
-        sys.exit(
-            print_error(
-                f"Collection [u magenta]{collection}[/u magenta] already exists."
-            )
-        )
+        error_msg(f"Collection [u magenta]{collection}[/u magenta] already exists.")
 
     # create new collection
     rename_collection(collection, new_name)
     rename_collection_data_dir(collection, new_name)
-    print_info(
+    info_msg(
         f"Renamed collection [u magenta]{collection}[/u magenta] to [u magenta]{new_name}[/u magenta]."
     )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/search.py` & `meeple_cli-0.1.0rc1/src/meeple/command/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-import sys
-
 import click
 
 from meeple.util.api_util import search_bgg
-from meeple.util.output_util import (
-    ItemHeader,
-    fmt_headers,
-    fmt_year,
-    print_table,
-    print_warning,
-)
+from meeple.util.fmt_util import fmt_headers, fmt_year
+from meeple.util.message_util import error_msg
+from meeple.util.table_util import ItemHeader, print_table
 
 
 @click.command()
 @click.argument("query")
 @click.help_option("-h", "--help")
 def search(query: str) -> None:
     """Search BoardGameGeek for items.
@@ -21,18 +15,16 @@
     - QUERY is the text to be searched for on BoardGameGeek. If searching multiple words, surround with quotes.
     """
     # search BoardGameGeek with user provided query
     result_items = search_bgg(query)
 
     # check that data exists after applied filters
     if not result_items:
-        sys.exit(
-            print_warning(
-                f"No items found on BoardGameGeek matching search term [i blue]{query}[i blue]."
-            )
+        error_msg(
+            f"No items found on BoardGameGeek matching search term [i blue]{query}[/i blue]."
         )
 
     result_items.sort(key=lambda x: x.id)
 
     # prepare table data
     headers = [ItemHeader.ID, ItemHeader.NAME, ItemHeader.YEAR]
     headers = fmt_headers(headers, None, None)
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/stats.py` & `meeple_cli-0.1.0rc1/src/meeple/command/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-import sys
-
 import click
 
 from meeple.util.collection_util import is_collection, is_pending_updates
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import get_collection_data
-from meeple.util.output_util import (
-    fmt_avg_rank,
-    fmt_rating,
-    fmt_weight,
-    print_error,
-    print_table,
-    print_warning,
-)
+from meeple.util.fmt_util import fmt_avg_rank, fmt_rating, fmt_weight
+from meeple.util.message_util import error_msg, invalid_collection_error, warn_msg
+from meeple.util.table_util import print_table
 
 
 @click.command()
 @click.argument("collection", shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
@@ -37,39 +30,35 @@
 def stats(collection: str, item_type: str) -> None:
     """Print out the details of a collection.
 
     - COLLECTION is the name of the collection to be detailed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
-        sys.exit(print_error(f"'{collection}' is not a valid collection"))
+        invalid_collection_error(collection)
 
-    boardgames, expansions = get_collection_data(collection)
+    board_games, expansions = get_collection_data(collection)
     # check that data exists for the given collection
-    if not boardgames and not expansions:
-        sys.exit(
-            print_error(
-                f"Local data not found for [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update {collection}[/green]"
-            )
+    if not board_games and not expansions:
+        error_msg(
+            f"Local data not found for [u magenta]{collection}[/u magenta]. To update, run: [green]meeple update {collection}[/green]"
         )
 
     # determine what to include in results depending on given flags
     if item_type == "bg":
-        out_list = boardgames
+        out_list = board_games
     elif item_type == "ex":
         out_list = expansions
     else:
-        out_list = boardgames + expansions
+        out_list = board_games + expansions
 
     # check that data exists after applied filters
     if not out_list:
-        sys.exit(
-            print_warning(
-                f"No items found matching provided filters for collection [u magenta]{collection}[/u magenta]."
-            )
+        error_msg(
+            f"No items found matching provided filters for collection [u magenta]{collection}[/u magenta]."
         )
 
     # calculate stats
     sum_ratings = (
         num_rated
     ) = sum_rank = num_ranked = sum_weight = num_weighted = sum_players = 0
 
@@ -99,32 +88,28 @@
     if num_weighted > 0:
         avg_weight = round(sum_weight / num_weighted, 2)
     else:
         avg_weight = 0
     avg_max_players = round(sum_players / len(out_list), 2)
 
     # format output
+    num_bgs_tag = f"{len(board_games)} Board Game(s)"
+    num_exps_tag = f"{len(expansions)} Expansion(s)"
     if item_type == "bg":
-        header = [
-            f"[u magenta]{collection}[/u magenta]",
-            f"{len(boardgames)} Board Game(s)",
-        ]
+        header = [f"[u magenta]{collection}[/u magenta]", num_bgs_tag]
     elif item_type == "ex":
-        header = [
-            f"[u magenta]{collection}[/u magenta]",
-            f"{len(expansions)} Expansion(s)",
-        ]
+        header = [f"[u magenta]{collection}[/u magenta]", num_exps_tag]
     else:
         header = [
             f"[u magenta]{collection}[/u magenta]",
-            f"{len(boardgames)} Board Game(s) | {len(expansions)} Expansion(s)",
+            f"{num_bgs_tag} | {num_exps_tag}",
         ]
 
     if is_pending_updates(collection):
-        print_warning(
+        warn_msg(
             f"Collection [u magenta]{collection}[/u magenta] has pending changes. To apply, run [green]meeple update {collection}[/green]"
         )
 
     print_table([header])
     print_table(
         [
             [
@@ -132,9 +117,9 @@
                 f"Avg. Max Players: {avg_max_players}",
             ],
             [
                 f"Avg. Rank: {fmt_avg_rank(avg_rank)}",
                 f"Avg. Weight: {fmt_weight(avg_weight)}",
             ],
         ],
-        lines=True,
+        row_lines=True,
     )
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/command/update.py` & `meeple_cli-0.1.0rc1/src/meeple/command/update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,75 @@
-import sys
 from datetime import date
 
 import click
 
 from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE, get_bgg_items
 from meeple.util.collection_util import (
     get_collections,
     is_collection,
     is_pending_updates,
     read_collection,
     update_collection,
 )
 from meeple.util.completion_util import complete_collections
 from meeple.util.data_util import last_updated, write_collection_data
-from meeple.util.output_util import print_error, print_info, printf
+from meeple.util.message_util import (
+    info_msg,
+    invalid_collection_error,
+    no_collections_exist_error,
+    print_msg,
+)
 from meeple.util.sort_util import sort_items
 
 
 @click.command()
 @click.argument("collection", required=False, shell_complete=complete_collections)
 @click.option("-f", "--force", is_flag=True, help="Force update.")
 @click.help_option("-h", "--help")
 def update(collection: str, force: bool) -> None:
     """Update local collection data.
 
     - COLLECTION (optional) is the name of the collection to be updated. If not provided, update all collections.
     """
-    print_info("Updating local collection data...")
-    # update only a specific collection, if given
+    info_msg("Updating collection data...")
+
+    # update only a specific collection, if given. otherwise, attempt to udpate all
     if collection:
         # check that the given collection is a valid collection
         if not is_collection(collection):
-            sys.exit(
-                print_error(f"[yellow]{collection}[/yellow] is not a valid collection.")
-            )
+            invalid_collection_error(collection)
         collections = [collection]
     else:
         collections = get_collections()
 
     # check that local collections exist
     if not collections:
-        sys.exit(
-            print_error(
-                "No local collections yet exist. To create one, run: [green]meeple new[/green]"
-            )
-        )
+        no_collections_exist_error()
 
     # update collection data
     for collection in collections:
-        # read board game ids from src file
+        # get collection item ids
         item_ids, to_add_ids, to_drop_ids = read_collection(collection)
+
+        # print warning and skip if collection is empty
         if not item_ids and not to_add_ids and not to_drop_ids:
-            printf(
+            print_msg(
                 f" ╰╴ [yellow]Warning[/yellow]: Could not update collection [u magenta]{collection}[/u magenta] because it is empty. To add to it, run: [green]meeple add[/green]"
             )
             continue
 
         # skip if collection not pending updates, has been updated today, and force flag not provided
         updated = last_updated(collection)
         if (
             not force
             and not is_pending_updates(collection)
             and updated == str(date.today())
         ):
-            printf(
-                f" ╰╴ Skipped collection [u magenta]{collection}[/u magenta]. Already up to date."
+            print_msg(
+                f" ╰╴ [dim]Skipped collection [u magenta]{collection}[/u magenta]. Already up to date.[/dim]"
             )
             continue
 
         # resolve pending updates, if any
         if to_add_ids:
             item_ids.extend(to_add_ids)
             item_ids.sort()
@@ -76,31 +77,26 @@
         if to_drop_ids:
             # nothing to resolve, just dump the pending update indicator
             to_drop_ids = []
         update_collection(collection, item_ids, to_add_ids, to_drop_ids)
 
         # get items from BoardGameGeek
         api_result = get_bgg_items(item_ids)
-        boardgames = []
-        expansions = []
+        board_games, expansions = [], []
         for item in api_result:
             item_type = item.type
             if item_type == BOARDGAME_TYPE:
-                boardgames.append(item)
+                board_games.append(item)
             if item_type == EXPANSION_TYPE:
                 expansions.append(item)
 
         # sort board games by rank and expansions by rating
-        if boardgames:
-            boardgames, _ = sort_items(boardgames, "rank")
+        if board_games:
+            board_games, _ = sort_items(board_games, "rank")
         if expansions:
             expansions, _ = sort_items(expansions, "rating")
 
-        # save results
-        update_result = {
-            "boardgames": [boardgame.__dict__ for boardgame in boardgames],
-            "expansions": [expansion.__dict__ for expansion in expansions],
-        }
-        write_collection_data(collection, update_result)
-        printf(f" ╰╴ Updated collection [u magenta]{collection}[/u magenta].")
+        # persist results
+        write_collection_data(collection, board_games, expansions)
+        print_msg(f" ╰╴ Updated collection [u magenta]{collection}[/u magenta].")
 
-    print_info("Updated local collection data.")
+    info_msg("Updated collection data.")
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/root.py` & `meeple_cli-0.1.0rc1/src/meeple/root.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/src/meeple/type/item.py` & `meeple_cli-0.1.0rc1/src/meeple/type/item.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/api_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/api_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     response = requests.get(url)
     if response.status_code == 200:
         resp_dict = xmltodict.parse(response.content)
         resp_list = resp_dict["items"].get("item", [])
         if not isinstance(resp_list, list):
             resp_list = [resp_list]
         return [Item.from_bgg_dict(bgg_dict) for bgg_dict in resp_list]
-    # TODO: provide better error handling and logging for bad requests
+    # TODO: provide better error handling and logging for bad requests/responses
     sys.exit(f"Error: HTTP {response.status_code}: {response.content}")
 
 
 def get_bgg_items(bgg_ids: List[int]) -> List[Item]:
     ids_str = ",".join(map(str, bgg_ids))
     url = f"{API2_BASE_URL}/thing?id={ids_str}&type={BOARDGAME_TYPE},{EXPANSION_TYPE}&stats=1"
     return _bgg_api_get_items(url)
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/cmd_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/cmd_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 
-import click
+from click import Group
 
 
-class SectionedHelpGroup(click.Group):
+class SectionedHelpGroup(Group):
     """Organize commands as sections"""
 
     def __init__(self, *args, **kwargs):
         self.section_commands = collections.defaultdict(list)
         super().__init__(*args, **kwargs)
 
     def add_command(self, cmd, name=None, section=None):
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/collection_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/collection_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import yaml
 
 from meeple.util.fs_util import get_collection_dir
 
 COLLECTION_DIR = get_collection_dir()
 
 _ITEM_LIST_KEY = "items"
-_OLD_ITEM_LIST_KEY = "bgg-ids"  # TODO: eventually remove
+_OLD_ITEM_LIST_KEY = "bgg-ids"  # TODO: deprecated - eventually remove
 _TO_ADD_LIST_KEY = "to_add"
 _TO_DROP_LIST_KEY = "to_drop"
 
 
 def _collection_file(collection_name: str) -> str:
     return join(COLLECTION_DIR, f"{collection_name}.yml")
 
@@ -60,15 +60,15 @@
 
 
 def read_collection(name: str) -> (List[int], List[int], List[int]):
     with open(_collection_file(name), "r") as f:
         data = yaml.load(f, Loader=yaml.FullLoader)
 
         # check if data is in old format
-        # TODO: eventually remove
+        # TODO: deprecated - eventually remove
         if data and _OLD_ITEM_LIST_KEY in data:
             bgg_ids = data[_OLD_ITEM_LIST_KEY]
             if not bgg_ids:
                 return [], [], []
 
             # remove non int values from list
             for bgg_id in bgg_ids:
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/data_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/data_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import List
 
 from meeple.type.item import Item
 from meeple.util.fs_util import get_data_dir
 
 DATA_DIR = get_data_dir()
 
+_BOARD_GAME_LIST_KEY = "boardgames"
+_EXPANSION_LIST_KEY = "expansions"
+
 
 def _collection_data_dir(collection_name: str) -> str:
     return join(DATA_DIR, collection_name)
 
 
 def _latest_data_file(collection_name: str) -> str:
     # find latest data dump file path for collection
@@ -33,46 +36,55 @@
     if Path(_collection_data_dir(current_name)).exists():
         rename(_collection_data_dir(current_name), join(DATA_DIR, new_name))
 
 
 def last_updated(collection_name: str) -> str:
     latest_data_file = _latest_data_file(collection_name)
     if not latest_data_file:
-        return "NA"
+        return "[dim]NA[/dim]"
     date = splitext(basename(latest_data_file))[0]
     return date
 
 
 def get_collection_data(collection_name: str) -> (List[Item], List[Item]):
     data_path = _latest_data_file(collection_name)
-    boardgames = []
-    expansions = []
+    board_games, expansions = [], []
     if not data_path:
-        return boardgames, expansions
+        return board_games, expansions
 
+    # get latest collection data
     with open(data_path, "r") as f:
         data = json.load(f)
 
-    for dict_item in data["boardgames"]:
-        item = json.loads(json.dumps(dict_item), object_hook=Item.from_json)
-        boardgames.append(item)
-    for dict_item in data["expansions"]:
-        item = json.loads(json.dumps(dict_item), object_hook=Item.from_json)
-        expansions.append(item)
-    return boardgames, expansions
+    for dict_item in data[_BOARD_GAME_LIST_KEY]:
+        board_games.append(
+            json.loads(json.dumps(dict_item), object_hook=Item.from_json)
+        )
+    for dict_item in data[_EXPANSION_LIST_KEY]:
+        expansions.append(json.loads(json.dumps(dict_item), object_hook=Item.from_json))
+    return board_games, expansions
 
 
-def write_collection_data(collection_name: str, result: dict) -> None:
+def write_collection_data(
+    collection_name: str, board_games: List[Item], expansions: List[Item]
+) -> None:
     today = date.today()
     data_path = f"{_collection_data_dir(collection_name)}/{today.strftime('%Y-%m')}"
     filename = f"{today}.json"
 
     # create out dirs if they do not exist
     if not Path(data_path).exists():
         Path(data_path).mkdir(parents=True)
 
+    # build data dictionary
+    data_dict = {
+        _BOARD_GAME_LIST_KEY: [board_game.__dict__ for board_game in board_games],
+        _EXPANSION_LIST_KEY: [expansion.__dict__ for expansion in expansions],
+    }
+
+    # persist data
     with open(join(data_path, filename), "w") as f:
-        json.dump(result, f, indent=4, ensure_ascii=False)
+        json.dump(data_dict, f, indent=4, ensure_ascii=False)
 
 
 def delete_collection_data(collection_name: str) -> None:
     shutil.rmtree(_collection_data_dir(collection_name))
```

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/filter_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/filter_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/fs_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/fs_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/src/meeple/util/sort_util.py` & `meeple_cli-0.1.0rc1/src/meeple/util/sort_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from meeple.type.collection import Collection
 from meeple.type.item import Item
-from meeple.util.output_util import SORT_ASC_SYMBOL, SORT_DESC_SYMBOL
+from meeple.util.fmt_util import SORT_ASC_SYMBOL, SORT_DESC_SYMBOL
 
 COLLECTION_SORT_KEYS = ["name", "boardgames", "expansions", "updated"]
 ITEM_SORT_KEYS = ["rank", "rating", "weight", "year", "name", "id", "time"]
 
 
 def _handle_str_rank(item: Item):
     try:
@@ -20,15 +20,15 @@
                 sorted(collection_list, key=lambda collection: collection.name),
                 SORT_ASC_SYMBOL,
             )
         case "boardgames":
             return (
                 sorted(
                     collection_list,
-                    key=lambda collection: len(collection.boardgames),
+                    key=lambda collection: len(collection.board_games),
                     reverse=True,
                 ),
                 SORT_DESC_SYMBOL,
             )
         case "expansions":
             return (
                 sorted(
```

### Comparing `meeple-cli-0.1.0b8/tests/util/test_filter_util.py` & `meeple_cli-0.1.0rc1/tests/util/test_filter_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/tests/util/test_fs_util.py` & `meeple_cli-0.1.0rc1/tests/util/test_fs_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/tests/util/test_output_util.py` & `meeple_cli-0.1.0rc1/tests/util/test_fmt_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from meeple.util.api_util import BOARDGAME_TYPE, EXPANSION_TYPE
-from meeple.util.output_util import (
+from meeple.util.fmt_util import (
     NA_VALUE,
     fmt_avg_rank,
+    fmt_item_type,
     fmt_players,
     fmt_playtime,
     fmt_rank,
     fmt_rating,
-    fmt_type,
     fmt_weight,
     fmt_year,
 )
 
 
 def test_fmt_players():
     na_output = fmt_players(0, 0)
@@ -63,22 +63,22 @@
     purple_output = fmt_rating(6.5)
     assert purple_output == "[magenta]6.50[/magenta]"
 
     red_output = fmt_rating(5.5)
     assert red_output == "[red]5.50[/red]"
 
 
-def test_fmt_type():
-    na_output = fmt_type("other")
+def test_fmt_item_type():
+    na_output = fmt_item_type("other")
     assert na_output == NA_VALUE
 
-    bg_output = fmt_type(BOARDGAME_TYPE)
+    bg_output = fmt_item_type(BOARDGAME_TYPE)
     assert bg_output == "Board Game"
 
-    ex_output = fmt_type(EXPANSION_TYPE)
+    ex_output = fmt_item_type(EXPANSION_TYPE)
     assert ex_output == "Expansion"
 
 
 def test_fmt_weight():
     na_output = fmt_weight(0)
     assert na_output == NA_VALUE
```

### Comparing `meeple-cli-0.1.0b8/tests/util/test_sort_util.py` & `meeple_cli-0.1.0rc1/tests/util/test_sort_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b8/PKG-INFO` & `meeple_cli-0.1.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeple-cli
-Version: 0.1.0b8
+Version: 0.1.0rc1
 Summary: Local board game collection manager. Powered by BoardGameGeek.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >=8
 Requires-Dist: rich >=13
@@ -160,14 +160,26 @@
 [BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
 provides limited _read-only_ data about user collections/GeekLists.
 
 While it is _technically_ feasible to interface with GeekLists via
 webscrapers/spiders, this kind of practice would be both complex and also
 violate [BoardGameGeek Terms of Service](https://boardgamegeek.com/terms#toc22).
 
+### Why do some items show a weight of `NA` when boardgamegeek.com has a value?
+
+This is a known and occasionally recurring bug in the BoardGameGeek database. It
+usually resolves itself within a day. For more info or additional support, read
+this [thread](https://boardgamegeek.com/thread/3049286/some-games-show-weight-000).
+
+Luckily for us, game weights do not often change drastically. In most cases, we
+can assume that the weight from yesterday is _close enough_.
+[In the future](https://github.com/boldandbrad/meeple-cli/issues/61),
+`meeple-cli` will account for this automatically and display the last known
+value by default, if there is one.
+
 ### Where does `meeple-cli` store data?
 
 `meeple-cli` stores collection data in `~/.meeple` and only makes network
 connections to retrieve data from the BoardGameGeek API.
 
 ## License
```

