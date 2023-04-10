# Comparing `tmp/srsgui-0.2.5.tar.gz` & `tmp/srsgui-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-oo971myr\srsgui-0.2.5.tar", last modified: Fri Apr  7 19:48:06 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-x9_b0d6j\srsgui-0.2.6.tar", last modified: Mon Apr 10 16:31:04 2023, max compression
```

## Comparing `srsgui-0.2.5.tar` & `srsgui-0.2.6.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.181560 srsgui-0.2.5/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.5/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3330 2023-04-07 19:48:06.181560 srsgui-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.088463 srsgui-0.2.5/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.109847 srsgui-0.2.5/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.119845 srsgui-0.2.5/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 19:48:06.181560 srsgui-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.119845 srsgui-0.2.5/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-04-07 19:44:30.000000 srsgui-0.2.5/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.5/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.079873 srsgui-0.2.5/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.129840 srsgui-0.2.5/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.129840 srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.139834 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.139834 srsgui-0.2.5/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.5/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9530 2023-04-07 18:58:15.000000 srsgui-0.2.5/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.149856 srsgui-0.2.5/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10031 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.5/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.149856 srsgui-0.2.5/srsgui/task/
--rw-rw-rw-   0        0        0        0 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.5/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.171563 srsgui-0.2.5/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.171563 srsgui-0.2.5/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0     2919 2023-04-07 19:30:21.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.py
--rw-rw-rw-   0        0        0     3339 2023-04-07 19:13:45.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.ui
--rw-rw-rw-   0        0        0     3324 2023-04-07 15:52:10.000000 srsgui-0.2.5/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     9222 2023-04-07 15:52:10.000000 srsgui-0.2.5/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     7585 2023-04-07 19:01:35.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     4996 2023-04-07 15:52:11.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3292 2023-04-07 19:41:07.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     9296 2023-04-07 16:02:56.000000 srsgui-0.2.5/srsgui/ui/commandtree/jsonmodel.py
--rw-rw-rw-   0        0        0     4781 2023-04-07 19:18:07.000000 srsgui-0.2.5/srsgui/ui/commandtree/ui_commandcapturewidget.py
--rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    14127 2023-04-07 19:34:20.000000 srsgui-0.2.5/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    11682 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.181560 srsgui-0.2.5/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.5/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24758 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.5/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.5/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.129840 srsgui-0.2.5/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-04-07 19:48:06.000000 srsgui-0.2.5/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.126513 srsgui-0.2.6/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.6/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-10 16:31:04.126513 srsgui-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.026562 srsgui-0.2.6/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.046576 srsgui-0.2.6/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 16:31:04.126513 srsgui-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-10 16:30:05.000000 srsgui-0.2.6/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.6/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.020107 srsgui-0.2.6/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.076539 srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.086534 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.086534 srsgui-0.2.6/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.6/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9530 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.096529 srsgui-0.2.6/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10031 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.6/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.096529 srsgui-0.2.6/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.6/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.116518 srsgui-0.2.6/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.126513 srsgui-0.2.6/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-10 16:08:39.000000 srsgui-0.2.6/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     9349 2023-04-10 16:09:08.000000 srsgui-0.2.6/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7581 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5161 2023-04-10 16:05:18.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     4071 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    11682 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.126513 srsgui-0.2.6/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.6/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.6/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.6/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.6/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2023-04-10 16:31:04.000000 srsgui-0.2.6/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.5/.gitignore` & `srsgui-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/LICENSE.txt` & `srsgui-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/PKG-INFO` & `srsgui-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.5
+Version: 0.2.6
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.5/README.md` & `srsgui-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/Makefile` & `srsgui-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/make.bat` & `srsgui-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.6/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.6/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.6/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.6/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.6/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.6/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.6/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.6/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.6/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.6/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/conf.py` & `srsgui-0.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/create-project.rst` & `srsgui-0.2.6/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/create-task.rst` & `srsgui-0.2.6/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/define-instrument.rst` & `srsgui-0.2.6/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/example.rst` & `srsgui-0.2.6/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/index.rst` & `srsgui-0.2.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/installation.rst` & `srsgui-0.2.6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.6/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/srsgui.inst.rst` & `srsgui-0.2.6/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/srsgui.task.rst` & `srsgui-0.2.6/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.6/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/docs/source/srsgui.ui.rst` & `srsgui-0.2.6/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/pyproject.toml` & `srsgui-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/__init__.py` & `srsgui-0.2.6/srsgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.5"  # Global version number
+__version__ = "0.2.6"  # Global version number
```

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/__init__.py` & `srsgui-0.2.6/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/commands.py` & `srsgui-0.2.6/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/communications/interface.py` & `srsgui-0.2.6/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.6/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.6/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.6/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/component.py` & `srsgui-0.2.6/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/exceptions.py` & `srsgui-0.2.6/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/indexcommands.py` & `srsgui-0.2.6/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/inst/instrument.py` & `srsgui-0.2.6/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/task/callbacks.py` & `srsgui-0.2.6/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/task/config.py` & `srsgui-0.2.6/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/task/inputs.py` & `srsgui-0.2.6/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/task/sessionhandler.py` & `srsgui-0.2.6/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/task/task.py` & `srsgui-0.2.6/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/task/taskresult.py` & `srsgui-0.2.6/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/commandhandler.py` & `srsgui-0.2.6/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/commandterminal.py` & `srsgui-0.2.6/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.py` & `srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files 2% similar despite different names*

#### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.ui`

```diff
@@ -17,43 +17,43 @@
       <item>
         <layout class="QHBoxLayout" name="horizontalLayout">
           <item>
             <layout class="QVBoxLayout" name="verticalLayout">
               <item>
                 <widget class="QCheckBox" name="query_only_checkbox">
                   <property name="text">
-                    <string>Include query-only cmds</string>
+                    <string>Show query-only cmds [QO]</string>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QCheckBox" name="set_only_checkbox">
                   <property name="text">
-                    <string>Show set-only cmds</string>
+                    <string>Show set-only cmds [SO]</string>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QCheckBox" name="excluded_checkbox">
                   <property name="text">
-                    <string>Show excluded cmds</string>
+                    <string>Show excluded cmds [EX]</string>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QCheckBox" name="method_checkbox">
                   <property name="text">
-                    <string>Show methods</string>
+                    <string>Show methods [M]</string>
                   </property>
                 </widget>
               </item>
               <item>
                 <widget class="QCheckBox" name="raw_command_checkbox">
                   <property name="text">
-                    <string>Show raw cmds</string>
+                    <string>Show cmd &lt;CMD&gt;</string>
                   </property>
                 </widget>
               </item>
             </layout>
           </item>
           <item>
             <spacer name="horizontalSpacer">
```

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.6/srsgui/ui/commandtree/commanddelegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,20 @@
         if item.comp_type == Index:
             comp = item.parent().comp
             comp_type = item.parent().comp_type
         else:
             comp = item.comp
             comp_type = item.comp_type
 
-        if comp_type in (FloatCommand, IntCommand,
-                         FloatIndexCommand, IntIndexCommand):
+        if comp_type in (FloatCommand, FloatIndexCommand):
+            value = editor.value()
+            model.setData(index, value, Qt.EditRole)
+            item.precision = editor.precision
+            return True
+        elif comp_type in (IntCommand, IntIndexCommand):
             value = editor.value()
             model.setData(index, value, Qt.EditRole)
             return True
         elif comp_type in (DictCommand, DictIndexCommand):
             val = editor.currentText()
             convert = type(list(comp.get_dict.keys())[0])
             value = convert(val)
