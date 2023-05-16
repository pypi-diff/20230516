# Comparing `tmp/tox-ansible-2.0.3.tar.gz` & `tmp/tox-ansible-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ansible-2.0.3.tar", last modified: Mon May 15 18:57:08 2023, max compression
+gzip compressed data, was "tox-ansible-2.0.4.tar", last modified: Mon May 15 21:37:33 2023, max compression
```

## Comparing `tox-ansible-2.0.3.tar` & `tox-ansible-2.0.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.560289 tox-ansible-2.0.3/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.564288 tox-ansible-2.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.568288 tox-ansible-2.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.568288 tox-ansible-2.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/integration.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/sanity.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/tox-ansible.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/docs/unit.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.552288 tox-ansible-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.572289 tox-ansible-2.0.3/src/tox_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/src/tox_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/src/tox_ansible/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.576289 tox-ansible-2.0.3/src/tox_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 18:57:08.000000 tox-ansible-2.0.3/src/tox_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.576289 tox-ansible-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.552288 tox-ansible-2.0.3/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.552288 tox-ansible-2.0.3/tests/fixtures/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.576289 tox-ansible-2.0.3/tests/fixtures/integration/test_basic/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_basic/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_basic/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/tests/fixtures/integration/test_user_provided/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_user_provided/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/fixtures/integration/test_user_provided/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:57:08.580289 tox-ansible-2.0.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/integration/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tests/integration/test_user_provided.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 18:56:50.000000 tox-ansible-2.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.033168 tox-ansible-2.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.025168 tox-ansible-2.0.4/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.config/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.025168 tox-ansible-2.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.025168 tox-ansible-2.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/workflows/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-15 21:37:33.033168 tox-ansible-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/docs/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/docs/integration.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/docs/sanity.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/docs/tox-ansible.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/docs/unit.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:37:33.033168 tox-ansible-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.021168 tox-ansible-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/src/tox_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/src/tox_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 21:37:32.000000 tox-ansible-2.0.4/src/tox_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/src/tox_ansible/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/src/tox_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-05-15 21:37:32.000000 tox-ansible-2.0.4/src/tox_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-15 21:37:33.000000 tox-ansible-2.0.4/src/tox_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:37:32.000000 tox-ansible-2.0.4/src/tox_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 21:37:32.000000 tox-ansible-2.0.4/src/tox_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 21:37:32.000000 tox-ansible-2.0.4/src/tox_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 21:37:32.000000 tox-ansible-2.0.4/src/tox_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.021168 tox-ansible-2.0.4/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.021168 tox-ansible-2.0.4/tests/fixtures/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/tests/fixtures/integration/test_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/fixtures/integration/test_basic/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/fixtures/integration/test_basic/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/tests/fixtures/integration/test_user_provided/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/fixtures/integration/test_user_provided/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/fixtures/integration/test_user_provided/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:37:33.029168 tox-ansible-2.0.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/integration/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tests/integration/test_user_provided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-15 21:37:18.000000 tox-ansible-2.0.4/tox.ini
```

### Comparing `tox-ansible-2.0.3/.flake8` & `tox-ansible-2.0.4/.flake8`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/.github/workflows/release.yml` & `tox-ansible-2.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/.github/workflows/run.yml` & `tox-ansible-2.0.4/.github/workflows/run.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/.github/workflows/tox.yml` & `tox-ansible-2.0.4/.github/workflows/tox.yml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     outputs:
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
     steps:
       - name: Determine matrix
         id: generate_matrix
         uses: coactions/dynamic-matrix@v1
         with:
-          min_python: "3.8"
+          min_python: "3.7"
           max_python: "3.11"
           default_python: "3.11" # used by jobs in other_names
           other_names: |
             lint
 
   tox:
     name: ${{ matrix.name }} / python ${{ matrix.python_version }}
```

