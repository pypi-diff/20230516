# Comparing `tmp/gpt_review-0.9.1rc773.post1.tar.gz` & `tmp/gpt_review-0.9.1rc775.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_review-0.9.1rc773.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gpt_review-0.9.1rc775.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gpt_review-0.9.1rc773.post1.tar` & `gpt_review-0.9.1rc775.post1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      336 2023-05-16 05:50:35.023675 gpt_review-0.9.1rc773.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-16 05:50:35.023675 gpt_review-0.9.1rc773.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-16 05:50:35.023675 gpt_review-0.9.1rc773.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-16 05:50:35.023675 gpt_review-0.9.1rc773.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-16 05:50:35.023675 gpt_review-0.9.1rc773.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-16 05:50:35.023675 gpt_review-0.9.1rc773.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4200 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1747 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1862 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/LICENSE
--rw-r--r--   0        0        0     3556 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/README.md
--rw-r--r--   0        0        0     2308 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/action.yml
--rw-r--r--   0        0        0      307 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/azure.yaml.template
--rw-r--r--   0        0        0      218 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/config.summary.template.yml
--rw-r--r--   0        0        0      362 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/prompt.template.yml
--rw-r--r--   0        0        0     8500 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-16 05:50:46.959734 gpt_review-0.9.1rc773.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      170 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-16 05:50:46.959734 gpt_review-0.9.1rc773.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      170 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     9453 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3520 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5998 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     6437 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     4241 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8558 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      955 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0     3227 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/context.py
--rw-r--r--   0        0        0      924 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      349 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/prompts/prompt_bug.yaml
--rw-r--r--   0        0        0      362 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/prompts/prompt_coverage.yaml
--rw-r--r--   0        0        0      327 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/prompts/prompt_summary.yaml
--rw-r--r--   0        0        0      863 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/src/gpt_review/utils.py
--rw-r--r--   0        0        0      218 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5573 2023-05-16 05:50:35.027675 gpt_review-0.9.1rc773.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/mock.diff
--rw-r--r--   0        0        0      375 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_context.py
--rw-r--r--   0        0        0      716 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_github.py
--rw-r--r--   0        0        0     5427 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1449 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-16 05:50:35.031675 gpt_review-0.9.1rc773.post1/tests/test_review.py
--rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 gpt_review-0.9.1rc773.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-16 05:58:50.005099 gpt_review-0.9.1rc775.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-16 05:58:50.005099 gpt_review-0.9.1rc775.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-16 05:58:50.005099 gpt_review-0.9.1rc775.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-16 05:58:50.005099 gpt_review-0.9.1rc775.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-16 05:58:50.005099 gpt_review-0.9.1rc775.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4200 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1829 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1862 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/LICENSE
+-rw-r--r--   0        0        0     3556 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/README.md
+-rw-r--r--   0        0        0     2308 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/action.yml
+-rw-r--r--   0        0        0      307 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/azure.yaml.template
+-rw-r--r--   0        0        0      218 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/config.summary.template.yml
+-rw-r--r--   0        0        0      362 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/prompt.template.yml
+-rw-r--r--   0        0        0     8500 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-16 05:58:58.593142 gpt_review-0.9.1rc775.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-16 05:58:58.593142 gpt_review-0.9.1rc775.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     9453 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3520 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5998 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     6437 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     4241 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8558 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      955 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0     3227 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/context.py
+-rw-r--r--   0        0        0      924 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      349 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/prompts/prompt_bug.yaml
+-rw-r--r--   0        0        0      362 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/prompts/prompt_coverage.yaml
+-rw-r--r--   0        0        0      327 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/prompts/prompt_summary.yaml
+-rw-r--r--   0        0        0      863 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/src/gpt_review/utils.py
+-rw-r--r--   0        0        0      218 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5573 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/mock.diff
+-rw-r--r--   0        0        0      375 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/test_context.py
+-rw-r--r--   0        0        0      716 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5427 2023-05-16 05:58:50.009100 gpt_review-0.9.1rc775.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-16 05:58:50.013100 gpt_review-0.9.1rc775.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1449 2023-05-16 05:58:50.013100 gpt_review-0.9.1rc775.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-16 05:58:50.013100 gpt_review-0.9.1rc775.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-16 05:58:50.013100 gpt_review-0.9.1rc775.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 gpt_review-0.9.1rc775.post1/PKG-INFO
```

### Comparing `gpt_review-0.9.1rc773.post1/.devcontainer/devcontainer.json` & `gpt_review-0.9.1rc775.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt_review-0.9.1rc775.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/dependabot.yml` & `gpt_review-0.9.1rc775.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/pull_request_template.md` & `gpt_review-0.9.1rc775.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/workflows/codeql.yml` & `gpt_review-0.9.1rc775.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/workflows/dependency-review.yml` & `gpt_review-0.9.1rc775.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt_review-0.9.1rc775.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/workflows/python.yml` & `gpt_review-0.9.1rc775.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.github/workflows/test-action.yml` & `gpt_review-0.9.1rc775.post1/.github/workflows/test-action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,25 @@
 
       - run: |
           sudo apt-get update
           python3 -m venv .env
           source .env/bin/activate
           python -m pip install --upgrade pip
           python -m pip install gpt-review
-
       - run: |
           source .env/bin/activate
 
           gpt github review \
             --access-token $GITHUB_TOKEN \
             --pull-request $PR_NUMBER \
             --repository $REPOSITORY_NAME
+        continue-on-error: true
+
+      - run: |
+          source .env/bin/activate
 
           pip install -e .
 
           gpt github review \
             --access-token $GITHUB_TOKEN \
             --pull-request $PR_NUMBER \
             --repository $REPOSITORY_NAME
```

### Comparing `gpt_review-0.9.1rc773.post1/.gitignore` & `gpt_review-0.9.1rc775.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/.vscode/settings.json` & `gpt_review-0.9.1rc775.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/LICENSE` & `gpt_review-0.9.1rc775.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/README.md` & `gpt_review-0.9.1rc775.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/action.yml` & `gpt_review-0.9.1rc775.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/pyproject.toml` & `gpt_review-0.9.1rc775.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_ask.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_git.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_github.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_gpt_cli.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_llama_index.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_openai.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_repository.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/_review.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/constants.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/context.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/context.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/main.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/prompts/_prompt.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/src/gpt_review/utils.py` & `gpt_review-0.9.1rc775.post1/src/gpt_review/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/conftest.py` & `gpt_review-0.9.1rc775.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/mock.diff` & `gpt_review-0.9.1rc775.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_git.py` & `gpt_review-0.9.1rc775.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_github.py` & `gpt_review-0.9.1rc775.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_gpt_cli.py` & `gpt_review-0.9.1rc775.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_llama_index.py` & `gpt_review-0.9.1rc775.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_openai.py` & `gpt_review-0.9.1rc775.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_report.py` & `gpt_review-0.9.1rc775.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/tests/test_review.py` & `gpt_review-0.9.1rc775.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt_review-0.9.1rc773.post1/PKG-INFO` & `gpt_review-0.9.1rc775.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.9.1rc773.post1
+Version: 0.9.1rc775.post1
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
-Metadata-Version: 2.1 Name: gpt-review Version: 0.9.1rc773.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.9.1rc775.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