```

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.6/srsgui/ui/commandtree/commanditem.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,555 +23,563 @@
 00000160: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00000170: 2020 7365 6c66 2e6e 616d 6520 3d20 2222    self.name = ""
 00000180: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
 00000190: 616c 7565 5f74 7970 6520 3d20 4e6f 6e65  alue_type = None
 000001a0: 2020 2320 5468 6572 6520 6172 6520 3320    # There are 3 
 000001b0: 7479 7065 7320 6f66 2076 616c 7565 733a  types of values:
 000001c0: 2073 7472 2c20 696e 742c 2061 6e64 2066   str, int, and f
-000001d0: 6c6f 6174 0d0a 0d0a 2020 2020 2020 2020  loat....        
-000001e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-000001f0: 6f6d 7020 3d20 4e6f 6e65 0d0a 2020 2020  omp = None..    
-00000200: 2020 2020 7365 6c66 2e63 6f6d 705f 7479      self.comp_ty
-00000210: 7065 203d 204e 6f6e 6520 2020 2320 5468  pe = None   # Th
-00000220: 6572 6520 6172 6520 3520 7479 7065 7320  ere are 5 types 
-00000230: 6f66 2063 6f6d 706f 6e65 6e74 733a 2043  of components: C
-00000240: 6f6d 706f 6e65 6e74 2c20 436f 6d6d 616e  omponent, Comman
-00000250: 6473 2c20 496e 6465 7843 6f6d 6d61 6e64  ds, IndexCommand
-00000260: 732c 206d 6574 686f 6420 616e 6420 496e  s, method and In
-00000270: 6465 780d 0a20 2020 2020 2020 2073 656c  dex..        sel
-00000280: 662e 7365 745f 656e 6162 6c65 203d 2046  f.set_enable = F
-00000290: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-000002a0: 6c66 2e67 6574 5f65 6e61 626c 6520 3d20  lf.get_enable = 
-000002b0: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
-000002c0: 656c 662e 6973 5f6d 6574 686f 6420 3d20  elf.is_method = 
-000002d0: 4661 6c73 650d 0a20 2020 2020 2020 2073  False..        s
-000002e0: 656c 662e 6578 636c 7564 6564 203d 2046  elf.excluded = F
-000002f0: 616c 7365 0d0a 2020 2020 2020 2020 7365  alse..        se
-00000300: 6c66 2e72 6177 5f72 656d 6f74 655f 636f  lf.raw_remote_co
-00000310: 6d6d 616e 6420 3d20 2222 0d0a 2020 2020  mmand = ""..    
-00000320: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
-00000330: 6d70 203d 2030 2e30 0d0a 0d0a 2020 2020  mp = 0.0....    
-00000340: 6465 6620 6170 7065 6e64 4368 696c 6428  def appendChild(
-00000350: 7365 6c66 2c20 6974 656d 3a20 2243 6f6d  self, item: "Com
-00000360: 6d61 6e64 4974 656d 2229 3a0d 0a20 2020  mandItem"):..   
-00000370: 2020 2020 2022 2222 4164 6420 6974 656d       """Add item
-00000380: 2061 7320 6120 6368 696c 6422 2222 0d0a   as a child"""..
-00000390: 2020 2020 2020 2020 7365 6c66 2e5f 6368          self._ch
-000003a0: 696c 6472 656e 2e61 7070 656e 6428 6974  ildren.append(it
-000003b0: 656d 290d 0a0d 0a20 2020 2064 6566 2063  em)....    def c
-000003c0: 6869 6c64 2873 656c 662c 2072 6f77 3a20  hild(self, row: 
-000003d0: 696e 7429 202d 3e20 2243 6f6d 6d61 6e64  int) -> "Command
-000003e0: 4974 656d 223a 0d0a 2020 2020 2020 2020  Item":..        
-000003f0: 2222 2252 6574 7572 6e20 7468 6520 6368  """Return the ch
-00000400: 696c 6420 6f66 2074 6865 2063 7572 7265  ild of the curre
-00000410: 6e74 2069 7465 6d20 6672 6f6d 2074 6865  nt item from the
-00000420: 2067 6976 656e 2072 6f77 2222 220d 0a20   given row""".. 
-00000430: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00000440: 6c66 2e5f 6368 696c 6472 656e 5b72 6f77  lf._children[row
-00000450: 5d0d 0a0d 0a20 2020 2064 6566 2070 6172  ]....    def par
-00000460: 656e 7428 7365 6c66 2920 2d3e 2022 436f  ent(self) -> "Co
-00000470: 6d6d 616e 6449 7465 6d22 3a0d 0a20 2020  mmandItem":..   
-00000480: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00000490: 6865 2070 6172 656e 7420 6f66 2074 6865  he parent of the
-000004a0: 2063 7572 7265 6e74 2069 7465 6d22 2222   current item"""
-000004b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000004c0: 2073 656c 662e 5f70 6172 656e 740d 0a0d   self._parent...
-000004d0: 0a20 2020 2064 6566 2063 6869 6c64 436f  .    def childCo
-000004e0: 756e 7428 7365 6c66 2920 2d3e 2069 6e74  unt(self) -> int
-000004f0: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
-00000500: 7475 726e 2074 6865 206e 756d 6265 7220  turn the number 
-00000510: 6f66 2063 6869 6c64 7265 6e20 6f66 2074  of children of t
-00000520: 6865 2063 7572 7265 6e74 2069 7465 6d22  he current item"
-00000530: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00000540: 726e 206c 656e 2873 656c 662e 5f63 6869  rn len(self._chi
-00000550: 6c64 7265 6e29 0d0a 0d0a 2020 2020 6465  ldren)....    de
-00000560: 6620 726f 7728 7365 6c66 2920 2d3e 2069  f row(self) -> i
-00000570: 6e74 3a0d 0a20 2020 2020 2020 2022 2222  nt:..        """
-00000580: 5265 7475 726e 2074 6865 2072 6f77 2077  Return the row w
-00000590: 6865 7265 2074 6865 2063 7572 7265 6e74  here the current
-000005a0: 2069 7465 6d20 6f63 6375 7069 6573 2069   item occupies i
-000005b0: 6e20 7468 6520 7061 7265 6e74 2222 220d  n the parent""".
-000005c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000005d0: 7365 6c66 2e5f 7061 7265 6e74 2e5f 6368  self._parent._ch
-000005e0: 696c 6472 656e 2e69 6e64 6578 2873 656c  ildren.index(sel
-000005f0: 6629 2069 6620 7365 6c66 2e5f 7061 7265  f) if self._pare
-00000600: 6e74 2065 6c73 6520 300d 0a0d 0a20 2020  nt else 0....   
-00000610: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00000620: 6465 6620 7661 6c75 6528 7365 6c66 293a  def value(self):
-00000630: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
-00000640: 7572 6e20 7468 6520 7661 6c75 6520 6f66  urn the value of
-00000650: 2074 6865 2063 7572 7265 6e74 2069 7465   the current ite
-00000660: 6d22 2222 0d0a 2020 2020 2020 2020 7473  m"""..        ts
-00000670: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
-00000680: 2020 2020 2020 2020 6966 2074 7320 2d20          if ts - 
-00000690: 7365 6c66 2e74 696d 6573 7461 6d70 203c  self.timestamp <
-000006a0: 2030 2e31 3a20 2320 5570 6461 7465 2076   0.1: # Update v
-000006b0: 616c 7565 206c 6174 6572 2074 6861 6e20  alue later than 
-000006c0: 302e 3120 730d 0a20 2020 2020 2020 2020  0.1 s..         
-000006d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000006e0: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
-000006f0: 2069 6620 7365 6c66 2e63 6f6d 705f 7479   if self.comp_ty
-00000700: 7065 203d 3d20 496e 6465 7820 616e 6420  pe == Index and 
-00000710: 7365 6c66 2e67 6574 5f65 6e61 626c 6520  self.get_enable 
-00000720: 616e 6420 6e6f 7420 7365 6c66 2e65 7863  and not self.exc
-00000730: 6c75 6465 643a 0d0a 2020 2020 2020 2020  luded:..        
-00000740: 2020 2020 7365 6c66 2e5f 7661 6c75 6520      self._value 
-00000750: 3d20 7365 6c66 2e5f 7061 7265 6e74 2e63  = self._parent.c
-00000760: 6f6d 702e 5f5f 6765 7469 7465 6d5f 5f28  omp.__getitem__(
-00000770: 7365 6c66 2e63 6f6d 7029 0d0a 2020 2020  self.comp)..    
-00000780: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00000790: 6c75 655f 7479 7065 203d 2074 7970 6528  lue_type = type(
-000007a0: 7365 6c66 2e5f 7661 6c75 6529 0d0a 2020  self._value)..  
-000007b0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-000007c0: 696d 6573 7461 6d70 203d 2074 730d 0a20  imestamp = ts.. 
-000007d0: 2020 2020 2020 2065 6c69 6620 6973 7375         elif issu
-000007e0: 6263 6c61 7373 2874 7970 6528 7365 6c66  bclass(type(self
-000007f0: 2e63 6f6d 7029 2c20 436f 6d6d 616e 6429  .comp), Command)
-00000800: 2061 6e64 2073 656c 662e 6765 745f 656e   and self.get_en
-00000810: 6162 6c65 2061 6e64 206e 6f74 2073 656c  able and not sel
-00000820: 662e 6578 636c 7564 6564 3a0d 0a20 2020  f.excluded:..   
-00000830: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
-00000840: 616c 7565 203d 2073 656c 662e 636f 6d70  alue = self.comp
-00000850: 2e5f 5f67 6574 5f5f 2873 656c 662e 5f70  .__get__(self._p
-00000860: 6172 656e 742e 636f 6d70 2c20 7365 6c66  arent.comp, self
-00000870: 2e5f 7061 7265 6e74 2e63 6f6d 702e 5f5f  ._parent.comp.__
-00000880: 636c 6173 735f 5f29 0d0a 2020 2020 2020  class__)..      
-00000890: 2020 2020 2020 7365 6c66 2e5f 7661 6c75        self._valu
-000008a0: 655f 7479 7065 203d 2074 7970 6528 7365  e_type = type(se
-000008b0: 6c66 2e5f 7661 6c75 6529 0d0a 2020 2020  lf._value)..    
-000008c0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-000008d0: 6573 7461 6d70 203d 2074 730d 0a20 2020  estamp = ts..   
-000008e0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000008f0: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00000900: 6c75 655f 7479 7065 203d 2074 7970 6528  lue_type = type(
-00000910: 7365 6c66 2e5f 7661 6c75 6529 0d0a 0d0a  self._value)....
-00000920: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000930: 656c 662e 5f76 616c 7565 0d0a 0d0a 2020  elf._value....  
-00000940: 2020 4076 616c 7565 2e73 6574 7465 720d    @value.setter.
-00000950: 0a20 2020 2064 6566 2076 616c 7565 2873  .    def value(s
-00000960: 656c 662c 2076 616c 7565 293a 0d0a 2020  elf, value):..  
-00000970: 2020 2020 2020 7365 6c66 2e5f 7661 6c75        self._valu
-00000980: 6520 3d20 7661 6c75 650d 0a0d 0a20 2020  e = value....   
-00000990: 2064 6566 2073 6574 5f76 616c 7565 2873   def set_value(s
-000009a0: 656c 662c 2076 616c 7565 293a 0d0a 2020  elf, value):..  
-000009b0: 2020 2020 2020 2222 2253 6574 2076 616c        """Set val
-000009c0: 7565 2074 6f20 7468 6520 696e 7374 7275  ue to the instru
-000009d0: 6d65 6e74 2061 6e64 2075 7064 6174 6520  ment and update 
-000009e0: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
-000009f0: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
-00000a00: 2020 6966 2073 656c 662e 636f 6d70 5f74    if self.comp_t
-00000a10: 7970 6520 3d3d 2049 6e64 6578 3a0d 0a20  ype == Index:.. 
-00000a20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000a30: 5f70 6172 656e 742e 636f 6d70 2e5f 5f73  _parent.comp.__s
-00000a40: 6574 6974 656d 5f5f 2873 656c 662e 636f  etitem__(self.co
-00000a50: 6d70 2c20 7661 6c75 6529 0d0a 2020 2020  mp, value)..    
-00000a60: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00000a70: 6c75 6520 3d20 7365 6c66 2e5f 7061 7265  lue = self._pare
-00000a80: 6e74 2e63 6f6d 702e 5f5f 6765 7469 7465  nt.comp.__getite
-00000a90: 6d5f 5f28 7365 6c66 2e63 6f6d 7029 0d0a  m__(self.comp)..
-00000aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000ab0: 2e74 696d 6573 7461 6d70 203d 2074 696d  .timestamp = tim
-00000ac0: 652e 7469 6d65 2829 0d0a 2020 2020 2020  e.time()..      
-00000ad0: 2020 656c 6966 2069 7373 7562 636c 6173    elif issubclas
-00000ae0: 7328 7479 7065 2873 656c 662e 636f 6d70  s(type(self.comp
-00000af0: 292c 2043 6f6d 6d61 6e64 293a 0d0a 2020  ), Command):..  
-00000b00: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00000b10: 6f6d 702e 5f5f 7365 745f 5f28 7365 6c66  omp.__set__(self
-00000b20: 2e5f 7061 7265 6e74 2e63 6f6d 702c 2076  ._parent.comp, v
-00000b30: 616c 7565 290d 0a20 2020 2020 2020 2020  alue)..         
-00000b40: 2020 2073 656c 662e 5f76 616c 7565 203d     self._value =
-00000b50: 2073 656c 662e 636f 6d70 2e5f 5f67 6574   self.comp.__get
-00000b60: 5f5f 2873 656c 662e 5f70 6172 656e 742e  __(self._parent.
-00000b70: 636f 6d70 2c20 7365 6c66 2e5f 7061 7265  comp, self._pare
-00000b80: 6e74 2e63 6f6d 702e 5f5f 636c 6173 735f  nt.comp.__class_
-00000b90: 5f29 0d0a 2020 2020 2020 2020 2020 2020  _)..            
-00000ba0: 7365 6c66 2e74 696d 6573 7461 6d70 203d  self.timestamp =
-00000bb0: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
-00000bc0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000bd0: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
-00000be0: 616c 7565 203d 2076 616c 7565 0d0a 0d0a  alue = value....
-00000bf0: 2020 2020 6465 6620 6973 5f65 6469 7461      def is_edita
-00000c00: 626c 6528 7365 6c66 293a 0d0a 2020 2020  ble(self):..    
-00000c10: 2020 2020 2222 2252 6574 7572 6e20 5472      """Return Tr
-00000c20: 7565 2069 6620 7468 6520 6974 656d 2069  ue if the item i
-00000c30: 7320 6564 6974 6162 6c65 2222 220d 0a20  s editable""".. 
-00000c40: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00000c50: 6f6d 705f 7479 7065 203d 3d20 496e 6465  omp_type == Inde
-00000c60: 7820 616e 6420 5c0d 0a20 2020 2020 2020  x and \..       
-00000c70: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00000c80: 745f 656e 6162 6c65 2061 6e64 2073 656c  t_enable and sel
-00000c90: 662e 6765 745f 656e 6162 6c65 2061 6e64  f.get_enable and
-00000ca0: 206e 6f74 2073 656c 662e 6578 636c 7564   not self.exclud
-00000cb0: 6564 3a0d 0a20 2020 2020 2020 2020 2020  ed:..           
-00000cc0: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
-00000cd0: 2020 2020 2020 656c 6966 2069 7373 7562        elif issub
-00000ce0: 636c 6173 7328 7479 7065 2873 656c 662e  class(type(self.
-00000cf0: 636f 6d70 292c 2043 6f6d 6d61 6e64 2920  comp), Command) 
-00000d00: 616e 6420 5c0d 0a20 2020 2020 2020 2020  and \..         
-00000d10: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00000d20: 656e 6162 6c65 2061 6e64 2073 656c 662e  enable and self.
-00000d30: 6765 745f 656e 6162 6c65 2061 6e64 206e  get_enable and n
-00000d40: 6f74 2073 656c 662e 6578 636c 7564 6564  ot self.excluded
-00000d50: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00000d60: 6574 7572 6e20 5472 7565 0d0a 2020 2020  eturn True..    
-00000d70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000d80: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00000d90: 6c73 650d 0a0d 0a20 2020 2064 6566 2067  lse....    def g
-00000da0: 6574 5f75 6e69 7428 7365 6c66 293a 0d0a  et_unit(self):..
-00000db0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00000dc0: 6e20 7468 6520 756e 6974 206f 6620 7468  n the unit of th
-00000dd0: 6520 6974 656d 2222 220d 0a20 2020 2020  e item"""..     
-00000de0: 2020 2063 6f6d 7020 3d20 4e6f 6e65 0d0a     comp = None..
-00000df0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00000e00: 636f 6d70 5f74 7970 6520 3d3d 2049 6e64  comp_type == Ind
-00000e10: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
-00000e20: 2063 6f6d 7020 3d20 7365 6c66 2e70 6172   comp = self.par
-00000e30: 656e 7428 292e 636f 6d70 0d0a 2020 2020  ent().comp..    
-00000e40: 2020 2020 656c 6966 2069 7373 7562 636c      elif issubcl
-00000e50: 6173 7328 7479 7065 2873 656c 662e 636f  ass(type(self.co
-00000e60: 6d70 292c 2043 6f6d 6d61 6e64 2920 6f72  mp), Command) or
-00000e70: 205c 0d0a 2020 2020 2020 2020 2020 2020   \..            
-00000e80: 2069 7373 7562 636c 6173 7328 7479 7065   issubclass(type
-00000e90: 2873 656c 662e 636f 6d70 292c 2049 6e64  (self.comp), Ind
-00000ea0: 6578 436f 6d6d 616e 6429 3a0d 0a20 2020  exCommand):..   
-00000eb0: 2020 2020 2020 2020 2063 6f6d 7020 3d20           comp = 
-00000ec0: 7365 6c66 2e63 6f6d 700d 0a0d 0a20 2020  self.comp....   
-00000ed0: 2020 2020 2069 6620 636f 6d70 2061 6e64       if comp and
-00000ee0: 2068 6173 6174 7472 2863 6f6d 702c 2027   hasattr(comp, '
-00000ef0: 756e 6974 2729 3a0d 0a20 2020 2020 2020  unit'):..       
-00000f00: 2020 2020 2072 6574 7572 6e20 636f 6d70       return comp
-00000f10: 2e75 6e69 740d 0a20 2020 2020 2020 2065  .unit..        e
-00000f20: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000f30: 2020 7265 7475 726e 2022 220d 0a0d 0a20    return "".... 
-00000f40: 2020 2040 636c 6173 736d 6574 686f 640d     @classmethod.
-00000f50: 0a20 2020 2064 6566 206c 6f61 6428 0d0a  .    def load(..
-00000f60: 2020 2020 2020 2020 636c 732c 2063 6f6d          cls, com
-00000f70: 702c 2070 6172 656e 743a 2022 436f 6d6d  p, parent: "Comm
-00000f80: 616e 6449 7465 6d22 203d 204e 6f6e 652c  andItem" = None,
-00000f90: 2073 6f72 743d 4661 6c73 650d 0a20 2020   sort=False..   
-00000fa0: 2029 202d 3e20 2243 6f6d 6d61 6e64 4974   ) -> "CommandIt
-00000fb0: 656d 223a 0d0a 2020 2020 2020 2020 2222  em":..        ""
-00000fc0: 2243 7265 6174 6520 6120 2772 6f6f 7427  "Create a 'root'
-00000fd0: 2043 6f6d 6d61 6e64 4974 656d 2066 726f   CommandItem fro
-00000fe0: 6d20 6120 436f 6d70 6f6e 656e 7420 616e  m a Component an
-00000ff0: 6420 0d0a 2020 2020 2020 2020 706f 7075  d ..        popu
-00001000: 6c61 7465 2069 7473 2073 7562 636f 6d70  late its subcomp
-00001010: 6f6e 656e 7420 616e 6420 636f 6d6d 616e  onent and comman
-00001020: 6473 2072 6563 7572 7369 7665 6c79 2e0d  ds recursively..
-00001030: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001040: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00001050: 2043 6f6d 6d61 6e64 4974 656d 3a20 436f   CommandItem: Co
-00001060: 6d6d 616e 6449 7465 6d0d 0a20 2020 2020  mmandItem..     
-00001070: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00001080: 726f 6f74 5f69 7465 6d20 3d20 436f 6d6d  root_item = Comm
-00001090: 616e 6449 7465 6d28 7061 7265 6e74 290d  andItem(parent).
-000010a0: 0a20 2020 2020 2020 2072 6f6f 745f 6974  .        root_it
-000010b0: 656d 2e6e 616d 6520 3d20 2272 6f6f 7422  em.name = "root"
-000010c0: 0d0a 2020 2020 2020 2020 726f 6f74 5f69  ..        root_i
-000010d0: 7465 6d2e 636f 6d70 203d 2063 6f6d 700d  tem.comp = comp.
-000010e0: 0a0d 0a20 2020 2020 2020 2069 6620 6973  ...        if is
-000010f0: 7375 6263 6c61 7373 2863 6f6d 702e 5f5f  subclass(comp.__
-00001100: 636c 6173 735f 5f2c 2043 6f6d 706f 6e65  class__, Compone
-00001110: 6e74 293a 0d0a 2020 2020 2020 2020 2020  nt):..          
-00001120: 2020 666f 7220 6a20 696e 2063 6f6d 702e    for j in comp.
-00001130: 5f5f 6469 6374 5f5f 3a0d 0a20 2020 2020  __dict__:..     
-00001140: 2020 2020 2020 2020 2020 2069 6620 6a20             if j 
-00001150: 3d3d 2027 5f70 6172 656e 7427 3a0d 0a20  == '_parent':.. 
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
-00001180: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
-00001190: 7461 6e63 6520 3d20 636f 6d70 2e5f 5f64  tance = comp.__d
-000011a0: 6963 745f 5f5b 6a5d 0d0a 2020 2020 2020  ict__[j]..      
-000011b0: 2020 2020 2020 2020 2020 6966 2069 7373            if iss
-000011c0: 7562 636c 6173 7328 696e 7374 616e 6365  ubclass(instance
-000011d0: 2e5f 5f63 6c61 7373 5f5f 2c20 2043 6f6d  .__class__,  Com
-000011e0: 706f 6e65 6e74 293a 2020 2020 2020 2020  ponent):        
-000011f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001200: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00001210: 696c 6420 3d20 636c 732e 6c6f 6164 2869  ild = cls.load(i
-00001220: 6e73 7461 6e63 652c 2072 6f6f 745f 6974  nstance, root_it
-00001230: 656d 2c20 736f 7274 290d 0a20 2020 2020  em, sort)..     
-00001240: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001250: 6869 6c64 2e6e 616d 6520 3d20 6a0d 0a20  hild.name = j.. 
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
-00001280: 696e 7374 616e 6365 0d0a 2020 2020 2020  instance..      
-00001290: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000012a0: 2069 6e73 7461 6e63 6520 696e 2063 6f6d   instance in com
-000012b0: 702e 6578 636c 7564 655f 6361 7074 7572  p.exclude_captur
-000012c0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000012d0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-000012e0: 642e 6578 636c 7564 6564 203d 2054 7275  d.excluded = Tru
-000012f0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00001300: 2020 2020 2020 2063 6869 6c64 2e63 6f6d         child.com
-00001310: 705f 7479 7065 203d 2074 7970 6528 696e  p_type = type(in
-00001320: 7374 616e 6365 290d 0a20 2020 2020 2020  stance)..       
-00001330: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00001340: 745f 6974 656d 2e61 7070 656e 6443 6869  t_item.appendChi
-00001350: 6c64 2863 6869 6c64 290d 0a0d 0a20 2020  ld(child)....   
-00001360: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-00001370: 5f61 7474 7269 6275 7465 7320 3d20 5b5d  _attributes = []
-00001380: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00001390: 7220 6320 696e 2063 6f6d 702e 5f5f 636c  r c in comp.__cl
-000013a0: 6173 735f 5f2e 5f5f 6d72 6f5f 5f3a 2020  ass__.__mro__:  
-000013b0: 2320 6c6f 6f70 2074 6872 6f75 6768 2074  # loop through t
-000013c0: 6865 2063 6c61 7373 6573 2069 6e63 6c75  he classes inclu
-000013d0: 6469 6e67 2073 7570 6572 2063 6c61 7373  ding super class
-000013e0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-000013f0: 2020 2020 6966 206e 6f74 2069 7373 7562      if not issub
-00001400: 636c 6173 7328 632c 2043 6f6d 706f 6e65  class(c, Compone
-00001410: 6e74 293a 2020 2320 6974 2073 686f 756c  nt):  # it shoul
-00001420: 6420 6265 2061 2073 7562 636c 6173 7320  d be a subclass 
-00001430: 6f66 2043 6f6d 706f 6e65 6e74 0d0a 2020  of Component..  
-00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001450: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-00001460: 2020 2020 2020 2020 2069 6620 6320 3d3d           if c ==
-00001470: 2043 6f6d 706f 6e65 6e74 3a20 2023 2042   Component:  # B
-00001480: 7574 2069 7420 7368 6f75 6c64 206e 6f74  ut it should not
-00001490: 2062 6520 436f 6d70 6f6e 656e 740d 0a20   be Component.. 
-000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014b0: 2020 2062 7265 616b 0d0a 0d0a 2020 2020     break....    
-000014c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000014d0: 6b65 7920 696e 2063 2e5f 5f64 6963 745f  key in c.__dict_
-000014e0: 5f3a 0d0a 2020 2020 2020 2020 2020 2020  _:..            
-000014f0: 2020 2020 2020 2020 636d 645f 696e 7374          cmd_inst
-00001500: 616e 6365 203d 2063 2e5f 5f64 6963 745f  ance = c.__dict_
-00001510: 5f5b 6b65 795d 0d0a 2020 2020 2020 2020  _[key]..        
-00001520: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00001530: 6579 2069 6e20 6375 7272 656e 745f 6174  ey in current_at
-00001540: 7472 6962 7574 6573 3a0d 0a20 2020 2020  tributes:..     
-00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001560: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2063 7572 7265 6e74 5f61 7474 7269 6275   current_attribu
-00001590: 7465 732e 6170 7065 6e64 286b 6579 290d  tes.append(key).
-000015a0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000015b0: 2020 2020 2020 2069 6620 6973 7375 6263         if issubc
-000015c0: 6c61 7373 2863 6d64 5f69 6e73 7461 6e63  lass(cmd_instanc
-000015d0: 652e 5f5f 636c 6173 735f 5f2c 2043 6f6d  e.__class__, Com
-000015e0: 6d61 6e64 293a 0d0a 2020 2020 2020 2020  mand):..        
+000001d0: 6c6f 6174 0d0a 2020 2020 2020 2020 7365  loat..        se
+000001e0: 6c66 2e70 7265 6369 7369 6f6e 203d 2034  lf.precision = 4
+000001f0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00000200: 2020 2020 7365 6c66 2e63 6f6d 7020 3d20      self.comp = 
+00000210: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
+00000220: 6c66 2e63 6f6d 705f 7479 7065 203d 204e  lf.comp_type = N
+00000230: 6f6e 6520 2020 2320 5468 6572 6520 6172  one   # There ar
+00000240: 6520 3520 7479 7065 7320 6f66 2063 6f6d  e 5 types of com
+00000250: 706f 6e65 6e74 733a 2043 6f6d 706f 6e65  ponents: Compone
+00000260: 6e74 2c20 436f 6d6d 616e 6473 2c20 496e  nt, Commands, In
+00000270: 6465 7843 6f6d 6d61 6e64 732c 206d 6574  dexCommands, met
+00000280: 686f 6420 616e 6420 496e 6465 780d 0a20  hod and Index.. 
+00000290: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
+000002a0: 656e 6162 6c65 203d 2046 616c 7365 0d0a  enable = False..
+000002b0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+000002c0: 5f65 6e61 626c 6520 3d20 4661 6c73 650d  _enable = False.
+000002d0: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
+000002e0: 5f6d 6574 686f 6420 3d20 4661 6c73 650d  _method = False.
+000002f0: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
+00000300: 636c 7564 6564 203d 2046 616c 7365 0d0a  cluded = False..
+00000310: 2020 2020 2020 2020 7365 6c66 2e72 6177          self.raw
+00000320: 5f72 656d 6f74 655f 636f 6d6d 616e 6420  _remote_command 
+00000330: 3d20 2222 0d0a 2020 2020 2020 2020 7365  = ""..        se
+00000340: 6c66 2e74 696d 6573 7461 6d70 203d 2030  lf.timestamp = 0
+00000350: 2e30 0d0a 0d0a 2020 2020 6465 6620 6170  .0....    def ap
+00000360: 7065 6e64 4368 696c 6428 7365 6c66 2c20  pendChild(self, 
+00000370: 6974 656d 3a20 2243 6f6d 6d61 6e64 4974  item: "CommandIt
+00000380: 656d 2229 3a0d 0a20 2020 2020 2020 2022  em"):..        "
+00000390: 2222 4164 6420 6974 656d 2061 7320 6120  ""Add item as a 
+000003a0: 6368 696c 6422 2222 0d0a 2020 2020 2020  child"""..      
+000003b0: 2020 7365 6c66 2e5f 6368 696c 6472 656e    self._children
+000003c0: 2e61 7070 656e 6428 6974 656d 290d 0a0d  .append(item)...
+000003d0: 0a20 2020 2064 6566 2063 6869 6c64 2873  .    def child(s
+000003e0: 656c 662c 2072 6f77 3a20 696e 7429 202d  elf, row: int) -
+000003f0: 3e20 2243 6f6d 6d61 6e64 4974 656d 223a  > "CommandItem":
+00000400: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00000410: 7572 6e20 7468 6520 6368 696c 6420 6f66  urn the child of
+00000420: 2074 6865 2063 7572 7265 6e74 2069 7465   the current ite
+00000430: 6d20 6672 6f6d 2074 6865 2067 6976 656e  m from the given
+00000440: 2072 6f77 2222 220d 0a20 2020 2020 2020   row"""..       
+00000450: 2072 6574 7572 6e20 7365 6c66 2e5f 6368   return self._ch
+00000460: 696c 6472 656e 5b72 6f77 5d0d 0a0d 0a20  ildren[row].... 
+00000470: 2020 2064 6566 2070 6172 656e 7428 7365     def parent(se
+00000480: 6c66 2920 2d3e 2022 436f 6d6d 616e 6449  lf) -> "CommandI
+00000490: 7465 6d22 3a0d 0a20 2020 2020 2020 2022  tem":..        "
+000004a0: 2222 5265 7475 726e 2074 6865 2070 6172  ""Return the par
+000004b0: 656e 7420 6f66 2074 6865 2063 7572 7265  ent of the curre
+000004c0: 6e74 2069 7465 6d22 2222 0d0a 2020 2020  nt item"""..    
+000004d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000004e0: 5f70 6172 656e 740d 0a0d 0a20 2020 2064  _parent....    d
+000004f0: 6566 2063 6869 6c64 436f 756e 7428 7365  ef childCount(se
+00000500: 6c66 2920 2d3e 2069 6e74 3a0d 0a20 2020  lf) -> int:..   
+00000510: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+00000520: 6865 206e 756d 6265 7220 6f66 2063 6869  he number of chi
+00000530: 6c64 7265 6e20 6f66 2074 6865 2063 7572  ldren of the cur
+00000540: 7265 6e74 2069 7465 6d22 2222 0d0a 2020  rent item"""..  
+00000550: 2020 2020 2020 7265 7475 726e 206c 656e        return len
+00000560: 2873 656c 662e 5f63 6869 6c64 7265 6e29  (self._children)
+00000570: 0d0a 0d0a 2020 2020 6465 6620 726f 7728  ....    def row(
+00000580: 7365 6c66 2920 2d3e 2069 6e74 3a0d 0a20  self) -> int:.. 
+00000590: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+000005a0: 2074 6865 2072 6f77 2077 6865 7265 2074   the row where t
+000005b0: 6865 2063 7572 7265 6e74 2069 7465 6d20  he current item 
+000005c0: 6f63 6375 7069 6573 2069 6e20 7468 6520  occupies in the 
+000005d0: 7061 7265 6e74 2222 220d 0a20 2020 2020  parent"""..     
+000005e0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+000005f0: 7061 7265 6e74 2e5f 6368 696c 6472 656e  parent._children
+00000600: 2e69 6e64 6578 2873 656c 6629 2069 6620  .index(self) if 
+00000610: 7365 6c66 2e5f 7061 7265 6e74 2065 6c73  self._parent els
+00000620: 6520 300d 0a0d 0a20 2020 2040 7072 6f70  e 0....    @prop
+00000630: 6572 7479 0d0a 2020 2020 6465 6620 7661  erty..    def va
+00000640: 6c75 6528 7365 6c66 293a 0d0a 2020 2020  lue(self):..    
+00000650: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+00000660: 6520 7661 6c75 6520 6f66 2074 6865 2063  e value of the c
+00000670: 7572 7265 6e74 2069 7465 6d22 2222 0d0a  urrent item"""..
+00000680: 2020 2020 2020 2020 7473 203d 2074 696d          ts = tim
+00000690: 652e 7469 6d65 2829 0d0a 2020 2020 2020  e.time()..      
+000006a0: 2020 6966 2074 7320 2d20 7365 6c66 2e74    if ts - self.t
+000006b0: 696d 6573 7461 6d70 203c 2030 2e31 3a20  imestamp < 0.1: 
+000006c0: 2320 5570 6461 7465 2076 616c 7565 206c  # Update value l
+000006d0: 6174 6572 2074 6861 6e20 302e 3120 730d  ater than 0.1 s.
+000006e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000006f0: 7572 6e20 7365 6c66 2e5f 7661 6c75 650d  urn self._value.
+00000700: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
+00000710: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
+00000720: 496e 6465 7820 616e 6420 7365 6c66 2e67  Index and self.g
+00000730: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
+00000740: 7420 7365 6c66 2e65 7863 6c75 6465 643a  t self.excluded:
+00000750: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000760: 6c66 2e5f 7661 6c75 6520 3d20 7365 6c66  lf._value = self
+00000770: 2e5f 7061 7265 6e74 2e63 6f6d 702e 5f5f  ._parent.comp.__
+00000780: 6765 7469 7465 6d5f 5f28 7365 6c66 2e63  getitem__(self.c
+00000790: 6f6d 7029 0d0a 2020 2020 2020 2020 2020  omp)..          
+000007a0: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
+000007b0: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
+000007c0: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+000007d0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
+000007e0: 6d70 203d 2074 730d 0a20 2020 2020 2020  mp = ts..       
+000007f0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
+00000800: 2874 7970 6528 7365 6c66 2e63 6f6d 7029  (type(self.comp)
+00000810: 2c20 436f 6d6d 616e 6429 2061 6e64 2073  , Command) and s
+00000820: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
+00000830: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
+00000840: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
+00000850: 2020 2073 656c 662e 5f76 616c 7565 203d     self._value =
+00000860: 2073 656c 662e 636f 6d70 2e5f 5f67 6574   self.comp.__get
+00000870: 5f5f 2873 656c 662e 5f70 6172 656e 742e  __(self._parent.
+00000880: 636f 6d70 2c20 7365 6c66 2e5f 7061 7265  comp, self._pare
+00000890: 6e74 2e63 6f6d 702e 5f5f 636c 6173 735f  nt.comp.__class_
+000008a0: 5f29 0d0a 2020 2020 2020 2020 2020 2020  _)..            
+000008b0: 7365 6c66 2e5f 7661 6c75 655f 7479 7065  self._value_type
+000008c0: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
+000008d0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
+000008e0: 2020 7365 6c66 2e74 696d 6573 7461 6d70    self.timestamp
+000008f0: 203d 2074 730d 0a20 2020 2020 2020 2065   = ts..        e
+00000900: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00000910: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
+00000920: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
+00000930: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
+00000940: 6966 2073 656c 662e 5f76 616c 7565 5f74  if self._value_t
+00000950: 7970 6520 3d3d 2066 6c6f 6174 3a0d 0a20  ype == float:.. 
+00000960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000970: 5f76 616c 7565 203d 2072 6f75 6e64 2873  _value = round(s
+00000980: 656c 662e 5f76 616c 7565 2c20 7365 6c66  elf._value, self
+00000990: 2e70 7265 6369 7369 6f6e 290d 0a0d 0a20  .precision).... 
+000009a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000009b0: 6c66 2e5f 7661 6c75 650d 0a0d 0a20 2020  lf._value....   
+000009c0: 2040 7661 6c75 652e 7365 7474 6572 0d0a   @value.setter..
+000009d0: 2020 2020 6465 6620 7661 6c75 6528 7365      def value(se
+000009e0: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
+000009f0: 2020 2020 2073 656c 662e 5f76 616c 7565       self._value
+00000a00: 203d 2076 616c 7565 0d0a 0d0a 2020 2020   = value....    
+00000a10: 6465 6620 7365 745f 7661 6c75 6528 7365  def set_value(se
+00000a20: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
+00000a30: 2020 2020 2022 2222 5365 7420 7661 6c75       """Set valu
+00000a40: 6520 746f 2074 6865 2069 6e73 7472 756d  e to the instrum
+00000a50: 656e 7420 616e 6420 7570 6461 7465 2074  ent and update t
+00000a60: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00000a70: 6974 656d 2222 220d 0a20 2020 2020 2020  item"""..       
+00000a80: 2069 6620 7365 6c66 2e63 6f6d 705f 7479   if self.comp_ty
+00000a90: 7065 203d 3d20 496e 6465 783a 0d0a 2020  pe == Index:..  
+00000aa0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00000ab0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 7365  parent.comp.__se
+00000ac0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
+00000ad0: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
+00000ae0: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+00000af0: 7565 203d 2073 656c 662e 5f70 6172 656e  ue = self._paren
+00000b00: 742e 636f 6d70 2e5f 5f67 6574 6974 656d  t.comp.__getitem
+00000b10: 5f5f 2873 656c 662e 636f 6d70 290d 0a20  __(self.comp).. 
+00000b20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000b30: 7469 6d65 7374 616d 7020 3d20 7469 6d65  timestamp = time
+00000b40: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
+00000b50: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
+00000b60: 2874 7970 6528 7365 6c66 2e63 6f6d 7029  (type(self.comp)
+00000b70: 2c20 436f 6d6d 616e 6429 3a0d 0a20 2020  , Command):..   
+00000b80: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00000b90: 6d70 2e5f 5f73 6574 5f5f 2873 656c 662e  mp.__set__(self.
+00000ba0: 5f70 6172 656e 742e 636f 6d70 2c20 7661  _parent.comp, va
+00000bb0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
+00000bc0: 2020 7365 6c66 2e5f 7661 6c75 6520 3d20    self._value = 
+00000bd0: 7365 6c66 2e63 6f6d 702e 5f5f 6765 745f  self.comp.__get_
+00000be0: 5f28 7365 6c66 2e5f 7061 7265 6e74 2e63  _(self._parent.c
+00000bf0: 6f6d 702c 2073 656c 662e 5f70 6172 656e  omp, self._paren
+00000c00: 742e 636f 6d70 2e5f 5f63 6c61 7373 5f5f  t.comp.__class__
+00000c10: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00000c20: 656c 662e 7469 6d65 7374 616d 7020 3d20  elf.timestamp = 
+00000c30: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
+00000c40: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00000c50: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00000c60: 6c75 6520 3d20 7661 6c75 650d 0a0d 0a20  lue = value.... 
+00000c70: 2020 2064 6566 2069 735f 6564 6974 6162     def is_editab
+00000c80: 6c65 2873 656c 6629 3a0d 0a20 2020 2020  le(self):..     
+00000c90: 2020 2022 2222 5265 7475 726e 2054 7275     """Return Tru
+00000ca0: 6520 6966 2074 6865 2069 7465 6d20 6973  e if the item is
+00000cb0: 2065 6469 7461 626c 6522 2222 0d0a 2020   editable"""..  
+00000cc0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00000cd0: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
+00000ce0: 2061 6e64 205c 0d0a 2020 2020 2020 2020   and \..        
+00000cf0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00000d00: 5f65 6e61 626c 6520 616e 6420 7365 6c66  _enable and self
+00000d10: 2e67 6574 5f65 6e61 626c 6520 616e 6420  .get_enable and 
+00000d20: 6e6f 7420 7365 6c66 2e65 7863 6c75 6465  not self.exclude
+00000d30: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
+00000d40: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
+00000d50: 2020 2020 2065 6c69 6620 6973 7375 6263       elif issubc
+00000d60: 6c61 7373 2874 7970 6528 7365 6c66 2e63  lass(type(self.c
+00000d70: 6f6d 7029 2c20 436f 6d6d 616e 6429 2061  omp), Command) a
+00000d80: 6e64 205c 0d0a 2020 2020 2020 2020 2020  nd \..          
+00000d90: 2020 2020 2020 7365 6c66 2e73 6574 5f65        self.set_e
+00000da0: 6e61 626c 6520 616e 6420 7365 6c66 2e67  nable and self.g
+00000db0: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
+00000dc0: 7420 7365 6c66 2e65 7863 6c75 6465 643a  t self.excluded:
+00000dd0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00000de0: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+00000df0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000e00: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00000e10: 7365 0d0a 0d0a 2020 2020 6465 6620 6765  se....    def ge
+00000e20: 745f 756e 6974 2873 656c 6629 3a0d 0a20  t_unit(self):.. 
+00000e30: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00000e40: 2074 6865 2075 6e69 7420 6f66 2074 6865   the unit of the
+00000e50: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
+00000e60: 2020 636f 6d70 203d 204e 6f6e 650d 0a20    comp = None.. 
+00000e70: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00000e80: 6f6d 705f 7479 7065 203d 3d20 496e 6465  omp_type == Inde
+00000e90: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
+00000ea0: 636f 6d70 203d 2073 656c 662e 7061 7265  comp = self.pare
+00000eb0: 6e74 2829 2e63 6f6d 700d 0a20 2020 2020  nt().comp..     
+00000ec0: 2020 2065 6c69 6620 6973 7375 6263 6c61     elif issubcla
+00000ed0: 7373 2874 7970 6528 7365 6c66 2e63 6f6d  ss(type(self.com
+00000ee0: 7029 2c20 436f 6d6d 616e 6429 206f 7220  p), Command) or 
+00000ef0: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
+00000f00: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
+00000f10: 7365 6c66 2e63 6f6d 7029 2c20 496e 6465  self.comp), Inde
+00000f20: 7843 6f6d 6d61 6e64 293a 0d0a 2020 2020  xCommand):..    
+00000f30: 2020 2020 2020 2020 636f 6d70 203d 2073          comp = s
+00000f40: 656c 662e 636f 6d70 0d0a 0d0a 2020 2020  elf.comp....    
+00000f50: 2020 2020 6966 2063 6f6d 7020 616e 6420      if comp and 
+00000f60: 6861 7361 7474 7228 636f 6d70 2c20 2775  hasattr(comp, 'u
+00000f70: 6e69 7427 293a 0d0a 2020 2020 2020 2020  nit'):..        
+00000f80: 2020 2020 7265 7475 726e 2063 6f6d 702e      return comp.
+00000f90: 756e 6974 0d0a 2020 2020 2020 2020 656c  unit..        el
+00000fa0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000fb0: 2072 6574 7572 6e20 2222 0d0a 0d0a 2020   return ""....  
+00000fc0: 2020 4063 6c61 7373 6d65 7468 6f64 0d0a    @classmethod..
+00000fd0: 2020 2020 6465 6620 6c6f 6164 280d 0a20      def load(.. 
+00000fe0: 2020 2020 2020 2063 6c73 2c20 636f 6d70         cls, comp
+00000ff0: 2c20 7061 7265 6e74 3a20 2243 6f6d 6d61  , parent: "Comma
+00001000: 6e64 4974 656d 2220 3d20 4e6f 6e65 2c20  ndItem" = None, 
+00001010: 736f 7274 3d46 616c 7365 0d0a 2020 2020  sort=False..    
+00001020: 2920 2d3e 2022 436f 6d6d 616e 6449 7465  ) -> "CommandIte
+00001030: 6d22 3a0d 0a20 2020 2020 2020 2022 2222  m":..        """
+00001040: 4372 6561 7465 2061 2027 726f 6f74 2720  Create a 'root' 
+00001050: 436f 6d6d 616e 6449 7465 6d20 6672 6f6d  CommandItem from
+00001060: 2061 2043 6f6d 706f 6e65 6e74 2061 6e64   a Component and
+00001070: 200d 0a20 2020 2020 2020 2070 6f70 756c   ..        popul
+00001080: 6174 6520 6974 7320 7375 6263 6f6d 706f  ate its subcompo
+00001090: 6e65 6e74 2061 6e64 2063 6f6d 6d61 6e64  nent and command
+000010a0: 7320 7265 6375 7273 6976 656c 792e 0d0a  s recursively...
+000010b0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000010c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000010d0: 436f 6d6d 616e 6449 7465 6d3a 2043 6f6d  CommandItem: Com
+000010e0: 6d61 6e64 4974 656d 0d0a 2020 2020 2020  mandItem..      
+000010f0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00001100: 6f6f 745f 6974 656d 203d 2043 6f6d 6d61  oot_item = Comma
+00001110: 6e64 4974 656d 2870 6172 656e 7429 0d0a  ndItem(parent)..
+00001120: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001130: 6d2e 6e61 6d65 203d 2022 726f 6f74 220d  m.name = "root".
+00001140: 0a20 2020 2020 2020 2072 6f6f 745f 6974  .        root_it
+00001150: 656d 2e63 6f6d 7020 3d20 636f 6d70 0d0a  em.comp = comp..
+00001160: 0d0a 2020 2020 2020 2020 6966 2069 7373  ..        if iss
+00001170: 7562 636c 6173 7328 636f 6d70 2e5f 5f63  ubclass(comp.__c
+00001180: 6c61 7373 5f5f 2c20 436f 6d70 6f6e 656e  lass__, Componen
+00001190: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
+000011a0: 2066 6f72 206a 2069 6e20 636f 6d70 2e5f   for j in comp._
+000011b0: 5f64 6963 745f 5f3a 0d0a 2020 2020 2020  _dict__:..      
+000011c0: 2020 2020 2020 2020 2020 6966 206a 203d            if j =
+000011d0: 3d20 275f 7061 7265 6e74 273a 0d0a 2020  = '_parent':..  
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
+00001200: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+00001210: 616e 6365 203d 2063 6f6d 702e 5f5f 6469  ance = comp.__di
+00001220: 6374 5f5f 5b6a 5d0d 0a20 2020 2020 2020  ct__[j]..       
+00001230: 2020 2020 2020 2020 2069 6620 6973 7375           if issu
+00001240: 6263 6c61 7373 2869 6e73 7461 6e63 652e  bclass(instance.
+00001250: 5f5f 636c 6173 735f 5f2c 2020 436f 6d70  __class__,  Comp
+00001260: 6f6e 656e 7429 3a20 2020 2020 2020 2020  onent):         
+00001270: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00001280: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00001290: 6c64 203d 2063 6c73 2e6c 6f61 6428 696e  ld = cls.load(in
+000012a0: 7374 616e 6365 2c20 726f 6f74 5f69 7465  stance, root_ite
+000012b0: 6d2c 2073 6f72 7429 0d0a 2020 2020 2020  m, sort)..      
+000012c0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000012d0: 696c 642e 6e61 6d65 203d 206a 0d0a 2020  ild.name = j..  
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 6368 696c 642e 636f 6d70 203d 2069    child.comp = i
+00001300: 6e73 7461 6e63 650d 0a20 2020 2020 2020  nstance..       
+00001310: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001320: 696e 7374 616e 6365 2069 6e20 636f 6d70  instance in comp
+00001330: 2e65 7863 6c75 6465 5f63 6170 7475 7265  .exclude_capture
+00001340: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001350: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00001360: 2e65 7863 6c75 6465 6420 3d20 5472 7565  .excluded = True
+00001370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001380: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
+00001390: 5f74 7970 6520 3d20 7479 7065 2869 6e73  _type = type(ins
+000013a0: 7461 6e63 6529 0d0a 2020 2020 2020 2020  tance)..        
+000013b0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+000013c0: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
+000013d0: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
+000013e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000013f0: 6174 7472 6962 7574 6573 203d 205b 5d0d  attributes = [].
+00001400: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00001410: 2063 2069 6e20 636f 6d70 2e5f 5f63 6c61   c in comp.__cla
+00001420: 7373 5f5f 2e5f 5f6d 726f 5f5f 3a20 2023  ss__.__mro__:  #
+00001430: 206c 6f6f 7020 7468 726f 7567 6820 7468   loop through th
+00001440: 6520 636c 6173 7365 7320 696e 636c 7564  e classes includ
+00001450: 696e 6720 7375 7065 7220 636c 6173 7365  ing super classe
+00001460: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00001470: 2020 2069 6620 6e6f 7420 6973 7375 6263     if not issubc
+00001480: 6c61 7373 2863 2c20 436f 6d70 6f6e 656e  lass(c, Componen
+00001490: 7429 3a20 2023 2069 7420 7368 6f75 6c64  t):  # it should
+000014a0: 2062 6520 6120 7375 6263 6c61 7373 206f   be a subclass o
+000014b0: 6620 436f 6d70 6f6e 656e 740d 0a20 2020  f Component..   
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+000014e0: 2020 2020 2020 2020 6966 2063 203d 3d20          if c == 
+000014f0: 436f 6d70 6f6e 656e 743a 2020 2320 4275  Component:  # Bu
+00001500: 7420 6974 2073 686f 756c 6420 6e6f 7420  t it should not 
+00001510: 6265 2043 6f6d 706f 6e65 6e74 0d0a 2020  be Component..  
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 6272 6561 6b0d 0a0d 0a20 2020 2020    break....     
+00001540: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00001550: 6579 2069 6e20 632e 5f5f 6469 6374 5f5f  ey in c.__dict__
+00001560: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001570: 2020 2020 2020 2063 6d64 5f69 6e73 7461         cmd_insta
+00001580: 6e63 6520 3d20 632e 5f5f 6469 6374 5f5f  nce = c.__dict__
+00001590: 5b6b 6579 5d0d 0a20 2020 2020 2020 2020  [key]..         
+000015a0: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+000015b0: 7920 696e 2063 7572 7265 6e74 5f61 7474  y in current_att
+000015c0: 7269 6275 7465 733a 0d0a 2020 2020 2020  ributes:..      
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
 000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 6368 696c 6420 3d20 636c 732e 6c6f 6164  child = cls.load
-00001610: 2863 6d64 5f69 6e73 7461 6e63 652c 2072  (cmd_instance, r
-00001620: 6f6f 745f 6974 656d 2c20 736f 7274 290d  oot_item, sort).
-00001630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001640: 2020 2020 2020 2020 2063 6869 6c64 2e6e           child.n
-00001650: 616d 6520 3d20 6b65 790d 0a20 2020 2020  ame = key..     
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2063 6869 6c64 2e63 6f6d 7020 3d20     child.comp = 
-00001680: 636d 645f 696e 7374 616e 6365 0d0a 2020  cmd_instance..  
-00001690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016a0: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
-000016b0: 5f74 7970 6520 3d20 7479 7065 2863 6d64  _type = type(cmd
-000016c0: 5f69 6e73 7461 6e63 6529 0d0a 0d0a 2020  _instance)....  
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-000016f0: 6170 7065 6e64 4368 696c 6428 6368 696c  appendChild(chil
-00001700: 6429 0d0a 0d0a 2020 2020 2020 2020 2020  d)....          
-00001710: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-00001720: 7373 7562 636c 6173 7328 636d 645f 696e  ssubclass(cmd_in
-00001730: 7374 616e 6365 2e5f 5f63 6c61 7373 5f5f  stance.__class__
-00001740: 2c20 496e 6465 7843 6f6d 6d61 6e64 293a  , IndexCommand):
-00001750: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001760: 2020 2020 2020 2020 2020 6368 696c 6420            child 
-00001770: 3d20 636c 732e 6c6f 6164 2863 6d64 5f69  = cls.load(cmd_i
-00001780: 6e73 7461 6e63 652c 2072 6f6f 745f 6974  nstance, root_it
-00001790: 656d 2c20 736f 7274 290d 0a20 2020 2020  em, sort)..     
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017b0: 2020 2063 6869 6c64 2e6e 616d 6520 3d20     child.name = 
-000017c0: 6b65 790d 0a20 2020 2020 2020 2020 2020  key..           
-000017d0: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-000017e0: 6c64 2e63 6f6d 7020 3d20 636d 645f 696e  ld.comp = cmd_in
-000017f0: 7374 616e 6365 0d0a 2020 2020 2020 2020  stance..        
-00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001810: 6368 696c 642e 636f 6d70 5f74 7970 6520  child.comp_type 
-00001820: 3d20 7479 7065 2863 6d64 5f69 6e73 7461  = type(cmd_insta
-00001830: 6e63 6529 0d0a 2020 2020 2020 2020 2020  nce)..          
-00001840: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00001850: 6f74 5f69 7465 6d2e 6170 7065 6e64 4368  ot_item.appendCh
-00001860: 696c 6428 6368 696c 6429 0d0a 0d0a 2020  ild(child)....  
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 656c 6966 2063 616c 6c61 626c 6528    elif callable(
-00001890: 636d 645f 696e 7374 616e 6365 293a 0d0a  cmd_instance):..
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018b0: 2020 2020 2020 2020 6966 2069 7373 7562          if issub
-000018c0: 636c 6173 7328 636d 645f 696e 7374 616e  class(cmd_instan
-000018d0: 6365 2e5f 5f63 6c61 7373 5f5f 2c20 7479  ce.__class__, ty
-000018e0: 7065 293a 0d0a 2020 2020 2020 2020 2020  pe):..          
+00001600: 6375 7272 656e 745f 6174 7472 6962 7574  current_attribut
+00001610: 6573 2e61 7070 656e 6428 6b65 7929 0d0a  es.append(key)..
+00001620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001630: 2020 2020 2020 6966 2069 7373 7562 636c        if issubcl
+00001640: 6173 7328 636d 645f 696e 7374 616e 6365  ass(cmd_instance
+00001650: 2e5f 5f63 6c61 7373 5f5f 2c20 436f 6d6d  .__class__, Comm
+00001660: 616e 6429 3a0d 0a20 2020 2020 2020 2020  and):..         
+00001670: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001680: 6869 6c64 203d 2063 6c73 2e6c 6f61 6428  hild = cls.load(
+00001690: 636d 645f 696e 7374 616e 6365 2c20 726f  cmd_instance, ro
+000016a0: 6f74 5f69 7465 6d2c 2073 6f72 7429 0d0a  ot_item, sort)..
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 2020 2020 6368 696c 642e 6e61          child.na
+000016d0: 6d65 203d 206b 6579 0d0a 2020 2020 2020  me = key..      
+000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016f0: 2020 6368 696c 642e 636f 6d70 203d 2063    child.comp = c
+00001700: 6d64 5f69 6e73 7461 6e63 650d 0a20 2020  md_instance..   
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
+00001730: 7479 7065 203d 2074 7970 6528 636d 645f  type = type(cmd_
+00001740: 696e 7374 616e 6365 290d 0a0d 0a20 2020  instance)....   
+00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001760: 2020 2020 2072 6f6f 745f 6974 656d 2e61       root_item.a
+00001770: 7070 656e 6443 6869 6c64 2863 6869 6c64  ppendChild(child
+00001780: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00001790: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+000017a0: 7375 6263 6c61 7373 2863 6d64 5f69 6e73  subclass(cmd_ins
+000017b0: 7461 6e63 652e 5f5f 636c 6173 735f 5f2c  tance.__class__,
+000017c0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
+000017d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000017e0: 2020 2020 2020 2020 2063 6869 6c64 203d           child =
+000017f0: 2063 6c73 2e6c 6f61 6428 636d 645f 696e   cls.load(cmd_in
+00001800: 7374 616e 6365 2c20 726f 6f74 5f69 7465  stance, root_ite
+00001810: 6d2c 2073 6f72 7429 0d0a 2020 2020 2020  m, sort)..      
+00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001830: 2020 6368 696c 642e 6e61 6d65 203d 206b    child.name = k
+00001840: 6579 0d0a 2020 2020 2020 2020 2020 2020  ey..            
+00001850: 2020 2020 2020 2020 2020 2020 6368 696c              chil
+00001860: 642e 636f 6d70 203d 2063 6d64 5f69 6e73  d.comp = cmd_ins
+00001870: 7461 6e63 650d 0a20 2020 2020 2020 2020  tance..         
+00001880: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001890: 6869 6c64 2e63 6f6d 705f 7479 7065 203d  hild.comp_type =
+000018a0: 2074 7970 6528 636d 645f 696e 7374 616e   type(cmd_instan
+000018b0: 6365 290d 0a20 2020 2020 2020 2020 2020  ce)..           
+000018c0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+000018d0: 745f 6974 656d 2e61 7070 656e 6443 6869  t_item.appendChi
+000018e0: 6c64 2863 6869 6c64 290d 0a0d 0a20 2020  ld(child)....   
 000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001900: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 2020 6966 206b 6579 2e73 7461 7274      if key.start
-00001930: 7377 6974 6828 275f 2729 3a0d 0a20 2020  swith('_'):..   
-00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001950: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00001960: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00001970: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001990: 2020 2020 2063 6869 6c64 203d 2063 6c73       child = cls
-000019a0: 2e6c 6f61 6428 636d 645f 696e 7374 616e  .load(cmd_instan
-000019b0: 6365 2c20 726f 6f74 5f69 7465 6d2c 2073  ce, root_item, s
-000019c0: 6f72 7429 0d0a 2020 2020 2020 2020 2020  ort)..          
-000019d0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-000019e0: 696c 642e 6e61 6d65 203d 206b 6579 0d0a  ild.name = key..
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2020 2020 2020 6368 696c 642e 636f          child.co
-00001a10: 6d70 203d 2063 6d64 5f69 6e73 7461 6e63  mp = cmd_instanc
-00001a20: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00001a30: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00001a40: 2e63 6f6d 705f 7479 7065 203d 2074 7970  .comp_type = typ
-00001a50: 6528 636d 645f 696e 7374 616e 6365 290d  e(cmd_instance).
-00001a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a70: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00001a80: 656d 2e61 7070 656e 6443 6869 6c64 2863  em.appendChild(c
-00001a90: 6869 6c64 290d 0a20 2020 2020 2020 2065  hild)..        e
-00001aa0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00001ab0: 2020 6966 2063 616c 6c61 626c 6528 636f    if callable(co
-00001ac0: 6d70 293a 0d0a 2020 2020 2020 2020 2020  mp):..          
-00001ad0: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00001ae0: 636f 6d70 203d 2063 6f6d 700d 0a20 2020  comp = comp..   
-00001af0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00001b00: 745f 6974 656d 2e63 6f6d 705f 7479 7065  t_item.comp_type
-00001b10: 203d 2074 7970 6528 636f 6d70 290d 0a20   = type(comp).. 
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001b30: 6f6f 745f 6974 656d 2e69 735f 6d65 7468  oot_item.is_meth
-00001b40: 6f64 203d 2054 7275 650d 0a0d 0a20 2020  od = True....   
-00001b50: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-00001b60: 7375 6263 6c61 7373 2874 7970 6528 636f  subclass(type(co
-00001b70: 6d70 292c 2043 6f6d 6d61 6e64 293a 0d0a  mp), Command):..
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 726f 6f74 5f69 7465 6d2e 636f 6d70 203d  root_item.comp =
-00001ba0: 2063 6f6d 700d 0a20 2020 2020 2020 2020   comp..         
-00001bb0: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
-00001bc0: 2e63 6f6d 705f 7479 7065 203d 2074 7970  .comp_type = typ
-00001bd0: 6528 636f 6d70 290d 0a20 2020 2020 2020  e(comp)..       
-00001be0: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-00001bf0: 656d 2e65 7863 6c75 6465 6420 3d20 636f  em.excluded = co
-00001c00: 6d70 2069 6e20 726f 6f74 5f69 7465 6d2e  mp in root_item.
-00001c10: 7061 7265 6e74 2829 2e63 6f6d 702e 6578  parent().comp.ex
-00001c20: 636c 7564 655f 6361 7074 7572 650d 0a20  clude_capture.. 
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001c40: 6f6f 745f 6974 656d 2e72 6177 5f72 656d  oot_item.raw_rem
-00001c50: 6f74 655f 636f 6d6d 616e 6420 3d20 636f  ote_command = co
-00001c60: 6d70 2e72 656d 6f74 655f 636f 6d6d 616e  mp.remote_comman
-00001c70: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
-00001c80: 2020 2072 6f6f 745f 6974 656d 2e73 6574     root_item.set
-00001c90: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
-00001ca0: 7365 745f 656e 6162 6c65 0d0a 2020 2020  set_enable..    
-00001cb0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00001cc0: 5f69 7465 6d2e 6765 745f 656e 6162 6c65  _item.get_enable
-00001cd0: 203d 2063 6f6d 702e 5f67 6574 5f65 6e61   = comp._get_ena
-00001ce0: 626c 650d 0a0d 0a20 2020 2020 2020 2020  ble....         
-00001cf0: 2020 2065 6c69 6620 6973 7375 6263 6c61     elif issubcla
-00001d00: 7373 2874 7970 6528 636f 6d70 292c 2049  ss(type(comp), I
-00001d10: 6e64 6578 436f 6d6d 616e 6429 3a0d 0a20  ndexCommand):.. 
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001d30: 6f6f 745f 6974 656d 2e63 6f6d 7020 3d20  oot_item.comp = 
-00001d40: 636f 6d70 0d0a 2020 2020 2020 2020 2020  comp..          
-00001d50: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00001d60: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
-00001d70: 2863 6f6d 7029 0d0a 2020 2020 2020 2020  (comp)..        
-00001d80: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00001d90: 6d2e 6578 636c 7564 6564 203d 2063 6f6d  m.excluded = com
-00001da0: 7020 696e 2072 6f6f 745f 6974 656d 2e70  p in root_item.p
-00001db0: 6172 656e 7428 292e 636f 6d70 2e65 7863  arent().comp.exc
-00001dc0: 6c75 6465 5f63 6170 7475 7265 0d0a 2020  lude_capture..  
-00001dd0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00001de0: 6f74 5f69 7465 6d2e 7261 775f 7265 6d6f  ot_item.raw_remo
-00001df0: 7465 5f63 6f6d 6d61 6e64 203d 2063 6f6d  te_command = com
-00001e00: 702e 7265 6d6f 7465 5f63 6f6d 6d61 6e64  p.remote_command
-00001e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001e20: 2020 726f 6f74 5f69 7465 6d2e 7365 745f    root_item.set_
-00001e30: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
-00001e40: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
-00001e50: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00001e60: 6974 656d 2e67 6574 5f65 6e61 626c 6520  item.get_enable 
-00001e70: 3d20 636f 6d70 2e5f 6765 745f 656e 6162  = comp._get_enab
-00001e80: 6c65 0d0a 0d0a 2020 2020 2020 2020 2020  le....          
-00001e90: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001eb0: 6966 2063 6f6d 702e 696e 6465 785f 6469  if comp.index_di
-00001ec0: 6374 2069 7320 4e6f 6e65 3a0d 0a20 2020  ct is None:..   
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 2020 2069 6e64 6578 203d 2063 6f6d       index = com
-00001ef0: 702e 696e 6465 785f 6d69 6e0d 0a20 2020  p.index_min..   
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f10: 2020 2020 2077 6869 6c65 2069 6e64 6578       while index
-00001f20: 203c 3d20 636f 6d70 2e69 6e64 6578 5f6d   <= comp.index_m
-00001f30: 6178 3a0d 0a20 2020 2020 2020 2020 2020  ax:..           
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2063 6869 6c64 203d 2063 6c73 2e6c 6f61   child = cls.loa
-00001f60: 6428 696e 6465 782c 2072 6f6f 745f 6974  d(index, root_it
-00001f70: 656d 2c20 736f 7274 290d 0a20 2020 2020  em, sort)..     
+00001900: 2065 6c69 6620 6361 6c6c 6162 6c65 2863   elif callable(c
+00001910: 6d64 5f69 6e73 7461 6e63 6529 3a0d 0a20  md_instance):.. 
+00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001930: 2020 2020 2020 2069 6620 6973 7375 6263         if issubc
+00001940: 6c61 7373 2863 6d64 5f69 6e73 7461 6e63  lass(cmd_instanc
+00001950: 652e 5f5f 636c 6173 735f 5f2c 2074 7970  e.__class__, typ
+00001960: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001980: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 2069 6620 6b65 792e 7374 6172 7473     if key.starts
+000019b0: 7769 7468 2827 5f27 293a 0d0a 2020 2020  with('_'):..    
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+000019e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000019f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2020 2020 6368 696c 6420 3d20 636c 732e      child = cls.
+00001a20: 6c6f 6164 2863 6d64 5f69 6e73 7461 6e63  load(cmd_instanc
+00001a30: 652c 2072 6f6f 745f 6974 656d 2c20 736f  e, root_item, so
+00001a40: 7274 290d 0a20 2020 2020 2020 2020 2020  rt)..           
+00001a50: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00001a60: 6c64 2e6e 616d 6520 3d20 6b65 790d 0a20  ld.name = key.. 
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2020 2020 2063 6869 6c64 2e63 6f6d         child.com
+00001a90: 7020 3d20 636d 645f 696e 7374 616e 6365  p = cmd_instance
+00001aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001ab0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
+00001ac0: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
+00001ad0: 2863 6d64 5f69 6e73 7461 6e63 6529 0d0a  (cmd_instance)..
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001b00: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
+00001b10: 696c 6429 0d0a 2020 2020 2020 2020 656c  ild)..        el
+00001b20: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001b30: 2069 6620 6361 6c6c 6162 6c65 2863 6f6d   if callable(com
+00001b40: 7029 3a0d 0a20 2020 2020 2020 2020 2020  p):..           
+00001b50: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
+00001b60: 6f6d 7020 3d20 636f 6d70 0d0a 2020 2020  omp = comp..    
+00001b70: 2020 2020 2020 2020 2020 2020 726f 6f74              root
+00001b80: 5f69 7465 6d2e 636f 6d70 5f74 7970 6520  _item.comp_type 
+00001b90: 3d20 7479 7065 2863 6f6d 7029 0d0a 2020  = type(comp)..  
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001bb0: 6f74 5f69 7465 6d2e 6973 5f6d 6574 686f  ot_item.is_metho
+00001bc0: 6420 3d20 5472 7565 0d0a 0d0a 2020 2020  d = True....    
+00001bd0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
+00001be0: 7562 636c 6173 7328 7479 7065 2863 6f6d  ubclass(type(com
+00001bf0: 7029 2c20 436f 6d6d 616e 6429 3a0d 0a20  p), Command):.. 
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001c10: 6f6f 745f 6974 656d 2e63 6f6d 7020 3d20  oot_item.comp = 
+00001c20: 636f 6d70 0d0a 2020 2020 2020 2020 2020  comp..          
+00001c30: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
+00001c40: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
+00001c50: 2863 6f6d 7029 0d0a 2020 2020 2020 2020  (comp)..        
+00001c60: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
+00001c70: 6d2e 6578 636c 7564 6564 203d 2063 6f6d  m.excluded = com
+00001c80: 7020 696e 2072 6f6f 745f 6974 656d 2e70  p in root_item.p
+00001c90: 6172 656e 7428 292e 636f 6d70 2e65 7863  arent().comp.exc
+00001ca0: 6c75 6465 5f63 6170 7475 7265 0d0a 2020  lude_capture..  
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001cc0: 6f74 5f69 7465 6d2e 7261 775f 7265 6d6f  ot_item.raw_remo
+00001cd0: 7465 5f63 6f6d 6d61 6e64 203d 2063 6f6d  te_command = com
+00001ce0: 702e 7265 6d6f 7465 5f63 6f6d 6d61 6e64  p.remote_command
+00001cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001d00: 2020 726f 6f74 5f69 7465 6d2e 7365 745f    root_item.set_
+00001d10: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
+00001d20: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
+00001d30: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00001d40: 6974 656d 2e67 6574 5f65 6e61 626c 6520  item.get_enable 
+00001d50: 3d20 636f 6d70 2e5f 6765 745f 656e 6162  = comp._get_enab
+00001d60: 6c65 0d0a 0d0a 2020 2020 2020 2020 2020  le....          
+00001d70: 2020 656c 6966 2069 7373 7562 636c 6173    elif issubclas
+00001d80: 7328 7479 7065 2863 6f6d 7029 2c20 496e  s(type(comp), In
+00001d90: 6465 7843 6f6d 6d61 6e64 293a 0d0a 2020  dexCommand):..  
+00001da0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00001db0: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
+00001dc0: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
+00001dd0: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
+00001de0: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
+00001df0: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
+00001e00: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
+00001e10: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
+00001e20: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
+00001e30: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
+00001e40: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
+00001e50: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
+00001e60: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
+00001e70: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
+00001e80: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
+00001e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ea0: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
+00001eb0: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
+00001ec0: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
+00001ed0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
+00001ee0: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
+00001ef0: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
+00001f00: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+00001f10: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001f30: 6620 636f 6d70 2e69 6e64 6578 5f64 6963  f comp.index_dic
+00001f40: 7420 6973 204e 6f6e 653a 0d0a 2020 2020  t is None:..    
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 2020 2020 696e 6465 7820 3d20 636f 6d70      index = comp
+00001f70: 2e69 6e64 6578 5f6d 696e 0d0a 2020 2020  .index_min..    
 00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f90: 2020 2020 2020 2063 6869 6c64 2e6e 616d         child.nam
-00001fa0: 6520 3d20 6627 7b69 6e64 6578 7d27 0d0a  e = f'{index}'..
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00001fd0: 642e 636f 6d70 203d 2069 6e64 6578 0d0a  d.comp = index..
-00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ff0: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00002000: 642e 636f 6d70 5f74 7970 6520 3d20 496e  d.comp_type = In
-00002010: 6465 780d 0a20 2020 2020 2020 2020 2020  dex..           
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2063 6869 6c64 2e65 7863 6c75 6465 6420   child.excluded 
-00002040: 3d20 726f 6f74 5f69 7465 6d2e 6578 636c  = root_item.excl
-00002050: 7564 6564 0d0a 2020 2020 2020 2020 2020  uded..          
+00001f90: 2020 2020 7768 696c 6520 696e 6465 7820      while index 
+00001fa0: 3c3d 2063 6f6d 702e 696e 6465 785f 6d61  <= comp.index_ma
+00001fb0: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 6368 696c 6420 3d20 636c 732e 6c6f 6164  child = cls.load
+00001fe0: 2869 6e64 6578 2c20 726f 6f74 5f69 7465  (index, root_ite
+00001ff0: 6d2c 2073 6f72 7429 0d0a 2020 2020 2020  m, sort)..      
+00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002010: 2020 2020 2020 6368 696c 642e 6e61 6d65        child.name
+00002020: 203d 2066 277b 696e 6465 787d 270d 0a20   = f'{index}'.. 
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00002050: 2e63 6f6d 7020 3d20 696e 6465 780d 0a20  .comp = index.. 
 00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 6368 696c 642e 7365 745f 656e 6162    child.set_enab
-00002080: 6c65 203d 2072 6f6f 745f 6974 656d 2e73  le = root_item.s
-00002090: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
+00002070: 2020 2020 2020 2020 2020 2063 6869 6c64             child
+00002080: 2e63 6f6d 705f 7479 7065 203d 2049 6e64  .comp_type = Ind
+00002090: 6578 0d0a 2020 2020 2020 2020 2020 2020  ex..            
 000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 2020 2020 2020 2063 6869 6c64 2e67 6574         child.get
-000020c0: 5f65 6e61 626c 6520 3d20 726f 6f74 5f69  _enable = root_i
-000020d0: 7465 6d2e 6765 745f 656e 6162 6c65 0d0a  tem.get_enable..
+000020b0: 6368 696c 642e 6578 636c 7564 6564 203d  child.excluded =
+000020c0: 2072 6f6f 745f 6974 656d 2e65 7863 6c75   root_item.exclu
+000020d0: 6465 640d 0a20 2020 2020 2020 2020 2020  ded..           
 000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020f0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00002100: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
-00002110: 6428 6368 696c 6429 0d0a 2020 2020 2020  d(child)..      
+000020f0: 2063 6869 6c64 2e73 6574 5f65 6e61 626c   child.set_enabl
+00002100: 6520 3d20 726f 6f74 5f69 7465 6d2e 7365  e = root_item.se
+00002110: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
 00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 696e 6465 7820 2b3d 2031        index += 1
-00002140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002150: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00002130: 2020 2020 2020 6368 696c 642e 6765 745f        child.get_
+00002140: 656e 6162 6c65 203d 2072 6f6f 745f 6974  enable = root_it
+00002150: 656d 2e67 6574 5f65 6e61 626c 650d 0a20  em.get_enable.. 
 00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
-00002180: 636f 6d70 2e69 6e64 6578 5f64 6963 743a  comp.index_dict:
-00002190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000021a0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-000021b0: 696c 6420 3d20 636c 732e 6c6f 6164 286b  ild = cls.load(k
-000021c0: 6579 2c20 726f 6f74 5f69 7465 6d2c 2073  ey, root_item, s
-000021d0: 6f72 7429 0d0a 2020 2020 2020 2020 2020  ort)..          
+00002170: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
+00002180: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
+00002190: 2863 6869 6c64 290d 0a20 2020 2020 2020  (child)..       
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 2020 2020 2069 6e64 6578 202b 3d20 310d       index += 1.
+000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021d0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
 000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2020 6368 696c 642e 6e61 6d65 203d 2066    child.name = f
-00002200: 277b 6b65 797d 270d 0a20 2020 2020 2020  '{key}'..       
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2063 6869 6c64 2e63 6f6d 7020       child.comp 
-00002230: 3d20 6b65 790d 0a20 2020 2020 2020 2020  = key..         
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2063 6869 6c64 2e63 6f6d 705f 7479     child.comp_ty
-00002260: 7065 203d 2049 6e64 6578 0d0a 2020 2020  pe = Index..    
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 2020 2020 2020 6368 696c 642e 6578          child.ex
-00002290: 6c75 6465 6420 3d20 726f 6f74 5f69 7465  luded = root_ite
-000022a0: 6d2e 6578 636c 7564 6564 0d0a 2020 2020  m.excluded..    
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2020 2020 6368 696c 642e 7365          child.se
-000022d0: 745f 656e 6162 6c65 203d 2063 6f6d 702e  t_enable = comp.
-000022e0: 5f73 6574 5f65 6e61 626c 650d 0a20 2020  _set_enable..   
+000021f0: 2020 2020 666f 7220 6b65 7920 696e 2063      for key in c
+00002200: 6f6d 702e 696e 6465 785f 6469 6374 3a0d  omp.index_dict:.
+00002210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002220: 2020 2020 2020 2020 2020 2020 2063 6869               chi
+00002230: 6c64 203d 2063 6c73 2e6c 6f61 6428 6b65  ld = cls.load(ke
+00002240: 792c 2072 6f6f 745f 6974 656d 2c20 736f  y, root_item, so
+00002250: 7274 290d 0a20 2020 2020 2020 2020 2020  rt)..           
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2063 6869 6c64 2e6e 616d 6520 3d20 6627   child.name = f'
+00002280: 7b6b 6579 7d27 0d0a 2020 2020 2020 2020  {key}'..        
+00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022a0: 2020 2020 6368 696c 642e 636f 6d70 203d      child.comp =
+000022b0: 206b 6579 0d0a 2020 2020 2020 2020 2020   key..          
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 6368 696c 642e 636f 6d70 5f74 7970    child.comp_typ
+000022e0: 6520 3d20 496e 6465 780d 0a20 2020 2020  e = Index..     
 000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2020 2063 6869 6c64 2e67           child.g
-00002310: 6574 5f65 6e61 626c 6520 3d20 636f 6d70  et_enable = comp
-00002320: 2e5f 6765 745f 656e 6162 6c65 0d0a 2020  ._get_enable..  
+00002300: 2020 2020 2020 2063 6869 6c64 2e65 786c         child.exl
+00002310: 7564 6564 203d 2072 6f6f 745f 6974 656d  uded = root_item
+00002320: 2e65 7863 6c75 6465 640d 0a20 2020 2020  .excluded..     
 00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
-00002350: 7465 6d2e 6170 7065 6e64 4368 696c 6428  tem.appendChild(
-00002360: 6368 696c 6429 0d0a 2020 2020 2020 2020  child)..        
-00002370: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00002380: 7863 6570 7469 6f6e 2061 7320 653a 0d0a  xception as e:..
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 7072 696e 7428 6627 2020 7b74      print(f'  {t
-000023b0: 7970 6528 6529 7d20 7b65 7d20 636f 6d6d  ype(e)} {e} comm
-000023c0: 616e 643a 7b63 6f6d 702e 7265 6d6f 7465  and:{comp.remote
-000023d0: 5f63 6f6d 6d61 6e64 7d20 696e 6465 783a  _command} index:
-000023e0: 207b 696e 6465 787d 2729 0d0a 2020 2020   {index}')..    
-000023f0: 2020 2020 7265 7475 726e 2072 6f6f 745f      return root_
-00002400: 6974 656d 0d0a                           item..
+00002340: 2020 2020 2020 2063 6869 6c64 2e73 6574         child.set
+00002350: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
+00002360: 7365 745f 656e 6162 6c65 0d0a 2020 2020  set_enable..    
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 6368 696c 642e 6765          child.ge
+00002390: 745f 656e 6162 6c65 203d 2063 6f6d 702e  t_enable = comp.
+000023a0: 5f67 6574 5f65 6e61 626c 650d 0a20 2020  _get_enable..   
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
+000023d0: 656d 2e61 7070 656e 6443 6869 6c64 2863  em.appendChild(c
+000023e0: 6869 6c64 290d 0a20 2020 2020 2020 2020  hild)..         
+000023f0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00002400: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
+00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002420: 2020 2070 7269 6e74 2866 2720 207b 7479     print(f'  {ty
+00002430: 7065 2865 297d 207b 657d 2063 6f6d 6d61  pe(e)} {e} comma
+00002440: 6e64 3a7b 636f 6d70 2e72 656d 6f74 655f  nd:{comp.remote_
+00002450: 636f 6d6d 616e 647d 2069 6e64 6578 3a20  command} index: 
+00002460: 7b69 6e64 6578 7d27 290d 0a20 2020 2020  {index}')..     
+00002470: 2020 2072 6574 7572 6e20 726f 6f74 5f69     return root_i
+00002480: 7465 6d0d 0a                             tem..
```

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.6/srsgui/ui/commandtree/commandmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.endResetModel()
 
         return True
 
     def data(self, index: QModelIndex, role: Qt.ItemDataRole) -> Any:
         """Override from QAbstractItemModel
 
-        Return data from a json item according index and role
+        Return data from an item according index and role
         """
 
         if not index.isValid():
             return None
 
         if role == Qt.DisplayRole:
             if index.column() == 0:
