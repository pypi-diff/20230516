# Comparing `tmp/hyperparameter-0.5.0.tar.gz` & `tmp/hyperparameter-0.5.1.tar.gz`

## Comparing `hyperparameter-0.5.0.tar` & `hyperparameter-0.5.1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 hyperparameter-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123      834 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      126 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0     1001      123      595 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      706 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/workflows/codecov.yml
--rw-r--r--   0     1001      123      845 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/workflows/mkdocs.yml
--rw-r--r--   0     1001      123     1202 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      123     2001 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.gitignore
--rw-r--r--   0     1001      123      356 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     5202 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123     9722 2023-05-12 09:08:52.000000 hyperparameter-0.5.0/Cargo.lock
--rw-r--r--   0     1001      123    11356 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/LICENSE
--rw-r--r--   0     1001      123     3861 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/README.md
--rw-r--r--   0     1001      123     3457 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/README.zh.md
--rw-r--r--   0     1001      123     2846 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/examples/optimization.md
--rw-r--r--   0     1001      123     2868 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/examples/optimization.zh.md
--rw-r--r--   0     1001      123     3861 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/index.md
--rw-r--r--   0     1001      123     3457 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/index.zh.md
--rw-r--r--   0     1001      123     3000 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/quick_start.md
--rw-r--r--   0     1001      123     3000 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/quick_start.zh.md
--rw-r--r--   0     1001      123       48 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/reference.md
--rw-r--r--   0     1001      123      110 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/requirements.txt
--rw-r--r--   0     1001      123     6738 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/docs/structured_parameter.md
--rw-r--r--   0     1001      123      337 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/application/README.md
--rw-r--r--   0     1001      123      789 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/application/app.py
--rw-r--r--   0     1001      123       46 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/application/cfg.json
--rw-r--r--   0     1001      123     4733 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/automl_optuna_mnist/automl_mnist.py
--rw-r--r--   0     1001      123     1382 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/cpp/cxx_test.cc
--rw-r--r--   0     1001      123       96 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/cpp/cxx_test.py
--rw-r--r--   0     1001      123      237 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/cpp/cxx_test.sh
--rw-r--r--   0     1001      123      152 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/README.md
--rw-r--r--   0     1001      123     5625 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/main.py
--rw-r--r--   0     1001      123     5899 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/main_with_hp.py
--rw-r--r--   0     1001      123     6202 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/main_with_hp_with_mlflow.py
--rw-r--r--   0     1001      123       18 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/mnist/requirements.txt
--rw-r--r--   0     1001      123     2846 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/README.md
--rw-r--r--   0     1001      123      230 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/example.py
--rw-r--r--   0     1001      123      527 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/example_hp.py
--rw-r--r--   0     1001      123      727 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/optuna/example_hp_nested.py
--rw-r--r--   0     1001      123     1650 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/README.md
--rw-r--r--   0     1001      123      581 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/example_1.py
--rw-r--r--   0     1001      123      934 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/example_2.py
--rw-r--r--   0     1001      123     1059 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/example_mlflow.py
--rw-r--r--   0     1001      123      867 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/sparse_lr/model.py
--rw-r--r--   0     1001      123     1631 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/examples/storage.rs
--rw-r--r--   0     1001      123        0 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hparam/__init__.py
--rw-r--r--   0     1001      123     3710 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hparam/__main__.py
--rw-r--r--   0     1001      123      314 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/__init__.py
--rw-r--r--   0     1001      123    16064 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/api.py
--rw-r--r--   0     1001      123     7032 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/hyperparameter.h
--rw-r--r--   0     1001      123      828 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/loader.py
--rw-r--r--   0     1001      123     3854 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/storage.py
--rw-r--r--   0     1001      123     2223 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/hyperparameter/tune.py
--rw-r--r--   0     1001      123     1249 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/mkdocs.yml
--rw-r--r--   0     1001      123      938 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/pyproject.toml
--rw-r--r--   0     1001      123     5802 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/entry.rs
--rw-r--r--   0     1001      123     5132 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/ext.rs
--rw-r--r--   0     1001      123     2038 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/ffi.rs
--rw-r--r--   0     1001      123      106 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123     8872 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/storage.rs
--rw-r--r--   0     1001      123     4528 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/src/xxh.rs
--rwxr-xr-x   0     1001      123    40754 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/a.out
--rw-r--r--   0     1001      123     3769 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/test_param_scope.py
--rw-r--r--   0     1001      123      697 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/test_param_scope_thread.py
--rw-r--r--   0     1001      123     2988 2023-05-12 09:08:34.000000 hyperparameter-0.5.0/tests/test_rust_backend.py
--rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 hyperparameter-0.5.1/Cargo.toml
+-rw-r--r--   0     1001      123      834 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      126 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0     1001      123      595 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      706 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/workflows/codecov.yml
+-rw-r--r--   0     1001      123      845 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0     1001      123     1202 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      123     2001 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.gitignore
+-rw-r--r--   0     1001      123      356 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5202 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123    22947 2023-05-16 03:06:41.000000 hyperparameter-0.5.1/Cargo.lock
+-rw-r--r--   0     1001      123    11356 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/LICENSE
+-rw-r--r--   0     1001      123     3861 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/README.md
+-rw-r--r--   0     1001      123     3457 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/README.zh.md
+-rw-r--r--   0     1001      123     2846 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/examples/optimization.md
+-rw-r--r--   0     1001      123     2868 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/examples/optimization.zh.md
+-rw-r--r--   0     1001      123     3861 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/index.md
+-rw-r--r--   0     1001      123     3457 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/index.zh.md
+-rw-r--r--   0     1001      123     3000 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/quick_start.md
+-rw-r--r--   0     1001      123     3000 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/quick_start.zh.md
+-rw-r--r--   0     1001      123       48 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/reference.md
+-rw-r--r--   0     1001      123      110 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/requirements.txt
+-rw-r--r--   0     1001      123     6738 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/docs/structured_parameter.md
+-rw-r--r--   0     1001      123      337 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/application/README.md
+-rw-r--r--   0     1001      123      789 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/application/app.py
+-rw-r--r--   0     1001      123       46 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/application/cfg.json
+-rw-r--r--   0     1001      123     4733 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/automl_optuna_mnist/automl_mnist.py
+-rw-r--r--   0     1001      123     2047 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/cpp/cxx_test.cc
+-rw-r--r--   0     1001      123      271 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/cpp/cxx_test.py
+-rw-r--r--   0     1001      123      237 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/cpp/cxx_test.sh
+-rw-r--r--   0     1001      123      152 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/README.md
+-rw-r--r--   0     1001      123     5625 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/main.py
+-rw-r--r--   0     1001      123     5899 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/main_with_hp.py
+-rw-r--r--   0     1001      123     6202 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/main_with_hp_with_mlflow.py
+-rw-r--r--   0     1001      123       18 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/mnist/requirements.txt
+-rw-r--r--   0     1001      123     2846 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/README.md
+-rw-r--r--   0     1001      123      230 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/example.py
+-rw-r--r--   0     1001      123      527 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/example_hp.py
+-rw-r--r--   0     1001      123      727 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/optuna/example_hp_nested.py
+-rw-r--r--   0     1001      123     1650 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/README.md
+-rw-r--r--   0     1001      123      581 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/example_1.py
+-rw-r--r--   0     1001      123      934 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/example_2.py
+-rw-r--r--   0     1001      123     1059 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/example_mlflow.py
+-rw-r--r--   0     1001      123      867 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/sparse_lr/model.py
+-rw-r--r--   0     1001      123     1631 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/examples/storage.rs
+-rw-r--r--   0     1001      123        0 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hparam/__init__.py
+-rw-r--r--   0     1001      123     3710 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hparam/__main__.py
+-rw-r--r--   0     1001      123      314 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/__init__.py
+-rw-r--r--   0     1001      123    17127 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/api.py
+-rw-r--r--   0     1001      123     7588 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/hyperparameter.h
+-rw-r--r--   0     1001      123      828 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/loader.py
+-rw-r--r--   0     1001      123     4196 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/storage.py
+-rw-r--r--   0     1001      123     2223 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/hyperparameter/tune.py
+-rw-r--r--   0     1001      123     1249 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/mkdocs.yml
+-rw-r--r--   0     1001      123      938 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/pyproject.toml
+-rw-r--r--   0     1001      123     5571 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/entry.rs
+-rw-r--r--   0     1001      123     6580 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/ext.rs
+-rw-r--r--   0     1001      123     2038 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/ffi.rs
+-rw-r--r--   0     1001      123      106 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/lib.rs
+-rw-r--r--   0     1001      123     8129 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/storage.rs
+-rw-r--r--   0     1001      123     4528 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/src/xxh.rs
+-rwxr-xr-x   0     1001      123    40754 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/a.out
+-rw-r--r--   0     1001      123      912 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_auto_param.py
+-rw-r--r--   0     1001      123     3769 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_param_scope.py
+-rw-r--r--   0     1001      123      697 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_param_scope_thread.py
+-rw-r--r--   0     1001      123     2988 2023-05-16 03:06:29.000000 hyperparameter-0.5.1/tests/test_rust_backend.py
+-rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.1/PKG-INFO
```

### Comparing `hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `hyperparameter-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/.github/workflows/codecov.yml` & `hyperparameter-0.5.1/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/.github/workflows/mkdocs.yml` & `hyperparameter-0.5.1/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/.github/workflows/python-publish.yml` & `hyperparameter-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/.gitignore` & `hyperparameter-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/CODE_OF_CONDUCT.md` & `hyperparameter-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/LICENSE` & `hyperparameter-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/README.md` & `hyperparameter-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/README.zh.md` & `hyperparameter-0.5.1/README.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/examples/optimization.md` & `hyperparameter-0.5.1/docs/examples/optimization.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/examples/optimization.zh.md` & `hyperparameter-0.5.1/docs/examples/optimization.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/index.md` & `hyperparameter-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/index.zh.md` & `hyperparameter-0.5.1/docs/index.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/quick_start.md` & `hyperparameter-0.5.1/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/quick_start.zh.md` & `hyperparameter-0.5.1/docs/quick_start.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/docs/structured_parameter.md` & `hyperparameter-0.5.1/docs/structured_parameter.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/application/app.py` & `hyperparameter-0.5.1/examples/application/app.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/automl_optuna_mnist/automl_mnist.py` & `hyperparameter-0.5.1/examples/automl_optuna_mnist/automl_mnist.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/mnist/main.py` & `hyperparameter-0.5.1/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/mnist/main_with_hp.py` & `hyperparameter-0.5.1/examples/mnist/main_with_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/mnist/main_with_hp_with_mlflow.py` & `hyperparameter-0.5.1/examples/mnist/main_with_hp_with_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/optuna/README.md` & `hyperparameter-0.5.1/examples/optuna/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/optuna/example_hp.py` & `hyperparameter-0.5.1/examples/optuna/example_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/optuna/example_hp_nested.py` & `hyperparameter-0.5.1/examples/optuna/example_hp_nested.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/sparse_lr/README.md` & `hyperparameter-0.5.1/examples/sparse_lr/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/sparse_lr/example_1.py` & `hyperparameter-0.5.1/examples/sparse_lr/example_1.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/sparse_lr/example_2.py` & `hyperparameter-0.5.1/examples/sparse_lr/example_2.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/sparse_lr/example_mlflow.py` & `hyperparameter-0.5.1/examples/sparse_lr/example_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/sparse_lr/model.py` & `hyperparameter-0.5.1/examples/sparse_lr/model.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/examples/storage.rs` & `hyperparameter-0.5.1/examples/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/hparam/__main__.py` & `hyperparameter-0.5.1/hparam/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/hyperparameter/api.py` & `hyperparameter-0.5.1/hyperparameter/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import inspect
 from typing import Any, Callable, Dict
 
-from hyperparameter.storage import TLSKVStorage
+from hyperparameter.storage import TLSKVStorage, has_rust_backend
+from hyperparameter.storage import xxh64
 from .tune import Suggester
 
 
 def _repr_dict(d):
     d = [(k, v) for k, v in d.items()]
     d.sort()
     return d
@@ -457,15 +458,15 @@
         retval._storage = TLSKVStorage.current()
         return retval
 
     @staticmethod
     def init(params=None):
         """init param_scope for a new thread."""
         param_scope(**params).__enter__()
-        
+
     @staticmethod
     def frozen():
         with param_scope():
             TLSKVStorage.frozen()
 
 
 _param_scope = param_scope._func
@@ -516,14 +517,46 @@
     ...     foo(2)
     2 4 c None
     """
 
     if callable(name_or_func):
         return auto_param(None)(name_or_func)
 
+    if has_rust_backend:
+
+        def hashed_wrapper(func):
+            predef_kws = {}
+
+            if name_or_func is None:
+                namespace = func.__name__
+            else:
+                namespace = name_or_func
+
+            signature = inspect.signature(func)
+            for k, v in signature.parameters.items():
+                if v.default != v.empty:
+                    name = "{}.{}".format(namespace, k)
+                    predef_kws[k] = xxh64(name)
+
+            @functools.wraps(func)
+            def inner(*arg, **kws):
+                with param_scope() as hp:
+                    for k, v in predef_kws.items():
+                        if k not in kws:
+                            try:
+                                val = hp._storage.get_by_hash(v)
+                                kws[k] = val
+                            except ValueError:
+                                pass
+                    return func(*arg, **kws)
+
+            return inner
+
+        return hashed_wrapper
+
     def wrapper(func):
         predef_kws = {}
         predef_val = {}
 
         if name_or_func is None:
             namespace = func.__name__
         else:
```

