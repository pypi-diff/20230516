# Comparing `tmp/eossr-1.0.1.tar.gz` & `tmp/eossr-1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eossr-1.0.1.tar", last modified: Tue May 16 12:00:43 2023, max compression
+gzip compressed data, was "eossr-1.0a0.tar", last modified: Tue Jan 17 13:25:50 2023, max compression
```

## Comparing `eossr-1.0.1.tar` & `eossr-1.0a0.tar`

### file list

```diff
@@ -1,139 +1,137 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.551214 eossr-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-05-16 12:00:18.000000 eossr-1.0.1/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.535214 eossr-1.0.1/.gitlab/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.539214 eossr-1.0.1/.gitlab/issue_templates/
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-05-16 12:00:18.000000 eossr-1.0.1/.gitlab/issue_templates/bug.md
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-16 12:00:18.000000 eossr-1.0.1/.gitlab/issue_templates/metadata.md
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-16 12:00:18.000000 eossr-1.0.1/.gitlab/issue_templates/new_feature.md
--rw-rw-rw-   0 root         (0) root         (0)     2020 2023-05-16 12:00:18.000000 eossr-1.0.1/.gitlab-ci-update-codemeta.yml
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-05-16 12:00:18.000000 eossr-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-05-16 12:00:18.000000 eossr-1.0.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3292 2023-05-16 12:00:18.000000 eossr-1.0.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-05-16 12:00:18.000000 eossr-1.0.1/CONTRIBUTING.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.539214 eossr-1.0.1/Docker/
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-05-16 12:00:18.000000 eossr-1.0.1/Docker/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-16 12:00:18.000000 eossr-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5019 2023-05-16 12:00:43.551214 eossr-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-05-16 12:00:18.000000 eossr-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.539214 eossr-1.0.1/binder/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-16 12:00:18.000000 eossr-1.0.1/binder/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     8917 2023-05-16 12:00:18.000000 eossr-1.0.1/codemeta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.541214 eossr-1.0.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.541214 eossr-1.0.1/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/_templates/page.html
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/_templates/versioning.htm
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/_templates/versions.html
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/doc_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.542214 eossr-1.0.1/docs/docstring_sources/
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr.api.rst
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr.api.zenodo.rst
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr.metadata.rst
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr.metadata.schema.rst
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.543214 eossr-1.0.1/docs/docstring_sources/eossr_cli/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli/eossr-check-connection-zenodo.rst
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli/eossr-codemeta2zenodo.rst
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli/eossr-metadata-validator.rst
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli/eossr-upload-repository.rst
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli/eossr-zenodo-validator.rst
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli/eossr-zip-repository.rst
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/docstring_sources/eossr_cli.rst
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)     5740 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/gitlab_to_zenodo.rst
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/howto_generate_docs.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.543214 eossr-1.0.1/docs/images/
--rw-rw-rw-   0 root         (0) root         (0)    56155 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/images/eossr_logo.png
--rw-rw-rw-   0 root         (0) root         (0)     6013 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/images/eossr_logo_200x100.png
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/images/gitlab_zenodo_chart.mmd
--rw-rw-rw-   0 root         (0) root         (0)   108988 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/images/zenodo_funding.png
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/index.html
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.544214 eossr-1.0.1/docs/metadata/
--rw-rw-rw-   0 root         (0) root         (0)    10762 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata/Harvest_zenodo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata/funder_codemeta.rst
--rw-rw-rw-   0 root         (0) root         (0)     3636 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata/metadata.rst
--rw-rw-rw-   0 root         (0) root         (0)     2259 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata/ossr_metadata.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7120 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata/validate_codemeta.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata/validate_codemeta.rst
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/metadata.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.544214 eossr-1.0.1/docs/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)     6402 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/notebooks/ossr_statistics.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2549 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/resources.rst
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-16 12:00:18.000000 eossr-1.0.1/docs/snippets.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.545214 eossr-1.0.1/eossr/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.546214 eossr-1.0.1/eossr/_dev_version/
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/_dev_version/_dev_version.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.546214 eossr-1.0.1/eossr/api/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/ossr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.546214 eossr-1.0.1/eossr/api/tests/
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/tests/test_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.546214 eossr-1.0.1/eossr/api/zenodo/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/zenodo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/zenodo/http_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.547214 eossr-1.0.1/eossr/api/zenodo/tests/
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/zenodo/tests/test_http_status.py
--rw-rw-rw-   0 root         (0) root         (0)    10564 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/zenodo/tests/test_zenodo.py
--rw-rw-rw-   0 root         (0) root         (0)    47368 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/api/zenodo/zenodo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.547214 eossr-1.0.1/eossr/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3375 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/codemeta.py
--rw-rw-rw-   0 root         (0) root         (0)    12965 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/codemeta2zenodo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.548214 eossr-1.0.1/eossr/metadata/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4407 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/schema/codemeta.json
--rw-rw-rw-   0 root         (0) root         (0)    17283 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/schema/escape_codemeta_crosswalk.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.548214 eossr-1.0.1/eossr/metadata/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.548214 eossr-1.0.1/eossr/metadata/tests/samples/
--rw-rw-rw-   0 root         (0) root         (0)     1986 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/samples/codemeta_contributors_sample.json
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/samples/codemeta_not_valid.json
--rw-rw-rw-   0 root         (0) root         (0)     4760 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/samples/codemeta_sample1.json
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/samples/codemeta_valid.json
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/test_codemeta.py
--rw-rw-rw-   0 root         (0) root         (0)     5754 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/test_codemeta2zenodo.py
--rw-rw-rw-   0 root         (0) root         (0)     4620 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/tests/test_zenodo_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/metadata/zenodo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.549214 eossr-1.0.1/eossr/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/check_connection_zenodo.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/eossr_codemeta2zenodo.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/eossr_metadata_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/eossr_upload_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/eossr_zenodo_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.549214 eossr-1.0.1/eossr/scripts/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2810 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/tests/test_scripts.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/update_codemeta_eossr.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/zenodo_user_entries_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/scripts/zip_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.550214 eossr-1.0.1/eossr/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2594 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/tests/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     6959 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-05-16 12:00:18.000000 eossr-1.0.1/eossr/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.545214 eossr-1.0.1/eossr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5019 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3528 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-16 12:00:43.000000 eossr-1.0.1/eossr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.537214 eossr-1.0.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.550214 eossr-1.0.1/examples/CI_code_snippets/
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/CI_code_snippets/1.ex_CI_build_docker_container.md
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/CI_code_snippets/2.ex_CI_build_singularity_image.md
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/CI_code_snippets/3.ex_CI_upload_ossr.md
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/CI_code_snippets/4.ex_CI_test_codemeta_master.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:00:43.550214 eossr-1.0.1/examples/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)     6435 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/notebooks/ZipUrl.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     6339 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/notebooks/ossr_api-Explore_the_OSSR.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8578 2023-05-16 12:00:18.000000 eossr-1.0.1/examples/notebooks/ossr_api-Upload_records_OSSR.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-16 12:00:18.000000 eossr-1.0.1/pytest.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 12:00:43.551214 eossr-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1875 2023-05-16 12:00:18.000000 eossr-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.847748 eossr-1.0a0/
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-01-17 13:25:31.000000 eossr-1.0a0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.833747 eossr-1.0a0/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.836747 eossr-1.0a0/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-01-17 13:25:31.000000 eossr-1.0a0/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-01-17 13:25:31.000000 eossr-1.0a0/.gitlab/issue_templates/metadata.md
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-01-17 13:25:31.000000 eossr-1.0a0/.gitlab/issue_templates/new_feature.md
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2023-01-17 13:25:31.000000 eossr-1.0a0/.gitlab-ci-update-codemeta.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-01-17 13:25:31.000000 eossr-1.0a0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-01-17 13:25:31.000000 eossr-1.0a0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.836747 eossr-1.0a0/Docker/
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-01-17 13:25:31.000000 eossr-1.0a0/Docker/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-01-17 13:25:31.000000 eossr-1.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-01-17 13:25:50.847748 eossr-1.0a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4301 2023-01-17 13:25:31.000000 eossr-1.0a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.836747 eossr-1.0a0/binder/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-01-17 13:25:31.000000 eossr-1.0a0/binder/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     8916 2023-01-17 13:25:31.000000 eossr-1.0a0/codemeta.json
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-01-17 13:25:31.000000 eossr-1.0a0/contributing.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.838747 eossr-1.0a0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.838747 eossr-1.0a0/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/_templates/page.html
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/_templates/versioning.htm
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/_templates/versions.html
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/doc_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.839747 eossr-1.0a0/docs/docstring_sources/
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr.api.rst
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr.api.zenodo.rst
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr.metadata.rst
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr.metadata.schema.rst
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.839747 eossr-1.0a0/docs/docstring_sources/eossr_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli/eossr-check-connection-zenodo.rst
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli/eossr-codemeta2zenodo.rst
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli/eossr-metadata-validator.rst
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli/eossr-upload-repository.rst
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli/eossr-zenodo-validator.rst
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli/eossr-zip-repository.rst
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/docstring_sources/eossr_cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5740 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/gitlab_to_zenodo.rst
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/howto_generate_docs.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.840747 eossr-1.0a0/docs/images/
+-rw-rw-rw-   0 root         (0) root         (0)    56155 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/images/eossr_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/images/gitlab_zenodo_chart.mmd
+-rw-rw-rw-   0 root         (0) root         (0)   108988 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/images/zenodo_funding.png
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/index.html
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.841747 eossr-1.0a0/docs/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)    10762 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata/Harvest_zenodo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata/funder_codemeta.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata/metadata.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2259 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata/ossr_metadata.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata/validate_codemeta.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata/validate_codemeta.rst
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/metadata.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.841747 eossr-1.0a0/docs/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/notebooks/ossr_statistics.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-17 13:25:31.000000 eossr-1.0a0/docs/snippets.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.841747 eossr-1.0a0/eossr/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.842747 eossr-1.0a0/eossr/_dev_version/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/_dev_version/_dev_version.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.842747 eossr-1.0a0/eossr/api/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/ossr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.842747 eossr-1.0a0/eossr/api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/tests/test_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.843747 eossr-1.0a0/eossr/api/zenodo/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/zenodo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/zenodo/http_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.843747 eossr-1.0a0/eossr/api/zenodo/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/zenodo/tests/test_http_status.py
+-rw-rw-rw-   0 root         (0) root         (0)    10564 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/zenodo/tests/test_zenodo.py
+-rw-rw-rw-   0 root         (0) root         (0)    46595 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/api/zenodo/zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.843747 eossr-1.0a0/eossr/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/codemeta.py
+-rw-rw-rw-   0 root         (0) root         (0)    12803 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/codemeta2zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.844747 eossr-1.0a0/eossr/metadata/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4407 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/schema/codemeta.json
+-rw-rw-rw-   0 root         (0) root         (0)    17283 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/schema/escape_codemeta_crosswalk.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.844747 eossr-1.0a0/eossr/metadata/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.844747 eossr-1.0a0/eossr/metadata/tests/samples/
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/samples/codemeta_contributors_sample.json
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/samples/codemeta_not_valid.json
+-rw-rw-rw-   0 root         (0) root         (0)     4760 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/samples/codemeta_sample1.json
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/samples/codemeta_valid.json
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/test_codemeta.py
+-rw-rw-rw-   0 root         (0) root         (0)     5529 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/test_codemeta2zenodo.py
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/tests/test_zenodo_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/metadata/zenodo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.845747 eossr-1.0a0/eossr/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/check_connection_zenodo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/eossr_codemeta2zenodo.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/eossr_metadata_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     7404 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/eossr_upload_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/eossr_zenodo_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.846747 eossr-1.0a0/eossr/scripts/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2810 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/tests/test_scripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/update_codemeta_eossr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/zenodo_user_entries_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/scripts/zip_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.846747 eossr-1.0a0/eossr/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/tests/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     6959 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-01-17 13:25:31.000000 eossr-1.0a0/eossr/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.842747 eossr-1.0a0/eossr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4655 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      432 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      175 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-01-17 13:25:50.000000 eossr-1.0a0/eossr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.835747 eossr-1.0a0/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.846747 eossr-1.0a0/examples/CI_code_snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/CI_code_snippets/1.ex_CI_build_docker_container.md
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/CI_code_snippets/2.ex_CI_build_singularity_image.md
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/CI_code_snippets/3.ex_CI_upload_ossr.md
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/CI_code_snippets/4.ex_CI_test_codemeta_master.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-17 13:25:50.847748 eossr-1.0a0/examples/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/notebooks/ZipUrl.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6339 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/notebooks/ossr_api-Explore_the_OSSR.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8578 2023-01-17 13:25:31.000000 eossr-1.0a0/examples/notebooks/ossr_api-Upload_records_OSSR.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-01-17 13:25:31.000000 eossr-1.0a0/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-17 13:25:50.847748 eossr-1.0a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-01-17 13:25:31.000000 eossr-1.0a0/setup.py
```

### Comparing `eossr-1.0.1/.gitlab-ci-update-codemeta.yml` & `eossr-1.0a0/.gitlab-ci-update-codemeta.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 workflow:
   rules:
     - if: '$CI_MERGE_REQUEST_EVENT_TYPE != "detached"'
 
 update_codemeta_test:
   stage: update_codemeta
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:dev
   script:
     # We need to be on master with no local changes
     - git fetch && git checkout --force $CI_DEFAULT_BRANCH && git reset --hard origin/$CI_DEFAULT_BRANCH
     # setuptools_scm needs to be installed before or it can't be used to determine eossr version during install
     - pip install setuptools_scm
     - pip install .
     - cat codemeta.json