```

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.6/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     """
     Adjust step size depending on the cursor postion
     """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.minimum_step = 0.1
         self.significant_figures = 4
+        self.precision = 1
 
     def set_minimum_step(self, value):
         self.minimum_step = value
         step = self.minimum_step if self.minimum_step > 1e-12 else 1e-12
         self.decimals = math.ceil(math.log10(1.0 / step))
 
     def set_significant_figures(self, value):
@@ -71,30 +72,33 @@
                 value = self.maximum()
         except ValueError:
             print('valueFromText ValueError', text, self.suffix())
             value = self.minimum()
         return value
 
     def textFromValue(self, value):
+        prec = self.decimals
         try:
             if value == 0:
                 return '0.0'
 
             digits = math.ceil(math.log10(abs(value)))
-            digits = 0 if digits < 0 else digits
+            # digits = 0 if digits < 0 else digits
 
             if digits == self.significant_figures:
                 step = 1
             else:
                 step = 10 ** (digits - self.significant_figures)
             value = round(value / step) * step
             prec = self.significant_figures - digits
+            if prec > self.decimals:
+                prec = self.decimals
         except Exception as e:
             print(e)
-
+        self.precision = prec
         format_string = '{:.' + str(prec) + 'f}'
         text = format_string.format(value)
         return text
     
     def stepBy(self, steps):        
         prefix_len = len(self.prefix())
         min_pos = prefix_len + 1 if self.value() < 0 else prefix_len
```

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.6/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import logging
 
