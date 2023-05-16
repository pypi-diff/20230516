# Comparing `tmp/srsgui-0.3.0.tar.gz` & `tmp/srsgui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-yimfk6ka\srsgui-0.3.0.tar", last modified: Tue May 16 20:00:29 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-muaozfbe\srsgui-0.3.1.tar", last modified: Tue May 16 20:21:57 2023, max compression
```

## Comparing `srsgui-0.3.0.tar` & `srsgui-0.3.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.579350 srsgui-0.3.0/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.494819 srsgui-0.3.0/.github/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.499707 srsgui-0.3.0/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.0/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsgui-0.3.0/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3751 2023-05-16 20:00:29.579350 srsgui-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2766 2023-05-16 18:43:29.000000 srsgui-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.519708 srsgui-0.3.0/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.529709 srsgui-0.3.0/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0      222 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     1957 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/create-task.rst
--rw-rw-rw-   0        0        0     6111 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/example.rst
--rw-rw-rw-   0        0        0     3726 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/index.rst
--rw-rw-rw-   0        0        0     4397 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.0/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     1542 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      557 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1761 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0      465 2023-05-16 18:43:29.000000 srsgui-0.3.0/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1511 2023-05-16 19:47:28.000000 srsgui-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 20:00:29.579350 srsgui-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.529709 srsgui-0.3.0/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.499707 srsgui-0.3.0/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.549709 srsgui-0.3.0/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9886 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.556325 srsgui-0.3.0/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8772 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14840 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10381 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9768 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.559347 srsgui-0.3.0/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.0/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5322 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6830 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    22136 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.569350 srsgui-0.3.0/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6138 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.579350 srsgui-0.3.0/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12049 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8334 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5072 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4247 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13808 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.579350 srsgui-0.3.0/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24814 2023-05-16 18:43:29.000000 srsgui-0.3.0/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.0/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:00:29.539708 srsgui-0.3.0/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3751 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 20:00:29.000000 srsgui-0.3.0/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.989693 srsgui-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.899459 srsgui-0.3.1/.github/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.910680 srsgui-0.3.1/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.1/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-15 17:35:24.000000 srsgui-0.3.1/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3730 2023-05-16 20:21:57.989693 srsgui-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2745 2023-05-16 20:18:44.000000 srsgui-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.930685 srsgui-0.3.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0      222 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1957 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/conf.py
+-rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6111 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/example.rst
+-rw-rw-rw-   0        0        0     3726 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/index.rst
+-rw-rw-rw-   0        0        0     4397 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.1/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     1542 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      557 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1761 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0      465 2023-05-16 18:43:29.000000 srsgui-0.3.1/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1511 2023-05-16 19:47:28.000000 srsgui-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 20:21:57.989693 srsgui-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-05-16 20:21:14.000000 srsgui-0.3.1/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.910680 srsgui-0.3.1/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.949690 srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.949690 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.949690 srsgui-0.3.1/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9886 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.959694 srsgui-0.3.1/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8772 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14840 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10381 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9768 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.959694 srsgui-0.3.1/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.1/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5322 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6830 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    22136 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.969694 srsgui-0.3.1/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6138 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.979694 srsgui-0.3.1/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12049 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8334 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5072 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4247 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    13808 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.989693 srsgui-0.3.1/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24814 2023-05-16 18:43:29.000000 srsgui-0.3.1/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.1/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:21:57.940684 srsgui-0.3.1/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3730 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 20:21:57.000000 srsgui-0.3.1/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.3.0/.gitignore` & `srsgui-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/LICENSE.txt` & `srsgui-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/PKG-INFO` & `srsgui-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.0
+Version: 0.3.1
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/html/changelog.html
@@ -32,15 +32,15 @@
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
@@ -91,8 +91,8 @@
 
 ## Create a project
 
 `Srsgui` is a platform that helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code with writing console-based 
 scripts. For programming API, refer to
