# Comparing `tmp/srsgui-0.2.4.tar.gz` & `tmp/srsgui-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-_k8aottr\srsgui-0.2.4.tar", last modified: Fri Apr  7 00:52:28 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-oo971myr\srsgui-0.2.5.tar", last modified: Fri Apr  7 19:48:06 2023, max compression
```

## Comparing `srsgui-0.2.4.tar` & `srsgui-0.2.5.tar`

### file list

```diff
@@ -1,107 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.599757 srsgui-0.2.4/
--rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.4/.gitignore
--rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3330 2023-04-07 00:52:28.599757 srsgui-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.539788 srsgui-0.2.4/docs/
--rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/Makefile
--rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/autodoc.bat
--rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.549784 srsgui-0.2.4/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.559806 srsgui-0.2.4/docs/source/_static/
--rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/conf.py
--rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.4/docs/source/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.4/docs/source/create-task.rst
--rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.4/docs/source/define-instrument.rst
--rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.4/docs/source/example.rst
--rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.4/docs/source/index.rst
--rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.4/docs/source/installation.rst
--rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/srsgui.inst.rst
--rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/srsgui.rst
--rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/srsgui.task.rst
--rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.4/docs/source/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1193 2023-04-05 21:32:45.000000 srsgui-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 00:52:28.599757 srsgui-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.559806 srsgui-0.2.4/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-04-07 00:39:13.000000 srsgui-0.2.4/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.4/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.523518 srsgui-0.2.4/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.559806 srsgui-0.2.4/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.559806 srsgui-0.2.4/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.569774 srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.569774 srsgui-0.2.4/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.4/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9299 2023-04-06 16:43:53.000000 srsgui-0.2.4/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.579792 srsgui-0.2.4/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    14572 2023-04-04 22:33:16.000000 srsgui-0.2.4/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10031 2023-04-06 16:43:14.000000 srsgui-0.2.4/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.4/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.579792 srsgui-0.2.4/srsgui/task/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:11:30.000000 srsgui-0.2.4/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6485 2023-04-06 18:10:52.000000 srsgui-0.2.4/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.4/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.599757 srsgui-0.2.4/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     2901 2023-04-05 22:30:32.000000 srsgui-0.2.4/srsgui/ui/capturecommandwidget.py
--rw-rw-rw-   0        0        0     3339 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/capturecommandwidget.ui
--rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/commandterminal.py
--rw-rw-rw-   0        0        0     9679 2023-04-06 22:26:43.000000 srsgui-0.2.4/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    14044 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    11682 2023-04-06 22:28:50.000000 srsgui-0.2.4/srsgui/ui/inputpanel.py
--rw-rw-rw-   0        0        0     9269 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/jsonmodel.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.599757 srsgui-0.2.4/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.4/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.4/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    24758 2023-04-07 00:51:55.000000 srsgui-0.2.4/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.4/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0     4754 2023-04-04 20:33:12.000000 srsgui-0.2.4/srsgui/ui/ui_capturecommandwidget.py
--rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.4/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-04-07 00:52:28.559806 srsgui-0.2.4/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-04-07 00:52:28.000000 srsgui-0.2.4/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2828 2023-04-07 00:52:28.000000 srsgui-0.2.4/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 00:52:28.000000 srsgui-0.2.4/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-07 00:52:28.000000 srsgui-0.2.4/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-04-07 00:52:28.000000 srsgui-0.2.4/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 00:52:28.000000 srsgui-0.2.4/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.181560 srsgui-0.2.5/
+-rw-rw-rw-   0        0        0     1345 2022-08-02 00:19:43.000000 srsgui-0.2.5/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-12-07 23:27:48.000000 srsgui-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3330 2023-04-07 19:48:06.181560 srsgui-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2633 2023-02-13 17:17:13.000000 srsgui-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.088463 srsgui-0.2.5/docs/
+-rw-rw-rw-   0        0        0      658 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/Makefile
+-rwxrwxrwx   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/autodoc.bat
+-rwxrwxrwx   0        0        0      804 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.109847 srsgui-0.2.5/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.119845 srsgui-0.2.5/docs/source/_static/
+-rw-rw-rw-   0        0        0    31067 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    71070 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    39412 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     1938 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0     5998 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/create-task.rst
+-rw-rw-rw-   0        0        0     6110 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/define-instrument.rst
+-rw-rw-rw-   0        0        0    15655 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/example.rst
+-rw-rw-rw-   0        0        0     3684 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4383 2023-04-04 20:33:11.000000 srsgui-0.2.5/docs/source/installation.rst
+-rw-rw-rw-   0        0        0      936 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      950 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      117 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.rst
+-rw-rw-rw-   0        0        0      989 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.task.rst
+-rw-rw-rw-   0        0        0      604 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1629 2023-01-30 16:55:49.000000 srsgui-0.2.5/docs/source/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1193 2023-04-07 01:13:40.000000 srsgui-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-07 19:48:06.181560 srsgui-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.119845 srsgui-0.2.5/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-04-07 19:44:30.000000 srsgui-0.2.5/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-04-07 00:52:02.000000 srsgui-0.2.5/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.079873 srsgui-0.2.5/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.129840 srsgui-0.2.5/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.129840 srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1709 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3025 2023-02-11 01:21:41.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.139834 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2401 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1543 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     3978 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2129 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     1893 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.139834 srsgui-0.2.5/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-04-04 20:33:11.000000 srsgui-0.2.5/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9530 2023-04-07 18:58:15.000000 srsgui-0.2.5/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.149856 srsgui-0.2.5/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1157 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8097 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    10762 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    14572 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      727 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10031 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9647 2023-02-09 17:58:55.000000 srsgui-0.2.5/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.149856 srsgui-0.2.5/srsgui/task/
+-rw-rw-rw-   0        0        0        0 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      692 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6485 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5171 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6865 2023-03-28 15:59:44.000000 srsgui-0.2.5/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    21917 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4108 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.171563 srsgui-0.2.5/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3775 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     5918 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.171563 srsgui-0.2.5/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0     2919 2023-04-07 19:30:21.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.py
+-rw-rw-rw-   0        0        0     3339 2023-04-07 19:13:45.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.ui
+-rw-rw-rw-   0        0        0     3324 2023-04-07 15:52:10.000000 srsgui-0.2.5/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     9222 2023-04-07 15:52:10.000000 srsgui-0.2.5/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     7585 2023-04-07 19:01:35.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     4996 2023-04-07 15:52:11.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3292 2023-04-07 19:41:07.000000 srsgui-0.2.5/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     9296 2023-04-07 16:02:56.000000 srsgui-0.2.5/srsgui/ui/commandtree/jsonmodel.py
+-rw-rw-rw-   0        0        0     4781 2023-04-07 19:18:07.000000 srsgui-0.2.5/srsgui/ui/commandtree/ui_commandcapturewidget.py
+-rw-rw-rw-   0        0        0     9679 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3856 2023-04-04 20:33:12.000000 srsgui-0.2.5/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    14127 2023-04-07 19:34:20.000000 srsgui-0.2.5/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    11682 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.181560 srsgui-0.2.5/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      678 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      556 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      656 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1457 2023-03-08 01:32:20.000000 srsgui-0.2.5/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1164 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15358 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2598 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0      886 2023-01-30 16:55:49.000000 srsgui-0.2.5/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    24758 2023-04-07 01:13:40.000000 srsgui-0.2.5/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-02-22 17:26:46.000000 srsgui-0.2.5/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-02-22 17:26:46.000000 srsgui-0.2.5/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-04-07 19:48:06.129840 srsgui-0.2.5/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3330 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2023-04-07 19:48:06.000000 srsgui-0.2.5/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-07 19:48:05.000000 srsgui-0.2.5/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.2.4/.gitignore` & `srsgui-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/LICENSE.txt` & `srsgui-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/PKG-INFO` & `srsgui-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.4
+Version: 0.2.5
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.4/README.md` & `srsgui-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/Makefile` & `srsgui-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/make.bat` & `srsgui-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.2.5/docs/source/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/cg-terminal-screen-capture.png` & `srsgui-0.2.5/docs/source/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/connect-dialog-box-capture.png` & `srsgui-0.2.5/docs/source/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/example-screen-capture-1.png` & `srsgui-0.2.5/docs/source/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/example-screen-capture-2.png` & `srsgui-0.2.5/docs/source/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/initial-screen-capture.png` & `srsgui-0.2.5/docs/source/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.2.5/docs/source/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/second-task-screen-capture.png` & `srsgui-0.2.5/docs/source/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/terminal-with-example-2.png` & `srsgui-0.2.5/docs/source/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/_static/terminal-with-example.png` & `srsgui-0.2.5/docs/source/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/conf.py` & `srsgui-0.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/create-project.rst` & `srsgui-0.2.5/docs/source/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/create-task.rst` & `srsgui-0.2.5/docs/source/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/define-instrument.rst` & `srsgui-0.2.5/docs/source/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/example.rst` & `srsgui-0.2.5/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/index.rst` & `srsgui-0.2.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/installation.rst` & `srsgui-0.2.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/srsgui.inst.communications.rst` & `srsgui-0.2.5/docs/source/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/srsgui.inst.rst` & `srsgui-0.2.5/docs/source/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/srsgui.task.rst` & `srsgui-0.2.5/docs/source/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/srsgui.ui.qt.rst` & `srsgui-0.2.5/docs/source/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/docs/source/srsgui.ui.rst` & `srsgui-0.2.5/docs/source/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/pyproject.toml` & `srsgui-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/__init__.py` & `srsgui-0.2.5/srsgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.2.4"  # Global version number
+__version__ = "0.2.5"  # Global version number
```

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.2.5/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/__init__.py` & `srsgui-0.2.5/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/commands.py` & `srsgui-0.2.5/srsgui/inst/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -256,14 +256,19 @@
     """
     Descriptor for a remote command to
     **set** and **query** using a conversion dictionary
     """
 
     def __init__(self, remote_command_name, set_dict, get_dict=None, unit='', fmt='{}', default_value=None):
         super().__init__(remote_command_name, default_value)
+        if type(set_dict) is not dict:
+            raise TypeError('set_dict must be a dictionary')
+        if get_dict is not None and type(get_dict) is not dict:
+            raise TypeError('get_dict must be a dictionary')
+
         self.set_dict = set_dict
         if get_dict is None:
             self.get_dict = set_dict
         else:
             self.get_dict = get_dict
         self.key_type = type(list(set_dict.keys())[0])
         self.value_type = type(list(set_dict.values())[0])
```

