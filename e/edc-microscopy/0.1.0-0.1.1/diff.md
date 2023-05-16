# Comparing `tmp/edc-microscopy-0.1.0.tar.gz` & `tmp/edc-microscopy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-microscopy-0.1.0.tar", last modified: Mon Nov 28 22:32:02 2022, max compression
+gzip compressed data, was "edc-microscopy-0.1.1.tar", last modified: Tue May 16 02:33:22 2023, max compression
```

## Comparing `edc-microscopy-0.1.0.tar` & `edc-microscopy-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.384238 edc-microscopy-0.1.0/
--rw-r--r--   0 erikvw     (501) staff       (20)      102 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.376625 edc-microscopy-0.1.0/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.379693 edc-microscopy-0.1.0/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1639 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-28 22:00:40.000000 edc-microscopy-0.1.0/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1526 2022-11-28 22:32:02.384321 edc-microscopy-0.1.0/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      712 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.380931 edc-microscopy-0.1.0/edc_microscopy/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      593 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.382028 edc-microscopy-0.1.0/edc_microscopy/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      428 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/form_validators/malaria_test_form_validator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.382357 edc-microscopy-0.1.0/edc_microscopy/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      932 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/model_mixins/malaria_test_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.382638 edc-microscopy-0.1.0/edc_microscopy/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      756 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.382792 edc-microscopy-0.1.0/edc_microscopy/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.384091 edc-microscopy-0.1.0/edc_microscopy/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/edc_microscopy/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-11-28 22:32:02.381699 edc-microscopy-0.1.0/edc_microscopy.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1526 2022-11-28 22:32:02.000000 edc-microscopy-0.1.0/edc_microscopy.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1303 2022-11-28 22:32:02.000000 edc-microscopy-0.1.0/edc_microscopy.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-28 22:32:02.000000 edc-microscopy-0.1.0/edc_microscopy.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-28 22:32:02.000000 edc-microscopy-0.1.0/edc_microscopy.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       15 2022-11-28 22:32:02.000000 edc-microscopy-0.1.0/edc_microscopy.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1608 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2022-11-28 22:31:54.000000 edc-microscopy-0.1.0/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1125 2022-11-28 22:32:02.384640 edc-microscopy-0.1.0/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.038676 edc-microscopy-0.1.1/
+-rw-r--r--   0 erikvw     (501) staff       (20)      102 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.031700 edc-microscopy-0.1.1/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.034782 edc-microscopy-0.1.1/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1645 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1173 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2022-11-28 22:00:40.000000 edc-microscopy-0.1.1/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-05-16 02:33:22.038751 edc-microscopy-0.1.1/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      712 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.035724 edc-microscopy-0.1.1/edc_microscopy/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      173 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      193 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      593 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      366 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.036715 edc-microscopy-0.1.1/edc_microscopy/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      427 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/edc_microscopy/form_validators/malaria_test_form_validator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.036999 edc-microscopy-0.1.1/edc_microscopy/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      931 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/edc_microscopy/model_mixins/malaria_test_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.037270 edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       70 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      755 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.037386 edc-microscopy-0.1.1/edc_microscopy/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.038537 edc-microscopy-0.1.1/edc_microscopy/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      301 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/edc_microscopy/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-16 02:33:22.036461 edc-microscopy-0.1.1/edc_microscopy.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-05-16 02:33:21.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1303 2023-05-16 02:33:22.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-16 02:33:21.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-11-28 22:32:02.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       15 2023-05-16 02:33:22.000000 edc-microscopy-0.1.1/edc_microscopy.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1695 2023-05-16 02:33:14.000000 edc-microscopy-0.1.1/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2022-11-28 22:31:54.000000 edc-microscopy-0.1.1/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2023-05-16 02:33:22.039060 edc-microscopy-0.1.1/setup.cfg
```

### Comparing `edc-microscopy-0.1.0/.github/workflows/build.yml` & `edc-microscopy-0.1.1/.github/workflows/build.yml`

 * *Files 10% similar despite different names*

```diff
@@ -7,37 +7,37 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.10']
+        python-version: ['3.10', '3.11']
         django-version: ['4.1', 'dev']
 
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
 
@@ -50,10 +50,10 @@
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
         with:
           name: Python ${{ matrix.python-version }}
```

### Comparing `edc-microscopy-0.1.0/.gitignore` & `edc-microscopy-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/.pre-commit-config.yaml` & `edc-microscopy-0.1.1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
-        language_version: python3.9
+        language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
+  - repo: https://github.com/rstcheck/rstcheck
+    rev: v6.1.2
+    hooks:
+      - id: rstcheck
+
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-microscopy-0.1.0/LICENSE` & `edc-microscopy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/PKG-INFO` & `edc-microscopy-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: edc-microscopy
-Version: 0.1.0
-Summary: Microcopy model mixins in clinicedc/edc projects
+Version: 0.1.1
+Summary: Microscopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microscopy
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microscopy,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 
 edc-microscopy
 --------------
