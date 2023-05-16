# Comparing `tmp/srsgui-0.2.17.tar.gz` & `tmp/srsgui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ukm9bb3w\srsgui-0.2.17.tar", last modified: Mon May 15 23:01:24 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-yimfk6ka\srsgui-0.3.0.tar", last modified: Tue May 16 20:00:29 2023, max compression
```

## Comparing `srsgui-0.2.17.tar` & `srsgui-0.3.0.tar`

### file list

```diff
@@ -1,210 +1,118 @@
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
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.579350 srsgui-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.494819 srsgui-0.3.0/.github/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.499707 srsgui-0.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.0/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsgui-0.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3751 2023-05-16 20:00:29.579350 srsgui-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2766 2023-05-16 18:43:29.000000 srsgui-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.519708 srsgui-0.3.0/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.529709 srsgui-0.3.0/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0      222 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1957 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6111 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/example.rst
+-rw-rw-rw-   0        0        0     3726 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/index.rst
+-rw-rw-rw-   0        0        0     4397 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.0/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     1542 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      557 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1761 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0      465 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1511 2023-05-16 19:47:28.000000 srsgui-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 20:00:29.579350 srsgui-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.529709 srsgui-0.3.0/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.499707 srsgui-0.3.0/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.549709 srsgui-0.3.0/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9886 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.556325 srsgui-0.3.0/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8772 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14840 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10381 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9768 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.559347 srsgui-0.3.0/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5322 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6830 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22136 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.569350 srsgui-0.3.0/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6138 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.579350 srsgui-0.3.0/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12049 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8334 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5072 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4247 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13808 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.579350 srsgui-0.3.0/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24814 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3751 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.17/.gitignore` & `srsgui-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/LICENSE.txt` & `srsgui-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/PKG-INFO` & `srsgui-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.17
+Version: 0.3.0
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
+Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
+Project-URL: changelog, https://thinksrs.github.io/srsgui/html/changelog.html
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
+Provides-Extra: docs
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple platform:
 
    - To define instrument classes for instruments that use remote communication,
```

### Comparing `srsgui-0.2.17/README.md` & `srsgui-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/Makefile` & `srsgui-0.3.0/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = .
-BUILDDIR      = ../docs
+BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `srsgui-0.2.17/doc-source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.3.0/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/cg-terminal-screen-capture.png` & `srsgui-0.3.0/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/connect-dialog-box-capture.png` & `srsgui-0.3.0/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/example-screen-capture-1.png` & `srsgui-0.3.0/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/example-screen-capture-2.png` & `srsgui-0.3.0/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/initial-screen-capture.png` & `srsgui-0.3.0/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.3.0/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/second-task-screen-capture.png` & `srsgui-0.3.0/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/terminal-with-example-2.png` & `srsgui-0.3.0/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/_static/terminal-with-example.png` & `srsgui-0.3.0/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/conf.py` & `srsgui-0.3.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from srsgui import __version__
 
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'srsgui'
-copyright = '2022, Chulhoon Kim'
+copyright = '2022, 2023, Stanford Research Systems'
 author = 'Chulhoon Kim'
 version = __version__
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
```

### Comparing `srsgui-0.2.17/doc-source/create-project.rst` & `srsgui-0.3.0/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/create-task.rst` & `srsgui-0.3.0/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/define-instrument.rst` & `srsgui-0.3.0/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/example.rst` & `srsgui-0.3.0/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/index.rst` & `srsgui-0.3.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 
    installation.rst
    create-project.rst
    define-instrument.rst
    create-task.rst
    example.rst
    srsgui.rst
