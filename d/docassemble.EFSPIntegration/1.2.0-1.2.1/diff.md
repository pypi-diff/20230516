# Comparing `tmp/docassemble.EFSPIntegration-1.2.0.tar.gz` & `tmp/docassemble.EFSPIntegration-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.EFSPIntegration-1.2.0.tar", last modified: Tue May  9 20:24:58 2023, max compression
+gzip compressed data, was "docassemble.EFSPIntegration-1.2.1.tar", last modified: Tue May 16 18:02:33 2023, max compression
```

## Comparing `docassemble.EFSPIntegration-1.2.0.tar` & `docassemble.EFSPIntegration-1.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.945632 docassemble.EFSPIntegration-1.2.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.949632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30386 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.941632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.949632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)    40916 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    26764 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    20187 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/case_search.yml
--rw-r--r--   0 runner    (1001) docker     (122)    32169 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml
--rw-r--r--   0 runner    (1001) docker     (122)     8870 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/login_qs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/toga_payments.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.949632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature
--rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/efm_client.py
--rw-r--r--   0 runner    (1001) docker     (122)    15778 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/interview_logic.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    38477 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/py_efsp_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18552 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/peoria_to_cr.json
--rw-r--r--   0 runner    (1001) docker     (122)   238595 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/temp2.json
--rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    55792 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/vars.json
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 20:24:58.945632 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 20:24:58.000000 docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-09 20:24:58.953632 docassemble.EFSPIntegration-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-09 20:24:42.000000 docassemble.EFSPIntegration-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.963621 docassemble.EFSPIntegration-1.2.1/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.963621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30386 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.963621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)    40916 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/admin_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    26764 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    20187 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/case_search.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    32169 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/efiling_integration.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     9636 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/login_qs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/minimal_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/toga_payments.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/admin_interview.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/example_upload.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/unauthenticated_interview.feature
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     3208 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/static/Ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/efm_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15778 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/interview_logic.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    38477 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/py_efsp_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.967621 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18552 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7090 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/peoria_to_cr.json
+-rw-r--r--   0 runner    (1001) docker     (122)   238595 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/temp2.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5698 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55792 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/vars.json
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 18:02:33.963621 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2174 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-16 18:02:33.000000 docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-16 18:02:33.971621 docassemble.EFSPIntegration-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-16 18:02:19.000000 docassemble.EFSPIntegration-1.2.1/setup.py
```

### Comparing `docassemble.EFSPIntegration-1.2.0/LICENSE` & `docassemble.EFSPIntegration-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/PKG-INFO` & `docassemble.EFSPIntegration-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.EFSPIntegration
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/SuffolkLITLab/docassemble-EFSPIntegration
 Author: Bryce Willey
 Author-email: bwilley@suffolk.edu
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.EFSPIntegration-1.2.0/README.md` & `docassemble.EFSPIntegration-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/conversions.py` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/conversions.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/admin_interview.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/admin_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/any_filing_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/case_search.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/case_search.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/efiling_integration.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/efiling_integration.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/login_qs.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/login_qs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -58,24 +58,46 @@
     tyler_header_name = f"TYLER-TOKEN-{jurisdiction_id.upper()}"
     try:
       if da_store.defined("EFSP-" + tyler_header_name):
         proxy_conn.proxy_client.headers[tyler_header_name] = da_store.get("EFSP-" + tyler_header_name)
         tyler_user = proxy_conn.get_user()
         if tyler_user.is_ok():
           my_username = tyler_user.data.get('email')
-          log(word("You are now connected to your e-filing account") + f" ({my_username})", "primary")
-          logged_in_user_is_admin, logged_in_user_is_global_admin = get_tyler_roles(proxy_conn, None, tyler_user)
-          tyler_login = True
+          if continue_stored_login:
+            log(word("You are now connected to your e-filing account") + f" ({my_username})", "primary")
+            logged_in_user_is_admin, logged_in_user_is_global_admin = get_tyler_roles(proxy_conn, None, tyler_user)
+            tyler_login = True
+          else:
+            da_store.set("EFSP-" + tyler_header_name, '')
+            da_store.set(tyler_user_id_key, '')
+    except NameError as err:
+      # Re-raise only name errors, so DA can work correctly
+      raise err
     except Exception as ex:
       log(f"Error when trying to get da_store Tyler token: {ex}")
 ---
+continue button field: continue_stored_login
+question: Login to eFile${ state_name_to_code(jurisdiction_id) } as ${my_username}?
+subquestion: |
+  You recently logged in to eFile${ state_name_to_code(jurisdiction_id) } with the email ${ my_username }.
+
+  Would you like to continue with this email?
+fields:
+  - no label: continue_stored_login
+    input type: radio
+    choices:
+      - Yes, log me in with this email.: True
+      - No, I want to use a different login email.: False
+---
+code: |
+  tyler_user_id_key = f"EFSP-TYLER-ID-{jurisdiction_id.lower()}"
+---
 only sets:
   - tyler_user_id
 code: |
-  tyler_user_id_key = f"EFSP-TYLER-ID-{jurisdiction_id.lower()}"
   if da_store.defined(tyler_user_id_key):
     tyler_user_id = da_store.get(tyler_user_id_key)
   else:
     # not there: will need to login to get the same info
     tyler_user_id = tyler_login_resp.data
 ---
 code: |
```

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/minimal_interview.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/minimal_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/toga_payments.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/toga_payments.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/toga_payments_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/unauthenticated_actions.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/questions/unauthenticated_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/admin_interview.feature` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/admin_interview.feature`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/any_filing_interview.feature`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/sources/example_upload.pdf` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/sources/example_upload.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/data/static/Ajax-loader.gif` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/data/static/Ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/efm_client.py` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/efm_client.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/interview_logic.py` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/interview_logic.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/py_efsp_client.py` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/py_efsp_client.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/integration_test.py` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/peoria_to_cr.json` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/peoria_to_cr.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/temp2.json` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/temp2.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/test_conversions.py` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble/EFSPIntegration/test/vars.json` & `docassemble.EFSPIntegration-1.2.1/docassemble/EFSPIntegration/test/vars.json`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/PKG-INFO` & `docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.EFSPIntegration
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/SuffolkLITLab/docassemble-EFSPIntegration
 Author: Bryce Willey
 Author-email: bwilley@suffolk.edu
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docassemble.EFSPIntegration-1.2.0/docassemble.EFSPIntegration.egg-info/SOURCES.txt` & `docassemble.EFSPIntegration-1.2.1/docassemble.EFSPIntegration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docassemble.EFSPIntegration-1.2.0/setup.py` & `docassemble.EFSPIntegration-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.EFSPIntegration',
-      version='1.2.0',
+      version='1.2.1',
       description=(''),
       long_description='# docassemble-EFSPIntegration\r\n\r\nA docassemble extension that talks to [a proxy e-filing server](https://github.com/SuffolkLITLab/EfileProxyServer/) easily within a docassemble interview.\r\n\r\nMain interviews of import:\r\n\r\n* any_filing_interview.yml: allows you to make any type of filing, initial or subsequent\r\n* admin_interview.yml: lets you handle admin / user functionality, outside of the context of cases and filings\r\n\r\nIn progress!\r\n\r\n## Authors\r\n\r\nQuinten Steenhuis (qsteenhuis@suffolk.edu)\r\nBryce Willey (bwilley@suffolk.edu)\r\n',
       long_description_content_type='text/markdown',
       author='Bryce Willey',
       author_email='bwilley@suffolk.edu',
       license='The MIT License (MIT)',
       url='https://github.com/SuffolkLITLab/docassemble-EFSPIntegration',
```

