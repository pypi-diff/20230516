# Comparing `tmp/pyikarus-0.3.0.dev202310000077.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000079.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000077.tar", last modified: Mon May 15 14:45:46 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000079.tar", last modified: Tue May 16 14:58:42 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000077.tar` & `pyikarus-0.3.0.dev202310000079.tar`

### file list

```diff
@@ -1,324 +1,328 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.980445 pyikarus-0.3.0.dev202310000077/
--rw-r--r--   0 user      (1001) user      (1001)      312 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/.bettercodehub.yml
--rw-r--r--   0 user      (1001) user      (1001)     1300 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/.clang-format
--rw-r--r--   0 user      (1001) user      (1001)     1017 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/.cmake-format
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.892445 pyikarus-0.3.0.dev202310000077/.github/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.904445 pyikarus-0.3.0.dev202310000077/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 user      (1001) user      (1001)      460 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 user      (1001) user      (1001)      615 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.904445 pyikarus-0.3.0.dev202310000077/.github/workflows/
--rw-r--r--   0 user      (1001) user      (1001)      476 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/codespell.yml
--rw-r--r--   0 user      (1001) user      (1001)     1034 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 user      (1001) user      (1001)     4900 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/createRelease.yml
--rw-r--r--   0 user      (1001) user      (1001)     1635 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/debian-coverage.yml
--rw-r--r--   0 user      (1001) user      (1001)     2414 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/debian.yml
--rw-r--r--   0 user      (1001) user      (1001)     2042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/ghpages.yml
--rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/reuseLint.yml
--rw-r--r--   0 user      (1001) user      (1001)     2854 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/runExamples.yml
--rw-r--r--   0 user      (1001) user      (1001)     1212 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/.github/workflows/style.yml
--rw-r--r--   0 user      (1001) user      (1001)      457 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/.gitignore
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.908445 pyikarus-0.3.0.dev202310000077/.reuse/
--rw-r--r--   0 user      (1001) user      (1001)      661 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/.reuse/dep5
--rw-r--r--   0 user      (1001) user      (1001)     3324 2023-05-15 08:38:51.000000 pyikarus-0.3.0.dev202310000077/CHANGELOG.md
--rw-r--r--   0 user      (1001) user      (1001)     1318 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5335 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/CODE_OF_CONDUCT.md
--rw-r--r--   0 user      (1001) user      (1001)      759 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/LICENSE.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.908445 pyikarus-0.3.0.dev202310000077/LICENSES/
--rw-r--r--   0 user      (1001) user      (1001)    18375 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     7048 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/LICENSES/CC0-1.0.txt
--rw-r--r--   0 user      (1001) user      (1001)    42098 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 user      (1001) user      (1001)     1078 2023-03-24 20:46:08.000000 pyikarus-0.3.0.dev202310000077/LICENSES/MIT.txt
--rw-r--r--   0 user      (1001) user      (1001)    16727 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/LICENSES/MPL-2.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-15 14:45:46.976445 pyikarus-0.3.0.dev202310000077/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     3229 2023-03-06 10:17:28.000000 pyikarus-0.3.0.dev202310000077/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.908445 pyikarus-0.3.0.dev202310000077/cmake/
--rw-r--r--   0 user      (1001) user      (1001)      973 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/cmake/CPM.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.908445 pyikarus-0.3.0.dev202310000077/cmake/FormatTarget/
--rw-r--r--   0 user      (1001) user      (1001)     1270 2023-03-10 08:15:25.000000 pyikarus-0.3.0.dev202310000077/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.908445 pyikarus-0.3.0.dev202310000077/cmake/modules/
--rw-r--r--   0 user      (1001) user      (1001)      715 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      683 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      740 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      691 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      226 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/cmake/modules/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      446 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 user      (1001) user      (1001)     2040 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/cmake/tools.cmake
--rw-r--r--   0 user      (1001) user      (1001)      148 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/codecov.yml
--rw-r--r--   0 user      (1001) user      (1001)      121 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/codespellignore
--rw-r--r--   0 user      (1001) user      (1001)     1588 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/config.h.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.912445 pyikarus-0.3.0.dev202310000077/docs/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.912445 pyikarus-0.3.0.dev202310000077/docs/BuildLocally/
--rw-r--r--   0 user      (1001) user      (1001)      439 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      333 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.912445 pyikarus-0.3.0.dev202310000077/docs/__pycache__/
--rw-r--r--   0 user      (1001) user      (1001)     1136 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 user      (1001) user      (1001)     6961 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/literature.bib
--rw-r--r--   0 user      (1001) user      (1001)      117 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/literature.bib.license
--rw-r--r--   0 user      (1001) user      (1001)     1245 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/mkdocs-macros.py
--rw-r--r--   0 user      (1001) user      (1001)      394 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/mkdocs.insiders.yml
--rw-r--r--   0 user      (1001) user      (1001)     5042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/docs/mkdocs.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.892445 pyikarus-0.3.0.dev202310000077/docs/overrides/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.912445 pyikarus-0.3.0.dev202310000077/docs/overrides/partials/
--rw-r--r--   0 user      (1001) user      (1001)     1732 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/overrides/partials/comments.html
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.912445 pyikarus-0.3.0.dev202310000077/docs/website/
--rw-r--r--   0 user      (1001) user      (1001)       24 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/.meta.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.916445 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/
--rw-r--r--   0 user      (1001) user      (1001)     4710 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/assembler.md
--rw-r--r--   0 user      (1001) user      (1001)     6387 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 user      (1001) user      (1001)     2024 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 user      (1001) user      (1001)     3237 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 user      (1001) user      (1001)     8524 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 user      (1001) user      (1001)     2745 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/grids.md
--rw-r--r--   0 user      (1001) user      (1001)     4121 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/index.md
--rw-r--r--   0 user      (1001) user      (1001)     4932 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/localBasis.md
--rw-r--r--   0 user      (1001) user      (1001)    44213 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 user      (1001) user      (1001)     3978 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/manifolds.md
--rw-r--r--   0 user      (1001) user      (1001)     2590 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 user      (1001) user      (1001)     3086 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/observer.md
--rw-r--r--   0 user      (1001) user      (1001)     5211 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.920445 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/
--rw-r--r--   0 user      (1001) user      (1001)     6655 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 user      (1001) user      (1001)     7251 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/computePi.md
--rw-r--r--   0 user      (1001) user      (1001)     5439 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 user      (1001) user      (1001)     7055 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 user      (1001) user      (1001)     2164 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/index.md
--rw-r--r--   0 user      (1001) user      (1001)     7702 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 user      (1001) user      (1001)     5114 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 user      (1001) user      (1001)     6200 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 user      (1001) user      (1001)     4071 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.920445 pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/
--rw-r--r--   0 user      (1001) user      (1001)     2439 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 user      (1001) user      (1001)     1002 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 user      (1001) user      (1001)     2415 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 user      (1001) user      (1001)     1762 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.920445 pyikarus-0.3.0.dev202310000077/docs/website/04_blog/
--rw-r--r--   0 user      (1001) user      (1001)      274 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/04_blog/.authors.yml
--rw-r--r--   0 user      (1001) user      (1001)        7 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/04_blog/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.920445 pyikarus-0.3.0.dev202310000077/docs/website/04_blog/posts/
--rw-r--r--   0 user      (1001) user      (1001)     7731 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.924445 pyikarus-0.3.0.dev202310000077/docs/website/05_cppReferences/
--rw-r--r--   0 user      (1001) user      (1001)     2324 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.924445 pyikarus-0.3.0.dev202310000077/docs/website/99_Literature/
--rw-r--r--   0 user      (1001) user      (1001)      169 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.924445 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.928445 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 user      (1001) user      (1001)    52795 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 user      (1001) user      (1001)    46250 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 user      (1001) user      (1001)     2852 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 user      (1001) user      (1001)    17924 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 user      (1001) user      (1001)     9455 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.932445 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 user      (1001) user      (1001)    35234 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 user      (1001) user      (1001)    62184 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 user      (1001) user      (1001)     2281 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 user      (1001) user      (1001)    40033 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 user      (1001) user      (1001)    25505 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 user      (1001) user      (1001)     8101 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 user      (1001) user      (1001)     8255 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 user      (1001) user      (1001)     4364 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000077/docs/website/download.md
--rw-r--r--   0 user      (1001) user      (1001)      244 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/gallery.md
--rw-r--r--   0 user      (1001) user      (1001)     1358 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.936445 pyikarus-0.3.0.dev202310000077/docs/website/javascripts/
--rw-r--r--   0 user      (1001) user      (1001)      486 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.936445 pyikarus-0.3.0.dev202310000077/docs/website/stylesheets/
--rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/docs/website/stylesheets/extra.css
--rw-r--r--   0 user      (1001) user      (1001)      502 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/dune.module
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.936445 pyikarus-0.3.0.dev202310000077/ikarus/
--rw-r--r--   0 user      (1001) user      (1001)      748 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/ikarus/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.936445 pyikarus-0.3.0.dev202310000077/ikarus/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      268 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)    11069 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 user      (1001) user      (1001)    10714 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.936445 pyikarus-0.3.0.dev202310000077/ikarus/controlRoutines/
--rw-r--r--   0 user      (1001) user      (1001)      239 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2575 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 user      (1001) user      (1001)     2970 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.940445 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/
--rw-r--r--   0 user      (1001) user      (1001)      349 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      185 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.940445 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/
--rw-r--r--   0 user      (1001) user      (1001)      282 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2925 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     2305 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     1827 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     1041 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feRequirements.cpp
--rw-r--r--   0 user      (1001) user      (1001)     8419 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 user      (1001) user      (1001)     1338 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.944445 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/
--rw-r--r--   0 user      (1001) user      (1001)      345 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)    19628 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 user      (1001) user      (1001)    12549 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.944445 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 user      (1001) user      (1001)      397 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5699 2023-05-08 12:58:29.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 user      (1001) user      (1001)     2718 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 user      (1001) user      (1001)     4635 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 user      (1001) user      (1001)     3809 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 user      (1001) user      (1001)     5734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 user      (1001) user      (1001)      473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 user      (1001) user      (1001)     8010 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 user      (1001) user      (1001)     1196 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 user      (1001) user      (1001)     7827 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 user      (1001) user      (1001)    12655 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.948445 pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/
--rw-r--r--   0 user      (1001) user      (1001)      301 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     6734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 user      (1001) user      (1001)     7791 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 user      (1001) user      (1001)    12303 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.948445 pyikarus-0.3.0.dev202310000077/ikarus/python/
--rw-r--r--   0 user      (1001) user      (1001)      294 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.948445 pyikarus-0.3.0.dev202310000077/ikarus/python/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      249 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3149 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.948445 pyikarus-0.3.0.dev202310000077/ikarus/python/basis/
--rw-r--r--   0 user      (1001) user      (1001)      237 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     4559 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.948445 pyikarus-0.3.0.dev202310000077/ikarus/python/dirichletValues/
--rw-r--r--   0 user      (1001) user      (1001)      257 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     4116 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.948445 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/
--rw-r--r--   0 user      (1001) user      (1001)      303 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5036 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.952445 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/materials/
--rw-r--r--   0 user      (1001) user      (1001)      259 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5107 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 user      (1001) user      (1001)     5503 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.956445 pyikarus-0.3.0.dev202310000077/ikarus/python/test/
--rw-r--r--   0 user      (1001) user      (1001)      564 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3978 2023-05-15 09:03:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 user      (1001) user      (1001)  2704357 2023-05-15 11:50:45.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/test/nameTest.vtu
--rw-r--r--   0 user      (1001) user      (1001)     4447 2023-05-15 09:03:11.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 user      (1001) user      (1001)      862 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.956445 pyikarus-0.3.0.dev202310000077/ikarus/python/utils/
--rw-r--r--   0 user      (1001) user      (1001)      245 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1181 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.956445 pyikarus-0.3.0.dev202310000077/ikarus/solver/
--rw-r--r--   0 user      (1001) user      (1001)      211 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.956445 pyikarus-0.3.0.dev202310000077/ikarus/solver/linearSolver/
--rw-r--r--   0 user      (1001) user      (1001)      244 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     8891 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.956445 pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 user      (1001) user      (1001)      272 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5407 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 user      (1001) user      (1001)     8297 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 user      (1001) user      (1001)    18574 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.964445 pyikarus-0.3.0.dev202310000077/ikarus/utils/
--rw-r--r--   0 user      (1001) user      (1001)      712 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1741 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/algorithms.hh
--rw-r--r--   0 user      (1001) user      (1001)      878 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     1445 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/basis.hh
--rw-r--r--   0 user      (1001) user      (1001)     6930 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/concepts.hh
--rw-r--r--   0 user      (1001) user      (1001)      503 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.964445 pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/
--rw-r--r--   0 user      (1001) user      (1001)      262 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1654 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 user      (1001) user      (1001)      544 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 user      (1001) user      (1001)      703 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     2484 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 user      (1001) user      (1001)     2347 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 user      (1001) user      (1001)      682 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 user      (1001) user      (1001)     1367 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 user      (1001) user      (1001)      724 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 user      (1001) user      (1001)     3611 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 user      (1001) user      (1001)     2171 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6359 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 user      (1001) user      (1001)     3152 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/init.hh
--rw-r--r--   0 user      (1001) user      (1001)    15244 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     1711 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.964445 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/
--rw-r--r--   0 user      (1001) user      (1001)      450 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1554 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 user      (1001) user      (1001)     2307 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 user      (1001) user      (1001)      905 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1053 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1132 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1985 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 user      (1001) user      (1001)     5497 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/observer.hh
--rw-r--r--   0 user      (1001) user      (1001)      489 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 user      (1001) user      (1001)     4159 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 user      (1001) user      (1001)     1131 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/polyfit.cpp
--rw-r--r--   0 user      (1001) user      (1001)      570 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/polyfit.hh
--rw-r--r--   0 user      (1001) user      (1001)    10054 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 user      (1001) user      (1001)    15044 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/ikarus/utils/traits.hh
--rw-r--r--   0 user      (1001) user      (1001)      432 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/ikarus.pc.in
--rw-r--r--   0 user      (1001) user      (1001)      196 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/iwyu.imp
--rw-r--r--   0 user      (1001) user      (1001)      422 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/python/
--rw-r--r--   0 user      (1001) user      (1001)      582 2023-05-15 14:44:44.000000 pyikarus-0.3.0.dev202310000077/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/python/ikarus/
--rw-r--r--   0 user      (1001) user      (1001)      517 2023-05-15 08:59:18.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      603 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     5636 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/python/ikarus/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      167 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2300 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/assembler/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     1491 2023-05-15 08:55:23.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/basis.py
--rw-r--r--   0 user      (1001) user      (1001)     1408 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/python/ikarus/finite_elements/
--rw-r--r--   0 user      (1001) user      (1001)      173 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3465 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     1792 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/python/ikarus/utils/
--rw-r--r--   0 user      (1001) user      (1001)      163 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1496 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000077/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-15 14:45:46.000000 pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     9884 2023-05-15 14:45:46.000000 pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-15 14:45:46.000000 pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-15 14:45:46.000000 pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-15 14:45:46.000000 pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) user      (1001)      632 2023-05-15 13:01:44.000000 pyikarus-0.3.0.dev202310000077/python/setup.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.968445 pyikarus-0.3.0.dev202310000077/sandbox/
--rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/sandbox/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.972445 pyikarus-0.3.0.dev202310000077/sandbox/src/
--rw-r--r--   0 user      (1001) user      (1001)     1220 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000077/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.972445 pyikarus-0.3.0.dev202310000077/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 user      (1001) user      (1001)   674469 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 user      (1001) user      (1001)      320 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/sandbox/src/sandbox.cpp
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-15 14:45:46.980445 pyikarus-0.3.0.dev202310000077/setup.cfg
--rw-r--r--   0 user      (1001) user      (1001)     1864 2023-05-15 14:45:42.000000 pyikarus-0.3.0.dev202310000077/setup.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.972445 pyikarus-0.3.0.dev202310000077/tests/
--rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/tests/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.976445 pyikarus-0.3.0.dev202310000077/tests/src/
--rw-r--r--   0 user      (1001) user      (1001)     1418 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3906 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000077/tests/src/assemblerTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     9913 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/common.hh
--rw-r--r--   0 user      (1001) user      (1001)     2639 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/dependenciesTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6520 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/dirichletValueTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     3820 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/easTest.hh
--rw-r--r--   0 user      (1001) user      (1001)     1473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/enhancedAssumedStrainsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)      608 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/factories.hh
--rw-r--r--   0 user      (1001) user      (1001)     1870 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/functionTraitsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     2661 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/linearElasticityTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     2378 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/manifoldsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     7961 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/materialTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6770 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000077/tests/src/nonLinearElasticityTest.hh
--rw-r--r--   0 user      (1001) user      (1001)      724 2023-05-08 13:07:10.000000 pyikarus-0.3.0.dev202310000077/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rw-r--r--   0 user      (1001) user      (1001)      729 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/nonLinearElasticityTestSVK.cpp
--rw-r--r--   0 user      (1001) user      (1001)     9936 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/nonLinearOperatorTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6327 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/pathFollowingTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     1651 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/polyFitTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)      695 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/pythonConversionTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     1292 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 user      (1001) user      (1001)     5805 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/testFEElement.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-15 14:45:46.976445 pyikarus-0.3.0.dev202310000077/tests/src/testFiles/
--rw-r--r--   0 user      (1001) user      (1001)     9028 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 user      (1001) user      (1001)      395 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 user      (1001) user      (1001)      497 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 user      (1001) user      (1001)      546 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 user      (1001) user      (1001)    11431 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 user      (1001) user      (1001)     1114 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000077/tests/src/testHelpers.hh
--rw-r--r--   0 user      (1001) user      (1001)    17595 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000077/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:42.346654 pyikarus-0.3.0.dev202310000079/
+-rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.bettercodehub.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.clang-format
+-rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.cmake-format
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:36.344557 pyikarus-0.3.0.dev202310000079/.github/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:36.767303 pyikarus-0.3.0.dev202310000079/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:36.932628 pyikarus-0.3.0.dev202310000079/.github/workflows/
+-rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/codespell.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/createDockerContainer.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/createRelease.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/debian-coverage.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2414 2023-05-12 10:14:28.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/debian.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/ghpages.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/reuseLint.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-10 14:46:43.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/runExamples.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.github/workflows/style.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      457 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/.gitignore
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:36.946950 pyikarus-0.3.0.dev202310000079/.reuse/
+-rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/.reuse/dep5
+-rwxrwxrwx   0 user      (1001) user      (1001)     3324 2023-05-16 14:57:34.000000 pyikarus-0.3.0.dev202310000079/CHANGELOG.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1318 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/LICENSE.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.008419 pyikarus-0.3.0.dev202310000079/LICENSES/
+-rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/LICENSES/CC-BY-SA-4.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/LICENSES/CC0-1.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/LICENSES/LGPL-3.0-or-later.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1078 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/LICENSES/MIT.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-16 14:58:42.340634 pyikarus-0.3.0.dev202310000079/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:36.356828 pyikarus-0.3.0.dev202310000079/Testing/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.038639 pyikarus-0.3.0.dev202310000079/Testing/Temporary/
+-rwxrwxrwx   0 user      (1001) user      (1001)        4 2023-05-16 14:57:34.000000 pyikarus-0.3.0.dev202310000079/Testing/Temporary/CTestCostData.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-16 14:57:34.000000 pyikarus-0.3.0.dev202310000079/Testing/Temporary/LastTest.log
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.064669 pyikarus-0.3.0.dev202310000079/cmake/
+-rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/CPM.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.080515 pyikarus-0.3.0.dev202310000079/cmake/FormatTarget/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.182029 pyikarus-0.3.0.dev202310000079/cmake/modules/
+-rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/modules/AddAutoDiffFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/modules/AddEigenFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/modules/AddMatplotppFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/modules/AddSpdlogFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      226 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/modules/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      446 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/modules/IkarusMacros.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/cmake/tools.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/codecov.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/codespellignore
+-rwxrwxrwx   0 user      (1001) user      (1001)     1588 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/config.h.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.257556 pyikarus-0.3.0.dev202310000079/docs/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.273201 pyikarus-0.3.0.dev202310000079/docs/BuildLocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/BuildLocally/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.305169 pyikarus-0.3.0.dev202310000079/docs/__pycache__/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000079/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/literature.bib
+-rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/literature.bib.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/mkdocs-macros.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/mkdocs.insiders.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/mkdocs.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:36.385502 pyikarus-0.3.0.dev202310000079/docs/overrides/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.323727 pyikarus-0.3.0.dev202310000079/docs/overrides/partials/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/overrides/partials/comments.html
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.391354 pyikarus-0.3.0.dev202310000079/docs/website/
+-rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/.meta.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.645740 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/
+-rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/assembler.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/controlRoutines.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/dirichletBCs.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/feRequirements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     8524 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/finiteElements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/grids.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/localBasis.md
+-rwxrwxrwx   0 user      (1001) user      (1001)    44213 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/localFunctions.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/manifolds.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/nonlinearOperator.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/observer.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.821803 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/
+-rwxrwxrwx   0 user      (1001) user      (1001)     6655 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/cantileverBeam.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7251 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/computePi.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5439 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/cooksMembrane.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7055 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/incompressibleRubberBlock.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7702 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/kirchhoffPlate.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5114 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/newtonRaphsonMethod.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6200 2023-05-12 06:42:50.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/nonLinearElasticity.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4071 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.902340 pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2439 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/buildDocumentationLocally.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/codeStyle.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/howToEdit.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.947448 pyikarus-0.3.0.dev202310000079/docs/website/04_blog/
+-rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/04_blog/.authors.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/04_blog/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.971418 pyikarus-0.3.0.dev202310000079/docs/website/04_blog/posts/
+-rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:37.994202 pyikarus-0.3.0.dev202310000079/docs/website/05_cppReferences/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.016119 pyikarus-0.3.0.dev202310000079/docs/website/99_Literature/
+-rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.095095 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.362589 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/
+-rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.601455 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)    35234 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    62184 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2281 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    40033 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    25505 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/logo_blue.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/logo_blue.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/logo_white.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/logo_white.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/download.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/gallery.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.622728 pyikarus-0.3.0.dev202310000079/docs/website/javascripts/
+-rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.643961 pyikarus-0.3.0.dev202310000079/docs/website/stylesheets/
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/docs/website/stylesheets/extra.css
+-rwxrwxrwx   0 user      (1001) user      (1001)      502 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/dune.module
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.659741 pyikarus-0.3.0.dev202310000079/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.708968 pyikarus-0.3.0.dev202310000079/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      268 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    11069 2023-05-11 06:17:45.000000 pyikarus-0.3.0.dev202310000079/ikarus/assembler/simpleAssemblers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10714 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.756702 pyikarus-0.3.0.dev202310000079/ikarus/controlRoutines/
+-rwxrwxrwx   0 user      (1001) user      (1001)      239 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/controlRoutines/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2575 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/controlRoutines/loadControl.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2970 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.851590 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      349 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:38.943988 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/
+-rwxrwxrwx   0 user      (1001) user      (1001)      282 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2925 2023-05-10 15:33:49.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/autodiffFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2305 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1827 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/scalarFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feRequirements.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feRequirements.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1338 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.045713 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/
+-rwxrwxrwx   0 user      (1001) user      (1001)      345 2023-05-10 14:47:54.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    19628 2023-05-11 07:03:09.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12549 2023-05-12 09:02:39.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.276079 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      397 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5699 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/interface.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2718 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4635 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3809 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5734 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/svk.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/tags.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8010 2023-05-10 14:49:29.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1196 2023-05-12 06:42:50.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7827 2023-05-12 10:28:12.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.346994 pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/
+-rwxrwxrwx   0 user      (1001) user      (1001)      301 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     6734 2023-05-10 14:50:47.000000 pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/dirichletValues.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7791 2023-05-10 14:50:53.000000 pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/nonLinearOperator.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.364920 pyikarus-0.3.0.dev202310000079/ikarus/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      294 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.416141 pyikarus-0.3.0.dev202310000079/ikarus/python/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      249 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3149 2023-05-12 09:32:15.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.464078 pyikarus-0.3.0.dev202310000079/ikarus/python/basis/
+-rwxrwxrwx   0 user      (1001) user      (1001)      237 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/basis/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4559 2023-05-15 06:46:15.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.506079 pyikarus-0.3.0.dev202310000079/ikarus/python/dirichletValues/
+-rwxrwxrwx   0 user      (1001) user      (1001)      257 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/dirichletValues/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4116 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.572265 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5036 2023-05-12 09:06:11.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.626038 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5107 2023-05-12 06:43:07.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/materials/material.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5503 2023-05-12 10:14:28.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.789994 pyikarus-0.3.0.dev202310000079/ikarus/python/test/
+-rwxrwxrwx   0 user      (1001) user      (1001)      564 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/test/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-16 14:57:34.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/test/linearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)  2704357 2023-05-16 13:28:26.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/test/nameTest.vtu
+-rwxrwxrwx   0 user      (1001) user      (1001)     4447 2023-05-16 14:57:34.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/test/nonLinearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.830905 pyikarus-0.3.0.dev202310000079/ikarus/python/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      245 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1181 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.849804 pyikarus-0.3.0.dev202310000079/ikarus/solver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:39.892675 pyikarus-0.3.0.dev202310000079/ikarus/solver/linearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/linearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.041491 pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      272 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5407 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8297 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    18574 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.401878 pyikarus-0.3.0.dev202310000079/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      712 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/algorithms.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/autodiffHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1445 2023-05-12 08:51:52.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/basis.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/concepts.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-10 14:50:59.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.473619 pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/
+-rwxrwxrwx   0 user      (1001) user      (1001)      262 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/griddrawer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/matplotHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/matplotHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/duneUtilities.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/eigenDuneTransformations.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/eigenSparseAddon.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/findLineSegment.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/findLineSegment.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3611 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/flatPreBasis.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/functionSanityChecks.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/functionSanityChecks.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3152 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/init.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/linearAlgebraHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.623061 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/
+-rwxrwxrwx   0 user      (1001) user      (1001)      450 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1554 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/controlLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/controlVTKWriter.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      905 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/genericControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1053 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/gridDrawerObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1132 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/loadControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5497 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/observer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/observerMessages.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4159 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/pathFollowingFunctions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/polyfit.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/polyfit.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10054 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/tensorUtils.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus/utils/traits.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/ikarus.pc.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/iwyu.imp
+-rwxrwxrwx   0 user      (1001) user      (1001)      422 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.649569 pyikarus-0.3.0.dev202310000079/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      582 2023-05-16 14:57:42.000000 pyikarus-0.3.0.dev202310000079/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.775337 pyikarus-0.3.0.dev202310000079/python/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      517 2023-05-15 06:28:49.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      603 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     5636 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.818369 pyikarus-0.3.0.dev202310000079/python/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/assembler/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1491 2023-05-16 13:28:26.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/basis.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.860794 pyikarus-0.3.0.dev202310000079/python/ikarus/finite_elements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/finite_elements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/finite_elements/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.901655 pyikarus-0.3.0.dev202310000079/python/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1496 2023-05-16 13:28:26.000000 pyikarus-0.3.0.dev202310000079/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.982584 pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-16 14:58:34.000000 pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     9951 2023-05-16 14:58:36.000000 pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-16 14:58:34.000000 pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-16 14:58:34.000000 pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-16 14:58:34.000000 pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      630 2023-05-16 14:57:34.000000 pyikarus-0.3.0.dev202310000079/python/setup.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:40.996963 pyikarus-0.3.0.dev202310000079/sandbox/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/sandbox/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:41.038493 pyikarus-0.3.0.dev202310000079/sandbox/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1220 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:41.063804 pyikarus-0.3.0.dev202310000079/sandbox/src/auxiliaryFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/sandbox/src/auxiliaryFiles/circle.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      320 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/sandbox/src/sandbox.cpp
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-16 14:58:42.347653 pyikarus-0.3.0.dev202310000079/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1864 2023-05-16 14:57:51.000000 pyikarus-0.3.0.dev202310000079/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:41.093997 pyikarus-0.3.0.dev202310000079/tests/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/tests/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:41.679441 pyikarus-0.3.0.dev202310000079/tests/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1418 2023-05-12 07:13:04.000000 pyikarus-0.3.0.dev202310000079/tests/src/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3906 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/tests/src/assemblerTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9913 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/tests/src/common.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2639 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/dependenciesTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6520 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/tests/src/dirichletValueTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/easTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/enhancedAssumedStrainsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/tests/src/factories.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1870 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/tests/src/functionTraitsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2661 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000079/tests/src/linearElasticityTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2378 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/manifoldsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     7961 2023-05-12 06:42:50.000000 pyikarus-0.3.0.dev202310000079/tests/src/materialTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6770 2023-05-15 06:25:18.000000 pyikarus-0.3.0.dev202310000079/tests/src/nonLinearElasticityTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-10 14:51:20.000000 pyikarus-0.3.0.dev202310000079/tests/src/nonLinearElasticityTestSVK.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9936 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/nonLinearOperatorTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6327 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/pathFollowingTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1651 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/polyFitTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      695 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/pythonConversionTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1292 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/testAutodiffHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     5805 2023-05-11 06:42:16.000000 pyikarus-0.3.0.dev202310000079/tests/src/testFEElement.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-16 14:58:42.186734 pyikarus-0.3.0.dev202310000079/tests/src/testFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredTest.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredTest.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredTest2.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000079/tests/src/testHelpers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    17595 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000079/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000077/.clang-format` & `pyikarus-0.3.0.dev202310000079/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.cmake-format` & `pyikarus-0.3.0.dev202310000079/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.0.dev202310000079/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/createRelease.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/debian.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/ghpages.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/runExamples.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.github/workflows/style.yml` & `pyikarus-0.3.0.dev202310000079/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/.reuse/dep5` & `pyikarus-0.3.0.dev202310000079/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/CHANGELOG.md` & `pyikarus-0.3.0.dev202310000079/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/CODE_OF_CONDUCT.md` & `pyikarus-0.3.0.dev202310000079/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/LICENSE.md` & `pyikarus-0.3.0.dev202310000079/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.0.dev202310000079/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.0.dev202310000079/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.0.dev202310000079/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/LICENSES/MIT.txt` & `pyikarus-0.3.0.dev202310000079/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.0.dev202310000079/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/PKG-INFO` & `pyikarus-0.3.0.dev202310000079/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000077
+Version: 0.3.0.dev202310000079
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000077 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000079 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000077/README.md` & `pyikarus-0.3.0.dev202310000079/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/CPM.cmake` & `pyikarus-0.3.0.dev202310000079/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.0.dev202310000079/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.0.dev202310000079/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.0.dev202310000079/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.0.dev202310000079/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/cmake/tools.cmake` & `pyikarus-0.3.0.dev202310000079/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/config.h.cmake` & `pyikarus-0.3.0.dev202310000079/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.0.dev202310000079/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/literature.bib` & `pyikarus-0.3.0.dev202310000079/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/mkdocs-macros.py` & `pyikarus-0.3.0.dev202310000079/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/mkdocs.yml` & `pyikarus-0.3.0.dev202310000079/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/overrides/partials/comments.html` & `pyikarus-0.3.0.dev202310000079/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/assembler.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/grids.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/index.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/observer.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/01_framework/solvers.md` & `pyikarus-0.3.0.dev202310000079/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/computePi.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/index.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.0.dev202310000079/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.0.dev202310000079/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.0.dev202310000079/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.0.dev202310000079/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.0.dev202310000079/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/download.md` & `pyikarus-0.3.0.dev202310000079/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/docs/website/index.md` & `pyikarus-0.3.0.dev202310000079/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.0.dev202310000079/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feRequirements.cpp` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feRequirements.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/basis/basis.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/ikarus/python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.0.dev202310000079/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/test/nameTest.vtu` & `pyikarus-0.3.0.dev202310000079/ikarus/python/test/nameTest.vtu`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.0.dev202310000079/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.0.dev202310000079/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/algorithms.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/basis.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/concepts.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/init.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/polyfit.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/ikarus/utils/traits.hh` & `pyikarus-0.3.0.dev202310000079/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/python/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/__init__.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/_ikarus.cc` & `pyikarus-0.3.0.dev202310000079/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/basis.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/materials.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/ikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000079/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000077
+Version: 0.3.0.dev202310000079
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000077 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000079 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000077/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.0.dev202310000079/python/pyikarus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 .github/workflows/style.yml
 .reuse/dep5
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/CC0-1.0.txt
 LICENSES/LGPL-3.0-or-later.txt
 LICENSES/MIT.txt
 LICENSES/MPL-2.0.txt
+Testing/Temporary/CTestCostData.txt
+Testing/Temporary/LastTest.log
 cmake/CPM.cmake
 cmake/tools.cmake
 cmake/FormatTarget/CMakeLists.txt
 cmake/modules/AddAutoDiffFlags.cmake
 cmake/modules/AddEigenFlags.cmake
 cmake/modules/AddMatplotppFlags.cmake
 cmake/modules/AddSpdlogFlags.cmake
```

