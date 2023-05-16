# Comparing `tmp/gpt_review-0.9.0rc741.post1.tar.gz` & `tmp/gpt_review-0.9.1rc762.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_review-0.9.0rc741.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gpt_review-0.9.1rc762.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpt_review-0.9.0rc741.post1.tar` & `gpt_review-0.9.1rc762.post1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      336 2023-05-15 23:36:53.634359 gpt_review-0.9.0rc741.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-15 23:36:53.634359 gpt_review-0.9.0rc741.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-15 23:36:53.634359 gpt_review-0.9.0rc741.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-15 23:36:53.634359 gpt_review-0.9.0rc741.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-15 23:36:53.634359 gpt_review-0.9.0rc741.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-15 23:36:53.634359 gpt_review-0.9.0rc741.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4200 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1649 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1862 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/LICENSE
--rw-r--r--   0        0        0     3556 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/README.md
--rw-r--r--   0        0        0     2308 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/action.yml
--rw-r--r--   0        0        0      307 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/azure.yaml.template
--rw-r--r--   0        0        0      218 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/config.summary.template.yml
--rw-r--r--   0        0        0      362 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/prompt.template.yml
--rw-r--r--   0        0        0     8500 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-15 23:36:59.450442 gpt_review-0.9.0rc741.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      170 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-15 23:36:59.450442 gpt_review-0.9.0rc741.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      170 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     9453 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3520 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5998 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     6437 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3672 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8558 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      955 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0     3053 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/context.py
--rw-r--r--   0        0        0      924 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      349 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/prompts/prompt_bug.yaml
--rw-r--r--   0        0        0      362 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/prompts/prompt_coverage.yaml
--rw-r--r--   0        0        0      327 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/prompts/prompt_summary.yaml
--rw-r--r--   0        0        0      863 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/src/gpt_review/utils.py
--rw-r--r--   0        0        0      218 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5523 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/mock.diff
--rw-r--r--   0        0        0      375 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_context.py
--rw-r--r--   0        0        0      716 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_github.py
--rw-r--r--   0        0        0     5427 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1449 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-15 23:36:53.638359 gpt_review-0.9.0rc741.post1/tests/test_review.py
--rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 gpt_review-0.9.0rc741.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4200 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1649 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1862 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/LICENSE
+-rw-r--r--   0        0        0     3556 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/README.md
+-rw-r--r--   0        0        0     2308 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/action.yml
+-rw-r--r--   0        0        0      307 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/azure.yaml.template
+-rw-r--r--   0        0        0      218 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/config.summary.template.yml
+-rw-r--r--   0        0        0      362 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/prompt.template.yml
+-rw-r--r--   0        0        0     8500 2023-05-16 04:19:02.189932 gpt_review-0.9.1rc762.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-16 04:19:11.725882 gpt_review-0.9.1rc762.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-16 04:19:11.725882 gpt_review-0.9.1rc762.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     9453 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3520 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5998 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     6437 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     4241 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8558 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      955 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0     3227 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/context.py
+-rw-r--r--   0        0        0      924 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      349 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/prompts/prompt_bug.yaml
+-rw-r--r--   0        0        0      362 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/prompts/prompt_coverage.yaml
+-rw-r--r--   0        0        0      327 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/prompts/prompt_summary.yaml
+-rw-r--r--   0        0        0      863 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/src/gpt_review/utils.py
+-rw-r--r--   0        0        0      218 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5573 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/mock.diff
+-rw-r--r--   0        0        0      375 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_context.py
+-rw-r--r--   0        0        0      716 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5427 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1449 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-16 04:19:02.193933 gpt_review-0.9.1rc762.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 gpt_review-0.9.1rc762.post1/PKG-INFO
```

### Comparing `gpt_review-0.9.0rc741.post1/.devcontainer/devcontainer.json` & `gpt_review-0.9.1rc762.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt_review-0.9.1rc762.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/dependabot.yml` & `gpt_review-0.9.1rc762.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/pull_request_template.md` & `gpt_review-0.9.1rc762.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/workflows/codeql.yml` & `gpt_review-0.9.1rc762.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/workflows/dependency-review.yml` & `gpt_review-0.9.1rc762.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt_review-0.9.1rc762.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/workflows/python.yml` & `gpt_review-0.9.1rc762.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.github/workflows/test-action.yml` & `gpt_review-0.9.1rc762.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.gitignore` & `gpt_review-0.9.1rc762.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/.vscode/settings.json` & `gpt_review-0.9.1rc762.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/LICENSE` & `gpt_review-0.9.1rc762.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/README.md` & `gpt_review-0.9.1rc762.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/action.yml` & `gpt_review-0.9.1rc762.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/pyproject.toml` & `gpt_review-0.9.1rc762.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_ask.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_git.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_github.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_gpt_cli.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_llama_index.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_openai.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_openai.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Open AI API Call Wrapper."""
+import os
 import logging
 
 import openai
 from openai.error import RateLimitError
 
 import gpt_review.constants as C
 from gpt_review.utils import _retry_with_exponential_backoff
@@ -75,28 +76,42 @@
         fast (bool, optional): Whether to use the fast model. Defaults to False.
         large (bool, optional): Whether to use the large model. Defaults to False.
 
     Returns:
         str: The response from GPT.
     """
     messages = messages or [{"role": "user", "content": prompt}]