### Comparing `srsgui-0.2.4/srsgui/inst/communications/interface.py` & `srsgui-0.2.5/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/communications/serial_ports.py` & `srsgui-0.2.5/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/communications/serialinterface.py` & `srsgui-0.2.5/srsgui/inst/communications/serialinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.2.5/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/component.py` & `srsgui-0.2.5/srsgui/inst/component.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/exceptions.py` & `srsgui-0.2.5/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/indexcommands.py` & `srsgui-0.2.5/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/inst/instrument.py` & `srsgui-0.2.5/srsgui/inst/instrument.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/task/callbacks.py` & `srsgui-0.2.5/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/task/config.py` & `srsgui-0.2.5/srsgui/task/config.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/task/inputs.py` & `srsgui-0.2.5/srsgui/task/inputs.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/task/sessionhandler.py` & `srsgui-0.2.5/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/task/task.py` & `srsgui-0.2.5/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/task/taskresult.py` & `srsgui-0.2.5/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/capturecommandwidget.py` & `srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 import logging
 from .jsonmodel import JsonModel
 
-from .qt.QtCore import Qt
-from .qt.QtWidgets import QWidget
-from .ui_capturecommandwidget import Ui_CaptureCommandWidget
+from srsgui.ui.qt.QtCore import Qt
+from srsgui.ui.qt.QtWidgets import QWidget
+from .ui_commandcapturewidget import Ui_CommandCaptureWidget
 
 logger = logging.getLogger(__name__)
 
 
