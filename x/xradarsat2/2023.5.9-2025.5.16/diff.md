# Comparing `tmp/xradarsat2-2023.5.9.tar.gz` & `tmp/xradarsat2-2025.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xradarsat2-2023.5.9.tar", last modified: Tue May  9 12:47:15 2023, max compression
+gzip compressed data, was "xradarsat2-2025.5.16.tar", last modified: Tue May 16 10:09:20 2023, max compression
```

## Comparing `xradarsat2-2023.5.9.tar` & `xradarsat2-2025.5.16.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.222527 xradarsat2-2023.5.9/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.222527 xradarsat2-2023.5.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.222527 xradarsat2-2023.5.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/Installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.218527 xradarsat2-2023.5.9/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.222527 xradarsat2-2023.5.9/docs/_build/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/Installation.doctree
--rw-r--r--   0 runner    (1001) docker     (123)   974530 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/doc_xradarsat2.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/environment.pickle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.222527 xradarsat2-2023.5.9/docs/_build/doctrees/generated/
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/generated/xradarsat2.load_digital_number.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/generated/xradarsat2.rs2_reader.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/modules.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.222527 xradarsat2-2023.5.9/docs/_build/doctrees/nbsphinx/
--rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/nbsphinx/doc_xradarsat2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/doctrees/radarSat2_xarray_reader.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.226527 xradarsat2-2023.5.9/docs/_build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/Installation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.230527 xradarsat2-2023.5.9/docs/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/Installation.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/doc_xradarsat2.ipynb.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.230527 xradarsat2-2023.5.9/docs/_build/html/_sources/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/generated/xradarsat2.load_digital_number.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/generated/xradarsat2.rs2_reader.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_sources/radarSat2_xarray_reader.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.230527 xradarsat2-2023.5.9/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.230527 xradarsat2-2023.5.9/docs/_build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.234527 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   443670 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   131658 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/docs/_build/html/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    19531 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/_static/underscore.js
--rw-r--r--   0 runner    (1001) docker     (123)   437012 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/doc_xradarsat2.html
--rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/doc_xradarsat2.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/docs/_build/html/generated/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/generated/xradarsat2.load_digital_number.html
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/generated/xradarsat2.rs2_reader.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/modules.html
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/radarSat2_xarray_reader.html
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)    27073 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/_build/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/doc_xradarsat2.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/docs/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/generated/xradarsat2.load_digital_number.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/generated/xradarsat2.rs2_reader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/docs/radarSat2_xarray_reader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.218527 xradarsat2-2023.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/src/xradarsat2/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/src/xradarsat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/src/xradarsat2/radarSat2_tiff_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    76217 2023-05-09 12:46:55.000000 xradarsat2-2023.5.9/src/xradarsat2/radarSat2_xarray_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:47:15.238527 xradarsat2-2023.5.9/src/xradarsat2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-05-09 12:47:15.000000 xradarsat2-2023.5.9/src/xradarsat2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-09 12:47:15.000000 xradarsat2-2023.5.9/src/xradarsat2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:47:15.000000 xradarsat2-2023.5.9/src/xradarsat2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 12:47:15.000000 xradarsat2-2023.5.9/src/xradarsat2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 12:47:15.000000 xradarsat2-2023.5.9/src/xradarsat2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.577886 xradarsat2-2025.5.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.549886 xradarsat2-2025.5.16/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.549886 xradarsat2-2025.5.16/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-16 10:09:20.577886 xradarsat2-2025.5.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.553886 xradarsat2-2025.5.16/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/Installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.545886 xradarsat2-2025.5.16/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.553886 xradarsat2-2025.5.16/docs/_build/doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/Installation.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)   974530 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/doc_xradarsat2.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/environment.pickle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.553886 xradarsat2-2025.5.16/docs/_build/doctrees/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/generated/xradarsat2.load_digital_number.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/generated/xradarsat2.rs2_reader.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.553886 xradarsat2-2025.5.16/docs/_build/doctrees/nbsphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/nbsphinx/doc_xradarsat2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/doctrees/radarSat2_xarray_reader.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.557886 xradarsat2-2025.5.16/docs/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/Installation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.561886 xradarsat2-2025.5.16/docs/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/Installation.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/doc_xradarsat2.ipynb.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.561886 xradarsat2-2025.5.16/docs/_build/html/_sources/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/generated/xradarsat2.load_digital_number.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/generated/xradarsat2.rs2_reader.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_sources/radarSat2_xarray_reader.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.565886 xradarsat2-2025.5.16/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.565886 xradarsat2-2025.5.16/docs/_build/html/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.573886 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   443670 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   131658 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.573886 xradarsat2-2025.5.16/docs/_build/html/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19531 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 runner    (1001) docker     (123)   437012 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/doc_xradarsat2.html
+-rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/doc_xradarsat2.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.573886 xradarsat2-2025.5.16/docs/_build/html/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/generated/xradarsat2.load_digital_number.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/generated/xradarsat2.rs2_reader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/modules.html
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/radarSat2_xarray_reader.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27073 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/_build/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   553774 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/doc_xradarsat2.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.573886 xradarsat2-2025.5.16/docs/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/generated/xradarsat2.load_digital_number.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/generated/xradarsat2.rs2_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/docs/radarSat2_xarray_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:09:20.577886 xradarsat2-2025.5.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.549886 xradarsat2-2025.5.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.573886 xradarsat2-2025.5.16/src/xradarsat2/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/src/xradarsat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/src/xradarsat2/radarSat2_tiff_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76190 2023-05-16 10:09:04.000000 xradarsat2-2025.5.16/src/xradarsat2/radarSat2_xarray_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:09:20.577886 xradarsat2-2025.5.16/src/xradarsat2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-16 10:09:20.000000 xradarsat2-2025.5.16/src/xradarsat2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-16 10:09:20.000000 xradarsat2-2025.5.16/src/xradarsat2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:09:20.000000 xradarsat2-2025.5.16/src/xradarsat2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 10:09:20.000000 xradarsat2-2025.5.16/src/xradarsat2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 10:09:20.000000 xradarsat2-2025.5.16/src/xradarsat2.egg-info/top_level.txt
```

### Comparing `xradarsat2-2023.5.9/.github/workflows/publish.yml` & `xradarsat2-2025.5.16/.github/workflows/publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         run: |
           python -m build --sdist --wheel .
       - name: Check the built archives
         run: |
           twine check dist/*
           pip install dist/*.whl
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@0bf742be3ebe032c25dd15117957dc15d0cfc38d
+        uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
         with:
           password: ${{ secrets.pypi_token }}
           repository_url: https://upload.pypi.org/legacy/
           verify_metadata: true
```

### Comparing `xradarsat2-2023.5.9/.gitignore` & `xradarsat2-2025.5.16/.gitignore`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/LICENSE.md` & `xradarsat2-2025.5.16/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/PKG-INFO` & `xradarsat2-2025.5.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xradarsat2
-Version: 2023.5.9
+Version: 2025.5.16
 Summary: xarray/dask distributed L1 sar file reader for radarSat2
 Author-email: Yann Reynaud <Yann.Reynaud.2@ifremer.fr>
 License: MIT
 Project-URL: Homepage, https://github.com/umr-lops/xradarsat2
 Project-URL: Bug Tracker, https://github.com/umr-lops/xradarsat2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xradarsat2-2023.5.9/README.md` & `xradarsat2-2025.5.16/README.md`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/Installation.rst` & `xradarsat2-2025.5.16/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/Makefile` & `xradarsat2-2025.5.16/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/Installation.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/Installation.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/doc_xradarsat2.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/doc_xradarsat2.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/environment.pickle` & `xradarsat2-2025.5.16/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/generated/xradarsat2.load_digital_number.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/generated/xradarsat2.load_digital_number.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/generated/xradarsat2.rs2_reader.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/generated/xradarsat2.rs2_reader.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/index.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/modules.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/nbsphinx/doc_xradarsat2.ipynb` & `xradarsat2-2025.5.16/docs/_build/doctrees/nbsphinx/doc_xradarsat2.ipynb`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/doctrees/radarSat2_xarray_reader.doctree` & `xradarsat2-2025.5.16/docs/_build/doctrees/radarSat2_xarray_reader.doctree`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/Installation.html` & `xradarsat2-2025.5.16/docs/_build/html/Installation.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_sources/Installation.rst.txt` & `xradarsat2-2025.5.16/docs/_build/html/_sources/Installation.rst.txt`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_sources/doc_xradarsat2.ipynb.txt` & `xradarsat2-2025.5.16/docs/_build/html/_sources/doc_xradarsat2.ipynb.txt`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_sources/index.rst.txt` & `xradarsat2-2025.5.16/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/basic.css` & `xradarsat2-2025.5.16/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/badge_only.css` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal.woff` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/css/theme.css` & `xradarsat2-2025.5.16/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/doctools.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/jquery-3.6.0.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/jquery.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/js/badge_only.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/js/html5shiv.min.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/js/theme.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/language_data.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/pygments.css` & `xradarsat2-2025.5.16/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/searchtools.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/sphinx_highlight.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/underscore-1.13.1.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/_static/underscore.js` & `xradarsat2-2025.5.16/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/doc_xradarsat2.html` & `xradarsat2-2025.5.16/docs/_build/html/doc_xradarsat2.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/doc_xradarsat2.ipynb` & `xradarsat2-2025.5.16/docs/_build/html/doc_xradarsat2.ipynb`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/generated/xradarsat2.load_digital_number.html` & `xradarsat2-2025.5.16/docs/_build/html/generated/xradarsat2.load_digital_number.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/generated/xradarsat2.rs2_reader.html` & `xradarsat2-2025.5.16/docs/_build/html/generated/xradarsat2.rs2_reader.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/genindex.html` & `xradarsat2-2025.5.16/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/index.html` & `xradarsat2-2025.5.16/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/modules.html` & `xradarsat2-2025.5.16/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/objects.inv` & `xradarsat2-2025.5.16/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/radarSat2_xarray_reader.html` & `xradarsat2-2025.5.16/docs/_build/html/radarSat2_xarray_reader.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/search.html` & `xradarsat2-2025.5.16/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/_build/html/searchindex.js` & `xradarsat2-2025.5.16/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/conf.py` & `xradarsat2-2025.5.16/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/doc_xradarsat2.ipynb` & `xradarsat2-2025.5.16/docs/doc_xradarsat2.ipynb`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/index.rst` & `xradarsat2-2025.5.16/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/docs/make.bat` & `xradarsat2-2025.5.16/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/pyproject.toml` & `xradarsat2-2025.5.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/src/xradarsat2/radarSat2_tiff_reader.py` & `xradarsat2-2025.5.16/src/xradarsat2/radarSat2_tiff_reader.py`

 * *Files identical despite different names*

### Comparing `xradarsat2-2023.5.9/src/xradarsat2/radarSat2_xarray_reader.py` & `xradarsat2-2025.5.16/src/xradarsat2/radarSat2_xarray_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -2121,15 +2121,14 @@
     """
     must_have_files = [
         "product.xml",
         "lutBeta.xml",
         "lutGamma.xml",
         "lutSigma.xml",
         "imagery_*.tif",
-        "BrowseImage.tif",
     ]
     for file in must_have_files:
         entire_file_path = os.path.join(folder_path, file)
         list_file = glob.glob(entire_file_path)
         if len(list_file) == 0:
             raise FileNotFoundError(
                 f"The file {file} is missing for the product {folder_path}"
```

### Comparing `xradarsat2-2023.5.9/src/xradarsat2.egg-info/PKG-INFO` & `xradarsat2-2025.5.16/src/xradarsat2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xradarsat2
-Version: 2023.5.9
+Version: 2025.5.16
 Summary: xarray/dask distributed L1 sar file reader for radarSat2
 Author-email: Yann Reynaud <Yann.Reynaud.2@ifremer.fr>
 License: MIT
 Project-URL: Homepage, https://github.com/umr-lops/xradarsat2
 Project-URL: Bug Tracker, https://github.com/umr-lops/xradarsat2/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xradarsat2-2023.5.9/src/xradarsat2.egg-info/SOURCES.txt` & `xradarsat2-2025.5.16/src/xradarsat2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