+    logging.debug("Prompt sent to GPT: %s\n", prompt)
+
     try:
         model = _get_model(prompt, max_tokens=max_tokens, fast=fast, large=large)
-        logging.info(f"Model Selected based on prompt size: {model}")
+        logging.debug(f"Model Selected based on prompt size: {model}")
 
-        logging.info("Prompt sent to GPT: %s\n", prompt)
-        completion = openai.ChatCompletion.create(
-            model=model,
-            messages=messages,
-            max_tokens=max_tokens,
-            temperature=temperature,
-            top_p=top_p,
-            frequency_penalty=frequency_penalty,
-            presence_penalty=presence_penalty,
-        )
+        if os.environ["OPENAI_API_TYPE"] == C.AZURE_API_TYPE:
+            logging.debug("Using Azure Open AI.")
+            completion = openai.ChatCompletion.create(
+                deployment_id=model,
+                messages=messages,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                top_p=top_p,
+                frequency_penalty=frequency_penalty,
+                presence_penalty=presence_penalty,
+            )
+        else:
+            logging.debug("Using Open AI.")
+            completion = openai.ChatCompletion.create(
+                model=model,
+                messages=messages,
+                max_tokens=max_tokens,
+                temperature=temperature,
+                top_p=top_p,
+                frequency_penalty=frequency_penalty,
+                presence_penalty=presence_penalty,
+            )
         return completion.choices[0].message.content  # type: ignore
     except RateLimitError as error:
         if retry < C.MAX_RETRIES:
             _retry_with_exponential_backoff(retry, error.headers["Retry-After"])
 
             return _call_gpt(prompt, temperature, max_tokens, top_p, frequency_penalty, presence_penalty, retry + 1)
         raise RateLimitError("Retry limit exceeded") from error
```

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_repository.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/_review.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/constants.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/context.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,27 @@
     Returns:
         Context: The context for the Azure OpenAI API and the models.
     """
     azure_config = _load_context_file() if os.path.exists(os.getenv("CONTEXT_FILE", C.AZURE_CONFIG_FILE)) else {}
 
     if azure_config.get("azure_api_type"):
         openai.api_type = os.environ["OPENAI_API_TYPE"] = azure_config.get("azure_api_type")
+    elif os.getenv("AZURE_OPENAI_API"):
+        openai.api_type = os.environ["OPENAI_API_TYPE"] = C.AZURE_API_TYPE
     elif "OPENAI_API_TYPE" in os.environ:
         openai.api_type = os.environ["OPENAI_API_TYPE"]
 
     if azure_config.get("azure_api_version"):
         openai.api_version = os.environ["OPENAI_API_VERSION"] = azure_config.get("azure_api_version")
+    elif os.getenv("AZURE_OPENAI_API"):
+        openai.api_version = os.environ["OPENAI_API_VERSION"] = C.AZURE_API_VERSION
     elif "OPENAI_API_VERSION" in os.environ:
         openai.api_version = os.environ["OPENAI_API_VERSION"]
 
-    if openai.api_type == C.AZURE_API_TYPE or (not openai.api_type and os.getenv("AZURE_OPENAI_API")):
+    if os.getenv("AZURE_OPENAI_API"):
         openai.api_type = os.environ["OPENAI_API_TYPE"] = C.AZURE_API_TYPE
         openai.api_base = os.environ["OPENAI_API_BASE"] = os.getenv("AZURE_OPENAI_API") or azure_config.get(
             "azure_api_base"
         )
         openai.api_key = os.environ["OPENAI_API_KEY"] = os.getenv("AZURE_OPENAI_API_KEY")  # type: ignore
     elif os.getenv("OPENAI_API_KEY"):
         openai.api_key = os.environ["OPENAI_API_KEY"]
```

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/main.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/prompts/_prompt.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/src/gpt_review/utils.py` & `gpt_review-0.9.1rc762.post1/src/gpt_review/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/conftest.py` & `gpt_review-0.9.1rc762.post1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,22 @@
             assert isinstance(question, str)
             return MockQueryResponse()
 
         def as_query_engine(self):
             return self
 
     def mock_create(
-        model,
-        messages,
-        temperature,
-        max_tokens,
-        top_p,
-        frequency_penalty,
-        presence_penalty,
+        model=None,
+        deployment_id=None,
+        messages=None,
+        temperature=0,
+        max_tokens=500,
+        top_p=1,
+        frequency_penalty=0,
+        presence_penalty=0,
     ) -> MockResponse:
         return MockResponse()
 
     def from_documents(documents, service_context=None) -> MockIndex:
         return MockIndex()
 
     def init_mock_reader(self, owner, repo, use_parser) -> None:
```

### Comparing `gpt_review-0.9.0rc741.post1/tests/mock.diff` & `gpt_review-0.9.1rc762.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_git.py` & `gpt_review-0.9.1rc762.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_github.py` & `gpt_review-0.9.1rc762.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_gpt_cli.py` & `gpt_review-0.9.1rc762.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_llama_index.py` & `gpt_review-0.9.1rc762.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_openai.py` & `gpt_review-0.9.1rc762.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_report.py` & `gpt_review-0.9.1rc762.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/tests/test_review.py` & `gpt_review-0.9.1rc762.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.0rc741.post1/PKG-INFO` & `gpt_review-0.9.1rc762.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.9.0rc741.post1
+Version: 0.9.1rc762.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.9.0rc741.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.9.1rc762.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