-class CaptureCommandWidget(QWidget, Ui_CaptureCommandWidget):
+class CommandCaptureWidget(QWidget, Ui_CommandCaptureWidget):
     def __init__(self, parent=None):
-        super(CaptureCommandWidget, self).__init__(parent)
+        super(CommandCaptureWidget, self).__init__(parent)
         self.parent = parent
         self.setupUi(self)
         #self.splitter.setStretchFactor(0, 1)
         #self.splitter.setStretchFactor(1, 2)
 
         self.inst = None
         self.name = None
```

### Comparing `srsgui-0.2.4/srsgui/ui/capturecommandwidget.ui` & `srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.ui`

 * *Files 1% similar despite different names*

#### Comparing `srsgui-0.2.4/srsgui/ui/capturecommandwidget.ui` & `srsgui-0.2.5/srsgui/ui/commandtree/commandcapturewidget.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>CaptureCommandWidget</class>
-  <widget class="QWidget" name="CaptureCommandWidget">
+  <class>CommandCaptureWidget</class>
+  <widget class="QWidget" name="CommandCaptureWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>398</width>
         <height>523</height>
       </rect>
```

### Comparing `srsgui-0.2.4/srsgui/ui/commandhandler.py` & `srsgui-0.2.5/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/commandterminal.py` & `srsgui-0.2.5/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/connectdlg.py` & `srsgui-0.2.5/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/deviceinfohandler.py` & `srsgui-0.2.5/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/dockhandler.py` & `srsgui-0.2.5/srsgui/ui/dockhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from matplotlib.figure import Figure
 import matplotlib.image as mpimg
 
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 
 from .commandterminal import CommandTerminal