### Comparing `tox-ansible-2.0.3/.gitignore` & `tox-ansible-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/.pre-commit-config.yaml` & `tox-ansible-2.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/LICENSE` & `tox-ansible-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/PKG-INFO` & `tox-ansible-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.3
+Version: 2.0.4
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -12,21 +12,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # tox-ansible
```

### Comparing `tox-ansible-2.0.3/README.md` & `tox-ansible-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/cspell.config.yaml` & `tox-ansible-2.0.4/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/docs/galaxy.yml` & `tox-ansible-2.0.4/docs/galaxy.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/docs/integration.ini` & `tox-ansible-2.0.4/docs/integration.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/docs/sanity.ini` & `tox-ansible-2.0.4/docs/sanity.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/docs/unit.ini` & `tox-ansible-2.0.4/docs/unit.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/pyproject.toml` & `tox-ansible-2.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 name = "tox-ansible"
 description = "A radical approach to testing ansible content"
 readme = "README.md"
 keywords = ["ansible", "collections", "tox"]
 license = { text = "MIT" }
 maintainers = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 authors = [{ "name" = "Bradley A. Thornton", "email" = "bthornto@redhat.com" }]
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
   'Development Status :: 2 - Pre-Alpha',
   'Intended Audience :: Developers',
   'License :: OSI Approved :: MIT License',
   'Operating System :: OS Independent',
   'Topic :: Software Development :: Testing',
   'Topic :: Software Development :: Quality Assurance',
   'Topic :: Utilities',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
+  'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: Implementation :: CPython',
   'Programming Language :: Python :: Implementation :: PyPy',
 ]
@@ -88,15 +89,15 @@
 # ARG = flake8 argument, overlap with pylint
 # FBT = flake8 boolean, silly
 # TID = flake8 tidy imports, need relative for pylint
 # C901 = flake8 complexity, fixme
 # PLR0915 = too many statments, fixme
 # RET504 = prefer less complex return statements
 ignore = ["ARG", "FBT", "TID", "C901", "PLR0915", "RET504"]
-target-version = "py38"
+target-version = "py37"
 
 [tool.ruff.isort]
 lines-after-imports = 2 # Ensures consistency for cases when there's variable vs function/class definitions after imports
 lines-between-types = 1 # Separate import/from with 1 line
 
 [tool.ruff.per-file-ignores]
 # S101 Allow assert in tests
```

### Comparing `tox-ansible-2.0.3/requirements.txt` & `tox-ansible-2.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/src/tox_ansible/plugin.py` & `tox-ansible-2.0.4/src/tox_ansible/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "rm",
     "rsync",
     "mkdir",
     "cd",
     "echo",
 ]
 ENV_LIST = """
-{integration, sanity, unit}-py3.8-{2.9, 2.12, 2.13}
+{integration, sanity, unit}-py3.{7,8}-{2.9, 2.12, 2.13}
 {integration, sanity, unit}-py3.9-{2.12, 2.13, 2.14, 2.15, milestone, devel}
 {integration, sanity, unit}-py3.10-{2.12, 2.13, 2.14, 2.15, milestone, devel}
 {integration, sanity, unit}-py3.11-{2.14, 2.15, milestone, devel}
 """
 TOX_WORK_DIR = Path()
 OUR_DEPS = [
     "pytest",
```

### Comparing `tox-ansible-2.0.3/src/tox_ansible.egg-info/PKG-INFO` & `tox-ansible-2.0.4/src/tox_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.3
+Version: 2.0.4
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -12,21 +12,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # tox-ansible
```

### Comparing `tox-ansible-2.0.3/src/tox_ansible.egg-info/SOURCES.txt` & `tox-ansible-2.0.4/src/tox_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/tests/conftest.py` & `tox-ansible-2.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/tests/integration/test_basic.py` & `tox-ansible-2.0.4/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/tests/integration/test_user_provided.py` & `tox-ansible-2.0.4/tests/integration/test_user_provided.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.3/tox.ini` & `tox-ansible-2.0.4/tox.ini`

 * *Files identical despite different names*

