# Comparing `tmp/TMD-2.3.0.tar.gz` & `tmp/TMD-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMD-2.3.0.tar", last modified: Fri Apr 28 11:43:56 2023, max compression
+gzip compressed data, was "TMD-2.3.1.tar", last modified: Tue May 16 08:59:57 2023, max compression
```

## Comparing `TMD-2.3.0.tar` & `TMD-2.3.1.tar`

### file list

```diff
@@ -1,142 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 11:43:44.000000 TMD-2.3.0/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-28 11:43:44.000000 TMD-2.3.0/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:44.000000 TMD-2.3.0/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 11:43:44.000000 TMD-2.3.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-28 11:43:44.000000 TMD-2.3.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 11:43:44.000000 TMD-2.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 11:43:44.000000 TMD-2.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-28 11:43:44.000000 TMD-2.3.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 11:43:44.000000 TMD-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-28 11:43:44.000000 TMD-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-28 11:43:44.000000 TMD-2.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-28 11:43:44.000000 TMD-2.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 11:43:44.000000 TMD-2.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-28 11:43:44.000000 TMD-2.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-28 11:43:44.000000 TMD-2.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-28 11:43:44.000000 TMD-2.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-28 11:43:44.000000 TMD-2.3.0/COPYRIGHT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-28 11:43:44.000000 TMD-2.3.0/LICENSE-BSD.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-28 11:43:44.000000 TMD-2.3.0/LICENSE-LGPL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 11:43:44.000000 TMD-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-28 11:43:56.051457 TMD-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-28 11:43:44.000000 TMD-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/TMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 11:43:56.000000 TMD-2.3.0/TMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 11:43:55.000000 TMD-2.3.0/TMD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-28 11:43:44.000000 TMD-2.3.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 11:43:44.000000 TMD-2.3.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.031457 TMD-2.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.035457 TMD-2.3.0/examples/Advanced/
--rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/advanced_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/diversity_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/polar_plot_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/time_series_tmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20425 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/Advanced/variability.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/distances_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/extract_ph.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:43:44.000000 TMD-2.3.0/examples/write_swc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 11:43:44.000000 TMD-2.3.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 11:43:44.000000 TMD-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:43:56.051457 TMD-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-28 11:43:44.000000 TMD-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.039457 TMD-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic.swc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_exotic_section_types.swc
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_no_comments.swc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_no_sec_ids.swc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/basic_options.swc
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/neuron.swc
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/neuron_ph_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/neuron_ph_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample.swc
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_disordered.swc
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_disordered_v1.h5
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_ph_0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_ph_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_v0.h5
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_v1.h5
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/sample_v2.h5
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/test_morph.swc
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/test_morph_v1.h5
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/test_morph_v2.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tests/data/valid/
--rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/C010398B-P2.CNG.swc
--rwxr-xr-x   0 runner    (1001) docker     (123)    33168 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/C010398B-P2.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/sample.swc
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/sample_v1.h5
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/data/valid/sample_v2.h5
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_neuron.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_neuron_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_neuron_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_soma.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_soma_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_swc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_topology_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_topology_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_topology_persistent_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 11:43:44.000000 TMD-2.3.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Neuron/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Neuron/Neuron.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Neuron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Neuron/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Population/
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Population/Population.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Population/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Soma/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Soma/Soma.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Soma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Soma/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.043457 TMD-2.3.0/tmd/Topology/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/persistent_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Topology/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/tmd/Tree/
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Tree/Tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/Tree/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/tmd/io/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/io/swc.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:43:56.051457 TMD-2.3.0/tmd/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    40938 2023-04-28 11:43:44.000000 TMD-2.3.0/tmd/view/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-28 11:43:44.000000 TMD-2.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.553034 TMD-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-16 08:59:45.000000 TMD-2.3.1/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-16 08:59:45.000000 TMD-2.3.1/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:45.000000 TMD-2.3.1/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 08:59:45.000000 TMD-2.3.1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-16 08:59:45.000000 TMD-2.3.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 08:59:45.000000 TMD-2.3.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-16 08:59:45.000000 TMD-2.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.537033 TMD-2.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-16 08:59:45.000000 TMD-2.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.537033 TMD-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-16 08:59:45.000000 TMD-2.3.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-16 08:59:45.000000 TMD-2.3.1/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-16 08:59:45.000000 TMD-2.3.1/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-16 08:59:45.000000 TMD-2.3.1/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 08:59:45.000000 TMD-2.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-16 08:59:45.000000 TMD-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-16 08:59:45.000000 TMD-2.3.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-16 08:59:45.000000 TMD-2.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 08:59:45.000000 TMD-2.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17436 2023-05-16 08:59:45.000000 TMD-2.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 08:59:45.000000 TMD-2.3.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-16 08:59:45.000000 TMD-2.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 08:59:45.000000 TMD-2.3.1/COPYRIGHT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-16 08:59:45.000000 TMD-2.3.1/LICENSE-BSD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-16 08:59:45.000000 TMD-2.3.1/LICENSE-LGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 08:59:45.000000 TMD-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 08:59:57.553034 TMD-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-16 08:59:45.000000 TMD-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.537033 TMD-2.3.1/TMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 08:59:57.000000 TMD-2.3.1/TMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-16 08:59:57.000000 TMD-2.3.1/TMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:59:57.000000 TMD-2.3.1/TMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 08:59:57.000000 TMD-2.3.1/TMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 08:59:57.000000 TMD-2.3.1/TMD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-16 08:59:45.000000 TMD-2.3.1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.537033 TMD-2.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 08:59:45.000000 TMD-2.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.537033 TMD-2.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-16 08:59:45.000000 TMD-2.3.1/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 08:59:45.000000 TMD-2.3.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-16 08:59:45.000000 TMD-2.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 08:59:45.000000 TMD-2.3.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-16 08:59:45.000000 TMD-2.3.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.541033 TMD-2.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.541033 TMD-2.3.1/examples/Advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)    34102 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/advanced_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/diversity_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/polar_plot_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/time_series_tmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20425 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/Advanced/variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/distances_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/extract_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-16 08:59:45.000000 TMD-2.3.1/examples/write_swc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-16 08:59:45.000000 TMD-2.3.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 08:59:45.000000 TMD-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:59:57.553034 TMD-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-16 08:59:45.000000 TMD-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.541033 TMD-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.545034 TMD-2.3.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/basic.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/basic_exotic_section_types.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/basic_no_comments.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/basic_no_sec_ids.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/basic_options.swc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/neuron.swc
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/neuron_ph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/neuron_ph_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_disordered.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_disordered_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_ph_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_ph_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_v0.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/sample_v2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/test_morph.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/test_morph_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/test_morph_v2.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.545034 TMD-2.3.1/tests/data/upper_case_names/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/upper_case_names/Sample1.ASC
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/upper_case_names/Sample1.H5
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/upper_case_names/Sample1.SWC
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/upper_case_names/Sample2.AsC
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/upper_case_names/Sample2.SwC
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tests/data/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)    48864 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/valid/C010398B-P2.CNG.swc
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33168 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/valid/C010398B-P2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/valid/sample.swc
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/valid/sample_v1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/data/valid/sample_v2.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_neuron_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_neuron_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_soma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_soma_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_swc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_topology_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_topology_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_topology_persistent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-16 08:59:45.000000 TMD-2.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/Neuron/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Neuron/Neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Neuron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Neuron/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/Population/
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Population/Population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Population/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/Soma/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Soma/Soma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Soma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Soma/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/Topology/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Topology/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Topology/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Topology/persistent_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Topology/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Topology/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/Tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Tree/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/Tree/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.549034 TMD-2.3.1/tmd/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/io/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/io/h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/io/swc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:59:57.553034 TMD-2.3.1/tmd/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/view/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/view/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40938 2023-05-16 08:59:45.000000 TMD-2.3.1/tmd/view/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-16 08:59:45.000000 TMD-2.3.1/tox.ini
```

### Comparing `TMD-2.3.0/.auto-changelog` & `TMD-2.3.1/.auto-changelog`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.auto-changelog-template.hbs` & `TMD-2.3.1/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.copier-answers.yml` & `TMD-2.3.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.github/dependabot.yml` & `TMD-2.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.github/workflows/codeql.yml` & `TMD-2.3.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.github/workflows/commitlint.yml` & `TMD-2.3.1/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.github/workflows/publish-sdist.yml` & `TMD-2.3.1/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.github/workflows/run-tox.yml` & `TMD-2.3.1/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.pre-commit-config.yaml` & `TMD-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/.pylintrc` & `TMD-2.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/CHANGELOG.md` & `TMD-2.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v2.3.1](https://github.com/BlueBrain/TMD/compare/v2.3.0..v2.3.1)
+
+> 15 May 2023
+
+### New Features
+
+- Files with upper-case extensions can be loaded (Adrien Berchet - [#78](https://github.com/BlueBrain/TMD/pull/78))
+
 ## [v2.3.0](https://github.com/BlueBrain/TMD/compare/v2.2.0..v2.3.0)
 
 > 28 April 2023
 
 ### Chores And Housekeeping
 
 - Update from Copier template (Adrien Berchet - [#73](https://github.com/BlueBrain/TMD/pull/73))
```