-from .capturecommandwidget import CaptureCommandWidget
+# from .commandtree.commandcapturewidget import CommandCaptureWidget
+from .commandtree.commandtreewidget import CommandTreeWidget
 
 logger = logging.getLogger(__name__)
 
 # define matplotlib level before importing to suppress debug messages
 logging.getLogger('matplotlib').setLevel(logging.WARNING)
 
 
@@ -88,15 +89,14 @@
             self.parent.menu_Plot.triggered.disconnect()
         except:
             pass
         actions = self.parent.menu_Plot.actions()
         for action in actions:
             self.parent.menu_Plot.removeAction(action)
 
-        # self.parent.menu_Plot.triggered.connect(self.onMenuPlotSelected)
         self.action_tight_layout = QAction(self.parent)
         self.action_tight_layout.setText('Adjust Layout')
         self.action_tight_layout.triggered.connect(self.onTightLayout)
         self.parent.menu_Plot.addAction(self.action_tight_layout)
 
         self.action_toolbar = QAction(self.parent)
         self.show_toolbar(False)
@@ -152,15 +152,17 @@
             inst_dock.setObjectName(name)
             inst_dock.setFloating(False)
 
             title = self.TitleFormat.format(name)
             inst_dock.setWindowTitle(title)
             inst_dock.setMinimumSize(200, 350)
 
-            inst_dock.command_capture_widget = CaptureCommandWidget(self.parent)
+            # inst_dock.command_capture_widget = CommandCaptureWidget(self.parent)
+            inst_dock.command_capture_widget = CommandTreeWidget(self.parent)
+
             inst_dock.setWidget(inst_dock.command_capture_widget)
             self.parent.addDockWidget(Qt.LeftDockWidgetArea, inst_dock)
             self.dock_dict[title] = inst_dock
             self.active_inst_dock_names.append(title)
             if len(self.active_inst_dock_names) > 1:
                 self.parent.tabifyDockWidget(
                     self.dock_dict[self.active_inst_dock_names[0]], inst_dock)
