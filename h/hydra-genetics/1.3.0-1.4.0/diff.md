# Comparing `tmp/hydra-genetics-1.3.0.tar.gz` & `tmp/hydra-genetics-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-genetics-1.3.0.tar", last modified: Wed May 10 08:23:13 2023, max compression
+gzip compressed data, was "hydra-genetics-1.4.0.tar", last modified: Tue May 16 09:56:44 2023, max compression
```

## Comparing `hydra-genetics-1.3.0.tar` & `hydra-genetics-1.4.0.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/commands/prep_pipeline_env.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/linters/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.968211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.tests/integration/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.tests/integration/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/config/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/config/output_files.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/config/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/config/units.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/images/
--rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/images/hydragenetics.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/rule-template/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/rule-template/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/rule-template/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/rule-template/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/rule-template/skeleton_rule.smk
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/rule-template/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/chr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/hotspot_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/multibp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/hydra_genetics/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/models/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/hydra_genetics/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.972211 hydra-genetics-1.3.0/hydra_genetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 08:23:13.000000 hydra-genetics-1.3.0/hydra_genetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/tests/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/io/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/io/test_mutations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:13.976211 hydra-genetics-1.3.0/tests/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/models/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/tests/utils/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-10 08:23:09.000000 hydra-genetics-1.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.694573 hydra-genetics-1.4.0/hydra_genetics/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33247 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/commands/prep_pipeline_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.698573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.698573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.698573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.690573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/output_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/output_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/config/units.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/images/hydragenetics.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/rule-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/skeleton_rule.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/rule-template/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.702573 hydra-genetics-1.4.0/hydra_genetics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/chr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/multibp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/hydra_genetics/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/models/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/hydra_genetics/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.694573 hydra-genetics-1.4.0/hydra_genetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 09:56:44.000000 hydra-genetics-1.4.0/hydra_genetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/io/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/io/test_mutations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:44.706573 hydra-genetics-1.4.0/tests/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/models/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/tests/utils/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-16 09:56:40.000000 hydra-genetics-1.4.0/versioneer.py
```

### Comparing `hydra-genetics-1.3.0/LICENSE.md` & `hydra-genetics-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/PKG-INFO` & `hydra-genetics-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.3.0
+Version: 1.4.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.3.0/README.md` & `hydra-genetics-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/__init__.py` & `hydra-genetics-1.4.0/hydra_genetics/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/__main__.py` & `hydra-genetics-1.4.0/hydra_genetics/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,16 +257,16 @@
                        sample_regex, read_number_regex, adapters, tc, force, default_barcode, validate, ask, th, nreads, every):
     input_files = CreateInputFiles(directory, outdir, post_file_modifier, platform, sample_type,
                                    sample_regex, read_number_regex, adapters, tc, force, default_barcode, validate, ask, th,
                                    nreads, every)
     input_files.init()
 
 
-@cli.command(short_help="download reference data")
-def referece_data():
-    pass
+#  @cli.command(short_help="download reference data")
+#  def referece_data():
+#    pass
 
 
 cli.add_command(environment)
 
 if __name__ == "__main__":
     run()
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/commands/create.py` & `hydra-genetics-1.4.0/hydra_genetics/commands/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         if not self.no_git:
             self.git_init_pipeline()
 
     def git_init_pipeline(self):
         """Initialises the new pipeline as a Git repository and submits first commit."""
         log.info("Initialising pipeline git repository")