-[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
+[`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.3.0/README.md` & `srsgui-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
@@ -67,8 +67,8 @@
 
 ## Create a project
 
 `Srsgui` is a platform that helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code with writing console-based 
 scripts. For programming API, refer to
-[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
+[`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.3.0/docs/Makefile` & `srsgui-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.3.1/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.3.1/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.3.1/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/example-screen-capture-1.png` & `srsgui-0.3.1/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/example-screen-capture-2.png` & `srsgui-0.3.1/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/initial-screen-capture.png` & `srsgui-0.3.1/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.3.1/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/second-task-screen-capture.png` & `srsgui-0.3.1/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/terminal-with-example-2.png` & `srsgui-0.3.1/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/_static/terminal-with-example.png` & `srsgui-0.3.1/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/conf.py` & `srsgui-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/create-project.rst` & `srsgui-0.3.1/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/create-task.rst` & `srsgui-0.3.1/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/define-instrument.rst` & `srsgui-0.3.1/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/example.rst` & `srsgui-0.3.1/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/index.rst` & `srsgui-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/installation.rst` & `srsgui-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/make.bat` & `srsgui-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/srsgui.inst.communications.rst` & `srsgui-0.3.1/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/srsgui.inst.rst` & `srsgui-0.3.1/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/srsgui.task.rst` & `srsgui-0.3.1/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/srsgui.ui.commandtree.rst` & `srsgui-0.3.1/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/srsgui.ui.qt.rst` & `srsgui-0.3.1/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/docs/srsgui.ui.rst` & `srsgui-0.3.1/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/pyproject.toml` & `srsgui-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/__init__.py` & `srsgui-0.3.1/srsgui/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.3.0"  # Global version number
+__version__ = "0.3.1"  # Global version number
```

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.3.1/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/__init__.py` & `srsgui-0.3.1/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/commands.py` & `srsgui-0.3.1/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/communications/interface.py` & `srsgui-0.3.1/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/communications/serial_ports.py` & `srsgui-0.3.1/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/communications/serialinterface.py` & `srsgui-0.3.1/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.3.1/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/component.py` & `srsgui-0.3.1/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/exceptions.py` & `srsgui-0.3.1/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/indexcommands.py` & `srsgui-0.3.1/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/inst/instrument.py` & `srsgui-0.3.1/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/task/callbacks.py` & `srsgui-0.3.1/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/task/config.py` & `srsgui-0.3.1/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/task/inputs.py` & `srsgui-0.3.1/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/task/sessionhandler.py` & `srsgui-0.3.1/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/task/task.py` & `srsgui-0.3.1/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/task/taskresult.py` & `srsgui-0.3.1/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandhandler.py` & `srsgui-0.3.1/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandterminal.py` & `srsgui-0.3.1/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commanditem.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.3.1/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.3.1/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/connectdlg.py` & `srsgui-0.3.1/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/deviceinfohandler.py` & `srsgui-0.3.1/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/dockhandler.py` & `srsgui-0.3.1/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/inputpanel.py` & `srsgui-0.3.1/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/qt/QtCore.py` & `srsgui-0.3.1/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/qt/QtGui.py` & `srsgui-0.3.1/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.3.1/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/qt/__init__.py` & `srsgui-0.3.1/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/qtloghandler.py` & `srsgui-0.3.1/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/resource_rc.py` & `srsgui-0.3.1/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/signalhandler.py` & `srsgui-0.3.1/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/srslogo.jpg` & `srsgui-0.3.1/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/stdout.py` & `srsgui-0.3.1/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/taskmain.py` & `srsgui-0.3.1/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/taskmain.ui` & `srsgui-0.3.1/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui/ui/ui_taskmain.py` & `srsgui-0.3.1/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.0/srsgui.egg-info/PKG-INFO` & `srsgui-0.3.1/srsgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.0
+Version: 0.3.1
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/html/changelog.html
@@ -32,15 +32,15 @@
 
    - To write Python scripts (tasks) that run in GUI environment with simple APIs
      provided in ``Task`` class.
 
    - To organize instrument classes and task scripts presented in a GUI application
      using a configuration (.taskconfig) file for a project
 
-![screenshot](https://thinksrs.github.io/srsgui/html/_images/example-screen-capture-2.png " ")
+![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
 To run ``srsgui`` as an application, create a virtual environment, if necessary, 
 and install using ``pip`` with [full] option:  
 
     python -m pip install srsgui[full]
@@ -91,8 +91,8 @@
 
 ## Create a project
 
 `Srsgui` is a platform that helps you to write your own instrument-controlling 
 Python scripts running as a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code with writing console-based 
 scripts. For programming API, refer to
-[`srsgui` documentation](https://thinksrs.github.io/srsgui/html/index.html).
+[`srsgui` documentation](https://thinksrs.github.io/srsgui).
```

### Comparing `srsgui-0.3.0/srsgui.egg-info/SOURCES.txt` & `srsgui-0.3.1/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

