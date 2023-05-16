# Comparing `tmp/mqt.bench-0.4.3.tar.gz` & `tmp/mqt.bench-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.bench-0.4.3.tar", last modified: Thu May  4 11:00:19 2023, max compression
+gzip compressed data, was "mqt.bench-0.4.4.tar", last modified: Tue May 16 10:22:33 2023, max compression
```

## Comparing `mqt.bench-0.4.3.tar` & `mqt.bench-0.4.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.707524 mqt.bench-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.695524 mqt.bench-0.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.695524 mqt.bench-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-04 11:00:19.707524 mqt.bench-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.699524 mqt.bench-0.4.3/img/
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/arch.png
--rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/level_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/level_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/level_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/level_4.png
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/mqt_light.png
--rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/img/mqtbench.png
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:00:19.707524 mqt.bench-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.691524 mqt.bench-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.695524 mqt.bench-0.4.3/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.699524 mqt.bench-0.4.3/src/mqt/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmark_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/ae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/dj.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/graphstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/hhl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qft.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qftentangled.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_ml/qgan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_nature/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qpeexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qpeinexact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/qwalk.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/realamprandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/shor.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/su2random.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/twolocalrandom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/vqe.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/benchmarks/wstate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/evaluation/evaluation_visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/bench/evaluation/results/
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/evaluation/results/pie.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/evaluation/results/qubit_dist.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/evaluation/results/violins.pdf
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/qiskit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/tket_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/bench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/benchviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/benchviewer/static/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.703524 mqt.bench-0.4.3/src/mqt/benchviewer/static/files/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/static/files/MQTBench_all.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.707524 mqt.bench-0.4.3/src/mqt/benchviewer/static/files/qasm_output/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/static/files/qasm_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/static/tum_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.707524 mqt.bench-0.4.3/src/mqt/benchviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/templates/benchmark_description.html
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/templates/description.html
--rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/src/mqt/benchviewer/templates/legal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.699524 mqt.bench-0.4.3/src/mqt.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-04 11:00:19.000000 mqt.bench-0.4.3/src/mqt.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-04 11:00:19.000000 mqt.bench-0.4.3/src/mqt.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:00:19.000000 mqt.bench-0.4.3/src/mqt.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 11:00:19.000000 mqt.bench-0.4.3/src/mqt.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-04 11:00:19.000000 mqt.bench-0.4.3/src/mqt.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 11:00:19.000000 mqt.bench-0.4.3/src/mqt.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:00:19.707524 mqt.bench-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25706 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-05-04 11:00:10.000000 mqt.bench-0.4.3/tests/test_benchviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.347708 mqt.bench-0.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/arch.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86005 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84500 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76051 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112485 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/level_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196044 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/img/mqtbench.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.347708 mqt.bench-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.347708 mqt.bench-0.4.4/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/src/mqt/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18653 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmark_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/ae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/graphstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/hhl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qftentangled.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_ml/qgan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_nature/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeinexact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/qwalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/realamprandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/shor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/su2random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/twolocalrandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/vqe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/benchmarks/wstate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation_visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.355708 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/pie.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/qubit_dist.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24435 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/evaluation/results/violins.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/qiskit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/tket_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/bench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25908 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/MQTBench_all.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/qasm_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/files/qasm_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    61137 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/static/tum_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/src/mqt/benchviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/benchmark_description.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/src/mqt/benchviewer/templates/legal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.351708 mqt.bench-0.4.4/src/mqt.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 10:22:33.000000 mqt.bench-0.4.4/src/mqt.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:22:33.359708 mqt.bench-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    26017 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-05-16 10:22:25.000000 mqt.bench-0.4.4/tests/test_benchviewer.py
```

### Comparing `mqt.bench-0.4.3/.github/dependabot.yml` & `mqt.bench-0.4.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/.github/release-drafter.yml` & `mqt.bench-0.4.4/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/.github/workflows/codeql.yml` & `mqt.bench-0.4.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/.github/workflows/coverage.yml` & `mqt.bench-0.4.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/.github/workflows/deploy.yml` & `mqt.bench-0.4.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/.gitignore` & `mqt.bench-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/.pre-commit-config.yaml` & `mqt.bench-0.4.4/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -66,21 +66,21 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.267
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         files: ^(src|tests|setup.py)
         args: []
         additional_dependencies:
           - importlib_resources
           - pytest