### Comparing `hyperparameter-0.5.0/hyperparameter/hyperparameter.h` & `hyperparameter-0.5.1/hyperparameter/hyperparameter.h`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     struct xxh64
     {
         static constexpr uint64_t hash(const char *p, uint64_t len, uint64_t seed = 42)
         {
             return finalize((len >= 32 ? h32bytes(p, len, seed) : seed + PRIME5) + len, p + (len & ~0x1F), len & 0x1F);
         }
-
+        
     private:
         static constexpr uint64_t PRIME1 = 11400714785074694791ULL;
         static constexpr uint64_t PRIME2 = 14029467366897019727ULL;
         static constexpr uint64_t PRIME3 = 1609587929392839161ULL;
         static constexpr uint64_t PRIME4 = 9650029242287828579ULL;
         static constexpr uint64_t PRIME5 = 2870177450012600261ULL;
 
@@ -187,10 +187,25 @@
     }
 
     template <>
     void Hyperparameter::put<const char *>(const char *key, const char *val)
     {
         return storage_put_str(_storage, key, val);
     }
+
+    std::shared_ptr<hyperparameter::Hyperparameter> get_hp() {
+      static std::shared_ptr<Hyperparameter> hp;
+      if (!hp) {
+        hp = hyperparameter::create_shared();
+      }
+      return hp;
+    }
 }
 