-from srsgui.ui.qt.QtCore import Qt
+from srsgui.ui.qt.QtCore import Qt, QModelIndex
 from srsgui.ui.qt.QtWidgets import QWidget
+
 from .ui_commandcapturewidget import Ui_CommandCaptureWidget
 
 from .commandmodel import CommandModel
 from .commanddelegate import CommandDelegate
 
 logger = logging.getLogger(__name__)
 
@@ -25,19 +26,14 @@
         self.method_included = False
         self.show_raw_command = False
 
         self.model = CommandModel()
         self.tree_view.setItemDelegate(CommandDelegate())
         self.tree_view.setModel(self.model)
 
-        self.query_only_checkbox.hide()
-        self.set_only_checkbox.hide()
-        self.excluded_checkbox.hide()
-        self.method_checkbox.hide()
-        self.raw_command_checkbox.hide()
         self.expand_button.hide()
 
         self.query_only_checkbox.stateChanged.connect(self.on_query_only_changed)
         self.set_only_checkbox.stateChanged.connect(self.on_set_only_changed)
         self.excluded_checkbox.stateChanged.connect(self.on_excluded_changed)
         self.method_checkbox.stateChanged.connect(self.on_method_changed)
         self.raw_command_checkbox.stateChanged.connect(self.on_raw_command_changed)