+   troubleshooting.rst
+   changelog.rst
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `srsgui-0.2.17/doc-source/installation.rst` & `srsgui-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/make.bat` & `srsgui-0.3.0/docs/make.bat`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR= .
-set BUILDDIR= ../docs
+set BUILDDIR= _build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
```

### Comparing `srsgui-0.2.17/doc-source/srsgui.inst.communications.rst` & `srsgui-0.3.0/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.inst.rst` & `srsgui-0.3.0/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.task.rst` & `srsgui-0.3.0/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.ui.commandtree.rst` & `srsgui-0.3.0/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.ui.qt.rst` & `srsgui-0.3.0/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/doc-source/srsgui.ui.rst` & `srsgui-0.3.0/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/docs/html/_sources/index.rst.txt` & `srsgui-0.3.0/srsgui.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,98 @@
-.. srsgui documentation master file, created by
-   sphinx-quickstart on Wed Dec  7 16:34:11 2022.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
+Metadata-Version: 2.1
+Name: srsgui
+Version: 0.3.0
+Summary: Framework to run instrument-controlling Python scripts in GUI
+Author: Chulhoon Kim
+License: MIT license
+Project-URL: homepage, https://github.com/thinkSRS/srsgui
+Project-URL: repository, https://github.com/thinkSRS/srsgui.git
+Project-URL: documentation, https://thinksrs.github.io/srsgui
+Project-URL: changelog, https://thinksrs.github.io/srsgui/html/changelog.html
+Keywords: instrument control,data acquisition,data visualization
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: docs
+License-File: LICENSE.txt
 
+# ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
-``srsgui`` : Organize your instrument-controlling Python scripts as a GUI application
-=======================================================================================
-
-``Srsgui`` is a simple framework:
+`Srsgui` is a simple platform:
 
    - To define instrument classes for instruments that use remote communication,
