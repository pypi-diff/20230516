# Comparing `tmp/salt-analytics-framework-0.1.1.tar.gz` & `tmp/salt-analytics-framework-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May 15 13:23:45 2023, max compression
+gzip compressed data, last modified: Tue May 16 17:23:19 2023, max compression
```

## Comparing `salt-analytics-framework-0.1.1.tar` & `salt-analytics-framework-0.2.0.tar`

### file list

```diff
@@ -1,159 +1,154 @@
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.bandit
--rw-r--r--   0 root         (0) root         (0)      684 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.coveragerc
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actionlint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actions/setup-actionlint/
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/actions/setup-actionlint/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)    10391 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3571 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)      967 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2487 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/changelog/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/changelog/_template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6553 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.collect.rst
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.forward.rst
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.process.rst
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.rst
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.saltext.engines.rst
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.saltext.rst
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/ref/saf.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    20016 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     4759 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/requirements/tools.txt
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/
--rw-r--r--   0 root         (0) root         (0)      914 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/beacons.py
--rw-r--r--   0 root         (0) root         (0)     5240 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/logs.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/noop.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/collect/salt_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1560 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/disk.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/noop.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/forward/test.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/manager.py
--rw-r--r--   0 root         (0) root         (0)    10262 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/models.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/noop.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/regex_mask.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/regex_mask.pyi
--rw-r--r--   0 root         (0) root         (0)     4442 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/process/shannon_mask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/saltext/engines/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/dt.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/utils/eventbus.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/saf/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3614 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      586 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1350 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/forwarders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/forwarders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/forwarders/test_concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/test_disabled_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/functional/manager/test_enabled_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_memusage.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/test_logs.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/logs/test_logs_with_parse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_arg.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_collatz.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_config_get.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/integration/engines/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/test_regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     5436 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/process/test_shannon_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tests/unit/salt/engines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/.ruff.toml
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5495 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/ci.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/pre_commit.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-05-15 13:23:45.000000 salt-analytics-framework-0.1.1/tools/pre_commit.py~
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.bandit
+-rw-r--r--   0 root         (0) root         (0)      684 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actionlint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)    10391 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      549 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/changelog/_template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.collect.rst
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.forward.rst
+-rw-r--r--   0 root         (0) root         (0)      603 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.process.rst
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.rst
+-rw-r--r--   0 root         (0) root         (0)      346 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.saltext.engines.rst
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/ref/saf.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    20016 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/requirements/tools.txt
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/beacons.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/file.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/collect/salt_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/disk.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/noop.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/forward/test.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/manager.py
+-rw-r--r--   0 root         (0) root         (0)    10262 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/models.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/noop.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/regex_mask.pyi
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/process/shannon_mask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/saltext/engines/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/dt.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/utils/eventbus.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/saf/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      586 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/forwarders/test_concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/test_disabled_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/functional/manager/test_enabled_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_memusage.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_collatz.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_config_get.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/integration/engines/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/test_regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/process/test_shannon_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tests/unit/salt/engines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/.ruff.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/ci.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/pre_commit.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-05-16 17:23:19.000000 salt-analytics-framework-0.2.0/tools/pre_commit.py~
```

### Comparing `salt-analytics-framework-0.1.1/.coveragerc` & `salt-analytics-framework-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.github/actions/setup-actionlint/action.yml` & `salt-analytics-framework-0.2.0/.github/actions/setup-actionlint/action.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.github/workflows/ci.yml` & `salt-analytics-framework-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.gitignore` & `salt-analytics-framework-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pre-commit-config.yaml` & `salt-analytics-framework-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pre-commit-hooks/check-changelog-entries.py` & `salt-analytics-framework-0.2.0/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pre-commit-hooks/check-cli-examples.py` & `salt-analytics-framework-0.2.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pre-commit-hooks/copyright-headers.py` & `salt-analytics-framework-0.2.0/.pre-commit-hooks/copyright-headers.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pre-commit-hooks/make-autodocs.py` & `salt-analytics-framework-0.2.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pre-commit-hooks/sort-pylint-spelling-words.py` & `salt-analytics-framework-0.2.0/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/.pylint-spelling-words` & `salt-analytics-framework-0.2.0/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/CHANGELOG.rst` & `salt-analytics-framework-0.2.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,36 @@
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
 