@@ -47,42 +43,66 @@
         self.collapse_button.clicked.connect(self.on_collapse_clicked)
 
     def set_inst(self, name, inst):
         self.inst = inst
         self.name = name
 
     def on_query_only_changed(self, state):
-        self.query_only_included = state != Qt.Unchecked
+        self.query_only_included = state
+        self.update_item_display()
+
+    def update_item_display(self, parent=QModelIndex()):
+        for i in range(self.model.rowCount(parent)):
+            index = self.model.index(i, 0, parent)
+            self.update_item_display(index)
+
+            item = index.internalPointer()
+            query_only = set_only = is_method = is_excluded = False
+            if not self.query_only_included:
+                if not item.set_enable and item.get_enable:
+                    query_only = True
+            if not self.set_only_included:
+                if item.set_enable and not item.get_enable:
+                    set_only = True
+            if not self.method_included:
+                if item.is_method:
+                    is_method = True
+            if not self.excluded_included:
+                if item.excluded:
+                    is_excluded = True
+            state = query_only or set_only or is_method or is_excluded
+            self.tree_view.setRowHidden(i, parent, state)
 
     def on_set_only_changed(self, state):
-        self.set_only_included = state != Qt.Unchecked
+        self.set_only_included = state
+        self.update_item_display()
 
     def on_excluded_changed(self, state):