+#define GETHP hyperparameter::get_hp()  
+
+// Implicit create hyperparameter object
+#define GETPARAM(p, default_val)                                              \
+  (GETHP->get(([](){ constexpr uint64_t x = hyperparameter::xxhash(#p,sizeof(#p)-1); return x;})(), default_val))
+#define PUTPARAM(p, default_val) (GETHP->put(#p, default_val))
+
 #endif
```

### Comparing `hyperparameter-0.5.0/hyperparameter/loader.py` & `hyperparameter-0.5.1/hyperparameter/loader.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/hyperparameter/storage.py` & `hyperparameter-0.5.1/hyperparameter/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,17 @@
                     storage[key] = v
 
         if kws is not None:
             return _update(kws, prefix=None)
 
     def clear(self):
         self._storage.clear()
+        
+    def get_by_hash(self, *args, **kwargs):
+        raise RuntimeError("hyperparameter is not build with rust backend")
 
     def get(self, name: str, accessor: Callable = None) -> Any:
         if name in self.__slots__:
             return self.__dict__[name]
         curr = self
         while curr is not None and curr._storage is not None:
             if name in curr._storage:
@@ -135,14 +138,25 @@
         return TLSKVStorage.tls.his[-1]
 
     @staticmethod
     def frozen():
         GLOBAL_STORAGE.update(TLSKVStorage.tls.his[-1].storage())
 
 
+has_rust_backend = False
+
+
+def xxh64(*args, **kwargs):
+    raise RuntimeError("hyperparameter is not build with rust backend")
+
+
 try:
     if os.environ.get("HYPERPARAMETER_BACKEND", "RUST") == "RUST":
         from hyperparameter.rbackend import KVStorage
+        from hyperparameter.rbackend import xxh64
+
         TLSKVStorage = KVStorage
+        has_rust_backend = True
 except:
     import traceback
+
     traceback.print_exc()
```

### Comparing `hyperparameter-0.5.0/hyperparameter/tune.py` & `hyperparameter-0.5.1/hyperparameter/tune.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/mkdocs.yml` & `hyperparameter-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/pyproject.toml` & `hyperparameter-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "hyperparameter"
-version = "0.5.0"
+version = "0.5.1"
 authors = [{ name = "Reiase", email = "reiase@gmail.com" }]
 description = "A hyper-parameter library for researchers, data scientists and machine learning engineers."
 requires-python = ">=3.7"
 readme = "README.md"
 license = { text = "Apache License Version 2.0" }
 
 [tool.maturin]
```

### Comparing `hyperparameter-0.5.0/src/entry.rs` & `hyperparameter-0.5.1/src/entry.rs`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 #[derive(Debug, Clone, PartialEq)]
 pub enum Value {
     Empty,
     Int(i64),
     Float(f64),
     Text(CacheString),
     Boolen(bool),
-    UserDefined(*mut c_void, Option<Arc<DeferUnsafe>>),
-    PyObject(*mut c_void, Arc<DeferUnsafe>),
+    UserDefined(
+        *mut c_void,              //data
+        i32,                      //kind
+        Option<Arc<DeferUnsafe>>, // de-allocator
+    ),
 }
 
 impl From<i64> for Value {
     fn from(value: i64) -> Self {
         Value::Int(value)
     }
 }
@@ -55,38 +58,39 @@
     fn from(value: bool) -> Self {
         Value::Boolen(value)
     }
 }
 
 impl From<*mut c_void> for Value {
     fn from(value: *mut c_void) -> Self {
-        Value::UserDefined(value, None)
+        Value::UserDefined(value, 0, None)
     }
 }
 
 impl Value {
-    pub fn pyobj(ptr: *mut c_void, free: unsafe fn(*mut c_void)) -> Value {
-        Value::PyObject(ptr, Arc::new(DeferUnsafe(ptr, free)))
+    pub fn managed(ptr: *mut c_void, kind: i32, free: unsafe fn(*mut c_void)) -> Value {
+        Value::UserDefined(ptr, kind, Arc::new(DeferUnsafe(ptr, free)).into())
     }
 }
 
 impl TryFrom<Value> for i64 {
     type Error = String;
 
     fn try_from(value: Value) -> Result<Self, Self::Error> {
         match value {
             Value::Empty => Err("empty value error".into()),
-            Value::Int(v) => Ok(v),
+            Value::Int(v) => Ok(v.into()),
             Value::Float(v) => Ok(v as i64),
             Value::Text(v) => v
                 .parse::<i64>()
                 .or_else(|_| Err(format!("error convert {} into i64", v))),
             Value::Boolen(v) => Ok(v.into()),
-            Value::UserDefined(_, _) => Err("data type not matched, `Userdefined` and i64".into()),
-            Value::PyObject(_, _) => Err("data type not matched, `PyObject` and i64".into()),
+            Value::UserDefined(_, _, _) => {
+                Err("data type not matched, `UserDefined` and i64".into())
+            }
         }
     }
 }
 
 impl TryFrom<Value> for f64 {
     type Error = String;
 
@@ -95,48 +99,51 @@
             Value::Empty => Err("empty value error".into()),
             Value::Int(v) => Ok(v as f64),
             Value::Float(v) => Ok(v),
             Value::Text(v) => v
                 .parse::<f64>()
                 .or_else(|_| Err(format!("error convert {} into i64", v))),
             Value::Boolen(_) => Err("data type not matched, `Boolen` and i64".into()),
-            Value::UserDefined(_, _) => Err("data type not matched, `Userdefined` and f64".into()),
-            Value::PyObject(_, _) => Err("data type not matched, `PyObject` and f64".into()),
+            Value::UserDefined(_, _, _) => {
+                Err("data type not matched, `UserDefined` and f64".into())
+            }
         }
     }
 }
 
 impl TryFrom<Value> for String {
     type Error = String;
 
     fn try_from(value: Value) -> Result<Self, Self::Error> {
         match value {
             Value::Empty => Err("empty value error".into()),
             Value::Int(v) => Ok(format!("{}", v)),
             Value::Float(v) => Ok(format!("{}", v)),
             Value::Text(v) => Ok(v.to_string()),
             Value::Boolen(v) => Ok(format!("{}", v)),
-            Value::UserDefined(_, _) => Err("data type not matched, `Userdefined` and str".into()),
-            Value::PyObject(_, _) => Err("data type not matched, `PyObject` and str".into()),
+            Value::UserDefined(_, _, _) => {
+                Err("data type not matched, `UserDefined` and str".into())
+            }
         }
     }
 }
 
 impl TryFrom<Value> for bool {
     type Error = String;
 
     fn try_from(value: Value) -> Result<Self, Self::Error> {
         match value {
             Value::Empty => Err("empty value error".into()),
             Value::Int(v) => Ok(v != 0),
             Value::Float(_) => Err("data type not matched, `Float` and bool".into()),
             Value::Text(_) => Err("data type not matched, `Text` and bool".into()),
             Value::Boolen(v) => Ok(v),
-            Value::UserDefined(_, _) => Err("data type not matched, `Userdefined` and str".into()),
-            Value::PyObject(_, _) => Err("data type not matched, `PyObject` and str".into()),
+            Value::UserDefined(_, _, _) => {
+                Err("data type not matched, `UserDefined` and str".into())
+            }
         }
     }
 }
 
 #[derive(Debug, Clone)]
 pub enum EntryValue {
     Single(Value),
@@ -178,31 +185,27 @@
     }
 
     pub fn clone_value(&self) -> Value {
         self.val.get().clone()
     }
 
     pub fn update<V: Into<Value>>(&mut self, val: V) {
-        let his = self.val.history();
-        if his.is_none() {
-            self.val = EntryValue::Single(val.into());
+        if let Some(his) = self.val.history() {
+            self.val = EntryValue::Versioned(val.into(), his.clone());
         } else {
-            self.val = EntryValue::Versioned(val.into(), (*his.unwrap()).clone());
+            self.val = EntryValue::Single(val.into());
         }
     }
 
     pub fn revision<V: Into<Value>>(&mut self, val: V) {
         let value = &self.val;
         self.val = EntryValue::Versioned(val.into(), Box::new(value.clone()));
     }
 
     pub fn rollback(&mut self) -> Result<(), ()> {
-        let his = self.val.history();
-        match his {
-            None => Err(()),
-            Some(h) => {
-                self.val = *h.clone();
-                Ok(())
-            }
+        if let Some(h) = self.val.history() {
+            self.val = *h.clone();
+            return Ok(());
         }
+        return Err(());
     }
 }
```

### Comparing `hyperparameter-0.5.0/src/ext.rs` & `hyperparameter-0.5.1/src/ext.rs`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,32 @@
 use pyo3::FromPyPointer;
 
 use crate::entry::Value;
 use crate::storage::frozen_as_global_storage;
 use crate::storage::Storage;
 use crate::storage::StorageManager;
 use crate::storage::MGR;
+use crate::xxh::xxhstr;
+
+#[repr(C)]
+enum UserDefinedType {
+    PyObjectType = 1,
+}
+
+impl Into<Value> for *mut pyo3::ffi::PyObject {
+    fn into(self) -> Value {
+        Value::managed(
+            self as *mut c_void,
+            UserDefinedType::PyObjectType as i32,
+            |obj: *mut c_void| unsafe {
+                Py_DecRef(obj as *mut pyo3::ffi::PyObject);
+            },
+        )
+    }
+}
 
 #[pyclass]
 pub struct KVStorage {
     storage: Storage,
     isview: bool,
 }
 
@@ -40,17 +58,20 @@
         for k in self.storage.keys().iter() {
             match self.storage.get(k).unwrap() {
                 Value::Empty => Ok(()),
                 Value::Int(v) => res.set_item(k, v),
                 Value::Float(v) => res.set_item(k, v),
                 Value::Text(v) => res.set_item(k, v.as_str()),
                 Value::Boolen(v) => res.set_item(k, v),
-                Value::UserDefined(v, _) => res.set_item(k, v as u64),
-                Value::PyObject(v, _) => {
-                    res.set_item(k, PyAny::from_owned_ptr(py, v as *mut pyo3::ffi::PyObject))
+                Value::UserDefined(v, k, _) => {
+                    if k == UserDefinedType::PyObjectType as i32 {
+                        res.set_item(k, PyAny::from_owned_ptr(py, v as *mut pyo3::ffi::PyObject))
+                    } else {
+                        res.set_item(k, v as u64)
+                    }
                 }
             }
             .unwrap();
         }
         Ok(res.into())
     }
 
@@ -89,49 +110,67 @@
         match self.storage.get(key) {
             Some(val) => match val {
                 Value::Empty => Err(PyValueError::new_err("not found")),
                 Value::Int(v) => Ok(Some(v.into_py(py))),
                 Value::Float(v) => Ok(Some(v.into_py(py))),
                 Value::Text(v) => Ok(Some(v.into_py(py))),
                 Value::Boolen(v) => Ok(Some(v.into_py(py))),
-                Value::UserDefined(v, _) => Ok(Some((v as u64).into_py(py))),
-                Value::PyObject(v, _) => Ok(Some(
-                    PyAny::from_borrowed_ptr(py, v as *mut pyo3::ffi::PyObject).into(),
-                )),
+                Value::UserDefined(v, k, _) => {
+                    if k == UserDefinedType::PyObjectType as i32 {
+                        Ok(Some(
+                            PyAny::from_borrowed_ptr(py, v as *mut pyo3::ffi::PyObject).into(),
+                        ))
+                    } else {
+                        Ok(Some((v as u64).into_py(py)))
+                    }
+                }
+            },
+            None => Err(PyValueError::new_err("not found")),
+        }
+    }
+
+    pub unsafe fn get_by_hash(&mut self, py: Python<'_>, hkey: u64) -> PyResult<Option<PyObject>> {
+        match self.storage.get_by_hash(hkey) {
+            Some(val) => match val {
+                Value::Empty => Err(PyValueError::new_err("not found")),
+                Value::Int(v) => Ok(Some(v.into_py(py))),
+                Value::Float(v) => Ok(Some(v.into_py(py))),
+                Value::Text(v) => Ok(Some(v.into_py(py))),
+                Value::Boolen(v) => Ok(Some(v.into_py(py))),
+                Value::UserDefined(v, k, _) => {
+                    if k == UserDefinedType::PyObjectType as i32 {
+                        Ok(Some(
+                            PyAny::from_borrowed_ptr(py, v as *mut pyo3::ffi::PyObject).into(),
+                        ))
+                    } else {
+                        Ok(Some((v as u64).into_py(py)))
+                    }
+                }
             },
             None => Err(PyValueError::new_err("not found")),
         }
     }
 
     pub unsafe fn put(&mut self, key: String, val: &PyAny) -> PyResult<()> {
         if self.isview {
             MGR.with(|mgr: &RefCell<StorageManager>| mgr.borrow_mut().put_key(key.clone()));
-            // MGR.with_borrow_mut(|mgr| mgr.put_key(key.clone()));
         }
         if val.is_none() {
             self.storage.put(key, Value::Empty);
-            return Ok(());
-        }
-        if val.is_instance_of::<PyBool>().unwrap() {
+        } else if val.is_instance_of::<PyBool>().unwrap() {
             self.storage.put(key, val.extract::<bool>().unwrap());
         } else if val.is_instance_of::<PyFloat>().unwrap() {
             self.storage.put(key, val.extract::<f64>().unwrap());
         } else if val.is_instance_of::<PyString>().unwrap() {
             self.storage.put(key, val.extract::<&str>().unwrap());
         } else if val.is_instance_of::<PyInt>().unwrap() {
             self.storage.put(key, val.extract::<i64>().unwrap());
         } else {
-            // TODO support release pyobj
             Py_IncRef(val.into_ptr());
-            self.storage.put(
-                key,
-                Value::pyobj(val.into_ptr() as *mut c_void, |obj: *mut c_void| {
-                    Py_DecRef(obj as *mut pyo3::ffi::PyObject);
-                }),
-            );
+            self.storage.put(key, val.into_ptr());
         }
         Ok(())
     }
 
     pub fn enter(&mut self) {
         self.storage.enter();
     }
@@ -152,12 +191,18 @@
 
     #[staticmethod]
     pub fn frozen() {
         frozen_as_global_storage();
     }
 }
 
+#[pyfunction]
+pub fn xxh64(s: &str) -> u64 {
+    xxhstr(s)
+}
+
 #[pymodule]
 fn rbackend(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<KVStorage>()?;
+    m.add_function(wrap_pyfunction!(xxh64, m)?)?;
     Ok(())
 }
```

### Comparing `hyperparameter-0.5.0/src/ffi.rs` & `hyperparameter-0.5.1/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/src/storage.rs` & `hyperparameter-0.5.1/src/storage.rs`

 * *Files 5% similar despite different names*

```diff
@@ -152,44 +152,26 @@
                 } else {
                     m.borrow_mut().tls.borrow_mut().insert(*k, v.clone());
                 }
             }
             let keys = self.tree().keys().cloned().collect();
             m.borrow_mut().stack.push(RefCell::new(keys));
         });
