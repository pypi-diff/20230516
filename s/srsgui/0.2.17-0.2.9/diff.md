# Comparing `tmp/srsgui-0.2.17.tar.gz` & `tmp/srsgui-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ukm9bb3w\srsgui-0.2.17.tar", last modified: Mon May 15 23:01:24 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ps3u1u8m\srsgui-0.2.9.tar", last modified: Tue Apr 11 21:39:00 2023, max compression
```

## Comparing `srsgui-0.2.17.tar` & `srsgui-0.2.9.tar`

### file list

```diff
@@ -1,210 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.208416 srsgui-0.2.17/
--rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsgui-0.2.17/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-15 22:00:06.000000 srsgui-0.2.17/LICENSE.txt
--rw-rw-rw-   0        0        0     3586 2023-05-15 23:01:24.208416 srsgui-0.2.17/PKG-INFO
--rw-rw-rw-   0        0        0     2766 2023-05-15 18:10:04.000000 srsgui-0.2.17/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.025657 srsgui-0.2.17/doc-source/
--rw-rw-rw-   0        0        0      655 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.046219 srsgui-0.2.17/doc-source/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/create-task.rst
--rw-rw-rw-   0        0        0     6111 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/index.rst
--rw-rw-rw-   0        0        0     4397 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/installation.rst
--rwxrwxrwx   0        0        0      803 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/make.bat
--rw-rw-rw-   0        0        0      936 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.task.rst
--rw-rw-rw-   0        0        0     1542 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      557 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1761 2023-05-15 17:35:24.000000 srsgui-0.2.17/doc-source/srsgui.ui.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.048299 srsgui-0.2.17/docs/
--rw-rw-rw-   0        0        0        0 2023-05-15 18:01:44.000000 srsgui-0.2.17/docs/.nojekyll
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.059334 srsgui-0.2.17/docs/html/
--rw-rw-rw-   0        0        0      234 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/.buildinfo
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.069364 srsgui-0.2.17/docs/html/_images/
--rw-rw-rw-   0        0        0    31067 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71011 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    37573 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_images/terminal-with-example.png
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.095821 srsgui-0.2.17/docs/html/_sources/
--rw-rw-rw-   0        0        0     6097 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/create-project.rst.txt
--rw-rw-rw-   0        0        0     6656 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/create-task.rst.txt
--rw-rw-rw-   0        0        0     6111 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/define-instrument.rst.txt
--rw-rw-rw-   0        0        0    15640 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/example.rst.txt
--rw-rw-rw-   0        0        0     3684 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0     4397 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/installation.rst.txt
--rw-rw-rw-   0        0        0      936 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.inst.communications.rst.txt
--rw-rw-rw-   0        0        0      950 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.inst.rst.txt
--rw-rw-rw-   0        0        0      117 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.rst.txt
--rw-rw-rw-   0        0        0      989 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.task.rst.txt
--rw-rw-rw-   0        0        0     1542 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.ui.commandtree.rst.txt
--rw-rw-rw-   0        0        0      557 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.ui.qt.rst.txt
--rw-rw-rw-   0        0        0     1761 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_sources/srsgui.ui.rst.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.118877 srsgui-0.2.17/docs/html/_static/
--rw-rw-rw-   0        0        0     4418 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-rw-   0        0        0    15519 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/_static/basic.css
--rw-rw-rw-   0        0        0    31067 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/connect-dialog-box-capture.png
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.118877 srsgui-0.2.17/docs/html/_static/css/
--rw-rw-rw-   0        0        0     3275 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/badge_only.css
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.149350 srsgui-0.2.17/docs/html/_static/css/fonts/
--rw-rw-rw-   0        0        0    87624 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-rw-   0        0        0    67312 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-rw-   0        0        0    86288 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-rw-   0        0        0    66444 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-rw-   0        0        0   165742 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   444379 2022-10-11 22:50:17.000000 srsgui-0.2.17/docs/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0   323344 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-rw-   0        0        0   193308 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-rw-   0        0        0   309728 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-bold.woff
--rw-rw-rw-   0        0        0   184912 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-bold.woff2
--rw-rw-rw-   0        0        0   328412 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-rw-   0        0        0   195704 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-rw-   0        0        0   309192 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-normal.woff
--rw-rw-rw-   0        0        0   182708 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/css/fonts/lato-normal.woff2
--rw-rw-rw-   0        0        0   129674 2022-10-11 22:50:17.000000 srsgui-0.2.17/docs/html/_static/css/theme.css
--rw-rw-rw-   0        0        0     4472 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/doctools.js
--rw-rw-rw-   0        0        0      428 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0    71070 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0      286 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/file.png
--rw-rw-rw-   0        0        0    56013 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0   288580 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/jquery-3.6.0.js
--rw-rw-rw-   0        0        0    89501 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/jquery.js
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.149350 srsgui-0.2.17/docs/html/_static/js/
--rw-rw-rw-   0        0        0      934 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/js/badge_only.js
--rw-rw-rw-   0        0        0     4370 2022-10-11 22:50:17.000000 srsgui-0.2.17/docs/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-rw-   0        0        0     2734 2022-10-11 22:50:17.000000 srsgui-0.2.17/docs/html/_static/js/html5shiv.min.js
--rw-rw-rw-   0        0        0     5023 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/js/theme.js
--rw-rw-rw-   0        0        0     4957 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/minus.png
--rw-rw-rw-   0        0        0    29667 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0       90 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/plus.png
--rw-rw-rw-   0        0        0     4892 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/_static/pygments.css
--rw-rw-rw-   0        0        0    18215 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    50740 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0     4712 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/sphinx_highlight.js
--rw-rw-rw-   0        0        0    39412 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/html/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0    68420 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    19530 2022-10-05 00:44:54.000000 srsgui-0.2.17/docs/html/_static/underscore.js
--rw-rw-rw-   0        0        0    16129 2023-05-15 18:10:51.000000 srsgui-0.2.17/docs/html/create-project.html
--rw-rw-rw-   0        0        0    18027 2023-05-15 18:10:51.000000 srsgui-0.2.17/docs/html/create-task.html
--rw-rw-rw-   0        0        0    21128 2023-05-15 18:10:51.000000 srsgui-0.2.17/docs/html/define-instrument.html
--rw-rw-rw-   0        0        0   102951 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/example.html
--rw-rw-rw-   0        0        0    90615 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/genindex.html
--rw-rw-rw-   0        0        0    13685 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/index.html
--rw-rw-rw-   0        0        0    14128 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/installation.html
--rw-rw-rw-   0        0        0     4886 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/objects.inv
--rw-rw-rw-   0        0        0    13108 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/py-modindex.html
--rw-rw-rw-   0        0        0     4382 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/search.html
--rw-rw-rw-   0        0        0   112445 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/searchindex.js
--rw-rw-rw-   0        0        0    88208 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.html
--rw-rw-rw-   0        0        0    42791 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.inst.communications.html
--rw-rw-rw-   0        0        0   112806 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.inst.html
--rw-rw-rw-   0        0        0    94766 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.task.html
--rw-rw-rw-   0        0        0    66847 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.ui.commandtree.html
--rw-rw-rw-   0        0        0   102105 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.ui.html
--rw-rw-rw-   0        0        0     8608 2023-05-15 18:10:52.000000 srsgui-0.2.17/docs/html/srsgui.ui.qt.html
--rw-rw-rw-   0        0        0       66 2023-05-15 17:35:24.000000 srsgui-0.2.17/docs/index.html
--rw-rw-rw-   0        0        0     1317 2023-05-15 22:58:22.000000 srsgui-0.2.17/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.17/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 23:01:24.208416 srsgui-0.2.17/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.17/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.149350 srsgui-0.2.17/srsgui/
--rw-rw-rw-   0        0        0     1538 2023-05-15 23:00:30.000000 srsgui-0.2.17/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.005625 srsgui-0.2.17/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.159369 srsgui-0.2.17/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.159369 srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.159369 srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.169383 srsgui-0.2.17/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9886 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.179374 srsgui-0.2.17/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8772 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14840 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10381 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9768 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.179374 srsgui-0.2.17/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6606 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5322 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6830 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22136 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-15 21:54:54.000000 srsgui-0.2.17/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.198372 srsgui-0.2.17/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6138 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.198372 srsgui-0.2.17/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12049 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8334 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5072 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4247 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13808 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.208416 srsgui-0.2.17/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24814 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.2.17/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:01:24.159369 srsgui-0.2.17/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3586 2023-05-15 23:01:23.000000 srsgui-0.2.17/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6596 2023-05-15 23:01:23.000000 srsgui-0.2.17/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 23:01:23.000000 srsgui-0.2.17/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-15 23:01:23.000000 srsgui-0.2.17/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-05-15 23:01:23.000000 srsgui-0.2.17/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 23:01:23.000000 srsgui-0.2.17/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.9/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.979862 srsgui-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.889910 srsgui-0.2.9/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.899904 srsgui-0.2.9/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.9/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.9/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:39:00.979862 srsgui-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-11 21:34:20.000000 srsgui-0.2.9/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.9/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.879943 srsgui-0.2.9/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.929916 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.9/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9578 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.939882 srsgui-0.2.9/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14665 2023-04-11 20:13:55.000000 srsgui-0.2.9/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10049 2023-04-11 18:04:43.000000 srsgui-0.2.9/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.9/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.949878 srsgui-0.2.9/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5203 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.9/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22234 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.959872 srsgui-0.2.9/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.969903 srsgui-0.2.9/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-11 17:28:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-11 17:29:16.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4755 2023-04-11 17:22:27.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3127 2023-04-11 21:33:12.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     3844 2023-04-11 17:33:14.000000 srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 22:51:26.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-04-11 17:35:42.000000 srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.9/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.9/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.9/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13671 2023-04-11 00:24:36.000000 srsgui-0.2.9/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.979862 srsgui-0.2.9/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.9/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.9/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.9/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.9/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:39:00.919894 srsgui-0.2.9/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3162 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 21:39:00.000000 srsgui-0.2.9/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.17/.gitignore` & `srsgui-0.2.9/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 lib64/
 parts/
 sdist/
 var/
 wheels/
 old/
 local data/
-doctrees/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
```

### Comparing `srsgui-0.2.17/LICENSE.txt` & `srsgui-0.2.9/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 The MIT License
 
-Copyright (c) 2022, 2023 Stanford Research Systems
+Copyright (c) 2022 Stanford Research Systems
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `srsgui-0.2.17/PKG-INFO` & `srsgui-0.2.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.17
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
-Project-URL: homepage, https://github.com/thinkSRS/srsgui
-Project-URL: documentation, https://thinksrs.github.io/srsgui
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,15 +27,15 @@
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+![screenshot](docs/source/_static/example-screen-capture-1.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
@@ -74,22 +72,22 @@
 It will start `srsgui` application.
 
 ## Run the example project
 
 By default, `srsgui` application starts with the last project it ran,
 when it is closed.
  
-To open the example project included in the `srsgui` package 
-(if it does not start with the example project), go to the `srsgui` package 
+To open the example project included in the `srsgui` package,
+, if it does not start with the example project, go to the `srsgui` package 
 directory, find the examples directory, and find a .taskconfig file in an 
 example project folder. 
 
 You can run the second and fifth task in the Task menu 
 even without any instruments connected.
 
 ## Create a project
 
 `Srsgui` is a platform that helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
+
 scripts running in GUI with the same amount of code with writing console-based 
-scripts. For programming API, refer to
-[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
+scripts.
```

### Comparing `srsgui-0.2.17/README.md` & `srsgui-0.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+![screenshot](docs/source/_static/example-screen-capture-1.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
@@ -53,22 +53,22 @@
 It will start `srsgui` application.
 
 ## Run the example project
 
 By default, `srsgui` application starts with the last project it ran,
 when it is closed.
  
-To open the example project included in the `srsgui` package 
-(if it does not start with the example project), go to the `srsgui` package 
+To open the example project included in the `srsgui` package,
+, if it does not start with the example project, go to the `srsgui` package 
 directory, find the examples directory, and find a .taskconfig file in an 
 example project folder. 
 
 You can run the second and fifth task in the Task menu 
 even without any instruments connected.
 
 ## Create a project
 
 `Srsgui` is a platform that helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
+
 scripts running in GUI with the same amount of code with writing console-based 