-        self.excluded_included = state != Qt.Unchecked
+        self.excluded_included = state
+        self.update_item_display()
 
     def on_method_changed(self, state):
-        self.method_included = state != Qt.Unchecked
+        self.method_included = state
+        self.update_item_display()
 
     def on_raw_command_changed(self, state):
-        self.show_raw_command = state != Qt.Unchecked
+        self.show_raw_command = state
+        self.model.show_raw_remote_command = self.show_raw_command
 
     def on_capture_clicked(self):
         if self.inst is not None and self.inst.is_connected():
-            # capture = self.inst.capture_commands(
-            #     self.query_only_included, self.set_only_included, self.excluded_included,
-            #     self.method_included, self.show_raw_command
-            # )
-            # self.model.load(capture, False)
             try:
+                self.model.show_raw_remote_command = self.show_raw_command
                 self.model.load(self.inst, False)
                 self.tree_view.expandToDepth(1)
                 self.tree_view.resizeColumnToContents(0)
-                self.tree_view.collapseAll()
+                # self.tree_view.collapseAll()
+                self.update_item_display()
             except Exception as e:
-                logger.error(f'Failed to capture commands from {self.name}: {e}')
+                logger.error(f'Failed to load command tree from {self.name}: {e}')
         else:
             logger.warning(f' {self.name} is NOT connected.')
 
     def on_expand_clicked(self):
         self.tree_view.expandAll()
 
     def on_collapse_clicked(self):