```

### Comparing `mqt.bench-0.4.3/LICENSE` & `mqt.bench-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/PKG-INFO` & `mqt.bench-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 0.4.3
+Version: 0.4.4
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mqt.bench-0.4.3/README.md` & `mqt.bench-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/config.json` & `mqt.bench-0.4.4/config.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/arch.png` & `mqt.bench-0.4.4/img/arch.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/level_1.png` & `mqt.bench-0.4.4/img/level_1.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/level_2.png` & `mqt.bench-0.4.4/img/level_2.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/level_3.png` & `mqt.bench-0.4.4/img/level_3.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/level_4.png` & `mqt.bench-0.4.4/img/level_4.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/mqt_dark.png` & `mqt.bench-0.4.4/img/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/mqt_light.png` & `mqt.bench-0.4.4/img/mqt_light.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/img/mqtbench.png` & `mqt.bench-0.4.4/img/mqtbench.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/pyproject.toml` & `mqt.bench-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 keywords = ["MQT",  "quantum computing", "benchmarking", "performance", "testing"]
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dynamic = ["version"]
 
 dependencies = [
-    "pytket-qiskit>=0.34.0,<0.39.0",  #  manages the dependencies for qiskit and tket in a combined fashion
+    "pytket-qiskit>=0.34.0,<0.40.0",  #  manages the dependencies for qiskit and tket in a combined fashion
     "qiskit[all]",  # this is merely to get the [all] dependencies. The versioning is covered by pytket-qiskit
     "pandas>=1.0.0",
     "flask>=2.0.0",
     "networkx>=2.0.0",
     "pyscf>=2.1.0",
     "packaging>=21.0",
     "tqdm>=4.0.0",
```

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmark_generator.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmark_generator.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/ae.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/ae.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/dj.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/dj.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/ghz.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/ghz.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/graphstate.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/graphstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/grover.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/grover.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/hhl.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/hhl.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qaoa.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qft.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qft.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qftentangled.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qftentangled.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_ml/qgan.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_ml/qgan.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qpeexact.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qpeinexact.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qpeinexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/qwalk.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/qwalk.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/realamprandom.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/realamprandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/shor.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/shor.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/su2random.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/su2random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/twolocalrandom.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/twolocalrandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/vqe.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/vqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/benchmarks/wstate.py` & `mqt.bench-0.4.4/src/mqt/bench/benchmarks/wstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/evaluation/evaluation.py` & `mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/evaluation/evaluation_visualization.ipynb` & `mqt.bench-0.4.4/src/mqt/bench/evaluation/evaluation_visualization.ipynb`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/evaluation/results/pie.pdf` & `mqt.bench-0.4.4/src/mqt/bench/evaluation/results/pie.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/evaluation/results/qubit_dist.pdf` & `mqt.bench-0.4.4/src/mqt/bench/evaluation/results/qubit_dist.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/evaluation/results/violins.pdf` & `mqt.bench-0.4.4/src/mqt/bench/evaluation/results/violins.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/qiskit_helper.py` & `mqt.bench-0.4.4/src/mqt/bench/qiskit_helper.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/bench/tket_helper.py` & `mqt.bench-0.4.4/src/mqt/bench/tket_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 from typing import TYPE_CHECKING, Literal, overload
 
 from mqt.bench import utils
 from pytket import OpType
 from pytket.architecture import Architecture  # type: ignore[attr-defined]
 from pytket.extensions.qiskit import qiskit_to_tk
 from pytket.passes import (  # type: ignore[attr-defined]
+    CliffordSimp,
     CXMappingPass,
     FullPeepholeOptimise,
+    KAKDecomposition,
     PlacementPass,
     RoutingPass,
+    SynthesiseTket,
     auto_rebase_pass,
 )
 from pytket.placement import GraphPlacement, LinePlacement  # type: ignore[attr-defined]
 from pytket.qasm import circuit_to_qasm_str
 from qiskit import QuantumCircuit, transpile
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -306,24 +309,32 @@
         print("TKET Exception Mapped: ", e)
         return False
 
     native_gatenames = get_rebase(gate_set_name, True)
     native_gate_set_rebase = get_rebase(gate_set_name)
     arch = Architecture(cmap)
 
+    # add blank wires to the circuit such that afterwards the number of qubits is equal to the number of qubits of the architecture
+    highest_used_qubit_index = max(max(sublist) for sublist in cmap)
+    diff = highest_used_qubit_index + 1 - qc_tket.n_qubits  # offset of one is added because the indices start at 0
+    qc_tket.add_blank_wires(diff)
+
     native_gate_set_rebase.apply(qc_tket)
     FullPeepholeOptimise(target_2qb_gate=OpType.TK2).apply(qc_tket)
     placer = LinePlacement(arch) if lineplacement else GraphPlacement(arch)
     PlacementPass(placer).apply(qc_tket)
     RoutingPass(arch).apply(qc_tket)
-    FullPeepholeOptimise(target_2qb_gate=OpType.TK2, allow_swaps=False).apply(qc_tket)
-    native_gate_set_rebase.apply(qc_tket)
+    SynthesiseTket().apply(qc_tket)
+    KAKDecomposition(allow_swaps=False).apply(qc_tket)
+    CliffordSimp(allow_swaps=False).apply(qc_tket)
+    SynthesiseTket().apply(qc_tket)
     if not qc_tket.valid_connectivity(arch, directed=True):
         CXMappingPass(arc=arch, placer=placer, directed_cx=True, delay_measures=False).apply(qc_tket)
     native_gate_set_rebase.apply(qc_tket)
+
     if return_qc:
         return qc_tket
     return utils.save_as_qasm(
         circuit_to_qasm_str(qc_tket),
         filename_mapped,
         native_gatenames,
         True,
```

### Comparing `mqt.bench-0.4.3/src/mqt/bench/utils.py` & `mqt.bench-0.4.4/src/mqt/bench/utils.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/backend.py` & `mqt.bench-0.4.4/src/mqt/benchviewer/backend.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/main.py` & `mqt.bench-0.4.4/src/mqt/benchviewer/main.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/static/favicon.ico` & `mqt.bench-0.4.4/src/mqt/benchviewer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/static/mqt_dark.png` & `mqt.bench-0.4.4/src/mqt/benchviewer/static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/static/tum_logo.svg` & `mqt.bench-0.4.4/src/mqt/benchviewer/static/tum_logo.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/templates/benchmark_description.html` & `mqt.bench-0.4.4/src/mqt/benchviewer/templates/benchmark_description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/templates/description.html` & `mqt.bench-0.4.4/src/mqt/benchviewer/templates/description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/templates/index.html` & `mqt.bench-0.4.4/src/mqt/benchviewer/templates/index.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt/benchviewer/templates/legal.html` & `mqt.bench-0.4.4/src/mqt/benchviewer/templates/legal.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/src/mqt.bench.egg-info/PKG-INFO` & `mqt.bench-0.4.4/src/mqt.bench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 0.4.3
+Version: 0.4.4
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@jku.at>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mqt.bench-0.4.3/src/mqt.bench.egg-info/SOURCES.txt` & `mqt.bench-0.4.4/src/mqt.bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqt.bench-0.4.3/tests/test_bench.py` & `mqt.bench-0.4.4/tests/test_bench.py`

 * *Files 2% similar despite different names*

```diff
@@ -967,7 +967,21 @@
         res_groundstate = groundstate.get_molecule(elem)
         assert res_groundstate
 
 
 def test_get_cmap_from_devicename() -> None:
     with pytest.raises(ValueError, match="Device wrong_name is not supported"):
         utils.get_cmap_from_devicename("wrong_name")
+
+
+def test_tket_mapped_circuit_qubit_number() -> None:
+    qc = get_benchmark("ghz", 1, 5)
+    res = tket_helper.get_mapped_level(
+        qc,
+        "ibm",
+        qc.num_qubits,
+        "ibm_washington",
+        True,
+        file_precheck=False,
+        return_qc=True,
+    )
+    assert res.n_qubits == 127
```

### Comparing `mqt.bench-0.4.3/tests/test_benchviewer.py` & `mqt.bench-0.4.4/tests/test_benchviewer.py`

 * *Files identical despite different names*