### Comparing `TMD-2.3.0/CITATION.cff` & `TMD-2.3.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/CONTRIBUTING.md` & `TMD-2.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/COPYRIGHT.txt` & `TMD-2.3.1/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/LICENSE-BSD.txt` & `TMD-2.3.1/LICENSE-BSD.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/LICENSE-LGPL.txt` & `TMD-2.3.1/LICENSE-LGPL.txt`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/PKG-INFO` & `TMD-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMD
-Version: 2.3.0
+Version: 2.3.1
 Summary: A python package for the topological analysis of neurons.
 Home-page: https://TMD.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU Lesser General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/TMD/issues
 Project-URL: Source, https://github.com/BlueBrain/TMD
 Classifier: Development Status :: 4 - Beta
```

### Comparing `TMD-2.3.0/README.md` & `TMD-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/TMD.egg-info/PKG-INFO` & `TMD-2.3.1/TMD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMD
-Version: 2.3.0
+Version: 2.3.1
 Summary: A python package for the topological analysis of neurons.
 Home-page: https://TMD.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: GNU Lesser General Public License v3.0
 Project-URL: Tracker, https://github.com/BlueBrain/TMD/issues
 Project-URL: Source, https://github.com/BlueBrain/TMD
 Classifier: Development Status :: 4 - Beta