@@ -29,15 +29,15 @@
     - eossr-metadata-validator codemeta.json
     - eossr-check-connection-zenodo --token $ZENODO_TOKEN -p $CI_PROJECT_DIR
   only:
     - master
 
 update_codemeta:
   stage: update_codemeta
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:dev
   script:
     # We need to be on master with no local changes
     - git fetch && git checkout --force $CI_DEFAULT_BRANCH && git reset --hard origin/$CI_DEFAULT_BRANCH
     # setuptools_scm needs to be installed before or it can't be used to determine eossr version during install
     - pip install setuptools_scm
     - pip install .
     - python eossr/scripts/update_codemeta_eossr.py -c codemeta.json
```

### Comparing `eossr-1.0.1/.gitlab-ci.yml` & `eossr-1.0a0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -108,25 +108,25 @@
       --destination "${CI_REGISTRY_IMAGE}:dev"
   only:
     - master
 
 
 deploy_zenodo:
   stage: zenodo
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
   dependencies:
     - build_docker
   before_script:
     - apt update && apt-get install git -y
+    - git clean -df
     - pip install .
-    - git clean -df -x
     - python eossr/scripts/update_codemeta_eossr.py -c codemeta.json
     - eossr-check-connection-zenodo --token $ZENODO_TOKEN -p $CI_PROJECT_DIR
   script:
-    - eossr-upload-repository --add-escape2020 -t $ZENODO_TOKEN -i $CI_PROJECT_DIR --archive-name $CI_PROJECT_NAME.zip -id $ZENODO_RECORD_ID
+    - eossr-upload-repository -t $ZENODO_TOKEN -i $CI_PROJECT_DIR --archive-name $CI_PROJECT_NAME.zip -id $ZENODO_RECORD_ID
   only:
     - tags
 
 
 pages:
   stage: deploy_pages
   image: python:3.9-slim
```

### Comparing `eossr-1.0.1/.pre-commit-config.yaml` & `eossr-1.0a0/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -35,17 +35,7 @@
     rev: 5.10.1
     hooks:
       - id: isort
         name: isort (python)
         args:
           - --line-length=120
           - --profile=black
-
--   repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.30.0
-    hooks:
-    -   id: markdownlint
-        args:
-          [
-            "--disable=MD041",
-            "--disable=MD013"
-          ]
```

### Comparing `eossr-1.0.1/CONTRIBUTING.md` & `eossr-1.0a0/contributing.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,47 @@
 # Contributing
 
 Contributions are most welcome.
 
-When contributing to this repository, it is good practice to first discuss
-the requested change through issues with the owners of this repository
-before making a change.
+When contributing to this repository, it is good practice to first discuss the requested change through issues with the owners of this repository before making a change.
 This will ensure the change you wish to make is aligned with current of planned developments.
 
 ## GitLab account
 
 To open issues or merge requests, you need first to create a gitlab account.
 