```

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/jsonmodel.py` & `srsgui-0.2.6/srsgui/ui/commandtree/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/commandtree/ui_commandcapturewidget.py` & `srsgui-0.2.6/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -92,17 +92,17 @@
         self.retranslateUi(CommandCaptureWidget)
 
         QMetaObject.connectSlotsByName(CommandCaptureWidget)
     # setupUi
 
     def retranslateUi(self, CommandCaptureWidget):
         CommandCaptureWidget.setWindowTitle(QCoreApplication.translate("CommandCaptureWidget", u"Form", None))
-        self.query_only_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Include query-only cmds", None))
-        self.set_only_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show set-only cmds", None))
-        self.excluded_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show excluded cmds", None))
-        self.method_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show methods", None))
-        self.raw_command_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show raw cmds", None))
+        self.query_only_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show query-only cmds [QO]", None))
+        self.set_only_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show set-only cmds [SO]", None))
+        self.excluded_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show excluded cmds [EX]", None))
+        self.method_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show methods [M]", None))
+        self.raw_command_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show raw cmds <CMD>", None))
         self.capture_button.setText(QCoreApplication.translate("CommandCaptureWidget", u"Capture", None))
         self.expand_button.setText(QCoreApplication.translate("CommandCaptureWidget", u"Expand all", None))
         self.collapse_button.setText(QCoreApplication.translate("CommandCaptureWidget", u"Collapse all", None))
     # retranslateUi
```

### Comparing `srsgui-0.2.5/srsgui/ui/connectdlg.py` & `srsgui-0.2.6/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.6/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/dockhandler.py` & `srsgui-0.2.6/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/inputpanel.py` & `srsgui-0.2.6/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.6/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.6/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.6/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/qt/__init__.py` & `srsgui-0.2.6/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/qtloghandler.py` & `srsgui-0.2.6/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/resource_rc.py` & `srsgui-0.2.6/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/signalhandler.py` & `srsgui-0.2.6/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/srslogo.jpg` & `srsgui-0.2.6/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/stdout.py` & `srsgui-0.2.6/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/taskmain.py` & `srsgui-0.2.6/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/taskmain.ui` & `srsgui-0.2.6/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.6/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.5/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.6/srsgui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.5
+Version: 0.2.6
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.5/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.6/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