```

### Comparing `srsgui-0.2.4/srsgui/ui/inputpanel.py` & `srsgui-0.2.5/srsgui/ui/inputpanel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/jsonmodel.py` & `srsgui-0.2.5/srsgui/ui/commandtree/jsonmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (C) 2022 The Qt Company Ltd.
 # SPDX-License-Identifier: LicenseRef-Qt-Commercial OR BSD-3-Clause
 
 import json
 import sys
 from typing import Any, Iterable, List, Dict, Union
 
-from .qt.QtWidgets import QTreeView, QApplication, QHeaderView
-from .qt.QtCore import QAbstractItemModel, QModelIndex, QObject, Qt, QFileInfo
-from .qt.QtGui import QBrush, QColor
+from srsgui.ui.qt.QtWidgets import QTreeView, QApplication, QHeaderView
+from srsgui.ui.qt.QtCore import QAbstractItemModel, QModelIndex, QObject, Qt, QFileInfo
+from srsgui.ui.qt.QtGui import QBrush, QColor
 
 
 class TreeItem:
     """A Json item corresponding to a line in QTreeView"""
 
     def __init__(self, parent: "TreeItem" = None):
         self._parent = parent
```

### Comparing `srsgui-0.2.4/srsgui/ui/qt/QtCore.py` & `srsgui-0.2.5/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/qt/QtGui.py` & `srsgui-0.2.5/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.2.5/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/qt/__init__.py` & `srsgui-0.2.5/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/qtloghandler.py` & `srsgui-0.2.5/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/resource_rc.py` & `srsgui-0.2.5/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/signalhandler.py` & `srsgui-0.2.5/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/srslogo.jpg` & `srsgui-0.2.5/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/stdout.py` & `srsgui-0.2.5/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/taskmain.py` & `srsgui-0.2.5/srsgui/ui/taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/taskmain.ui` & `srsgui-0.2.5/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui/ui/ui_capturecommandwidget.py` & `srsgui-0.2.5/srsgui/ui/commandtree/ui_commandcapturewidget.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
-## Form generated from reading UI file 'capturecommandwidget.ui'
+## Form generated from reading UI file 'commandcapturewidget.ui'
 ##
 ## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from .qt.QtCore import *
-from .qt.QtGui import *
-from .qt.QtWidgets import *
+from srsgui.ui.qt.QtCore import *
+from srsgui.ui.qt.QtGui import *
+from srsgui.ui.qt.QtWidgets import *
 
 
-class Ui_CaptureCommandWidget(object):
-    def setupUi(self, CaptureCommandWidget):
-        if not CaptureCommandWidget.objectName():
-            CaptureCommandWidget.setObjectName(u"CaptureCommandWidget")
-        CaptureCommandWidget.resize(398, 523)
-        self.verticalLayout_3 = QVBoxLayout(CaptureCommandWidget)
+class Ui_CommandCaptureWidget(object):
+    def setupUi(self, CommandCaptureWidget):
+        if not CommandCaptureWidget.objectName():
+            CommandCaptureWidget.setObjectName(u"CommandCaptureWidget")
+        CommandCaptureWidget.resize(398, 523)
+        self.verticalLayout_3 = QVBoxLayout(CommandCaptureWidget)
         self.verticalLayout_3.setObjectName(u"verticalLayout_3")
         self.horizontalLayout = QHBoxLayout()
         self.horizontalLayout.setObjectName(u"horizontalLayout")
         self.verticalLayout = QVBoxLayout()
         self.verticalLayout.setObjectName(u"verticalLayout")