-scripts. For programming API, refer to
-[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
+scripts.
```

### Comparing `srsgui-0.2.17/doc-source/Makefile` & `srsgui-0.2.9/docs/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = ../docs
+SOURCEDIR     = source
+BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `srsgui-0.2.17/doc-source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.9/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/example-screen-capture-1.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/example-screen-capture-2.png` & `srsgui-0.2.9/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/initial-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/second-task-screen-capture.png` & `srsgui-0.2.9/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/terminal-with-example-2.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/terminal-with-example.png` & `srsgui-0.2.9/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/conf.py` & `srsgui-0.2.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/create-project.rst` & `srsgui-0.2.9/docs/source/create-project.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
     /Project root directory
         /instruments
         /tasks
         project.taskconfig
 
 A project directory has a .taskconfig configuration file and multiple Python
-modules in two special subdirectory: instruments and tasks.
+modules in two special subdirectory: instruments, tasks.
 Whenever open a .taskconfig file from the SRSGUI application,
-Python modules in those directories will be forced to reload.
+Python modules in those directories are forced to reload.
 
 Typically, a Python interpreter loads a module when it is imported for the first time,
-and never check again if the module is modified. When you make changes to a module, save it,
-and run a script using it, you would not see the changes because the Python interpreter
-would not use the modified module, as long as the previous copy of the module is in memory.
-The Python interpreter needs to restart to take an effect of the changed modules.
+and never check again if the module is modified. When you make changes to a module,
+and import the module again with a Python interpreter, it ignores it
+because it is already imported before. The Python interpreter needs to restart
+to take an effect of the changed modules.
 
 When you open a .taskconfig file again from the ``srsgui`` application,
 it reloads all the Python modules in the 2 subdirectories.
 It helps when you modify and debug a module in the subdirectories.
 Instead of restart the application every time a module is changed,
 you can reopen the .taskconfig file to see the changes from modified modules.
 If you modify a Python module other than the ones in the 2 directories
@@ -70,26 +70,26 @@
 .. code-block::
 
     name: srsgui example project using an oscilloscope and a clock generator
 
     inst: cg,  instruments.cg635,   CG635
     inst: osc, instruments.sds1202, SDS1202
 
-    task: *IDN test,    tasks.first,  FirstTask
+    task: \*IDN test,    tasks.first,  FirstTask
     task: Plot example, tasks.second, SecondTask
     ...
 
 
 The keyword 'name:' is use as
 
     - Title of the SRSGUI application main window (Look at the top of
       this :ref:`screen capture <top-of-screen-capture-1>`.
     - Directory name for the project data saving under ~/home/task-results
 
-You can specify a list of instrument classes to be included in the project using 'inst:' keyword.
+You can specify a list instrument classes to be included in the project using 'inst:' keyword.
 The first column after the keyword is the name of the instrument used across the project:
 
     - Menu items under **Instruments** menu. It is used to connect and disconnect
       the selected instrument.
     - Tab labels in Instrument Info panel (in the top left corner under the red STOP button
       in this :ref:`screen capture <top-of-screen-capture-1>`.
     - Name used in terminal to specify a instrument. Make it short if you use a lot
@@ -132,15 +132,15 @@
 
 The keyword 'task:' is used to specify a task class to be used in the configuration file.
 the first column after the 'task:' keyword is the name of the task,
 the second is path to the module, the third one is the name of the task class.
 It specifies a task class in the same way with instrument classes.
 
 When you open a .taskconfig file, in ``srsgui`` application, the names of the tasks
-appear as menu items under the Task menu, as shown at the top of
+appear as menu items under the Task menu (at the top of
 this :ref:`screen capture <top-of-screen-capture-1>`.
 
 You can select one of the task items and run the task.
 
 
 .. _PyVisa: https://pyvisa.readthedocs.io/en/latest/
 .. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/
```

### Comparing `srsgui-0.2.17/doc-source/create-task.rst` & `srsgui-0.2.9/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/define-instrument.rst` & `srsgui-0.2.9/docs/source/define-instrument.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-Defining instrument classes------------------------------an instrument class is a subclass derived from the:class:`Instrument<srsgui.inst.instrument.Instrument>` class.Minimum requirement is to have **_IdString** to check if a connectedinstrument is a correct instrument  that can be used with the class... code-block::    from srsgui import Instrument    class CG635(Instrument):        _IdString = 'CG635'        _term_char = b'\r'  # Add this line if the carriage return is the termination character                            # of the instrument, instead of the line feed (ASCII: 0x10, b'\n').If the instrument has:    1. the **\*IDN?** remote command    2. either RS232 serial communication or Ethernet TCPIP communication port available,the instrument can be connected and used in task scripts and in the terminal,with 4 lines of definition like above. If it does not have the \*IDN? remote command,:meth:`check_id()<srsgui.inst.instrument.Instrument.check_id>` method in Instrumentclass needs to be reimplemented.Available_interfaces^^^^^^^^^^^^^^^^^^^^^`Available_interface` defines what kind of communication is available for the instrument,the base :class:`Instrument<srsgui.inst.instrument.Instrument>` class has the followingdefinition for serial and TCPIP communication interfaces:.. code-block::    available_interfaces = [        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 115200]),                'hardware_flow_control': BoolInput(['Off', 'On'])            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': IntegerInput(23)            }        ]    ]If your instrument needs other than serial and TCPIP interfaces, ``srsgui`` allows to addother communication classes derived from:class:`Interface <srsgui.inst.communication.interface.Interface>` class.Currently there are two external communication interfaces are available from`srsinst.sr860`_ package: ``Vxi11Interface`` and ``VisaInterface``,which covers for VXI11_, GPIB_ and USB-TMC_. You can import the interface modulesfrom `srsinst.sr860`_ .Available_interfaces in SSR865 class is define as following:.. code-block::    available_interfaces = [        [   Vxi11Interface,            {                'ip_address': Ip4Input('192.168.1.10'),            }        ],        [   VisaInterface,            {                'resource': FindListInput(),            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': 23            }        ],        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 19200, 38400, 115200,                                               230400, 460800], 3)            }        ],    ]The definition of available_interfaces is all you need to do to get a customizeddialog box opened for the instrument in ``srsgui`` application... figure:: ./_static/connect-dialog-box-capture.png    :align: center    :figclass: align-centerFor ``VisaInterface``, you have to get PyVISA_ working before running ``srsgui`` application.It involves installation of the PyVISA package and its backend library.Refer to PyVISA_ documentation for installation detail.From Python interpreter, you can connect and use a instrument, once its ``Instrument`` class is defined... code-block::    C:\srsgui>python    Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32    Type "help", "copyright", "credits" or "license" for more information.    >>>    >>> from srsinst.sr860 import SR860    >>> from srsgui import SerialInte    >>> SerialInterface.find()    ['COM3', 'COM4', 'COM256']    >>> lia = SR860('serial','COM4',115200, False)    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34'    >>> lia.disconnect()    >>>    >>> from srsinst.sr860 import VisaInterface    >>> VisaInterface.find()    ['USB0::0xB506::0x2000::002725::INSTR', 'GPIB0::4::INSTR']    >>> lia.connect('visa', 'USB0::0xB506::0x2000::002725::INSTR')    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34\n'    >>>Well, these operations are what you can do with PyVISA_ itself. Defining an instrument class,adding it in a .taskconfig file, and opening it in ``srsgui`` application let youuse the terminal to interact with multiple instrument at once, and use high level ``Instrument``class attributes and methods.Below is an image of terminal captured with the example project opened.As you can see, you can interact with the clock generator and oscilloscope in many ways.There are two commands for osc: \*idn?, sara? used, and two commands for cg:\*idn?, freq(?) used in the terminal... figure:: ./_static/terminal-with-example.png    :align: center    :figclass: align-center|Component, Commands and IndexCommands^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^:class:`Instrument <srsgui.inst.instrument.Instrument>` class uses:class:`Component <srsgui.inst.component.Component>` class,:mod:`Command <srsgui.inst.commands>` classes and:mod:`IndexCommand <srsgui.inst.indexcommands>` classesto organize the functionality of an instrument.If you have to deal with hundreds of remote commands to use an instrument remotely,organizing them in a manageable way is crucial. `Srsinst.sr860`_ package shows how theseconvenience classes are used to organize a large set of remote commands... _PyVisa: https://pyvisa.readthedocs.io/en/latest/.. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/.. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx.. _GPIB: https://en.wikipedia.org/wiki/IEEE-488.. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/.. _thread: https://realpython.com/intro-to-python-threading/.. _QThread: https://doc.qt.io/qt-6/qthread.html
+Defining instrument classes------------------------------an instrument class is a subclass derived from the:class:`Instrument<srsgui.inst.instrument.Instrument>` class.Minimum requirement is to have **_IdString** to check if a connectedinstrument is a correct instrument  that can be used with the class... code-block::    from srsgui import Instrument    class CG635(Instrument):        _IdString = 'CG635'        _term_char = b'\r'  # Add this line if the carriage return is the termination character                            # of the instrument, instead of the line feed (ASCII: 0x10, b'\n').If the instrument has:    1. the **\*IDN?** remote command    2. either RS232 serial communication or Ethernet TCPIP communication port available,the instrument can be connected and used in task scripts and in the terminal,with 4 lines of definition like above. If it does not have the \*IDN? remote command,:meth:`check_id()<srsgui.inst.instrument.Instrument.check_id>` method in Instrumentclass needs to be reimplemented.Available_interfaces^^^^^^^^^^^^^^^^^^^^^`Available_interface` defines what kind of communication is available for the instrument,the base :class:`Instrument<srsgui.inst.instrument.Instrument>` class has the followingdefinition for serial and TCPIP communication interfaces:.. code-block::    available_interfaces = [        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 115200]),                'hardware_flow_control': BoolInput(['Off', 'On'])            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': IntegerInput(23)            }        ]    ]If your instrument needs other than serial and TCPIP interfaces, ``srsgui`` allows to addother communication classes derived from:class:`Interface <srsgui.inst.communication.interface.Interface>` class.Currently there are two external communication interfaces are available from`srsinst.sr860`_ package: ``Vxi11Interface`` and ``VisaInterface``,which covers for VXI11_, GPIB_ and USB-TMC_. You can import the interface modulesfrom `srsinst.sr860`_ .Available_interfaces in SSR865 class is define as following:.. code-block::    available_interfaces = [        [   Vxi11Interface,            {                'ip_address': Ip4Input('192.168.1.10'),            }        ],        [   VisaInterface,            {                'resource': FindListInput(),            }        ],        [   TcpipInterface,            {                'ip_address': Ip4Input('192.168.1.10'),                'port': 23            }        ],        [   SerialInterface,            {                'port': FindListInput(),                'baud_rate': IntegerListInput([9600, 19200, 38400, 115200,                                               230400, 460800], 3)            }        ],    ]The definition of available_interfaces is all you need to do to get a customizeddialog box opened for the instrument in ``srsgui`` application... figure:: ./_static/connect-dialog-box-capture.png    :align: center    :figclass: align-centerFor ``VisaInterface``, you have to get PyVISA_ working before running ``srsgui`` application.It involves installation of the PyVISA package and its backend library.Refer to PyVISA_ documentation for installation detail.From Python interpreter, you can connect and use a instrument, once its ``Instrument`` class is defined... code-block::    C:\srsgui>python    Python 3.8.3 (tags/v3.8.3:6f8c832, May 13 2020, 22:37:02) [MSC v.1924 64 bit (AMD64)] on win32    Type "help", "copyright", "credits" or "license" for more information.    >>>    >>> from srsinst.sr860 import SR865    >>> from srsgui import SerialInte    >>> SerialInterface.find()    ['COM3', 'COM4', 'COM256']    >>> lia = SR865('serial','COM4',115200, False)    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34'    >>> lia.disconnect()    >>>    >>> from srsinst.sr860 import VisaInterface    >>> VisaInterface.find()    ['USB0::0xB506::0x2000::002725::INSTR', 'GPIB0::4::INSTR']    >>> lia.connect('visa', 'USB0::0xB506::0x2000::002725::INSTR')    >>> lia.query_text('*idn?')    'Stanford_Research_Systems,SR865A,002725,v1.34\n'    >>>Well, these operations are what you can do with PyVISA_ itself. Defining an instrument class,adding it in a .taskconfig file, and opening it in ``srsgui`` application let youuse the terminal to interact with multiple instrument at once, and use high level ``Instrument``class attributes and methods.Below is an image of terminal captured with the example project opened.As you can see, you can interact with the clock generator and oscilloscope in many ways.There are two commands for osc: \*idn?, sara? used, and two commands for cg:\*idn?, freq(?) used in the terminal... figure:: ./_static/terminal-with-example.png    :align: center    :figclass: align-center|Component, Commands and IndexCommands^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^:class:`Instrument <srsgui.inst.instrument.Instrument>` class uses:class:`Component <srsgui.inst.component.Component>` class,:mod:`Command <srsgui.inst.commands>` classes and:mod:`IndexCommand <srsgui.inst.indexcommands>` classesto organize the functionality of an instrument.If you have to deal with hundreds of remote commands to use an instrument remotely,organizing them in a manageable way is crucial. `Srsinst.sr860`_ package shows how theseconvenience classes are used to organize a large set of remote commands... _PyVisa: https://pyvisa.readthedocs.io/en/latest/.. _srsinst.sr860: https://pypi.org/project/srsinst.sr860/.. _VXI11: https://www.lxistandard.org/About/VXI-11-and-LXI.aspx.. _GPIB: https://en.wikipedia.org/wiki/IEEE-488.. _USB-TMC: https://www.testandmeasurementtips.com/remote-communication-with-usbtmc-faq/.. _thread: https://realpython.com/intro-to-python-threading/.. _QThread: https://doc.qt.io/qt-6/qthread.html
```

### Comparing `srsgui-0.2.17/doc-source/example.rst` & `srsgui-0.2.9/docs/source/example.rst`

 * *Files 1% similar despite different names*

```diff
@@ -669,310 +669,311 @@
 000029c0: 6566 3a60 6261 7265 2062 6f6e 6520 7374  ef:`bare bone st
 000029d0: 7275 6374 7572 6520 3c74 6f70 2d6f 662d  ructure <top-of-
 000029e0: 6261 7265 2d62 6f6e 652d 7461 736b 3e60  bare-bone-task>`
 000029f0: 0d0a 7368 6f77 6e20 696e 2074 6865 203a  ..shown in the :
 00002a00: 7265 663a 6057 7269 7469 6e67 2061 2074  ref:`Writing a t
 00002a10: 6173 6b20 7363 7269 7074 6020 7365 6374  ask script` sect
 00002a20: 696f 6e2e 0d0a 0d0a 2e2e 206c 6974 6572  ion....... liter
-00002a30: 616c 696e 636c 7564 653a 3a20 2e2e 2f73  alinclude:: ../s
-00002a40: 7273 6775 692f 6578 616d 706c 6573 2f6f  rsgui/examples/o
-00002a50: 7363 696c 6c6f 7363 6f70 6520 6578 616d  scilloscope exam
-00002a60: 706c 652f 7461 736b 732f 6669 7273 742e  ple/tasks/first.
-00002a70: 7079 0d0a 2020 2020 3a6c 616e 6775 6167  py..    :languag
-00002a80: 653a 2050 7974 686f 6e0d 0a20 2020 203a  e: Python..    :
-00002a90: 6c69 6e65 6e6f 733a 0d0a 0d0a 5573 696e  linenos:....Usin
-00002aa0: 6720 2a2a 7365 6c66 2e6c 6f67 6765 722a  g **self.logger*
-00002ab0: 2a20 7365 6e64 7320 7468 6520 6c6f 6767  * sends the logg
-00002ac0: 696e 6720 6f75 7470 7574 2074 6f20 7468  ing output to th
-00002ad0: 6520 636f 6e73 6f6c 6520 7769 6e64 6f77  e console window
-00002ae0: 2c20 7468 6520 6d61 7374 6572 206c 6f67  , the master log
-00002af0: 6769 6e67 2066 696c 6520 696e 0d0a 7e2f  ging file in..~/
-00002b00: 7461 736b 2d72 6573 756c 7473 2064 6972  task-results dir
-00002b10: 6563 746f 7279 2f6d 6169 6e6c 6f67 2d78  ectory/mainlog-x
-00002b20: 782e 7478 742e 782c 2061 6e64 2074 6f20  x.txt.x, and to 
-00002b30: 7468 6520 7461 736b 2072 6573 756c 7420  the task result 
-00002b40: 6461 7461 2066 696c 6520 6c6f 6361 7465  data file locate
-00002b50: 6420 696e 0d0a 7e2f 7461 736b 2d72 6573  d in..~/task-res
-00002b60: 756c 7473 2f70 726f 6a65 6374 2d6e 616d  ults/project-nam
-00002b70: 652d 696e 2d63 6f6e 6669 672d 6669 6c65  e-in-config-file
-00002b80: 2f52 4e78 7878 2064 6972 6563 746f 7279  /RNxxx directory
-00002b90: 2e0d 0a0d 0a57 6974 6820 3a6d 6574 683a  .....With :meth:
-00002ba0: 6067 6574 5f69 6e73 7472 756d 656e 7420  `get_instrument 
-00002bb0: 3c73 7273 6775 692e 7461 736b 2e74 6173  <srsgui.task.tas
-00002bc0: 6b2e 5461 736b 2e67 6574 5f69 6e73 7472  k.Task.get_instr
-00002bd0: 756d 656e 743e 6020 796f 7520 6361 6e20  ument>` you can 
-00002be0: 6765 7420 7468 6520 696e 7374 7275 6d65  get the instrume
-00002bf0: 6e74 0d0a 6465 6669 6e65 6420 696e 2074  nt..defined in t
-00002c00: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-00002c10: 2066 696c 6520 696e 2061 2074 6173 6b2e   file in a task.
-00002c20: 202a 2a44 6f20 6e6f 7420 6469 7363 6f6e   **Do not discon
-00002c30: 6e65 6374 2074 6865 2069 6e73 7472 756d  nect the instrum
-00002c40: 656e 7420 696e 2074 6865 2074 6173 6b21  ent in the task!
-00002c50: 2a2a 0d0a 496e 7374 7275 6d65 6e74 2043  **..Instrument C
-00002c60: 6f6e 6e65 6374 6976 6974 7920 6973 206d  onnectivity is m
-00002c70: 616e 6167 6564 2069 6e20 7468 6520 6170  anaged in the ap
-00002c80: 706c 6963 6174 696f 6e20 6c65 7665 6c2e  plication level.
-00002c90: 0d0a 0d0a 4974 2073 686f 7720 686f 7720  ....It show how 
-00002ca0: 6d75 6368 2069 7420 7369 6d70 6c69 6669  much it simplifi
-00002cb0: 6573 2072 656d 6f74 6520 636f 6d6d 616e  es remote comman
-00002cc0: 6420 7365 7420 616e 6420 7175 6572 7920  d set and query 
-00002cd0: 7472 616e 7361 6374 696f 6e73 2062 7920  transactions by 
-00002ce0: 6465 6669 6e69 6e67 2066 7265 7175 656e  defining frequen
-00002cf0: 6379 0d0a 6174 7472 6962 7574 6520 7573  cy..attribute us
-00002d00: 696e 6720 3a6d 6f64 3a60 7372 7367 7569  ing :mod:`srsgui
-00002d10: 2e69 6e73 742e 636f 6d6d 616e 6473 6020  .inst.commands` 
-00002d20: 6d6f 6475 6c65 2e0d 0a0d 0a53 6563 6f6e  module.....Secon
-00002d30: 6454 6173 6b0d 0a2d 2d2d 2d2d 2d2d 2d2d  dTask..---------
-00002d40: 2d2d 0d0a 0d0a 5468 6520 7365 636f 6e64  --....The second
-00002d50: 2074 6173 6b20 7368 6f77 733a 0d0a 0d0a   task shows:....
-00002d60: 2020 2020 2d20 486f 7720 746f 2064 6566      - How to def
-00002d70: 696e 6520 3a61 7474 723a 6069 6e70 7574  ine :attr:`input
-00002d80: 5f70 6172 616d 6574 6572 7320 3c73 7273  _parameters <srs
-00002d90: 6775 692e 7461 736b 2e74 6173 6b2e 5461  gui.task.task.Ta
-00002da0: 736b 2e69 6e70 7574 5f70 6172 616d 6574  sk.input_paramet
-00002db0: 6572 733e 600d 0a20 2020 2020 2066 6f72  ers>`..      for
-00002dc0: 2069 6e74 6572 6163 7469 7665 2075 7365   interactive use
-00002dd0: 7220 696e 7075 7420 6672 6f6d 2074 6865  r input from the
-00002de0: 2061 7070 6c69 6361 7469 6f6e 2069 6e70   application inp
-00002df0: 7574 2070 616e 656c 0d0a 2020 2020 2d20  ut panel..    - 
-00002e00: 486f 7720 746f 2067 6574 206d 6174 706c  How to get matpl
-00002e10: 6f67 6c69 6220 6669 6775 7265 2061 6e64  oglib figure and
-00002e20: 2075 7365 2069 7420 746f 2070 6c6f 740d   use it to plot.
-00002e30: 0a20 2020 202d 2048 6f77 2074 6f20 7365  .    - How to se
-00002e40: 6e64 2074 6578 7420 6f75 7470 7574 2074  nd text output t
-00002e50: 6f20 7265 7375 6c74 2077 696e 646f 7720  o result window 
-00002e60: 7573 696e 670d 0a20 2020 2020 203a 6d65  using..      :me
-00002e70: 7468 3a60 6469 7370 6c61 795f 7265 7375  th:`display_resu
-00002e80: 6c74 2829 203c 7372 7367 7569 2e74 6173  lt() <srsgui.tas
-00002e90: 6b2e 7461 736b 2e54 6173 6b2e 6469 7370  k.task.Task.disp
-00002ea0: 6c61 795f 7265 7375 6c74 3e60 0d0a 2020  lay_result>`..  
-00002eb0: 2020 2d20 486f 7720 746f 2073 746f 7020    - How to stop 
-00002ec0: 7468 6520 6d61 696e 206c 6f6f 7020 6279  the main loop by
-00002ed0: 2063 6865 636b 696e 670d 0a20 2020 2020   checking..     
-00002ee0: 203a 6d65 7468 3a60 6973 5f72 756e 6e69   :meth:`is_runni
-00002ef0: 6e67 2829 203c 7372 7367 7569 2e74 6173  ng() <srsgui.tas
-00002f00: 6b2e 7461 736b 2e54 6173 6b2e 6973 5f72  k.task.Task.is_r
-00002f10: 756e 6e69 6e67 3e60 2e0d 0a0d 0a2e 2e20  unning>`....... 
-00002f20: 6c69 7465 7261 6c69 6e63 6c75 6465 3a3a  literalinclude::
-00002f30: 202e 2e2f 7372 7367 7569 2f65 7861 6d70   ../srsgui/examp
-00002f40: 6c65 732f 6f73 6369 6c6c 6f73 636f 7065  les/oscilloscope
-00002f50: 2065 7861 6d70 6c65 2f74 6173 6b73 2f73   example/tasks/s
-00002f60: 6563 6f6e 642e 7079 0d0a 2020 2020 3a6c  econd.py..    :l
-00002f70: 616e 6775 6167 653a 2050 7974 686f 6e0d  anguage: Python.
-00002f80: 0a20 2020 203a 6c69 6e65 6e6f 733a 0d0a  .    :linenos:..
-00002f90: 0d0a 5573 696e 6720 6d61 7470 6c6f 746c  ..Using matplotl
-00002fa0: 6962 5f20 6973 2073 7472 6169 6768 7466  ib_ is straightf
-00002fb0: 6f72 7761 7264 2e20 4e6f 2068 6172 6465  orward. No harde
-00002fc0: 7220 7468 616e 2073 7461 6e64 6172 6420  r than standard 
-00002fd0: 706c 6f74 7320 7573 696e 6720 6669 6775  plots using figu
-00002fe0: 7265 7320 616e 6420 6178 6573 2e0d 0a52  res and axes...R
-00002ff0: 6566 6572 2074 6f20 6d61 7470 6c6f 746c  efer to matplotl
-00003000: 6962 5f20 646f 6375 6d65 6e74 6174 696f  ib_ documentatio
-00003010: 6e20 6f6e 2068 6f77 2074 6f20 7573 6520  n on how to use 
-00003020: 6974 2e0d 0a0d 0a54 6865 2069 6d70 6f72  it.....The impor
-00003030: 7461 6e74 2064 6966 6665 7265 6e63 6573  tant differences
-00003040: 2075 7369 6e67 206d 6174 706c 6f74 6c69   using matplotli
-00003050: 6220 696e 2060 6073 7273 6775 6960 6020  b in ``srsgui`` 
-00003060: 6172 653a 0d0a 2020 2020 2d20 596f 7520  are:..    - You 
-00003070: 6861 7665 2074 6f20 6765 7420 7468 6520  have to get the 
-00003080: 6669 6775 7265 2075 7369 6e67 2067 6574  figure using get
-00003090: 5f66 6967 7572 6528 292c 206e 6f74 2063  _figure(), not c
-000030a0: 7265 6174 696e 6720 6f6e 6520 206f 6e20  reating one  on 
-000030b0: 796f 7572 206f 776e 2e0d 0a20 2020 202d  your own...    -
-000030c0: 2059 6f75 2063 7265 6174 6520 706c 6f74   You create plot
-000030d0: 7320 6475 7269 6e67 2073 6574 7570 2829  s during setup()
-000030e0: 2c20 6265 6361 7573 6520 6974 2069 7320  , because it is 
-000030f0: 736c 6f77 2070 726f 6365 7373 2e20 4475  slow process. Du
-00003100: 7269 6e67 2074 6573 7428 292c 0d0a 2020  ring test(),..  
-00003110: 2020 2020 796f 7520 6a75 7374 2075 7064      you just upd
-00003120: 6174 6520 6461 7461 2075 7369 6e67 2073  ate data using s
-00003130: 6574 5f64 6174 6128 2920 6f72 2073 696d  et_data() or sim
-00003140: 696c 6961 7220 6d65 7468 6f64 7320 666f  iliar methods fo
-00003150: 7220 6461 7461 2075 7064 6174 652e 0d0a  r data update...
-00003160: 2020 2020 2d20 596f 7520 6861 7665 2075      - You have u
-00003170: 7365 2072 6571 7565 7374 5f66 6967 7572  se request_figur
-00003180: 655f 7570 6461 7465 2829 2074 6f20 7265  e_update() to re
-00003190: 6472 6177 2074 6865 2070 6c6f 742c 2061  draw the plot, a
-000031a0: 6674 6572 2073 6574 5f64 6174 6128 292e  fter set_data().
-000031b0: 0d0a 2020 2020 2020 5468 6520 6576 656e  ..      The even
-000031c0: 7420 6c6f 6f70 2068 616e 646c 6572 2069  t loop handler i
-000031d0: 6e20 7468 6520 6d61 696e 2061 7070 6c69  n the main appli
-000031e0: 6361 7469 6f6e 2077 696c 6c20 7570 6461  cation will upda
-000031f0: 7465 2074 6865 2070 6c6f 7420 6174 2069  te the plot at i
-00003200: 7473 2065 6172 6c69 6573 740d 0a20 2020  ts earliest..   
-00003210: 2020 2063 6f6e 7665 6e69 656e 6365 2e0d     convenience..
-00003220: 0a0d 0a0d 0a2e 2e20 6669 6775 7265 3a3a  ....... figure::
-00003230: 202e 2f5f 7374 6174 6963 2f73 6563 6f6e   ./_static/secon
-00003240: 642d 7461 736b 2d73 6372 6565 6e2d 6361  d-task-screen-ca
-00003250: 7074 7572 652e 706e 670d 0a20 2020 203a  pture.png..    :
-00003260: 616c 6967 6e3a 2063 656e 7465 720d 0a20  align: center.. 
-00003270: 2020 203a 6669 6763 6c61 7373 3a20 616c     :figclass: al
-00003280: 6967 6e2d 6365 6e74 6572 0d0a 0d0a 7c0d  ign-center....|.
-00003290: 0a0d 0a54 6869 7264 5461 736b 0d0a 2d2d  ...ThirdTask..--
-000032a0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54 6865  ---------....The
-000032b0: 2074 6869 7264 2074 6173 6b20 7573 6573   third task uses
-000032c0: 2074 6865 206f 7363 696c 6c6f 7363 6f70   the oscilloscop
-000032d0: 6520 6f6e 6c79 2e20 4974 2067 6574 7320  e only. It gets 
-000032e0: 7468 6520 6e75 6d62 6572 206f 6620 6361  the number of ca
-000032f0: 7074 7572 6573 2066 726f 6d20 7573 6572  ptures from user
-00003300: 2069 6e70 7574 2c0d 0a72 6570 6561 7420   input,..repeat 
-00003310: 6f73 6369 6c6c 6f73 636f 7065 2077 6176  oscilloscope wav
-00003320: 6566 6f72 6d20 6361 7074 7572 6520 616e  eform capture an
-00003330: 6420 7570 6461 7465 2074 6865 2077 6176  d update the wav
-00003340: 6566 6f72 6d20 706c 6f74 2e20 4974 2073  eform plot. It s
-00003350: 746f 7073 2061 6674 6572 2072 6570 6561  tops after repea
-00003360: 7473 0d0a 7468 6520 6e75 6d62 6572 206f  ts..the number o
-00003370: 6620 7469 6d65 7320 7365 6c65 6374 6564  f times selected
-00003380: 2062 6572 666f 7265 2072 756e 2c20 6f72   berfore run, or
-00003390: 2077 6865 6e20 7468 6520 5374 6f70 2062   when the Stop b
-000033a0: 7574 746f 6e20 6973 2070 7265 7373 7565  utton is pressue
-000033b0: 642e 0d0a 5768 656e 2069 7420 7275 6e73  d...When it runs
-000033c0: 2069 7420 6361 7074 7572 6573 2061 6e64   it captures and
-000033d0: 2064 6973 706c 6179 2061 2077 6176 6566   display a wavef
-000033e0: 6f72 6d20 7769 7468 2037 3030 3030 3020  orm with 700000 
-000033f0: 706f 696e 7473 2065 7665 7279 2030 2e32  points every 0.2
-00003400: 2073 6563 6f6e 640d 0a6f 7665 7220 5443   second..over TC
-00003410: 5049 5020 636f 6d6d 756e 6361 7469 6f6e  PIP communcation
-00003420: 2e0d 0a0d 0a0d 0a2e 2e20 6c69 7465 7261  ......... litera
-00003430: 6c69 6e63 6c75 6465 3a3a 202e 2e2f 7372  linclude:: ../sr
-00003440: 7367 7569 2f65 7861 6d70 6c65 732f 6f73  sgui/examples/os
-00003450: 6369 6c6c 6f73 636f 7065 2065 7861 6d70  cilloscope examp
-00003460: 6c65 2f74 6173 6b73 2f74 6869 7264 2e70  le/tasks/third.p
-00003470: 790d 0a20 2020 203a 6c61 6e67 7561 6765  y..    :language
-00003480: 3a20 5079 7468 6f6e 0d0a 2020 2020 3a6c  : Python..    :l
-00003490: 696e 656e 6f73 3a0d 0a0d 0a46 6f75 7274  inenos:....Fourt
-000034a0: 6854 6173 6b0d 0a2d 2d2d 2d2d 2d2d 2d2d  hTask..---------
-000034b0: 2d2d 0d0a 0d0a 5468 6520 666f 7572 7468  --....The fourth
-000034c0: 2065 7861 6d70 6c65 2069 7320 7468 6520   example is the 
-000034d0: 636c 696d 6178 206f 6620 7468 6520 6578  climax of the ex
-000034e0: 616d 706c 6573 2073 6572 6965 732e 2049  amples series. I
-000034f0: 7420 7573 6573 2069 6e70 7574 5f70 6172  t uses input_par
-00003500: 616d 6574 6572 730d 0a74 6f20 6368 616e  ameters..to chan
-00003510: 6765 206f 7574 7075 7420 6672 6571 7565  ge output freque
-00003520: 6e63 7920 6f66 2074 6865 2063 6c6f 636b  ncy of the clock
-00003530: 2067 656e 6572 6174 6f72 2069 6e74 6572   generator inter
-00003540: 6163 7469 7665 6c79 2c20 6361 7074 7572  actively, captur
-00003550: 6573 2077 6176 6566 6f72 6d73 0d0a 6672  es waveforms..fr
-00003560: 6f6d 2074 6865 206f 7363 696c 6c6f 7363  om the oscillosc
-00003570: 6f70 652c 2072 756e 2046 4654 206f 6620  ope, run FFT of 
-00003580: 7468 6520 7761 7665 666f 726d 7320 7769  the waveforms wi
-00003590: 7468 204e 756d 7079 2c20 616e 6420 706c  th Numpy, and pl
-000035a0: 6f74 0d0a 7573 696e 6720 3220 6d61 7470  ot..using 2 matp
-000035b0: 6c6f 746c 6962 2066 6967 7572 6573 2e0d  lotlib figures..
-000035c0: 0a0d 0a62 7920 6164 6469 6e67 2074 6865  ...by adding the
-000035d0: 206e 616d 6573 206f 6620 6669 6775 7265   names of figure
-000035e0: 7320 7468 6174 2079 6f75 2077 616e 7420  s that you want 
-000035f0: 746f 2075 7365 2069 6e20 6164 6469 7469  to use in additi
-00003600: 6f6e 616c 5f66 6967 7572 655f 6e61 6d65  onal_figure_name
-00003610: 732c 0d0a 6060 7372 7367 7569 6060 2070  s,..``srsgui`` p
-00003620: 726f 7669 6465 7320 6d6f 7265 2066 6967  rovides more fig
-00003630: 7572 6573 2074 6f20 7468 6520 7461 736b  ures to the task
-00003640: 2062 6566 6f72 6520 6974 2073 7461 7274   before it start
-00003650: 732e 0d0a 0d0a 2e2e 206c 6974 6572 616c  s....... literal
-00003660: 696e 636c 7564 653a 3a20 2e2e 2f73 7273  include:: ../srs
-00003670: 6775 692f 6578 616d 706c 6573 2f6f 7363  gui/examples/osc
-00003680: 696c 6c6f 7363 6f70 6520 6578 616d 706c  illoscope exampl
-00003690: 652f 7461 736b 732f 666f 7572 7468 2e70  e/tasks/fourth.p
-000036a0: 790d 0a20 2020 203a 6c61 6e67 7561 6765  y..    :language
-000036b0: 3a20 5079 7468 6f6e 0d0a 2020 2020 3a6c  : Python..    :l
-000036c0: 696e 656e 6f73 3a0d 0a0d 0a46 6966 7468  inenos:....Fifth
-000036d0: 5461 736b 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  Task..----------
-000036e0: 0d0a 0d0a 7468 6520 6669 6674 6820 6578  ....the fifth ex
-000036f0: 616d 706c 6573 2069 7320 746f 2073 686f  amples is to sho
-00003700: 7720 686f 7720 746f 2073 7562 636c 6173  w how to subclas
-00003710: 7320 616e 2065 7869 7374 696e 6720 7461  s an existing ta
-00003720: 736b 2063 6c61 7373 2074 6f20 7265 7573  sk class to reus
-00003730: 652e 0d0a 7468 6520 6d65 7468 6f64 2067  e...the method g
-00003740: 6574 5f77 6176 6566 6f72 6d28 2920 696e  et_waveform() in
-00003750: 2074 6865 2066 6f75 7274 6820 6578 616d   the fourth exam
-00003760: 706c 6520 6973 2072 6569 6d70 6c65 6d65  ple is reimpleme
-00003770: 6e74 6564 2074 6f20 6765 6e65 7261 7465  nted to generate
-00003780: 0d0a 7369 6d75 6c61 7465 6420 7761 7665  ..simulated wave
-00003790: 666f 726d 2074 6861 7420 7275 6e73 2077  form that runs w
-000037a0: 6974 686f 7574 2061 6e79 2072 6561 6c20  ithout any real 
-000037b0: 6f73 6369 6c6c 6f73 636f 7065 2e0d 0a0d  oscilloscope....
-000037c0: 0a4e 6f74 6520 7468 6174 2074 6865 2073  .Note that the s
-000037d0: 7175 6172 6520 7761 7665 2065 6467 6520  quare wave edge 
-000037e0: 6361 6c63 756c 6174 696f 6e20 6973 2063  calculation is c
-000037f0: 7275 6465 2c20 616e 6420 6361 7573 696e  rude, and causin
-00003800: 6720 6d6f 6475 6c61 7469 6f6e 2069 6e20  g modulation in 
-00003810: 7075 6c73 6520 7769 6474 680d 0a74 6861  pulse width..tha
-00003820: 7420 7368 6f77 7320 7369 6465 2062 616e  t shows side ban
-00003830: 6473 2069 6e20 4646 5420 7370 6563 7472  ds in FFT spectr
-00003840: 756d 2c20 6966 2074 6865 2073 6574 2066  um, if the set f
-00003850: 7265 7175 656e 6379 2069 7320 6e6f 7420  requency is not 
-00003860: 636f 6d6d 656e 7375 7261 7465 6420 7769  commensurated wi
-00003870: 7468 0d0a 7468 6520 7361 6d70 6c69 6e67  th..the sampling
-00003880: 2072 6174 652e 2054 6f20 6765 6e65 7261   rate. To genera
-00003890: 7465 2063 6c65 616e 2073 7175 6172 6520  te clean square 
-000038a0: 7761 7665 2c20 7468 6520 7269 7369 6e67  wave, the rising
-000038b0: 2061 6e64 2066 616c 6c69 6e67 2065 6467   and falling edg
-000038c0: 6573 2073 686f 756c 640d 0a68 6176 6520  es should..have 
-000038d0: 6174 206c 6561 7374 2074 776f 2070 6f69  at least two poi
-000038e0: 6e74 7320 746f 2072 6570 7265 7365 6e74  nts to represent
-000038f0: 2065 7861 6374 2070 6861 7365 2e20 4469   exact phase. Di
-00003900: 7265 6374 2074 7261 6e73 6974 696f 6e20  rect transition 
-00003910: 6672 6f6d 206c 6f77 2074 6f20 6869 6768  from low to high
-00003920: 0d0a 7769 7468 6f75 7420 616e 7920 696e  ..without any in
-00003930: 7465 726d 6564 6961 7465 2070 6f69 6e74  termediate point
-00003940: 7320 7375 6666 6572 7320 6672 6f6d 2073  s suffers from s
-00003950: 7562 746c 6520 6d6f 6475 6c61 7469 6f6e  ubtle modulation
-00003960: 2069 6e20 7469 6d65 2064 6f6d 6169 6e2c   in time domain,
-00003970: 0d0a 7768 6963 6820 6d61 6e69 6665 7374  ..which manifest
-00003980: 7320 6173 2073 6964 6520 6261 6e64 7320  s as side bands 
-00003990: 696e 2046 4654 2e20 5468 6973 2069 7320  in FFT. This is 
-000039a0: 6120 636f 6d6d 6f6e 2070 726f 626c 656d  a common problem
-000039b0: 2069 6e20 6469 6769 7461 6c20 7369 676e   in digital sign
-000039c0: 616c 0d0a 7072 6f63 6573 7369 6e67 2e20  al..processing. 
-000039d0: 4974 2069 7320 6e6f 7420 6120 7072 6f62  It is not a prob
-000039e0: 6c65 6d20 696e 2074 6865 2072 6561 6c20  lem in the real 
-000039f0: 776f 726c 642c 2062 6563 6175 7365 2074  world, because t
-00003a00: 6865 2073 6967 6e61 6c20 6973 2061 6e61  he signal is ana
-00003a10: 6c6f 672c 0d0a 616e 6420 7468 6520 7361  log,..and the sa
-00003a20: 6d70 6c69 6e67 2072 6174 6520 6973 206c  mpling rate is l
-00003a30: 696d 6974 6564 2062 7920 7468 6520 6261  imited by the ba
-00003a40: 6e64 7769 6474 6820 6f66 2074 6865 2073  ndwidth of the s
-00003a50: 6967 6e61 6c2e 0d0a 0d0a 0d0a 2e2e 206c  ignal......... l
-00003a60: 6974 6572 616c 696e 636c 7564 653a 3a20  iteralinclude:: 
-00003a70: 2e2e 2f73 7273 6775 692f 6578 616d 706c  ../srsgui/exampl
-00003a80: 6573 2f6f 7363 696c 6c6f 7363 6f70 6520  es/oscilloscope 
-00003a90: 6578 616d 706c 652f 7461 736b 732f 666f  example/tasks/fo
-00003aa0: 7572 7468 2e70 790d 0a20 2020 203a 6c61  urth.py..    :la
-00003ab0: 6e67 7561 6765 3a20 5079 7468 6f6e 0d0a  nguage: Python..
-00003ac0: 2020 2020 3a6c 696e 656e 6f73 3a0d 0a0d      :linenos:...
-00003ad0: 0a0d 0a0d 0a2e 2e20 5f50 7956 6973 613a  ....... _PyVisa:
-00003ae0: 2068 7474 7073 3a2f 2f70 7976 6973 612e   https://pyvisa.
-00003af0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00003b00: 6e2f 6c61 7465 7374 2f0d 0a2e 2e20 5f73  n/latest/.... _s
-00003b10: 7273 696e 7374 2e73 7238 3630 3a20 6874  rsinst.sr860: ht
-00003b20: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00003b30: 726f 6a65 6374 2f73 7273 696e 7374 2e73  roject/srsinst.s
-00003b40: 7238 3630 2f0d 0a2e 2e20 5f56 5849 3131  r860/.... _VXI11
-00003b50: 3a20 6874 7470 733a 2f2f 7777 772e 6c78  : https://www.lx
-00003b60: 6973 7461 6e64 6172 642e 6f72 672f 4162  istandard.org/Ab
-00003b70: 6f75 742f 5658 492d 3131 2d61 6e64 2d4c  out/VXI-11-and-L
-00003b80: 5849 2e61 7370 780d 0a2e 2e20 5f47 5049  XI.aspx.... _GPI
-00003b90: 423a 2068 7474 7073 3a2f 2f65 6e2e 7769  B: https://en.wi
-00003ba0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00003bb0: 2f49 4545 452d 3438 380d 0a2e 2e20 5f55  /IEEE-488.... _U
-00003bc0: 5342 2d54 4d43 3a20 6874 7470 733a 2f2f  SB-TMC: https://
-00003bd0: 7777 772e 7465 7374 616e 646d 6561 7375  www.testandmeasu
-00003be0: 7265 6d65 6e74 7469 7073 2e63 6f6d 2f72  rementtips.com/r
-00003bf0: 656d 6f74 652d 636f 6d6d 756e 6963 6174  emote-communicat
-00003c00: 696f 6e2d 7769 7468 2d75 7362 746d 632d  ion-with-usbtmc-
-00003c10: 6661 712f 0d0a 2e2e 205f 5344 5331 3230  faq/.... _SDS120
-00003c20: 3258 453a 2068 7474 7073 3a2f 2f73 6967  2XE: https://sig
-00003c30: 6c65 6e74 6e61 2e63 6f6d 2f70 726f 6475  lentna.com/produ
-00003c40: 6374 2f73 6473 3132 3032 782d 652f 0d0a  ct/sds1202x-e/..
-00003c50: 2e2e 205f 5352 533a 2068 7474 7073 3a2f  .. _SRS: https:/
-00003c60: 2f74 6869 6e6b 7372 732e 636f 6d2f 0d0a  /thinksrs.com/..
-00003c70: 2e2e 205f 4347 3633 353a 2068 7474 7073  .. _CG635: https
-00003c80: 3a2f 2f74 6869 6e6b 7372 732e 636f 6d2f  ://thinksrs.com/
-00003c90: 7072 6f64 7563 7473 2f63 6736 3335 2e68  products/cg635.h
-00003ca0: 746d 6c0d 0a2e 2e20 5f6c 6f67 6769 6e67  tml.... _logging
-00003cb0: 3a20 6874 7470 733a 2f2f 646f 6373 2e70  : https://docs.p
-00003cc0: 7974 686f 6e2e 6f72 672f 332f 686f 7774  ython.org/3/howt
-00003cd0: 6f2f 6c6f 6767 696e 672e 6874 6d6c 0d0a  o/logging.html..
-00003ce0: 2e2e 205f 6d61 7470 6c6f 746c 6962 3a20  .. _matplotlib: 
-00003cf0: 6874 7470 733a 2f2f 6d61 7470 6c6f 746c  https://matplotl
-00003d00: 6962 2e6f 7267 2f73 7461 626c 652f 696e  ib.org/stable/in
-00003d10: 6465 782e 6874 6d6c                      dex.html
+00002a30: 616c 696e 636c 7564 653a 3a20 2e2e 2f2e  alinclude:: ../.
+00002a40: 2e2f 7372 7367 7569 2f65 7861 6d70 6c65  ./srsgui/example
+00002a50: 732f 6f73 6369 6c6c 6f73 636f 7065 2065  s/oscilloscope e
+00002a60: 7861 6d70 6c65 2f74 6173 6b73 2f66 6972  xample/tasks/fir
+00002a70: 7374 2e70 790d 0a20 2020 203a 6c61 6e67  st.py..    :lang
+00002a80: 7561 6765 3a20 5079 7468 6f6e 0d0a 2020  uage: Python..  
+00002a90: 2020 3a6c 696e 656e 6f73 3a0d 0a0d 0a55    :linenos:....U
+00002aa0: 7369 6e67 202a 2a73 656c 662e 6c6f 6767  sing **self.logg
+00002ab0: 6572 2a2a 2073 656e 6473 2074 6865 206c  er** sends the l
+00002ac0: 6f67 6769 6e67 206f 7574 7075 7420 746f  ogging output to
+00002ad0: 2074 6865 2063 6f6e 736f 6c65 2077 696e   the console win
+00002ae0: 646f 772c 2074 6865 206d 6173 7465 7220  dow, the master 
+00002af0: 6c6f 6767 696e 6720 6669 6c65 2069 6e0d  logging file in.
+00002b00: 0a7e 2f74 6173 6b2d 7265 7375 6c74 7320  .~/task-results 
+00002b10: 6469 7265 6374 6f72 792f 6d61 696e 6c6f  directory/mainlo
+00002b20: 672d 7878 2e74 7874 2e78 2c20 616e 6420  g-xx.txt.x, and 
+00002b30: 746f 2074 6865 2074 6173 6b20 7265 7375  to the task resu
+00002b40: 6c74 2064 6174 6120 6669 6c65 206c 6f63  lt data file loc
+00002b50: 6174 6564 2069 6e0d 0a7e 2f74 6173 6b2d  ated in..~/task-
+00002b60: 7265 7375 6c74 732f 7072 6f6a 6563 742d  results/project-
+00002b70: 6e61 6d65 2d69 6e2d 636f 6e66 6967 2d66  name-in-config-f
+00002b80: 696c 652f 524e 7878 7820 6469 7265 6374  ile/RNxxx direct
+00002b90: 6f72 792e 0d0a 0d0a 5769 7468 203a 6d65  ory.....With :me
+00002ba0: 7468 3a60 6765 745f 696e 7374 7275 6d65  th:`get_instrume
+00002bb0: 6e74 203c 7372 7367 7569 2e74 6173 6b2e  nt <srsgui.task.
+00002bc0: 7461 736b 2e54 6173 6b2e 6765 745f 696e  task.Task.get_in
+00002bd0: 7374 7275 6d65 6e74 3e60 2079 6f75 2063  strument>` you c
+00002be0: 616e 2067 6574 2074 6865 2069 6e73 7472  an get the instr
+00002bf0: 756d 656e 740d 0a64 6566 696e 6564 2069  ument..defined i
+00002c00: 6e20 7468 6520 636f 6e66 6967 7572 6174  n the configurat
+00002c10: 696f 6e20 6669 6c65 2069 6e20 6120 7461  ion file in a ta
+00002c20: 736b 2e20 2a2a 446f 206e 6f74 2064 6973  sk. **Do not dis
+00002c30: 636f 6e6e 6563 7420 7468 6520 696e 7374  connect the inst
+00002c40: 7275 6d65 6e74 2069 6e20 7468 6520 7461  rument in the ta
+00002c50: 736b 212a 2a0d 0a49 6e73 7472 756d 656e  sk!**..Instrumen
+00002c60: 7420 436f 6e6e 6563 7469 7669 7479 2069  t Connectivity i
+00002c70: 7320 6d61 6e61 6765 6420 696e 2074 6865  s managed in the
+00002c80: 2061 7070 6c69 6361 7469 6f6e 206c 6576   application lev
+00002c90: 656c 2e0d 0a0d 0a49 7420 7368 6f77 2068  el.....It show h
+00002ca0: 6f77 206d 7563 6820 6974 2073 696d 706c  ow much it simpl
+00002cb0: 6966 6965 7320 7265 6d6f 7465 2063 6f6d  ifies remote com
+00002cc0: 6d61 6e64 2073 6574 2061 6e64 2071 7565  mand set and que
+00002cd0: 7279 2074 7261 6e73 6163 7469 6f6e 7320  ry transactions 
+00002ce0: 6279 2064 6566 696e 696e 6720 6672 6571  by defining freq
+00002cf0: 7565 6e63 790d 0a61 7474 7269 6275 7465  uency..attribute
+00002d00: 2075 7369 6e67 203a 6d6f 643a 6073 7273   using :mod:`srs
+00002d10: 6775 692e 696e 7374 2e63 6f6d 6d61 6e64  gui.inst.command
+00002d20: 7360 206d 6f64 756c 652e 0d0a 0d0a 5365  s` module.....Se
+00002d30: 636f 6e64 5461 736b 0d0a 2d2d 2d2d 2d2d  condTask..------
+00002d40: 2d2d 2d2d 2d0d 0a0d 0a54 6865 2073 6563  -----....The sec
+00002d50: 6f6e 6420 7461 736b 2073 686f 7773 3a0d  ond task shows:.
+00002d60: 0a0d 0a20 2020 202d 2048 6f77 2074 6f20  ...    - How to 
+00002d70: 6465 6669 6e65 203a 6174 7472 3a60 696e  define :attr:`in
+00002d80: 7075 745f 7061 7261 6d65 7465 7273 203c  put_parameters <
+00002d90: 7372 7367 7569 2e74 6173 6b2e 7461 736b  srsgui.task.task
+00002da0: 2e54 6173 6b2e 696e 7075 745f 7061 7261  .Task.input_para
+00002db0: 6d65 7465 7273 3e60 0d0a 2020 2020 2020  meters>`..      
+00002dc0: 666f 7220 696e 7465 7261 6374 6976 6520  for interactive 
+00002dd0: 7573 6572 2069 6e70 7574 2066 726f 6d20  user input from 
+00002de0: 7468 6520 6170 706c 6963 6174 696f 6e20  the application 
+00002df0: 696e 7075 7420 7061 6e65 6c0d 0a20 2020  input panel..   
+00002e00: 202d 2048 6f77 2074 6f20 6765 7420 6d61   - How to get ma
+00002e10: 7470 6c6f 676c 6962 2066 6967 7572 6520  tploglib figure 
+00002e20: 616e 6420 7573 6520 6974 2074 6f20 706c  and use it to pl
+00002e30: 6f74 0d0a 2020 2020 2d20 486f 7720 746f  ot..    - How to
+00002e40: 2073 656e 6420 7465 7874 206f 7574 7075   send text outpu
+00002e50: 7420 746f 2072 6573 756c 7420 7769 6e64  t to result wind
+00002e60: 6f77 2075 7369 6e67 0d0a 2020 2020 2020  ow using..      
+00002e70: 3a6d 6574 683a 6064 6973 706c 6179 5f72  :meth:`display_r
+00002e80: 6573 756c 7428 2920 3c73 7273 6775 692e  esult() <srsgui.
+00002e90: 7461 736b 2e74 6173 6b2e 5461 736b 2e64  task.task.Task.d
+00002ea0: 6973 706c 6179 5f72 6573 756c 743e 600d  isplay_result>`.
+00002eb0: 0a20 2020 202d 2048 6f77 2074 6f20 7374  .    - How to st
+00002ec0: 6f70 2074 6865 206d 6169 6e20 6c6f 6f70  op the main loop
+00002ed0: 2062 7920 6368 6563 6b69 6e67 0d0a 2020   by checking..  
+00002ee0: 2020 2020 3a6d 6574 683a 6069 735f 7275      :meth:`is_ru
+00002ef0: 6e6e 696e 6728 2920 3c73 7273 6775 692e  nning() <srsgui.
+00002f00: 7461 736b 2e74 6173 6b2e 5461 736b 2e69  task.task.Task.i
+00002f10: 735f 7275 6e6e 696e 673e 602e 0d0a 0d0a  s_running>`.....
+00002f20: 2e2e 206c 6974 6572 616c 696e 636c 7564  .. literalinclud
+00002f30: 653a 3a20 2e2e 2f2e 2e2f 7372 7367 7569  e:: ../../srsgui
+00002f40: 2f65 7861 6d70 6c65 732f 6f73 6369 6c6c  /examples/oscill
+00002f50: 6f73 636f 7065 2065 7861 6d70 6c65 2f74  oscope example/t
+00002f60: 6173 6b73 2f73 6563 6f6e 642e 7079 0d0a  asks/second.py..
+00002f70: 2020 2020 3a6c 616e 6775 6167 653a 2050      :language: P
+00002f80: 7974 686f 6e0d 0a20 2020 203a 6c69 6e65  ython..    :line
+00002f90: 6e6f 733a 0d0a 0d0a 5573 696e 6720 6d61  nos:....Using ma
+00002fa0: 7470 6c6f 746c 6962 5f20 6973 2073 7472  tplotlib_ is str
+00002fb0: 6169 6768 7466 6f72 7761 7264 2e20 4e6f  aightforward. No
+00002fc0: 2068 6172 6465 7220 7468 616e 2073 7461   harder than sta
+00002fd0: 6e64 6172 6420 706c 6f74 7320 7573 696e  ndard plots usin
+00002fe0: 6720 6669 6775 7265 7320 616e 6420 6178  g figures and ax
+00002ff0: 6573 2e0d 0a52 6566 6572 2074 6f20 6d61  es...Refer to ma
+00003000: 7470 6c6f 746c 6962 5f20 646f 6375 6d65  tplotlib_ docume
+00003010: 6e74 6174 696f 6e20 6f6e 2068 6f77 2074  ntation on how t
+00003020: 6f20 7573 6520 6974 2e0d 0a0d 0a54 6865  o use it.....The
+00003030: 2069 6d70 6f72 7461 6e74 2064 6966 6665   important diffe
+00003040: 7265 6e63 6573 2075 7369 6e67 206d 6174  rences using mat
+00003050: 706c 6f74 6c69 6220 696e 2060 6073 7273  plotlib in ``srs
+00003060: 6775 6960 6020 6172 653a 0d0a 2020 2020  gui`` are:..    
+00003070: 2d20 596f 7520 6861 7665 2074 6f20 6765  - You have to ge
+00003080: 7420 7468 6520 6669 6775 7265 2075 7369  t the figure usi
+00003090: 6e67 2067 6574 5f66 6967 7572 6528 292c  ng get_figure(),
+000030a0: 206e 6f74 2063 7265 6174 696e 6720 6f6e   not creating on
+000030b0: 6520 206f 6e20 796f 7572 206f 776e 2e0d  e  on your own..
+000030c0: 0a20 2020 202d 2059 6f75 2063 7265 6174  .    - You creat
+000030d0: 6520 706c 6f74 7320 6475 7269 6e67 2073  e plots during s
+000030e0: 6574 7570 2829 2c20 6265 6361 7573 6520  etup(), because 
+000030f0: 6974 2069 7320 736c 6f77 2070 726f 6365  it is slow proce
+00003100: 7373 2e20 4475 7269 6e67 2074 6573 7428  ss. During test(
+00003110: 292c 0d0a 2020 2020 2020 796f 7520 6a75  ),..      you ju
+00003120: 7374 2075 7064 6174 6520 6461 7461 2075  st update data u
+00003130: 7369 6e67 2073 6574 5f64 6174 6128 2920  sing set_data() 
+00003140: 6f72 2073 696d 696c 6961 7220 6d65 7468  or similiar meth
+00003150: 6f64 7320 666f 7220 6461 7461 2075 7064  ods for data upd
+00003160: 6174 652e 0d0a 2020 2020 2d20 596f 7520  ate...    - You 
+00003170: 6861 7665 2075 7365 2072 6571 7565 7374  have use request
+00003180: 5f66 6967 7572 655f 7570 6461 7465 2829  _figure_update()
+00003190: 2074 6f20 7265 6472 6177 2074 6865 2070   to redraw the p
+000031a0: 6c6f 742c 2061 6674 6572 2073 6574 5f64  lot, after set_d
+000031b0: 6174 6128 292e 0d0a 2020 2020 2020 5468  ata()...      Th
+000031c0: 6520 6576 656e 7420 6c6f 6f70 2068 616e  e event loop han
+000031d0: 646c 6572 2069 6e20 7468 6520 6d61 696e  dler in the main
+000031e0: 2061 7070 6c69 6361 7469 6f6e 2077 696c   application wil
+000031f0: 6c20 7570 6461 7465 2074 6865 2070 6c6f  l update the plo
+00003200: 7420 6174 2069 7473 2065 6172 6c69 6573  t at its earlies
+00003210: 740d 0a20 2020 2020 2063 6f6e 7665 6e69  t..      conveni
+00003220: 656e 6365 2e0d 0a0d 0a0d 0a2e 2e20 6669  ence......... fi
+00003230: 6775 7265 3a3a 202e 2f5f 7374 6174 6963  gure:: ./_static
+00003240: 2f73 6563 6f6e 642d 7461 736b 2d73 6372  /second-task-scr
+00003250: 6565 6e2d 6361 7074 7572 652e 706e 670d  een-capture.png.
+00003260: 0a20 2020 203a 616c 6967 6e3a 2063 656e  .    :align: cen
+00003270: 7465 720d 0a20 2020 203a 6669 6763 6c61  ter..    :figcla
+00003280: 7373 3a20 616c 6967 6e2d 6365 6e74 6572  ss: align-center
+00003290: 0d0a 0d0a 7c0d 0a0d 0a54 6869 7264 5461  ....|....ThirdTa
+000032a0: 736b 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d  sk..-----------.
+000032b0: 0a0d 0a54 6865 2074 6869 7264 2074 6173  ...The third tas
+000032c0: 6b20 7573 6573 2074 6865 206f 7363 696c  k uses the oscil
+000032d0: 6c6f 7363 6f70 6520 6f6e 6c79 2e20 4974  loscope only. It
+000032e0: 2067 6574 7320 7468 6520 6e75 6d62 6572   gets the number
+000032f0: 206f 6620 6361 7074 7572 6573 2066 726f   of captures fro
+00003300: 6d20 7573 6572 2069 6e70 7574 2c0d 0a72  m user input,..r
+00003310: 6570 6561 7420 6f73 6369 6c6c 6f73 636f  epeat oscillosco
+00003320: 7065 2077 6176 6566 6f72 6d20 6361 7074  pe waveform capt
+00003330: 7572 6520 616e 6420 7570 6461 7465 2074  ure and update t
+00003340: 6865 2077 6176 6566 6f72 6d20 706c 6f74  he waveform plot
+00003350: 2e20 4974 2073 746f 7073 2061 6674 6572  . It stops after
+00003360: 2072 6570 6561 7473 0d0a 7468 6520 6e75   repeats..the nu
+00003370: 6d62 6572 206f 6620 7469 6d65 7320 7365  mber of times se
+00003380: 6c65 6374 6564 2062 6572 666f 7265 2072  lected berfore r
+00003390: 756e 2c20 6f72 2077 6865 6e20 7468 6520  un, or when the 
+000033a0: 5374 6f70 2062 7574 746f 6e20 6973 2070  Stop button is p
+000033b0: 7265 7373 7565 642e 0d0a 5768 656e 2069  ressued...When i
+000033c0: 7420 7275 6e73 2069 7420 6361 7074 7572  t runs it captur
+000033d0: 6573 2061 6e64 2064 6973 706c 6179 2061  es and display a
+000033e0: 2077 6176 6566 6f72 6d20 7769 7468 2037   waveform with 7
+000033f0: 3030 3030 3020 706f 696e 7473 2065 7665  00000 points eve
+00003400: 7279 2030 2e32 2073 6563 6f6e 640d 0a6f  ry 0.2 second..o
+00003410: 7665 7220 5443 5049 5020 636f 6d6d 756e  ver TCPIP commun
+00003420: 6361 7469 6f6e 2e0d 0a0d 0a0d 0a2e 2e20  cation......... 
+00003430: 6c69 7465 7261 6c69 6e63 6c75 6465 3a3a  literalinclude::
+00003440: 202e 2e2f 2e2e 2f73 7273 6775 692f 6578   ../../srsgui/ex
+00003450: 616d 706c 6573 2f6f 7363 696c 6c6f 7363  amples/oscillosc
+00003460: 6f70 6520 6578 616d 706c 652f 7461 736b  ope example/task
+00003470: 732f 7468 6972 642e 7079 0d0a 2020 2020  s/third.py..    
+00003480: 3a6c 616e 6775 6167 653a 2050 7974 686f  :language: Pytho
+00003490: 6e0d 0a20 2020 203a 6c69 6e65 6e6f 733a  n..    :linenos:
+000034a0: 0d0a 0d0a 466f 7572 7468 5461 736b 0d0a  ....FourthTask..
+000034b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54  -----------....T
+000034c0: 6865 2066 6f75 7274 6820 6578 616d 706c  he fourth exampl
+000034d0: 6520 6973 2074 6865 2063 6c69 6d61 7820  e is the climax 
+000034e0: 6f66 2074 6865 2065 7861 6d70 6c65 7320  of the examples 
+000034f0: 7365 7269 6573 2e20 4974 2075 7365 7320  series. It uses 
+00003500: 696e 7075 745f 7061 7261 6d65 7465 7273  input_parameters
+00003510: 0d0a 746f 2063 6861 6e67 6520 6f75 7470  ..to change outp
+00003520: 7574 2066 7265 7175 656e 6379 206f 6620  ut frequency of 
+00003530: 7468 6520 636c 6f63 6b20 6765 6e65 7261  the clock genera
+00003540: 746f 7220 696e 7465 7261 6374 6976 656c  tor interactivel
+00003550: 792c 2063 6170 7475 7265 7320 7761 7665  y, captures wave
+00003560: 666f 726d 730d 0a66 726f 6d20 7468 6520  forms..from the 
+00003570: 6f73 6369 6c6c 6f73 636f 7065 2c20 7275  oscilloscope, ru
+00003580: 6e20 4646 5420 6f66 2074 6865 2077 6176  n FFT of the wav
+00003590: 6566 6f72 6d73 2077 6974 6820 4e75 6d70  eforms with Nump
+000035a0: 792c 2061 6e64 2070 6c6f 740d 0a75 7369  y, and plot..usi
+000035b0: 6e67 2032 206d 6174 706c 6f74 6c69 6220  ng 2 matplotlib 
+000035c0: 6669 6775 7265 732e 0d0a 0d0a 6279 2061  figures.....by a
+000035d0: 6464 696e 6720 7468 6520 6e61 6d65 7320  dding the names 
+000035e0: 6f66 2066 6967 7572 6573 2074 6861 7420  of figures that 
+000035f0: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
+00003600: 696e 2061 6464 6974 696f 6e61 6c5f 6669  in additional_fi
+00003610: 6775 7265 5f6e 616d 6573 2c0d 0a60 6073  gure_names,..``s
+00003620: 7273 6775 6960 6020 7072 6f76 6964 6573  rsgui`` provides
+00003630: 206d 6f72 6520 6669 6775 7265 7320 746f   more figures to
+00003640: 2074 6865 2074 6173 6b20 6265 666f 7265   the task before
+00003650: 2069 7420 7374 6172 7473 2e0d 0a0d 0a2e   it starts......
+00003660: 2e20 6c69 7465 7261 6c69 6e63 6c75 6465  . literalinclude
+00003670: 3a3a 202e 2e2f 2e2e 2f73 7273 6775 692f  :: ../../srsgui/
+00003680: 6578 616d 706c 6573 2f6f 7363 696c 6c6f  examples/oscillo
+00003690: 7363 6f70 6520 6578 616d 706c 652f 7461  scope example/ta
+000036a0: 736b 732f 666f 7572 7468 2e70 790d 0a20  sks/fourth.py.. 
+000036b0: 2020 203a 6c61 6e67 7561 6765 3a20 5079     :language: Py
+000036c0: 7468 6f6e 0d0a 2020 2020 3a6c 696e 656e  thon..    :linen
+000036d0: 6f73 3a0d 0a0d 0a46 6966 7468 5461 736b  os:....FifthTask
+000036e0: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ..----------....
+000036f0: 7468 6520 6669 6674 6820 6578 616d 706c  the fifth exampl
+00003700: 6573 2069 7320 746f 2073 686f 7720 686f  es is to show ho
+00003710: 7720 746f 2073 7562 636c 6173 7320 616e  w to subclass an
+00003720: 2065 7869 7374 696e 6720 7461 736b 2063   existing task c
+00003730: 6c61 7373 2074 6f20 7265 7573 652e 0d0a  lass to reuse...
+00003740: 7468 6520 6d65 7468 6f64 2067 6574 5f77  the method get_w
+00003750: 6176 6566 6f72 6d28 2920 696e 2074 6865  aveform() in the
+00003760: 2066 6f75 7274 6820 6578 616d 706c 6520   fourth example 
+00003770: 6973 2072 6569 6d70 6c65 6d65 6e74 6564  is reimplemented
+00003780: 2074 6f20 6765 6e65 7261 7465 0d0a 7369   to generate..si
+00003790: 6d75 6c61 7465 6420 7761 7665 666f 726d  mulated waveform
+000037a0: 2074 6861 7420 7275 6e73 2077 6974 686f   that runs witho
+000037b0: 7574 2061 6e79 2072 6561 6c20 6f73 6369  ut any real osci
+000037c0: 6c6c 6f73 636f 7065 2e0d 0a0d 0a4e 6f74  lloscope.....Not
+000037d0: 6520 7468 6174 2074 6865 2073 7175 6172  e that the squar
+000037e0: 6520 7761 7665 2065 6467 6520 6361 6c63  e wave edge calc
+000037f0: 756c 6174 696f 6e20 6973 2063 7275 6465  ulation is crude
+00003800: 2c20 616e 6420 6361 7573 696e 6720 6d6f  , and causing mo
+00003810: 6475 6c61 7469 6f6e 2069 6e20 7075 6c73  dulation in puls
+00003820: 6520 7769 6474 680d 0a74 6861 7420 7368  e width..that sh
+00003830: 6f77 7320 7369 6465 2062 616e 6473 2069  ows side bands i
+00003840: 6e20 4646 5420 7370 6563 7472 756d 2c20  n FFT spectrum, 
+00003850: 6966 2074 6865 2073 6574 2066 7265 7175  if the set frequ
+00003860: 656e 6379 2069 7320 6e6f 7420 636f 6d6d  ency is not comm
+00003870: 656e 7375 7261 7465 6420 7769 7468 0d0a  ensurated with..
+00003880: 7468 6520 7361 6d70 6c69 6e67 2072 6174  the sampling rat
+00003890: 652e 2054 6f20 6765 6e65 7261 7465 2063  e. To generate c
+000038a0: 6c65 616e 2073 7175 6172 6520 7761 7665  lean square wave
+000038b0: 2c20 7468 6520 7269 7369 6e67 2061 6e64  , the rising and
+000038c0: 2066 616c 6c69 6e67 2065 6467 6573 2073   falling edges s
+000038d0: 686f 756c 640d 0a68 6176 6520 6174 206c  hould..have at l
+000038e0: 6561 7374 2074 776f 2070 6f69 6e74 7320  east two points 
+000038f0: 746f 2072 6570 7265 7365 6e74 2065 7861  to represent exa
+00003900: 6374 2070 6861 7365 2e20 4469 7265 6374  ct phase. Direct
+00003910: 2074 7261 6e73 6974 696f 6e20 6672 6f6d   transition from
+00003920: 206c 6f77 2074 6f20 6869 6768 0d0a 7769   low to high..wi
+00003930: 7468 6f75 7420 616e 7920 696e 7465 726d  thout any interm
+00003940: 6564 6961 7465 2070 6f69 6e74 7320 7375  ediate points su
+00003950: 6666 6572 7320 6672 6f6d 2073 7562 746c  ffers from subtl
+00003960: 6520 6d6f 6475 6c61 7469 6f6e 2069 6e20  e modulation in 
+00003970: 7469 6d65 2064 6f6d 6169 6e2c 0d0a 7768  time domain,..wh
+00003980: 6963 6820 6d61 6e69 6665 7374 7320 6173  ich manifests as
+00003990: 2073 6964 6520 6261 6e64 7320 696e 2046   side bands in F
+000039a0: 4654 2e20 5468 6973 2069 7320 6120 636f  FT. This is a co
+000039b0: 6d6d 6f6e 2070 726f 626c 656d 2069 6e20  mmon problem in 
+000039c0: 6469 6769 7461 6c20 7369 676e 616c 0d0a  digital signal..
+000039d0: 7072 6f63 6573 7369 6e67 2e20 4974 2069  processing. It i
+000039e0: 7320 6e6f 7420 6120 7072 6f62 6c65 6d20  s not a problem 
+000039f0: 696e 2074 6865 2072 6561 6c20 776f 726c  in the real worl
+00003a00: 642c 2062 6563 6175 7365 2074 6865 2073  d, because the s
+00003a10: 6967 6e61 6c20 6973 2061 6e61 6c6f 672c  ignal is analog,
+00003a20: 0d0a 616e 6420 7468 6520 7361 6d70 6c69  ..and the sampli
+00003a30: 6e67 2072 6174 6520 6973 206c 696d 6974  ng rate is limit
+00003a40: 6564 2062 7920 7468 6520 6261 6e64 7769  ed by the bandwi
+00003a50: 6474 6820 6f66 2074 6865 2073 6967 6e61  dth of the signa
+00003a60: 6c2e 0d0a 0d0a 0d0a 2e2e 206c 6974 6572  l......... liter
+00003a70: 616c 696e 636c 7564 653a 3a20 2e2e 2f2e  alinclude:: ../.
+00003a80: 2e2f 7372 7367 7569 2f65 7861 6d70 6c65  ./srsgui/example
+00003a90: 732f 6f73 6369 6c6c 6f73 636f 7065 2065  s/oscilloscope e
+00003aa0: 7861 6d70 6c65 2f74 6173 6b73 2f66 6f75  xample/tasks/fou
+00003ab0: 7274 682e 7079 0d0a 2020 2020 3a6c 616e  rth.py..    :lan
+00003ac0: 6775 6167 653a 2050 7974 686f 6e0d 0a20  guage: Python.. 
+00003ad0: 2020 203a 6c69 6e65 6e6f 733a 0d0a 0d0a     :linenos:....
+00003ae0: 0d0a 0d0a 2e2e 205f 5079 5669 7361 3a20  ...... _PyVisa: 
+00003af0: 6874 7470 733a 2f2f 7079 7669 7361 2e72  https://pyvisa.r
+00003b00: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00003b10: 2f6c 6174 6573 742f 0d0a 2e2e 205f 7372  /latest/.... _sr
+00003b20: 7369 6e73 742e 7372 3836 303a 2068 7474  sinst.sr860: htt
+00003b30: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00003b40: 6f6a 6563 742f 7372 7369 6e73 742e 7372  oject/srsinst.sr
+00003b50: 3836 302f 0d0a 2e2e 205f 5658 4931 313a  860/.... _VXI11:
+00003b60: 2068 7474 7073 3a2f 2f77 7777 2e6c 7869   https://www.lxi
+00003b70: 7374 616e 6461 7264 2e6f 7267 2f41 626f  standard.org/Abo
+00003b80: 7574 2f56 5849 2d31 312d 616e 642d 4c58  ut/VXI-11-and-LX
+00003b90: 492e 6173 7078 0d0a 2e2e 205f 4750 4942  I.aspx.... _GPIB
+00003ba0: 3a20 6874 7470 733a 2f2f 656e 2e77 696b  : https://en.wik
+00003bb0: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00003bc0: 4945 4545 2d34 3838 0d0a 2e2e 205f 5553  IEEE-488.... _US
+00003bd0: 422d 544d 433a 2068 7474 7073 3a2f 2f77  B-TMC: https://w
+00003be0: 7777 2e74 6573 7461 6e64 6d65 6173 7572  ww.testandmeasur
+00003bf0: 656d 656e 7474 6970 732e 636f 6d2f 7265  ementtips.com/re
+00003c00: 6d6f 7465 2d63 6f6d 6d75 6e69 6361 7469  mote-communicati
+00003c10: 6f6e 2d77 6974 682d 7573 6274 6d63 2d66  on-with-usbtmc-f
+00003c20: 6171 2f0d 0a2e 2e20 5f53 4453 3132 3032  aq/.... _SDS1202
+00003c30: 5845 3a20 6874 7470 733a 2f2f 7369 676c  XE: https://sigl
+00003c40: 656e 746e 612e 636f 6d2f 7072 6f64 7563  entna.com/produc
+00003c50: 742f 7364 7331 3230 3278 2d65 2f0d 0a2e  t/sds1202x-e/...
+00003c60: 2e20 5f53 5253 3a20 6874 7470 733a 2f2f  . _SRS: https://
+00003c70: 7468 696e 6b73 7273 2e63 6f6d 2f0d 0a2e  thinksrs.com/...
+00003c80: 2e20 5f43 4736 3335 3a20 6874 7470 733a  . _CG635: https:
+00003c90: 2f2f 7468 696e 6b73 7273 2e63 6f6d 2f70  //thinksrs.com/p
+00003ca0: 726f 6475 6374 732f 6367 3633 352e 6874  roducts/cg635.ht
+00003cb0: 6d6c 0d0a 2e2e 205f 6c6f 6767 696e 673a  ml.... _logging:
+00003cc0: 2068 7474 7073 3a2f 2f64 6f63 732e 7079   https://docs.py
+00003cd0: 7468 6f6e 2e6f 7267 2f33 2f68 6f77 746f  thon.org/3/howto
+00003ce0: 2f6c 6f67 6769 6e67 2e68 746d 6c0d 0a2e  /logging.html...
+00003cf0: 2e20 5f6d 6174 706c 6f74 6c69 623a 2068  . _matplotlib: h
+00003d00: 7474 7073 3a2f 2f6d 6174 706c 6f74 6c69  ttps://matplotli
+00003d10: 622e 6f72 672f 7374 6162 6c65 2f69 6e64  b.org/stable/ind
+00003d20: 6578 2e68 746d 6c                        ex.html
```

### Comparing `srsgui-0.2.17/doc-source/index.rst` & `srsgui-0.2.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/installation.rst` & `srsgui-0.2.9/docs/source/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         python -m pip show pyqt5
 
     will show if pyside2_ or pyqt5_ is installed.
 
 .. note::
     In order to maintain the MIT_ license for your projects or modified ``srsgui``, you have to use
-    pyside6_ or pyside2_. Note that pyqt5_ imposes GPLv3_ license to packages using pyqt5_.
+    pyside6_ or pyside2_. Note that GPLv3_ is the license requirement of pyqt5_.
 
 Running srsgui application
 ----------------------------
 
 After ``srsgui`` is installed, you can start ``srsgui`` application from the command line
 
 .. code-block::
@@ -101,15 +101,15 @@
 
 If you see the application is open and running, the installation is successful!
 
 .. note::
     Instead of seeing the application running, you may get errors, probably ImportError.
     Carefully look through the exception traceback to find out which package causes the error.
     When the latest python is installed, some packages may not install properly. If the problem
-    is not from ``srsgui`` directly, web search of the problem usually leads to a fix.
+    is not from ``srsgui`` directly, web search of the problem usually finds a fix.
 
 
 .. _install-packages: https://packaging.python.org/en/latest/tutorials/installing-packages/
 .. _install-python: https://realpython.com/installing-python/
 .. _virtual-environment: https://realpython.com/python-virtual-environments-a-primer/
 .. _venv: https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/
 .. _pip: https://realpython.com/what-is-pip/
```

### Comparing `srsgui-0.2.17/doc-source/make.bat` & `srsgui-0.2.9/docs/make.bat`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR= .
-set BUILDDIR= ../docs
+set SOURCEDIR=source
+set BUILDDIR=build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `srsgui-0.2.17/doc-source/srsgui.inst.communications.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.inst.rst` & `srsgui-0.2.9/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.task.rst` & `srsgui-0.2.9/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.ui.commandtree.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,85 @@
+srsgui.ui package
+=================
 
-.. automodule:: srsgui.ui.commandtree
+srsgui.ui.taskmain module
+-------------------------
+
+.. automodule:: srsgui.ui.taskmain
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commanditem module
------------------------------------------
+srsgui.ui.connectdlg module
+-------------------------------
 
-.. automodule:: srsgui.ui.commandtree.commanditem
+.. automodule:: srsgui.ui.connectdlg
    :members:
    :undoc-members:
+   :inherited-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandmodel module
-------------------------------------------
+   
+srsgui.ui.commandterminal module
+--------------------------------
+
+.. automodule:: srsgui.ui.commandterminal
+   :members:
+   :undoc-members:
+   :show-inheritance:
+   
+srsgui.ui.deviceinfohandler module
+----------------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandmodel
+.. automodule:: srsgui.ui.deviceinfohandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandhandler module
---------------------------------------------
+srsgui.ui.dockhandler module
+----------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandhandler
+.. automodule:: srsgui.ui.dockhandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commanddelegate module
----------------------------------------------
+srsgui.ui.inputpanel module
+---------------------------
 
-.. automodule:: srsgui.ui.commandtree.commanddelegate
+.. automodule:: srsgui.ui.inputpanel
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandspinbox module
---------------------------------------------
+srsgui.ui.qtloghandler module
+-----------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandspinbox
+.. automodule:: srsgui.ui.qtloghandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandtreeview module
----------------------------------------------
+srsgui.ui.signalhandler module
+------------------------------
 
-.. automodule:: srsgui.ui.commandtree.commandtreeview
+.. automodule:: srsgui.ui.signalhandler
    :members:
    :undoc-members:
    :show-inheritance:
 
-srsgui.ui.commandtree.commandtreewidget module
------------------------------------------------
+srsgui.ui.stdout module
+-----------------------
 
-.. automodule:: srsgui.ui.commandtree.commandtreewidget
+.. automodule:: srsgui.ui.stdout
    :members:
    :undoc-members:
    :show-inheritance:
 
+srsgui.ui.qt package
+----------------------
+
+.. toctree::
+   :maxdepth: 4
+
+   srsgui.ui.qt.rst
+
```

### Comparing `srsgui-0.2.17/doc-source/srsgui.ui.qt.rst` & `srsgui-0.2.9/docs/source/srsgui.ui.qt.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+srsgui.ui.qt package~
+======================
 
 .. automodule:: srsgui.ui.qt
    :members:
    :undoc-members:
    :show-inheritance:
 
 srsgui.ui.qt.QtCore module
```

### Comparing `srsgui-0.2.17/srsgui/__init__.py` & `srsgui-0.2.9/srsgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.17"  # Global version number
+__version__ = "0.2.9"  # Global version number
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,107 @@
-00000000: 2323 2120 0d0a 2323 2120 436f 7074 7269  ##! ..##! Coptri
-00000010: 6768 7428 6329 2032 3032 322c 2032 3032  ght(c) 2022, 202
-00000020: 3320 5374 616e 666f 7264 2052 6573 6561  3 Stanford Resea
-00000030: 7263 6820 5379 7374 656d 732c 2041 6c6c  rch Systems, All
-00000040: 2072 6967 6874 2072 6573 6572 7665 640d   right reserved.
-00000050: 0a23 2321 2053 7562 6a65 6374 2074 6f20  .##! Subject to 
-00000060: 7468 6520 4d49 5420 4c69 6365 6e73 650d  the MIT License.
-00000070: 0a23 2321 200d 0a0d 0a66 726f 6d20 7372  .##! ....from sr
-00000080: 7367 7569 2069 6d70 6f72 7420 496e 7374  sgui import Inst
-00000090: 7275 6d65 6e74 0d0a 6672 6f6d 2073 7273  rument..from srs
-000000a0: 6775 692e 696e 7374 2069 6d70 6f72 7420  gui.inst import 
-000000b0: 466c 6f61 7443 6f6d 6d61 6e64 0d0a 0d0a  FloatCommand....
-000000c0: 2320 556e 636f 6d6d 656e 7420 7468 6520  # Uncomment the 
-000000d0: 666f 6c6c 6f77 696e 6720 696d 706f 7274  following import
-000000e0: 2074 6f20 7573 6520 5669 7361 496e 7465   to use VisaInte
-000000f0: 7266 6163 650d 0a23 2066 726f 6d20 7372  rface..# from sr
-00000100: 7367 7569 2069 6d70 6f72 7420 5365 7269  sgui import Seri
-00000110: 616c 496e 7465 7266 6163 652c 2046 696e  alInterface, Fin
-00000120: 644c 6973 7449 6e70 7574 0d0a 2320 6672  dListInput..# fr
-00000130: 6f6d 2073 7273 696e 7374 2e73 7238 3630  om srsinst.sr860
-00000140: 2069 6d70 6f72 7420 5669 7361 496e 7465   import VisaInte
-00000150: 7266 6163 650d 0a0d 0a0d 0a63 6c61 7373  rface......class
-00000160: 2043 4736 3335 2849 6e73 7472 756d 656e   CG635(Instrumen
-00000170: 7429 3a0d 0a20 2020 205f 4964 5374 7269  t):..    _IdStri
-00000180: 6e67 203d 2027 4347 3633 3527 0d0a 2020  ng = 'CG635'..  
-00000190: 2020 2320 5f74 6572 6d5f 6368 6172 203d    # _term_char =
-000001a0: 2062 275c 7227 2020 2320 6966 2079 6f75   b'\r'  # if you
-000001b0: 7220 696e 7374 7275 6d65 6e74 2075 7365  r instrument use
-000001c0: 7320 6361 7272 6961 6765 2072 6574 7572  s carriage retur
-000001d0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-000001e0: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-000001f0: 6e73 7465 6164 206f 6620 6c69 656e 6665  nstead of lienfe
-00000200: 6564 2028 2062 275c 6e27 2029 2c0d 0a20  ed ( b'\n' ),.. 
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 2020 2020 2020 2023 2061 7320 7468           # as th
-00000230: 6520 7465 726d 696e 6174 696f 6e20 6368  e termination ch
-00000240: 6172 6163 7465 722c 2075 6e63 6f6d 6d65  aracter, uncomme
-00000250: 6e74 2074 6869 7320 6c69 6e65 2e0d 0a0d  nt this line....
-00000260: 0a20 2020 2023 2055 6e63 6f6d 6d65 6e74  .    # Uncomment
-00000270: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00000280: 6963 7469 6f6e 6172 7920 746f 2075 7365  ictionary to use
-00000290: 2061 2063 7573 6f6d 697a 6564 200d 0a20   a cusomized .. 
-000002a0: 2020 2023 2043 6f6d 6d75 6e69 6361 7469     # Communicati
-000002b0: 6f6e 2069 6e74 6572 6661 6365 2064 6566  on interface def
-000002c0: 696e 6974 696f 6e2e 0d0a 2020 2020 2320  inition...    # 
-000002d0: 5669 6149 6e74 6572 6661 6365 2069 7320  ViaInterface is 
-000002e0: 6176 6169 6c61 6265 2066 726f 6d20 7372  availabe from sr
-000002f0: 7369 6e73 742e 7372 3836 3020 7061 636b  sinst.sr860 pack
-00000300: 6167 652e 0d0a 2020 2020 2320 5669 7361  age...    # Visa
-00000310: 496e 7465 7266 6163 6520 7265 7175 6972  Interface requir
-00000320: 6573 2050 7956 6973 6120 7061 636b 6167  es PyVisa packag
-00000330: 6520 746f 2062 6520 696e 7374 616c 6c65  e to be installe
-00000340: 6420 6d61 6e75 616c 6c79 2e0d 0a20 2020  d manually...   
-00000350: 2023 204e 6f74 6520 7468 6174 2050 7956   # Note that PyV
-00000360: 6973 6120 7265 7175 6972 6573 2061 2073  isa requires a s
-00000370: 6570 6172 6174 6520 6261 636b 656e 6420  eparate backend 
-00000380: 6472 6976 6572 2069 6e73 7461 6c6c 6174  driver installat
-00000390: 696f 6e2c 2074 6f6f 2e0d 0a20 2020 2022  ion, too...    "
-000003a0: 2222 0d0a 2020 2020 6176 6169 6c61 626c  ""..    availabl
-000003b0: 655f 696e 7465 7266 6163 6573 203d 205b  e_interfaces = [
-000003c0: 0d0a 2020 2020 2020 2020 5b20 2020 5365  ..        [   Se
-000003d0: 7269 616c 496e 7465 7266 6163 652c 0d0a  rialInterface,..
-000003e0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-000003f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000400: 434f 4d20 706f 7274 273a 2046 696e 644c  COM port': FindL
-00000410: 6973 7449 6e70 7574 2829 2c0d 0a20 2020  istInput(),..   
-00000420: 2020 2020 2020 2020 2020 2020 2027 6261               'ba
-00000430: 7564 2072 6174 6527 3a20 3936 3030 0d0a  ud rate': 9600..
-00000440: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00000450: 2020 2020 2020 205d 2c20 2020 200d 0a20         ],    .. 
-00000460: 2020 2020 2020 205b 2020 2056 6973 6149         [   VisaI
-00000470: 6e74 6572 6661 6365 2c0d 0a20 2020 2020  nterface,..     
-00000480: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00000490: 2020 2020 2020 2020 2020 2772 6573 6f75            'resou
-000004a0: 7263 6527 3a20 4669 6e64 4c69 7374 496e  rce': FindListIn
-000004b0: 7075 7428 292c 0d0a 2020 2020 2020 2020  put(),..        
-000004c0: 2020 2020 7d0d 0a20 2020 2020 2020 205d      }..        ]
-000004d0: 2c20 2020 2020 2020 200d 0a20 2020 205d  ,        ..    ]
-000004e0: 0d0a 2020 2020 2222 220d 0a0d 0a20 2020  ..    """....   
-000004f0: 2066 7265 7175 656e 6379 203d 2046 6c6f   frequency = Flo
-00000500: 6174 436f 6d6d 616e 6428 2746 5245 5127  atCommand('FREQ'
-00000510: 290d 0a20 2020 2022 2222 0d0a 2020 2020  )..    """..    
-00000520: 466c 6f61 7443 6f6d 6d61 6e64 2069 7320  FloatCommand is 
-00000530: 7573 6564 2074 6f20 656e 6361 7073 756c  used to encapsul
-00000540: 6174 6520 6120 7265 6d6f 7465 2063 6f6d  ate a remote com
-00000550: 6d61 6e64 2074 6f20 7365 7420 616e 6420  mand to set and 
-00000560: 7175 7274 7920 6120 666c 6f61 7420 7661  qurty a float va
-00000570: 6c75 650d 0a20 2020 2054 6f20 7365 7420  lue..    To set 
-00000580: 6120 7661 6c75 652c 0d0a 2020 2020 2020  a value,..      
-00000590: 2020 6367 2e66 7265 7165 756e 6379 203d    cg.freqeuncy =
-000005a0: 2031 6537 0d0a 2020 2020 2020 2020 0d0a   1e7..        ..
-000005b0: 2020 2020 746f 2071 7565 7279 2061 2076      to query a v
-000005c0: 616c 7565 0d0a 2020 2020 2020 2020 6620  alue..        f 
-000005d0: 3d20 6367 2e66 7265 7175 656d 6379 0d0a  = cg.frequemcy..
-000005e0: 2020 2020 2222 220d 0a0d 0a20 2020 2023      """....    #
-000005f0: 2054 6f20 7573 6520 7072 6f6d 6f74 6564   To use promoted
-00000600: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2063   communication c
-00000610: 6c61 7373 206d 6574 686f 6473 2074 6f20  lass methods to 
-00000620: 7365 7420 616e 6420 7175 6572 7920 6120  set and query a 
-00000630: 7265 6d6f 7465 2063 6f6d 6d61 6e64 2066  remote command f
-00000640: 6f72 2061 2066 6c6f 6174 2076 616c 7565  or a float value
-00000650: 2c0d 0a20 2020 2023 2075 6e63 6f6d 6d65  ,..    # uncomme
-00000660: 6e74 2074 6865 2066 6f6c 6c6f 7769 6e67  nt the following
-00000670: 206d 6574 686f 6473 2e20 2020 200d 0a20   methods.    .. 
-00000680: 2020 2022 2222 0d0a 2020 2020 6465 6620     """..    def 
-00000690: 7365 745f 6672 6571 7565 6e63 7928 7365  set_frequency(se
-000006a0: 6c66 2c20 6629 3a0d 0a20 2020 2020 2020  lf, f):..       
-000006b0: 2073 656c 662e 7365 6e64 2866 2746 5245   self.send(f'FRE
-000006c0: 5120 7b66 7d27 290d 0a20 2020 2020 2020  Q {f}')..       
-000006d0: 200d 0a20 2020 2064 6566 2067 6574 5f66   ..    def get_f
-000006e0: 7265 7175 656e 6379 2873 656c 6629 3a0d  requency(self):.
-000006f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000700: 7365 6c66 2e71 7565 7279 5f66 6c6f 6174  self.query_float
-00000710: 2827 4652 4551 3f27 290d 0a20 2020 2022  ('FREQ?')..    "
-00000720: 2222 0d0a                                ""..
+00000000: 0d0a 6672 6f6d 2073 7273 6775 6920 696d  ..from srsgui im
+00000010: 706f 7274 2049 6e73 7472 756d 656e 740d  port Instrument.
+00000020: 0a66 726f 6d20 7372 7367 7569 2e69 6e73  .from srsgui.ins
+00000030: 7420 696d 706f 7274 2046 6c6f 6174 436f  t import FloatCo
+00000040: 6d6d 616e 640d 0a0d 0a23 2055 6e63 6f6d  mmand....# Uncom
+00000050: 6d65 6e74 2074 6865 2066 6f6c 6c6f 7769  ment the followi
+00000060: 6e67 2069 6d70 6f72 7420 746f 2075 7365  ng import to use
+00000070: 2056 6973 6149 6e74 6572 6661 6365 0d0a   VisaInterface..
+00000080: 2320 6672 6f6d 2073 7273 6775 6920 696d  # from srsgui im
+00000090: 706f 7274 2053 6572 6961 6c49 6e74 6572  port SerialInter
+000000a0: 6661 6365 2c20 4669 6e64 4c69 7374 496e  face, FindListIn
+000000b0: 7075 740d 0a23 2066 726f 6d20 7372 7369  put..# from srsi
+000000c0: 6e73 742e 7372 3836 3020 696d 706f 7274  nst.sr860 import
+000000d0: 2056 6973 6149 6e74 6572 6661 6365 0d0a   VisaInterface..
+000000e0: 0d0a 0d0a 636c 6173 7320 4347 3633 3528  ....class CG635(
+000000f0: 496e 7374 7275 6d65 6e74 293a 0d0a 2020  Instrument):..  
+00000100: 2020 5f49 6453 7472 696e 6720 3d20 2743    _IdString = 'C
+00000110: 4736 3335 270d 0a20 2020 2023 205f 7465  G635'..    # _te
+00000120: 726d 5f63 6861 7220 3d20 6227 5c72 2720  rm_char = b'\r' 
+00000130: 2023 2069 6620 796f 7572 2069 6e73 7472   # if your instr
+00000140: 756d 656e 7420 7573 6573 2063 6172 7269  ument uses carri
+00000150: 6167 6520 7265 7475 726e 0d0a 2020 2020  age return..    
+00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000170: 2020 2020 2020 2320 696e 7374 6561 6420        # instead 
+00000180: 6f66 206c 6965 6e66 6565 6420 2820 6227  of lienfeed ( b'
+00000190: 5c6e 2720 292c 0d0a 2020 2020 2020 2020  \n' ),..        
+000001a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001b0: 2020 2320 6173 2074 6865 2074 6572 6d69    # as the termi
+000001c0: 6e61 7469 6f6e 2063 6861 7261 6374 6572  nation character
+000001d0: 2c20 756e 636f 6d6d 656e 7420 7468 6973  , uncomment this
+000001e0: 206c 696e 652e 0d0a 0d0a 2020 2020 2320   line.....    # 
+000001f0: 556e 636f 6d6d 656e 7420 7468 6520 666f  Uncomment the fo
+00000200: 6c6c 6f77 696e 6720 6469 6374 696f 6e61  llowing dictiona
+00000210: 7279 2074 6f20 7573 6520 6120 6375 736f  ry to use a cuso
+00000220: 6d69 7a65 6420 0d0a 2020 2020 2320 436f  mized ..    # Co
+00000230: 6d6d 756e 6963 6174 696f 6e20 696e 7465  mmunication inte
+00000240: 7266 6163 6520 6465 6669 6e69 7469 6f6e  rface definition
+00000250: 2e0d 0a20 2020 2023 2056 6961 496e 7465  ...    # ViaInte
+00000260: 7266 6163 6520 6973 2061 7661 696c 6162  rface is availab
+00000270: 6520 6672 6f6d 2073 7273 696e 7374 2e73  e from srsinst.s
+00000280: 7238 3630 2070 6163 6b61 6765 2e0d 0a20  r860 package... 
+00000290: 2020 2023 2056 6973 6149 6e74 6572 6661     # VisaInterfa
+000002a0: 6365 2072 6571 7569 7265 7320 5079 5669  ce requires PyVi
+000002b0: 7361 2070 6163 6b61 6765 2074 6f20 6265  sa package to be
+000002c0: 2069 6e73 7461 6c6c 6564 206d 616e 7561   installed manua
+000002d0: 6c6c 792e 0d0a 2020 2020 2320 4e6f 7465  lly...    # Note
+000002e0: 2074 6861 7420 5079 5669 7361 2072 6571   that PyVisa req
+000002f0: 7569 7265 7320 6120 7365 7061 7261 7465  uires a separate
+00000300: 2062 6163 6b65 6e64 2064 7269 7665 7220   backend driver 
+00000310: 696e 7374 616c 6c61 7469 6f6e 2c20 746f  installation, to
+00000320: 6f2e 0d0a 2020 2020 2222 220d 0a20 2020  o...    """..   
+00000330: 2061 7661 696c 6162 6c65 5f69 6e74 6572   available_inter
+00000340: 6661 6365 7320 3d20 5b0d 0a20 2020 2020  faces = [..     
+00000350: 2020 205b 2020 2053 6572 6961 6c49 6e74     [   SerialInt
+00000360: 6572 6661 6365 2c0d 0a20 2020 2020 2020  erface,..       
+00000370: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00000380: 2020 2020 2020 2020 2743 4f4d 2070 6f72          'COM por
+00000390: 7427 3a20 4669 6e64 4c69 7374 496e 7075  t': FindListInpu
+000003a0: 7428 292c 0d0a 2020 2020 2020 2020 2020  t(),..          
+000003b0: 2020 2020 2020 2762 6175 6420 7261 7465        'baud rate
+000003c0: 273a 2039 3630 300d 0a20 2020 2020 2020  ': 9600..       
+000003d0: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+000003e0: 5d2c 2020 2020 0d0a 2020 2020 2020 2020  ],    ..        
+000003f0: 5b20 2020 5669 7361 496e 7465 7266 6163  [   VisaInterfac
+00000400: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000410: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00000420: 2020 2027 7265 736f 7572 6365 273a 2046     'resource': F
+00000430: 696e 644c 6973 7449 6e70 7574 2829 2c0d  indListInput(),.
+00000440: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
+00000450: 2020 2020 2020 2020 5d2c 2020 2020 2020          ],      
+00000460: 2020 0d0a 2020 2020 5d0d 0a20 2020 2022    ..    ]..    "
+00000470: 2222 0d0a 0d0a 2020 2020 6672 6571 7565  ""....    freque
+00000480: 6e63 7920 3d20 466c 6f61 7443 6f6d 6d61  ncy = FloatComma
+00000490: 6e64 2827 4652 4551 2729 0d0a 2020 2020  nd('FREQ')..    
+000004a0: 2222 220d 0a20 2020 2046 6c6f 6174 436f  """..    FloatCo
+000004b0: 6d6d 616e 6420 6973 2075 7365 6420 746f  mmand is used to
+000004c0: 2065 6e63 6170 7375 6c61 7465 2061 2072   encapsulate a r
+000004d0: 656d 6f74 6520 636f 6d6d 616e 6420 746f  emote command to
+000004e0: 2073 6574 2061 6e64 2071 7572 7479 2061   set and qurty a
+000004f0: 2066 6c6f 6174 2076 616c 7565 0d0a 2020   float value..  
+00000500: 2020 546f 2073 6574 2061 2076 616c 7565    To set a value
+00000510: 2c0d 0a20 2020 2020 2020 2063 672e 6672  ,..        cg.fr
+00000520: 6571 6575 6e63 7920 3d20 3165 370d 0a20  eqeuncy = 1e7.. 
+00000530: 2020 2020 2020 200d 0a20 2020 2074 6f20         ..    to 
+00000540: 7175 6572 7920 6120 7661 6c75 650d 0a20  query a value.. 
+00000550: 2020 2020 2020 2066 203d 2063 672e 6672         f = cg.fr
+00000560: 6571 7565 6d63 790d 0a20 2020 2022 2222  equemcy..    """
+00000570: 0d0a 0d0a 2020 2020 2320 546f 2075 7365  ....    # To use
+00000580: 2070 726f 6d6f 7465 6420 636f 6d6d 756e   promoted commun
+00000590: 6963 6174 696f 6e20 636c 6173 7320 6d65  ication class me
+000005a0: 7468 6f64 7320 746f 2073 6574 2061 6e64  thods to set and
+000005b0: 2071 7565 7279 2061 2072 656d 6f74 6520   query a remote 
+000005c0: 636f 6d6d 616e 6420 666f 7220 6120 666c  command for a fl
+000005d0: 6f61 7420 7661 6c75 652c 0d0a 2020 2020  oat value,..    
+000005e0: 2320 756e 636f 6d6d 656e 7420 7468 6520  # uncomment the 
+000005f0: 666f 6c6c 6f77 696e 6720 6d65 7468 6f64  following method
+00000600: 732e 2020 2020 0d0a 2020 2020 2222 220d  s.    ..    """.
+00000610: 0a20 2020 2064 6566 2073 6574 5f66 7265  .    def set_fre
+00000620: 7175 656e 6379 2873 656c 662c 2066 293a  quency(self, f):
+00000630: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00000640: 656e 6428 6627 4652 4551 207b 667d 2729  end(f'FREQ {f}')
+00000650: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00000660: 6465 6620 6765 745f 6672 6571 7565 6e63  def get_frequenc
+00000670: 7928 7365 6c66 293a 0d0a 2020 2020 2020  y(self):..      
+00000680: 2020 7265 7475 726e 2073 656c 662e 7175    return self.qu
+00000690: 6572 795f 666c 6f61 7428 2746 5245 513f  ery_float('FREQ?
+000006a0: 2729 0d0a 2020 2020 2222 220d 0a         ')..    """..
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import numpy as np
 from srsgui import Instrument
 
 # Uncomment the following import to use the customized interface definition
 # from srsgui import TcpipInterface, Ip4Input, FindListInput, StringInput
 # from srsinst.sr860 import VisaInterface, Vxi11Interface
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import time
 import math
 import logging
 import numpy as np
 
 from srsgui import Task
 from srsgui import IntegerInput
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 from srsgui import Task
 
 
 class FirstTask(Task):
     """
 Query *IDN? to instruments, 'cg' and 'osc' \
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import time
 import numpy as np
 from srsgui import Task
 from srsgui import IntegerInput
 
 
 class FourthTask(Task):
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import time
 import math
 
 from srsgui import Task
 from srsgui import IntegerInput
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.9/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import time
 from srsgui import Task
 from srsgui import IntegerInput
 
 
 class ThirdTask(Task):
     """
```

### Comparing `srsgui-0.2.17/srsgui/inst/__init__.py` & `srsgui-0.2.9/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/commands.py` & `srsgui-0.2.9/srsgui/inst/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 """
 Module to wrap remote commands used in communication with an instrument
 in `Python descriptors <https://docs.python.org/3/howto/descriptor.html>`_.
 
 If an instrument has a remote command 'FREQ' for  setting and querying a value,
 you will use the command from a terminal,
@@ -77,28 +73,25 @@
 
     def __get__(self, instance, instance_type):
         if instance is None:
             return self
         query_string = self._get_command_format.format(self.remote_command)
         reply = None
         try:
-            reply = instance.comm.query_text(query_string).strip()
+            reply = instance.comm.query_text(query_string)
             if callable(self._get_convert_function):
                 self._value = self._get_convert_function(reply)
 
             else:
                 self._value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
         except ValueError:
-            if reply:
-                raise InstQueryError('Error during conversion CMD: {} Reply: {}, Hex:{}'
-                                     .format(query_string, reply, (*map(hex, reply.encode('ascii')),)))
-            else:
-                raise InstQueryError('CMD: {} returned "{}"'.format(query_string, reply))
+            raise InstQueryError('Error during conversion CMD: {} Reply: {}'
+                                 .format(query_string, reply))
         return self._value
 
     def __set__(self, instance, value):
         if instance is None:
             return
 
         try:
@@ -219,15 +212,15 @@
 
 class FloatCommand(Command):
     """
     Descriptor for a remote command to
     **set** and **query** a **float** value
     """
 
-    def __init__(self, remote_command_name, unit='', min=-1e6, max=1e6, step=1e-9,
+    def __init__(self, remote_command_name, unit='', min=-1000.0, max=1000.0, step=0.1,
                  significant_figures=4, default_value=None):
         super().__init__(remote_command_name, default_value)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = max
         self.minimum = min
```

### Comparing `srsgui-0.2.17/srsgui/inst/communications/interface.py` & `srsgui-0.2.9/srsgui/inst/communications/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import threading
 
 TERM_CHAR = b'\n'   # Termination character for communication
 
 
 class Interface(object):
@@ -129,23 +125,14 @@
         Use send instead.
 
         :param cmd: a string of command that will be internally converted to bytes
         :return: None
         """
         raise NotImplementedError
 
-    def _write_binary(self, binary_array: bytes):
-        """
-        Send an array of bytes over an interface without the lock.
-        It does not append the termination character at the end of the array.
-
-        :return: None
-        """
-        raise NotImplementedError
-
     def _recv(self):
         """
         Receive a reply up to the termination character over an interface without the lock.
         It should be implemented in subclasses.
         This is a protected method that a user should not call directly,
         because it is not thread-safe.  Use recv instead.
```

### Comparing `srsgui-0.2.17/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.9/srsgui/inst/communications/serial_ports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 """
 Get all available serial ports.
 
 Snippet from http://stackoverflow.com/questions/12090503/listing-available-com-ports-with-python
 """
```

### Comparing `srsgui-0.2.17/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/serialinterface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import time
 
 from srsgui.inst.exceptions import InstCommunicationError
 from .interface import Interface
 from .serial_ports import serial_ports
 
@@ -140,25 +136,14 @@
         try:
             self._serial.write(bytecmd)
         except (self.port_not_open_error, AttributeError):
             raise InstCommunicationError('Port not open to write')
         except serial.SerialException:
             raise InstCommunicationError("Sending cmd '{}' to port '{}' failed".format(cmd, self._port))
 
-    def _write_bibary(self, binary_array):
-        if type(binary_array) not in (bytes, bytearray):
-            raise TypeError('_write_binary requires bytes or bytearray')
-        try:
-            self._serial.write(binary_array)
-        except (self.port_not_open_error, AttributeError):
-            raise InstCommunicationError('Port not open to write')
-        except serial.SerialException:
-            raise InstCommunicationError("writing binary '{}' to port '{}' failed".format(
-                (*map(hex, binary_array),), self._port))
-
     def _recv(self):
         """
         Receive a reply over serial interface without the lock.
         This is a protected method that a user should not call directly,
         because it is not thread-safe. Use recv instead.
 
         :return: bytes. It should be converted to string explicitly
```

### Comparing `srsgui-0.2.17/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.9/srsgui/inst/communications/tcpipinterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import time
 
 import socket
 import select
 
 from srsgui.inst.exceptions import InstCommunicationError, InstLoginFailureError
@@ -54,23 +50,14 @@
 
         try:
             self.socket.sendall(byte_cmd)
         except OSError:
             raise InstCommunicationError("Sending cmd '{}' to IP address: '{}' failed"
                                          .format(cmd, self._ip_address))
 
-    def _write_binary(self, binary_array):
-        if type(binary_array) not in (bytes, bytearray):
-            raise TypeError('_write_binary requires bytes or bytearray')
-        try:
-            self.socket.sendall(binary_array)
-        except OSError:
-            raise InstCommunicationError("Writing binary '{}' to IP address: '{}' failed"
-                                         .format((*map(hex, binary_array),), self._ip_address))
-
     def _recv(self):
         """
         Receive a reply over TCP/IP without the lock.
         This is a protected method that a user should not call directly,
         because it is not thread-safe.  Use recv instead.
 
         :return: bytes. It should be converted to string explicitly
```

### Comparing `srsgui-0.2.17/srsgui/inst/component.py` & `srsgui-0.2.9/srsgui/inst/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 from .communications import Interface
 from .commands import Command, GetCommand, BoolCommand, IntCommand, \
                       FloatCommand, DictCommand
 from .indexcommands import IndexCommand, BoolIndexCommand, IntIndexCommand, \
                            FloatIndexCommand, DictIndexCommand
 
 
@@ -86,17 +81,14 @@
 
     def is_connected(self):
         """
         check if the current communication interface is open
         """
         return self.comm.is_connected()
 
-    def parent(self):
-        return self._parent
-
     def set_name(self, name):
         """
         Set the name of the component
         """
         self._name = name
 
     def get_name(self):
```

### Comparing `srsgui-0.2.17/srsgui/inst/indexcommands.py` & `srsgui-0.2.9/srsgui/inst/indexcommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 """
 Module to wrap remote commands with an index argument in dunder methods, __setitem__ and __get_item__.
 
 If an instrument has a remote command using an index, 'PARAM', for  setting and querying a value,
 you will use the command from a terminal,
 
 .. code-block::
@@ -91,31 +86,27 @@
     def __set__(self, instance, value):
         raise InstSetError('No set for IndexCommand for {}'
                            .format(self.remote_command))
 
     def __getitem__(self, index):
         converted_index = self._convert_index(index)
         query_string = '{}? {}'.format(self.remote_command, converted_index)
-        reply = None
         value = None
         try:
             reply = self._parent.comm.query_text(query_string)
             if callable(self._get_convert_function):
                 value = self._get_convert_function(reply)
 
             else:
                 value = reply
         except InstCommunicationError:
             raise InstQueryError('Error during querying: CMD: {}'.format(query_string))
         except ValueError:
-            if reply:
-                raise InstQueryError('Error during conversion CMD: {} Reply: {}, Hex:{}'
-                                     .format(query_string, reply, (*map(hex, reply.encode('ascii')),)))
-            else:
-                raise InstQueryError('CMD: {} returned "{}"'.format(query_string, reply))
+            raise InstQueryError('Error during conversion CMD: {} Reply: {}'
+                                 .format(query_string, reply))
         return value
 
     def __setitem__(self, index, value):
         converted_index = self._convert_index(index)
         set_string = '{} {}, '.format(self.remote_command, converted_index)
         try:
             if callable(self._set_convert_function):
@@ -208,28 +199,27 @@
 
 class IntIndexGetCommand(IntIndexCommand):
     """
     Command class for a remote command with index
     using only **query** returning an **integer**, without **set**.
     """
     _set_enable = False
-
     def __setitem__(self, instance, value):
         raise InstIndexError('No set allowed for index command {}'
                              .format(self.remote_command))
 
 
 class FloatIndexCommand(IndexCommand):
     """
     Command class for a remote command with index
     using **set** and **query** returning an **float**
     """
 
     def __init__(self, remote_command_name, index_max, index_min=0, index_dict=None,
-                 unit='', value_min=-1e6, value_max=1e6, step=1e-9, significant_figures=4, default_valaue=0.0 ):
+                 unit='', value_min=-1e6, value_max=1e6, step=0.1, significant_figures=4, default_valaue=0.0 ):
         super().__init__(remote_command_name, index_max, index_min, index_dict)
         self._get_convert_function = float
 
         self.unit = unit
         self.maximum = value_max
         self.minimum = value_min
         self.step = step
```

### Comparing `srsgui-0.2.17/srsgui/inst/instrument.py` & `srsgui-0.2.9/srsgui/inst/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import re
 import time
 from .communications import Interface, SerialInterface, TcpipInterface
 from .component import Component
 from .exceptions import InstIdError
 
 from srsgui.task.inputs import FindListInput, IntegerListInput, BoolInput, \
```

### Comparing `srsgui-0.2.17/srsgui/task/config.py` & `srsgui-0.2.9/srsgui/task/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import sys
 import os
 import logging
 from pathlib import Path
 from importlib import import_module, reload, invalidate_caches
 
 from srsgui.task.task import Task, GreenNormal, RedNormal
```

### Comparing `srsgui-0.2.17/srsgui/task/inputs.py` & `srsgui-0.2.9/srsgui/task/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 """
 Interface for input variables between Task and InputPanel in GUI
 
 """
```

### Comparing `srsgui-0.2.17/srsgui/task/sessionhandler.py` & `srsgui-0.2.9/srsgui/task/sessionhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import json
 import logging
 from pathlib import Path
 from datetime import datetime
 
+# from wip.local_results import LocalClient
+# from wip.wip_api import DutNotRegisteredError
+
 from srsgui.task.taskresult import TaskResult
 
 RedBold = '<font color="red"><b>{}</b></font>'
 logger = logging.getLogger(__name__)
 
+logging.getLogger('urllib3').setLevel(logging.WARNING)
+
 
 class SessionHandler(object):
     def __init__(self, use_file=False, use_db=False, use_api=False):
         self.use_file = False
         self.use_db = False
         self.use_api = False
         self._is_session_open = False
```

### Comparing `srsgui-0.2.17/srsgui/task/task.py` & `srsgui-0.2.9/srsgui/task/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import sys
 import traceback
 import logging
 import time
 
 try:
@@ -280,15 +276,15 @@
             self._keep_running = False
 
     def delay(self, seconds):
         """
         Check if the task is stopped and wait for the given seconds.
         """
         if not self._keep_running:
-            raise Task.TaskException('Task is requested to stop')
+            raise KeyboardInterrupt('Task is stopped')
         else:
             time.sleep(seconds)
 
     def set_session_handler(self, session_handler):
         """
         Parent should set a session handler for Task to use file output.
         """
@@ -354,15 +350,15 @@
     def clear_figures(self):
         """
         Clear all the figures in figure_dict
         """
         for fig in self.figure_dict.values():
             if hasattr(fig, 'canvas'):
                 fig.clear()
-                self.request_figure_update(fig)
+                self.request_figure_update()
 
     def is_running(self):
         """
         Task should check is_running() is True.
         If it returns False, Task should stop ASAP.
         """
         return self._keep_running
@@ -516,18 +512,24 @@
             raise TypeError('{} is not  a Figure'.format(type(figure)))
         self.callbacks.figure_update_requested(figure)
 
     # It needs a matching update() as a slot to run from UI
     def notify_data_available(self, data={}):
         self.callbacks.data_available(data)
 
+    # These callbacks are used to update display for streaming data from another class or thread
+    # Signals are wrapped as a callback functions 
+
+    def data_available_callback(self, data={}, *args):
+        self.callbacks.data_available(data)
+
     def update(self, data: dict):
         """
-        when notify_data_available is called, this method handles data processing
-        and display update. By default, it does no data handling, but figure update request.
+        when data_available signal emits, this method handles display update.
+        By default, it does no data handling, but figure update request.
         GUI related data processing needs to be done here to be handled
         in proper order by the GUI event loop handler.
         """
         self.request_figure_update()
 
     def get_instrument(self, name):
         """Get an instrument from parent's inst_dict and check its validity"""
```

### Comparing `srsgui-0.2.17/srsgui/task/taskresult.py` & `srsgui-0.2.9/srsgui/task/taskresult.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
+
 
 from datetime import datetime
 
 import logging
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandhandler.py` & `srsgui-0.2.9/srsgui/ui/commandhandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,244 +1,236 @@
-00000000: 2323 2120 0d0a 2323 2120 436f 7074 7269  ##! ..##! Coptri
-00000010: 6768 7428 6329 2032 3032 322c 2032 3032  ght(c) 2022, 202
-00000020: 3320 5374 616e 666f 7264 2052 6573 6561  3 Stanford Resea
-00000030: 7263 6820 5379 7374 656d 732c 2041 6c6c  rch Systems, All
-00000040: 2072 6967 6874 2072 6573 6572 7665 640d   right reserved.
-00000050: 0a23 2321 2053 7562 6a65 6374 2074 6f20  .##! Subject to 
-00000060: 7468 6520 4d49 5420 4c69 6365 6e73 650d  the MIT License.
-00000070: 0a23 2321 200d 0a0d 0a69 6d70 6f72 7420  .##! ....import 
-00000080: 7469 6d65 0d0a 696d 706f 7274 206c 6f67  time..import log
-00000090: 6769 6e67 0d0a 6672 6f6d 202e 7174 2e51  ging..from .qt.Q
-000000a0: 7443 6f72 6520 696d 706f 7274 2051 4f62  tCore import QOb
-000000b0: 6a65 6374 2c20 5154 6872 6561 642c 2053  ject, QThread, S
-000000c0: 6967 6e61 6c2c 2053 6c6f 740d 0a66 726f  ignal, Slot..fro
-000000d0: 6d20 2e71 742e 5174 5769 6467 6574 7320  m .qt.QtWidgets 
-000000e0: 696d 706f 7274 2051 4d65 7373 6167 6542  import QMessageB
-000000f0: 6f78 0d0a 0d0a 6672 6f6d 2073 7273 6775  ox....from srsgu
-00000100: 692e 696e 7374 2e69 6e73 7472 756d 656e  i.inst.instrumen
-00000110: 7420 696d 706f 7274 2049 6e73 7472 756d  t import Instrum
-00000120: 656e 740d 0a0d 0a6c 6f67 6765 7220 3d20  ent....logger = 
-00000130: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
-00000140: 7228 5f5f 6e61 6d65 5f5f 290d 0a0d 0a0d  r(__name__).....
-00000150: 0a63 6c61 7373 2043 6f6d 6d61 6e64 576f  .class CommandWo
-00000160: 726b 6572 2851 4f62 6a65 6374 293a 0d0a  rker(QObject):..
-00000170: 2020 2020 636f 6d6d 616e 645f 7072 6f63      command_proc
-00000180: 6573 7365 6420 3d20 5369 676e 616c 2873  essed = Signal(s
-00000190: 7472 2c20 7374 7229 0d0a 2020 2020 696e  tr, str)..    in
-000001a0: 7374 5f64 6963 7420 3d20 7b7d 0d0a 2020  st_dict = {}..  
-000001b0: 2020 6669 6775 7265 5f64 6963 7420 3d20    figure_dict = 
-000001c0: 7b7d 0d0a 0d0a 2020 2020 6465 6620 5f63  {}....    def _c
-000001d0: 6865 636b 5f63 6f6e 6e65 6374 6564 2873  heck_connected(s
-000001e0: 656c 662c 2069 6e73 7429 3a0d 0a20 2020  elf, inst):..   
-000001f0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00000200: 6365 2869 6e73 742c 2049 6e73 7472 756d  ce(inst, Instrum
-00000210: 656e 7429 2061 6e64 2069 6e73 742e 6973  ent) and inst.is
-00000220: 5f63 6f6e 6e65 6374 6564 2829 3a0d 0a20  _connected():.. 
-00000230: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000240: 6e20 5472 7565 0d0a 2020 2020 2020 2020  n True..        
-00000250: 2320 7261 6973 6520 5661 6c75 6545 7272  # raise ValueErr
-00000260: 6f72 2827 227b 7d22 2069 7320 4e4f 5420  or('"{}" is NOT 
-00000270: 636f 6e6e 6563 7465 6427 2e66 6f72 6d61  connected'.forma
-00000280: 7428 696e 7374 2e67 6574 5f6e 616d 6528  t(inst.get_name(
-00000290: 2929 290d 0a20 2020 2020 2020 2072 6574  )))..        ret
-000002a0: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-000002b0: 2064 6566 2068 616e 646c 655f 636f 6d6d   def handle_comm
-000002c0: 616e 6428 7365 6c66 2c20 636d 642c 2072  and(self, cmd, r
-000002d0: 6570 6c79 293a 0d0a 2020 2020 2020 2020  eply):..        
-000002e0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000002f0: 2020 7265 706c 7920 3d20 274e 6f74 2063    reply = 'Not c
-00000300: 6f6e 6e65 6374 6564 270d 0a20 2020 2020  onnected'..     
-00000310: 2020 2020 2020 206b 6579 7320 3d20 6c69         keys = li
-00000320: 7374 2873 656c 662e 696e 7374 5f64 6963  st(self.inst_dic
-00000330: 742e 6b65 7973 2829 290d 0a0d 0a20 2020  t.keys())....   
-00000340: 2020 2020 2020 2020 2069 6e73 745f 6e61           inst_na
-00000350: 6d65 203d 2063 6d64 2e73 706c 6974 2827  me = cmd.split('
-00000360: 2e27 2c20 3129 5b30 5d0d 0a20 2020 2020  .', 1)[0]..     
-00000370: 2020 2020 2020 2069 6620 696e 7374 5f6e         if inst_n
-00000380: 616d 6520 696e 206b 6579 733a 0d0a 2020  ame in keys:..  
-00000390: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000003a0: 7374 203d 2073 656c 662e 696e 7374 5f64  st = self.inst_d
-000003b0: 6963 745b 696e 7374 5f6e 616d 655d 0d0a  ict[inst_name]..
-000003c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003d0: 6966 2073 656c 662e 5f63 6865 636b 5f63  if self._check_c
-000003e0: 6f6e 6e65 6374 6564 2869 6e73 7429 3a0d  onnected(inst):.
-000003f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000400: 2020 2020 2072 6570 6c79 203d 2073 656c       reply = sel
-00000410: 662e 6576 616c 2863 6d64 290d 0a20 2020  f.eval(cmd)..   
-00000420: 2020 2020 2020 2020 2065 6c69 6620 696e           elif in
-00000430: 7374 5f6e 616d 6520 696e 2073 656c 662e  st_name in self.
-00000440: 6669 6775 7265 5f64 6963 743a 0d0a 2020  figure_dict:..  
-00000450: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000460: 706c 7920 3d20 7365 6c66 2e65 7661 6c28  ply = self.eval(
-00000470: 636d 6429 0d0a 2020 2020 2020 2020 2020  cmd)..          
-00000480: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000490: 2020 2020 2020 2020 2069 6e73 745f 6e61           inst_na
-000004a0: 6d65 203d 2063 6d64 2e73 706c 6974 2827  me = cmd.split('
-000004b0: 3a27 2c20 3129 5b30 5d0d 0a20 2020 2020  :', 1)[0]..     
-000004c0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-000004d0: 7374 5f6e 616d 6520 696e 206b 6579 733a  st_name in keys:
-000004e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000004f0: 2020 2020 2020 696e 7374 203d 2073 656c        inst = sel
-00000500: 662e 696e 7374 5f64 6963 745b 696e 7374  f.inst_dict[inst
-00000510: 5f6e 616d 655d 0d0a 2020 2020 2020 2020  _name]..        
-00000520: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00000530: 656c 662e 5f63 6865 636b 5f63 6f6e 6e65  elf._check_conne
-00000540: 6374 6564 2869 6e73 7429 3a0d 0a20 2020  cted(inst):..   
-00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2020 2020 2063 6f6d 6d61 6e64 203d 2063       command = c
-00000570: 6d64 2e73 706c 6974 2827 3a27 2c20 3129  md.split(':', 1)
-00000580: 5b31 5d0d 0a20 2020 2020 2020 2020 2020  [1]..           
-00000590: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-000005a0: 6c79 203d 2069 6e73 742e 6861 6e64 6c65  ly = inst.handle
-000005b0: 5f63 6f6d 6d61 6e64 2863 6f6d 6d61 6e64  _command(command
-000005c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000005d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000005e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000005f0: 206b 6579 733a 0d0a 2020 2020 2020 2020   keys:..        
-00000600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000610: 696e 7374 203d 2073 656c 662e 696e 7374  inst = self.inst
-00000620: 5f64 6963 745b 6b65 7973 5b30 5d5d 0d0a  _dict[keys[0]]..
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00000650: 5f63 6865 636b 5f63 6f6e 6e65 6374 6564  _check_connected
-00000660: 2869 6e73 7429 3a0d 0a20 2020 2020 2020  (inst):..       
-00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 2020 2020 2072 6570 6c79 203d 2069 6e73       reply = ins
-00000690: 742e 6861 6e64 6c65 5f63 6f6d 6d61 6e64  t.handle_command
-000006a0: 2863 6d64 290d 0a20 2020 2020 2020 2020  (cmd)..         
-000006b0: 2020 2073 656c 662e 636f 6d6d 616e 645f     self.command_
-000006c0: 7072 6f63 6573 7365 642e 656d 6974 2863  processed.emit(c
-000006d0: 6d64 2c20 7265 706c 7929 0d0a 2020 2020  md, reply)..    
-000006e0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-000006f0: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-00000700: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00000710: 7272 6f72 2827 4572 726f 7220 6672 6f6d  rror('Error from
-00000720: 2043 6f6d 6d61 6e64 4861 6e64 6c65 723a   CommandHandler:
-00000730: 207b 7d27 2e66 6f72 6d61 7428 7374 7228   {}'.format(str(
-00000740: 6529 2929 0d0a 0d0a 2020 2020 6465 6620  e)))....    def 
-00000750: 6576 616c 2873 656c 662c 2063 6d64 293a  eval(self, cmd):
-00000760: 0d0a 2020 2020 2020 2020 6966 2027 3d27  ..        if '='
-00000770: 2069 6e20 636d 643a 0d0a 2020 2020 2020   in cmd:..      
-00000780: 2020 2020 2020 2320 544f 444f 3a20 6368        # TODO: ch
-00000790: 6563 6b20 6966 2061 7373 6967 6e65 6420  eck if assigned 
-000007a0: 746f 2061 2063 6f6d 6d61 6e64 0d0a 2020  to a command..  
-000007b0: 2020 2020 2020 2020 2020 6578 6563 2863            exec(c
-000007c0: 6d64 2c20 7b7d 2c20 7365 6c66 2e69 6e73  md, {}, self.ins
-000007d0: 745f 6469 6374 290d 0a20 2020 2020 2020  t_dict)..       
-000007e0: 2020 2020 2072 6574 7572 6e20 2727 0d0a       return ''..
-000007f0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00000800: 2020 2020 2020 2020 2020 2022 2222 0d0a             """..
-00000810: 2020 2020 2020 2020 2020 2020 2320 616c              # al
-00000820: 7465 726e 6174 6976 6520 6576 616c 2066  ternative eval f
-00000830: 756e 6374 696f 6e3a 2064 6f65 7320 6e6f  unction: does no
-00000840: 7420 776f 726b 2077 6974 6820 496e 6465  t work with Inde
-00000850: 7843 6f6d 6d61 6e64 2079 6574 0d0a 2020  xCommand yet..  
-00000860: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
-00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000880: 746f 6b65 6e73 203d 2063 6d64 2e73 706c  tokens = cmd.spl
-00000890: 6974 2827 2e27 290d 0a20 2020 2020 2020  it('.')..       
-000008a0: 2020 2020 2020 2020 2069 6620 746f 6b65           if toke
-000008b0: 6e73 5b30 5d20 696e 2073 656c 662e 696e  ns[0] in self.in
-000008c0: 7374 5f64 6963 743a 0d0a 2020 2020 2020  st_dict:..      
-000008d0: 2020 2020 2020 2020 2020 2020 2020 6174                at
-000008e0: 7472 203d 2073 656c 662e 696e 7374 5f64  tr = self.inst_d
-000008f0: 6963 745b 746f 6b65 6e73 5b30 5d5d 0d0a  ict[tokens[0]]..
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 666f 7220 746f 6b65 6e20 696e      for token in
-00000920: 2074 6f6b 656e 735b 313a 5d3a 0d0a 2020   tokens[1:]:..  
-00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000940: 2020 2020 2020 6174 7472 203d 2067 6574        attr = get
-00000950: 6174 7472 2861 7474 722c 2074 6f6b 656e  attr(attr, token
-00000960: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00000970: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00000980: 7228 6174 7472 290d 0a20 2020 2020 2020  r(attr)..       
-00000990: 2020 2020 2020 2020 2065 6c69 6620 746f           elif to
-000009a0: 6b65 6e73 5b30 5d20 696e 2073 656c 662e  kens[0] in self.
-000009b0: 6669 6775 7265 5f64 6963 743a 0d0a 2020  figure_dict:..  
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 6174 7472 203d 2073 656c 662e 6669    attr = self.fi
-000009e0: 6775 7265 5f64 6963 745b 746f 6b65 6e73  gure_dict[tokens
-000009f0: 5b30 5d5d 0d0a 2020 2020 2020 2020 2020  [0]]..          
-00000a00: 2020 2020 2020 2020 2020 666f 7220 746f            for to
-00000a10: 6b65 6e20 696e 2074 6f6b 656e 735b 313a  ken in tokens[1:
-00000a20: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
-00000a30: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-00000a40: 203d 2067 6574 6174 7472 2861 7474 722c   = getattr(attr,
-00000a50: 2074 6f6b 656e 290d 0a20 2020 2020 2020   token)..       
-00000a60: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00000a70: 7572 6e20 7374 7228 6174 7472 290d 0a20  urn str(attr).. 
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00000a90: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000aa0: 2020 2020 2020 2020 2020 4b65 7945 7272            KeyErr
-00000ab0: 6f72 2827 556e 6b6e 6f77 6e20 6174 7472  or('Unknown attr
-00000ac0: 6962 7574 653a 207b 7d27 2e66 6f72 6d61  ibute: {}'.forma
-00000ad0: 7428 746f 6b65 6e73 5b30 5d29 290d 0a20  t(tokens[0])).. 
-00000ae0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00000af0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00000b00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000b10: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
-00000b20: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00000b30: 2020 2020 7265 7475 726e 2027 270d 0a20      return ''.. 
-00000b40: 2020 2020 2020 2020 2020 2022 2222 0d0a             """..
-00000b50: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00000b60: 7920 3d20 6576 616c 2863 6d64 2c20 7365  y = eval(cmd, se
-00000b70: 6c66 2e66 6967 7572 655f 6469 6374 2c20  lf.figure_dict, 
-00000b80: 7365 6c66 2e69 6e73 745f 6469 6374 290d  self.inst_dict).
-00000b90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000ba0: 7265 706c 7920 6973 206e 6f74 204e 6f6e  reply is not Non
-00000bb0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000bc0: 2020 2020 7265 7475 726e 2073 7472 2872      return str(r
-00000bd0: 6570 6c79 290d 0a20 2020 2020 2020 2020  eply)..         
-00000be0: 2020 2072 6574 7572 6e20 2727 0d0a 0d0a     return ''....
-00000bf0: 0d0a 636c 6173 7320 436f 6d6d 616e 6448  ..class CommandH
-00000c00: 616e 646c 6572 2851 4f62 6a65 6374 293a  andler(QObject):
-00000c10: 0d0a 2020 2020 7265 7175 6573 745f 636f  ..    request_co
-00000c20: 6d6d 616e 6420 3d20 5369 676e 616c 2873  mmand = Signal(s
-00000c30: 7472 2c20 7374 7229 0d0a 2020 2020 636f  tr, str)..    co
-00000c40: 6d6d 616e 645f 7072 6f63 6573 7365 6420  mmand_processed 
-00000c50: 3d20 5369 676e 616c 2873 7472 2c20 7374  = Signal(str, st
-00000c60: 7229 0d0a 0d0a 2020 2020 6465 6620 5f5f  r)....    def __
-00000c70: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
-00000c80: 656e 7429 3a0d 0a20 2020 2020 2020 2073  ent):..        s
-00000c90: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00000ca0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000cb0: 7061 7265 6e74 203d 2070 6172 656e 740d  parent = parent.
-00000cc0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-00000cd0: 726b 6572 5f74 6872 6561 6420 3d20 5154  rker_thread = QT
-00000ce0: 6872 6561 6428 290d 0a0d 0a20 2020 2020  hread()....     
-00000cf0: 2020 2073 656c 662e 776f 726b 6572 203d     self.worker =
-00000d00: 2043 6f6d 6d61 6e64 576f 726b 6572 2829   CommandWorker()
-00000d10: 0d0a 2020 2020 2020 2020 7365 6c66 2e77  ..        self.w
-00000d20: 6f72 6b65 722e 6d6f 7665 546f 5468 7265  orker.moveToThre
-00000d30: 6164 2873 656c 662e 776f 726b 6572 5f74  ad(self.worker_t
-00000d40: 6872 6561 6429 0d0a 2020 2020 2020 2020  hread)..        
-00000d50: 7365 6c66 2e72 6571 7565 7374 5f63 6f6d  self.request_com
-00000d60: 6d61 6e64 2e63 6f6e 6e65 6374 2873 656c  mand.connect(sel
-00000d70: 662e 776f 726b 6572 2e68 616e 646c 655f  f.worker.handle_
-00000d80: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
-00000d90: 2020 7365 6c66 2e77 6f72 6b65 722e 636f    self.worker.co
-00000da0: 6d6d 616e 645f 7072 6f63 6573 7365 642e  mmand_processed.
-00000db0: 636f 6e6e 6563 7428 7365 6c66 2e63 6f6d  connect(self.com
-00000dc0: 6d61 6e64 5f70 726f 6365 7373 6564 290d  mand_processed).
-00000dd0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-00000de0: 726b 6572 5f74 6872 6561 642e 7374 6172  rker_thread.star
-00000df0: 7428 290d 0a0d 0a20 2020 2064 6566 2070  t()....    def p
-00000e00: 726f 6365 7373 5f63 6f6d 6d61 6e64 2873  rocess_command(s
-00000e10: 656c 662c 2063 6d64 2c20 7265 706c 7929  elf, cmd, reply)
-00000e20: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
-00000e30: 776f 726b 6572 2e69 6e73 745f 6469 6374  worker.inst_dict
-00000e40: 203d 2073 656c 662e 7061 7265 6e74 2e69   = self.parent.i
-00000e50: 6e73 745f 6469 6374 0d0a 2020 2020 2020  nst_dict..      
-00000e60: 2020 7365 6c66 2e77 6f72 6b65 722e 6669    self.worker.fi
-00000e70: 6775 7265 5f64 6963 7420 3d20 7365 6c66  gure_dict = self
-00000e80: 2e70 6172 656e 742e 646f 636b 5f68 616e  .parent.dock_han
-00000e90: 646c 6572 2e67 6574 5f66 6967 7572 655f  dler.get_figure_
-00000ea0: 6469 6374 2829 0d0a 2020 2020 2020 2020  dict()..        
-00000eb0: 7365 6c66 2e72 6571 7565 7374 5f63 6f6d  self.request_com
-00000ec0: 6d61 6e64 2e65 6d69 7428 636d 642c 2072  mand.emit(cmd, r
-00000ed0: 6570 6c79 290d 0a0d 0a20 2020 2064 6566  eply)....    def
-00000ee0: 2073 746f 7028 7365 6c66 293a 0d0a 2020   stop(self):..  
-00000ef0: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
-00000f00: 725f 7468 7265 6164 2e71 7569 7428 290d  r_thread.quit().
-00000f10: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-00000f20: 726b 6572 5f74 6872 6561 642e 7761 6974  rker_thread.wait
-00000f30: 2829 0d0a 0d0a                           ()....
+00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
+00000010: 6d70 6f72 7420 6c6f 6767 696e 670d 0a66  mport logging..f
+00000020: 726f 6d20 2e71 742e 5174 436f 7265 2069  rom .qt.QtCore i
+00000030: 6d70 6f72 7420 514f 626a 6563 742c 2051  mport QObject, Q
+00000040: 5468 7265 6164 2c20 5369 676e 616c 2c20  Thread, Signal, 
+00000050: 536c 6f74 0d0a 6672 6f6d 202e 7174 2e51  Slot..from .qt.Q
+00000060: 7457 6964 6765 7473 2069 6d70 6f72 7420  tWidgets import 
+00000070: 514d 6573 7361 6765 426f 780d 0a0d 0a66  QMessageBox....f
+00000080: 726f 6d20 7372 7367 7569 2e69 6e73 742e  rom srsgui.inst.
+00000090: 696e 7374 7275 6d65 6e74 2069 6d70 6f72  instrument impor
+000000a0: 7420 496e 7374 7275 6d65 6e74 0d0a 0d0a  t Instrument....
+000000b0: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
+000000c0: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
+000000d0: 655f 5f29 0d0a 0d0a 0d0a 636c 6173 7320  e__)......class 
+000000e0: 436f 6d6d 616e 6457 6f72 6b65 7228 514f  CommandWorker(QO
+000000f0: 626a 6563 7429 3a0d 0a20 2020 2063 6f6d  bject):..    com
+00000100: 6d61 6e64 5f70 726f 6365 7373 6564 203d  mand_processed =
+00000110: 2053 6967 6e61 6c28 7374 722c 2073 7472   Signal(str, str
+00000120: 290d 0a20 2020 2069 6e73 745f 6469 6374  )..    inst_dict
+00000130: 203d 207b 7d0d 0a20 2020 2066 6967 7572   = {}..    figur
+00000140: 655f 6469 6374 203d 207b 7d0d 0a0d 0a20  e_dict = {}.... 
+00000150: 2020 2064 6566 205f 6368 6563 6b5f 636f     def _check_co
+00000160: 6e6e 6563 7465 6428 7365 6c66 2c20 696e  nnected(self, in
+00000170: 7374 293a 0d0a 2020 2020 2020 2020 6966  st):..        if
+00000180: 2069 7369 6e73 7461 6e63 6528 696e 7374   isinstance(inst
+00000190: 2c20 496e 7374 7275 6d65 6e74 2920 616e  , Instrument) an
+000001a0: 6420 696e 7374 2e69 735f 636f 6e6e 6563  d inst.is_connec
+000001b0: 7465 6428 293a 0d0a 2020 2020 2020 2020  ted():..        
+000001c0: 2020 2020 7265 7475 726e 2054 7275 650d      return True.
+000001d0: 0a20 2020 2020 2020 2023 2072 6169 7365  .        # raise
+000001e0: 2056 616c 7565 4572 726f 7228 2722 7b7d   ValueError('"{}
+000001f0: 2220 6973 204e 4f54 2063 6f6e 6e65 6374  " is NOT connect
+00000200: 6564 272e 666f 726d 6174 2869 6e73 742e  ed'.format(inst.
+00000210: 6765 745f 6e61 6d65 2829 2929 0d0a 2020  get_name()))..  
+00000220: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00000230: 7365 0d0a 0d0a 2020 2020 6465 6620 6861  se....    def ha
+00000240: 6e64 6c65 5f63 6f6d 6d61 6e64 2873 656c  ndle_command(sel
+00000250: 662c 2063 6d64 2c20 7265 706c 7929 3a0d  f, cmd, reply):.
+00000260: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00000270: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
+00000280: 203d 2027 4e6f 7420 636f 6e6e 6563 7465   = 'Not connecte
+00000290: 6427 0d0a 2020 2020 2020 2020 2020 2020  d'..            
+000002a0: 6b65 7973 203d 206c 6973 7428 7365 6c66  keys = list(self
+000002b0: 2e69 6e73 745f 6469 6374 2e6b 6579 7328  .inst_dict.keys(
+000002c0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000002d0: 2020 696e 7374 5f6e 616d 6520 3d20 636d    inst_name = cm
+000002e0: 642e 7370 6c69 7428 272e 272c 2031 295b  d.split('.', 1)[
+000002f0: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00000300: 6966 2069 6e73 745f 6e61 6d65 2069 6e20  if inst_name in 
+00000310: 6b65 7973 3a0d 0a20 2020 2020 2020 2020  keys:..         
+00000320: 2020 2020 2020 2069 6e73 7420 3d20 7365         inst = se
+00000330: 6c66 2e69 6e73 745f 6469 6374 5b69 6e73  lf.inst_dict[ins
+00000340: 745f 6e61 6d65 5d0d 0a20 2020 2020 2020  t_name]..       
+00000350: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00000360: 2e5f 6368 6563 6b5f 636f 6e6e 6563 7465  ._check_connecte
+00000370: 6428 696e 7374 293a 0d0a 2020 2020 2020  d(inst):..      
+00000380: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000390: 706c 7920 3d20 7365 6c66 2e65 7661 6c28  ply = self.eval(
+000003a0: 636d 6429 0d0a 2020 2020 2020 2020 2020  cmd)..          
+000003b0: 2020 656c 6966 2069 6e73 745f 6e61 6d65    elif inst_name
+000003c0: 2069 6e20 7365 6c66 2e66 6967 7572 655f   in self.figure_
+000003d0: 6469 6374 3a0d 0a20 2020 2020 2020 2020  dict:..         
+000003e0: 2020 2020 2020 2072 6570 6c79 203d 2073         reply = s
+000003f0: 656c 662e 6576 616c 2863 6d64 290d 0a20  elf.eval(cmd).. 
+00000400: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00000410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000420: 2020 696e 7374 5f6e 616d 6520 3d20 636d    inst_name = cm
+00000430: 642e 7370 6c69 7428 273a 272c 2031 295b  d.split(':', 1)[
+00000440: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
+00000450: 2020 2020 6966 2069 6e73 745f 6e61 6d65      if inst_name
+00000460: 2069 6e20 6b65 7973 3a0d 0a20 2020 2020   in keys:..     
+00000470: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000480: 6e73 7420 3d20 7365 6c66 2e69 6e73 745f  nst = self.inst_
+00000490: 6469 6374 5b69 6e73 745f 6e61 6d65 5d0d  dict[inst_name].
+000004a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000004b0: 2020 2020 2069 6620 7365 6c66 2e5f 6368       if self._ch
+000004c0: 6563 6b5f 636f 6e6e 6563 7465 6428 696e  eck_connected(in
+000004d0: 7374 293a 0d0a 2020 2020 2020 2020 2020  st):..          
+000004e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000004f0: 6d6d 616e 6420 3d20 636d 642e 7370 6c69  mmand = cmd.spli
+00000500: 7428 273a 272c 2031 295b 315d 0d0a 2020  t(':', 1)[1]..  
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 2020 2020 2020 7265 706c 7920 3d20 696e        reply = in
+00000530: 7374 2e68 616e 646c 655f 636f 6d6d 616e  st.handle_comman
+00000540: 6428 636f 6d6d 616e 6429 0d0a 2020 2020  d(command)..    
+00000550: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00000560: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000570: 2020 2020 2020 2069 6620 6b65 7973 3a0d         if keys:.
+00000580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000590: 2020 2020 2020 2020 2069 6e73 7420 3d20           inst = 
+000005a0: 7365 6c66 2e69 6e73 745f 6469 6374 5b6b  self.inst_dict[k
+000005b0: 6579 735b 305d 5d0d 0a20 2020 2020 2020  eys[0]]..       
+000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005d0: 2069 6620 7365 6c66 2e5f 6368 6563 6b5f   if self._check_
+000005e0: 636f 6e6e 6563 7465 6428 696e 7374 293a  connected(inst):
+000005f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000600: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000610: 706c 7920 3d20 696e 7374 2e68 616e 646c  ply = inst.handl
+00000620: 655f 636f 6d6d 616e 6428 636d 6429 0d0a  e_command(cmd)..
+00000630: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000640: 2e63 6f6d 6d61 6e64 5f70 726f 6365 7373  .command_process
+00000650: 6564 2e65 6d69 7428 636d 642c 2072 6570  ed.emit(cmd, rep
+00000660: 6c79 290d 0a20 2020 2020 2020 2065 7863  ly)..        exc
+00000670: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00000680: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
+00000690: 206c 6f67 6765 722e 6572 726f 7228 2745   logger.error('E
+000006a0: 7272 6f72 2066 726f 6d20 436f 6d6d 616e  rror from Comman
+000006b0: 6448 616e 646c 6572 3a20 7b7d 272e 666f  dHandler: {}'.fo
+000006c0: 726d 6174 2873 7472 2865 2929 290d 0a0d  rmat(str(e)))...
+000006d0: 0a20 2020 2064 6566 2065 7661 6c28 7365  .    def eval(se
+000006e0: 6c66 2c20 636d 6429 3a0d 0a20 2020 2020  lf, cmd):..     
+000006f0: 2020 2069 6620 273d 2720 696e 2063 6d64     if '=' in cmd
+00000700: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00000710: 2054 4f44 4f3a 2063 6865 636b 2069 6620   TODO: check if 
+00000720: 6173 7369 676e 6564 2074 6f20 6120 636f  assigned to a co
+00000730: 6d6d 616e 640d 0a20 2020 2020 2020 2020  mmand..         
+00000740: 2020 2065 7865 6328 636d 642c 207b 7d2c     exec(cmd, {},
+00000750: 2073 656c 662e 696e 7374 5f64 6963 7429   self.inst_dict)
+00000760: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00000770: 7475 726e 2027 270d 0a20 2020 2020 2020  turn ''..       
+00000780: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00000790: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000007a0: 2020 2020 2023 2061 6c74 6572 6e61 7469       # alternati
+000007b0: 7665 2065 7661 6c20 6675 6e63 7469 6f6e  ve eval function
+000007c0: 3a20 646f 6573 206e 6f74 2077 6f72 6b20  : does not work 
+000007d0: 7769 7468 2049 6e64 6578 436f 6d6d 616e  with IndexComman
+000007e0: 6420 7965 740d 0a20 2020 2020 2020 2020  d yet..         
+000007f0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00000800: 2020 2020 2020 2020 2074 6f6b 656e 7320           tokens 
+00000810: 3d20 636d 642e 7370 6c69 7428 272e 2729  = cmd.split('.')
+00000820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000830: 2020 6966 2074 6f6b 656e 735b 305d 2069    if tokens[0] i
+00000840: 6e20 7365 6c66 2e69 6e73 745f 6469 6374  n self.inst_dict
+00000850: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000860: 2020 2020 2020 2061 7474 7220 3d20 7365         attr = se
+00000870: 6c66 2e69 6e73 745f 6469 6374 5b74 6f6b  lf.inst_dict[tok
+00000880: 656e 735b 305d 5d0d 0a20 2020 2020 2020  ens[0]]..       
+00000890: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000008a0: 2074 6f6b 656e 2069 6e20 746f 6b65 6e73   token in tokens
+000008b0: 5b31 3a5d 3a0d 0a20 2020 2020 2020 2020  [1:]:..         
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000008d0: 7474 7220 3d20 6765 7461 7474 7228 6174  ttr = getattr(at
+000008e0: 7472 2c20 746f 6b65 6e29 0d0a 2020 2020  tr, token)..    
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 7265 7475 726e 2073 7472 2861 7474 7229  return str(attr)
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000920: 2020 656c 6966 2074 6f6b 656e 735b 305d    elif tokens[0]
+00000930: 2069 6e20 7365 6c66 2e66 6967 7572 655f   in self.figure_
+00000940: 6469 6374 3a0d 0a20 2020 2020 2020 2020  dict:..         
+00000950: 2020 2020 2020 2020 2020 2061 7474 7220             attr 
+00000960: 3d20 7365 6c66 2e66 6967 7572 655f 6469  = self.figure_di
+00000970: 6374 5b74 6f6b 656e 735b 305d 5d0d 0a20  ct[tokens[0]].. 
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 2020 2066 6f72 2074 6f6b 656e 2069 6e20     for token in 
+000009a0: 746f 6b65 6e73 5b31 3a5d 3a0d 0a20 2020  tokens[1:]:..   
+000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009c0: 2020 2020 2061 7474 7220 3d20 6765 7461       attr = geta
+000009d0: 7474 7228 6174 7472 2c20 746f 6b65 6e29  ttr(attr, token)
+000009e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000009f0: 2020 2020 2020 7265 7475 726e 2073 7472        return str
+00000a00: 2861 7474 7229 0d0a 2020 2020 2020 2020  (attr)..        
+00000a10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a30: 2020 204b 6579 4572 726f 7228 2755 6e6b     KeyError('Unk
+00000a40: 6e6f 776e 2061 7474 7269 6275 7465 3a20  nown attribute: 
+00000a50: 7b7d 272e 666f 726d 6174 2874 6f6b 656e  {}'.format(token
+00000a60: 735b 305d 2929 0d0a 2020 2020 2020 2020  s[0]))..        
+00000a70: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00000a80: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
+00000a90: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00000aa0: 6572 2e65 7272 6f72 2865 290d 0a20 2020  er.error(e)..   
+00000ab0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000ac0: 7572 6e20 2727 0d0a 2020 2020 2020 2020  urn ''..        
+00000ad0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00000ae0: 2020 2020 2072 6570 6c79 203d 2065 7661       reply = eva
+00000af0: 6c28 636d 642c 2073 656c 662e 6669 6775  l(cmd, self.figu
+00000b00: 7265 5f64 6963 742c 2073 656c 662e 696e  re_dict, self.in
+00000b10: 7374 5f64 6963 7429 0d0a 2020 2020 2020  st_dict)..      
+00000b20: 2020 2020 2020 6966 2072 6570 6c79 2069        if reply i
+00000b30: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00000b40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00000b50: 7572 6e20 7374 7228 7265 706c 7929 0d0a  urn str(reply)..
+00000b60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000b70: 726e 2027 270d 0a0d 0a0d 0a63 6c61 7373  rn ''......class
+00000b80: 2043 6f6d 6d61 6e64 4861 6e64 6c65 7228   CommandHandler(
+00000b90: 514f 626a 6563 7429 3a0d 0a20 2020 2072  QObject):..    r
+00000ba0: 6571 7565 7374 5f63 6f6d 6d61 6e64 203d  equest_command =
+00000bb0: 2053 6967 6e61 6c28 7374 722c 2073 7472   Signal(str, str
+00000bc0: 290d 0a20 2020 2063 6f6d 6d61 6e64 5f70  )..    command_p
+00000bd0: 726f 6365 7373 6564 203d 2053 6967 6e61  rocessed = Signa
+00000be0: 6c28 7374 722c 2073 7472 290d 0a0d 0a20  l(str, str).... 
+00000bf0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000c00: 7365 6c66 2c20 7061 7265 6e74 293a 0d0a  self, parent):..
+00000c10: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00000c20: 5f5f 696e 6974 5f5f 2829 0d0a 2020 2020  __init__()..    
+00000c30: 2020 2020 7365 6c66 2e70 6172 656e 7420      self.parent 
+00000c40: 3d20 7061 7265 6e74 0d0a 2020 2020 2020  = parent..      
+00000c50: 2020 7365 6c66 2e77 6f72 6b65 725f 7468    self.worker_th
+00000c60: 7265 6164 203d 2051 5468 7265 6164 2829  read = QThread()
+00000c70: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00000c80: 2e77 6f72 6b65 7220 3d20 436f 6d6d 616e  .worker = Comman
+00000c90: 6457 6f72 6b65 7228 290d 0a20 2020 2020  dWorker()..     
+00000ca0: 2020 2073 656c 662e 776f 726b 6572 2e6d     self.worker.m
+00000cb0: 6f76 6554 6f54 6872 6561 6428 7365 6c66  oveToThread(self
+00000cc0: 2e77 6f72 6b65 725f 7468 7265 6164 290d  .worker_thread).
+00000cd0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00000ce0: 7175 6573 745f 636f 6d6d 616e 642e 636f  quest_command.co
+00000cf0: 6e6e 6563 7428 7365 6c66 2e77 6f72 6b65  nnect(self.worke
+00000d00: 722e 6861 6e64 6c65 5f63 6f6d 6d61 6e64  r.handle_command
+00000d10: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00000d20: 776f 726b 6572 2e63 6f6d 6d61 6e64 5f70  worker.command_p
+00000d30: 726f 6365 7373 6564 2e63 6f6e 6e65 6374  rocessed.connect
+00000d40: 2873 656c 662e 636f 6d6d 616e 645f 7072  (self.command_pr
+00000d50: 6f63 6573 7365 6429 0d0a 2020 2020 2020  ocessed)..      
+00000d60: 2020 7365 6c66 2e77 6f72 6b65 725f 7468    self.worker_th
+00000d70: 7265 6164 2e73 7461 7274 2829 0d0a 0d0a  read.start()....
+00000d80: 2020 2020 6465 6620 7072 6f63 6573 735f      def process_
+00000d90: 636f 6d6d 616e 6428 7365 6c66 2c20 636d  command(self, cm
+00000da0: 642c 2072 6570 6c79 293a 0d0a 2020 2020  d, reply):..    
+00000db0: 2020 2020 7365 6c66 2e77 6f72 6b65 722e      self.worker.
+00000dc0: 696e 7374 5f64 6963 7420 3d20 7365 6c66  inst_dict = self
+00000dd0: 2e70 6172 656e 742e 696e 7374 5f64 6963  .parent.inst_dic
+00000de0: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+00000df0: 776f 726b 6572 2e66 6967 7572 655f 6469  worker.figure_di
+00000e00: 6374 203d 2073 656c 662e 7061 7265 6e74  ct = self.parent
+00000e10: 2e64 6f63 6b5f 6861 6e64 6c65 722e 6765  .dock_handler.ge
+00000e20: 745f 6669 6775 7265 5f64 6963 7428 290d  t_figure_dict().
+00000e30: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00000e40: 7175 6573 745f 636f 6d6d 616e 642e 656d  quest_command.em
+00000e50: 6974 2863 6d64 2c20 7265 706c 7929 0d0a  it(cmd, reply)..
+00000e60: 0d0a 2020 2020 6465 6620 7374 6f70 2873  ..    def stop(s
+00000e70: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+00000e80: 656c 662e 776f 726b 6572 5f74 6872 6561  elf.worker_threa
+00000e90: 642e 7175 6974 2829 0d0a 2020 2020 2020  d.quit()..      
+00000ea0: 2020 7365 6c66 2e77 6f72 6b65 725f 7468    self.worker_th
+00000eb0: 7265 6164 2e77 6169 7428 290d 0a0d 0a    read.wait()....
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandterminal.py` & `srsgui-0.2.9/srsgui/ui/commandterminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import logging
 from .qt.QtCore import Signal
 
 from .qt.QtGui import QKeySequence
 from .qt.QtWidgets import QFrame, QMessageBox, QShortcut, \
                           QVBoxLayout, QHBoxLayout, QTextBrowser, QPushButton, QLineEdit
@@ -151,14 +147,10 @@
             self.command_requested.emit(cmd, '')
 
         except Exception as e:
             self.tbCommand.append('Error: {}'.format(str(e)))
 
     def handle_command(self, cmd, reply):
         try:
-            if reply:
-                self.tbCommand.append(f'{cmd}   ==>   {reply}')
-            else:
-                self.tbCommand.append(f'{cmd}')
-
+            self.tbCommand.append(f'{cmd}  :  {reply}')
         except Exception as e:
             self.tbCommand.append('Error from CommandTerminal: {}'.format(str(e)))
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanddelegate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,17 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
-import logging
 
 from srsgui.ui.qt.QtCore import Qt
 from srsgui.ui.qt.QtWidgets import QStyledItemDelegate, QComboBox
 
 from srsgui.inst import DictCommand, FloatCommand, IntCommand, \
                         FloatIndexCommand, IntIndexCommand, DictIndexCommand
 
 from .commandspinbox import FloatSpinBox, IntegerSpinBox
 from .commanditem import Index
 
-logger = logging.getLogger(__file__)
-
 
 class CommandDelegate(QStyledItemDelegate):
     """ A custom delegate for editing CommandItem """
     def __init__(self, parent=None):
         super().__init__(parent)
 
     def createEditor(self, parent, option, index):
@@ -27,80 +19,75 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
             editor = FloatSpinBox(parent)
             editor.setDecimals(10)
             editor.setSingleStep(0.1)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             editor.set_significant_figures(comp.significant_figures)
             editor.set_minimum_step(comp.step)
             return editor
 
-        elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
+        elif comp_type in (IntCommand, IntIndexCommand):
             editor = IntegerSpinBox(parent)
             editor.setMinimum(comp.minimum)
             editor.setMaximum(comp.maximum)
-            editor.setSuffix(' ' + comp.unit)
+            editor.setSuffix(comp.unit)
             return editor
 
         elif comp_type in (DictCommand, DictIndexCommand):
             editor = QComboBox(parent)
             for key in comp.set_dict.keys():
                 editor.addItem(str(key))
             return editor
 
         else:
             return super().createEditor(parent, option, index)
 
     def setEditorData(self, editor, index):
-
         if type(editor) in (FloatSpinBox, IntegerSpinBox):
             item = index.internalPointer()
             val = index.model().data(index, Qt.EditRole)
             editor.setValue(val)
 
         elif type(editor) == QComboBox:
             item = index.internalPointer()
             val = index.model().data(index, Qt.EditRole)
             editor.setCurrentText(str(val))
         return super().setEditorData(editor, index)
 
     def setModelData(self, editor, model, index):
+        item = index.internalPointer()
+        if item.comp_type == Index:
+            comp = item.parent().comp
+            comp_type = item.parent().comp_type
+        else:
+            comp = item.comp
+            comp_type = item.comp_type
 
-        try:
-            item = index.internalPointer()
-            if item.comp_type == Index:
-                comp = item.parent().comp
-                comp_type = item.parent().comp_type
-            else:
-                comp = item.comp
-                comp_type = item.comp_type
-
-            if issubclass(comp_type, FloatCommand) or issubclass(comp_type, FloatIndexCommand):
-                value = editor.value()
-                model.setData(index, value, Qt.EditRole)
-                item.precision = editor.precision
-            elif issubclass(comp_type, IntCommand) or issubclass(comp_type, IntIndexCommand):
-                pass
-
-                value = editor.value()
-                model.setData(index, value, Qt.EditRole)
-            elif comp_type in (DictCommand, DictIndexCommand):
-                val = editor.currentText()
-                convert = type(list(comp.get_dict.keys())[0])
-                value = convert(val)
-                model.setData(index, value, Qt.EditRole)
-            else:
-                return super().setModelData(editor, model, index)
-        except Exception as e:
-            logger.error(e)
+        if comp_type in (FloatCommand, FloatIndexCommand):
+            value = editor.value()
+            model.setData(index, value, Qt.EditRole)
+            item.precision = editor.precision
+            return True
+        elif comp_type in (IntCommand, IntIndexCommand):
+            value = editor.value()
+            model.setData(index, value, Qt.EditRole)
+            return True
+        elif comp_type in (DictCommand, DictIndexCommand):
+            val = editor.currentText()
+            convert = type(list(comp.get_dict.keys())[0])
+            value = convert(val)
+            model.setData(index, value, Qt.EditRole)
+            return True
+        return super().setModelData(editor, model, index)
 
     def updateEditorGeometry(self, editor, option, index):
         return super().updateEditorGeometry(editor, option, index)
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commanditem.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,754 +1,637 @@
-00000000: 2323 2120 0d0a 2323 2120 436f 7074 7269  ##! ..##! Coptri
-00000010: 6768 7428 6329 2032 3032 322c 2032 3032  ght(c) 2022, 202
-00000020: 3320 5374 616e 666f 7264 2052 6573 6561  3 Stanford Resea
-00000030: 7263 6820 5379 7374 656d 732c 2041 6c6c  rch Systems, All
-00000040: 2072 6967 6874 2072 6573 6572 7665 640d   right reserved.
-00000050: 0a23 2321 2053 7562 6a65 6374 2074 6f20  .##! Subject to 
-00000060: 7468 6520 4d49 5420 4c69 6365 6e73 650d  the MIT License.
-00000070: 0a23 2321 200d 0a0d 0a69 6d70 6f72 7420  .##! ....import 
-00000080: 7469 6d65 0d0a 696d 706f 7274 206d 6174  time..import mat
-00000090: 680d 0a0d 0a66 726f 6d20 7372 7367 7569  h....from srsgui
-000000a0: 2069 6d70 6f72 7420 436f 6d70 6f6e 656e   import Componen
-000000b0: 740d 0a66 726f 6d20 7372 7367 7569 2e69  t..from srsgui.i
-000000c0: 6e73 7420 696d 706f 7274 2043 6f6d 6d61  nst import Comma
-000000d0: 6e64 2c20 496e 6465 7843 6f6d 6d61 6e64  nd, IndexCommand
-000000e0: 2c20 5c0d 0a20 2020 2020 2020 2020 2020  , \..           
-000000f0: 2020 2020 2020 2020 2020 2020 2046 6c6f               Flo
-00000100: 6174 436f 6d6d 616e 642c 2046 6c6f 6174  atCommand, Float
-00000110: 496e 6465 7843 6f6d 6d61 6e64 0d0a 0d0a  IndexCommand....
-00000120: 0d0a 636c 6173 7320 496e 6465 783a 0d0a  ..class Index:..
-00000130: 2020 2020 7061 7373 0d0a 0d0a 0d0a 636c      pass......cl
-00000140: 6173 7320 436f 6d6d 616e 6449 7465 6d3a  ass CommandItem:
-00000150: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
-00000160: 6f6d 6d61 6e64 2069 7465 6d20 636f 7272  ommand item corr
-00000170: 6573 706f 6e64 696e 6720 746f 2061 206c  esponding to a l
-00000180: 696e 6520 696e 2051 5472 6565 5669 6577  ine in QTreeView
-00000190: 2e20 4974 2065 6e63 6170 7375 6c61 7465  . It encapsulate
-000001a0: 730d 0a20 2020 2043 6f6d 706f 6e65 6e74  s..    Component
-000001b0: 2c20 436f 6d6d 616e 642c 2061 6e64 2049  , Command, and I
-000001c0: 6e64 6578 2063 6c61 7373 2075 7365 6420  ndex class used 
-000001d0: 696e 2073 7273 6775 692e 496e 7374 7275  in srsgui.Instru
-000001e0: 6d65 6e74 2063 6c61 7373 2e0d 0a20 2020  ment class...   
-000001f0: 2022 2222 0d0a 0d0a 2020 2020 6465 6620   """....    def 
-00000200: 5f5f 696e 6974 5f5f 2873 656c 662c 2070  __init__(self, p
-00000210: 6172 656e 743a 2022 436f 6d6d 616e 6449  arent: "CommandI
-00000220: 7465 6d22 203d 204e 6f6e 6529 3a0d 0a20  tem" = None):.. 
-00000230: 2020 2020 2020 2073 656c 662e 5f70 6172         self._par
-00000240: 656e 7420 3d20 7061 7265 6e74 0d0a 2020  ent = parent..  
-00000250: 2020 2020 2020 7365 6c66 2e5f 6368 696c        self._chil
-00000260: 6472 656e 203d 205b 5d0d 0a20 2020 2020  dren = []..     
-00000270: 2020 2073 656c 662e 5f76 616c 7565 203d     self._value =
-00000280: 204e 6f6e 650d 0a20 2020 2020 2020 200d   None..        .
-00000290: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-000002a0: 6d65 203d 2022 220d 0a20 2020 2020 2020  me = ""..       
-000002b0: 2073 656c 662e 7661 6c75 655f 7479 7065   self.value_type
-000002c0: 203d 204e 6f6e 6520 2023 2054 6865 7265   = None  # There
-000002d0: 2061 7265 2033 2074 7970 6573 206f 6620   are 3 types of 
-000002e0: 7661 6c75 6573 3a20 7374 722c 2069 6e74  values: str, int
-000002f0: 2c20 616e 6420 666c 6f61 740d 0a0d 0a20  , and float.... 
-00000300: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
-00000310: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00000320: 2073 656c 662e 636f 6d70 5f74 7970 6520   self.comp_type 
-00000330: 3d20 4e6f 6e65 2020 2023 2054 6865 7265  = None   # There
-00000340: 2061 7265 2035 2074 7970 6573 206f 6620   are 5 types of 
-00000350: 636f 6d70 6f6e 656e 7473 3a20 436f 6d70  components: Comp
-00000360: 6f6e 656e 742c 2043 6f6d 6d61 6e64 732c  onent, Commands,
-00000370: 2049 6e64 6578 436f 6d6d 616e 6473 2c20   IndexCommands, 
-00000380: 6d65 7468 6f64 2061 6e64 2049 6e64 6578  method and Index
-00000390: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-000003a0: 6574 5f65 6e61 626c 6520 3d20 4661 6c73  et_enable = Fals
-000003b0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-000003c0: 6765 745f 656e 6162 6c65 203d 2046 616c  get_enable = Fal
-000003d0: 7365 0d0a 2020 2020 2020 2020 7365 6c66  se..        self
-000003e0: 2e69 735f 6d65 7468 6f64 203d 2046 616c  .is_method = Fal
-000003f0: 7365 0d0a 2020 2020 2020 2020 7365 6c66  se..        self
-00000400: 2e65 7863 6c75 6465 6420 3d20 4661 6c73  .excluded = Fals
-00000410: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
-00000420: 7261 775f 7265 6d6f 7465 5f63 6f6d 6d61  raw_remote_comma
-00000430: 6e64 203d 2022 220d 0a20 2020 2020 2020  nd = ""..       
-00000440: 2073 656c 662e 7469 6d65 7374 616d 7020   self.timestamp 
-00000450: 3d20 302e 300d 0a20 2020 2020 2020 2073  = 0.0..        s
-00000460: 656c 662e 7175 6572 795f 7570 6461 7465  elf.query_update
-00000470: 5f70 6572 696f 6420 3d20 302e 330d 0a0d  _period = 0.3...
-00000480: 0a20 2020 2064 6566 2061 7070 656e 6443  .    def appendC
-00000490: 6869 6c64 2873 656c 662c 2069 7465 6d3a  hild(self, item:
-000004a0: 2022 436f 6d6d 616e 6449 7465 6d22 293a   "CommandItem"):
-000004b0: 0d0a 2020 2020 2020 2020 2222 2241 6464  ..        """Add
-000004c0: 2069 7465 6d20 6173 2061 2063 6869 6c64   item as a child
-000004d0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-000004e0: 662e 5f63 6869 6c64 7265 6e2e 6170 7065  f._children.appe
-000004f0: 6e64 2869 7465 6d29 0d0a 0d0a 2020 2020  nd(item)....    
-00000500: 6465 6620 6368 696c 6428 7365 6c66 2c20  def child(self, 
-00000510: 726f 773a 2069 6e74 2920 2d3e 2022 436f  row: int) -> "Co
-00000520: 6d6d 616e 6449 7465 6d22 3a0d 0a20 2020  mmandItem":..   
-00000530: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00000540: 6865 2063 6869 6c64 206f 6620 7468 6520  he child of the 
-00000550: 6375 7272 656e 7420 6974 656d 2066 726f  current item fro
-00000560: 6d20 7468 6520 6769 7665 6e20 726f 7722  m the given row"
-00000570: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00000580: 726e 2073 656c 662e 5f63 6869 6c64 7265  rn self._childre
-00000590: 6e5b 726f 775d 0d0a 0d0a 2020 2020 6465  n[row]....    de
-000005a0: 6620 7061 7265 6e74 2873 656c 6629 202d  f parent(self) -
-000005b0: 3e20 2243 6f6d 6d61 6e64 4974 656d 223a  > "CommandItem":
-000005c0: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
-000005d0: 7572 6e20 7468 6520 7061 7265 6e74 206f  urn the parent o
-000005e0: 6620 7468 6520 6375 7272 656e 7420 6974  f the current it
-000005f0: 656d 2222 220d 0a20 2020 2020 2020 2072  em"""..        r
-00000600: 6574 7572 6e20 7365 6c66 2e5f 7061 7265  eturn self._pare
-00000610: 6e74 0d0a 0d0a 2020 2020 6465 6620 6368  nt....    def ch
-00000620: 696c 6443 6f75 6e74 2873 656c 6629 202d  ildCount(self) -
-00000630: 3e20 696e 743a 0d0a 2020 2020 2020 2020  > int:..        
-00000640: 2222 2252 6574 7572 6e20 7468 6520 6e75  """Return the nu
-00000650: 6d62 6572 206f 6620 6368 696c 6472 656e  mber of children
-00000660: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
-00000670: 6974 656d 2222 220d 0a20 2020 2020 2020  item"""..       
-00000680: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
-00000690: 2e5f 6368 696c 6472 656e 290d 0a0d 0a20  ._children).... 
-000006a0: 2020 2064 6566 2072 6f77 2873 656c 6629     def row(self)
-000006b0: 202d 3e20 696e 743a 0d0a 2020 2020 2020   -> int:..      
-000006c0: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
-000006d0: 726f 7720 7768 6572 6520 7468 6520 6375  row where the cu
-000006e0: 7272 656e 7420 6974 656d 206f 6363 7570  rrent item occup
-000006f0: 6965 7320 696e 2074 6865 2070 6172 656e  ies in the paren
-00000700: 7422 2222 0d0a 2020 2020 2020 2020 7265  t"""..        re
-00000710: 7475 726e 2073 656c 662e 5f70 6172 656e  turn self._paren
-00000720: 742e 5f63 6869 6c64 7265 6e2e 696e 6465  t._children.inde
-00000730: 7828 7365 6c66 2920 6966 2073 656c 662e  x(self) if self.
-00000740: 5f70 6172 656e 7420 656c 7365 2030 0d0a  _parent else 0..
-00000750: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-00000760: 0a20 2020 2064 6566 2076 616c 7565 2873  .    def value(s
-00000770: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00000780: 2222 5265 7475 726e 2074 6865 2076 616c  ""Return the val
-00000790: 7565 206f 6620 7468 6520 6375 7272 656e  ue of the curren
-000007a0: 7420 6974 656d 2222 220d 0a20 2020 2020  t item"""..     
-000007b0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000007c0: 7661 6c75 650d 0a0d 0a20 2020 2040 7661  value....    @va
-000007d0: 6c75 652e 7365 7474 6572 0d0a 2020 2020  lue.setter..    
-000007e0: 6465 6620 7661 6c75 6528 7365 6c66 2c20  def value(self, 
-000007f0: 7661 6c75 6529 3a0d 0a20 2020 2020 2020  value):..       
-00000800: 2073 656c 662e 5f76 616c 7565 203d 2076   self._value = v
-00000810: 616c 7565 0d0a 0d0a 2020 2020 6465 6620  alue....    def 
-00000820: 7175 6572 795f 7661 6c75 6528 7365 6c66  query_value(self
-00000830: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
-00000840: 0d0a 2020 2020 2020 2020 2020 2020 7473  ..            ts
-00000850: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
-00000860: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00000870: 7320 2d20 7365 6c66 2e74 696d 6573 7461  s - self.timesta
-00000880: 6d70 203c 2073 656c 662e 7175 6572 795f  mp < self.query_
-00000890: 7570 6461 7465 5f70 6572 696f 643a 2020  update_period:  
-000008a0: 2320 446f 6e27 7420 7570 6461 7465 2074  # Don't update t
-000008b0: 6f6f 206f 6674 656e 0d0a 2020 2020 2020  oo often..      
-000008c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000008d0: 2073 656c 662e 5f76 616c 7565 0d0a 0d0a   self._value....
-000008e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000008f0: 656c 662e 636f 6d70 5f74 7970 6520 3d3d  elf.comp_type ==
-00000900: 2049 6e64 6578 2061 6e64 2073 656c 662e   Index and self.
-00000910: 6765 745f 656e 6162 6c65 2061 6e64 206e  get_enable and n
-00000920: 6f74 2073 656c 662e 6578 636c 7564 6564  ot self.excluded
-00000930: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000940: 2020 2073 656c 662e 5f76 616c 7565 203d     self._value =
-00000950: 2073 656c 662e 5f70 6172 656e 742e 636f   self._parent.co
-00000960: 6d70 2e5f 5f67 6574 6974 656d 5f5f 2873  mp.__getitem__(s
-00000970: 656c 662e 636f 6d70 290d 0a20 2020 2020  elf.comp)..     
-00000980: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000990: 7661 6c75 655f 7479 7065 203d 2074 7970  value_type = typ
-000009a0: 6528 7365 6c66 2e5f 7661 6c75 6529 0d0a  e(self._value)..
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 7365 6c66 2e74 696d 6573 7461 6d70 203d  self.timestamp =
-000009d0: 2074 730d 0a20 2020 2020 2020 2020 2020   ts..           
-000009e0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
-000009f0: 2874 7970 6528 7365 6c66 2e63 6f6d 7029  (type(self.comp)
-00000a00: 2c20 436f 6d6d 616e 6429 2061 6e64 2073  , Command) and s
-00000a10: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
-00000a20: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
-00000a30: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
-00000a40: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-00000a50: 7565 203d 2073 656c 662e 636f 6d70 2e5f  ue = self.comp._
-00000a60: 5f67 6574 5f5f 2873 656c 662e 5f70 6172  _get__(self._par
-00000a70: 656e 742e 636f 6d70 2c20 7365 6c66 2e5f  ent.comp, self._
-00000a80: 7061 7265 6e74 2e63 6f6d 702e 5f5f 636c  parent.comp.__cl
-00000a90: 6173 735f 5f29 0d0a 2020 2020 2020 2020  ass__)..        
-00000aa0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00000ab0: 7565 5f74 7970 6520 3d20 7479 7065 2873  ue_type = type(s
-00000ac0: 656c 662e 5f76 616c 7565 290d 0a20 2020  elf._value)..   
-00000ad0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000ae0: 662e 7469 6d65 7374 616d 7020 3d20 7473  f.timestamp = ts
-00000af0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00000b00: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00000b10: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00000b20: 696e 7428 2751 7565 7279 2065 7272 6f72  int('Query error
-00000b30: 3a20 7b7d 207b 7d27 2e66 6f72 6d61 7428  : {} {}'.format(
-00000b40: 652c 2073 656c 662e 6e61 6d65 2929 0d0a  e, self.name))..
-00000b50: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
-00000b60: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000b70: 7475 726e 2073 656c 662e 5f76 616c 7565  turn self._value
-00000b80: 0d0a 0d0a 2020 2020 6465 6620 7365 745f  ....    def set_
-00000b90: 7661 6c75 6528 7365 6c66 2c20 7661 6c75  value(self, valu
-00000ba0: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00000bb0: 5365 7420 7661 6c75 6520 746f 2074 6865  Set value to the
-00000bc0: 2069 6e73 7472 756d 656e 7420 616e 6420   instrument and 
-00000bd0: 7570 6461 7465 2074 6865 2076 616c 7565  update the value
-00000be0: 206f 6620 7468 6520 6974 656d 2222 220d   of the item""".
-00000bf0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00000c00: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00000c10: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
-00000c20: 496e 6465 783a 0d0a 2020 2020 2020 2020  Index:..        
-00000c30: 2020 2020 2020 2020 7365 6c66 2e5f 7061          self._pa
-00000c40: 7265 6e74 2e63 6f6d 702e 5f5f 7365 7469  rent.comp.__seti
-00000c50: 7465 6d5f 5f28 7365 6c66 2e63 6f6d 702c  tem__(self.comp,
-00000c60: 2076 616c 7565 290d 0a20 2020 2020 2020   value)..       
-00000c70: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
-00000c80: 616c 7565 203d 2073 656c 662e 5f70 6172  alue = self._par
-00000c90: 656e 742e 636f 6d70 2e5f 5f67 6574 6974  ent.comp.__getit
-00000ca0: 656d 5f5f 2873 656c 662e 636f 6d70 290d  em__(self.comp).
-00000cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cc0: 2073 656c 662e 7469 6d65 7374 616d 7020   self.timestamp 
-00000cd0: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
-00000ce0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00000cf0: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
-00000d00: 7365 6c66 2e63 6f6d 7029 2c20 436f 6d6d  self.comp), Comm
-00000d10: 616e 6429 3a0d 0a20 2020 2020 2020 2020  and):..         
-00000d20: 2020 2020 2020 2073 656c 662e 636f 6d70         self.comp
-00000d30: 2e5f 5f73 6574 5f5f 2873 656c 662e 5f70  .__set__(self._p
-00000d40: 6172 656e 742e 636f 6d70 2c20 7661 6c75  arent.comp, valu
-00000d50: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00000d60: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
-00000d70: 3d20 7365 6c66 2e63 6f6d 702e 5f5f 6765  = self.comp.__ge
-00000d80: 745f 5f28 7365 6c66 2e5f 7061 7265 6e74  t__(self._parent
-00000d90: 2e63 6f6d 702c 2073 656c 662e 5f70 6172  .comp, self._par
-00000da0: 656e 742e 636f 6d70 2e5f 5f63 6c61 7373  ent.comp.__class
-00000db0: 5f5f 290d 0a20 2020 2020 2020 2020 2020  __)..           
-00000dc0: 2020 2020 2073 656c 662e 7469 6d65 7374       self.timest
-00000dd0: 616d 7020 3d20 7469 6d65 2e74 696d 6528  amp = time.time(
-00000de0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000df0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000e00: 2020 2020 2020 7365 6c66 2e5f 7661 6c75        self._valu
-00000e10: 6520 3d20 7661 6c75 650d 0a20 2020 2020  e = value..     
-00000e20: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00000e30: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00000e40: 2020 2020 2020 2070 7269 6e74 2827 5365         print('Se
-00000e50: 7420 6572 726f 723a 207b 7d20 7b7d 272e  t error: {} {}'.
-00000e60: 666f 726d 6174 2865 2c20 7365 6c66 2e6e  format(e, self.n
-00000e70: 616d 6529 290d 0a0d 0a20 2020 2064 6566  ame))....    def
-00000e80: 2069 735f 6564 6974 6162 6c65 2873 656c   is_editable(sel
-00000e90: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
-00000ea0: 5265 7475 726e 2054 7275 6520 6966 2074  Return True if t
-00000eb0: 6865 2069 7465 6d20 6973 2065 6469 7461  he item is edita
-00000ec0: 626c 6522 2222 0d0a 2020 2020 2020 2020  ble"""..        
-00000ed0: 6966 2073 656c 662e 636f 6d70 5f74 7970  if self.comp_typ
-00000ee0: 6520 3d3d 2049 6e64 6578 2061 6e64 205c  e == Index and \
-00000ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000f00: 2020 7365 6c66 2e73 6574 5f65 6e61 626c    self.set_enabl
-00000f10: 6520 616e 6420 7365 6c66 2e67 6574 5f65  e and self.get_e
-00000f20: 6e61 626c 6520 616e 6420 6e6f 7420 7365  nable and not se
-00000f30: 6c66 2e65 7863 6c75 6465 643a 0d0a 2020  lf.excluded:..  
-00000f40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000f50: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
-00000f60: 6c69 6620 6973 7375 6263 6c61 7373 2874  lif issubclass(t
-00000f70: 7970 6528 7365 6c66 2e63 6f6d 7029 2c20  ype(self.comp), 
-00000f80: 436f 6d6d 616e 6429 2061 6e64 205c 0d0a  Command) and \..
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 7365 6c66 2e73 6574 5f65 6e61 626c 6520  self.set_enable 
-00000fb0: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
-00000fc0: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
-00000fd0: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
-00000fe0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00000ff0: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
-00001000: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001010: 7265 7475 726e 2046 616c 7365 0d0a 0d0a  return False....
-00001020: 2020 2020 6465 6620 6765 745f 666f 726d      def get_form
-00001030: 6174 7465 645f 7661 6c75 6528 7365 6c66  atted_value(self
-00001040: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
-00001050: 6574 7572 6e20 666f 726d 6174 7465 6420  eturn formatted 
-00001060: 7661 6c75 6520 6f66 2061 2066 6c6f 6174  value of a float
-00001070: 2222 220d 0a0d 0a20 2020 2020 2020 2076  """....        v
-00001080: 616c 7565 203d 2073 656c 662e 7661 6c75  alue = self.valu
-00001090: 650d 0a20 2020 2020 2020 2069 6620 7661  e..        if va
-000010a0: 6c75 6520 6973 204e 6f6e 653a 0d0a 2020  lue is None:..  
-000010b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000010c0: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
-000010d0: 2063 6f6d 7020 3d20 4e6f 6e65 0d0a 2020   comp = None..  
-000010e0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-000010f0: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
-00001100: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
-00001110: 6f6d 7020 3d20 7365 6c66 2e70 6172 656e  omp = self.paren
-00001120: 7428 292e 636f 6d70 0d0a 2020 2020 2020  t().comp..      
-00001130: 2020 656c 6966 2069 7373 7562 636c 6173    elif issubclas
-00001140: 7328 7479 7065 2873 656c 662e 636f 6d70  s(type(self.comp
-00001150: 292c 2043 6f6d 6d61 6e64 2920 6f72 205c  ), Command) or \
-00001160: 0d0a 2020 2020 2020 2020 2020 2020 2069  ..             i
-00001170: 7373 7562 636c 6173 7328 7479 7065 2873  ssubclass(type(s
-00001180: 656c 662e 636f 6d70 292c 2049 6e64 6578  elf.comp), Index
-00001190: 436f 6d6d 616e 6429 3a0d 0a20 2020 2020  Command):..     
-000011a0: 2020 2020 2020 2063 6f6d 7020 3d20 7365         comp = se
-000011b0: 6c66 2e63 6f6d 700d 0a0d 0a20 2020 2020  lf.comp....     
-000011c0: 2020 2066 6d74 203d 2063 6f6d 702e 666d     fmt = comp.fm
-000011d0: 7420 6966 2063 6f6d 7020 616e 6420 6861  t if comp and ha
-000011e0: 7361 7474 7228 636f 6d70 2c20 2766 6d74  sattr(comp, 'fmt
-000011f0: 2729 2065 6c73 6520 2727 0d0a 2020 2020  ') else ''..    
-00001200: 2020 2020 756e 6974 203d 2063 6f6d 702e      unit = comp.
-00001210: 756e 6974 2069 6620 636f 6d70 2061 6e64  unit if comp and
-00001220: 2068 6173 6174 7472 2863 6f6d 702c 2027   hasattr(comp, '
-00001230: 756e 6974 2729 2065 6c73 6520 2727 0d0a  unit') else ''..
-00001240: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
-00001250: 7020 616e 6420 2869 7373 7562 636c 6173  p and (issubclas
-00001260: 7328 7479 7065 2863 6f6d 7029 2c20 466c  s(type(comp), Fl
-00001270: 6f61 7449 6e64 6578 436f 6d6d 616e 6429  oatIndexCommand)
-00001280: 206f 720d 0a20 2020 2020 2020 2020 2020   or..           
-00001290: 2020 2020 2020 2020 2020 6973 7375 6263            issubc
-000012a0: 6c61 7373 2874 7970 6528 636f 6d70 292c  lass(type(comp),
-000012b0: 2046 6c6f 6174 436f 6d6d 616e 6429 293a   FloatCommand)):
-000012c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000012d0: 2076 616c 7565 203d 3d20 302e 303a 0d0a   value == 0.0:..
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 7265 7475 726e 2027 3027 202b 2066 2720  return '0' + f' 
-00001300: 7b75 6e69 747d 270d 0a20 2020 2020 2020  {unit}'..       
-00001310: 2020 2020 2073 7465 7020 3d20 636f 6d70       step = comp
-00001320: 2e73 7465 700d 0a20 2020 2020 2020 2020  .step..         
-00001330: 2020 2073 6967 6e69 6669 6361 6e74 5f66     significant_f
-00001340: 6967 7572 6573 203d 2063 6f6d 702e 7369  igures = comp.si
-00001350: 676e 6966 6963 616e 745f 6669 6775 7265  gnificant_figure
-00001360: 730d 0a0d 0a20 2020 2020 2020 2020 2020  s....           
-00001370: 2064 6563 696d 616c 7320 3d20 6d61 7468   decimals = math
-00001380: 2e63 6569 6c28 2d6d 6174 682e 6c6f 6731  .ceil(-math.log1
-00001390: 3028 7374 6570 2929 0d0a 2020 2020 2020  0(step))..      
-000013a0: 2020 2020 2020 6469 6769 7473 203d 206d        digits = m
-000013b0: 6174 682e 6365 696c 286d 6174 682e 6c6f  ath.ceil(math.lo
-000013c0: 6731 3028 6162 7328 7661 6c75 6529 2929  g10(abs(value)))
-000013d0: 2069 6620 7661 6c75 6520 656c 7365 2030   if value else 0
-000013e0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-000013f0: 6563 6973 696f 6e20 3d20 6d69 6e28 6465  ecision = min(de
-00001400: 6369 6d61 6c73 2c20 7369 676e 6966 6963  cimals, signific
-00001410: 616e 745f 6669 6775 7265 7320 2d20 6469  ant_figures - di
-00001420: 6769 7473 290d 0a20 2020 2020 2020 2020  gits)..         
-00001430: 2020 2070 7265 6369 7369 6f6e 203d 206d     precision = m
-00001440: 6178 2870 7265 6369 7369 6f6e 2c20 3029  ax(precision, 0)
-00001450: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001460: 2061 6273 2876 616c 7565 2920 3e3d 2030   abs(value) >= 0
-00001470: 2e31 206f 7220 7072 6563 6973 696f 6e20  .1 or precision 
-00001480: 3c20 7369 676e 6966 6963 616e 745f 6669  < significant_fi
-00001490: 6775 7265 733a 0d0a 2020 2020 2020 2020  gures:..        
-000014a0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-000014b0: 2074 7261 696c 696e 6720 7a65 726f 7320   trailing zeros 
-000014c0: 616e 6420 7265 7475 726e 0d0a 2020 2020  and return..    
-000014d0: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
-000014e0: 6627 7b76 616c 7565 3a2e 7b70 7265 6369  f'{value:.{preci
-000014f0: 7369 6f6e 7d66 7d27 0d0a 2020 2020 2020  sion}f}'..      
-00001500: 2020 2020 2020 2020 2020 6966 2027 2e27            if '.'
-00001510: 2069 6e20 733a 0d0a 2020 2020 2020 2020   in s:..        
-00001520: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001530: 726e 2073 2e72 7374 7269 7028 2730 2729  rn s.rstrip('0')
-00001540: 2e72 7374 7269 7028 272e 2729 202b 2066  .rstrip('.') + f
-00001550: 2720 7b75 6e69 747d 270d 0a20 2020 2020  ' {unit}'..     
-00001560: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00001570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001580: 2020 2020 2020 7265 7475 726e 2073 202b        return s +
-00001590: 2066 2720 7b75 6e69 747d 270d 0a20 2020   f' {unit}'..   
-000015a0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 7620 3d20 6627 7b76 616c 7565 3a2e 7b73  v = f'{value:.{s
-000015d0: 6967 6e69 6669 6361 6e74 5f66 6967 7572  ignificant_figur
-000015e0: 6573 7d65 7d27 0d0a 2020 2020 2020 2020  es}e}'..        
-000015f0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
-00001600: 2074 7261 696c 696e 6720 7a65 726f 7320   trailing zeros 
-00001610: 6265 666f 7265 2027 6527 2061 6e64 2072  before 'e' and r
-00001620: 6574 7572 6e0d 0a20 2020 2020 2020 2020  eturn..         
-00001630: 2020 2020 2020 2074 203d 2076 2e73 706c         t = v.spl
-00001640: 6974 2827 6527 290d 0a20 2020 2020 2020  it('e')..       
-00001650: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001660: 6627 7b74 5b30 5d2e 7273 7472 6970 2822  f'{t[0].rstrip("
-00001670: 3022 292e 7273 7472 6970 2822 2e22 297d  0").rstrip(".")}
-00001680: 657b 745b 315d 7d27 202b 2066 2720 207b  e{t[1]}' + f'  {
-00001690: 756e 6974 7d27 0d0a 2020 2020 2020 2020  unit}'..        
-000016a0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000016b0: 2020 2072 6574 7572 6e20 6627 7b76 616c     return f'{val
-000016c0: 7565 3a7b 666d 747d 7d27 202b 2066 2720  ue:{fmt}}' + f' 
-000016d0: 7b75 6e69 747d 270d 0a0d 0a20 2020 2064  {unit}'....    d
-000016e0: 6566 2063 6f6e 7374 7275 6374 5f73 6574  ef construct_set
-000016f0: 5f63 6f6d 6d61 6e64 5f73 7472 696e 6728  _command_string(
-00001700: 7365 6c66 2c20 7661 6c75 6529 3a0d 0a20  self, value):.. 
-00001710: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001720: 2020 2020 436f 6e73 7472 7563 7420 7079      Construct py
-00001730: 7468 6f6e 2063 6f6d 6d61 6e64 2073 7472  thon command str
-00001740: 696e 6720 636f 7272 6573 706f 6e64 696e  ing correspondin
-00001750: 6720 746f 2074 6865 2069 7465 6d0d 0a20  g to the item.. 
-00001760: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001770: 2020 2020 7365 6c66 2e6e 616d 655f 6275      self.name_bu
-00001780: 6666 6572 203d 205b 5d0d 0a20 2020 2020  ffer = []..     
-00001790: 2020 2073 656c 662e 6765 745f 6e61 6d65     self.get_name
-000017a0: 5f73 7472 696e 6728 7365 6c66 290d 0a20  _string(self).. 
-000017b0: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
-000017c0: 5f62 7566 6665 722e 7265 7665 7273 6528  _buffer.reverse(
-000017d0: 290d 0a20 2020 2020 2020 2069 6620 7479  )..        if ty
-000017e0: 7065 2876 616c 7565 2920 6973 2073 7472  pe(value) is str
-000017f0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00001800: 203d 2027 7b7d 203d 2022 7b7d 2227 2e66   = '{} = "{}"'.f
-00001810: 6f72 6d61 7428 272e 272e 6a6f 696e 2873  ormat('.'.join(s
-00001820: 656c 662e 6e61 6d65 5f62 7566 6665 7229  elf.name_buffer)
-00001830: 2c20 7661 6c75 6529 0d0a 2020 2020 2020  , value)..      
-00001840: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00001850: 2020 2020 2073 203d 2027 7b7d 203d 207b       s = '{} = {
-00001860: 7d27 2e66 6f72 6d61 7428 272e 272e 6a6f  }'.format('.'.jo
-00001870: 696e 2873 656c 662e 6e61 6d65 5f62 7566  in(self.name_buf
-00001880: 6665 7229 2c20 7661 6c75 6529 0d0a 0d0a  fer), value)....
-00001890: 2020 2020 2020 2020 7320 3d20 732e 7265          s = s.re
-000018a0: 706c 6163 6528 272e 5b27 2c20 275b 2729  place('.[', '[')
-000018b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000018c0: 2073 0d0a 0d0a 2020 2020 6465 6620 6765   s....    def ge
-000018d0: 745f 6e61 6d65 5f73 7472 696e 6728 7365  t_name_string(se
-000018e0: 6c66 2c20 6974 656d 293a 0d0a 2020 2020  lf, item):..    
-000018f0: 2020 2020 6966 2069 7465 6d2e 636f 6d70      if item.comp
-00001900: 5f74 7970 6520 3d3d 2049 6e64 6578 3a0d  _type == Index:.
-00001910: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001920: 7479 7065 2869 7465 6d2e 636f 6d70 2920  type(item.comp) 
-00001930: 6973 2073 7472 3a0d 0a20 2020 2020 2020  is str:..       
-00001940: 2020 2020 2020 2020 2073 656c 662e 6e61           self.na
-00001950: 6d65 5f62 7566 6665 722e 6170 7065 6e64  me_buffer.append
-00001960: 2827 5b22 7b7d 225d 272e 666f 726d 6174  ('["{}"]'.format
-00001970: 2869 7465 6d2e 6e61 6d65 2929 0d0a 2020  (item.name))..  
-00001980: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
-00001990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019a0: 2073 656c 662e 6e61 6d65 5f62 7566 6665   self.name_buffe
-000019b0: 722e 6170 7065 6e64 2827 5b7b 7d5d 272e  r.append('[{}]'.
-000019c0: 666f 726d 6174 2869 7465 6d2e 6e61 6d65  format(item.name
-000019d0: 2929 0d0a 2020 2020 2020 2020 656c 7365  ))..        else
-000019e0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000019f0: 656c 662e 6e61 6d65 5f62 7566 6665 722e  elf.name_buffer.
-00001a00: 6170 7065 6e64 2869 7465 6d2e 6e61 6d65  append(item.name
-00001a10: 290d 0a20 2020 2020 2020 2069 6620 6974  )..        if it
-00001a20: 656d 2e70 6172 656e 7428 293a 0d0a 2020  em.parent():..  
-00001a30: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-00001a40: 6574 5f6e 616d 655f 7374 7269 6e67 2869  et_name_string(i
-00001a50: 7465 6d2e 7061 7265 6e74 2829 290d 0a0d  tem.parent())...
-00001a60: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00001a70: 640d 0a20 2020 2064 6566 206c 6f61 6428  d..    def load(
-00001a80: 0d0a 2020 2020 2020 2020 636c 732c 2063  ..        cls, c
-00001a90: 6f6d 702c 2070 6172 656e 743a 2022 436f  omp, parent: "Co
-00001aa0: 6d6d 616e 6449 7465 6d22 203d 204e 6f6e  mmandItem" = Non
-00001ab0: 6529 202d 3e20 2243 6f6d 6d61 6e64 4974  e) -> "CommandIt
-00001ac0: 656d 223a 0d0a 2020 2020 2020 2020 2222  em":..        ""
-00001ad0: 2243 7265 6174 6520 6120 2772 6f6f 7427  "Create a 'root'
-00001ae0: 2043 6f6d 6d61 6e64 4974 656d 2066 726f   CommandItem fro
-00001af0: 6d20 6120 436f 6d70 6f6e 656e 7420 616e  m a Component an
-00001b00: 6420 0d0a 2020 2020 2020 2020 706f 7075  d ..        popu
-00001b10: 6c61 7465 2069 7473 2073 7562 636f 6d70  late its subcomp
-00001b20: 6f6e 656e 7420 616e 6420 636f 6d6d 616e  onent and comman
-00001b30: 6473 2072 6563 7572 7369 7665 6c79 2e0d  ds recursively..
-00001b40: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001b50: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00001b60: 2043 6f6d 6d61 6e64 4974 656d 3a20 436f   CommandItem: Co
-00001b70: 6d6d 616e 6449 7465 6d0d 0a20 2020 2020  mmandItem..     
-00001b80: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00001b90: 726f 6f74 5f69 7465 6d20 3d20 436f 6d6d  root_item = Comm
-00001ba0: 616e 6449 7465 6d28 7061 7265 6e74 290d  andItem(parent).
-00001bb0: 0a20 2020 2020 2020 2072 6f6f 745f 6974  .        root_it
-00001bc0: 656d 2e6e 616d 6520 3d20 2272 6f6f 7422  em.name = "root"
-00001bd0: 0d0a 2020 2020 2020 2020 726f 6f74 5f69  ..        root_i
-00001be0: 7465 6d2e 636f 6d70 203d 2063 6f6d 700d  tem.comp = comp.
-00001bf0: 0a0d 0a20 2020 2020 2020 2069 6620 6973  ...        if is
-00001c00: 7375 6263 6c61 7373 2863 6f6d 702e 5f5f  subclass(comp.__
-00001c10: 636c 6173 735f 5f2c 2043 6f6d 706f 6e65  class__, Compone
-00001c20: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
-00001c30: 2020 726f 6f74 5f69 7465 6d2e 6e61 6d65    root_item.name
-00001c40: 203d 2063 6f6d 702e 6765 745f 6e61 6d65   = comp.get_name
-00001c50: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00001c60: 666f 7220 6a20 696e 2063 6f6d 702e 5f5f  for j in comp.__
-00001c70: 6469 6374 5f5f 3a0d 0a20 2020 2020 2020  dict__:..       
-00001c80: 2020 2020 2020 2020 2069 6620 6a20 3d3d           if j ==
-00001c90: 2027 5f70 6172 656e 7427 3a0d 0a20 2020   '_parent':..   
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-00001cc0: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
-00001cd0: 6e63 6520 3d20 636f 6d70 2e5f 5f64 6963  nce = comp.__dic
-00001ce0: 745f 5f5b 6a5d 0d0a 2020 2020 2020 2020  t__[j]..        
-00001cf0: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
-00001d00: 636c 6173 7328 696e 7374 616e 6365 2e5f  class(instance._
-00001d10: 5f63 6c61 7373 5f5f 2c20 2043 6f6d 706f  _class__,  Compo
-00001d20: 6e65 6e74 293a 2020 2020 2020 2020 2020  nent):          
-00001d30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00001d40: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00001d50: 6420 3d20 636c 732e 6c6f 6164 2869 6e73  d = cls.load(ins
-00001d60: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
-00001d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001d80: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
-00001d90: 6520 3d20 6a0d 0a20 2020 2020 2020 2020  e = j..         
-00001da0: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00001db0: 2e63 6f6d 7020 3d20 696e 7374 616e 6365  .comp = instance
-00001dc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001dd0: 2020 2020 2020 6966 2069 6e73 7461 6e63        if instanc
-00001de0: 6520 696e 2063 6f6d 702e 6578 636c 7564  e in comp.exclud
-00001df0: 655f 6361 7074 7572 653a 0d0a 2020 2020  e_capture:..    
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 6368 696c 642e 6578 636c 7564      child.exclud
-00001e20: 6564 203d 2054 7275 650d 0a20 2020 2020  ed = True..     
-00001e30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001e40: 6869 6c64 2e63 6f6d 705f 7479 7065 203d  hild.comp_type =
-00001e50: 2074 7970 6528 696e 7374 616e 6365 290d   type(instance).
-00001e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e70: 2020 2020 2072 6f6f 745f 6974 656d 2e61       root_item.a
-00001e80: 7070 656e 6443 6869 6c64 2863 6869 6c64  ppendChild(child
-00001e90: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00001ea0: 2063 7572 7265 6e74 5f61 7474 7269 6275   current_attribu
-00001eb0: 7465 7320 3d20 5b5d 0d0a 2020 2020 2020  tes = []..      
-00001ec0: 2020 2020 2020 666f 7220 6320 696e 2063        for c in c
-00001ed0: 6f6d 702e 5f5f 636c 6173 735f 5f2e 5f5f  omp.__class__.__
-00001ee0: 6d72 6f5f 5f3a 2020 2320 6c6f 6f70 2074  mro__:  # loop t
-00001ef0: 6872 6f75 6768 2074 6865 2063 6c61 7373  hrough the class
-00001f00: 6573 2069 6e63 6c75 6469 6e67 2073 7570  es including sup
-00001f10: 6572 2063 6c61 7373 6573 0d0a 2020 2020  er classes..    
-00001f20: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00001f30: 6f74 2069 7373 7562 636c 6173 7328 632c  ot issubclass(c,
-00001f40: 2043 6f6d 706f 6e65 6e74 293a 2020 2320   Component):  # 
-00001f50: 6974 2073 686f 756c 6420 6265 2061 2073  it should be a s
-00001f60: 7562 636c 6173 7320 6f66 2043 6f6d 706f  ubclass of Compo
-00001f70: 6e65 6e74 0d0a 2020 2020 2020 2020 2020  nent..          
-00001f80: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
-00001f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001fa0: 2069 6620 6320 3d3d 2043 6f6d 706f 6e65   if c == Compone
-00001fb0: 6e74 3a20 2023 2042 7574 2069 7420 7368  nt:  # But it sh
-00001fc0: 6f75 6c64 206e 6f74 2062 6520 436f 6d70  ould not be Comp
-00001fd0: 6f6e 656e 740d 0a20 2020 2020 2020 2020  onent..         
-00001fe0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00001ff0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002000: 2020 2020 666f 7220 6b65 7920 696e 2063      for key in c
-00002010: 2e5f 5f64 6963 745f 5f3a 0d0a 2020 2020  .__dict__:..    
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 636d 645f 696e 7374 616e 6365 203d 2063  cmd_instance = c
-00002040: 2e5f 5f64 6963 745f 5f5b 6b65 795d 0d0a  .__dict__[key]..
-00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002060: 2020 2020 6966 206b 6579 2069 6e20 6375      if key in cu
-00002070: 7272 656e 745f 6174 7472 6962 7574 6573  rrent_attributes
-00002080: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002090: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-000020a0: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
-000020b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000020c0: 5f61 7474 7269 6275 7465 732e 6170 7065  _attributes.appe
-000020d0: 6e64 286b 6579 290d 0a0d 0a20 2020 2020  nd(key)....     
-000020e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000020f0: 6620 6973 7375 6263 6c61 7373 2863 6d64  f issubclass(cmd
-00002100: 5f69 6e73 7461 6e63 652e 5f5f 636c 6173  _instance.__clas
-00002110: 735f 5f2c 2043 6f6d 6d61 6e64 293a 0d0a  s__, Command):..
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
-00002140: 636c 732e 6c6f 6164 2863 6d64 5f69 6e73  cls.load(cmd_ins
-00002150: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
-00002160: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002170: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002180: 2e6e 616d 6520 3d20 6b65 790d 0a20 2020  .name = key..   
-00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021a0: 2020 2020 2063 6869 6c64 2e63 6f6d 7020       child.comp 
-000021b0: 3d20 636d 645f 696e 7374 616e 6365 0d0a  = cmd_instance..
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021d0: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-000021e0: 6d70 5f74 7970 6520 3d20 7479 7065 2863  mp_type = type(c
-000021f0: 6d64 5f69 6e73 7461 6e63 6529 0d0a 0d0a  md_instance)....
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00002220: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
-00002230: 696c 6429 0d0a 0d0a 2020 2020 2020 2020  ild)....        
-00002240: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00002250: 2069 7373 7562 636c 6173 7328 636d 645f   issubclass(cmd_
-00002260: 696e 7374 616e 6365 2e5f 5f63 6c61 7373  instance.__class
-00002270: 5f5f 2c20 496e 6465 7843 6f6d 6d61 6e64  __, IndexCommand
-00002280: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00002290: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-000022a0: 6420 3d20 636c 732e 6c6f 6164 2863 6d64  d = cls.load(cmd
-000022b0: 5f69 6e73 7461 6e63 652c 2072 6f6f 745f  _instance, root_
-000022c0: 6974 656d 290d 0a20 2020 2020 2020 2020  item)..         
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000022e0: 6869 6c64 2e6e 616d 6520 3d20 6b65 790d  hild.name = key.
-000022f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002300: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
-00002310: 6f6d 7020 3d20 636d 645f 696e 7374 616e  omp = cmd_instan
-00002320: 6365 0d0a 2020 2020 2020 2020 2020 2020  ce..            
-00002330: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002340: 642e 636f 6d70 5f74 7970 6520 3d20 7479  d.comp_type = ty
-00002350: 7065 2863 6d64 5f69 6e73 7461 6e63 6529  pe(cmd_instance)
-00002360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002370: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
-00002380: 7465 6d2e 6170 7065 6e64 4368 696c 6428  tem.appendChild(
-00002390: 6368 696c 6429 0d0a 0d0a 2020 2020 2020  child)....      
-000023a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000023b0: 6966 2063 616c 6c61 626c 6528 636d 645f  if callable(cmd_
-000023c0: 696e 7374 616e 6365 293a 0d0a 2020 2020  instance):..    
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2020 2020 6966 2069 7373 7562 636c 6173      if issubclas
-000023f0: 7328 636d 645f 696e 7374 616e 6365 2e5f  s(cmd_instance._
-00002400: 5f63 6c61 7373 5f5f 2c20 7479 7065 293a  _class__, type):
-00002410: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002420: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002430: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 6966 206b 6579 2e73 7461 7274 7377 6974  if key.startswit
-00002460: 6828 275f 2729 3a0d 0a20 2020 2020 2020  h('_'):..       
-00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2063 6869 6c64 203d 2063 6c73 2e6c 6f61   child = cls.loa
-000024d0: 6428 636d 645f 696e 7374 616e 6365 2c20  d(cmd_instance, 
-000024e0: 726f 6f74 5f69 7465 6d29 0d0a 2020 2020  root_item)..    
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 2020 2020 6368 696c 642e 6e61 6d65 203d      child.name =
-00002510: 206b 6579 0d0a 2020 2020 2020 2020 2020   key..          
-00002520: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002530: 696c 642e 636f 6d70 203d 2063 6d64 5f69  ild.comp = cmd_i
-00002540: 6e73 7461 6e63 650d 0a20 2020 2020 2020  nstance..       
+00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a66  ..import time..f
+00000010: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
+00000020: 7420 436f 6d70 6f6e 656e 740d 0a66 726f  t Component..fro
+00000030: 6d20 7372 7367 7569 2e69 6e73 7420 696d  m srsgui.inst im
+00000040: 706f 7274 2043 6f6d 6d61 6e64 2c20 496e  port Command, In
+00000050: 6465 7843 6f6d 6d61 6e64 2c20 5c0d 0a20  dexCommand, \.. 
+00000060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000070: 2020 2020 2020 2046 6c6f 6174 436f 6d6d         FloatComm
+00000080: 616e 642c 2046 6c6f 6174 496e 6465 7843  and, FloatIndexC
+00000090: 6f6d 6d61 6e64 0d0a 0d0a 0d0a 636c 6173  ommand......clas
+000000a0: 7320 496e 6465 783a 0d0a 2020 2020 7061  s Index:..    pa
+000000b0: 7373 0d0a 0d0a 0d0a 636c 6173 7320 436f  ss......class Co
+000000c0: 6d6d 616e 6449 7465 6d3a 0d0a 2020 2020  mmandItem:..    
+000000d0: 2222 2241 2043 6f6d 6d61 6e64 2069 7465  """A Command ite
+000000e0: 6d20 636f 7272 6573 706f 6e64 696e 6720  m corresponding 
+000000f0: 746f 2061 206c 696e 6520 696e 2051 5472  to a line in QTr
+00000100: 6565 5669 6577 2222 220d 0a0d 0a20 2020  eeView"""....   
+00000110: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000120: 6c66 2c20 7061 7265 6e74 3a20 2243 6f6d  lf, parent: "Com
+00000130: 6d61 6e64 4974 656d 2220 3d20 4e6f 6e65  mandItem" = None
+00000140: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00000150: 2e5f 7061 7265 6e74 203d 2070 6172 656e  ._parent = paren
+00000160: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+00000170: 5f63 6869 6c64 7265 6e20 3d20 5b5d 0d0a  _children = []..
+00000180: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00000190: 6c75 6520 3d20 4e6f 6e65 0d0a 2020 2020  lue = None..    
+000001a0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
+000001b0: 6c66 2e6e 616d 6520 3d20 2222 0d0a 2020  lf.name = ""..  
+000001c0: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
+000001d0: 5f74 7970 6520 3d20 4e6f 6e65 2020 2320  _type = None  # 
+000001e0: 5468 6572 6520 6172 6520 3320 7479 7065  There are 3 type
+000001f0: 7320 6f66 2076 616c 7565 733a 2073 7472  s of values: str
+00000200: 2c20 696e 742c 2061 6e64 2066 6c6f 6174  , int, and float
+00000210: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000220: 7265 6369 7369 6f6e 203d 2034 0d0a 2020  recision = 4..  
+00000230: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000240: 7365 6c66 2e63 6f6d 7020 3d20 4e6f 6e65  self.comp = None
+00000250: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00000260: 6f6d 705f 7479 7065 203d 204e 6f6e 6520  omp_type = None 
+00000270: 2020 2320 5468 6572 6520 6172 6520 3520    # There are 5 
+00000280: 7479 7065 7320 6f66 2063 6f6d 706f 6e65  types of compone
+00000290: 6e74 733a 2043 6f6d 706f 6e65 6e74 2c20  nts: Component, 
+000002a0: 436f 6d6d 616e 6473 2c20 496e 6465 7843  Commands, IndexC
+000002b0: 6f6d 6d61 6e64 732c 206d 6574 686f 6420  ommands, method 
+000002c0: 616e 6420 496e 6465 780d 0a20 2020 2020  and Index..     
+000002d0: 2020 2073 656c 662e 7365 745f 656e 6162     self.set_enab
+000002e0: 6c65 203d 2046 616c 7365 0d0a 2020 2020  le = False..    
+000002f0: 2020 2020 7365 6c66 2e67 6574 5f65 6e61      self.get_ena
+00000300: 626c 6520 3d20 4661 6c73 650d 0a20 2020  ble = False..   
+00000310: 2020 2020 2073 656c 662e 6973 5f6d 6574       self.is_met
+00000320: 686f 6420 3d20 4661 6c73 650d 0a20 2020  hod = False..   
+00000330: 2020 2020 2073 656c 662e 6578 636c 7564       self.exclud
+00000340: 6564 203d 2046 616c 7365 0d0a 2020 2020  ed = False..    
+00000350: 2020 2020 7365 6c66 2e72 6177 5f72 656d      self.raw_rem
+00000360: 6f74 655f 636f 6d6d 616e 6420 3d20 2222  ote_command = ""
+00000370: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000380: 696d 6573 7461 6d70 203d 2030 2e30 0d0a  imestamp = 0.0..
+00000390: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+000003a0: 4368 696c 6428 7365 6c66 2c20 6974 656d  Child(self, item
+000003b0: 3a20 2243 6f6d 6d61 6e64 4974 656d 2229  : "CommandItem")
+000003c0: 3a0d 0a20 2020 2020 2020 2022 2222 4164  :..        """Ad
+000003d0: 6420 6974 656d 2061 7320 6120 6368 696c  d item as a chil
+000003e0: 6422 2222 0d0a 2020 2020 2020 2020 7365  d"""..        se
+000003f0: 6c66 2e5f 6368 696c 6472 656e 2e61 7070  lf._children.app
+00000400: 656e 6428 6974 656d 290d 0a0d 0a20 2020  end(item)....   
+00000410: 2064 6566 2063 6869 6c64 2873 656c 662c   def child(self,
+00000420: 2072 6f77 3a20 696e 7429 202d 3e20 2243   row: int) -> "C
+00000430: 6f6d 6d61 6e64 4974 656d 223a 0d0a 2020  ommandItem":..  
+00000440: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00000450: 7468 6520 6368 696c 6420 6f66 2074 6865  the child of the
+00000460: 2063 7572 7265 6e74 2069 7465 6d20 6672   current item fr
+00000470: 6f6d 2074 6865 2067 6976 656e 2072 6f77  om the given row
+00000480: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00000490: 7572 6e20 7365 6c66 2e5f 6368 696c 6472  urn self._childr
+000004a0: 656e 5b72 6f77 5d0d 0a0d 0a20 2020 2064  en[row]....    d
+000004b0: 6566 2070 6172 656e 7428 7365 6c66 2920  ef parent(self) 
+000004c0: 2d3e 2022 436f 6d6d 616e 6449 7465 6d22  -> "CommandItem"
+000004d0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+000004e0: 7475 726e 2074 6865 2070 6172 656e 7420  turn the parent 
+000004f0: 6f66 2074 6865 2063 7572 7265 6e74 2069  of the current i
+00000500: 7465 6d22 2222 0d0a 2020 2020 2020 2020  tem"""..        
+00000510: 7265 7475 726e 2073 656c 662e 5f70 6172  return self._par
+00000520: 656e 740d 0a0d 0a20 2020 2064 6566 2063  ent....    def c
+00000530: 6869 6c64 436f 756e 7428 7365 6c66 2920  hildCount(self) 
+00000540: 2d3e 2069 6e74 3a0d 0a20 2020 2020 2020  -> int:..       
+00000550: 2022 2222 5265 7475 726e 2074 6865 206e   """Return the n
+00000560: 756d 6265 7220 6f66 2063 6869 6c64 7265  umber of childre
+00000570: 6e20 6f66 2074 6865 2063 7572 7265 6e74  n of the current
+00000580: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
+00000590: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
+000005a0: 662e 5f63 6869 6c64 7265 6e29 0d0a 0d0a  f._children)....
+000005b0: 2020 2020 6465 6620 726f 7728 7365 6c66      def row(self
+000005c0: 2920 2d3e 2069 6e74 3a0d 0a20 2020 2020  ) -> int:..     
+000005d0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
+000005e0: 2072 6f77 2077 6865 7265 2074 6865 2063   row where the c
+000005f0: 7572 7265 6e74 2069 7465 6d20 6f63 6375  urrent item occu
+00000600: 7069 6573 2069 6e20 7468 6520 7061 7265  pies in the pare
+00000610: 6e74 2222 220d 0a20 2020 2020 2020 2072  nt"""..        r
+00000620: 6574 7572 6e20 7365 6c66 2e5f 7061 7265  eturn self._pare
+00000630: 6e74 2e5f 6368 696c 6472 656e 2e69 6e64  nt._children.ind
+00000640: 6578 2873 656c 6629 2069 6620 7365 6c66  ex(self) if self
+00000650: 2e5f 7061 7265 6e74 2065 6c73 6520 300d  ._parent else 0.
+00000660: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00000670: 0d0a 2020 2020 6465 6620 7661 6c75 6528  ..    def value(
+00000680: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000690: 2222 2252 6574 7572 6e20 7468 6520 7661  """Return the va
+000006a0: 6c75 6520 6f66 2074 6865 2063 7572 7265  lue of the curre
+000006b0: 6e74 2069 7465 6d22 2222 0d0a 2020 2020  nt item"""..    
+000006c0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+000006d0: 2020 2020 2020 7473 203d 2074 696d 652e        ts = time.
+000006e0: 7469 6d65 2829 0d0a 2020 2020 2020 2020  time()..        
+000006f0: 2020 2020 6966 2074 7320 2d20 7365 6c66      if ts - self
+00000700: 2e74 696d 6573 7461 6d70 203c 2030 2e31  .timestamp < 0.1
+00000710: 3a20 2320 5570 6461 7465 2076 616c 7565  : # Update value
+00000720: 206c 6174 6572 2074 6861 6e20 302e 3120   later than 0.1 
+00000730: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00000740: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00000750: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
+00000760: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
+00000770: 705f 7479 7065 203d 3d20 496e 6465 7820  p_type == Index 
+00000780: 616e 6420 7365 6c66 2e67 6574 5f65 6e61  and self.get_ena
+00000790: 626c 6520 616e 6420 6e6f 7420 7365 6c66  ble and not self
+000007a0: 2e65 7863 6c75 6465 643a 0d0a 2020 2020  .excluded:..    
+000007b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000007c0: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+000007d0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+000007e0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+000007f0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000800: 2020 2020 7365 6c66 2e5f 7661 6c75 655f      self._value_
+00000810: 7479 7065 203d 2074 7970 6528 7365 6c66  type = type(self
+00000820: 2e5f 7661 6c75 6529 0d0a 2020 2020 2020  ._value)..      
+00000830: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00000840: 696d 6573 7461 6d70 203d 2074 730d 0a20  imestamp = ts.. 
+00000850: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00000860: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
+00000870: 7365 6c66 2e63 6f6d 7029 2c20 436f 6d6d  self.comp), Comm
+00000880: 616e 6429 2061 6e64 2073 656c 662e 6765  and) and self.ge
+00000890: 745f 656e 6162 6c65 2061 6e64 206e 6f74  t_enable and not
+000008a0: 2073 656c 662e 6578 636c 7564 6564 3a0d   self.excluded:.
+000008b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008c0: 2073 656c 662e 5f76 616c 7565 203d 2073   self._value = s
+000008d0: 656c 662e 636f 6d70 2e5f 5f67 6574 5f5f  elf.comp.__get__
+000008e0: 2873 656c 662e 5f70 6172 656e 742e 636f  (self._parent.co
+000008f0: 6d70 2c20 7365 6c66 2e5f 7061 7265 6e74  mp, self._parent
+00000900: 2e63 6f6d 702e 5f5f 636c 6173 735f 5f29  .comp.__class__)
+00000910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000920: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
+00000930: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
+00000940: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+00000950: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+00000960: 6573 7461 6d70 203d 2074 730d 0a20 2020  estamp = ts..   
+00000970: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 7365 6c66 2e5f 7661 6c75 655f 7479 7065  self._value_type
+000009a0: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
+000009b0: 6c75 6529 0d0a 0d0a 2020 2020 2020 2020  lue)....        
+000009c0: 2020 2020 2320 526f 756e 6420 666c 6f61      # Round floa
+000009d0: 7420 746f 2069 7473 2070 7265 6369 7369  t to its precisi
+000009e0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000009f0: 6966 2073 656c 662e 636f 6d70 5f74 7970  if self.comp_typ
+00000a00: 6520 3d3d 2046 6c6f 6174 436f 6d6d 616e  e == FloatComman
+00000a10: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00000a20: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
+00000a30: 3d20 726f 756e 6428 7365 6c66 2e5f 7661  = round(self._va
+00000a40: 6c75 652c 2073 656c 662e 7072 6563 6973  lue, self.precis
+00000a50: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00000a60: 2020 656c 6966 2073 656c 662e 636f 6d70    elif self.comp
+00000a70: 5f74 7970 6520 3d3d 2049 6e64 6578 2061  _type == Index a
+00000a80: 6e64 2073 656c 662e 5f70 6172 656e 742e  nd self._parent.
+00000a90: 636f 6d70 5f74 7970 6520 3d3d 2046 6c6f  comp_type == Flo
+00000aa0: 6174 496e 6465 7843 6f6d 6d61 6e64 3a0d  atIndexCommand:.
+00000ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ac0: 2073 656c 662e 5f76 616c 7565 203d 2072   self._value = r
+00000ad0: 6f75 6e64 2873 656c 662e 5f76 616c 7565  ound(self._value
+00000ae0: 2c20 7365 6c66 2e70 7265 6369 7369 6f6e  , self.precision
+00000af0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00000b00: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00000b10: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00000b20: 7269 6e74 2865 2c20 7365 6c66 2e6e 616d  rint(e, self.nam
+00000b30: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
+00000b40: 726e 2073 656c 662e 5f76 616c 7565 0d0a  rn self._value..
+00000b50: 0d0a 2020 2020 4076 616c 7565 2e73 6574  ..    @value.set
+00000b60: 7465 720d 0a20 2020 2064 6566 2076 616c  ter..    def val
+00000b70: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000b80: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00000b90: 7661 6c75 6520 3d20 7661 6c75 650d 0a0d  value = value...
+00000ba0: 0a20 2020 2064 6566 2073 6574 5f76 616c  .    def set_val
+00000bb0: 7565 2873 656c 662c 2076 616c 7565 293a  ue(self, value):
+00000bc0: 0d0a 2020 2020 2020 2020 2222 2253 6574  ..        """Set
+00000bd0: 2076 616c 7565 2074 6f20 7468 6520 696e   value to the in
+00000be0: 7374 7275 6d65 6e74 2061 6e64 2075 7064  strument and upd
+00000bf0: 6174 6520 7468 6520 7661 6c75 6520 6f66  ate the value of
+00000c00: 2074 6865 2069 7465 6d22 2222 0d0a 2020   the item"""..  
+00000c10: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00000c20: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
+00000c30: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00000c40: 656c 662e 5f70 6172 656e 742e 636f 6d70  elf._parent.comp
+00000c50: 2e5f 5f73 6574 6974 656d 5f5f 2873 656c  .__setitem__(sel
+00000c60: 662e 636f 6d70 2c20 7661 6c75 6529 0d0a  f.comp, value)..
+00000c70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000c80: 2e5f 7661 6c75 6520 3d20 7365 6c66 2e5f  ._value = self._
+00000c90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 6765  parent.comp.__ge
+00000ca0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+00000cb0: 7029 0d0a 2020 2020 2020 2020 2020 2020  p)..            
+00000cc0: 7365 6c66 2e74 696d 6573 7461 6d70 203d  self.timestamp =
+00000cd0: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
+00000ce0: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
+00000cf0: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
+00000d00: 636f 6d70 292c 2043 6f6d 6d61 6e64 293a  comp), Command):
+00000d10: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000d20: 6c66 2e63 6f6d 702e 5f5f 7365 745f 5f28  lf.comp.__set__(
+00000d30: 7365 6c66 2e5f 7061 7265 6e74 2e63 6f6d  self._parent.com
+00000d40: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
+00000d50: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+00000d60: 7565 203d 2073 656c 662e 636f 6d70 2e5f  ue = self.comp._
+00000d70: 5f67 6574 5f5f 2873 656c 662e 5f70 6172  _get__(self._par
+00000d80: 656e 742e 636f 6d70 2c20 7365 6c66 2e5f  ent.comp, self._
+00000d90: 7061 7265 6e74 2e63 6f6d 702e 5f5f 636c  parent.comp.__cl
+00000da0: 6173 735f 5f29 0d0a 2020 2020 2020 2020  ass__)..        
+00000db0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
+00000dc0: 6d70 203d 2074 696d 652e 7469 6d65 2829  mp = time.time()
+00000dd0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00000de0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000df0: 662e 5f76 616c 7565 203d 2076 616c 7565  f._value = value
+00000e00: 0d0a 0d0a 2020 2020 6465 6620 6973 5f65  ....    def is_e
+00000e10: 6469 7461 626c 6528 7365 6c66 293a 0d0a  ditable(self):..
+00000e20: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00000e30: 6e20 5472 7565 2069 6620 7468 6520 6974  n True if the it
+00000e40: 656d 2069 7320 6564 6974 6162 6c65 2222  em is editable""
+00000e50: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00000e60: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
+00000e70: 496e 6465 7820 616e 6420 5c0d 0a20 2020  Index and \..   
+00000e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000e90: 662e 7365 745f 656e 6162 6c65 2061 6e64  f.set_enable and
+00000ea0: 2073 656c 662e 6765 745f 656e 6162 6c65   self.get_enable
+00000eb0: 2061 6e64 206e 6f74 2073 656c 662e 6578   and not self.ex
+00000ec0: 636c 7564 6564 3a0d 0a20 2020 2020 2020  cluded:..       
+00000ed0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00000ee0: 0d0a 2020 2020 2020 2020 656c 6966 2069  ..        elif i
+00000ef0: 7373 7562 636c 6173 7328 7479 7065 2873  ssubclass(type(s
+00000f00: 656c 662e 636f 6d70 292c 2043 6f6d 6d61  elf.comp), Comma
+00000f10: 6e64 2920 616e 6420 5c0d 0a20 2020 2020  nd) and \..     
+00000f20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000f30: 7365 745f 656e 6162 6c65 2061 6e64 2073  set_enable and s
+00000f40: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
+00000f50: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
+00000f60: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
+00000f70: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
+00000f80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00000f90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000fa0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
+00000fb0: 6566 2067 6574 5f75 6e69 7428 7365 6c66  ef get_unit(self
+00000fc0: 293a 0d0a 2020 2020 2020 2020 2222 2252  ):..        """R
+00000fd0: 6574 7572 6e20 7468 6520 756e 6974 206f  eturn the unit o
+00000fe0: 6620 7468 6520 6974 656d 2222 220d 0a20  f the item""".. 
+00000ff0: 2020 2020 2020 2063 6f6d 7020 3d20 4e6f         comp = No
+00001000: 6e65 0d0a 2020 2020 2020 2020 6966 2073  ne..        if s
+00001010: 656c 662e 636f 6d70 5f74 7970 6520 3d3d  elf.comp_type ==
+00001020: 2049 6e64 6578 3a0d 0a20 2020 2020 2020   Index:..       
+00001030: 2020 2020 2063 6f6d 7020 3d20 7365 6c66       comp = self
+00001040: 2e70 6172 656e 7428 292e 636f 6d70 0d0a  .parent().comp..
+00001050: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001060: 7562 636c 6173 7328 7479 7065 2873 656c  ubclass(type(sel
+00001070: 662e 636f 6d70 292c 2043 6f6d 6d61 6e64  f.comp), Command
+00001080: 2920 6f72 205c 0d0a 2020 2020 2020 2020  ) or \..        
+00001090: 2020 2020 2069 7373 7562 636c 6173 7328       issubclass(
+000010a0: 7479 7065 2873 656c 662e 636f 6d70 292c  type(self.comp),
+000010b0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
+000010c0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+000010d0: 7020 3d20 7365 6c66 2e63 6f6d 700d 0a0d  p = self.comp...
+000010e0: 0a20 2020 2020 2020 2069 6620 636f 6d70  .        if comp
+000010f0: 2061 6e64 2068 6173 6174 7472 2863 6f6d   and hasattr(com
+00001100: 702c 2027 756e 6974 2729 3a0d 0a20 2020  p, 'unit'):..   
+00001110: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001120: 636f 6d70 2e75 6e69 740d 0a20 2020 2020  comp.unit..     
+00001130: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001140: 2020 2020 2020 7265 7475 726e 2022 220d        return "".
+00001150: 0a0d 0a20 2020 2064 6566 2067 6574 5f66  ...    def get_f
+00001160: 6f72 6d61 7428 7365 6c66 293a 0d0a 2020  ormat(self):..  
+00001170: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
+00001180: 7468 6520 666f 726d 6174 206f 6620 7468  the format of th
+00001190: 6520 6974 656d 2222 220d 0a20 2020 2020  e item"""..     
+000011a0: 2020 2063 6f6d 7020 3d20 4e6f 6e65 0d0a     comp = None..
+000011b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000011c0: 636f 6d70 5f74 7970 6520 3d3d 2049 6e64  comp_type == Ind
+000011d0: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
+000011e0: 2063 6f6d 7020 3d20 7365 6c66 2e70 6172   comp = self.par
+000011f0: 656e 7428 292e 636f 6d70 0d0a 2020 2020  ent().comp..    
+00001200: 2020 2020 656c 6966 2069 7373 7562 636c      elif issubcl
+00001210: 6173 7328 7479 7065 2873 656c 662e 636f  ass(type(self.co
+00001220: 6d70 292c 2043 6f6d 6d61 6e64 2920 6f72  mp), Command) or
+00001230: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
+00001240: 2069 7373 7562 636c 6173 7328 7479 7065   issubclass(type
+00001250: 2873 656c 662e 636f 6d70 292c 2049 6e64  (self.comp), Ind
+00001260: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+00001270: 2020 2020 2020 2020 2063 6f6d 7020 3d20           comp = 
+00001280: 7365 6c66 2e63 6f6d 700d 0a0d 0a20 2020  self.comp....   
+00001290: 2020 2020 2069 6620 636f 6d70 2061 6e64       if comp and
+000012a0: 2068 6173 6174 7472 2863 6f6d 702c 2027   hasattr(comp, '
+000012b0: 666d 7427 293a 0d0a 2020 2020 2020 2020  fmt'):..        
+000012c0: 2020 2020 7265 7475 726e 2063 6f6d 702e      return comp.
+000012d0: 666d 740d 0a20 2020 2020 2020 2065 6c73  fmt..        els
+000012e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000012f0: 7265 7475 726e 2027 270d 0a0d 0a20 2020  return ''....   
+00001300: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
+00001310: 2020 2064 6566 206c 6f61 6428 0d0a 2020     def load(..  
+00001320: 2020 2020 2020 636c 732c 2063 6f6d 702c        cls, comp,
+00001330: 2070 6172 656e 743a 2022 436f 6d6d 616e   parent: "Comman
+00001340: 6449 7465 6d22 203d 204e 6f6e 652c 2073  dItem" = None, s
+00001350: 6f72 743d 4661 6c73 650d 0a20 2020 2029  ort=False..    )
+00001360: 202d 3e20 2243 6f6d 6d61 6e64 4974 656d   -> "CommandItem
+00001370: 223a 0d0a 2020 2020 2020 2020 2222 2243  ":..        """C
+00001380: 7265 6174 6520 6120 2772 6f6f 7427 2043  reate a 'root' C
+00001390: 6f6d 6d61 6e64 4974 656d 2066 726f 6d20  ommandItem from 
+000013a0: 6120 436f 6d70 6f6e 656e 7420 616e 6420  a Component and 
+000013b0: 0d0a 2020 2020 2020 2020 706f 7075 6c61  ..        popula
+000013c0: 7465 2069 7473 2073 7562 636f 6d70 6f6e  te its subcompon
+000013d0: 656e 7420 616e 6420 636f 6d6d 616e 6473  ent and commands
+000013e0: 2072 6563 7572 7369 7665 6c79 2e0d 0a0d   recursively....
+000013f0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001400: 3a0d 0a20 2020 2020 2020 2020 2020 2043  :..            C
+00001410: 6f6d 6d61 6e64 4974 656d 3a20 436f 6d6d  ommandItem: Comm
+00001420: 616e 6449 7465 6d0d 0a20 2020 2020 2020  andItem..       
+00001430: 2022 2222 0d0a 2020 2020 2020 2020 726f   """..        ro
+00001440: 6f74 5f69 7465 6d20 3d20 436f 6d6d 616e  ot_item = Comman
+00001450: 6449 7465 6d28 7061 7265 6e74 290d 0a20  dItem(parent).. 
+00001460: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001470: 2e6e 616d 6520 3d20 2272 6f6f 7422 0d0a  .name = "root"..
+00001480: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001490: 6d2e 636f 6d70 203d 2063 6f6d 700d 0a0d  m.comp = comp...
+000014a0: 0a20 2020 2020 2020 2069 6620 6973 7375  .        if issu
+000014b0: 6263 6c61 7373 2863 6f6d 702e 5f5f 636c  bclass(comp.__cl
+000014c0: 6173 735f 5f2c 2043 6f6d 706f 6e65 6e74  ass__, Component
+000014d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000014e0: 666f 7220 6a20 696e 2063 6f6d 702e 5f5f  for j in comp.__
+000014f0: 6469 6374 5f5f 3a0d 0a20 2020 2020 2020  dict__:..       
+00001500: 2020 2020 2020 2020 2069 6620 6a20 3d3d           if j ==
+00001510: 2027 5f70 6172 656e 7427 3a0d 0a20 2020   '_parent':..   
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001540: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
+00001550: 6e63 6520 3d20 636f 6d70 2e5f 5f64 6963  nce = comp.__dic
+00001560: 745f 5f5b 6a5d 0d0a 2020 2020 2020 2020  t__[j]..        
+00001570: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
+00001580: 636c 6173 7328 696e 7374 616e 6365 2e5f  class(instance._
+00001590: 5f63 6c61 7373 5f5f 2c20 2043 6f6d 706f  _class__,  Compo
+000015a0: 6e65 6e74 293a 2020 2020 2020 2020 2020  nent):          
+000015b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000015c0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+000015d0: 6420 3d20 636c 732e 6c6f 6164 2869 6e73  d = cls.load(ins
+000015e0: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+000015f0: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001600: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00001610: 6c64 2e6e 616d 6520 3d20 6a0d 0a20 2020  ld.name = j..   
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2063 6869 6c64 2e63 6f6d 7020 3d20 696e   child.comp = in
+00001640: 7374 616e 6365 0d0a 2020 2020 2020 2020  stance..        
+00001650: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00001660: 6e73 7461 6e63 6520 696e 2063 6f6d 702e  nstance in comp.
+00001670: 6578 636c 7564 655f 6361 7074 7572 653a  exclude_capture:
+00001680: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001690: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000016a0: 6578 636c 7564 6564 203d 2054 7275 650d  excluded = True.
+000016b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016c0: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
+000016d0: 7479 7065 203d 2074 7970 6528 696e 7374  type = type(inst
+000016e0: 616e 6365 290d 0a20 2020 2020 2020 2020  ance)..         
+000016f0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001700: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
+00001710: 2863 6869 6c64 290d 0a0d 0a20 2020 2020  (child)....     
+00001720: 2020 2020 2020 2063 7572 7265 6e74 5f61         current_a
+00001730: 7474 7269 6275 7465 7320 3d20 5b5d 0d0a  ttributes = []..
+00001740: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00001750: 6320 696e 2063 6f6d 702e 5f5f 636c 6173  c in comp.__clas
+00001760: 735f 5f2e 5f5f 6d72 6f5f 5f3a 2020 2320  s__.__mro__:  # 
+00001770: 6c6f 6f70 2074 6872 6f75 6768 2074 6865  loop through the
+00001780: 2063 6c61 7373 6573 2069 6e63 6c75 6469   classes includi
+00001790: 6e67 2073 7570 6572 2063 6c61 7373 6573  ng super classes
+000017a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017b0: 2020 6966 206e 6f74 2069 7373 7562 636c    if not issubcl
+000017c0: 6173 7328 632c 2043 6f6d 706f 6e65 6e74  ass(c, Component
+000017d0: 293a 2020 2320 6974 2073 686f 756c 6420  ):  # it should 
+000017e0: 6265 2061 2073 7562 636c 6173 7320 6f66  be a subclass of
+000017f0: 2043 6f6d 706f 6e65 6e74 0d0a 2020 2020   Component..    
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
+00001820: 2020 2020 2020 2069 6620 6320 3d3d 2043         if c == C
+00001830: 6f6d 706f 6e65 6e74 3a20 2023 2042 7574  omponent:  # But
+00001840: 2069 7420 7368 6f75 6c64 206e 6f74 2062   it should not b
+00001850: 6520 436f 6d70 6f6e 656e 740d 0a20 2020  e Component..   
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2062 7265 616b 0d0a 0d0a 2020 2020 2020   break....      
+00001880: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
+00001890: 7920 696e 2063 2e5f 5f64 6963 745f 5f3a  y in c.__dict__:
+000018a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000018b0: 2020 2020 2020 636d 645f 696e 7374 616e        cmd_instan
+000018c0: 6365 203d 2063 2e5f 5f64 6963 745f 5f5b  ce = c.__dict__[
+000018d0: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+000018e0: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+000018f0: 2069 6e20 6375 7272 656e 745f 6174 7472   in current_attr
+00001900: 6962 7574 6573 3a0d 0a20 2020 2020 2020  ibutes:..       
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001930: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001940: 7572 7265 6e74 5f61 7474 7269 6275 7465  urrent_attribute
+00001950: 732e 6170 7065 6e64 286b 6579 290d 0a0d  s.append(key)...
+00001960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001970: 2020 2020 2069 6620 6973 7375 6263 6c61       if issubcla
+00001980: 7373 2863 6d64 5f69 6e73 7461 6e63 652e  ss(cmd_instance.
+00001990: 5f5f 636c 6173 735f 5f2c 2043 6f6d 6d61  __class__, Comma
+000019a0: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
+000019b0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000019c0: 696c 6420 3d20 636c 732e 6c6f 6164 2863  ild = cls.load(c
+000019d0: 6d64 5f69 6e73 7461 6e63 652c 2072 6f6f  md_instance, roo
+000019e0: 745f 6974 656d 2c20 736f 7274 290d 0a20  t_item, sort).. 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
+00001a10: 6520 3d20 6b65 790d 0a20 2020 2020 2020  e = key..       
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2063 6869 6c64 2e63 6f6d 7020 3d20 636d   child.comp = cm
+00001a40: 645f 696e 7374 616e 6365 0d0a 2020 2020  d_instance..    
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 6368 696c 642e 636f 6d70 5f74      child.comp_t
+00001a70: 7970 6520 3d20 7479 7065 2863 6d64 5f69  ype = type(cmd_i
+00001a80: 6e73 7461 6e63 6529 0d0a 0d0a 2020 2020  nstance)....    
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2020 726f 6f74 5f69 7465 6d2e 6170      root_item.ap
+00001ab0: 7065 6e64 4368 696c 6428 6368 696c 6429  pendChild(child)
+00001ac0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00001ad0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001ae0: 7562 636c 6173 7328 636d 645f 696e 7374  ubclass(cmd_inst
+00001af0: 616e 6365 2e5f 5f63 6c61 7373 5f5f 2c20  ance.__class__, 
+00001b00: 496e 6465 7843 6f6d 6d61 6e64 293a 0d0a  IndexCommand):..
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2020 2020 6368 696c 6420 3d20          child = 
+00001b30: 636c 732e 6c6f 6164 2863 6d64 5f69 6e73  cls.load(cmd_ins
+00001b40: 7461 6e63 652c 2072 6f6f 745f 6974 656d  tance, root_item
+00001b50: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2063 6869 6c64 2e6e 616d 6520 3d20 6b65   child.name = ke
+00001b80: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
+00001b90: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00001ba0: 2e63 6f6d 7020 3d20 636d 645f 696e 7374  .comp = cmd_inst
+00001bb0: 616e 6365 0d0a 2020 2020 2020 2020 2020  ance..          
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00001bd0: 696c 642e 636f 6d70 5f74 7970 6520 3d20  ild.comp_type = 
+00001be0: 7479 7065 2863 6d64 5f69 6e73 7461 6e63  type(cmd_instanc
+00001bf0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001c00: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00001c10: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
+00001c20: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 656c 6966 2063 616c 6c61 626c 6528 636d  elif callable(cm
+00001c50: 645f 696e 7374 616e 6365 293a 0d0a 2020  d_instance):..  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 6966 2069 7373 7562 636c        if issubcl
+00001c80: 6173 7328 636d 645f 696e 7374 616e 6365  ass(cmd_instance
+00001c90: 2e5f 5f63 6c61 7373 5f5f 2c20 7479 7065  .__class__, type
+00001ca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 6966 206b 6579 2e73 7461 7274 7377    if key.startsw
+00001cf0: 6974 6828 275f 2729 3a0d 0a20 2020 2020  ith('_'):..     
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00001d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d30: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2063 6869 6c64 203d 2063 6c73 2e6c     child = cls.l
+00001d60: 6f61 6428 636d 645f 696e 7374 616e 6365  oad(cmd_instance
+00001d70: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00001d80: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00001d90: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00001da0: 642e 6e61 6d65 203d 206b 6579 0d0a 2020  d.name = key..  
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
+00001dd0: 203d 2063 6d64 5f69 6e73 7461 6e63 650d   = cmd_instance.
+00001de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001df0: 2020 2020 2020 2020 2063 6869 6c64 2e63           child.c
+00001e00: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001e10: 636d 645f 696e 7374 616e 6365 290d 0a20  cmd_instance).. 
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001e40: 2e61 7070 656e 6443 6869 6c64 2863 6869  .appendChild(chi
+00001e50: 6c64 290d 0a20 2020 2020 2020 2065 6c73  ld)..        els
+00001e60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001e70: 6966 2063 616c 6c61 626c 6528 636f 6d70  if callable(comp
+00001e80: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001e90: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00001ea0: 6d70 203d 2063 6f6d 700d 0a20 2020 2020  mp = comp..     
+00001eb0: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001ec0: 6974 656d 2e63 6f6d 705f 7479 7065 203d  item.comp_type =
+00001ed0: 2074 7970 6528 636f 6d70 290d 0a20 2020   type(comp)..   
+00001ee0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00001ef0: 745f 6974 656d 2e69 735f 6d65 7468 6f64  t_item.is_method
+00001f00: 203d 2054 7275 650d 0a0d 0a20 2020 2020   = True....     
+00001f10: 2020 2020 2020 2065 6c69 6620 6973 7375         elif issu
+00001f20: 6263 6c61 7373 2874 7970 6528 636f 6d70  bclass(type(comp
+00001f30: 292c 2043 6f6d 6d61 6e64 293a 0d0a 2020  ), Command):..  
+00001f40: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001f50: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
+00001f60: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
+00001f70: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
+00001f80: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001f90: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
+00001fa0: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001fb0: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
+00001fc0: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
+00001fd0: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
+00001fe0: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
+00001ff0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00002000: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
+00002010: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
+00002020: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
+00002050: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
+00002060: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
+00002070: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+00002080: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
+00002090: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
+000020a0: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+000020b0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
+000020c0: 2874 7970 6528 636f 6d70 292c 2049 6e64  (type(comp), Ind
+000020d0: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
+000020e0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+000020f0: 745f 6974 656d 2e63 6f6d 7020 3d20 636f  t_item.comp = co
+00002100: 6d70 0d0a 2020 2020 2020 2020 2020 2020  mp..            
+00002110: 2020 2020 726f 6f74 5f69 7465 6d2e 636f      root_item.co
+00002120: 6d70 5f74 7970 6520 3d20 7479 7065 2863  mp_type = type(c
+00002130: 6f6d 7029 0d0a 2020 2020 2020 2020 2020  omp)..          
+00002140: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
+00002150: 6578 636c 7564 6564 203d 2063 6f6d 7020  excluded = comp 
+00002160: 696e 2072 6f6f 745f 6974 656d 2e70 6172  in root_item.par
+00002170: 656e 7428 292e 636f 6d70 2e65 7863 6c75  ent().comp.exclu
+00002180: 6465 5f63 6170 7475 7265 0d0a 2020 2020  de_capture..    
+00002190: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+000021a0: 5f69 7465 6d2e 7261 775f 7265 6d6f 7465  _item.raw_remote
+000021b0: 5f63 6f6d 6d61 6e64 203d 2063 6f6d 702e  _command = comp.
+000021c0: 7265 6d6f 7465 5f63 6f6d 6d61 6e64 0d0a  remote_command..
+000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021e0: 726f 6f74 5f69 7465 6d2e 7365 745f 656e  root_item.set_en
+000021f0: 6162 6c65 203d 2063 6f6d 702e 5f73 6574  able = comp._set
+00002200: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002210: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
+00002220: 656d 2e67 6574 5f65 6e61 626c 6520 3d20  em.get_enable = 
+00002230: 636f 6d70 2e5f 6765 745f 656e 6162 6c65  comp._get_enable
+00002240: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002250: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002270: 2063 6f6d 702e 696e 6465 785f 6469 6374   comp.index_dict
+00002280: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2069 6e64 6578 203d 2063 6f6d 702e     index = comp.
+000022b0: 696e 6465 785f 6d69 6e0d 0a20 2020 2020  index_min..     
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 2077 6869 6c65 2069 6e64 6578 203c     while index <
+000022e0: 3d20 636f 6d70 2e69 6e64 6578 5f6d 6178  = comp.index_max
+000022f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002300: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002310: 6869 6c64 203d 2063 6c73 2e6c 6f61 6428  hild = cls.load(
+00002320: 696e 6465 782c 2072 6f6f 745f 6974 656d  index, root_item
+00002330: 2c20 736f 7274 290d 0a20 2020 2020 2020  , sort)..       
+00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002350: 2020 2020 2063 6869 6c64 2e6e 616d 6520       child.name 
+00002360: 3d20 6627 7b69 6e64 6578 7d27 0d0a 2020  = f'{index}'..  
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+00002390: 636f 6d70 203d 2069 6e64 6578 0d0a 2020  comp = index..  
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+000023c0: 636f 6d70 5f74 7970 6520 3d20 496e 6465  comp_type = Inde
+000023d0: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000023f0: 6869 6c64 2e65 7863 6c75 6465 6420 3d20  hild.excluded = 
+00002400: 726f 6f74 5f69 7465 6d2e 6578 636c 7564  root_item.exclud
+00002410: 6564 0d0a 2020 2020 2020 2020 2020 2020  ed..            
+00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002430: 6368 696c 642e 7365 745f 656e 6162 6c65  child.set_enable
+00002440: 203d 2072 6f6f 745f 6974 656d 2e73 6574   = root_item.set
+00002450: 5f65 6e61 626c 650d 0a20 2020 2020 2020  _enable..       
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 2020 2020 2063 6869 6c64 2e67 6574 5f65       child.get_e
+00002480: 6e61 626c 6520 3d20 726f 6f74 5f69 7465  nable = root_ite
+00002490: 6d2e 6765 745f 656e 6162 6c65 0d0a 2020  m.get_enable..  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+000024c0: 7465 6d2e 6170 7065 6e64 4368 696c 6428  tem.appendChild(
+000024d0: 6368 696c 6429 0d0a 2020 2020 2020 2020  child)..        
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 2020 696e 6465 7820 2b3d 2031 0d0a      index += 1..
+00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002510: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 2066 6f72 206b 6579 2069 6e20 636f     for key in co
+00002540: 6d70 2e69 6e64 6578 5f64 6963 743a 0d0a  mp.index_dict:..
 00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
-00002570: 203d 2074 7970 6528 636d 645f 696e 7374   = type(cmd_inst
-00002580: 616e 6365 290d 0a20 2020 2020 2020 2020  ance)..         
-00002590: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000025a0: 6f6f 745f 6974 656d 2e61 7070 656e 6443  oot_item.appendC
-000025b0: 6869 6c64 2863 6869 6c64 290d 0a20 2020  hild(child)..   
-000025c0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000025d0: 2020 2020 2020 2020 6966 2063 616c 6c61          if calla
-000025e0: 626c 6528 636f 6d70 293a 0d0a 2020 2020  ble(comp):..    
-000025f0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00002600: 5f69 7465 6d2e 636f 6d70 203d 2063 6f6d  _item.comp = com
-00002610: 700d 0a20 2020 2020 2020 2020 2020 2020  p..             
-00002620: 2020 2072 6f6f 745f 6974 656d 2e63 6f6d     root_item.com
-00002630: 705f 7479 7065 203d 2074 7970 6528 636f  p_type = type(co
-00002640: 6d70 290d 0a20 2020 2020 2020 2020 2020  mp)..           
-00002650: 2020 2020 2072 6f6f 745f 6974 656d 2e69       root_item.i
-00002660: 735f 6d65 7468 6f64 203d 2054 7275 650d  s_method = True.
-00002670: 0a0d 0a20 2020 2020 2020 2020 2020 2065  ...            e
-00002680: 6c69 6620 6973 7375 6263 6c61 7373 2874  lif issubclass(t
-00002690: 7970 6528 636f 6d70 292c 2043 6f6d 6d61  ype(comp), Comma
-000026a0: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
-000026b0: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-000026c0: 636f 6d70 203d 2063 6f6d 700d 0a20 2020  comp = comp..   
-000026d0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-000026e0: 745f 6974 656d 2e63 6f6d 705f 7479 7065  t_item.comp_type
-000026f0: 203d 2074 7970 6528 636f 6d70 290d 0a20   = type(comp).. 
-00002700: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002710: 6f6f 745f 6974 656d 2e65 7863 6c75 6465  oot_item.exclude
-00002720: 6420 3d20 636f 6d70 2069 6e20 726f 6f74  d = comp in root
-00002730: 5f69 7465 6d2e 7061 7265 6e74 2829 2e63  _item.parent().c
-00002740: 6f6d 702e 6578 636c 7564 655f 6361 7074  omp.exclude_capt
-00002750: 7572 650d 0a20 2020 2020 2020 2020 2020  ure..           
-00002760: 2020 2020 2072 6f6f 745f 6974 656d 2e72       root_item.r
-00002770: 6177 5f72 656d 6f74 655f 636f 6d6d 616e  aw_remote_comman
-00002780: 6420 3d20 636f 6d70 2e72 656d 6f74 655f  d = comp.remote_
-00002790: 636f 6d6d 616e 640d 0a20 2020 2020 2020  command..       
-000027a0: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-000027b0: 656d 2e73 6574 5f65 6e61 626c 6520 3d20  em.set_enable = 
-000027c0: 636f 6d70 2e5f 7365 745f 656e 6162 6c65  comp._set_enable
-000027d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000027e0: 2020 726f 6f74 5f69 7465 6d2e 6765 745f    root_item.get_
-000027f0: 656e 6162 6c65 203d 2063 6f6d 702e 5f67  enable = comp._g
-00002800: 6574 5f65 6e61 626c 650d 0a0d 0a20 2020  et_enable....   
-00002810: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00002820: 7375 6263 6c61 7373 2874 7970 6528 636f  subclass(type(co
-00002830: 6d70 292c 2049 6e64 6578 436f 6d6d 616e  mp), IndexComman
-00002840: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
-00002850: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
-00002860: 6f6d 7020 3d20 636f 6d70 0d0a 2020 2020  omp = comp..    
-00002870: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00002880: 5f69 7465 6d2e 636f 6d70 5f74 7970 6520  _item.comp_type 
-00002890: 3d20 7479 7065 2863 6f6d 7029 0d0a 2020  = type(comp)..  
-000028a0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-000028b0: 6f74 5f69 7465 6d2e 6578 636c 7564 6564  ot_item.excluded
-000028c0: 203d 2063 6f6d 7020 696e 2072 6f6f 745f   = comp in root_
-000028d0: 6974 656d 2e70 6172 656e 7428 292e 636f  item.parent().co
-000028e0: 6d70 2e65 7863 6c75 6465 5f63 6170 7475  mp.exclude_captu
-000028f0: 7265 0d0a 2020 2020 2020 2020 2020 2020  re..            
-00002900: 2020 2020 726f 6f74 5f69 7465 6d2e 7261      root_item.ra
-00002910: 775f 7265 6d6f 7465 5f63 6f6d 6d61 6e64  w_remote_command
-00002920: 203d 2063 6f6d 702e 7265 6d6f 7465 5f63   = comp.remote_c
-00002930: 6f6d 6d61 6e64 0d0a 2020 2020 2020 2020  ommand..        
-00002940: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00002950: 6d2e 7365 745f 656e 6162 6c65 203d 2063  m.set_enable = c
-00002960: 6f6d 702e 5f73 6574 5f65 6e61 626c 650d  omp._set_enable.
-00002970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002980: 2072 6f6f 745f 6974 656d 2e67 6574 5f65   root_item.get_e
-00002990: 6e61 626c 6520 3d20 636f 6d70 2e5f 6765  nable = comp._ge
-000029a0: 745f 656e 6162 6c65 0d0a 0d0a 2020 2020  t_enable....    
-000029b0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000029c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000029d0: 2020 2020 2020 6966 2063 6f6d 702e 696e        if comp.in
-000029e0: 6465 785f 6469 6374 2069 7320 4e6f 6e65  dex_dict is None
-000029f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002a00: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00002a10: 203d 2063 6f6d 702e 696e 6465 785f 6d69   = comp.index_mi
-00002a20: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-00002a30: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00002a40: 2069 6e64 6578 203c 3d20 636f 6d70 2e69   index <= comp.i
-00002a50: 6e64 6578 5f6d 6178 3a0d 0a20 2020 2020  ndex_max:..     
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2063 6869 6c64 203d 2063         child = c
-00002a80: 6c73 2e6c 6f61 6428 696e 6465 782c 2072  ls.load(index, r
-00002a90: 6f6f 745f 6974 656d 290d 0a20 2020 2020  oot_item)..     
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
-00002ac0: 6520 3d20 6627 7b69 6e64 6578 7d27 0d0a  e = f'{index}'..
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002af0: 642e 636f 6d70 203d 2069 6e64 6578 0d0a  d.comp = index..
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002b20: 642e 636f 6d70 5f74 7970 6520 3d20 496e  d.comp_type = In
-00002b30: 6465 780d 0a20 2020 2020 2020 2020 2020  dex..           
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2063 6869 6c64 2e65 7863 6c75 6465 6420   child.excluded 
-00002b60: 3d20 726f 6f74 5f69 7465 6d2e 6578 636c  = root_item.excl
-00002b70: 7564 6564 0d0a 2020 2020 2020 2020 2020  uded..          
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 6368 696c 642e 7365 745f 656e 6162    child.set_enab
-00002ba0: 6c65 203d 2072 6f6f 745f 6974 656d 2e73  le = root_item.s
-00002bb0: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
-00002be0: 5f65 6e61 626c 6520 3d20 726f 6f74 5f69  _enable = root_i
-00002bf0: 7465 6d2e 6765 745f 656e 6162 6c65 0d0a  tem.get_enable..
-00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00002c20: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
-00002c30: 6428 6368 696c 6429 0d0a 2020 2020 2020  d(child)..      
-00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c50: 2020 2020 2020 696e 6465 7820 2b3d 2031        index += 1
-00002c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002c70: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c90: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
-00002ca0: 636f 6d70 2e69 6e64 6578 5f64 6963 743a  comp.index_dict:
-00002cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002cd0: 696c 6420 3d20 636c 732e 6c6f 6164 286b  ild = cls.load(k
-00002ce0: 6579 2c20 726f 6f74 5f69 7465 6d29 0d0a  ey, root_item)..
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002d10: 642e 6e61 6d65 203d 2066 277b 6b65 797d  d.name = f'{key}
-00002d20: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002d40: 6869 6c64 2e63 6f6d 7020 3d20 6b65 790d  hild.comp = key.
-00002d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d60: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00002d70: 6c64 2e63 6f6d 705f 7479 7065 203d 2049  ld.comp_type = I
-00002d80: 6e64 6578 0d0a 2020 2020 2020 2020 2020  ndex..          
-00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2020 6368 696c 642e 6578 6c75 6465 6420    child.exluded 
-00002db0: 3d20 726f 6f74 5f69 7465 6d2e 6578 636c  = root_item.excl
-00002dc0: 7564 6564 0d0a 2020 2020 2020 2020 2020  uded..          
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 6368 696c 642e 7365 745f 656e 6162    child.set_enab
-00002df0: 6c65 203d 2063 6f6d 702e 5f73 6574 5f65  le = comp._set_e
-00002e00: 6e61 626c 650d 0a20 2020 2020 2020 2020  nable..         
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e20: 2020 2063 6869 6c64 2e67 6574 5f65 6e61     child.get_ena
-00002e30: 626c 6520 3d20 636f 6d70 2e5f 6765 745f  ble = comp._get_
-00002e40: 656e 6162 6c65 0d0a 2020 2020 2020 2020  enable..        
-00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 2020 2020 726f 6f74 5f69 7465 6d2e 6170      root_item.ap
-00002e70: 7065 6e64 4368 696c 6428 6368 696c 6429  pendChild(child)
-00002e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e90: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-00002ea0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-00002eb0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002ec0: 696e 7428 6627 2020 7b74 7970 6528 6529  int(f'  {type(e)
-00002ed0: 7d20 7b65 7d20 636f 6d6d 616e 643a 7b63  } {e} command:{c
-00002ee0: 6f6d 702e 7265 6d6f 7465 5f63 6f6d 6d61  omp.remote_comma
-00002ef0: 6e64 7d27 290d 0a20 2020 2020 2020 2072  nd}')..        r
-00002f00: 6574 7572 6e20 726f 6f74 5f69 7465 6d0d  eturn root_item.
-00002f10: 0a                                       .
+00002560: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00002570: 6420 3d20 636c 732e 6c6f 6164 286b 6579  d = cls.load(key
+00002580: 2c20 726f 6f74 5f69 7465 6d2c 2073 6f72  , root_item, sor
+00002590: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 6368 696c 642e 6e61 6d65 203d 2066 277b  child.name = f'{
+000025c0: 6b65 797d 270d 0a20 2020 2020 2020 2020  key}'..         
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
+000025f0: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2063 6869 6c64 2e63 6f6d 705f 7479 7065   child.comp_type
+00002620: 203d 2049 6e64 6578 0d0a 2020 2020 2020   = Index..      
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 6368 696c 642e 6578 6c75        child.exlu
+00002650: 6465 6420 3d20 726f 6f74 5f69 7465 6d2e  ded = root_item.
+00002660: 6578 636c 7564 6564 0d0a 2020 2020 2020  excluded..      
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 2020 2020 2020 6368 696c 642e 7365 745f        child.set_
+00002690: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
+000026a0: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
+000026d0: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
+000026e0: 6765 745f 656e 6162 6c65 0d0a 2020 2020  get_enable..    
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002700: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00002710: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
+00002720: 696c 6429 0d0a 2020 2020 2020 2020 2020  ild)..          
+00002730: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00002740: 6570 7469 6f6e 2061 7320 653a 0d0a 2020  eption as e:..  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 7072 696e 7428 6627 2020 7b74 7970    print(f'  {typ
+00002770: 6528 6529 7d20 7b65 7d20 636f 6d6d 616e  e(e)} {e} comman
+00002780: 643a 7b63 6f6d 702e 7265 6d6f 7465 5f63  d:{comp.remote_c
+00002790: 6f6d 6d61 6e64 7d20 696e 6465 783a 207b  ommand} index: {
+000027a0: 696e 6465 787d 2729 0d0a 2020 2020 2020  index}')..      
+000027b0: 2020 7265 7475 726e 2072 6f6f 745f 6974    return root_it
+000027c0: 656d 0d0a                                em..
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,60 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
+import time
+import json
 import sys
-
 from typing import Any, Iterable, List, Dict, Union
 
 from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
 from srsgui.ui.qt.QtGui import QBrush, QColor
-from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, \
-                                QObject, Qt, Signal
+from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, QObject, Qt, QFileInfo
 
 from srsgui import Component
 
 from .commanditem import CommandItem, Index
 from .commanddelegate import CommandDelegate
-from .commandhandler import CommandHandler
 
 
 class CommandModel(QAbstractItemModel):
     """ An editable model of Command and Component """
 
-    # Signal to request to process a query to an outside command processor
-    query_requested = Signal(QModelIndex)
-
-    # Signal to request to process a set to an outside command processor
-    set_requested = Signal(tuple)
-
-    # Signal to display full Python command to CommandTerminal
-    set_command_sent = Signal(str, str)
-
     def __init__(self, parent: QObject = None):
         super().__init__(parent)
 
+        self.show_methods = True
+        self.show_excluded = True
+        self.show_set_only = True
+        self.show_query_only = True
         self.show_raw_remote_command = True
 
         self._rootItem = CommandItem()
-        self._headers = ("  Command  ", "  Value  ")
+        self._headers = ("  command  ", "  value  ")
 
     def clear(self):
         """ Clear data from the model """
         self.load(Component())
 
-    def load(self, document: Component):
+    def load(self, document: Component, sort=False):
         """Load model from a nested dictionary returned by json.loads()
 
         Arguments:
             document (dict): JSON-compatible dictionary
         """
 
         assert isinstance(
             document, Component
-        ), "`document` must be a Component, " f"not {type(document)}"
+        ), "`document` must be of dict, list or tuple, " f"not {type(document)}"
 
         self.beginResetModel()
 
-        self._rootItem = CommandItem.load(document)
+        self._rootItem = CommandItem.load(document, sort=sort)
         self._rootItem.value_type = type(document)
 
         self.endResetModel()
+
         return True
 
     def data(self, index: QModelIndex, role: Qt.ItemDataRole) -> Any:
         """Override from QAbstractItemModel
 
         Return data from an item according index and role
         """
@@ -74,72 +65,76 @@
         if role == Qt.DisplayRole:
             if index.column() == 0:
                 item = index.internalPointer()
                 name = item.name
 
                 if self.show_raw_remote_command:
                     name += f' <{item.raw_remote_command}>' if item.raw_remote_command else ''
-
-                name += ' [M]' if item.is_method else ''
-                name += ' [EX]' if item.excluded else ''
-                name += ' [SO]' if item.set_enable and not item.get_enable else ''
-                name += ' [QO]' if item.get_enable and not item.set_enable else ''
+                if self.show_methods:
+                    name += ' [M]' if item.is_method else ''
+                if self.show_excluded:
+                    name += ' [EX]' if item.excluded else ''
+                if self.show_set_only:
+                    name += ' [SO]' if item.set_enable and not item.get_enable else ''
+                if self.show_query_only:
+                    name += ' [QO]' if item.get_enable and not item.set_enable else ''
                 return name
 
             if index.column() == 1:
                 item = index.internalPointer()
-                self.query_requested.emit(index)
-                return item.get_formatted_value()
+                v = item.value
+                if v is None:
+                    return
+                unit = item.get_unit()
+                fmt = item.get_format()
+                try:
+                    if unit:
+                        val = f'{v:{fmt}}  {item.get_unit()}'
+                    else:
+                        val = f'{v:{fmt}}'
+                except ValueError:
+                    print(f'ValueError: {item.raw_remote_command} {v} {fmt} {unit}')
+                    val = f'{v}'
+                return val
 
         elif role == Qt.EditRole:
             if index.column() == 1:
                 item = index.internalPointer()
-                self.query_requested.emit(index)
-                return item.value
+                val = item.value
+                # print('data', item.name, item.comp, val)
+                return val
 
         elif role == Qt.BackgroundRole:
             item = index.internalPointer()
             if item.comp_type != Index and issubclass(item.comp_type, Component):
                 return QBrush(QColor(243, 230, 225))
             if item.row() % 2 == 0:
                 return QBrush(QColor(240, 240, 253))
 
-        elif role == Qt.ToolTipRole:
-            item = index.internalPointer()
-            if item.is_method or issubclass(item.comp_type, Component):
-                if hasattr(item.comp, '__doc__') and index.column() == 0:
-                    return item.comp.__doc__
-
     def setData(self, index: QModelIndex, value: Any, role: Qt.ItemDataRole):
         """Override from QAbstractItemModel
 
         Set CommandItem according to index and role
 
         Args:
             index (QModelIndex)
             value (Any)
             role (Qt.ItemDataRole)
         """
 
         if role == Qt.EditRole:
-
             if index.column() == 1:
                 item = index.internalPointer()
-                self.set_requested.emit((index, value))
-                sent_command = item.construct_set_command_string(value)
-                self.set_command_sent.emit(sent_command, None)
-
-                # item.set_value(value)
-                # self.dataChanged.emit(index, index, [Qt.EditRole])
+                item.set_value(value)
+                self.dataChanged.emit(index, index, [Qt.EditRole])
                 return True
-
             return False
     
     def headerData(self, section: int, orientation: Qt.Orientation,
-                   role: Qt.ItemDataRole):
+                   role: Qt.ItemDataRole    ):
         """Override from QAbstractItemModel
 
         it returns only data for columns (orientation = Horizontal)
         """
         if role != Qt.DisplayRole:
             return None
 
@@ -220,24 +215,14 @@
         """Return True if item is editable, False otherwise"""
         item = index.internalPointer()
         if type(item) == CommandItem:
             return item.is_editable()
         else:
             return False
 
-    def handle_command(self, cmd_tuple):
-        """
-        External command processor calls this slot once a command is processed
-        """
-        index = cmd_tuple[0]
-        value = cmd_tuple[1]
-        changed = cmd_tuple[2]
-        if changed:
-            self.dataChanged.emit(index, index, [Qt.DisplayRole, Qt.EditRole])
-
 
 if __name__ == "__main__":
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
     view = QTreeView()
     delegate = CommandDelegate()
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import sys
 import math
 
 from srsgui.ui.qt.QtCore import Qt, Signal
 from srsgui.ui.qt.QtWidgets import QApplication, QWidget, QSpinBox, QDoubleSpinBox, \
                                    QLabel, QFormLayout, QWidget, QPushButton, \
                                    QHBoxLayout, QSpacerItem, QSizePolicy
 
 
 class IntegerSpinBox(QSpinBox):
     """
-    Adjust step size depending on the cursor position
+    Adjust step size depending on the cursor postion
     """
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
-        suffix_len = len(self.suffix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
-        sep_pos = len(text) - suffix_len
+        sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
 
         exponent = sep_pos - cur_pos
 
         single_step = 10 ** exponent
@@ -37,94 +32,89 @@
         super().stepBy(steps)
 
         self.lineEdit().deselect()
 
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
-        new_sep_pos = len(text) - suffix_len
+        new_sep_pos = len(text)
 
         new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
 
 
 class FloatSpinBox(QDoubleSpinBox):
     """
-    Adjust step size depending on the cursor position
+    Adjust step size depending on the cursor postion
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.minimum_step = 0.1
         self.significant_figures = 4
-        self.precision = 3
-        self.decis = 3
+        self.precision = 1
 
     def set_minimum_step(self, value):
         self.minimum_step = value
         step = self.minimum_step if self.minimum_step > 1e-12 else 1e-12
-        self.decis = math.ceil(-math.log10(step))
+        self.decimals = math.ceil(math.log10(1.0 / step))
 
     def set_significant_figures(self, value):
         self.significant_figures = value
 
     def valueFromText(self, text):
         try:
             if self.suffix():
                 unit_len = len(self.suffix())
                 value = float(text[:-unit_len])
-
             else:
                 value = float(text)
             if value < self.minimum():
                 value = self.minimum()
             elif value > self.maximum():
                 value = self.maximum()
-
         except ValueError:
             print('valueFromText ValueError', text, self.suffix())
             value = self.minimum()
         return value
 
     def textFromValue(self, value):
-        prec = self.decis
+        prec = self.decimals
         try:
             if value == 0:
                 return '0.0'
 
             digits = math.ceil(math.log10(abs(value)))
-            """
+            # digits = 0 if digits < 0 else digits
+
             if digits == self.significant_figures:
                 step = 1
             else:
                 step = 10 ** (digits - self.significant_figures)
             value = round(value / step) * step
-            """
             prec = self.significant_figures - digits
-            prec = self.decis if prec > self.decis else prec
-            prec = 0 if prec < 0 else prec
-            self.precision = prec
-            format_string = '{:.' + str(prec) + 'f}'
-            text = format_string.format(value)
+            if prec > self.decimals:
+                prec = self.decimals
         except Exception as e:
             print(e)
-            return ''
+        self.precision = prec
+        format_string = '{:.' + str(prec) + 'f}'
+        text = format_string.format(value)
         return text
 
     def stepBy(self, steps):
         prefix_len = len(self.prefix())
-        suffix_len = len(self.suffix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         cur_pos = self.lineEdit().cursorPosition()
         sep_pos = text.find('.')
         if sep_pos < 0:
-            sep_pos = len(text) - suffix_len
+            sep_pos = len(text)
 
         if cur_pos < min_pos:
             return
 
         exponent = sep_pos - cur_pos
         if exponent == -1:
             cur_pos += 1
@@ -140,15 +130,15 @@
         self.lineEdit().deselect()
 
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
 
         text = self.lineEdit().text()
         new_sep_pos = text.find('.')
         if new_sep_pos < 0:
-            new_sep_pos = len(text) - suffix_len
+            new_sep_pos = len(text)
 
         new_cur_pos = cur_pos + new_sep_pos - sep_pos
         if new_cur_pos < min_pos:
             new_cur_pos = min_pos
         self.lineEdit().setCursorPosition(new_cur_pos)
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreeview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import sys
 import inspect
 import logging
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
-from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
+from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView, QPushButton
 
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 from .commandspinbox import RunButton
 
 
 class CommandTreeView(QTreeView):
@@ -52,20 +47,15 @@
         for i in range(self.model().rowCount(parent)):
             index = self.model().index(i, 0, parent)
             self.connect_methods_to_buttons(index)
             try:
                 item = index.internalPointer()
                 if item.is_method:
                     widget_index = self.model().index(i, 1, parent)
-                    spec = inspect.getfullargspec(item.comp)
-                    if spec.defaults is None:
-                        flag = len(spec.args) == 1
-                    else:
-                        flag = len(spec.args) - len(spec.defaults) == 1
-                    if flag:
+                    if len(inspect.getfullargspec(item.comp).args) == 1:
                         parent_comp = item.parent().comp
                         meth = getattr(parent_comp, item.name)
                         if meth and meth.__func__ in parent_comp.allow_run_button:
                             button = RunButton()
                             button.pressed.connect(meth)
                             self.setIndexWidget(widget_index, button)
             except Exception as e:
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import logging
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
 from srsgui.ui.qt.QtWidgets import QWidget
 
 from .ui_commandtreewidget import Ui_CommandTreeWidget
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 
 logger = logging.getLogger(__name__)
 
 
 class CommandTreeWidget(QWidget, Ui_CommandTreeWidget):
-    """
-    CommandTreeWidget is used to display an Instrument class in a tree view
-    based on Qt Model/View architecture.
-    """
-
     def __init__(self, parent=None):
         super(CommandTreeWidget, self).__init__(parent)
         self.parent = parent
         self.setupUi(self)
 
         self.inst = None
         self.name = None
@@ -69,21 +60,20 @@
     def on_method_changed(self, state):
         self.tree_view.method_included = state
         self.tree_view.update_item_display()
 
     def on_raw_command_changed(self, state):
         self.tree_view.show_raw_command = state
         self.model.show_raw_remote_command = self.tree_view.show_raw_command
-        self.model.dataChanged.emit(QModelIndex(), QModelIndex())
 
     def on_capture_clicked(self):
         if self.inst is not None and self.inst.is_connected():
             try:
                 self.model.show_raw_remote_command = self.show_raw_command
-                self.model.load(self.inst)
+                self.model.load(self.inst, False)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
                 # self.tree_view.collapseAll()
                 self.tree_view.update_item_display()
                 self.tree_view.connect_methods_to_buttons()
 
             except Exception as e:
@@ -93,16 +83,14 @@
 
     def on_expand_clicked(self):
         self.tree_view.expandAll()
 
     def on_collapse_clicked(self):
         self.tree_view.collapseAll()
 
-    def closeEvent(self, event) -> None:
-        self.model.command_handler.stop()
 
 if __name__ == '__main__':
     import sys
     from srsgui.ui.qt.QtWidgets import QApplication, QHeaderView
     from srsinst.sr860 import SR860
 
     app = QApplication(sys.argv)
```

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.2.9/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/connectdlg.py` & `srsgui-0.2.9/srsgui/ui/connectdlg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import logging
 from .qt.QtCore import Qt, QSettings
 from .qt.QtWidgets import QDialog, QDialogButtonBox, \
                           QVBoxLayout, QGridLayout,\
                           QSpacerItem, QSizePolicy, \
                           QTabWidget, QWidget, QLabel, \
```

### Comparing `srsgui-0.2.17/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.9/srsgui/ui/deviceinfohandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import logging
 
 from .qt.QtWidgets import QTabWidget, QWidget,  QTextBrowser, QHBoxLayout
 
 logger = logging.getLogger(__name__)
```

### Comparing `srsgui-0.2.17/srsgui/ui/dockhandler.py` & `srsgui-0.2.9/srsgui/ui/dockhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,22 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 import time
 import logging
 
 from .qt.QtCore import Qt
 from .qt.QtWidgets import QDockWidget, QMenu, QAction, QWidget, \
                           QVBoxLayout, QTextBrowser
 
 
 from matplotlib.figure import Figure
 import matplotlib.image as mpimg
 
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
-from .commandhandler import CommandHandler as TerminalCommandHandler
-from .commandtree.commandhandler import CommandHandler as CommandTreeCommandHandler
-
 from .commandterminal import CommandTerminal
-
 # from .commandtree.commandcapturewidget import CommandCaptureWidget
 from .commandtree.commandtreewidget import CommandTreeWidget
 
 logger = logging.getLogger(__name__)
 
 # define matplotlib level before importing to suppress debug messages
 logging.getLogger('matplotlib').setLevel(logging.WARNING)
@@ -65,20 +56,14 @@
             parent.menu_Docks.triggered.disconnect()
         except:
             pass
         actions = parent.menu_Docks.actions()
         for action in actions:
             parent.menu_Docks.removeAction(action)
 
-        # terminal_command_handler needs to access to self.parent.inst_dict
-        self.terminal_command_handler = TerminalCommandHandler(self.parent)
-
-        # CommandItemModel uses command_tree_command_handler to access Commands
-        self.command_tree_command_handler = CommandTreeCommandHandler()
-
         self.init_figure_dock(self.DefaultFigureName)
         self.init_terminal()
         self.init_console()
         self.init_inst_dock('instrument info')
         list(self.dock_dict.values())[-1].hide()
 
         fig = self.dock_dict.pop(self.DefaultFigureName)
@@ -154,19 +139,14 @@
             terminal_dock.setWindowTitle(name)
             terminal_dock.setMinimumSize(250, 150)
 
             self.terminal_widget = CommandTerminal(self.parent)
             terminal_dock.setWidget(self.terminal_widget)
             self.parent.addDockWidget(Qt.RightDockWidgetArea, terminal_dock)
             self.dock_dict[name] = terminal_dock
-
-            # Commands from terminal are processed by terminal_command_handler
-            self.terminal_widget.command_requested.connect(self.terminal_command_handler.process_command)
-            self.terminal_command_handler.command_processed.connect(self.terminal_widget.handle_command)
-
         except Exception as e:
             logger.error(e)
 
     def init_inst_dock(self, name):
         try:
             inst_dock = QDockWidget(self.parent)
             inst_dock.setObjectName(name)
@@ -175,21 +155,14 @@
             title = self.TitleFormat.format(name)
             inst_dock.setWindowTitle(title)
             inst_dock.setMinimumSize(200, 350)
 
             # inst_dock.command_capture_widget = CommandCaptureWidget(self.parent)
             inst_dock.command_capture_widget = CommandTreeWidget(self.parent)
 
-            # Connect the command handler in parent to signals and slots in CommandModel
-            inst_dock.command_capture_widget.model.set_command_sent.connect(self.terminal_widget.handle_command)
-            inst_dock.command_capture_widget.model.query_requested.connect(self.command_tree_command_handler.worker.handle_query)
-            inst_dock.command_capture_widget.model.set_requested.connect(self.command_tree_command_handler.worker.handle_set)
-            self.command_tree_command_handler.worker.query_processed.connect(inst_dock.command_capture_widget.model.handle_command)
-            self.command_tree_command_handler.worker.set_processed.connect(inst_dock.command_capture_widget.model.handle_command)
-
             inst_dock.setWidget(inst_dock.command_capture_widget)
             self.parent.addDockWidget(Qt.LeftDockWidgetArea, inst_dock)
             self.dock_dict[title] = inst_dock
             self.active_inst_dock_names.append(title)
             if len(self.active_inst_dock_names) > 1:
                 self.parent.tabifyDockWidget(
                     self.dock_dict[self.active_inst_dock_names[0]], inst_dock)
@@ -385,11 +358,7 @@
                     dock.toolbar.show()
         else:
             self.action_toolbar.setText('Show Toolbar')
             self.toolbar_visible = False
             for dock in self.dock_dict.values():
                 if hasattr(dock, 'toolbar'):
                     dock.toolbar.hide()
-
-    def stop_command_handlers(self):
-        self.terminal_command_handler.stop()
-        self.command_tree_command_handler.stop()
```

### Comparing `srsgui-0.2.17/srsgui/ui/inputpanel.py` & `srsgui-0.2.9/srsgui/ui/inputpanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import math
 from .qt.QtCore import Qt
 from .qt.QtWidgets import QWidget, QDoubleSpinBox, QSpinBox, QComboBox, \
                           QLineEdit, QLabel, QGridLayout, QPushButton, QScrollArea
 
 from srsgui.inst.commands import Command, IntCommand, FloatCommand, DictCommand
@@ -95,24 +91,24 @@
                     if not self.inst_dict[self.inst_name].is_connected:
                         raise ValueError('{} is not connected'.format(self.inst_name))
 
                     p.set_inst_name(self.inst_name)
                     if issubclass(p.cmd_instance.__class__, IntCommand) or \
                        issubclass(p.cmd_instance.__class__, IntIndexCommand):
                         widget = QSpinBox()
-                        widget.setSuffix(' ' + p.cmd_instance.unit)
+                        widget.setSuffix(p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
                         widget.setSingleStep(p.cmd_instance.step)
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, FloatCommand) or \
                          issubclass(p.cmd_instance.__class__, FloatIndexCommand):
                         widget = QDoubleSpinBox()
-                        widget.setSuffix(' ' + p.cmd_instance.unit)
+                        widget.setSuffix(p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
                         widget.setSingleStep(p.cmd_instance.step)
                         widget.setDecimals(math.ceil(math.log10(1.0 / p.cmd_instance.step)))
                         widget.setAlignment(Qt.AlignRight)
 
                     elif issubclass(p.cmd_instance.__class__, DictCommand) or \
@@ -156,15 +152,15 @@
                     widget.setMaximum(p.value)
                     widget.setEnabled(False)
                 else:
                     widget.setMinimum(p.minimum)
                     widget.setMaximum(p.maximum)
                     widget.setEnabled(True)
                 widget.setSingleStep(p.single_step)
-                widget.setSuffix(' ' + p.suffix)
+                widget.setSuffix(p.suffix)
                 widget.setValue(p.value)
 
                 label = QLabel(name.capitalize())
                 layout.addWidget(label, row, self.FirstColumn)
                 layout.addWidget(widget, row, self.SecondColumn)
                 row += 1
```

### Comparing `srsgui-0.2.17/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.9/srsgui/ui/qt/QtCore.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 """
 Adapter module for QtCore package for PySide6, PySide2 and PyQt5.
 """
 
 # For full extension, use QtPy package
 
 from . import QT_BINDER, PYSIDE6, PYSIDE2, PYQT6, PYQT5
```

### Comparing `srsgui-0.2.17/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.9/srsgui/ui/qt/QtGui.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 """
-Adapter module for QtWidgets package for PySide6, PySide2 and PyQt5
+Adapter module for QtGui package for  PySide6, PySide2 and PyQt5
 """
 
 # For full extension, use QtPy package
 
 from . import QT_BINDER, PYSIDE6, PYSIDE2, PYQT6, PYQT5
 
 if QT_BINDER == PYSIDE6:
-    from PySide6.QtWidgets import *
-    from PySide6.QtGui import QAction
-    from PySide6.QtGui import QShortcut
+    from PySide6.QtGui import *
+    del QAction
+    del QShortcut
     
 elif QT_BINDER == PYSIDE2:
-    from PySide2.QtWidgets import *
+    from PySide2.QtGui import *
 
 elif QT_BINDER == PYQT6:
-    from PyQt6.QtWidgets import *
-    from PyQt6.QtGui import QAction
-    from PyQt6.QtGui import QShortcut
+    from PyQt6.QtGui import *
+    del QAction
+    del QShortcut
 
 elif QT_BINDER == PYQT5:
-    from PyQt5.QtWidgets import *
+    from PyQt5.QtGui import *
 
 else:
-    raise Exception('QT_BINDER is not defined')
+    raise Exception('QT_BINDER is not defined in')
```

### Comparing `srsgui-0.2.17/srsgui/ui/qt/__init__.py` & `srsgui-0.2.9/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/qtloghandler.py` & `srsgui-0.2.9/srsgui/ui/qtloghandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 from logging import getLogger, Handler
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
 
 logger = getLogger(__name__)
```

### Comparing `srsgui-0.2.17/srsgui/ui/resource_rc.py` & `srsgui-0.2.9/srsgui/ui/resource_rc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
-
 # -*- coding: utf-8 -*-
 
 # Resource object code
 #
 # Created by: The Resource Compiler for PyQt5 (Qt v5.15.0)
 #
 # WARNING! All changes made in this file will be lost!
```

### Comparing `srsgui-0.2.17/srsgui/ui/signalhandler.py` & `srsgui-0.2.9/srsgui/ui/signalhandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
 
 from matplotlib.figure import Figure
 
 from srsgui.task.callbacks import Callbacks
```

### Comparing `srsgui-0.2.17/srsgui/ui/srslogo.jpg` & `srsgui-0.2.9/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/stdout.py` & `srsgui-0.2.9/srsgui/ui/stdout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import sys
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
```

### Comparing `srsgui-0.2.17/srsgui/ui/taskmain.py` & `srsgui-0.2.9/srsgui/ui/taskmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
-##! Subject to the MIT License
-##! 
 
 import os
 import sys
 
 import logging
 import logging.handlers
 
@@ -24,16 +20,16 @@
 
 from .inputpanel import InputPanel
 from .signalhandler import SignalHandler
 
 from .stdout import StdOut
 from .qtloghandler import QtLogHandler
 from .deviceinfohandler import DeviceInfoHandler
-
 from .dockhandler import DockHandler
+from .commandhandler import CommandHandler
 
 from srsgui.task.config import Config
 from srsgui.task.sessionhandler import SessionHandler
 from srsgui.task.task import Task, Bold
 
 from srsgui import __version__
 
@@ -77,20 +73,22 @@
         self.data_dict = {}
 
         # self.inst_dict holds instances of subclass of Instrument
         self.inst_dict = {}
         self.inst_info_handler = DeviceInfoHandler(self)
 
         self.dock_handler = DockHandler(self)
-        self.command_handler = self.dock_handler.terminal_command_handler
         self.console = self.dock_handler.console
         self.terminal_widget = self.dock_handler.terminal_widget
         self.plotDockWidget = self.dock_handler.get_dock()
 
         # Make the terminal not blocking for log query
+        self.command_handler = CommandHandler(self)
+        self.terminal_widget.command_requested.connect(self.command_handler.process_command)
+        self.command_handler.command_processed.connect(self.terminal_widget.handle_command)
 
         self.geometry_dict = {}
         try:
             default_config_file = self.DefaultConfigFile
             self.config = Config()
             self.base_data_dir = self.config.base_data_dir
             self.base_log_file_name = self.config.base_log_file_name
@@ -222,43 +220,44 @@
             for name in self.task_dict:
                 m = self.menu_Tasks
 
                 # set up submenu structure
                 p = self.config.task_path_dict[name]
                 if p:
                     tokens = p.split('/')
+                    exists = False
                     for token in tokens:
-                        exists = False
-                        na = None
                         if type(m) == QAction:
                             ma = m.menu()
                             if ma:
                                 m = ma
                             else:
                                 continue
                         for action in m.actions():
                             if token == action.text():
                                 na = action
                                 exists = True
                                 break
                         if not exists:
                             na = m.addMenu(QMenu(token, m))
                         m = na
+                        exists = False
                     if type(m) == QAction:
                         ma = m.menu()
                         if ma:
                             m = ma
                         else:
                             continue
                 action_task = QAction(self)
                 action_task.setText(name)
                 m.addAction(action_task)
         except Exception as e:
             logger.error('Error adding to Task menu Task:{}  Error: {}'.format(name, e))
 
+
     def get_logo_file(self):
         return self.LogoFile
 
     def print_redirect(self, text):
         """
         Handles text output for stdout, stderr and various text output
         from :class:`srsgui.task.task.Task`
@@ -557,15 +556,15 @@
             logger.error('display_question error: {}'.format(e))
 
     def closeEvent(self, event):
         if self.okToContinue():
             # Save settings
             self.save_settings()
 
-            self.dock_handler.stop_command_handlers()
+            self.command_handler.stop()
 
             # Close instruments
             inst_dict = self.inst_dict
             for key in inst_dict:
                 if hasattr(inst_dict[key], "disconnect"):
                     inst_dict[key].disconnect()
         else:
@@ -585,20 +584,15 @@
         except Exception as e:
             logger.error(f"Error in handle_initial_image: {e}")
 
     def onAbout(self,checked):
         msg = ''
         for name in self.inst_dict:
             inst = self.inst_dict[name]
-            if hasattr(inst, __version__):
-                version = inst.__version__
-            else:
-                version = 'N/A'
-
-            msg += '{} version: {}\n'.format(inst.__class__.__name__, version)
+            msg += '{} version: {}\n'.format(inst.__class__.__name__, inst.__version__)
         msg += '\nSrsgui version: {}\n'.format(__version__)
         msg += '\n{} version: {}\n'.format(QT_BINDER, QT_BINDER_VERSION)
         msg += 'Python version: {}\n'.format(sys.version)
         self.display_question(msg, None)
 
     def load_settings(self):
         try:
```

### Comparing `srsgui-0.2.17/srsgui/ui/taskmain.ui` & `srsgui-0.2.9/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.9/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.9/srsgui.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.17
+Version: 0.2.9
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
-Project-URL: homepage, https://github.com/thinkSRS/srsgui
-Project-URL: documentation, https://thinksrs.github.io/srsgui
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,15 +27,15 @@
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+![screenshot](docs/source/_static/example-screen-capture-1.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
@@ -74,22 +72,22 @@
 It will start `srsgui` application.
 
 ## Run the example project
 
 By default, `srsgui` application starts with the last project it ran,
 when it is closed.
  
-To open the example project included in the `srsgui` package 
-(if it does not start with the example project), go to the `srsgui` package 
+To open the example project included in the `srsgui` package,
+, if it does not start with the example project, go to the `srsgui` package 
 directory, find the examples directory, and find a .taskconfig file in an 
 example project folder. 
 
 You can run the second and fifth task in the Task menu 
 even without any instruments connected.
 
 ## Create a project
 
 `Srsgui` is a platform that helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
+
 scripts running in GUI with the same amount of code with writing console-based 
-scripts. For programming API, refer to
-[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
+scripts.
```

