# Comparing `tmp/PyQt6-6.4.2.tar.gz` & `tmp/PyQt6-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6-6.4.2.tar", last modified: Sat Feb  4 11:48:54 2023, max compression
+gzip compressed data, was "PyQt6-6.5.0.tar", last modified: Wed Apr  5 12:16:56 2023, max compression
```

## Comparing `PyQt6-6.4.2.tar` & `PyQt6-6.5.0.tar`

### file list

```diff
@@ -1,1143 +1,1156 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.434892 PyQt6-6.4.2/
--rw-r--r--   0 phil       (501) staff       (20)   115522 2023-02-04 11:48:42.520630 PyQt6-6.4.2/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-02-04 11:48:42.000548 PyQt6-6.4.2/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)     3099 2023-02-04 11:48:42.522349 PyQt6-6.4.2/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     2075 2023-02-04 11:48:54.435013 PyQt6-6.4.2/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1735 2023-02-04 11:48:42.762704 PyQt6-6.4.2/README
--rw-r--r--   0 phil       (501) staff       (20)      960 2023-02-04 11:48:42.533192 PyQt6-6.4.2/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.074576 PyQt6-6.4.2/config-tests/
--rw-r--r--   0 phil       (501) staff       (20)      756 2023-02-04 11:48:42.531929 PyQt6-6.4.2/config-tests/cfgtest_QtCore.cpp
--rw-r--r--   0 phil       (501) staff       (20)      813 2023-02-04 11:48:42.530690 PyQt6-6.4.2/config-tests/cfgtest_QtGui.cpp
--rw-r--r--   0 phil       (501) staff       (20)      569 2023-02-04 11:48:42.532435 PyQt6-6.4.2/config-tests/cfgtest_QtNetwork.cpp
--rw-r--r--   0 phil       (501) staff       (20)      752 2023-02-04 11:48:42.531340 PyQt6-6.4.2/config-tests/cfgtest_QtPrintSupport.cpp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.072340 PyQt6-6.4.2/dbus/
--rw-r--r--   0 phil       (501) staff       (20)    11344 2023-02-04 11:48:42.755979 PyQt6-6.4.2/dbus/dbus.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2067 2023-02-04 11:48:42.753728 PyQt6-6.4.2/dbus/helper.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.182947 PyQt6-6.4.2/designer/
--rw-r--r--   0 phil       (501) staff       (20)      435 2023-02-04 11:48:42.756780 PyQt6-6.4.2/designer/designer.pro-in
--rw-r--r--   0 phil       (501) staff       (20)     9229 2023-02-04 11:48:42.758572 PyQt6-6.4.2/designer/pluginloader.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1982 2023-02-04 11:48:42.759070 PyQt6-6.4.2/designer/pluginloader.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.181037 PyQt6-6.4.2/examples/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.172659 PyQt6-6.4.2/examples/designer/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.173600 PyQt6-6.4.2/examples/designer/calculatorform/
--rw-r--r--   0 phil       (501) staff       (20)     2805 2023-02-04 11:01:32.202841 PyQt6-6.4.2/examples/designer/calculatorform/calculatorform.py
--rw-r--r--   0 phil       (501) staff       (20)     7150 2023-02-04 11:01:32.202970 PyQt6-6.4.2/examples/designer/calculatorform/calculatorform.ui
--rw-r--r--   0 phil       (501) staff       (20)     5538 2023-02-04 11:01:32.205079 PyQt6-6.4.2/examples/designer/calculatorform/ui_calculatorform.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.169502 PyQt6-6.4.2/examples/designer/plugins/
--rw-r--r--   0 phil       (501) staff       (20)     3578 2023-02-04 11:01:32.198458 PyQt6-6.4.2/examples/designer/plugins/plugins.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.169158 PyQt6-6.4.2/examples/designer/plugins/python/
--rw-r--r--   0 phil       (501) staff       (20)     5548 2023-02-04 11:01:32.198795 PyQt6-6.4.2/examples/designer/plugins/python/analogclockplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     5106 2023-02-04 11:01:32.199624 PyQt6-6.4.2/examples/designer/plugins/python/bubbleswidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     3447 2023-02-04 11:01:32.317283 PyQt6-6.4.2/examples/designer/plugins/python/counterlabelplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4401 2023-02-04 11:01:32.200002 PyQt6-6.4.2/examples/designer/plugins/python/datetimeeditplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     3566 2023-02-04 11:01:32.200459 PyQt6-6.4.2/examples/designer/plugins/python/helloglwidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     5126 2023-02-04 11:01:32.201009 PyQt6-6.4.2/examples/designer/plugins/python/multipagewidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4714 2023-02-04 11:01:32.201365 PyQt6-6.4.2/examples/designer/plugins/python/polygonwidgetplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4184 2023-02-04 11:01:32.204226 PyQt6-6.4.2/examples/designer/plugins/python/pydemoplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     4612 2023-02-04 11:01:32.204274 PyQt6-6.4.2/examples/designer/plugins/python/pythonconsoleplugin.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.172342 PyQt6-6.4.2/examples/designer/plugins/widgets/
--rw-r--r--   0 phil       (501) staff       (20)     6253 2023-02-04 11:01:32.204263 PyQt6-6.4.2/examples/designer/plugins/widgets/analogclock.py
--rw-r--r--   0 phil       (501) staff       (20)    10365 2023-02-04 11:01:32.206675 PyQt6-6.4.2/examples/designer/plugins/widgets/bubbleswidget.py
--rw-r--r--   0 phil       (501) staff       (20)     5187 2023-02-04 11:01:32.199905 PyQt6-6.4.2/examples/designer/plugins/widgets/counterlabel.py
--rw-r--r--   0 phil       (501) staff       (20)    16152 2023-02-04 11:01:32.200565 PyQt6-6.4.2/examples/designer/plugins/widgets/datetimeedit.py
--rw-r--r--   0 phil       (501) staff       (20)     8302 2023-02-04 11:01:32.202341 PyQt6-6.4.2/examples/designer/plugins/widgets/helloglwidget.py
--rw-r--r--   0 phil       (501) staff       (20)     3985 2023-02-04 11:01:32.317936 PyQt6-6.4.2/examples/designer/plugins/widgets/multipagewidget.py
--rw-r--r--   0 phil       (501) staff       (20)     5827 2023-02-04 11:01:32.202208 PyQt6-6.4.2/examples/designer/plugins/widgets/polygonwidget.py
--rw-r--r--   0 phil       (501) staff       (20)     5619 2023-02-04 11:01:32.201545 PyQt6-6.4.2/examples/designer/plugins/widgets/pydemo.py
--rw-r--r--   0 phil       (501) staff       (20)     3016 2023-02-04 11:01:32.202015 PyQt6-6.4.2/examples/designer/plugins/widgets/pythonconsolewidget.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.162581 PyQt6-6.4.2/examples/desktop/
--rw-r--r--   0 phil       (501) staff       (20)     6605 2023-02-04 11:01:32.202617 PyQt6-6.4.2/examples/desktop/screenshot.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.163047 PyQt6-6.4.2/examples/desktop/systray/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.163806 PyQt6-6.4.2/examples/desktop/systray/images/
--rw-r--r--   0 phil       (501) staff       (20)     2496 2023-02-04 11:01:32.206031 PyQt6-6.4.2/examples/desktop/systray/images/bad.png
--rw-r--r--   0 phil       (501) staff       (20)    25780 2023-02-04 11:01:32.206571 PyQt6-6.4.2/examples/desktop/systray/images/heart.png
--rw-r--r--   0 phil       (501) staff       (20)    12128 2023-02-04 11:01:32.206249 PyQt6-6.4.2/examples/desktop/systray/images/trash.png
--rw-r--r--   0 phil       (501) staff       (20)     9595 2023-02-04 11:01:32.208308 PyQt6-6.4.2/examples/desktop/systray/systray.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.179116 PyQt6-6.4.2/examples/dialogs/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.176410 PyQt6-6.4.2/examples/dialogs/classwizard/
--rw-r--r--   0 phil       (501) staff       (20)    15515 2023-02-04 11:01:32.201269 PyQt6-6.4.2/examples/dialogs/classwizard/classwizard.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.178710 PyQt6-6.4.2/examples/dialogs/classwizard/images/
--rw-r--r--   0 phil       (501) staff       (20)    22578 2023-02-04 11:01:32.202858 PyQt6-6.4.2/examples/dialogs/classwizard/images/background.png
--rw-r--r--   0 phil       (501) staff       (20)     3947 2023-02-04 11:01:32.203672 PyQt6-6.4.2/examples/dialogs/classwizard/images/banner.png
--rw-r--r--   0 phil       (501) staff       (20)     1619 2023-02-04 11:01:32.318697 PyQt6-6.4.2/examples/dialogs/classwizard/images/logo1.png
--rw-r--r--   0 phil       (501) staff       (20)     1619 2023-02-04 11:01:32.203631 PyQt6-6.4.2/examples/dialogs/classwizard/images/logo2.png
--rw-r--r--   0 phil       (501) staff       (20)     1619 2023-02-04 11:01:32.202866 PyQt6-6.4.2/examples/dialogs/classwizard/images/logo3.png
--rw-r--r--   0 phil       (501) staff       (20)    14516 2023-02-04 11:01:32.203287 PyQt6-6.4.2/examples/dialogs/classwizard/images/watermark1.png
--rw-r--r--   0 phil       (501) staff       (20)    14912 2023-02-04 11:01:32.204749 PyQt6-6.4.2/examples/dialogs/classwizard/images/watermark2.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.179578 PyQt6-6.4.2/examples/dialogs/configdialog/
--rw-r--r--   0 phil       (501) staff       (20)     8989 2023-02-04 11:01:32.207926 PyQt6-6.4.2/examples/dialogs/configdialog/configdialog.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.180579 PyQt6-6.4.2/examples/dialogs/configdialog/images/
--rw-r--r--   0 phil       (501) staff       (20)     7059 2023-02-04 11:01:32.208236 PyQt6-6.4.2/examples/dialogs/configdialog/images/config.png
--rw-r--r--   0 phil       (501) staff       (20)     2269 2023-02-04 11:01:32.207867 PyQt6-6.4.2/examples/dialogs/configdialog/images/query.png
--rw-r--r--   0 phil       (501) staff       (20)     8296 2023-02-04 11:01:32.210423 PyQt6-6.4.2/examples/dialogs/configdialog/images/update.png
--rw-r--r--   0 phil       (501) staff       (20)     4434 2023-02-04 11:01:32.202675 PyQt6-6.4.2/examples/dialogs/extension.py
--rw-r--r--   0 phil       (501) staff       (20)     8264 2023-02-04 11:01:32.204374 PyQt6-6.4.2/examples/dialogs/findfiles.py
--rw-r--r--   0 phil       (501) staff       (20)    13995 2023-02-04 11:01:32.204986 PyQt6-6.4.2/examples/dialogs/standarddialogs.py
--rw-r--r--   0 phil       (501) staff       (20)     7401 2023-02-04 11:01:32.319390 PyQt6-6.4.2/examples/dialogs/tabdialog.py
--rw-r--r--   0 phil       (501) staff       (20)     3603 2023-02-04 11:01:32.204659 PyQt6-6.4.2/examples/dialogs/trivialwizard.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.121781 PyQt6-6.4.2/examples/draganddrop/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.121041 PyQt6-6.4.2/examples/draganddrop/delayedencoding/
--rw-r--r--   0 phil       (501) staff       (20)     4979 2023-02-04 11:01:32.204536 PyQt6-6.4.2/examples/draganddrop/delayedencoding/delayedencoding.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.121504 PyQt6-6.4.2/examples/draganddrop/delayedencoding/images/
--rw-r--r--   0 phil       (501) staff       (20)      977 2023-02-04 11:01:32.204724 PyQt6-6.4.2/examples/draganddrop/delayedencoding/images/drag.png
--rw-r--r--   0 phil       (501) staff       (20)     2689 2023-02-04 11:01:32.206027 PyQt6-6.4.2/examples/draganddrop/delayedencoding/images/example.svg
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.118671 PyQt6-6.4.2/examples/draganddrop/draggableicons/
--rw-r--r--   0 phil       (501) staff       (20)     5975 2023-02-04 11:01:32.209682 PyQt6-6.4.2/examples/draganddrop/draggableicons/draggableicons.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.119568 PyQt6-6.4.2/examples/draganddrop/draggableicons/images/
--rw-r--r--   0 phil       (501) staff       (20)     2772 2023-02-04 11:01:32.210002 PyQt6-6.4.2/examples/draganddrop/draggableicons/images/boat.png
--rw-r--r--   0 phil       (501) staff       (20)     2963 2023-02-04 11:01:32.209676 PyQt6-6.4.2/examples/draganddrop/draggableicons/images/car.png
--rw-r--r--   0 phil       (501) staff       (20)     3292 2023-02-04 11:01:32.211919 PyQt6-6.4.2/examples/draganddrop/draggableicons/images/house.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.120303 PyQt6-6.4.2/examples/draganddrop/draggabletext/
--rw-r--r--   0 phil       (501) staff       (20)     5414 2023-02-04 11:01:32.204534 PyQt6-6.4.2/examples/draganddrop/draggabletext/draggabletext.py
--rw-r--r--   0 phil       (501) staff       (20)      247 2023-02-04 11:01:32.205719 PyQt6-6.4.2/examples/draganddrop/draggabletext/words.txt
--rw-r--r--   0 phil       (501) staff       (20)     6826 2023-02-04 11:01:32.206369 PyQt6-6.4.2/examples/draganddrop/dropsite.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.122236 PyQt6-6.4.2/examples/draganddrop/fridgemagnets/
--rw-r--r--   0 phil       (501) staff       (20)     6903 2023-02-04 11:01:32.320121 PyQt6-6.4.2/examples/draganddrop/fridgemagnets/fridgemagnets.py
--rw-r--r--   0 phil       (501) staff       (20)      278 2023-02-04 11:01:32.205823 PyQt6-6.4.2/examples/draganddrop/fridgemagnets/words.txt
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.117904 PyQt6-6.4.2/examples/draganddrop/puzzle/
--rw-r--r--   0 phil       (501) staff       (20)    42654 2023-02-04 11:01:32.206884 PyQt6-6.4.2/examples/draganddrop/puzzle/example.jpg
--rw-r--r--   0 phil       (501) staff       (20)    12900 2023-02-04 11:01:32.206020 PyQt6-6.4.2/examples/draganddrop/puzzle/puzzle.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.164514 PyQt6-6.4.2/examples/multimedia/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.165443 PyQt6-6.4.2/examples/multimedia/audiodevices/
--rw-r--r--   0 phil       (501) staff       (20)     7889 2023-02-04 11:01:32.208032 PyQt6-6.4.2/examples/multimedia/audiodevices/audiodevices.py
--rw-r--r--   0 phil       (501) staff       (20)    11927 2023-02-04 11:01:32.211209 PyQt6-6.4.2/examples/multimedia/audiodevices/audiodevicesbase.ui
--rw-r--r--   0 phil       (501) staff       (20)    12232 2023-02-04 11:01:32.211761 PyQt6-6.4.2/examples/multimedia/audiodevices/ui_audiodevicesbase.py
--rw-r--r--   0 phil       (501) staff       (20)     9047 2023-02-04 11:01:32.211380 PyQt6-6.4.2/examples/multimedia/audiooutput.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.127636 PyQt6-6.4.2/examples/multimediawidgets/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.130282 PyQt6-6.4.2/examples/multimediawidgets/camera/
--rw-r--r--   0 phil       (501) staff       (20)    21481 2023-02-04 11:01:32.214244 PyQt6-6.4.2/examples/multimediawidgets/camera/camera.py
--rw-r--r--   0 phil       (501) staff       (20)    13064 2023-02-04 11:01:32.206263 PyQt6-6.4.2/examples/multimediawidgets/camera/camera.ui
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.130391 PyQt6-6.4.2/examples/multimediawidgets/camera/images/
--rw-r--r--   0 phil       (501) staff       (20)     1491 2023-02-04 11:01:32.207503 PyQt6-6.4.2/examples/multimediawidgets/camera/images/shutter.svg
--rw-r--r--   0 phil       (501) staff       (20)     3290 2023-02-04 11:01:32.207863 PyQt6-6.4.2/examples/multimediawidgets/camera/imagesettings.ui
--rw-r--r--   0 phil       (501) staff       (20)    10689 2023-02-04 11:01:32.320878 PyQt6-6.4.2/examples/multimediawidgets/camera/ui_camera.py
--rw-r--r--   0 phil       (501) staff       (20)     3453 2023-02-04 11:01:32.207237 PyQt6-6.4.2/examples/multimediawidgets/camera/ui_imagesettings.py
--rw-r--r--   0 phil       (501) staff       (20)     6492 2023-02-04 11:01:32.208561 PyQt6-6.4.2/examples/multimediawidgets/camera/ui_videosettings.py
--rw-r--r--   0 phil       (501) staff       (20)     5727 2023-02-04 11:01:32.207627 PyQt6-6.4.2/examples/multimediawidgets/camera/videosettings.ui
--rw-r--r--   0 phil       (501) staff       (20)     6277 2023-02-04 11:01:32.209741 PyQt6-6.4.2/examples/multimediawidgets/videographicsitem.py
--rw-r--r--   0 phil       (501) staff       (20)     5857 2023-02-04 11:01:32.212506 PyQt6-6.4.2/examples/multimediawidgets/videowidget.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.122616 PyQt6-6.4.2/examples/qml/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.126431 PyQt6-6.4.2/examples/qml/referenceexamples/
--rwxr-xr-x   0 phil       (501) staff       (20)     3228 2023-02-04 11:01:32.213082 PyQt6-6.4.2/examples/qml/referenceexamples/adding.py
--rwxr-xr-x   0 phil       (501) staff       (20)     6032 2023-02-04 11:01:32.212674 PyQt6-6.4.2/examples/qml/referenceexamples/attached.py
--rwxr-xr-x   0 phil       (501) staff       (20)     8823 2023-02-04 11:01:32.215655 PyQt6-6.4.2/examples/qml/referenceexamples/binding.py
--rwxr-xr-x   0 phil       (501) staff       (20)     4133 2023-02-04 11:01:32.208161 PyQt6-6.4.2/examples/qml/referenceexamples/coercion.py
--rwxr-xr-x   0 phil       (501) staff       (20)     4168 2023-02-04 11:01:32.209346 PyQt6-6.4.2/examples/qml/referenceexamples/default.py
--rwxr-xr-x   0 phil       (501) staff       (20)     5630 2023-02-04 11:01:32.209350 PyQt6-6.4.2/examples/qml/referenceexamples/grouped.py
--rwxr-xr-x   0 phil       (501) staff       (20)     4157 2023-02-04 11:01:32.321887 PyQt6-6.4.2/examples/qml/referenceexamples/methods.py
--rwxr-xr-x   0 phil       (501) staff       (20)     3945 2023-02-04 11:01:32.208755 PyQt6-6.4.2/examples/qml/referenceexamples/properties.py
--rwxr-xr-x   0 phil       (501) staff       (20)     6504 2023-02-04 11:01:32.210007 PyQt6-6.4.2/examples/qml/referenceexamples/signal.py
--rwxr-xr-x   0 phil       (501) staff       (20)     8821 2023-02-04 11:01:32.209345 PyQt6-6.4.2/examples/qml/referenceexamples/valuesource.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.161346 PyQt6-6.4.2/examples/quick/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.138367 PyQt6-6.4.2/examples/quick/animation/
--rw-r--r--   0 phil       (501) staff       (20)     2415 2023-02-04 11:01:32.211001 PyQt6-6.4.2/examples/quick/animation/animation.py
--rw-r--r--   0 phil       (501) staff       (20)     3371 2023-02-04 11:01:32.213622 PyQt6-6.4.2/examples/quick/animation/animation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.133090 PyQt6-6.4.2/examples/quick/animation/basics/
--rw-r--r--   0 phil       (501) staff       (20)     4957 2023-02-04 11:01:32.214552 PyQt6-6.4.2/examples/quick/animation/basics/color-animation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.135010 PyQt6-6.4.2/examples/quick/animation/basics/images/
--rw-r--r--   0 phil       (501) staff       (20)    15408 2023-02-04 11:01:32.214656 PyQt6-6.4.2/examples/quick/animation/basics/images/face-smile.png
--rw-r--r--   0 phil       (501) staff       (20)     2433 2023-02-04 11:01:32.217195 PyQt6-6.4.2/examples/quick/animation/basics/images/moon.png
--rw-r--r--   0 phil       (501) staff       (20)      425 2023-02-04 11:01:32.210346 PyQt6-6.4.2/examples/quick/animation/basics/images/shadow.png
--rw-r--r--   0 phil       (501) staff       (20)      349 2023-02-04 11:01:32.211077 PyQt6-6.4.2/examples/quick/animation/basics/images/star.png
--rw-r--r--   0 phil       (501) staff       (20)     8153 2023-02-04 11:01:32.210945 PyQt6-6.4.2/examples/quick/animation/basics/images/sun.png
--rw-r--r--   0 phil       (501) staff       (20)     4187 2023-02-04 11:01:32.322758 PyQt6-6.4.2/examples/quick/animation/basics/property-animation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.138062 PyQt6-6.4.2/examples/quick/animation/behaviors/
--rw-r--r--   0 phil       (501) staff       (20)     2401 2023-02-04 11:01:32.210512 PyQt6-6.4.2/examples/quick/animation/behaviors/SideRect.qml
--rw-r--r--   0 phil       (501) staff       (20)     4444 2023-02-04 11:01:32.211675 PyQt6-6.4.2/examples/quick/animation/behaviors/behavior-example.qml
--rw-r--r--   0 phil       (501) staff       (20)     4376 2023-02-04 11:01:32.211012 PyQt6-6.4.2/examples/quick/animation/behaviors/tvtennis.qml
--rw-r--r--   0 phil       (501) staff       (20)     4090 2023-02-04 11:01:32.212572 PyQt6-6.4.2/examples/quick/animation/behaviors/wigglytext.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.135466 PyQt6-6.4.2/examples/quick/animation/easing/
--rw-r--r--   0 phil       (501) staff       (20)     8398 2023-02-04 11:01:32.215046 PyQt6-6.4.2/examples/quick/animation/easing/easing.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.136460 PyQt6-6.4.2/examples/quick/animation/pathanimation/
--rw-r--r--   0 phil       (501) staff       (20)     3407 2023-02-04 11:01:32.215966 PyQt6-6.4.2/examples/quick/animation/pathanimation/pathanimation.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.136048 PyQt6-6.4.2/examples/quick/animation/pathinterpolator/
--rw-r--r--   0 phil       (501) staff       (20)     3596 2023-02-04 11:01:32.216073 PyQt6-6.4.2/examples/quick/animation/pathinterpolator/pathinterpolator.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.139210 PyQt6-6.4.2/examples/quick/animation/states/
--rw-r--r--   0 phil       (501) staff       (20)     5149 2023-02-04 11:01:32.218641 PyQt6-6.4.2/examples/quick/animation/states/qt-logo.png
--rw-r--r--   0 phil       (501) staff       (20)     3876 2023-02-04 11:01:32.211750 PyQt6-6.4.2/examples/quick/animation/states/states.qml
--rw-r--r--   0 phil       (501) staff       (20)     4932 2023-02-04 11:01:32.212665 PyQt6-6.4.2/examples/quick/animation/states/transitions.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.154662 PyQt6-6.4.2/examples/quick/canvas/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.154223 PyQt6-6.4.2/examples/quick/canvas/bezierCurve/
--rw-r--r--   0 phil       (501) staff       (20)     4728 2023-02-04 11:01:32.212671 PyQt6-6.4.2/examples/quick/canvas/bezierCurve/bezierCurve.qml
--rw-r--r--   0 phil       (501) staff       (20)     2412 2023-02-04 11:01:32.323570 PyQt6-6.4.2/examples/quick/canvas/canvas.py
--rw-r--r--   0 phil       (501) staff       (20)     3069 2023-02-04 11:01:32.211953 PyQt6-6.4.2/examples/quick/canvas/canvas.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.151682 PyQt6-6.4.2/examples/quick/canvas/clip/
--rw-r--r--   0 phil       (501) staff       (20)     5037 2023-02-04 11:01:32.213332 PyQt6-6.4.2/examples/quick/canvas/clip/clip.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.147248 PyQt6-6.4.2/examples/quick/canvas/contents/
--rw-r--r--   0 phil       (501) staff       (20)     3026 2023-02-04 11:01:32.212440 PyQt6-6.4.2/examples/quick/canvas/contents/Button.qml
--rw-r--r--   0 phil       (501) staff       (20)     3391 2023-02-04 11:01:32.214015 PyQt6-6.4.2/examples/quick/canvas/contents/ScrollBar.qml
--rw-r--r--   0 phil       (501) staff       (20)     3915 2023-02-04 11:01:32.216247 PyQt6-6.4.2/examples/quick/canvas/contents/Slider.qml
--rw-r--r--   0 phil       (501) staff       (20)     2826 2023-02-04 11:01:32.216945 PyQt6-6.4.2/examples/quick/canvas/contents/TitleBar.qml
--rw-r--r--   0 phil       (501) staff       (20)     2564 2023-02-04 11:01:32.217362 PyQt6-6.4.2/examples/quick/canvas/contents/ToolBar.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.151297 PyQt6-6.4.2/examples/quick/canvas/contents/images/
--rw-r--r--   0 phil       (501) staff       (20)      571 2023-02-04 11:01:32.219975 PyQt6-6.4.2/examples/quick/canvas/contents/images/button-pressed.png
--rw-r--r--   0 phil       (501) staff       (20)      564 2023-02-04 11:01:32.213411 PyQt6-6.4.2/examples/quick/canvas/contents/images/button.png
--rw-r--r--   0 phil       (501) staff       (20)     7458 2023-02-04 11:01:32.214352 PyQt6-6.4.2/examples/quick/canvas/contents/images/default.svg
--rw-r--r--   0 phil       (501) staff       (20)     1236 2023-02-04 11:01:32.214192 PyQt6-6.4.2/examples/quick/canvas/contents/images/gloss.png
--rw-r--r--   0 phil       (501) staff       (20)     1415 2023-02-04 11:01:32.324513 PyQt6-6.4.2/examples/quick/canvas/contents/images/lineedit.png
--rw-r--r--   0 phil       (501) staff       (20)       87 2023-02-04 11:01:32.213205 PyQt6-6.4.2/examples/quick/canvas/contents/images/lineedit.sci
--rw-r--r--   0 phil       (501) staff       (20)     2369 2023-02-04 11:01:32.214778 PyQt6-6.4.2/examples/quick/canvas/contents/images/quit.png
--rw-r--r--   0 phil       (501) staff       (20)      257 2023-02-04 11:01:32.213557 PyQt6-6.4.2/examples/quick/canvas/contents/images/stripes.png
--rw-r--r--   0 phil       (501) staff       (20)     1436 2023-02-04 11:01:32.215427 PyQt6-6.4.2/examples/quick/canvas/contents/images/titlebar.png
--rw-r--r--   0 phil       (501) staff       (20)       87 2023-02-04 11:01:32.217433 PyQt6-6.4.2/examples/quick/canvas/contents/images/titlebar.sci
--rw-r--r--   0 phil       (501) staff       (20)     2550 2023-02-04 11:01:32.218431 PyQt6-6.4.2/examples/quick/canvas/contents/images/toolbutton.png
--rw-r--r--   0 phil       (501) staff       (20)       87 2023-02-04 11:01:32.218578 PyQt6-6.4.2/examples/quick/canvas/contents/images/toolbutton.sci
--rw-r--r--   0 phil       (501) staff       (20)    23519 2023-02-04 11:01:32.221534 PyQt6-6.4.2/examples/quick/canvas/contents/qt-logo.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.153016 PyQt6-6.4.2/examples/quick/canvas/quadraticCurveTo/
--rw-r--r--   0 phil       (501) staff       (20)     4992 2023-02-04 11:01:32.214935 PyQt6-6.4.2/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.144727 PyQt6-6.4.2/examples/quick/canvas/roundedrect/
--rw-r--r--   0 phil       (501) staff       (20)     5070 2023-02-04 11:01:32.215809 PyQt6-6.4.2/examples/quick/canvas/roundedrect/roundedrect.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.154773 PyQt6-6.4.2/examples/quick/canvas/smile/
--rw-r--r--   0 phil       (501) staff       (20)     5063 2023-02-04 11:01:32.215518 PyQt6-6.4.2/examples/quick/canvas/smile/smile.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.153740 PyQt6-6.4.2/examples/quick/canvas/squircle/
--rw-r--r--   0 phil       (501) staff       (20)      771 2023-02-04 11:01:32.325687 PyQt6-6.4.2/examples/quick/canvas/squircle/squircle.png
--rw-r--r--   0 phil       (501) staff       (20)     5379 2023-02-04 11:01:32.214855 PyQt6-6.4.2/examples/quick/canvas/squircle/squircle.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.152503 PyQt6-6.4.2/examples/quick/canvas/tiger/
--rw-r--r--   0 phil       (501) staff       (20)    93676 2023-02-04 11:01:32.217720 PyQt6-6.4.2/examples/quick/canvas/tiger/tiger.js
--rw-r--r--   0 phil       (501) staff       (20)     4864 2023-02-04 11:01:32.215146 PyQt6-6.4.2/examples/quick/canvas/tiger/tiger.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.142983 PyQt6-6.4.2/examples/quick/models/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.142661 PyQt6-6.4.2/examples/quick/models/abstractitemmodel/
--rw-r--r--   0 phil       (501) staff       (20)     4051 2023-02-04 11:01:32.216498 PyQt6-6.4.2/examples/quick/models/abstractitemmodel/abstractitemmodel.py
--rw-r--r--   0 phil       (501) staff       (20)     2151 2023-02-04 11:01:32.218512 PyQt6-6.4.2/examples/quick/models/abstractitemmodel/view.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.141924 PyQt6-6.4.2/examples/quick/models/objectlistmodel/
--rw-r--r--   0 phil       (501) staff       (20)     3630 2023-02-04 11:01:32.219603 PyQt6-6.4.2/examples/quick/models/objectlistmodel/objectlistmodel.py
--rw-r--r--   0 phil       (501) staff       (20)     2784 2023-02-04 11:01:32.219830 PyQt6-6.4.2/examples/quick/models/objectlistmodel/view.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.143389 PyQt6-6.4.2/examples/quick/models/stringlistmodel/
--rw-r--r--   0 phil       (501) staff       (20)     2607 2023-02-04 11:01:32.222916 PyQt6-6.4.2/examples/quick/models/stringlistmodel/stringlistmodel.py
--rw-r--r--   0 phil       (501) staff       (20)     2772 2023-02-04 11:01:32.216250 PyQt6-6.4.2/examples/quick/models/stringlistmodel/view.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.161393 PyQt6-6.4.2/examples/quick/scenegraph/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.161816 PyQt6-6.4.2/examples/quick/scenegraph/customgeometry/
--rw-r--r--   0 phil       (501) staff       (20)     5922 2023-02-04 11:01:32.217073 PyQt6-6.4.2/examples/quick/scenegraph/customgeometry/customgeometry.py
--rw-r--r--   0 phil       (501) staff       (20)     2732 2023-02-04 11:01:32.216836 PyQt6-6.4.2/examples/quick/scenegraph/customgeometry/main.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.140678 PyQt6-6.4.2/examples/quick/shared/
--rw-r--r--   0 phil       (501) staff       (20)     3291 2023-02-04 11:01:32.326645 PyQt6-6.4.2/examples/quick/shared/Button.qml
--rw-r--r--   0 phil       (501) staff       (20)     5174 2023-02-04 11:01:32.217080 PyQt6-6.4.2/examples/quick/shared/LauncherList.qml
--rw-r--r--   0 phil       (501) staff       (20)     3287 2023-02-04 11:01:32.218814 PyQt6-6.4.2/examples/quick/shared/SimpleLauncherDelegate.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.141082 PyQt6-6.4.2/examples/quick/shared/images/
--rw-r--r--   0 phil       (501) staff       (20)     1590 2023-02-04 11:01:32.217290 PyQt6-6.4.2/examples/quick/shared/images/back.png
--rw-r--r--   0 phil       (501) staff       (20)     1371 2023-02-04 11:01:32.217600 PyQt6-6.4.2/examples/quick/shared/images/next.png
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.155237 PyQt6-6.4.2/examples/quick/tutorials/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.160392 PyQt6-6.4.2/examples/quick/tutorials/extending/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.160885 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter1-basics/
--rw-r--r--   0 phil       (501) staff       (20)     2385 2023-02-04 11:01:32.219814 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter1-basics/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3492 2023-02-04 11:01:32.220795 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.155755 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter2-methods/
--rw-r--r--   0 phil       (501) staff       (20)     2532 2023-02-04 11:01:32.221293 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter2-methods/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3538 2023-02-04 11:01:32.224485 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.156586 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter3-bindings/
--rw-r--r--   0 phil       (501) staff       (20)     2650 2023-02-04 11:01:32.217861 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter3-bindings/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3625 2023-02-04 11:01:32.218269 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.158076 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/
--rw-r--r--   0 phil       (501) staff       (20)     2361 2023-02-04 11:01:32.218153 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     3724 2023-02-04 11:01:32.327534 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.157343 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter5-listproperties/
--rw-r--r--   0 phil       (501) staff       (20)     2643 2023-02-04 11:01:32.218385 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter5-listproperties/app.qml
--rw-r--r--   0 phil       (501) staff       (20)     4116 2023-02-04 11:01:32.220158 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.158918 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.160064 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/
--rw-r--r--   0 phil       (501) staff       (20)     2292 2023-02-04 11:01:32.218983 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py
--rw-r--r--   0 phil       (501) staff       (20)     2587 2023-02-04 11:01:32.218972 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py
--rw-r--r--   0 phil       (501) staff       (20)     3132 2023-02-04 11:01:32.221194 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py
--rw-r--r--   0 phil       (501) staff       (20)       36 2023-02-04 11:01:32.222035 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/qmldir
--rw-r--r--   0 phil       (501) staff       (20)     2643 2023-02-04 11:01:32.222651 PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/app.qml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.181089 PyQt6-6.4.2/examples/richtext/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.181544 PyQt6-6.4.2/examples/richtext/textobject/
--rw-r--r--   0 phil       (501) staff       (20)     3873 2023-02-04 11:01:32.225563 PyQt6-6.4.2/examples/richtext/textobject/heart.svg
--rw-r--r--   0 phil       (501) staff       (20)     4491 2023-02-04 11:01:32.219196 PyQt6-6.4.2/examples/richtext/textobject/textobject.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.059202 PyQt6-6.4.2/lupdate/
--rw-r--r--   0 phil       (501) staff       (20)      875 2023-02-04 11:48:42.718141 PyQt6-6.4.2/lupdate/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2479 2023-02-04 11:48:42.719270 PyQt6-6.4.2/lupdate/designer_source.py
--rw-r--r--   0 phil       (501) staff       (20)     3416 2023-02-04 11:48:42.722119 PyQt6-6.4.2/lupdate/lupdate.py
--rw-r--r--   0 phil       (501) staff       (20)     3062 2023-02-04 11:48:42.715044 PyQt6-6.4.2/lupdate/pylupdate.py
--rw-r--r--   0 phil       (501) staff       (20)    11176 2023-02-04 11:48:42.721296 PyQt6-6.4.2/lupdate/python_source.py
--rw-r--r--   0 phil       (501) staff       (20)     1114 2023-02-04 11:48:42.718603 PyQt6-6.4.2/lupdate/source_file.py
--rw-r--r--   0 phil       (501) staff       (20)    14976 2023-02-04 11:48:42.716994 PyQt6-6.4.2/lupdate/translation_file.py
--rw-r--r--   0 phil       (501) staff       (20)     1633 2023-02-04 11:48:42.717594 PyQt6-6.4.2/lupdate/translations.py
--rw-r--r--   0 phil       (501) staff       (20)     1504 2023-02-04 11:48:42.714284 PyQt6-6.4.2/lupdate/user.py
--rw-r--r--   0 phil       (501) staff       (20)    28302 2023-02-04 11:48:42.765914 PyQt6-6.4.2/project.py
--rw-r--r--   0 phil       (501) staff       (20)      546 2023-02-04 11:48:42.766171 PyQt6-6.4.2/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.434559 PyQt6-6.4.2/qmlscene/
--rw-r--r--   0 phil       (501) staff       (20)     9302 2023-02-04 11:48:42.761775 PyQt6-6.4.2/qmlscene/pluginloader.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1670 2023-02-04 11:48:42.762249 PyQt6-6.4.2/qmlscene/pluginloader.h
--rw-r--r--   0 phil       (501) staff       (20)      451 2023-02-04 11:48:42.759803 PyQt6-6.4.2/qmlscene/qmlscene.pro-in
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.099596 PyQt6-6.4.2/qpy/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.116488 PyQt6-6.4.2/qpy/QtCore/
--rw-r--r--   0 phil       (501) staff       (20)     3878 2023-02-04 11:48:42.619785 PyQt6-6.4.2/qpy/QtCore/qpycore_api.h
--rw-r--r--   0 phil       (501) staff       (20)    48161 2023-02-04 11:48:42.575099 PyQt6-6.4.2/qpy/QtCore/qpycore_chimera.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9449 2023-02-04 11:48:42.587534 PyQt6-6.4.2/qpy/QtCore/qpycore_chimera.h
--rw-r--r--   0 phil       (501) staff       (20)     2557 2023-02-04 11:48:42.607258 PyQt6-6.4.2/qpy/QtCore/qpycore_chimera_signature.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3515 2023-02-04 11:48:42.604827 PyQt6-6.4.2/qpy/QtCore/qpycore_chimera_storage.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3077 2023-02-04 11:48:42.608334 PyQt6-6.4.2/qpy/QtCore/qpycore_classinfo.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1089 2023-02-04 11:48:42.538310 PyQt6-6.4.2/qpy/QtCore/qpycore_classinfo.h
--rw-r--r--   0 phil       (501) staff       (20)     4385 2023-02-04 11:48:42.567558 PyQt6-6.4.2/qpy/QtCore/qpycore_decorators.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5508 2023-02-04 11:48:42.562251 PyQt6-6.4.2/qpy/QtCore/qpycore_enums_flags.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-02-04 11:48:42.606440 PyQt6-6.4.2/qpy/QtCore/qpycore_enums_flags.h
--rw-r--r--   0 phil       (501) staff       (20)     4006 2023-02-04 11:48:42.543375 PyQt6-6.4.2/qpy/QtCore/qpycore_event_handlers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1376 2023-02-04 11:48:42.609435 PyQt6-6.4.2/qpy/QtCore/qpycore_event_handlers.h
--rw-r--r--   0 phil       (501) staff       (20)     3908 2023-02-04 11:48:42.563558 PyQt6-6.4.2/qpy/QtCore/qpycore_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1815 2023-02-04 11:48:42.588779 PyQt6-6.4.2/qpy/QtCore/qpycore_misc.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1136 2023-02-04 11:48:42.550247 PyQt6-6.4.2/qpy/QtCore/qpycore_misc.h
--rw-r--r--   0 phil       (501) staff       (20)     1136 2023-02-04 11:48:42.565413 PyQt6-6.4.2/qpy/QtCore/qpycore_namespace.h
--rw-r--r--   0 phil       (501) staff       (20)     1183 2023-02-04 11:48:42.592650 PyQt6-6.4.2/qpy/QtCore/qpycore_objectified_strings.h
--rw-r--r--   0 phil       (501) staff       (20)     4375 2023-02-04 11:48:42.544919 PyQt6-6.4.2/qpy/QtCore/qpycore_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12835 2023-02-04 11:48:42.612609 PyQt6-6.4.2/qpy/QtCore/qpycore_public_api.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4908 2023-02-04 11:48:42.610175 PyQt6-6.4.2/qpy/QtCore/qpycore_public_api.h
--rw-r--r--   0 phil       (501) staff       (20)    29292 2023-02-04 11:48:42.599564 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtboundsignal.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2023 2023-02-04 11:48:42.613924 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtboundsignal.h
--rw-r--r--   0 phil       (501) staff       (20)     6090 2023-02-04 11:48:42.600900 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtconfigure.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7424 2023-02-04 11:48:42.595630 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmethodproxy.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1769 2023-02-04 11:48:42.566642 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmethodproxy.h
--rw-r--r--   0 phil       (501) staff       (20)     2072 2023-02-04 11:48:42.605977 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmutexlocker.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1438 2023-02-04 11:48:42.583485 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmutexlocker.h
--rw-r--r--   0 phil       (501) staff       (20)    15571 2023-02-04 11:48:42.560361 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtproperty.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2076 2023-02-04 11:48:42.560930 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtproperty.h
--rw-r--r--   0 phil       (501) staff       (20)     4765 2023-02-04 11:48:42.590897 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtpyobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1742 2023-02-04 11:48:42.565950 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtpyobject.h
--rw-r--r--   0 phil       (501) staff       (20)    20440 2023-02-04 11:48:42.542018 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtsignal.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2537 2023-02-04 11:48:42.589595 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtsignal.h
--rw-r--r--   0 phil       (501) staff       (20)     9102 2023-02-04 11:48:42.577059 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslot.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2284 2023-02-04 11:48:42.610651 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslot.h
--rw-r--r--   0 phil       (501) staff       (20)    10864 2023-02-04 11:48:42.602692 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslotproxy.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3552 2023-02-04 11:48:42.593489 PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslotproxy.h
--rw-r--r--   0 phil       (501) staff       (20)     4375 2023-02-04 11:48:42.613446 PyQt6-6.4.2/qpy/QtCore/qpycore_qjsonvalue.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3016 2023-02-04 11:48:42.609001 PyQt6-6.4.2/qpy/QtCore/qpycore_qmessagelogger.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4296 2023-02-04 11:48:42.584348 PyQt6-6.4.2/qpy/QtCore/qpycore_qmetaobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     4569 2023-02-04 11:48:42.604174 PyQt6-6.4.2/qpy/QtCore/qpycore_qmetaobject_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3505 2023-02-04 11:48:42.585993 PyQt6-6.4.2/qpy/QtCore/qpycore_qmetaobjectbuilder.h
--rw-r--r--   0 phil       (501) staff       (20)     4273 2023-02-04 11:48:42.594315 PyQt6-6.4.2/qpy/QtCore/qpycore_qobject_getattr.cpp
--rw-r--r--   0 phil       (501) staff       (20)     8681 2023-02-04 11:48:42.592300 PyQt6-6.4.2/qpy/QtCore/qpycore_qobject_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1408 2023-02-04 11:48:42.614401 PyQt6-6.4.2/qpy/QtCore/qpycore_qobject_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     4181 2023-02-04 11:48:42.577792 PyQt6-6.4.2/qpy/QtCore/qpycore_qstring.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3178 2023-02-04 11:48:42.552909 PyQt6-6.4.2/qpy/QtCore/qpycore_qt_conf.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2535 2023-02-04 11:48:42.605472 PyQt6-6.4.2/qpy/QtCore/qpycore_qvariant.cpp
--rw-r--r--   0 phil       (501) staff       (20)     6459 2023-02-04 11:48:42.564916 PyQt6-6.4.2/qpy/QtCore/qpycore_qvariant_value.cpp
--rw-r--r--   0 phil       (501) staff       (20)    16884 2023-02-04 11:48:42.556448 PyQt6-6.4.2/qpy/QtCore/qpycore_types.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1576 2023-02-04 11:48:42.557485 PyQt6-6.4.2/qpy/QtCore/qpycore_types.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.097155 PyQt6-6.4.2/qpy/QtDBus/
--rw-r--r--   0 phil       (501) staff       (20)      999 2023-02-04 11:48:42.623921 PyQt6-6.4.2/qpy/QtDBus/qpydbus_api.h
--rw-r--r--   0 phil       (501) staff       (20)     5739 2023-02-04 11:48:42.627456 PyQt6-6.4.2/qpy/QtDBus/qpydbus_chimera_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1236 2023-02-04 11:48:42.626287 PyQt6-6.4.2/qpy/QtDBus/qpydbus_chimera_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     1471 2023-02-04 11:48:42.622847 PyQt6-6.4.2/qpy/QtDBus/qpydbus_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1865 2023-02-04 11:48:42.623565 PyQt6-6.4.2/qpy/QtDBus/qpydbuspendingreply.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1340 2023-02-04 11:48:42.625883 PyQt6-6.4.2/qpy/QtDBus/qpydbuspendingreply.h
--rw-r--r--   0 phil       (501) staff       (20)     3583 2023-02-04 11:48:42.625298 PyQt6-6.4.2/qpy/QtDBus/qpydbusreply.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1788 2023-02-04 11:48:42.622398 PyQt6-6.4.2/qpy/QtDBus/qpydbusreply.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.088761 PyQt6-6.4.2/qpy/QtDesigner/
--rw-r--r--   0 phil       (501) staff       (20)     1410 2023-02-04 11:48:42.629706 PyQt6-6.4.2/qpy/QtDesigner/qpydesignercontainerextension.h
--rw-r--r--   0 phil       (501) staff       (20)     1492 2023-02-04 11:48:42.631757 PyQt6-6.4.2/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h
--rw-r--r--   0 phil       (501) staff       (20)     1402 2023-02-04 11:48:42.630983 PyQt6-6.4.2/qpy/QtDesigner/qpydesignercustomwidgetplugin.h
--rw-r--r--   0 phil       (501) staff       (20)     1430 2023-02-04 11:48:42.628913 PyQt6-6.4.2/qpy/QtDesigner/qpydesignermembersheetextension.h
--rw-r--r--   0 phil       (501) staff       (20)     1450 2023-02-04 11:48:42.630208 PyQt6-6.4.2/qpy/QtDesigner/qpydesignerpropertysheetextension.h
--rw-r--r--   0 phil       (501) staff       (20)     1400 2023-02-04 11:48:42.632744 PyQt6-6.4.2/qpy/QtDesigner/qpydesignertaskmenuextension.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.079992 PyQt6-6.4.2/qpy/QtOpenGL/
--rw-r--r--   0 phil       (501) staff       (20)   209932 2023-02-04 11:48:42.666378 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_add_constants.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2585 2023-02-04 11:48:42.673277 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_api.h
--rw-r--r--   0 phil       (501) staff       (20)     4002 2023-02-04 11:48:42.671385 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_array_convertors.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7165 2023-02-04 11:48:42.668809 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_attribute_array.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5002 2023-02-04 11:48:42.672572 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_data_cache.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2413 2023-02-04 11:48:42.642009 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_data_cache.h
--rw-r--r--   0 phil       (501) staff       (20)     4686 2023-02-04 11:48:42.667378 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_get.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1228 2023-02-04 11:48:42.673856 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-02-04 11:48:42.642499 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_misc.h
--rw-r--r--   0 phil       (501) staff       (20)    12637 2023-02-04 11:48:42.644635 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9947 2023-02-04 11:48:42.646861 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_value_array.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3103 2023-02-04 11:48:42.669656 PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_version_functions.cpp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.086377 PyQt6-6.4.2/qpy/QtQml/
--rw-r--r--   0 phil       (501) staff       (20)     2279 2023-02-04 11:48:42.686184 PyQt6-6.4.2/qpy/QtQml/qpyqml_api.h
--rw-r--r--   0 phil       (501) staff       (20)     1799 2023-02-04 11:48:42.691037 PyQt6-6.4.2/qpy/QtQml/qpyqml_listdata.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1431 2023-02-04 11:48:42.696528 PyQt6-6.4.2/qpy/QtQml/qpyqml_listdata.h
--rw-r--r--   0 phil       (501) staff       (20)     2595 2023-02-04 11:48:42.692204 PyQt6-6.4.2/qpy/QtQml/qpyqml_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3089 2023-02-04 11:48:42.690619 PyQt6-6.4.2/qpy/QtQml/qpyqml_qjsvalue.cpp
--rw-r--r--   0 phil       (501) staff       (20)     5283 2023-02-04 11:48:42.682561 PyQt6-6.4.2/qpy/QtQml/qpyqml_register_singleton_type.cpp
--rw-r--r--   0 phil       (501) staff       (20)    12648 2023-02-04 11:48:42.694175 PyQt6-6.4.2/qpy/QtQml/qpyqml_register_type.cpp
--rw-r--r--   0 phil       (501) staff       (20)     9495 2023-02-04 11:48:42.695883 PyQt6-6.4.2/qpy/QtQml/qpyqmllistproperty.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1118 2023-02-04 11:48:42.689916 PyQt6-6.4.2/qpy/QtQml/qpyqmllistproperty.h
--rw-r--r--   0 phil       (501) staff       (20)     6171 2023-02-04 11:48:42.688014 PyQt6-6.4.2/qpy/QtQml/qpyqmllistpropertywrapper.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1884 2023-02-04 11:48:42.686713 PyQt6-6.4.2/qpy/QtQml/qpyqmllistpropertywrapper.h
--rw-r--r--   0 phil       (501) staff       (20)    17618 2023-02-04 11:48:42.685545 PyQt6-6.4.2/qpy/QtQml/qpyqmlobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     7477 2023-02-04 11:48:42.677753 PyQt6-6.4.2/qpy/QtQml/qpyqmlobject.h
--rw-r--r--   0 phil       (501) staff       (20)     3201 2023-02-04 11:48:42.688829 PyQt6-6.4.2/qpy/QtQml/qpyqmlsingletonobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3097 2023-02-04 11:48:42.678533 PyQt6-6.4.2/qpy/QtQml/qpyqmlsingletonobject.h
--rw-r--r--   0 phil       (501) staff       (20)    10140 2023-02-04 11:48:42.681468 PyQt6-6.4.2/qpy/QtQml/qpyqmlvalidator.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3440 2023-02-04 11:48:42.679450 PyQt6-6.4.2/qpy/QtQml/qpyqmlvalidator.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.094520 PyQt6-6.4.2/qpy/QtQuick/
--rw-r--r--   0 phil       (501) staff       (20)     1136 2023-02-04 11:48:42.700513 PyQt6-6.4.2/qpy/QtQuick/qpyquick_api.h
--rw-r--r--   0 phil       (501) staff       (20)     4162 2023-02-04 11:48:42.701281 PyQt6-6.4.2/qpy/QtQuick/qpyquick_chimera_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1601 2023-02-04 11:48:42.699168 PyQt6-6.4.2/qpy/QtQuick/qpyquick_chimera_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     2528 2023-02-04 11:48:42.697328 PyQt6-6.4.2/qpy/QtQuick/qpyquick_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2490 2023-02-04 11:48:42.698663 PyQt6-6.4.2/qpy/QtQuick/qpyquick_register_type.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1297 2023-02-04 11:48:42.704809 PyQt6-6.4.2/qpy/QtQuick/qpyquick_register_type.h
--rw-r--r--   0 phil       (501) staff       (20)     6763 2023-02-04 11:48:42.702223 PyQt6-6.4.2/qpy/QtQuick/qpyquickframebufferobject.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3136 2023-02-04 11:48:42.698140 PyQt6-6.4.2/qpy/QtQuick/qpyquickframebufferobject.h
--rw-r--r--   0 phil       (501) staff       (20)     7803 2023-02-04 11:48:42.706167 PyQt6-6.4.2/qpy/QtQuick/qpyquickitem.cpp
--rw-r--r--   0 phil       (501) staff       (20)     3255 2023-02-04 11:48:42.706837 PyQt6-6.4.2/qpy/QtQuick/qpyquickitem.h
--rw-r--r--   0 phil       (501) staff       (20)     6215 2023-02-04 11:48:42.700105 PyQt6-6.4.2/qpy/QtQuick/qpyquickpainteditem.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2873 2023-02-04 11:48:42.702884 PyQt6-6.4.2/qpy/QtQuick/qpyquickpainteditem.h
--rw-r--r--   0 phil       (501) staff       (20)     5020 2023-02-04 11:48:42.703782 PyQt6-6.4.2/qpy/QtQuick/qpyquickview.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2326 2023-02-04 11:48:42.708455 PyQt6-6.4.2/qpy/QtQuick/qpyquickview.h
--rw-r--r--   0 phil       (501) staff       (20)     5160 2023-02-04 11:48:42.707653 PyQt6-6.4.2/qpy/QtQuick/qpyquickwindow.cpp
--rw-r--r--   0 phil       (501) staff       (20)     2396 2023-02-04 11:48:42.704399 PyQt6-6.4.2/qpy/QtQuick/qpyquickwindow.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.099238 PyQt6-6.4.2/qpy/QtWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     1008 2023-02-04 11:48:42.709639 PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_api.h
--rw-r--r--   0 phil       (501) staff       (20)     1805 2023-02-04 11:48:42.710719 PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1247 2023-02-04 11:48:42.711810 PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_chimera_helpers.h
--rw-r--r--   0 phil       (501) staff       (20)     1703 2023-02-04 11:48:42.712635 PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_post_init.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1195 2023-02-04 11:48:42.710222 PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp
--rw-r--r--   0 phil       (501) staff       (20)     1147 2023-02-04 11:48:42.712240 PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_qaction_helpers.h
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.432980 PyQt6-6.4.2/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.248827 PyQt6-6.4.2/sip/QAxContainer/
--rw-r--r--   0 phil       (501) staff       (20)     1998 2023-02-04 11:48:49.991296 PyQt6-6.4.2/sip/QAxContainer/QAxContainermod.sip
--rw-r--r--   0 phil       (501) staff       (20)     4938 2023-02-04 11:48:49.992061 PyQt6-6.4.2/sip/QAxContainer/qaxbase.sip
--rw-r--r--   0 phil       (501) staff       (20)     2540 2023-02-04 11:48:49.993570 PyQt6-6.4.2/sip/QAxContainer/qaxobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1251 2023-02-04 11:48:49.992501 PyQt6-6.4.2/sip/QAxContainer/qaxobjectinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     2350 2023-02-04 11:48:49.993030 PyQt6-6.4.2/sip/QAxContainer/qaxwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.215500 PyQt6-6.4.2/sip/QtBluetooth/
--rw-r--r--   0 phil       (501) staff       (20)     2777 2023-02-04 11:48:49.887837 PyQt6-6.4.2/sip/QtBluetooth/QtBluetoothmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1559 2023-02-04 11:48:49.886822 PyQt6-6.4.2/sip/QtBluetooth/qbluetooth.sip
--rw-r--r--   0 phil       (501) staff       (20)     1673 2023-02-04 11:48:49.877999 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothaddress.sip
--rw-r--r--   0 phil       (501) staff       (20)     2670 2023-02-04 11:48:49.882455 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip
--rw-r--r--   0 phil       (501) staff       (20)     6598 2023-02-04 11:48:49.876019 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothdeviceinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1541 2023-02-04 11:48:49.889532 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothhostinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2570 2023-02-04 11:48:49.887378 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothlocaldevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3360 2023-02-04 11:48:49.888473 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     2467 2023-02-04 11:48:49.880173 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip
--rw-r--r--   0 phil       (501) staff       (20)     3324 2023-02-04 11:48:49.890321 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothserviceinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     5134 2023-02-04 11:48:49.876824 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     9422 2023-02-04 11:48:49.885666 PyQt6-6.4.2/sip/QtBluetooth/qbluetoothuuid.sip
--rw-r--r--   0 phil       (501) staff       (20)     2334 2023-02-04 11:48:49.874856 PyQt6-6.4.2/sip/QtBluetooth/qlowenergyadvertisingdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3006 2023-02-04 11:48:49.874333 PyQt6-6.4.2/sip/QtBluetooth/qlowenergyadvertisingparameters.sip
--rw-r--r--   0 phil       (501) staff       (20)     2262 2023-02-04 11:48:49.878524 PyQt6-6.4.2/sip/QtBluetooth/qlowenergycharacteristic.sip
--rw-r--r--   0 phil       (501) staff       (20)     2472 2023-02-04 11:48:49.886144 PyQt6-6.4.2/sip/QtBluetooth/qlowenergycharacteristicdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1843 2023-02-04 11:48:49.888908 PyQt6-6.4.2/sip/QtBluetooth/qlowenergyconnectionparameters.sip
--rw-r--r--   0 phil       (501) staff       (20)     4203 2023-02-04 11:48:49.877520 PyQt6-6.4.2/sip/QtBluetooth/qlowenergycontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1568 2023-02-04 11:48:49.882998 PyQt6-6.4.2/sip/QtBluetooth/qlowenergydescriptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2201 2023-02-04 11:48:49.884124 PyQt6-6.4.2/sip/QtBluetooth/qlowenergydescriptordata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3661 2023-02-04 11:48:49.880907 PyQt6-6.4.2/sip/QtBluetooth/qlowenergyservice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2201 2023-02-04 11:48:49.883646 PyQt6-6.4.2/sip/QtBluetooth/qlowenergyservicedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3358 2023-02-04 11:48:49.881785 PyQt6-6.4.2/sip/QtBluetooth/qpybluetooth_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     4039 2023-02-04 11:48:49.879516 PyQt6-6.4.2/sip/QtBluetooth/qpybluetooth_qmultihash.sip
--rw-r--r--   0 phil       (501) staff       (20)     2860 2023-02-04 11:48:49.873675 PyQt6-6.4.2/sip/QtBluetooth/qpybluetooth_quint128.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.428839 PyQt6-6.4.2/sip/QtCore/
--rw-r--r--   0 phil       (501) staff       (20)     6207 2023-02-04 11:48:50.579733 PyQt6-6.4.2/sip/QtCore/QtCoremod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2557 2023-02-04 11:48:50.691456 PyQt6-6.4.2/sip/QtCore/qabstractanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     2449 2023-02-04 11:48:50.648336 PyQt6-6.4.2/sip/QtCore/qabstracteventdispatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)    13972 2023-02-04 11:48:50.531455 PyQt6-6.4.2/sip/QtCore/qabstractitemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1335 2023-02-04 11:48:50.690030 PyQt6-6.4.2/sip/QtCore/qabstractnativeeventfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3493 2023-02-04 11:48:50.676010 PyQt6-6.4.2/sip/QtCore/qabstractproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1649 2023-02-04 11:48:50.542796 PyQt6-6.4.2/sip/QtCore/qanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     2718 2023-02-04 11:48:50.494759 PyQt6-6.4.2/sip/QtCore/qanystringview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1338 2023-02-04 11:48:50.543624 PyQt6-6.4.2/sip/QtCore/qbasictimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2909 2023-02-04 11:48:50.673648 PyQt6-6.4.2/sip/QtCore/qbitarray.sip
--rw-r--r--   0 phil       (501) staff       (20)     3628 2023-02-04 11:48:50.523940 PyQt6-6.4.2/sip/QtCore/qbuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)    14158 2023-02-04 11:48:50.643111 PyQt6-6.4.2/sip/QtCore/qbytearray.sip
--rw-r--r--   0 phil       (501) staff       (20)     1144 2023-02-04 11:48:50.543186 PyQt6-6.4.2/sip/QtCore/qbytearrayalgorithms.sip
--rw-r--r--   0 phil       (501) staff       (20)     2976 2023-02-04 11:48:50.532381 PyQt6-6.4.2/sip/QtCore/qbytearraylist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1906 2023-02-04 11:48:50.679478 PyQt6-6.4.2/sip/QtCore/qbytearraymatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2023-02-04 11:48:50.684688 PyQt6-6.4.2/sip/QtCore/qbytearrayview.sip
--rw-r--r--   0 phil       (501) staff       (20)     3336 2023-02-04 11:48:50.495924 PyQt6-6.4.2/sip/QtCore/qcalendar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2452 2023-02-04 11:48:50.598866 PyQt6-6.4.2/sip/QtCore/qcborcommon.sip
--rw-r--r--   0 phil       (501) staff       (20)     3894 2023-02-04 11:48:50.680297 PyQt6-6.4.2/sip/QtCore/qcborstreamreader.sip
--rw-r--r--   0 phil       (501) staff       (20)     2475 2023-02-04 11:48:50.639532 PyQt6-6.4.2/sip/QtCore/qcborstreamwriter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1591 2023-02-04 11:48:50.583610 PyQt6-6.4.2/sip/QtCore/qchar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2161 2023-02-04 11:48:50.541729 PyQt6-6.4.2/sip/QtCore/qcollator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2203 2023-02-04 11:48:50.643614 PyQt6-6.4.2/sip/QtCore/qcommandlineoption.sip
--rw-r--r--   0 phil       (501) staff       (20)     2825 2023-02-04 11:48:50.674212 PyQt6-6.4.2/sip/QtCore/qcommandlineparser.sip
--rw-r--r--   0 phil       (501) staff       (20)     4086 2023-02-04 11:48:50.650898 PyQt6-6.4.2/sip/QtCore/qconcatenatetablesproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)    10878 2023-02-04 11:48:50.549306 PyQt6-6.4.2/sip/QtCore/qcoreapplication.sip
--rw-r--r--   0 phil       (501) staff       (20)     6998 2023-02-04 11:48:50.574577 PyQt6-6.4.2/sip/QtCore/qcoreevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2298 2023-02-04 11:48:50.555074 PyQt6-6.4.2/sip/QtCore/qcryptographichash.sip
--rw-r--r--   0 phil       (501) staff       (20)    10967 2023-02-04 11:48:50.578767 PyQt6-6.4.2/sip/QtCore/qdatastream.sip
--rw-r--r--   0 phil       (501) staff       (20)    15238 2023-02-04 11:48:50.634626 PyQt6-6.4.2/sip/QtCore/qdatetime.sip
--rw-r--r--   0 phil       (501) staff       (20)     2791 2023-02-04 11:48:50.638439 PyQt6-6.4.2/sip/QtCore/qdeadlinetimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     6102 2023-02-04 11:48:50.581264 PyQt6-6.4.2/sip/QtCore/qdir.sip
--rw-r--r--   0 phil       (501) staff       (20)     2019 2023-02-04 11:48:50.497686 PyQt6-6.4.2/sip/QtCore/qdiriterator.sip
--rw-r--r--   0 phil       (501) staff       (20)     6671 2023-02-04 11:48:50.529264 PyQt6-6.4.2/sip/QtCore/qeasingcurve.sip
--rw-r--r--   0 phil       (501) staff       (20)     1833 2023-02-04 11:48:50.576756 PyQt6-6.4.2/sip/QtCore/qelapsedtimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2197 2023-02-04 11:48:50.649766 PyQt6-6.4.2/sip/QtCore/qeventloop.sip
--rw-r--r--   0 phil       (501) staff       (20)     3031 2023-02-04 11:48:50.682177 PyQt6-6.4.2/sip/QtCore/qfile.sip
--rw-r--r--   0 phil       (501) staff       (20)     6316 2023-02-04 11:48:50.637517 PyQt6-6.4.2/sip/QtCore/qfiledevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3371 2023-02-04 11:48:50.582653 PyQt6-6.4.2/sip/QtCore/qfileinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1365 2023-02-04 11:48:50.626970 PyQt6-6.4.2/sip/QtCore/qfileselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     1597 2023-02-04 11:48:50.627459 PyQt6-6.4.2/sip/QtCore/qfilesystemwatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-02-04 11:48:50.524755 PyQt6-6.4.2/sip/QtCore/qflags.sip
--rw-r--r--   0 phil       (501) staff       (20)     4442 2023-02-04 11:48:50.635688 PyQt6-6.4.2/sip/QtCore/qglobal.sip
--rw-r--r--   0 phil       (501) staff       (20)     3095 2023-02-04 11:48:50.686898 PyQt6-6.4.2/sip/QtCore/qidentityproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)    12510 2023-02-04 11:48:50.598076 PyQt6-6.4.2/sip/QtCore/qiodevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1380 2023-02-04 11:48:50.645480 PyQt6-6.4.2/sip/QtCore/qiodevicebase.sip
--rw-r--r--   0 phil       (501) staff       (20)     8829 2023-02-04 11:48:50.686436 PyQt6-6.4.2/sip/QtCore/qitemselectionmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     3263 2023-02-04 11:48:50.640636 PyQt6-6.4.2/sip/QtCore/qjsonarray.sip
--rw-r--r--   0 phil       (501) staff       (20)     2862 2023-02-04 11:48:50.594909 PyQt6-6.4.2/sip/QtCore/qjsondocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     3500 2023-02-04 11:48:50.536814 PyQt6-6.4.2/sip/QtCore/qjsonobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2892 2023-02-04 11:48:50.630473 PyQt6-6.4.2/sip/QtCore/qjsonvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     2418 2023-02-04 11:48:50.593819 PyQt6-6.4.2/sip/QtCore/qlibrary.sip
--rw-r--r--   0 phil       (501) staff       (20)     1606 2023-02-04 11:48:50.596298 PyQt6-6.4.2/sip/QtCore/qlibraryinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     5198 2023-02-04 11:48:50.595828 PyQt6-6.4.2/sip/QtCore/qline.sip
--rw-r--r--   0 phil       (501) staff       (20)    27874 2023-02-04 11:48:50.554388 PyQt6-6.4.2/sip/QtCore/qlocale.sip
--rw-r--r--   0 phil       (501) staff       (20)     1671 2023-02-04 11:48:50.532925 PyQt6-6.4.2/sip/QtCore/qlockfile.sip
--rw-r--r--   0 phil       (501) staff       (20)     5565 2023-02-04 11:48:50.649260 PyQt6-6.4.2/sip/QtCore/qlogging.sip
--rw-r--r--   0 phil       (501) staff       (20)     1612 2023-02-04 11:48:50.526384 PyQt6-6.4.2/sip/QtCore/qloggingcategory.sip
--rw-r--r--   0 phil       (501) staff       (20)     4347 2023-02-04 11:48:50.582039 PyQt6-6.4.2/sip/QtCore/qmargins.sip
--rw-r--r--   0 phil       (501) staff       (20)     1862 2023-02-04 11:48:50.680761 PyQt6-6.4.2/sip/QtCore/qmessageauthenticationcode.sip
--rw-r--r--   0 phil       (501) staff       (20)     8100 2023-02-04 11:48:50.632450 PyQt6-6.4.2/sip/QtCore/qmetaobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     3837 2023-02-04 11:48:50.550130 PyQt6-6.4.2/sip/QtCore/qmetatype.sip
--rw-r--r--   0 phil       (501) staff       (20)     1954 2023-02-04 11:48:50.497241 PyQt6-6.4.2/sip/QtCore/qmimedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     2082 2023-02-04 11:48:50.630945 PyQt6-6.4.2/sip/QtCore/qmimedatabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     1812 2023-02-04 11:48:50.626085 PyQt6-6.4.2/sip/QtCore/qmimetype.sip
--rw-r--r--   0 phil       (501) staff       (20)     1527 2023-02-04 11:48:50.496405 PyQt6-6.4.2/sip/QtCore/qmutex.sip
--rw-r--r--   0 phil       (501) staff       (20)     1961 2023-02-04 11:48:50.692577 PyQt6-6.4.2/sip/QtCore/qmutexlocker.sip
--rw-r--r--   0 phil       (501) staff       (20)    34028 2023-02-04 11:48:50.590783 PyQt6-6.4.2/sip/QtCore/qnamespace.sip
--rw-r--r--   0 phil       (501) staff       (20)     1150 2023-02-04 11:48:50.626499 PyQt6-6.4.2/sip/QtCore/qnumeric.sip
--rw-r--r--   0 phil       (501) staff       (20)    20046 2023-02-04 11:48:50.535868 PyQt6-6.4.2/sip/QtCore/qobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1248 2023-02-04 11:48:50.647810 PyQt6-6.4.2/sip/QtCore/qobjectcleanuphandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     7642 2023-02-04 11:48:50.646412 PyQt6-6.4.2/sip/QtCore/qobjectdefs.sip
--rw-r--r--   0 phil       (501) staff       (20)     7259 2023-02-04 11:48:50.537908 PyQt6-6.4.2/sip/QtCore/qoperatingsystemversion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1502 2023-02-04 11:48:50.545239 PyQt6-6.4.2/sip/QtCore/qparallelanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     1373 2023-02-04 11:48:50.631386 PyQt6-6.4.2/sip/QtCore/qpauseanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1555 2023-02-04 11:48:50.496801 PyQt6-6.4.2/sip/QtCore/qpluginloader.sip
--rw-r--r--   0 phil       (501) staff       (20)     4684 2023-02-04 11:48:50.644491 PyQt6-6.4.2/sip/QtCore/qpoint.sip
--rw-r--r--   0 phil       (501) staff       (20)     7887 2023-02-04 11:48:50.678552 PyQt6-6.4.2/sip/QtCore/qprocess.sip
--rw-r--r--   0 phil       (501) staff       (20)     1695 2023-02-04 11:48:50.625629 PyQt6-6.4.2/sip/QtCore/qpropertyanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)    11135 2023-02-04 11:48:50.688997 PyQt6-6.4.2/sip/QtCore/qpycore_qhash.sip
--rw-r--r--   0 phil       (501) staff       (20)    28558 2023-02-04 11:48:50.604335 PyQt6-6.4.2/sip/QtCore/qpycore_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)    10053 2023-02-04 11:48:50.684055 PyQt6-6.4.2/sip/QtCore/qpycore_qmap.sip
--rw-r--r--   0 phil       (501) staff       (20)     5229 2023-02-04 11:48:50.544836 PyQt6-6.4.2/sip/QtCore/qpycore_qset.sip
--rw-r--r--   0 phil       (501) staff       (20)    11619 2023-02-04 11:48:50.541078 PyQt6-6.4.2/sip/QtCore/qpycore_std_pair.sip
--rw-r--r--   0 phil       (501) staff       (20)      976 2023-02-04 11:48:50.650167 PyQt6-6.4.2/sip/QtCore/qpycore_virtual_error_handler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1863 2023-02-04 11:48:50.545678 PyQt6-6.4.2/sip/QtCore/qrandom.sip
--rw-r--r--   0 phil       (501) staff       (20)     2706 2023-02-04 11:48:50.636319 PyQt6-6.4.2/sip/QtCore/qreadwritelock.sip
--rw-r--r--   0 phil       (501) staff       (20)     9654 2023-02-04 11:48:50.677397 PyQt6-6.4.2/sip/QtCore/qrect.sip
--rw-r--r--   0 phil       (501) staff       (20)     6701 2023-02-04 11:48:50.690903 PyQt6-6.4.2/sip/QtCore/qregularexpression.sip
--rw-r--r--   0 phil       (501) staff       (20)     2661 2023-02-04 11:48:50.575282 PyQt6-6.4.2/sip/QtCore/qresource.sip
--rw-r--r--   0 phil       (501) staff       (20)     1718 2023-02-04 11:48:50.594255 PyQt6-6.4.2/sip/QtCore/qrunnable.sip
--rw-r--r--   0 phil       (501) staff       (20)     2390 2023-02-04 11:48:50.685196 PyQt6-6.4.2/sip/QtCore/qsavefile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1620 2023-02-04 11:48:50.647345 PyQt6-6.4.2/sip/QtCore/qsemaphore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1721 2023-02-04 11:48:50.679000 PyQt6-6.4.2/sip/QtCore/qsequentialanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     5109 2023-02-04 11:48:50.606107 PyQt6-6.4.2/sip/QtCore/qsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     2332 2023-02-04 11:48:50.592660 PyQt6-6.4.2/sip/QtCore/qsharedmemory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1641 2023-02-04 11:48:50.644932 PyQt6-6.4.2/sip/QtCore/qsignalmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     5173 2023-02-04 11:48:50.605295 PyQt6-6.4.2/sip/QtCore/qsize.sip
--rw-r--r--   0 phil       (501) staff       (20)     1673 2023-02-04 11:48:50.525346 PyQt6-6.4.2/sip/QtCore/qsocketnotifier.sip
--rw-r--r--   0 phil       (501) staff       (20)     5908 2023-02-04 11:48:50.593341 PyQt6-6.4.2/sip/QtCore/qsortfilterproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2023-02-04 11:48:50.542342 PyQt6-6.4.2/sip/QtCore/qstandardpaths.sip
--rw-r--r--   0 phil       (501) staff       (20)     1966 2023-02-04 11:48:50.576221 PyQt6-6.4.2/sip/QtCore/qstorageinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1485 2023-02-04 11:48:50.527774 PyQt6-6.4.2/sip/QtCore/qstring.sip
--rw-r--r--   0 phil       (501) staff       (20)     3205 2023-02-04 11:48:50.538633 PyQt6-6.4.2/sip/QtCore/qstringconverter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2134 2023-02-04 11:48:50.675488 PyQt6-6.4.2/sip/QtCore/qstringconverter_base.sip
--rw-r--r--   0 phil       (501) staff       (20)     2937 2023-02-04 11:48:50.629697 PyQt6-6.4.2/sip/QtCore/qstringlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     2403 2023-02-04 11:48:50.591747 PyQt6-6.4.2/sip/QtCore/qstringlistmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1537 2023-02-04 11:48:50.547792 PyQt6-6.4.2/sip/QtCore/qstringview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1572 2023-02-04 11:48:50.525891 PyQt6-6.4.2/sip/QtCore/qsysinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1790 2023-02-04 11:48:50.555544 PyQt6-6.4.2/sip/QtCore/qsystemsemaphore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1463 2023-02-04 11:48:50.599289 PyQt6-6.4.2/sip/QtCore/qtemporarydir.sip
--rw-r--r--   0 phil       (501) staff       (20)     1798 2023-02-04 11:48:50.529772 PyQt6-6.4.2/sip/QtCore/qtemporaryfile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1998 2023-02-04 11:48:50.646895 PyQt6-6.4.2/sip/QtCore/qtextboundaryfinder.sip
--rw-r--r--   0 phil       (501) staff       (20)     5603 2023-02-04 11:48:50.681669 PyQt6-6.4.2/sip/QtCore/qtextstream.sip
--rw-r--r--   0 phil       (501) staff       (20)     2691 2023-02-04 11:48:50.584362 PyQt6-6.4.2/sip/QtCore/qthread.sip
--rw-r--r--   0 phil       (501) staff       (20)     4994 2023-02-04 11:48:50.546644 PyQt6-6.4.2/sip/QtCore/qthreadpool.sip
--rw-r--r--   0 phil       (501) staff       (20)     2431 2023-02-04 11:48:50.495328 PyQt6-6.4.2/sip/QtCore/qtimeline.sip
--rw-r--r--   0 phil       (501) staff       (20)     2585 2023-02-04 11:48:50.547291 PyQt6-6.4.2/sip/QtCore/qtimer.sip
--rw-r--r--   0 phil       (501) staff       (20)     4892 2023-02-04 11:48:50.527199 PyQt6-6.4.2/sip/QtCore/qtimezone.sip
--rw-r--r--   0 phil       (501) staff       (20)     1837 2023-02-04 11:48:50.592142 PyQt6-6.4.2/sip/QtCore/qtranslator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2945 2023-02-04 11:48:50.583126 PyQt6-6.4.2/sip/QtCore/qtransposeproxymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     7344 2023-02-04 11:48:50.628364 PyQt6-6.4.2/sip/QtCore/qurl.sip
--rw-r--r--   0 phil       (501) staff       (20)     2784 2023-02-04 11:48:50.575777 PyQt6-6.4.2/sip/QtCore/qurlquery.sip
--rw-r--r--   0 phil       (501) staff       (20)     3479 2023-02-04 11:48:50.689641 PyQt6-6.4.2/sip/QtCore/quuid.sip
--rw-r--r--   0 phil       (501) staff       (20)     3169 2023-02-04 11:48:50.580361 PyQt6-6.4.2/sip/QtCore/qvariant.sip
--rw-r--r--   0 phil       (501) staff       (20)     2197 2023-02-04 11:48:50.692042 PyQt6-6.4.2/sip/QtCore/qvariantanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     3856 2023-02-04 11:48:50.674888 PyQt6-6.4.2/sip/QtCore/qversionnumber.sip
--rw-r--r--   0 phil       (501) staff       (20)     1578 2023-02-04 11:48:50.591323 PyQt6-6.4.2/sip/QtCore/qwaitcondition.sip
--rw-r--r--   0 phil       (501) staff       (20)     1577 2023-02-04 11:48:50.628915 PyQt6-6.4.2/sip/QtCore/qwineventnotifier.sip
--rw-r--r--   0 phil       (501) staff       (20)    13357 2023-02-04 11:48:50.625128 PyQt6-6.4.2/sip/QtCore/qxmlstream.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.318826 PyQt6-6.4.2/sip/QtDBus/
--rw-r--r--   0 phil       (501) staff       (20)     2340 2023-02-04 11:48:50.249389 PyQt6-6.4.2/sip/QtDBus/QtDBusmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1271 2023-02-04 11:48:50.244629 PyQt6-6.4.2/sip/QtDBus/qdbusabstractadaptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     7394 2023-02-04 11:48:50.247960 PyQt6-6.4.2/sip/QtDBus/qdbusabstractinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     4871 2023-02-04 11:48:50.245494 PyQt6-6.4.2/sip/QtDBus/qdbusargument.sip
--rw-r--r--   0 phil       (501) staff       (20)     9428 2023-02-04 11:48:50.243020 PyQt6-6.4.2/sip/QtDBus/qdbusconnection.sip
--rw-r--r--   0 phil       (501) staff       (20)     2976 2023-02-04 11:48:50.246516 PyQt6-6.4.2/sip/QtDBus/qdbusconnectioninterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     1933 2023-02-04 11:48:50.248898 PyQt6-6.4.2/sip/QtDBus/qdbuserror.sip
--rw-r--r--   0 phil       (501) staff       (20)     2507 2023-02-04 11:48:50.243589 PyQt6-6.4.2/sip/QtDBus/qdbusextratypes.sip
--rw-r--r--   0 phil       (501) staff       (20)     1299 2023-02-04 11:48:50.246894 PyQt6-6.4.2/sip/QtDBus/qdbusinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     3015 2023-02-04 11:48:50.244203 PyQt6-6.4.2/sip/QtDBus/qdbusmessage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1745 2023-02-04 11:48:50.245945 PyQt6-6.4.2/sip/QtDBus/qdbuspendingcall.sip
--rw-r--r--   0 phil       (501) staff       (20)     2225 2023-02-04 11:48:50.248406 PyQt6-6.4.2/sip/QtDBus/qdbusservicewatcher.sip
--rw-r--r--   0 phil       (501) staff       (20)     1450 2023-02-04 11:48:50.241244 PyQt6-6.4.2/sip/QtDBus/qdbusunixfiledescriptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1739 2023-02-04 11:48:50.241765 PyQt6-6.4.2/sip/QtDBus/qpydbuspendingreply.sip
--rw-r--r--   0 phil       (501) staff       (20)     5291 2023-02-04 11:48:50.240789 PyQt6-6.4.2/sip/QtDBus/qpydbusreply.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.240588 PyQt6-6.4.2/sip/QtDesigner/
--rw-r--r--   0 phil       (501) staff       (20)     2809 2023-02-04 11:48:49.979671 PyQt6-6.4.2/sip/QtDesigner/QtDesignermod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1493 2023-02-04 11:48:49.946827 PyQt6-6.4.2/sip/QtDesigner/abstractactioneditor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-02-04 11:48:49.980465 PyQt6-6.4.2/sip/QtDesigner/abstractformbuilder.sip
--rw-r--r--   0 phil       (501) staff       (20)     2021 2023-02-04 11:48:49.977954 PyQt6-6.4.2/sip/QtDesigner/abstractformeditor.sip
--rw-r--r--   0 phil       (501) staff       (20)     4737 2023-02-04 11:48:49.947471 PyQt6-6.4.2/sip/QtDesigner/abstractformwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     2532 2023-02-04 11:48:49.976261 PyQt6-6.4.2/sip/QtDesigner/abstractformwindowcursor.sip
--rw-r--r--   0 phil       (501) staff       (20)     3286 2023-02-04 11:48:49.944703 PyQt6-6.4.2/sip/QtDesigner/abstractformwindowmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     1402 2023-02-04 11:48:49.978744 PyQt6-6.4.2/sip/QtDesigner/abstractobjectinspector.sip
--rw-r--r--   0 phil       (501) staff       (20)     1736 2023-02-04 11:48:49.979175 PyQt6-6.4.2/sip/QtDesigner/abstractpropertyeditor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1397 2023-02-04 11:48:49.977077 PyQt6-6.4.2/sip/QtDesigner/abstractwidgetbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     1633 2023-02-04 11:48:49.977509 PyQt6-6.4.2/sip/QtDesigner/container.sip
--rw-r--r--   0 phil       (501) staff       (20)     1884 2023-02-04 11:48:49.975333 PyQt6-6.4.2/sip/QtDesigner/customwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1438 2023-02-04 11:48:49.978351 PyQt6-6.4.2/sip/QtDesigner/default_extensionfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1571 2023-02-04 11:48:49.975759 PyQt6-6.4.2/sip/QtDesigner/extension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1345 2023-02-04 11:48:49.973897 PyQt6-6.4.2/sip/QtDesigner/formbuilder.sip
--rw-r--r--   0 phil       (501) staff       (20)     1993 2023-02-04 11:48:49.974838 PyQt6-6.4.2/sip/QtDesigner/membersheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     2084 2023-02-04 11:48:49.945949 PyQt6-6.4.2/sip/QtDesigner/propertysheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     3397 2023-02-04 11:48:49.946453 PyQt6-6.4.2/sip/QtDesigner/qextensionmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     1228 2023-02-04 11:48:49.944147 PyQt6-6.4.2/sip/QtDesigner/qpydesignercontainerextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1308 2023-02-04 11:48:49.945479 PyQt6-6.4.2/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip
--rw-r--r--   0 phil       (501) staff       (20)     1235 2023-02-04 11:48:49.973424 PyQt6-6.4.2/sip/QtDesigner/qpydesignercustomwidgetplugin.sip
--rw-r--r--   0 phil       (501) staff       (20)     1242 2023-02-04 11:48:49.980082 PyQt6-6.4.2/sip/QtDesigner/qpydesignermembersheetextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1259 2023-02-04 11:48:49.976688 PyQt6-6.4.2/sip/QtDesigner/qpydesignerpropertysheetextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1221 2023-02-04 11:48:49.974338 PyQt6-6.4.2/sip/QtDesigner/qpydesignertaskmenuextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1300 2023-02-04 11:48:49.945078 PyQt6-6.4.2/sip/QtDesigner/taskmenu.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.299173 PyQt6-6.4.2/sip/QtGui/
--rw-r--r--   0 phil       (501) staff       (20)     4147 2023-02-04 11:48:50.147902 PyQt6-6.4.2/sip/QtGui/QtGuimod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1404 2023-02-04 11:48:50.145531 PyQt6-6.4.2/sip/QtGui/opengl_types.sip
--rw-r--r--   0 phil       (501) staff       (20)     1809 2023-02-04 11:48:50.076626 PyQt6-6.4.2/sip/QtGui/qabstractfileiconprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)     3726 2023-02-04 11:48:50.073617 PyQt6-6.4.2/sip/QtGui/qabstracttextdocumentlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     4672 2023-02-04 11:48:50.130269 PyQt6-6.4.2/sip/QtGui/qaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     1946 2023-02-04 11:48:50.077756 PyQt6-6.4.2/sip/QtGui/qactiongroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     1568 2023-02-04 11:48:50.150686 PyQt6-6.4.2/sip/QtGui/qbackingstore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1848 2023-02-04 11:48:50.088678 PyQt6-6.4.2/sip/QtGui/qbitmap.sip
--rw-r--r--   0 phil       (501) staff       (20)    10739 2023-02-04 11:48:50.185006 PyQt6-6.4.2/sip/QtGui/qbrush.sip
--rw-r--r--   0 phil       (501) staff       (20)     3492 2023-02-04 11:48:50.185600 PyQt6-6.4.2/sip/QtGui/qclipboard.sip
--rw-r--r--   0 phil       (501) staff       (20)    12351 2023-02-04 11:48:50.103135 PyQt6-6.4.2/sip/QtGui/qcolor.sip
--rw-r--r--   0 phil       (501) staff       (20)     4476 2023-02-04 11:48:50.080987 PyQt6-6.4.2/sip/QtGui/qcolorspace.sip
--rw-r--r--   0 phil       (501) staff       (20)     1554 2023-02-04 11:48:50.094176 PyQt6-6.4.2/sip/QtGui/qcolortransform.sip
--rw-r--r--   0 phil       (501) staff       (20)     3042 2023-02-04 11:48:50.132990 PyQt6-6.4.2/sip/QtGui/qcursor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2418 2023-02-04 11:48:50.174912 PyQt6-6.4.2/sip/QtGui/qdesktopservices.sip
--rw-r--r--   0 phil       (501) staff       (20)     1971 2023-02-04 11:48:50.180859 PyQt6-6.4.2/sip/QtGui/qdrag.sip
--rw-r--r--   0 phil       (501) staff       (20)    23005 2023-02-04 11:48:50.178702 PyQt6-6.4.2/sip/QtGui/qevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2495 2023-02-04 11:48:50.141267 PyQt6-6.4.2/sip/QtGui/qeventpoint.sip
--rw-r--r--   0 phil       (501) staff       (20)     4840 2023-02-04 11:48:50.097396 PyQt6-6.4.2/sip/QtGui/qfilesystemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     5846 2023-02-04 11:48:50.079521 PyQt6-6.4.2/sip/QtGui/qfont.sip
--rw-r--r--   0 phil       (501) staff       (20)     3645 2023-02-04 11:48:50.080299 PyQt6-6.4.2/sip/QtGui/qfontdatabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     1495 2023-02-04 11:48:50.083902 PyQt6-6.4.2/sip/QtGui/qfontinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     6681 2023-02-04 11:48:50.098413 PyQt6-6.4.2/sip/QtGui/qfontmetrics.sip
--rw-r--r--   0 phil       (501) staff       (20)    25528 2023-02-04 11:48:50.136659 PyQt6-6.4.2/sip/QtGui/qgenericmatrix.sip
--rw-r--r--   0 phil       (501) staff       (20)     2324 2023-02-04 11:48:50.141798 PyQt6-6.4.2/sip/QtGui/qglyphrun.sip
--rw-r--r--   0 phil       (501) staff       (20)     9541 2023-02-04 11:48:50.182227 PyQt6-6.4.2/sip/QtGui/qguiapplication.sip
--rw-r--r--   0 phil       (501) staff       (20)     4245 2023-02-04 11:48:50.140705 PyQt6-6.4.2/sip/QtGui/qicon.sip
--rw-r--r--   0 phil       (501) staff       (20)     2384 2023-02-04 11:48:50.081503 PyQt6-6.4.2/sip/QtGui/qiconengine.sip
--rw-r--r--   0 phil       (501) staff       (20)    13954 2023-02-04 11:48:50.087147 PyQt6-6.4.2/sip/QtGui/qimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     2751 2023-02-04 11:48:50.126159 PyQt6-6.4.2/sip/QtGui/qimageiohandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     3480 2023-02-04 11:48:50.148518 PyQt6-6.4.2/sip/QtGui/qimagereader.sip
--rw-r--r--   0 phil       (501) staff       (20)     2666 2023-02-04 11:48:50.132429 PyQt6-6.4.2/sip/QtGui/qimagewriter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2591 2023-02-04 11:48:50.085460 PyQt6-6.4.2/sip/QtGui/qinputdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2303 2023-02-04 11:48:50.180378 PyQt6-6.4.2/sip/QtGui/qinputmethod.sip
--rw-r--r--   0 phil       (501) staff       (20)     7031 2023-02-04 11:48:50.143859 PyQt6-6.4.2/sip/QtGui/qkeysequence.sip
--rw-r--r--   0 phil       (501) staff       (20)     9803 2023-02-04 11:48:50.082872 PyQt6-6.4.2/sip/QtGui/qmatrix4x4.sip
--rw-r--r--   0 phil       (501) staff       (20)     2857 2023-02-04 11:48:50.179356 PyQt6-6.4.2/sip/QtGui/qmovie.sip
--rw-r--r--   0 phil       (501) staff       (20)     1585 2023-02-04 11:48:50.139913 PyQt6-6.4.2/sip/QtGui/qoffscreensurface.sip
--rw-r--r--   0 phil       (501) staff       (20)     2580 2023-02-04 11:48:50.090103 PyQt6-6.4.2/sip/QtGui/qopenglcontext.sip
--rw-r--r--   0 phil       (501) staff       (20)     1686 2023-02-04 11:48:50.083424 PyQt6-6.4.2/sip/QtGui/qpagedpaintdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3104 2023-02-04 11:48:50.093288 PyQt6-6.4.2/sip/QtGui/qpagelayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     2145 2023-02-04 11:48:50.129463 PyQt6-6.4.2/sip/QtGui/qpageranges.sip
--rw-r--r--   0 phil       (501) staff       (20)     5591 2023-02-04 11:48:50.125566 PyQt6-6.4.2/sip/QtGui/qpagesize.sip
--rw-r--r--   0 phil       (501) staff       (20)     1994 2023-02-04 11:48:50.098911 PyQt6-6.4.2/sip/QtGui/qpaintdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1415 2023-02-04 11:48:50.147091 PyQt6-6.4.2/sip/QtGui/qpaintdevicewindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     5665 2023-02-04 11:48:50.149430 PyQt6-6.4.2/sip/QtGui/qpaintengine.sip
--rw-r--r--   0 phil       (501) staff       (20)    20805 2023-02-04 11:48:50.128500 PyQt6-6.4.2/sip/QtGui/qpainter.sip
--rw-r--r--   0 phil       (501) staff       (20)     6554 2023-02-04 11:48:50.137790 PyQt6-6.4.2/sip/QtGui/qpainterpath.sip
--rw-r--r--   0 phil       (501) staff       (20)     4511 2023-02-04 11:48:50.078467 PyQt6-6.4.2/sip/QtGui/qpalette.sip
--rw-r--r--   0 phil       (501) staff       (20)     1885 2023-02-04 11:48:50.104990 PyQt6-6.4.2/sip/QtGui/qpdfwriter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3397 2023-02-04 11:48:50.077276 PyQt6-6.4.2/sip/QtGui/qpen.sip
--rw-r--r--   0 phil       (501) staff       (20)     2021 2023-02-04 11:48:50.145087 PyQt6-6.4.2/sip/QtGui/qpicture.sip
--rw-r--r--   0 phil       (501) staff       (20)     5520 2023-02-04 11:48:50.124505 PyQt6-6.4.2/sip/QtGui/qpixelformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     4917 2023-02-04 11:48:50.045344 PyQt6-6.4.2/sip/QtGui/qpixmap.sip
--rw-r--r--   0 phil       (501) staff       (20)     2240 2023-02-04 11:48:50.103778 PyQt6-6.4.2/sip/QtGui/qpixmapcache.sip
--rw-r--r--   0 phil       (501) staff       (20)     2499 2023-02-04 11:48:50.179864 PyQt6-6.4.2/sip/QtGui/qpointingdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)    11953 2023-02-04 11:48:50.092729 PyQt6-6.4.2/sip/QtGui/qpolygon.sip
--rw-r--r--   0 phil       (501) staff       (20)     2719 2023-02-04 11:48:50.104561 PyQt6-6.4.2/sip/QtGui/qpygui_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     5076 2023-02-04 11:48:50.090882 PyQt6-6.4.2/sip/QtGui/qquaternion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1230 2023-02-04 11:48:50.138262 PyQt6-6.4.2/sip/QtGui/qrasterwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     3616 2023-02-04 11:48:50.089395 PyQt6-6.4.2/sip/QtGui/qrawfont.sip
--rw-r--r--   0 phil       (501) staff       (20)     3768 2023-02-04 11:48:50.142465 PyQt6-6.4.2/sip/QtGui/qregion.sip
--rw-r--r--   0 phil       (501) staff       (20)     1271 2023-02-04 11:48:50.044670 PyQt6-6.4.2/sip/QtGui/qrgb.sip
--rw-r--r--   0 phil       (501) staff       (20)     2141 2023-02-04 11:48:50.174418 PyQt6-6.4.2/sip/QtGui/qrgba64.sip
--rw-r--r--   0 phil       (501) staff       (20)     3073 2023-02-04 11:48:50.087773 PyQt6-6.4.2/sip/QtGui/qscreen.sip
--rw-r--r--   0 phil       (501) staff       (20)     1990 2023-02-04 11:48:50.146691 PyQt6-6.4.2/sip/QtGui/qsessionmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     6080 2023-02-04 11:48:50.150283 PyQt6-6.4.2/sip/QtGui/qshortcut.sip
--rw-r--r--   0 phil       (501) staff       (20)     9704 2023-02-04 11:48:50.099901 PyQt6-6.4.2/sip/QtGui/qstandarditemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1953 2023-02-04 11:48:50.093771 PyQt6-6.4.2/sip/QtGui/qstatictext.sip
--rw-r--r--   0 phil       (501) staff       (20)     2842 2023-02-04 11:48:50.173868 PyQt6-6.4.2/sip/QtGui/qstylehints.sip
--rw-r--r--   0 phil       (501) staff       (20)     1634 2023-02-04 11:48:50.088259 PyQt6-6.4.2/sip/QtGui/qsurface.sip
--rw-r--r--   0 phil       (501) staff       (20)     3651 2023-02-04 11:48:50.076152 PyQt6-6.4.2/sip/QtGui/qsurfaceformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     2965 2023-02-04 11:48:50.047625 PyQt6-6.4.2/sip/QtGui/qsyntaxhighlighter.sip
--rw-r--r--   0 phil       (501) staff       (20)     5531 2023-02-04 11:48:50.131128 PyQt6-6.4.2/sip/QtGui/qtextcursor.sip
--rw-r--r--   0 phil       (501) staff       (20)    12118 2023-02-04 11:48:50.101499 PyQt6-6.4.2/sip/QtGui/qtextdocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     1935 2023-02-04 11:48:50.045757 PyQt6-6.4.2/sip/QtGui/qtextdocumentfragment.sip
--rw-r--r--   0 phil       (501) staff       (20)     1714 2023-02-04 11:48:50.175333 PyQt6-6.4.2/sip/QtGui/qtextdocumentwriter.sip
--rw-r--r--   0 phil       (501) staff       (20)    19535 2023-02-04 11:48:50.096708 PyQt6-6.4.2/sip/QtGui/qtextformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     5324 2023-02-04 11:48:50.047072 PyQt6-6.4.2/sip/QtGui/qtextlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     1462 2023-02-04 11:48:50.046141 PyQt6-6.4.2/sip/QtGui/qtextlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     7691 2023-02-04 11:48:50.074999 PyQt6-6.4.2/sip/QtGui/qtextobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2786 2023-02-04 11:48:50.146224 PyQt6-6.4.2/sip/QtGui/qtextoption.sip
--rw-r--r--   0 phil       (501) staff       (20)     2569 2023-02-04 11:48:50.182757 PyQt6-6.4.2/sip/QtGui/qtexttable.sip
--rw-r--r--   0 phil       (501) staff       (20)     4946 2023-02-04 11:48:50.123677 PyQt6-6.4.2/sip/QtGui/qtransform.sip
--rw-r--r--   0 phil       (501) staff       (20)     2042 2023-02-04 11:48:50.075477 PyQt6-6.4.2/sip/QtGui/qundogroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     3004 2023-02-04 11:48:50.131914 PyQt6-6.4.2/sip/QtGui/qundostack.sip
--rw-r--r--   0 phil       (501) staff       (20)     3361 2023-02-04 11:48:50.144625 PyQt6-6.4.2/sip/QtGui/qvalidator.sip
--rw-r--r--   0 phil       (501) staff       (20)     9152 2023-02-04 11:48:50.139490 PyQt6-6.4.2/sip/QtGui/qvectornd.sip
--rw-r--r--   0 phil       (501) staff       (20)     7236 2023-02-04 11:48:50.084902 PyQt6-6.4.2/sip/QtGui/qwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1009 2023-02-04 11:48:50.128946 PyQt6-6.4.2/sip/QtGui/qwindowdefs.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.247112 PyQt6-6.4.2/sip/QtHelp/
--rw-r--r--   0 phil       (501) staff       (20)     2347 2023-02-04 11:48:49.987288 PyQt6-6.4.2/sip/QtHelp/QtHelpmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1429 2023-02-04 11:48:49.984281 PyQt6-6.4.2/sip/QtHelp/qcompressedhelpinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2348 2023-02-04 11:48:49.986370 PyQt6-6.4.2/sip/QtHelp/qhelpcontentwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1361 2023-02-04 11:48:49.986796 PyQt6-6.4.2/sip/QtHelp/qhelpengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     4184 2023-02-04 11:48:49.985669 PyQt6-6.4.2/sip/QtHelp/qhelpenginecore.sip
--rw-r--r--   0 phil       (501) staff       (20)     1430 2023-02-04 11:48:49.985044 PyQt6-6.4.2/sip/QtHelp/qhelpfilterdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1889 2023-02-04 11:48:49.990807 PyQt6-6.4.2/sip/QtHelp/qhelpfilterengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-02-04 11:48:49.990164 PyQt6-6.4.2/sip/QtHelp/qhelpfiltersettingswidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1836 2023-02-04 11:48:49.987841 PyQt6-6.4.2/sip/QtHelp/qhelpindexwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1048 2023-02-04 11:48:49.989666 PyQt6-6.4.2/sip/QtHelp/qhelplink.sip
--rw-r--r--   0 phil       (501) staff       (20)     2399 2023-02-04 11:48:49.988554 PyQt6-6.4.2/sip/QtHelp/qhelpsearchengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1552 2023-02-04 11:48:49.989183 PyQt6-6.4.2/sip/QtHelp/qhelpsearchquerywidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1222 2023-02-04 11:48:49.984661 PyQt6-6.4.2/sip/QtHelp/qhelpsearchresultwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.375703 PyQt6-6.4.2/sip/QtMultimedia/
--rw-r--r--   0 phil       (501) staff       (20)     2628 2023-02-04 11:48:50.445601 PyQt6-6.4.2/sip/QtMultimedia/QtMultimediamod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1516 2023-02-04 11:48:50.476191 PyQt6-6.4.2/sip/QtMultimedia/qaudio.sip
--rw-r--r--   0 phil       (501) staff       (20)     1993 2023-02-04 11:48:50.442439 PyQt6-6.4.2/sip/QtMultimedia/qaudiobuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2206 2023-02-04 11:48:50.479448 PyQt6-6.4.2/sip/QtMultimedia/qaudiodecoder.sip
--rw-r--r--   0 phil       (501) staff       (20)     1930 2023-02-04 11:48:50.441417 PyQt6-6.4.2/sip/QtMultimedia/qaudiodevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3341 2023-02-04 11:48:50.446298 PyQt6-6.4.2/sip/QtMultimedia/qaudioformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     1565 2023-02-04 11:48:50.477915 PyQt6-6.4.2/sip/QtMultimedia/qaudioinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1567 2023-02-04 11:48:50.441988 PyQt6-6.4.2/sip/QtMultimedia/qaudiooutput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1838 2023-02-04 11:48:50.443554 PyQt6-6.4.2/sip/QtMultimedia/qaudiosink.sip
--rw-r--r--   0 phil       (501) staff       (20)     1862 2023-02-04 11:48:50.476760 PyQt6-6.4.2/sip/QtMultimedia/qaudiosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     7286 2023-02-04 11:48:50.447358 PyQt6-6.4.2/sip/QtMultimedia/qcamera.sip
--rw-r--r--   0 phil       (501) staff       (20)     2093 2023-02-04 11:48:50.448519 PyQt6-6.4.2/sip/QtMultimedia/qcameradevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3030 2023-02-04 11:48:50.443078 PyQt6-6.4.2/sip/QtMultimedia/qimagecapture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1947 2023-02-04 11:48:50.482512 PyQt6-6.4.2/sip/QtMultimedia/qmediacapturesession.sip
--rw-r--r--   0 phil       (501) staff       (20)     1540 2023-02-04 11:48:50.481078 PyQt6-6.4.2/sip/QtMultimedia/qmediadevices.sip
--rw-r--r--   0 phil       (501) staff       (20)     3349 2023-02-04 11:48:50.480618 PyQt6-6.4.2/sip/QtMultimedia/qmediaformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     2186 2023-02-04 11:48:50.449053 PyQt6-6.4.2/sip/QtMultimedia/qmediametadata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3965 2023-02-04 11:48:50.478866 PyQt6-6.4.2/sip/QtMultimedia/qmediaplayer.sip
--rw-r--r--   0 phil       (501) staff       (20)     3680 2023-02-04 11:48:50.444307 PyQt6-6.4.2/sip/QtMultimedia/qmediarecorder.sip
--rw-r--r--   0 phil       (501) staff       (20)     3046 2023-02-04 11:48:50.447924 PyQt6-6.4.2/sip/QtMultimedia/qmediatimerange.sip
--rw-r--r--   0 phil       (501) staff       (20)    10957 2023-02-04 11:48:50.475533 PyQt6-6.4.2/sip/QtMultimedia/qpymultimedia_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     2198 2023-02-04 11:48:50.477397 PyQt6-6.4.2/sip/QtMultimedia/qsoundeffect.sip
--rw-r--r--   0 phil       (501) staff       (20)     3181 2023-02-04 11:48:50.445065 PyQt6-6.4.2/sip/QtMultimedia/qvideoframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     4710 2023-02-04 11:48:50.481979 PyQt6-6.4.2/sip/QtMultimedia/qvideoframeformat.sip
--rw-r--r--   0 phil       (501) staff       (20)     1508 2023-02-04 11:48:50.479913 PyQt6-6.4.2/sip/QtMultimedia/qvideosink.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.430136 PyQt6-6.4.2/sip/QtMultimediaWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2083 2023-02-04 11:48:50.693286 PyQt6-6.4.2/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2007 2023-02-04 11:48:50.694515 PyQt6-6.4.2/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2399 2023-02-04 11:48:50.693995 PyQt6-6.4.2/sip/QtMultimediaWidgets/qvideowidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.231029 PyQt6-6.4.2/sip/QtNetwork/
--rw-r--r--   0 phil       (501) staff       (20)     3090 2023-02-04 11:48:49.894003 PyQt6-6.4.2/sip/QtNetwork/QtNetworkmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2995 2023-02-04 11:48:49.929217 PyQt6-6.4.2/sip/QtNetwork/qabstractnetworkcache.sip
--rw-r--r--   0 phil       (501) staff       (20)    10970 2023-02-04 11:48:49.931220 PyQt6-6.4.2/sip/QtNetwork/qabstractsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     1584 2023-02-04 11:48:49.928069 PyQt6-6.4.2/sip/QtNetwork/qauthenticator.sip
--rw-r--r--   0 phil       (501) staff       (20)     4595 2023-02-04 11:48:49.894834 PyQt6-6.4.2/sip/QtNetwork/qdnslookup.sip
--rw-r--r--   0 phil       (501) staff       (20)     5644 2023-02-04 11:48:49.896973 PyQt6-6.4.2/sip/QtNetwork/qhostaddress.sip
--rw-r--r--   0 phil       (501) staff       (20)     2987 2023-02-04 11:48:49.898059 PyQt6-6.4.2/sip/QtNetwork/qhostinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     1906 2023-02-04 11:48:49.937672 PyQt6-6.4.2/sip/QtNetwork/qhstspolicy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1863 2023-02-04 11:48:49.934100 PyQt6-6.4.2/sip/QtNetwork/qhttp2configuration.sip
--rw-r--r--   0 phil       (501) staff       (20)     2111 2023-02-04 11:48:49.942123 PyQt6-6.4.2/sip/QtNetwork/qhttpmultipart.sip
--rw-r--r--   0 phil       (501) staff       (20)     2417 2023-02-04 11:48:49.897473 PyQt6-6.4.2/sip/QtNetwork/qlocalserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     6739 2023-02-04 11:48:49.932204 PyQt6-6.4.2/sip/QtNetwork/qlocalsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     4835 2023-02-04 11:48:49.925665 PyQt6-6.4.2/sip/QtNetwork/qnetworkaccessmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     2540 2023-02-04 11:48:49.893430 PyQt6-6.4.2/sip/QtNetwork/qnetworkcookie.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2023-02-04 11:48:49.941632 PyQt6-6.4.2/sip/QtNetwork/qnetworkcookiejar.sip
--rw-r--r--   0 phil       (501) staff       (20)     1941 2023-02-04 11:48:49.890881 PyQt6-6.4.2/sip/QtNetwork/qnetworkdatagram.sip
--rw-r--r--   0 phil       (501) staff       (20)     1881 2023-02-04 11:48:49.928503 PyQt6-6.4.2/sip/QtNetwork/qnetworkdiskcache.sip
--rw-r--r--   0 phil       (501) staff       (20)     2950 2023-02-04 11:48:49.925004 PyQt6-6.4.2/sip/QtNetwork/qnetworkinformation.sip
--rw-r--r--   0 phil       (501) staff       (20)     3720 2023-02-04 11:48:49.923732 PyQt6-6.4.2/sip/QtNetwork/qnetworkinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     5091 2023-02-04 11:48:49.942891 PyQt6-6.4.2/sip/QtNetwork/qnetworkproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     5728 2023-02-04 11:48:49.895681 PyQt6-6.4.2/sip/QtNetwork/qnetworkreply.sip
--rw-r--r--   0 phil       (501) staff       (20)     4892 2023-02-04 11:48:49.934896 PyQt6-6.4.2/sip/QtNetwork/qnetworkrequest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2020 2023-02-04 11:48:49.940187 PyQt6-6.4.2/sip/QtNetwork/qocspresponse.sip
--rw-r--r--   0 phil       (501) staff       (20)     1379 2023-02-04 11:48:49.896044 PyQt6-6.4.2/sip/QtNetwork/qpassworddigestor.sip
--rw-r--r--   0 phil       (501) staff       (20)     3458 2023-02-04 11:48:49.941171 PyQt6-6.4.2/sip/QtNetwork/qpynetwork_qhash.sip
--rw-r--r--   0 phil       (501) staff       (20)     7009 2023-02-04 11:48:49.937144 PyQt6-6.4.2/sip/QtNetwork/qpynetwork_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     4985 2023-02-04 11:48:49.926730 PyQt6-6.4.2/sip/QtNetwork/qpynetwork_qmap.sip
--rw-r--r--   0 phil       (501) staff       (20)     3643 2023-02-04 11:48:49.933145 PyQt6-6.4.2/sip/QtNetwork/qssl.sip
--rw-r--r--   0 phil       (501) staff       (20)     3763 2023-02-04 11:48:49.943657 PyQt6-6.4.2/sip/QtNetwork/qsslcertificate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1426 2023-02-04 11:48:49.933676 PyQt6-6.4.2/sip/QtNetwork/qsslcertificateextension.sip
--rw-r--r--   0 phil       (501) staff       (20)     1694 2023-02-04 11:48:49.898470 PyQt6-6.4.2/sip/QtNetwork/qsslcipher.sip
--rw-r--r--   0 phil       (501) staff       (20)     5201 2023-02-04 11:48:49.892901 PyQt6-6.4.2/sip/QtNetwork/qsslconfiguration.sip
--rw-r--r--   0 phil       (501) staff       (20)     2171 2023-02-04 11:48:49.924300 PyQt6-6.4.2/sip/QtNetwork/qssldiffiehellmanparameters.sip
--rw-r--r--   0 phil       (501) staff       (20)     1594 2023-02-04 11:48:49.927628 PyQt6-6.4.2/sip/QtNetwork/qsslellipticcurve.sip
--rw-r--r--   0 phil       (501) staff       (20)     2803 2023-02-04 11:48:49.929779 PyQt6-6.4.2/sip/QtNetwork/qsslerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     2021 2023-02-04 11:48:49.927181 PyQt6-6.4.2/sip/QtNetwork/qsslkey.sip
--rw-r--r--   0 phil       (501) staff       (20)     1883 2023-02-04 11:48:49.892227 PyQt6-6.4.2/sip/QtNetwork/qsslpresharedkeyauthenticator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2150 2023-02-04 11:48:49.891805 PyQt6-6.4.2/sip/QtNetwork/qsslserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     8621 2023-02-04 11:48:49.938733 PyQt6-6.4.2/sip/QtNetwork/qsslsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     2339 2023-02-04 11:48:49.935392 PyQt6-6.4.2/sip/QtNetwork/qtcpserver.sip
--rw-r--r--   0 phil       (501) staff       (20)     1134 2023-02-04 11:48:49.891248 PyQt6-6.4.2/sip/QtNetwork/qtcpsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     3235 2023-02-04 11:48:49.939461 PyQt6-6.4.2/sip/QtNetwork/qudpsocket.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.302132 PyQt6-6.4.2/sip/QtNfc/
--rw-r--r--   0 phil       (501) staff       (20)     2146 2023-02-04 11:48:50.189166 PyQt6-6.4.2/sip/QtNfc/QtNfcmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1772 2023-02-04 11:48:50.191907 PyQt6-6.4.2/sip/QtNfc/qndeffilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2185 2023-02-04 11:48:50.190040 PyQt6-6.4.2/sip/QtNfc/qndefmessage.sip
--rw-r--r--   0 phil       (501) staff       (20)     3351 2023-02-04 11:48:50.188603 PyQt6-6.4.2/sip/QtNfc/qndefnfcsmartposterrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     1471 2023-02-04 11:48:50.190725 PyQt6-6.4.2/sip/QtNfc/qndefnfctextrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     1213 2023-02-04 11:48:50.187811 PyQt6-6.4.2/sip/QtNfc/qndefnfcurirecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     2536 2023-02-04 11:48:50.186295 PyQt6-6.4.2/sip/QtNfc/qndefrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     3014 2023-02-04 11:48:50.187169 PyQt6-6.4.2/sip/QtNfc/qnearfieldmanager.sip
--rw-r--r--   0 phil       (501) staff       (20)     3250 2023-02-04 11:48:50.191447 PyQt6-6.4.2/sip/QtNfc/qnearfieldtarget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.196663 PyQt6-6.4.2/sip/QtOpenGL/
--rw-r--r--   0 phil       (501) staff       (20)     2618 2023-02-04 11:48:49.824366 PyQt6-6.4.2/sip/QtOpenGL/QtOpenGLmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2586 2023-02-04 11:48:49.823775 PyQt6-6.4.2/sip/QtOpenGL/qopenglbuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)     5913 2023-02-04 11:48:49.823018 PyQt6-6.4.2/sip/QtOpenGL/qopengldebug.sip
--rw-r--r--   0 phil       (501) staff       (20)     5082 2023-02-04 11:48:49.798063 PyQt6-6.4.2/sip/QtOpenGL/qopenglframebufferobject.sip
--rw-r--r--   0 phil       (501) staff       (20)   111265 2023-02-04 11:48:49.810190 PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_2_0.sip
--rw-r--r--   0 phil       (501) staff       (20)   111310 2023-02-04 11:48:49.821320 PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_2_1.sip
--rw-r--r--   0 phil       (501) staff       (20)    42567 2023-02-04 11:48:49.792860 PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_4_1_core.sip
--rw-r--r--   0 phil       (501) staff       (20)    28956 2023-02-04 11:48:49.828425 PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_es2.sip
--rw-r--r--   0 phil       (501) staff       (20)     1751 2023-02-04 11:48:49.797245 PyQt6-6.4.2/sip/QtOpenGL/qopenglpaintdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1865 2023-02-04 11:48:49.828902 PyQt6-6.4.2/sip/QtOpenGL/qopenglpixeltransferoptions.sip
--rw-r--r--   0 phil       (501) staff       (20)    15899 2023-02-04 11:48:49.831390 PyQt6-6.4.2/sip/QtOpenGL/qopenglshaderprogram.sip
--rw-r--r--   0 phil       (501) staff       (20)    14995 2023-02-04 11:48:49.796715 PyQt6-6.4.2/sip/QtOpenGL/qopengltexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     2010 2023-02-04 11:48:49.829982 PyQt6-6.4.2/sip/QtOpenGL/qopengltextureblitter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2095 2023-02-04 11:48:49.794037 PyQt6-6.4.2/sip/QtOpenGL/qopengltimerquery.sip
--rw-r--r--   0 phil       (501) staff       (20)     1168 2023-02-04 11:48:49.794464 PyQt6-6.4.2/sip/QtOpenGL/qopenglversionfunctions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1350 2023-02-04 11:48:49.793439 PyQt6-6.4.2/sip/QtOpenGL/qopenglversionfunctionsfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1814 2023-02-04 11:48:49.829330 PyQt6-6.4.2/sip/QtOpenGL/qopenglversionprofile.sip
--rw-r--r--   0 phil       (501) staff       (20)     1909 2023-02-04 11:48:49.831998 PyQt6-6.4.2/sip/QtOpenGL/qopenglvertexarrayobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2173 2023-02-04 11:48:49.821898 PyQt6-6.4.2/sip/QtOpenGL/qopenglwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     2926 2023-02-04 11:48:49.787778 PyQt6-6.4.2/sip/QtOpenGL/qpyopengl_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     3170 2023-02-04 11:48:49.825262 PyQt6-6.4.2/sip/QtOpenGL/qpyopengl_std_pair.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.264841 PyQt6-6.4.2/sip/QtOpenGLWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2059 2023-02-04 11:48:50.043431 PyQt6-6.4.2/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2762 2023-02-04 11:48:50.044129 PyQt6-6.4.2/sip/QtOpenGLWidgets/qopenglwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.263963 PyQt6-6.4.2/sip/QtPdf/
--rw-r--r--   0 phil       (501) staff       (20)     2169 2023-02-04 11:48:50.038769 PyQt6-6.4.2/sip/QtPdf/QtPdfmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1876 2023-02-04 11:48:50.041505 PyQt6-6.4.2/sip/QtPdf/qpdfbookmarkmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     3512 2023-02-04 11:48:50.040602 PyQt6-6.4.2/sip/QtPdf/qpdfdocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     2081 2023-02-04 11:48:50.042124 PyQt6-6.4.2/sip/QtPdf/qpdfdocumentrenderoptions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1460 2023-02-04 11:48:50.039214 PyQt6-6.4.2/sip/QtPdf/qpdflink.sip
--rw-r--r--   0 phil       (501) staff       (20)     1827 2023-02-04 11:48:50.041073 PyQt6-6.4.2/sip/QtPdf/qpdfpagenavigator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1681 2023-02-04 11:48:50.039711 PyQt6-6.4.2/sip/QtPdf/qpdfpagerenderer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1900 2023-02-04 11:48:50.042591 PyQt6-6.4.2/sip/QtPdf/qpdfsearchmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1430 2023-02-04 11:48:50.043005 PyQt6-6.4.2/sip/QtPdf/qpdfselection.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.433468 PyQt6-6.4.2/sip/QtPdfWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2012 2023-02-04 11:48:50.723309 PyQt6-6.4.2/sip/QtPdfWidgets/QtPdfWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2848 2023-02-04 11:48:50.724061 PyQt6-6.4.2/sip/QtPdfWidgets/qpdfview.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.382139 PyQt6-6.4.2/sip/QtPositioning/
--rw-r--r--   0 phil       (501) staff       (20)     2365 2023-02-04 11:48:50.483601 PyQt6-6.4.2/sip/QtPositioning/QtPositioningmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2273 2023-02-04 11:48:50.491488 PyQt6-6.4.2/sip/QtPositioning/qgeoaddress.sip
--rw-r--r--   0 phil       (501) staff       (20)     2226 2023-02-04 11:48:50.489755 PyQt6-6.4.2/sip/QtPositioning/qgeoareamonitorinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     3002 2023-02-04 11:48:50.488182 PyQt6-6.4.2/sip/QtPositioning/qgeoareamonitorsource.sip
--rw-r--r--   0 phil       (501) staff       (20)     1635 2023-02-04 11:48:50.486815 PyQt6-6.4.2/sip/QtPositioning/qgeocircle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2775 2023-02-04 11:48:50.492119 PyQt6-6.4.2/sip/QtPositioning/qgeocoordinate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1850 2023-02-04 11:48:50.490289 PyQt6-6.4.2/sip/QtPositioning/qgeolocation.sip
--rw-r--r--   0 phil       (501) staff       (20)     2156 2023-02-04 11:48:50.488761 PyQt6-6.4.2/sip/QtPositioning/qgeopath.sip
--rw-r--r--   0 phil       (501) staff       (20)     2375 2023-02-04 11:48:50.489273 PyQt6-6.4.2/sip/QtPositioning/qgeopolygon.sip
--rw-r--r--   0 phil       (501) staff       (20)     2502 2023-02-04 11:48:50.483152 PyQt6-6.4.2/sip/QtPositioning/qgeopositioninfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     4135 2023-02-04 11:48:50.487507 PyQt6-6.4.2/sip/QtPositioning/qgeopositioninfosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2023-02-04 11:48:50.484634 PyQt6-6.4.2/sip/QtPositioning/qgeorectangle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2343 2023-02-04 11:48:50.485825 PyQt6-6.4.2/sip/QtPositioning/qgeosatelliteinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2640 2023-02-04 11:48:50.490974 PyQt6-6.4.2/sip/QtPositioning/qgeosatelliteinfosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     2434 2023-02-04 11:48:50.486402 PyQt6-6.4.2/sip/QtPositioning/qgeoshape.sip
--rw-r--r--   0 phil       (501) staff       (20)     2205 2023-02-04 11:48:50.485155 PyQt6-6.4.2/sip/QtPositioning/qnmeapositioninfosource.sip
--rw-r--r--   0 phil       (501) staff       (20)     2448 2023-02-04 11:48:50.484119 PyQt6-6.4.2/sip/QtPositioning/qnmeasatelliteinfosource.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.189777 PyQt6-6.4.2/sip/QtPrintSupport/
--rw-r--r--   0 phil       (501) staff       (20)     2261 2023-02-04 11:48:49.781916 PyQt6-6.4.2/sip/QtPrintSupport/QtPrintSupportmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3959 2023-02-04 11:48:49.781423 PyQt6-6.4.2/sip/QtPrintSupport/qabstractprintdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2569 2023-02-04 11:48:49.784572 PyQt6-6.4.2/sip/QtPrintSupport/qpagesetupdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2959 2023-02-04 11:48:49.779979 PyQt6-6.4.2/sip/QtPrintSupport/qprintdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2327 2023-02-04 11:48:49.785728 PyQt6-6.4.2/sip/QtPrintSupport/qprintengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     4672 2023-02-04 11:48:49.786804 PyQt6-6.4.2/sip/QtPrintSupport/qprinter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2194 2023-02-04 11:48:49.785114 PyQt6-6.4.2/sip/QtPrintSupport/qprinterinfo.sip
--rw-r--r--   0 phil       (501) staff       (20)     2034 2023-02-04 11:48:49.780542 PyQt6-6.4.2/sip/QtPrintSupport/qprintpreviewdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2558 2023-02-04 11:48:49.782591 PyQt6-6.4.2/sip/QtPrintSupport/qprintpreviewwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     4887 2023-02-04 11:48:49.783937 PyQt6-6.4.2/sip/QtPrintSupport/qpyprintsupport_qlist.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.206090 PyQt6-6.4.2/sip/QtQml/
--rw-r--r--   0 phil       (501) staff       (20)     2708 2023-02-04 11:48:49.838683 PyQt6-6.4.2/sip/QtQml/QtQmlmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     5894 2023-02-04 11:48:49.839782 PyQt6-6.4.2/sip/QtQml/qjsengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     3449 2023-02-04 11:48:49.844224 PyQt6-6.4.2/sip/QtQml/qjsmanagedvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     3260 2023-02-04 11:48:49.834701 PyQt6-6.4.2/sip/QtQml/qjsprimitivevalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     3624 2023-02-04 11:48:49.837643 PyQt6-6.4.2/sip/QtQml/qjsvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     1267 2023-02-04 11:48:49.833908 PyQt6-6.4.2/sip/QtQml/qjsvalueiterator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1412 2023-02-04 11:48:49.833403 PyQt6-6.4.2/sip/QtQml/qmlattachedpropertiesobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2851 2023-02-04 11:48:49.843157 PyQt6-6.4.2/sip/QtQml/qmlregistertype.sip
--rw-r--r--   0 phil       (501) staff       (20)     1413 2023-02-04 11:48:49.841008 PyQt6-6.4.2/sip/QtQml/qpyqmllistproperty.sip
--rw-r--r--   0 phil       (501) staff       (20)     1852 2023-02-04 11:48:49.846583 PyQt6-6.4.2/sip/QtQml/qqml.sip
--rw-r--r--   0 phil       (501) staff       (20)     1354 2023-02-04 11:48:49.841966 PyQt6-6.4.2/sip/QtQml/qqmlabstracturlinterceptor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1880 2023-02-04 11:48:49.836972 PyQt6-6.4.2/sip/QtQml/qqmlapplicationengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     2938 2023-02-04 11:48:49.836218 PyQt6-6.4.2/sip/QtQml/qqmlcomponent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2006 2023-02-04 11:48:49.846039 PyQt6-6.4.2/sip/QtQml/qqmlcontext.sip
--rw-r--r--   0 phil       (501) staff       (20)     5156 2023-02-04 11:48:49.847391 PyQt6-6.4.2/sip/QtQml/qqmlengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     1624 2023-02-04 11:48:49.847834 PyQt6-6.4.2/sip/QtQml/qqmlerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     1925 2023-02-04 11:48:49.845202 PyQt6-6.4.2/sip/QtQml/qqmlexpression.sip
--rw-r--r--   0 phil       (501) staff       (20)     1583 2023-02-04 11:48:49.841451 PyQt6-6.4.2/sip/QtQml/qqmlextensionplugin.sip
--rw-r--r--   0 phil       (501) staff       (20)     1303 2023-02-04 11:48:49.835666 PyQt6-6.4.2/sip/QtQml/qqmlfileselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     2332 2023-02-04 11:48:49.835290 PyQt6-6.4.2/sip/QtQml/qqmlincubator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1898 2023-02-04 11:48:49.840397 PyQt6-6.4.2/sip/QtQml/qqmllist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1199 2023-02-04 11:48:49.843613 PyQt6-6.4.2/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1235 2023-02-04 11:48:49.844731 PyQt6-6.4.2/sip/QtQml/qqmlparserstatus.sip
--rw-r--r--   0 phil       (501) staff       (20)     4182 2023-02-04 11:48:49.832793 PyQt6-6.4.2/sip/QtQml/qqmlproperty.sip
--rw-r--r--   0 phil       (501) staff       (20)     1769 2023-02-04 11:48:49.838136 PyQt6-6.4.2/sip/QtQml/qqmlpropertymap.sip
--rw-r--r--   0 phil       (501) staff       (20)     1254 2023-02-04 11:48:49.845572 PyQt6-6.4.2/sip/QtQml/qqmlpropertyvaluesource.sip
--rw-r--r--   0 phil       (501) staff       (20)     1457 2023-02-04 11:48:49.842454 PyQt6-6.4.2/sip/QtQml/qqmlscriptstring.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.313380 PyQt6-6.4.2/sip/QtQuick/
--rw-r--r--   0 phil       (501) staff       (20)     2852 2023-02-04 11:48:50.228711 PyQt6-6.4.2/sip/QtQuick/QtQuickmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2548 2023-02-04 11:48:50.225076 PyQt6-6.4.2/sip/QtQuick/qquickframebufferobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     1498 2023-02-04 11:48:50.235716 PyQt6-6.4.2/sip/QtQuick/qquickgraphicsconfiguration.sip
--rw-r--r--   0 phil       (501) staff       (20)     1298 2023-02-04 11:48:50.194568 PyQt6-6.4.2/sip/QtQuick/qquickgraphicsdevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2820 2023-02-04 11:48:50.234277 PyQt6-6.4.2/sip/QtQuick/qquickimageprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)    10164 2023-02-04 11:48:50.239293 PyQt6-6.4.2/sip/QtQuick/qquickitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     1368 2023-02-04 11:48:50.237655 PyQt6-6.4.2/sip/QtQuick/qquickitemgrabresult.sip
--rw-r--r--   0 phil       (501) staff       (20)     2983 2023-02-04 11:48:50.197043 PyQt6-6.4.2/sip/QtQuick/qquickpainteditem.sip
--rw-r--r--   0 phil       (501) staff       (20)     1662 2023-02-04 11:48:50.228141 PyQt6-6.4.2/sip/QtQuick/qquickrendercontrol.sip
--rw-r--r--   0 phil       (501) staff       (20)     2100 2023-02-04 11:48:50.196467 PyQt6-6.4.2/sip/QtQuick/qquickrendertarget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1160 2023-02-04 11:48:50.231468 PyQt6-6.4.2/sip/QtQuick/qquicktextdocument.sip
--rw-r--r--   0 phil       (501) staff       (20)     2345 2023-02-04 11:48:50.236708 PyQt6-6.4.2/sip/QtQuick/qquickview.sip
--rw-r--r--   0 phil       (501) staff       (20)     6928 2023-02-04 11:48:50.230378 PyQt6-6.4.2/sip/QtQuick/qquickwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1377 2023-02-04 11:48:50.223471 PyQt6-6.4.2/sip/QtQuick/qsgflatcolormaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)    11740 2023-02-04 11:48:50.227621 PyQt6-6.4.2/sip/QtQuick/qsggeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2762 2023-02-04 11:48:50.224362 PyQt6-6.4.2/sip/QtQuick/qsgimagenode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1747 2023-02-04 11:48:50.234768 PyQt6-6.4.2/sip/QtQuick/qsgmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     4124 2023-02-04 11:48:50.195983 PyQt6-6.4.2/sip/QtQuick/qsgmaterialshader.sip
--rw-r--r--   0 phil       (501) staff       (20)     1033 2023-02-04 11:48:50.197912 PyQt6-6.4.2/sip/QtQuick/qsgmaterialtype.sip
--rw-r--r--   0 phil       (501) staff       (20)     8652 2023-02-04 11:48:50.233638 PyQt6-6.4.2/sip/QtQuick/qsgnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1343 2023-02-04 11:48:50.237158 PyQt6-6.4.2/sip/QtQuick/qsgrectanglenode.sip
--rw-r--r--   0 phil       (501) staff       (20)     3077 2023-02-04 11:48:50.225822 PyQt6-6.4.2/sip/QtQuick/qsgrendererinterface.sip
--rw-r--r--   0 phil       (501) staff       (20)     2456 2023-02-04 11:48:50.231020 PyQt6-6.4.2/sip/QtQuick/qsgrendernode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1354 2023-02-04 11:48:50.231948 PyQt6-6.4.2/sip/QtQuick/qsgsimplerectnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     2097 2023-02-04 11:48:50.235261 PyQt6-6.4.2/sip/QtQuick/qsgsimpletexturenode.sip
--rw-r--r--   0 phil       (501) staff       (20)     2513 2023-02-04 11:48:50.195123 PyQt6-6.4.2/sip/QtQuick/qsgtexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1446 2023-02-04 11:48:50.229220 PyQt6-6.4.2/sip/QtQuick/qsgtexture_platform.sip
--rw-r--r--   0 phil       (501) staff       (20)     2207 2023-02-04 11:48:50.197483 PyQt6-6.4.2/sip/QtQuick/qsgtexturematerial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1152 2023-02-04 11:48:50.236135 PyQt6-6.4.2/sip/QtQuick/qsgtextureprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)     1324 2023-02-04 11:48:50.198285 PyQt6-6.4.2/sip/QtQuick/qsgvertexcolormaterial.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.242415 PyQt6-6.4.2/sip/QtQuick3D/
--rw-r--r--   0 phil       (501) staff       (20)     2086 2023-02-04 11:48:49.982863 PyQt6-6.4.2/sip/QtQuick3D/QtQuick3Dmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1086 2023-02-04 11:48:49.982480 PyQt6-6.4.2/sip/QtQuick3D/qquick3d.sip
--rw-r--r--   0 phil       (501) staff       (20)     3758 2023-02-04 11:48:49.982112 PyQt6-6.4.2/sip/QtQuick3D/qquick3dgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2159 2023-02-04 11:48:49.983798 PyQt6-6.4.2/sip/QtQuick3D/qquick3dobject.sip
--rw-r--r--   0 phil       (501) staff       (20)     2181 2023-02-04 11:48:49.981242 PyQt6-6.4.2/sip/QtQuick3D/qquick3dtexturedata.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.319517 PyQt6-6.4.2/sip/QtQuickWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2080 2023-02-04 11:48:50.273318 PyQt6-6.4.2/sip/QtQuickWidgets/QtQuickWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3345 2023-02-04 11:48:50.274090 PyQt6-6.4.2/sip/QtQuickWidgets/qquickwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.254500 PyQt6-6.4.2/sip/QtRemoteObjects/
--rw-r--r--   0 phil       (501) staff       (20)     2163 2023-02-04 11:48:50.027010 PyQt6-6.4.2/sip/QtRemoteObjects/QtRemoteObjectsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2298 2023-02-04 11:48:50.025115 PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip
--rw-r--r--   0 phil       (501) staff       (20)     1221 2023-02-04 11:48:50.024136 PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip
--rw-r--r--   0 phil       (501) staff       (20)     6469 2023-02-04 11:48:50.026099 PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1429 2023-02-04 11:48:50.027435 PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectregistry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1689 2023-02-04 11:48:50.026596 PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectreplica.sip
--rw-r--r--   0 phil       (501) staff       (20)     2093 2023-02-04 11:48:50.024648 PyQt6-6.4.2/sip/QtRemoteObjects/qtremoteobjectglobal.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.260814 PyQt6-6.4.2/sip/QtSensors/
--rw-r--r--   0 phil       (501) staff       (20)     2393 2023-02-04 11:48:50.037145 PyQt6-6.4.2/sip/QtSensors/QtSensorsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2037 2023-02-04 11:48:50.031337 PyQt6-6.4.2/sip/QtSensors/qaccelerometer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1842 2023-02-04 11:48:50.028033 PyQt6-6.4.2/sip/QtSensors/qambientlightsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1726 2023-02-04 11:48:50.032955 PyQt6-6.4.2/sip/QtSensors/qambienttemperaturesensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1641 2023-02-04 11:48:50.036464 PyQt6-6.4.2/sip/QtSensors/qcompass.sip
--rw-r--r--   0 phil       (501) staff       (20)     1645 2023-02-04 11:48:50.033523 PyQt6-6.4.2/sip/QtSensors/qgyroscope.sip
--rw-r--r--   0 phil       (501) staff       (20)     1701 2023-02-04 11:48:50.032271 PyQt6-6.4.2/sip/QtSensors/qhumiditysensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1649 2023-02-04 11:48:50.031799 PyQt6-6.4.2/sip/QtSensors/qirproximitysensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2023-02-04 11:48:50.028602 PyQt6-6.4.2/sip/QtSensors/qlidsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1692 2023-02-04 11:48:50.030822 PyQt6-6.4.2/sip/QtSensors/qlightsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1918 2023-02-04 11:48:50.037721 PyQt6-6.4.2/sip/QtSensors/qmagnetometer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1856 2023-02-04 11:48:50.029162 PyQt6-6.4.2/sip/QtSensors/qorientationsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1682 2023-02-04 11:48:50.030143 PyQt6-6.4.2/sip/QtSensors/qpressuresensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1607 2023-02-04 11:48:50.029674 PyQt6-6.4.2/sip/QtSensors/qproximitysensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1749 2023-02-04 11:48:50.038231 PyQt6-6.4.2/sip/QtSensors/qrotationsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     7556 2023-02-04 11:48:50.035968 PyQt6-6.4.2/sip/QtSensors/qsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     2079 2023-02-04 11:48:50.034758 PyQt6-6.4.2/sip/QtSensors/qtapsensor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1641 2023-02-04 11:48:50.034134 PyQt6-6.4.2/sip/QtSensors/qtiltsensor.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.303200 PyQt6-6.4.2/sip/QtSerialPort/
--rw-r--r--   0 phil       (501) staff       (20)     1982 2023-02-04 11:48:50.192775 PyQt6-6.4.2/sip/QtSerialPort/QtSerialPortmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     7926 2023-02-04 11:48:50.194072 PyQt6-6.4.2/sip/QtSerialPort/qserialport.sip
--rw-r--r--   0 phil       (501) staff       (20)     1768 2023-02-04 11:48:50.192400 PyQt6-6.4.2/sip/QtSerialPort/qserialportinfo.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.366309 PyQt6-6.4.2/sip/QtSql/
--rw-r--r--   0 phil       (501) staff       (20)     2287 2023-02-04 11:48:50.439337 PyQt6-6.4.2/sip/QtSql/QtSqlmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3746 2023-02-04 11:48:50.438845 PyQt6-6.4.2/sip/QtSql/qsqldatabase.sip
--rw-r--r--   0 phil       (501) staff       (20)     5000 2023-02-04 11:48:50.434328 PyQt6-6.4.2/sip/QtSql/qsqldriver.sip
--rw-r--r--   0 phil       (501) staff       (20)     1749 2023-02-04 11:48:50.432689 PyQt6-6.4.2/sip/QtSql/qsqlerror.sip
--rw-r--r--   0 phil       (501) staff       (20)     2360 2023-02-04 11:48:50.440835 PyQt6-6.4.2/sip/QtSql/qsqlfield.sip
--rw-r--r--   0 phil       (501) staff       (20)     1497 2023-02-04 11:48:50.438051 PyQt6-6.4.2/sip/QtSql/qsqlindex.sip
--rw-r--r--   0 phil       (501) staff       (20)     3080 2023-02-04 11:48:50.435764 PyQt6-6.4.2/sip/QtSql/qsqlquery.sip
--rw-r--r--   0 phil       (501) staff       (20)     2942 2023-02-04 11:48:50.437638 PyQt6-6.4.2/sip/QtSql/qsqlquerymodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     2260 2023-02-04 11:48:50.436359 PyQt6-6.4.2/sip/QtSql/qsqlrecord.sip
--rw-r--r--   0 phil       (501) staff       (20)     1542 2023-02-04 11:48:50.435215 PyQt6-6.4.2/sip/QtSql/qsqlrelationaldelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2023-02-04 11:48:50.439885 PyQt6-6.4.2/sip/QtSql/qsqlrelationaltablemodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     3175 2023-02-04 11:48:50.433412 PyQt6-6.4.2/sip/QtSql/qsqlresult.sip
--rw-r--r--   0 phil       (501) staff       (20)     3763 2023-02-04 11:48:50.436936 PyQt6-6.4.2/sip/QtSql/qsqltablemodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1512 2023-02-04 11:48:50.434792 PyQt6-6.4.2/sip/QtSql/qtsqlglobal.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.250027 PyQt6-6.4.2/sip/QtSvg/
--rw-r--r--   0 phil       (501) staff       (20)     1987 2023-02-04 11:48:49.995084 PyQt6-6.4.2/sip/QtSvg/QtSvgmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1819 2023-02-04 11:48:49.994118 PyQt6-6.4.2/sip/QtSvg/qsvggenerator.sip
--rw-r--r--   0 phil       (501) staff       (20)     3043 2023-02-04 11:48:49.994705 PyQt6-6.4.2/sip/QtSvg/qsvgrenderer.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.252035 PyQt6-6.4.2/sip/QtSvgWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     2071 2023-02-04 11:48:49.998402 PyQt6-6.4.2/sip/QtSvgWidgets/QtSvgWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1911 2023-02-04 11:48:49.998021 PyQt6-6.4.2/sip/QtSvgWidgets/qgraphicssvgitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2035 2023-02-04 11:48:50.023598 PyQt6-6.4.2/sip/QtSvgWidgets/qsvgwidget.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.432636 PyQt6-6.4.2/sip/QtTest/
--rw-r--r--   0 phil       (501) staff       (20)     2110 2023-02-04 11:48:50.695186 PyQt6-6.4.2/sip/QtTest/QtTestmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1689 2023-02-04 11:48:50.697587 PyQt6-6.4.2/sip/QtTest/qabstractitemmodeltester.sip
--rw-r--r--   0 phil       (501) staff       (20)     3285 2023-02-04 11:48:50.696296 PyQt6-6.4.2/sip/QtTest/qsignalspy.sip
--rw-r--r--   0 phil       (501) staff       (20)     3740 2023-02-04 11:48:50.695680 PyQt6-6.4.2/sip/QtTest/qtestkeyboard.sip
--rw-r--r--   0 phil       (501) staff       (20)     2446 2023-02-04 11:48:50.697177 PyQt6-6.4.2/sip/QtTest/qtestmouse.sip
--rw-r--r--   0 phil       (501) staff       (20)     1381 2023-02-04 11:48:50.696674 PyQt6-6.4.2/sip/QtTest/qtestsystem.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.383359 PyQt6-6.4.2/sip/QtTextToSpeech/
--rw-r--r--   0 phil       (501) staff       (20)     1981 2023-02-04 11:48:50.493932 PyQt6-6.4.2/sip/QtTextToSpeech/QtTextToSpeechmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     3550 2023-02-04 11:48:50.492848 PyQt6-6.4.2/sip/QtTextToSpeech/qtexttospeech.sip
--rw-r--r--   0 phil       (501) staff       (20)     1760 2023-02-04 11:48:50.493480 PyQt6-6.4.2/sip/QtTextToSpeech/qvoice.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.320508 PyQt6-6.4.2/sip/QtWebChannel/
--rw-r--r--   0 phil       (501) staff       (20)     1995 2023-02-04 11:48:50.274607 PyQt6-6.4.2/sip/QtWebChannel/QtWebChannelmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2363 2023-02-04 11:48:50.275597 PyQt6-6.4.2/sip/QtWebChannel/qwebchannel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1425 2023-02-04 11:48:50.275043 PyQt6-6.4.2/sip/QtWebChannel/qwebchannelabstracttransport.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.185885 PyQt6-6.4.2/sip/QtWebSockets/
--rw-r--r--   0 phil       (501) staff       (20)     2158 2023-02-04 11:48:49.778068 PyQt6-6.4.2/sip/QtWebSockets/QtWebSocketsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1238 2023-02-04 11:48:49.778525 PyQt6-6.4.2/sip/QtWebSockets/qmaskgenerator.sip
--rw-r--r--   0 phil       (501) staff       (20)     5947 2023-02-04 11:48:49.777584 PyQt6-6.4.2/sip/QtWebSockets/qwebsocket.sip
--rw-r--r--   0 phil       (501) staff       (20)     1445 2023-02-04 11:48:49.776447 PyQt6-6.4.2/sip/QtWebSockets/qwebsocketcorsauthenticator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1623 2023-02-04 11:48:49.775896 PyQt6-6.4.2/sip/QtWebSockets/qwebsockethandshakeoptions.sip
--rw-r--r--   0 phil       (501) staff       (20)     1741 2023-02-04 11:48:49.775361 PyQt6-6.4.2/sip/QtWebSockets/qwebsocketprotocol.sip
--rw-r--r--   0 phil       (501) staff       (20)     3249 2023-02-04 11:48:49.779249 PyQt6-6.4.2/sip/QtWebSockets/qwebsocketserver.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.361453 PyQt6-6.4.2/sip/QtWidgets/
--rw-r--r--   0 phil       (501) staff       (20)     4913 2023-02-04 11:48:50.380605 PyQt6-6.4.2/sip/QtWidgets/QtWidgetsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2732 2023-02-04 11:48:50.398629 PyQt6-6.4.2/sip/QtWidgets/qabstractbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     2621 2023-02-04 11:48:50.330650 PyQt6-6.4.2/sip/QtWidgets/qabstractitemdelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)    10372 2023-02-04 11:48:50.293986 PyQt6-6.4.2/sip/QtWidgets/qabstractitemview.sip
--rw-r--r--   0 phil       (501) staff       (20)     3459 2023-02-04 11:48:50.423577 PyQt6-6.4.2/sip/QtWidgets/qabstractscrollarea.sip
--rw-r--r--   0 phil       (501) staff       (20)     3009 2023-02-04 11:48:50.280280 PyQt6-6.4.2/sip/QtWidgets/qabstractslider.sip
--rw-r--r--   0 phil       (501) staff       (20)     4021 2023-02-04 11:48:50.379249 PyQt6-6.4.2/sip/QtWidgets/qabstractspinbox.sip
--rw-r--r--   0 phil       (501) staff       (20)    14136 2023-02-04 11:48:50.345540 PyQt6-6.4.2/sip/QtWidgets/qapplication.sip
--rw-r--r--   0 phil       (501) staff       (20)     4795 2023-02-04 11:48:50.295383 PyQt6-6.4.2/sip/QtWidgets/qboxlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     1835 2023-02-04 11:48:50.324617 PyQt6-6.4.2/sip/QtWidgets/qbuttongroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     4043 2023-02-04 11:48:50.395990 PyQt6-6.4.2/sip/QtWidgets/qcalendarwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1799 2023-02-04 11:48:50.329010 PyQt6-6.4.2/sip/QtWidgets/qcheckbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2995 2023-02-04 11:48:50.349378 PyQt6-6.4.2/sip/QtWidgets/qcolordialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2872 2023-02-04 11:48:50.327645 PyQt6-6.4.2/sip/QtWidgets/qcolumnview.sip
--rw-r--r--   0 phil       (501) staff       (20)     6343 2023-02-04 11:48:50.430515 PyQt6-6.4.2/sip/QtWidgets/qcombobox.sip
--rw-r--r--   0 phil       (501) staff       (20)     1749 2023-02-04 11:48:50.391313 PyQt6-6.4.2/sip/QtWidgets/qcommandlinkbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     3141 2023-02-04 11:48:50.389985 PyQt6-6.4.2/sip/QtWidgets/qcommonstyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     3315 2023-02-04 11:48:50.299370 PyQt6-6.4.2/sip/QtWidgets/qcompleter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2437 2023-02-04 11:48:50.379788 PyQt6-6.4.2/sip/QtWidgets/qdatawidgetmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     5039 2023-02-04 11:48:50.392695 PyQt6-6.4.2/sip/QtWidgets/qdatetimeedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     1866 2023-02-04 11:48:50.292226 PyQt6-6.4.2/sip/QtWidgets/qdial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2692 2023-02-04 11:48:50.292750 PyQt6-6.4.2/sip/QtWidgets/qdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     3396 2023-02-04 11:48:50.381286 PyQt6-6.4.2/sip/QtWidgets/qdialogbuttonbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2666 2023-02-04 11:48:50.397210 PyQt6-6.4.2/sip/QtWidgets/qdockwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2730 2023-02-04 11:48:50.395319 PyQt6-6.4.2/sip/QtWidgets/qdrawutil.sip
--rw-r--r--   0 phil       (501) staff       (20)     1389 2023-02-04 11:48:50.326148 PyQt6-6.4.2/sip/QtWidgets/qerrormessage.sip
--rw-r--r--   0 phil       (501) staff       (20)    12183 2023-02-04 11:48:50.351401 PyQt6-6.4.2/sip/QtWidgets/qfiledialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     1261 2023-02-04 11:48:50.324152 PyQt6-6.4.2/sip/QtWidgets/qfileiconprovider.sip
--rw-r--r--   0 phil       (501) staff       (20)      957 2023-02-04 11:48:50.331087 PyQt6-6.4.2/sip/QtWidgets/qfilesystemmodel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1392 2023-02-04 11:48:50.428602 PyQt6-6.4.2/sip/QtWidgets/qfocusframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     2764 2023-02-04 11:48:50.294552 PyQt6-6.4.2/sip/QtWidgets/qfontcombobox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2916 2023-02-04 11:48:50.286873 PyQt6-6.4.2/sip/QtWidgets/qfontdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     4981 2023-02-04 11:48:50.286244 PyQt6-6.4.2/sip/QtWidgets/qformlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     2164 2023-02-04 11:48:50.277698 PyQt6-6.4.2/sip/QtWidgets/qframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     5339 2023-02-04 11:48:50.394450 PyQt6-6.4.2/sip/QtWidgets/qgesture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1738 2023-02-04 11:48:50.391762 PyQt6-6.4.2/sip/QtWidgets/qgesturerecognizer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-02-04 11:48:50.289004 PyQt6-6.4.2/sip/QtWidgets/qgraphicsanchorlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     5015 2023-02-04 11:48:50.429615 PyQt6-6.4.2/sip/QtWidgets/qgraphicseffect.sip
--rw-r--r--   0 phil       (501) staff       (20)     4207 2023-02-04 11:48:50.431196 PyQt6-6.4.2/sip/QtWidgets/qgraphicsgridlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)    26805 2023-02-04 11:48:50.426862 PyQt6-6.4.2/sip/QtWidgets/qgraphicsitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     1730 2023-02-04 11:48:50.282000 PyQt6-6.4.2/sip/QtWidgets/qgraphicslayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     3128 2023-02-04 11:48:50.289578 PyQt6-6.4.2/sip/QtWidgets/qgraphicslayoutitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     3150 2023-02-04 11:48:50.346842 PyQt6-6.4.2/sip/QtWidgets/qgraphicslinearlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     3920 2023-02-04 11:48:50.329645 PyQt6-6.4.2/sip/QtWidgets/qgraphicsproxywidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     8768 2023-02-04 11:48:50.382147 PyQt6-6.4.2/sip/QtWidgets/qgraphicsscene.sip
--rw-r--r--   0 phil       (501) staff       (20)     6166 2023-02-04 11:48:50.325738 PyQt6-6.4.2/sip/QtWidgets/qgraphicssceneevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2441 2023-02-04 11:48:50.377462 PyQt6-6.4.2/sip/QtWidgets/qgraphicstransform.sip
--rw-r--r--   0 phil       (501) staff       (20)     8125 2023-02-04 11:48:50.432154 PyQt6-6.4.2/sip/QtWidgets/qgraphicsview.sip
--rw-r--r--   0 phil       (501) staff       (20)     5459 2023-02-04 11:48:50.346297 PyQt6-6.4.2/sip/QtWidgets/qgraphicswidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     5537 2023-02-04 11:48:50.298698 PyQt6-6.4.2/sip/QtWidgets/qgridlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     2122 2023-02-04 11:48:50.373475 PyQt6-6.4.2/sip/QtWidgets/qgroupbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     7170 2023-02-04 11:48:50.331964 PyQt6-6.4.2/sip/QtWidgets/qheaderview.sip
--rw-r--r--   0 phil       (501) staff       (20)     5360 2023-02-04 11:48:50.278948 PyQt6-6.4.2/sip/QtWidgets/qinputdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     2931 2023-02-04 11:48:50.398082 PyQt6-6.4.2/sip/QtWidgets/qitemdelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1812 2023-02-04 11:48:50.341275 PyQt6-6.4.2/sip/QtWidgets/qitemeditorfactory.sip
--rw-r--r--   0 phil       (501) staff       (20)     1864 2023-02-04 11:48:50.278168 PyQt6-6.4.2/sip/QtWidgets/qkeysequenceedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     6063 2023-02-04 11:48:50.374725 PyQt6-6.4.2/sip/QtWidgets/qlabel.sip
--rw-r--r--   0 phil       (501) staff       (20)     5894 2023-02-04 11:48:50.287795 PyQt6-6.4.2/sip/QtWidgets/qlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     3732 2023-02-04 11:48:50.348000 PyQt6-6.4.2/sip/QtWidgets/qlayoutitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     2378 2023-02-04 11:48:50.276323 PyQt6-6.4.2/sip/QtWidgets/qlcdnumber.sip
--rw-r--r--   0 phil       (501) staff       (20)     5210 2023-02-04 11:48:50.342755 PyQt6-6.4.2/sip/QtWidgets/qlineedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     4961 2023-02-04 11:48:50.323712 PyQt6-6.4.2/sip/QtWidgets/qlistview.sip
--rw-r--r--   0 phil       (501) staff       (20)     7358 2023-02-04 11:48:50.388787 PyQt6-6.4.2/sip/QtWidgets/qlistwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     4691 2023-02-04 11:48:50.343785 PyQt6-6.4.2/sip/QtWidgets/qmainwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     4174 2023-02-04 11:48:50.279694 PyQt6-6.4.2/sip/QtWidgets/qmdiarea.sip
--rw-r--r--   0 phil       (501) staff       (20)     4054 2023-02-04 11:48:50.396705 PyQt6-6.4.2/sip/QtWidgets/qmdisubwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     5652 2023-02-04 11:48:50.291664 PyQt6-6.4.2/sip/QtWidgets/qmenu.sip
--rw-r--r--   0 phil       (501) staff       (20)     3601 2023-02-04 11:48:50.387761 PyQt6-6.4.2/sip/QtWidgets/qmenubar.sip
--rw-r--r--   0 phil       (501) staff       (20)     6307 2023-02-04 11:48:50.348831 PyQt6-6.4.2/sip/QtWidgets/qmessagebox.sip
--rw-r--r--   0 phil       (501) staff       (20)     7249 2023-02-04 11:48:50.384416 PyQt6-6.4.2/sip/QtWidgets/qplaintextedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     2226 2023-02-04 11:48:50.288377 PyQt6-6.4.2/sip/QtWidgets/qprogressbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2903 2023-02-04 11:48:50.281583 PyQt6-6.4.2/sip/QtWidgets/qprogressdialog.sip
--rw-r--r--   0 phil       (501) staff       (20)     3947 2023-02-04 11:48:50.280741 PyQt6-6.4.2/sip/QtWidgets/qproxystyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2069 2023-02-04 11:48:50.351872 PyQt6-6.4.2/sip/QtWidgets/qpushbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     2905 2023-02-04 11:48:50.376396 PyQt6-6.4.2/sip/QtWidgets/qpywidgets_qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1555 2023-02-04 11:48:50.390858 PyQt6-6.4.2/sip/QtWidgets/qradiobutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     1794 2023-02-04 11:48:50.347299 PyQt6-6.4.2/sip/QtWidgets/qrubberband.sip
--rw-r--r--   0 phil       (501) staff       (20)     1895 2023-02-04 11:48:50.383477 PyQt6-6.4.2/sip/QtWidgets/qscrollarea.sip
--rw-r--r--   0 phil       (501) staff       (20)     1773 2023-02-04 11:48:50.282503 PyQt6-6.4.2/sip/QtWidgets/qscrollbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2896 2023-02-04 11:48:50.332553 PyQt6-6.4.2/sip/QtWidgets/qscroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     2485 2023-02-04 11:48:50.341955 PyQt6-6.4.2/sip/QtWidgets/qscrollerproperties.sip
--rw-r--r--   0 phil       (501) staff       (20)     1640 2023-02-04 11:48:50.300365 PyQt6-6.4.2/sip/QtWidgets/qsizegrip.sip
--rw-r--r--   0 phil       (501) staff       (20)     3272 2023-02-04 11:48:50.328415 PyQt6-6.4.2/sip/QtWidgets/qsizepolicy.sip
--rw-r--r--   0 phil       (501) staff       (20)     1921 2023-02-04 11:48:50.387010 PyQt6-6.4.2/sip/QtWidgets/qslider.sip
--rw-r--r--   0 phil       (501) staff       (20)     3301 2023-02-04 11:48:50.349997 PyQt6-6.4.2/sip/QtWidgets/qspinbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     1798 2023-02-04 11:48:50.296575 PyQt6-6.4.2/sip/QtWidgets/qsplashscreen.sip
--rw-r--r--   0 phil       (501) staff       (20)     3429 2023-02-04 11:48:50.382915 PyQt6-6.4.2/sip/QtWidgets/qsplitter.sip
--rw-r--r--   0 phil       (501) staff       (20)     3651 2023-02-04 11:48:50.375568 PyQt6-6.4.2/sip/QtWidgets/qstackedlayout.sip
--rw-r--r--   0 phil       (501) staff       (20)     1662 2023-02-04 11:48:50.394911 PyQt6-6.4.2/sip/QtWidgets/qstackedwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1956 2023-02-04 11:48:50.297846 PyQt6-6.4.2/sip/QtWidgets/qstatusbar.sip
--rw-r--r--   0 phil       (501) staff       (20)    22575 2023-02-04 11:48:50.285346 PyQt6-6.4.2/sip/QtWidgets/qstyle.sip
--rw-r--r--   0 phil       (501) staff       (20)     2426 2023-02-04 11:48:50.376865 PyQt6-6.4.2/sip/QtWidgets/qstyleditemdelegate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1122 2023-02-04 11:48:50.297319 PyQt6-6.4.2/sip/QtWidgets/qstylefactory.sip
--rw-r--r--   0 phil       (501) staff       (20)    20087 2023-02-04 11:48:50.336532 PyQt6-6.4.2/sip/QtWidgets/qstyleoption.sip
--rw-r--r--   0 phil       (501) staff       (20)     1732 2023-02-04 11:48:50.397630 PyQt6-6.4.2/sip/QtWidgets/qstylepainter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2317 2023-02-04 11:48:50.330189 PyQt6-6.4.2/sip/QtWidgets/qsystemtrayicon.sip
--rw-r--r--   0 phil       (501) staff       (20)     5251 2023-02-04 11:48:50.337535 PyQt6-6.4.2/sip/QtWidgets/qtabbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     4837 2023-02-04 11:48:50.393421 PyQt6-6.4.2/sip/QtWidgets/qtableview.sip
--rw-r--r--   0 phil       (501) staff       (20)     9246 2023-02-04 11:48:50.290876 PyQt6-6.4.2/sip/QtWidgets/qtablewidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     4240 2023-02-04 11:48:50.338271 PyQt6-6.4.2/sip/QtWidgets/qtabwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-02-04 11:48:50.327146 PyQt6-6.4.2/sip/QtWidgets/qtextbrowser.sip
--rw-r--r--   0 phil       (501) staff       (20)     7388 2023-02-04 11:48:50.386562 PyQt6-6.4.2/sip/QtWidgets/qtextedit.sip
--rw-r--r--   0 phil       (501) staff       (20)     4343 2023-02-04 11:48:50.296148 PyQt6-6.4.2/sip/QtWidgets/qtoolbar.sip
--rw-r--r--   0 phil       (501) staff       (20)     2421 2023-02-04 11:48:50.299847 PyQt6-6.4.2/sip/QtWidgets/qtoolbox.sip
--rw-r--r--   0 phil       (501) staff       (20)     2556 2023-02-04 11:48:50.378526 PyQt6-6.4.2/sip/QtWidgets/qtoolbutton.sip
--rw-r--r--   0 phil       (501) staff       (20)     1399 2023-02-04 11:48:50.343148 PyQt6-6.4.2/sip/QtWidgets/qtooltip.sip
--rw-r--r--   0 phil       (501) staff       (20)     6474 2023-02-04 11:48:50.277159 PyQt6-6.4.2/sip/QtWidgets/qtreeview.sip
--rw-r--r--   0 phil       (501) staff       (20)    10328 2023-02-04 11:48:50.385554 PyQt6-6.4.2/sip/QtWidgets/qtreewidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2195 2023-02-04 11:48:50.377971 PyQt6-6.4.2/sip/QtWidgets/qtreewidgetitemiterator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1597 2023-02-04 11:48:50.326584 PyQt6-6.4.2/sip/QtWidgets/qundoview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1353 2023-02-04 11:48:50.389348 PyQt6-6.4.2/sip/QtWidgets/qwhatsthis.sip
--rw-r--r--   0 phil       (501) staff       (20)    18362 2023-02-04 11:48:50.340659 PyQt6-6.4.2/sip/QtWidgets/qwidget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1627 2023-02-04 11:48:50.296966 PyQt6-6.4.2/sip/QtWidgets/qwidgetaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     7633 2023-02-04 11:48:50.428139 PyQt6-6.4.2/sip/QtWidgets/qwizard.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.250850 PyQt6-6.4.2/sip/QtXml/
--rw-r--r--   0 phil       (501) staff       (20)     1925 2023-02-04 11:48:49.997535 PyQt6-6.4.2/sip/QtXml/QtXmlmod.sip
--rw-r--r--   0 phil       (501) staff       (20)    14767 2023-02-04 11:48:49.997028 PyQt6-6.4.2/sip/QtXml/qdom.sip
--rw-r--r--   0 phil       (501) staff       (20)       22 2023-02-04 11:48:49.774678 PyQt6-6.4.2/sip/pyqt-gpl.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.068661 PyQt6-6.4.2/uic/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.071479 PyQt6-6.4.2/uic/Compiler/
--rw-r--r--   0 phil       (501) staff       (20)     1004 2023-02-04 11:48:42.746445 PyQt6-6.4.2/uic/Compiler/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     1412 2023-02-04 11:48:42.749345 PyQt6-6.4.2/uic/Compiler/as_string.py
--rw-r--r--   0 phil       (501) staff       (20)     3934 2023-02-04 11:48:42.745939 PyQt6-6.4.2/uic/Compiler/compiler.py
--rw-r--r--   0 phil       (501) staff       (20)     2742 2023-02-04 11:48:42.747067 PyQt6-6.4.2/uic/Compiler/indenter.py
--rw-r--r--   0 phil       (501) staff       (20)     2374 2023-02-04 11:48:42.744855 PyQt6-6.4.2/uic/Compiler/misc.py
--rw-r--r--   0 phil       (501) staff       (20)     4324 2023-02-04 11:48:42.748926 PyQt6-6.4.2/uic/Compiler/proxy_metaclass.py
--rw-r--r--   0 phil       (501) staff       (20)     5839 2023-02-04 11:48:42.748196 PyQt6-6.4.2/uic/Compiler/qobjectcreator.py
--rw-r--r--   0 phil       (501) staff       (20)    16164 2023-02-04 11:48:42.751752 PyQt6-6.4.2/uic/Compiler/qtproxies.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.068315 PyQt6-6.4.2/uic/Loader/
--rw-r--r--   0 phil       (501) staff       (20)     1004 2023-02-04 11:48:42.739359 PyQt6-6.4.2/uic/Loader/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2625 2023-02-04 11:48:42.740996 PyQt6-6.4.2/uic/Loader/loader.py
--rw-r--r--   0 phil       (501) staff       (20)     5187 2023-02-04 11:48:42.740336 PyQt6-6.4.2/uic/Loader/qobjectcreator.py
--rw-r--r--   0 phil       (501) staff       (20)     1003 2023-02-04 11:48:42.738560 PyQt6-6.4.2/uic/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5473 2023-02-04 11:48:42.752930 PyQt6-6.4.2/uic/compile_ui.py
--rw-r--r--   0 phil       (501) staff       (20)    31764 2023-02-04 11:48:42.738201 PyQt6-6.4.2/uic/enum_map.py
--rw-r--r--   0 phil       (501) staff       (20)     2609 2023-02-04 11:48:42.743344 PyQt6-6.4.2/uic/exceptions.py
--rw-r--r--   0 phil       (501) staff       (20)     5047 2023-02-04 11:48:42.742011 PyQt6-6.4.2/uic/icon_cache.py
--rw-r--r--   0 phil       (501) staff       (20)     3327 2023-02-04 11:48:42.742692 PyQt6-6.4.2/uic/load_ui.py
--rw-r--r--   0 phil       (501) staff       (20)     6097 2023-02-04 11:48:42.728942 PyQt6-6.4.2/uic/objcreator.py
--rw-r--r--   0 phil       (501) staff       (20)    18275 2023-02-04 11:48:42.731845 PyQt6-6.4.2/uic/properties.py
--rw-r--r--   0 phil       (501) staff       (20)     4653 2023-02-04 11:48:42.744095 PyQt6-6.4.2/uic/pyuic.py
--rw-r--r--   0 phil       (501) staff       (20)     3213 2023-02-04 11:48:42.723100 PyQt6-6.4.2/uic/ui_file.py
--rw-r--r--   0 phil       (501) staff       (20)    37502 2023-02-04 11:48:42.727838 PyQt6-6.4.2/uic/uiparser.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-02-04 11:48:54.067113 PyQt6-6.4.2/uic/widget-plugins/
--rw-r--r--   0 phil       (501) staff       (20)     1557 2023-02-04 11:48:42.735419 PyQt6-6.4.2/uic/widget-plugins/qaxcontainer.py
--rw-r--r--   0 phil       (501) staff       (20)     1553 2023-02-04 11:48:42.732751 PyQt6-6.4.2/uic/widget-plugins/qscintilla.py
--rw-r--r--   0 phil       (501) staff       (20)     1562 2023-02-04 11:48:42.733883 PyQt6-6.4.2/uic/widget-plugins/qtcharts.py
--rw-r--r--   0 phil       (501) staff       (20)     1588 2023-02-04 11:48:42.734408 PyQt6-6.4.2/uic/widget-plugins/qtprintsupport.py
--rw-r--r--   0 phil       (501) staff       (20)     1562 2023-02-04 11:48:42.734835 PyQt6-6.4.2/uic/widget-plugins/qtquickwidgets.py
--rw-r--r--   0 phil       (501) staff       (20)     1568 2023-02-04 11:48:42.733246 PyQt6-6.4.2/uic/widget-plugins/qtwebenginewidgets.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.787990 PyQt6-6.5.0/
+-rw-r--r--   0 phil       (501) staff       (20)   118547 2023-04-05 12:16:47.435856 PyQt6-6.5.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-05 12:16:46.806233 PyQt6-6.5.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)     3204 2023-04-05 12:16:47.437537 PyQt6-6.5.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     2075 2023-04-05 12:16:56.788123 PyQt6-6.5.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1735 2023-04-05 12:16:47.681962 PyQt6-6.5.0/README
+-rw-r--r--   0 phil       (501) staff       (20)      960 2023-04-05 12:16:47.448166 PyQt6-6.5.0/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.406566 PyQt6-6.5.0/config-tests/
+-rw-r--r--   0 phil       (501) staff       (20)      756 2023-04-05 12:16:47.446821 PyQt6-6.5.0/config-tests/cfgtest_QtCore.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      813 2023-04-05 12:16:47.445301 PyQt6-6.5.0/config-tests/cfgtest_QtGui.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      569 2023-04-05 12:16:47.447534 PyQt6-6.5.0/config-tests/cfgtest_QtNetwork.cpp
+-rw-r--r--   0 phil       (501) staff       (20)      752 2023-04-05 12:16:47.446224 PyQt6-6.5.0/config-tests/cfgtest_QtPrintSupport.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.404886 PyQt6-6.5.0/dbus/
+-rw-r--r--   0 phil       (501) staff       (20)    11344 2023-04-05 12:16:47.675820 PyQt6-6.5.0/dbus/dbus.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2067 2023-04-05 12:16:47.673592 PyQt6-6.5.0/dbus/helper.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.528614 PyQt6-6.5.0/designer/
+-rw-r--r--   0 phil       (501) staff       (20)      435 2023-04-05 12:16:47.676338 PyQt6-6.5.0/designer/designer.pro-in
+-rw-r--r--   0 phil       (501) staff       (20)     9229 2023-04-05 12:16:47.677933 PyQt6-6.5.0/designer/pluginloader.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1982 2023-04-05 12:16:47.678372 PyQt6-6.5.0/designer/pluginloader.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.526970 PyQt6-6.5.0/examples/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.518158 PyQt6-6.5.0/examples/designer/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.519020 PyQt6-6.5.0/examples/designer/calculatorform/
+-rw-r--r--   0 phil       (501) staff       (20)     2805 2023-04-05 11:42:27.292690 PyQt6-6.5.0/examples/designer/calculatorform/calculatorform.py
+-rw-r--r--   0 phil       (501) staff       (20)     7150 2023-04-05 11:42:27.293101 PyQt6-6.5.0/examples/designer/calculatorform/calculatorform.ui
+-rw-r--r--   0 phil       (501) staff       (20)     5538 2023-04-05 11:42:27.297877 PyQt6-6.5.0/examples/designer/calculatorform/ui_calculatorform.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.514743 PyQt6-6.5.0/examples/designer/plugins/
+-rw-r--r--   0 phil       (501) staff       (20)     3578 2023-04-05 11:42:27.289630 PyQt6-6.5.0/examples/designer/plugins/plugins.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.514351 PyQt6-6.5.0/examples/designer/plugins/python/
+-rw-r--r--   0 phil       (501) staff       (20)     5548 2023-04-05 11:42:27.291092 PyQt6-6.5.0/examples/designer/plugins/python/analogclockplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     5106 2023-04-05 11:42:27.291624 PyQt6-6.5.0/examples/designer/plugins/python/bubbleswidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     3447 2023-04-05 11:42:27.416821 PyQt6-6.5.0/examples/designer/plugins/python/counterlabelplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4401 2023-04-05 11:42:27.291427 PyQt6-6.5.0/examples/designer/plugins/python/datetimeeditplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     3566 2023-04-05 11:42:27.292829 PyQt6-6.5.0/examples/designer/plugins/python/helloglwidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     5126 2023-04-05 11:42:27.292459 PyQt6-6.5.0/examples/designer/plugins/python/multipagewidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4714 2023-04-05 11:42:27.295611 PyQt6-6.5.0/examples/designer/plugins/python/polygonwidgetplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4184 2023-04-05 11:42:27.295513 PyQt6-6.5.0/examples/designer/plugins/python/pydemoplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     4612 2023-04-05 11:42:27.294802 PyQt6-6.5.0/examples/designer/plugins/python/pythonconsoleplugin.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.517853 PyQt6-6.5.0/examples/designer/plugins/widgets/
+-rw-r--r--   0 phil       (501) staff       (20)     6253 2023-04-05 11:42:27.294957 PyQt6-6.5.0/examples/designer/plugins/widgets/analogclock.py
+-rw-r--r--   0 phil       (501) staff       (20)    10365 2023-04-05 11:42:27.299748 PyQt6-6.5.0/examples/designer/plugins/widgets/bubbleswidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     5187 2023-04-05 11:42:27.291329 PyQt6-6.5.0/examples/designer/plugins/widgets/counterlabel.py
+-rw-r--r--   0 phil       (501) staff       (20)    16152 2023-04-05 11:42:27.292533 PyQt6-6.5.0/examples/designer/plugins/widgets/datetimeedit.py
+-rw-r--r--   0 phil       (501) staff       (20)     8302 2023-04-05 11:42:27.293399 PyQt6-6.5.0/examples/designer/plugins/widgets/helloglwidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     3985 2023-04-05 11:42:27.417628 PyQt6-6.5.0/examples/designer/plugins/widgets/multipagewidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     5827 2023-04-05 11:42:27.293032 PyQt6-6.5.0/examples/designer/plugins/widgets/polygonwidget.py
+-rw-r--r--   0 phil       (501) staff       (20)     5619 2023-04-05 11:42:27.294561 PyQt6-6.5.0/examples/designer/plugins/widgets/pydemo.py
+-rw-r--r--   0 phil       (501) staff       (20)     3016 2023-04-05 11:42:27.294137 PyQt6-6.5.0/examples/designer/plugins/widgets/pythonconsolewidget.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.505487 PyQt6-6.5.0/examples/desktop/
+-rw-r--r--   0 phil       (501) staff       (20)     6605 2023-04-05 11:42:27.297148 PyQt6-6.5.0/examples/desktop/screenshot.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.505901 PyQt6-6.5.0/examples/desktop/systray/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.506868 PyQt6-6.5.0/examples/desktop/systray/images/
+-rw-r--r--   0 phil       (501) staff       (20)     2496 2023-04-05 11:42:27.297138 PyQt6-6.5.0/examples/desktop/systray/images/bad.png
+-rw-r--r--   0 phil       (501) staff       (20)    25780 2023-04-05 11:42:27.297524 PyQt6-6.5.0/examples/desktop/systray/images/heart.png
+-rw-r--r--   0 phil       (501) staff       (20)    12128 2023-04-05 11:42:27.297407 PyQt6-6.5.0/examples/desktop/systray/images/trash.png
+-rw-r--r--   0 phil       (501) staff       (20)     9595 2023-04-05 11:42:27.301374 PyQt6-6.5.0/examples/desktop/systray/systray.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.524888 PyQt6-6.5.0/examples/dialogs/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.522234 PyQt6-6.5.0/examples/dialogs/classwizard/
+-rw-r--r--   0 phil       (501) staff       (20)    15515 2023-04-05 11:42:27.293489 PyQt6-6.5.0/examples/dialogs/classwizard/classwizard.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.524546 PyQt6-6.5.0/examples/dialogs/classwizard/images/
+-rw-r--r--   0 phil       (501) staff       (20)    22578 2023-04-05 11:42:27.294930 PyQt6-6.5.0/examples/dialogs/classwizard/images/background.png
+-rw-r--r--   0 phil       (501) staff       (20)     3947 2023-04-05 11:42:27.295131 PyQt6-6.5.0/examples/dialogs/classwizard/images/banner.png
+-rw-r--r--   0 phil       (501) staff       (20)     1619 2023-04-05 11:42:27.418288 PyQt6-6.5.0/examples/dialogs/classwizard/images/logo1.png
+-rw-r--r--   0 phil       (501) staff       (20)     1619 2023-04-05 11:42:27.294902 PyQt6-6.5.0/examples/dialogs/classwizard/images/logo2.png
+-rw-r--r--   0 phil       (501) staff       (20)     1619 2023-04-05 11:42:27.296111 PyQt6-6.5.0/examples/dialogs/classwizard/images/logo3.png
+-rw-r--r--   0 phil       (501) staff       (20)    14516 2023-04-05 11:42:27.296341 PyQt6-6.5.0/examples/dialogs/classwizard/images/watermark1.png
+-rw-r--r--   0 phil       (501) staff       (20)    14912 2023-04-05 11:42:27.298856 PyQt6-6.5.0/examples/dialogs/classwizard/images/watermark2.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.525583 PyQt6-6.5.0/examples/dialogs/configdialog/
+-rw-r--r--   0 phil       (501) staff       (20)     8989 2023-04-05 11:42:27.299045 PyQt6-6.5.0/examples/dialogs/configdialog/configdialog.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.526523 PyQt6-6.5.0/examples/dialogs/configdialog/images/
+-rw-r--r--   0 phil       (501) staff       (20)     7059 2023-04-05 11:42:27.299546 PyQt6-6.5.0/examples/dialogs/configdialog/images/config.png
+-rw-r--r--   0 phil       (501) staff       (20)     2269 2023-04-05 11:42:27.299269 PyQt6-6.5.0/examples/dialogs/configdialog/images/query.png
+-rw-r--r--   0 phil       (501) staff       (20)     8296 2023-04-05 11:42:27.303442 PyQt6-6.5.0/examples/dialogs/configdialog/images/update.png
+-rw-r--r--   0 phil       (501) staff       (20)     4434 2023-04-05 11:42:27.295392 PyQt6-6.5.0/examples/dialogs/extension.py
+-rw-r--r--   0 phil       (501) staff       (20)     8264 2023-04-05 11:42:27.296508 PyQt6-6.5.0/examples/dialogs/findfiles.py
+-rw-r--r--   0 phil       (501) staff       (20)    13995 2023-04-05 11:42:27.296716 PyQt6-6.5.0/examples/dialogs/standarddialogs.py
+-rw-r--r--   0 phil       (501) staff       (20)     7401 2023-04-05 11:42:27.418889 PyQt6-6.5.0/examples/dialogs/tabdialog.py
+-rw-r--r--   0 phil       (501) staff       (20)     3603 2023-04-05 11:42:27.295955 PyQt6-6.5.0/examples/dialogs/trivialwizard.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.460160 PyQt6-6.5.0/examples/draganddrop/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.459258 PyQt6-6.5.0/examples/draganddrop/delayedencoding/
+-rw-r--r--   0 phil       (501) staff       (20)     4979 2023-04-05 11:42:27.297534 PyQt6-6.5.0/examples/draganddrop/delayedencoding/delayedencoding.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.459781 PyQt6-6.5.0/examples/draganddrop/delayedencoding/images/
+-rw-r--r--   0 phil       (501) staff       (20)      977 2023-04-05 11:42:27.298282 PyQt6-6.5.0/examples/draganddrop/delayedencoding/images/drag.png
+-rw-r--r--   0 phil       (501) staff       (20)     2689 2023-04-05 11:42:27.300410 PyQt6-6.5.0/examples/draganddrop/delayedencoding/images/example.svg
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.456592 PyQt6-6.5.0/examples/draganddrop/draggableicons/
+-rw-r--r--   0 phil       (501) staff       (20)     5975 2023-04-05 11:42:27.300553 PyQt6-6.5.0/examples/draganddrop/draggableicons/draggableicons.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.457456 PyQt6-6.5.0/examples/draganddrop/draggableicons/images/
+-rw-r--r--   0 phil       (501) staff       (20)     2772 2023-04-05 11:42:27.301031 PyQt6-6.5.0/examples/draganddrop/draggableicons/images/boat.png
+-rw-r--r--   0 phil       (501) staff       (20)     2963 2023-04-05 11:42:27.300962 PyQt6-6.5.0/examples/draganddrop/draggableicons/images/car.png
+-rw-r--r--   0 phil       (501) staff       (20)     3292 2023-04-05 11:42:27.304863 PyQt6-6.5.0/examples/draganddrop/draggableicons/images/house.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.458416 PyQt6-6.5.0/examples/draganddrop/draggabletext/
+-rw-r--r--   0 phil       (501) staff       (20)     5414 2023-04-05 11:42:27.297232 PyQt6-6.5.0/examples/draganddrop/draggabletext/draggabletext.py
+-rw-r--r--   0 phil       (501) staff       (20)      247 2023-04-05 11:42:27.297796 PyQt6-6.5.0/examples/draganddrop/draggabletext/words.txt
+-rw-r--r--   0 phil       (501) staff       (20)     6826 2023-04-05 11:42:27.298271 PyQt6-6.5.0/examples/draganddrop/dropsite.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.460787 PyQt6-6.5.0/examples/draganddrop/fridgemagnets/
+-rw-r--r--   0 phil       (501) staff       (20)     6903 2023-04-05 11:42:27.419677 PyQt6-6.5.0/examples/draganddrop/fridgemagnets/fridgemagnets.py
+-rw-r--r--   0 phil       (501) staff       (20)      278 2023-04-05 11:42:27.297380 PyQt6-6.5.0/examples/draganddrop/fridgemagnets/words.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.455725 PyQt6-6.5.0/examples/draganddrop/puzzle/
+-rw-r--r--   0 phil       (501) staff       (20)    42654 2023-04-05 11:42:27.300219 PyQt6-6.5.0/examples/draganddrop/puzzle/example.jpg
+-rw-r--r--   0 phil       (501) staff       (20)    12900 2023-04-05 11:42:27.299977 PyQt6-6.5.0/examples/draganddrop/puzzle/puzzle.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.507585 PyQt6-6.5.0/examples/multimedia/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.508474 PyQt6-6.5.0/examples/multimedia/audiodevices/
+-rw-r--r--   0 phil       (501) staff       (20)     7889 2023-04-05 11:42:27.302192 PyQt6-6.5.0/examples/multimedia/audiodevices/audiodevices.py
+-rw-r--r--   0 phil       (501) staff       (20)    11927 2023-04-05 11:42:27.302083 PyQt6-6.5.0/examples/multimedia/audiodevices/audiodevicesbase.ui
+-rw-r--r--   0 phil       (501) staff       (20)    12232 2023-04-05 11:42:27.302586 PyQt6-6.5.0/examples/multimedia/audiodevices/ui_audiodevicesbase.py
+-rw-r--r--   0 phil       (501) staff       (20)     9047 2023-04-05 11:42:27.302360 PyQt6-6.5.0/examples/multimedia/audiooutput.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.467302 PyQt6-6.5.0/examples/multimediawidgets/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.470203 PyQt6-6.5.0/examples/multimediawidgets/camera/
+-rw-r--r--   0 phil       (501) staff       (20)    21481 2023-04-05 11:42:27.307109 PyQt6-6.5.0/examples/multimediawidgets/camera/camera.py
+-rw-r--r--   0 phil       (501) staff       (20)    13064 2023-04-05 11:42:27.299413 PyQt6-6.5.0/examples/multimediawidgets/camera/camera.ui
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.470324 PyQt6-6.5.0/examples/multimediawidgets/camera/images/
+-rw-r--r--   0 phil       (501) staff       (20)     1491 2023-04-05 11:42:27.299633 PyQt6-6.5.0/examples/multimediawidgets/camera/images/shutter.svg
+-rw-r--r--   0 phil       (501) staff       (20)     3290 2023-04-05 11:42:27.299631 PyQt6-6.5.0/examples/multimediawidgets/camera/imagesettings.ui
+-rw-r--r--   0 phil       (501) staff       (20)    10689 2023-04-05 11:42:27.420357 PyQt6-6.5.0/examples/multimediawidgets/camera/ui_camera.py
+-rw-r--r--   0 phil       (501) staff       (20)     3453 2023-04-05 11:42:27.299194 PyQt6-6.5.0/examples/multimediawidgets/camera/ui_imagesettings.py
+-rw-r--r--   0 phil       (501) staff       (20)     6492 2023-04-05 11:42:27.301828 PyQt6-6.5.0/examples/multimediawidgets/camera/ui_videosettings.py
+-rw-r--r--   0 phil       (501) staff       (20)     5727 2023-04-05 11:42:27.301694 PyQt6-6.5.0/examples/multimediawidgets/camera/videosettings.ui
+-rw-r--r--   0 phil       (501) staff       (20)     6277 2023-04-05 11:42:27.304052 PyQt6-6.5.0/examples/multimediawidgets/videographicsitem.py
+-rw-r--r--   0 phil       (501) staff       (20)     5857 2023-04-05 11:42:27.303851 PyQt6-6.5.0/examples/multimediawidgets/videowidget.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.461236 PyQt6-6.5.0/examples/qml/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.465797 PyQt6-6.5.0/examples/qml/referenceexamples/
+-rwxr-xr-x   0 phil       (501) staff       (20)     3228 2023-04-05 11:42:27.304054 PyQt6-6.5.0/examples/qml/referenceexamples/adding.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     6032 2023-04-05 11:42:27.303769 PyQt6-6.5.0/examples/qml/referenceexamples/attached.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     8823 2023-04-05 11:42:27.308921 PyQt6-6.5.0/examples/qml/referenceexamples/binding.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     4133 2023-04-05 11:42:27.301359 PyQt6-6.5.0/examples/qml/referenceexamples/coercion.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     4168 2023-04-05 11:42:27.301160 PyQt6-6.5.0/examples/qml/referenceexamples/default.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     5630 2023-04-05 11:42:27.301153 PyQt6-6.5.0/examples/qml/referenceexamples/grouped.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     4157 2023-04-05 11:42:27.421005 PyQt6-6.5.0/examples/qml/referenceexamples/methods.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     3945 2023-04-05 11:42:27.301127 PyQt6-6.5.0/examples/qml/referenceexamples/properties.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     6504 2023-04-05 11:42:27.303428 PyQt6-6.5.0/examples/qml/referenceexamples/signal.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     8821 2023-04-05 11:42:27.303343 PyQt6-6.5.0/examples/qml/referenceexamples/valuesource.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.504245 PyQt6-6.5.0/examples/quick/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.478244 PyQt6-6.5.0/examples/quick/animation/
+-rw-r--r--   0 phil       (501) staff       (20)     2415 2023-04-05 11:42:27.305481 PyQt6-6.5.0/examples/quick/animation/animation.py
+-rw-r--r--   0 phil       (501) staff       (20)     3371 2023-04-05 11:42:27.305262 PyQt6-6.5.0/examples/quick/animation/animation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.472490 PyQt6-6.5.0/examples/quick/animation/basics/
+-rw-r--r--   0 phil       (501) staff       (20)     4957 2023-04-05 11:42:27.305674 PyQt6-6.5.0/examples/quick/animation/basics/color-animation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.474026 PyQt6-6.5.0/examples/quick/animation/basics/images/
+-rw-r--r--   0 phil       (501) staff       (20)    15408 2023-04-05 11:42:27.305868 PyQt6-6.5.0/examples/quick/animation/basics/images/face-smile.png
+-rw-r--r--   0 phil       (501) staff       (20)     2433 2023-04-05 11:42:27.310921 PyQt6-6.5.0/examples/quick/animation/basics/images/moon.png
+-rw-r--r--   0 phil       (501) staff       (20)      425 2023-04-05 11:42:27.303338 PyQt6-6.5.0/examples/quick/animation/basics/images/shadow.png
+-rw-r--r--   0 phil       (501) staff       (20)      349 2023-04-05 11:42:27.303253 PyQt6-6.5.0/examples/quick/animation/basics/images/star.png
+-rw-r--r--   0 phil       (501) staff       (20)     8153 2023-04-05 11:42:27.303170 PyQt6-6.5.0/examples/quick/animation/basics/images/sun.png
+-rw-r--r--   0 phil       (501) staff       (20)     4187 2023-04-05 11:42:27.421720 PyQt6-6.5.0/examples/quick/animation/basics/property-animation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.477767 PyQt6-6.5.0/examples/quick/animation/behaviors/
+-rw-r--r--   0 phil       (501) staff       (20)     2401 2023-04-05 11:42:27.303041 PyQt6-6.5.0/examples/quick/animation/behaviors/SideRect.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4444 2023-04-05 11:42:27.305521 PyQt6-6.5.0/examples/quick/animation/behaviors/behavior-example.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4376 2023-04-05 11:42:27.305358 PyQt6-6.5.0/examples/quick/animation/behaviors/tvtennis.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4090 2023-04-05 11:42:27.306839 PyQt6-6.5.0/examples/quick/animation/behaviors/wigglytext.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.474549 PyQt6-6.5.0/examples/quick/animation/easing/
+-rw-r--r--   0 phil       (501) staff       (20)     8398 2023-04-05 11:42:27.307330 PyQt6-6.5.0/examples/quick/animation/easing/easing.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.475641 PyQt6-6.5.0/examples/quick/animation/pathanimation/
+-rw-r--r--   0 phil       (501) staff       (20)     3407 2023-04-05 11:42:27.307403 PyQt6-6.5.0/examples/quick/animation/pathanimation/pathanimation.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.475015 PyQt6-6.5.0/examples/quick/animation/pathinterpolator/
+-rw-r--r--   0 phil       (501) staff       (20)     3596 2023-04-05 11:42:27.307494 PyQt6-6.5.0/examples/quick/animation/pathinterpolator/pathinterpolator.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.479727 PyQt6-6.5.0/examples/quick/animation/states/
+-rw-r--r--   0 phil       (501) staff       (20)     5149 2023-04-05 11:42:27.312476 PyQt6-6.5.0/examples/quick/animation/states/qt-logo.png
+-rw-r--r--   0 phil       (501) staff       (20)     3876 2023-04-05 11:42:27.304889 PyQt6-6.5.0/examples/quick/animation/states/states.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4932 2023-04-05 11:42:27.304933 PyQt6-6.5.0/examples/quick/animation/states/transitions.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.496567 PyQt6-6.5.0/examples/quick/canvas/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.496088 PyQt6-6.5.0/examples/quick/canvas/bezierCurve/
+-rw-r--r--   0 phil       (501) staff       (20)     4728 2023-04-05 11:42:27.304933 PyQt6-6.5.0/examples/quick/canvas/bezierCurve/bezierCurve.qml
+-rw-r--r--   0 phil       (501) staff       (20)     2412 2023-04-05 11:42:27.422365 PyQt6-6.5.0/examples/quick/canvas/canvas.py
+-rw-r--r--   0 phil       (501) staff       (20)     3069 2023-04-05 11:42:27.304775 PyQt6-6.5.0/examples/quick/canvas/canvas.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.493296 PyQt6-6.5.0/examples/quick/canvas/clip/
+-rw-r--r--   0 phil       (501) staff       (20)     5037 2023-04-05 11:42:27.307030 PyQt6-6.5.0/examples/quick/canvas/clip/clip.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.488146 PyQt6-6.5.0/examples/quick/canvas/contents/
+-rw-r--r--   0 phil       (501) staff       (20)     3026 2023-04-05 11:42:27.306778 PyQt6-6.5.0/examples/quick/canvas/contents/Button.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3391 2023-04-05 11:42:27.308526 PyQt6-6.5.0/examples/quick/canvas/contents/ScrollBar.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3915 2023-04-05 11:42:27.309081 PyQt6-6.5.0/examples/quick/canvas/contents/Slider.qml
+-rw-r--r--   0 phil       (501) staff       (20)     2826 2023-04-05 11:42:27.309546 PyQt6-6.5.0/examples/quick/canvas/contents/TitleBar.qml
+-rw-r--r--   0 phil       (501) staff       (20)     2564 2023-04-05 11:42:27.308794 PyQt6-6.5.0/examples/quick/canvas/contents/ToolBar.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.492729 PyQt6-6.5.0/examples/quick/canvas/contents/images/
+-rw-r--r--   0 phil       (501) staff       (20)      571 2023-04-05 11:42:27.314649 PyQt6-6.5.0/examples/quick/canvas/contents/images/button-pressed.png
+-rw-r--r--   0 phil       (501) staff       (20)      564 2023-04-05 11:42:27.306400 PyQt6-6.5.0/examples/quick/canvas/contents/images/button.png
+-rw-r--r--   0 phil       (501) staff       (20)     7458 2023-04-05 11:42:27.306550 PyQt6-6.5.0/examples/quick/canvas/contents/images/default.svg
+-rw-r--r--   0 phil       (501) staff       (20)     1236 2023-04-05 11:42:27.306314 PyQt6-6.5.0/examples/quick/canvas/contents/images/gloss.png
+-rw-r--r--   0 phil       (501) staff       (20)     1415 2023-04-05 11:42:27.423063 PyQt6-6.5.0/examples/quick/canvas/contents/images/lineedit.png
+-rw-r--r--   0 phil       (501) staff       (20)       87 2023-04-05 11:42:27.306370 PyQt6-6.5.0/examples/quick/canvas/contents/images/lineedit.sci
+-rw-r--r--   0 phil       (501) staff       (20)     2369 2023-04-05 11:42:27.308712 PyQt6-6.5.0/examples/quick/canvas/contents/images/quit.png
+-rw-r--r--   0 phil       (501) staff       (20)      257 2023-04-05 11:42:27.308337 PyQt6-6.5.0/examples/quick/canvas/contents/images/stripes.png
+-rw-r--r--   0 phil       (501) staff       (20)     1436 2023-04-05 11:42:27.309998 PyQt6-6.5.0/examples/quick/canvas/contents/images/titlebar.png
+-rw-r--r--   0 phil       (501) staff       (20)       87 2023-04-05 11:42:27.311189 PyQt6-6.5.0/examples/quick/canvas/contents/images/titlebar.sci
+-rw-r--r--   0 phil       (501) staff       (20)     2550 2023-04-05 11:42:27.311353 PyQt6-6.5.0/examples/quick/canvas/contents/images/toolbutton.png
+-rw-r--r--   0 phil       (501) staff       (20)       87 2023-04-05 11:42:27.310441 PyQt6-6.5.0/examples/quick/canvas/contents/images/toolbutton.sci
+-rw-r--r--   0 phil       (501) staff       (20)    23519 2023-04-05 11:42:27.316391 PyQt6-6.5.0/examples/quick/canvas/contents/qt-logo.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.494727 PyQt6-6.5.0/examples/quick/canvas/quadraticCurveTo/
+-rw-r--r--   0 phil       (501) staff       (20)     4992 2023-04-05 11:42:27.308078 PyQt6-6.5.0/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.485538 PyQt6-6.5.0/examples/quick/canvas/roundedrect/
+-rw-r--r--   0 phil       (501) staff       (20)     5070 2023-04-05 11:42:27.308447 PyQt6-6.5.0/examples/quick/canvas/roundedrect/roundedrect.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.496675 PyQt6-6.5.0/examples/quick/canvas/smile/
+-rw-r--r--   0 phil       (501) staff       (20)     5063 2023-04-05 11:42:27.307806 PyQt6-6.5.0/examples/quick/canvas/smile/smile.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.495515 PyQt6-6.5.0/examples/quick/canvas/squircle/
+-rw-r--r--   0 phil       (501) staff       (20)      771 2023-04-05 11:42:27.423657 PyQt6-6.5.0/examples/quick/canvas/squircle/squircle.png
+-rw-r--r--   0 phil       (501) staff       (20)     5379 2023-04-05 11:42:27.308373 PyQt6-6.5.0/examples/quick/canvas/squircle/squircle.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.494295 PyQt6-6.5.0/examples/quick/canvas/tiger/
+-rw-r--r--   0 phil       (501) staff       (20)    93676 2023-04-05 11:42:27.312788 PyQt6-6.5.0/examples/quick/canvas/tiger/tiger.js
+-rw-r--r--   0 phil       (501) staff       (20)     4864 2023-04-05 11:42:27.310081 PyQt6-6.5.0/examples/quick/canvas/tiger/tiger.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.483855 PyQt6-6.5.0/examples/quick/models/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.483550 PyQt6-6.5.0/examples/quick/models/abstractitemmodel/
+-rw-r--r--   0 phil       (501) staff       (20)     4051 2023-04-05 11:42:27.312444 PyQt6-6.5.0/examples/quick/models/abstractitemmodel/abstractitemmodel.py
+-rw-r--r--   0 phil       (501) staff       (20)     2151 2023-04-05 11:42:27.313244 PyQt6-6.5.0/examples/quick/models/abstractitemmodel/view.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.482483 PyQt6-6.5.0/examples/quick/models/objectlistmodel/
+-rw-r--r--   0 phil       (501) staff       (20)     3630 2023-04-05 11:42:27.312957 PyQt6-6.5.0/examples/quick/models/objectlistmodel/objectlistmodel.py
+-rw-r--r--   0 phil       (501) staff       (20)     2784 2023-04-05 11:42:27.311805 PyQt6-6.5.0/examples/quick/models/objectlistmodel/view.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.484267 PyQt6-6.5.0/examples/quick/models/stringlistmodel/
+-rw-r--r--   0 phil       (501) staff       (20)     2607 2023-04-05 11:42:27.317743 PyQt6-6.5.0/examples/quick/models/stringlistmodel/stringlistmodel.py
+-rw-r--r--   0 phil       (501) staff       (20)     2772 2023-04-05 11:42:27.310349 PyQt6-6.5.0/examples/quick/models/stringlistmodel/view.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.504293 PyQt6-6.5.0/examples/quick/scenegraph/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.504764 PyQt6-6.5.0/examples/quick/scenegraph/customgeometry/
+-rw-r--r--   0 phil       (501) staff       (20)     5922 2023-04-05 11:42:27.310097 PyQt6-6.5.0/examples/quick/scenegraph/customgeometry/customgeometry.py
+-rw-r--r--   0 phil       (501) staff       (20)     2732 2023-04-05 11:42:27.309405 PyQt6-6.5.0/examples/quick/scenegraph/customgeometry/main.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.481130 PyQt6-6.5.0/examples/quick/shared/
+-rw-r--r--   0 phil       (501) staff       (20)     3291 2023-04-05 11:42:27.424227 PyQt6-6.5.0/examples/quick/shared/Button.qml
+-rw-r--r--   0 phil       (501) staff       (20)     5174 2023-04-05 11:42:27.310102 PyQt6-6.5.0/examples/quick/shared/LauncherList.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3287 2023-04-05 11:42:27.314367 PyQt6-6.5.0/examples/quick/shared/SimpleLauncherDelegate.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.481609 PyQt6-6.5.0/examples/quick/shared/images/
+-rw-r--r--   0 phil       (501) staff       (20)     1590 2023-04-05 11:42:27.312454 PyQt6-6.5.0/examples/quick/shared/images/back.png
+-rw-r--r--   0 phil       (501) staff       (20)     1371 2023-04-05 11:42:27.314176 PyQt6-6.5.0/examples/quick/shared/images/next.png
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.497178 PyQt6-6.5.0/examples/quick/tutorials/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.503397 PyQt6-6.5.0/examples/quick/tutorials/extending/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.503905 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter1-basics/
+-rw-r--r--   0 phil       (501) staff       (20)     2385 2023-04-05 11:42:27.314975 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter1-basics/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3492 2023-04-05 11:42:27.314849 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.497836 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter2-methods/
+-rw-r--r--   0 phil       (501) staff       (20)     2532 2023-04-05 11:42:27.314344 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter2-methods/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3538 2023-04-05 11:42:27.319227 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.498842 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter3-bindings/
+-rw-r--r--   0 phil       (501) staff       (20)     2650 2023-04-05 11:42:27.312487 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter3-bindings/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3625 2023-04-05 11:42:27.312706 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.500877 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter4-customPropertyTypes/
+-rw-r--r--   0 phil       (501) staff       (20)     2361 2023-04-05 11:42:27.312145 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     3724 2023-04-05 11:42:27.424899 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.499878 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter5-listproperties/
+-rw-r--r--   0 phil       (501) staff       (20)     2643 2023-04-05 11:42:27.312018 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter5-listproperties/app.qml
+-rw-r--r--   0 phil       (501) staff       (20)     4116 2023-04-05 11:42:27.316189 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.501764 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.503101 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/
+-rw-r--r--   0 phil       (501) staff       (20)     2292 2023-04-05 11:42:27.315236 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py
+-rw-r--r--   0 phil       (501) staff       (20)     2587 2023-04-05 11:42:27.315923 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py
+-rw-r--r--   0 phil       (501) staff       (20)     3132 2023-04-05 11:42:27.316456 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py
+-rw-r--r--   0 phil       (501) staff       (20)       36 2023-04-05 11:42:27.316184 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/qmldir
+-rw-r--r--   0 phil       (501) staff       (20)     2643 2023-04-05 11:42:27.315511 PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/app.qml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.527043 PyQt6-6.5.0/examples/richtext/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.527516 PyQt6-6.5.0/examples/richtext/textobject/
+-rw-r--r--   0 phil       (501) staff       (20)     3873 2023-04-05 11:42:27.320680 PyQt6-6.5.0/examples/richtext/textobject/heart.svg
+-rw-r--r--   0 phil       (501) staff       (20)     4491 2023-04-05 11:42:27.314879 PyQt6-6.5.0/examples/richtext/textobject/textobject.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.391743 PyQt6-6.5.0/lupdate/
+-rw-r--r--   0 phil       (501) staff       (20)      875 2023-04-05 12:16:47.640385 PyQt6-6.5.0/lupdate/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2479 2023-04-05 12:16:47.641466 PyQt6-6.5.0/lupdate/designer_source.py
+-rw-r--r--   0 phil       (501) staff       (20)     3416 2023-04-05 12:16:47.644309 PyQt6-6.5.0/lupdate/lupdate.py
+-rw-r--r--   0 phil       (501) staff       (20)     3062 2023-04-05 12:16:47.636978 PyQt6-6.5.0/lupdate/pylupdate.py
+-rw-r--r--   0 phil       (501) staff       (20)    11176 2023-04-05 12:16:47.643508 PyQt6-6.5.0/lupdate/python_source.py
+-rw-r--r--   0 phil       (501) staff       (20)     1114 2023-04-05 12:16:47.640900 PyQt6-6.5.0/lupdate/source_file.py
+-rw-r--r--   0 phil       (501) staff       (20)    14976 2023-04-05 12:16:47.639359 PyQt6-6.5.0/lupdate/translation_file.py
+-rw-r--r--   0 phil       (501) staff       (20)     1633 2023-04-05 12:16:47.639941 PyQt6-6.5.0/lupdate/translations.py
+-rw-r--r--   0 phil       (501) staff       (20)     1504 2023-04-05 12:16:47.636164 PyQt6-6.5.0/lupdate/user.py
+-rw-r--r--   0 phil       (501) staff       (20)    28670 2023-04-05 12:16:47.685877 PyQt6-6.5.0/project.py
+-rw-r--r--   0 phil       (501) staff       (20)      546 2023-04-05 12:16:47.686265 PyQt6-6.5.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.787732 PyQt6-6.5.0/qmlscene/
+-rw-r--r--   0 phil       (501) staff       (20)     9302 2023-04-05 12:16:47.680770 PyQt6-6.5.0/qmlscene/pluginloader.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1670 2023-04-05 12:16:47.681499 PyQt6-6.5.0/qmlscene/pluginloader.h
+-rw-r--r--   0 phil       (501) staff       (20)      451 2023-04-05 12:16:47.679069 PyQt6-6.5.0/qmlscene/qmlscene.pro-in
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.434771 PyQt6-6.5.0/qpy/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.454146 PyQt6-6.5.0/qpy/QtCore/
+-rw-r--r--   0 phil       (501) staff       (20)     3878 2023-04-05 12:16:47.538939 PyQt6-6.5.0/qpy/QtCore/qpycore_api.h
+-rw-r--r--   0 phil       (501) staff       (20)    49695 2023-04-05 12:16:47.493384 PyQt6-6.5.0/qpy/QtCore/qpycore_chimera.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9586 2023-04-05 12:16:47.507003 PyQt6-6.5.0/qpy/QtCore/qpycore_chimera.h
+-rw-r--r--   0 phil       (501) staff       (20)     2557 2023-04-05 12:16:47.526595 PyQt6-6.5.0/qpy/QtCore/qpycore_chimera_signature.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3515 2023-04-05 12:16:47.524513 PyQt6-6.5.0/qpy/QtCore/qpycore_chimera_storage.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3077 2023-04-05 12:16:47.527656 PyQt6-6.5.0/qpy/QtCore/qpycore_classinfo.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1089 2023-04-05 12:16:47.453311 PyQt6-6.5.0/qpy/QtCore/qpycore_classinfo.h
+-rw-r--r--   0 phil       (501) staff       (20)     4385 2023-04-05 12:16:47.484361 PyQt6-6.5.0/qpy/QtCore/qpycore_decorators.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5930 2023-04-05 12:16:47.479182 PyQt6-6.5.0/qpy/QtCore/qpycore_enums_flags.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-04-05 12:16:47.525980 PyQt6-6.5.0/qpy/QtCore/qpycore_enums_flags.h
+-rw-r--r--   0 phil       (501) staff       (20)     4006 2023-04-05 12:16:47.458804 PyQt6-6.5.0/qpy/QtCore/qpycore_event_handlers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1376 2023-04-05 12:16:47.528794 PyQt6-6.5.0/qpy/QtCore/qpycore_event_handlers.h
+-rw-r--r--   0 phil       (501) staff       (20)     3908 2023-04-05 12:16:47.480468 PyQt6-6.5.0/qpy/QtCore/qpycore_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1815 2023-04-05 12:16:47.508108 PyQt6-6.5.0/qpy/QtCore/qpycore_misc.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1136 2023-04-05 12:16:47.466443 PyQt6-6.5.0/qpy/QtCore/qpycore_misc.h
+-rw-r--r--   0 phil       (501) staff       (20)     1136 2023-04-05 12:16:47.482308 PyQt6-6.5.0/qpy/QtCore/qpycore_namespace.h
+-rw-r--r--   0 phil       (501) staff       (20)     1183 2023-04-05 12:16:47.511883 PyQt6-6.5.0/qpy/QtCore/qpycore_objectified_strings.h
+-rw-r--r--   0 phil       (501) staff       (20)     4375 2023-04-05 12:16:47.460467 PyQt6-6.5.0/qpy/QtCore/qpycore_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12835 2023-04-05 12:16:47.532241 PyQt6-6.5.0/qpy/QtCore/qpycore_public_api.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4908 2023-04-05 12:16:47.529407 PyQt6-6.5.0/qpy/QtCore/qpycore_public_api.h
+-rw-r--r--   0 phil       (501) staff       (20)    29552 2023-04-05 12:16:47.518521 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtboundsignal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2023 2023-04-05 12:16:47.533524 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtboundsignal.h
+-rw-r--r--   0 phil       (501) staff       (20)     6090 2023-04-05 12:16:47.519750 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtconfigure.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7424 2023-04-05 12:16:47.514640 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmethodproxy.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1769 2023-04-05 12:16:47.483471 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmethodproxy.h
+-rw-r--r--   0 phil       (501) staff       (20)     2072 2023-04-05 12:16:47.525598 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmutexlocker.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1438 2023-04-05 12:16:47.503532 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmutexlocker.h
+-rw-r--r--   0 phil       (501) staff       (20)    15571 2023-04-05 12:16:47.477022 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtproperty.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2076 2023-04-05 12:16:47.477742 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtproperty.h
+-rw-r--r--   0 phil       (501) staff       (20)     4765 2023-04-05 12:16:47.509799 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtpyobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1742 2023-04-05 12:16:47.482929 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtpyobject.h
+-rw-r--r--   0 phil       (501) staff       (20)    20440 2023-04-05 12:16:47.457524 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtsignal.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2537 2023-04-05 12:16:47.508714 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtsignal.h
+-rw-r--r--   0 phil       (501) staff       (20)     9102 2023-04-05 12:16:47.495567 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslot.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2284 2023-04-05 12:16:47.530003 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslot.h
+-rw-r--r--   0 phil       (501) staff       (20)    10864 2023-04-05 12:16:47.521935 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslotproxy.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3552 2023-04-05 12:16:47.512545 PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslotproxy.h
+-rw-r--r--   0 phil       (501) staff       (20)     4375 2023-04-05 12:16:47.533062 PyQt6-6.5.0/qpy/QtCore/qpycore_qjsonvalue.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3016 2023-04-05 12:16:47.528228 PyQt6-6.5.0/qpy/QtCore/qpycore_qmessagelogger.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4296 2023-04-05 12:16:47.504332 PyQt6-6.5.0/qpy/QtCore/qpycore_qmetaobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     4569 2023-04-05 12:16:47.523761 PyQt6-6.5.0/qpy/QtCore/qpycore_qmetaobject_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3505 2023-04-05 12:16:47.505390 PyQt6-6.5.0/qpy/QtCore/qpycore_qmetaobjectbuilder.h
+-rw-r--r--   0 phil       (501) staff       (20)     4273 2023-04-05 12:16:47.513198 PyQt6-6.5.0/qpy/QtCore/qpycore_qobject_getattr.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     8681 2023-04-05 12:16:47.511505 PyQt6-6.5.0/qpy/QtCore/qpycore_qobject_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1408 2023-04-05 12:16:47.533963 PyQt6-6.5.0/qpy/QtCore/qpycore_qobject_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     4181 2023-04-05 12:16:47.496687 PyQt6-6.5.0/qpy/QtCore/qpycore_qstring.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3178 2023-04-05 12:16:47.468896 PyQt6-6.5.0/qpy/QtCore/qpycore_qt_conf.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2535 2023-04-05 12:16:47.525003 PyQt6-6.5.0/qpy/QtCore/qpycore_qvariant.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     6459 2023-04-05 12:16:47.481790 PyQt6-6.5.0/qpy/QtCore/qpycore_qvariant_value.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    17334 2023-04-05 12:16:47.472634 PyQt6-6.5.0/qpy/QtCore/qpycore_types.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1576 2023-04-05 12:16:47.473558 PyQt6-6.5.0/qpy/QtCore/qpycore_types.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.431917 PyQt6-6.5.0/qpy/QtDBus/
+-rw-r--r--   0 phil       (501) staff       (20)      999 2023-04-05 12:16:47.542498 PyQt6-6.5.0/qpy/QtDBus/qpydbus_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     5739 2023-04-05 12:16:47.546250 PyQt6-6.5.0/qpy/QtDBus/qpydbus_chimera_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1236 2023-04-05 12:16:47.545007 PyQt6-6.5.0/qpy/QtDBus/qpydbus_chimera_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     1471 2023-04-05 12:16:47.541689 PyQt6-6.5.0/qpy/QtDBus/qpydbus_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1865 2023-04-05 12:16:47.542151 PyQt6-6.5.0/qpy/QtDBus/qpydbuspendingreply.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1340 2023-04-05 12:16:47.544661 PyQt6-6.5.0/qpy/QtDBus/qpydbuspendingreply.h
+-rw-r--r--   0 phil       (501) staff       (20)     3583 2023-04-05 12:16:47.544166 PyQt6-6.5.0/qpy/QtDBus/qpydbusreply.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1788 2023-04-05 12:16:47.541263 PyQt6-6.5.0/qpy/QtDBus/qpydbusreply.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.421697 PyQt6-6.5.0/qpy/QtDesigner/
+-rw-r--r--   0 phil       (501) staff       (20)     1410 2023-04-05 12:16:47.548434 PyQt6-6.5.0/qpy/QtDesigner/qpydesignercontainerextension.h
+-rw-r--r--   0 phil       (501) staff       (20)     1492 2023-04-05 12:16:47.550557 PyQt6-6.5.0/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h
+-rw-r--r--   0 phil       (501) staff       (20)     1402 2023-04-05 12:16:47.549877 PyQt6-6.5.0/qpy/QtDesigner/qpydesignercustomwidgetplugin.h
+-rw-r--r--   0 phil       (501) staff       (20)     1430 2023-04-05 12:16:47.547533 PyQt6-6.5.0/qpy/QtDesigner/qpydesignermembersheetextension.h
+-rw-r--r--   0 phil       (501) staff       (20)     1450 2023-04-05 12:16:47.549220 PyQt6-6.5.0/qpy/QtDesigner/qpydesignerpropertysheetextension.h
+-rw-r--r--   0 phil       (501) staff       (20)     1400 2023-04-05 12:16:47.551279 PyQt6-6.5.0/qpy/QtDesigner/qpydesignertaskmenuextension.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.412116 PyQt6-6.5.0/qpy/QtOpenGL/
+-rw-r--r--   0 phil       (501) staff       (20)   209932 2023-04-05 12:16:47.589600 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_add_constants.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2585 2023-04-05 12:16:47.596000 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     4002 2023-04-05 12:16:47.594446 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_array_convertors.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7165 2023-04-05 12:16:47.591923 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_attribute_array.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5002 2023-04-05 12:16:47.595524 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_data_cache.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2413 2023-04-05 12:16:47.561689 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_data_cache.h
+-rw-r--r--   0 phil       (501) staff       (20)     4686 2023-04-05 12:16:47.590743 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_get.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1228 2023-04-05 12:16:47.596411 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-04-05 12:16:47.562072 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_misc.h
+-rw-r--r--   0 phil       (501) staff       (20)    12637 2023-04-05 12:16:47.564048 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9947 2023-04-05 12:16:47.566098 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_value_array.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3103 2023-04-05 12:16:47.592520 PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_version_functions.cpp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.418902 PyQt6-6.5.0/qpy/QtQml/
+-rw-r--r--   0 phil       (501) staff       (20)     2279 2023-04-05 12:16:47.607855 PyQt6-6.5.0/qpy/QtQml/qpyqml_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     1799 2023-04-05 12:16:47.612600 PyQt6-6.5.0/qpy/QtQml/qpyqml_listdata.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1431 2023-04-05 12:16:47.617458 PyQt6-6.5.0/qpy/QtQml/qpyqml_listdata.h
+-rw-r--r--   0 phil       (501) staff       (20)     2595 2023-04-05 12:16:47.613559 PyQt6-6.5.0/qpy/QtQml/qpyqml_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3089 2023-04-05 12:16:47.612045 PyQt6-6.5.0/qpy/QtQml/qpyqml_qjsvalue.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     5283 2023-04-05 12:16:47.604385 PyQt6-6.5.0/qpy/QtQml/qpyqml_register_singleton_type.cpp
+-rw-r--r--   0 phil       (501) staff       (20)    12648 2023-04-05 12:16:47.615375 PyQt6-6.5.0/qpy/QtQml/qpyqml_register_type.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     9495 2023-04-05 12:16:47.617019 PyQt6-6.5.0/qpy/QtQml/qpyqmllistproperty.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1118 2023-04-05 12:16:47.611393 PyQt6-6.5.0/qpy/QtQml/qpyqmllistproperty.h
+-rw-r--r--   0 phil       (501) staff       (20)     6171 2023-04-05 12:16:47.609645 PyQt6-6.5.0/qpy/QtQml/qpyqmllistpropertywrapper.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1884 2023-04-05 12:16:47.608449 PyQt6-6.5.0/qpy/QtQml/qpyqmllistpropertywrapper.h
+-rw-r--r--   0 phil       (501) staff       (20)    17618 2023-04-05 12:16:47.607310 PyQt6-6.5.0/qpy/QtQml/qpyqmlobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     7477 2023-04-05 12:16:47.599879 PyQt6-6.5.0/qpy/QtQml/qpyqmlobject.h
+-rw-r--r--   0 phil       (501) staff       (20)     3201 2023-04-05 12:16:47.610231 PyQt6-6.5.0/qpy/QtQml/qpyqmlsingletonobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3097 2023-04-05 12:16:47.600627 PyQt6-6.5.0/qpy/QtQml/qpyqmlsingletonobject.h
+-rw-r--r--   0 phil       (501) staff       (20)    10140 2023-04-05 12:16:47.603402 PyQt6-6.5.0/qpy/QtQml/qpyqmlvalidator.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3440 2023-04-05 12:16:47.601658 PyQt6-6.5.0/qpy/QtQml/qpyqmlvalidator.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.428084 PyQt6-6.5.0/qpy/QtQuick/
+-rw-r--r--   0 phil       (501) staff       (20)     1136 2023-04-05 12:16:47.621564 PyQt6-6.5.0/qpy/QtQuick/qpyquick_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     4162 2023-04-05 12:16:47.622846 PyQt6-6.5.0/qpy/QtQuick/qpyquick_chimera_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1601 2023-04-05 12:16:47.619853 PyQt6-6.5.0/qpy/QtQuick/qpyquick_chimera_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     2528 2023-04-05 12:16:47.618255 PyQt6-6.5.0/qpy/QtQuick/qpyquick_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2490 2023-04-05 12:16:47.619442 PyQt6-6.5.0/qpy/QtQuick/qpyquick_register_type.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1297 2023-04-05 12:16:47.626820 PyQt6-6.5.0/qpy/QtQuick/qpyquick_register_type.h
+-rw-r--r--   0 phil       (501) staff       (20)     6763 2023-04-05 12:16:47.623882 PyQt6-6.5.0/qpy/QtQuick/qpyquickframebufferobject.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3136 2023-04-05 12:16:47.618995 PyQt6-6.5.0/qpy/QtQuick/qpyquickframebufferobject.h
+-rw-r--r--   0 phil       (501) staff       (20)     7803 2023-04-05 12:16:47.628000 PyQt6-6.5.0/qpy/QtQuick/qpyquickitem.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     3255 2023-04-05 12:16:47.628832 PyQt6-6.5.0/qpy/QtQuick/qpyquickitem.h
+-rw-r--r--   0 phil       (501) staff       (20)     6215 2023-04-05 12:16:47.621173 PyQt6-6.5.0/qpy/QtQuick/qpyquickpainteditem.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2873 2023-04-05 12:16:47.624683 PyQt6-6.5.0/qpy/QtQuick/qpyquickpainteditem.h
+-rw-r--r--   0 phil       (501) staff       (20)     5020 2023-04-05 12:16:47.625696 PyQt6-6.5.0/qpy/QtQuick/qpyquickview.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2326 2023-04-05 12:16:47.630489 PyQt6-6.5.0/qpy/QtQuick/qpyquickview.h
+-rw-r--r--   0 phil       (501) staff       (20)     5160 2023-04-05 12:16:47.629766 PyQt6-6.5.0/qpy/QtQuick/qpyquickwindow.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     2396 2023-04-05 12:16:47.626461 PyQt6-6.5.0/qpy/QtQuick/qpyquickwindow.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.434347 PyQt6-6.5.0/qpy/QtWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     1008 2023-04-05 12:16:47.631454 PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_api.h
+-rw-r--r--   0 phil       (501) staff       (20)     1805 2023-04-05 12:16:47.632284 PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1247 2023-04-05 12:16:47.633444 PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_chimera_helpers.h
+-rw-r--r--   0 phil       (501) staff       (20)     1703 2023-04-05 12:16:47.634563 PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_post_init.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1195 2023-04-05 12:16:47.631872 PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp
+-rw-r--r--   0 phil       (501) staff       (20)     1147 2023-04-05 12:16:47.633959 PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_qaction_helpers.h
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.786212 PyQt6-6.5.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.602625 PyQt6-6.5.0/sip/QAxContainer/
+-rw-r--r--   0 phil       (501) staff       (20)     1998 2023-04-05 12:16:54.955533 PyQt6-6.5.0/sip/QAxContainer/QAxContainermod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4938 2023-04-05 12:16:54.956373 PyQt6-6.5.0/sip/QAxContainer/qaxbase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2540 2023-04-05 12:16:54.958130 PyQt6-6.5.0/sip/QAxContainer/qaxobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1251 2023-04-05 12:16:54.956777 PyQt6-6.5.0/sip/QAxContainer/qaxobjectinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2350 2023-04-05 12:16:54.957321 PyQt6-6.5.0/sip/QAxContainer/qaxwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.564873 PyQt6-6.5.0/sip/QtBluetooth/
+-rw-r--r--   0 phil       (501) staff       (20)     2777 2023-04-05 12:16:54.851294 PyQt6-6.5.0/sip/QtBluetooth/QtBluetoothmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1559 2023-04-05 12:16:54.825622 PyQt6-6.5.0/sip/QtBluetooth/qbluetooth.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1673 2023-04-05 12:16:54.817445 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothaddress.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2670 2023-04-05 12:16:54.821661 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6598 2023-04-05 12:16:54.815329 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothdeviceinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1541 2023-04-05 12:16:54.853331 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothhostinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2570 2023-04-05 12:16:54.826235 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothlocaldevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3360 2023-04-05 12:16:54.852187 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2467 2023-04-05 12:16:54.819593 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3324 2023-04-05 12:16:54.854083 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothserviceinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5134 2023-04-05 12:16:54.816079 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9422 2023-04-05 12:16:54.824617 PyQt6-6.5.0/sip/QtBluetooth/qbluetoothuuid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2334 2023-04-05 12:16:54.814053 PyQt6-6.5.0/sip/QtBluetooth/qlowenergyadvertisingdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3006 2023-04-05 12:16:54.813453 PyQt6-6.5.0/sip/QtBluetooth/qlowenergyadvertisingparameters.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2262 2023-04-05 12:16:54.818052 PyQt6-6.5.0/sip/QtBluetooth/qlowenergycharacteristic.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2472 2023-04-05 12:16:54.825179 PyQt6-6.5.0/sip/QtBluetooth/qlowenergycharacteristicdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1843 2023-04-05 12:16:54.852734 PyQt6-6.5.0/sip/QtBluetooth/qlowenergyconnectionparameters.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4355 2023-04-05 12:16:54.816772 PyQt6-6.5.0/sip/QtBluetooth/qlowenergycontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1568 2023-04-05 12:16:54.822210 PyQt6-6.5.0/sip/QtBluetooth/qlowenergydescriptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2201 2023-04-05 12:16:54.823145 PyQt6-6.5.0/sip/QtBluetooth/qlowenergydescriptordata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3661 2023-04-05 12:16:54.820248 PyQt6-6.5.0/sip/QtBluetooth/qlowenergyservice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2201 2023-04-05 12:16:54.822686 PyQt6-6.5.0/sip/QtBluetooth/qlowenergyservicedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3358 2023-04-05 12:16:54.821089 PyQt6-6.5.0/sip/QtBluetooth/qpybluetooth_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4039 2023-04-05 12:16:54.819051 PyQt6-6.5.0/sip/QtBluetooth/qpybluetooth_qmultihash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2860 2023-04-05 12:16:54.812882 PyQt6-6.5.0/sip/QtBluetooth/qpybluetooth_quint128.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.782785 PyQt6-6.5.0/sip/QtCore/
+-rw-r--r--   0 phil       (501) staff       (20)     6295 2023-04-05 12:16:55.531872 PyQt6-6.5.0/sip/QtCore/QtCoremod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2557 2023-04-05 12:16:55.670798 PyQt6-6.5.0/sip/QtCore/qabstractanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2449 2023-04-05 12:16:55.621063 PyQt6-6.5.0/sip/QtCore/qabstracteventdispatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)    13972 2023-04-05 12:16:55.476475 PyQt6-6.5.0/sip/QtCore/qabstractitemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1335 2023-04-05 12:16:55.668952 PyQt6-6.5.0/sip/QtCore/qabstractnativeeventfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3493 2023-04-05 12:16:55.628173 PyQt6-6.5.0/sip/QtCore/qabstractproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1649 2023-04-05 12:16:55.507346 PyQt6-6.5.0/sip/QtCore/qanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2718 2023-04-05 12:16:55.464153 PyQt6-6.5.0/sip/QtCore/qanystringview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1338 2023-04-05 12:16:55.508279 PyQt6-6.5.0/sip/QtCore/qbasictimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2909 2023-04-05 12:16:55.625186 PyQt6-6.5.0/sip/QtCore/qbitarray.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3743 2023-04-05 12:16:55.469316 PyQt6-6.5.0/sip/QtCore/qbuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14436 2023-04-05 12:16:55.614941 PyQt6-6.5.0/sip/QtCore/qbytearray.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1144 2023-04-05 12:16:55.507797 PyQt6-6.5.0/sip/QtCore/qbytearrayalgorithms.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2976 2023-04-05 12:16:55.477456 PyQt6-6.5.0/sip/QtCore/qbytearraylist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1906 2023-04-05 12:16:55.654841 PyQt6-6.5.0/sip/QtCore/qbytearraymatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2692 2023-04-05 12:16:55.661821 PyQt6-6.5.0/sip/QtCore/qbytearrayview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3336 2023-04-05 12:16:55.465706 PyQt6-6.5.0/sip/QtCore/qcalendar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2452 2023-04-05 12:16:55.570465 PyQt6-6.5.0/sip/QtCore/qcborcommon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3894 2023-04-05 12:16:55.655936 PyQt6-6.5.0/sip/QtCore/qcborstreamreader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2475 2023-04-05 12:16:55.611677 PyQt6-6.5.0/sip/QtCore/qcborstreamwriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1591 2023-04-05 12:16:55.536806 PyQt6-6.5.0/sip/QtCore/qchar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2161 2023-04-05 12:16:55.506192 PyQt6-6.5.0/sip/QtCore/qcollator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2203 2023-04-05 12:16:55.615585 PyQt6-6.5.0/sip/QtCore/qcommandlineoption.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2825 2023-04-05 12:16:55.625868 PyQt6-6.5.0/sip/QtCore/qcommandlineparser.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4086 2023-04-05 12:16:55.624491 PyQt6-6.5.0/sip/QtCore/qconcatenatetablesproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10878 2023-04-05 12:16:55.515679 PyQt6-6.5.0/sip/QtCore/qcoreapplication.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6998 2023-04-05 12:16:55.525347 PyQt6-6.5.0/sip/QtCore/qcoreevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2546 2023-04-05 12:16:55.523249 PyQt6-6.5.0/sip/QtCore/qcryptographichash.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11005 2023-04-05 12:16:55.530588 PyQt6-6.5.0/sip/QtCore/qdatastream.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15385 2023-04-05 12:16:55.606427 PyQt6-6.5.0/sip/QtCore/qdatetime.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2791 2023-04-05 12:16:55.610696 PyQt6-6.5.0/sip/QtCore/qdeadlinetimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6571 2023-04-05 12:16:55.534085 PyQt6-6.5.0/sip/QtCore/qdir.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2019 2023-04-05 12:16:55.467946 PyQt6-6.5.0/sip/QtCore/qdiriterator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6671 2023-04-05 12:16:55.474241 PyQt6-6.5.0/sip/QtCore/qeasingcurve.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1833 2023-04-05 12:16:55.528016 PyQt6-6.5.0/sip/QtCore/qelapsedtimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2197 2023-04-05 12:16:55.623256 PyQt6-6.5.0/sip/QtCore/qeventloop.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3031 2023-04-05 12:16:55.658736 PyQt6-6.5.0/sip/QtCore/qfile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6316 2023-04-05 12:16:55.609999 PyQt6-6.5.0/sip/QtCore/qfiledevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3371 2023-04-05 12:16:55.535676 PyQt6-6.5.0/sip/QtCore/qfileinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1365 2023-04-05 12:16:55.585421 PyQt6-6.5.0/sip/QtCore/qfileselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1597 2023-04-05 12:16:55.585968 PyQt6-6.5.0/sip/QtCore/qfilesystemwatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-04-05 12:16:55.469859 PyQt6-6.5.0/sip/QtCore/qflags.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5036 2023-04-05 12:16:55.607793 PyQt6-6.5.0/sip/QtCore/qglobal.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3095 2023-04-05 12:16:55.664555 PyQt6-6.5.0/sip/QtCore/qidentityproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12510 2023-04-05 12:16:55.569425 PyQt6-6.5.0/sip/QtCore/qiodevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1380 2023-04-05 12:16:55.617641 PyQt6-6.5.0/sip/QtCore/qiodevicebase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8829 2023-04-05 12:16:55.663993 PyQt6-6.5.0/sip/QtCore/qitemselectionmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3263 2023-04-05 12:16:55.612646 PyQt6-6.5.0/sip/QtCore/qjsonarray.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2862 2023-04-05 12:16:55.565038 PyQt6-6.5.0/sip/QtCore/qjsondocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3500 2023-04-05 12:16:55.481223 PyQt6-6.5.0/sip/QtCore/qjsonobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2892 2023-04-05 12:16:55.589520 PyQt6-6.5.0/sip/QtCore/qjsonvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2418 2023-04-05 12:16:55.563578 PyQt6-6.5.0/sip/QtCore/qlibrary.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1661 2023-04-05 12:16:55.567162 PyQt6-6.5.0/sip/QtCore/qlibraryinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5198 2023-04-05 12:16:55.566413 PyQt6-6.5.0/sip/QtCore/qline.sip
+-rw-r--r--   0 phil       (501) staff       (20)    28155 2023-04-05 12:16:55.522355 PyQt6-6.5.0/sip/QtCore/qlocale.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1671 2023-04-05 12:16:55.477908 PyQt6-6.5.0/sip/QtCore/qlockfile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6581 2023-04-05 12:16:55.622563 PyQt6-6.5.0/sip/QtCore/qlogging.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1612 2023-04-05 12:16:55.471386 PyQt6-6.5.0/sip/QtCore/qloggingcategory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4347 2023-04-05 12:16:55.534918 PyQt6-6.5.0/sip/QtCore/qmargins.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1862 2023-04-05 12:16:55.656871 PyQt6-6.5.0/sip/QtCore/qmessageauthenticationcode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9269 2023-04-05 12:16:55.603943 PyQt6-6.5.0/sip/QtCore/qmetaobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4273 2023-04-05 12:16:55.516831 PyQt6-6.5.0/sip/QtCore/qmetatype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1954 2023-04-05 12:16:55.467385 PyQt6-6.5.0/sip/QtCore/qmimedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2082 2023-04-05 12:16:55.601791 PyQt6-6.5.0/sip/QtCore/qmimedatabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1812 2023-04-05 12:16:55.584373 PyQt6-6.5.0/sip/QtCore/qmimetype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1527 2023-04-05 12:16:55.466274 PyQt6-6.5.0/sip/QtCore/qmutex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1961 2023-04-05 12:16:55.672064 PyQt6-6.5.0/sip/QtCore/qmutexlocker.sip
+-rw-r--r--   0 phil       (501) staff       (20)    34139 2023-04-05 12:16:55.559121 PyQt6-6.5.0/sip/QtCore/qnamespace.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1410 2023-04-05 12:16:55.584926 PyQt6-6.5.0/sip/QtCore/qnumeric.sip
+-rw-r--r--   0 phil       (501) staff       (20)    20046 2023-04-05 12:16:55.480389 PyQt6-6.5.0/sip/QtCore/qobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1248 2023-04-05 12:16:55.620451 PyQt6-6.5.0/sip/QtCore/qobjectcleanuphandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8135 2023-04-05 12:16:55.618803 PyQt6-6.5.0/sip/QtCore/qobjectdefs.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7658 2023-04-05 12:16:55.502207 PyQt6-6.5.0/sip/QtCore/qoperatingsystemversion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1502 2023-04-05 12:16:55.510610 PyQt6-6.5.0/sip/QtCore/qparallelanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1373 2023-04-05 12:16:55.602381 PyQt6-6.5.0/sip/QtCore/qpauseanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1555 2023-04-05 12:16:55.466780 PyQt6-6.5.0/sip/QtCore/qpluginloader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4684 2023-04-05 12:16:55.616559 PyQt6-6.5.0/sip/QtCore/qpoint.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7887 2023-04-05 12:16:55.653698 PyQt6-6.5.0/sip/QtCore/qprocess.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1695 2023-04-05 12:16:55.583735 PyQt6-6.5.0/sip/QtCore/qpropertyanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11135 2023-04-05 12:16:55.667497 PyQt6-6.5.0/sip/QtCore/qpycore_qhash.sip
+-rw-r--r--   0 phil       (501) staff       (20)    30380 2023-04-05 12:16:55.578110 PyQt6-6.5.0/sip/QtCore/qpycore_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10053 2023-04-05 12:16:55.661010 PyQt6-6.5.0/sip/QtCore/qpycore_qmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5229 2023-04-05 12:16:55.509852 PyQt6-6.5.0/sip/QtCore/qpycore_qset.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11619 2023-04-05 12:16:55.505544 PyQt6-6.5.0/sip/QtCore/qpycore_std_pair.sip
+-rw-r--r--   0 phil       (501) staff       (20)      976 2023-04-05 12:16:55.623766 PyQt6-6.5.0/sip/QtCore/qpycore_virtual_error_handler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1863 2023-04-05 12:16:55.511220 PyQt6-6.5.0/sip/QtCore/qrandom.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2706 2023-04-05 12:16:55.608694 PyQt6-6.5.0/sip/QtCore/qreadwritelock.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9654 2023-04-05 12:16:55.652256 PyQt6-6.5.0/sip/QtCore/qrect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7257 2023-04-05 12:16:55.670102 PyQt6-6.5.0/sip/QtCore/qregularexpression.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2661 2023-04-05 12:16:55.526015 PyQt6-6.5.0/sip/QtCore/qresource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1718 2023-04-05 12:16:55.564184 PyQt6-6.5.0/sip/QtCore/qrunnable.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2390 2023-04-05 12:16:55.662470 PyQt6-6.5.0/sip/QtCore/qsavefile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1620 2023-04-05 12:16:55.619972 PyQt6-6.5.0/sip/QtCore/qsemaphore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1721 2023-04-05 12:16:55.654244 PyQt6-6.5.0/sip/QtCore/qsequentialanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5109 2023-04-05 12:16:55.580378 PyQt6-6.5.0/sip/QtCore/qsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2332 2023-04-05 12:16:55.561859 PyQt6-6.5.0/sip/QtCore/qsharedmemory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1641 2023-04-05 12:16:55.617098 PyQt6-6.5.0/sip/QtCore/qsignalmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5173 2023-04-05 12:16:55.579303 PyQt6-6.5.0/sip/QtCore/qsize.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1673 2023-04-05 12:16:55.470389 PyQt6-6.5.0/sip/QtCore/qsocketnotifier.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5908 2023-04-05 12:16:55.562901 PyQt6-6.5.0/sip/QtCore/qsortfilterproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2598 2023-04-05 12:16:55.506852 PyQt6-6.5.0/sip/QtCore/qstandardpaths.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1966 2023-04-05 12:16:55.527436 PyQt6-6.5.0/sip/QtCore/qstorageinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1485 2023-04-05 12:16:55.472841 PyQt6-6.5.0/sip/QtCore/qstring.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3205 2023-04-05 12:16:55.503060 PyQt6-6.5.0/sip/QtCore/qstringconverter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2134 2023-04-05 12:16:55.627521 PyQt6-6.5.0/sip/QtCore/qstringconverter_base.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2937 2023-04-05 12:16:55.588807 PyQt6-6.5.0/sip/QtCore/qstringlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2403 2023-04-05 12:16:55.560634 PyQt6-6.5.0/sip/QtCore/qstringlistmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1537 2023-04-05 12:16:55.513774 PyQt6-6.5.0/sip/QtCore/qstringview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1572 2023-04-05 12:16:55.470893 PyQt6-6.5.0/sip/QtCore/qsysinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1790 2023-04-05 12:16:55.523825 PyQt6-6.5.0/sip/QtCore/qsystemsemaphore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1463 2023-04-05 12:16:55.571036 PyQt6-6.5.0/sip/QtCore/qtemporarydir.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1798 2023-04-05 12:16:55.474694 PyQt6-6.5.0/sip/QtCore/qtemporaryfile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1455 2023-04-05 12:16:55.551231 PyQt6-6.5.0/sip/QtCore/qtenvironmentvariables.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1998 2023-04-05 12:16:55.619412 PyQt6-6.5.0/sip/QtCore/qtextboundaryfinder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5603 2023-04-05 12:16:55.658045 PyQt6-6.5.0/sip/QtCore/qtextstream.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2691 2023-04-05 12:16:55.537471 PyQt6-6.5.0/sip/QtCore/qthread.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4994 2023-04-05 12:16:55.512455 PyQt6-6.5.0/sip/QtCore/qthreadpool.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2431 2023-04-05 12:16:55.464955 PyQt6-6.5.0/sip/QtCore/qtimeline.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2585 2023-04-05 12:16:55.513181 PyQt6-6.5.0/sip/QtCore/qtimer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5446 2023-04-05 12:16:55.472316 PyQt6-6.5.0/sip/QtCore/qtimezone.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1837 2023-04-05 12:16:55.561174 PyQt6-6.5.0/sip/QtCore/qtranslator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2945 2023-04-05 12:16:55.536222 PyQt6-6.5.0/sip/QtCore/qtransposeproxymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1057 2023-04-05 12:16:55.601147 PyQt6-6.5.0/sip/QtCore/qtversion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1843 2023-04-05 12:16:55.468565 PyQt6-6.5.0/sip/QtCore/qtypes.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7344 2023-04-05 12:16:55.587134 PyQt6-6.5.0/sip/QtCore/qurl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2784 2023-04-05 12:16:55.526668 PyQt6-6.5.0/sip/QtCore/qurlquery.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3479 2023-04-05 12:16:55.668434 PyQt6-6.5.0/sip/QtCore/quuid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3169 2023-04-05 12:16:55.532866 PyQt6-6.5.0/sip/QtCore/qvariant.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2197 2023-04-05 12:16:55.671380 PyQt6-6.5.0/sip/QtCore/qvariantanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3856 2023-04-05 12:16:55.626764 PyQt6-6.5.0/sip/QtCore/qversionnumber.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1578 2023-04-05 12:16:55.559872 PyQt6-6.5.0/sip/QtCore/qwaitcondition.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1577 2023-04-05 12:16:55.587767 PyQt6-6.5.0/sip/QtCore/qwineventnotifier.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15570 2023-04-05 12:16:55.583067 PyQt6-6.5.0/sip/QtCore/qxmlstream.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.673509 PyQt6-6.5.0/sip/QtDBus/
+-rw-r--r--   0 phil       (501) staff       (20)     2340 2023-04-05 12:16:55.214459 PyQt6-6.5.0/sip/QtDBus/QtDBusmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1271 2023-04-05 12:16:55.208916 PyQt6-6.5.0/sip/QtDBus/qdbusabstractadaptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7394 2023-04-05 12:16:55.212754 PyQt6-6.5.0/sip/QtDBus/qdbusabstractinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4871 2023-04-05 12:16:55.209881 PyQt6-6.5.0/sip/QtDBus/qdbusargument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9428 2023-04-05 12:16:55.207206 PyQt6-6.5.0/sip/QtDBus/qdbusconnection.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2976 2023-04-05 12:16:55.210984 PyQt6-6.5.0/sip/QtDBus/qdbusconnectioninterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1933 2023-04-05 12:16:55.213956 PyQt6-6.5.0/sip/QtDBus/qdbuserror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2507 2023-04-05 12:16:55.207868 PyQt6-6.5.0/sip/QtDBus/qdbusextratypes.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1299 2023-04-05 12:16:55.211450 PyQt6-6.5.0/sip/QtDBus/qdbusinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3015 2023-04-05 12:16:55.208460 PyQt6-6.5.0/sip/QtDBus/qdbusmessage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1745 2023-04-05 12:16:55.210400 PyQt6-6.5.0/sip/QtDBus/qdbuspendingcall.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2225 2023-04-05 12:16:55.213344 PyQt6-6.5.0/sip/QtDBus/qdbusservicewatcher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1450 2023-04-05 12:16:55.204749 PyQt6-6.5.0/sip/QtDBus/qdbusunixfiledescriptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1739 2023-04-05 12:16:55.205471 PyQt6-6.5.0/sip/QtDBus/qpydbuspendingreply.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5291 2023-04-05 12:16:55.204215 PyQt6-6.5.0/sip/QtDBus/qpydbusreply.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.593064 PyQt6-6.5.0/sip/QtDesigner/
+-rw-r--r--   0 phil       (501) staff       (20)     2809 2023-04-05 12:16:54.918248 PyQt6-6.5.0/sip/QtDesigner/QtDesignermod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1493 2023-04-05 12:16:54.910126 PyQt6-6.5.0/sip/QtDesigner/abstractactioneditor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-04-05 12:16:54.919056 PyQt6-6.5.0/sip/QtDesigner/abstractformbuilder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2021 2023-04-05 12:16:54.916439 PyQt6-6.5.0/sip/QtDesigner/abstractformeditor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4737 2023-04-05 12:16:54.910784 PyQt6-6.5.0/sip/QtDesigner/abstractformwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2532 2023-04-05 12:16:54.914655 PyQt6-6.5.0/sip/QtDesigner/abstractformwindowcursor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3286 2023-04-05 12:16:54.907841 PyQt6-6.5.0/sip/QtDesigner/abstractformwindowmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1402 2023-04-05 12:16:54.917307 PyQt6-6.5.0/sip/QtDesigner/abstractobjectinspector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1736 2023-04-05 12:16:54.917769 PyQt6-6.5.0/sip/QtDesigner/abstractpropertyeditor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1397 2023-04-05 12:16:54.915464 PyQt6-6.5.0/sip/QtDesigner/abstractwidgetbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1633 2023-04-05 12:16:54.916021 PyQt6-6.5.0/sip/QtDesigner/container.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1884 2023-04-05 12:16:54.913479 PyQt6-6.5.0/sip/QtDesigner/customwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1438 2023-04-05 12:16:54.916834 PyQt6-6.5.0/sip/QtDesigner/default_extensionfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1571 2023-04-05 12:16:54.914137 PyQt6-6.5.0/sip/QtDesigner/extension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2023-04-05 12:16:54.911688 PyQt6-6.5.0/sip/QtDesigner/formbuilder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1993 2023-04-05 12:16:54.912667 PyQt6-6.5.0/sip/QtDesigner/membersheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2084 2023-04-05 12:16:54.909175 PyQt6-6.5.0/sip/QtDesigner/propertysheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3397 2023-04-05 12:16:54.909734 PyQt6-6.5.0/sip/QtDesigner/qextensionmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1228 2023-04-05 12:16:54.907209 PyQt6-6.5.0/sip/QtDesigner/qpydesignercontainerextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1308 2023-04-05 12:16:54.908715 PyQt6-6.5.0/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1235 2023-04-05 12:16:54.911317 PyQt6-6.5.0/sip/QtDesigner/qpydesignercustomwidgetplugin.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1242 2023-04-05 12:16:54.918665 PyQt6-6.5.0/sip/QtDesigner/qpydesignermembersheetextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1259 2023-04-05 12:16:54.915082 PyQt6-6.5.0/sip/QtDesigner/qpydesignerpropertysheetextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1221 2023-04-05 12:16:54.912132 PyQt6-6.5.0/sip/QtDesigner/qpydesignertaskmenuextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1300 2023-04-05 12:16:54.908256 PyQt6-6.5.0/sip/QtDesigner/taskmenu.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.652947 PyQt6-6.5.0/sip/QtGui/
+-rw-r--r--   0 phil       (501) staff       (20)     4178 2023-04-05 12:16:55.117387 PyQt6-6.5.0/sip/QtGui/QtGuimod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1404 2023-04-05 12:16:55.114328 PyQt6-6.5.0/sip/QtGui/opengl_types.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2023-04-05 12:16:55.020486 PyQt6-6.5.0/sip/QtGui/qabstractfileiconprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3726 2023-04-05 12:16:55.017215 PyQt6-6.5.0/sip/QtGui/qabstracttextdocumentlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4672 2023-04-05 12:16:55.079569 PyQt6-6.5.0/sip/QtGui/qaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1946 2023-04-05 12:16:55.021892 PyQt6-6.5.0/sip/QtGui/qactiongroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1568 2023-04-05 12:16:55.120810 PyQt6-6.5.0/sip/QtGui/qbackingstore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1848 2023-04-05 12:16:55.052499 PyQt6-6.5.0/sip/QtGui/qbitmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10739 2023-04-05 12:16:55.133695 PyQt6-6.5.0/sip/QtGui/qbrush.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3492 2023-04-05 12:16:55.134319 PyQt6-6.5.0/sip/QtGui/qclipboard.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12351 2023-04-05 12:16:55.069671 PyQt6-6.5.0/sip/QtGui/qcolor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4476 2023-04-05 12:16:55.025406 PyQt6-6.5.0/sip/QtGui/qcolorspace.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1554 2023-04-05 12:16:55.058475 PyQt6-6.5.0/sip/QtGui/qcolortransform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3042 2023-04-05 12:16:55.083047 PyQt6-6.5.0/sip/QtGui/qcursor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2418 2023-04-05 12:16:55.122637 PyQt6-6.5.0/sip/QtGui/qdesktopservices.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1971 2023-04-05 12:16:55.129665 PyQt6-6.5.0/sip/QtGui/qdrag.sip
+-rw-r--r--   0 phil       (501) staff       (20)    23127 2023-04-05 12:16:55.127050 PyQt6-6.5.0/sip/QtGui/qevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2495 2023-04-05 12:16:55.109600 PyQt6-6.5.0/sip/QtGui/qeventpoint.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4840 2023-04-05 12:16:55.062748 PyQt6-6.5.0/sip/QtGui/qfilesystemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5846 2023-04-05 12:16:55.023881 PyQt6-6.5.0/sip/QtGui/qfont.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3645 2023-04-05 12:16:55.024608 PyQt6-6.5.0/sip/QtGui/qfontdatabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1495 2023-04-05 12:16:55.028895 PyQt6-6.5.0/sip/QtGui/qfontinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6681 2023-04-05 12:16:55.063881 PyQt6-6.5.0/sip/QtGui/qfontmetrics.sip
+-rw-r--r--   0 phil       (501) staff       (20)    25528 2023-04-05 12:16:55.104807 PyQt6-6.5.0/sip/QtGui/qgenericmatrix.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2611 2023-04-05 12:16:55.110335 PyQt6-6.5.0/sip/QtGui/qglyphrun.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9603 2023-04-05 12:16:55.131078 PyQt6-6.5.0/sip/QtGui/qguiapplication.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4245 2023-04-05 12:16:55.108946 PyQt6-6.5.0/sip/QtGui/qicon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2384 2023-04-05 12:16:55.026086 PyQt6-6.5.0/sip/QtGui/qiconengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)    13954 2023-04-05 12:16:55.032853 PyQt6-6.5.0/sip/QtGui/qimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2751 2023-04-05 12:16:55.075186 PyQt6-6.5.0/sip/QtGui/qimageiohandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3480 2023-04-05 12:16:55.118199 PyQt6-6.5.0/sip/QtGui/qimagereader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2666 2023-04-05 12:16:55.082405 PyQt6-6.5.0/sip/QtGui/qimagewriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2591 2023-04-05 12:16:55.030822 PyQt6-6.5.0/sip/QtGui/qinputdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2303 2023-04-05 12:16:55.129155 PyQt6-6.5.0/sip/QtGui/qinputmethod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7031 2023-04-05 12:16:55.112484 PyQt6-6.5.0/sip/QtGui/qkeysequence.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9803 2023-04-05 12:16:55.027842 PyQt6-6.5.0/sip/QtGui/qmatrix4x4.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2857 2023-04-05 12:16:55.127911 PyQt6-6.5.0/sip/QtGui/qmovie.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1585 2023-04-05 12:16:55.108222 PyQt6-6.5.0/sip/QtGui/qoffscreensurface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2580 2023-04-05 12:16:55.053867 PyQt6-6.5.0/sip/QtGui/qopenglcontext.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1686 2023-04-05 12:16:55.028396 PyQt6-6.5.0/sip/QtGui/qpagedpaintdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3104 2023-04-05 12:16:55.057476 PyQt6-6.5.0/sip/QtGui/qpagelayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2145 2023-04-05 12:16:55.078776 PyQt6-6.5.0/sip/QtGui/qpageranges.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5591 2023-04-05 12:16:55.074579 PyQt6-6.5.0/sip/QtGui/qpagesize.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1994 2023-04-05 12:16:55.064493 PyQt6-6.5.0/sip/QtGui/qpaintdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1415 2023-04-05 12:16:55.116549 PyQt6-6.5.0/sip/QtGui/qpaintdevicewindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5665 2023-04-05 12:16:55.119336 PyQt6-6.5.0/sip/QtGui/qpaintengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)    20805 2023-04-05 12:16:55.077828 PyQt6-6.5.0/sip/QtGui/qpainter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6554 2023-04-05 12:16:55.105933 PyQt6-6.5.0/sip/QtGui/qpainterpath.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4511 2023-04-05 12:16:55.022729 PyQt6-6.5.0/sip/QtGui/qpalette.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1885 2023-04-05 12:16:55.071766 PyQt6-6.5.0/sip/QtGui/qpdfwriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3397 2023-04-05 12:16:55.021267 PyQt6-6.5.0/sip/QtGui/qpen.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2021 2023-04-05 12:16:55.113792 PyQt6-6.5.0/sip/QtGui/qpicture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5520 2023-04-05 12:16:55.073454 PyQt6-6.5.0/sip/QtGui/qpixelformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4917 2023-04-05 12:16:55.013596 PyQt6-6.5.0/sip/QtGui/qpixmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2240 2023-04-05 12:16:55.070394 PyQt6-6.5.0/sip/QtGui/qpixmapcache.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2499 2023-04-05 12:16:55.128546 PyQt6-6.5.0/sip/QtGui/qpointingdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11953 2023-04-05 12:16:55.056825 PyQt6-6.5.0/sip/QtGui/qpolygon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2719 2023-04-05 12:16:55.071249 PyQt6-6.5.0/sip/QtGui/qpygui_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5076 2023-04-05 12:16:55.054656 PyQt6-6.5.0/sip/QtGui/qquaternion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1230 2023-04-05 12:16:55.106396 PyQt6-6.5.0/sip/QtGui/qrasterwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3616 2023-04-05 12:16:55.053206 PyQt6-6.5.0/sip/QtGui/qrawfont.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3768 2023-04-05 12:16:55.111180 PyQt6-6.5.0/sip/QtGui/qregion.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1271 2023-04-05 12:16:55.012863 PyQt6-6.5.0/sip/QtGui/qrgb.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2141 2023-04-05 12:16:55.122065 PyQt6-6.5.0/sip/QtGui/qrgba64.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3073 2023-04-05 12:16:55.051377 PyQt6-6.5.0/sip/QtGui/qscreen.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1990 2023-04-05 12:16:55.115880 PyQt6-6.5.0/sip/QtGui/qsessionmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6080 2023-04-05 12:16:55.120347 PyQt6-6.5.0/sip/QtGui/qshortcut.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9704 2023-04-05 12:16:55.065663 PyQt6-6.5.0/sip/QtGui/qstandarditemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1953 2023-04-05 12:16:55.057986 PyQt6-6.5.0/sip/QtGui/qstatictext.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3060 2023-04-05 12:16:55.121504 PyQt6-6.5.0/sip/QtGui/qstylehints.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1634 2023-04-05 12:16:55.051982 PyQt6-6.5.0/sip/QtGui/qsurface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3651 2023-04-05 12:16:55.019966 PyQt6-6.5.0/sip/QtGui/qsurfaceformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2965 2023-04-05 12:16:55.016511 PyQt6-6.5.0/sip/QtGui/qsyntaxhighlighter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5531 2023-04-05 12:16:55.080938 PyQt6-6.5.0/sip/QtGui/qtextcursor.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12118 2023-04-05 12:16:55.067697 PyQt6-6.5.0/sip/QtGui/qtextdocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1935 2023-04-05 12:16:55.014101 PyQt6-6.5.0/sip/QtGui/qtextdocumentfragment.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1714 2023-04-05 12:16:55.123111 PyQt6-6.5.0/sip/QtGui/qtextdocumentwriter.sip
+-rw-r--r--   0 phil       (501) staff       (20)    19535 2023-04-05 12:16:55.061848 PyQt6-6.5.0/sip/QtGui/qtextformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5890 2023-04-05 12:16:55.015838 PyQt6-6.5.0/sip/QtGui/qtextlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1462 2023-04-05 12:16:55.014712 PyQt6-6.5.0/sip/QtGui/qtextlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7691 2023-04-05 12:16:55.018666 PyQt6-6.5.0/sip/QtGui/qtextobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2023-04-05 12:16:55.115264 PyQt6-6.5.0/sip/QtGui/qtextoption.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2569 2023-04-05 12:16:55.131730 PyQt6-6.5.0/sip/QtGui/qtexttable.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5139 2023-04-05 12:16:55.072602 PyQt6-6.5.0/sip/QtGui/qtransform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2042 2023-04-05 12:16:55.019204 PyQt6-6.5.0/sip/QtGui/qundogroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3004 2023-04-05 12:16:55.081756 PyQt6-6.5.0/sip/QtGui/qundostack.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1692 2023-04-05 12:16:55.080000 PyQt6-6.5.0/sip/QtGui/qutimimeconverter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3361 2023-04-05 12:16:55.113263 PyQt6-6.5.0/sip/QtGui/qvalidator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9152 2023-04-05 12:16:55.107745 PyQt6-6.5.0/sip/QtGui/qvectornd.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7236 2023-04-05 12:16:55.030087 PyQt6-6.5.0/sip/QtGui/qwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1009 2023-04-05 12:16:55.078283 PyQt6-6.5.0/sip/QtGui/qwindowdefs.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.600239 PyQt6-6.5.0/sip/QtHelp/
+-rw-r--r--   0 phil       (501) staff       (20)     2347 2023-04-05 12:16:54.952241 PyQt6-6.5.0/sip/QtHelp/QtHelpmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1429 2023-04-05 12:16:54.922145 PyQt6-6.5.0/sip/QtHelp/qcompressedhelpinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2348 2023-04-05 12:16:54.951310 PyQt6-6.5.0/sip/QtHelp/qhelpcontentwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1361 2023-04-05 12:16:54.951778 PyQt6-6.5.0/sip/QtHelp/qhelpengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4184 2023-04-05 12:16:54.923785 PyQt6-6.5.0/sip/QtHelp/qhelpenginecore.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1430 2023-04-05 12:16:54.922915 PyQt6-6.5.0/sip/QtHelp/qhelpfilterdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1889 2023-04-05 12:16:54.955064 PyQt6-6.5.0/sip/QtHelp/qhelpfilterengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-04-05 12:16:54.954599 PyQt6-6.5.0/sip/QtHelp/qhelpfiltersettingswidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1836 2023-04-05 12:16:54.952733 PyQt6-6.5.0/sip/QtHelp/qhelpindexwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1048 2023-04-05 12:16:54.954196 PyQt6-6.5.0/sip/QtHelp/qhelplink.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2399 2023-04-05 12:16:54.953360 PyQt6-6.5.0/sip/QtHelp/qhelpsearchengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1552 2023-04-05 12:16:54.953810 PyQt6-6.5.0/sip/QtHelp/qhelpsearchquerywidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1222 2023-04-05 12:16:54.922531 PyQt6-6.5.0/sip/QtHelp/qhelpsearchresultwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.727912 PyQt6-6.5.0/sip/QtMultimedia/
+-rw-r--r--   0 phil       (501) staff       (20)     2656 2023-04-05 12:16:55.408442 PyQt6-6.5.0/sip/QtMultimedia/QtMultimediamod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1516 2023-04-05 12:16:55.415619 PyQt6-6.5.0/sip/QtMultimedia/qaudio.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1993 2023-04-05 12:16:55.405045 PyQt6-6.5.0/sip/QtMultimedia/qaudiobuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2206 2023-04-05 12:16:55.419358 PyQt6-6.5.0/sip/QtMultimedia/qaudiodecoder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1930 2023-04-05 12:16:55.403876 PyQt6-6.5.0/sip/QtMultimedia/qaudiodevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3341 2023-04-05 12:16:55.409372 PyQt6-6.5.0/sip/QtMultimedia/qaudioformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1565 2023-04-05 12:16:55.417191 PyQt6-6.5.0/sip/QtMultimedia/qaudioinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1567 2023-04-05 12:16:55.404460 PyQt6-6.5.0/sip/QtMultimedia/qaudiooutput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1838 2023-04-05 12:16:55.406290 PyQt6-6.5.0/sip/QtMultimedia/qaudiosink.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1862 2023-04-05 12:16:55.416128 PyQt6-6.5.0/sip/QtMultimedia/qaudiosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7429 2023-04-05 12:16:55.410673 PyQt6-6.5.0/sip/QtMultimedia/qcamera.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2093 2023-04-05 12:16:55.411980 PyQt6-6.5.0/sip/QtMultimedia/qcameradevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3030 2023-04-05 12:16:55.405753 PyQt6-6.5.0/sip/QtMultimedia/qimagecapture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2160 2023-04-05 12:16:55.423158 PyQt6-6.5.0/sip/QtMultimedia/qmediacapturesession.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1540 2023-04-05 12:16:55.421733 PyQt6-6.5.0/sip/QtMultimedia/qmediadevices.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3349 2023-04-05 12:16:55.420881 PyQt6-6.5.0/sip/QtMultimedia/qmediaformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2186 2023-04-05 12:16:55.412615 PyQt6-6.5.0/sip/QtMultimedia/qmediametadata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4095 2023-04-05 12:16:55.418537 PyQt6-6.5.0/sip/QtMultimedia/qmediaplayer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3680 2023-04-05 12:16:55.407074 PyQt6-6.5.0/sip/QtMultimedia/qmediarecorder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3046 2023-04-05 12:16:55.411359 PyQt6-6.5.0/sip/QtMultimedia/qmediatimerange.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10957 2023-04-05 12:16:55.415085 PyQt6-6.5.0/sip/QtMultimedia/qpymultimedia_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1795 2023-04-05 12:16:55.417719 PyQt6-6.5.0/sip/QtMultimedia/qscreencapture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2198 2023-04-05 12:16:55.416724 PyQt6-6.5.0/sip/QtMultimedia/qsoundeffect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3181 2023-04-05 12:16:55.407872 PyQt6-6.5.0/sip/QtMultimedia/qvideoframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4710 2023-04-05 12:16:55.422643 PyQt6-6.5.0/sip/QtMultimedia/qvideoframeformat.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1508 2023-04-05 12:16:55.420118 PyQt6-6.5.0/sip/QtMultimedia/qvideosink.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.783898 PyQt6-6.5.0/sip/QtMultimediaWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2083 2023-04-05 12:16:55.672622 PyQt6-6.5.0/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2007 2023-04-05 12:16:55.673904 PyQt6-6.5.0/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2399 2023-04-05 12:16:55.673324 PyQt6-6.5.0/sip/QtMultimediaWidgets/qvideowidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.582625 PyQt6-6.5.0/sip/QtNetwork/
+-rw-r--r--   0 phil       (501) staff       (20)     3123 2023-04-05 12:16:54.858396 PyQt6-6.5.0/sip/QtNetwork/QtNetworkmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2995 2023-04-05 12:16:54.870570 PyQt6-6.5.0/sip/QtNetwork/qabstractnetworkcache.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10970 2023-04-05 12:16:54.872622 PyQt6-6.5.0/sip/QtNetwork/qabstractsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1584 2023-04-05 12:16:54.869602 PyQt6-6.5.0/sip/QtNetwork/qauthenticator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4595 2023-04-05 12:16:54.859405 PyQt6-6.5.0/sip/QtNetwork/qdnslookup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5644 2023-04-05 12:16:54.861806 PyQt6-6.5.0/sip/QtNetwork/qhostaddress.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2987 2023-04-05 12:16:54.862869 PyQt6-6.5.0/sip/QtNetwork/qhostinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1906 2023-04-05 12:16:54.878761 PyQt6-6.5.0/sip/QtNetwork/qhstspolicy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1632 2023-04-05 12:16:54.863316 PyQt6-6.5.0/sip/QtNetwork/qhttp1configuration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1863 2023-04-05 12:16:54.875496 PyQt6-6.5.0/sip/QtNetwork/qhttp2configuration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2111 2023-04-05 12:16:54.905143 PyQt6-6.5.0/sip/QtNetwork/qhttpmultipart.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2417 2023-04-05 12:16:54.862320 PyQt6-6.5.0/sip/QtNetwork/qlocalserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6739 2023-04-05 12:16:54.873613 PyQt6-6.5.0/sip/QtNetwork/qlocalsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4835 2023-04-05 12:16:54.866662 PyQt6-6.5.0/sip/QtNetwork/qnetworkaccessmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2540 2023-04-05 12:16:54.857752 PyQt6-6.5.0/sip/QtNetwork/qnetworkcookie.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1719 2023-04-05 12:16:54.904593 PyQt6-6.5.0/sip/QtNetwork/qnetworkcookiejar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1941 2023-04-05 12:16:54.854632 PyQt6-6.5.0/sip/QtNetwork/qnetworkdatagram.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1881 2023-04-05 12:16:54.870030 PyQt6-6.5.0/sip/QtNetwork/qnetworkdiskcache.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2950 2023-04-05 12:16:54.865834 PyQt6-6.5.0/sip/QtNetwork/qnetworkinformation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3720 2023-04-05 12:16:54.864614 PyQt6-6.5.0/sip/QtNetwork/qnetworkinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5091 2023-04-05 12:16:54.905976 PyQt6-6.5.0/sip/QtNetwork/qnetworkproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5728 2023-04-05 12:16:54.860330 PyQt6-6.5.0/sip/QtNetwork/qnetworkreply.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5117 2023-04-05 12:16:54.876345 PyQt6-6.5.0/sip/QtNetwork/qnetworkrequest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2020 2023-04-05 12:16:54.903319 PyQt6-6.5.0/sip/QtNetwork/qocspresponse.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1379 2023-04-05 12:16:54.860742 PyQt6-6.5.0/sip/QtNetwork/qpassworddigestor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3458 2023-04-05 12:16:54.904152 PyQt6-6.5.0/sip/QtNetwork/qpynetwork_qhash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7009 2023-04-05 12:16:54.878325 PyQt6-6.5.0/sip/QtNetwork/qpynetwork_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4985 2023-04-05 12:16:54.867901 PyQt6-6.5.0/sip/QtNetwork/qpynetwork_qmap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3643 2023-04-05 12:16:54.874441 PyQt6-6.5.0/sip/QtNetwork/qssl.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3763 2023-04-05 12:16:54.906649 PyQt6-6.5.0/sip/QtNetwork/qsslcertificate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1426 2023-04-05 12:16:54.874867 PyQt6-6.5.0/sip/QtNetwork/qsslcertificateextension.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1694 2023-04-05 12:16:54.863941 PyQt6-6.5.0/sip/QtNetwork/qsslcipher.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5201 2023-04-05 12:16:54.856893 PyQt6-6.5.0/sip/QtNetwork/qsslconfiguration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2171 2023-04-05 12:16:54.865082 PyQt6-6.5.0/sip/QtNetwork/qssldiffiehellmanparameters.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1594 2023-04-05 12:16:54.869072 PyQt6-6.5.0/sip/QtNetwork/qsslellipticcurve.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2803 2023-04-05 12:16:54.871135 PyQt6-6.5.0/sip/QtNetwork/qsslerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2021 2023-04-05 12:16:54.868489 PyQt6-6.5.0/sip/QtNetwork/qsslkey.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1883 2023-04-05 12:16:54.856090 PyQt6-6.5.0/sip/QtNetwork/qsslpresharedkeyauthenticator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2150 2023-04-05 12:16:54.855571 PyQt6-6.5.0/sip/QtNetwork/qsslserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8621 2023-04-05 12:16:54.901944 PyQt6-6.5.0/sip/QtNetwork/qsslsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2339 2023-04-05 12:16:54.876848 PyQt6-6.5.0/sip/QtNetwork/qtcpserver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1134 2023-04-05 12:16:54.855085 PyQt6-6.5.0/sip/QtNetwork/qtcpsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3235 2023-04-05 12:16:54.902720 PyQt6-6.5.0/sip/QtNetwork/qudpsocket.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.656131 PyQt6-6.5.0/sip/QtNfc/
+-rw-r--r--   0 phil       (501) staff       (20)     2146 2023-04-05 12:16:55.153710 PyQt6-6.5.0/sip/QtNfc/QtNfcmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1772 2023-04-05 12:16:55.155935 PyQt6-6.5.0/sip/QtNfc/qndeffilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2185 2023-04-05 12:16:55.154256 PyQt6-6.5.0/sip/QtNfc/qndefmessage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3351 2023-04-05 12:16:55.153272 PyQt6-6.5.0/sip/QtNfc/qndefnfcsmartposterrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1471 2023-04-05 12:16:55.154723 PyQt6-6.5.0/sip/QtNfc/qndefnfctextrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1213 2023-04-05 12:16:55.152620 PyQt6-6.5.0/sip/QtNfc/qndefnfcurirecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2536 2023-04-05 12:16:55.151390 PyQt6-6.5.0/sip/QtNfc/qndefrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3014 2023-04-05 12:16:55.152187 PyQt6-6.5.0/sip/QtNfc/qnearfieldmanager.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3250 2023-04-05 12:16:55.155428 PyQt6-6.5.0/sip/QtNfc/qnearfieldtarget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.543143 PyQt6-6.5.0/sip/QtOpenGL/
+-rw-r--r--   0 phil       (501) staff       (20)     2618 2023-04-05 12:16:54.766581 PyQt6-6.5.0/sip/QtOpenGL/QtOpenGLmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2645 2023-04-05 12:16:54.766075 PyQt6-6.5.0/sip/QtOpenGL/qopenglbuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5913 2023-04-05 12:16:54.765401 PyQt6-6.5.0/sip/QtOpenGL/qopengldebug.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5082 2023-04-05 12:16:54.733681 PyQt6-6.5.0/sip/QtOpenGL/qopenglframebufferobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)   111265 2023-04-05 12:16:54.746842 PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_2_0.sip
+-rw-r--r--   0 phil       (501) staff       (20)   111310 2023-04-05 12:16:54.763727 PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_2_1.sip
+-rw-r--r--   0 phil       (501) staff       (20)    42567 2023-04-05 12:16:54.728242 PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_4_1_core.sip
+-rw-r--r--   0 phil       (501) staff       (20)    28956 2023-04-05 12:16:54.771072 PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_es2.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1751 2023-04-05 12:16:54.732830 PyQt6-6.5.0/sip/QtOpenGL/qopenglpaintdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1865 2023-04-05 12:16:54.771623 PyQt6-6.5.0/sip/QtOpenGL/qopenglpixeltransferoptions.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15899 2023-04-05 12:16:54.774161 PyQt6-6.5.0/sip/QtOpenGL/qopenglshaderprogram.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14995 2023-04-05 12:16:54.732256 PyQt6-6.5.0/sip/QtOpenGL/qopengltexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2010 2023-04-05 12:16:54.772593 PyQt6-6.5.0/sip/QtOpenGL/qopengltextureblitter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2095 2023-04-05 12:16:54.729414 PyQt6-6.5.0/sip/QtOpenGL/qopengltimerquery.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1168 2023-04-05 12:16:54.729877 PyQt6-6.5.0/sip/QtOpenGL/qopenglversionfunctions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1350 2023-04-05 12:16:54.728787 PyQt6-6.5.0/sip/QtOpenGL/qopenglversionfunctionsfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1814 2023-04-05 12:16:54.772096 PyQt6-6.5.0/sip/QtOpenGL/qopenglversionprofile.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1909 2023-04-05 12:16:54.774800 PyQt6-6.5.0/sip/QtOpenGL/qopenglvertexarrayobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2173 2023-04-05 12:16:54.764448 PyQt6-6.5.0/sip/QtOpenGL/qopenglwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2926 2023-04-05 12:16:54.722952 PyQt6-6.5.0/sip/QtOpenGL/qpyopengl_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3170 2023-04-05 12:16:54.767398 PyQt6-6.5.0/sip/QtOpenGL/qpyopengl_std_pair.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.619979 PyQt6-6.5.0/sip/QtOpenGLWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2059 2023-04-05 12:16:55.011453 PyQt6-6.5.0/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3230 2023-04-05 12:16:55.012268 PyQt6-6.5.0/sip/QtOpenGLWidgets/qopenglwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.619223 PyQt6-6.5.0/sip/QtPdf/
+-rw-r--r--   0 phil       (501) staff       (20)     2169 2023-04-05 12:16:55.006174 PyQt6-6.5.0/sip/QtPdf/QtPdfmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1876 2023-04-05 12:16:55.008999 PyQt6-6.5.0/sip/QtPdf/qpdfbookmarkmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3512 2023-04-05 12:16:55.007903 PyQt6-6.5.0/sip/QtPdf/qpdfdocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2081 2023-04-05 12:16:55.009634 PyQt6-6.5.0/sip/QtPdf/qpdfdocumentrenderoptions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1460 2023-04-05 12:16:55.006637 PyQt6-6.5.0/sip/QtPdf/qpdflink.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1827 2023-04-05 12:16:55.008418 PyQt6-6.5.0/sip/QtPdf/qpdfpagenavigator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1681 2023-04-05 12:16:55.007120 PyQt6-6.5.0/sip/QtPdf/qpdfpagerenderer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1900 2023-04-05 12:16:55.010368 PyQt6-6.5.0/sip/QtPdf/qpdfsearchmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1430 2023-04-05 12:16:55.010857 PyQt6-6.5.0/sip/QtPdf/qpdfselection.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.786641 PyQt6-6.5.0/sip/QtPdfWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2012 2023-04-05 12:16:55.701292 PyQt6-6.5.0/sip/QtPdfWidgets/QtPdfWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2848 2023-04-05 12:16:55.702189 PyQt6-6.5.0/sip/QtPdfWidgets/qpdfview.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.735701 PyQt6-6.5.0/sip/QtPositioning/
+-rw-r--r--   0 phil       (501) staff       (20)     2365 2023-04-05 12:16:55.451948 PyQt6-6.5.0/sip/QtPositioning/QtPositioningmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2273 2023-04-05 12:16:55.460561 PyQt6-6.5.0/sip/QtPositioning/qgeoaddress.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2226 2023-04-05 12:16:55.458744 PyQt6-6.5.0/sip/QtPositioning/qgeoareamonitorinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3002 2023-04-05 12:16:55.457085 PyQt6-6.5.0/sip/QtPositioning/qgeoareamonitorsource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1857 2023-04-05 12:16:55.455703 PyQt6-6.5.0/sip/QtPositioning/qgeocircle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2775 2023-04-05 12:16:55.461247 PyQt6-6.5.0/sip/QtPositioning/qgeocoordinate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1850 2023-04-05 12:16:55.459285 PyQt6-6.5.0/sip/QtPositioning/qgeolocation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2370 2023-04-05 12:16:55.457632 PyQt6-6.5.0/sip/QtPositioning/qgeopath.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-05 12:16:55.458191 PyQt6-6.5.0/sip/QtPositioning/qgeopolygon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2502 2023-04-05 12:16:55.451247 PyQt6-6.5.0/sip/QtPositioning/qgeopositioninfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4135 2023-04-05 12:16:55.456472 PyQt6-6.5.0/sip/QtPositioning/qgeopositioninfosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2832 2023-04-05 12:16:55.453148 PyQt6-6.5.0/sip/QtPositioning/qgeorectangle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2343 2023-04-05 12:16:55.454487 PyQt6-6.5.0/sip/QtPositioning/qgeosatelliteinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2640 2023-04-05 12:16:55.459902 PyQt6-6.5.0/sip/QtPositioning/qgeosatelliteinfosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2434 2023-04-05 12:16:55.455178 PyQt6-6.5.0/sip/QtPositioning/qgeoshape.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2205 2023-04-05 12:16:55.453844 PyQt6-6.5.0/sip/QtPositioning/qnmeapositioninfosource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2448 2023-04-05 12:16:55.452543 PyQt6-6.5.0/sip/QtPositioning/qnmeasatelliteinfosource.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.535652 PyQt6-6.5.0/sip/QtPrintSupport/
+-rw-r--r--   0 phil       (501) staff       (20)     2261 2023-04-05 12:16:54.716488 PyQt6-6.5.0/sip/QtPrintSupport/QtPrintSupportmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3959 2023-04-05 12:16:54.715909 PyQt6-6.5.0/sip/QtPrintSupport/qabstractprintdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2569 2023-04-05 12:16:54.719423 PyQt6-6.5.0/sip/QtPrintSupport/qpagesetupdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2959 2023-04-05 12:16:54.714233 PyQt6-6.5.0/sip/QtPrintSupport/qprintdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2327 2023-04-05 12:16:54.720726 PyQt6-6.5.0/sip/QtPrintSupport/qprintengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4672 2023-04-05 12:16:54.721885 PyQt6-6.5.0/sip/QtPrintSupport/qprinter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2194 2023-04-05 12:16:54.720039 PyQt6-6.5.0/sip/QtPrintSupport/qprinterinfo.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2034 2023-04-05 12:16:54.714887 PyQt6-6.5.0/sip/QtPrintSupport/qprintpreviewdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2558 2023-04-05 12:16:54.717244 PyQt6-6.5.0/sip/QtPrintSupport/qprintpreviewwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4887 2023-04-05 12:16:54.718736 PyQt6-6.5.0/sip/QtPrintSupport/qpyprintsupport_qlist.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.554303 PyQt6-6.5.0/sip/QtQml/
+-rw-r--r--   0 phil       (501) staff       (20)     2708 2023-04-05 12:16:54.802739 PyQt6-6.5.0/sip/QtQml/QtQmlmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6133 2023-04-05 12:16:54.803831 PyQt6-6.5.0/sip/QtQml/qjsengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3449 2023-04-05 12:16:54.808224 PyQt6-6.5.0/sip/QtQml/qjsmanagedvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3260 2023-04-05 12:16:54.777501 PyQt6-6.5.0/sip/QtQml/qjsprimitivevalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3624 2023-04-05 12:16:54.801581 PyQt6-6.5.0/sip/QtQml/qjsvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1267 2023-04-05 12:16:54.776696 PyQt6-6.5.0/sip/QtQml/qjsvalueiterator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1412 2023-04-05 12:16:54.776268 PyQt6-6.5.0/sip/QtQml/qmlattachedpropertiesobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2851 2023-04-05 12:16:54.807054 PyQt6-6.5.0/sip/QtQml/qmlregistertype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1413 2023-04-05 12:16:54.804899 PyQt6-6.5.0/sip/QtQml/qpyqmllistproperty.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1852 2023-04-05 12:16:54.810494 PyQt6-6.5.0/sip/QtQml/qqml.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1354 2023-04-05 12:16:54.805834 PyQt6-6.5.0/sip/QtQml/qqmlabstracturlinterceptor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2102 2023-04-05 12:16:54.779518 PyQt6-6.5.0/sip/QtQml/qqmlapplicationengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3497 2023-04-05 12:16:54.778973 PyQt6-6.5.0/sip/QtQml/qqmlcomponent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2006 2023-04-05 12:16:54.810092 PyQt6-6.5.0/sip/QtQml/qqmlcontext.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5776 2023-04-05 12:16:54.811532 PyQt6-6.5.0/sip/QtQml/qqmlengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1624 2023-04-05 12:16:54.812063 PyQt6-6.5.0/sip/QtQml/qqmlerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1925 2023-04-05 12:16:54.809146 PyQt6-6.5.0/sip/QtQml/qqmlexpression.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1583 2023-04-05 12:16:54.805389 PyQt6-6.5.0/sip/QtQml/qqmlextensionplugin.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1303 2023-04-05 12:16:54.778413 PyQt6-6.5.0/sip/QtQml/qqmlfileselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2332 2023-04-05 12:16:54.778047 PyQt6-6.5.0/sip/QtQml/qqmlincubator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1898 2023-04-05 12:16:54.804346 PyQt6-6.5.0/sip/QtQml/qqmllist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1199 2023-04-05 12:16:54.807553 PyQt6-6.5.0/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1235 2023-04-05 12:16:54.808639 PyQt6-6.5.0/sip/QtQml/qqmlparserstatus.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4182 2023-04-05 12:16:54.775748 PyQt6-6.5.0/sip/QtQml/qqmlproperty.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1769 2023-04-05 12:16:54.802226 PyQt6-6.5.0/sip/QtQml/qqmlpropertymap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1254 2023-04-05 12:16:54.809567 PyQt6-6.5.0/sip/QtQml/qqmlpropertyvaluesource.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1457 2023-04-05 12:16:54.806317 PyQt6-6.5.0/sip/QtQml/qqmlscriptstring.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.667992 PyQt6-6.5.0/sip/QtQuick/
+-rw-r--r--   0 phil       (501) staff       (20)     2852 2023-04-05 12:16:55.168253 PyQt6-6.5.0/sip/QtQuick/QtQuickmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2548 2023-04-05 12:16:55.164767 PyQt6-6.5.0/sip/QtQuick/qquickframebufferobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2308 2023-04-05 12:16:55.174973 PyQt6-6.5.0/sip/QtQuick/qquickgraphicsconfiguration.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1298 2023-04-05 12:16:55.158763 PyQt6-6.5.0/sip/QtQuick/qquickgraphicsdevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2820 2023-04-05 12:16:55.173561 PyQt6-6.5.0/sip/QtQuick/qquickimageprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10164 2023-04-05 12:16:55.202816 PyQt6-6.5.0/sip/QtQuick/qquickitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1368 2023-04-05 12:16:55.201172 PyQt6-6.5.0/sip/QtQuick/qquickitemgrabresult.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2983 2023-04-05 12:16:55.162031 PyQt6-6.5.0/sip/QtQuick/qquickpainteditem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1662 2023-04-05 12:16:55.167780 PyQt6-6.5.0/sip/QtQuick/qquickrendercontrol.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2023-04-05 12:16:55.161195 PyQt6-6.5.0/sip/QtQuick/qquickrendertarget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1160 2023-04-05 12:16:55.170657 PyQt6-6.5.0/sip/QtQuick/qquicktextdocument.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2345 2023-04-05 12:16:55.176017 PyQt6-6.5.0/sip/QtQuick/qquickview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6928 2023-04-05 12:16:55.169734 PyQt6-6.5.0/sip/QtQuick/qquickwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1377 2023-04-05 12:16:55.163756 PyQt6-6.5.0/sip/QtQuick/qsgflatcolormaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)    11740 2023-04-05 12:16:55.167100 PyQt6-6.5.0/sip/QtQuick/qsggeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2762 2023-04-05 12:16:55.164244 PyQt6-6.5.0/sip/QtQuick/qsgimagenode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1747 2023-04-05 12:16:55.174002 PyQt6-6.5.0/sip/QtQuick/qsgmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4807 2023-04-05 12:16:55.160362 PyQt6-6.5.0/sip/QtQuick/qsgmaterialshader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1033 2023-04-05 12:16:55.162878 PyQt6-6.5.0/sip/QtQuick/qsgmaterialtype.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8652 2023-04-05 12:16:55.172938 PyQt6-6.5.0/sip/QtQuick/qsgnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1343 2023-04-05 12:16:55.176389 PyQt6-6.5.0/sip/QtQuick/qsgrectanglenode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3077 2023-04-05 12:16:55.165387 PyQt6-6.5.0/sip/QtQuick/qsgrendererinterface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2526 2023-04-05 12:16:55.170262 PyQt6-6.5.0/sip/QtQuick/qsgrendernode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1354 2023-04-05 12:16:55.171029 PyQt6-6.5.0/sip/QtQuick/qsgsimplerectnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2097 2023-04-05 12:16:55.174456 PyQt6-6.5.0/sip/QtQuick/qsgsimpletexturenode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2513 2023-04-05 12:16:55.159366 PyQt6-6.5.0/sip/QtQuick/qsgtexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1446 2023-04-05 12:16:55.168660 PyQt6-6.5.0/sip/QtQuick/qsgtexture_platform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2207 2023-04-05 12:16:55.162485 PyQt6-6.5.0/sip/QtQuick/qsgtexturematerial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1152 2023-04-05 12:16:55.175492 PyQt6-6.5.0/sip/QtQuick/qsgtextureprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1324 2023-04-05 12:16:55.163251 PyQt6-6.5.0/sip/QtQuick/qsgvertexcolormaterial.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.595013 PyQt6-6.5.0/sip/QtQuick3D/
+-rw-r--r--   0 phil       (501) staff       (20)     2086 2023-04-05 12:16:54.921130 PyQt6-6.5.0/sip/QtQuick3D/QtQuick3Dmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1086 2023-04-05 12:16:54.920753 PyQt6-6.5.0/sip/QtQuick3D/qquick3d.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3758 2023-04-05 12:16:54.920402 PyQt6-6.5.0/sip/QtQuick3D/qquick3dgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2159 2023-04-05 12:16:54.921706 PyQt6-6.5.0/sip/QtQuick3D/qquick3dobject.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2181 2023-04-05 12:16:54.919699 PyQt6-6.5.0/sip/QtQuick3D/qquick3dtexturedata.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.674297 PyQt6-6.5.0/sip/QtQuickWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2080 2023-04-05 12:16:55.214979 PyQt6-6.5.0/sip/QtQuickWidgets/QtQuickWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3345 2023-04-05 12:16:55.215690 PyQt6-6.5.0/sip/QtQuickWidgets/qquickwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.608564 PyQt6-6.5.0/sip/QtRemoteObjects/
+-rw-r--r--   0 phil       (501) staff       (20)     2163 2023-04-05 12:16:54.968404 PyQt6-6.5.0/sip/QtRemoteObjects/QtRemoteObjectsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2298 2023-04-05 12:16:54.966479 PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1221 2023-04-05 12:16:54.965454 PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6469 2023-04-05 12:16:54.967528 PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1429 2023-04-05 12:16:54.968888 PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectregistry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1689 2023-04-05 12:16:54.968016 PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectreplica.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2093 2023-04-05 12:16:54.965995 PyQt6-6.5.0/sip/QtRemoteObjects/qtremoteobjectglobal.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.616115 PyQt6-6.5.0/sip/QtSensors/
+-rw-r--r--   0 phil       (501) staff       (20)     2393 2023-04-05 12:16:55.004457 PyQt6-6.5.0/sip/QtSensors/QtSensorsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2037 2023-04-05 12:16:54.972993 PyQt6-6.5.0/sip/QtSensors/qaccelerometer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1842 2023-04-05 12:16:54.969784 PyQt6-6.5.0/sip/QtSensors/qambientlightsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1726 2023-04-05 12:16:54.974447 PyQt6-6.5.0/sip/QtSensors/qambienttemperaturesensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1641 2023-04-05 12:16:55.003934 PyQt6-6.5.0/sip/QtSensors/qcompass.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1645 2023-04-05 12:16:54.974930 PyQt6-6.5.0/sip/QtSensors/qgyroscope.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1701 2023-04-05 12:16:54.973980 PyQt6-6.5.0/sip/QtSensors/qhumiditysensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1649 2023-04-05 12:16:54.973507 PyQt6-6.5.0/sip/QtSensors/qirproximitysensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1719 2023-04-05 12:16:54.970488 PyQt6-6.5.0/sip/QtSensors/qlidsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1692 2023-04-05 12:16:54.972464 PyQt6-6.5.0/sip/QtSensors/qlightsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1918 2023-04-05 12:16:55.005055 PyQt6-6.5.0/sip/QtSensors/qmagnetometer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1856 2023-04-05 12:16:54.970997 PyQt6-6.5.0/sip/QtSensors/qorientationsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1682 2023-04-05 12:16:54.971944 PyQt6-6.5.0/sip/QtSensors/qpressuresensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1607 2023-04-05 12:16:54.971465 PyQt6-6.5.0/sip/QtSensors/qproximitysensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2023-04-05 12:16:55.005638 PyQt6-6.5.0/sip/QtSensors/qrotationsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7556 2023-04-05 12:16:55.003278 PyQt6-6.5.0/sip/QtSensors/qsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2079 2023-04-05 12:16:55.002040 PyQt6-6.5.0/sip/QtSensors/qtapsensor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1641 2023-04-05 12:16:55.001319 PyQt6-6.5.0/sip/QtSensors/qtiltsensor.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.657422 PyQt6-6.5.0/sip/QtSerialPort/
+-rw-r--r--   0 phil       (501) staff       (20)     1982 2023-04-05 12:16:55.156889 PyQt6-6.5.0/sip/QtSerialPort/QtSerialPortmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7926 2023-04-05 12:16:55.158248 PyQt6-6.5.0/sip/QtSerialPort/qserialport.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1768 2023-04-05 12:16:55.156467 PyQt6-6.5.0/sip/QtSerialPort/qserialportinfo.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.730006 PyQt6-6.5.0/sip/QtSpatialAudio/
+-rw-r--r--   0 phil       (501) staff       (20)     2107 2023-04-05 12:16:55.423623 PyQt6-6.5.0/sip/QtSpatialAudio/QtSpatialAudiomod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1672 2023-04-05 12:16:55.424903 PyQt6-6.5.0/sip/QtSpatialAudio/qambientsound.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2978 2023-04-05 12:16:55.426742 PyQt6-6.5.0/sip/QtSpatialAudio/qaudioengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1342 2023-04-05 12:16:55.425316 PyQt6-6.5.0/sip/QtSpatialAudio/qaudiolistener.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2771 2023-04-05 12:16:55.425962 PyQt6-6.5.0/sip/QtSpatialAudio/qaudioroom.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2891 2023-04-05 12:16:55.424314 PyQt6-6.5.0/sip/QtSpatialAudio/qspatialsound.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.719124 PyQt6-6.5.0/sip/QtSql/
+-rw-r--r--   0 phil       (501) staff       (20)     2287 2023-04-05 12:16:55.402026 PyQt6-6.5.0/sip/QtSql/QtSqlmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3746 2023-04-05 12:16:55.401476 PyQt6-6.5.0/sip/QtSql/qsqldatabase.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5000 2023-04-05 12:16:55.377452 PyQt6-6.5.0/sip/QtSql/qsqldriver.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2023-04-05 12:16:55.375849 PyQt6-6.5.0/sip/QtSql/qsqlerror.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2360 2023-04-05 12:16:55.403222 PyQt6-6.5.0/sip/QtSql/qsqlfield.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1497 2023-04-05 12:16:55.381414 PyQt6-6.5.0/sip/QtSql/qsqlindex.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3080 2023-04-05 12:16:55.379075 PyQt6-6.5.0/sip/QtSql/qsqlquery.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3117 2023-04-05 12:16:55.380938 PyQt6-6.5.0/sip/QtSql/qsqlquerymodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2260 2023-04-05 12:16:55.379622 PyQt6-6.5.0/sip/QtSql/qsqlrecord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1542 2023-04-05 12:16:55.378440 PyQt6-6.5.0/sip/QtSql/qsqlrelationaldelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2598 2023-04-05 12:16:55.402634 PyQt6-6.5.0/sip/QtSql/qsqlrelationaltablemodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3175 2023-04-05 12:16:55.376523 PyQt6-6.5.0/sip/QtSql/qsqlresult.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3785 2023-04-05 12:16:55.380323 PyQt6-6.5.0/sip/QtSql/qsqltablemodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1512 2023-04-05 12:16:55.377997 PyQt6-6.5.0/sip/QtSql/qtsqlglobal.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.603903 PyQt6-6.5.0/sip/QtSvg/
+-rw-r--r--   0 phil       (501) staff       (20)     1987 2023-04-05 12:16:54.959990 PyQt6-6.5.0/sip/QtSvg/QtSvgmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2082 2023-04-05 12:16:54.958936 PyQt6-6.5.0/sip/QtSvg/qsvggenerator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3043 2023-04-05 12:16:54.959579 PyQt6-6.5.0/sip/QtSvg/qsvgrenderer.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.605890 PyQt6-6.5.0/sip/QtSvgWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     2071 2023-04-05 12:16:54.964321 PyQt6-6.5.0/sip/QtSvgWidgets/QtSvgWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1911 2023-04-05 12:16:54.963920 PyQt6-6.5.0/sip/QtSvgWidgets/qgraphicssvgitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2035 2023-04-05 12:16:54.964815 PyQt6-6.5.0/sip/QtSvgWidgets/qsvgwidget.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.785901 PyQt6-6.5.0/sip/QtTest/
+-rw-r--r--   0 phil       (501) staff       (20)     2110 2023-04-05 12:16:55.674488 PyQt6-6.5.0/sip/QtTest/QtTestmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1689 2023-04-05 12:16:55.677312 PyQt6-6.5.0/sip/QtTest/qabstractitemmodeltester.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3285 2023-04-05 12:16:55.675821 PyQt6-6.5.0/sip/QtTest/qsignalspy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3740 2023-04-05 12:16:55.675067 PyQt6-6.5.0/sip/QtTest/qtestkeyboard.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2446 2023-04-05 12:16:55.676798 PyQt6-6.5.0/sip/QtTest/qtestmouse.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1381 2023-04-05 12:16:55.676304 PyQt6-6.5.0/sip/QtTest/qtestsystem.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.736757 PyQt6-6.5.0/sip/QtTextToSpeech/
+-rw-r--r--   0 phil       (501) staff       (20)     1981 2023-04-05 12:16:55.463113 PyQt6-6.5.0/sip/QtTextToSpeech/QtTextToSpeechmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3550 2023-04-05 12:16:55.462108 PyQt6-6.5.0/sip/QtTextToSpeech/qtexttospeech.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1760 2023-04-05 12:16:55.462664 PyQt6-6.5.0/sip/QtTextToSpeech/qvoice.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.675370 PyQt6-6.5.0/sip/QtWebChannel/
+-rw-r--r--   0 phil       (501) staff       (20)     1995 2023-04-05 12:16:55.216180 PyQt6-6.5.0/sip/QtWebChannel/QtWebChannelmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2363 2023-04-05 12:16:55.217334 PyQt6-6.5.0/sip/QtWebChannel/qwebchannel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1425 2023-04-05 12:16:55.216663 PyQt6-6.5.0/sip/QtWebChannel/qwebchannelabstracttransport.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.531944 PyQt6-6.5.0/sip/QtWebSockets/
+-rw-r--r--   0 phil       (501) staff       (20)     2158 2023-04-05 12:16:54.712049 PyQt6-6.5.0/sip/QtWebSockets/QtWebSocketsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1238 2023-04-05 12:16:54.712580 PyQt6-6.5.0/sip/QtWebSockets/qmaskgenerator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6039 2023-04-05 12:16:54.711501 PyQt6-6.5.0/sip/QtWebSockets/qwebsocket.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1445 2023-04-05 12:16:54.710239 PyQt6-6.5.0/sip/QtWebSockets/qwebsocketcorsauthenticator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1623 2023-04-05 12:16:54.709686 PyQt6-6.5.0/sip/QtWebSockets/qwebsockethandshakeoptions.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1741 2023-04-05 12:16:54.709089 PyQt6-6.5.0/sip/QtWebSockets/qwebsocketprotocol.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3249 2023-04-05 12:16:54.713411 PyQt6-6.5.0/sip/QtWebSockets/qwebsocketserver.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.714505 PyQt6-6.5.0/sip/QtWidgets/
+-rw-r--r--   0 phil       (501) staff       (20)     4913 2023-04-05 12:16:55.324521 PyQt6-6.5.0/sip/QtWidgets/QtWidgetsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2732 2023-04-05 12:16:55.365531 PyQt6-6.5.0/sip/QtWidgets/qabstractbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2621 2023-04-05 12:16:55.273313 PyQt6-6.5.0/sip/QtWidgets/qabstractitemdelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10372 2023-04-05 12:16:55.257523 PyQt6-6.5.0/sip/QtWidgets/qabstractitemview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3459 2023-04-05 12:16:55.366132 PyQt6-6.5.0/sip/QtWidgets/qabstractscrollarea.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3009 2023-04-05 12:16:55.222602 PyQt6-6.5.0/sip/QtWidgets/qabstractslider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4021 2023-04-05 12:16:55.323071 PyQt6-6.5.0/sip/QtWidgets/qabstractspinbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)    14136 2023-04-05 12:16:55.308479 PyQt6-6.5.0/sip/QtWidgets/qapplication.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4795 2023-04-05 12:16:55.259146 PyQt6-6.5.0/sip/QtWidgets/qboxlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1835 2023-04-05 12:16:55.266774 PyQt6-6.5.0/sip/QtWidgets/qbuttongroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4043 2023-04-05 12:16:55.361675 PyQt6-6.5.0/sip/QtWidgets/qcalendarwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1799 2023-04-05 12:16:55.271379 PyQt6-6.5.0/sip/QtWidgets/qcheckbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2995 2023-04-05 12:16:55.313118 PyQt6-6.5.0/sip/QtWidgets/qcolordialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2872 2023-04-05 12:16:55.270120 PyQt6-6.5.0/sip/QtWidgets/qcolumnview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6343 2023-04-05 12:16:55.373322 PyQt6-6.5.0/sip/QtWidgets/qcombobox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2023-04-05 12:16:55.356580 PyQt6-6.5.0/sip/QtWidgets/qcommandlinkbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3141 2023-04-05 12:16:55.355606 PyQt6-6.5.0/sip/QtWidgets/qcommonstyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3315 2023-04-05 12:16:55.263974 PyQt6-6.5.0/sip/QtWidgets/qcompleter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2437 2023-04-05 12:16:55.323655 PyQt6-6.5.0/sip/QtWidgets/qdatawidgetmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5039 2023-04-05 12:16:55.357953 PyQt6-6.5.0/sip/QtWidgets/qdatetimeedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1866 2023-04-05 12:16:55.255270 PyQt6-6.5.0/sip/QtWidgets/qdial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2692 2023-04-05 12:16:55.255941 PyQt6-6.5.0/sip/QtWidgets/qdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3396 2023-04-05 12:16:55.325229 PyQt6-6.5.0/sip/QtWidgets/qdialogbuttonbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2666 2023-04-05 12:16:55.363740 PyQt6-6.5.0/sip/QtWidgets/qdockwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2730 2023-04-05 12:16:55.360785 PyQt6-6.5.0/sip/QtWidgets/qdrawutil.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1389 2023-04-05 12:16:55.268524 PyQt6-6.5.0/sip/QtWidgets/qerrormessage.sip
+-rw-r--r--   0 phil       (501) staff       (20)    12183 2023-04-05 12:16:55.315452 PyQt6-6.5.0/sip/QtWidgets/qfiledialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2023-04-05 12:16:55.266286 PyQt6-6.5.0/sip/QtWidgets/qfileiconprovider.sip
+-rw-r--r--   0 phil       (501) staff       (20)      957 2023-04-05 12:16:55.273722 PyQt6-6.5.0/sip/QtWidgets/qfilesystemmodel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1392 2023-04-05 12:16:55.371201 PyQt6-6.5.0/sip/QtWidgets/qfocusframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2764 2023-04-05 12:16:55.258205 PyQt6-6.5.0/sip/QtWidgets/qfontcombobox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2916 2023-04-05 12:16:55.229776 PyQt6-6.5.0/sip/QtWidgets/qfontdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4981 2023-04-05 12:16:55.229093 PyQt6-6.5.0/sip/QtWidgets/qformlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2164 2023-04-05 12:16:55.219682 PyQt6-6.5.0/sip/QtWidgets/qframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5339 2023-04-05 12:16:55.359730 PyQt6-6.5.0/sip/QtWidgets/qgesture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1738 2023-04-05 12:16:55.357073 PyQt6-6.5.0/sip/QtWidgets/qgesturerecognizer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-04-05 12:16:55.251385 PyQt6-6.5.0/sip/QtWidgets/qgraphicsanchorlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5015 2023-04-05 12:16:55.372287 PyQt6-6.5.0/sip/QtWidgets/qgraphicseffect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4207 2023-04-05 12:16:55.374044 PyQt6-6.5.0/sip/QtWidgets/qgraphicsgridlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)    26805 2023-04-05 12:16:55.369315 PyQt6-6.5.0/sip/QtWidgets/qgraphicsitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1730 2023-04-05 12:16:55.224230 PyQt6-6.5.0/sip/QtWidgets/qgraphicslayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3128 2023-04-05 12:16:55.252227 PyQt6-6.5.0/sip/QtWidgets/qgraphicslayoutitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3150 2023-04-05 12:16:55.310026 PyQt6-6.5.0/sip/QtWidgets/qgraphicslinearlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3920 2023-04-05 12:16:55.272062 PyQt6-6.5.0/sip/QtWidgets/qgraphicsproxywidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8768 2023-04-05 12:16:55.326208 PyQt6-6.5.0/sip/QtWidgets/qgraphicsscene.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6166 2023-04-05 12:16:55.268057 PyQt6-6.5.0/sip/QtWidgets/qgraphicssceneevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2441 2023-04-05 12:16:55.320927 PyQt6-6.5.0/sip/QtWidgets/qgraphicstransform.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8125 2023-04-05 12:16:55.375181 PyQt6-6.5.0/sip/QtWidgets/qgraphicsview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5459 2023-04-05 12:16:55.309391 PyQt6-6.5.0/sip/QtWidgets/qgraphicswidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5537 2023-04-05 12:16:55.263254 PyQt6-6.5.0/sip/QtWidgets/qgridlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2122 2023-04-05 12:16:55.316627 PyQt6-6.5.0/sip/QtWidgets/qgroupbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7170 2023-04-05 12:16:55.274734 PyQt6-6.5.0/sip/QtWidgets/qheaderview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5360 2023-04-05 12:16:55.221096 PyQt6-6.5.0/sip/QtWidgets/qinputdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2931 2023-04-05 12:16:55.364914 PyQt6-6.5.0/sip/QtWidgets/qitemdelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1812 2023-04-05 12:16:55.303815 PyQt6-6.5.0/sip/QtWidgets/qitemeditorfactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2219 2023-04-05 12:16:55.220289 PyQt6-6.5.0/sip/QtWidgets/qkeysequenceedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6063 2023-04-05 12:16:55.317731 PyQt6-6.5.0/sip/QtWidgets/qlabel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5894 2023-04-05 12:16:55.230779 PyQt6-6.5.0/sip/QtWidgets/qlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3732 2023-04-05 12:16:55.311358 PyQt6-6.5.0/sip/QtWidgets/qlayoutitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2378 2023-04-05 12:16:55.218144 PyQt6-6.5.0/sip/QtWidgets/qlcdnumber.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5210 2023-04-05 12:16:55.305473 PyQt6-6.5.0/sip/QtWidgets/qlineedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4961 2023-04-05 12:16:55.265865 PyQt6-6.5.0/sip/QtWidgets/qlistview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7358 2023-04-05 12:16:55.354618 PyQt6-6.5.0/sip/QtWidgets/qlistwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4691 2023-04-05 12:16:55.306735 PyQt6-6.5.0/sip/QtWidgets/qmainwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4174 2023-04-05 12:16:55.221900 PyQt6-6.5.0/sip/QtWidgets/qmdiarea.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4054 2023-04-05 12:16:55.362782 PyQt6-6.5.0/sip/QtWidgets/qmdisubwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5652 2023-04-05 12:16:55.254700 PyQt6-6.5.0/sip/QtWidgets/qmenu.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3601 2023-04-05 12:16:55.353528 PyQt6-6.5.0/sip/QtWidgets/qmenubar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6307 2023-04-05 12:16:55.312438 PyQt6-6.5.0/sip/QtWidgets/qmessagebox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7249 2023-04-05 12:16:55.329048 PyQt6-6.5.0/sip/QtWidgets/qplaintextedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2226 2023-04-05 12:16:55.231362 PyQt6-6.5.0/sip/QtWidgets/qprogressbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2903 2023-04-05 12:16:55.223769 PyQt6-6.5.0/sip/QtWidgets/qprogressdialog.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3947 2023-04-05 12:16:55.223142 PyQt6-6.5.0/sip/QtWidgets/qproxystyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2069 2023-04-05 12:16:55.316049 PyQt6-6.5.0/sip/QtWidgets/qpushbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2905 2023-04-05 12:16:55.319739 PyQt6-6.5.0/sip/QtWidgets/qpywidgets_qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1555 2023-04-05 12:16:55.356084 PyQt6-6.5.0/sip/QtWidgets/qradiobutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1794 2023-04-05 12:16:55.310559 PyQt6-6.5.0/sip/QtWidgets/qrubberband.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1895 2023-04-05 12:16:55.327639 PyQt6-6.5.0/sip/QtWidgets/qscrollarea.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1773 2023-04-05 12:16:55.224701 PyQt6-6.5.0/sip/QtWidgets/qscrollbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2896 2023-04-05 12:16:55.275417 PyQt6-6.5.0/sip/QtWidgets/qscroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2485 2023-04-05 12:16:55.304482 PyQt6-6.5.0/sip/QtWidgets/qscrollerproperties.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1640 2023-04-05 12:16:55.265036 PyQt6-6.5.0/sip/QtWidgets/qsizegrip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3272 2023-04-05 12:16:55.270860 PyQt6-6.5.0/sip/QtWidgets/qsizepolicy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1921 2023-04-05 12:16:55.352813 PyQt6-6.5.0/sip/QtWidgets/qslider.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3301 2023-04-05 12:16:55.313849 PyQt6-6.5.0/sip/QtWidgets/qspinbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1798 2023-04-05 12:16:55.260624 PyQt6-6.5.0/sip/QtWidgets/qsplashscreen.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3429 2023-04-05 12:16:55.327127 PyQt6-6.5.0/sip/QtWidgets/qsplitter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3651 2023-04-05 12:16:55.318772 PyQt6-6.5.0/sip/QtWidgets/qstackedlayout.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1662 2023-04-05 12:16:55.360311 PyQt6-6.5.0/sip/QtWidgets/qstackedwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1956 2023-04-05 12:16:55.262304 PyQt6-6.5.0/sip/QtWidgets/qstatusbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)    22575 2023-04-05 12:16:55.227992 PyQt6-6.5.0/sip/QtWidgets/qstyle.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2426 2023-04-05 12:16:55.320262 PyQt6-6.5.0/sip/QtWidgets/qstyleditemdelegate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1122 2023-04-05 12:16:55.261675 PyQt6-6.5.0/sip/QtWidgets/qstylefactory.sip
+-rw-r--r--   0 phil       (501) staff       (20)    20087 2023-04-05 12:16:55.280254 PyQt6-6.5.0/sip/QtWidgets/qstyleoption.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1732 2023-04-05 12:16:55.364429 PyQt6-6.5.0/sip/QtWidgets/qstylepainter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2317 2023-04-05 12:16:55.272770 PyQt6-6.5.0/sip/QtWidgets/qsystemtrayicon.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5251 2023-04-05 12:16:55.281370 PyQt6-6.5.0/sip/QtWidgets/qtabbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4837 2023-04-05 12:16:55.358721 PyQt6-6.5.0/sip/QtWidgets/qtableview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     9246 2023-04-05 12:16:55.253687 PyQt6-6.5.0/sip/QtWidgets/qtablewidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4240 2023-04-05 12:16:55.282786 PyQt6-6.5.0/sip/QtWidgets/qtabwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2740 2023-04-05 12:16:55.269585 PyQt6-6.5.0/sip/QtWidgets/qtextbrowser.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7388 2023-04-05 12:16:55.352162 PyQt6-6.5.0/sip/QtWidgets/qtextedit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4343 2023-04-05 12:16:55.260059 PyQt6-6.5.0/sip/QtWidgets/qtoolbar.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2421 2023-04-05 12:16:55.264545 PyQt6-6.5.0/sip/QtWidgets/qtoolbox.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2556 2023-04-05 12:16:55.322227 PyQt6-6.5.0/sip/QtWidgets/qtoolbutton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1399 2023-04-05 12:16:55.305932 PyQt6-6.5.0/sip/QtWidgets/qtooltip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6474 2023-04-05 12:16:55.219063 PyQt6-6.5.0/sip/QtWidgets/qtreeview.sip
+-rw-r--r--   0 phil       (501) staff       (20)    10328 2023-04-05 12:16:55.330805 PyQt6-6.5.0/sip/QtWidgets/qtreewidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2195 2023-04-05 12:16:55.321529 PyQt6-6.5.0/sip/QtWidgets/qtreewidgetitemiterator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1597 2023-04-05 12:16:55.268985 PyQt6-6.5.0/sip/QtWidgets/qundoview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1353 2023-04-05 12:16:55.355094 PyQt6-6.5.0/sip/QtWidgets/qwhatsthis.sip
+-rw-r--r--   0 phil       (501) staff       (20)    18362 2023-04-05 12:16:55.303142 PyQt6-6.5.0/sip/QtWidgets/qwidget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1627 2023-04-05 12:16:55.261190 PyQt6-6.5.0/sip/QtWidgets/qwidgetaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7633 2023-04-05 12:16:55.370736 PyQt6-6.5.0/sip/QtWidgets/qwizard.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.604769 PyQt6-6.5.0/sip/QtXml/
+-rw-r--r--   0 phil       (501) staff       (20)     1925 2023-04-05 12:16:54.963218 PyQt6-6.5.0/sip/QtXml/QtXmlmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)    16807 2023-04-05 12:16:54.962666 PyQt6-6.5.0/sip/QtXml/qdom.sip
+-rw-r--r--   0 phil       (501) staff       (20)       22 2023-04-05 12:16:54.708319 PyQt6-6.5.0/sip/pyqt-gpl.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.401027 PyQt6-6.5.0/uic/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.403966 PyQt6-6.5.0/uic/Compiler/
+-rw-r--r--   0 phil       (501) staff       (20)     1004 2023-04-05 12:16:47.666494 PyQt6-6.5.0/uic/Compiler/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     1412 2023-04-05 12:16:47.669584 PyQt6-6.5.0/uic/Compiler/as_string.py
+-rw-r--r--   0 phil       (501) staff       (20)     3934 2023-04-05 12:16:47.666209 PyQt6-6.5.0/uic/Compiler/compiler.py
+-rw-r--r--   0 phil       (501) staff       (20)     2742 2023-04-05 12:16:47.667366 PyQt6-6.5.0/uic/Compiler/indenter.py
+-rw-r--r--   0 phil       (501) staff       (20)     2374 2023-04-05 12:16:47.665586 PyQt6-6.5.0/uic/Compiler/misc.py
+-rw-r--r--   0 phil       (501) staff       (20)     4324 2023-04-05 12:16:47.669173 PyQt6-6.5.0/uic/Compiler/proxy_metaclass.py
+-rw-r--r--   0 phil       (501) staff       (20)     5839 2023-04-05 12:16:47.668475 PyQt6-6.5.0/uic/Compiler/qobjectcreator.py
+-rw-r--r--   0 phil       (501) staff       (20)    16164 2023-04-05 12:16:47.671774 PyQt6-6.5.0/uic/Compiler/qtproxies.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.400608 PyQt6-6.5.0/uic/Loader/
+-rw-r--r--   0 phil       (501) staff       (20)     1004 2023-04-05 12:16:47.659712 PyQt6-6.5.0/uic/Loader/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2625 2023-04-05 12:16:47.661665 PyQt6-6.5.0/uic/Loader/loader.py
+-rw-r--r--   0 phil       (501) staff       (20)     5187 2023-04-05 12:16:47.660974 PyQt6-6.5.0/uic/Loader/qobjectcreator.py
+-rw-r--r--   0 phil       (501) staff       (20)     1003 2023-04-05 12:16:47.659134 PyQt6-6.5.0/uic/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5473 2023-04-05 12:16:47.672638 PyQt6-6.5.0/uic/compile_ui.py
+-rw-r--r--   0 phil       (501) staff       (20)    31764 2023-04-05 12:16:47.658684 PyQt6-6.5.0/uic/enum_map.py
+-rw-r--r--   0 phil       (501) staff       (20)     2609 2023-04-05 12:16:47.664066 PyQt6-6.5.0/uic/exceptions.py
+-rw-r--r--   0 phil       (501) staff       (20)     5047 2023-04-05 12:16:47.662753 PyQt6-6.5.0/uic/icon_cache.py
+-rw-r--r--   0 phil       (501) staff       (20)     3327 2023-04-05 12:16:47.663348 PyQt6-6.5.0/uic/load_ui.py
+-rw-r--r--   0 phil       (501) staff       (20)     6097 2023-04-05 12:16:47.650556 PyQt6-6.5.0/uic/objcreator.py
+-rw-r--r--   0 phil       (501) staff       (20)    18275 2023-04-05 12:16:47.653209 PyQt6-6.5.0/uic/properties.py
+-rw-r--r--   0 phil       (501) staff       (20)     4653 2023-04-05 12:16:47.664907 PyQt6-6.5.0/uic/pyuic.py
+-rw-r--r--   0 phil       (501) staff       (20)     3213 2023-04-05 12:16:47.645389 PyQt6-6.5.0/uic/ui_file.py
+-rw-r--r--   0 phil       (501) staff       (20)    37502 2023-04-05 12:16:47.649697 PyQt6-6.5.0/uic/uiparser.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-05 12:16:56.399310 PyQt6-6.5.0/uic/widget-plugins/
+-rw-r--r--   0 phil       (501) staff       (20)     1557 2023-04-05 12:16:47.656400 PyQt6-6.5.0/uic/widget-plugins/qaxcontainer.py
+-rw-r--r--   0 phil       (501) staff       (20)     1553 2023-04-05 12:16:47.654236 PyQt6-6.5.0/uic/widget-plugins/qscintilla.py
+-rw-r--r--   0 phil       (501) staff       (20)     1562 2023-04-05 12:16:47.655157 PyQt6-6.5.0/uic/widget-plugins/qtcharts.py
+-rw-r--r--   0 phil       (501) staff       (20)     1588 2023-04-05 12:16:47.655530 PyQt6-6.5.0/uic/widget-plugins/qtprintsupport.py
+-rw-r--r--   0 phil       (501) staff       (20)     1562 2023-04-05 12:16:47.655852 PyQt6-6.5.0/uic/widget-plugins/qtquickwidgets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1568 2023-04-05 12:16:47.654764 PyQt6-6.5.0/uic/widget-plugins/qtwebenginewidgets.py
```

### Comparing `PyQt6-6.4.2/ChangeLog` & `PyQt6-6.5.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,109 @@
+2023-04-05  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qpy/QtCore/qpycore_chimera.cpp:
+	Fixed a regression in the handling of QFlags as signal arguments.
+	[db2b0386d4f1] [6.5.0]
+
+2023-04-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp, project.py, pyproject.toml:
+	Added the QtSpatialAudio module.
+	[077c776029a6]
+
+2023-04-03  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp:
+	Updated for Qt v6.5.0.
+	[729660e6fc61]
+
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* PyQt6.msp:
+	Updated QtWidgets for Qt v6.5.0rc.
+	[626287dd0ed1]
+
+	* NEWS, PyQt6.msp:
+	Updated QtRemoteObjects, QtSensors, QtSql, QtSvg, QtSvgWidgets,
+	QtTest, QtTextToSpeech, QtWebChannel, QtWebSockets and QtXml for Qt
+	v6.5.0rc.
+	[161ffed7ef69]
+
+2023-03-30  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* PyQt6.msp:
+	Updated QtQml, QtQuick, QtQuick3D and QtQuickWidgets for Qt
+	v6.5.0rc.
+	[8ae811bd2c98]
+
+	* NEWS, PyQt6.msp:
+	Updated QtNetwork, QtNfc, QtOpenGL, QtOpenGLWidgets, QtPdf,
+	QtPdfWidgets, QtPoitioning and QtPrintSupport for Qt v6.5.0rc.
+	[b4b6ff5dc2d6]
+
+	* PyQt6.msp, mksccode/QtMultimedia.versions:
+	Updated the sub-class convertor code for QtMultimedia.
+	[5fbc985e8383]
+
+	* PyQt6.msp, qpy/QtCore/qpycore_qlist.sip:
+	Updated QtDBus, QtDesigner, QtGui, QtHelp, QtMultimedia and
+	QtMultimediaWidgets for Qt v6.5.0rc.
+	[a721ab062d44]
+
+2023-03-29  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp:
+	Updated QtBluetooth and QtCore for Qt v6.5.0rc.
+	[8f2a4645ecca]
+
+	* Merged the 6.4-maint branch.
+	[43d0515da1a2]
+
+2023-03-25  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* qpy/QtCore/qpycore_chimera.cpp, qpy/QtCore/qpycore_chimera.h:
+	Ensure Qt property getters and setters handle user-defined enums
+	properly. Note that Designer still requires enums to be registered.
+	[1765171f142d] <6.4-maint>
+
+	* NEWS, PyQt6.msp:
+	Improved the error checking when writing an enum property.
+	[8432953b3600] <6.4-maint>
+
+2023-03-24  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6.msp:
+	Fixed QMetaProperty.write() to handle values of unregistered enums.
+	[2064a87dba00] <6.4-maint>
+
+2023-03-19  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* qpy/QtCore/qpycore_chimera.cpp, qpy/QtCore/qpycore_chimera.h:
+	Further improvements to reading user-defined Enum properties.
+	[be6f382a1f57] <6.4-maint>
+
+	* NEWS, qpy/QtCore/qpycore_chimera.cpp, qpy/QtCore/qpycore_chimera.h,
+	qpy/QtCore/qpycore_enums_flags.cpp, qpy/QtCore/qpycore_types.cpp,
+	test/metaobject/test_pyqtproperty.py:
+	Fixed QMetaProperty.read() for user-defined enums.
+	[9ef37f530e08] <6.4-maint>
+
+2023-03-08  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, qpy/QtCore/qpycore_pyqtboundsignal.cpp:
+	When comparing types of a decorated slot, use the name of the C++
+	type rather rather than the meta-type (which may have changed).
+	[9d77aaabfdff] <6.4-maint>
+
+2023-02-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 6.4.2 for changeset 0cf0f5deb862
+	[6008d812dbde] <6.4-maint>
+
 2023-01-28  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, extras/lupdate/lupdate.py:
 	Fixed a regression in pylupdate.
 	[0cf0f5deb862] [6.4.2] <6.4-maint>
 
 2023-01-27  Phil Thompson  <phil@riverbankcomputing.com>
```

### Comparing `PyQt6-6.4.2/LICENSE` & `PyQt6-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/NEWS` & `PyQt6-6.5.0/NEWS`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v6.5.0 5th April 2023
+  - Added support for Qt v6.5 including the QtSpatialAudio module.
+  - Bug fixes.
+
 v6.4.2 28th January 2023
   - Bug fixes.
 
 v6.4.1 27th January 2023
   - Added allocationLimit() and setAllocationLimit() to QImageReader.
   - Added toHBITMAP(), fromHBITMAP(), toHICON() and fromHICON() to QImage on
     Windows.
```

### Comparing `PyQt6-6.4.2/PKG-INFO` & `PyQt6-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6
-Version: 6.4.2
+Version: 6.5.0
 Requires-Python: >=3.6.1
 Summary: Python bindings for the Qt cross platform application toolkit
 Home-Page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6-sip (>=13.4, <14)
```

### Comparing `PyQt6-6.4.2/README` & `PyQt6-6.5.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/__init__.py` & `PyQt6-6.5.0/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/config-tests/cfgtest_QtCore.cpp` & `PyQt6-6.5.0/config-tests/cfgtest_QtCore.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/config-tests/cfgtest_QtGui.cpp` & `PyQt6-6.5.0/config-tests/cfgtest_QtGui.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/config-tests/cfgtest_QtNetwork.cpp` & `PyQt6-6.5.0/config-tests/cfgtest_QtNetwork.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/config-tests/cfgtest_QtPrintSupport.cpp` & `PyQt6-6.5.0/config-tests/cfgtest_QtPrintSupport.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/dbus/dbus.cpp` & `PyQt6-6.5.0/dbus/dbus.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/dbus/helper.h` & `PyQt6-6.5.0/dbus/helper.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/designer/pluginloader.cpp` & `PyQt6-6.5.0/designer/pluginloader.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/designer/pluginloader.h` & `PyQt6-6.5.0/designer/pluginloader.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/calculatorform/calculatorform.py` & `PyQt6-6.5.0/examples/designer/calculatorform/calculatorform.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/calculatorform/calculatorform.ui` & `PyQt6-6.5.0/examples/designer/calculatorform/calculatorform.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/calculatorform/ui_calculatorform.py` & `PyQt6-6.5.0/examples/designer/calculatorform/ui_calculatorform.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/plugins.py` & `PyQt6-6.5.0/examples/designer/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/analogclockplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/analogclockplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/bubbleswidgetplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/bubbleswidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/counterlabelplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/counterlabelplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/datetimeeditplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/datetimeeditplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/helloglwidgetplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/helloglwidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/multipagewidgetplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/multipagewidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/polygonwidgetplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/polygonwidgetplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/pydemoplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/pydemoplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/python/pythonconsoleplugin.py` & `PyQt6-6.5.0/examples/designer/plugins/python/pythonconsoleplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/analogclock.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/analogclock.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/bubbleswidget.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/bubbleswidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/counterlabel.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/counterlabel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/datetimeedit.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/helloglwidget.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/helloglwidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/multipagewidget.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/multipagewidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/polygonwidget.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/polygonwidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/pydemo.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/pydemo.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/designer/plugins/widgets/pythonconsolewidget.py` & `PyQt6-6.5.0/examples/designer/plugins/widgets/pythonconsolewidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/desktop/screenshot.py` & `PyQt6-6.5.0/examples/desktop/screenshot.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/desktop/systray/images/bad.png` & `PyQt6-6.5.0/examples/desktop/systray/images/bad.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/desktop/systray/images/heart.png` & `PyQt6-6.5.0/examples/desktop/systray/images/heart.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/desktop/systray/images/trash.png` & `PyQt6-6.5.0/examples/desktop/systray/images/trash.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/desktop/systray/systray.py` & `PyQt6-6.5.0/examples/desktop/systray/systray.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/classwizard.py` & `PyQt6-6.5.0/examples/dialogs/classwizard/classwizard.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/background.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/background.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/banner.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/banner.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/logo1.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/logo1.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/logo2.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/logo2.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/logo3.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/logo3.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/watermark1.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/watermark1.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/classwizard/images/watermark2.png` & `PyQt6-6.5.0/examples/dialogs/classwizard/images/watermark2.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/configdialog/configdialog.py` & `PyQt6-6.5.0/examples/dialogs/configdialog/configdialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/configdialog/images/config.png` & `PyQt6-6.5.0/examples/dialogs/configdialog/images/config.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/configdialog/images/query.png` & `PyQt6-6.5.0/examples/dialogs/configdialog/images/query.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/configdialog/images/update.png` & `PyQt6-6.5.0/examples/dialogs/configdialog/images/update.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/extension.py` & `PyQt6-6.5.0/examples/dialogs/extension.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/findfiles.py` & `PyQt6-6.5.0/examples/dialogs/findfiles.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/standarddialogs.py` & `PyQt6-6.5.0/examples/dialogs/standarddialogs.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/tabdialog.py` & `PyQt6-6.5.0/examples/dialogs/tabdialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/dialogs/trivialwizard.py` & `PyQt6-6.5.0/examples/dialogs/trivialwizard.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/delayedencoding/delayedencoding.py` & `PyQt6-6.5.0/examples/draganddrop/delayedencoding/delayedencoding.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/delayedencoding/images/drag.png` & `PyQt6-6.5.0/examples/draganddrop/delayedencoding/images/drag.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/delayedencoding/images/example.svg` & `PyQt6-6.5.0/examples/draganddrop/delayedencoding/images/example.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/draggableicons/draggableicons.py` & `PyQt6-6.5.0/examples/draganddrop/draggableicons/draggableicons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/draggableicons/images/boat.png` & `PyQt6-6.5.0/examples/draganddrop/draggableicons/images/boat.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/draggableicons/images/car.png` & `PyQt6-6.5.0/examples/draganddrop/draggableicons/images/car.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/draggableicons/images/house.png` & `PyQt6-6.5.0/examples/draganddrop/draggableicons/images/house.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/draggabletext/draggabletext.py` & `PyQt6-6.5.0/examples/draganddrop/draggabletext/draggabletext.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/dropsite.py` & `PyQt6-6.5.0/examples/draganddrop/dropsite.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/fridgemagnets/fridgemagnets.py` & `PyQt6-6.5.0/examples/draganddrop/fridgemagnets/fridgemagnets.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/puzzle/example.jpg` & `PyQt6-6.5.0/examples/draganddrop/puzzle/example.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/draganddrop/puzzle/puzzle.py` & `PyQt6-6.5.0/examples/draganddrop/puzzle/puzzle.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimedia/audiodevices/audiodevices.py` & `PyQt6-6.5.0/examples/multimedia/audiodevices/audiodevices.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimedia/audiodevices/audiodevicesbase.ui` & `PyQt6-6.5.0/examples/multimedia/audiodevices/audiodevicesbase.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimedia/audiodevices/ui_audiodevicesbase.py` & `PyQt6-6.5.0/examples/multimedia/audiodevices/ui_audiodevicesbase.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimedia/audiooutput.py` & `PyQt6-6.5.0/examples/multimedia/audiooutput.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/camera.py` & `PyQt6-6.5.0/examples/multimediawidgets/camera/camera.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/camera.ui` & `PyQt6-6.5.0/examples/multimediawidgets/camera/camera.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/images/shutter.svg` & `PyQt6-6.5.0/examples/multimediawidgets/camera/images/shutter.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/imagesettings.ui` & `PyQt6-6.5.0/examples/multimediawidgets/camera/imagesettings.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/ui_camera.py` & `PyQt6-6.5.0/examples/multimediawidgets/camera/ui_camera.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/ui_imagesettings.py` & `PyQt6-6.5.0/examples/multimediawidgets/camera/ui_imagesettings.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/ui_videosettings.py` & `PyQt6-6.5.0/examples/multimediawidgets/camera/ui_videosettings.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/camera/videosettings.ui` & `PyQt6-6.5.0/examples/multimediawidgets/camera/videosettings.ui`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/videographicsitem.py` & `PyQt6-6.5.0/examples/multimediawidgets/videographicsitem.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/multimediawidgets/videowidget.py` & `PyQt6-6.5.0/examples/multimediawidgets/videowidget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/adding.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/adding.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/attached.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/attached.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/binding.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/binding.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/coercion.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/coercion.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/default.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/default.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/grouped.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/grouped.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/methods.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/methods.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/properties.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/properties.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/signal.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/signal.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/qml/referenceexamples/valuesource.py` & `PyQt6-6.5.0/examples/qml/referenceexamples/valuesource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/animation.py` & `PyQt6-6.5.0/examples/quick/animation/animation.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/animation.qml` & `PyQt6-6.5.0/examples/quick/animation/animation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/basics/color-animation.qml` & `PyQt6-6.5.0/examples/quick/animation/basics/color-animation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/basics/images/face-smile.png` & `PyQt6-6.5.0/examples/quick/animation/basics/images/face-smile.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/basics/images/moon.png` & `PyQt6-6.5.0/examples/quick/animation/basics/images/moon.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/basics/images/sun.png` & `PyQt6-6.5.0/examples/quick/animation/basics/images/sun.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/basics/property-animation.qml` & `PyQt6-6.5.0/examples/quick/animation/basics/property-animation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/behaviors/SideRect.qml` & `PyQt6-6.5.0/examples/quick/animation/behaviors/SideRect.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/behaviors/behavior-example.qml` & `PyQt6-6.5.0/examples/quick/animation/behaviors/behavior-example.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/behaviors/tvtennis.qml` & `PyQt6-6.5.0/examples/quick/animation/behaviors/tvtennis.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/behaviors/wigglytext.qml` & `PyQt6-6.5.0/examples/quick/animation/behaviors/wigglytext.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/easing/easing.qml` & `PyQt6-6.5.0/examples/quick/animation/easing/easing.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/pathanimation/pathanimation.qml` & `PyQt6-6.5.0/examples/quick/animation/pathanimation/pathanimation.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/pathinterpolator/pathinterpolator.qml` & `PyQt6-6.5.0/examples/quick/animation/pathinterpolator/pathinterpolator.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/states/qt-logo.png` & `PyQt6-6.5.0/examples/quick/animation/states/qt-logo.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/states/states.qml` & `PyQt6-6.5.0/examples/quick/animation/states/states.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/animation/states/transitions.qml` & `PyQt6-6.5.0/examples/quick/animation/states/transitions.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/bezierCurve/bezierCurve.qml` & `PyQt6-6.5.0/examples/quick/canvas/bezierCurve/bezierCurve.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/canvas.py` & `PyQt6-6.5.0/examples/quick/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/canvas.qml` & `PyQt6-6.5.0/examples/quick/canvas/canvas.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/clip/clip.qml` & `PyQt6-6.5.0/examples/quick/canvas/clip/clip.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/Button.qml` & `PyQt6-6.5.0/examples/quick/canvas/contents/Button.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/ScrollBar.qml` & `PyQt6-6.5.0/examples/quick/canvas/contents/ScrollBar.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/Slider.qml` & `PyQt6-6.5.0/examples/quick/canvas/contents/Slider.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/TitleBar.qml` & `PyQt6-6.5.0/examples/quick/canvas/contents/TitleBar.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/ToolBar.qml` & `PyQt6-6.5.0/examples/quick/canvas/contents/ToolBar.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/button-pressed.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/button-pressed.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/button.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/button.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/default.svg` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/default.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/gloss.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/gloss.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/lineedit.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/lineedit.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/quit.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/quit.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/titlebar.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/titlebar.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/images/toolbutton.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/images/toolbutton.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/contents/qt-logo.png` & `PyQt6-6.5.0/examples/quick/canvas/contents/qt-logo.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml` & `PyQt6-6.5.0/examples/quick/canvas/quadraticCurveTo/quadraticCurveTo.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/roundedrect/roundedrect.qml` & `PyQt6-6.5.0/examples/quick/canvas/roundedrect/roundedrect.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/smile/smile.qml` & `PyQt6-6.5.0/examples/quick/canvas/smile/smile.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/squircle/squircle.png` & `PyQt6-6.5.0/examples/quick/canvas/squircle/squircle.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/squircle/squircle.qml` & `PyQt6-6.5.0/examples/quick/canvas/squircle/squircle.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/tiger/tiger.js` & `PyQt6-6.5.0/examples/quick/canvas/tiger/tiger.js`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/canvas/tiger/tiger.qml` & `PyQt6-6.5.0/examples/quick/canvas/tiger/tiger.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/models/abstractitemmodel/abstractitemmodel.py` & `PyQt6-6.5.0/examples/quick/models/abstractitemmodel/abstractitemmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/models/abstractitemmodel/view.qml` & `PyQt6-6.5.0/examples/quick/models/abstractitemmodel/view.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/models/objectlistmodel/objectlistmodel.py` & `PyQt6-6.5.0/examples/quick/models/objectlistmodel/objectlistmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/models/objectlistmodel/view.qml` & `PyQt6-6.5.0/examples/quick/models/objectlistmodel/view.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/models/stringlistmodel/stringlistmodel.py` & `PyQt6-6.5.0/examples/quick/models/stringlistmodel/stringlistmodel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/models/stringlistmodel/view.qml` & `PyQt6-6.5.0/examples/quick/models/stringlistmodel/view.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/scenegraph/customgeometry/customgeometry.py` & `PyQt6-6.5.0/examples/quick/scenegraph/customgeometry/customgeometry.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/scenegraph/customgeometry/main.qml` & `PyQt6-6.5.0/examples/quick/scenegraph/customgeometry/main.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/shared/Button.qml` & `PyQt6-6.5.0/examples/quick/shared/Button.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/shared/LauncherList.qml` & `PyQt6-6.5.0/examples/quick/shared/LauncherList.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/shared/SimpleLauncherDelegate.qml` & `PyQt6-6.5.0/examples/quick/shared/SimpleLauncherDelegate.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/shared/images/back.png` & `PyQt6-6.5.0/examples/quick/shared/images/back.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/shared/images/next.png` & `PyQt6-6.5.0/examples/quick/shared/images/next.png`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter1-basics/app.qml` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter1-basics/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter1-basics/chapter1-basics.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter2-methods/app.qml` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter2-methods/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter2-methods/chapter2-methods.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter3-bindings/app.qml` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter3-bindings/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter3-bindings/chapter3-bindings.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter4-customPropertyTypes/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter4-customPropertyTypes/chapter4-customPropertyTypes.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter5-listproperties/app.qml` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter5-listproperties/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter5-listproperties/chapter5-listproperties.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/chartsplugin.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/piechart.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/Charts/pieslice.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/quick/tutorials/extending/chapter6-plugins/app.qml` & `PyQt6-6.5.0/examples/quick/tutorials/extending/chapter6-plugins/app.qml`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/richtext/textobject/heart.svg` & `PyQt6-6.5.0/examples/richtext/textobject/heart.svg`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/examples/richtext/textobject/textobject.py` & `PyQt6-6.5.0/examples/richtext/textobject/textobject.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/__init__.py` & `PyQt6-6.5.0/lupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/designer_source.py` & `PyQt6-6.5.0/lupdate/designer_source.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/lupdate.py` & `PyQt6-6.5.0/lupdate/lupdate.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/pylupdate.py` & `PyQt6-6.5.0/lupdate/pylupdate.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/python_source.py` & `PyQt6-6.5.0/lupdate/python_source.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/source_file.py` & `PyQt6-6.5.0/lupdate/source_file.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/translation_file.py` & `PyQt6-6.5.0/lupdate/translation_file.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/translations.py` & `PyQt6-6.5.0/lupdate/translations.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/lupdate/user.py` & `PyQt6-6.5.0/lupdate/user.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/project.py` & `PyQt6-6.5.0/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         # QtLocation is still to be ported to Qt6.
         self.bindings_factories = [QtCore, QtNetwork, QtGui, QtQml, QtWidgets,
                 QtDBus, QtDesigner, QtHelp, QtOpenGL, QtOpenGLWidgets,
                 QtPrintSupport, QtQuick, QtQuick3D, QtQuickWidgets, QtSql,
                 QtSvg, QtSvgWidgets, QtTest, QtXml, QtMultimedia,
                 QtMultimediaWidgets, QtPositioning, QtRemoteObjects, QtSensors,
                 QtSerialPort, QtWebChannel, QtWebSockets, QtBluetooth, QtNfc,
-                QtPdf, QtPdfWidgets, QtTextToSpeech, QAxContainer]
+                QtPdf, QtPdfWidgets, QtSpatialAudio, QtTextToSpeech,
+                QAxContainer]
 
     def apply_user_defaults(self, tool):
         """ Set default values where needed. """
 
         if self.license_dir is None:
             self.license_dir = os.path.join(self.root_dir, 'sip')
         else:
@@ -765,14 +766,25 @@
         """ Initialise the bindings. """
 
         super().__init__(project, 'QtSerialPort', qmake_QT=['serialport'],
                 test_headers=['qserialport.h'],
                 test_statement='new QSerialPort()')
 
 
+class QtSpatialAudio(PyQtBindings):
+    """ The QtSpatialAudio bindings. """
+
+    def __init__(self, project):
+        """ Initialise the bindings. """
+
+        super().__init__(project, 'QtSpatialAudio', qmake_QT=['spatialaudio'],
+                test_headers=['qaudioengine.h'],
+                test_statement='new QAudioEngine()')
+
+
 class QtSql(PyQtBindings):
     """ The QtSql bindings. """
 
     def __init__(self, project):
         """ Initialise the bindings. """
 
         super().__init__(project, 'QtSql', qmake_QT=['sql', 'widgets'],
```

### Comparing `PyQt6-6.4.2/pyproject.toml` & `PyQt6-6.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Specify the build system for the project.
 [build-system]
-requires = ["sip >=6.5, <7", "PyQt-builder >=1.11, <2"]
+requires = ["sip >=6.5, <7", "PyQt-builder >=1.15, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6"
-version = "6.4.2"
+version = "6.5.0"
 summary = "Python bindings for the Qt cross platform application toolkit"
 home-page = "https://www.riverbankcomputing.com/software/pyqt/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-python = ">=3.6.1"
```

### Comparing `PyQt6-6.4.2/qmlscene/pluginloader.cpp` & `PyQt6-6.5.0/qmlscene/pluginloader.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qmlscene/pluginloader.h` & `PyQt6-6.5.0/qmlscene/pluginloader.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_api.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_chimera.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_chimera.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 #include "qpycore_pyqtpyobject.h"
 #include "qpycore_types.h"
 
 #include "sipAPIQtCore.h"
 
 
 // The registered user-defined Python enum types.
-QSet<PyObject *> Chimera::_py_enum_types;
+QHash<PyObject *, QByteArray> Chimera::_py_enum_types;
 
 // The cache of previously parsed argument type lists.
 QHash<QByteArray, QList<const Chimera *> > Chimera::_previously_parsed;
 
 // The registered QVariant to PyObject convertors.
 Chimera::FromQVariantConvertors Chimera::registeredFromQVariantConvertors;
 
@@ -154,19 +154,21 @@
 // Destroy the type.
 Chimera::~Chimera()
 {
     Py_XDECREF((PyObject *)_py_type);
 }
 
 
-// Register the type of a user-defined Python enum.
-void Chimera::registerPyEnum(PyObject *enum_type)
+// Register the type and pseudo fully qualified C++ name of a user-defined
+// Python enum.
+void Chimera::registerPyEnum(PyObject *enum_type,
+        const QByteArray &cpp_qualname)
 {
     Py_INCREF(enum_type);
-    _py_enum_types.insert(enum_type);
+    _py_enum_types.insert(enum_type, cpp_qualname);
 }
 
 
 // Parse an object as a type.
 const Chimera *Chimera::parse(PyObject *obj)
 {
     Chimera *ct = new Chimera;
@@ -518,15 +520,17 @@
                 }
             }
         }
     }
     else if (_py_enum_types.contains((PyObject *)type_obj))
     {
         metatype = QMetaType(QMetaType::Int);
-        _name = sipPyTypeName(type_obj);
+
+        // Note that we use the fully qualified name.
+        _name = _py_enum_types.value((PyObject *)type_obj);
     }
     else if (type_obj == &PyList_Type)
     {
         metatype = QMetaType(QMetaType::QVariantList);
     }
     else if (type_obj == &PyUnicode_Type)
     {
@@ -822,20 +826,19 @@
 
     case QMetaType::Bool:
         *reinterpret_cast<bool *>(cpp) = PyLong_AsLong(py);
         break;
 
     case QMetaType::Int:
         {
-            int ival = PyLong_AsLong(py);
-
             if (isEnumOrFlag())
-                *reinterpret_cast<QVariant *>(cpp) = QVariant(ival);
+                *reinterpret_cast<QVariant *>(cpp) = QVariant(
+                        get_enum_value(py));
             else
-                *reinterpret_cast<int *>(cpp) = ival;
+                *reinterpret_cast<int *>(cpp) = PyLong_AsLong(py);
 
             break;
         }
 
     case QMetaType::UInt:
         *reinterpret_cast<unsigned int *>(cpp) = sipLong_AsUnsignedLong(py);
         break;
@@ -1120,18 +1123,17 @@
         break;
 
     case QMetaType::Bool:
         tmp_storage.tmp_bool = PyLong_AsLong(py);
         break;
 
     case QMetaType::Int:
-        if (_type && sipTypeIsEnum(_type))
+        if (isEnumOrFlag())
         {
-            // Note that this will be an unregistered enum.
-            tmp_storage.tmp_int = sipConvertToEnum(py, _type);
+            tmp_storage.tmp_int = get_enum_value(py);
         }
         else if (_inexact)
         {
             // Fit it into the smallest C++ type we can.
 
             qlonglong qll = PyLong_AsLongLong(py);
 
@@ -1469,19 +1471,25 @@
 
             return variant_map.fromMappedType(&qvm);
         }
 
         // A sanity check.
         if (metatype != var.metaType())
         {
-            PyErr_Format(PyExc_TypeError,
-                    "unable to convert a QVariant of type %d to a QMetaType of type %d",
-                    var.metaType().id(), metatype.id());
+            // However having an Int QVariant value and having an invalid
+            // QMetaType is the case that we are dealing with a user-defined
+            // enum and so is valid.
+            if (!(var.metaType().id() == QMetaType::Int && metatype.id() == QMetaType::UnknownType))
+            {
+                PyErr_Format(PyExc_TypeError,
+                        "unable to convert a QVariant of type %d to a QMetaType of type %d",
+                        var.metaType().id(), metatype.id());
 
-            return 0;
+                return 0;
+            }
         }
 
         // Deal with the simple case of unwrapping a Python object rather than
         // converting it.
         if (metatype == QMetaType::fromType<PyQt_PyObject>())
         {
             PyQt_PyObject pyobj_wrapper = var.value<PyQt_PyObject>();
@@ -1553,32 +1561,36 @@
         return pyobj_wrapper->pyobject;
     }
 
     PyObject *py = 0;
 
     switch (metatype.id())
     {
+    case QMetaType::UnknownType:
+        // In invalid QMetaType probably means a user-defined enum.
+        py = get_enum_key(*reinterpret_cast<int *>(cpp));
+        break;
+
     case QMetaType::Nullptr:
         py = Py_None;
         Py_INCREF(py);
         break;
 
     case QMetaType::Bool:
         py = PyBool_FromLong(*reinterpret_cast<bool *>(cpp));
         break;
 
     case QMetaType::Int:
-        if (_type && sipTypeIsEnum(_type))
+        if (_is_qflags)
         {
-            // Note that this will be an unregistered enum.
-            py = sipConvertFromEnum(*reinterpret_cast<int *>(cpp), _type);
+            py = sipConvertFromType(cpp, _type, 0);
         }
-        else if (_is_qflags)
+        else if (isEnumOrFlag())
         {
-            py = sipConvertFromType(cpp, _type, 0);
+            py = get_enum_key(*reinterpret_cast<int *>(cpp));
         }
         else
         {
             py = PyLong_FromLong(*reinterpret_cast<int *>(cpp));
         }
 
         break;
@@ -1814,14 +1826,67 @@
     if (_is_qflags)
         return true;
 
     return (_py_type ? _py_enum_types.contains((PyObject *)_py_type) : false);
 }
 
 
+// Return the value of an enum, either a wrapped one or a user-defined one.
+int Chimera::get_enum_value(PyObject *py) const
+{
+    int value = 0;
+
+    if (_type)
+    {
+        value = sipConvertToEnum(py, _type);
+    }
+    else
+    {
+        PyObject *value_obj = PyObject_GetAttrString(py, "value");
+
+        if (value_obj)
+        {
+            value = PyLong_AsLong(value_obj);
+            Py_DECREF(value_obj);
+        }
+    }
+
+    return value;
+}
+
+
+// Return the key of an enum, either a wrapped one or a user-defined one.
+PyObject *Chimera::get_enum_key(int cpp) const
+{
+    PyObject *py = NULL;
+
+    if (_type)
+    {
+        py = sipConvertFromEnum(cpp, _type);
+    }
+    else
+    {
+        QHashIterator<PyObject *, QByteArray> it(_py_enum_types);
+
+        while (it.hasNext())
+        {
+            it.next();
+
+            if (it.value() == _name)
+            {
+                py = PyObject_CallFunction(it.key(), "(i)", cpp);
+                break;
+            }
+        }
+    }
+
+    return py;
+}
+
+
 // Convert a Python object to C++, allocating storage as necessary.
 Chimera::Storage *Chimera::fromPyObjectToStorage(PyObject *py) const
 {
     Chimera::Storage *st = new Chimera::Storage(this, py);
 
     if (!st->isValid())
     {
```

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_chimera.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_chimera.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 #include <Python.h>
 
 #include <QByteArray>
 #include <QHash>
 #include <QList>
 #include <QMetaType>
 #include <QMetaProperty>
-#include <QSet>
 #include <QVariant>
 
 #include "sipAPIQtCore.h"
 
 
 // This describes a type that can be understood by Python and C++ (specifically
 // Qt's meta-type system).  The implementation assumes that the GIL is held.
@@ -220,15 +219,16 @@
     // Returns true if the type is a C++ or Python enum or flag.
     bool isEnumOrFlag() const;
 
     // Returns the SIP generated type structure.
     const sipTypeDef *typeDef() const {return _type;}
 
     // Register a type as a Python enum.
-    static void registerPyEnum(PyObject *enum_type);
+    static void registerPyEnum(PyObject *enum_type,
+            const QByteArray &cpp_qualname);
 
     // The Qt meta-type.
     QMetaType metatype;
 
     // The type identifer.  This will be the meta-type identifier or -1 if the
     // type is char *.
     int typeId() const {return _is_char_star ? -1 : metatype.id();}
@@ -250,16 +250,16 @@
 
     // The C++ name of the type.
     QByteArray _name;
 
     // Set if the C++ type is char *.  This needs special handling.
     bool _is_char_star;
 
-    // The registered int types.
-    static QSet<PyObject *> _py_enum_types;
+    // The registered user-defined enums.
+    static QHash<PyObject *, QByteArray> _py_enum_types;
 
     // The cache of previously parsed argument type lists.
     static QHash<QByteArray, QList<const Chimera *> > _previously_parsed;
 
     Chimera();
 
     bool parse_cpp_type(const QByteArray &type);
@@ -269,13 +269,15 @@
     static bool to_char16_t(PyObject *py, char16_t &cpp);
     static bool to_char32_t(PyObject *py, char32_t &cpp);
     static void raiseParseCppException(const char *type,
             const char *context = 0);
     static QVariant keep_as_pyobject(PyObject *py);
     static int extract_raw_type(const QByteArray &type, QByteArray &raw_type);
     static QByteArray resolve_types(const QByteArray &type);
+    int get_enum_value(PyObject *py) const;
+    PyObject *get_enum_key(int cpp) const;
 
     Chimera &operator=(const Chimera &);
 };
 
 
 #endif
```

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_chimera_signature.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_chimera_signature.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_chimera_storage.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_chimera_storage.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_classinfo.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_classinfo.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_classinfo.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_classinfo.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_decorators.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_decorators.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_enums_flags.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_enums_flags.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -108,16 +108,31 @@
     bool ok = parse_members(members, enum_flag);
 
     Py_DECREF(members);
 
     if (!ok)
         return 0;
 
+    // Get the pseudo fully qualified C++ name.
+    static PyObject *qualname_s = 0;
+
+    if (!objectify("__qualname__", &qualname_s))
+        return 0;
+
+    PyObject *qualname = PyObject_GetAttr(enum_cls, qualname_s);
+    if (!qualname)
+        return 0;
+
+    QByteArray cpp_qualname = qpycore_convert_ASCII(qualname);
+    Py_DECREF(qualname);
+
+    cpp_qualname.replace(QByteArray("."), QByteArray("::"));
+
     // Register the enum with our type system.
-    Chimera::registerPyEnum(enum_cls);
+    Chimera::registerPyEnum(enum_cls, cpp_qualname);
 
     // Save the parsed enum for later.
     Py_INCREF(enum_cls);
     enums_hash.insert(enum_cls, enum_flag);
 
     // Return the enum class.
     Py_INCREF(enum_cls);
```

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_enums_flags.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_enums_flags.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_event_handlers.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_event_handlers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_event_handlers.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_event_handlers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_init.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_misc.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_misc.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_misc.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_misc.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_namespace.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_namespace.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_objectified_strings.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_objectified_strings.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_post_init.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_public_api.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_public_api.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_public_api.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_public_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtboundsignal.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtboundsignal.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -949,16 +949,19 @@
             continue;
 
         for (int a = 0; a < slot_nr_args; ++a)
         {
             const Chimera *sig_arg = signal->parsed_arguments.at(a);
             const Chimera *slot_arg = slot->parsed_arguments.at(a);
 
-            // We simply compare meta-types.
-            if (sig_arg->metatype != slot_arg->metatype)
+            // We simply compare the C++ names. We used to compare meta-types
+            // but this is unreliable as the signal's type may have been
+            // registered by Qt internally (and so given a new meta-type) after
+            // the slot was defined (and has the meta-type of PyQt_PyObject).
+            if (sig_arg->name() != slot_arg->name())
             {
                 slot = 0;
                 break;
             }
         }
 
         // If all of the slot's arguments were Ok then this will be the best
```

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtboundsignal.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtboundsignal.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtconfigure.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtconfigure.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmethodproxy.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmethodproxy.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmethodproxy.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmethodproxy.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmutexlocker.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmutexlocker.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtmutexlocker.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtmutexlocker.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtproperty.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtproperty.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtproperty.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtproperty.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtpyobject.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtpyobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtpyobject.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtpyobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtsignal.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtsignal.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtsignal.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtsignal.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslot.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslot.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslot.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslot.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslotproxy.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslotproxy.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_pyqtslotproxy.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_pyqtslotproxy.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qjsonvalue.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qjsonvalue.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qmessagelogger.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qmessagelogger.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qmetaobject.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qmetaobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qmetaobject_helpers.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qmetaobject_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qmetaobjectbuilder.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qmetaobjectbuilder.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qobject_getattr.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qobject_getattr.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qobject_helpers.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qobject_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qobject_helpers.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qobject_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qstring.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qstring.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qt_conf.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qt_conf.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qvariant.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qvariant.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_qvariant_value.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_qvariant_value.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_types.cpp` & `PyQt6-6.5.0/qpy/QtCore/qpycore_types.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,20 @@
             }
         }
         else
         {
             prop_type = pp->pyqtprop_parsed_type->name();
         }
 
+        // Note that there is an addProperty() overload that also takes a
+        // QMetaType argument (rather than call QMetaType::fromType() as this
+        // overload does) so we could pass the QMetaType that the parser
+        // created.  However this breaks properties that are application Python
+        // enums which have a parsed QMetaType that describes an int whereas Qt
+        // seems to need an invalid QMetaType for these to work.
         QMetaPropertyBuilder prop_builder = builder.addProperty(
                 QByteArray(prop_name), prop_type, notifier_id);
 
         // Reset the defaults.
         prop_builder.setReadable(false);
         prop_builder.setWritable(false);
```

### Comparing `PyQt6-6.4.2/qpy/QtCore/qpycore_types.h` & `PyQt6-6.5.0/qpy/QtCore/qpycore_types.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbus_api.h` & `PyQt6-6.5.0/qpy/QtDBus/qpydbus_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbus_chimera_helpers.cpp` & `PyQt6-6.5.0/qpy/QtDBus/qpydbus_chimera_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbus_chimera_helpers.h` & `PyQt6-6.5.0/qpy/QtDBus/qpydbus_chimera_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbus_post_init.cpp` & `PyQt6-6.5.0/qpy/QtDBus/qpydbus_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbuspendingreply.cpp` & `PyQt6-6.5.0/qpy/QtDBus/qpydbuspendingreply.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbuspendingreply.h` & `PyQt6-6.5.0/qpy/QtDBus/qpydbuspendingreply.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbusreply.cpp` & `PyQt6-6.5.0/qpy/QtDBus/qpydbusreply.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDBus/qpydbusreply.h` & `PyQt6-6.5.0/qpy/QtDBus/qpydbusreply.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDesigner/qpydesignercontainerextension.h` & `PyQt6-6.5.0/qpy/QtDesigner/qpydesignercontainerextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h` & `PyQt6-6.5.0/qpy/QtDesigner/qpydesignercustomwidgetcollectionplugin.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDesigner/qpydesignercustomwidgetplugin.h` & `PyQt6-6.5.0/qpy/QtDesigner/qpydesignercustomwidgetplugin.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDesigner/qpydesignermembersheetextension.h` & `PyQt6-6.5.0/qpy/QtDesigner/qpydesignermembersheetextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDesigner/qpydesignerpropertysheetextension.h` & `PyQt6-6.5.0/qpy/QtDesigner/qpydesignerpropertysheetextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtDesigner/qpydesignertaskmenuextension.h` & `PyQt6-6.5.0/qpy/QtDesigner/qpydesignertaskmenuextension.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_add_constants.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_add_constants.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_api.h` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_array_convertors.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_array_convertors.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_attribute_array.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_attribute_array.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_data_cache.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_data_cache.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_data_cache.h` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_data_cache.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_get.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_get.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_init.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_misc.h` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_misc.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_uniform_value_array.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_value_array.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_value_array.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtOpenGL/qpyopengl_version_functions.cpp` & `PyQt6-6.5.0/qpy/QtOpenGL/qpyopengl_version_functions.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_api.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_listdata.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_listdata.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_listdata.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_listdata.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_post_init.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_qjsvalue.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_qjsvalue.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_register_singleton_type.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_register_singleton_type.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqml_register_type.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqml_register_type.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmllistproperty.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqmllistproperty.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmllistproperty.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqmllistproperty.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmllistpropertywrapper.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqmllistpropertywrapper.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmllistpropertywrapper.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqmllistpropertywrapper.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmlobject.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqmlobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmlobject.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqmlobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmlsingletonobject.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqmlsingletonobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmlsingletonobject.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqmlsingletonobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmlvalidator.cpp` & `PyQt6-6.5.0/qpy/QtQml/qpyqmlvalidator.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQml/qpyqmlvalidator.h` & `PyQt6-6.5.0/qpy/QtQml/qpyqmlvalidator.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquick_api.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquick_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquick_chimera_helpers.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquick_chimera_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquick_chimera_helpers.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquick_chimera_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquick_post_init.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquick_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquick_register_type.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquick_register_type.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquick_register_type.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquick_register_type.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickframebufferobject.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickframebufferobject.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickframebufferobject.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickframebufferobject.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickitem.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickitem.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickitem.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickitem.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickpainteditem.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickpainteditem.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickpainteditem.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickpainteditem.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickview.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickview.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickview.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickview.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickwindow.cpp` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickwindow.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtQuick/qpyquickwindow.h` & `PyQt6-6.5.0/qpy/QtQuick/qpyquickwindow.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_api.h` & `PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_api.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp` & `PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_chimera_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_chimera_helpers.h` & `PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_chimera_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_post_init.cpp` & `PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_post_init.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp` & `PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_qaction_helpers.cpp`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/qpy/QtWidgets/qpywidgets_qaction_helpers.h` & `PyQt6-6.5.0/qpy/QtWidgets/qpywidgets_qaction_helpers.h`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QAxContainer/QAxContainermod.sip` & `PyQt6-6.5.0/sip/QAxContainer/QAxContainermod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QAxContainer/qaxbase.sip` & `PyQt6-6.5.0/sip/QAxContainer/qaxbase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QAxContainer/qaxobject.sip` & `PyQt6-6.5.0/sip/QAxContainer/qaxobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QAxContainer/qaxobjectinterface.sip` & `PyQt6-6.5.0/sip/QAxContainer/qaxobjectinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QAxContainer/qaxwidget.sip` & `PyQt6-6.5.0/sip/QAxContainer/qaxwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/QtBluetoothmod.sip` & `PyQt6-6.5.0/sip/QtBluetooth/QtBluetoothmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetooth.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetooth.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothaddress.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothaddress.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothdevicediscoveryagent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothdeviceinfo.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothdeviceinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothhostinfo.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothhostinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothlocaldevice.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothlocaldevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothserver.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothservicediscoveryagent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothserviceinfo.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothserviceinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothsocket.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qbluetoothuuid.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qbluetoothuuid.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergyadvertisingdata.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergyadvertisingdata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergyadvertisingparameters.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergyadvertisingparameters.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergycharacteristic.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergycharacteristic.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergycharacteristicdata.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergycharacteristicdata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergyconnectionparameters.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergyconnectionparameters.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergycontroller.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergycontroller.sip`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         ConnectionError,
         AdvertisingError,
         RemoteHostClosedError,
         AuthorizationError,
 %If (Qt_6_4_0 -)
         MissingPermissionsError,
 %End
+%If (Qt_6_5_0 -)
+        RssiReadError,
+%End
     };
 
     enum ControllerState
     {
         UnconnectedState,
         ConnectingState,
         ConnectedState,
@@ -101,14 +104,22 @@
     static QLowEnergyController *createPeripheral(QObject *parent /TransferThis/ = 0) /Factory/;
     void startAdvertising(const QLowEnergyAdvertisingParameters &parameters, const QLowEnergyAdvertisingData &advertisingData, const QLowEnergyAdvertisingData &scanResponseData = QLowEnergyAdvertisingData());
     void stopAdvertising();
     QLowEnergyService *addService(const QLowEnergyServiceData &service, QObject *parent /TransferThis/ = 0) /Factory/;
     void requestConnectionUpdate(const QLowEnergyConnectionParameters &parameters);
     QLowEnergyController::Role role() const;
     QBluetoothUuid remoteDeviceUuid() const;
+%If (Qt_6_5_0 -)
+    void readRssi();
+%End
+
+signals:
+%If (Qt_6_5_0 -)
+    void rssiRead(qint16 rssi);
+%End
 
 private:
     QLowEnergyController(const QBluetoothDeviceInfo &remoteDevice, const QBluetoothAddress &localDevice, QObject *parent = 0);
     QLowEnergyController(const QBluetoothAddress &localDevice, QObject *parent = 0);
 };
 
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergydescriptor.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergydescriptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergydescriptordata.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergydescriptordata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergyservice.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergyservice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qlowenergyservicedata.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qlowenergyservicedata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qpybluetooth_qlist.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qpybluetooth_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qpybluetooth_qmultihash.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qpybluetooth_qmultihash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtBluetooth/qpybluetooth_quint128.sip` & `PyQt6-6.5.0/sip/QtBluetooth/qpybluetooth_quint128.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/QtCoremod.sip` & `PyQt6-6.5.0/sip/QtCore/QtCoremod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 %Module(name=PyQt6.QtCore, call_super_init=True, default_VirtualErrorHandler=PyQt6, keyword_arguments="Optional", use_limited_api=True, py_ssize_t_clean=True)
 
-%Timeline {Qt_6_0_0 Qt_6_1_0 Qt_6_2_0 Qt_6_3_0 Qt_6_4_0}
+%Timeline {Qt_6_0_0 Qt_6_1_0 Qt_6_2_0 Qt_6_3_0 Qt_6_4_0 Qt_6_5_0}
 
 %Platforms {Android iOS Linux macOS WebAssembly Windows}
 
 %Feature PyQt_Accessibility
 %Feature PyQt_SessionManager
 %Feature PyQt_SSL
 %Feature PyQt_qreal_double
@@ -70,19 +70,21 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_VERSION;
 const char *PYQT_VERSION_STR;
 
 %ModuleCode
-static int PYQT_VERSION = 0x060402;
-static const char *PYQT_VERSION_STR = "6.4.2";
+static int PYQT_VERSION = 0x060500;
+static const char *PYQT_VERSION_STR = "6.5.0";
 %End
 
 %Include qglobal.sip
+%Include qtenvironmentvariables.sip
+%Include qtversion.sip
 %Include qnamespace.sip
 %Include qabstractanimation.sip
 %Include qabstracteventdispatcher.sip
 %Include qabstractitemmodel.sip
 %Include qabstractnativeeventfilter.sip
 %Include qabstractproxymodel.sip
 %Include qanimationgroup.sip
@@ -177,14 +179,15 @@
 %Include qthread.sip
 %Include qthreadpool.sip
 %Include qtimeline.sip
 %Include qtimer.sip
 %Include qtimezone.sip
 %Include qtranslator.sip
 %Include qtransposeproxymodel.sip
+%Include qtypes.sip
 %Include qurl.sip
 %Include qurlquery.sip
 %Include quuid.sip
 %Include qvariant.sip
 %Include qvariantanimation.sip
 %Include qversionnumber.sip
 %Include qwaitcondition.sip
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qabstractanimation.sip` & `PyQt6-6.5.0/sip/QtCore/qabstractanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qabstracteventdispatcher.sip` & `PyQt6-6.5.0/sip/QtCore/qabstracteventdispatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qabstractitemmodel.sip` & `PyQt6-6.5.0/sip/QtCore/qabstractitemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qabstractnativeeventfilter.sip` & `PyQt6-6.5.0/sip/QtCore/qabstractnativeeventfilter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qabstractproxymodel.sip` & `PyQt6-6.5.0/sip/QtCore/qabstractproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qanimationgroup.sip` & `PyQt6-6.5.0/sip/QtCore/qanimationgroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qanystringview.sip` & `PyQt6-6.5.0/sip/QtCore/qanystringview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qbasictimer.sip` & `PyQt6-6.5.0/sip/QtCore/qbasictimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qbitarray.sip` & `PyQt6-6.5.0/sip/QtCore/qbitarray.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qbuffer.sip` & `PyQt6-6.5.0/sip/QtCore/qbuffer.sip`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,20 @@
     explicit QBuffer(QObject *parent /TransferThis/ = 0);
     QBuffer(QByteArray *byteArray /Constrained/, QObject *parent /TransferThis/ = 0);
     virtual ~QBuffer();
     QByteArray &buffer();
     const QByteArray &data() const;
     void setBuffer(QByteArray *a /Constrained/);
     void setData(const QByteArray &data);
+%If (- Qt_6_5_0)
     void setData(const char *adata /Array/, int alen /ArraySize/);
+%End
+%If (Qt_6_5_0 -)
+    void setData(const char *data /Array/, qsizetype len /ArraySize/);
+%End
     virtual bool open(QIODeviceBase::OpenMode openMode);
     virtual void close();
     virtual qint64 size() const;
     virtual qint64 pos() const;
     virtual bool seek(qint64 off);
     virtual bool atEnd() const;
     virtual bool canReadLine() const;
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qbytearray.sip` & `PyQt6-6.5.0/sip/QtCore/qbytearray.sip`

 * *Files 2% similar despite different names*

```diff
@@ -411,23 +411,37 @@
     QByteArray sliced(qsizetype pos, qsizetype n) const;
 %If (Qt_6_3_0 -)
     bool isValidUtf8() const;
 %End
 %If (Qt_6_4_0 -)
     QByteArray percentDecoded(char percent = '%') const;
 %End
+%If (Qt_6_5_0 -)
+    QByteArray &removeAt(qsizetype pos);
+%End
+%If (Qt_6_5_0 -)
+    QByteArray &removeFirst();
+%End
+%If (Qt_6_5_0 -)
+    QByteArray &removeLast();
+%End
 };
 
 bool operator==(const QByteArray &a1, const QByteArray &a2);
 bool operator!=(const QByteArray &a1, const QByteArray &a2);
 bool operator<(const QByteArray &a1, const QByteArray &a2);
 bool operator<=(const QByteArray &a1, const QByteArray &a2);
 bool operator>(const QByteArray &a1, const QByteArray &a2);
 bool operator>=(const QByteArray &a1, const QByteArray &a2);
+%If (Qt_6_5_0 -)
+QByteArray operator+(const QByteArray &a1, const QByteArray &a2);
+%End
+%If (- Qt_6_5_0)
 const QByteArray operator+(const QByteArray &a1, const QByteArray &a2);
+%End
 QDataStream &operator<<(QDataStream &, const QByteArray & /Constrained/) /ReleaseGIL/;
 QDataStream &operator>>(QDataStream &, QByteArray & /Constrained/) /ReleaseGIL/;
 QByteArray qCompress(const uchar *data /Array/, qsizetype nbytes /ArraySize/, int compressionLevel = -1);
 QByteArray qCompress(const QByteArray &data, int compressionLevel = -1);
 QByteArray qUncompress(const uchar *data /Array/, qsizetype nbytes /ArraySize/);
 QByteArray qUncompress(const QByteArray &data);
 %If (- Qt_6_2_0)
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qbytearrayalgorithms.sip` & `PyQt6-6.5.0/sip/QtCore/qbytearrayalgorithms.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qbytearraylist.sip` & `PyQt6-6.5.0/sip/QtCore/qbytearraylist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qbytearraymatcher.sip` & `PyQt6-6.5.0/sip/QtCore/qbytearraymatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qbytearrayview.sip` & `PyQt6-6.5.0/sip/QtCore/qbytearrayview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcalendar.sip` & `PyQt6-6.5.0/sip/QtCore/qcalendar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcborcommon.sip` & `PyQt6-6.5.0/sip/QtCore/qcborcommon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcborstreamreader.sip` & `PyQt6-6.5.0/sip/QtCore/qcborstreamreader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcborstreamwriter.sip` & `PyQt6-6.5.0/sip/QtCore/qcborstreamwriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qchar.sip` & `PyQt6-6.5.0/sip/QtCore/qchar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcollator.sip` & `PyQt6-6.5.0/sip/QtCore/qcollator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcommandlineoption.sip` & `PyQt6-6.5.0/sip/QtCore/qcommandlineoption.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcommandlineparser.sip` & `PyQt6-6.5.0/sip/QtCore/qcommandlineparser.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qconcatenatetablesproxymodel.sip` & `PyQt6-6.5.0/sip/QtCore/qconcatenatetablesproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcoreapplication.sip` & `PyQt6-6.5.0/sip/QtCore/qcoreapplication.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcoreevent.sip` & `PyQt6-6.5.0/sip/QtCore/qcoreevent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qcryptographichash.sip` & `PyQt6-6.5.0/sip/QtCore/qcryptographichash.sip`

 * *Files 6% similar despite different names*

```diff
@@ -72,11 +72,20 @@
 %If (Qt_6_3_0 -)
     static QByteArray hash(QByteArrayView data, QCryptographicHash::Algorithm method);
 %End
 %If (- Qt_6_3_0)
     static QByteArray hash(const QByteArray &data, QCryptographicHash::Algorithm method);
 %End
     static int hashLength(QCryptographicHash::Algorithm method);
+%If (Qt_6_5_0 -)
+    void swap(QCryptographicHash &other /Constrained/);
+%End
+%If (Qt_6_5_0 -)
+    QCryptographicHash::Algorithm algorithm() const;
+%End
+%If (Qt_6_5_0 -)
+    static bool supportsAlgorithm(QCryptographicHash::Algorithm method);
+%End
 
 private:
     QCryptographicHash(const QCryptographicHash &);
 };
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qdatastream.sip` & `PyQt6-6.5.0/sip/QtCore/qdatastream.sip`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 %End
 %If (Qt_6_3_0 -)
         Qt_6_3,
 %End
 %If (Qt_6_4_0 -)
         Qt_6_4,
 %End
+%If (Qt_6_5_0 -)
+        Qt_6_5,
+%End
     };
 
     enum ByteOrder
     {
         BigEndian,
         LittleEndian,
     };
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qdatetime.sip` & `PyQt6-6.5.0/sip/QtCore/qdatetime.sip`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,17 @@
     QDateTime addMSecs(qint64 msecs) const;
     QDateTime toTimeSpec(Qt::TimeSpec spec) const;
     QDateTime toLocalTime() const;
     QDateTime toUTC() const;
     qint64 daysTo(const QDateTime &) const;
     qint64 secsTo(const QDateTime &) const;
     static QDateTime currentDateTime();
+%If (Qt_6_5_0 -)
+    static QDateTime currentDateTime(const QTimeZone &zone);
+%End
     static QDateTime fromString(const QString &string, Qt::DateFormat format = Qt::TextDate);
     qint64 toMSecsSinceEpoch() const;
     void setMSecsSinceEpoch(qint64 msecs);
     qint64 msecsTo(const QDateTime &) const;
     static QDateTime currentDateTimeUtc();
     static qint64 currentMSecsSinceEpoch();
     void swap(QDateTime &other /Constrained/);
@@ -429,14 +432,17 @@
         Last,
     };
 
     void setDate(QDate date);
     void setTime(QTime time);
     QString toString(const QString &format, QCalendar cal = QCalendar()) const;
     static QDateTime fromString(const QString &string, const QString &format, QCalendar cal = QCalendar());
+%If (Qt_6_5_0 -)
+    QTimeZone timeRepresentation() const;
+%End
 };
 
 QDataStream &operator<<(QDataStream &, QDate) /ReleaseGIL/;
 QDataStream &operator>>(QDataStream &, QDate & /Constrained/) /ReleaseGIL/;
 QDataStream &operator<<(QDataStream &, QTime) /ReleaseGIL/;
 QDataStream &operator>>(QDataStream &, QTime & /Constrained/) /ReleaseGIL/;
 QDataStream &operator<<(QDataStream &, const QDateTime &) /ReleaseGIL/;
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qdeadlinetimer.sip` & `PyQt6-6.5.0/sip/QtCore/qdeadlinetimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qdir.sip` & `PyQt6-6.5.0/sip/QtCore/qdir.sip`

 * *Files 4% similar despite different names*

```diff
@@ -86,25 +86,48 @@
     bool cdUp();
     QStringList nameFilters() const;
     void setNameFilters(const QStringList &nameFilters);
     QDir::Filters filter() const;
     void setFilter(QDir::Filters filter);
     QDir::SortFlags sorting() const;
     void setSorting(QDir::SortFlags sort);
+%If (Qt_6_5_0 -)
+    qsizetype count() const /__len__/;
+%MethodCode
+        sipRes = sipCpp->count(Qt::Disambiguated);
+%End
+
+%End
+%If (- Qt_6_5_0)
     uint count() const /__len__/;
+%End
+%If (Qt_6_5_0 -)
+    QString operator[](qsizetype) const;
+%MethodCode
+        Py_ssize_t idx = sipConvertFromSequenceIndex(a0, sipCpp->count());
+        
+        if (idx < 0)
+            sipIsErr = 1;
+        else
+            sipRes = new QString(sipCpp->operator[]((qsizetype)idx));
+%End
+
+%End
+%If (- Qt_6_5_0)
     QString operator[](int) const;
 %MethodCode
         Py_ssize_t idx = sipConvertFromSequenceIndex(a0, sipCpp->count());
         
         if (idx < 0)
             sipIsErr = 1;
         else
             sipRes = new QString(sipCpp->operator[]((int)idx));
 %End
 
+%End
     QStringList operator[](SIP_PYSLICE) const;
 %MethodCode
         Py_ssize_t start, stop, step, slicelength;
         
         if (sipConvertFromSliceObject(a0, sipCpp->count(), &start, &stop, &step, &slicelength) < 0)
         {
             sipIsErr = 1;
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qdiriterator.sip` & `PyQt6-6.5.0/sip/QtCore/qdiriterator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qeasingcurve.sip` & `PyQt6-6.5.0/sip/QtCore/qeasingcurve.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qelapsedtimer.sip` & `PyQt6-6.5.0/sip/QtCore/qelapsedtimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qeventloop.sip` & `PyQt6-6.5.0/sip/QtCore/qeventloop.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qfile.sip` & `PyQt6-6.5.0/sip/QtCore/qfile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qfiledevice.sip` & `PyQt6-6.5.0/sip/QtCore/qfiledevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qfileinfo.sip` & `PyQt6-6.5.0/sip/QtCore/qfileinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qfileselector.sip` & `PyQt6-6.5.0/sip/QtCore/qfileselector.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qfilesystemwatcher.sip` & `PyQt6-6.5.0/sip/QtCore/qfilesystemwatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qflags.sip` & `PyQt6-6.5.0/sip/QtCore/qflags.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qidentityproxymodel.sip` & `PyQt6-6.5.0/sip/QtCore/qidentityproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qiodevice.sip` & `PyQt6-6.5.0/sip/QtCore/qiodevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qiodevicebase.sip` & `PyQt6-6.5.0/sip/QtCore/qiodevicebase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qitemselectionmodel.sip` & `PyQt6-6.5.0/sip/QtCore/qitemselectionmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qjsonarray.sip` & `PyQt6-6.5.0/sip/QtCore/qjsonarray.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qjsondocument.sip` & `PyQt6-6.5.0/sip/QtCore/qjsondocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qjsonobject.sip` & `PyQt6-6.5.0/sip/QtCore/qjsonobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qjsonvalue.sip` & `PyQt6-6.5.0/sip/QtCore/qjsonvalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qlibrary.sip` & `PyQt6-6.5.0/sip/QtCore/qlibrary.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qlibraryinfo.sip` & `PyQt6-6.5.0/sip/QtCore/qlibraryinfo.sip`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 {
 %TypeHeaderCode
 #include <qlibraryinfo.h>
 %End
 
 public:
     static bool isDebugBuild();
+%If (Qt_6_5_0 -)
+    static bool isSharedBuild();
+%End
     static QString path(QLibraryInfo::LibraryPath p) /ReleaseGIL/;
     static QVersionNumber version();
 
 private:
     QLibraryInfo();
 
 public:
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qline.sip` & `PyQt6-6.5.0/sip/QtCore/qline.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qlocale.sip` & `PyQt6-6.5.0/sip/QtCore/qlocale.sip`

 * *Files 5% similar despite different names*

```diff
@@ -379,14 +379,35 @@
         Wolaytta,
 %If (Qt_6_3_0 -)
         Kaingang,
 %End
 %If (Qt_6_3_0 -)
         Nheengatu,
 %End
+%If (Qt_6_5_0 -)
+        Haryanvi,
+%End
+%If (Qt_6_5_0 -)
+        NorthernFrisian,
+%End
+%If (Qt_6_5_0 -)
+        Rajasthani,
+%End
+%If (Qt_6_5_0 -)
+        Moksha,
+%End
+%If (Qt_6_5_0 -)
+        TokiPona,
+%End
+%If (Qt_6_5_0 -)
+        Pijin,
+%End
+%If (Qt_6_5_0 -)
+        Obolo,
+%End
     };
 
     enum Country
     {
         AnyCountry,
 %If (Qt_6_2_0 -)
         AnyTerritory,
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qlockfile.sip` & `PyQt6-6.5.0/sip/QtCore/qlockfile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qlogging.sip` & `PyQt6-6.5.0/sip/QtCore/qlogging.sip`

 * *Files 17% similar despite different names*

```diff
@@ -60,42 +60,80 @@
     void debug(const char *msg) const /ReleaseGIL/;
 %MethodCode
         Py_BEGIN_ALLOW_THREADS
         sipCpp->debug("%s", a0);
         Py_END_ALLOW_THREADS
 %End
 
+    void debug(const QLoggingCategory &cat, const char *msg) const /ReleaseGIL/;
+%MethodCode
+        Py_BEGIN_ALLOW_THREADS
+        sipCpp->debug(*a0, "%s", a1);
+        Py_END_ALLOW_THREADS
+%End
+
+    void info(const char *msg) const /ReleaseGIL/;
+%MethodCode
+        Py_BEGIN_ALLOW_THREADS
+        sipCpp->info("%s", a0);
+        Py_END_ALLOW_THREADS
+%End
+
+    void info(const QLoggingCategory &cat, const char *msg) const /ReleaseGIL/;
+%MethodCode
+        Py_BEGIN_ALLOW_THREADS
+        sipCpp->info(*a0, "%s", a1);
+        Py_END_ALLOW_THREADS
+%End
+
     void warning(const char *msg) const /ReleaseGIL/;
 %MethodCode
         Py_BEGIN_ALLOW_THREADS
         sipCpp->warning("%s", a0);
         Py_END_ALLOW_THREADS
 %End
 
+    void warning(const QLoggingCategory &cat, const char *msg) const /ReleaseGIL/;
+%MethodCode
+        Py_BEGIN_ALLOW_THREADS
+        sipCpp->warning(*a0, "%s", a1);
+        Py_END_ALLOW_THREADS
+%End
+
     void critical(const char *msg) const /ReleaseGIL/;
 %MethodCode
         Py_BEGIN_ALLOW_THREADS
         sipCpp->critical("%s", a0);
         Py_END_ALLOW_THREADS
 %End
 
+    void critical(const QLoggingCategory &cat, const char *msg) const /ReleaseGIL/;
+%MethodCode
+        Py_BEGIN_ALLOW_THREADS
+        sipCpp->critical(*a0, "%s", a1);
+        Py_END_ALLOW_THREADS
+%End
+
     void fatal(const char *msg) const /ReleaseGIL/;
 %MethodCode
         Py_BEGIN_ALLOW_THREADS
         sipCpp->fatal("%s", a0);
         Py_END_ALLOW_THREADS
 %End
 
-    void info(const char *msg) const /ReleaseGIL/;
+%If (Qt_6_5_0 -)
+    void fatal(const QLoggingCategory &cat, const char *msg) const /ReleaseGIL/;
 %MethodCode
         Py_BEGIN_ALLOW_THREADS
-        sipCpp->info("%s", a0);
+        sipCpp->fatal(*a0, "%s", a1);
         Py_END_ALLOW_THREADS
 %End
 
+%End
+
 private:
     QMessageLogger(const QMessageLogger &);
 };
 
 void qCritical(const char *msg) /ReleaseGIL/;
 %MethodCode
     const char *file, *function;
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qloggingcategory.sip` & `PyQt6-6.5.0/sip/QtCore/qloggingcategory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmargins.sip` & `PyQt6-6.5.0/sip/QtCore/qmargins.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmessageauthenticationcode.sip` & `PyQt6-6.5.0/sip/QtCore/qmessageauthenticationcode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmetaobject.sip` & `PyQt6-6.5.0/sip/QtCore/qmetaobject.sip`

 * *Files 15% similar despite different names*

```diff
@@ -193,14 +193,52 @@
 %MethodCode
         // Make use of the QMetaProperty to provide the extra information to correctly
         // handle enums.
         sipRes = qpycore_PyObject_FromQVariant(*sipCpp, sipCpp->read(a0));
 %End
 
     bool write(QObject *obj, const QVariant &value) const;
+%MethodCode
+        // If it looks like we are trying to write an int to an enum then we are
+        // probably trying to write to an unregistered enum.  Converting the int to the
+        // name of the corresponding key should work (although this isn't a documented
+        // feature).
+        
+        QMetaEnum me = sipCpp->enumerator();
+        if (me.isValid() && a1->typeId() == QMetaType::Int)
+        {
+            QString key;
+        
+            if (me.isFlag())
+            {
+                key = QString(me.valueToKeys(a1->toInt()));
+            }
+            else
+            {
+                const char *key_s = me.valueToKey(a1->toInt());
+                
+                if (key_s)
+                {
+                    key = QString(key_s);
+                }
+                else
+                {
+                    PyErr_Format(PyExc_ValueError, "%S is not a valid enum member", a1);
+                    sipIsErr = 1;
+                }
+            }
+            
+            if (!sipIsErr)
+                *const_cast<QVariant *>(a1) = QVariant(key);
+        }
+        
+        if (!sipIsErr)
+            sipRes = sipCpp->write(a0, *a1);
+%End
+
     bool reset(QObject *obj) const;
     bool hasStdCppSet() const;
     bool isValid() const;
     bool isResettable() const;
     bool isUser() const;
     int userType() const;
     bool hasNotifySignal() const;
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qmetatype.sip` & `PyQt6-6.5.0/sip/QtCore/qmetatype.sip`

 * *Files 16% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         Char,
         Char16,
         Char32,
         ULong,
         UShort,
         UChar,
         Float,
+%If (Qt_6_5_0 -)
+        Float16,
+%End
         QObjectStar,
         QMatrix4x4,
         QVector2D,
         QVector3D,
         QVector4D,
         QQuaternion,
         QEasingCurve,
@@ -128,14 +131,20 @@
         IsUnsignedEnumeration,
         IsPointer,
         RelocatableType,
         IsQmlList,
 %If (Qt_6_2_0 -)
         IsConst,
 %End
+%If (Qt_6_5_0 -)
+        NeedsCopyConstruction,
+%End
+%If (Qt_6_5_0 -)
+        NeedsMoveConstruction,
+%End
     };
 
     typedef QFlags<QMetaType::TypeFlag> TypeFlags;
     qsizetype sizeOf() const;
     QMetaType::TypeFlags flags() const;
     bool isValid() const;
     bool isRegistered() const;
@@ -154,14 +163,29 @@
 %If (Qt_6_4_0 -)
     Py_hash_t __hash__() const;
 %MethodCode
         sipRes = qHash(*sipCpp);
 %End
 
 %End
+%If (Qt_6_5_0 -)
+    void registerType() const;
+%End
+%If (Qt_6_5_0 -)
+    bool isDefaultConstructible() const;
+%End
+%If (Qt_6_5_0 -)
+    bool isCopyConstructible() const;
+%End
+%If (Qt_6_5_0 -)
+    bool isMoveConstructible() const;
+%End
+%If (Qt_6_5_0 -)
+    bool isDestructible() const;
+%End
 
 private:
     QMetaType(const QMetaType &);
 };
 
 bool operator==(QMetaType a, QMetaType b);
 bool operator!=(QMetaType a, QMetaType b);
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qmimedata.sip` & `PyQt6-6.5.0/sip/QtCore/qmimedata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmimedatabase.sip` & `PyQt6-6.5.0/sip/QtCore/qmimedatabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmimetype.sip` & `PyQt6-6.5.0/sip/QtCore/qmimetype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmutex.sip` & `PyQt6-6.5.0/sip/QtCore/qmutex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qmutexlocker.sip` & `PyQt6-6.5.0/sip/QtCore/qmutexlocker.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qnamespace.sip` & `PyQt6-6.5.0/sip/QtCore/qnamespace.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1537,14 +1537,25 @@
     {
         Round,
         Ceil,
         Floor,
         RoundPreferFloor,
         PassThrough,
     };
+
+%If (Qt_6_5_0 -)
+
+    enum class ColorScheme
+    {
+        Unknown,
+        Light,
+        Dark,
+    };
+
+%End
 };
 
 class QKeyCombination
 {
 %TypeHeaderCode
 #include <qnamespace.h>
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qnumeric.sip` & `PyQt6-6.5.0/sip/QtQuick/qquicktextdocument.sip`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-// qnumeric.sip generated by MetaSIP
+// qquicktextdocument.sip generated by MetaSIP
 //
-// This file is part of the QtCore Python extension module.
+// This file is part of the QtQuick Python extension module.
 //
 // Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
@@ -16,18 +16,17 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-%ModuleCode
-#include <qnumeric.h>
+class QQuickTextDocument : QObject
+{
+%TypeHeaderCode
+#include <qquicktextdocument.h>
 %End
 
-bool qIsInf(double d);
-bool qIsFinite(double d);
-bool qIsNaN(double d);
-double qInf();
-double qSNaN();
-double qQNaN();
-quint64 qFloatDistance(double a, double b);
+public:
+    QQuickTextDocument(QQuickItem *parent /TransferThis/);
+    QTextDocument *textDocument() const;
+};
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qobject.sip` & `PyQt6-6.5.0/sip/QtCore/qobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qobjectcleanuphandler.sip` & `PyQt6-6.5.0/sip/QtCore/qobjectcleanuphandler.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qobjectdefs.sip` & `PyQt6-6.5.0/sip/QtCore/qobjectdefs.sip`

 * *Files 20% similar despite different names*

```diff
@@ -135,14 +135,17 @@
         }
         else
         {
             qtcore_invokeMethod_exception();
         }
 %End
 
+%If (Qt_6_5_0 -)
+    QObject *newInstance(QGenericArgument value0, QGenericArgument value1 = QGenericArgument(), QGenericArgument value2 = QGenericArgument(), QGenericArgument value3 = QGenericArgument(), QGenericArgument value4 = QGenericArgument(), QGenericArgument value5 = QGenericArgument(), QGenericArgument value6 = QGenericArgument(), QGenericArgument value7 = QGenericArgument(), QGenericArgument value8 = QGenericArgument(), QGenericArgument value9 = QGenericArgument()) const;
+%End
     int constructorCount() const;
     int indexOfConstructor(const char *constructor) const;
     QMetaMethod constructor(int index) const;
     static bool checkConnectArgs(const QMetaMethod &signal, const QMetaMethod &method);
     bool inherits(const QMetaObject *metaObject) const;
 
     class Connection
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qoperatingsystemversion.sip` & `PyQt6-6.5.0/sip/QtCore/qoperatingsystemversion.sip`

 * *Files 5% similar despite different names*

```diff
@@ -62,35 +62,50 @@
     static const QOperatingSystemVersion OSXElCapitan;
     static const QOperatingSystemVersion MacOSSierra;
     static const QOperatingSystemVersion MacOSHighSierra;
     static const QOperatingSystemVersion MacOSMojave;
     static const QOperatingSystemVersion MacOSCatalina;
     static const QOperatingSystemVersion MacOSBigSur;
     static const QOperatingSystemVersion MacOSMonterey;
+%If (Qt_6_5_0 -)
+    static const QOperatingSystemVersionBase MacOSVentura;
+%End
     static const QOperatingSystemVersion AndroidJellyBean;
     static const QOperatingSystemVersion AndroidJellyBean_MR1;
     static const QOperatingSystemVersion AndroidJellyBean_MR2;
     static const QOperatingSystemVersion AndroidKitKat;
     static const QOperatingSystemVersion AndroidLollipop;
     static const QOperatingSystemVersion AndroidLollipop_MR1;
     static const QOperatingSystemVersion AndroidMarshmallow;
     static const QOperatingSystemVersion AndroidNougat;
     static const QOperatingSystemVersion AndroidNougat_MR1;
     static const QOperatingSystemVersion AndroidOreo;
     static const QOperatingSystemVersion AndroidOreo_MR1;
     static const QOperatingSystemVersion AndroidPie;
     static const QOperatingSystemVersion Android10;
     static const QOperatingSystemVersion Android11;
+%If (Qt_6_5_0 -)
+    static const QOperatingSystemVersionBase Android12;
+%End
+%If (Qt_6_5_0 -)
+    static const QOperatingSystemVersionBase Android12L;
+%End
+%If (Qt_6_5_0 -)
+    static const QOperatingSystemVersionBase Android13;
+%End
     static const QOperatingSystemVersionBase Windows10_1809;
     static const QOperatingSystemVersionBase Windows10_1903;
     static const QOperatingSystemVersionBase Windows10_1909;
     static const QOperatingSystemVersionBase Windows10_2004;
     static const QOperatingSystemVersionBase Windows10_20H2;
     static const QOperatingSystemVersionBase Windows10_21H1;
     static const QOperatingSystemVersionBase Windows10_21H2;
+%If (Qt_6_5_0 -)
+    static const QOperatingSystemVersionBase Windows10_22H2;
+%End
     static const QOperatingSystemVersionBase Windows11;
 %If (Qt_6_4_0 -)
     static const QOperatingSystemVersionBase Windows11_21H2;
 %End
 %If (Qt_6_4_0 -)
     static const QOperatingSystemVersionBase Windows11_22H2;
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qparallelanimationgroup.sip` & `PyQt6-6.5.0/sip/QtCore/qparallelanimationgroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpauseanimation.sip` & `PyQt6-6.5.0/sip/QtCore/qpauseanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpluginloader.sip` & `PyQt6-6.5.0/sip/QtCore/qpluginloader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpoint.sip` & `PyQt6-6.5.0/sip/QtCore/qpoint.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qprocess.sip` & `PyQt6-6.5.0/sip/QtCore/qprocess.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpropertyanimation.sip` & `PyQt6-6.5.0/sip/QtCore/qpropertyanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpycore_qhash.sip` & `PyQt6-6.5.0/sip/QtCore/qpycore_qhash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpycore_qlist.sip` & `PyQt6-6.5.0/sip/QtCore/qpycore_qlist.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1080,14 +1080,119 @@
     return sipGetState(sipTransferObj);
 %End
 };
 
 %End
 
 
+%If (Qt_6_5_0 -)
+
+%MappedType QList<qsizetype>
+        /TypeHintIn="Iterable[int]", TypeHintOut="List[int]",
+        TypeHintValue="[]"/
+{
+%TypeHeaderCode
+#include <qlist.h>
+%End
+
+%ConvertFromTypeCode
+    PyObject *l = PyList_New(sipCpp->size());
+
+    if (!l)
+        return 0;
+
+    for (int i = 0; i < sipCpp->size(); ++i)
+    {
+        PyObject *pobj = PyLong_FromLongLong(sipCpp->value(i));
+
+        if (!pobj)
+        {
+            Py_DECREF(l);
+
+            return 0;
+        }
+
+        PyList_SetItem(l, i, pobj);
+    }
+
+    return l;
+%End
+
+%ConvertToTypeCode
+    PyObject *iter = PyObject_GetIter(sipPy);
+
+    if (!sipIsErr)
+    {
+        PyErr_Clear();
+        Py_XDECREF(iter);
+
+        return (iter && !PyBytes_Check(sipPy) && !PyUnicode_Check(sipPy));
+    }
+
+    if (!iter)
+    {
+        *sipIsErr = 1;
+
+        return 0;
+    }
+
+    QList<qsizetype> *ql = new QList<qsizetype>;
+ 
+    for (Py_ssize_t i = 0; ; ++i)
+    {
+        PyErr_Clear();
+        PyObject *itm = PyIter_Next(iter);
+
+        if (!itm)
+        {
+            if (PyErr_Occurred())
+            {
+                delete ql;
+                Py_DECREF(iter);
+                *sipIsErr = 1;
+
+                return 0;
+            }
+
+            break;
+        }
+
+        PyErr_Clear();
+        qsizetype val = PyLong_AsLongLong(itm);
+        
+        if (PyErr_Occurred())
+        {
+            PyErr_Format(PyExc_TypeError,
+                    "index %zd has type '%s' but 'int' is expected", i,
+                    sipPyTypeName(Py_TYPE(itm)));
+
+            Py_DECREF(itm);
+            delete ql;
+            Py_DECREF(iter);
+            *sipIsErr = 1;
+
+            return 0;
+        }
+
+        ql->append(val);
+
+        Py_DECREF(itm);
+    }
+
+    Py_DECREF(iter);
+ 
+    *sipCppPtr = ql;
+ 
+    return sipGetState(sipTransferObj);
+%End
+};
+
+%End
+
+
 %MappedType QList<float>
         /TypeHintIn="Iterable[float]", TypeHintOut="List[float]",
         TypeHintValue="[]"/
 {
 %TypeHeaderCode
 #include <qlist.h>
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qpycore_qmap.sip` & `PyQt6-6.5.0/sip/QtCore/qpycore_qmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpycore_qset.sip` & `PyQt6-6.5.0/sip/QtCore/qpycore_qset.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpycore_std_pair.sip` & `PyQt6-6.5.0/sip/QtCore/qpycore_std_pair.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qpycore_virtual_error_handler.sip` & `PyQt6-6.5.0/sip/QtCore/qpycore_virtual_error_handler.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qrandom.sip` & `PyQt6-6.5.0/sip/QtCore/qrandom.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qreadwritelock.sip` & `PyQt6-6.5.0/sip/QtCore/qreadwritelock.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qrect.sip` & `PyQt6-6.5.0/sip/QtCore/qrect.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qregularexpression.sip` & `PyQt6-6.5.0/sip/QtCore/qregularexpression.sip`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,22 @@
     {
         NoMatchOption,
         AnchorAtOffsetMatchOption,
         DontCheckSubjectStringMatchOption,
     };
 
     typedef QFlags<QRegularExpression::MatchOption> MatchOptions;
-    QRegularExpressionMatch match(QStringView subjectView, qsizetype offset = 0, QRegularExpression::MatchType matchType = QRegularExpression::NormalMatch, QRegularExpression::MatchOptions matchOptions = QRegularExpression::NoMatchOption) const;
-    QRegularExpressionMatchIterator globalMatch(QStringView subjectView, qsizetype offset = 0, QRegularExpression::MatchType matchType = QRegularExpression::NormalMatch, QRegularExpression::MatchOptions matchOptions = QRegularExpression::NoMatchOption) const;
+    QRegularExpressionMatch match(const QString &subject, qsizetype offset = 0, QRegularExpression::MatchType matchType = QRegularExpression::NormalMatch, QRegularExpression::MatchOptions matchOptions = QRegularExpression::NoMatchOption) const;
+%If (Qt_6_5_0 -)
+    QRegularExpressionMatch matchView(QStringView subjectView, qsizetype offset = 0, QRegularExpression::MatchType matchType = QRegularExpression::NormalMatch, QRegularExpression::MatchOptions matchOptions = QRegularExpression::NoMatchOption) const;
+%End
+    QRegularExpressionMatchIterator globalMatch(const QString &subject, qsizetype offset = 0, QRegularExpression::MatchType matchType = QRegularExpression::NormalMatch, QRegularExpression::MatchOptions matchOptions = QRegularExpression::NoMatchOption) const;
+%If (Qt_6_5_0 -)
+    QRegularExpressionMatchIterator globalMatchView(QStringView subjectView, qsizetype offset = 0, QRegularExpression::MatchType matchType = QRegularExpression::NormalMatch, QRegularExpression::MatchOptions matchOptions = QRegularExpression::NoMatchOption) const;
+%End
     static QString escape(const QString &str);
     QStringList namedCaptureGroups() const;
     bool operator==(const QRegularExpression &re) const;
     bool operator!=(const QRegularExpression &re) const;
     void optimize() const;
     Py_hash_t __hash__() const;
 %MethodCode
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qresource.sip` & `PyQt6-6.5.0/sip/QtCore/qresource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qrunnable.sip` & `PyQt6-6.5.0/sip/QtCore/qrunnable.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsavefile.sip` & `PyQt6-6.5.0/sip/QtCore/qsavefile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsemaphore.sip` & `PyQt6-6.5.0/sip/QtCore/qsemaphore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsequentialanimationgroup.sip` & `PyQt6-6.5.0/sip/QtCore/qsequentialanimationgroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsettings.sip` & `PyQt6-6.5.0/sip/QtCore/qsettings.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsharedmemory.sip` & `PyQt6-6.5.0/sip/QtCore/qsharedmemory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsignalmapper.sip` & `PyQt6-6.5.0/sip/QtCore/qsignalmapper.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsize.sip` & `PyQt6-6.5.0/sip/QtCore/qsize.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsocketnotifier.sip` & `PyQt6-6.5.0/sip/QtCore/qsocketnotifier.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsortfilterproxymodel.sip` & `PyQt6-6.5.0/sip/QtCore/qsortfilterproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstandardpaths.sip` & `PyQt6-6.5.0/sip/QtCore/qstandardpaths.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstorageinfo.sip` & `PyQt6-6.5.0/sip/QtCore/qstorageinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstring.sip` & `PyQt6-6.5.0/sip/QtCore/qstring.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstringconverter.sip` & `PyQt6-6.5.0/sip/QtCore/qstringconverter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstringconverter_base.sip` & `PyQt6-6.5.0/sip/QtCore/qstringconverter_base.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstringlist.sip` & `PyQt6-6.5.0/sip/QtCore/qstringlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstringlistmodel.sip` & `PyQt6-6.5.0/sip/QtCore/qstringlistmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qstringview.sip` & `PyQt6-6.5.0/sip/QtCore/qstringview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsysinfo.sip` & `PyQt6-6.5.0/sip/QtCore/qsysinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qsystemsemaphore.sip` & `PyQt6-6.5.0/sip/QtCore/qsystemsemaphore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtemporarydir.sip` & `PyQt6-6.5.0/sip/QtCore/qtemporarydir.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtemporaryfile.sip` & `PyQt6-6.5.0/sip/QtCore/qtemporaryfile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtextboundaryfinder.sip` & `PyQt6-6.5.0/sip/QtCore/qtextboundaryfinder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtextstream.sip` & `PyQt6-6.5.0/sip/QtCore/qtextstream.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qthread.sip` & `PyQt6-6.5.0/sip/QtCore/qthread.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qthreadpool.sip` & `PyQt6-6.5.0/sip/QtCore/qthreadpool.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtimeline.sip` & `PyQt6-6.5.0/sip/QtCore/qtimeline.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtimer.sip` & `PyQt6-6.5.0/sip/QtCore/qtimer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtimezone.sip` & `PyQt6-6.5.0/sip/QtCore/qtimezone.sip`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         QDateTime atUtc;
         int offsetFromUtc;
         int standardTimeOffset;
         int daylightTimeOffset;
     };
 
     typedef QList<QTimeZone::OffsetData> OffsetDataList;
+%If (Qt_6_5_0 -)
+    QTimeZone(QTimeZone::Initialization spec);
+%End
 %If (Qt_6_2_0 -)
     QTimeZone(const QByteArray &zoneId, int offsetSeconds, const QString &name, const QString &abbreviation, QLocale::Territory territory = QLocale::AnyTerritory, const QString &comment = QString());
 %End
 %If (- Qt_6_2_0)
     QTimeZone(const QByteArray &zoneId, int offsetSeconds, const QString &name, const QString &abbreviation, QLocale::Country country = QLocale::AnyCountry, const QString &comment = QString());
 %End
     explicit QTimeZone(const QByteArray &ianaId);
@@ -113,11 +116,38 @@
     static QList<QByteArray> windowsIdToIanaIds(const QByteArray &windowsId, QLocale::Territory territory);
 %End
 %If (- Qt_6_2_0)
     static QList<QByteArray> windowsIdToIanaIds(const QByteArray &windowsId, QLocale::Country country);
 %End
     static QTimeZone systemTimeZone();
     static QTimeZone utc();
+%If (Qt_6_5_0 -)
+
+    enum Initialization
+    {
+        LocalTime,
+        UTC,
+    };
+
+%End
+%If (Qt_6_5_0 -)
+    static QTimeZone fromSecondsAheadOfUtc(int offset);
+%End
+%If (Qt_6_5_0 -)
+    Qt::TimeSpec timeSpec() const;
+%End
+%If (Qt_6_5_0 -)
+    int fixedSecondsAheadOfUtc() const;
+%End
+%If (Qt_6_5_0 -)
+    bool isUtcOrFixedOffset() const;
+%End
+%If (Qt_6_5_0 -)
+    static bool isUtcOrFixedOffset(Qt::TimeSpec spec);
+%End
+%If (Qt_6_5_0 -)
+    QTimeZone asBackendZone() const;
+%End
 };
 
 QDataStream &operator<<(QDataStream &ds, const QTimeZone &tz) /ReleaseGIL/;
 QDataStream &operator>>(QDataStream &ds, QTimeZone &tz /Constrained/) /ReleaseGIL/;
```

### Comparing `PyQt6-6.4.2/sip/QtCore/qtranslator.sip` & `PyQt6-6.5.0/sip/QtCore/qtranslator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qtransposeproxymodel.sip` & `PyQt6-6.5.0/sip/QtCore/qtransposeproxymodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qurl.sip` & `PyQt6-6.5.0/sip/QtCore/qurl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qurlquery.sip` & `PyQt6-6.5.0/sip/QtCore/qurlquery.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/quuid.sip` & `PyQt6-6.5.0/sip/QtCore/quuid.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qvariant.sip` & `PyQt6-6.5.0/sip/QtCore/qvariant.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qvariantanimation.sip` & `PyQt6-6.5.0/sip/QtCore/qvariantanimation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qversionnumber.sip` & `PyQt6-6.5.0/sip/QtCore/qversionnumber.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qwaitcondition.sip` & `PyQt6-6.5.0/sip/QtCore/qwaitcondition.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qwineventnotifier.sip` & `PyQt6-6.5.0/sip/QtCore/qwineventnotifier.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtCore/qxmlstream.sip` & `PyQt6-6.5.0/sip/QtWidgets/qfiledialog.sip`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-// qxmlstream.sip generated by MetaSIP
+// qfiledialog.sip generated by MetaSIP
 //
-// This file is part of the QtCore Python extension module.
+// This file is part of the QtWidgets Python extension module.
 //
 // Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
@@ -16,418 +16,296 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QXmlStreamAttribute
+class QFileDialog : QDialog
 {
 %TypeHeaderCode
-#include <qxmlstream.h>
+#include <qfiledialog.h>
 %End
 
 public:
-    QXmlStreamAttribute();
-    QXmlStreamAttribute(const QString &qualifiedName, const QString &value);
-    QXmlStreamAttribute(const QString &namespaceUri, const QString &name, const QString &value);
-    QStringView namespaceUri() const;
-    QStringView name() const;
-    QStringView qualifiedName() const;
-    QStringView prefix() const;
-    QStringView value() const;
-    bool isDefault() const;
-    bool operator==(const QXmlStreamAttribute &other) const;
-    bool operator!=(const QXmlStreamAttribute &other) const;
-};
-
-class QXmlStreamNamespaceDeclaration
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
-
-public:
-    QXmlStreamNamespaceDeclaration();
-    QXmlStreamNamespaceDeclaration(const QString &prefix, const QString &namespaceUri);
-    QStringView prefix() const;
-    QStringView namespaceUri() const;
-    bool operator==(const QXmlStreamNamespaceDeclaration &other) const;
-    bool operator!=(const QXmlStreamNamespaceDeclaration &other) const;
-};
-
-typedef QList<QXmlStreamNamespaceDeclaration> QXmlStreamNamespaceDeclarations;
-
-class QXmlStreamNotationDeclaration
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
-
-public:
-    QXmlStreamNotationDeclaration();
-    QStringView name() const;
-    QStringView systemId() const;
-    QStringView publicId() const;
-    bool operator==(const QXmlStreamNotationDeclaration &other) const;
-    bool operator!=(const QXmlStreamNotationDeclaration &other) const;
-};
-
-typedef QList<QXmlStreamNotationDeclaration> QXmlStreamNotationDeclarations;
-
-class QXmlStreamEntityDeclaration
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
-
-public:
-    QXmlStreamEntityDeclaration();
-    QStringView name() const;
-    QStringView notationName() const;
-    QStringView systemId() const;
-    QStringView publicId() const;
-    QStringView value() const;
-    bool operator==(const QXmlStreamEntityDeclaration &other) const;
-    bool operator!=(const QXmlStreamEntityDeclaration &other) const;
-};
-
-typedef QList<QXmlStreamEntityDeclaration> QXmlStreamEntityDeclarations;
-
-class QXmlStreamEntityResolver
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
-
-public:
-    virtual ~QXmlStreamEntityResolver();
-    virtual QString resolveUndeclaredEntity(const QString &name);
-};
-
-class QXmlStreamReader
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
-
-public:
-    enum TokenType
+    enum ViewMode
     {
-        NoToken,
-        Invalid,
-        StartDocument,
-        EndDocument,
-        StartElement,
-        EndElement,
-        Characters,
-        Comment,
-        DTD,
-        EntityReference,
-        ProcessingInstruction,
+        Detail,
+        List,
     };
 
-    QXmlStreamReader();
-    explicit QXmlStreamReader(QIODevice *device);
-    explicit QXmlStreamReader(const QByteArray &data);
-    explicit QXmlStreamReader(const QString &data);
-    ~QXmlStreamReader();
-    void setDevice(QIODevice *device);
-    QIODevice *device() const;
-    void addData(const QByteArray &data);
-    void addData(const QString &data);
-    void clear();
-    bool atEnd() const;
-    QXmlStreamReader::TokenType readNext();
-    QXmlStreamReader::TokenType tokenType() const;
-    QString tokenString() const;
-    void setNamespaceProcessing(bool);
-    bool namespaceProcessing() const;
-    bool isStartDocument() const;
-    bool isEndDocument() const;
-    bool isStartElement() const;
-    bool isEndElement() const;
-    bool isCharacters() const;
-    bool isWhitespace() const;
-    bool isCDATA() const;
-    bool isComment() const;
-    bool isDTD() const;
-    bool isEntityReference() const;
-    bool isProcessingInstruction() const;
-    bool isStandaloneDocument() const;
-    QStringView documentVersion() const;
-    QStringView documentEncoding() const;
-    qint64 lineNumber() const;
-    qint64 columnNumber() const;
-    qint64 characterOffset() const;
-    QXmlStreamAttributes attributes() const;
-
-    enum ReadElementTextBehaviour
+    enum FileMode
     {
-        ErrorOnUnexpectedElement,
-        IncludeChildElements,
-        SkipChildElements,
+        AnyFile,
+        ExistingFile,
+        Directory,
+        ExistingFiles,
     };
 
-    QString readElementText(QXmlStreamReader::ReadElementTextBehaviour behaviour = QXmlStreamReader::ErrorOnUnexpectedElement);
-    QStringView name() const;
-    QStringView namespaceUri() const;
-    QStringView qualifiedName() const;
-    QStringView prefix() const;
-    QStringView processingInstructionTarget() const;
-    QStringView processingInstructionData() const;
-    QStringView text() const;
-    QXmlStreamNamespaceDeclarations namespaceDeclarations() const;
-    void addExtraNamespaceDeclaration(const QXmlStreamNamespaceDeclaration &extraNamespaceDeclaraction);
-    void addExtraNamespaceDeclarations(const QXmlStreamNamespaceDeclarations &extraNamespaceDeclaractions);
-    QXmlStreamNotationDeclarations notationDeclarations() const;
-    QXmlStreamEntityDeclarations entityDeclarations() const;
-    QStringView dtdName() const;
-    QStringView dtdPublicId() const;
-    QStringView dtdSystemId() const;
-
-    enum Error
+    enum AcceptMode
     {
-        NoError,
-        UnexpectedElementError,
-        CustomError,
-        NotWellFormedError,
-        PrematureEndOfDocumentError,
+        AcceptOpen,
+        AcceptSave,
     };
 
-    void raiseError(const QString &message = QString());
-    QString errorString() const;
-    QXmlStreamReader::Error error() const;
-    bool hasError() const;
-    void setEntityResolver(QXmlStreamEntityResolver *resolver /KeepReference/);
-    QXmlStreamEntityResolver *entityResolver() const;
-    bool readNextStartElement();
-    void skipCurrentElement();
-    int entityExpansionLimit() const;
-    void setEntityExpansionLimit(int limit);
-
-private:
-    QXmlStreamReader(const QXmlStreamReader &);
-};
-
-class QXmlStreamWriter
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
-
-public:
-    QXmlStreamWriter();
-    explicit QXmlStreamWriter(QIODevice *device);
-    explicit QXmlStreamWriter(QByteArray *array);
-    ~QXmlStreamWriter();
-    void setDevice(QIODevice *device);
-    QIODevice *device() const;
-    void setAutoFormatting(bool);
-    bool autoFormatting() const;
-    void setAutoFormattingIndent(int spaces);
-    int autoFormattingIndent() const;
-    void writeAttribute(const QString &qualifiedName, const QString &value);
-    void writeAttribute(const QString &namespaceUri, const QString &name, const QString &value);
-    void writeAttribute(const QXmlStreamAttribute &attribute);
-    void writeAttributes(const QXmlStreamAttributes &attributes);
-    void writeCDATA(const QString &text);
-    void writeCharacters(const QString &text);
-    void writeComment(const QString &text);
-    void writeDTD(const QString &dtd);
-    void writeEmptyElement(const QString &qualifiedName);
-    void writeEmptyElement(const QString &namespaceUri, const QString &name);
-    void writeTextElement(const QString &qualifiedName, const QString &text);
-    void writeTextElement(const QString &namespaceUri, const QString &name, const QString &text);
-    void writeEndDocument();
-    void writeEndElement();
-    void writeEntityReference(const QString &name);
-    void writeNamespace(const QString &namespaceUri, const QString &prefix = QString());
-    void writeDefaultNamespace(const QString &namespaceUri);
-    void writeProcessingInstruction(const QString &target, const QString &data = QString());
-    void writeStartDocument();
-    void writeStartDocument(const QString &version);
-    void writeStartDocument(const QString &version, bool standalone);
-    void writeStartElement(const QString &qualifiedName);
-    void writeStartElement(const QString &namespaceUri, const QString &name);
-    void writeCurrentToken(const QXmlStreamReader &reader);
-    bool hasError() const;
+    enum DialogLabel
+    {
+        LookIn,
+        FileName,
+        FileType,
+        Accept,
+        Reject,
+    };
 
-private:
-    QXmlStreamWriter(const QXmlStreamWriter &);
-};
+    enum Option /BaseType=Flag/
+    {
+        ShowDirsOnly,
+        DontResolveSymlinks,
+        DontConfirmOverwrite,
+        DontUseNativeDialog,
+        ReadOnly,
+        HideNameFilterDetails,
+        DontUseCustomDirectoryIcons,
+    };
 
-class QXmlStreamAttributes
-{
-%TypeHeaderCode
-#include <qxmlstream.h>
-%End
+    typedef QFlags<QFileDialog::Option> Options;
+    QFileDialog(QWidget *parent /TransferThis/, Qt::WindowFlags f);
+    QFileDialog(QWidget *parent /TransferThis/ = 0, const QString &caption = QString(), const QString &directory = QString(), const QString &filter = QString());
+    virtual ~QFileDialog();
+    void setDirectory(const QString &directory);
+    void setDirectory(const QDir &adirectory);
+    QDir directory() const;
+    void selectFile(const QString &filename);
+    QStringList selectedFiles() const;
+    void setViewMode(QFileDialog::ViewMode mode);
+    QFileDialog::ViewMode viewMode() const;
+    void setFileMode(QFileDialog::FileMode mode);
+    QFileDialog::FileMode fileMode() const;
+    void setAcceptMode(QFileDialog::AcceptMode mode);
+    QFileDialog::AcceptMode acceptMode() const;
+    void setDefaultSuffix(const QString &suffix);
+    QString defaultSuffix() const;
+    void setHistory(const QStringList &paths);
+    QStringList history() const;
+    void setItemDelegate(QAbstractItemDelegate *delegate /KeepReference/);
+    QAbstractItemDelegate *itemDelegate() const;
+    void setIconProvider(QAbstractFileIconProvider *provider /KeepReference/);
+    QAbstractFileIconProvider *iconProvider() const;
+    void setLabelText(QFileDialog::DialogLabel label, const QString &text);
+    QString labelText(QFileDialog::DialogLabel label) const;
+
+signals:
+    void currentChanged(const QString &path);
+    void directoryEntered(const QString &directory);
+    void filesSelected(const QStringList &files);
+    void filterSelected(const QString &filter);
+    void fileSelected(const QString &file);
 
 public:
-    QXmlStreamAttributes();
-    QStringView value(const QString &namespaceUri, const QString &name) const;
-    QStringView value(const QString &qualifiedName) const;
-    void append(const QString &namespaceUri, const QString &name, const QString &value);
-    void append(const QString &qualifiedName, const QString &value);
-    bool hasAttribute(const QString &namespaceUri, const QString &name) const;
-    bool hasAttribute(const QString &qualifiedName) const;
-// Methods inherited from QList<QXmlStreamAttribute> and Python special methods.
-// Keep in sync with QPolygon and QPolygonF.
-
-
-void append(const QXmlStreamAttribute &value);
-
-const QXmlStreamAttribute &at(int i) const;
-void clear();
-bool contains(const QXmlStreamAttribute &value) const;
-int count(const QXmlStreamAttribute &value) const;
-int count() const /__len__/;
-void *data();
-
-// Note the Qt return value is discarded as it would require handwritten code
-// and seems pretty useless.
-void fill(const QXmlStreamAttribute &value, int size = -1);
-
-QXmlStreamAttribute &first();
-int indexOf(const QXmlStreamAttribute &value, int from = 0) const;
-void insert(int i, const QXmlStreamAttribute &value);
-bool isEmpty() const;
-QXmlStreamAttribute &last();
-int lastIndexOf(const QXmlStreamAttribute &value, int from = -1) const;
-
-// Note the Qt return type is QList<QXmlStreamAttribute>.  We can't do the
-// usual trick because there is no QXmlStreamAttributes ctor that takes a
-// QList<QXmlStreamAttribute> argument.  We could use handwritten code but we
-// don't bother.
-//QXmlStreamAttributes mid(int pos, int length = -1) const;
-
-void prepend(const QXmlStreamAttribute &value);
-void remove(int i);
-void remove(int i, int count);
-void resize(qsizetype size);
-void replace(int i, const QXmlStreamAttribute &value);
-int size() const;
-
-// These are hidden by other implementations in QXmlStreamAttributes.
-//QXmlStreamAttribute value(int i) const;
-//QXmlStreamAttribute value(int i, const QXmlStreamAttribute &defaultValue) const;
-
-bool operator!=(const QXmlStreamAttributes &other) const;
-
-// Note the Qt return type is QList<QXmlStreamAttribute>.  We can't do the
-// usual trick because there is no QXmlStreamAttributes ctor that takes a
-// QList<QXmlStreamAttribute> argument.  We could use handwritten code but we
-// don't bother.
-//QXmlStreamAttributes operator+(const QXmlStreamAttributes &other) const;
-
-QXmlStreamAttributes &operator+=(const QXmlStreamAttributes &other);
-QXmlStreamAttributes &operator+=(const QXmlStreamAttribute &value);
-
-bool operator==(const QXmlStreamAttributes &other) const;
-
-QXmlStreamAttribute &operator[](int i);
+    static QString getExistingDirectory(QWidget *parent = 0, const QString &caption = QString(), const QString &directory = QString(), QFileDialog::Options options = QFileDialog::ShowDirsOnly) /ReleaseGIL/;
+    static QUrl getExistingDirectoryUrl(QWidget *parent = 0, const QString &caption = QString(), const QUrl &directory = QUrl(), QFileDialog::Options options = QFileDialog::ShowDirsOnly, const QStringList &supportedSchemes = QStringList()) /ReleaseGIL/;
+    static SIP_PYTUPLE getOpenFileName(QWidget *parent = 0, const QString &caption = QString(), const QString &directory = QString(), const QString &filter = QString(), const QString &initialFilter = QString(), Options options = QFileDialog::Options()) /TypeHint="Tuple[QString, QString]", ReleaseGIL/;
 %MethodCode
-Py_ssize_t idx = sipConvertFromSequenceIndex(a0, sipCpp->count());
-
-if (idx < 0)
-    sipIsErr = 1;
-else
-    sipRes = &sipCpp->operator[]((int)idx);
+        QString *name;
+        QString *filter = new QString(*a4);
+        
+        Py_BEGIN_ALLOW_THREADS
+        
+        name = new QString(QFileDialog::getOpenFileName(a0, *a1, *a2, *a3, filter, *a5));
+        
+        Py_END_ALLOW_THREADS
+        
+        PyObject *name_obj = sipConvertFromNewType(name, sipType_QString, NULL);
+        PyObject *filter_obj = sipConvertFromNewType(filter, sipType_QString, NULL);
+        
+        if (name_obj && filter_obj)
+            sipRes = PyTuple_Pack(2, name_obj, filter_obj);
+        
+        Py_XDECREF(name_obj);
+        Py_XDECREF(filter_obj);
 %End
 
-// Some additional Python special methods.
-
-void __setitem__(int i, const QXmlStreamAttribute &value);
+    static SIP_PYTUPLE getOpenFileNames(QWidget *parent = 0, const QString &caption = QString(), const QString &directory = QString(), const QString &filter = QString(), const QString &initialFilter = QString(), Options options = QFileDialog::Options()) /TypeHint="Tuple[QStringList, QString]", ReleaseGIL/;
 %MethodCode
-int len;
-
-len = sipCpp->count();
-
-if ((a0 = (int)sipConvertFromSequenceIndex(a0, len)) < 0)
-    sipIsErr = 1;
-else
-    (*sipCpp)[a0] = *a1;
+        QStringList *names;
+        QString *filter = new QString(*a4);
+        
+        Py_BEGIN_ALLOW_THREADS
+        
+        names = new QStringList(QFileDialog::getOpenFileNames(a0, *a1, *a2, *a3, filter, *a5));
+        
+        Py_END_ALLOW_THREADS
+        
+        PyObject *names_obj = sipConvertFromNewType(names, sipType_QStringList, NULL);
+        PyObject *filter_obj = sipConvertFromNewType(filter, sipType_QString, NULL);
+        
+        if (names_obj && filter_obj)
+            sipRes = PyTuple_Pack(2, names_obj, filter_obj);
+        
+        Py_XDECREF(names_obj);
+        Py_XDECREF(filter_obj);
 %End
 
-void __setitem__(SIP_PYSLICE slice, const QXmlStreamAttributes &list);
+    static SIP_PYTUPLE getSaveFileName(QWidget *parent = 0, const QString &caption = QString(), const QString &directory = QString(), const QString &filter = QString(), const QString &initialFilter = QString(), Options options = QFileDialog::Options()) /TypeHint="Tuple[QString, QString]", ReleaseGIL/;
 %MethodCode
-Py_ssize_t start, stop, step, slicelength;
-
-if (sipConvertFromSliceObject(a0, sipCpp->count(), &start, &stop, &step, &slicelength) < 0)
-{
-    sipIsErr = 1;
-}
-else
-{
-    int vlen = a1->count();
+        QString *name;
+        QString *filter = new QString(*a4);
+        
+        Py_BEGIN_ALLOW_THREADS
+        
+        name = new QString(QFileDialog::getSaveFileName(a0, *a1, *a2, *a3, filter, *a5));
+        
+        Py_END_ALLOW_THREADS
+        
+        PyObject *name_obj = sipConvertFromNewType(name, sipType_QString, NULL);
+        PyObject *filter_obj = sipConvertFromNewType(filter, sipType_QString, NULL);
+        
+        if (name_obj && filter_obj)
+            sipRes = PyTuple_Pack(2, name_obj, filter_obj);
+        
+        Py_XDECREF(name_obj);
+        Py_XDECREF(filter_obj);
+%End
+
+protected:
+    virtual void done(int result);
+    virtual void accept();
+    virtual void changeEvent(QEvent *e);
 
-    if (vlen != slicelength)
-    {
-        sipBadLengthForSlice(vlen, slicelength);
-        sipIsErr = 1;
-    }
-    else
-    {
-        QList<QXmlStreamAttribute>::const_iterator it = a1->begin();
-
-        for (Py_ssize_t i = 0; i < slicelength; ++i)
+public:
+    void setSidebarUrls(const QList<QUrl> &urls);
+    QList<QUrl> sidebarUrls() const;
+    QByteArray saveState() const;
+    bool restoreState(const QByteArray &state);
+    void setProxyModel(QAbstractProxyModel *model /Transfer/);
+    QAbstractProxyModel *proxyModel() const;
+    void setNameFilter(const QString &filter);
+    void setNameFilters(const QStringList &filters);
+    QStringList nameFilters() const;
+    void selectNameFilter(const QString &filter);
+    QString selectedNameFilter() const;
+    QDir::Filters filter() const;
+    void setFilter(QDir::Filters filters);
+    void setOption(QFileDialog::Option option, bool on = true);
+    bool testOption(QFileDialog::Option option) const;
+    void setOptions(QFileDialog::Options options);
+    QFileDialog::Options options() const;
+    virtual void open();
+    void open(SIP_PYOBJECT slot /TypeHint="PYQT_SLOT"/);
+%MethodCode
+        QObject *receiver;
+        QByteArray slot_signature;
+        
+        if ((sipError = pyqt6_qtwidgets_get_connection_parts(a0, sipCpp, "()", false, &receiver, slot_signature)) == sipErrorNone)
         {
-            (*sipCpp)[start] = *it;
-            start += step;
-            ++it;
+            sipCpp->open(receiver, slot_signature.constData());
+        }
+        else if (sipError == sipErrorContinue)
+        {
+            sipError = sipBadCallableArg(0, a0);
         }
-    }
-}
 %End
 
-void __delitem__(int i);
-%MethodCode
-if ((a0 = (int)sipConvertFromSequenceIndex(a0, sipCpp->count())) < 0)
-    sipIsErr = 1;
-else
-    sipCpp->remove(a0);
-%End
+    virtual void setVisible(bool visible);
+    void setDirectoryUrl(const QUrl &directory);
+    QUrl directoryUrl() const;
+    void selectUrl(const QUrl &url);
+    QList<QUrl> selectedUrls() const;
+    void setMimeTypeFilters(const QStringList &filters);
+    QStringList mimeTypeFilters() const;
+    void selectMimeTypeFilter(const QString &filter);
+
+signals:
+    void urlSelected(const QUrl &url);
+    void urlsSelected(const QList<QUrl> &urls);
+    void currentUrlChanged(const QUrl &url);
+    void directoryUrlEntered(const QUrl &directory);
 
-void __delitem__(SIP_PYSLICE slice);
+public:
+    static SIP_PYTUPLE getOpenFileUrl(QWidget *parent = 0, const QString &caption = QString(), const QUrl &directory = QUrl(), const QString &filter = QString(), const QString &initialFilter = QString(), Options options = QFileDialog::Options(), const QStringList &supportedSchemes = QStringList()) /TypeHint="Tuple[QUrl, QString]", ReleaseGIL/;
 %MethodCode
-Py_ssize_t start, stop, step, slicelength;
-
-if (sipConvertFromSliceObject(a0, sipCpp->count(), &start, &stop, &step, &slicelength) < 0)
-{
-    sipIsErr = 1;
-}
-else
-{
-    for (Py_ssize_t i = 0; i < slicelength; ++i)
-    {
-        sipCpp->remove(start);
-        start += step - 1;
-    }
-}
+        QUrl *url;
+        QString *filter = new QString(*a4);
+        
+        Py_BEGIN_ALLOW_THREADS
+        
+        url = new QUrl(QFileDialog::getOpenFileUrl(a0, *a1, *a2, *a3, filter, *a5, *a6));
+        
+        Py_END_ALLOW_THREADS
+        
+        PyObject *url_obj = sipConvertFromNewType(url, sipType_QUrl, NULL);
+        PyObject *filter_obj = sipConvertFromNewType(filter, sipType_QString, NULL);
+        
+        if (url_obj && filter_obj)
+            sipRes = PyTuple_Pack(2, url_obj, filter_obj);
+        
+        Py_XDECREF(url_obj);
+        Py_XDECREF(filter_obj);
 %End
 
-QXmlStreamAttributes operator[](SIP_PYSLICE slice);
+    static SIP_PYTUPLE getOpenFileUrls(QWidget *parent = 0, const QString &caption = QString(), const QUrl &directory = QUrl(), const QString &filter = QString(), const QString &initialFilter = QString(), Options options = QFileDialog::Options(), const QStringList &supportedSchemes = QStringList()) /TypeHint="Tuple[List[QUrl], QString]", ReleaseGIL/;
 %MethodCode
-Py_ssize_t start, stop, step, slicelength;
-
-if (sipConvertFromSliceObject(a0, sipCpp->count(), &start, &stop, &step, &slicelength) < 0)
-{
-    sipIsErr = 1;
-}
-else
-{
-    sipRes = new QXmlStreamAttributes();
-
-    for (Py_ssize_t i = 0; i < slicelength; ++i)
-    {
-        (*sipRes) += (*sipCpp)[start];
-        start += step;
-    }
-}
+        QList<QUrl> url_list;
+        QString *filter = new QString(*a4);
+        
+        Py_BEGIN_ALLOW_THREADS
+        
+        url_list = QFileDialog::getOpenFileUrls(a0, *a1, *a2, *a3, filter, *a5, *a6);
+        
+        Py_END_ALLOW_THREADS
+        
+        PyObject *url_list_obj = PyList_New(url_list.size());
+        
+        if (url_list_obj)
+        {
+            for (int i = 0; i < url_list.size(); ++i)
+            {
+                QUrl *url = new QUrl(url_list.at(i));
+                PyObject *url_obj = sipConvertFromNewType(url, sipType_QUrl, NULL);
+                
+                if (!url_obj)
+                {
+                    delete url;
+                    Py_DECREF(url_list_obj);
+                    url_list_obj = 0;
+                    break;
+                }
+                
+                PyList_SetItem(url_list_obj, i, url_obj);
+            }
+        }
+        
+        PyObject *filter_obj = sipConvertFromNewType(filter, sipType_QString, NULL);
+        
+        if (url_list_obj && filter_obj)
+            sipRes = PyTuple_Pack(2, url_list_obj, filter_obj);
+        
+        Py_XDECREF(url_list_obj);
+        Py_XDECREF(filter_obj);
 %End
 
-int __contains__(const QXmlStreamAttribute &value);
+    static SIP_PYTUPLE getSaveFileUrl(QWidget *parent = 0, const QString &caption = QString(), const QUrl &directory = QUrl(), const QString &filter = QString(), const QString &initialFilter = QString(), Options options = QFileDialog::Options(), const QStringList &supportedSchemes = QStringList()) /TypeHint="Tuple[QUrl, QString]", ReleaseGIL/;
 %MethodCode
-// It looks like you can't assign QBool to int.
-sipRes = bool(sipCpp->contains(*a0));
-%End
+        QUrl *url;
+        QString *filter = new QString(*a4);
+        
+        Py_BEGIN_ALLOW_THREADS
+        
+        url = new QUrl(QFileDialog::getSaveFileUrl(a0, *a1, *a2, *a3, filter, *a5, *a6));
+        
+        Py_END_ALLOW_THREADS
+        
+        PyObject *url_obj = sipConvertFromNewType(url, sipType_QUrl, NULL);
+        PyObject *filter_obj = sipConvertFromNewType(filter, sipType_QString, NULL);
+        
+        if (url_obj && filter_obj)
+            sipRes = PyTuple_Pack(2, url_obj, filter_obj);
+        
+        Py_XDECREF(url_obj);
+        Py_XDECREF(filter_obj);
+%End
+
+    void setSupportedSchemes(const QStringList &schemes);
+    QStringList supportedSchemes() const;
+    QString selectedMimeTypeFilter() const;
+    static void saveFileContent(const QByteArray &fileContent, const QString &fileNameHint = QString()) /ReleaseGIL/;
 };
```

### Comparing `PyQt6-6.4.2/sip/QtDBus/QtDBusmod.sip` & `PyQt6-6.5.0/sip/QtDBus/QtDBusmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusabstractadaptor.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusabstractadaptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusabstractinterface.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusabstractinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusargument.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusargument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusconnection.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusconnection.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusconnectioninterface.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusconnectioninterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbuserror.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbuserror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusextratypes.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusextratypes.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusinterface.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusmessage.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusmessage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbuspendingcall.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbuspendingcall.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusservicewatcher.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusservicewatcher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qdbusunixfiledescriptor.sip` & `PyQt6-6.5.0/sip/QtDBus/qdbusunixfiledescriptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qpydbuspendingreply.sip` & `PyQt6-6.5.0/sip/QtDBus/qpydbuspendingreply.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDBus/qpydbusreply.sip` & `PyQt6-6.5.0/sip/QtDBus/qpydbusreply.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/QtDesignermod.sip` & `PyQt6-6.5.0/sip/QtDesigner/QtDesignermod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractactioneditor.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractactioneditor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractformbuilder.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractformbuilder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractformeditor.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractformeditor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractformwindow.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractformwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractformwindowcursor.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractformwindowcursor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractformwindowmanager.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractformwindowmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractobjectinspector.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractobjectinspector.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractpropertyeditor.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractpropertyeditor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/abstractwidgetbox.sip` & `PyQt6-6.5.0/sip/QtDesigner/abstractwidgetbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/container.sip` & `PyQt6-6.5.0/sip/QtDesigner/container.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/customwidget.sip` & `PyQt6-6.5.0/sip/QtDesigner/customwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/default_extensionfactory.sip` & `PyQt6-6.5.0/sip/QtDesigner/default_extensionfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/extension.sip` & `PyQt6-6.5.0/sip/QtDesigner/extension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/formbuilder.sip` & `PyQt6-6.5.0/sip/QtDesigner/formbuilder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/membersheet.sip` & `PyQt6-6.5.0/sip/QtDesigner/membersheet.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/propertysheet.sip` & `PyQt6-6.5.0/sip/QtDesigner/propertysheet.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qextensionmanager.sip` & `PyQt6-6.5.0/sip/QtDesigner/qextensionmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qpydesignercontainerextension.sip` & `PyQt6-6.5.0/sip/QtDesigner/qpydesignercontainerextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip` & `PyQt6-6.5.0/sip/QtDesigner/qpydesignercustomwidgetcollectionplugin.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qpydesignercustomwidgetplugin.sip` & `PyQt6-6.5.0/sip/QtDesigner/qpydesignercustomwidgetplugin.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qpydesignermembersheetextension.sip` & `PyQt6-6.5.0/sip/QtDesigner/qpydesignermembersheetextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qpydesignerpropertysheetextension.sip` & `PyQt6-6.5.0/sip/QtDesigner/qpydesignerpropertysheetextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/qpydesignertaskmenuextension.sip` & `PyQt6-6.5.0/sip/QtDesigner/qpydesignertaskmenuextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtDesigner/taskmenu.sip` & `PyQt6-6.5.0/sip/QtDesigner/taskmenu.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/QtGuimod.sip` & `PyQt6-6.5.0/sip/QtGui/QtGuimod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -124,13 +124,14 @@
 %Include qtextlist.sip
 %Include qtextobject.sip
 %Include qtextoption.sip
 %Include qtexttable.sip
 %Include qtransform.sip
 %Include qundogroup.sip
 %Include qundostack.sip
+%Include qutimimeconverter.sip
 %Include qvalidator.sip
 %Include qvectornd.sip
 %Include qwindow.sip
 %Include qwindowdefs.sip
 %Include qpygui_qlist.sip
 %Include opengl_types.sip
```

### Comparing `PyQt6-6.4.2/sip/QtGui/opengl_types.sip` & `PyQt6-6.5.0/sip/QtGui/opengl_types.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qabstractfileiconprovider.sip` & `PyQt6-6.5.0/sip/QtGui/qabstractfileiconprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qabstracttextdocumentlayout.sip` & `PyQt6-6.5.0/sip/QtGui/qabstracttextdocumentlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qaction.sip` & `PyQt6-6.5.0/sip/QtGui/qaction.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qactiongroup.sip` & `PyQt6-6.5.0/sip/QtGui/qactiongroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qbackingstore.sip` & `PyQt6-6.5.0/sip/QtGui/qbackingstore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qbitmap.sip` & `PyQt6-6.5.0/sip/QtGui/qbitmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qbrush.sip` & `PyQt6-6.5.0/sip/QtGui/qbrush.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qclipboard.sip` & `PyQt6-6.5.0/sip/QtGui/qclipboard.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qcolor.sip` & `PyQt6-6.5.0/sip/QtGui/qcolor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qcolorspace.sip` & `PyQt6-6.5.0/sip/QtGui/qcolorspace.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qcolortransform.sip` & `PyQt6-6.5.0/sip/QtGui/qcolortransform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qcursor.sip` & `PyQt6-6.5.0/sip/QtGui/qcursor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qdesktopservices.sip` & `PyQt6-6.5.0/sip/QtGui/qdesktopservices.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qdrag.sip` & `PyQt6-6.5.0/sip/QtGui/qdrag.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qevent.sip` & `PyQt6-6.5.0/sip/QtGui/qevent.sip`

 * *Files 0% similar despite different names*

```diff
@@ -574,14 +574,17 @@
 {
 %TypeHeaderCode
 #include <qevent.h>
 %End
 
 public:
     QShortcutEvent(const QKeySequence &key, int id, bool ambiguous = false);
+%If (Qt_6_5_0 -)
+    QShortcutEvent(const QKeySequence &key, const QShortcut *shortcut = 0, bool ambiguous = false);
+%End
     virtual ~QShortcutEvent();
     bool isAmbiguous() const;
     const QKeySequence &key() const;
     int shortcutId() const;
     virtual QShortcutEvent *clone() const /Factory/;
 };
```

### Comparing `PyQt6-6.4.2/sip/QtGui/qeventpoint.sip` & `PyQt6-6.5.0/sip/QtGui/qeventpoint.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qfilesystemmodel.sip` & `PyQt6-6.5.0/sip/QtGui/qfilesystemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qfont.sip` & `PyQt6-6.5.0/sip/QtGui/qfont.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qfontdatabase.sip` & `PyQt6-6.5.0/sip/QtGui/qfontdatabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qfontinfo.sip` & `PyQt6-6.5.0/sip/QtGui/qfontinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qfontmetrics.sip` & `PyQt6-6.5.0/sip/QtGui/qfontmetrics.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qgenericmatrix.sip` & `PyQt6-6.5.0/sip/QtGui/qgenericmatrix.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qglyphrun.sip` & `PyQt6-6.5.0/sip/QtGui/qglyphrun.sip`

 * *Files 15% similar despite different names*

```diff
@@ -63,10 +63,22 @@
     void setFlag(QGlyphRun::GlyphRunFlag flag, bool enabled = true);
     void setFlags(QGlyphRun::GlyphRunFlags flags);
     QGlyphRun::GlyphRunFlags flags() const;
     void setBoundingRect(const QRectF &boundingRect);
     QRectF boundingRect() const;
     bool isEmpty() const;
     void swap(QGlyphRun &other /Constrained/);
+%If (Qt_6_5_0 -)
+    QList<qsizetype> stringIndexes() const;
+%End
+%If (Qt_6_5_0 -)
+    void setStringIndexes(const QList<qsizetype> &stringIndexes);
+%End
+%If (Qt_6_5_0 -)
+    void setSourceString(const QString &sourceString);
+%End
+%If (Qt_6_5_0 -)
+    QString sourceString() const;
+%End
 };
 
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtGui/qguiapplication.sip` & `PyQt6-6.5.0/sip/QtGui/qguiapplication.sip`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,17 @@
 
 public:
     static void setDesktopFileName(const QString &name);
     static QString desktopFileName();
     static QScreen *screenAt(const QPoint &point);
     static void setHighDpiScaleFactorRoundingPolicy(Qt::HighDpiScaleFactorRoundingPolicy policy);
     static Qt::HighDpiScaleFactorRoundingPolicy highDpiScaleFactorRoundingPolicy();
+%If (Qt_6_5_0 -)
+    void setBadgeNumber(qint64 number);
+%End
 
 protected:
     virtual bool event(QEvent *);
 };
 
 %ModuleHeaderCode
 // Imports from QtCore.
```

### Comparing `PyQt6-6.4.2/sip/QtGui/qicon.sip` & `PyQt6-6.5.0/sip/QtGui/qicon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qiconengine.sip` & `PyQt6-6.5.0/sip/QtGui/qiconengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qimage.sip` & `PyQt6-6.5.0/sip/QtGui/qimage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qimageiohandler.sip` & `PyQt6-6.5.0/sip/QtGui/qimageiohandler.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qimagereader.sip` & `PyQt6-6.5.0/sip/QtGui/qimagereader.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qimagewriter.sip` & `PyQt6-6.5.0/sip/QtGui/qimagewriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qinputdevice.sip` & `PyQt6-6.5.0/sip/QtGui/qinputdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qinputmethod.sip` & `PyQt6-6.5.0/sip/QtGui/qinputmethod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qkeysequence.sip` & `PyQt6-6.5.0/sip/QtGui/qkeysequence.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qmatrix4x4.sip` & `PyQt6-6.5.0/sip/QtGui/qmatrix4x4.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qmovie.sip` & `PyQt6-6.5.0/sip/QtGui/qmovie.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qoffscreensurface.sip` & `PyQt6-6.5.0/sip/QtGui/qoffscreensurface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qopenglcontext.sip` & `PyQt6-6.5.0/sip/QtGui/qopenglcontext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpagedpaintdevice.sip` & `PyQt6-6.5.0/sip/QtGui/qpagedpaintdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpagelayout.sip` & `PyQt6-6.5.0/sip/QtGui/qpagelayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpageranges.sip` & `PyQt6-6.5.0/sip/QtGui/qpageranges.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpagesize.sip` & `PyQt6-6.5.0/sip/QtGui/qpagesize.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpaintdevice.sip` & `PyQt6-6.5.0/sip/QtGui/qpaintdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpaintdevicewindow.sip` & `PyQt6-6.5.0/sip/QtGui/qpaintdevicewindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpaintengine.sip` & `PyQt6-6.5.0/sip/QtGui/qpaintengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpainter.sip` & `PyQt6-6.5.0/sip/QtGui/qpainter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpainterpath.sip` & `PyQt6-6.5.0/sip/QtGui/qpainterpath.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpalette.sip` & `PyQt6-6.5.0/sip/QtGui/qpalette.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpdfwriter.sip` & `PyQt6-6.5.0/sip/QtGui/qpdfwriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpen.sip` & `PyQt6-6.5.0/sip/QtGui/qpen.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpicture.sip` & `PyQt6-6.5.0/sip/QtGui/qpicture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpixelformat.sip` & `PyQt6-6.5.0/sip/QtGui/qpixelformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpixmap.sip` & `PyQt6-6.5.0/sip/QtGui/qpixmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpixmapcache.sip` & `PyQt6-6.5.0/sip/QtGui/qpixmapcache.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpointingdevice.sip` & `PyQt6-6.5.0/sip/QtGui/qpointingdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpolygon.sip` & `PyQt6-6.5.0/sip/QtGui/qpolygon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qpygui_qlist.sip` & `PyQt6-6.5.0/sip/QtGui/qpygui_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qquaternion.sip` & `PyQt6-6.5.0/sip/QtGui/qquaternion.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qrasterwindow.sip` & `PyQt6-6.5.0/sip/QtGui/qrasterwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qrawfont.sip` & `PyQt6-6.5.0/sip/QtGui/qrawfont.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qregion.sip` & `PyQt6-6.5.0/sip/QtGui/qregion.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qrgb.sip` & `PyQt6-6.5.0/sip/QtGui/qrgb.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qrgba64.sip` & `PyQt6-6.5.0/sip/QtGui/qrgba64.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qscreen.sip` & `PyQt6-6.5.0/sip/QtGui/qscreen.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qsessionmanager.sip` & `PyQt6-6.5.0/sip/QtGui/qsessionmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qshortcut.sip` & `PyQt6-6.5.0/sip/QtGui/qshortcut.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qstandarditemmodel.sip` & `PyQt6-6.5.0/sip/QtGui/qstandarditemmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qstatictext.sip` & `PyQt6-6.5.0/sip/QtGui/qstatictext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qstylehints.sip` & `PyQt6-6.5.0/sip/QtGui/qstylehints.sip`

 * *Files 14% similar despite different names*

```diff
@@ -79,11 +79,22 @@
 
 signals:
     void showShortcutsInContextMenusChanged(bool);
 
 public:
     int mouseDoubleClickDistance() const;
     int touchDoubleTapDistance() const;
+%If (Qt_6_5_0 -)
+    qreal keyboardAutoRepeatRateF() const;
+%End
+%If (Qt_6_5_0 -)
+    Qt::ColorScheme colorScheme() const;
+%End
+
+signals:
+%If (Qt_6_5_0 -)
+    void colorSchemeChanged(Qt::ColorScheme colorScheme);
+%End
 
 private:
     QStyleHints();
 };
```

### Comparing `PyQt6-6.4.2/sip/QtGui/qsurface.sip` & `PyQt6-6.5.0/sip/QtGui/qsurface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qsurfaceformat.sip` & `PyQt6-6.5.0/sip/QtGui/qsurfaceformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qsyntaxhighlighter.sip` & `PyQt6-6.5.0/sip/QtGui/qsyntaxhighlighter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextcursor.sip` & `PyQt6-6.5.0/sip/QtGui/qtextcursor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextdocument.sip` & `PyQt6-6.5.0/sip/QtGui/qtextdocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextdocumentfragment.sip` & `PyQt6-6.5.0/sip/QtGui/qtextdocumentfragment.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextdocumentwriter.sip` & `PyQt6-6.5.0/sip/QtGui/qtextdocumentwriter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextformat.sip` & `PyQt6-6.5.0/sip/QtGui/qtextformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextlayout.sip` & `PyQt6-6.5.0/sip/QtGui/qtextlayout.sip`

 * *Files 6% similar despite different names*

```diff
@@ -105,20 +105,40 @@
     void setCursorMoveStyle(Qt::CursorMoveStyle style);
     Qt::CursorMoveStyle cursorMoveStyle() const;
     int leftCursorPosition(int oldPos) const;
     int rightCursorPosition(int oldPos) const;
 %If (PyQt_RawFont)
     QList<QGlyphRun> glyphRuns(int from = -1, int length = -1) const;
 %End
+%If (Qt_6_5_0 -)
+    QList<QGlyphRun> glyphRuns(int from, int length, QTextLayout::GlyphRunRetrievalFlags flags) const;
+%End
     void setFormats(const QList<QTextLayout::FormatRange> &overrides);
     QList<QTextLayout::FormatRange> formats() const;
     void clearFormats();
 
 private:
     QTextLayout(const QTextLayout &);
+
+public:
+%If (Qt_6_5_0 -)
+
+    enum GlyphRunRetrievalFlag
+    {
+        RetrieveGlyphIndexes,
+        RetrieveGlyphPositions,
+        RetrieveStringIndexes,
+        RetrieveString,
+        RetrieveAll,
+    };
+
+%End
+%If (Qt_6_5_0 -)
+    typedef QFlags<QTextLayout::GlyphRunRetrievalFlag> GlyphRunRetrievalFlags;
+%End
 };
 
 class QTextLine
 {
 %TypeHeaderCode
 #include <qtextlayout.h>
 %End
@@ -162,11 +182,14 @@
     qreal leading() const;
     void setLeadingIncluded(bool included);
     bool leadingIncluded() const;
     qreal horizontalAdvance() const;
 %If (PyQt_RawFont)
     QList<QGlyphRun> glyphRuns(int from = -1, int length = -1) const;
 %End
+%If (Qt_6_5_0 -)
+    QList<QGlyphRun> glyphRuns(int from, int length, QTextLayout::GlyphRunRetrievalFlags flags) const;
+%End
 };
 
 bool operator==(const QTextLayout::FormatRange &lhs, const QTextLayout::FormatRange &rhs);
 bool operator!=(const QTextLayout::FormatRange &lhs, const QTextLayout::FormatRange &rhs);
```

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextlist.sip` & `PyQt6-6.5.0/sip/QtGui/qtextlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextobject.sip` & `PyQt6-6.5.0/sip/QtGui/qtextobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtextoption.sip` & `PyQt6-6.5.0/sip/QtGui/qtextoption.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtexttable.sip` & `PyQt6-6.5.0/sip/QtGui/qtexttable.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qtransform.sip` & `PyQt6-6.5.0/sip/QtGui/qtransform.sip`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,21 @@
     QTransform inverted(bool *invertible = 0) const;
     QTransform adjoint() const;
     QTransform transposed() const;
     QTransform &translate(qreal dx, qreal dy);
     QTransform &scale(qreal sx, qreal sy);
     QTransform &shear(qreal sh, qreal sv);
     QTransform &rotate(qreal angle, Qt::Axis axis = Qt::ZAxis);
+%If (Qt_6_5_0 -)
+    QTransform &rotate(qreal a, Qt::Axis axis, qreal distanceToPlane);
+%End
     QTransform &rotateRadians(qreal angle, Qt::Axis axis = Qt::ZAxis);
+%If (Qt_6_5_0 -)
+    QTransform &rotateRadians(qreal a, Qt::Axis axis, qreal distanceToPlane);
+%End
     static bool squareToQuad(const QPolygonF &square, QTransform &result);
     static bool quadToSquare(const QPolygonF &quad, QTransform &result);
     static bool quadToQuad(const QPolygonF &one, const QPolygonF &two, QTransform &result);
     bool operator==(const QTransform &) const;
     bool operator!=(const QTransform &) const;
     QTransform &operator*=(const QTransform &) /__imatmul__/;
     QTransform operator*(const QTransform &o) const /__matmul__/;
```

### Comparing `PyQt6-6.4.2/sip/QtGui/qundogroup.sip` & `PyQt6-6.5.0/sip/QtGui/qundogroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qundostack.sip` & `PyQt6-6.5.0/sip/QtGui/qundostack.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qvalidator.sip` & `PyQt6-6.5.0/sip/QtGui/qvalidator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qvectornd.sip` & `PyQt6-6.5.0/sip/QtGui/qvectornd.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qwindow.sip` & `PyQt6-6.5.0/sip/QtGui/qwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtGui/qwindowdefs.sip` & `PyQt6-6.5.0/sip/QtGui/qwindowdefs.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/QtHelpmod.sip` & `PyQt6-6.5.0/sip/QtHelp/QtHelpmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qcompressedhelpinfo.sip` & `PyQt6-6.5.0/sip/QtHelp/qcompressedhelpinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpcontentwidget.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpcontentwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpengine.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpenginecore.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpenginecore.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpfilterdata.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpfilterdata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpfilterengine.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpfilterengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpfiltersettingswidget.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpfiltersettingswidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpindexwidget.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpindexwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelplink.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelplink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpsearchengine.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpsearchengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpsearchquerywidget.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpsearchquerywidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtHelp/qhelpsearchresultwidget.sip` & `PyQt6-6.5.0/sip/QtHelp/qhelpsearchresultwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/QtMultimediamod.sip` & `PyQt6-6.5.0/sip/QtMultimedia/QtMultimediamod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -62,12 +62,13 @@
 %Include qmediacapturesession.sip
 %Include qmediadevices.sip
 %Include qmediaformat.sip
 %Include qmediametadata.sip
 %Include qmediaplayer.sip
 %Include qmediarecorder.sip
 %Include qmediatimerange.sip
+%Include qscreencapture.sip
 %Include qsoundeffect.sip
 %Include qvideoframe.sip
 %Include qvideoframeformat.sip
 %Include qvideosink.sip
 %Include qpymultimedia_qlist.sip
```

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudio.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudio.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudiobuffer.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudiobuffer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudiodecoder.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudiodecoder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudiodevice.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudiodevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudioformat.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudioformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudioinput.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudioinput.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudiooutput.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudiooutput.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudiosink.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudiosink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qaudiosource.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qaudiosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qcamera.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qcamera.sip`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,20 @@
         {sipName_QAudioSource, &sipType_QAudioSource, -1, 5},
         {sipName_QCamera, &sipType_QCamera, -1, 6},
         {sipName_QImageCapture, &sipType_QImageCapture, -1, 7},
         {sipName_QMediaCaptureSession, &sipType_QMediaCaptureSession, -1, 8},
         {sipName_QMediaDevices, &sipType_QMediaDevices, -1, 9},
         {sipName_QMediaPlayer, &sipType_QMediaPlayer, -1, 10},
         {sipName_QMediaRecorder, &sipType_QMediaRecorder, -1, 11},
-        {sipName_QSoundEffect, &sipType_QSoundEffect, -1, 12},
+    #if QT_VERSION >= 0x060500
+        {sipName_QScreenCapture, &sipType_QScreenCapture, -1, 12},
+    #else
+        {0, 0, -1, 12},
+    #endif
+        {sipName_QSoundEffect, &sipType_QSoundEffect, -1, 13},
         {sipName_QVideoSink, &sipType_QVideoSink, -1, -1},
     };
     
     int i = 0;
     
     sipType = NULL;
```

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qcameradevice.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qcameradevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qimagecapture.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qimagecapture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediacapturesession.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediacapturesession.sip`

 * *Files 12% similar despite different names*

```diff
@@ -49,10 +49,23 @@
 signals:
     void audioInputChanged();
     void cameraChanged();
     void imageCaptureChanged();
     void recorderChanged();
     void videoOutputChanged();
     void audioOutputChanged();
+
+public:
+%If (Qt_6_5_0 -)
+    QScreenCapture *screenCapture();
+%End
+%If (Qt_6_5_0 -)
+    void setScreenCapture(QScreenCapture *screenCapture);
+%End
+
+signals:
+%If (Qt_6_5_0 -)
+    void screenCaptureChanged();
+%End
 };
 
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediadevices.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediadevices.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediaformat.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediaformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediametadata.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediametadata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediaplayer.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediaplayer.sip`

 * *Files 3% similar despite different names*

```diff
@@ -127,10 +127,20 @@
     };
 
     int loops() const;
     void setLoops(int loops);
 
 signals:
     void loopsChanged();
+
+public:
+%If (Qt_6_5_0 -)
+    bool isPlaying() const;
+%End
+
+signals:
+%If (Qt_6_5_0 -)
+    void playingChanged(bool playing);
+%End
 };
 
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediarecorder.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediarecorder.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qmediatimerange.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qmediatimerange.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qpymultimedia_qlist.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qpymultimedia_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qsoundeffect.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qsoundeffect.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qvideoframe.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qvideoframe.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qvideoframeformat.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qvideoframeformat.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimedia/qvideosink.sip` & `PyQt6-6.5.0/sip/QtMultimedia/qvideosink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip` & `PyQt6-6.5.0/sip/QtMultimediaWidgets/QtMultimediaWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip` & `PyQt6-6.5.0/sip/QtMultimediaWidgets/qgraphicsvideoitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtMultimediaWidgets/qvideowidget.sip` & `PyQt6-6.5.0/sip/QtMultimediaWidgets/qvideowidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/QtNetworkmod.sip` & `PyQt6-6.5.0/sip/QtNetwork/QtNetworkmod.sip`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 %Include qabstractnetworkcache.sip
 %Include qabstractsocket.sip
 %Include qauthenticator.sip
 %Include qdnslookup.sip
 %Include qhostaddress.sip
 %Include qhostinfo.sip
 %Include qhstspolicy.sip
+%Include qhttp1configuration.sip
 %Include qhttp2configuration.sip
 %Include qhttpmultipart.sip
 %Include qlocalserver.sip
 %Include qlocalsocket.sip
 %Include qnetworkaccessmanager.sip
 %Include qnetworkcookie.sip
 %Include qnetworkcookiejar.sip
```

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qabstractnetworkcache.sip` & `PyQt6-6.5.0/sip/QtNetwork/qabstractnetworkcache.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qabstractsocket.sip` & `PyQt6-6.5.0/sip/QtNetwork/qabstractsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qauthenticator.sip` & `PyQt6-6.5.0/sip/QtNetwork/qauthenticator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qdnslookup.sip` & `PyQt6-6.5.0/sip/QtNetwork/qdnslookup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qhostaddress.sip` & `PyQt6-6.5.0/sip/QtNetwork/qhostaddress.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qhostinfo.sip` & `PyQt6-6.5.0/sip/QtNetwork/qhostinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qhstspolicy.sip` & `PyQt6-6.5.0/sip/QtNetwork/qhstspolicy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qhttp2configuration.sip` & `PyQt6-6.5.0/sip/QtNetwork/qhttp2configuration.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qhttpmultipart.sip` & `PyQt6-6.5.0/sip/QtNetwork/qhttpmultipart.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qlocalserver.sip` & `PyQt6-6.5.0/sip/QtNetwork/qlocalserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qlocalsocket.sip` & `PyQt6-6.5.0/sip/QtNetwork/qlocalsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkaccessmanager.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkaccessmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkcookie.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkcookie.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkcookiejar.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkcookiejar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkdatagram.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkdatagram.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkdiskcache.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkdiskcache.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkinformation.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkinformation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkinterface.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkproxy.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkproxy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkreply.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkreply.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qnetworkrequest.sip` & `PyQt6-6.5.0/sip/QtNetwork/qnetworkrequest.sip`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,17 @@
         AutoDeleteReplyOnFinishAttribute,
 %If (Qt_6_3_0 -)
         ConnectionCacheExpiryTimeoutSecondsAttribute,
 %End
 %If (Qt_6_3_0 -)
         Http2CleartextAllowedAttribute,
 %End
+%If (Qt_6_5_0 -)
+        UseCredentialsAttribute,
+%End
         User,
         UserMax,
     };
 
     enum CacheLoadControl
     {
         AlwaysNetwork,
@@ -135,15 +138,21 @@
         NoLessSafeRedirectPolicy,
         SameOriginRedirectPolicy,
         UserVerifiedRedirectPolicy,
     };
 
     QString peerVerifyName() const;
     void setPeerVerifyName(const QString &peerName);
+%If (Qt_6_5_0 -)
+    QHttp1Configuration http1Configuration() const;
+%End
     QHttp2Configuration http2Configuration() const;
+%If (Qt_6_5_0 -)
+    void setHttp1Configuration(const QHttp1Configuration &configuration);
+%End
     void setHttp2Configuration(const QHttp2Configuration &configuration);
 
     enum TransferTimeoutConstant
     {
         DefaultTransferTimeoutConstant,
     };
```

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qocspresponse.sip` & `PyQt6-6.5.0/sip/QtNetwork/qocspresponse.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qpassworddigestor.sip` & `PyQt6-6.5.0/sip/QtNetwork/qpassworddigestor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qpynetwork_qhash.sip` & `PyQt6-6.5.0/sip/QtNetwork/qpynetwork_qhash.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qpynetwork_qlist.sip` & `PyQt6-6.5.0/sip/QtNetwork/qpynetwork_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qpynetwork_qmap.sip` & `PyQt6-6.5.0/sip/QtNetwork/qpynetwork_qmap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qssl.sip` & `PyQt6-6.5.0/sip/QtNetwork/qssl.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslcertificate.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslcertificate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslcertificateextension.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslcertificateextension.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslcipher.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslcipher.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslconfiguration.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslconfiguration.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qssldiffiehellmanparameters.sip` & `PyQt6-6.5.0/sip/QtNetwork/qssldiffiehellmanparameters.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslellipticcurve.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslellipticcurve.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslerror.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslerror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslkey.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslkey.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslpresharedkeyauthenticator.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslpresharedkeyauthenticator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslserver.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qsslsocket.sip` & `PyQt6-6.5.0/sip/QtNetwork/qsslsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qtcpserver.sip` & `PyQt6-6.5.0/sip/QtNetwork/qtcpserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qtcpsocket.sip` & `PyQt6-6.5.0/sip/QtNetwork/qtcpsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNetwork/qudpsocket.sip` & `PyQt6-6.5.0/sip/QtNetwork/qudpsocket.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/QtNfcmod.sip` & `PyQt6-6.5.0/sip/QtNfc/QtNfcmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qndeffilter.sip` & `PyQt6-6.5.0/sip/QtNfc/qndeffilter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qndefmessage.sip` & `PyQt6-6.5.0/sip/QtNfc/qndefmessage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qndefnfcsmartposterrecord.sip` & `PyQt6-6.5.0/sip/QtNfc/qndefnfcsmartposterrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qndefnfctextrecord.sip` & `PyQt6-6.5.0/sip/QtNfc/qndefnfctextrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qndefnfcurirecord.sip` & `PyQt6-6.5.0/sip/QtNfc/qndefnfcurirecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qndefrecord.sip` & `PyQt6-6.5.0/sip/QtNfc/qndefrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qnearfieldmanager.sip` & `PyQt6-6.5.0/sip/QtNfc/qnearfieldmanager.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtNfc/qnearfieldtarget.sip` & `PyQt6-6.5.0/sip/QtNfc/qnearfieldtarget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/QtOpenGLmod.sip` & `PyQt6-6.5.0/sip/QtOpenGL/QtOpenGLmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglbuffer.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglbuffer.sip`

 * *Files 4% similar despite different names*

```diff
@@ -86,8 +86,11 @@
         RangeInvalidateBuffer,
         RangeFlushExplicit,
         RangeUnsynchronized,
     };
 
     typedef QFlags<QOpenGLBuffer::RangeAccessFlag> RangeAccessFlags;
     void *mapRange(int offset, int count, QOpenGLBuffer::RangeAccessFlags access);
+%If (Qt_6_5_0 -)
+    void swap(QOpenGLBuffer &other);
+%End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopengldebug.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopengldebug.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglframebufferobject.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglframebufferobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_2_0.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_2_0.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_2_1.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_2_1.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_4_1_core.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_4_1_core.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglfunctions_es2.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglfunctions_es2.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglpaintdevice.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglpaintdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglpixeltransferoptions.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglpixeltransferoptions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglshaderprogram.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglshaderprogram.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopengltexture.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopengltexture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopengltextureblitter.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopengltextureblitter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopengltimerquery.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopengltimerquery.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglversionfunctions.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglversionfunctions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglversionfunctionsfactory.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglversionfunctionsfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglversionprofile.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglversionprofile.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglvertexarrayobject.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglvertexarrayobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qopenglwindow.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qopenglwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qpyopengl_qlist.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qpyopengl_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGL/qpyopengl_std_pair.sip` & `PyQt6-6.5.0/sip/QtOpenGL/qpyopengl_std_pair.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip` & `PyQt6-6.5.0/sip/QtOpenGLWidgets/QtOpenGLWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtOpenGLWidgets/qopenglwidget.sip` & `PyQt6-6.5.0/sip/QtOpenGLWidgets/qopenglwidget.sip`

 * *Files 17% similar despite different names*

```diff
@@ -57,18 +57,27 @@
 public:
     QOpenGLWidget(QWidget *parent /TransferThis/ = 0, Qt::WindowFlags flags = Qt::WindowFlags());
     virtual ~QOpenGLWidget();
     void setFormat(const QSurfaceFormat &format);
     QSurfaceFormat format() const;
     bool isValid() const;
     void makeCurrent();
+%If (Qt_6_5_0 -)
+    void makeCurrent(QOpenGLWidget::TargetBuffer targetBuffer);
+%End
     void doneCurrent();
     QOpenGLContext *context() const;
     GLuint defaultFramebufferObject() const;
+%If (Qt_6_5_0 -)
+    GLuint defaultFramebufferObject(QOpenGLWidget::TargetBuffer targetBuffer) const;
+%End
     QImage grabFramebuffer();
+%If (Qt_6_5_0 -)
+    QImage grabFramebuffer(QOpenGLWidget::TargetBuffer targetBuffer);
+%End
 
 signals:
     void aboutToCompose();
     void frameSwapped();
     void aboutToResize();
     void resized();
 
@@ -89,8 +98,20 @@
         PartialUpdate,
     };
 
     void setUpdateBehavior(QOpenGLWidget::UpdateBehavior updateBehavior);
     QOpenGLWidget::UpdateBehavior updateBehavior() const;
     GLenum textureFormat() const;
     void setTextureFormat(GLenum texFormat);
+%If (Qt_6_5_0 -)
+
+    enum TargetBuffer
+    {
+        LeftBuffer,
+        RightBuffer,
+    };
+
+%End
+%If (Qt_6_5_0 -)
+    QOpenGLWidget::TargetBuffer currentTargetBuffer() const;
+%End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtPdf/QtPdfmod.sip` & `PyQt6-6.5.0/sip/QtPdf/QtPdfmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfbookmarkmodel.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfbookmarkmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfdocument.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfdocument.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfdocumentrenderoptions.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfdocumentrenderoptions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdflink.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdflink.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfpagenavigator.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfpagenavigator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfpagerenderer.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfpagerenderer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfsearchmodel.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfsearchmodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdf/qpdfselection.sip` & `PyQt6-6.5.0/sip/QtPdf/qpdfselection.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdfWidgets/QtPdfWidgetsmod.sip` & `PyQt6-6.5.0/sip/QtPdfWidgets/QtPdfWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPdfWidgets/qpdfview.sip` & `PyQt6-6.5.0/sip/QtPdfWidgets/qpdfview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/QtPositioningmod.sip` & `PyQt6-6.5.0/sip/QtPositioning/QtPositioningmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeoaddress.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeoaddress.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeoareamonitorinfo.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeoareamonitorinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeoareamonitorsource.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeoareamonitorsource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeocircle.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeocircle.sip`

 * *Files 14% similar despite different names*

```diff
@@ -41,7 +41,13 @@
     void translate(double degreesLatitude, double degreesLongitude);
     QGeoCircle translated(double degreesLatitude, double degreesLongitude) const;
     QString toString() const;
     void extendCircle(const QGeoCoordinate &coordinate);
 };
 
 %End
+%If (Qt_6_5_0 -)
+QDataStream &operator<<(QDataStream &stream, const QGeoCircle &circle) /ReleaseGIL/;
+%End
+%If (Qt_6_5_0 -)
+QDataStream &operator>>(QDataStream &stream, QGeoCircle &circle /Constrained/) /ReleaseGIL/;
+%End
```

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeocoordinate.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeocoordinate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeolocation.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeolocation.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeopath.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeopath.sip`

 * *Files 12% similar despite different names*

```diff
@@ -50,7 +50,13 @@
     void removeCoordinate(qsizetype index);
     QString toString() const;
     qsizetype size() const;
     void clearPath();
 };
 
 %End
+%If (Qt_6_5_0 -)
+QDataStream &operator<<(QDataStream &stream, const QGeoPath &path) /ReleaseGIL/;
+%End
+%If (Qt_6_5_0 -)
+QDataStream &operator>>(QDataStream &stream, QGeoPath &path /Constrained/) /ReleaseGIL/;
+%End
```

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeopolygon.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeopolygon.sip`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,13 @@
     void removeHole(qsizetype index);
     qsizetype holesCount() const;
     void setPerimeter(const QList<QGeoCoordinate> &path);
     const QList<QGeoCoordinate> &perimeter() const;
 };
 
 %End
+%If (Qt_6_5_0 -)
+QDataStream &operator<<(QDataStream &stream, const QGeoPolygon &polygon) /ReleaseGIL/;
+%End
+%If (Qt_6_5_0 -)
+QDataStream &operator>>(QDataStream &stream, QGeoPolygon &polygon /Constrained/) /ReleaseGIL/;
+%End
```

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeopositioninfo.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeopositioninfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeopositioninfosource.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeopositioninfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeorectangle.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeorectangle.sip`

 * *Files 20% similar despite different names*

```diff
@@ -58,7 +58,13 @@
     QGeoRectangle &operator|=(const QGeoRectangle &rectangle);
     QGeoRectangle operator|(const QGeoRectangle &rectangle) const;
     QString toString() const;
     void extendRectangle(const QGeoCoordinate &coordinate);
 };
 
 %End
+%If (Qt_6_5_0 -)
+QDataStream &operator<<(QDataStream &stream, const QGeoRectangle &rectangle) /ReleaseGIL/;
+%End
+%If (Qt_6_5_0 -)
+QDataStream &operator>>(QDataStream &stream, QGeoRectangle &rectangle /Constrained/) /ReleaseGIL/;
+%End
```

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeosatelliteinfo.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeosatelliteinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeosatelliteinfosource.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeosatelliteinfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qgeoshape.sip` & `PyQt6-6.5.0/sip/QtPositioning/qgeoshape.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qnmeapositioninfosource.sip` & `PyQt6-6.5.0/sip/QtPositioning/qnmeapositioninfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPositioning/qnmeasatelliteinfosource.sip` & `PyQt6-6.5.0/sip/QtPositioning/qnmeasatelliteinfosource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/QtPrintSupportmod.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/QtPrintSupportmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qabstractprintdialog.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qabstractprintdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qpagesetupdialog.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qpagesetupdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qprintdialog.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qprintdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qprintengine.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qprintengine.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qprinter.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qprinter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qprinterinfo.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qprinterinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qprintpreviewdialog.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qprintpreviewdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qprintpreviewwidget.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qprintpreviewwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtPrintSupport/qpyprintsupport_qlist.sip` & `PyQt6-6.5.0/sip/QtPrintSupport/qpyprintsupport_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/QtQmlmod.sip` & `PyQt6-6.5.0/sip/QtQml/QtQmlmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qjsengine.sip` & `PyQt6-6.5.0/sip/QtQml/qjsengine.sip`

 * *Files 3% similar despite different names*

```diff
@@ -182,14 +182,23 @@
 public:
 %If (Qt_6_2_0 -)
     bool registerModule(const QString &moduleName, const QJSValue &value);
 %End
 %If (Qt_6_2_0 -)
     QJSValue newSymbol(const QString &name);
 %End
+%If (Qt_6_5_0 -)
+    QJSValue toScriptValue(const QVariant &value);
+%End
+%If (Qt_6_5_0 -)
+    QJSManagedValue toManagedValue(const QVariant &value);
+%End
+%If (Qt_6_5_0 -)
+    QJSPrimitiveValue toPrimitiveValue(const QVariant &value);
+%End
 };
 
 QJSEngine *qjsEngine(const QObject *);
 
 %ModuleHeaderCode
 #include "qpyqml_api.h"
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtQml/qjsmanagedvalue.sip` & `PyQt6-6.5.0/sip/QtQml/qjsmanagedvalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qjsprimitivevalue.sip` & `PyQt6-6.5.0/sip/QtQml/qjsprimitivevalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qjsvalue.sip` & `PyQt6-6.5.0/sip/QtQml/qjsvalue.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qjsvalueiterator.sip` & `PyQt6-6.5.0/sip/QtQml/qjsvalueiterator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qmlattachedpropertiesobject.sip` & `PyQt6-6.5.0/sip/QtQml/qmlattachedpropertiesobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qmlregistertype.sip` & `PyQt6-6.5.0/sip/QtQml/qmlregistertype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qpyqmllistproperty.sip` & `PyQt6-6.5.0/sip/QtQml/qpyqmllistproperty.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqml.sip` & `PyQt6-6.5.0/sip/QtQml/qqml.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlabstracturlinterceptor.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlabstracturlinterceptor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlapplicationengine.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlapplicationengine.sip`

 * *Files 12% similar despite different names*

```diff
@@ -26,23 +26,29 @@
 #include <qqmlapplicationengine.h>
 %End
 
 public:
     QQmlApplicationEngine(QObject *parent /TransferThis/ = 0);
     QQmlApplicationEngine(const QUrl &url, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
     QQmlApplicationEngine(const QString &filePath, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
+%If (Qt_6_5_0 -)
+    QQmlApplicationEngine(QAnyStringView uri, QAnyStringView typeName, QObject *parent /TransferThis/ = 0);
+%End
     virtual ~QQmlApplicationEngine();
     QList<QObject *> rootObjects() const;
 
 public slots:
     void load(const QUrl &url) /ReleaseGIL/;
     void load(const QString &filePath) /ReleaseGIL/;
     void loadData(const QByteArray &data, const QUrl &url = QUrl()) /ReleaseGIL/;
     void setExtraFileSelectors(const QStringList &extraFileSelectors);
     void setInitialProperties(const QVariantMap &initialProperties);
+%If (Qt_6_5_0 -)
+    void loadFromModule(QAnyStringView uri, QAnyStringView typeName);
+%End
 
 signals:
     void objectCreated(QObject *object, const QUrl &url);
 %If (Qt_6_4_0 -)
     void objectCreationFailed(const QUrl &url);
 %End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlcomponent.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlcomponent.sip`

 * *Files 20% similar despite different names*

```diff
@@ -34,26 +34,35 @@
     };
 
     QQmlComponent(QQmlEngine *, QObject *parent /TransferThis/ = 0);
     QQmlComponent(QQmlEngine *, const QString &fileName, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
     QQmlComponent(QQmlEngine *, const QString &fileName, QQmlComponent::CompilationMode mode, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
     QQmlComponent(QQmlEngine *, const QUrl &url, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
     QQmlComponent(QQmlEngine *, const QUrl &url, QQmlComponent::CompilationMode mode, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
+%If (Qt_6_5_0 -)
+    QQmlComponent(QQmlEngine *engine, QAnyStringView uri, QAnyStringView typeName, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
+%End
+%If (Qt_6_5_0 -)
+    QQmlComponent(QQmlEngine *engine, QAnyStringView uri, QAnyStringView typeName, QQmlComponent::CompilationMode mode, QObject *parent /TransferThis/ = 0) /ReleaseGIL/;
+%End
     QQmlComponent(QObject *parent /TransferThis/ = 0);
     virtual ~QQmlComponent();
 
     enum Status
     {
         Null,
         Ready,
         Loading,
         Error,
     };
 
     QQmlComponent::Status status() const;
+%If (Qt_6_5_0 -)
+    bool isBound() const;
+%End
     bool isNull() const;
     bool isReady() const;
     bool isError() const;
     bool isLoading() const;
     QList<QQmlError> errors() const;
     qreal progress() const;
     QUrl url() const;
@@ -64,14 +73,17 @@
     void create(QQmlIncubator &, QQmlContext *context = 0, QQmlContext *forContext = 0);
     QQmlContext *creationContext() const;
 
 public slots:
     void loadUrl(const QUrl &url) /ReleaseGIL/;
     void loadUrl(const QUrl &url, QQmlComponent::CompilationMode mode) /ReleaseGIL/;
     void setData(const QByteArray &, const QUrl &baseUrl);
+%If (Qt_6_5_0 -)
+    void loadFromModule(QAnyStringView uri, QAnyStringView typeName, QQmlComponent::CompilationMode mode = QQmlComponent::PreferSynchronous);
+%End
 
 signals:
     void statusChanged(QQmlComponent::Status);
     void progressChanged(qreal);
 
 public:
     QQmlEngine *engine() const;
```

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlcontext.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlcontext.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlengine.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlengine.sip`

 * *Files 6% similar despite different names*

```diff
@@ -114,23 +114,48 @@
         else
         {
             sipRes = Py_None;
             Py_INCREF(sipRes);
         }
 %End
 
+%If (Qt_6_5_0 -)
+    SIP_PYOBJECT singletonInstance(QAnyStringView moduleName, QAnyStringView typeName) /TypeHint="QObject"/;
+%MethodCode
+        QJSValue instance = sipCpp->singletonInstance<QJSValue>(*a0, *a1);
+        
+        if (instance.isQObject())
+        {
+            sipRes = sipConvertFromType(instance.toQObject(), sipType_QObject, NULL);
+                
+            if (!sipRes)
+                sipError = sipErrorFail;
+        }
+        else
+        {
+            sipRes = Py_None;
+            Py_INCREF(sipRes);
+        }
+%End
+
+%End
     void addUrlInterceptor(QQmlAbstractUrlInterceptor *urlInterceptor);
     void removeUrlInterceptor(QQmlAbstractUrlInterceptor *urlInterceptor);
     QUrl interceptUrl(const QUrl &url, QQmlAbstractUrlInterceptor::DataType type) const;
 %If (Qt_6_2_0 -)
     QList<QQmlAbstractUrlInterceptor *> urlInterceptors() const;
 %End
 %If (Qt_6_3_0 -)
     void clearSingletons();
 %End
+
+signals:
+%If (Qt_6_5_0 -)
+    void offlineStoragePathChanged();
+%End
 };
 
 class QQmlImageProviderBase : QObject
 {
 %TypeHeaderCode
 #include <qqmlengine.h>
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlerror.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlerror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlexpression.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlexpression.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlextensionplugin.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlextensionplugin.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlfileselector.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlfileselector.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlincubator.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlincubator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmllist.sip` & `PyQt6-6.5.0/sip/QtQml/qqmllist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlnetworkaccessmanagerfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlparserstatus.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlparserstatus.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlproperty.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlproperty.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlpropertymap.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlpropertymap.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlpropertyvaluesource.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlpropertyvaluesource.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQml/qqmlscriptstring.sip` & `PyQt6-6.5.0/sip/QtQml/qqmlscriptstring.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/QtQuickmod.sip` & `PyQt6-6.5.0/sip/QtQuick/QtQuickmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickframebufferobject.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickframebufferobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickgraphicsconfiguration.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickgraphicsconfiguration.sip`

 * *Files 21% similar despite different names*

```diff
@@ -33,8 +33,44 @@
     void setDeviceExtensions(const QByteArrayList &extensions);
     QByteArrayList deviceExtensions() const;
     void setDepthBufferFor2D(bool enable);
     bool isDepthBufferEnabledFor2D() const;
 %If (Qt_6_1_0 -)
     static QByteArrayList preferredInstanceExtensions();
 %End
+%If (Qt_6_5_0 -)
+    void setDebugLayer(bool enable);
+%End
+%If (Qt_6_5_0 -)
+    bool isDebugLayerEnabled() const;
+%End
+%If (Qt_6_5_0 -)
+    void setDebugMarkers(bool enable);
+%End
+%If (Qt_6_5_0 -)
+    bool isDebugMarkersEnabled() const;
+%End
+%If (Qt_6_5_0 -)
+    void setPreferSoftwareDevice(bool enable);
+%End
+%If (Qt_6_5_0 -)
+    bool prefersSoftwareDevice() const;
+%End
+%If (Qt_6_5_0 -)
+    void setAutomaticPipelineCache(bool enable);
+%End
+%If (Qt_6_5_0 -)
+    bool isAutomaticPipelineCacheEnabled() const;
+%End
+%If (Qt_6_5_0 -)
+    void setPipelineCacheSaveFile(const QString &filename);
+%End
+%If (Qt_6_5_0 -)
+    QString pipelineCacheSaveFile() const;
+%End
+%If (Qt_6_5_0 -)
+    void setPipelineCacheLoadFile(const QString &filename);
+%End
+%If (Qt_6_5_0 -)
+    QString pipelineCacheLoadFile() const;
+%End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickgraphicsdevice.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickgraphicsdevice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickimageprovider.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickimageprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickitem.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickitemgrabresult.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickitemgrabresult.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickpainteditem.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickpainteditem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickrendercontrol.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickrendercontrol.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickrendertarget.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickrendertarget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquicktextdocument.sip` & `PyQt6-6.5.0/sip/QtWidgets/qfilesystemmodel.sip`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-// qquicktextdocument.sip generated by MetaSIP
+// qfilesystemmodel.sip generated by MetaSIP
 //
-// This file is part of the QtQuick Python extension module.
+// This file is part of the QtWidgets Python extension module.
 //
 // Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
@@ -15,18 +15,7 @@
 // If you do not wish to use this file under the terms of the GPL version 3.0
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
-
-class QQuickTextDocument : QObject
-{
-%TypeHeaderCode
-#include <qquicktextdocument.h>
-%End
-
-public:
-    QQuickTextDocument(QQuickItem *parent /TransferThis/);
-    QTextDocument *textDocument() const;
-};
```

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickview.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qquickwindow.sip` & `PyQt6-6.5.0/sip/QtQuick/qquickwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgflatcolormaterial.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgflatcolormaterial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsggeometry.sip` & `PyQt6-6.5.0/sip/QtQuick/qsggeometry.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgimagenode.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgimagenode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgmaterial.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgmaterial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgmaterialtype.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgmaterialtype.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgnode.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgnode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgrectanglenode.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgrectanglenode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgrendererinterface.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgrendererinterface.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgrendernode.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgrendernode.sip`

 * *Files 3% similar despite different names*

```diff
@@ -72,8 +72,11 @@
     virtual void releaseResources();
     virtual QSGRenderNode::RenderingFlags flags() const;
     virtual QRectF rect() const;
     const QMatrix4x4 *matrix() const;
     const QSGClipNode *clipList() const;
     qreal inheritedOpacity() const;
     virtual void prepare();
+%If (Qt_6_5_0 -)
+    const QMatrix4x4 *projectionMatrix() const;
+%End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgsimplerectnode.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgsimplerectnode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgsimpletexturenode.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgsimpletexturenode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgtexture.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgtexture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgtexture_platform.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgtexture_platform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgtexturematerial.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgtexturematerial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgtextureprovider.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgtextureprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick/qsgvertexcolormaterial.sip` & `PyQt6-6.5.0/sip/QtQuick/qsgvertexcolormaterial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick3D/QtQuick3Dmod.sip` & `PyQt6-6.5.0/sip/QtQuick3D/QtQuick3Dmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick3D/qquick3d.sip` & `PyQt6-6.5.0/sip/QtQuick3D/qquick3d.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick3D/qquick3dgeometry.sip` & `PyQt6-6.5.0/sip/QtQuick3D/qquick3dgeometry.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick3D/qquick3dobject.sip` & `PyQt6-6.5.0/sip/QtQuick3D/qquick3dobject.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuick3D/qquick3dtexturedata.sip` & `PyQt6-6.5.0/sip/QtQuick3D/qquick3dtexturedata.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuickWidgets/QtQuickWidgetsmod.sip` & `PyQt6-6.5.0/sip/QtQuickWidgets/QtQuickWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtQuickWidgets/qquickwidget.sip` & `PyQt6-6.5.0/sip/QtQuickWidgets/qquickwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/QtRemoteObjectsmod.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/QtRemoteObjectsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectabstractitemmodelreplica.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectdynamicreplica.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectnode.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectnode.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectregistry.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectregistry.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/qremoteobjectreplica.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/qremoteobjectreplica.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtRemoteObjects/qtremoteobjectglobal.sip` & `PyQt6-6.5.0/sip/QtRemoteObjects/qtremoteobjectglobal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/QtSensorsmod.sip` & `PyQt6-6.5.0/sip/QtSensors/QtSensorsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qaccelerometer.sip` & `PyQt6-6.5.0/sip/QtSensors/qaccelerometer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qambientlightsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qambientlightsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qambienttemperaturesensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qambienttemperaturesensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qcompass.sip` & `PyQt6-6.5.0/sip/QtSensors/qcompass.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qgyroscope.sip` & `PyQt6-6.5.0/sip/QtSensors/qgyroscope.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qhumiditysensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qhumiditysensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qirproximitysensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qirproximitysensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qlidsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qlidsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qlightsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qlightsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qmagnetometer.sip` & `PyQt6-6.5.0/sip/QtSensors/qmagnetometer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qorientationsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qorientationsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qpressuresensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qpressuresensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qproximitysensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qproximitysensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qrotationsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qrotationsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qtapsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qtapsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSensors/qtiltsensor.sip` & `PyQt6-6.5.0/sip/QtSensors/qtiltsensor.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSerialPort/QtSerialPortmod.sip` & `PyQt6-6.5.0/sip/QtSerialPort/QtSerialPortmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSerialPort/qserialport.sip` & `PyQt6-6.5.0/sip/QtSerialPort/qserialport.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSerialPort/qserialportinfo.sip` & `PyQt6-6.5.0/sip/QtSerialPort/qserialportinfo.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/QtSqlmod.sip` & `PyQt6-6.5.0/sip/QtSql/QtSqlmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqldatabase.sip` & `PyQt6-6.5.0/sip/QtSql/qsqldatabase.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqldriver.sip` & `PyQt6-6.5.0/sip/QtSql/qsqldriver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlerror.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlerror.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlfield.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlfield.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlindex.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlindex.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlquery.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlquery.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlquerymodel.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlquerymodel.sip`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,24 @@
     virtual QVariant data(const QModelIndex &item, int role = Qt::DisplayRole) const;
     virtual QVariant headerData(int section, Qt::Orientation orientation, int role = Qt::DisplayRole) const;
     virtual bool setHeaderData(int section, Qt::Orientation orientation, const QVariant &value, int role = Qt::EditRole);
     virtual bool insertColumns(int column, int count, const QModelIndex &parent = QModelIndex());
     virtual bool removeColumns(int column, int count, const QModelIndex &parent = QModelIndex());
     void setQuery(const QSqlQuery &query);
     void setQuery(const QString &query, const QSqlDatabase &db = QSqlDatabase());
+%If (Qt_6_5_0 -)
+    const QSqlQuery &query() const;
+%MethodCode
+        sipRes = const_cast<QSqlQuery *>(&sipCpp->query(Qt::Disambiguated));
+%End
+
+%End
+%If (- Qt_6_5_0)
     QSqlQuery query() const;
+%End
     virtual void clear();
     QSqlError lastError() const;
     virtual void fetchMore(const QModelIndex &parent = QModelIndex());
     virtual bool canFetchMore(const QModelIndex &parent = QModelIndex()) const;
 
 protected:
     virtual void queryChange();
```

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlrecord.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlrecord.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlrelationaldelegate.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlrelationaldelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlrelationaltablemodel.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlrelationaltablemodel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqlresult.sip` & `PyQt6-6.5.0/sip/QtSql/qsqlresult.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSql/qsqltablemodel.sip` & `PyQt6-6.5.0/sip/QtSql/qsqltablemodel.sip`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,17 @@
 protected:
     virtual bool updateRowInTable(int row, const QSqlRecord &values);
     virtual bool insertRowIntoTable(const QSqlRecord &values);
     virtual bool deleteRowFromTable(int row);
     virtual QString orderByClause() const;
     virtual QString selectStatement() const;
     void setPrimaryKey(const QSqlIndex &key);
+%If (- Qt_6_5_0)
     void setQuery(const QSqlQuery &query);
+%End
     virtual QModelIndex indexInQuery(const QModelIndex &item) const;
     QSqlRecord primaryValues(int row) const;
 
 public:
     virtual bool selectRow(int row);
     QSqlRecord record() const;
     QSqlRecord record(int row) const;
```

### Comparing `PyQt6-6.4.2/sip/QtSql/qtsqlglobal.sip` & `PyQt6-6.5.0/sip/QtSql/qtsqlglobal.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSvg/QtSvgmod.sip` & `PyQt6-6.5.0/sip/QtSvg/QtSvgmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSvg/qsvggenerator.sip` & `PyQt6-6.5.0/sip/QtSvg/qsvggenerator.sip`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 {
 %TypeHeaderCode
 #include <qsvggenerator.h>
 %End
 
 public:
     QSvgGenerator();
+%If (Qt_6_5_0 -)
+    explicit QSvgGenerator(QSvgGenerator::SvgVersion version);
+%End
     virtual ~QSvgGenerator();
     QSize size() const;
     void setSize(const QSize &size);
     QString fileName() const;
     void setFileName(const QString &fileName);
     QIODevice *outputDevice() const;
     void setOutputDevice(QIODevice *outputDevice);
@@ -45,8 +48,22 @@
     QRectF viewBoxF() const;
     void setViewBox(const QRect &viewBox);
     void setViewBox(const QRectF &viewBox);
 
 protected:
     virtual QPaintEngine *paintEngine() const;
     virtual int metric(QPaintDevice::PaintDeviceMetric metric) const;
+
+public:
+%If (Qt_6_5_0 -)
+
+    enum class SvgVersion
+    {
+        SvgTiny12,
+        Svg11,
+    };
+
+%End
+%If (Qt_6_5_0 -)
+    QSvgGenerator::SvgVersion svgVersion() const;
+%End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtSvg/qsvgrenderer.sip` & `PyQt6-6.5.0/sip/QtSvg/qsvgrenderer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSvgWidgets/QtSvgWidgetsmod.sip` & `PyQt6-6.5.0/sip/QtSvgWidgets/QtSvgWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSvgWidgets/qgraphicssvgitem.sip` & `PyQt6-6.5.0/sip/QtSvgWidgets/qgraphicssvgitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtSvgWidgets/qsvgwidget.sip` & `PyQt6-6.5.0/sip/QtSvgWidgets/qsvgwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTest/QtTestmod.sip` & `PyQt6-6.5.0/sip/QtTest/QtTestmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTest/qabstractitemmodeltester.sip` & `PyQt6-6.5.0/sip/QtTest/qabstractitemmodeltester.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTest/qsignalspy.sip` & `PyQt6-6.5.0/sip/QtTest/qsignalspy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTest/qtestkeyboard.sip` & `PyQt6-6.5.0/sip/QtTest/qtestkeyboard.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTest/qtestmouse.sip` & `PyQt6-6.5.0/sip/QtTest/qtestmouse.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTest/qtestsystem.sip` & `PyQt6-6.5.0/sip/QtTest/qtestsystem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTextToSpeech/QtTextToSpeechmod.sip` & `PyQt6-6.5.0/sip/QtTextToSpeech/QtTextToSpeechmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTextToSpeech/qtexttospeech.sip` & `PyQt6-6.5.0/sip/QtTextToSpeech/qtexttospeech.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtTextToSpeech/qvoice.sip` & `PyQt6-6.5.0/sip/QtTextToSpeech/qvoice.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebChannel/QtWebChannelmod.sip` & `PyQt6-6.5.0/sip/QtWebChannel/QtWebChannelmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebChannel/qwebchannel.sip` & `PyQt6-6.5.0/sip/QtWebChannel/qwebchannel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebChannel/qwebchannelabstracttransport.sip` & `PyQt6-6.5.0/sip/QtWebChannel/qwebchannelabstracttransport.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/QtWebSocketsmod.sip` & `PyQt6-6.5.0/sip/QtWebSockets/QtWebSocketsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/qmaskgenerator.sip` & `PyQt6-6.5.0/sip/QtWebSockets/qmaskgenerator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/qwebsocket.sip` & `PyQt6-6.5.0/sip/QtWebSockets/qwebsocket.sip`

 * *Files 2% similar despite different names*

```diff
@@ -166,10 +166,15 @@
 public:
 %If (Qt_6_4_0 -)
     QWebSocketHandshakeOptions handshakeOptions() const;
 %End
 %If (Qt_6_4_0 -)
     QString subprotocol() const;
 %End
+
+signals:
+%If (Qt_6_5_0 -)
+    void errorOccurred(QAbstractSocket::SocketError error);
+%End
 };
 
 %End
```

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/qwebsocketcorsauthenticator.sip` & `PyQt6-6.5.0/sip/QtWebSockets/qwebsocketcorsauthenticator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/qwebsockethandshakeoptions.sip` & `PyQt6-6.5.0/sip/QtWebSockets/qwebsockethandshakeoptions.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/qwebsocketprotocol.sip` & `PyQt6-6.5.0/sip/QtWebSockets/qwebsocketprotocol.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWebSockets/qwebsocketserver.sip` & `PyQt6-6.5.0/sip/QtWebSockets/qwebsocketserver.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/QtWidgetsmod.sip` & `PyQt6-6.5.0/sip/QtWidgets/QtWidgetsmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qabstractbutton.sip` & `PyQt6-6.5.0/sip/QtWidgets/qabstractbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qabstractitemdelegate.sip` & `PyQt6-6.5.0/sip/QtWidgets/qabstractitemdelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qabstractitemview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qabstractitemview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qabstractscrollarea.sip` & `PyQt6-6.5.0/sip/QtWidgets/qabstractscrollarea.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qabstractslider.sip` & `PyQt6-6.5.0/sip/QtWidgets/qabstractslider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qabstractspinbox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qabstractspinbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qapplication.sip` & `PyQt6-6.5.0/sip/QtWidgets/qapplication.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qboxlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qboxlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qbuttongroup.sip` & `PyQt6-6.5.0/sip/QtWidgets/qbuttongroup.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcalendarwidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcalendarwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcheckbox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcheckbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcolordialog.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcolordialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcolumnview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcolumnview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcombobox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcombobox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcommandlinkbutton.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcommandlinkbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcommonstyle.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcommonstyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qcompleter.sip` & `PyQt6-6.5.0/sip/QtWidgets/qcompleter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdatawidgetmapper.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdatawidgetmapper.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdatetimeedit.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdatetimeedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdial.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdial.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdialog.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdialogbuttonbox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdialogbuttonbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdockwidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdockwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qdrawutil.sip` & `PyQt6-6.5.0/sip/QtWidgets/qdrawutil.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qerrormessage.sip` & `PyQt6-6.5.0/sip/QtWidgets/qerrormessage.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qfileiconprovider.sip` & `PyQt6-6.5.0/sip/QtWidgets/qfileiconprovider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qfilesystemmodel.sip` & `PyQt6-6.5.0/uic/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-// qfilesystemmodel.sip generated by MetaSIP
-//
-// This file is part of the QtWidgets Python extension module.
-//
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
-// 
-// This file is part of PyQt6.
-// 
-// This file may be used under the terms of the GNU General Public License
-// version 3.0 as published by the Free Software Foundation and appearing in
-// the file LICENSE included in the packaging of this file.  Please review the
-// following information to ensure the GNU General Public License version 3.0
-// requirements will be met: http://www.gnu.org/copyleft/gpl.html.
-// 
-// If you do not wish to use this file under the terms of the GPL version 3.0
-// then you may purchase a commercial license.  For more information contact
-// info@riverbankcomputing.com.
-// 
-// This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
-// WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
+# Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+# 
+# This file is part of PyQt6.
+# 
+# This file may be used under the terms of the GNU General Public License
+# version 3.0 as published by the Free Software Foundation and appearing in
+# the file LICENSE included in the packaging of this file.  Please review the
+# following information to ensure the GNU General Public License version 3.0
+# requirements will be met: http://www.gnu.org/copyleft/gpl.html.
+# 
+# If you do not wish to use this file under the terms of the GPL version 3.0
+# then you may purchase a commercial license.  For more information contact
+# info@riverbankcomputing.com.
+# 
+# This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
+# WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
+
+# The public API.
+from .compile_ui import compileUi, compileUiDir
+from .load_ui import loadUi, loadUiType
+from .objcreator import widgetPluginPath
+from .ui_file import UIFile
```

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qfocusframe.sip` & `PyQt6-6.5.0/sip/QtWidgets/qfocusframe.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qfontcombobox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qfontcombobox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qfontdialog.sip` & `PyQt6-6.5.0/sip/QtWidgets/qfontdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qformlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qformlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qframe.sip` & `PyQt6-6.5.0/sip/QtWidgets/qframe.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgesture.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgesture.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgesturerecognizer.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgesturerecognizer.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicsanchorlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicsanchorlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicseffect.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicseffect.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicsgridlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicsgridlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicsitem.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicsitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicslayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicslayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicslayoutitem.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicslayoutitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicslinearlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicslinearlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicsproxywidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicsproxywidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicsscene.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicsscene.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicssceneevent.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicssceneevent.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicstransform.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicstransform.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicsview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicsview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgraphicswidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgraphicswidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgridlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgridlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qgroupbox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qgroupbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qheaderview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qheaderview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qinputdialog.sip` & `PyQt6-6.5.0/sip/QtWidgets/qinputdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qitemdelegate.sip` & `PyQt6-6.5.0/sip/QtWidgets/qitemdelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qitemeditorfactory.sip` & `PyQt6-6.5.0/sip/QtWidgets/qitemeditorfactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qkeysequenceedit.sip` & `PyQt6-6.5.0/sip/QtWidgets/qkeysequenceedit.sip`

 * *Files 12% similar despite different names*

```diff
@@ -52,8 +52,22 @@
 public:
 %If (Qt_6_4_0 -)
     void setClearButtonEnabled(bool enable);
 %End
 %If (Qt_6_4_0 -)
     bool isClearButtonEnabled() const;
 %End
+%If (Qt_6_5_0 -)
+    qsizetype maximumSequenceLength() const;
+%End
+%If (Qt_6_5_0 -)
+    void setFinishingKeyCombinations(const QList<QKeyCombination> &finishingKeyCombinations);
+%End
+%If (Qt_6_5_0 -)
+    QList<QKeyCombination> finishingKeyCombinations() const;
+%End
+
+public slots:
+%If (Qt_6_5_0 -)
+    void setMaximumSequenceLength(qsizetype count);
+%End
 };
```

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlabel.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlabel.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlayoutitem.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlayoutitem.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlcdnumber.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlcdnumber.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlineedit.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlineedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlistview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlistview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qlistwidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qlistwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qmainwindow.sip` & `PyQt6-6.5.0/sip/QtWidgets/qmainwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qmdiarea.sip` & `PyQt6-6.5.0/sip/QtWidgets/qmdiarea.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qmdisubwindow.sip` & `PyQt6-6.5.0/sip/QtWidgets/qmdisubwindow.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qmenu.sip` & `PyQt6-6.5.0/sip/QtWidgets/qmenu.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qmenubar.sip` & `PyQt6-6.5.0/sip/QtWidgets/qmenubar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qmessagebox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qmessagebox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qplaintextedit.sip` & `PyQt6-6.5.0/sip/QtWidgets/qplaintextedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qprogressbar.sip` & `PyQt6-6.5.0/sip/QtWidgets/qprogressbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qprogressdialog.sip` & `PyQt6-6.5.0/sip/QtWidgets/qprogressdialog.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qproxystyle.sip` & `PyQt6-6.5.0/sip/QtWidgets/qproxystyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qpushbutton.sip` & `PyQt6-6.5.0/sip/QtWidgets/qpushbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qpywidgets_qlist.sip` & `PyQt6-6.5.0/sip/QtWidgets/qpywidgets_qlist.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qradiobutton.sip` & `PyQt6-6.5.0/sip/QtWidgets/qradiobutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qrubberband.sip` & `PyQt6-6.5.0/sip/QtWidgets/qrubberband.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qscrollarea.sip` & `PyQt6-6.5.0/sip/QtWidgets/qscrollarea.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qscrollbar.sip` & `PyQt6-6.5.0/sip/QtWidgets/qscrollbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qscroller.sip` & `PyQt6-6.5.0/sip/QtWidgets/qscroller.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qscrollerproperties.sip` & `PyQt6-6.5.0/sip/QtWidgets/qscrollerproperties.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qsizegrip.sip` & `PyQt6-6.5.0/sip/QtWidgets/qsizegrip.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qsizepolicy.sip` & `PyQt6-6.5.0/sip/QtWidgets/qsizepolicy.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qslider.sip` & `PyQt6-6.5.0/sip/QtWidgets/qslider.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qspinbox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qspinbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qsplashscreen.sip` & `PyQt6-6.5.0/sip/QtWidgets/qsplashscreen.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qsplitter.sip` & `PyQt6-6.5.0/sip/QtWidgets/qsplitter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstackedlayout.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstackedlayout.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstackedwidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstackedwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstatusbar.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstatusbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstyle.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstyle.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstyleditemdelegate.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstyleditemdelegate.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstylefactory.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstylefactory.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstyleoption.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstyleoption.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qstylepainter.sip` & `PyQt6-6.5.0/sip/QtWidgets/qstylepainter.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qsystemtrayicon.sip` & `PyQt6-6.5.0/sip/QtWidgets/qsystemtrayicon.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtabbar.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtabbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtableview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtableview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtablewidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtablewidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtabwidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtabwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtextbrowser.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtextbrowser.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtextedit.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtextedit.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtoolbar.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtoolbar.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtoolbox.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtoolbox.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtoolbutton.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtoolbutton.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtooltip.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtooltip.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtreeview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtreeview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtreewidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtreewidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qtreewidgetitemiterator.sip` & `PyQt6-6.5.0/sip/QtWidgets/qtreewidgetitemiterator.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qundoview.sip` & `PyQt6-6.5.0/sip/QtWidgets/qundoview.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qwhatsthis.sip` & `PyQt6-6.5.0/sip/QtWidgets/qwhatsthis.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qwidget.sip` & `PyQt6-6.5.0/sip/QtWidgets/qwidget.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qwidgetaction.sip` & `PyQt6-6.5.0/sip/QtWidgets/qwidgetaction.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtWidgets/qwizard.sip` & `PyQt6-6.5.0/sip/QtWidgets/qwizard.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtXml/QtXmlmod.sip` & `PyQt6-6.5.0/sip/QtXml/QtXmlmod.sip`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/sip/QtXml/qdom.sip` & `PyQt6-6.5.0/sip/QtXml/qdom.sip`

 * *Files 12% similar despite different names*

```diff
@@ -212,20 +212,88 @@
     QDomAttr createAttributeNS(const QString &nsURI, const QString &qName);
     QDomNodeList elementsByTagNameNS(const QString &nsURI, const QString &localName);
     QDomElement elementById(const QString &elementId);
     QDomDocumentType doctype() const;
     QDomImplementation implementation() const;
     QDomElement documentElement() const;
     QDomNode::NodeType nodeType() const;
+%If (Qt_6_5_0 -)
+
+    enum class ParseOption
+    {
+        Default,
+        UseNamespaceProcessing,
+        PreserveSpacingOnlyNodes,
+    };
+
+%End
+%If (Qt_6_5_0 -)
+    typedef QFlags<QDomDocument::ParseOption> ParseOptions;
+%End
+%If (Qt_6_5_0 -)
+    SIP_PYOBJECT setContent(QXmlStreamReader *reader, QDomDocument::ParseOptions options = QDomDocument::ParseOption::Default) /ReleaseGIL,TypeHint="Tuple [bool, str, int, int]"/;
+%MethodCode
+        QDomDocument::ParseResult pr;
+        
+        Py_BEGIN_ALLOW_THREADS
+        pr = sipCpp->setContent(a0, *a1);
+        Py_END_ALLOW_THREADS
+        
+        return sipBuildResult(NULL, "(bNnn)",
+                (int)bool(pr),
+                new QString(pr.errorMessage), sipType_QString, NULL,
+                (long long)pr.errorLine,
+                (long long)pr.errorColumn);
+%End
+
+%End
+%If (Qt_6_5_0 -)
+    SIP_PYOBJECT setContent(QIODevice *device, QDomDocument::ParseOptions options = QDomDocument::ParseOption::Default) /ReleaseGIL,TypeHint="Tuple [bool, str, int, int]"/;
+%MethodCode
+        QDomDocument::ParseResult pr;
+        
+        Py_BEGIN_ALLOW_THREADS
+        pr = sipCpp->setContent(a0, *a1);
+        Py_END_ALLOW_THREADS
+        
+        return sipBuildResult(NULL, "(bNnn)",
+                (int)bool(pr),
+                new QString(pr.errorMessage), sipType_QString, NULL,
+                (long long)pr.errorLine,
+                (long long)pr.errorColumn);
+%End
+
+%End
+%If (Qt_6_5_0 -)
+    SIP_PYOBJECT setContent(QAnyStringView data, QDomDocument::ParseOptions options = QDomDocument::ParseOption::Default) /TypeHint="Tuple [bool, str, int, int]"/;
+%MethodCode
+        QDomDocument::ParseResult pr;
+        
+        pr = sipCpp->setContent(*a0, *a1);
+        
+        return sipBuildResult(NULL, "(bNnn)",
+                (int)bool(pr),
+                new QString(pr.errorMessage), sipType_QString, NULL,
+                (long long)pr.errorLine,
+                (long long)pr.errorColumn);
+%End
+
+%End
     bool setContent(const QByteArray &text, bool namespaceProcessing, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0);
     bool setContent(const QString &text, bool namespaceProcessing, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0);
     bool setContent(QIODevice *dev, bool namespaceProcessing, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0) /ReleaseGIL/;
+%If (- Qt_6_5_0)
     bool setContent(const QByteArray &text, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0);
+%End
+%If (- Qt_6_5_0)
     bool setContent(const QString &text, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0);
+%End
+%If (- Qt_6_5_0)
     bool setContent(QIODevice *dev, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0) /ReleaseGIL/;
+%End
     bool setContent(QXmlStreamReader *reader, bool namespaceProcessing, QString *errorMsg /Out/ = 0, int *errorLine = 0, int *errorColumn = 0);
     QString toString(int indent = 1) const;
     QByteArray toByteArray(int indent = 1) const;
 };
 
 class QDomNamedNodeMap
 {
```

### Comparing `PyQt6-6.4.2/uic/Compiler/__init__.py` & `PyQt6-6.5.0/uic/Compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/as_string.py` & `PyQt6-6.5.0/uic/Compiler/as_string.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/compiler.py` & `PyQt6-6.5.0/uic/Compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/indenter.py` & `PyQt6-6.5.0/uic/Compiler/indenter.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/misc.py` & `PyQt6-6.5.0/uic/Compiler/misc.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/proxy_metaclass.py` & `PyQt6-6.5.0/uic/Compiler/proxy_metaclass.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/qobjectcreator.py` & `PyQt6-6.5.0/uic/Compiler/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Compiler/qtproxies.py` & `PyQt6-6.5.0/uic/Compiler/qtproxies.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Loader/__init__.py` & `PyQt6-6.5.0/uic/Loader/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Loader/loader.py` & `PyQt6-6.5.0/uic/Loader/loader.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/Loader/qobjectcreator.py` & `PyQt6-6.5.0/uic/Loader/qobjectcreator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/__init__.py` & `PyQt6-6.5.0/sip/QtSpatialAudio/QtSpatialAudiomod.sip`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,53 @@
-# Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
-# 
-# This file is part of PyQt6.
-# 
-# This file may be used under the terms of the GNU General Public License
-# version 3.0 as published by the Free Software Foundation and appearing in
-# the file LICENSE included in the packaging of this file.  Please review the
-# following information to ensure the GNU General Public License version 3.0
-# requirements will be met: http://www.gnu.org/copyleft/gpl.html.
-# 
-# If you do not wish to use this file under the terms of the GPL version 3.0
-# then you may purchase a commercial license.  For more information contact
-# info@riverbankcomputing.com.
-# 
-# This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
-# WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
-
-
-# The public API.
-from .compile_ui import compileUi, compileUiDir
-from .load_ui import loadUi, loadUiType
-from .objcreator import widgetPluginPath
-from .ui_file import UIFile
+// QtSpatialAudiomod.sip generated by MetaSIP
+//
+// This file is part of the QtSpatialAudio Python extension module.
+//
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// 
+// This file is part of PyQt6.
+// 
+// This file may be used under the terms of the GNU General Public License
+// version 3.0 as published by the Free Software Foundation and appearing in
+// the file LICENSE included in the packaging of this file.  Please review the
+// following information to ensure the GNU General Public License version 3.0
+// requirements will be met: http://www.gnu.org/copyleft/gpl.html.
+// 
+// If you do not wish to use this file under the terms of the GPL version 3.0
+// then you may purchase a commercial license.  For more information contact
+// info@riverbankcomputing.com.
+// 
+// This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
+// WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
+
+
+%Module(name=PyQt6.QtSpatialAudio, keyword_arguments="Optional", use_limited_api=True)
+
+%Import QtCore/QtCoremod.sip
+%Import QtMultimedia/QtMultimediamod.sip
+
+%Copying
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+
+This file is part of PyQt6.
+
+This file may be used under the terms of the GNU General Public License
+version 3.0 as published by the Free Software Foundation and appearing in
+the file LICENSE included in the packaging of this file.  Please review the
+following information to ensure the GNU General Public License version 3.0
+requirements will be met: http://www.gnu.org/copyleft/gpl.html.
+
+If you do not wish to use this file under the terms of the GPL version 3.0
+then you may purchase a commercial license.  For more information contact
+info@riverbankcomputing.com.
+
+This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
+WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
+%End
+
+%DefaultSupertype PyQt6.sip.simplewrapper
+
+%Include qambientsound.sip
+%Include qaudioengine.sip
+%Include qaudiolistener.sip
+%Include qaudioroom.sip
+%Include qspatialsound.sip
```

### Comparing `PyQt6-6.4.2/uic/compile_ui.py` & `PyQt6-6.5.0/uic/compile_ui.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/enum_map.py` & `PyQt6-6.5.0/uic/enum_map.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/exceptions.py` & `PyQt6-6.5.0/uic/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/icon_cache.py` & `PyQt6-6.5.0/uic/icon_cache.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/load_ui.py` & `PyQt6-6.5.0/uic/load_ui.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/objcreator.py` & `PyQt6-6.5.0/uic/objcreator.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/properties.py` & `PyQt6-6.5.0/uic/properties.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/pyuic.py` & `PyQt6-6.5.0/uic/pyuic.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/ui_file.py` & `PyQt6-6.5.0/uic/ui_file.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/uiparser.py` & `PyQt6-6.5.0/uic/uiparser.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/widget-plugins/qaxcontainer.py` & `PyQt6-6.5.0/uic/widget-plugins/qaxcontainer.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/widget-plugins/qscintilla.py` & `PyQt6-6.5.0/uic/widget-plugins/qscintilla.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/widget-plugins/qtcharts.py` & `PyQt6-6.5.0/uic/widget-plugins/qtcharts.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/widget-plugins/qtprintsupport.py` & `PyQt6-6.5.0/uic/widget-plugins/qtprintsupport.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/widget-plugins/qtquickwidgets.py` & `PyQt6-6.5.0/uic/widget-plugins/qtquickwidgets.py`

 * *Files identical despite different names*

### Comparing `PyQt6-6.4.2/uic/widget-plugins/qtwebenginewidgets.py` & `PyQt6-6.5.0/uic/widget-plugins/qtwebenginewidgets.py`

 * *Files identical despite different names*