-        repo = git.Repo.init(self.outdir)
+        repo = git.Repo.init(self.outdir, initial_branch='main')
         repo.git.add(A=True)
         repo.index.commit(f"initial template build from hydra-genetics/tools, version {hydra_genetics.__version__}")
         # Add TEMPLATE branch to git repository
         repo.git.branch("develop")
         log.info(
             "Done. Remember to add a remote and push to GitHub:\n"
             f"[white on grey23] cd {self.outdir} \n"
@@ -326,15 +326,15 @@
     def __init__(self,
                  directory,
                  outdir=None,
                  post_file_modifier=None,
                  platform="Illumina",
                  sample_type="T",
                  sample_regex=r"^([A-Za-z0-9-]+)_.*\.fastq.gz",
-                 read_number_regex="_(R[12]{1})_",
+                 read_number_regex="_(R[12]{1})[_.]{1}",
                  adapters="AGATCGGAAGAGCACACGTCTGAACTCCAGTCA,AGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGT",
                  tc=1.0,
                  force=False,
                  default_barcode=None,
                  validate_run_information=False,
                  ask_for_input=False,
                  occurrences_warning_th=0.9,
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/commands/prep_pipeline_env.py` & `hydra-genetics-1.4.0/hydra_genetics/commands/prep_pipeline_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import yaml
 
 
 def create_docker_file_path(storage_path, container):
     return os.path.join(storage_path, container.replace('docker://', '').replace("/", "_").replace(":", "_") + ".sif")
 
 
-@click.group("prepare-environment", short_help="prepare for singularty environment")
+@click.group("prepare-environment", short_help="prepare for singularity environment")
 def environment():
     pass
 
 
 @environment.command(short_help="update config with path to container cache")
 @click.option(
     "-c",
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -42,8 +42,8 @@
           mamba install -c conda-forge -c bioconda singularity=3.8.6
       - name: Add conda to system path
         run: |
           echo $CONDA/bin >> $GITHUB_PATH
       - name: Integration test - small dataset
         working-directory: .tests/integration
         run: |
-          snakemake -s ../../workflow/Snakefile -j 1 --show-failed-logs --configfile config.yaml  --use-singularity --singularity-args  " --cleanenv --bind /home/runner "
+          snakemake -s ../../workflow/Snakefile -j 1 --show-failed-logs --configfile config/config.yaml  --use-singularity --singularity-args  " --cleanenv --bind /home/runner "
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/LICENSE.md` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/README.md` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/extra.css` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/extra.css`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/docs/index.md` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/images/hydragenetics.png` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/images/hydragenetics.png`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/mkdocs.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/rules/common.smk` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/rules/common.smk`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 f'@workflow.shellcmd("{copy_container}")',
                 "@workflow.run\n",
                 f"def __rule_{rule_name}(input, output, params, wildcards, threads, resources, "
                 "log, version, rule, conda_env, container_img, singularity_args, use_singularity, "
                 "env_modules, bench_record, jobid, is_shell, bench_iteration, cleanup_scripts, "
                 "shadow_dir, edit_notebook, conda_base_path, basedir, runtime_sourcecache_path, "
                 "__is_snakemake_rule_func=True):",
-                '\tshell("(cp {input[0]} {output[0]}) &> {log}", bench_record=bench_record, '
+                '\tshell("(cp --preserve=timestamps {input[0]} {output[0]}) &> {log}", bench_record=bench_record, '
                 "bench_iteration=bench_iteration)\n\n",
             ]
         )
 
         rulestrings.append(rule_code)
 
     exec(compile("\n".join(rulestrings), "copy_result_files", "exec"), workflow.globals)
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 $schema: "http://json-schema.org/draft-04/schema#"
 description: snakemake configuration file
 type: object
 properties:
   default_resources:
     type: object
     properties:
-      threads:
-        type: integer
-        description: default number of threads that will be used by a rule
-      time:
-        type: string
-        description: default max execution time for a rule
       mem_mb:
         type: integer
         description: default memory used for a rule
       mem_per_cpu:
         type: integer
         description: default memory used per cpu for a rule
       partition:
         type: string
         description: default partition to use on the cluser for a rule
-
+      threads:
+        type: integer
+        description: default number of threads that will be used by a rule
+      time:
+        type: string
+        description: default max execution time for a rule
 required:
   - default_resources
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/rule-template/config.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/rule-template/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/rule-template/resources.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/rule-template/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/rule-template/rules.schema.yaml` & `hydra-genetics-1.4.0/hydra_genetics/rule-template/rules.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/rule-template/skeleton_rule.smk` & `hydra-genetics-1.4.0/hydra_genetics/rule-template/skeleton_rule.smk`

 * *Files 8% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         mem_per_cpu=config.get("{{ name }}", {}).get("mem_per_cpu", config["default_resources"]["mem_per_cpu"]),
         partition=config.get("{{ name }}", {}).get("partition", config["default_resources"]["partition"]),
         threads=config.get("{{ name }}", {}).get("threads", config["default_resources"]["threads"]),
         time=config.get("{{ name }}", {}).get("time", config["default_resources"]["time"]),
     container:
         config.get("{{ name }}", {}).get("container", config["default_container"])
     message:
-        "{rule}: Do stuff on {{ module_name }}/{rule}/{wildcards.sample}_{wildcards.type}.input"
+        "{rule}: do stuff on {input.input1}"
     wrapper:
         "..."
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/io/chr.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/io/chr.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/io/hotspot.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/io/hotspot_report.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/io/hotspot_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/io/multibp.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/io/multibp.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/io/utils.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/io/utils.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/misc.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/models/hotspot.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/models/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/samples.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/hydra_genetics/utils/units.py` & `hydra-genetics-1.4.0/hydra_genetics/utils/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         wildcards: wildcards object with at least the following wildcard names
                sample, type, flowcell, and lane
     Returns:
         Series containing data of the selected row
     Raises:
         raises an exception (KeyError) if no unit can be extracted from the Dataframe
     """
-    unit = units.loc[(wildcards.sample, wildcards.type, wildcards.flowcell, wildcards.lane, wildcards.barcode)].dropna()
+    unit = units.loc[(wildcards.sample, wildcards.type, wildcards.flowcell, wildcards.lane, wildcards.barcode)]
     return unit
 
 
 def get_fastq_file(units: pandas.DataFrame, wildcards: snakemake.io.Wildcards, read_pair: str = "fastq1") -> str:
     """
     function used to extract path for one unit(row) from units.tsv
     Args:
@@ -72,15 +72,15 @@
     Raises:
         raises an exception (KeyError) if no unit can be extracted from the Dataframe
     """
     return set([u.barcode for u in units.loc[
         (units['sample'] == wildcards.sample) &
         (units['flowcell'] == wildcards.flowcell) &
         (units['type'] == wildcards.type),
-    ].dropna().itertuples()])
+    ].itertuples()])
 
 
 def get_unit_machine(units: pandas.DataFrame, wildcards: snakemake.io.Wildcards) -> str:
     """
     function used to extract machine for one unit(row) from units.tsv
     Args:
         units: DataFrame generate by importing a file following schema defintion
@@ -142,17 +142,17 @@
     Returns:
         all units from the DataFrame that can be filtereted out using sample name
         and unit type (N,T,R)
     Raises:
         raises an exception (KeyError) if no unit(s) can be extracted from the Dataframe
     """
     if type is None:
-        files = units.loc[(wildcards.sample, wildcards.type)].dropna()
+        files = units.loc[(wildcards.sample, wildcards.type)]
     else:
-        files = units.loc[(wildcards.sample, type)].dropna()
+        files = units.loc[(wildcards.sample, type)]
     if isinstance(files, pandas.Series):
         files = pandas.DataFrame(
             [[f[1] for f in files.items()], ], columns=[f[0] for f in files.items()]
         ).set_index(units.index.names)
     return [file for file in files.itertuples()]
 
 
@@ -183,15 +183,15 @@
         wildcards: wildcards object with at least the following wildcard names
                sample, type.
     Returns:
         set of string
     Raises:
         raises an exception (KeyError) if no unit(s) can be extracted from the Dataframe
     """
-    return set([u.platform for u in units.loc[(wildcards.sample, wildcards.type)].dropna().itertuples()])
+    return set([u.platform for u in units.loc[(wildcards.sample, wildcards.type)].itertuples()])
 
 
 def get_unit_types(units: pandas.DataFrame, sample: str) -> set:
     """
     function used to extract all types of units found for a sample in units.tsv (N,T,R)
     Args:
         units: DataFrame generate by importing a file following schema defintion
@@ -199,15 +199,15 @@
         wildcards: wildcards object with at least the following wildcard names
                sample.
     Returns:
         set of type types ex set("N","T")
     Raises:
         raises an exception (KeyError) if no unit(s) can be extracted from the Dataframe
     """
-    return set([u.type for u in units.loc[(sample,)].dropna().itertuples()])
+    return set([u.type for u in units.loc[(sample,)].itertuples()])
 
 
 def get_units_per_flowcell(units: pandas.DataFrame, wildcards: snakemake.io.Wildcards):
     """
     function used to extract all sample and type combinations for one sequencing flowcell
     Args:
         units: DataFrame generate by importing a file following schema defintion
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics.egg-info/PKG-INFO` & `hydra-genetics-1.4.0/hydra_genetics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.3.0
+Version: 1.4.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.3.0/hydra_genetics.egg-info/SOURCES.txt` & `hydra-genetics-1.4.0/hydra_genetics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,21 @@
 hydra_genetics/pipeline-template/.github/workflows/integration.yaml
 hydra_genetics/pipeline-template/.github/workflows/lint.yaml
 hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
 hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
 hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
 hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
 hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
-hydra_genetics/pipeline-template/.tests/integration/config.yaml
-hydra_genetics/pipeline-template/.tests/integration/resources.yaml
 hydra_genetics/pipeline-template/.tests/integration/samples.tsv
 hydra_genetics/pipeline-template/.tests/integration/units.tsv
+hydra_genetics/pipeline-template/.tests/integration/config/config.yaml
+hydra_genetics/pipeline-template/.tests/integration/config/output_files.yaml
+hydra_genetics/pipeline-template/.tests/integration/config/resources.yaml
 hydra_genetics/pipeline-template/config/config.yaml
-hydra_genetics/pipeline-template/config/output_files.json
+hydra_genetics/pipeline-template/config/output_files.yaml
 hydra_genetics/pipeline-template/config/resources.yaml
 hydra_genetics/pipeline-template/config/samples.tsv
 hydra_genetics/pipeline-template/config/units.tsv
 hydra_genetics/pipeline-template/docs/extra.css
 hydra_genetics/pipeline-template/docs/index.md
 hydra_genetics/pipeline-template/docs/intro.md
 hydra_genetics/pipeline-template/docs/requirements.txt
```

### Comparing `hydra-genetics-1.3.0/setup.py` & `hydra-genetics-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/io/test_hotspot.py` & `hydra-genetics-1.4.0/tests/utils/io/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/io/test_mutations_report.py` & `hydra-genetics-1.4.0/tests/utils/io/test_mutations_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/models/test_hotspot.py` & `hydra-genetics-1.4.0/tests/utils/models/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/test_misc.py` & `hydra-genetics-1.4.0/tests/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/test_resources.py` & `hydra-genetics-1.4.0/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/test_samples.py` & `hydra-genetics-1.4.0/tests/utils/test_samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/tests/utils/test_units.py` & `hydra-genetics-1.4.0/tests/utils/test_units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.3.0/versioneer.py` & `hydra-genetics-1.4.0/versioneer.py`

 * *Files identical despite different names*