```

### Comparing `TMD-2.3.0/TMD.egg-info/SOURCES.txt` & `TMD-2.3.1/TMD.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,19 @@
 tests/data/sample_ph_1.txt
 tests/data/sample_v0.h5
 tests/data/sample_v1.h5
 tests/data/sample_v2.h5
 tests/data/test_morph.swc
 tests/data/test_morph_v1.h5
 tests/data/test_morph_v2.h5
+tests/data/upper_case_names/Sample1.ASC
+tests/data/upper_case_names/Sample1.H5
+tests/data/upper_case_names/Sample1.SWC
+tests/data/upper_case_names/Sample2.AsC
+tests/data/upper_case_names/Sample2.SwC
 tests/data/valid/C010398B-P2.CNG.swc
 tests/data/valid/C010398B-P2.h5
 tests/data/valid/sample.swc
 tests/data/valid/sample_v1.h5
 tests/data/valid/sample_v2.h5
 tmd/__init__.py
 tmd/utils.py
```

### Comparing `TMD-2.3.0/commitlint.config.js` & `TMD-2.3.1/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/docs/Makefile` & `TMD-2.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/docs/source/conf.py` & `TMD-2.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/advanced_plot.py` & `TMD-2.3.1/examples/Advanced/advanced_plot.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/classification.py` & `TMD-2.3.1/examples/Advanced/classification.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/diversity_index.py` & `TMD-2.3.1/examples/Advanced/diversity_index.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/matching.py` & `TMD-2.3.1/examples/Advanced/matching.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/polar_plot_generation.py` & `TMD-2.3.1/examples/Advanced/polar_plot_generation.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/time_series_tmd.py` & `TMD-2.3.1/examples/Advanced/time_series_tmd.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/Advanced/variability.py` & `TMD-2.3.1/examples/Advanced/variability.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/classifier.py` & `TMD-2.3.1/examples/classifier.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/distances_example.py` & `TMD-2.3.1/examples/distances_example.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/examples/extract_ph.py` & `TMD-2.3.1/examples/extract_ph.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/package.json` & `TMD-2.3.1/package.json`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/pyproject.toml` & `TMD-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/setup.py` & `TMD-2.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 reqs = [
     "h5py>=2.8.0",
     "scipy>=1.1.0",
     "numpy>=1.15.0",
     "scikit-learn>=0.20.0",
     "munkres>=1.0.12",
     "cached-property>=1.5.1",
-    "morphio>=3.3.3",
+    "morphio>=3.3.4",
 ]
 
 doc_reqs = [
     "m2r2",
     "sphinx",
     "sphinx-bluebrain-theme",
     "sphinx-click",
```