-If you are from an academic partner,
-you may be able to connect directly so using EduGAIN.
+If you are from an academic partner, you may be able to connect directly so using EduGAIN.
 Otherwise, [register](https://gitlab.in2p3.fr/users/sign_up).
 
 ## Merge request process
 
 1. If you are a new contributor, please add your contact information to `codemeta.json`
 
-2. Update the `modifiedDate`, `version` and other necessary information in `codemeta.json`.
-You may use the script `eossr/script/update_codemeta.py`.
+2. Update the `modifiedDate`, `version` and other necessary information in `codemeta.json`. You may use the script `eossr/script/update_codemeta.py`.
 
 3. (Re-)Install the eossr after you made changes: `pip install ".[extras]"`
 
 4. Unit tests:
+- If you are adding a new function / method, please add the corresponding unit tests.
+- Run `pytest eossr`.
+- Note that some tests will not run if you don't setup a zenodo token in your env (see README).
+These will be tested during the CI after you opened a merge request though.
 
-   - If you are adding a new function / method,
-   please add the corresponding unit tests.
-   - Run `pytest eossr`.
-   - Note that some tests will not run if you don't setup
-   a zenodo token in your env (see README).
-
-   These will be tested during the CI after you opened a merge request though.
-
-5. Committing your changes will automatically run pre-commit hooks
-that will lint your code.
+5. Committing your changes will automatically run pre-commit hooks that will lint your code.
 Some changes might need to be addressed and/or committed again.
 
-6. Open a merge request.
+7. Open a merge request.
 All tests must pass for the merge request to be reviewed (and accepted).
 
 Note that all contributions will be under the MIT license.
 
 ## Issues
 
 ### Bug report / features requests
 
-If you wish to report a bug and request for a new feature,
-please open an issue and use the corresponding template.
+If you wish to report a bug and request for a new feature, please open an issue and use the corresponding template.
 Be as precise and exhaustive as possible to fasten the implementation of a fix.
 
 ### Metadata discussion
 
-The eOSSR repository is also the place to discuss the metadata schema
-of the OSSR implemented in `codemeta.json`.
-If you want to modify OSSR metadata schema,
-open an issue and add the `MetaData` label.
+The eOSSR repository is also the place to discuss the metadata schema of the OSSR implemented in `codemeta.json`.
+If you want to modify OSSR metadata schema, open an issue and add the `MetaData` label.
```

### Comparing `eossr-1.0.1/LICENSE` & `eossr-1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/PKG-INFO` & `eossr-1.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 Metadata-Version: 2.1
 Name: eossr
-Version: 1.0.1
+Version: 1.0a0
 Summary: ESCAPE OSSR library
 Home-page: https://gitlab.in2p3.fr/escape2020/wp3/eossr
 Author: Thomas Vuillaume, Enrique Garcia
 Author-email: vuillaume@lapp.in2p3.fr
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: extras
 License-File: LICENSE
 
-![eossr_logo](docs/images/eossr_logo_200x100.png)
+<p align="left">
+<img src="docs/images/eossr_logo.png" width="400px" >
+</p>
+
 
 # The ESCAPE OSSR library
 
 The eOSSR Python library gathers all the developments made for the OSSR. In particular, it includes:
-
 - an API to programmatically access the OSSR, retrieve records and publish content
 - functions to map and crosswalk metadata between the CodeMeta schema adopted for the OSSR and Zenodo internal schema
 - functions to help developers automatically contribute to the OSSR, in particular using their continuous integration (see also code snippets)
 
+
 Code: [https://gitlab.in2p3.fr/escape2020/wp3/eossr](https://gitlab.in2p3.fr/escape2020/wp3/eossr)
 Documentation: [https://escape2020.pages.in2p3.fr/wp3/eossr/](https://escape2020.pages.in2p3.fr/wp3/eossr/)
 
-[![pipeline_badge](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/pipeline.svg)](
+
+
+[![](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/pipeline.svg)](
 https://gitlab.in2p3.fr/escape2020/wp3/eossr/-/commits/master)
-[![coverage_badge](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/coverage.svg)](
+[![](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/coverage.svg)](
 https://gitlab.in2p3.fr/escape2020/wp3/eossr/-/commits/master)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5712/badge)](https://bestpractices.coreinfrastructure.org/projects/5712)
-[![SQAaaS badge shields.io](https://img.shields.io/badge/sqaaas%20software-silver-lightgrey)](https://api.eu.badgr.io/public/assertions/aiB2ndZOSL6IuVTOmljRCw "SQAaaS silver badge achieved")
-[![MIT_license_badge](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![zenodo_badge](https://zenodo.org/badge/DOI/10.5281/zenodo.5524912.svg)](https://doi.org/10.5281/zenodo.5524912)
+[![](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![](https://zenodo.org/badge/DOI/10.5281/zenodo.5524912.svg)](https://doi.org/10.5281/zenodo.5524912)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgitlab.in2p3.fr%2Fescape2020%2Fwp3%2Feossr/HEAD?labpath=examples%2Fnotebooks%2Fossr_api-Explore_the_OSSR.ipynb)
 
+
 ## Former stable versions
 
-- v1.0: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7544514.svg)](https://doi.org/10.5281/zenodo.7544514)
 - v0.6: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6475946.svg)](https://doi.org/10.5281/zenodo.6475946)
 - v0.5: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6352039.svg)](https://doi.org/10.5281/zenodo.6352039)
 - v0.4: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6326454.svg)](https://doi.org/10.5281/zenodo.6326454)
-- v0.3.3: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592584.svg)](https://doi.org/10.5281/zenodo.5592584)
-- v0.2 : [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5524913.svg)](https://doi.org/10.5281/zenodo.5524913)
+- v0.3.3: [![](https://zenodo.org/badge/DOI/10.5281/zenodo.5592584.svg)](https://doi.org/10.5281/zenodo.5592584)
+- v0.2 : [![](https://zenodo.org/badge/DOI/10.5281/zenodo.5524913.svg)](https://doi.org/10.5281/zenodo.5524913)
+
 
 ## Install
 
 Commands to be run in your terminal.
 
 ### For users
-
-```bash
+```
 cd eossr
 pip install .
 ```
 
 You can also run it with docker:
-
-```bash
+```
 docker run -it gitlab-registry.in2p3.fr/escape2020/wp3/eossr:latest
 ```
 
 [Visit our registry](https://gitlab.in2p3.fr/escape2020/wp3/eossr/container_registry) to see the available docker containers.
 
 Note that `latest` tag always point to the latest stable released container.
 
+
 ### For developers
 
-```bash
+```
 git clone https://gitlab.in2p3.fr/escape2020/wp3/eossr.git
 cd eossr
 pip install -e .
 ```
 
 #### Running tests
-
 To run tests locally, run:
-
-```bash
+```
 pip install -e ".[tests]"
 
 pytest eossr
 ```
 
 Some tests will be skiped if `SANDBOX_ZENODO_TOKEN` is not defined in your environment variables.
 If you want to run these tests, you will need to create a [sandbox zenodo token](https://sandbox.zenodo.org/account/settings/applications/tokens/new/) and add it to your env:
-
-```bash
+```
 export SANDBOX_ZENODO_TOKEN="your_sandbox_token"
 ```
 
 ## Online CodeMeta validator for the OSSR
 
 The eOSSR powers an online validator for your CodeMeta metadata and to convert it to Zenodo metadata.
 
@@ -100,15 +101,15 @@
 
 See [LICENSE](LICENSE)
 
 ## Cite
 
 To cite this library, please cite our ADASS proceedings:
 
-```latex
+```
 @misc{https://doi.org/10.48550/arxiv.2212.00499,
   doi = {10.48550/ARXIV.2212.00499},
   url = {https://arxiv.org/abs/2212.00499},
   author = {Vuillaume, Thomas and Garcia, Enrique and Tacke, Christian and Gal, Tamas},
   keywords = {Instrumentation and Methods for Astrophysics (astro-ph.IM), FOS: Physical sciences, FOS: Physical sciences},
   title = {The eOSSR library},
   publisher = {arXiv},
@@ -116,7 +117,9 @@
   copyright = {arXiv.org perpetual, non-exclusive license}
 }
 ```
 
 If you used the library in a workflow, please cite the version used as well, using the cite section in [the Zenodo page](https://zenodo.org/record/5592584#.YiALJRPMI-Q) (right column, below the `Versions` section).
 
 
+
+
```

### Comparing `eossr-1.0.1/README.md` & `eossr-1.0a0/eossr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,82 +1,97 @@
-![eossr_logo](docs/images/eossr_logo_200x100.png)
+Metadata-Version: 2.1
+Name: eossr
+Version: 1.0a0
+Summary: ESCAPE OSSR library
+Home-page: https://gitlab.in2p3.fr/escape2020/wp3/eossr
+Author: Thomas Vuillaume, Enrique Garcia
+Author-email: vuillaume@lapp.in2p3.fr
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: extras
+License-File: LICENSE
+
+<p align="left">
+<img src="docs/images/eossr_logo.png" width="400px" >
+</p>
+
 
 # The ESCAPE OSSR library
 
 The eOSSR Python library gathers all the developments made for the OSSR. In particular, it includes:
-
 - an API to programmatically access the OSSR, retrieve records and publish content
 - functions to map and crosswalk metadata between the CodeMeta schema adopted for the OSSR and Zenodo internal schema
 - functions to help developers automatically contribute to the OSSR, in particular using their continuous integration (see also code snippets)
 
+
 Code: [https://gitlab.in2p3.fr/escape2020/wp3/eossr](https://gitlab.in2p3.fr/escape2020/wp3/eossr)
 Documentation: [https://escape2020.pages.in2p3.fr/wp3/eossr/](https://escape2020.pages.in2p3.fr/wp3/eossr/)
 
-[![pipeline_badge](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/pipeline.svg)](
+
+
+[![](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/pipeline.svg)](
 https://gitlab.in2p3.fr/escape2020/wp3/eossr/-/commits/master)
-[![coverage_badge](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/coverage.svg)](
+[![](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/coverage.svg)](
 https://gitlab.in2p3.fr/escape2020/wp3/eossr/-/commits/master)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5712/badge)](https://bestpractices.coreinfrastructure.org/projects/5712)
-[![SQAaaS badge shields.io](https://img.shields.io/badge/sqaaas%20software-silver-lightgrey)](https://api.eu.badgr.io/public/assertions/aiB2ndZOSL6IuVTOmljRCw "SQAaaS silver badge achieved")
-[![MIT_license_badge](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![zenodo_badge](https://zenodo.org/badge/DOI/10.5281/zenodo.5524912.svg)](https://doi.org/10.5281/zenodo.5524912)
+[![](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![](https://zenodo.org/badge/DOI/10.5281/zenodo.5524912.svg)](https://doi.org/10.5281/zenodo.5524912)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgitlab.in2p3.fr%2Fescape2020%2Fwp3%2Feossr/HEAD?labpath=examples%2Fnotebooks%2Fossr_api-Explore_the_OSSR.ipynb)
 
+
 ## Former stable versions
 
-- v1.0: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7544514.svg)](https://doi.org/10.5281/zenodo.7544514)
 - v0.6: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6475946.svg)](https://doi.org/10.5281/zenodo.6475946)
 - v0.5: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6352039.svg)](https://doi.org/10.5281/zenodo.6352039)
 - v0.4: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6326454.svg)](https://doi.org/10.5281/zenodo.6326454)
-- v0.3.3: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592584.svg)](https://doi.org/10.5281/zenodo.5592584)
-- v0.2 : [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5524913.svg)](https://doi.org/10.5281/zenodo.5524913)
+- v0.3.3: [![](https://zenodo.org/badge/DOI/10.5281/zenodo.5592584.svg)](https://doi.org/10.5281/zenodo.5592584)
+- v0.2 : [![](https://zenodo.org/badge/DOI/10.5281/zenodo.5524913.svg)](https://doi.org/10.5281/zenodo.5524913)
+
 
 ## Install
 
 Commands to be run in your terminal.
 
 ### For users
-
-```bash
+```
 cd eossr
 pip install .
 ```
 
 You can also run it with docker:
-
-```bash
+```
 docker run -it gitlab-registry.in2p3.fr/escape2020/wp3/eossr:latest
 ```
 
 [Visit our registry](https://gitlab.in2p3.fr/escape2020/wp3/eossr/container_registry) to see the available docker containers.
 
 Note that `latest` tag always point to the latest stable released container.
 
+
 ### For developers
 
-```bash
+```
 git clone https://gitlab.in2p3.fr/escape2020/wp3/eossr.git
 cd eossr
 pip install -e .
 ```
 
 #### Running tests
-
 To run tests locally, run:
-
-```bash
+```
 pip install -e ".[tests]"
 
 pytest eossr
 ```
 
 Some tests will be skiped if `SANDBOX_ZENODO_TOKEN` is not defined in your environment variables.
 If you want to run these tests, you will need to create a [sandbox zenodo token](https://sandbox.zenodo.org/account/settings/applications/tokens/new/) and add it to your env:
-
-```bash
+```
 export SANDBOX_ZENODO_TOKEN="your_sandbox_token"
 ```
 
 ## Online CodeMeta validator for the OSSR
 
 The eOSSR powers an online validator for your CodeMeta metadata and to convert it to Zenodo metadata.
 
@@ -86,21 +101,25 @@
 
 See [LICENSE](LICENSE)
 
 ## Cite
 
 To cite this library, please cite our ADASS proceedings:
 
-```latex
+```
 @misc{https://doi.org/10.48550/arxiv.2212.00499,
   doi = {10.48550/ARXIV.2212.00499},
   url = {https://arxiv.org/abs/2212.00499},
   author = {Vuillaume, Thomas and Garcia, Enrique and Tacke, Christian and Gal, Tamas},
   keywords = {Instrumentation and Methods for Astrophysics (astro-ph.IM), FOS: Physical sciences, FOS: Physical sciences},
   title = {The eOSSR library},
   publisher = {arXiv},
   year = {2022},
   copyright = {arXiv.org perpetual, non-exclusive license}
 }
 ```
 
 If you used the library in a workflow, please cite the version used as well, using the cite section in [the Zenodo page](https://zenodo.org/record/5592584#.YiALJRPMI-Q) (right column, below the `Versions` section).
+
+
+
+
```

### Comparing `eossr-1.0.1/codemeta.json` & `eossr-1.0a0/codemeta.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -551,8 +551,8 @@
 00002260: 6e20 436f 6d6d 6973 7369 6f6e 222c 0a20  n Commission",. 
 00002270: 2020 2020 2020 2020 2020 2022 4069 6422             "@id"
 00002280: 3a20 2268 7474 7073 3a2f 2f64 6f69 2e6f  : "https://doi.o
 00002290: 7267 2f31 302e 3133 3033 392f 3530 3131  rg/10.13039/5011
 000022a0: 3030 3030 3037 3830 220a 2020 2020 2020  00000780".      
 000022b0: 2020 7d0a 2020 2020 5d2c 0a20 2020 2022    }.    ],.    "
 000022c0: 6675 6e64 696e 6722 3a20 2238 3234 3036  funding": "82406
-000022d0: 3422 0a7d 0a                             4".}.
+000022d0: 3422 0a7d                                4".}
```

### Comparing `eossr-1.0.1/docs/Makefile` & `eossr-1.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/_templates/page.html` & `eossr-1.0a0/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/_templates/versions.html` & `eossr-1.0a0/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/conf.py` & `eossr-1.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/docstring_sources/eossr.metadata.rst` & `eossr-1.0a0/docs/docstring_sources/eossr.metadata.rst`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/gitlab_to_zenodo.rst` & `eossr-1.0a0/docs/gitlab_to_zenodo.rst`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/howto_generate_docs.md` & `eossr-1.0a0/docs/howto_generate_docs.md`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/images/eossr_logo.png` & `eossr-1.0a0/docs/images/eossr_logo.png`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/images/gitlab_zenodo_chart.mmd` & `eossr-1.0a0/docs/images/gitlab_zenodo_chart.mmd`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/images/zenodo_funding.png` & `eossr-1.0a0/docs/images/zenodo_funding.png`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/index.rst` & `eossr-1.0a0/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 .. eossr documentation master file, created by
    sphinx-quickstart on Wed Sep  8 16:24:23 2021.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-
-.. include:: README.md
-   :parser: myst_parser.sphinx_
-
-
-Documentation table of contents
-===============================
+Welcome to eOSSR's documentation!
+=================================
 
 .. toctree::
-   :maxdepth: 3
+   :maxdepth: 4
    :glob:
 
    README
    docstring
    metadata
    notebooks/ossr_statistics.ipynb
    examples
```

### Comparing `eossr-1.0.1/docs/make.bat` & `eossr-1.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/metadata/Harvest_zenodo.ipynb` & `eossr-1.0a0/docs/metadata/Harvest_zenodo.ipynb`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/metadata/funder_codemeta.rst` & `eossr-1.0a0/docs/metadata/funder_codemeta.rst`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/metadata/metadata.rst` & `eossr-1.0a0/docs/metadata/metadata.rst`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/metadata/ossr_metadata.ipynb` & `eossr-1.0a0/docs/metadata/ossr_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/metadata/validate_codemeta.ipynb` & `eossr-1.0a0/docs/metadata/validate_codemeta.ipynb`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/docs/resources.rst` & `eossr-1.0a0/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/api/ossr.py` & `eossr-1.0a0/eossr/api/ossr.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/api/zenodo/http_status.py` & `eossr-1.0a0/eossr/api/zenodo/http_status.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/api/zenodo/tests/test_http_status.py` & `eossr-1.0a0/eossr/api/zenodo/tests/test_http_status.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/api/zenodo/tests/test_zenodo.py` & `eossr-1.0a0/eossr/api/zenodo/tests/test_zenodo.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/api/zenodo/zenodo.py` & `eossr-1.0a0/eossr/api/zenodo/zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 
 import concurrent.futures
 import json
 import os
 import pprint
-import re
 import sys
-import textwrap
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from urllib.parse import urlencode
 from urllib.request import urlopen, urlretrieve
 
 import requests
+from bs4 import BeautifulSoup
 
 from ...metadata.codemeta2zenodo import converter, parse_codemeta_and_write_zenodo_metadata_file
 from ...metadata.zenodo import write_zenodo_metadata
 from ...utils import get_codemeta_from_zipurl, write_json
 from . import http_status
 
 __all__ = [
@@ -739,60 +738,35 @@
         for record in get_zenodo_records(f'conceptrecid:{conceptrecid}', sandbox=self.from_sandbox, **params):
             if 'version' in record.metadata:
                 versions[record.id] = record.metadata['version']
             else:
                 versions[record.id] = None
         return versions
 
-    def _summary(self, linebreak='\n'):
-        """
-        Generate a summary of the record information.
-        The information includes the record id, title, version, DOI, URL and description.
-        If certain information is unavailable, it defaults to 'Unknown'.
-        HTML tags in the description are stripped before being included in the summary.
-
-        :param linebreak: string
-            line break character. default: '\n'
-
-        :return: string
-            The summary string.
-        """
-        lines = [f"=== Record #{self.id} ===", f"Title: {self.title}"]
-        version = self.metadata.get('version', 'Unknown')
-        lines.append(f"Version: {version}")
-        lines.append(f"DOI: {self.data.get('doi', 'Unknown')}")
-
-        links = self.data.get('links', {})
-        if 'html' in links:
-            lines.append(f"URL: {links['html']}")
-
-        description = self.metadata.get('description', '')
-        # Replace paragraph tags with newlines
-        description = re.sub('<p>', linebreak, re.sub('</p>', linebreak, description))
-        # Then strip the remaining HTML tags
-        stripped_description = re.sub('<[^<]+?>', '', description)
-
-        # Wrap description text to 70 characters wide
-        wrapped_description = textwrap.fill(stripped_description, width=70)
-        lines.append(wrapped_description)
-
-        descrp = linebreak.join(lines)
-        return descrp
-
     def print_info(self, linebreak='\n', file=sys.stdout):
         """
-        Print the summary of the record information to a stream, or to sys.stdout by default.
+        Print general information about the record to a stream, or to sys.stdout by default.
 
         :param linebreak: string
             line break character. default: '\n'
         :param file: a file-like object (stream); defaults to the current sys.stdout.
-
-        :return: None
+        :return:
         """
-        print(self._summary(linebreak=linebreak), file=file)
+        metadata = self.data['metadata']
+        descrp = f"=== Record #{self.id} === {linebreak}"
+        descrp += f"Title: {self.title} {linebreak}"
+        version = self.metadata['version'] if 'version' in self.metadata else 'Unknown'
+        descrp += f"Version: {version} {linebreak}"
+        descrp += f"DOI: {self.data['doi']} {linebreak}"
+        if 'links' in self.data.keys() and 'html' in self.data['links'].keys():
+            descrp += f"URL: {self.data['links']['html']} {linebreak}"
+        if 'description' in metadata:
+            descrp += BeautifulSoup(metadata['description'], features='html.parser').get_text()
+        descrp += f"{linebreak}"
+        print(descrp, file=file)
 
     @classmethod
     def from_id(cls, record_id, sandbox=False):
         """
         Retrieve a record from its record id.
 
         :param record_id: int
```

### Comparing `eossr-1.0.1/eossr/metadata/codemeta.py` & `eossr-1.0a0/eossr/metadata/codemeta.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/codemeta2zenodo.py` & `eossr-1.0a0/eossr/metadata/codemeta2zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 
 import json
-import re
 import warnings
 from datetime import date
 from pathlib import Path
 
 from ..utils import spdx_licenses
 from .zenodo import (
     add_escape2020_community,
@@ -41,21 +40,20 @@
     zenodo_person = {}
 
     name = person_property['familyName']
     if 'givenName' in person_property:
         name += f', {person_property["givenName"]}'
     zenodo_person['name'] = name
 
-    # author ID in CodeMeta can be anything, not only ORCID
-    # if format is 0000-0000-0000-0000, it is assumed to be an ORCID
-    if "@id" in person_property and (
-        "orcid.org/" in person_property["@id"] or re.match(r'^\d{4}-\d{4}-\d{4}-\d{3}[0-9X]$', person_property["@id"])
-    ):
-        # reformat "https://orcid.org/0000-0002-5686-2078" to "0000-0002-5686-2078"
-        zenodo_person['orcid'] = person_property["@id"].split('orcid.org/')[-1]
+    if "@id" in person_property:
+        if 'orcid.org/' in person_property["@id"]:
+            # reformat "https://orcid.org/0000-0002-5686-2078"
+            zenodo_person['orcid'] = person_property["@id"].split('orcid.org/')[-1]
+        else:
+            zenodo_person['orcid'] = person_property["@id"]
 
     if "affiliation" in person_property:
         zenodo_person['affiliation'] = person_property['affiliation']['name']
 
     # Parse correctly the contributors
     if contributor_field in codemeta_contributors_fields:
```

### Comparing `eossr-1.0.1/eossr/metadata/schema/codemeta.json` & `eossr-1.0a0/eossr/metadata/schema/codemeta.json`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/schema/escape_codemeta_crosswalk.csv` & `eossr-1.0a0/eossr/metadata/schema/escape_codemeta_crosswalk.csv`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/tests/samples/codemeta_contributors_sample.json` & `eossr-1.0a0/eossr/metadata/tests/samples/codemeta_contributors_sample.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9461538461538462%*

 * *Differences: {"'author'": "{0: {delete: ['affiliation', 'email', '@id']}}",*

 * * "'creator'": "{delete: ['affiliation', 'email', '@id']}",*

 * * "'maintainer'": "{delete: ['affiliation', '@id']}"}*

```diff
@@ -1,53 +1,36 @@
 {
     "@context": "https://doi.org/10.5063/schema/codemeta-2.0",
     "@type": "SoftwareSourceCode",
     "author": [
         {
-            "@id": "Author-and-Creator-same-person-identifier",
             "@type": "Person",
-            "affiliation": {
-                "@type": "Organization",
-                "name": "Author-and-Creator-same-person-affiliation"
-            },
-            "email": "Author-and-Creator-same-person-email",
             "familyName": "Author-and-Creator-same-person-surname",
             "givenName": "Author-and-Creator-same-person-name"
         }
     ],
     "contributor": [
         {
             "@type": "Person",
             "familyName": "Contributor-surname",
             "givenName": "Contributor-name"
         }
     ],
     "creator": {
-        "@id": "Author-and-Creator-same-person-identifier",
         "@type": "Person",
-        "affiliation": {
-            "@type": "Organization",
-            "name": "Author-and-Creator-same-person-affiliation"
-        },
-        "email": "Author-and-Creator-same-person-email",
         "familyName": "Author-and-Creator-same-person-surname",
         "givenName": "Author-and-Creator-same-person-name"
     },
     "editor": {
         "@type": "Person",
         "familyName": "Editor-surname",
         "givenName": "Editor-name"
     },
     "maintainer": {
-        "@id": "https://orcid.org/0000-0000-0000-0000",
         "@type": "Person",
-        "affiliation": {
-            "@type": "Organization",
-            "name": "Maintainer-affiliation"
-        },
         "familyName": "Maintainer-surname",
         "givenName": "Maintainer-name"
     },
     "name": "Codemeta sample with all king of accepted Zenodo schema person properties.",
     "producer": {
         "@type": "Person",
         "familyName": "Producer-surname",
```

### Comparing `eossr-1.0.1/eossr/metadata/tests/samples/codemeta_sample1.json` & `eossr-1.0a0/eossr/metadata/tests/samples/codemeta_sample1.json`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/tests/samples/codemeta_valid.json` & `eossr-1.0a0/eossr/metadata/tests/samples/codemeta_valid.json`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/tests/test_codemeta.py` & `eossr-1.0a0/eossr/metadata/tests/test_codemeta.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/tests/test_codemeta2zenodo.py` & `eossr-1.0a0/eossr/metadata/tests/test_codemeta2zenodo.py`

 * *Files 16% similar despite different names*

```diff
@@ -106,18 +106,14 @@
         codemeta2zenodo.add_author_metadata(zenodo_metadata, codemeta_metadata[person], person)
 
     assert 'creators' in zenodo_metadata
     # 4 'creators' one repeated, should not be duplicated.
     # Maintainer and Contributor. Author and Creator are the same person
     assert len(zenodo_metadata['creators']) == 3
 
-    assert 'orcid' not in zenodo_metadata['creators'][0]
-    assert zenodo_metadata['creators'][1]['name'] == 'Maintainer-surname, Maintainer-name'
-    assert zenodo_metadata['creators'][1]['orcid'] == '0000-0000-0000-0000'
-
     assert 'contributors' in zenodo_metadata
     # Editor, Producer, Publisher, Provider and Sponsor
     assert len(zenodo_metadata['contributors']) == 5
 
 
 def test_parse_person_schema_property():
```

### Comparing `eossr-1.0.1/eossr/metadata/tests/test_zenodo_metadata.py` & `eossr-1.0a0/eossr/metadata/tests/test_zenodo_metadata.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/metadata/zenodo.py` & `eossr-1.0a0/eossr/metadata/zenodo.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/check_connection_zenodo.py` & `eossr-1.0a0/eossr/scripts/check_connection_zenodo.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/eossr_codemeta2zenodo.py` & `eossr-1.0a0/eossr/scripts/eossr_codemeta2zenodo.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/eossr_metadata_validator.py` & `eossr-1.0a0/eossr/scripts/eossr_metadata_validator.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/eossr_upload_repository.py` & `eossr-1.0a0/eossr/scripts/eossr_upload_repository.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/eossr_zenodo_validator.py` & `eossr-1.0a0/eossr/scripts/eossr_zenodo_validator.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/tests/test_scripts.py` & `eossr-1.0a0/eossr/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/update_codemeta_eossr.py` & `eossr-1.0a0/eossr/scripts/update_codemeta_eossr.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/zenodo_user_entries_cleanup.py` & `eossr-1.0a0/eossr/scripts/zenodo_user_entries_cleanup.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/scripts/zip_repository.py` & `eossr-1.0a0/eossr/scripts/zip_repository.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/tests/test_utils.py` & `eossr-1.0a0/eossr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/utils.py` & `eossr-1.0a0/eossr/utils.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr/version.py` & `eossr-1.0a0/eossr/version.py`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/eossr.egg-info/PKG-INFO` & `eossr-1.0a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,83 @@
-Metadata-Version: 2.1
-Name: eossr
-Version: 1.0.1
-Summary: ESCAPE OSSR library
-Home-page: https://gitlab.in2p3.fr/escape2020/wp3/eossr
-Author: Thomas Vuillaume, Enrique Garcia
-Author-email: vuillaume@lapp.in2p3.fr
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: extras
-License-File: LICENSE
+<p align="left">
+<img src="docs/images/eossr_logo.png" width="400px" >
+</p>
 
-![eossr_logo](docs/images/eossr_logo_200x100.png)
 
 # The ESCAPE OSSR library
 
 The eOSSR Python library gathers all the developments made for the OSSR. In particular, it includes:
-
 - an API to programmatically access the OSSR, retrieve records and publish content
 - functions to map and crosswalk metadata between the CodeMeta schema adopted for the OSSR and Zenodo internal schema
 - functions to help developers automatically contribute to the OSSR, in particular using their continuous integration (see also code snippets)
 
+
 Code: [https://gitlab.in2p3.fr/escape2020/wp3/eossr](https://gitlab.in2p3.fr/escape2020/wp3/eossr)
 Documentation: [https://escape2020.pages.in2p3.fr/wp3/eossr/](https://escape2020.pages.in2p3.fr/wp3/eossr/)
 
-[![pipeline_badge](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/pipeline.svg)](
+
+
+[![](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/pipeline.svg)](
 https://gitlab.in2p3.fr/escape2020/wp3/eossr/-/commits/master)
-[![coverage_badge](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/coverage.svg)](
+[![](https://gitlab.in2p3.fr/escape2020/wp3/eossr/badges/master/coverage.svg)](
 https://gitlab.in2p3.fr/escape2020/wp3/eossr/-/commits/master)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/5712/badge)](https://bestpractices.coreinfrastructure.org/projects/5712)
-[![SQAaaS badge shields.io](https://img.shields.io/badge/sqaaas%20software-silver-lightgrey)](https://api.eu.badgr.io/public/assertions/aiB2ndZOSL6IuVTOmljRCw "SQAaaS silver badge achieved")
-[![MIT_license_badge](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![zenodo_badge](https://zenodo.org/badge/DOI/10.5281/zenodo.5524912.svg)](https://doi.org/10.5281/zenodo.5524912)
+[![](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![](https://zenodo.org/badge/DOI/10.5281/zenodo.5524912.svg)](https://doi.org/10.5281/zenodo.5524912)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgitlab.in2p3.fr%2Fescape2020%2Fwp3%2Feossr/HEAD?labpath=examples%2Fnotebooks%2Fossr_api-Explore_the_OSSR.ipynb)
 
+
 ## Former stable versions
 
-- v1.0: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7544514.svg)](https://doi.org/10.5281/zenodo.7544514)
 - v0.6: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6475946.svg)](https://doi.org/10.5281/zenodo.6475946)
 - v0.5: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6352039.svg)](https://doi.org/10.5281/zenodo.6352039)
 - v0.4: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6326454.svg)](https://doi.org/10.5281/zenodo.6326454)
-- v0.3.3: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5592584.svg)](https://doi.org/10.5281/zenodo.5592584)
-- v0.2 : [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5524913.svg)](https://doi.org/10.5281/zenodo.5524913)
+- v0.3.3: [![](https://zenodo.org/badge/DOI/10.5281/zenodo.5592584.svg)](https://doi.org/10.5281/zenodo.5592584)
+- v0.2 : [![](https://zenodo.org/badge/DOI/10.5281/zenodo.5524913.svg)](https://doi.org/10.5281/zenodo.5524913)
+
 
 ## Install
 
 Commands to be run in your terminal.
 
 ### For users
-
-```bash
+```
 cd eossr
 pip install .
 ```
 
 You can also run it with docker:
-
-```bash
+```
 docker run -it gitlab-registry.in2p3.fr/escape2020/wp3/eossr:latest
 ```
 
 [Visit our registry](https://gitlab.in2p3.fr/escape2020/wp3/eossr/container_registry) to see the available docker containers.
 
 Note that `latest` tag always point to the latest stable released container.
 
+
 ### For developers
 
-```bash
+```
 git clone https://gitlab.in2p3.fr/escape2020/wp3/eossr.git
 cd eossr
 pip install -e .
 ```
 
 #### Running tests
-
 To run tests locally, run:
-
-```bash
+```
 pip install -e ".[tests]"
 
 pytest eossr
 ```
 
 Some tests will be skiped if `SANDBOX_ZENODO_TOKEN` is not defined in your environment variables.
 If you want to run these tests, you will need to create a [sandbox zenodo token](https://sandbox.zenodo.org/account/settings/applications/tokens/new/) and add it to your env:
-
-```bash
+```
 export SANDBOX_ZENODO_TOKEN="your_sandbox_token"
 ```
 
 ## Online CodeMeta validator for the OSSR
 
 The eOSSR powers an online validator for your CodeMeta metadata and to convert it to Zenodo metadata.
 
@@ -100,15 +87,15 @@
 
 See [LICENSE](LICENSE)
 
 ## Cite
 
 To cite this library, please cite our ADASS proceedings:
 
-```latex
+```
 @misc{https://doi.org/10.48550/arxiv.2212.00499,
   doi = {10.48550/ARXIV.2212.00499},
   url = {https://arxiv.org/abs/2212.00499},
   author = {Vuillaume, Thomas and Garcia, Enrique and Tacke, Christian and Gal, Tamas},
   keywords = {Instrumentation and Methods for Astrophysics (astro-ph.IM), FOS: Physical sciences, FOS: Physical sciences},
   title = {The eOSSR library},
   publisher = {arXiv},
```

### Comparing `eossr-1.0.1/eossr.egg-info/SOURCES.txt` & `eossr-1.0a0/eossr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 .gitignore
 .gitlab-ci-update-codemeta.yml
 .gitlab-ci.yml
 .pre-commit-config.yaml
-CODE_OF_CONDUCT.md
-CONTRIBUTING.md
 LICENSE
 README.md
 codemeta.json
+contributing.md
 pytest.ini
 setup.py
 .gitlab/issue_templates/bug.md
 .gitlab/issue_templates/metadata.md
 .gitlab/issue_templates/new_feature.md
 Docker/Dockerfile
 binder/requirements.txt
@@ -40,15 +39,14 @@
 docs/docstring_sources/eossr_cli/eossr-check-connection-zenodo.rst
 docs/docstring_sources/eossr_cli/eossr-codemeta2zenodo.rst
 docs/docstring_sources/eossr_cli/eossr-metadata-validator.rst
 docs/docstring_sources/eossr_cli/eossr-upload-repository.rst
 docs/docstring_sources/eossr_cli/eossr-zenodo-validator.rst
 docs/docstring_sources/eossr_cli/eossr-zip-repository.rst
 docs/images/eossr_logo.png
-docs/images/eossr_logo_200x100.png
 docs/images/gitlab_zenodo_chart.mmd
 docs/images/zenodo_funding.png
 docs/metadata/Harvest_zenodo.ipynb
 docs/metadata/funder_codemeta.rst
 docs/metadata/metadata.rst
 docs/metadata/ossr_metadata.ipynb
 docs/metadata/validate_codemeta.ipynb
```

### Comparing `eossr-1.0.1/examples/CI_code_snippets/1.ex_CI_build_docker_container.md` & `eossr-1.0a0/examples/CI_code_snippets/1.ex_CI_build_docker_container.md`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/examples/CI_code_snippets/2.ex_CI_build_singularity_image.md` & `eossr-1.0a0/examples/CI_code_snippets/2.ex_CI_build_singularity_image.md`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/examples/CI_code_snippets/3.ex_CI_upload_ossr.md` & `eossr-1.0a0/examples/CI_code_snippets/3.ex_CI_upload_ossr.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ```yaml
 stages:
  - deploy
 
 deploy_zenodo:
   stage: deploy
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
   before_script:
     - eossr-check-connection-zenodo --token $ZENODO_TOKEN -p $CI_PROJECT_DIR
   script:
     - eossr-upload-repository --add-escape2020 -t $ZENODO_TOKEN -i $CI_PROJECT_DIR --archive-name $CI_PROJECT_NAME.zip [-id $ZENODO_PROJECT_ID]
   only:
     - tags
 
@@ -48,23 +48,23 @@
 
 ```yaml
 stages:
  - deploy
 
 deploy_zenodo:
   stage: deploy
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
   before_script:
     - eossr-check-connection-zenodo --token $SANDBOX_ZENODO_TOKEN -p $CI_PROJECT_DIR --sandbox
   script:
     - eossr-upload-repository --add-escape2020 -t $SANDBOX_ZENODO_TOKEN --sandbox -i $CI_PROJECT_DIR --archive-name $CI_PROJECT_NAME.zip [-id $SANDBOX_ZENODO_PROJECT_ID]
   only:
     - tags
 ```
 
 Note: you might want to restore the directory to its tag stage if you made changes in previous CI stages
 (for example removing build subdirs from previous test stages).
 You may do so using adding the following in the `before_script` section:
 ```
 - apt-get install git -y
-- git reset --hard HEAD && git clean -fd -x
+- git reset --hard HEAD && git clean -fd
 ```
```

### Comparing `eossr-1.0.1/examples/CI_code_snippets/4.ex_CI_test_codemeta_master.md` & `eossr-1.0a0/examples/CI_code_snippets/4.ex_CI_test_codemeta_master.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,135 +9,81 @@
 
 Please note that this snippet will only work if you have linked your
 gitlab account with Zenodo. If not, please follow this [tutorial](
 https://escape2020.pages.in2p3.fr/wp3/eossr/gitlab_to_zenodo.html#link-your-gitlab-project-with-zenodo
 )
 
 ### Test your `codemeta.json` file
-
-The `eossr-metadata-validator` will test the validity of your `codemeta.json` against ESCAPE OSSR requirements.
-
 ```yaml
 stages:
- - test
+ - test_codemeta
 
-test_codemeta:
-  stage: test
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+test_codemeta_ingestion:
+  stage: test_codemeta
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
   script:
-    - eossr-metadata-validator codemeta.json
+    - eossr-check-connection-zenodo --token $ZENODO_TOKEN -p $CI_PROJECT_DIR
   rules:
     - if: '$CI_PIPELINE_SOURCE == "merge_request_event" && $CI_MERGE_REQUEST_TARGET_BRANCH_NAME == $CI_DEFAULT_BRANCH'
     - changes:
       - codemeta.json
 ```
 
 ### Test your `.zenodo.json` file
 
-You may test the validity of your `.zenodo.json` and its correct upload to Zenodo.
-
 ```yaml
 stages:
- - test
+ - test_zenodo
 
-test_zenodo_upload:
-  stage: test
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
+test_codemeta_ingestion:
+  stage: test_codemeta
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
   script:
-    - eossr-zenodo-validator .zenodo.json
     - eossr-check-connection-zenodo --token $ZENODO_TOKEN -p $CI_PROJECT_DIR
   rules:
     - if: '$CI_PIPELINE_SOURCE == "merge_request_event" && $CI_MERGE_REQUEST_TARGET_BRANCH_NAME == $CI_DEFAULT_BRANCH'
     - changes:
       - .zenodo.json
 ```
 
 ## GitHub
 
 If you are hosting your developments on GitHub, you are probably using [the GitHub-Zenodo integration](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content) to upload your code to Zenodo when making a GitHub release.
 
 The GitHub-Zenodo integration can use three sources for its metadata:
 1. GitHub - if no other source of metadata exist, information such as release title and notes, versioning, contributors, etc... will be provided by GitHub metadata. Metadata from former releases or edited on the Zenodo web portal are **updated**.
 2. `CITATION.cff` - if a `CITATION.cff` file lives at the root of your repository, it will be used by Zenodo to **update** existing metadata (from a former release or from GitHub)
-3. `.zenodo.json` - if a `.zenodo.json` file lives at the root of your repository, it will be used by Zenodo as **unique** source of metadata and will **replace** all existing metadata
+3. `.zenodo.json` - if a `.zenodo.json` file lives at the root of your repository, it will be used by Zenodo as **unique** source of metadata and will **replace** all existing metadata 
 
 In order to have a unique source of metadata for your project and depending on your workflow, you _might_ want to to convert your `codemeta.json` file to a `.zenodo.json` file before releases using [the `ossr-codemeta2zenodo` CLI](../docstring_sources/eossr_cli/eossr-codemeta2zenodo).
 
-### Test your `codemeta.json` file
-
-You can test the validity of your `codemeta.json` file against the OSSR requirements using the following:
-
-```yaml
-name: validate codemeta
-
-on:
-  push:
-    paths:
-      - codemeta.json
-  
-jobs:
-  build:
-    runs-on: ubuntu-latest
-    container:
-      image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
-    steps:
-      - uses: actions/checkout@v2
-      - name: validate codemeta
-        run: eossr-metadata-validator codemeta.json
-```
-
 
 ### Test your `.zenodo.json` file
 
-A simple validation test can be done using the `eossr-zenodo-validator` CLI.
-
-```yaml
-name: validate zenodo
-
-on:
-  push:
-    paths:
-      - .zenodo.json
-  
-jobs:
-  build:
-    runs-on: ubuntu-latest
-    container:
-      image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v1.0
-    steps:
-      - uses: actions/checkout@v2
-      - name: validate zenodo
-        run: eossr-zenodo-validator .zenodo.json
-```
-
-For a more complete test, you can use the `eossr-check-connection-zenodo` CLI
-that will try to upload your `.zenodo.json` file to Zenodo and check that the upload was successful.
-
-
 First, you will need to:
 - [create an access token in Zenodo](https://zenodo.org/account/settings/applications/tokens/new/)
 (or [sandbox](https://sandbox.zenodo.org/account/settings/applications/tokens/new/)) with a `deposit:write` access
 - add it to [your repository secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets)
 under the name `ZENODO_TOKEN`.
 
 Then, you can use the following GitHub action snippet to check the validity of your `.zenodo.json` file.
 To do so, add this code snippet in a file `.github/workflows/check_zenodo.yml` in your repository:
 
 ```yaml
-name: check zenodo publication
+name: check zenodo
 
 on:
   push:
     paths:
       - .zenodo.json
 
 jobs:
   build:
     runs-on: ubuntu-latest
     container:
       image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
     steps:
       - uses: actions/checkout@v2
-      - name: check zenodo publication
+      - name: check zenodo
         run: |
           eossr-check-connection-zenodo --token ${{ secrets.ZENODO_TOKEN }} -p .
 ```
```

### Comparing `eossr-1.0.1/examples/notebooks/ZipUrl.ipynb` & `eossr-1.0a0/examples/notebooks/ZipUrl.ipynb`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/examples/notebooks/ossr_api-Explore_the_OSSR.ipynb` & `eossr-1.0a0/examples/notebooks/ossr_api-Explore_the_OSSR.ipynb`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/examples/notebooks/ossr_api-Upload_records_OSSR.ipynb` & `eossr-1.0a0/examples/notebooks/ossr_api-Upload_records_OSSR.ipynb`

 * *Files identical despite different names*

### Comparing `eossr-1.0.1/setup.py` & `eossr-1.0a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     name='eossr',
     description="ESCAPE OSSR library",
     long_description=long_description,
     long_description_content_type='text/markdown',
     setup_requires="setuptools_scm",
     install_requires=[
         "requests>=2.25.0,<3.0",
+        "beautifulsoup4>=4.10.0,<5.0",
         "markdown>=3.3.6,<4.0",
         "pandas",
         "remotezip==0.9.3",
         "semver>=2,<3",
         "jsonschema",
         "jsonref",
     ],
```