-        self.query_only_checkbox = QCheckBox(CaptureCommandWidget)
+        self.query_only_checkbox = QCheckBox(CommandCaptureWidget)
         self.query_only_checkbox.setObjectName(u"query_only_checkbox")
 
         self.verticalLayout.addWidget(self.query_only_checkbox)
 
-        self.set_only_checkbox = QCheckBox(CaptureCommandWidget)
+        self.set_only_checkbox = QCheckBox(CommandCaptureWidget)
         self.set_only_checkbox.setObjectName(u"set_only_checkbox")
 
         self.verticalLayout.addWidget(self.set_only_checkbox)
 
-        self.excluded_checkbox = QCheckBox(CaptureCommandWidget)
+        self.excluded_checkbox = QCheckBox(CommandCaptureWidget)
         self.excluded_checkbox.setObjectName(u"excluded_checkbox")
 
         self.verticalLayout.addWidget(self.excluded_checkbox)
 
-        self.method_checkbox = QCheckBox(CaptureCommandWidget)
+        self.method_checkbox = QCheckBox(CommandCaptureWidget)
         self.method_checkbox.setObjectName(u"method_checkbox")
 
         self.verticalLayout.addWidget(self.method_checkbox)
 
-        self.raw_command_checkbox = QCheckBox(CaptureCommandWidget)
+        self.raw_command_checkbox = QCheckBox(CommandCaptureWidget)
         self.raw_command_checkbox.setObjectName(u"raw_command_checkbox")
 
         self.verticalLayout.addWidget(self.raw_command_checkbox)
 
 
         self.horizontalLayout.addLayout(self.verticalLayout)
 
         self.horizontalSpacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout.addItem(self.horizontalSpacer)
 
         self.verticalLayout_2 = QVBoxLayout()
         self.verticalLayout_2.setObjectName(u"verticalLayout_2")
-        self.capture_button = QPushButton(CaptureCommandWidget)
+        self.capture_button = QPushButton(CommandCaptureWidget)
         self.capture_button.setObjectName(u"capture_button")
 
         self.verticalLayout_2.addWidget(self.capture_button)
 
         self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Minimum)
 
         self.verticalLayout_2.addItem(self.verticalSpacer)
 
-        self.expand_button = QPushButton(CaptureCommandWidget)
+        self.expand_button = QPushButton(CommandCaptureWidget)
         self.expand_button.setObjectName(u"expand_button")
 
         self.verticalLayout_2.addWidget(self.expand_button)
 
-        self.collapse_button = QPushButton(CaptureCommandWidget)
+        self.collapse_button = QPushButton(CommandCaptureWidget)
         self.collapse_button.setObjectName(u"collapse_button")
 
         self.verticalLayout_2.addWidget(self.collapse_button)
 
 
         self.horizontalLayout.addLayout(self.verticalLayout_2)
 
 
         self.verticalLayout_3.addLayout(self.horizontalLayout)
 
-        self.tree_view = QTreeView(CaptureCommandWidget)
+        self.tree_view = QTreeView(CommandCaptureWidget)
         self.tree_view.setObjectName(u"tree_view")
 
         self.verticalLayout_3.addWidget(self.tree_view)
 
 
-        self.retranslateUi(CaptureCommandWidget)
+        self.retranslateUi(CommandCaptureWidget)
 
-        QMetaObject.connectSlotsByName(CaptureCommandWidget)
+        QMetaObject.connectSlotsByName(CommandCaptureWidget)
     # setupUi
 
