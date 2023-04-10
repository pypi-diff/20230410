# Comparing `tmp/srsgui-0.2.6.tar.gz` & `tmp/srsgui-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-x9_b0d6j\srsgui-0.2.6.tar", last modified: Mon Apr 10 16:31:04 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-ryn3s73s\srsgui-0.2.7.tar", last modified: Mon Apr 10 18:10:58 2023, max compression
```

## Comparing `srsgui-0.2.6.tar` & `srsgui-0.2.7.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.126513 srsgui-0.2.6/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.6/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3330 2023-04-10 16:31:04.126513 srsgui-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.026562 srsgui-0.2.6/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.046576 srsgui-0.2.6/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.6/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.6/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 16:31:04.126513 srsgui-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-04-10 16:30:05.000000 srsgui-0.2.6/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.6/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.020107 srsgui-0.2.6/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.076539 srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.086534 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.086534 srsgui-0.2.6/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.6/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9530 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.096529 srsgui-0.2.6/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10031 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.6/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.096529 srsgui-0.2.6/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.6/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.116518 srsgui-0.2.6/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.126513 srsgui-0.2.6/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.py
--rw-rw-rw-   0        0        0     3362 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.ui
--rw-rw-rw-   0        0        0     3489 2023-04-10 16:08:39.000000 srsgui-0.2.6/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     9349 2023-04-10 16:09:08.000000 srsgui-0.2.6/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     7581 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5161 2023-04-10 16:05:18.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     4071 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/ui/commandtree/jsonmodel.py
--rw-rw-rw-   0        0        0     4803 2023-04-10 15:41:31.000000 srsgui-0.2.6/srsgui/ui/commandtree/ui_commandcapturewidget.py
--rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.6/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.6/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    11682 2023-04-07 01:13:40.000000 srsgui-0.2.6/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.126513 srsgui-0.2.6/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.6/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.6/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.6/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.6/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.6/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-10 16:31:04.066545 srsgui-0.2.6/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-04-10 16:31:04.000000 srsgui-0.2.6/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 16:31:03.000000 srsgui-0.2.6/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.659996 srsgui-0.2.7/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.7/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-10 18:10:58.659996 srsgui-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.590006 srsgui-0.2.7/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.600037 srsgui-0.2.7/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.609999 srsgui-0.2.7/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.7/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.7/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 18:10:58.659996 srsgui-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.609999 srsgui-0.2.7/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-10 18:09:46.000000 srsgui-0.2.7/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.7/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.584070 srsgui-0.2.7/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.629989 srsgui-0.2.7/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.7/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9583 2023-04-10 17:21:10.000000 srsgui-0.2.7/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.629989 srsgui-0.2.7/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10031 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.7/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.640009 srsgui-0.2.7/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.7/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.649978 srsgui-0.2.7/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.659996 srsgui-0.2.7/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:57:55.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3362 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3489 2023-04-10 16:08:39.000000 srsgui-0.2.7/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0    10180 2023-04-10 18:03:49.000000 srsgui-0.2.7/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7833 2023-04-10 17:30:59.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5161 2023-04-10 16:05:18.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     4071 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 19:57:55.000000 srsgui-0.2.7/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4803 2023-04-10 15:41:31.000000 srsgui-0.2.7/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.7/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:57:55.000000 srsgui-0.2.7/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    11682 2023-04-07 01:13:40.000000 srsgui-0.2.7/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.659996 srsgui-0.2.7/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.7/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.7/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-10 15:41:10.000000 srsgui-0.2.7/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.7/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.7/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:10:58.619994 srsgui-0.2.7/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 18:10:58.000000 srsgui-0.2.7/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.6/.gitignore` & `srsgui-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/LICENSE.txt` & `srsgui-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/PKG-INFO` & `srsgui-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.6
+Version: 0.2.7
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.6/README.md` & `srsgui-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/Makefile` & `srsgui-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/make.bat` & `srsgui-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.7/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.7/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.7/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.7/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.7/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.7/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.7/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.7/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.7/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.7/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/conf.py` & `srsgui-0.2.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/create-project.rst` & `srsgui-0.2.7/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/create-task.rst` & `srsgui-0.2.7/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/define-instrument.rst` & `srsgui-0.2.7/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/example.rst` & `srsgui-0.2.7/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/index.rst` & `srsgui-0.2.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/installation.rst` & `srsgui-0.2.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.7/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/srsgui.inst.rst` & `srsgui-0.2.7/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/srsgui.task.rst` & `srsgui-0.2.7/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.7/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/docs/source/srsgui.ui.rst` & `srsgui-0.2.7/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/pyproject.toml` & `srsgui-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/__init__.py` & `srsgui-0.2.7/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.6"  # Global version number
+__version__ = "0.2.7"  # Global version number
```

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.7/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/__init__.py` & `srsgui-0.2.7/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/commands.py` & `srsgui-0.2.7/srsgui/inst/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,16 @@
         self._get_convert_function = None
         self._set_convert_function = None
 
         self._value = ''
         self.default_value = default_value
         if default_value:
             self._value = default_value
-        self.fmt = '{}'  # format for string conversion
+        self.fmt = ''  # format for string conversion
+                       # '.3f' , '10.3e', 's', 'd', 'x'
 
     def __get__(self, instance, instance_type):
         if instance is None:
             return self
         query_string = self._get_command_format.format(self.remote_command)
         reply = None
         try:
@@ -254,15 +255,15 @@
 
 class DictCommand(Command):
     """
     Descriptor for a remote command to
     **set** and **query** using a conversion dictionary
     """
 
-    def __init__(self, remote_command_name, set_dict, get_dict=None, unit='', fmt='{}', default_value=None):
+    def __init__(self, remote_command_name, set_dict, get_dict=None, unit='', fmt='', default_value=None):
         super().__init__(remote_command_name, default_value)
         if type(set_dict) is not dict:
             raise TypeError('set_dict must be a dictionary')
         if get_dict is not None and type(get_dict) is not dict:
             raise TypeError('get_dict must be a dictionary')
 
         self.set_dict = set_dict
```

### Comparing `srsgui-0.2.6/srsgui/inst/communications/interface.py` & `srsgui-0.2.7/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.7/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.7/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.7/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/component.py` & `srsgui-0.2.7/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/exceptions.py` & `srsgui-0.2.7/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/indexcommands.py` & `srsgui-0.2.7/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/inst/instrument.py` & `srsgui-0.2.7/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/task/callbacks.py` & `srsgui-0.2.7/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/task/config.py` & `srsgui-0.2.7/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/task/inputs.py` & `srsgui-0.2.7/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/task/sessionhandler.py` & `srsgui-0.2.7/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/task/task.py` & `srsgui-0.2.7/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/task/taskresult.py` & `srsgui-0.2.7/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandhandler.py` & `srsgui-0.2.7/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandterminal.py` & `srsgui-0.2.7/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.py` & `srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commandcapturewidget.ui` & `srsgui-0.2.7/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.2.7/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.2.7/srsgui/ui/commandtree/commanditem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,585 +1,637 @@
 00000000: 0d0a 696d 706f 7274 2074 696d 650d 0a66  ..import time..f
 00000010: 726f 6d20 7372 7367 7569 2069 6d70 6f72  rom srsgui impor
 00000020: 7420 436f 6d70 6f6e 656e 740d 0a66 726f  t Component..fro
 00000030: 6d20 7372 7367 7569 2e69 6e73 7420 696d  m srsgui.inst im
 00000040: 706f 7274 2043 6f6d 6d61 6e64 2c20 496e  port Command, In