-Microcopy model mixins in clinicedc/edc projects
+Microscopy model mixins in clinicedc/edc projects
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edc-microscopy.svg
     :target: https://pypi.python.org/pypi/edc-microscopy
 
 .. |actions| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-microscopy/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-microscopy
 
 .. |downloads| image:: https://pepy.tech/badge/edc-microscopy
    :target: https://pepy.tech/project/edc-microscopy
-
```

### Comparing `edc-microscopy-0.1.0/README.rst` & `edc-microscopy-0.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 |pypi| |actions| |codecov| |downloads|
 
 
 edc-microscopy
 --------------
-Microcopy model mixins in clinicedc/edc projects
+Microscopy model mixins in clinicedc/edc projects
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edc-microscopy.svg
     :target: https://pypi.python.org/pypi/edc-microscopy
 
 .. |actions| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-microscopy/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-microscopy
 
 .. |downloads| image:: https://pepy.tech/badge/edc-microscopy
    :target: https://pepy.tech/project/edc-microscopy
-
```

### Comparing `edc-microscopy-0.1.0/edc_microscopy/auth_objects.py` & `edc-microscopy-0.1.1/edc_microscopy/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/edc_microscopy/model_mixins/malaria_test_model_mixin.py` & `edc-microscopy-0.1.1/edc_microscopy/model_mixins/malaria_test_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from edc_constants.choices import PRESENT_ABSENT_NA, YES_NO
 from edc_constants.constants import NOT_APPLICABLE
 
 from ..choices import MALARIA_TEST_CHOICES
 
 
 class MalariaTestModelMixin(models.Model):
-
     performed = models.CharField(
         verbose_name="Was the malaria test performed?",
         max_length=15,
         choices=YES_NO,
     )
 
     not_performed_reason = models.CharField(
```

### Comparing `edc-microscopy-0.1.0/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py` & `edc-microscopy-0.1.1/edc_microscopy/modeladmin_mixins/malaria_test_modeladmin_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.contrib import admin
 from django_audit_fields.admin import audit_fieldset_tuple
 from edc_crf.fieldset import crf_status_fieldset
 
 
 class MalariaTestModelAdminMixin:
-
     form = None
 
     fieldsets = (
         (
             None,
             {
                 "fields": (
```

### Comparing `edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-rsa-local-private.pem` & `edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/edc_microscopy/tests/etc/user-rsa-restricted-private.pem` & `edc-microscopy-0.1.1/edc_microscopy/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/edc_microscopy.egg-info/PKG-INFO` & `edc-microscopy-0.1.1/edc_microscopy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: edc-microscopy
-Version: 0.1.0
-Summary: Microcopy model mixins in clinicedc/edc projects
+Version: 0.1.1
+Summary: Microscopy model mixins in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-microscopy
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc microscopy,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |codecov| |downloads|
 
 
 edc-microscopy
 --------------
-Microcopy model mixins in clinicedc/edc projects
+Microscopy model mixins in clinicedc/edc projects
 
 
 .. |pypi| image:: https://img.shields.io/pypi/v/edc-microscopy.svg
     :target: https://pypi.python.org/pypi/edc-microscopy
 
 .. |actions| image:: https://github.com/clinicedc/edc-microscopy/workflows/build/badge.svg?branch=develop
   :target: https://github.com/clinicedc/edc-microscopy/actions?query=workflow:build
 
 .. |codecov| image:: https://codecov.io/gh/clinicedc/edc-microscopy/branch/develop/graph/badge.svg
   :target: https://codecov.io/gh/clinicedc/edc-microscopy
 
 .. |downloads| image:: https://pepy.tech/badge/edc-microscopy
    :target: https://pepy.tech/project/edc-microscopy
-
```

### Comparing `edc-microscopy-0.1.0/edc_microscopy.egg-info/SOURCES.txt` & `edc-microscopy-0.1.1/edc_microscopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/pyproject.toml` & `edc-microscopy-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,47 +3,52 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py39"]
+target-version = ["py310"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "39"
+py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
 parallel = true
 branch = true
 source = ["edc_microscopy"]
 
 [tool.coverage.paths]
 source = ["edc_microscopy"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{310}-dj{41,dev},
+    py{310,311}-dj{41,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.10: py310, lint
+    3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
     4.1: dj41, lint
     dev: djdev
 
 [testenv]
```

### Comparing `edc-microscopy-0.1.0/runtests.py` & `edc-microscopy-0.1.1/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-microscopy-0.1.0/setup.cfg` & `edc-microscopy-0.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [metadata]
 name = edc-microscopy
 version = attr: _version
 author = Erik van Widenfelt
 author_email = ew2789@gmail.com
 url = https://github.com/clinicedc/edc-microscopy
 license = GPL license, see LICENSE
-description = Microcopy model mixins in clinicedc/edc projects
+description = Microscopy model mixins in clinicedc/edc projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc microscopy, CRF, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
 python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
```