-     based on :class:`Instrument<srsgui.inst.instrument.Instrument>`
-     class and the communication
-     :class:`Interface<srsgui.inst.communications.interface.Interface>` class.
+     based on `Instrument` class and the communication `Interface` class 
+     (By default, serial, TCPIP is available, extendable to VXI11, GPIB and USB-TMC).
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
-     provided in :class:`Task<srsgui.task.task.Task>` class.
+     provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-``Srsgui`` provides the following I/O functionality to a task:
+![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+
+## Installation
+
+To run ``srsgui`` as an application, create a virtual environment, if necessary, 
+and install using ``pip`` with [full] option:  
+
+    python -m pip install srsgui[full]
+
+if it fails, you have to install 
+[pyserial](https://pypi.org/project/pyserial/), 
+[matplotlib](https://pypi.org/project/matplotlib/) and 
+a Python Qt binder ([PySide6](https://pypi.org/project/PySide6/),
+[PySide2](https://pypi.org/project/PySide2/) or 
+[PyQt5](https://pypi.org/project/PyQt5/)) manually.
+``srsgui`` package has these 3 dependencies only.
+
+Some Linux distributions offer some of the Python packages from their 
+repositories only, not from ``pip``. Run web search for more information on 
+system specific installation.   
+
+When matplotlib and one of the Qt binders
+are installed properly, install ``srsgui`` without [full] option:
+
+    python -m pip install srsgui
+
+## Start ``srsgui`` application
+    
+if the Python Script directory is in PATH environment variable,
+Start the application by typing from the command line:
+
+    srsgui
+    
+
+If the script directory is not in PATH,
+
+    python -m srsgui
+    
+It will start `srsgui` application.
+
+## Run the example project
+
+By default, `srsgui` application starts with the last project it ran,
+when it is closed.
+ 
+To open the example project included in the `srsgui` package 
+(if it does not start with the example project), go to the `srsgui` package 
+directory, find the examples directory, and find a .taskconfig file in an 
+example project folder. 
+
+You can run the second and fifth task in the Task menu 
+even without any instruments connected.
 
-   - Python logging output to a console window and a log file
-   - `print` function redirected to the console window
-   - text streaming to multiple selectable windows
-   - terminal from which you can control and query interactively all the instrument defined in the configuration file
-   - real-time updating, non-blocking, multiple matplotlib figures_ that can include multiple axes_
-   - interactively changeable  input parameters fed into a running task
-   - Qt's dockable windows makes layout flexible(
-     :ref:`before <top-of-initial-screen-capture>` and
-     :ref:`after <top-of-screen-capture-1>`)
-   - dedicated output data file generated for each run of a task
-
-Here is a screen shot of ``srsgui`` running with the :ref:`example project <top-of-example-project>`
-included in the ``srsgui`` package.
-
-.. _top-of-screen-capture-1:
-
-.. figure:: ./_static/example-screen-capture-2.png
-    :align: center
-    :figclass: align-center
-
-From the :ref:`Example project <top-of-example-project>` directory, you can see how many lines of code
-you need write to get ``srsgui`` working for control and data acquisition
-from a couple of arbitrary instruments and data visualization for a small task.
-
-   - 5 lines of code for CG635 to control its
-     output frequency (if not count comment lines);
-   - 40 lines to capture waveforms from an oscilloscope (it has a method
-     to download a waveform from the oscilloscope);
-   - 100 lines in the fourth example to check if set frequency
-     changed from the input panel, set a new frequency if changed,
-     capture a new waveform of 700000 points, calculate FFT of the waveform
-     and plot them every 0.2 second;
-   - 8 line in the configuration file to put all together.
-
-If you want to implement a well-defined single operation, it will be as simple as this.
-Well, it is mostly thanks to conciseness of Python code and its rich libraries, though.
-
-When you implement many tasks handling multiple operations along with larger sets of
-remote commands for multiple instruments, ``srsgui`` also provides more ways to
-organize your code.
-
-Here are more information on how to use ``srsgui``.
-
-
-.. toctree::
-   :maxdepth: 2
-
-   installation.rst
-   create-project.rst
-   define-instrument.rst
-   create-task.rst
-   example.rst
-   srsgui.rst
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+## Create a project
 
-.. _figures: https://matplotlib.org/stable/tutorials/introductory/quick_start.html#figure
-.. _axes: https://matplotlib.org/stable/tutorials/introductory/quick_start.html#axes
+`Srsgui` is a platform that helps you to write your own instrument-controlling 
+Python scripts running as a GUI application. Using its APIs, you can write 
+scripts running in GUI with the same amount of code with writing console-based 
+scripts. For programming API, refer to
+[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
```

### Comparing `srsgui-0.2.17/pyproject.toml` & `srsgui-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,17 +28,20 @@
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "srsgui.__version__"}
 
 [project.optional-dependencies]
 full = ['matplotlib >= 3.6.2', 'pyside6 <= 6.4.3']
+docs = ['matplotlib', 'pyside2', 'sphinx>=5', 'sphinx-rtd-theme>=1']
 
 [project.urls]
 homepage = "https://github.com/thinkSRS/srsgui"
+repository = "https://github.com/thinkSRS/srsgui.git"
 documentation = "https://thinksrs.github.io/srsgui"
+changelog = "https://thinksrs.github.io/srsgui/html/changelog.html"
 
 [project.scripts]
 srsgui = "srsgui.__main__:main"
 
 # ... other project metadata fields as specified in:
 #     https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
```

### Comparing `srsgui-0.2.17/srsgui/__init__.py` & `srsgui-0.3.0/srsgui/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.17"  # Global version number
+__version__ = "0.3.0"  # Global version number
```

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/__init__.py` & `srsgui-0.3.0/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/commands.py` & `srsgui-0.3.0/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/communications/interface.py` & `srsgui-0.3.0/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/communications/serial_ports.py` & `srsgui-0.3.0/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/communications/serialinterface.py` & `srsgui-0.3.0/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.3.0/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/component.py` & `srsgui-0.3.0/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/exceptions.py` & `srsgui-0.3.0/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/indexcommands.py` & `srsgui-0.3.0/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/inst/instrument.py` & `srsgui-0.3.0/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/task/callbacks.py` & `srsgui-0.3.0/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/task/config.py` & `srsgui-0.3.0/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/task/inputs.py` & `srsgui-0.3.0/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/task/sessionhandler.py` & `srsgui-0.3.0/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/task/task.py` & `srsgui-0.3.0/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/task/taskresult.py` & `srsgui-0.3.0/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandhandler.py` & `srsgui-0.3.0/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandterminal.py` & `srsgui-0.3.0/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.3.0/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.3.0/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/connectdlg.py` & `srsgui-0.3.0/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/deviceinfohandler.py` & `srsgui-0.3.0/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/dockhandler.py` & `srsgui-0.3.0/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/inputpanel.py` & `srsgui-0.3.0/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/qt/QtCore.py` & `srsgui-0.3.0/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/qt/QtGui.py` & `srsgui-0.3.0/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.3.0/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/qt/__init__.py` & `srsgui-0.3.0/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/qtloghandler.py` & `srsgui-0.3.0/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/resource_rc.py` & `srsgui-0.3.0/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/signalhandler.py` & `srsgui-0.3.0/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/srslogo.jpg` & `srsgui-0.3.0/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/stdout.py` & `srsgui-0.3.0/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/taskmain.py` & `srsgui-0.3.0/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/taskmain.ui` & `srsgui-0.3.0/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.17/srsgui/ui/ui_taskmain.py` & `srsgui-0.3.0/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