### Comparing `pyikarus-0.3.0.dev202310000077/python/setup.py.in` & `pyikarus-0.3.0.dev202310000079/python/setup.py.in`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
     name="pyikarus",
     description="${ProjectDescription}",
     version="${ProjectVersionString}",
     author="${ProjectAuthor}",
     author_email="${ProjectMaintainerEmail}",
     packages=find_packages(exclude=["docs/*"]),
     zip_safe=0,
-    package_data={"": ["*.so"], "pyikarus": ["data/*.cmake"]},
+    package_data={"": ["*.so"], "ikarus": ["data/*.cmake"]},
     install_requires=REQUIRED_PACKAGES,
     include_package_data=True,
 )
```

### Comparing `pyikarus-0.3.0.dev202310000077/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.0.dev202310000079/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/setup.py` & `pyikarus-0.3.0.dev202310000079/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # You are logged in as $(whoami)
 # EOF
 # nano ~/.pypirc
 # python -m venv /dune/dune-common/build-cmake/dune-env/
 # source /dune/dune-common/build-cmake/dune-env/bin/activate
 # pip install ikarus  --no-build-isolation
 
-ikarusVersion = "0.3.0.dev202310000077" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.0.dev202310000079" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor sicne ikarus pypi package already exists
 print(metadata)
```

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000079/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/assemblerTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/assemblerTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/common.hh` & `pyikarus-0.3.0.dev202310000079/tests/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/dirichletValueTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/easTest.hh` & `pyikarus-0.3.0.dev202310000079/tests/src/easTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/factories.hh` & `pyikarus-0.3.0.dev202310000079/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/linearElasticityTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/materialTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/materialTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/nonLinearElasticityTest.hh` & `pyikarus-0.3.0.dev202310000079/tests/src/nonLinearElasticityTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/polyFitTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/testFEElement.hh` & `pyikarus-0.3.0.dev202310000079/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.0.dev202310000079/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/testHelpers.hh` & `pyikarus-0.3.0.dev202310000079/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000077/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.0.dev202310000079/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