### Comparing `TMD-2.3.0/tests/conftest.py` & `TMD-2.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/sample.swc` & `TMD-2.3.1/tests/data/sample.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/sample_disordered.swc` & `TMD-2.3.1/tests/data/sample_disordered.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/sample_disordered_v1.h5` & `TMD-2.3.1/tests/data/sample_disordered_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/sample_v0.h5` & `TMD-2.3.1/tests/data/sample_v0.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/sample_v1.h5` & `TMD-2.3.1/tests/data/sample_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/sample_v2.h5` & `TMD-2.3.1/tests/data/sample_v2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/test_morph.swc` & `TMD-2.3.1/tests/data/test_morph.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/test_morph_v1.h5` & `TMD-2.3.1/tests/data/test_morph_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/test_morph_v2.h5` & `TMD-2.3.1/tests/data/test_morph_v2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/valid/C010398B-P2.CNG.swc` & `TMD-2.3.1/tests/data/valid/C010398B-P2.CNG.swc`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/valid/C010398B-P2.h5` & `TMD-2.3.1/tests/data/valid/C010398B-P2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/valid/sample.swc` & `TMD-2.3.1/tests/data/upper_case_names/Sample1.SWC`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/valid/sample_v1.h5` & `TMD-2.3.1/tests/data/valid/sample_v1.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/data/valid/sample_v2.h5` & `TMD-2.3.1/tests/data/valid/sample_v2.h5`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_h5.py` & `TMD-2.3.1/tests/test_h5.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_io.py` & `TMD-2.3.1/tests/test_io.py`

 * *Files 11% similar despite different names*

```diff
@@ -157,7 +157,18 @@
 
     def point(section):
         return np.column_stack([section.x, section.y, section.z])
 
     npt.assert_array_equal(point(neuron.apical_dendrite[0]), [[3, 4, 5]])
     npt.assert_array_equal(point(neuron.basal_dendrite[0]), [[4, 5, 6]])
     npt.assert_array_equal(point(neuron.axon[0]), [[5, 6, 7], [5, 6, 7]])
+
+
+@pytest.mark.parametrize("use_morphio", [True, False])
+def test_upper_case(DATA_PATH, use_morphio):
+    """Read files with upper-case extensions."""
+    path = Path(DATA_PATH) / "upper_case_names"
+    if use_morphio:
+        files = path
+    else:
+        files = [i for i in path.iterdir() if i.suffix.lower() != ".asc"]
+    io.load_population(files, use_morphio=use_morphio)
```

### Comparing `TMD-2.3.0/tests/test_neuron.py` & `TMD-2.3.1/tests/test_neuron.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_neuron_conversion.py` & `TMD-2.3.1/tests/test_neuron_conversion.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_population.py` & `TMD-2.3.1/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_soma.py` & `TMD-2.3.1/tests/test_soma.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_soma_methods.py` & `TMD-2.3.1/tests/test_soma_methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_swc.py` & `TMD-2.3.1/tests/test_swc.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_topology_analysis.py` & `TMD-2.3.1/tests/test_topology_analysis.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_topology_methods.py` & `TMD-2.3.1/tests/test_topology_methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_topology_persistent_properties.py` & `TMD-2.3.1/tests/test_topology_persistent_properties.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_tree.py` & `TMD-2.3.1/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tests/test_tree_methods.py` & `TMD-2.3.1/tests/test_tree_methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Neuron/Neuron.py` & `TMD-2.3.1/tmd/Neuron/Neuron.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Neuron/__init__.py` & `TMD-2.3.1/tmd/Neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Neuron/methods.py` & `TMD-2.3.1/tmd/Neuron/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Population/Population.py` & `TMD-2.3.1/tmd/Population/Population.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Population/__init__.py` & `TMD-2.3.1/tmd/Population/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Soma/Soma.py` & `TMD-2.3.1/tmd/Soma/Soma.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Soma/__init__.py` & `TMD-2.3.1/tmd/Soma/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Soma/methods.py` & `TMD-2.3.1/tmd/Soma/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Topology/__init__.py` & `TMD-2.3.1/tmd/Topology/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Topology/analysis.py` & `TMD-2.3.1/tmd/Topology/analysis.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Topology/methods.py` & `TMD-2.3.1/tmd/Topology/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Topology/persistent_properties.py` & `TMD-2.3.1/tmd/Topology/persistent_properties.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Topology/statistics.py` & `TMD-2.3.1/tmd/Topology/statistics.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Topology/transformations.py` & `TMD-2.3.1/tmd/Topology/transformations.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Tree/Tree.py` & `TMD-2.3.1/tmd/Tree/Tree.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Tree/__init__.py` & `TMD-2.3.1/tmd/Tree/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/Tree/methods.py` & `TMD-2.3.1/tmd/Tree/methods.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/__init__.py` & `TMD-2.3.1/tmd/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/io/__init__.py` & `TMD-2.3.1/tmd/io/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/io/conversion.py` & `TMD-2.3.1/tmd/io/conversion.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/io/h5.py` & `TMD-2.3.1/tmd/io/h5.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/io/io.py` & `TMD-2.3.1/tmd/io/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,22 +85,28 @@
     # Definition of swc types from type_dict function
     if soma_type is None:
         soma_index = SOMA_TYPE
     else:
         soma_index = soma_type
 
     # Make neuron with correct filename and load data