-    def retranslateUi(self, CaptureCommandWidget):
-        CaptureCommandWidget.setWindowTitle(QCoreApplication.translate("CaptureCommandWidget", u"Form", None))
-        self.query_only_checkbox.setText(QCoreApplication.translate("CaptureCommandWidget", u"Include query-only cmds", None))
-        self.set_only_checkbox.setText(QCoreApplication.translate("CaptureCommandWidget", u"Show set-only cmds", None))
-        self.excluded_checkbox.setText(QCoreApplication.translate("CaptureCommandWidget", u"Show excluded cmds", None))
-        self.method_checkbox.setText(QCoreApplication.translate("CaptureCommandWidget", u"Show methods", None))
-        self.raw_command_checkbox.setText(QCoreApplication.translate("CaptureCommandWidget", u"Show raw cmds", None))
-        self.capture_button.setText(QCoreApplication.translate("CaptureCommandWidget", u"Capture", None))
-        self.expand_button.setText(QCoreApplication.translate("CaptureCommandWidget", u"Expand all", None))
-        self.collapse_button.setText(QCoreApplication.translate("CaptureCommandWidget", u"Collapse all", None))
+    def retranslateUi(self, CommandCaptureWidget):
+        CommandCaptureWidget.setWindowTitle(QCoreApplication.translate("CommandCaptureWidget", u"Form", None))
+        self.query_only_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Include query-only cmds", None))
+        self.set_only_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show set-only cmds", None))
+        self.excluded_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show excluded cmds", None))
+        self.method_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show methods", None))
+        self.raw_command_checkbox.setText(QCoreApplication.translate("CommandCaptureWidget", u"Show raw cmds", None))
+        self.capture_button.setText(QCoreApplication.translate("CommandCaptureWidget", u"Capture", None))
+        self.expand_button.setText(QCoreApplication.translate("CommandCaptureWidget", u"Expand all", None))
+        self.collapse_button.setText(QCoreApplication.translate("CommandCaptureWidget", u"Collapse all", None))
     # retranslateUi
```

### Comparing `srsgui-0.2.4/srsgui/ui/ui_taskmain.py` & `srsgui-0.2.5/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.2.4/srsgui.egg-info/PKG-INFO` & `srsgui-0.2.5/srsgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.2.4
+Version: 0.2.5
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `srsgui-0.2.4/srsgui.egg-info/SOURCES.txt` & `srsgui-0.2.5/srsgui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -62,30 +62,35 @@
 srsgui/task/callbacks.py
 srsgui/task/config.py
 srsgui/task/inputs.py
 srsgui/task/sessionhandler.py
 srsgui/task/task.py
 srsgui/task/taskresult.py
 srsgui/ui/__init__.py
-srsgui/ui/capturecommandwidget.py
-srsgui/ui/capturecommandwidget.ui
 srsgui/ui/commandhandler.py
 srsgui/ui/commandterminal.py
 srsgui/ui/connectdlg.py
 srsgui/ui/deviceinfohandler.py
 srsgui/ui/dockhandler.py
 srsgui/ui/inputpanel.py
-srsgui/ui/jsonmodel.py
 srsgui/ui/qtloghandler.py
 srsgui/ui/resource.qrc
 srsgui/ui/resource_rc.py
 srsgui/ui/signalhandler.py
 srsgui/ui/srslogo.jpg
 srsgui/ui/stdout.py
 srsgui/ui/taskmain.py
 srsgui/ui/taskmain.ui
-srsgui/ui/ui_capturecommandwidget.py
 srsgui/ui/ui_taskmain.py
+srsgui/ui/commandtree/commandcapturewidget.py
+srsgui/ui/commandtree/commandcapturewidget.ui
+srsgui/ui/commandtree/commanddelegate.py
+srsgui/ui/commandtree/commanditem.py
+srsgui/ui/commandtree/commandmodel.py
+srsgui/ui/commandtree/commandspinbox.py
+srsgui/ui/commandtree/commandtreewidget.py
+srsgui/ui/commandtree/jsonmodel.py
+srsgui/ui/commandtree/ui_commandcapturewidget.py
 srsgui/ui/qt/QtCore.py
 srsgui/ui/qt/QtGui.py
 srsgui/ui/qt/QtWidgets.py
 srsgui/ui/qt/__init__.py
```