-        // MGR.with_borrow_mut(|m| {
-        //     for (k, v) in self.tree().iter() {
-        //         if m.tls.borrow().contains_key(&k) {
-        //             tree_revision(m.tls.borrow_mut(), *k, v.clone_value());
-        //         } else {
-        //             m.tls.borrow_mut().insert(*k, v.clone());
-        //         }
-        //     }
-        //     let keys = self.tree().keys().cloned().collect();
-        //     m.stack.push(RefCell::new(keys));
-        // });
         self.isview += 1;
     }
 
     pub fn exit(&mut self) {
         MGR.with(|m| {
             let mut m = m.borrow_mut();
             if let Some(keys) = m.stack.pop() {
                 keys.borrow()
                     .iter()
                     .for_each(|k| tree_rollback(m.tls.borrow_mut(), *k));
             }
         });
-        // MGR.with_borrow_mut(|m| {
-        //     if let Some(keys) = m.stack.pop() {
-        //         keys.borrow()
-        //             .iter()
-        //             .for_each(|k| tree_rollback(m.tls.borrow_mut(), *k));
-        //     }
-        // });
         self.isview -= 1;
     }
 
     pub fn get_by_hash(&self, key: u64) -> Option<Value> {
         if self.isview == 0 {
             if let Some(e) = self.tree().get(&key) {
                 return Some(e.clone_value());
```

### Comparing `hyperparameter-0.5.0/src/xxh.rs` & `hyperparameter-0.5.1/src/xxh.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/tests/a.out` & `hyperparameter-0.5.1/tests/a.out`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/tests/test_param_scope.py` & `hyperparameter-0.5.1/tests/test_param_scope.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/tests/test_param_scope_thread.py` & `hyperparameter-0.5.1/tests/test_param_scope_thread.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/tests/test_rust_backend.py` & `hyperparameter-0.5.1/tests/test_rust_backend.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.0/PKG-INFO` & `hyperparameter-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter
-Version: 0.5.0
+Version: 0.5.1
 License-File: LICENSE
 Summary: A hyper-parameter library for researchers, data scientists and machine learning engineers.
 Author-email: Reiase <reiase@gmail.com>
 License: Apache License Version 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