+0.2.0 (2023-05-16)
+==================
+
+Improvements
+------------
+
+- `#31 <https://github.com/saltstack/pytest-skip-markers/issues/31>`_: Refactored the logs collector into a generic file collector
+
+- `#33 <https://github.com/saltstack/pytest-skip-markers/issues/33>`_: If a processor decides not to return the passed event, no attempts to run the next processor on it or just forward it should be made
+
+- `#34 <https://github.com/saltstack/pytest-skip-markers/issues/34>`_: Log the traceback on the first time a pipeline run raises an exception
+
+- `#37 <https://github.com/saltstack/pytest-skip-markers/issues/37>`_: Processors can now return 1 or more events, they'll all get forwarded
+
+
+
+Bug Fixes
+---------
+
+- `#32 <https://github.com/saltstack/pytest-skip-markers/issues/32>`_: If one of the processors raises an exception, stop processing the event
+
+
 0.1.1 (2023-05-15)
 ==================
 
 Improvements
 ------------
 
 - `#30 <https://github.com/saltstack/pytest-skip-markers/issues/30>`_: The `CollectedEvent.data` type is now `Mapping` instead of `Dict`. This allows to use `TypedDict`'s for that attribute.
```

### Comparing `salt-analytics-framework-0.1.1/CODE_OF_CONDUCT.md` & `salt-analytics-framework-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/CONTRIBUTING.md` & `salt-analytics-framework-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/LICENSE` & `salt-analytics-framework-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/NOTICE` & `salt-analytics-framework-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/PKG-INFO` & `salt-analytics-framework-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.1.1
+Version: 0.2.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.1.1/README.rst` & `salt-analytics-framework-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/changelog/_template.rst` & `salt-analytics-framework-0.2.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/Makefile` & `salt-analytics-framework-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/conf.py` & `salt-analytics-framework-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/index.rst` & `salt-analytics-framework-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/make.bat` & `salt-analytics-framework-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/ref/saf.collect.rst` & `salt-analytics-framework-0.2.0/docs/ref/saf.collect.rst`

 * *Files 15% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 --------------------------
 
 .. automodule:: saf.collect.beacons
    :members:
    :undoc-members:
    :show-inheritance:
 
-saf.collect.logs module
+saf.collect.file module
 -----------------------
 
-.. automodule:: saf.collect.logs
+.. automodule:: saf.collect.file
    :members:
    :undoc-members:
    :show-inheritance:
 
 saf.collect.noop module
 -----------------------
```