-    if os.path.splitext(input_file)[-1] == ".swc":
+    ext = os.path.splitext(input_file)[-1].lower()
+    if ext == ".swc":
         data = swc_to_data(read_swc(input_file=input_file, line_delimiter=line_delimiter))
         neuron = Neuron.Neuron(name=str(input_file).replace(".swc", ""))
 
-    elif os.path.splitext(input_file)[-1] == ".h5":
+    elif ext == ".h5":
         data = read_h5(input_file=input_file, remove_duplicates=remove_duplicates)
         neuron = Neuron.Neuron(name=str(input_file).replace(".h5", ""))
 
+    else:
+        raise LoadNeuronError(
+            f"{input_file} is not a valid h5 or swc file. If asc set use_morphio to True."
+        )
+
     # Check for duplicated IDs
     IDs, counts = _np.unique(data[:, 0], return_counts=True)
     if (counts != 1).any():
         warnings.warn(f"The following IDs are duplicated: {IDs[counts > 1]}")
 
     data_T = _np.transpose(data)
 
@@ -130,16 +136,15 @@
         raise LoadNeuronError("Cannot create connectivity, nodes not connected correctly.") from exc
 
     # assuming soma points are in the beginning of the file.
     comp = cs.connected_components(dA[len(soma_ids) :, len(soma_ids) :])
 
     # Extract trees
     for i in range(comp[0]):
-        tree_ids = _np.where(comp[1] == i)[0] + len(soma_ids)
-        tree = make_tree(data[tree_ids])
+        tree = make_tree(data[_np.where(comp[1] == i)[0] + len(soma_ids)])
         neuron.append_tree(tree, tree_types)
 
     return neuron
 
 
 def load_neuron_from_morphio(path_or_obj, user_tree_types=None):
     """Create Neuron object from morphio object or from path loaded via morphio.
@@ -195,24 +200,25 @@
             f"Got: {neurons}"
         )
 
     pop = Population.Population(name=name)
 
     for filename in files:
         try:
-            ext = os.path.splitext(filename)[-1][1:]
+            ext = os.path.splitext(filename)[-1][1:].lower()
             if not use_morphio:
                 assert ext in ("h5", "swc")
                 pop.append_neuron(load_neuron(filename, user_tree_types=user_tree_types))
             else:
                 assert ext in ("h5", "swc", "asc")
                 pop.append_neuron(
                     load_neuron_from_morphio(filename, user_tree_types=user_tree_types)
                 )
 
         except AssertionError as exc:
-            error_msg = "{} is not a valid h5, swc or asc file. If asc set use_morphio to True."
-            raise Warning(error_msg.format(filename)) from exc
+            raise Warning(
+                "{filename} is not a valid h5, swc or asc file. If asc set use_morphio to True."
+            ) from exc
         except LoadNeuronError:
             print(f"File failed to load: {filename}")
 
     return pop
```

### Comparing `TMD-2.3.0/tmd/io/swc.py` & `TMD-2.3.1/tmd/io/swc.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/utils.py` & `TMD-2.3.1/tmd/utils.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/view/__init__.py` & `TMD-2.3.1/tmd/view/__init__.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/view/common.py` & `TMD-2.3.1/tmd/view/common.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/view/plot.py` & `TMD-2.3.1/tmd/view/plot.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tmd/view/view.py` & `TMD-2.3.1/tmd/view/view.py`

 * *Files identical despite different names*

### Comparing `TMD-2.3.0/tox.ini` & `TMD-2.3.1/tox.ini`

 * *Files identical despite different names*