-00000050: 6465 7843 6f6d 6d61 6e64 0d0a 0d0a 0d0a  dexCommand......
-00000060: 636c 6173 7320 496e 6465 783a 0d0a 2020  class Index:..  
-00000070: 2020 7061 7373 0d0a 0d0a 0d0a 636c 6173    pass......clas
-00000080: 7320 436f 6d6d 616e 6449 7465 6d3a 0d0a  s CommandItem:..
-00000090: 2020 2020 2222 2241 2043 6f6d 6d61 6e64      """A Command
-000000a0: 2069 7465 6d20 636f 7272 6573 706f 6e64   item correspond
-000000b0: 696e 6720 746f 2061 206c 696e 6520 696e  ing to a line in
-000000c0: 2051 5472 6565 5669 6577 2222 220d 0a0d   QTreeView"""...
-000000d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000000e0: 5f28 7365 6c66 2c20 7061 7265 6e74 3a20  _(self, parent: 
-000000f0: 2243 6f6d 6d61 6e64 4974 656d 2220 3d20  "CommandItem" = 
-00000100: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-00000110: 7365 6c66 2e5f 7061 7265 6e74 203d 2070  self._parent = p
-00000120: 6172 656e 740d 0a20 2020 2020 2020 2073  arent..        s
-00000130: 656c 662e 5f63 6869 6c64 7265 6e20 3d20  elf._children = 
-00000140: 5b5d 0d0a 2020 2020 2020 2020 7365 6c66  []..        self
-00000150: 2e5f 7661 6c75 6520 3d20 4e6f 6e65 0d0a  ._value = None..
-00000160: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000170: 2020 7365 6c66 2e6e 616d 6520 3d20 2222    self.name = ""
-00000180: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
-00000190: 616c 7565 5f74 7970 6520 3d20 4e6f 6e65  alue_type = None
-000001a0: 2020 2320 5468 6572 6520 6172 6520 3320    # There are 3 
-000001b0: 7479 7065 7320 6f66 2076 616c 7565 733a  types of values:
-000001c0: 2073 7472 2c20 696e 742c 2061 6e64 2066   str, int, and f
-000001d0: 6c6f 6174 0d0a 2020 2020 2020 2020 7365  loat..        se
-000001e0: 6c66 2e70 7265 6369 7369 6f6e 203d 2034  lf.precision = 4
-000001f0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00000200: 2020 2020 7365 6c66 2e63 6f6d 7020 3d20      self.comp = 
-00000210: 4e6f 6e65 0d0a 2020 2020 2020 2020 7365  None..        se
-00000220: 6c66 2e63 6f6d 705f 7479 7065 203d 204e  lf.comp_type = N
-00000230: 6f6e 6520 2020 2320 5468 6572 6520 6172  one   # There ar
-00000240: 6520 3520 7479 7065 7320 6f66 2063 6f6d  e 5 types of com
-00000250: 706f 6e65 6e74 733a 2043 6f6d 706f 6e65  ponents: Compone
-00000260: 6e74 2c20 436f 6d6d 616e 6473 2c20 496e  nt, Commands, In
-00000270: 6465 7843 6f6d 6d61 6e64 732c 206d 6574  dexCommands, met
-00000280: 686f 6420 616e 6420 496e 6465 780d 0a20  hod and Index.. 
-00000290: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-000002a0: 656e 6162 6c65 203d 2046 616c 7365 0d0a  enable = False..
-000002b0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-000002c0: 5f65 6e61 626c 6520 3d20 4661 6c73 650d  _enable = False.
-000002d0: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
-000002e0: 5f6d 6574 686f 6420 3d20 4661 6c73 650d  _method = False.
-000002f0: 0a20 2020 2020 2020 2073 656c 662e 6578  .        self.ex
-00000300: 636c 7564 6564 203d 2046 616c 7365 0d0a  cluded = False..
-00000310: 2020 2020 2020 2020 7365 6c66 2e72 6177          self.raw
-00000320: 5f72 656d 6f74 655f 636f 6d6d 616e 6420  _remote_command 
-00000330: 3d20 2222 0d0a 2020 2020 2020 2020 7365  = ""..        se
-00000340: 6c66 2e74 696d 6573 7461 6d70 203d 2030  lf.timestamp = 0
-00000350: 2e30 0d0a 0d0a 2020 2020 6465 6620 6170  .0....    def ap
-00000360: 7065 6e64 4368 696c 6428 7365 6c66 2c20  pendChild(self, 
-00000370: 6974 656d 3a20 2243 6f6d 6d61 6e64 4974  item: "CommandIt
-00000380: 656d 2229 3a0d 0a20 2020 2020 2020 2022  em"):..        "
-00000390: 2222 4164 6420 6974 656d 2061 7320 6120  ""Add item as a 
-000003a0: 6368 696c 6422 2222 0d0a 2020 2020 2020  child"""..      
-000003b0: 2020 7365 6c66 2e5f 6368 696c 6472 656e    self._children
-000003c0: 2e61 7070 656e 6428 6974 656d 290d 0a0d  .append(item)...
-000003d0: 0a20 2020 2064 6566 2063 6869 6c64 2873  .    def child(s
-000003e0: 656c 662c 2072 6f77 3a20 696e 7429 202d  elf, row: int) -
-000003f0: 3e20 2243 6f6d 6d61 6e64 4974 656d 223a  > "CommandItem":
-00000400: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
-00000410: 7572 6e20 7468 6520 6368 696c 6420 6f66  urn the child of
-00000420: 2074 6865 2063 7572 7265 6e74 2069 7465   the current ite
-00000430: 6d20 6672 6f6d 2074 6865 2067 6976 656e  m from the given
-00000440: 2072 6f77 2222 220d 0a20 2020 2020 2020   row"""..       
-00000450: 2072 6574 7572 6e20 7365 6c66 2e5f 6368   return self._ch
-00000460: 696c 6472 656e 5b72 6f77 5d0d 0a0d 0a20  ildren[row].... 
-00000470: 2020 2064 6566 2070 6172 656e 7428 7365     def parent(se
-00000480: 6c66 2920 2d3e 2022 436f 6d6d 616e 6449  lf) -> "CommandI
-00000490: 7465 6d22 3a0d 0a20 2020 2020 2020 2022  tem":..        "
-000004a0: 2222 5265 7475 726e 2074 6865 2070 6172  ""Return the par
-000004b0: 656e 7420 6f66 2074 6865 2063 7572 7265  ent of the curre
-000004c0: 6e74 2069 7465 6d22 2222 0d0a 2020 2020  nt item"""..    
-000004d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000004e0: 5f70 6172 656e 740d 0a0d 0a20 2020 2064  _parent....    d
-000004f0: 6566 2063 6869 6c64 436f 756e 7428 7365  ef childCount(se
-00000500: 6c66 2920 2d3e 2069 6e74 3a0d 0a20 2020  lf) -> int:..   
-00000510: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
-00000520: 6865 206e 756d 6265 7220 6f66 2063 6869  he number of chi
-00000530: 6c64 7265 6e20 6f66 2074 6865 2063 7572  ldren of the cur
-00000540: 7265 6e74 2069 7465 6d22 2222 0d0a 2020  rent item"""..  
-00000550: 2020 2020 2020 7265 7475 726e 206c 656e        return len
-00000560: 2873 656c 662e 5f63 6869 6c64 7265 6e29  (self._children)
-00000570: 0d0a 0d0a 2020 2020 6465 6620 726f 7728  ....    def row(
-00000580: 7365 6c66 2920 2d3e 2069 6e74 3a0d 0a20  self) -> int:.. 
-00000590: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-000005a0: 2074 6865 2072 6f77 2077 6865 7265 2074   the row where t
-000005b0: 6865 2063 7572 7265 6e74 2069 7465 6d20  he current item 
-000005c0: 6f63 6375 7069 6573 2069 6e20 7468 6520  occupies in the 
-000005d0: 7061 7265 6e74 2222 220d 0a20 2020 2020  parent"""..     
-000005e0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000005f0: 7061 7265 6e74 2e5f 6368 696c 6472 656e  parent._children
-00000600: 2e69 6e64 6578 2873 656c 6629 2069 6620  .index(self) if 
-00000610: 7365 6c66 2e5f 7061 7265 6e74 2065 6c73  self._parent els
-00000620: 6520 300d 0a0d 0a20 2020 2040 7072 6f70  e 0....    @prop
-00000630: 6572 7479 0d0a 2020 2020 6465 6620 7661  erty..    def va
-00000640: 6c75 6528 7365 6c66 293a 0d0a 2020 2020  lue(self):..    
-00000650: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-00000660: 6520 7661 6c75 6520 6f66 2074 6865 2063  e value of the c
-00000670: 7572 7265 6e74 2069 7465 6d22 2222 0d0a  urrent item"""..
-00000680: 2020 2020 2020 2020 7473 203d 2074 696d          ts = tim
-00000690: 652e 7469 6d65 2829 0d0a 2020 2020 2020  e.time()..      
-000006a0: 2020 6966 2074 7320 2d20 7365 6c66 2e74    if ts - self.t
-000006b0: 696d 6573 7461 6d70 203c 2030 2e31 3a20  imestamp < 0.1: 
-000006c0: 2320 5570 6461 7465 2076 616c 7565 206c  # Update value l
-000006d0: 6174 6572 2074 6861 6e20 302e 3120 730d  ater than 0.1 s.
-000006e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000006f0: 7572 6e20 7365 6c66 2e5f 7661 6c75 650d  urn self._value.
-00000700: 0a0d 0a20 2020 2020 2020 2069 6620 7365  ...        if se
-00000710: 6c66 2e63 6f6d 705f 7479 7065 203d 3d20  lf.comp_type == 
-00000720: 496e 6465 7820 616e 6420 7365 6c66 2e67  Index and self.g
-00000730: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
-00000740: 7420 7365 6c66 2e65 7863 6c75 6465 643a  t self.excluded:
-00000750: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00000760: 6c66 2e5f 7661 6c75 6520 3d20 7365 6c66  lf._value = self
-00000770: 2e5f 7061 7265 6e74 2e63 6f6d 702e 5f5f  ._parent.comp.__
-00000780: 6765 7469 7465 6d5f 5f28 7365 6c66 2e63  getitem__(self.c
-00000790: 6f6d 7029 0d0a 2020 2020 2020 2020 2020  omp)..          
-000007a0: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
-000007b0: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
-000007c0: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
-000007d0: 2020 2020 7365 6c66 2e74 696d 6573 7461      self.timesta
-000007e0: 6d70 203d 2074 730d 0a20 2020 2020 2020  mp = ts..       
-000007f0: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
-00000800: 2874 7970 6528 7365 6c66 2e63 6f6d 7029  (type(self.comp)
-00000810: 2c20 436f 6d6d 616e 6429 2061 6e64 2073  , Command) and s
-00000820: 656c 662e 6765 745f 656e 6162 6c65 2061  elf.get_enable a
-00000830: 6e64 206e 6f74 2073 656c 662e 6578 636c  nd not self.excl
-00000840: 7564 6564 3a0d 0a20 2020 2020 2020 2020  uded:..         
-00000850: 2020 2073 656c 662e 5f76 616c 7565 203d     self._value =
-00000860: 2073 656c 662e 636f 6d70 2e5f 5f67 6574   self.comp.__get
-00000870: 5f5f 2873 656c 662e 5f70 6172 656e 742e  __(self._parent.
-00000880: 636f 6d70 2c20 7365 6c66 2e5f 7061 7265  comp, self._pare
-00000890: 6e74 2e63 6f6d 702e 5f5f 636c 6173 735f  nt.comp.__class_
-000008a0: 5f29 0d0a 2020 2020 2020 2020 2020 2020  _)..            
-000008b0: 7365 6c66 2e5f 7661 6c75 655f 7479 7065  self._value_type
-000008c0: 203d 2074 7970 6528 7365 6c66 2e5f 7661   = type(self._va
-000008d0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
-000008e0: 2020 7365 6c66 2e74 696d 6573 7461 6d70    self.timestamp
-000008f0: 203d 2074 730d 0a20 2020 2020 2020 2065   = ts..        e
-00000900: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00000910: 2020 7365 6c66 2e5f 7661 6c75 655f 7479    self._value_ty
-00000920: 7065 203d 2074 7970 6528 7365 6c66 2e5f  pe = type(self._
-00000930: 7661 6c75 6529 0d0a 2020 2020 2020 2020  value)..        
-00000940: 6966 2073 656c 662e 5f76 616c 7565 5f74  if self._value_t
-00000950: 7970 6520 3d3d 2066 6c6f 6174 3a0d 0a20  ype == float:.. 
-00000960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000970: 5f76 616c 7565 203d 2072 6f75 6e64 2873  _value = round(s
-00000980: 656c 662e 5f76 616c 7565 2c20 7365 6c66  elf._value, self
-00000990: 2e70 7265 6369 7369 6f6e 290d 0a0d 0a20  .precision).... 
-000009a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000009b0: 6c66 2e5f 7661 6c75 650d 0a0d 0a20 2020  lf._value....   
-000009c0: 2040 7661 6c75 652e 7365 7474 6572 0d0a   @value.setter..
-000009d0: 2020 2020 6465 6620 7661 6c75 6528 7365      def value(se
-000009e0: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
-000009f0: 2020 2020 2073 656c 662e 5f76 616c 7565       self._value
-00000a00: 203d 2076 616c 7565 0d0a 0d0a 2020 2020   = value....    
-00000a10: 6465 6620 7365 745f 7661 6c75 6528 7365  def set_value(se
-00000a20: 6c66 2c20 7661 6c75 6529 3a0d 0a20 2020  lf, value):..   
-00000a30: 2020 2020 2022 2222 5365 7420 7661 6c75       """Set valu
-00000a40: 6520 746f 2074 6865 2069 6e73 7472 756d  e to the instrum
-00000a50: 656e 7420 616e 6420 7570 6461 7465 2074  ent and update t
-00000a60: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00000a70: 6974 656d 2222 220d 0a20 2020 2020 2020  item"""..       
-00000a80: 2069 6620 7365 6c66 2e63 6f6d 705f 7479   if self.comp_ty
-00000a90: 7065 203d 3d20 496e 6465 783a 0d0a 2020  pe == Index:..  
-00000aa0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00000ab0: 7061 7265 6e74 2e63 6f6d 702e 5f5f 7365  parent.comp.__se
-00000ac0: 7469 7465 6d5f 5f28 7365 6c66 2e63 6f6d  titem__(self.com
-00000ad0: 702c 2076 616c 7565 290d 0a20 2020 2020  p, value)..     
-00000ae0: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
-00000af0: 7565 203d 2073 656c 662e 5f70 6172 656e  ue = self._paren
-00000b00: 742e 636f 6d70 2e5f 5f67 6574 6974 656d  t.comp.__getitem
-00000b10: 5f5f 2873 656c 662e 636f 6d70 290d 0a20  __(self.comp).. 
-00000b20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000b30: 7469 6d65 7374 616d 7020 3d20 7469 6d65  timestamp = time
-00000b40: 2e74 696d 6528 290d 0a20 2020 2020 2020  .time()..       
-00000b50: 2065 6c69 6620 6973 7375 6263 6c61 7373   elif issubclass
-00000b60: 2874 7970 6528 7365 6c66 2e63 6f6d 7029  (type(self.comp)
-00000b70: 2c20 436f 6d6d 616e 6429 3a0d 0a20 2020  , Command):..   
-00000b80: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00000b90: 6d70 2e5f 5f73 6574 5f5f 2873 656c 662e  mp.__set__(self.
-00000ba0: 5f70 6172 656e 742e 636f 6d70 2c20 7661  _parent.comp, va
-00000bb0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
-00000bc0: 2020 7365 6c66 2e5f 7661 6c75 6520 3d20    self._value = 
-00000bd0: 7365 6c66 2e63 6f6d 702e 5f5f 6765 745f  self.comp.__get_
-00000be0: 5f28 7365 6c66 2e5f 7061 7265 6e74 2e63  _(self._parent.c
-00000bf0: 6f6d 702c 2073 656c 662e 5f70 6172 656e  omp, self._paren
-00000c00: 742e 636f 6d70 2e5f 5f63 6c61 7373 5f5f  t.comp.__class__
-00000c10: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00000c20: 656c 662e 7469 6d65 7374 616d 7020 3d20  elf.timestamp = 
-00000c30: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00000c40: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000c50: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00000c60: 6c75 6520 3d20 7661 6c75 650d 0a0d 0a20  lue = value.... 
-00000c70: 2020 2064 6566 2069 735f 6564 6974 6162     def is_editab
-00000c80: 6c65 2873 656c 6629 3a0d 0a20 2020 2020  le(self):..     
-00000c90: 2020 2022 2222 5265 7475 726e 2054 7275     """Return Tru
-00000ca0: 6520 6966 2074 6865 2069 7465 6d20 6973  e if the item is
-00000cb0: 2065 6469 7461 626c 6522 2222 0d0a 2020   editable"""..  
-00000cc0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00000cd0: 6d70 5f74 7970 6520 3d3d 2049 6e64 6578  mp_type == Index
-00000ce0: 2061 6e64 205c 0d0a 2020 2020 2020 2020   and \..        
-00000cf0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00000d00: 5f65 6e61 626c 6520 616e 6420 7365 6c66  _enable and self
-00000d10: 2e67 6574 5f65 6e61 626c 6520 616e 6420  .get_enable and 
-00000d20: 6e6f 7420 7365 6c66 2e65 7863 6c75 6465  not self.exclude
-00000d30: 643a 0d0a 2020 2020 2020 2020 2020 2020  d:..            
-00000d40: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00000d50: 2020 2020 2065 6c69 6620 6973 7375 6263       elif issubc
-00000d60: 6c61 7373 2874 7970 6528 7365 6c66 2e63  lass(type(self.c
-00000d70: 6f6d 7029 2c20 436f 6d6d 616e 6429 2061  omp), Command) a
-00000d80: 6e64 205c 0d0a 2020 2020 2020 2020 2020  nd \..          
-00000d90: 2020 2020 2020 7365 6c66 2e73 6574 5f65        self.set_e
-00000da0: 6e61 626c 6520 616e 6420 7365 6c66 2e67  nable and self.g
-00000db0: 6574 5f65 6e61 626c 6520 616e 6420 6e6f  et_enable and no
-00000dc0: 7420 7365 6c66 2e65 7863 6c75 6465 643a  t self.excluded:
-00000dd0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00000de0: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00000df0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00000e00: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00000e10: 7365 0d0a 0d0a 2020 2020 6465 6620 6765  se....    def ge
-00000e20: 745f 756e 6974 2873 656c 6629 3a0d 0a20  t_unit(self):.. 
-00000e30: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00000e40: 2074 6865 2075 6e69 7420 6f66 2074 6865   the unit of the
-00000e50: 2069 7465 6d22 2222 0d0a 2020 2020 2020   item"""..      
-00000e60: 2020 636f 6d70 203d 204e 6f6e 650d 0a20    comp = None.. 
-00000e70: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00000e80: 6f6d 705f 7479 7065 203d 3d20 496e 6465  omp_type == Inde
-00000e90: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
-00000ea0: 636f 6d70 203d 2073 656c 662e 7061 7265  comp = self.pare
-00000eb0: 6e74 2829 2e63 6f6d 700d 0a20 2020 2020  nt().comp..     
-00000ec0: 2020 2065 6c69 6620 6973 7375 6263 6c61     elif issubcla
-00000ed0: 7373 2874 7970 6528 7365 6c66 2e63 6f6d  ss(type(self.com
-00000ee0: 7029 2c20 436f 6d6d 616e 6429 206f 7220  p), Command) or 
-00000ef0: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-00000f00: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
-00000f10: 7365 6c66 2e63 6f6d 7029 2c20 496e 6465  self.comp), Inde
-00000f20: 7843 6f6d 6d61 6e64 293a 0d0a 2020 2020  xCommand):..    
-00000f30: 2020 2020 2020 2020 636f 6d70 203d 2073          comp = s
-00000f40: 656c 662e 636f 6d70 0d0a 0d0a 2020 2020  elf.comp....    
-00000f50: 2020 2020 6966 2063 6f6d 7020 616e 6420      if comp and 
-00000f60: 6861 7361 7474 7228 636f 6d70 2c20 2775  hasattr(comp, 'u
-00000f70: 6e69 7427 293a 0d0a 2020 2020 2020 2020  nit'):..        
-00000f80: 2020 2020 7265 7475 726e 2063 6f6d 702e      return comp.
-00000f90: 756e 6974 0d0a 2020 2020 2020 2020 656c  unit..        el
-00000fa0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00000fb0: 2072 6574 7572 6e20 2222 0d0a 0d0a 2020   return ""....  
-00000fc0: 2020 4063 6c61 7373 6d65 7468 6f64 0d0a    @classmethod..
-00000fd0: 2020 2020 6465 6620 6c6f 6164 280d 0a20      def load(.. 
-00000fe0: 2020 2020 2020 2063 6c73 2c20 636f 6d70         cls, comp
-00000ff0: 2c20 7061 7265 6e74 3a20 2243 6f6d 6d61  , parent: "Comma
-00001000: 6e64 4974 656d 2220 3d20 4e6f 6e65 2c20  ndItem" = None, 
-00001010: 736f 7274 3d46 616c 7365 0d0a 2020 2020  sort=False..    
-00001020: 2920 2d3e 2022 436f 6d6d 616e 6449 7465  ) -> "CommandIte
-00001030: 6d22 3a0d 0a20 2020 2020 2020 2022 2222  m":..        """
-00001040: 4372 6561 7465 2061 2027 726f 6f74 2720  Create a 'root' 
-00001050: 436f 6d6d 616e 6449 7465 6d20 6672 6f6d  CommandItem from
-00001060: 2061 2043 6f6d 706f 6e65 6e74 2061 6e64   a Component and
-00001070: 200d 0a20 2020 2020 2020 2070 6f70 756c   ..        popul
-00001080: 6174 6520 6974 7320 7375 6263 6f6d 706f  ate its subcompo
-00001090: 6e65 6e74 2061 6e64 2063 6f6d 6d61 6e64  nent and command
-000010a0: 7320 7265 6375 7273 6976 656c 792e 0d0a  s recursively...
-000010b0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000010c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000010d0: 436f 6d6d 616e 6449 7465 6d3a 2043 6f6d  CommandItem: Com
-000010e0: 6d61 6e64 4974 656d 0d0a 2020 2020 2020  mandItem..      
-000010f0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00001100: 6f6f 745f 6974 656d 203d 2043 6f6d 6d61  oot_item = Comma
-00001110: 6e64 4974 656d 2870 6172 656e 7429 0d0a  ndItem(parent)..
-00001120: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00001130: 6d2e 6e61 6d65 203d 2022 726f 6f74 220d  m.name = "root".
-00001140: 0a20 2020 2020 2020 2072 6f6f 745f 6974  .        root_it
-00001150: 656d 2e63 6f6d 7020 3d20 636f 6d70 0d0a  em.comp = comp..
-00001160: 0d0a 2020 2020 2020 2020 6966 2069 7373  ..        if iss
-00001170: 7562 636c 6173 7328 636f 6d70 2e5f 5f63  ubclass(comp.__c
-00001180: 6c61 7373 5f5f 2c20 436f 6d70 6f6e 656e  lass__, Componen
-00001190: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
-000011a0: 2066 6f72 206a 2069 6e20 636f 6d70 2e5f   for j in comp._
-000011b0: 5f64 6963 745f 5f3a 0d0a 2020 2020 2020  _dict__:..      
-000011c0: 2020 2020 2020 2020 2020 6966 206a 203d            if j =
-000011d0: 3d20 275f 7061 7265 6e74 273a 0d0a 2020  = '_parent':..  
-000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011f0: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-00001200: 2020 2020 2020 2020 2020 2020 696e 7374              inst
-00001210: 616e 6365 203d 2063 6f6d 702e 5f5f 6469  ance = comp.__di
-00001220: 6374 5f5f 5b6a 5d0d 0a20 2020 2020 2020  ct__[j]..       
-00001230: 2020 2020 2020 2020 2069 6620 6973 7375           if issu
-00001240: 6263 6c61 7373 2869 6e73 7461 6e63 652e  bclass(instance.
-00001250: 5f5f 636c 6173 735f 5f2c 2020 436f 6d70  __class__,  Comp
-00001260: 6f6e 656e 7429 3a20 2020 2020 2020 2020  onent):         
-00001270: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001280: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00001290: 6c64 203d 2063 6c73 2e6c 6f61 6428 696e  ld = cls.load(in
-000012a0: 7374 616e 6365 2c20 726f 6f74 5f69 7465  stance, root_ite
-000012b0: 6d2c 2073 6f72 7429 0d0a 2020 2020 2020  m, sort)..      
-000012c0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-000012d0: 696c 642e 6e61 6d65 203d 206a 0d0a 2020  ild.name = j..  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 6368 696c 642e 636f 6d70 203d 2069    child.comp = i
-00001300: 6e73 7461 6e63 650d 0a20 2020 2020 2020  nstance..       
-00001310: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001320: 696e 7374 616e 6365 2069 6e20 636f 6d70  instance in comp
-00001330: 2e65 7863 6c75 6465 5f63 6170 7475 7265  .exclude_capture
-00001340: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001350: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00001360: 2e65 7863 6c75 6465 6420 3d20 5472 7565  .excluded = True
-00001370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001380: 2020 2020 2020 6368 696c 642e 636f 6d70        child.comp
-00001390: 5f74 7970 6520 3d20 7479 7065 2869 6e73  _type = type(ins
-000013a0: 7461 6e63 6529 0d0a 2020 2020 2020 2020  tance)..        
-000013b0: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-000013c0: 5f69 7465 6d2e 6170 7065 6e64 4368 696c  _item.appendChil
-000013d0: 6428 6368 696c 6429 0d0a 0d0a 2020 2020  d(child)....    
-000013e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000013f0: 6174 7472 6962 7574 6573 203d 205b 5d0d  attributes = [].
-00001400: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00001410: 2063 2069 6e20 636f 6d70 2e5f 5f63 6c61   c in comp.__cla
-00001420: 7373 5f5f 2e5f 5f6d 726f 5f5f 3a20 2023  ss__.__mro__:  #
-00001430: 206c 6f6f 7020 7468 726f 7567 6820 7468   loop through th
-00001440: 6520 636c 6173 7365 7320 696e 636c 7564  e classes includ
-00001450: 696e 6720 7375 7065 7220 636c 6173 7365  ing super classe
-00001460: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00001470: 2020 2069 6620 6e6f 7420 6973 7375 6263     if not issubc
-00001480: 6c61 7373 2863 2c20 436f 6d70 6f6e 656e  lass(c, Componen
-00001490: 7429 3a20 2023 2069 7420 7368 6f75 6c64  t):  # it should
-000014a0: 2062 6520 6120 7375 6263 6c61 7373 206f   be a subclass o
-000014b0: 6620 436f 6d70 6f6e 656e 740d 0a20 2020  f Component..   
-000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014d0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
-000014e0: 2020 2020 2020 2020 6966 2063 203d 3d20          if c == 
-000014f0: 436f 6d70 6f6e 656e 743a 2020 2320 4275  Component:  # Bu
-00001500: 7420 6974 2073 686f 756c 6420 6e6f 7420  t it should not 
-00001510: 6265 2043 6f6d 706f 6e65 6e74 0d0a 2020  be Component..  
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
 00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001530: 2020 6272 6561 6b0d 0a0d 0a20 2020 2020    break....     
-00001540: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00001550: 6579 2069 6e20 632e 5f5f 6469 6374 5f5f  ey in c.__dict__
-00001560: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001570: 2020 2020 2020 2063 6d64 5f69 6e73 7461         cmd_insta
-00001580: 6e63 6520 3d20 632e 5f5f 6469 6374 5f5f  nce = c.__dict__
-00001590: 5b6b 6579 5d0d 0a20 2020 2020 2020 2020  [key]..         
-000015a0: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
-000015b0: 7920 696e 2063 7572 7265 6e74 5f61 7474  y in current_att
-000015c0: 7269 6275 7465 733a 0d0a 2020 2020 2020  ributes:..      
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 6375 7272 656e 745f 6174 7472 6962 7574  current_attribut
-00001610: 6573 2e61 7070 656e 6428 6b65 7929 0d0a  es.append(key)..
-00001620: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001630: 2020 2020 2020 6966 2069 7373 7562 636c        if issubcl
-00001640: 6173 7328 636d 645f 696e 7374 616e 6365  ass(cmd_instance
-00001650: 2e5f 5f63 6c61 7373 5f5f 2c20 436f 6d6d  .__class__, Comm
-00001660: 616e 6429 3a0d 0a20 2020 2020 2020 2020  and):..         
-00001670: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001680: 6869 6c64 203d 2063 6c73 2e6c 6f61 6428  hild = cls.load(
-00001690: 636d 645f 696e 7374 616e 6365 2c20 726f  cmd_instance, ro
-000016a0: 6f74 5f69 7465 6d2c 2073 6f72 7429 0d0a  ot_item, sort)..
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2020 2020 2020 2020 6368 696c 642e 6e61          child.na
-000016d0: 6d65 203d 206b 6579 0d0a 2020 2020 2020  me = key..      
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 6368 696c 642e 636f 6d70 203d 2063    child.comp = c
-00001700: 6d64 5f69 6e73 7461 6e63 650d 0a20 2020  md_instance..   
-00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 2063 6869 6c64 2e63 6f6d 705f       child.comp_
-00001730: 7479 7065 203d 2074 7970 6528 636d 645f  type = type(cmd_
-00001740: 696e 7374 616e 6365 290d 0a0d 0a20 2020  instance)....   
-00001750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001760: 2020 2020 2072 6f6f 745f 6974 656d 2e61       root_item.a
-00001770: 7070 656e 6443 6869 6c64 2863 6869 6c64  ppendChild(child
-00001780: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00001790: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
-000017a0: 7375 6263 6c61 7373 2863 6d64 5f69 6e73  subclass(cmd_ins
-000017b0: 7461 6e63 652e 5f5f 636c 6173 735f 5f2c  tance.__class__,
-000017c0: 2049 6e64 6578 436f 6d6d 616e 6429 3a0d   IndexCommand):.
-000017d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000017e0: 2020 2020 2020 2020 2063 6869 6c64 203d           child =
-000017f0: 2063 6c73 2e6c 6f61 6428 636d 645f 696e   cls.load(cmd_in
-00001800: 7374 616e 6365 2c20 726f 6f74 5f69 7465  stance, root_ite
-00001810: 6d2c 2073 6f72 7429 0d0a 2020 2020 2020  m, sort)..      
-00001820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001830: 2020 6368 696c 642e 6e61 6d65 203d 206b    child.name = k
-00001840: 6579 0d0a 2020 2020 2020 2020 2020 2020  ey..            
-00001850: 2020 2020 2020 2020 2020 2020 6368 696c              chil
-00001860: 642e 636f 6d70 203d 2063 6d64 5f69 6e73  d.comp = cmd_ins
-00001870: 7461 6e63 650d 0a20 2020 2020 2020 2020  tance..         
-00001880: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001890: 6869 6c64 2e63 6f6d 705f 7479 7065 203d  hild.comp_type =
-000018a0: 2074 7970 6528 636d 645f 696e 7374 616e   type(cmd_instan
-000018b0: 6365 290d 0a20 2020 2020 2020 2020 2020  ce)..           
-000018c0: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-000018d0: 745f 6974 656d 2e61 7070 656e 6443 6869  t_item.appendChi
-000018e0: 6c64 2863 6869 6c64 290d 0a0d 0a20 2020  ld(child)....   
-000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001900: 2065 6c69 6620 6361 6c6c 6162 6c65 2863   elif callable(c
-00001910: 6d64 5f69 6e73 7461 6e63 6529 3a0d 0a20  md_instance):.. 
-00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 2020 2020 2020 2069 6620 6973 7375 6263         if issubc
-00001940: 6c61 7373 2863 6d64 5f69 6e73 7461 6e63  lass(cmd_instanc
-00001950: 652e 5f5f 636c 6173 735f 5f2c 2074 7970  e.__class__, typ
-00001960: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 2069 6620 6b65 792e 7374 6172 7473     if key.starts
-000019b0: 7769 7468 2827 5f27 293a 0d0a 2020 2020  with('_'):..    
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-000019e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000019f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2020 6368 696c 6420 3d20 636c 732e      child = cls.
-00001a20: 6c6f 6164 2863 6d64 5f69 6e73 7461 6e63  load(cmd_instanc
-00001a30: 652c 2072 6f6f 745f 6974 656d 2c20 736f  e, root_item, so
-00001a40: 7274 290d 0a20 2020 2020 2020 2020 2020  rt)..           
-00001a50: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00001a60: 6c64 2e6e 616d 6520 3d20 6b65 790d 0a20  ld.name = key.. 
-00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a80: 2020 2020 2020 2063 6869 6c64 2e63 6f6d         child.com
-00001a90: 7020 3d20 636d 645f 696e 7374 616e 6365  p = cmd_instance
-00001aa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ab0: 2020 2020 2020 2020 2020 6368 696c 642e            child.
-00001ac0: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
-00001ad0: 2863 6d64 5f69 6e73 7461 6e63 6529 0d0a  (cmd_instance)..
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00001b00: 6d2e 6170 7065 6e64 4368 696c 6428 6368  m.appendChild(ch
-00001b10: 696c 6429 0d0a 2020 2020 2020 2020 656c  ild)..        el
-00001b20: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00001b30: 2069 6620 6361 6c6c 6162 6c65 2863 6f6d   if callable(com
-00001b40: 7029 3a0d 0a20 2020 2020 2020 2020 2020  p):..           
-00001b50: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
-00001b60: 6f6d 7020 3d20 636f 6d70 0d0a 2020 2020  omp = comp..    
-00001b70: 2020 2020 2020 2020 2020 2020 726f 6f74              root
-00001b80: 5f69 7465 6d2e 636f 6d70 5f74 7970 6520  _item.comp_type 
-00001b90: 3d20 7479 7065 2863 6f6d 7029 0d0a 2020  = type(comp)..  
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00001bb0: 6f74 5f69 7465 6d2e 6973 5f6d 6574 686f  ot_item.is_metho
-00001bc0: 6420 3d20 5472 7565 0d0a 0d0a 2020 2020  d = True....    
-00001bd0: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
-00001be0: 7562 636c 6173 7328 7479 7065 2863 6f6d  ubclass(type(com
-00001bf0: 7029 2c20 436f 6d6d 616e 6429 3a0d 0a20  p), Command):.. 
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001c10: 6f6f 745f 6974 656d 2e63 6f6d 7020 3d20  oot_item.comp = 
-00001c20: 636f 6d70 0d0a 2020 2020 2020 2020 2020  comp..          
-00001c30: 2020 2020 2020 726f 6f74 5f69 7465 6d2e        root_item.
-00001c40: 636f 6d70 5f74 7970 6520 3d20 7479 7065  comp_type = type
-00001c50: 2863 6f6d 7029 0d0a 2020 2020 2020 2020  (comp)..        
-00001c60: 2020 2020 2020 2020 726f 6f74 5f69 7465          root_ite
-00001c70: 6d2e 6578 636c 7564 6564 203d 2063 6f6d  m.excluded = com
-00001c80: 7020 696e 2072 6f6f 745f 6974 656d 2e70  p in root_item.p
-00001c90: 6172 656e 7428 292e 636f 6d70 2e65 7863  arent().comp.exc
-00001ca0: 6c75 6465 5f63 6170 7475 7265 0d0a 2020  lude_capture..  
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00001cc0: 6f74 5f69 7465 6d2e 7261 775f 7265 6d6f  ot_item.raw_remo
-00001cd0: 7465 5f63 6f6d 6d61 6e64 203d 2063 6f6d  te_command = com
-00001ce0: 702e 7265 6d6f 7465 5f63 6f6d 6d61 6e64  p.remote_command
-00001cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001d00: 2020 726f 6f74 5f69 7465 6d2e 7365 745f    root_item.set_
-00001d10: 656e 6162 6c65 203d 2063 6f6d 702e 5f73  enable = comp._s
-00001d20: 6574 5f65 6e61 626c 650d 0a20 2020 2020  et_enable..     
-00001d30: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00001d40: 6974 656d 2e67 6574 5f65 6e61 626c 6520  item.get_enable 
-00001d50: 3d20 636f 6d70 2e5f 6765 745f 656e 6162  = comp._get_enab
-00001d60: 6c65 0d0a 0d0a 2020 2020 2020 2020 2020  le....          
-00001d70: 2020 656c 6966 2069 7373 7562 636c 6173    elif issubclas
-00001d80: 7328 7479 7065 2863 6f6d 7029 2c20 496e  s(type(comp), In
-00001d90: 6465 7843 6f6d 6d61 6e64 293a 0d0a 2020  dexCommand):..  
-00001da0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00001db0: 6f74 5f69 7465 6d2e 636f 6d70 203d 2063  ot_item.comp = c
-00001dc0: 6f6d 700d 0a20 2020 2020 2020 2020 2020  omp..           
-00001dd0: 2020 2020 2072 6f6f 745f 6974 656d 2e63       root_item.c
-00001de0: 6f6d 705f 7479 7065 203d 2074 7970 6528  omp_type = type(
-00001df0: 636f 6d70 290d 0a20 2020 2020 2020 2020  comp)..         
-00001e00: 2020 2020 2020 2072 6f6f 745f 6974 656d         root_item
-00001e10: 2e65 7863 6c75 6465 6420 3d20 636f 6d70  .excluded = comp
-00001e20: 2069 6e20 726f 6f74 5f69 7465 6d2e 7061   in root_item.pa
-00001e30: 7265 6e74 2829 2e63 6f6d 702e 6578 636c  rent().comp.excl
-00001e40: 7564 655f 6361 7074 7572 650d 0a20 2020  ude_capture..   
-00001e50: 2020 2020 2020 2020 2020 2020 2072 6f6f               roo
-00001e60: 745f 6974 656d 2e72 6177 5f72 656d 6f74  t_item.raw_remot
-00001e70: 655f 636f 6d6d 616e 6420 3d20 636f 6d70  e_command = comp
-00001e80: 2e72 656d 6f74 655f 636f 6d6d 616e 640d  .remote_command.
-00001e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ea0: 2072 6f6f 745f 6974 656d 2e73 6574 5f65   root_item.set_e
-00001eb0: 6e61 626c 6520 3d20 636f 6d70 2e5f 7365  nable = comp._se
-00001ec0: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
-00001ed0: 2020 2020 2020 2020 2020 726f 6f74 5f69            root_i
-00001ee0: 7465 6d2e 6765 745f 656e 6162 6c65 203d  tem.get_enable =
-00001ef0: 2063 6f6d 702e 5f67 6574 5f65 6e61 626c   comp._get_enabl
-00001f00: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-00001f10: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001f30: 6620 636f 6d70 2e69 6e64 6578 5f64 6963  f comp.index_dic
-00001f40: 7420 6973 204e 6f6e 653a 0d0a 2020 2020  t is None:..    
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2020 2020 696e 6465 7820 3d20 636f 6d70      index = comp
-00001f70: 2e69 6e64 6578 5f6d 696e 0d0a 2020 2020  .index_min..    
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f90: 2020 2020 7768 696c 6520 696e 6465 7820      while index 
-00001fa0: 3c3d 2063 6f6d 702e 696e 6465 785f 6d61  <= comp.index_ma
-00001fb0: 783a 0d0a 2020 2020 2020 2020 2020 2020  x:..            
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 6368 696c 6420 3d20 636c 732e 6c6f 6164  child = cls.load
-00001fe0: 2869 6e64 6578 2c20 726f 6f74 5f69 7465  (index, root_ite
-00001ff0: 6d2c 2073 6f72 7429 0d0a 2020 2020 2020  m, sort)..      
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 6368 696c 642e 6e61 6d65        child.name
-00002020: 203d 2066 277b 696e 6465 787d 270d 0a20   = f'{index}'.. 
-00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002040: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002050: 2e63 6f6d 7020 3d20 696e 6465 780d 0a20  .comp = index.. 
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 2020 2020 2063 6869 6c64             child
-00002080: 2e63 6f6d 705f 7479 7065 203d 2049 6e64  .comp_type = Ind
-00002090: 6578 0d0a 2020 2020 2020 2020 2020 2020  ex..            
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 6368 696c 642e 6578 636c 7564 6564 203d  child.excluded =
-000020c0: 2072 6f6f 745f 6974 656d 2e65 7863 6c75   root_item.exclu
-000020d0: 6465 640d 0a20 2020 2020 2020 2020 2020  ded..           
-000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020f0: 2063 6869 6c64 2e73 6574 5f65 6e61 626c   child.set_enabl
-00002100: 6520 3d20 726f 6f74 5f69 7465 6d2e 7365  e = root_item.se
-00002110: 745f 656e 6162 6c65 0d0a 2020 2020 2020  t_enable..      
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 6368 696c 642e 6765 745f        child.get_
-00002140: 656e 6162 6c65 203d 2072 6f6f 745f 6974  enable = root_it
-00002150: 656d 2e67 6574 5f65 6e61 626c 650d 0a20  em.get_enable.. 
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 2020 2020 2020 2020 2020 2072 6f6f 745f             root_
-00002180: 6974 656d 2e61 7070 656e 6443 6869 6c64  item.appendChild
-00002190: 2863 6869 6c64 290d 0a20 2020 2020 2020  (child)..       
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 2069 6e64 6578 202b 3d20 310d       index += 1.
-000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021d0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2020 2020 666f 7220 6b65 7920 696e 2063      for key in c
-00002200: 6f6d 702e 696e 6465 785f 6469 6374 3a0d  omp.index_dict:.
-00002210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002220: 2020 2020 2020 2020 2020 2020 2063 6869               chi
-00002230: 6c64 203d 2063 6c73 2e6c 6f61 6428 6b65  ld = cls.load(ke
-00002240: 792c 2072 6f6f 745f 6974 656d 2c20 736f  y, root_item, so
-00002250: 7274 290d 0a20 2020 2020 2020 2020 2020  rt)..           
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2063 6869 6c64 2e6e 616d 6520 3d20 6627   child.name = f'
-00002280: 7b6b 6579 7d27 0d0a 2020 2020 2020 2020  {key}'..        
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
 00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 6368 696c 642e 636f 6d70 203d      child.comp =
-000022b0: 206b 6579 0d0a 2020 2020 2020 2020 2020   key..          
+000022a0: 2020 2069 6e64 6578 203d 2063 6f6d 702e     index = comp.
+000022b0: 696e 6465 785f 6d69 6e0d 0a20 2020 2020  index_min..     
 000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 6368 696c 642e 636f 6d70 5f74 7970    child.comp_typ
-000022e0: 6520 3d20 496e 6465 780d 0a20 2020 2020  e = Index..     
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2063 6869 6c64 2e65 786c         child.exl
-00002310: 7564 6564 203d 2072 6f6f 745f 6974 656d  uded = root_item
-00002320: 2e65 7863 6c75 6465 640d 0a20 2020 2020  .excluded..     
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2063 6869 6c64 2e73 6574         child.set
-00002350: 5f65 6e61 626c 6520 3d20 636f 6d70 2e5f  _enable = comp._
-00002360: 7365 745f 656e 6162 6c65 0d0a 2020 2020  set_enable..    
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
 00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 2020 2020 6368 696c 642e 6765          child.ge
-00002390: 745f 656e 6162 6c65 203d 2063 6f6d 702e  t_enable = comp.
-000023a0: 5f67 6574 5f65 6e61 626c 650d 0a20 2020  _get_enable..   
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 2020 2020 2072 6f6f 745f 6974           root_it
-000023d0: 656d 2e61 7070 656e 6443 6869 6c64 2863  em.appendChild(c
-000023e0: 6869 6c64 290d 0a20 2020 2020 2020 2020  hild)..         
-000023f0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00002400: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002420: 2020 2070 7269 6e74 2866 2720 207b 7479     print(f'  {ty
-00002430: 7065 2865 297d 207b 657d 2063 6f6d 6d61  pe(e)} {e} comma
-00002440: 6e64 3a7b 636f 6d70 2e72 656d 6f74 655f  nd:{comp.remote_
-00002450: 636f 6d6d 616e 647d 2069 6e64 6578 3a20  command} index: 
-00002460: 7b69 6e64 6578 7d27 290d 0a20 2020 2020  {index}')..     
-00002470: 2020 2072 6574 7572 6e20 726f 6f74 5f69     return root_i
-00002480: 7465 6d0d 0a                             tem..
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
+00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
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

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.2.7/srsgui/ui/commandtree/commandmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,18 +81,23 @@
 
             if index.column() == 1:
                 item = index.internalPointer()
                 v = item.value
                 if v is None:
                     return
                 unit = item.get_unit()
-                if unit:
-                    val = f'{v}  {item.get_unit()}'
-                else:
-                    val = v
+                fmt = item.get_format()
+                try:
+                    if unit:
+                        val = f'{v:{fmt}}  {item.get_unit()}'
+                    else:
+                        val = f'{v:{fmt}}'
+                except ValueError:
+                    print(f'ValueError: {item.raw_remote_command} {v} {fmt} {unit}')
+                    val = f'{v}'
                 return val
 
         elif role == Qt.EditRole:
             if index.column() == 1:
                 item = index.internalPointer()
                 val = item.value
                 # print('data', item.name, item.comp, val)
```

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.2.7/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.2.7/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/jsonmodel.py` & `srsgui-0.2.7/srsgui/ui/commandtree/jsonmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/commandtree/ui_commandcapturewidget.py` & `srsgui-0.2.7/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/connectdlg.py` & `srsgui-0.2.7/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.7/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/dockhandler.py` & `srsgui-0.2.7/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/inputpanel.py` & `srsgui-0.2.7/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.7/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.7/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.7/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/qt/__init__.py` & `srsgui-0.2.7/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/qtloghandler.py` & `srsgui-0.2.7/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/resource_rc.py` & `srsgui-0.2.7/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/signalhandler.py` & `srsgui-0.2.7/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/srslogo.jpg` & `srsgui-0.2.7/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/stdout.py` & `srsgui-0.2.7/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/taskmain.py` & `srsgui-0.2.7/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/taskmain.ui` & `srsgui-0.2.7/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.7/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.6/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.7/srsgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.6
+Version: 0.2.7
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.6/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.7/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