### Comparing `salt-analytics-framework-0.1.1/docs/ref/saf.forward.rst` & `salt-analytics-framework-0.2.0/docs/ref/saf.forward.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/ref/saf.process.rst` & `salt-analytics-framework-0.2.0/docs/ref/saf.process.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/docs/ref/saf.rst` & `salt-analytics-framework-0.2.0/docs/ref/saf.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/noxfile.py` & `salt-analytics-framework-0.2.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/pyproject.toml` & `salt-analytics-framework-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -171,7 +171,13 @@
 [tool.ruff.pep8-naming]
 ignore-names = [
   "__virtual__",
 ]
 [tool.ruff.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
+
+[tool.ruff.mccabe]
+max-complexity = 20
+
+[tool.ruff.pylint]
+max-branches = 25
```

### Comparing `salt-analytics-framework-0.1.1/setup.cfg` & `salt-analytics-framework-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 saf = py.typed
 
 [options.entry_points]
 salt.loader = 
 	salt-analytics-framework = saf.saltext
 saf.collect = 
 	noop = saf.collect.noop
-	logs = saf.collect.logs
+	file = saf.collect.file
 	beacons = saf.collect.beacons
 	salt_exec = saf.collect.salt_exec
 saf.process = 
 	noop = saf.process.noop
 	regex_mask = saf.process.regex_mask
 	shannon_mask = saf.process.shannon_mask
 saf.forward =
```

### Comparing `salt-analytics-framework-0.1.1/src/saf/__init__.py` & `salt-analytics-framework-0.2.0/src/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/collect/beacons.py` & `salt-analytics-framework-0.2.0/src/saf/collect/beacons.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/collect/noop.py` & `salt-analytics-framework-0.2.0/src/saf/collect/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/collect/salt_exec.py` & `salt-analytics-framework-0.2.0/src/saf/collect/salt_exec.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/forward/disk.py` & `salt-analytics-framework-0.2.0/src/saf/forward/disk.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/forward/noop.py` & `salt-analytics-framework-0.2.0/src/saf/forward/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/forward/test.py` & `salt-analytics-framework-0.2.0/src/saf/forward/test.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/manager.py` & `salt-analytics-framework-0.2.0/src/saf/manager.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/models.py` & `salt-analytics-framework-0.2.0/src/saf/models.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/plugins.py` & `salt-analytics-framework-0.2.0/src/saf/plugins.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/process/noop.py` & `salt-analytics-framework-0.2.0/src/saf/process/noop.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 The NOOP process plugins exists as an implementation example.
 
 It doesn't really do anything to the collected event
 """
 from __future__ import annotations
 
 import logging
+from typing import AsyncIterator
 from typing import Type
 
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
 from saf.models import ProcessConfigBase
 
 log = logging.getLogger(__name__)
@@ -24,13 +25,13 @@
     return ProcessConfigBase
 
 
 async def process(
     *,
     ctx: PipelineRunContext[ProcessConfigBase],  # noqa: ARG001
     event: CollectedEvent,
-) -> CollectedEvent:
+) -> AsyncIterator[CollectedEvent]:
     """
     Method called to process the event.
     """
     log.info("Processing: %s", event)
-    return event
+    yield event
```

### Comparing `salt-analytics-framework-0.1.1/src/saf/process/regex_mask.py` & `salt-analytics-framework-0.2.0/src/saf/process/regex_mask.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 from __future__ import annotations
 
 import functools
 import logging
 import re
 from typing import Any
+from typing import AsyncIterator
 from typing import Dict
 from typing import Match
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 from pydantic import Field
@@ -93,16 +94,16 @@
     return obj
 
 
 async def process(
     *,
     ctx: PipelineRunContext[RegexMaskProcessConfig],
     event: CollectedEvent,
-) -> CollectedEvent:
+) -> AsyncIterator[CollectedEvent]:
     """
     Method called to mask the data based on provided regex rules.
     """
     config = ctx.config
     log.info("Processing event in regex_mask: %s", event.json())
     event_dict = event.dict()
     processed_event_dict = _regex_process(event_dict, config)
-    return event.parse_obj(processed_event_dict)
+    yield event.parse_obj(processed_event_dict)
```

### Comparing `salt-analytics-framework-0.1.1/src/saf/process/regex_mask.pyi` & `salt-analytics-framework-0.2.0/src/saf/process/regex_mask.pyi`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/process/shannon_mask.py` & `salt-analytics-framework-0.2.0/src/saf/process/shannon_mask.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 from __future__ import annotations
 
 import logging
 import math
 import string
 from typing import Any
+from typing import AsyncIterator
 from typing import Optional
 from typing import Type
 
 from pydantic import Field
 
 from saf.models import CollectedEvent
 from saf.models import PipelineRunContext
@@ -115,16 +116,16 @@
     return obj
 
 
 async def process(
     *,
     ctx: PipelineRunContext[ShannonMaskProcessConfig],
     event: CollectedEvent,
-) -> CollectedEvent:
+) -> AsyncIterator[CollectedEvent]:
     """
     Method called to mask the data based on normalized Shannon index values.
     """
     config = ctx.config
     log.info("Processing event in shannon_mask: %s", event.json())
     event_dict = event.dict()
     processed_event_dict = _shannon_process(event_dict, config)
-    return event.parse_obj(processed_event_dict)
+    yield event.parse_obj(processed_event_dict)
```

### Comparing `salt-analytics-framework-0.1.1/src/saf/saltext/engines/analytics.py` & `salt-analytics-framework-0.2.0/src/saf/saltext/engines/analytics.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/src/saf/utils/eventbus.py` & `salt-analytics-framework-0.2.0/src/saf/utils/eventbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         )
         log.debug("Constructed SaltEvent: %s", salt_event)
     except Exception:
         log.exception("Failed to construct a SaltEvent")
     return salt_event
 
 
-def _process_events(  # noqa: C901
+def _process_events(
     opts: dict[str, Any],
     events_queue: Queue[SaltEvent],
     tags: set[str],
 ) -> None:
     """
     Collect events from Salt's event bus.
```

### Comparing `salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/PKG-INFO` & `salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.1.1
+Version: 0.2.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
```

### Comparing `salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/SOURCES.txt` & `salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 src/saf/models.py
 src/saf/pipeline.py
 src/saf/plugins.py
 src/saf/py.typed
 src/saf/version.py
 src/saf/collect/__init__.py
 src/saf/collect/beacons.py
-src/saf/collect/logs.py
+src/saf/collect/file.py
 src/saf/collect/noop.py
 src/saf/collect/salt_exec.py
 src/saf/forward/__init__.py
 src/saf/forward/disk.py
 src/saf/forward/noop.py
 src/saf/forward/test.py
 src/saf/process/__init__.py
@@ -96,18 +96,14 @@
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/collectors/__init__.py
 tests/integration/collectors/beacons/__init__.py
 tests/integration/collectors/beacons/test_memusage.py
 tests/integration/collectors/beacons/test_multiple.py
 tests/integration/collectors/beacons/test_status.py
-tests/integration/collectors/logs/__init__.py
-tests/integration/collectors/logs/conftest.py
-tests/integration/collectors/logs/test_logs.py
-tests/integration/collectors/logs/test_logs_with_parse.py
 tests/integration/collectors/salt_exec/__init__.py
 tests/integration/collectors/salt_exec/conftest.py
 tests/integration/collectors/salt_exec/test_arg.py
 tests/integration/collectors/salt_exec/test_collatz.py
 tests/integration/collectors/salt_exec/test_config_get.py
 tests/integration/engines/__init__.py
 tests/integration/engines/test_engine.py
```

### Comparing `salt-analytics-framework-0.1.1/src/salt_analytics_framework.egg-info/requires.txt` & `salt-analytics-framework-0.2.0/src/salt_analytics_framework.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/__init__.py` & `salt-analytics-framework-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/conftest.py` & `salt-analytics-framework-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/functional/conftest.py` & `salt-analytics-framework-0.2.0/tests/functional/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING
 from typing import Any
+from typing import AsyncIterator
 
 import pytest
 import pytest_asyncio
 
 from saf.manager import Manager
 from saf.models import AnalyticsConfig
 
-if TYPE_CHECKING:
-    try:
-        from typing import AsyncGenerator
-    except ImportError:
-        from typing import AsyncGenerator
-
 try:
     asyncio_fixture = pytest_asyncio.fixture
 except AttributeError:
     # On Py3.6 and older version of the pytest gets installed which does not
     # have the `.fixture` function.
     # Fallback to `pytest.fixture`.
     asyncio_fixture = pytest.fixture
@@ -39,15 +33,15 @@
 
 @pytest.fixture
 def analytics_config(analytics_config_dict: dict[str, Any]):
     return AnalyticsConfig.parse_obj(analytics_config_dict)
 
 
 @asyncio_fixture
-async def manager(analytics_config: AnalyticsConfig) -> AsyncGenerator[Manager, None]:
+async def manager(analytics_config: AnalyticsConfig) -> AsyncIterator[Manager]:
     _manager = Manager(analytics_config)
     loop = asyncio.get_event_loop()
     task = loop.create_task(_run_manager(_manager))
     try:
         yield _manager
     finally:
         if not task.done():
```

### Comparing `salt-analytics-framework-0.1.1/tests/functional/forwarders/test_concurrency.py` & `salt-analytics-framework-0.2.0/tests/functional/forwarders/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/functional/manager/conftest.py` & `salt-analytics-framework-0.2.0/tests/functional/manager/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/functional/manager/test_disabled_pipeline.py` & `salt-analytics-framework-0.2.0/tests/functional/manager/test_disabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/functional/manager/test_enabled_pipeline.py` & `salt-analytics-framework-0.2.0/tests/functional/manager/test_enabled_pipeline.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_memusage.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_memusage.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_multiple.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_multiple.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/beacons/test_status.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/beacons/test_status.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/logs/conftest.py` & `salt-analytics-framework-0.2.0/tests/integration/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from __future__ import annotations
 
+import pathlib
 import shutil
+from typing import Iterator
 
 import pytest
+from saltfactories.cli.run import SaltRun
+from saltfactories.cli.salt import SaltCli
 from saltfactories.daemons.master import SaltMaster
-from saltfactories.daemons.minion import SaltMinion
 from saltfactories.utils import random_string
 
 
-@pytest.fixture(scope="module")
-def temp_logs_dir(tmp_path_factory):
-    tmp_dir = tmp_path_factory.mktemp("logs")
-    yield tmp_dir
-    shutil.rmtree(tmp_dir)
-
-
-@pytest.fixture(scope="module", autouse=True)
-def minion(
-    master: SaltMaster, analytics_events_dump_directory, analytics_config_contents
-) -> SaltMinion:
-    default_config = {
-        "engines": ["analytics"],
-    }
-    factory = master.salt_minion_daemon(random_string("minion-"), defaults=default_config)
-    with pytest.helpers.temp_file(
-        "analytics", contents=analytics_config_contents, directory=factory.config_dir
-    ):
-        with factory.started():
-            yield factory
+@pytest.fixture(scope="package")
+def analytics_events_dump_directory(tmp_path_factory) -> Iterator[pathlib.Path]:
+    dump_path = tmp_path_factory.mktemp("analytics-events-dump")
+    try:
+        yield dump_path
+    finally:
+        shutil.rmtree(str(dump_path), ignore_errors=True)
+
+
+@pytest.fixture(autouse=True)
+def cleanup_analytics_events_dump_directory(
+    analytics_events_dump_directory: pathlib.Path,
+) -> Iterator[pathlib.Path]:
+    try:
+        yield analytics_events_dump_directory
+    finally:
+        for path in analytics_events_dump_directory.iterdir():
+            path.unlink()
+
+
+@pytest.fixture(scope="package")
+def master(salt_factories, analytics_events_dump_directory) -> SaltMaster:
+    factory = salt_factories.salt_master_daemon(random_string("master-"))
+    with factory.started():
+        yield factory
+
+
+@pytest.fixture
+def salt_run_cli(master: SaltMaster) -> SaltRun:
+    return master.get_salt_run_cli()
+
+
+@pytest.fixture
+def salt_cli(master: SaltMaster) -> SaltCli:
+    return master.get_salt_cli()
```

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/conftest.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_arg.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_arg.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_collatz.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_collatz.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/collectors/salt_exec/test_config_get.py` & `salt-analytics-framework-0.2.0/tests/integration/collectors/salt_exec/test_config_get.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/integration/conftest.py` & `salt-analytics-framework-0.2.0/tests/integration/engines/test_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 from __future__ import annotations
 
-import pathlib
-import shutil
-from typing import Iterator
+import time
 
 import pytest
-from saltfactories.cli.run import SaltRun
-from saltfactories.cli.salt import SaltCli
 from saltfactories.daemons.master import SaltMaster
+from saltfactories.daemons.minion import SaltMinion
 from saltfactories.utils import random_string
 
 
-@pytest.fixture(scope="package")
-def analytics_events_dump_directory(tmp_path_factory) -> Iterator[pathlib.Path]:
-    dump_path = tmp_path_factory.mktemp("analytics-events-dump")
-    try:
-        yield dump_path
-    finally:
-        shutil.rmtree(str(dump_path), ignore_errors=True)
-
-
-@pytest.fixture(autouse=True)
-def cleanup_analytics_events_dump_directory(
-    analytics_events_dump_directory: pathlib.Path,
-) -> Iterator[pathlib.Path]:
-    try:
-        yield analytics_events_dump_directory
-    finally:
-        for path in analytics_events_dump_directory.iterdir():
-            path.unlink()
-
-
-@pytest.fixture(scope="package")
-def master(salt_factories, analytics_events_dump_directory) -> SaltMaster:
-    factory = salt_factories.salt_master_daemon(random_string("master-"))
-    with factory.started():
-        yield factory
-
-
-@pytest.fixture
-def salt_run_cli(master: SaltMaster) -> SaltRun:
-    return master.get_salt_run_cli()
-
-
-@pytest.fixture
-def salt_cli(master: SaltMaster) -> SaltCli:
-    return master.get_salt_cli()
+@pytest.fixture(scope="module", autouse=True)
+def minion(master: SaltMaster, analytics_events_dump_directory) -> SaltMinion:
+    default_config = {
+        "engines": ["analytics"],
+    }
+    factory = master.salt_minion_daemon(random_string("minion-"), defaults=default_config)
+    analytics_config = """
+    collectors:
+      noop-collector:
+        plugin: noop
+        interval: 1
+
+    processors:
+      noop-processor:
+        plugin: noop
+
+
+    forwarders:
+      disk-forwarder:
+        plugin: disk
+        path: {}
+
+
+    pipelines:
+      my-pipeline:
+        collect: noop-collector
+        process: noop-processor
+        forward: disk-forwarder
+    """.format(
+        analytics_events_dump_directory
+    )
+    with pytest.helpers.temp_file(
+        "analytics", contents=analytics_config, directory=factory.config_dir
+    ):
+        with factory.started():
+            yield factory
+
+
+def test_events_dumped_to_disk(analytics_events_dump_directory):
+    timeout = 10
+    while timeout:
+        time.sleep(1)
+        timeout -= 1
+        if len(list(analytics_events_dump_directory.iterdir())) > 3:
+            break
+    else:
+        pytest.fail(f"Failed to find dumped events in {analytics_events_dump_directory}")
```

### Comparing `salt-analytics-framework-0.1.1/tests/unit/process/test_regex_mask.py` & `salt-analytics-framework-0.2.0/tests/unit/process/test_regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tests/unit/process/test_shannon_mask.py` & `salt-analytics-framework-0.2.0/tests/unit/process/test_shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tools/ci.py` & `salt-analytics-framework-0.2.0/tools/ci.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tools/pre_commit.py` & `salt-analytics-framework-0.2.0/tools/pre_commit.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.1.1/tools/pre_commit.py~` & `salt-analytics-framework-0.2.0/tools/pre_commit.py~`

 * *Files identical despite different names*

